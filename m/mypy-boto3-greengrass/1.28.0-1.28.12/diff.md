# Comparing `tmp/mypy-boto3-greengrass-1.28.0.tar.gz` & `tmp/mypy-boto3-greengrass-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-greengrass-1.28.0.tar", last modified: Thu Jul  6 20:59:40 2023, max compression
+gzip compressed data, was "mypy-boto3-greengrass-1.28.12.tar", last modified: Thu Jul 27 05:34:44 2023, max compression
```

## Comparing `mypy-boto3-greengrass-1.28.0.tar` & `mypy-boto3-greengrass-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:40.498314 mypy-boto3-greengrass-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:42:14.000000 mypy-boto3-greengrass-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27719 2023-07-06 20:59:40.498314 mypy-boto3-greengrass-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26222 2023-07-06 20:42:14.000000 mypy-boto3-greengrass-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:40.494314 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-06 20:42:14.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-06 20:42:14.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:42:14.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68713 2023-07-06 20:42:15.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    68595 2023-07-06 20:42:15.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-06 20:42:16.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-07-06 20:42:15.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-07-06 20:42:15.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-07-06 20:42:15.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:14.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    89019 2023-07-06 20:42:20.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    88902 2023-07-06 20:42:17.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:42:14.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:40.498314 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27719 2023-07-06 20:59:40.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 20:59:40.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:40.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:40.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:40.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:59:40.000000 mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:40.498314 mypy-boto3-greengrass-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:42:14.000000 mypy-boto3-greengrass-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.672500 mypy-boto3-greengrass-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28933 2023-07-27 05:34:44.668500 mypy-boto3-greengrass-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27434 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.656499 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68713 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68595 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    99009 2023-07-27 05:23:07.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98880 2023-07-27 05:23:06.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.668500 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28933 2023-07-27 05:34:44.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:44.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:44.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:44.000000 mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:44.672500 mypy-boto3-greengrass-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:23:04.000000 mypy-boto3-greengrass-1.28.12/setup.py
```

### Comparing `mypy-boto3-greengrass-1.28.0/LICENSE` & `mypy-boto3-greengrass-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.0/PKG-INFO` & `mypy-boto3-greengrass-1.28.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrass
-Version: 1.28.0
-Summary: Type annotations for boto3.Greengrass 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Greengrass 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-greengrass"></a>
 
 # mypy-boto3-greengrass
 
 [![PyPI - mypy-boto3-greengrass](https://img.shields.io/pypi/v/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-greengrass?color=blue)](https://pypistats.org/packages/mypy-boto3-greengrass)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrass)](https://pepy.tech/project/mypy-boto3-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Greengrass 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[boto3.Greengrass 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
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
 [mypy-boto3-greengrass docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/).
 
 See how it helps to find and fix potential bugs:
 
@@ -429,16 +429,19 @@
     AssociateRoleToGroupRequestRequestTypeDef,
     AssociateRoleToGroupResponseTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
     AssociateServiceRoleToAccountResponseTypeDef,
     BulkDeploymentMetricsTypeDef,
     ErrorDetailTypeDef,
     BulkDeploymentTypeDef,
+    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
+    ConnectorOutputTypeDef,
     ConnectorTypeDef,
+    CoreOutputTypeDef,
     CoreTypeDef,
     CreateConnectorDefinitionResponseTypeDef,
     CreateConnectorDefinitionVersionResponseTypeDef,
     CreateCoreDefinitionResponseTypeDef,
     CreateCoreDefinitionVersionResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     CreateDeploymentResponseTypeDef,
@@ -469,19 +472,22 @@
     DeleteDeviceDefinitionRequestRequestTypeDef,
     DeleteFunctionDefinitionRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteLoggerDefinitionRequestRequestTypeDef,
     DeleteResourceDefinitionRequestRequestTypeDef,
     DeleteSubscriptionDefinitionRequestRequestTypeDef,
     DeploymentTypeDef,
+    DeviceOutputTypeDef,
     DisassociateRoleFromGroupRequestRequestTypeDef,
     DisassociateRoleFromGroupResponseTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    ResourceAccessPolicyOutputTypeDef,
     ResourceAccessPolicyTypeDef,
+    FunctionRunAsConfigOutputTypeDef,
     FunctionRunAsConfigTypeDef,
     GetAssociatedRoleRequestRequestTypeDef,
     GetAssociatedRoleResponseTypeDef,
     GetBulkDeploymentStatusRequestRequestTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetConnectorDefinitionRequestRequestTypeDef,
     GetConnectorDefinitionResponseTypeDef,
@@ -499,27 +505,29 @@
     GetGroupCertificateAuthorityRequestRequestTypeDef,
     GetGroupCertificateAuthorityResponseTypeDef,
     GetGroupCertificateConfigurationRequestRequestTypeDef,
     GetGroupCertificateConfigurationResponseTypeDef,
     GetGroupRequestRequestTypeDef,
     GetGroupResponseTypeDef,
     GetGroupVersionRequestRequestTypeDef,
+    GroupVersionOutputTypeDef,
     GetLoggerDefinitionRequestRequestTypeDef,
     GetLoggerDefinitionResponseTypeDef,
     GetLoggerDefinitionVersionRequestRequestTypeDef,
     GetResourceDefinitionRequestRequestTypeDef,
     GetResourceDefinitionResponseTypeDef,
     GetResourceDefinitionVersionRequestRequestTypeDef,
     GetServiceRoleForAccountResponseTypeDef,
     GetSubscriptionDefinitionRequestRequestTypeDef,
     GetSubscriptionDefinitionResponseTypeDef,
     GetSubscriptionDefinitionVersionRequestRequestTypeDef,
     GetThingRuntimeConfigurationRequestRequestTypeDef,
     GroupCertificateAuthorityPropertiesTypeDef,
     GroupInformationTypeDef,
+    GroupOwnerSettingOutputTypeDef,
     GroupOwnerSettingTypeDef,
     ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
     ListBulkDeploymentDetailedReportsRequestRequestTypeDef,
     ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef,
     ListBulkDeploymentsRequestRequestTypeDef,
     ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
     ListConnectorDefinitionVersionsRequestRequestTypeDef,
@@ -555,24 +563,28 @@
     ListResourceDefinitionsRequestRequestTypeDef,
     ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
     ListSubscriptionDefinitionVersionsRequestRequestTypeDef,
     ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef,
     ListSubscriptionDefinitionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    LoggerOutputTypeDef,
     PaginatorConfigTypeDef,
     ResetDeploymentsRequestRequestTypeDef,
     ResetDeploymentsResponseTypeDef,
+    SecretsManagerSecretResourceDataOutputTypeDef,
     SecretsManagerSecretResourceDataTypeDef,
+    ResourceDownloadOwnerSettingOutputTypeDef,
     ResourceDownloadOwnerSettingTypeDef,
     ResponseMetadataTypeDef,
     TelemetryConfigurationTypeDef,
     StartBulkDeploymentRequestRequestTypeDef,
     StartBulkDeploymentResponseTypeDef,
     StopBulkDeploymentRequestRequestTypeDef,
+    SubscriptionOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     TelemetryConfigurationUpdateTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectivityInfoResponseTypeDef,
     UpdateConnectorDefinitionRequestRequestTypeDef,
     UpdateCoreDefinitionRequestRequestTypeDef,
     UpdateDeviceDefinitionRequestRequestTypeDef,
@@ -585,78 +597,97 @@
     UpdateSubscriptionDefinitionRequestRequestTypeDef,
     BulkDeploymentResultTypeDef,
     GetBulkDeploymentStatusResponseTypeDef,
     GetDeploymentStatusResponseTypeDef,
     ListBulkDeploymentsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
+    ConnectorDefinitionVersionOutputTypeDef,
     ConnectorDefinitionVersionTypeDef,
     CreateConnectorDefinitionVersionRequestRequestTypeDef,
+    CoreDefinitionVersionOutputTypeDef,
     CoreDefinitionVersionTypeDef,
     CreateCoreDefinitionVersionRequestRequestTypeDef,
     CreateDeviceDefinitionVersionRequestRequestTypeDef,
     DeviceDefinitionVersionTypeDef,
     CreateGroupRequestRequestTypeDef,
-    GetGroupVersionResponseTypeDef,
     CreateLoggerDefinitionVersionRequestRequestTypeDef,
     LoggerDefinitionVersionTypeDef,
     CreateSubscriptionDefinitionVersionRequestRequestTypeDef,
     SubscriptionDefinitionVersionTypeDef,
     ListConnectorDefinitionsResponseTypeDef,
     ListCoreDefinitionsResponseTypeDef,
     ListDeviceDefinitionsResponseTypeDef,
     ListFunctionDefinitionsResponseTypeDef,
     ListLoggerDefinitionsResponseTypeDef,
     ListResourceDefinitionsResponseTypeDef,
     ListSubscriptionDefinitionsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
+    DeviceDefinitionVersionOutputTypeDef,
+    FunctionDefaultExecutionConfigOutputTypeDef,
+    FunctionExecutionConfigOutputTypeDef,
     FunctionDefaultExecutionConfigTypeDef,
     FunctionExecutionConfigTypeDef,
+    GetGroupVersionResponseTypeDef,
     ListGroupCertificateAuthoritiesResponseTypeDef,
     ListGroupsResponseTypeDef,
+    LocalDeviceResourceDataOutputTypeDef,
+    LocalVolumeResourceDataOutputTypeDef,
     LocalDeviceResourceDataTypeDef,
     LocalVolumeResourceDataTypeDef,
     ListConnectorDefinitionVersionsResponseTypeDef,
     ListCoreDefinitionVersionsResponseTypeDef,
     ListDeviceDefinitionVersionsResponseTypeDef,
     ListFunctionDefinitionVersionsResponseTypeDef,
     ListGroupVersionsResponseTypeDef,
     ListLoggerDefinitionVersionsResponseTypeDef,
     ListResourceDefinitionVersionsResponseTypeDef,
     ListSubscriptionDefinitionVersionsResponseTypeDef,
+    LoggerDefinitionVersionOutputTypeDef,
+    S3MachineLearningModelResourceDataOutputTypeDef,
+    SageMakerMachineLearningModelResourceDataOutputTypeDef,
     S3MachineLearningModelResourceDataTypeDef,
     SageMakerMachineLearningModelResourceDataTypeDef,
     RuntimeConfigurationTypeDef,
+    SubscriptionDefinitionVersionOutputTypeDef,
     UpdateThingRuntimeConfigurationRequestRequestTypeDef,
     ListBulkDeploymentDetailedReportsResponseTypeDef,
-    CreateConnectorDefinitionRequestRequestTypeDef,
     GetConnectorDefinitionVersionResponseTypeDef,
-    CreateCoreDefinitionRequestRequestTypeDef,
+    CreateConnectorDefinitionRequestRequestTypeDef,
     GetCoreDefinitionVersionResponseTypeDef,
+    CreateCoreDefinitionRequestRequestTypeDef,
     CreateDeviceDefinitionRequestRequestTypeDef,
-    GetDeviceDefinitionVersionResponseTypeDef,
     CreateLoggerDefinitionRequestRequestTypeDef,
-    GetLoggerDefinitionVersionResponseTypeDef,
     CreateSubscriptionDefinitionRequestRequestTypeDef,
-    GetSubscriptionDefinitionVersionResponseTypeDef,
+    GetDeviceDefinitionVersionResponseTypeDef,
+    FunctionDefaultConfigOutputTypeDef,
+    FunctionConfigurationEnvironmentOutputTypeDef,
     FunctionDefaultConfigTypeDef,
     FunctionConfigurationEnvironmentTypeDef,
+    GetLoggerDefinitionVersionResponseTypeDef,
+    ResourceDataContainerOutputTypeDef,
     ResourceDataContainerTypeDef,
     GetThingRuntimeConfigurationResponseTypeDef,
+    GetSubscriptionDefinitionVersionResponseTypeDef,
+    FunctionConfigurationOutputTypeDef,
     FunctionConfigurationTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
+    FunctionOutputTypeDef,
     FunctionTypeDef,
+    ResourceDefinitionVersionOutputTypeDef,
     CreateResourceDefinitionVersionRequestRequestTypeDef,
     ResourceDefinitionVersionTypeDef,
+    FunctionDefinitionVersionOutputTypeDef,
     CreateFunctionDefinitionVersionRequestRequestTypeDef,
     FunctionDefinitionVersionTypeDef,
-    CreateResourceDefinitionRequestRequestTypeDef,
     GetResourceDefinitionVersionResponseTypeDef,
-    CreateFunctionDefinitionRequestRequestTypeDef,
+    CreateResourceDefinitionRequestRequestTypeDef,
     GetFunctionDefinitionVersionResponseTypeDef,
+    CreateFunctionDefinitionRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AssociateRoleToGroupRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-greengrass-1.28.0/README.md` & `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-greengrass
+Version: 1.28.12
+Summary: Type annotations for boto3.Greengrass 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 greengrass type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-greengrass"></a>
 
 # mypy-boto3-greengrass
 
 [![PyPI - mypy-boto3-greengrass](https://img.shields.io/pypi/v/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-greengrass?color=blue)](https://pypistats.org/packages/mypy-boto3-greengrass)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrass)](https://pepy.tech/project/mypy-boto3-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Greengrass 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[boto3.Greengrass 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
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
 [mypy-boto3-greengrass docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/).
 
 See how it helps to find and fix potential bugs:
 
@@ -397,16 +429,19 @@
     AssociateRoleToGroupRequestRequestTypeDef,
     AssociateRoleToGroupResponseTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
     AssociateServiceRoleToAccountResponseTypeDef,
     BulkDeploymentMetricsTypeDef,
     ErrorDetailTypeDef,
     BulkDeploymentTypeDef,
+    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
+    ConnectorOutputTypeDef,
     ConnectorTypeDef,
+    CoreOutputTypeDef,
     CoreTypeDef,
     CreateConnectorDefinitionResponseTypeDef,
     CreateConnectorDefinitionVersionResponseTypeDef,
     CreateCoreDefinitionResponseTypeDef,
     CreateCoreDefinitionVersionResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     CreateDeploymentResponseTypeDef,
@@ -437,19 +472,22 @@
     DeleteDeviceDefinitionRequestRequestTypeDef,
     DeleteFunctionDefinitionRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteLoggerDefinitionRequestRequestTypeDef,
     DeleteResourceDefinitionRequestRequestTypeDef,
     DeleteSubscriptionDefinitionRequestRequestTypeDef,
     DeploymentTypeDef,
+    DeviceOutputTypeDef,
     DisassociateRoleFromGroupRequestRequestTypeDef,
     DisassociateRoleFromGroupResponseTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    ResourceAccessPolicyOutputTypeDef,
     ResourceAccessPolicyTypeDef,
+    FunctionRunAsConfigOutputTypeDef,
     FunctionRunAsConfigTypeDef,
     GetAssociatedRoleRequestRequestTypeDef,
     GetAssociatedRoleResponseTypeDef,
     GetBulkDeploymentStatusRequestRequestTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetConnectorDefinitionRequestRequestTypeDef,
     GetConnectorDefinitionResponseTypeDef,
@@ -467,27 +505,29 @@
     GetGroupCertificateAuthorityRequestRequestTypeDef,
     GetGroupCertificateAuthorityResponseTypeDef,
     GetGroupCertificateConfigurationRequestRequestTypeDef,
     GetGroupCertificateConfigurationResponseTypeDef,
     GetGroupRequestRequestTypeDef,
     GetGroupResponseTypeDef,
     GetGroupVersionRequestRequestTypeDef,
+    GroupVersionOutputTypeDef,
     GetLoggerDefinitionRequestRequestTypeDef,
     GetLoggerDefinitionResponseTypeDef,
     GetLoggerDefinitionVersionRequestRequestTypeDef,
     GetResourceDefinitionRequestRequestTypeDef,
     GetResourceDefinitionResponseTypeDef,
     GetResourceDefinitionVersionRequestRequestTypeDef,
     GetServiceRoleForAccountResponseTypeDef,
     GetSubscriptionDefinitionRequestRequestTypeDef,
     GetSubscriptionDefinitionResponseTypeDef,
     GetSubscriptionDefinitionVersionRequestRequestTypeDef,
     GetThingRuntimeConfigurationRequestRequestTypeDef,
     GroupCertificateAuthorityPropertiesTypeDef,
     GroupInformationTypeDef,
+    GroupOwnerSettingOutputTypeDef,
     GroupOwnerSettingTypeDef,
     ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
     ListBulkDeploymentDetailedReportsRequestRequestTypeDef,
     ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef,
     ListBulkDeploymentsRequestRequestTypeDef,
     ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
     ListConnectorDefinitionVersionsRequestRequestTypeDef,
@@ -523,24 +563,28 @@
     ListResourceDefinitionsRequestRequestTypeDef,
     ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
     ListSubscriptionDefinitionVersionsRequestRequestTypeDef,
     ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef,
     ListSubscriptionDefinitionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    LoggerOutputTypeDef,
     PaginatorConfigTypeDef,
     ResetDeploymentsRequestRequestTypeDef,
     ResetDeploymentsResponseTypeDef,
+    SecretsManagerSecretResourceDataOutputTypeDef,
     SecretsManagerSecretResourceDataTypeDef,
+    ResourceDownloadOwnerSettingOutputTypeDef,
     ResourceDownloadOwnerSettingTypeDef,
     ResponseMetadataTypeDef,
     TelemetryConfigurationTypeDef,
     StartBulkDeploymentRequestRequestTypeDef,
     StartBulkDeploymentResponseTypeDef,
     StopBulkDeploymentRequestRequestTypeDef,
+    SubscriptionOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     TelemetryConfigurationUpdateTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectivityInfoResponseTypeDef,
     UpdateConnectorDefinitionRequestRequestTypeDef,
     UpdateCoreDefinitionRequestRequestTypeDef,
     UpdateDeviceDefinitionRequestRequestTypeDef,
@@ -553,78 +597,97 @@
     UpdateSubscriptionDefinitionRequestRequestTypeDef,
     BulkDeploymentResultTypeDef,
     GetBulkDeploymentStatusResponseTypeDef,
     GetDeploymentStatusResponseTypeDef,
     ListBulkDeploymentsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
+    ConnectorDefinitionVersionOutputTypeDef,
     ConnectorDefinitionVersionTypeDef,
     CreateConnectorDefinitionVersionRequestRequestTypeDef,
+    CoreDefinitionVersionOutputTypeDef,
     CoreDefinitionVersionTypeDef,
     CreateCoreDefinitionVersionRequestRequestTypeDef,
     CreateDeviceDefinitionVersionRequestRequestTypeDef,
     DeviceDefinitionVersionTypeDef,
     CreateGroupRequestRequestTypeDef,
-    GetGroupVersionResponseTypeDef,
     CreateLoggerDefinitionVersionRequestRequestTypeDef,
     LoggerDefinitionVersionTypeDef,
     CreateSubscriptionDefinitionVersionRequestRequestTypeDef,
     SubscriptionDefinitionVersionTypeDef,
     ListConnectorDefinitionsResponseTypeDef,
     ListCoreDefinitionsResponseTypeDef,
     ListDeviceDefinitionsResponseTypeDef,
     ListFunctionDefinitionsResponseTypeDef,
     ListLoggerDefinitionsResponseTypeDef,
     ListResourceDefinitionsResponseTypeDef,
     ListSubscriptionDefinitionsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
+    DeviceDefinitionVersionOutputTypeDef,
+    FunctionDefaultExecutionConfigOutputTypeDef,
+    FunctionExecutionConfigOutputTypeDef,
     FunctionDefaultExecutionConfigTypeDef,
     FunctionExecutionConfigTypeDef,
+    GetGroupVersionResponseTypeDef,
     ListGroupCertificateAuthoritiesResponseTypeDef,
     ListGroupsResponseTypeDef,
+    LocalDeviceResourceDataOutputTypeDef,
+    LocalVolumeResourceDataOutputTypeDef,
     LocalDeviceResourceDataTypeDef,
     LocalVolumeResourceDataTypeDef,
     ListConnectorDefinitionVersionsResponseTypeDef,
     ListCoreDefinitionVersionsResponseTypeDef,
     ListDeviceDefinitionVersionsResponseTypeDef,
     ListFunctionDefinitionVersionsResponseTypeDef,
     ListGroupVersionsResponseTypeDef,
     ListLoggerDefinitionVersionsResponseTypeDef,
     ListResourceDefinitionVersionsResponseTypeDef,
     ListSubscriptionDefinitionVersionsResponseTypeDef,
+    LoggerDefinitionVersionOutputTypeDef,
+    S3MachineLearningModelResourceDataOutputTypeDef,
+    SageMakerMachineLearningModelResourceDataOutputTypeDef,
     S3MachineLearningModelResourceDataTypeDef,
     SageMakerMachineLearningModelResourceDataTypeDef,
     RuntimeConfigurationTypeDef,
+    SubscriptionDefinitionVersionOutputTypeDef,
     UpdateThingRuntimeConfigurationRequestRequestTypeDef,
     ListBulkDeploymentDetailedReportsResponseTypeDef,
-    CreateConnectorDefinitionRequestRequestTypeDef,
     GetConnectorDefinitionVersionResponseTypeDef,
-    CreateCoreDefinitionRequestRequestTypeDef,
+    CreateConnectorDefinitionRequestRequestTypeDef,
     GetCoreDefinitionVersionResponseTypeDef,
+    CreateCoreDefinitionRequestRequestTypeDef,
     CreateDeviceDefinitionRequestRequestTypeDef,
-    GetDeviceDefinitionVersionResponseTypeDef,
     CreateLoggerDefinitionRequestRequestTypeDef,
-    GetLoggerDefinitionVersionResponseTypeDef,
     CreateSubscriptionDefinitionRequestRequestTypeDef,
-    GetSubscriptionDefinitionVersionResponseTypeDef,
+    GetDeviceDefinitionVersionResponseTypeDef,
+    FunctionDefaultConfigOutputTypeDef,
+    FunctionConfigurationEnvironmentOutputTypeDef,
     FunctionDefaultConfigTypeDef,
     FunctionConfigurationEnvironmentTypeDef,
+    GetLoggerDefinitionVersionResponseTypeDef,
+    ResourceDataContainerOutputTypeDef,
     ResourceDataContainerTypeDef,
     GetThingRuntimeConfigurationResponseTypeDef,
+    GetSubscriptionDefinitionVersionResponseTypeDef,
+    FunctionConfigurationOutputTypeDef,
     FunctionConfigurationTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
+    FunctionOutputTypeDef,
     FunctionTypeDef,
+    ResourceDefinitionVersionOutputTypeDef,
     CreateResourceDefinitionVersionRequestRequestTypeDef,
     ResourceDefinitionVersionTypeDef,
+    FunctionDefinitionVersionOutputTypeDef,
     CreateFunctionDefinitionVersionRequestRequestTypeDef,
     FunctionDefinitionVersionTypeDef,
-    CreateResourceDefinitionRequestRequestTypeDef,
     GetResourceDefinitionVersionResponseTypeDef,
-    CreateFunctionDefinitionRequestRequestTypeDef,
+    CreateResourceDefinitionRequestRequestTypeDef,
     GetFunctionDefinitionVersionResponseTypeDef,
+    CreateFunctionDefinitionRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AssociateRoleToGroupRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/__init__.py` & `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/__init__.pyi` & `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/__main__.py` & `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Greengrass 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Greengrass 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass\nOther"
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

### Comparing `mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/client.py` & `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/client.pyi` & `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/literals.py` & `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,15 @@
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
@@ -302,26 +303,28 @@
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

### Comparing `mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/literals.pyi` & `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,15 @@
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
@@ -300,26 +301,28 @@
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

### Comparing `mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/paginator.py` & `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/paginator.pyi` & `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/type_defs.py` & `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,16 +41,19 @@
     "AssociateRoleToGroupRequestRequestTypeDef",
     "AssociateRoleToGroupResponseTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     "AssociateServiceRoleToAccountResponseTypeDef",
     "BulkDeploymentMetricsTypeDef",
     "ErrorDetailTypeDef",
     "BulkDeploymentTypeDef",
+    "ConnectivityInfoOutputTypeDef",
     "ConnectivityInfoTypeDef",
+    "ConnectorOutputTypeDef",
     "ConnectorTypeDef",
+    "CoreOutputTypeDef",
     "CoreTypeDef",
     "CreateConnectorDefinitionResponseTypeDef",
     "CreateConnectorDefinitionVersionResponseTypeDef",
     "CreateCoreDefinitionResponseTypeDef",
     "CreateCoreDefinitionVersionResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "CreateDeploymentResponseTypeDef",
@@ -81,19 +84,22 @@
     "DeleteDeviceDefinitionRequestRequestTypeDef",
     "DeleteFunctionDefinitionRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteLoggerDefinitionRequestRequestTypeDef",
     "DeleteResourceDefinitionRequestRequestTypeDef",
     "DeleteSubscriptionDefinitionRequestRequestTypeDef",
     "DeploymentTypeDef",
+    "DeviceOutputTypeDef",
     "DisassociateRoleFromGroupRequestRequestTypeDef",
     "DisassociateRoleFromGroupResponseTypeDef",
     "DisassociateServiceRoleFromAccountResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "ResourceAccessPolicyOutputTypeDef",
     "ResourceAccessPolicyTypeDef",
+    "FunctionRunAsConfigOutputTypeDef",
     "FunctionRunAsConfigTypeDef",
     "GetAssociatedRoleRequestRequestTypeDef",
     "GetAssociatedRoleResponseTypeDef",
     "GetBulkDeploymentStatusRequestRequestTypeDef",
     "GetConnectivityInfoRequestRequestTypeDef",
     "GetConnectorDefinitionRequestRequestTypeDef",
     "GetConnectorDefinitionResponseTypeDef",
@@ -111,27 +117,29 @@
     "GetGroupCertificateAuthorityRequestRequestTypeDef",
     "GetGroupCertificateAuthorityResponseTypeDef",
     "GetGroupCertificateConfigurationRequestRequestTypeDef",
     "GetGroupCertificateConfigurationResponseTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetGroupResponseTypeDef",
     "GetGroupVersionRequestRequestTypeDef",
+    "GroupVersionOutputTypeDef",
     "GetLoggerDefinitionRequestRequestTypeDef",
     "GetLoggerDefinitionResponseTypeDef",
     "GetLoggerDefinitionVersionRequestRequestTypeDef",
     "GetResourceDefinitionRequestRequestTypeDef",
     "GetResourceDefinitionResponseTypeDef",
     "GetResourceDefinitionVersionRequestRequestTypeDef",
     "GetServiceRoleForAccountResponseTypeDef",
     "GetSubscriptionDefinitionRequestRequestTypeDef",
     "GetSubscriptionDefinitionResponseTypeDef",
     "GetSubscriptionDefinitionVersionRequestRequestTypeDef",
     "GetThingRuntimeConfigurationRequestRequestTypeDef",
     "GroupCertificateAuthorityPropertiesTypeDef",
     "GroupInformationTypeDef",
+    "GroupOwnerSettingOutputTypeDef",
     "GroupOwnerSettingTypeDef",
     "ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
     "ListBulkDeploymentDetailedReportsRequestRequestTypeDef",
     "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
     "ListBulkDeploymentsRequestRequestTypeDef",
     "ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
     "ListConnectorDefinitionVersionsRequestRequestTypeDef",
@@ -167,24 +175,28 @@
     "ListResourceDefinitionsRequestRequestTypeDef",
     "ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
     "ListSubscriptionDefinitionVersionsRequestRequestTypeDef",
     "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
     "ListSubscriptionDefinitionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "LoggerOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ResetDeploymentsRequestRequestTypeDef",
     "ResetDeploymentsResponseTypeDef",
+    "SecretsManagerSecretResourceDataOutputTypeDef",
     "SecretsManagerSecretResourceDataTypeDef",
+    "ResourceDownloadOwnerSettingOutputTypeDef",
     "ResourceDownloadOwnerSettingTypeDef",
     "ResponseMetadataTypeDef",
     "TelemetryConfigurationTypeDef",
     "StartBulkDeploymentRequestRequestTypeDef",
     "StartBulkDeploymentResponseTypeDef",
     "StopBulkDeploymentRequestRequestTypeDef",
+    "SubscriptionOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TelemetryConfigurationUpdateTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateConnectivityInfoResponseTypeDef",
     "UpdateConnectorDefinitionRequestRequestTypeDef",
     "UpdateCoreDefinitionRequestRequestTypeDef",
     "UpdateDeviceDefinitionRequestRequestTypeDef",
@@ -197,78 +209,97 @@
     "UpdateSubscriptionDefinitionRequestRequestTypeDef",
     "BulkDeploymentResultTypeDef",
     "GetBulkDeploymentStatusResponseTypeDef",
     "GetDeploymentStatusResponseTypeDef",
     "ListBulkDeploymentsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
+    "ConnectorDefinitionVersionOutputTypeDef",
     "ConnectorDefinitionVersionTypeDef",
     "CreateConnectorDefinitionVersionRequestRequestTypeDef",
+    "CoreDefinitionVersionOutputTypeDef",
     "CoreDefinitionVersionTypeDef",
     "CreateCoreDefinitionVersionRequestRequestTypeDef",
     "CreateDeviceDefinitionVersionRequestRequestTypeDef",
     "DeviceDefinitionVersionTypeDef",
     "CreateGroupRequestRequestTypeDef",
-    "GetGroupVersionResponseTypeDef",
     "CreateLoggerDefinitionVersionRequestRequestTypeDef",
     "LoggerDefinitionVersionTypeDef",
     "CreateSubscriptionDefinitionVersionRequestRequestTypeDef",
     "SubscriptionDefinitionVersionTypeDef",
     "ListConnectorDefinitionsResponseTypeDef",
     "ListCoreDefinitionsResponseTypeDef",
     "ListDeviceDefinitionsResponseTypeDef",
     "ListFunctionDefinitionsResponseTypeDef",
     "ListLoggerDefinitionsResponseTypeDef",
     "ListResourceDefinitionsResponseTypeDef",
     "ListSubscriptionDefinitionsResponseTypeDef",
     "ListDeploymentsResponseTypeDef",
+    "DeviceDefinitionVersionOutputTypeDef",
+    "FunctionDefaultExecutionConfigOutputTypeDef",
+    "FunctionExecutionConfigOutputTypeDef",
     "FunctionDefaultExecutionConfigTypeDef",
     "FunctionExecutionConfigTypeDef",
+    "GetGroupVersionResponseTypeDef",
     "ListGroupCertificateAuthoritiesResponseTypeDef",
     "ListGroupsResponseTypeDef",
+    "LocalDeviceResourceDataOutputTypeDef",
+    "LocalVolumeResourceDataOutputTypeDef",
     "LocalDeviceResourceDataTypeDef",
     "LocalVolumeResourceDataTypeDef",
     "ListConnectorDefinitionVersionsResponseTypeDef",
     "ListCoreDefinitionVersionsResponseTypeDef",
     "ListDeviceDefinitionVersionsResponseTypeDef",
     "ListFunctionDefinitionVersionsResponseTypeDef",
     "ListGroupVersionsResponseTypeDef",
     "ListLoggerDefinitionVersionsResponseTypeDef",
     "ListResourceDefinitionVersionsResponseTypeDef",
     "ListSubscriptionDefinitionVersionsResponseTypeDef",
+    "LoggerDefinitionVersionOutputTypeDef",
+    "S3MachineLearningModelResourceDataOutputTypeDef",
+    "SageMakerMachineLearningModelResourceDataOutputTypeDef",
     "S3MachineLearningModelResourceDataTypeDef",
     "SageMakerMachineLearningModelResourceDataTypeDef",
     "RuntimeConfigurationTypeDef",
+    "SubscriptionDefinitionVersionOutputTypeDef",
     "UpdateThingRuntimeConfigurationRequestRequestTypeDef",
     "ListBulkDeploymentDetailedReportsResponseTypeDef",
-    "CreateConnectorDefinitionRequestRequestTypeDef",
     "GetConnectorDefinitionVersionResponseTypeDef",
-    "CreateCoreDefinitionRequestRequestTypeDef",
+    "CreateConnectorDefinitionRequestRequestTypeDef",
     "GetCoreDefinitionVersionResponseTypeDef",
+    "CreateCoreDefinitionRequestRequestTypeDef",
     "CreateDeviceDefinitionRequestRequestTypeDef",
-    "GetDeviceDefinitionVersionResponseTypeDef",
     "CreateLoggerDefinitionRequestRequestTypeDef",
-    "GetLoggerDefinitionVersionResponseTypeDef",
     "CreateSubscriptionDefinitionRequestRequestTypeDef",
-    "GetSubscriptionDefinitionVersionResponseTypeDef",
+    "GetDeviceDefinitionVersionResponseTypeDef",
+    "FunctionDefaultConfigOutputTypeDef",
+    "FunctionConfigurationEnvironmentOutputTypeDef",
     "FunctionDefaultConfigTypeDef",
     "FunctionConfigurationEnvironmentTypeDef",
+    "GetLoggerDefinitionVersionResponseTypeDef",
+    "ResourceDataContainerOutputTypeDef",
     "ResourceDataContainerTypeDef",
     "GetThingRuntimeConfigurationResponseTypeDef",
+    "GetSubscriptionDefinitionVersionResponseTypeDef",
+    "FunctionConfigurationOutputTypeDef",
     "FunctionConfigurationTypeDef",
+    "ResourceOutputTypeDef",
     "ResourceTypeDef",
+    "FunctionOutputTypeDef",
     "FunctionTypeDef",
+    "ResourceDefinitionVersionOutputTypeDef",
     "CreateResourceDefinitionVersionRequestRequestTypeDef",
     "ResourceDefinitionVersionTypeDef",
+    "FunctionDefinitionVersionOutputTypeDef",
     "CreateFunctionDefinitionVersionRequestRequestTypeDef",
     "FunctionDefinitionVersionTypeDef",
-    "CreateResourceDefinitionRequestRequestTypeDef",
     "GetResourceDefinitionVersionResponseTypeDef",
-    "CreateFunctionDefinitionRequestRequestTypeDef",
+    "CreateResourceDefinitionRequestRequestTypeDef",
     "GetFunctionDefinitionVersionResponseTypeDef",
+    "CreateFunctionDefinitionRequestRequestTypeDef",
 )
 
 AssociateRoleToGroupRequestRequestTypeDef = TypedDict(
     "AssociateRoleToGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "RoleArn": str,
@@ -323,25 +354,56 @@
         "BulkDeploymentArn": str,
         "BulkDeploymentId": str,
         "CreatedAt": str,
     },
     total=False,
 )
 
+ConnectivityInfoOutputTypeDef = TypedDict(
+    "ConnectivityInfoOutputTypeDef",
+    {
+        "HostAddress": str,
+        "Id": str,
+        "Metadata": str,
+        "PortNumber": int,
+    },
+    total=False,
+)
+
 ConnectivityInfoTypeDef = TypedDict(
     "ConnectivityInfoTypeDef",
     {
         "HostAddress": str,
         "Id": str,
         "Metadata": str,
         "PortNumber": int,
     },
     total=False,
 )
 
+_RequiredConnectorOutputTypeDef = TypedDict(
+    "_RequiredConnectorOutputTypeDef",
+    {
+        "ConnectorArn": str,
+        "Id": str,
+    },
+)
+_OptionalConnectorOutputTypeDef = TypedDict(
+    "_OptionalConnectorOutputTypeDef",
+    {
+        "Parameters": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class ConnectorOutputTypeDef(_RequiredConnectorOutputTypeDef, _OptionalConnectorOutputTypeDef):
+    pass
+
+
 _RequiredConnectorTypeDef = TypedDict(
     "_RequiredConnectorTypeDef",
     {
         "ConnectorArn": str,
         "Id": str,
     },
 )
@@ -354,14 +416,35 @@
 )
 
 
 class ConnectorTypeDef(_RequiredConnectorTypeDef, _OptionalConnectorTypeDef):
     pass
 
 
+_RequiredCoreOutputTypeDef = TypedDict(
+    "_RequiredCoreOutputTypeDef",
+    {
+        "CertificateArn": str,
+        "Id": str,
+        "ThingArn": str,
+    },
+)
+_OptionalCoreOutputTypeDef = TypedDict(
+    "_OptionalCoreOutputTypeDef",
+    {
+        "SyncShadow": bool,
+    },
+    total=False,
+)
+
+
+class CoreOutputTypeDef(_RequiredCoreOutputTypeDef, _OptionalCoreOutputTypeDef):
+    pass
+
+
 _RequiredCoreTypeDef = TypedDict(
     "_RequiredCoreTypeDef",
     {
         "CertificateArn": str,
         "Id": str,
         "ThingArn": str,
     },
@@ -854,14 +937,35 @@
         "DeploymentId": str,
         "DeploymentType": DeploymentTypeType,
         "GroupArn": str,
     },
     total=False,
 )
 
+_RequiredDeviceOutputTypeDef = TypedDict(
+    "_RequiredDeviceOutputTypeDef",
+    {
+        "CertificateArn": str,
+        "Id": str,
+        "ThingArn": str,
+    },
+)
+_OptionalDeviceOutputTypeDef = TypedDict(
+    "_OptionalDeviceOutputTypeDef",
+    {
+        "SyncShadow": bool,
+    },
+    total=False,
+)
+
+
+class DeviceOutputTypeDef(_RequiredDeviceOutputTypeDef, _OptionalDeviceOutputTypeDef):
+    pass
+
+
 DisassociateRoleFromGroupRequestRequestTypeDef = TypedDict(
     "DisassociateRoleFromGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
@@ -884,14 +988,35 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredResourceAccessPolicyOutputTypeDef = TypedDict(
+    "_RequiredResourceAccessPolicyOutputTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalResourceAccessPolicyOutputTypeDef = TypedDict(
+    "_OptionalResourceAccessPolicyOutputTypeDef",
+    {
+        "Permission": PermissionType,
+    },
+    total=False,
+)
+
+
+class ResourceAccessPolicyOutputTypeDef(
+    _RequiredResourceAccessPolicyOutputTypeDef, _OptionalResourceAccessPolicyOutputTypeDef
+):
+    pass
+
+
 _RequiredResourceAccessPolicyTypeDef = TypedDict(
     "_RequiredResourceAccessPolicyTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalResourceAccessPolicyTypeDef = TypedDict(
@@ -905,14 +1030,23 @@
 
 class ResourceAccessPolicyTypeDef(
     _RequiredResourceAccessPolicyTypeDef, _OptionalResourceAccessPolicyTypeDef
 ):
     pass
 
 
+FunctionRunAsConfigOutputTypeDef = TypedDict(
+    "FunctionRunAsConfigOutputTypeDef",
+    {
+        "Gid": int,
+        "Uid": int,
+    },
+    total=False,
+)
+
 FunctionRunAsConfigTypeDef = TypedDict(
     "FunctionRunAsConfigTypeDef",
     {
         "Gid": int,
         "Uid": int,
     },
     total=False,
@@ -1182,14 +1316,28 @@
     "GetGroupVersionRequestRequestTypeDef",
     {
         "GroupId": str,
         "GroupVersionId": str,
     },
 )
 
+GroupVersionOutputTypeDef = TypedDict(
+    "GroupVersionOutputTypeDef",
+    {
+        "ConnectorDefinitionVersionArn": str,
+        "CoreDefinitionVersionArn": str,
+        "DeviceDefinitionVersionArn": str,
+        "FunctionDefinitionVersionArn": str,
+        "LoggerDefinitionVersionArn": str,
+        "ResourceDefinitionVersionArn": str,
+        "SubscriptionDefinitionVersionArn": str,
+    },
+    total=False,
+)
+
 GetLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "GetLoggerDefinitionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 
@@ -1341,14 +1489,23 @@
         "LatestVersion": str,
         "LatestVersionArn": str,
         "Name": str,
     },
     total=False,
 )
 
+GroupOwnerSettingOutputTypeDef = TypedDict(
+    "GroupOwnerSettingOutputTypeDef",
+    {
+        "AutoAddGroupOwner": bool,
+        "GroupOwner": str,
+    },
+    total=False,
+)
+
 GroupOwnerSettingTypeDef = TypedDict(
     "GroupOwnerSettingTypeDef",
     {
         "AutoAddGroupOwner": bool,
         "GroupOwner": str,
     },
     total=False,
@@ -1984,14 +2141,36 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredLoggerOutputTypeDef = TypedDict(
+    "_RequiredLoggerOutputTypeDef",
+    {
+        "Component": LoggerComponentType,
+        "Id": str,
+        "Level": LoggerLevelType,
+        "Type": LoggerTypeType,
+    },
+)
+_OptionalLoggerOutputTypeDef = TypedDict(
+    "_OptionalLoggerOutputTypeDef",
+    {
+        "Space": int,
+    },
+    total=False,
+)
+
+
+class LoggerOutputTypeDef(_RequiredLoggerOutputTypeDef, _OptionalLoggerOutputTypeDef):
+    pass
+
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -2025,23 +2204,40 @@
     {
         "DeploymentArn": str,
         "DeploymentId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SecretsManagerSecretResourceDataOutputTypeDef = TypedDict(
+    "SecretsManagerSecretResourceDataOutputTypeDef",
+    {
+        "ARN": str,
+        "AdditionalStagingLabelsToDownload": List[str],
+    },
+    total=False,
+)
+
 SecretsManagerSecretResourceDataTypeDef = TypedDict(
     "SecretsManagerSecretResourceDataTypeDef",
     {
         "ARN": str,
         "AdditionalStagingLabelsToDownload": Sequence[str],
     },
     total=False,
 )
 
+ResourceDownloadOwnerSettingOutputTypeDef = TypedDict(
+    "ResourceDownloadOwnerSettingOutputTypeDef",
+    {
+        "GroupOwner": str,
+        "GroupPermission": PermissionType,
+    },
+)
+
 ResourceDownloadOwnerSettingTypeDef = TypedDict(
     "ResourceDownloadOwnerSettingTypeDef",
     {
         "GroupOwner": str,
         "GroupPermission": PermissionType,
     },
 )
@@ -2114,14 +2310,24 @@
 StopBulkDeploymentRequestRequestTypeDef = TypedDict(
     "StopBulkDeploymentRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 
+SubscriptionOutputTypeDef = TypedDict(
+    "SubscriptionOutputTypeDef",
+    {
+        "Id": str,
+        "Source": str,
+        "Subject": str,
+        "Target": str,
+    },
+)
+
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
@@ -2418,15 +2624,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConnectivityInfoResponseTypeDef = TypedDict(
     "GetConnectivityInfoResponseTypeDef",
     {
-        "ConnectivityInfo": List[ConnectivityInfoTypeDef],
+        "ConnectivityInfo": List[ConnectivityInfoOutputTypeDef],
         "Message": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateConnectivityInfoRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectivityInfoRequestRequestTypeDef",
@@ -2446,14 +2652,22 @@
 class UpdateConnectivityInfoRequestRequestTypeDef(
     _RequiredUpdateConnectivityInfoRequestRequestTypeDef,
     _OptionalUpdateConnectivityInfoRequestRequestTypeDef,
 ):
     pass
 
 
+ConnectorDefinitionVersionOutputTypeDef = TypedDict(
+    "ConnectorDefinitionVersionOutputTypeDef",
+    {
+        "Connectors": List[ConnectorOutputTypeDef],
+    },
+    total=False,
+)
+
 ConnectorDefinitionVersionTypeDef = TypedDict(
     "ConnectorDefinitionVersionTypeDef",
     {
         "Connectors": Sequence[ConnectorTypeDef],
     },
     total=False,
 )
@@ -2477,14 +2691,22 @@
 class CreateConnectorDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
 
+CoreDefinitionVersionOutputTypeDef = TypedDict(
+    "CoreDefinitionVersionOutputTypeDef",
+    {
+        "Cores": List[CoreOutputTypeDef],
+    },
+    total=False,
+)
+
 CoreDefinitionVersionTypeDef = TypedDict(
     "CoreDefinitionVersionTypeDef",
     {
         "Cores": Sequence[CoreTypeDef],
     },
     total=False,
 )
@@ -2562,26 +2784,14 @@
 
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
 
-GetGroupVersionResponseTypeDef = TypedDict(
-    "GetGroupVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": GroupVersionTypeDef,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 _OptionalCreateLoggerDefinitionVersionRequestRequestTypeDef = TypedDict(
@@ -2708,14 +2918,40 @@
     {
         "Deployments": List[DeploymentTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeviceDefinitionVersionOutputTypeDef = TypedDict(
+    "DeviceDefinitionVersionOutputTypeDef",
+    {
+        "Devices": List[DeviceOutputTypeDef],
+    },
+    total=False,
+)
+
+FunctionDefaultExecutionConfigOutputTypeDef = TypedDict(
+    "FunctionDefaultExecutionConfigOutputTypeDef",
+    {
+        "IsolationMode": FunctionIsolationModeType,
+        "RunAs": FunctionRunAsConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+FunctionExecutionConfigOutputTypeDef = TypedDict(
+    "FunctionExecutionConfigOutputTypeDef",
+    {
+        "IsolationMode": FunctionIsolationModeType,
+        "RunAs": FunctionRunAsConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 FunctionDefaultExecutionConfigTypeDef = TypedDict(
     "FunctionDefaultExecutionConfigTypeDef",
     {
         "IsolationMode": FunctionIsolationModeType,
         "RunAs": FunctionRunAsConfigTypeDef,
     },
     total=False,
@@ -2726,14 +2962,26 @@
     {
         "IsolationMode": FunctionIsolationModeType,
         "RunAs": FunctionRunAsConfigTypeDef,
     },
     total=False,
 )
 
+GetGroupVersionResponseTypeDef = TypedDict(
+    "GetGroupVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": GroupVersionOutputTypeDef,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListGroupCertificateAuthoritiesResponseTypeDef = TypedDict(
     "ListGroupCertificateAuthoritiesResponseTypeDef",
     {
         "GroupCertificateAuthorities": List[GroupCertificateAuthorityPropertiesTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2743,14 +2991,33 @@
     {
         "Groups": List[GroupInformationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LocalDeviceResourceDataOutputTypeDef = TypedDict(
+    "LocalDeviceResourceDataOutputTypeDef",
+    {
+        "GroupOwnerSetting": GroupOwnerSettingOutputTypeDef,
+        "SourcePath": str,
+    },
+    total=False,
+)
+
+LocalVolumeResourceDataOutputTypeDef = TypedDict(
+    "LocalVolumeResourceDataOutputTypeDef",
+    {
+        "DestinationPath": str,
+        "GroupOwnerSetting": GroupOwnerSettingOutputTypeDef,
+        "SourcePath": str,
+    },
+    total=False,
+)
+
 LocalDeviceResourceDataTypeDef = TypedDict(
     "LocalDeviceResourceDataTypeDef",
     {
         "GroupOwnerSetting": GroupOwnerSettingTypeDef,
         "SourcePath": str,
     },
     total=False,
@@ -2834,14 +3101,42 @@
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LoggerDefinitionVersionOutputTypeDef = TypedDict(
+    "LoggerDefinitionVersionOutputTypeDef",
+    {
+        "Loggers": List[LoggerOutputTypeDef],
+    },
+    total=False,
+)
+
+S3MachineLearningModelResourceDataOutputTypeDef = TypedDict(
+    "S3MachineLearningModelResourceDataOutputTypeDef",
+    {
+        "DestinationPath": str,
+        "OwnerSetting": ResourceDownloadOwnerSettingOutputTypeDef,
+        "S3Uri": str,
+    },
+    total=False,
+)
+
+SageMakerMachineLearningModelResourceDataOutputTypeDef = TypedDict(
+    "SageMakerMachineLearningModelResourceDataOutputTypeDef",
+    {
+        "DestinationPath": str,
+        "OwnerSetting": ResourceDownloadOwnerSettingOutputTypeDef,
+        "SageMakerJobArn": str,
+    },
+    total=False,
+)
+
 S3MachineLearningModelResourceDataTypeDef = TypedDict(
     "S3MachineLearningModelResourceDataTypeDef",
     {
         "DestinationPath": str,
         "OwnerSetting": ResourceDownloadOwnerSettingTypeDef,
         "S3Uri": str,
     },
@@ -2862,14 +3157,22 @@
     "RuntimeConfigurationTypeDef",
     {
         "TelemetryConfiguration": TelemetryConfigurationTypeDef,
     },
     total=False,
 )
 
+SubscriptionDefinitionVersionOutputTypeDef = TypedDict(
+    "SubscriptionDefinitionVersionOutputTypeDef",
+    {
+        "Subscriptions": List[SubscriptionOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredUpdateThingRuntimeConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateThingRuntimeConfigurationRequestRequestTypeDef",
     {
         "ThingName": str,
     },
 )
 _OptionalUpdateThingRuntimeConfigurationRequestRequestTypeDef = TypedDict(
@@ -2893,133 +3196,127 @@
     {
         "Deployments": List[BulkDeploymentResultTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateConnectorDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateConnectorDefinitionRequestRequestTypeDef",
-    {
-        "AmznClientToken": str,
-        "InitialVersion": ConnectorDefinitionVersionTypeDef,
-        "Name": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
 GetConnectorDefinitionVersionResponseTypeDef = TypedDict(
     "GetConnectorDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": ConnectorDefinitionVersionTypeDef,
+        "Definition": ConnectorDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateCoreDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateCoreDefinitionRequestRequestTypeDef",
+CreateConnectorDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateConnectorDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
-        "InitialVersion": CoreDefinitionVersionTypeDef,
+        "InitialVersion": ConnectorDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 GetCoreDefinitionVersionResponseTypeDef = TypedDict(
     "GetCoreDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": CoreDefinitionVersionTypeDef,
+        "Definition": CoreDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDeviceDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateDeviceDefinitionRequestRequestTypeDef",
+CreateCoreDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateCoreDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
-        "InitialVersion": DeviceDefinitionVersionTypeDef,
+        "InitialVersion": CoreDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-GetDeviceDefinitionVersionResponseTypeDef = TypedDict(
-    "GetDeviceDefinitionVersionResponseTypeDef",
+CreateDeviceDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateDeviceDefinitionRequestRequestTypeDef",
     {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": DeviceDefinitionVersionTypeDef,
-        "Id": str,
-        "NextToken": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AmznClientToken": str,
+        "InitialVersion": DeviceDefinitionVersionTypeDef,
+        "Name": str,
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
 CreateLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "CreateLoggerDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": LoggerDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-GetLoggerDefinitionVersionResponseTypeDef = TypedDict(
-    "GetLoggerDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": LoggerDefinitionVersionTypeDef,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "CreateSubscriptionDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": SubscriptionDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-GetSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
-    "GetSubscriptionDefinitionVersionResponseTypeDef",
+GetDeviceDefinitionVersionResponseTypeDef = TypedDict(
+    "GetDeviceDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": SubscriptionDefinitionVersionTypeDef,
+        "Definition": DeviceDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FunctionDefaultConfigOutputTypeDef = TypedDict(
+    "FunctionDefaultConfigOutputTypeDef",
+    {
+        "Execution": FunctionDefaultExecutionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+FunctionConfigurationEnvironmentOutputTypeDef = TypedDict(
+    "FunctionConfigurationEnvironmentOutputTypeDef",
+    {
+        "AccessSysfs": bool,
+        "Execution": FunctionExecutionConfigOutputTypeDef,
+        "ResourceAccessPolicies": List[ResourceAccessPolicyOutputTypeDef],
+        "Variables": Dict[str, str],
+    },
+    total=False,
+)
+
 FunctionDefaultConfigTypeDef = TypedDict(
     "FunctionDefaultConfigTypeDef",
     {
         "Execution": FunctionDefaultExecutionConfigTypeDef,
     },
     total=False,
 )
@@ -3031,14 +3328,40 @@
         "Execution": FunctionExecutionConfigTypeDef,
         "ResourceAccessPolicies": Sequence[ResourceAccessPolicyTypeDef],
         "Variables": Mapping[str, str],
     },
     total=False,
 )
 
+GetLoggerDefinitionVersionResponseTypeDef = TypedDict(
+    "GetLoggerDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": LoggerDefinitionVersionOutputTypeDef,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ResourceDataContainerOutputTypeDef = TypedDict(
+    "ResourceDataContainerOutputTypeDef",
+    {
+        "LocalDeviceResourceData": LocalDeviceResourceDataOutputTypeDef,
+        "LocalVolumeResourceData": LocalVolumeResourceDataOutputTypeDef,
+        "S3MachineLearningModelResourceData": S3MachineLearningModelResourceDataOutputTypeDef,
+        "SageMakerMachineLearningModelResourceData": (
+            SageMakerMachineLearningModelResourceDataOutputTypeDef
+        ),
+        "SecretsManagerSecretResourceData": SecretsManagerSecretResourceDataOutputTypeDef,
+    },
+    total=False,
+)
+
 ResourceDataContainerTypeDef = TypedDict(
     "ResourceDataContainerTypeDef",
     {
         "LocalDeviceResourceData": LocalDeviceResourceDataTypeDef,
         "LocalVolumeResourceData": LocalVolumeResourceDataTypeDef,
         "S3MachineLearningModelResourceData": S3MachineLearningModelResourceDataTypeDef,
         "SageMakerMachineLearningModelResourceData": (
@@ -3053,14 +3376,42 @@
     "GetThingRuntimeConfigurationResponseTypeDef",
     {
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GetSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
+    "GetSubscriptionDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": SubscriptionDefinitionVersionOutputTypeDef,
+        "Id": str,
+        "NextToken": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+FunctionConfigurationOutputTypeDef = TypedDict(
+    "FunctionConfigurationOutputTypeDef",
+    {
+        "EncodingType": EncodingTypeType,
+        "Environment": FunctionConfigurationEnvironmentOutputTypeDef,
+        "ExecArgs": str,
+        "Executable": str,
+        "MemorySize": int,
+        "Pinned": bool,
+        "Timeout": int,
+        "FunctionRuntimeOverride": str,
+    },
+    total=False,
+)
+
 FunctionConfigurationTypeDef = TypedDict(
     "FunctionConfigurationTypeDef",
     {
         "EncodingType": EncodingTypeType,
         "Environment": FunctionConfigurationEnvironmentTypeDef,
         "ExecArgs": str,
         "Executable": str,
@@ -3068,23 +3419,52 @@
         "Pinned": bool,
         "Timeout": int,
         "FunctionRuntimeOverride": str,
     },
     total=False,
 )
 
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "ResourceDataContainer": ResourceDataContainerOutputTypeDef,
+    },
+)
+
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Id": str,
         "Name": str,
         "ResourceDataContainer": ResourceDataContainerTypeDef,
     },
 )
 
+_RequiredFunctionOutputTypeDef = TypedDict(
+    "_RequiredFunctionOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalFunctionOutputTypeDef = TypedDict(
+    "_OptionalFunctionOutputTypeDef",
+    {
+        "FunctionArn": str,
+        "FunctionConfiguration": FunctionConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class FunctionOutputTypeDef(_RequiredFunctionOutputTypeDef, _OptionalFunctionOutputTypeDef):
+    pass
+
+
 _RequiredFunctionTypeDef = TypedDict(
     "_RequiredFunctionTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalFunctionTypeDef = TypedDict(
@@ -3097,14 +3477,22 @@
 )
 
 
 class FunctionTypeDef(_RequiredFunctionTypeDef, _OptionalFunctionTypeDef):
     pass
 
 
+ResourceDefinitionVersionOutputTypeDef = TypedDict(
+    "ResourceDefinitionVersionOutputTypeDef",
+    {
+        "Resources": List[ResourceOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 _OptionalCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
@@ -3128,14 +3516,23 @@
     "ResourceDefinitionVersionTypeDef",
     {
         "Resources": Sequence[ResourceTypeDef],
     },
     total=False,
 )
 
+FunctionDefinitionVersionOutputTypeDef = TypedDict(
+    "FunctionDefinitionVersionOutputTypeDef",
+    {
+        "DefaultConfig": FunctionDefaultConfigOutputTypeDef,
+        "Functions": List[FunctionOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 _OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
@@ -3161,53 +3558,53 @@
     {
         "DefaultConfig": FunctionDefaultConfigTypeDef,
         "Functions": Sequence[FunctionTypeDef],
     },
     total=False,
 )
 
-CreateResourceDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateResourceDefinitionRequestRequestTypeDef",
-    {
-        "AmznClientToken": str,
-        "InitialVersion": ResourceDefinitionVersionTypeDef,
-        "Name": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
 GetResourceDefinitionVersionResponseTypeDef = TypedDict(
     "GetResourceDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": ResourceDefinitionVersionTypeDef,
+        "Definition": ResourceDefinitionVersionOutputTypeDef,
         "Id": str,
         "Version": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFunctionDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateFunctionDefinitionRequestRequestTypeDef",
+CreateResourceDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateResourceDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
-        "InitialVersion": FunctionDefinitionVersionTypeDef,
+        "InitialVersion": ResourceDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 GetFunctionDefinitionVersionResponseTypeDef = TypedDict(
     "GetFunctionDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": FunctionDefinitionVersionTypeDef,
+        "Definition": FunctionDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
+
+CreateFunctionDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateFunctionDefinitionRequestRequestTypeDef",
+    {
+        "AmznClientToken": str,
+        "InitialVersion": FunctionDefinitionVersionTypeDef,
+        "Name": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
```

### Comparing `mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass/type_defs.pyi` & `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -40,16 +40,19 @@
     "AssociateRoleToGroupRequestRequestTypeDef",
     "AssociateRoleToGroupResponseTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     "AssociateServiceRoleToAccountResponseTypeDef",
     "BulkDeploymentMetricsTypeDef",
     "ErrorDetailTypeDef",
     "BulkDeploymentTypeDef",
+    "ConnectivityInfoOutputTypeDef",
     "ConnectivityInfoTypeDef",
+    "ConnectorOutputTypeDef",
     "ConnectorTypeDef",
+    "CoreOutputTypeDef",
     "CoreTypeDef",
     "CreateConnectorDefinitionResponseTypeDef",
     "CreateConnectorDefinitionVersionResponseTypeDef",
     "CreateCoreDefinitionResponseTypeDef",
     "CreateCoreDefinitionVersionResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "CreateDeploymentResponseTypeDef",
@@ -80,19 +83,22 @@
     "DeleteDeviceDefinitionRequestRequestTypeDef",
     "DeleteFunctionDefinitionRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteLoggerDefinitionRequestRequestTypeDef",
     "DeleteResourceDefinitionRequestRequestTypeDef",
     "DeleteSubscriptionDefinitionRequestRequestTypeDef",
     "DeploymentTypeDef",
+    "DeviceOutputTypeDef",
     "DisassociateRoleFromGroupRequestRequestTypeDef",
     "DisassociateRoleFromGroupResponseTypeDef",
     "DisassociateServiceRoleFromAccountResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "ResourceAccessPolicyOutputTypeDef",
     "ResourceAccessPolicyTypeDef",
+    "FunctionRunAsConfigOutputTypeDef",
     "FunctionRunAsConfigTypeDef",
     "GetAssociatedRoleRequestRequestTypeDef",
     "GetAssociatedRoleResponseTypeDef",
     "GetBulkDeploymentStatusRequestRequestTypeDef",
     "GetConnectivityInfoRequestRequestTypeDef",
     "GetConnectorDefinitionRequestRequestTypeDef",
     "GetConnectorDefinitionResponseTypeDef",
@@ -110,27 +116,29 @@
     "GetGroupCertificateAuthorityRequestRequestTypeDef",
     "GetGroupCertificateAuthorityResponseTypeDef",
     "GetGroupCertificateConfigurationRequestRequestTypeDef",
     "GetGroupCertificateConfigurationResponseTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetGroupResponseTypeDef",
     "GetGroupVersionRequestRequestTypeDef",
+    "GroupVersionOutputTypeDef",
     "GetLoggerDefinitionRequestRequestTypeDef",
     "GetLoggerDefinitionResponseTypeDef",
     "GetLoggerDefinitionVersionRequestRequestTypeDef",
     "GetResourceDefinitionRequestRequestTypeDef",
     "GetResourceDefinitionResponseTypeDef",
     "GetResourceDefinitionVersionRequestRequestTypeDef",
     "GetServiceRoleForAccountResponseTypeDef",
     "GetSubscriptionDefinitionRequestRequestTypeDef",
     "GetSubscriptionDefinitionResponseTypeDef",
     "GetSubscriptionDefinitionVersionRequestRequestTypeDef",
     "GetThingRuntimeConfigurationRequestRequestTypeDef",
     "GroupCertificateAuthorityPropertiesTypeDef",
     "GroupInformationTypeDef",
+    "GroupOwnerSettingOutputTypeDef",
     "GroupOwnerSettingTypeDef",
     "ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
     "ListBulkDeploymentDetailedReportsRequestRequestTypeDef",
     "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
     "ListBulkDeploymentsRequestRequestTypeDef",
     "ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
     "ListConnectorDefinitionVersionsRequestRequestTypeDef",
@@ -166,24 +174,28 @@
     "ListResourceDefinitionsRequestRequestTypeDef",
     "ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
     "ListSubscriptionDefinitionVersionsRequestRequestTypeDef",
     "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
     "ListSubscriptionDefinitionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "LoggerOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ResetDeploymentsRequestRequestTypeDef",
     "ResetDeploymentsResponseTypeDef",
+    "SecretsManagerSecretResourceDataOutputTypeDef",
     "SecretsManagerSecretResourceDataTypeDef",
+    "ResourceDownloadOwnerSettingOutputTypeDef",
     "ResourceDownloadOwnerSettingTypeDef",
     "ResponseMetadataTypeDef",
     "TelemetryConfigurationTypeDef",
     "StartBulkDeploymentRequestRequestTypeDef",
     "StartBulkDeploymentResponseTypeDef",
     "StopBulkDeploymentRequestRequestTypeDef",
+    "SubscriptionOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TelemetryConfigurationUpdateTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateConnectivityInfoResponseTypeDef",
     "UpdateConnectorDefinitionRequestRequestTypeDef",
     "UpdateCoreDefinitionRequestRequestTypeDef",
     "UpdateDeviceDefinitionRequestRequestTypeDef",
@@ -196,78 +208,97 @@
     "UpdateSubscriptionDefinitionRequestRequestTypeDef",
     "BulkDeploymentResultTypeDef",
     "GetBulkDeploymentStatusResponseTypeDef",
     "GetDeploymentStatusResponseTypeDef",
     "ListBulkDeploymentsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
+    "ConnectorDefinitionVersionOutputTypeDef",
     "ConnectorDefinitionVersionTypeDef",
     "CreateConnectorDefinitionVersionRequestRequestTypeDef",
+    "CoreDefinitionVersionOutputTypeDef",
     "CoreDefinitionVersionTypeDef",
     "CreateCoreDefinitionVersionRequestRequestTypeDef",
     "CreateDeviceDefinitionVersionRequestRequestTypeDef",
     "DeviceDefinitionVersionTypeDef",
     "CreateGroupRequestRequestTypeDef",
-    "GetGroupVersionResponseTypeDef",
     "CreateLoggerDefinitionVersionRequestRequestTypeDef",
     "LoggerDefinitionVersionTypeDef",
     "CreateSubscriptionDefinitionVersionRequestRequestTypeDef",
     "SubscriptionDefinitionVersionTypeDef",
     "ListConnectorDefinitionsResponseTypeDef",
     "ListCoreDefinitionsResponseTypeDef",
     "ListDeviceDefinitionsResponseTypeDef",
     "ListFunctionDefinitionsResponseTypeDef",
     "ListLoggerDefinitionsResponseTypeDef",
     "ListResourceDefinitionsResponseTypeDef",
     "ListSubscriptionDefinitionsResponseTypeDef",
     "ListDeploymentsResponseTypeDef",
+    "DeviceDefinitionVersionOutputTypeDef",
+    "FunctionDefaultExecutionConfigOutputTypeDef",
+    "FunctionExecutionConfigOutputTypeDef",
     "FunctionDefaultExecutionConfigTypeDef",
     "FunctionExecutionConfigTypeDef",
+    "GetGroupVersionResponseTypeDef",
     "ListGroupCertificateAuthoritiesResponseTypeDef",
     "ListGroupsResponseTypeDef",
+    "LocalDeviceResourceDataOutputTypeDef",
+    "LocalVolumeResourceDataOutputTypeDef",
     "LocalDeviceResourceDataTypeDef",
     "LocalVolumeResourceDataTypeDef",
     "ListConnectorDefinitionVersionsResponseTypeDef",
     "ListCoreDefinitionVersionsResponseTypeDef",
     "ListDeviceDefinitionVersionsResponseTypeDef",
     "ListFunctionDefinitionVersionsResponseTypeDef",
     "ListGroupVersionsResponseTypeDef",
     "ListLoggerDefinitionVersionsResponseTypeDef",
     "ListResourceDefinitionVersionsResponseTypeDef",
     "ListSubscriptionDefinitionVersionsResponseTypeDef",
+    "LoggerDefinitionVersionOutputTypeDef",
+    "S3MachineLearningModelResourceDataOutputTypeDef",
+    "SageMakerMachineLearningModelResourceDataOutputTypeDef",
     "S3MachineLearningModelResourceDataTypeDef",
     "SageMakerMachineLearningModelResourceDataTypeDef",
     "RuntimeConfigurationTypeDef",
+    "SubscriptionDefinitionVersionOutputTypeDef",
     "UpdateThingRuntimeConfigurationRequestRequestTypeDef",
     "ListBulkDeploymentDetailedReportsResponseTypeDef",
-    "CreateConnectorDefinitionRequestRequestTypeDef",
     "GetConnectorDefinitionVersionResponseTypeDef",
-    "CreateCoreDefinitionRequestRequestTypeDef",
+    "CreateConnectorDefinitionRequestRequestTypeDef",
     "GetCoreDefinitionVersionResponseTypeDef",
+    "CreateCoreDefinitionRequestRequestTypeDef",
     "CreateDeviceDefinitionRequestRequestTypeDef",
-    "GetDeviceDefinitionVersionResponseTypeDef",
     "CreateLoggerDefinitionRequestRequestTypeDef",
-    "GetLoggerDefinitionVersionResponseTypeDef",
     "CreateSubscriptionDefinitionRequestRequestTypeDef",
-    "GetSubscriptionDefinitionVersionResponseTypeDef",
+    "GetDeviceDefinitionVersionResponseTypeDef",
+    "FunctionDefaultConfigOutputTypeDef",
+    "FunctionConfigurationEnvironmentOutputTypeDef",
     "FunctionDefaultConfigTypeDef",
     "FunctionConfigurationEnvironmentTypeDef",
+    "GetLoggerDefinitionVersionResponseTypeDef",
+    "ResourceDataContainerOutputTypeDef",
     "ResourceDataContainerTypeDef",
     "GetThingRuntimeConfigurationResponseTypeDef",
+    "GetSubscriptionDefinitionVersionResponseTypeDef",
+    "FunctionConfigurationOutputTypeDef",
     "FunctionConfigurationTypeDef",
+    "ResourceOutputTypeDef",
     "ResourceTypeDef",
+    "FunctionOutputTypeDef",
     "FunctionTypeDef",
+    "ResourceDefinitionVersionOutputTypeDef",
     "CreateResourceDefinitionVersionRequestRequestTypeDef",
     "ResourceDefinitionVersionTypeDef",
+    "FunctionDefinitionVersionOutputTypeDef",
     "CreateFunctionDefinitionVersionRequestRequestTypeDef",
     "FunctionDefinitionVersionTypeDef",
-    "CreateResourceDefinitionRequestRequestTypeDef",
     "GetResourceDefinitionVersionResponseTypeDef",
-    "CreateFunctionDefinitionRequestRequestTypeDef",
+    "CreateResourceDefinitionRequestRequestTypeDef",
     "GetFunctionDefinitionVersionResponseTypeDef",
+    "CreateFunctionDefinitionRequestRequestTypeDef",
 )
 
 AssociateRoleToGroupRequestRequestTypeDef = TypedDict(
     "AssociateRoleToGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "RoleArn": str,
@@ -322,25 +353,54 @@
         "BulkDeploymentArn": str,
         "BulkDeploymentId": str,
         "CreatedAt": str,
     },
     total=False,
 )
 
+ConnectivityInfoOutputTypeDef = TypedDict(
+    "ConnectivityInfoOutputTypeDef",
+    {
+        "HostAddress": str,
+        "Id": str,
+        "Metadata": str,
+        "PortNumber": int,
+    },
+    total=False,
+)
+
 ConnectivityInfoTypeDef = TypedDict(
     "ConnectivityInfoTypeDef",
     {
         "HostAddress": str,
         "Id": str,
         "Metadata": str,
         "PortNumber": int,
     },
     total=False,
 )
 
+_RequiredConnectorOutputTypeDef = TypedDict(
+    "_RequiredConnectorOutputTypeDef",
+    {
+        "ConnectorArn": str,
+        "Id": str,
+    },
+)
+_OptionalConnectorOutputTypeDef = TypedDict(
+    "_OptionalConnectorOutputTypeDef",
+    {
+        "Parameters": Dict[str, str],
+    },
+    total=False,
+)
+
+class ConnectorOutputTypeDef(_RequiredConnectorOutputTypeDef, _OptionalConnectorOutputTypeDef):
+    pass
+
 _RequiredConnectorTypeDef = TypedDict(
     "_RequiredConnectorTypeDef",
     {
         "ConnectorArn": str,
         "Id": str,
     },
 )
@@ -351,14 +411,33 @@
     },
     total=False,
 )
 
 class ConnectorTypeDef(_RequiredConnectorTypeDef, _OptionalConnectorTypeDef):
     pass
 
+_RequiredCoreOutputTypeDef = TypedDict(
+    "_RequiredCoreOutputTypeDef",
+    {
+        "CertificateArn": str,
+        "Id": str,
+        "ThingArn": str,
+    },
+)
+_OptionalCoreOutputTypeDef = TypedDict(
+    "_OptionalCoreOutputTypeDef",
+    {
+        "SyncShadow": bool,
+    },
+    total=False,
+)
+
+class CoreOutputTypeDef(_RequiredCoreOutputTypeDef, _OptionalCoreOutputTypeDef):
+    pass
+
 _RequiredCoreTypeDef = TypedDict(
     "_RequiredCoreTypeDef",
     {
         "CertificateArn": str,
         "Id": str,
         "ThingArn": str,
     },
@@ -837,14 +916,33 @@
         "DeploymentId": str,
         "DeploymentType": DeploymentTypeType,
         "GroupArn": str,
     },
     total=False,
 )
 
+_RequiredDeviceOutputTypeDef = TypedDict(
+    "_RequiredDeviceOutputTypeDef",
+    {
+        "CertificateArn": str,
+        "Id": str,
+        "ThingArn": str,
+    },
+)
+_OptionalDeviceOutputTypeDef = TypedDict(
+    "_OptionalDeviceOutputTypeDef",
+    {
+        "SyncShadow": bool,
+    },
+    total=False,
+)
+
+class DeviceOutputTypeDef(_RequiredDeviceOutputTypeDef, _OptionalDeviceOutputTypeDef):
+    pass
+
 DisassociateRoleFromGroupRequestRequestTypeDef = TypedDict(
     "DisassociateRoleFromGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
@@ -867,14 +965,33 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredResourceAccessPolicyOutputTypeDef = TypedDict(
+    "_RequiredResourceAccessPolicyOutputTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalResourceAccessPolicyOutputTypeDef = TypedDict(
+    "_OptionalResourceAccessPolicyOutputTypeDef",
+    {
+        "Permission": PermissionType,
+    },
+    total=False,
+)
+
+class ResourceAccessPolicyOutputTypeDef(
+    _RequiredResourceAccessPolicyOutputTypeDef, _OptionalResourceAccessPolicyOutputTypeDef
+):
+    pass
+
 _RequiredResourceAccessPolicyTypeDef = TypedDict(
     "_RequiredResourceAccessPolicyTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalResourceAccessPolicyTypeDef = TypedDict(
@@ -886,14 +1003,23 @@
 )
 
 class ResourceAccessPolicyTypeDef(
     _RequiredResourceAccessPolicyTypeDef, _OptionalResourceAccessPolicyTypeDef
 ):
     pass
 
+FunctionRunAsConfigOutputTypeDef = TypedDict(
+    "FunctionRunAsConfigOutputTypeDef",
+    {
+        "Gid": int,
+        "Uid": int,
+    },
+    total=False,
+)
+
 FunctionRunAsConfigTypeDef = TypedDict(
     "FunctionRunAsConfigTypeDef",
     {
         "Gid": int,
         "Uid": int,
     },
     total=False,
@@ -1157,14 +1283,28 @@
     "GetGroupVersionRequestRequestTypeDef",
     {
         "GroupId": str,
         "GroupVersionId": str,
     },
 )
 
+GroupVersionOutputTypeDef = TypedDict(
+    "GroupVersionOutputTypeDef",
+    {
+        "ConnectorDefinitionVersionArn": str,
+        "CoreDefinitionVersionArn": str,
+        "DeviceDefinitionVersionArn": str,
+        "FunctionDefinitionVersionArn": str,
+        "LoggerDefinitionVersionArn": str,
+        "ResourceDefinitionVersionArn": str,
+        "SubscriptionDefinitionVersionArn": str,
+    },
+    total=False,
+)
+
 GetLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "GetLoggerDefinitionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 
@@ -1312,14 +1452,23 @@
         "LatestVersion": str,
         "LatestVersionArn": str,
         "Name": str,
     },
     total=False,
 )
 
+GroupOwnerSettingOutputTypeDef = TypedDict(
+    "GroupOwnerSettingOutputTypeDef",
+    {
+        "AutoAddGroupOwner": bool,
+        "GroupOwner": str,
+    },
+    total=False,
+)
+
 GroupOwnerSettingTypeDef = TypedDict(
     "GroupOwnerSettingTypeDef",
     {
         "AutoAddGroupOwner": bool,
         "GroupOwner": str,
     },
     total=False,
@@ -1915,14 +2064,34 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredLoggerOutputTypeDef = TypedDict(
+    "_RequiredLoggerOutputTypeDef",
+    {
+        "Component": LoggerComponentType,
+        "Id": str,
+        "Level": LoggerLevelType,
+        "Type": LoggerTypeType,
+    },
+)
+_OptionalLoggerOutputTypeDef = TypedDict(
+    "_OptionalLoggerOutputTypeDef",
+    {
+        "Space": int,
+    },
+    total=False,
+)
+
+class LoggerOutputTypeDef(_RequiredLoggerOutputTypeDef, _OptionalLoggerOutputTypeDef):
+    pass
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1954,23 +2123,40 @@
     {
         "DeploymentArn": str,
         "DeploymentId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SecretsManagerSecretResourceDataOutputTypeDef = TypedDict(
+    "SecretsManagerSecretResourceDataOutputTypeDef",
+    {
+        "ARN": str,
+        "AdditionalStagingLabelsToDownload": List[str],
+    },
+    total=False,
+)
+
 SecretsManagerSecretResourceDataTypeDef = TypedDict(
     "SecretsManagerSecretResourceDataTypeDef",
     {
         "ARN": str,
         "AdditionalStagingLabelsToDownload": Sequence[str],
     },
     total=False,
 )
 
+ResourceDownloadOwnerSettingOutputTypeDef = TypedDict(
+    "ResourceDownloadOwnerSettingOutputTypeDef",
+    {
+        "GroupOwner": str,
+        "GroupPermission": PermissionType,
+    },
+)
+
 ResourceDownloadOwnerSettingTypeDef = TypedDict(
     "ResourceDownloadOwnerSettingTypeDef",
     {
         "GroupOwner": str,
         "GroupPermission": PermissionType,
     },
 )
@@ -2039,14 +2225,24 @@
 StopBulkDeploymentRequestRequestTypeDef = TypedDict(
     "StopBulkDeploymentRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 
+SubscriptionOutputTypeDef = TypedDict(
+    "SubscriptionOutputTypeDef",
+    {
+        "Id": str,
+        "Source": str,
+        "Subject": str,
+        "Target": str,
+    },
+)
+
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
@@ -2323,15 +2519,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConnectivityInfoResponseTypeDef = TypedDict(
     "GetConnectivityInfoResponseTypeDef",
     {
-        "ConnectivityInfo": List[ConnectivityInfoTypeDef],
+        "ConnectivityInfo": List[ConnectivityInfoOutputTypeDef],
         "Message": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateConnectivityInfoRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectivityInfoRequestRequestTypeDef",
@@ -2349,14 +2545,22 @@
 
 class UpdateConnectivityInfoRequestRequestTypeDef(
     _RequiredUpdateConnectivityInfoRequestRequestTypeDef,
     _OptionalUpdateConnectivityInfoRequestRequestTypeDef,
 ):
     pass
 
+ConnectorDefinitionVersionOutputTypeDef = TypedDict(
+    "ConnectorDefinitionVersionOutputTypeDef",
+    {
+        "Connectors": List[ConnectorOutputTypeDef],
+    },
+    total=False,
+)
+
 ConnectorDefinitionVersionTypeDef = TypedDict(
     "ConnectorDefinitionVersionTypeDef",
     {
         "Connectors": Sequence[ConnectorTypeDef],
     },
     total=False,
 )
@@ -2378,14 +2582,22 @@
 
 class CreateConnectorDefinitionVersionRequestRequestTypeDef(
     _RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef,
     _OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef,
 ):
     pass
 
+CoreDefinitionVersionOutputTypeDef = TypedDict(
+    "CoreDefinitionVersionOutputTypeDef",
+    {
+        "Cores": List[CoreOutputTypeDef],
+    },
+    total=False,
+)
+
 CoreDefinitionVersionTypeDef = TypedDict(
     "CoreDefinitionVersionTypeDef",
     {
         "Cores": Sequence[CoreTypeDef],
     },
     total=False,
 )
@@ -2457,26 +2669,14 @@
 )
 
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
-GetGroupVersionResponseTypeDef = TypedDict(
-    "GetGroupVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": GroupVersionTypeDef,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 _OptionalCreateLoggerDefinitionVersionRequestRequestTypeDef = TypedDict(
@@ -2599,14 +2799,40 @@
     {
         "Deployments": List[DeploymentTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeviceDefinitionVersionOutputTypeDef = TypedDict(
+    "DeviceDefinitionVersionOutputTypeDef",
+    {
+        "Devices": List[DeviceOutputTypeDef],
+    },
+    total=False,
+)
+
+FunctionDefaultExecutionConfigOutputTypeDef = TypedDict(
+    "FunctionDefaultExecutionConfigOutputTypeDef",
+    {
+        "IsolationMode": FunctionIsolationModeType,
+        "RunAs": FunctionRunAsConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+FunctionExecutionConfigOutputTypeDef = TypedDict(
+    "FunctionExecutionConfigOutputTypeDef",
+    {
+        "IsolationMode": FunctionIsolationModeType,
+        "RunAs": FunctionRunAsConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 FunctionDefaultExecutionConfigTypeDef = TypedDict(
     "FunctionDefaultExecutionConfigTypeDef",
     {
         "IsolationMode": FunctionIsolationModeType,
         "RunAs": FunctionRunAsConfigTypeDef,
     },
     total=False,
@@ -2617,14 +2843,26 @@
     {
         "IsolationMode": FunctionIsolationModeType,
         "RunAs": FunctionRunAsConfigTypeDef,
     },
     total=False,
 )
 
+GetGroupVersionResponseTypeDef = TypedDict(
+    "GetGroupVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": GroupVersionOutputTypeDef,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListGroupCertificateAuthoritiesResponseTypeDef = TypedDict(
     "ListGroupCertificateAuthoritiesResponseTypeDef",
     {
         "GroupCertificateAuthorities": List[GroupCertificateAuthorityPropertiesTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2634,14 +2872,33 @@
     {
         "Groups": List[GroupInformationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LocalDeviceResourceDataOutputTypeDef = TypedDict(
+    "LocalDeviceResourceDataOutputTypeDef",
+    {
+        "GroupOwnerSetting": GroupOwnerSettingOutputTypeDef,
+        "SourcePath": str,
+    },
+    total=False,
+)
+
+LocalVolumeResourceDataOutputTypeDef = TypedDict(
+    "LocalVolumeResourceDataOutputTypeDef",
+    {
+        "DestinationPath": str,
+        "GroupOwnerSetting": GroupOwnerSettingOutputTypeDef,
+        "SourcePath": str,
+    },
+    total=False,
+)
+
 LocalDeviceResourceDataTypeDef = TypedDict(
     "LocalDeviceResourceDataTypeDef",
     {
         "GroupOwnerSetting": GroupOwnerSettingTypeDef,
         "SourcePath": str,
     },
     total=False,
@@ -2725,14 +2982,42 @@
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LoggerDefinitionVersionOutputTypeDef = TypedDict(
+    "LoggerDefinitionVersionOutputTypeDef",
+    {
+        "Loggers": List[LoggerOutputTypeDef],
+    },
+    total=False,
+)
+
+S3MachineLearningModelResourceDataOutputTypeDef = TypedDict(
+    "S3MachineLearningModelResourceDataOutputTypeDef",
+    {
+        "DestinationPath": str,
+        "OwnerSetting": ResourceDownloadOwnerSettingOutputTypeDef,
+        "S3Uri": str,
+    },
+    total=False,
+)
+
+SageMakerMachineLearningModelResourceDataOutputTypeDef = TypedDict(
+    "SageMakerMachineLearningModelResourceDataOutputTypeDef",
+    {
+        "DestinationPath": str,
+        "OwnerSetting": ResourceDownloadOwnerSettingOutputTypeDef,
+        "SageMakerJobArn": str,
+    },
+    total=False,
+)
+
 S3MachineLearningModelResourceDataTypeDef = TypedDict(
     "S3MachineLearningModelResourceDataTypeDef",
     {
         "DestinationPath": str,
         "OwnerSetting": ResourceDownloadOwnerSettingTypeDef,
         "S3Uri": str,
     },
@@ -2753,14 +3038,22 @@
     "RuntimeConfigurationTypeDef",
     {
         "TelemetryConfiguration": TelemetryConfigurationTypeDef,
     },
     total=False,
 )
 
+SubscriptionDefinitionVersionOutputTypeDef = TypedDict(
+    "SubscriptionDefinitionVersionOutputTypeDef",
+    {
+        "Subscriptions": List[SubscriptionOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredUpdateThingRuntimeConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateThingRuntimeConfigurationRequestRequestTypeDef",
     {
         "ThingName": str,
     },
 )
 _OptionalUpdateThingRuntimeConfigurationRequestRequestTypeDef = TypedDict(
@@ -2782,133 +3075,127 @@
     {
         "Deployments": List[BulkDeploymentResultTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateConnectorDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateConnectorDefinitionRequestRequestTypeDef",
-    {
-        "AmznClientToken": str,
-        "InitialVersion": ConnectorDefinitionVersionTypeDef,
-        "Name": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
 GetConnectorDefinitionVersionResponseTypeDef = TypedDict(
     "GetConnectorDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": ConnectorDefinitionVersionTypeDef,
+        "Definition": ConnectorDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateCoreDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateCoreDefinitionRequestRequestTypeDef",
+CreateConnectorDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateConnectorDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
-        "InitialVersion": CoreDefinitionVersionTypeDef,
+        "InitialVersion": ConnectorDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 GetCoreDefinitionVersionResponseTypeDef = TypedDict(
     "GetCoreDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": CoreDefinitionVersionTypeDef,
+        "Definition": CoreDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDeviceDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateDeviceDefinitionRequestRequestTypeDef",
+CreateCoreDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateCoreDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
-        "InitialVersion": DeviceDefinitionVersionTypeDef,
+        "InitialVersion": CoreDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-GetDeviceDefinitionVersionResponseTypeDef = TypedDict(
-    "GetDeviceDefinitionVersionResponseTypeDef",
+CreateDeviceDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateDeviceDefinitionRequestRequestTypeDef",
     {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": DeviceDefinitionVersionTypeDef,
-        "Id": str,
-        "NextToken": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AmznClientToken": str,
+        "InitialVersion": DeviceDefinitionVersionTypeDef,
+        "Name": str,
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
 CreateLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "CreateLoggerDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": LoggerDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-GetLoggerDefinitionVersionResponseTypeDef = TypedDict(
-    "GetLoggerDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Definition": LoggerDefinitionVersionTypeDef,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "CreateSubscriptionDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": SubscriptionDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-GetSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
-    "GetSubscriptionDefinitionVersionResponseTypeDef",
+GetDeviceDefinitionVersionResponseTypeDef = TypedDict(
+    "GetDeviceDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": SubscriptionDefinitionVersionTypeDef,
+        "Definition": DeviceDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FunctionDefaultConfigOutputTypeDef = TypedDict(
+    "FunctionDefaultConfigOutputTypeDef",
+    {
+        "Execution": FunctionDefaultExecutionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+FunctionConfigurationEnvironmentOutputTypeDef = TypedDict(
+    "FunctionConfigurationEnvironmentOutputTypeDef",
+    {
+        "AccessSysfs": bool,
+        "Execution": FunctionExecutionConfigOutputTypeDef,
+        "ResourceAccessPolicies": List[ResourceAccessPolicyOutputTypeDef],
+        "Variables": Dict[str, str],
+    },
+    total=False,
+)
+
 FunctionDefaultConfigTypeDef = TypedDict(
     "FunctionDefaultConfigTypeDef",
     {
         "Execution": FunctionDefaultExecutionConfigTypeDef,
     },
     total=False,
 )
@@ -2920,14 +3207,40 @@
         "Execution": FunctionExecutionConfigTypeDef,
         "ResourceAccessPolicies": Sequence[ResourceAccessPolicyTypeDef],
         "Variables": Mapping[str, str],
     },
     total=False,
 )
 
+GetLoggerDefinitionVersionResponseTypeDef = TypedDict(
+    "GetLoggerDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": LoggerDefinitionVersionOutputTypeDef,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ResourceDataContainerOutputTypeDef = TypedDict(
+    "ResourceDataContainerOutputTypeDef",
+    {
+        "LocalDeviceResourceData": LocalDeviceResourceDataOutputTypeDef,
+        "LocalVolumeResourceData": LocalVolumeResourceDataOutputTypeDef,
+        "S3MachineLearningModelResourceData": S3MachineLearningModelResourceDataOutputTypeDef,
+        "SageMakerMachineLearningModelResourceData": (
+            SageMakerMachineLearningModelResourceDataOutputTypeDef
+        ),
+        "SecretsManagerSecretResourceData": SecretsManagerSecretResourceDataOutputTypeDef,
+    },
+    total=False,
+)
+
 ResourceDataContainerTypeDef = TypedDict(
     "ResourceDataContainerTypeDef",
     {
         "LocalDeviceResourceData": LocalDeviceResourceDataTypeDef,
         "LocalVolumeResourceData": LocalVolumeResourceDataTypeDef,
         "S3MachineLearningModelResourceData": S3MachineLearningModelResourceDataTypeDef,
         "SageMakerMachineLearningModelResourceData": (
@@ -2942,14 +3255,42 @@
     "GetThingRuntimeConfigurationResponseTypeDef",
     {
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GetSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
+    "GetSubscriptionDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Definition": SubscriptionDefinitionVersionOutputTypeDef,
+        "Id": str,
+        "NextToken": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+FunctionConfigurationOutputTypeDef = TypedDict(
+    "FunctionConfigurationOutputTypeDef",
+    {
+        "EncodingType": EncodingTypeType,
+        "Environment": FunctionConfigurationEnvironmentOutputTypeDef,
+        "ExecArgs": str,
+        "Executable": str,
+        "MemorySize": int,
+        "Pinned": bool,
+        "Timeout": int,
+        "FunctionRuntimeOverride": str,
+    },
+    total=False,
+)
+
 FunctionConfigurationTypeDef = TypedDict(
     "FunctionConfigurationTypeDef",
     {
         "EncodingType": EncodingTypeType,
         "Environment": FunctionConfigurationEnvironmentTypeDef,
         "ExecArgs": str,
         "Executable": str,
@@ -2957,23 +3298,50 @@
         "Pinned": bool,
         "Timeout": int,
         "FunctionRuntimeOverride": str,
     },
     total=False,
 )
 
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "ResourceDataContainer": ResourceDataContainerOutputTypeDef,
+    },
+)
+
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Id": str,
         "Name": str,
         "ResourceDataContainer": ResourceDataContainerTypeDef,
     },
 )
 
+_RequiredFunctionOutputTypeDef = TypedDict(
+    "_RequiredFunctionOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalFunctionOutputTypeDef = TypedDict(
+    "_OptionalFunctionOutputTypeDef",
+    {
+        "FunctionArn": str,
+        "FunctionConfiguration": FunctionConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class FunctionOutputTypeDef(_RequiredFunctionOutputTypeDef, _OptionalFunctionOutputTypeDef):
+    pass
+
 _RequiredFunctionTypeDef = TypedDict(
     "_RequiredFunctionTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalFunctionTypeDef = TypedDict(
@@ -2984,14 +3352,22 @@
     },
     total=False,
 )
 
 class FunctionTypeDef(_RequiredFunctionTypeDef, _OptionalFunctionTypeDef):
     pass
 
+ResourceDefinitionVersionOutputTypeDef = TypedDict(
+    "ResourceDefinitionVersionOutputTypeDef",
+    {
+        "Resources": List[ResourceOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 _OptionalCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
@@ -3013,14 +3389,23 @@
     "ResourceDefinitionVersionTypeDef",
     {
         "Resources": Sequence[ResourceTypeDef],
     },
     total=False,
 )
 
+FunctionDefinitionVersionOutputTypeDef = TypedDict(
+    "FunctionDefinitionVersionOutputTypeDef",
+    {
+        "DefaultConfig": FunctionDefaultConfigOutputTypeDef,
+        "Functions": List[FunctionOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 _OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
@@ -3044,53 +3429,53 @@
     {
         "DefaultConfig": FunctionDefaultConfigTypeDef,
         "Functions": Sequence[FunctionTypeDef],
     },
     total=False,
 )
 
-CreateResourceDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateResourceDefinitionRequestRequestTypeDef",
-    {
-        "AmznClientToken": str,
-        "InitialVersion": ResourceDefinitionVersionTypeDef,
-        "Name": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
 GetResourceDefinitionVersionResponseTypeDef = TypedDict(
     "GetResourceDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": ResourceDefinitionVersionTypeDef,
+        "Definition": ResourceDefinitionVersionOutputTypeDef,
         "Id": str,
         "Version": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFunctionDefinitionRequestRequestTypeDef = TypedDict(
-    "CreateFunctionDefinitionRequestRequestTypeDef",
+CreateResourceDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateResourceDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
-        "InitialVersion": FunctionDefinitionVersionTypeDef,
+        "InitialVersion": ResourceDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 GetFunctionDefinitionVersionResponseTypeDef = TypedDict(
     "GetFunctionDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
-        "Definition": FunctionDefinitionVersionTypeDef,
+        "Definition": FunctionDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
+
+CreateFunctionDefinitionRequestRequestTypeDef = TypedDict(
+    "CreateFunctionDefinitionRequestRequestTypeDef",
+    {
+        "AmznClientToken": str,
+        "InitialVersion": FunctionDefinitionVersionTypeDef,
+        "Name": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
```

### Comparing `mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass.egg-info/PKG-INFO` & `mypy-boto3-greengrass-1.28.12/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-greengrass
-Version: 1.28.0
-Summary: Type annotations for boto3.Greengrass 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 greengrass type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-greengrass"></a>
 
 # mypy-boto3-greengrass
 
 [![PyPI - mypy-boto3-greengrass](https://img.shields.io/pypi/v/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-greengrass?color=blue)](https://pypistats.org/packages/mypy-boto3-greengrass)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrass)](https://pepy.tech/project/mypy-boto3-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Greengrass 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[boto3.Greengrass 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
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
 [mypy-boto3-greengrass docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/).
 
 See how it helps to find and fix potential bugs:
 
@@ -429,16 +397,19 @@
     AssociateRoleToGroupRequestRequestTypeDef,
     AssociateRoleToGroupResponseTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
     AssociateServiceRoleToAccountResponseTypeDef,
     BulkDeploymentMetricsTypeDef,
     ErrorDetailTypeDef,
     BulkDeploymentTypeDef,
+    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
+    ConnectorOutputTypeDef,
     ConnectorTypeDef,
+    CoreOutputTypeDef,
     CoreTypeDef,
     CreateConnectorDefinitionResponseTypeDef,
     CreateConnectorDefinitionVersionResponseTypeDef,
     CreateCoreDefinitionResponseTypeDef,
     CreateCoreDefinitionVersionResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     CreateDeploymentResponseTypeDef,
@@ -469,19 +440,22 @@
     DeleteDeviceDefinitionRequestRequestTypeDef,
     DeleteFunctionDefinitionRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteLoggerDefinitionRequestRequestTypeDef,
     DeleteResourceDefinitionRequestRequestTypeDef,
     DeleteSubscriptionDefinitionRequestRequestTypeDef,
     DeploymentTypeDef,
+    DeviceOutputTypeDef,
     DisassociateRoleFromGroupRequestRequestTypeDef,
     DisassociateRoleFromGroupResponseTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    ResourceAccessPolicyOutputTypeDef,
     ResourceAccessPolicyTypeDef,
+    FunctionRunAsConfigOutputTypeDef,
     FunctionRunAsConfigTypeDef,
     GetAssociatedRoleRequestRequestTypeDef,
     GetAssociatedRoleResponseTypeDef,
     GetBulkDeploymentStatusRequestRequestTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetConnectorDefinitionRequestRequestTypeDef,
     GetConnectorDefinitionResponseTypeDef,
@@ -499,27 +473,29 @@
     GetGroupCertificateAuthorityRequestRequestTypeDef,
     GetGroupCertificateAuthorityResponseTypeDef,
     GetGroupCertificateConfigurationRequestRequestTypeDef,
     GetGroupCertificateConfigurationResponseTypeDef,
     GetGroupRequestRequestTypeDef,
     GetGroupResponseTypeDef,
     GetGroupVersionRequestRequestTypeDef,
+    GroupVersionOutputTypeDef,
     GetLoggerDefinitionRequestRequestTypeDef,
     GetLoggerDefinitionResponseTypeDef,
     GetLoggerDefinitionVersionRequestRequestTypeDef,
     GetResourceDefinitionRequestRequestTypeDef,
     GetResourceDefinitionResponseTypeDef,
     GetResourceDefinitionVersionRequestRequestTypeDef,
     GetServiceRoleForAccountResponseTypeDef,
     GetSubscriptionDefinitionRequestRequestTypeDef,
     GetSubscriptionDefinitionResponseTypeDef,
     GetSubscriptionDefinitionVersionRequestRequestTypeDef,
     GetThingRuntimeConfigurationRequestRequestTypeDef,
     GroupCertificateAuthorityPropertiesTypeDef,
     GroupInformationTypeDef,
+    GroupOwnerSettingOutputTypeDef,
     GroupOwnerSettingTypeDef,
     ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
     ListBulkDeploymentDetailedReportsRequestRequestTypeDef,
     ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef,
     ListBulkDeploymentsRequestRequestTypeDef,
     ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
     ListConnectorDefinitionVersionsRequestRequestTypeDef,
@@ -555,24 +531,28 @@
     ListResourceDefinitionsRequestRequestTypeDef,
     ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
     ListSubscriptionDefinitionVersionsRequestRequestTypeDef,
     ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef,
     ListSubscriptionDefinitionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    LoggerOutputTypeDef,
     PaginatorConfigTypeDef,
     ResetDeploymentsRequestRequestTypeDef,
     ResetDeploymentsResponseTypeDef,
+    SecretsManagerSecretResourceDataOutputTypeDef,
     SecretsManagerSecretResourceDataTypeDef,
+    ResourceDownloadOwnerSettingOutputTypeDef,
     ResourceDownloadOwnerSettingTypeDef,
     ResponseMetadataTypeDef,
     TelemetryConfigurationTypeDef,
     StartBulkDeploymentRequestRequestTypeDef,
     StartBulkDeploymentResponseTypeDef,
     StopBulkDeploymentRequestRequestTypeDef,
+    SubscriptionOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     TelemetryConfigurationUpdateTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectivityInfoResponseTypeDef,
     UpdateConnectorDefinitionRequestRequestTypeDef,
     UpdateCoreDefinitionRequestRequestTypeDef,
     UpdateDeviceDefinitionRequestRequestTypeDef,
@@ -585,78 +565,97 @@
     UpdateSubscriptionDefinitionRequestRequestTypeDef,
     BulkDeploymentResultTypeDef,
     GetBulkDeploymentStatusResponseTypeDef,
     GetDeploymentStatusResponseTypeDef,
     ListBulkDeploymentsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
+    ConnectorDefinitionVersionOutputTypeDef,
     ConnectorDefinitionVersionTypeDef,
     CreateConnectorDefinitionVersionRequestRequestTypeDef,
+    CoreDefinitionVersionOutputTypeDef,
     CoreDefinitionVersionTypeDef,
     CreateCoreDefinitionVersionRequestRequestTypeDef,
     CreateDeviceDefinitionVersionRequestRequestTypeDef,
     DeviceDefinitionVersionTypeDef,
     CreateGroupRequestRequestTypeDef,
-    GetGroupVersionResponseTypeDef,
     CreateLoggerDefinitionVersionRequestRequestTypeDef,
     LoggerDefinitionVersionTypeDef,
     CreateSubscriptionDefinitionVersionRequestRequestTypeDef,
     SubscriptionDefinitionVersionTypeDef,
     ListConnectorDefinitionsResponseTypeDef,
     ListCoreDefinitionsResponseTypeDef,
     ListDeviceDefinitionsResponseTypeDef,
     ListFunctionDefinitionsResponseTypeDef,
     ListLoggerDefinitionsResponseTypeDef,
     ListResourceDefinitionsResponseTypeDef,
     ListSubscriptionDefinitionsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
+    DeviceDefinitionVersionOutputTypeDef,
+    FunctionDefaultExecutionConfigOutputTypeDef,
+    FunctionExecutionConfigOutputTypeDef,
     FunctionDefaultExecutionConfigTypeDef,
     FunctionExecutionConfigTypeDef,
+    GetGroupVersionResponseTypeDef,
     ListGroupCertificateAuthoritiesResponseTypeDef,
     ListGroupsResponseTypeDef,
+    LocalDeviceResourceDataOutputTypeDef,
+    LocalVolumeResourceDataOutputTypeDef,
     LocalDeviceResourceDataTypeDef,
     LocalVolumeResourceDataTypeDef,
     ListConnectorDefinitionVersionsResponseTypeDef,
     ListCoreDefinitionVersionsResponseTypeDef,
     ListDeviceDefinitionVersionsResponseTypeDef,
     ListFunctionDefinitionVersionsResponseTypeDef,
     ListGroupVersionsResponseTypeDef,
     ListLoggerDefinitionVersionsResponseTypeDef,
     ListResourceDefinitionVersionsResponseTypeDef,
     ListSubscriptionDefinitionVersionsResponseTypeDef,
+    LoggerDefinitionVersionOutputTypeDef,
+    S3MachineLearningModelResourceDataOutputTypeDef,
+    SageMakerMachineLearningModelResourceDataOutputTypeDef,
     S3MachineLearningModelResourceDataTypeDef,
     SageMakerMachineLearningModelResourceDataTypeDef,
     RuntimeConfigurationTypeDef,
+    SubscriptionDefinitionVersionOutputTypeDef,
     UpdateThingRuntimeConfigurationRequestRequestTypeDef,
     ListBulkDeploymentDetailedReportsResponseTypeDef,
-    CreateConnectorDefinitionRequestRequestTypeDef,
     GetConnectorDefinitionVersionResponseTypeDef,
-    CreateCoreDefinitionRequestRequestTypeDef,
+    CreateConnectorDefinitionRequestRequestTypeDef,
     GetCoreDefinitionVersionResponseTypeDef,
+    CreateCoreDefinitionRequestRequestTypeDef,
     CreateDeviceDefinitionRequestRequestTypeDef,
-    GetDeviceDefinitionVersionResponseTypeDef,
     CreateLoggerDefinitionRequestRequestTypeDef,
-    GetLoggerDefinitionVersionResponseTypeDef,
     CreateSubscriptionDefinitionRequestRequestTypeDef,
-    GetSubscriptionDefinitionVersionResponseTypeDef,
+    GetDeviceDefinitionVersionResponseTypeDef,
+    FunctionDefaultConfigOutputTypeDef,
+    FunctionConfigurationEnvironmentOutputTypeDef,
     FunctionDefaultConfigTypeDef,
     FunctionConfigurationEnvironmentTypeDef,
+    GetLoggerDefinitionVersionResponseTypeDef,
+    ResourceDataContainerOutputTypeDef,
     ResourceDataContainerTypeDef,
     GetThingRuntimeConfigurationResponseTypeDef,
+    GetSubscriptionDefinitionVersionResponseTypeDef,
+    FunctionConfigurationOutputTypeDef,
     FunctionConfigurationTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
+    FunctionOutputTypeDef,
     FunctionTypeDef,
+    ResourceDefinitionVersionOutputTypeDef,
     CreateResourceDefinitionVersionRequestRequestTypeDef,
     ResourceDefinitionVersionTypeDef,
+    FunctionDefinitionVersionOutputTypeDef,
     CreateFunctionDefinitionVersionRequestRequestTypeDef,
     FunctionDefinitionVersionTypeDef,
-    CreateResourceDefinitionRequestRequestTypeDef,
     GetResourceDefinitionVersionResponseTypeDef,
-    CreateFunctionDefinitionRequestRequestTypeDef,
+    CreateResourceDefinitionRequestRequestTypeDef,
     GetFunctionDefinitionVersionResponseTypeDef,
+    CreateFunctionDefinitionRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AssociateRoleToGroupRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-greengrass-1.28.0/mypy_boto3_greengrass.egg-info/SOURCES.txt` & `mypy-boto3-greengrass-1.28.12/mypy_boto3_greengrass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.0/setup.py` & `mypy-boto3-greengrass-1.28.12/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-greengrass",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_greengrass"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Greengrass 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Greengrass 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

