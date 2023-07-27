# Comparing `tmp/mypy-boto3-appflow-1.28.0.tar.gz` & `tmp/mypy-boto3-appflow-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appflow-1.28.0.tar", last modified: Thu Jul  6 20:58:58 2023, max compression
+gzip compressed data, was "mypy-boto3-appflow-1.28.12.tar", last modified: Thu Jul 27 05:34:18 2023, max compression
```

## Comparing `mypy-boto3-appflow-1.28.0.tar` & `mypy-boto3-appflow-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.666221 mypy-boto3-appflow-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:33:14.000000 mypy-boto3-appflow-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19743 2023-07-06 20:58:58.666221 mypy-boto3-appflow-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18258 2023-07-06 20:33:14.000000 mypy-boto3-appflow-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.658220 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-06 20:33:14.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-06 20:33:14.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:33:14.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19559 2023-07-06 20:33:14.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-07-06 20:33:14.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18359 2023-07-06 20:33:15.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18357 2023-07-06 20:33:15.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:33:14.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71155 2023-07-06 20:33:18.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71053 2023-07-06 20:33:17.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:33:14.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.666221 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19743 2023-07-06 20:58:58.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-06 20:58:58.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:58.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 20:58:58.000000 mypy-boto3-appflow-1.28.0/mypy_boto3_appflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:58.666221 mypy-boto3-appflow-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:33:14.000000 mypy-boto3-appflow-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.356577 mypy-boto3-appflow-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-07-27 05:34:18.348577 mypy-boto3-appflow-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.344577 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19559 2023-07-27 05:17:20.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-07-27 05:17:20.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18437 2023-07-27 05:17:20.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-07-27 05:17:20.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   101626 2023-07-27 05:17:22.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101472 2023-07-27 05:17:21.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.348577 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-07-27 05:34:18.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-27 05:34:18.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:18.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:18.000000 mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:18.356577 mypy-boto3-appflow-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:17:19.000000 mypy-boto3-appflow-1.28.12/setup.py
```

### Comparing `mypy-boto3-appflow-1.28.0/LICENSE` & `mypy-boto3-appflow-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.0/PKG-INFO` & `mypy-boto3-appflow-1.28.12/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appflow
-Version: 1.28.0
-Summary: Type annotations for boto3.Appflow 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Appflow 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-appflow"></a>
 
 # mypy-boto3-appflow
 
 [![PyPI - mypy-boto3-appflow](https://img.shields.io/pypi/v/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appflow?color=blue)](https://pypistats.org/packages/mypy-boto3-appflow)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appflow)](https://pepy.tech/project/mypy-boto3-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Appflow 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[boto3.Appflow 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,189 +339,257 @@
 ### Typed dictionaries
 
 `mypy_boto3_appflow.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appflow.type_defs import (
+    AggregationConfigOutputTypeDef,
     AggregationConfigTypeDef,
     AmplitudeConnectorProfileCredentialsTypeDef,
+    AmplitudeSourcePropertiesOutputTypeDef,
     AmplitudeSourcePropertiesTypeDef,
     ApiKeyCredentialsTypeDef,
     AuthParameterTypeDef,
     BasicAuthCredentialsTypeDef,
     CancelFlowExecutionsRequestRequestTypeDef,
     CancelFlowExecutionsResponseTypeDef,
     ConnectorRuntimeSettingTypeDef,
-    DataTransferApiTypeDef,
+    DataTransferApiOutputTypeDef,
     ConnectorDetailTypeDef,
     DestinationFieldPropertiesTypeDef,
     SourceFieldPropertiesTypeDef,
     ConnectorEntityTypeDef,
     GoogleAnalyticsMetadataTypeDef,
     HoneycodeMetadataTypeDef,
     SalesforceMetadataTypeDef,
     SlackMetadataTypeDef,
     SnowflakeMetadataTypeDef,
     ZendeskMetadataTypeDef,
     ConnectorOAuthRequestTypeDef,
+    ConnectorOperatorOutputTypeDef,
     ConnectorOperatorTypeDef,
     DatadogConnectorProfileCredentialsTypeDef,
     DynatraceConnectorProfileCredentialsTypeDef,
     InforNexusConnectorProfileCredentialsTypeDef,
     RedshiftConnectorProfileCredentialsTypeDef,
     ServiceNowConnectorProfileCredentialsTypeDef,
     SingularConnectorProfileCredentialsTypeDef,
     SnowflakeConnectorProfileCredentialsTypeDef,
     TrendmicroConnectorProfileCredentialsTypeDef,
     VeevaConnectorProfileCredentialsTypeDef,
+    DatadogConnectorProfilePropertiesOutputTypeDef,
+    DynatraceConnectorProfilePropertiesOutputTypeDef,
+    InforNexusConnectorProfilePropertiesOutputTypeDef,
+    MarketoConnectorProfilePropertiesOutputTypeDef,
+    PardotConnectorProfilePropertiesOutputTypeDef,
+    RedshiftConnectorProfilePropertiesOutputTypeDef,
+    SalesforceConnectorProfilePropertiesOutputTypeDef,
+    ServiceNowConnectorProfilePropertiesOutputTypeDef,
+    SlackConnectorProfilePropertiesOutputTypeDef,
+    SnowflakeConnectorProfilePropertiesOutputTypeDef,
+    VeevaConnectorProfilePropertiesOutputTypeDef,
+    ZendeskConnectorProfilePropertiesOutputTypeDef,
     DatadogConnectorProfilePropertiesTypeDef,
     DynatraceConnectorProfilePropertiesTypeDef,
     InforNexusConnectorProfilePropertiesTypeDef,
     MarketoConnectorProfilePropertiesTypeDef,
     PardotConnectorProfilePropertiesTypeDef,
     RedshiftConnectorProfilePropertiesTypeDef,
     SalesforceConnectorProfilePropertiesTypeDef,
     ServiceNowConnectorProfilePropertiesTypeDef,
     SlackConnectorProfilePropertiesTypeDef,
     SnowflakeConnectorProfilePropertiesTypeDef,
     VeevaConnectorProfilePropertiesTypeDef,
     ZendeskConnectorProfilePropertiesTypeDef,
     PrivateConnectionProvisioningStateTypeDef,
+    LambdaConnectorProvisioningConfigOutputTypeDef,
     LambdaConnectorProvisioningConfigTypeDef,
     CreateConnectorProfileResponseTypeDef,
     CreateFlowResponseTypeDef,
     CustomAuthCredentialsTypeDef,
+    ErrorHandlingConfigOutputTypeDef,
     ErrorHandlingConfigTypeDef,
+    OAuth2PropertiesOutputTypeDef,
     OAuth2PropertiesTypeDef,
+    DataTransferApiTypeDef,
+    CustomerProfilesDestinationPropertiesOutputTypeDef,
     CustomerProfilesDestinationPropertiesTypeDef,
+    DatadogSourcePropertiesOutputTypeDef,
     DatadogSourcePropertiesTypeDef,
     DeleteConnectorProfileRequestRequestTypeDef,
     DeleteFlowRequestRequestTypeDef,
     DescribeConnectorEntityRequestRequestTypeDef,
     DescribeConnectorProfilesRequestRequestTypeDef,
     DescribeConnectorRequestRequestTypeDef,
     DescribeConnectorsRequestRequestTypeDef,
     DescribeFlowExecutionRecordsRequestRequestTypeDef,
     DescribeFlowRequestRequestTypeDef,
     ExecutionDetailsTypeDef,
+    DynatraceSourcePropertiesOutputTypeDef,
     DynatraceSourcePropertiesTypeDef,
     ErrorInfoTypeDef,
     RangeTypeDef,
+    GlueDataCatalogConfigOutputTypeDef,
     GlueDataCatalogConfigTypeDef,
+    GoogleAnalyticsSourcePropertiesOutputTypeDef,
     GoogleAnalyticsSourcePropertiesTypeDef,
+    IncrementalPullConfigOutputTypeDef,
     IncrementalPullConfigTypeDef,
+    InforNexusSourcePropertiesOutputTypeDef,
     InforNexusSourcePropertiesTypeDef,
     ListConnectorEntitiesRequestRequestTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListFlowsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    MarketoSourcePropertiesOutputTypeDef,
     MarketoSourcePropertiesTypeDef,
     RegistrationOutputTypeDef,
     OAuth2CustomParameterTypeDef,
+    OAuthPropertiesOutputTypeDef,
     OAuthPropertiesTypeDef,
+    PardotSourcePropertiesOutputTypeDef,
     PardotSourcePropertiesTypeDef,
+    PrefixConfigOutputTypeDef,
     PrefixConfigTypeDef,
     RegisterConnectorResponseTypeDef,
     ResetConnectorMetadataCacheRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    S3InputFormatConfigOutputTypeDef,
     S3InputFormatConfigTypeDef,
+    SuccessResponseHandlingConfigOutputTypeDef,
     SuccessResponseHandlingConfigTypeDef,
+    SAPODataSourcePropertiesOutputTypeDef,
     SAPODataSourcePropertiesTypeDef,
+    SalesforceSourcePropertiesOutputTypeDef,
     SalesforceSourcePropertiesTypeDef,
+    ScheduledTriggerPropertiesOutputTypeDef,
     ScheduledTriggerPropertiesTypeDef,
+    ServiceNowSourcePropertiesOutputTypeDef,
     ServiceNowSourcePropertiesTypeDef,
+    SingularSourcePropertiesOutputTypeDef,
     SingularSourcePropertiesTypeDef,
+    SlackSourcePropertiesOutputTypeDef,
     SlackSourcePropertiesTypeDef,
+    TrendmicroSourcePropertiesOutputTypeDef,
+    VeevaSourcePropertiesOutputTypeDef,
+    ZendeskSourcePropertiesOutputTypeDef,
     TrendmicroSourcePropertiesTypeDef,
     VeevaSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     StartFlowRequestRequestTypeDef,
     StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
     StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UnregisterConnectorRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
     CustomAuthConfigTypeDef,
-    CustomConnectorSourcePropertiesTypeDef,
+    CustomConnectorSourcePropertiesOutputTypeDef,
     ListConnectorsResponseTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ConnectorMetadataTypeDef,
     GoogleAnalyticsConnectorProfileCredentialsTypeDef,
     HoneycodeConnectorProfileCredentialsTypeDef,
     MarketoConnectorProfileCredentialsTypeDef,
     OAuth2CredentialsTypeDef,
     OAuthCredentialsTypeDef,
     PardotConnectorProfileCredentialsTypeDef,
     SalesforceConnectorProfileCredentialsTypeDef,
     SlackConnectorProfileCredentialsTypeDef,
     ZendeskConnectorProfileCredentialsTypeDef,
+    TaskOutputTypeDef,
     TaskTypeDef,
+    ConnectorProvisioningConfigOutputTypeDef,
     ConnectorProvisioningConfigTypeDef,
+    CustomConnectorDestinationPropertiesOutputTypeDef,
+    EventBridgeDestinationPropertiesOutputTypeDef,
+    HoneycodeDestinationPropertiesOutputTypeDef,
+    MarketoDestinationPropertiesOutputTypeDef,
+    RedshiftDestinationPropertiesOutputTypeDef,
+    SalesforceDestinationPropertiesOutputTypeDef,
+    SnowflakeDestinationPropertiesOutputTypeDef,
+    ZendeskDestinationPropertiesOutputTypeDef,
     CustomConnectorDestinationPropertiesTypeDef,
     EventBridgeDestinationPropertiesTypeDef,
     HoneycodeDestinationPropertiesTypeDef,
     MarketoDestinationPropertiesTypeDef,
     RedshiftDestinationPropertiesTypeDef,
     SalesforceDestinationPropertiesTypeDef,
     SnowflakeDestinationPropertiesTypeDef,
     ZendeskDestinationPropertiesTypeDef,
+    CustomConnectorProfilePropertiesOutputTypeDef,
     CustomConnectorProfilePropertiesTypeDef,
+    CustomConnectorSourcePropertiesTypeDef,
     FlowDefinitionTypeDef,
     ExecutionResultTypeDef,
     FieldTypeDetailsTypeDef,
+    MetadataCatalogConfigOutputTypeDef,
     MetadataCatalogConfigTypeDef,
     MetadataCatalogDetailTypeDef,
     OAuth2DefaultsTypeDef,
+    SAPODataConnectorProfilePropertiesOutputTypeDef,
     SAPODataConnectorProfilePropertiesTypeDef,
+    S3OutputFormatConfigOutputTypeDef,
+    UpsolverS3OutputFormatConfigOutputTypeDef,
     S3OutputFormatConfigTypeDef,
     UpsolverS3OutputFormatConfigTypeDef,
+    S3SourcePropertiesOutputTypeDef,
     S3SourcePropertiesTypeDef,
+    SAPODataDestinationPropertiesOutputTypeDef,
     SAPODataDestinationPropertiesTypeDef,
+    TriggerPropertiesOutputTypeDef,
     TriggerPropertiesTypeDef,
     CustomConnectorProfileCredentialsTypeDef,
     SAPODataConnectorProfileCredentialsTypeDef,
     RegisterConnectorRequestRequestTypeDef,
     UpdateConnectorRegistrationRequestRequestTypeDef,
     ListFlowsResponseTypeDef,
     SupportedFieldTypeDetailsTypeDef,
     ExecutionRecordTypeDef,
     AuthenticationConfigTypeDef,
+    ConnectorProfilePropertiesOutputTypeDef,
     ConnectorProfilePropertiesTypeDef,
+    S3DestinationPropertiesOutputTypeDef,
+    UpsolverDestinationPropertiesOutputTypeDef,
     S3DestinationPropertiesTypeDef,
     UpsolverDestinationPropertiesTypeDef,
+    SourceConnectorPropertiesOutputTypeDef,
     SourceConnectorPropertiesTypeDef,
+    TriggerConfigOutputTypeDef,
     TriggerConfigTypeDef,
     ConnectorProfileCredentialsTypeDef,
     ConnectorEntityFieldTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     ConnectorConfigurationTypeDef,
     ConnectorProfileTypeDef,
+    DestinationConnectorPropertiesOutputTypeDef,
     DestinationConnectorPropertiesTypeDef,
+    SourceFlowConfigOutputTypeDef,
     SourceFlowConfigTypeDef,
     ConnectorProfileConfigTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
+    DestinationFlowConfigOutputTypeDef,
     DestinationFlowConfigTypeDef,
     CreateConnectorProfileRequestRequestTypeDef,
     UpdateConnectorProfileRequestRequestTypeDef,
-    CreateFlowRequestRequestTypeDef,
     DescribeFlowResponseTypeDef,
+    CreateFlowRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AggregationConfigTypeDef:
+def get_structure() -> AggregationConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appflow-1.28.0/README.md` & `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-appflow
+Version: 1.28.12
+Summary: Type annotations for boto3.Appflow 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 appflow type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-appflow"></a>
 
 # mypy-boto3-appflow
 
 [![PyPI - mypy-boto3-appflow](https://img.shields.io/pypi/v/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appflow?color=blue)](https://pypistats.org/packages/mypy-boto3-appflow)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appflow)](https://pepy.tech/project/mypy-boto3-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Appflow 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[boto3.Appflow 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -307,189 +339,257 @@
 ### Typed dictionaries
 
 `mypy_boto3_appflow.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appflow.type_defs import (
+    AggregationConfigOutputTypeDef,
     AggregationConfigTypeDef,
     AmplitudeConnectorProfileCredentialsTypeDef,
+    AmplitudeSourcePropertiesOutputTypeDef,
     AmplitudeSourcePropertiesTypeDef,
     ApiKeyCredentialsTypeDef,
     AuthParameterTypeDef,
     BasicAuthCredentialsTypeDef,
     CancelFlowExecutionsRequestRequestTypeDef,
     CancelFlowExecutionsResponseTypeDef,
     ConnectorRuntimeSettingTypeDef,
-    DataTransferApiTypeDef,
+    DataTransferApiOutputTypeDef,
     ConnectorDetailTypeDef,
     DestinationFieldPropertiesTypeDef,
     SourceFieldPropertiesTypeDef,
     ConnectorEntityTypeDef,
     GoogleAnalyticsMetadataTypeDef,
     HoneycodeMetadataTypeDef,
     SalesforceMetadataTypeDef,
     SlackMetadataTypeDef,
     SnowflakeMetadataTypeDef,
     ZendeskMetadataTypeDef,
     ConnectorOAuthRequestTypeDef,
+    ConnectorOperatorOutputTypeDef,
     ConnectorOperatorTypeDef,
     DatadogConnectorProfileCredentialsTypeDef,
     DynatraceConnectorProfileCredentialsTypeDef,
     InforNexusConnectorProfileCredentialsTypeDef,
     RedshiftConnectorProfileCredentialsTypeDef,
     ServiceNowConnectorProfileCredentialsTypeDef,
     SingularConnectorProfileCredentialsTypeDef,
     SnowflakeConnectorProfileCredentialsTypeDef,
     TrendmicroConnectorProfileCredentialsTypeDef,
     VeevaConnectorProfileCredentialsTypeDef,
+    DatadogConnectorProfilePropertiesOutputTypeDef,
+    DynatraceConnectorProfilePropertiesOutputTypeDef,
+    InforNexusConnectorProfilePropertiesOutputTypeDef,
+    MarketoConnectorProfilePropertiesOutputTypeDef,
+    PardotConnectorProfilePropertiesOutputTypeDef,
+    RedshiftConnectorProfilePropertiesOutputTypeDef,
+    SalesforceConnectorProfilePropertiesOutputTypeDef,
+    ServiceNowConnectorProfilePropertiesOutputTypeDef,
+    SlackConnectorProfilePropertiesOutputTypeDef,
+    SnowflakeConnectorProfilePropertiesOutputTypeDef,
+    VeevaConnectorProfilePropertiesOutputTypeDef,
+    ZendeskConnectorProfilePropertiesOutputTypeDef,
     DatadogConnectorProfilePropertiesTypeDef,
     DynatraceConnectorProfilePropertiesTypeDef,
     InforNexusConnectorProfilePropertiesTypeDef,
     MarketoConnectorProfilePropertiesTypeDef,
     PardotConnectorProfilePropertiesTypeDef,
     RedshiftConnectorProfilePropertiesTypeDef,
     SalesforceConnectorProfilePropertiesTypeDef,
     ServiceNowConnectorProfilePropertiesTypeDef,
     SlackConnectorProfilePropertiesTypeDef,
     SnowflakeConnectorProfilePropertiesTypeDef,
     VeevaConnectorProfilePropertiesTypeDef,
     ZendeskConnectorProfilePropertiesTypeDef,
     PrivateConnectionProvisioningStateTypeDef,
+    LambdaConnectorProvisioningConfigOutputTypeDef,
     LambdaConnectorProvisioningConfigTypeDef,
     CreateConnectorProfileResponseTypeDef,
     CreateFlowResponseTypeDef,
     CustomAuthCredentialsTypeDef,
+    ErrorHandlingConfigOutputTypeDef,
     ErrorHandlingConfigTypeDef,
+    OAuth2PropertiesOutputTypeDef,
     OAuth2PropertiesTypeDef,
+    DataTransferApiTypeDef,
+    CustomerProfilesDestinationPropertiesOutputTypeDef,
     CustomerProfilesDestinationPropertiesTypeDef,
+    DatadogSourcePropertiesOutputTypeDef,
     DatadogSourcePropertiesTypeDef,
     DeleteConnectorProfileRequestRequestTypeDef,
     DeleteFlowRequestRequestTypeDef,
     DescribeConnectorEntityRequestRequestTypeDef,
     DescribeConnectorProfilesRequestRequestTypeDef,
     DescribeConnectorRequestRequestTypeDef,
     DescribeConnectorsRequestRequestTypeDef,
     DescribeFlowExecutionRecordsRequestRequestTypeDef,
     DescribeFlowRequestRequestTypeDef,
     ExecutionDetailsTypeDef,
+    DynatraceSourcePropertiesOutputTypeDef,
     DynatraceSourcePropertiesTypeDef,
     ErrorInfoTypeDef,
     RangeTypeDef,
+    GlueDataCatalogConfigOutputTypeDef,
     GlueDataCatalogConfigTypeDef,
+    GoogleAnalyticsSourcePropertiesOutputTypeDef,
     GoogleAnalyticsSourcePropertiesTypeDef,
+    IncrementalPullConfigOutputTypeDef,
     IncrementalPullConfigTypeDef,
+    InforNexusSourcePropertiesOutputTypeDef,
     InforNexusSourcePropertiesTypeDef,
     ListConnectorEntitiesRequestRequestTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListFlowsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    MarketoSourcePropertiesOutputTypeDef,
     MarketoSourcePropertiesTypeDef,
     RegistrationOutputTypeDef,
     OAuth2CustomParameterTypeDef,
+    OAuthPropertiesOutputTypeDef,
     OAuthPropertiesTypeDef,
+    PardotSourcePropertiesOutputTypeDef,
     PardotSourcePropertiesTypeDef,
+    PrefixConfigOutputTypeDef,
     PrefixConfigTypeDef,
     RegisterConnectorResponseTypeDef,
     ResetConnectorMetadataCacheRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    S3InputFormatConfigOutputTypeDef,
     S3InputFormatConfigTypeDef,
+    SuccessResponseHandlingConfigOutputTypeDef,
     SuccessResponseHandlingConfigTypeDef,
+    SAPODataSourcePropertiesOutputTypeDef,
     SAPODataSourcePropertiesTypeDef,
+    SalesforceSourcePropertiesOutputTypeDef,
     SalesforceSourcePropertiesTypeDef,
+    ScheduledTriggerPropertiesOutputTypeDef,
     ScheduledTriggerPropertiesTypeDef,
+    ServiceNowSourcePropertiesOutputTypeDef,
     ServiceNowSourcePropertiesTypeDef,
+    SingularSourcePropertiesOutputTypeDef,
     SingularSourcePropertiesTypeDef,
+    SlackSourcePropertiesOutputTypeDef,
     SlackSourcePropertiesTypeDef,
+    TrendmicroSourcePropertiesOutputTypeDef,
+    VeevaSourcePropertiesOutputTypeDef,
+    ZendeskSourcePropertiesOutputTypeDef,
     TrendmicroSourcePropertiesTypeDef,
     VeevaSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     StartFlowRequestRequestTypeDef,
     StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
     StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UnregisterConnectorRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
     CustomAuthConfigTypeDef,
-    CustomConnectorSourcePropertiesTypeDef,
+    CustomConnectorSourcePropertiesOutputTypeDef,
     ListConnectorsResponseTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ConnectorMetadataTypeDef,
     GoogleAnalyticsConnectorProfileCredentialsTypeDef,
     HoneycodeConnectorProfileCredentialsTypeDef,
     MarketoConnectorProfileCredentialsTypeDef,
     OAuth2CredentialsTypeDef,
     OAuthCredentialsTypeDef,
     PardotConnectorProfileCredentialsTypeDef,
     SalesforceConnectorProfileCredentialsTypeDef,
     SlackConnectorProfileCredentialsTypeDef,
     ZendeskConnectorProfileCredentialsTypeDef,
+    TaskOutputTypeDef,
     TaskTypeDef,
+    ConnectorProvisioningConfigOutputTypeDef,
     ConnectorProvisioningConfigTypeDef,
+    CustomConnectorDestinationPropertiesOutputTypeDef,
+    EventBridgeDestinationPropertiesOutputTypeDef,
+    HoneycodeDestinationPropertiesOutputTypeDef,
+    MarketoDestinationPropertiesOutputTypeDef,
+    RedshiftDestinationPropertiesOutputTypeDef,
+    SalesforceDestinationPropertiesOutputTypeDef,
+    SnowflakeDestinationPropertiesOutputTypeDef,
+    ZendeskDestinationPropertiesOutputTypeDef,
     CustomConnectorDestinationPropertiesTypeDef,
     EventBridgeDestinationPropertiesTypeDef,
     HoneycodeDestinationPropertiesTypeDef,
     MarketoDestinationPropertiesTypeDef,
     RedshiftDestinationPropertiesTypeDef,
     SalesforceDestinationPropertiesTypeDef,
     SnowflakeDestinationPropertiesTypeDef,
     ZendeskDestinationPropertiesTypeDef,
+    CustomConnectorProfilePropertiesOutputTypeDef,
     CustomConnectorProfilePropertiesTypeDef,
+    CustomConnectorSourcePropertiesTypeDef,
     FlowDefinitionTypeDef,
     ExecutionResultTypeDef,
     FieldTypeDetailsTypeDef,
+    MetadataCatalogConfigOutputTypeDef,
     MetadataCatalogConfigTypeDef,
     MetadataCatalogDetailTypeDef,
     OAuth2DefaultsTypeDef,
+    SAPODataConnectorProfilePropertiesOutputTypeDef,
     SAPODataConnectorProfilePropertiesTypeDef,
+    S3OutputFormatConfigOutputTypeDef,
+    UpsolverS3OutputFormatConfigOutputTypeDef,
     S3OutputFormatConfigTypeDef,
     UpsolverS3OutputFormatConfigTypeDef,
+    S3SourcePropertiesOutputTypeDef,
     S3SourcePropertiesTypeDef,
+    SAPODataDestinationPropertiesOutputTypeDef,
     SAPODataDestinationPropertiesTypeDef,
+    TriggerPropertiesOutputTypeDef,
     TriggerPropertiesTypeDef,
     CustomConnectorProfileCredentialsTypeDef,
     SAPODataConnectorProfileCredentialsTypeDef,
     RegisterConnectorRequestRequestTypeDef,
     UpdateConnectorRegistrationRequestRequestTypeDef,
     ListFlowsResponseTypeDef,
     SupportedFieldTypeDetailsTypeDef,
     ExecutionRecordTypeDef,
     AuthenticationConfigTypeDef,
+    ConnectorProfilePropertiesOutputTypeDef,
     ConnectorProfilePropertiesTypeDef,
+    S3DestinationPropertiesOutputTypeDef,
+    UpsolverDestinationPropertiesOutputTypeDef,
     S3DestinationPropertiesTypeDef,
     UpsolverDestinationPropertiesTypeDef,
+    SourceConnectorPropertiesOutputTypeDef,
     SourceConnectorPropertiesTypeDef,
+    TriggerConfigOutputTypeDef,
     TriggerConfigTypeDef,
     ConnectorProfileCredentialsTypeDef,
     ConnectorEntityFieldTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     ConnectorConfigurationTypeDef,
     ConnectorProfileTypeDef,
+    DestinationConnectorPropertiesOutputTypeDef,
     DestinationConnectorPropertiesTypeDef,
+    SourceFlowConfigOutputTypeDef,
     SourceFlowConfigTypeDef,
     ConnectorProfileConfigTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
+    DestinationFlowConfigOutputTypeDef,
     DestinationFlowConfigTypeDef,
     CreateConnectorProfileRequestRequestTypeDef,
     UpdateConnectorProfileRequestRequestTypeDef,
-    CreateFlowRequestRequestTypeDef,
     DescribeFlowResponseTypeDef,
+    CreateFlowRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AggregationConfigTypeDef:
+def get_structure() -> AggregationConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/__main__.py` & `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Appflow 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Appflow 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow\nOther"
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

### Comparing `mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/client.py` & `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/client.pyi` & `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/literals.py` & `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -585,14 +585,15 @@
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
@@ -671,26 +672,28 @@
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

### Comparing `mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/literals.pyi` & `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -583,14 +583,15 @@
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
@@ -669,26 +670,28 @@
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

### Comparing `mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/type_defs.py` & `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/type_defs.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for appflow service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_appflow.type_defs import AggregationConfigTypeDef
+    from mypy_boto3_appflow.type_defs import AggregationConfigOutputTypeDef
 
-    data: AggregationConfigTypeDef = {...}
+    data: AggregationConfigOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -64,189 +64,265 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AggregationConfigOutputTypeDef",
     "AggregationConfigTypeDef",
     "AmplitudeConnectorProfileCredentialsTypeDef",
+    "AmplitudeSourcePropertiesOutputTypeDef",
     "AmplitudeSourcePropertiesTypeDef",
     "ApiKeyCredentialsTypeDef",
     "AuthParameterTypeDef",
     "BasicAuthCredentialsTypeDef",
     "CancelFlowExecutionsRequestRequestTypeDef",
     "CancelFlowExecutionsResponseTypeDef",
     "ConnectorRuntimeSettingTypeDef",
-    "DataTransferApiTypeDef",
+    "DataTransferApiOutputTypeDef",
     "ConnectorDetailTypeDef",
     "DestinationFieldPropertiesTypeDef",
     "SourceFieldPropertiesTypeDef",
     "ConnectorEntityTypeDef",
     "GoogleAnalyticsMetadataTypeDef",
     "HoneycodeMetadataTypeDef",
     "SalesforceMetadataTypeDef",
     "SlackMetadataTypeDef",
     "SnowflakeMetadataTypeDef",
     "ZendeskMetadataTypeDef",
     "ConnectorOAuthRequestTypeDef",
+    "ConnectorOperatorOutputTypeDef",
     "ConnectorOperatorTypeDef",
     "DatadogConnectorProfileCredentialsTypeDef",
     "DynatraceConnectorProfileCredentialsTypeDef",
     "InforNexusConnectorProfileCredentialsTypeDef",
     "RedshiftConnectorProfileCredentialsTypeDef",
     "ServiceNowConnectorProfileCredentialsTypeDef",
     "SingularConnectorProfileCredentialsTypeDef",
     "SnowflakeConnectorProfileCredentialsTypeDef",
     "TrendmicroConnectorProfileCredentialsTypeDef",
     "VeevaConnectorProfileCredentialsTypeDef",
+    "DatadogConnectorProfilePropertiesOutputTypeDef",
+    "DynatraceConnectorProfilePropertiesOutputTypeDef",
+    "InforNexusConnectorProfilePropertiesOutputTypeDef",
+    "MarketoConnectorProfilePropertiesOutputTypeDef",
+    "PardotConnectorProfilePropertiesOutputTypeDef",
+    "RedshiftConnectorProfilePropertiesOutputTypeDef",
+    "SalesforceConnectorProfilePropertiesOutputTypeDef",
+    "ServiceNowConnectorProfilePropertiesOutputTypeDef",
+    "SlackConnectorProfilePropertiesOutputTypeDef",
+    "SnowflakeConnectorProfilePropertiesOutputTypeDef",
+    "VeevaConnectorProfilePropertiesOutputTypeDef",
+    "ZendeskConnectorProfilePropertiesOutputTypeDef",
     "DatadogConnectorProfilePropertiesTypeDef",
     "DynatraceConnectorProfilePropertiesTypeDef",
     "InforNexusConnectorProfilePropertiesTypeDef",
     "MarketoConnectorProfilePropertiesTypeDef",
     "PardotConnectorProfilePropertiesTypeDef",
     "RedshiftConnectorProfilePropertiesTypeDef",
     "SalesforceConnectorProfilePropertiesTypeDef",
     "ServiceNowConnectorProfilePropertiesTypeDef",
     "SlackConnectorProfilePropertiesTypeDef",
     "SnowflakeConnectorProfilePropertiesTypeDef",
     "VeevaConnectorProfilePropertiesTypeDef",
     "ZendeskConnectorProfilePropertiesTypeDef",
     "PrivateConnectionProvisioningStateTypeDef",
+    "LambdaConnectorProvisioningConfigOutputTypeDef",
     "LambdaConnectorProvisioningConfigTypeDef",
     "CreateConnectorProfileResponseTypeDef",
     "CreateFlowResponseTypeDef",
     "CustomAuthCredentialsTypeDef",
+    "ErrorHandlingConfigOutputTypeDef",
     "ErrorHandlingConfigTypeDef",
+    "OAuth2PropertiesOutputTypeDef",
     "OAuth2PropertiesTypeDef",
+    "DataTransferApiTypeDef",
+    "CustomerProfilesDestinationPropertiesOutputTypeDef",
     "CustomerProfilesDestinationPropertiesTypeDef",
+    "DatadogSourcePropertiesOutputTypeDef",
     "DatadogSourcePropertiesTypeDef",
     "DeleteConnectorProfileRequestRequestTypeDef",
     "DeleteFlowRequestRequestTypeDef",
     "DescribeConnectorEntityRequestRequestTypeDef",
     "DescribeConnectorProfilesRequestRequestTypeDef",
     "DescribeConnectorRequestRequestTypeDef",
     "DescribeConnectorsRequestRequestTypeDef",
     "DescribeFlowExecutionRecordsRequestRequestTypeDef",
     "DescribeFlowRequestRequestTypeDef",
     "ExecutionDetailsTypeDef",
+    "DynatraceSourcePropertiesOutputTypeDef",
     "DynatraceSourcePropertiesTypeDef",
     "ErrorInfoTypeDef",
     "RangeTypeDef",
+    "GlueDataCatalogConfigOutputTypeDef",
     "GlueDataCatalogConfigTypeDef",
+    "GoogleAnalyticsSourcePropertiesOutputTypeDef",
     "GoogleAnalyticsSourcePropertiesTypeDef",
+    "IncrementalPullConfigOutputTypeDef",
     "IncrementalPullConfigTypeDef",
+    "InforNexusSourcePropertiesOutputTypeDef",
     "InforNexusSourcePropertiesTypeDef",
     "ListConnectorEntitiesRequestRequestTypeDef",
     "ListConnectorsRequestRequestTypeDef",
     "ListFlowsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "MarketoSourcePropertiesOutputTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "RegistrationOutputTypeDef",
     "OAuth2CustomParameterTypeDef",
+    "OAuthPropertiesOutputTypeDef",
     "OAuthPropertiesTypeDef",
+    "PardotSourcePropertiesOutputTypeDef",
     "PardotSourcePropertiesTypeDef",
+    "PrefixConfigOutputTypeDef",
     "PrefixConfigTypeDef",
     "RegisterConnectorResponseTypeDef",
     "ResetConnectorMetadataCacheRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "S3InputFormatConfigOutputTypeDef",
     "S3InputFormatConfigTypeDef",
+    "SuccessResponseHandlingConfigOutputTypeDef",
     "SuccessResponseHandlingConfigTypeDef",
+    "SAPODataSourcePropertiesOutputTypeDef",
     "SAPODataSourcePropertiesTypeDef",
+    "SalesforceSourcePropertiesOutputTypeDef",
     "SalesforceSourcePropertiesTypeDef",
+    "ScheduledTriggerPropertiesOutputTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
+    "ServiceNowSourcePropertiesOutputTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
+    "SingularSourcePropertiesOutputTypeDef",
     "SingularSourcePropertiesTypeDef",
+    "SlackSourcePropertiesOutputTypeDef",
     "SlackSourcePropertiesTypeDef",
+    "TrendmicroSourcePropertiesOutputTypeDef",
+    "VeevaSourcePropertiesOutputTypeDef",
+    "ZendeskSourcePropertiesOutputTypeDef",
     "TrendmicroSourcePropertiesTypeDef",
     "VeevaSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "StartFlowRequestRequestTypeDef",
     "StartFlowResponseTypeDef",
     "StopFlowRequestRequestTypeDef",
     "StopFlowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnregisterConnectorRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateConnectorProfileResponseTypeDef",
     "UpdateConnectorRegistrationResponseTypeDef",
     "UpdateFlowResponseTypeDef",
     "CustomAuthConfigTypeDef",
-    "CustomConnectorSourcePropertiesTypeDef",
+    "CustomConnectorSourcePropertiesOutputTypeDef",
     "ListConnectorsResponseTypeDef",
     "ListConnectorEntitiesResponseTypeDef",
     "ConnectorMetadataTypeDef",
     "GoogleAnalyticsConnectorProfileCredentialsTypeDef",
     "HoneycodeConnectorProfileCredentialsTypeDef",
     "MarketoConnectorProfileCredentialsTypeDef",
     "OAuth2CredentialsTypeDef",
     "OAuthCredentialsTypeDef",
     "PardotConnectorProfileCredentialsTypeDef",
     "SalesforceConnectorProfileCredentialsTypeDef",
     "SlackConnectorProfileCredentialsTypeDef",
     "ZendeskConnectorProfileCredentialsTypeDef",
+    "TaskOutputTypeDef",
     "TaskTypeDef",
+    "ConnectorProvisioningConfigOutputTypeDef",
     "ConnectorProvisioningConfigTypeDef",
+    "CustomConnectorDestinationPropertiesOutputTypeDef",
+    "EventBridgeDestinationPropertiesOutputTypeDef",
+    "HoneycodeDestinationPropertiesOutputTypeDef",
+    "MarketoDestinationPropertiesOutputTypeDef",
+    "RedshiftDestinationPropertiesOutputTypeDef",
+    "SalesforceDestinationPropertiesOutputTypeDef",
+    "SnowflakeDestinationPropertiesOutputTypeDef",
+    "ZendeskDestinationPropertiesOutputTypeDef",
     "CustomConnectorDestinationPropertiesTypeDef",
     "EventBridgeDestinationPropertiesTypeDef",
     "HoneycodeDestinationPropertiesTypeDef",
     "MarketoDestinationPropertiesTypeDef",
     "RedshiftDestinationPropertiesTypeDef",
     "SalesforceDestinationPropertiesTypeDef",
     "SnowflakeDestinationPropertiesTypeDef",
     "ZendeskDestinationPropertiesTypeDef",
+    "CustomConnectorProfilePropertiesOutputTypeDef",
     "CustomConnectorProfilePropertiesTypeDef",
+    "CustomConnectorSourcePropertiesTypeDef",
     "FlowDefinitionTypeDef",
     "ExecutionResultTypeDef",
     "FieldTypeDetailsTypeDef",
+    "MetadataCatalogConfigOutputTypeDef",
     "MetadataCatalogConfigTypeDef",
     "MetadataCatalogDetailTypeDef",
     "OAuth2DefaultsTypeDef",
+    "SAPODataConnectorProfilePropertiesOutputTypeDef",
     "SAPODataConnectorProfilePropertiesTypeDef",
+    "S3OutputFormatConfigOutputTypeDef",
+    "UpsolverS3OutputFormatConfigOutputTypeDef",
     "S3OutputFormatConfigTypeDef",
     "UpsolverS3OutputFormatConfigTypeDef",
+    "S3SourcePropertiesOutputTypeDef",
     "S3SourcePropertiesTypeDef",
+    "SAPODataDestinationPropertiesOutputTypeDef",
     "SAPODataDestinationPropertiesTypeDef",
+    "TriggerPropertiesOutputTypeDef",
     "TriggerPropertiesTypeDef",
     "CustomConnectorProfileCredentialsTypeDef",
     "SAPODataConnectorProfileCredentialsTypeDef",
     "RegisterConnectorRequestRequestTypeDef",
     "UpdateConnectorRegistrationRequestRequestTypeDef",
     "ListFlowsResponseTypeDef",
     "SupportedFieldTypeDetailsTypeDef",
     "ExecutionRecordTypeDef",
     "AuthenticationConfigTypeDef",
+    "ConnectorProfilePropertiesOutputTypeDef",
     "ConnectorProfilePropertiesTypeDef",
+    "S3DestinationPropertiesOutputTypeDef",
+    "UpsolverDestinationPropertiesOutputTypeDef",
     "S3DestinationPropertiesTypeDef",
     "UpsolverDestinationPropertiesTypeDef",
+    "SourceConnectorPropertiesOutputTypeDef",
     "SourceConnectorPropertiesTypeDef",
+    "TriggerConfigOutputTypeDef",
     "TriggerConfigTypeDef",
     "ConnectorProfileCredentialsTypeDef",
     "ConnectorEntityFieldTypeDef",
     "DescribeFlowExecutionRecordsResponseTypeDef",
     "ConnectorConfigurationTypeDef",
     "ConnectorProfileTypeDef",
+    "DestinationConnectorPropertiesOutputTypeDef",
     "DestinationConnectorPropertiesTypeDef",
+    "SourceFlowConfigOutputTypeDef",
     "SourceFlowConfigTypeDef",
     "ConnectorProfileConfigTypeDef",
     "DescribeConnectorEntityResponseTypeDef",
     "DescribeConnectorResponseTypeDef",
     "DescribeConnectorsResponseTypeDef",
     "DescribeConnectorProfilesResponseTypeDef",
+    "DestinationFlowConfigOutputTypeDef",
     "DestinationFlowConfigTypeDef",
     "CreateConnectorProfileRequestRequestTypeDef",
     "UpdateConnectorProfileRequestRequestTypeDef",
-    "CreateFlowRequestRequestTypeDef",
     "DescribeFlowResponseTypeDef",
+    "CreateFlowRequestRequestTypeDef",
     "UpdateFlowRequestRequestTypeDef",
 )
 
+AggregationConfigOutputTypeDef = TypedDict(
+    "AggregationConfigOutputTypeDef",
+    {
+        "aggregationType": AggregationTypeType,
+        "targetFileSize": int,
+    },
+    total=False,
+)
+
 AggregationConfigTypeDef = TypedDict(
     "AggregationConfigTypeDef",
     {
         "aggregationType": AggregationTypeType,
         "targetFileSize": int,
     },
     total=False,
@@ -256,14 +332,21 @@
     "AmplitudeConnectorProfileCredentialsTypeDef",
     {
         "apiKey": str,
         "secretKey": str,
     },
 )
 
+AmplitudeSourcePropertiesOutputTypeDef = TypedDict(
+    "AmplitudeSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 AmplitudeSourcePropertiesTypeDef = TypedDict(
     "AmplitudeSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -277,21 +360,19 @@
     "_OptionalApiKeyCredentialsTypeDef",
     {
         "apiSecretKey": str,
     },
     total=False,
 )
 
-
 class ApiKeyCredentialsTypeDef(
     _RequiredApiKeyCredentialsTypeDef, _OptionalApiKeyCredentialsTypeDef
 ):
     pass
 
-
 AuthParameterTypeDef = TypedDict(
     "AuthParameterTypeDef",
     {
         "key": str,
         "isRequired": bool,
         "label": str,
         "description": str,
@@ -319,22 +400,20 @@
     "_OptionalCancelFlowExecutionsRequestRequestTypeDef",
     {
         "executionIds": Sequence[str],
     },
     total=False,
 )
 
-
 class CancelFlowExecutionsRequestRequestTypeDef(
     _RequiredCancelFlowExecutionsRequestRequestTypeDef,
     _OptionalCancelFlowExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 CancelFlowExecutionsResponseTypeDef = TypedDict(
     "CancelFlowExecutionsResponseTypeDef",
     {
         "invalidExecutions": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -349,16 +428,16 @@
         "description": str,
         "scope": str,
         "connectorSuppliedValueOptions": List[str],
     },
     total=False,
 )
 
-DataTransferApiTypeDef = TypedDict(
-    "DataTransferApiTypeDef",
+DataTransferApiOutputTypeDef = TypedDict(
+    "DataTransferApiOutputTypeDef",
     {
         "Name": str,
         "Type": DataTransferApiTypeType,
     },
     total=False,
 )
 
@@ -415,19 +494,17 @@
     {
         "label": str,
         "hasNestedEntities": bool,
     },
     total=False,
 )
 
-
 class ConnectorEntityTypeDef(_RequiredConnectorEntityTypeDef, _OptionalConnectorEntityTypeDef):
     pass
 
-
 GoogleAnalyticsMetadataTypeDef = TypedDict(
     "GoogleAnalyticsMetadataTypeDef",
     {
         "oAuthScopes": List[str],
     },
     total=False,
 )
@@ -479,14 +556,38 @@
     {
         "authCode": str,
         "redirectUri": str,
     },
     total=False,
 )
 
+ConnectorOperatorOutputTypeDef = TypedDict(
+    "ConnectorOperatorOutputTypeDef",
+    {
+        "Amplitude": Literal["BETWEEN"],
+        "Datadog": DatadogConnectorOperatorType,
+        "Dynatrace": DynatraceConnectorOperatorType,
+        "GoogleAnalytics": GoogleAnalyticsConnectorOperatorType,
+        "InforNexus": InforNexusConnectorOperatorType,
+        "Marketo": MarketoConnectorOperatorType,
+        "S3": S3ConnectorOperatorType,
+        "Salesforce": SalesforceConnectorOperatorType,
+        "ServiceNow": ServiceNowConnectorOperatorType,
+        "Singular": SingularConnectorOperatorType,
+        "Slack": SlackConnectorOperatorType,
+        "Trendmicro": TrendmicroConnectorOperatorType,
+        "Veeva": VeevaConnectorOperatorType,
+        "Zendesk": ZendeskConnectorOperatorType,
+        "SAPOData": SAPODataConnectorOperatorType,
+        "CustomConnector": OperatorType,
+        "Pardot": PardotConnectorOperatorType,
+    },
+    total=False,
+)
+
 ConnectorOperatorTypeDef = TypedDict(
     "ConnectorOperatorTypeDef",
     {
         "Amplitude": Literal["BETWEEN"],
         "Datadog": DatadogConnectorOperatorType,
         "Dynatrace": DynatraceConnectorOperatorType,
         "GoogleAnalytics": GoogleAnalyticsConnectorOperatorType,
@@ -575,14 +676,142 @@
     "VeevaConnectorProfileCredentialsTypeDef",
     {
         "username": str,
         "password": str,
     },
 )
 
+DatadogConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "DatadogConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
+DynatraceConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "DynatraceConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
+InforNexusConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "InforNexusConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
+MarketoConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "MarketoConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
+PardotConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "PardotConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+        "isSandboxEnvironment": bool,
+        "businessUnitId": str,
+    },
+    total=False,
+)
+
+_RequiredRedshiftConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_RequiredRedshiftConnectorProfilePropertiesOutputTypeDef",
+    {
+        "bucketName": str,
+        "roleArn": str,
+    },
+)
+_OptionalRedshiftConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_OptionalRedshiftConnectorProfilePropertiesOutputTypeDef",
+    {
+        "databaseUrl": str,
+        "bucketPrefix": str,
+        "dataApiRoleArn": str,
+        "isRedshiftServerless": bool,
+        "clusterIdentifier": str,
+        "workgroupName": str,
+        "databaseName": str,
+    },
+    total=False,
+)
+
+class RedshiftConnectorProfilePropertiesOutputTypeDef(
+    _RequiredRedshiftConnectorProfilePropertiesOutputTypeDef,
+    _OptionalRedshiftConnectorProfilePropertiesOutputTypeDef,
+):
+    pass
+
+SalesforceConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "SalesforceConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+        "isSandboxEnvironment": bool,
+        "usePrivateLinkForMetadataAndAuthorization": bool,
+    },
+    total=False,
+)
+
+ServiceNowConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "ServiceNowConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
+SlackConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "SlackConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
+_RequiredSnowflakeConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_RequiredSnowflakeConnectorProfilePropertiesOutputTypeDef",
+    {
+        "warehouse": str,
+        "stage": str,
+        "bucketName": str,
+    },
+)
+_OptionalSnowflakeConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_OptionalSnowflakeConnectorProfilePropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+        "privateLinkServiceName": str,
+        "accountName": str,
+        "region": str,
+    },
+    total=False,
+)
+
+class SnowflakeConnectorProfilePropertiesOutputTypeDef(
+    _RequiredSnowflakeConnectorProfilePropertiesOutputTypeDef,
+    _OptionalSnowflakeConnectorProfilePropertiesOutputTypeDef,
+):
+    pass
+
+VeevaConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "VeevaConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
+ZendeskConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "ZendeskConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
 DatadogConnectorProfilePropertiesTypeDef = TypedDict(
     "DatadogConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
     },
 )
 
@@ -634,22 +863,20 @@
         "clusterIdentifier": str,
         "workgroupName": str,
         "databaseName": str,
     },
     total=False,
 )
 
-
 class RedshiftConnectorProfilePropertiesTypeDef(
     _RequiredRedshiftConnectorProfilePropertiesTypeDef,
     _OptionalRedshiftConnectorProfilePropertiesTypeDef,
 ):
     pass
 
-
 SalesforceConnectorProfilePropertiesTypeDef = TypedDict(
     "SalesforceConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
         "isSandboxEnvironment": bool,
         "usePrivateLinkForMetadataAndAuthorization": bool,
     },
@@ -685,22 +912,20 @@
         "privateLinkServiceName": str,
         "accountName": str,
         "region": str,
     },
     total=False,
 )
 
-
 class SnowflakeConnectorProfilePropertiesTypeDef(
     _RequiredSnowflakeConnectorProfilePropertiesTypeDef,
     _OptionalSnowflakeConnectorProfilePropertiesTypeDef,
 ):
     pass
 
-
 VeevaConnectorProfilePropertiesTypeDef = TypedDict(
     "VeevaConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
     },
 )
 
@@ -717,14 +942,21 @@
         "status": PrivateConnectionProvisioningStatusType,
         "failureMessage": str,
         "failureCause": PrivateConnectionProvisioningFailureCauseType,
     },
     total=False,
 )
 
+LambdaConnectorProvisioningConfigOutputTypeDef = TypedDict(
+    "LambdaConnectorProvisioningConfigOutputTypeDef",
+    {
+        "lambdaArn": str,
+    },
+)
+
 LambdaConnectorProvisioningConfigTypeDef = TypedDict(
     "LambdaConnectorProvisioningConfigTypeDef",
     {
         "lambdaArn": str,
     },
 )
 
@@ -755,31 +987,59 @@
     "_OptionalCustomAuthCredentialsTypeDef",
     {
         "credentialsMap": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CustomAuthCredentialsTypeDef(
     _RequiredCustomAuthCredentialsTypeDef, _OptionalCustomAuthCredentialsTypeDef
 ):
     pass
 
+ErrorHandlingConfigOutputTypeDef = TypedDict(
+    "ErrorHandlingConfigOutputTypeDef",
+    {
+        "failOnFirstDestinationError": bool,
+        "bucketPrefix": str,
+        "bucketName": str,
+    },
+    total=False,
+)
 
 ErrorHandlingConfigTypeDef = TypedDict(
     "ErrorHandlingConfigTypeDef",
     {
         "failOnFirstDestinationError": bool,
         "bucketPrefix": str,
         "bucketName": str,
     },
     total=False,
 )
 
+_RequiredOAuth2PropertiesOutputTypeDef = TypedDict(
+    "_RequiredOAuth2PropertiesOutputTypeDef",
+    {
+        "tokenUrl": str,
+        "oAuth2GrantType": OAuth2GrantTypeType,
+    },
+)
+_OptionalOAuth2PropertiesOutputTypeDef = TypedDict(
+    "_OptionalOAuth2PropertiesOutputTypeDef",
+    {
+        "tokenUrlCustomProperties": Dict[str, str],
+    },
+    total=False,
+)
+
+class OAuth2PropertiesOutputTypeDef(
+    _RequiredOAuth2PropertiesOutputTypeDef, _OptionalOAuth2PropertiesOutputTypeDef
+):
+    pass
+
 _RequiredOAuth2PropertiesTypeDef = TypedDict(
     "_RequiredOAuth2PropertiesTypeDef",
     {
         "tokenUrl": str,
         "oAuth2GrantType": OAuth2GrantTypeType,
     },
 )
@@ -787,18 +1047,45 @@
     "_OptionalOAuth2PropertiesTypeDef",
     {
         "tokenUrlCustomProperties": Mapping[str, str],
     },
     total=False,
 )
 
-
 class OAuth2PropertiesTypeDef(_RequiredOAuth2PropertiesTypeDef, _OptionalOAuth2PropertiesTypeDef):
     pass
 
+DataTransferApiTypeDef = TypedDict(
+    "DataTransferApiTypeDef",
+    {
+        "Name": str,
+        "Type": DataTransferApiTypeType,
+    },
+    total=False,
+)
+
+_RequiredCustomerProfilesDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredCustomerProfilesDestinationPropertiesOutputTypeDef",
+    {
+        "domainName": str,
+    },
+)
+_OptionalCustomerProfilesDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalCustomerProfilesDestinationPropertiesOutputTypeDef",
+    {
+        "objectTypeName": str,
+    },
+    total=False,
+)
+
+class CustomerProfilesDestinationPropertiesOutputTypeDef(
+    _RequiredCustomerProfilesDestinationPropertiesOutputTypeDef,
+    _OptionalCustomerProfilesDestinationPropertiesOutputTypeDef,
+):
+    pass
 
 _RequiredCustomerProfilesDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomerProfilesDestinationPropertiesTypeDef",
     {
         "domainName": str,
     },
 )
@@ -806,21 +1093,26 @@
     "_OptionalCustomerProfilesDestinationPropertiesTypeDef",
     {
         "objectTypeName": str,
     },
     total=False,
 )
 
-
 class CustomerProfilesDestinationPropertiesTypeDef(
     _RequiredCustomerProfilesDestinationPropertiesTypeDef,
     _OptionalCustomerProfilesDestinationPropertiesTypeDef,
 ):
     pass
 
+DatadogSourcePropertiesOutputTypeDef = TypedDict(
+    "DatadogSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
 
 DatadogSourcePropertiesTypeDef = TypedDict(
     "DatadogSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
@@ -835,43 +1127,39 @@
     "_OptionalDeleteConnectorProfileRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
-
 class DeleteConnectorProfileRequestRequestTypeDef(
     _RequiredDeleteConnectorProfileRequestRequestTypeDef,
     _OptionalDeleteConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteFlowRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 _OptionalDeleteFlowRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFlowRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
-
 class DeleteFlowRequestRequestTypeDef(
     _RequiredDeleteFlowRequestRequestTypeDef, _OptionalDeleteFlowRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeConnectorEntityRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConnectorEntityRequestRequestTypeDef",
     {
         "connectorEntityName": str,
     },
 )
 _OptionalDescribeConnectorEntityRequestRequestTypeDef = TypedDict(
@@ -880,22 +1168,20 @@
         "connectorType": ConnectorTypeType,
         "connectorProfileName": str,
         "apiVersion": str,
     },
     total=False,
 )
 
-
 class DescribeConnectorEntityRequestRequestTypeDef(
     _RequiredDescribeConnectorEntityRequestRequestTypeDef,
     _OptionalDescribeConnectorEntityRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeConnectorProfilesRequestRequestTypeDef = TypedDict(
     "DescribeConnectorProfilesRequestRequestTypeDef",
     {
         "connectorProfileNames": Sequence[str],
         "connectorType": ConnectorTypeType,
         "connectorLabel": str,
         "maxResults": int,
@@ -914,21 +1200,19 @@
     "_OptionalDescribeConnectorRequestRequestTypeDef",
     {
         "connectorLabel": str,
     },
     total=False,
 )
 
-
 class DescribeConnectorRequestRequestTypeDef(
     _RequiredDescribeConnectorRequestRequestTypeDef, _OptionalDescribeConnectorRequestRequestTypeDef
 ):
     pass
 
-
 DescribeConnectorsRequestRequestTypeDef = TypedDict(
     "DescribeConnectorsRequestRequestTypeDef",
     {
         "connectorTypes": Sequence[ConnectorTypeType],
         "maxResults": int,
         "nextToken": str,
     },
@@ -946,22 +1230,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class DescribeFlowExecutionRecordsRequestRequestTypeDef(
     _RequiredDescribeFlowExecutionRecordsRequestRequestTypeDef,
     _OptionalDescribeFlowExecutionRecordsRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeFlowRequestRequestTypeDef = TypedDict(
     "DescribeFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 
@@ -971,14 +1253,21 @@
         "mostRecentExecutionMessage": str,
         "mostRecentExecutionTime": datetime,
         "mostRecentExecutionStatus": ExecutionStatusType,
     },
     total=False,
 )
 
+DynatraceSourcePropertiesOutputTypeDef = TypedDict(
+    "DynatraceSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 DynatraceSourcePropertiesTypeDef = TypedDict(
     "DynatraceSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -996,38 +1285,69 @@
     {
         "maximum": float,
         "minimum": float,
     },
     total=False,
 )
 
+GlueDataCatalogConfigOutputTypeDef = TypedDict(
+    "GlueDataCatalogConfigOutputTypeDef",
+    {
+        "roleArn": str,
+        "databaseName": str,
+        "tablePrefix": str,
+    },
+)
+
 GlueDataCatalogConfigTypeDef = TypedDict(
     "GlueDataCatalogConfigTypeDef",
     {
         "roleArn": str,
         "databaseName": str,
         "tablePrefix": str,
     },
 )
 
+GoogleAnalyticsSourcePropertiesOutputTypeDef = TypedDict(
+    "GoogleAnalyticsSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 GoogleAnalyticsSourcePropertiesTypeDef = TypedDict(
     "GoogleAnalyticsSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
+IncrementalPullConfigOutputTypeDef = TypedDict(
+    "IncrementalPullConfigOutputTypeDef",
+    {
+        "datetimeTypeFieldName": str,
+    },
+    total=False,
+)
+
 IncrementalPullConfigTypeDef = TypedDict(
     "IncrementalPullConfigTypeDef",
     {
         "datetimeTypeFieldName": str,
     },
     total=False,
 )
 
+InforNexusSourcePropertiesOutputTypeDef = TypedDict(
+    "InforNexusSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 InforNexusSourcePropertiesTypeDef = TypedDict(
     "InforNexusSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1073,14 +1393,21 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MarketoSourcePropertiesOutputTypeDef = TypedDict(
+    "MarketoSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1104,30 +1431,56 @@
         "isSensitiveField": bool,
         "connectorSuppliedValues": List[str],
         "type": OAuth2CustomPropTypeType,
     },
     total=False,
 )
 
+OAuthPropertiesOutputTypeDef = TypedDict(
+    "OAuthPropertiesOutputTypeDef",
+    {
+        "tokenUrl": str,
+        "authCodeUrl": str,
+        "oAuthScopes": List[str],
+    },
+)
+
 OAuthPropertiesTypeDef = TypedDict(
     "OAuthPropertiesTypeDef",
     {
         "tokenUrl": str,
         "authCodeUrl": str,
         "oAuthScopes": Sequence[str],
     },
 )
 
+PardotSourcePropertiesOutputTypeDef = TypedDict(
+    "PardotSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 PardotSourcePropertiesTypeDef = TypedDict(
     "PardotSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
+PrefixConfigOutputTypeDef = TypedDict(
+    "PrefixConfigOutputTypeDef",
+    {
+        "prefixType": PrefixTypeType,
+        "prefixFormat": PrefixFormatType,
+        "pathPrefixHierarchy": List[PathPrefixType],
+    },
+    total=False,
+)
+
 PrefixConfigTypeDef = TypedDict(
     "PrefixConfigTypeDef",
     {
         "prefixType": PrefixTypeType,
         "prefixFormat": PrefixFormatType,
         "pathPrefixHierarchy": Sequence[PathPrefixType],
     },
@@ -1161,39 +1514,86 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+S3InputFormatConfigOutputTypeDef = TypedDict(
+    "S3InputFormatConfigOutputTypeDef",
+    {
+        "s3InputFileType": S3InputFileTypeType,
+    },
+    total=False,
+)
+
 S3InputFormatConfigTypeDef = TypedDict(
     "S3InputFormatConfigTypeDef",
     {
         "s3InputFileType": S3InputFileTypeType,
     },
     total=False,
 )
 
+SuccessResponseHandlingConfigOutputTypeDef = TypedDict(
+    "SuccessResponseHandlingConfigOutputTypeDef",
+    {
+        "bucketPrefix": str,
+        "bucketName": str,
+    },
+    total=False,
+)
+
 SuccessResponseHandlingConfigTypeDef = TypedDict(
     "SuccessResponseHandlingConfigTypeDef",
     {
         "bucketPrefix": str,
         "bucketName": str,
     },
     total=False,
 )
 
+SAPODataSourcePropertiesOutputTypeDef = TypedDict(
+    "SAPODataSourcePropertiesOutputTypeDef",
+    {
+        "objectPath": str,
+    },
+    total=False,
+)
+
 SAPODataSourcePropertiesTypeDef = TypedDict(
     "SAPODataSourcePropertiesTypeDef",
     {
         "objectPath": str,
     },
     total=False,
 )
 
+_RequiredSalesforceSourcePropertiesOutputTypeDef = TypedDict(
+    "_RequiredSalesforceSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalSalesforceSourcePropertiesOutputTypeDef = TypedDict(
+    "_OptionalSalesforceSourcePropertiesOutputTypeDef",
+    {
+        "enableDynamicFieldUpdate": bool,
+        "includeDeletedRecords": bool,
+        "dataTransferApi": SalesforceDataTransferApiType,
+    },
+    total=False,
+)
+
+class SalesforceSourcePropertiesOutputTypeDef(
+    _RequiredSalesforceSourcePropertiesOutputTypeDef,
+    _OptionalSalesforceSourcePropertiesOutputTypeDef,
+):
+    pass
+
 _RequiredSalesforceSourcePropertiesTypeDef = TypedDict(
     "_RequiredSalesforceSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalSalesforceSourcePropertiesTypeDef = TypedDict(
@@ -1202,20 +1602,44 @@
         "enableDynamicFieldUpdate": bool,
         "includeDeletedRecords": bool,
         "dataTransferApi": SalesforceDataTransferApiType,
     },
     total=False,
 )
 
-
 class SalesforceSourcePropertiesTypeDef(
     _RequiredSalesforceSourcePropertiesTypeDef, _OptionalSalesforceSourcePropertiesTypeDef
 ):
     pass
 
+_RequiredScheduledTriggerPropertiesOutputTypeDef = TypedDict(
+    "_RequiredScheduledTriggerPropertiesOutputTypeDef",
+    {
+        "scheduleExpression": str,
+    },
+)
+_OptionalScheduledTriggerPropertiesOutputTypeDef = TypedDict(
+    "_OptionalScheduledTriggerPropertiesOutputTypeDef",
+    {
+        "dataPullMode": DataPullModeType,
+        "scheduleStartTime": datetime,
+        "scheduleEndTime": datetime,
+        "timezone": str,
+        "scheduleOffset": int,
+        "firstExecutionFrom": datetime,
+        "flowErrorDeactivationThreshold": int,
+    },
+    total=False,
+)
+
+class ScheduledTriggerPropertiesOutputTypeDef(
+    _RequiredScheduledTriggerPropertiesOutputTypeDef,
+    _OptionalScheduledTriggerPropertiesOutputTypeDef,
+):
+    pass
 
 _RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
     "_RequiredScheduledTriggerPropertiesTypeDef",
     {
         "scheduleExpression": str,
     },
 )
@@ -1229,42 +1653,97 @@
         "scheduleOffset": int,
         "firstExecutionFrom": Union[datetime, str],
         "flowErrorDeactivationThreshold": int,
     },
     total=False,
 )
 
-
 class ScheduledTriggerPropertiesTypeDef(
     _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
 ):
     pass
 
+ServiceNowSourcePropertiesOutputTypeDef = TypedDict(
+    "ServiceNowSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
 
 ServiceNowSourcePropertiesTypeDef = TypedDict(
     "ServiceNowSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
+SingularSourcePropertiesOutputTypeDef = TypedDict(
+    "SingularSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 SingularSourcePropertiesTypeDef = TypedDict(
     "SingularSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
+SlackSourcePropertiesOutputTypeDef = TypedDict(
+    "SlackSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 SlackSourcePropertiesTypeDef = TypedDict(
     "SlackSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
+TrendmicroSourcePropertiesOutputTypeDef = TypedDict(
+    "TrendmicroSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
+_RequiredVeevaSourcePropertiesOutputTypeDef = TypedDict(
+    "_RequiredVeevaSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalVeevaSourcePropertiesOutputTypeDef = TypedDict(
+    "_OptionalVeevaSourcePropertiesOutputTypeDef",
+    {
+        "documentType": str,
+        "includeSourceFiles": bool,
+        "includeRenditions": bool,
+        "includeAllVersions": bool,
+    },
+    total=False,
+)
+
+class VeevaSourcePropertiesOutputTypeDef(
+    _RequiredVeevaSourcePropertiesOutputTypeDef, _OptionalVeevaSourcePropertiesOutputTypeDef
+):
+    pass
+
+ZendeskSourcePropertiesOutputTypeDef = TypedDict(
+    "ZendeskSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 TrendmicroSourcePropertiesTypeDef = TypedDict(
     "TrendmicroSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1281,21 +1760,19 @@
         "includeSourceFiles": bool,
         "includeRenditions": bool,
         "includeAllVersions": bool,
     },
     total=False,
 )
 
-
 class VeevaSourcePropertiesTypeDef(
     _RequiredVeevaSourcePropertiesTypeDef, _OptionalVeevaSourcePropertiesTypeDef
 ):
     pass
 
-
 ZendeskSourcePropertiesTypeDef = TypedDict(
     "ZendeskSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1309,21 +1786,19 @@
     "_OptionalStartFlowRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class StartFlowRequestRequestTypeDef(
     _RequiredStartFlowRequestRequestTypeDef, _OptionalStartFlowRequestRequestTypeDef
 ):
     pass
 
-
 StartFlowResponseTypeDef = TypedDict(
     "StartFlowResponseTypeDef",
     {
         "flowArn": str,
         "flowStatus": FlowStatusType,
         "executionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1364,22 +1839,20 @@
     "_OptionalUnregisterConnectorRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
-
 class UnregisterConnectorRequestRequestTypeDef(
     _RequiredUnregisterConnectorRequestRequestTypeDef,
     _OptionalUnregisterConnectorRequestRequestTypeDef,
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1413,36 +1886,35 @@
     {
         "customAuthenticationType": str,
         "authParameters": List[AuthParameterTypeDef],
     },
     total=False,
 )
 
-_RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
-    "_RequiredCustomConnectorSourcePropertiesTypeDef",
+_RequiredCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
+    "_RequiredCustomConnectorSourcePropertiesOutputTypeDef",
     {
         "entityName": str,
     },
 )
-_OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
-    "_OptionalCustomConnectorSourcePropertiesTypeDef",
+_OptionalCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
+    "_OptionalCustomConnectorSourcePropertiesOutputTypeDef",
     {
-        "customProperties": Mapping[str, str],
-        "dataTransferApi": DataTransferApiTypeDef,
+        "customProperties": Dict[str, str],
+        "dataTransferApi": DataTransferApiOutputTypeDef,
     },
     total=False,
 )
 
-
-class CustomConnectorSourcePropertiesTypeDef(
-    _RequiredCustomConnectorSourcePropertiesTypeDef, _OptionalCustomConnectorSourcePropertiesTypeDef
+class CustomConnectorSourcePropertiesOutputTypeDef(
+    _RequiredCustomConnectorSourcePropertiesOutputTypeDef,
+    _OptionalCustomConnectorSourcePropertiesOutputTypeDef,
 ):
     pass
 
-
 ListConnectorsResponseTypeDef = TypedDict(
     "ListConnectorsResponseTypeDef",
     {
         "connectors": List[ConnectorDetailTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1499,22 +1971,20 @@
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
-
 class GoogleAnalyticsConnectorProfileCredentialsTypeDef(
     _RequiredGoogleAnalyticsConnectorProfileCredentialsTypeDef,
     _OptionalGoogleAnalyticsConnectorProfileCredentialsTypeDef,
 ):
     pass
 
-
 HoneycodeConnectorProfileCredentialsTypeDef = TypedDict(
     "HoneycodeConnectorProfileCredentialsTypeDef",
     {
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
@@ -1533,22 +2003,20 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
-
 class MarketoConnectorProfileCredentialsTypeDef(
     _RequiredMarketoConnectorProfileCredentialsTypeDef,
     _OptionalMarketoConnectorProfileCredentialsTypeDef,
 ):
     pass
 
-
 OAuth2CredentialsTypeDef = TypedDict(
     "OAuth2CredentialsTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
         "accessToken": str,
         "refreshToken": str,
@@ -1570,19 +2038,17 @@
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
-
 class OAuthCredentialsTypeDef(_RequiredOAuthCredentialsTypeDef, _OptionalOAuthCredentialsTypeDef):
     pass
 
-
 PardotConnectorProfileCredentialsTypeDef = TypedDict(
     "PardotConnectorProfileCredentialsTypeDef",
     {
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
         "clientCredentialsArn": str,
@@ -1615,22 +2081,20 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
-
 class SlackConnectorProfileCredentialsTypeDef(
     _RequiredSlackConnectorProfileCredentialsTypeDef,
     _OptionalSlackConnectorProfileCredentialsTypeDef,
 ):
     pass
 
-
 _RequiredZendeskConnectorProfileCredentialsTypeDef = TypedDict(
     "_RequiredZendeskConnectorProfileCredentialsTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
     },
 )
@@ -1639,21 +2103,39 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
-
 class ZendeskConnectorProfileCredentialsTypeDef(
     _RequiredZendeskConnectorProfileCredentialsTypeDef,
     _OptionalZendeskConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+_RequiredTaskOutputTypeDef = TypedDict(
+    "_RequiredTaskOutputTypeDef",
+    {
+        "sourceFields": List[str],
+        "taskType": TaskTypeType,
+    },
+)
+_OptionalTaskOutputTypeDef = TypedDict(
+    "_OptionalTaskOutputTypeDef",
+    {
+        "connectorOperator": ConnectorOperatorOutputTypeDef,
+        "destinationField": str,
+        "taskProperties": Dict[OperatorPropertiesKeysType, str],
+    },
+    total=False,
+)
+
+class TaskOutputTypeDef(_RequiredTaskOutputTypeDef, _OptionalTaskOutputTypeDef):
+    pass
 
 _RequiredTaskTypeDef = TypedDict(
     "_RequiredTaskTypeDef",
     {
         "sourceFields": Sequence[str],
         "taskType": TaskTypeType,
     },
@@ -1664,27 +2146,205 @@
         "connectorOperator": ConnectorOperatorTypeDef,
         "destinationField": str,
         "taskProperties": Mapping[OperatorPropertiesKeysType, str],
     },
     total=False,
 )
 
-
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
+ConnectorProvisioningConfigOutputTypeDef = TypedDict(
+    "ConnectorProvisioningConfigOutputTypeDef",
+    {
+        "lambda": LambdaConnectorProvisioningConfigOutputTypeDef,
+    },
+    total=False,
+)
 
 ConnectorProvisioningConfigTypeDef = TypedDict(
     "ConnectorProvisioningConfigTypeDef",
     {
         "lambda": LambdaConnectorProvisioningConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredCustomConnectorDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredCustomConnectorDestinationPropertiesOutputTypeDef",
+    {
+        "entityName": str,
+    },
+)
+_OptionalCustomConnectorDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalCustomConnectorDestinationPropertiesOutputTypeDef",
+    {
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+        "idFieldNames": List[str],
+        "customProperties": Dict[str, str],
+    },
+    total=False,
+)
+
+class CustomConnectorDestinationPropertiesOutputTypeDef(
+    _RequiredCustomConnectorDestinationPropertiesOutputTypeDef,
+    _OptionalCustomConnectorDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+_RequiredEventBridgeDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredEventBridgeDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalEventBridgeDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalEventBridgeDestinationPropertiesOutputTypeDef",
+    {
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class EventBridgeDestinationPropertiesOutputTypeDef(
+    _RequiredEventBridgeDestinationPropertiesOutputTypeDef,
+    _OptionalEventBridgeDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+_RequiredHoneycodeDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredHoneycodeDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalHoneycodeDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalHoneycodeDestinationPropertiesOutputTypeDef",
+    {
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class HoneycodeDestinationPropertiesOutputTypeDef(
+    _RequiredHoneycodeDestinationPropertiesOutputTypeDef,
+    _OptionalHoneycodeDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+_RequiredMarketoDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredMarketoDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalMarketoDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalMarketoDestinationPropertiesOutputTypeDef",
+    {
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class MarketoDestinationPropertiesOutputTypeDef(
+    _RequiredMarketoDestinationPropertiesOutputTypeDef,
+    _OptionalMarketoDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+_RequiredRedshiftDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredRedshiftDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+        "intermediateBucketName": str,
+    },
+)
+_OptionalRedshiftDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalRedshiftDestinationPropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class RedshiftDestinationPropertiesOutputTypeDef(
+    _RequiredRedshiftDestinationPropertiesOutputTypeDef,
+    _OptionalRedshiftDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+_RequiredSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredSalesforceDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalSalesforceDestinationPropertiesOutputTypeDef",
+    {
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+        "dataTransferApi": SalesforceDataTransferApiType,
+    },
+    total=False,
+)
+
+class SalesforceDestinationPropertiesOutputTypeDef(
+    _RequiredSalesforceDestinationPropertiesOutputTypeDef,
+    _OptionalSalesforceDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+_RequiredSnowflakeDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredSnowflakeDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+        "intermediateBucketName": str,
+    },
+)
+_OptionalSnowflakeDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalSnowflakeDestinationPropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class SnowflakeDestinationPropertiesOutputTypeDef(
+    _RequiredSnowflakeDestinationPropertiesOutputTypeDef,
+    _OptionalSnowflakeDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+_RequiredZendeskDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredZendeskDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalZendeskDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalZendeskDestinationPropertiesOutputTypeDef",
+    {
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+    },
+    total=False,
+)
+
+class ZendeskDestinationPropertiesOutputTypeDef(
+    _RequiredZendeskDestinationPropertiesOutputTypeDef,
+    _OptionalZendeskDestinationPropertiesOutputTypeDef,
+):
+    pass
+
 _RequiredCustomConnectorDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomConnectorDestinationPropertiesTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorDestinationPropertiesTypeDef = TypedDict(
@@ -1694,86 +2354,78 @@
         "writeOperationType": WriteOperationTypeType,
         "idFieldNames": Sequence[str],
         "customProperties": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CustomConnectorDestinationPropertiesTypeDef(
     _RequiredCustomConnectorDestinationPropertiesTypeDef,
     _OptionalCustomConnectorDestinationPropertiesTypeDef,
 ):
     pass
 
-
 _RequiredEventBridgeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredEventBridgeDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalEventBridgeDestinationPropertiesTypeDef = TypedDict(
     "_OptionalEventBridgeDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
-
 class EventBridgeDestinationPropertiesTypeDef(
     _RequiredEventBridgeDestinationPropertiesTypeDef,
     _OptionalEventBridgeDestinationPropertiesTypeDef,
 ):
     pass
 
-
 _RequiredHoneycodeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredHoneycodeDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalHoneycodeDestinationPropertiesTypeDef = TypedDict(
     "_OptionalHoneycodeDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
-
 class HoneycodeDestinationPropertiesTypeDef(
     _RequiredHoneycodeDestinationPropertiesTypeDef, _OptionalHoneycodeDestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredMarketoDestinationPropertiesTypeDef = TypedDict(
     "_RequiredMarketoDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalMarketoDestinationPropertiesTypeDef = TypedDict(
     "_OptionalMarketoDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
-
 class MarketoDestinationPropertiesTypeDef(
     _RequiredMarketoDestinationPropertiesTypeDef, _OptionalMarketoDestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredRedshiftDestinationPropertiesTypeDef = TypedDict(
     "_RequiredRedshiftDestinationPropertiesTypeDef",
     {
         "object": str,
         "intermediateBucketName": str,
     },
 )
@@ -1782,21 +2434,19 @@
     {
         "bucketPrefix": str,
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
-
 class RedshiftDestinationPropertiesTypeDef(
     _RequiredRedshiftDestinationPropertiesTypeDef, _OptionalRedshiftDestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredSalesforceDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSalesforceDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalSalesforceDestinationPropertiesTypeDef = TypedDict(
@@ -1806,21 +2456,19 @@
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
         "dataTransferApi": SalesforceDataTransferApiType,
     },
     total=False,
 )
 
-
 class SalesforceDestinationPropertiesTypeDef(
     _RequiredSalesforceDestinationPropertiesTypeDef, _OptionalSalesforceDestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredSnowflakeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSnowflakeDestinationPropertiesTypeDef",
     {
         "object": str,
         "intermediateBucketName": str,
     },
 )
@@ -1829,21 +2477,19 @@
     {
         "bucketPrefix": str,
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
-
 class SnowflakeDestinationPropertiesTypeDef(
     _RequiredSnowflakeDestinationPropertiesTypeDef, _OptionalSnowflakeDestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredZendeskDestinationPropertiesTypeDef = TypedDict(
     "_RequiredZendeskDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalZendeskDestinationPropertiesTypeDef = TypedDict(
@@ -1852,30 +2498,57 @@
         "idFieldNames": Sequence[str],
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
     },
     total=False,
 )
 
-
 class ZendeskDestinationPropertiesTypeDef(
     _RequiredZendeskDestinationPropertiesTypeDef, _OptionalZendeskDestinationPropertiesTypeDef
 ):
     pass
 
+CustomConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "CustomConnectorProfilePropertiesOutputTypeDef",
+    {
+        "profileProperties": Dict[str, str],
+        "oAuth2Properties": OAuth2PropertiesOutputTypeDef,
+    },
+    total=False,
+)
 
 CustomConnectorProfilePropertiesTypeDef = TypedDict(
     "CustomConnectorProfilePropertiesTypeDef",
     {
         "profileProperties": Mapping[str, str],
         "oAuth2Properties": OAuth2PropertiesTypeDef,
     },
     total=False,
 )
 
+_RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
+    "_RequiredCustomConnectorSourcePropertiesTypeDef",
+    {
+        "entityName": str,
+    },
+)
+_OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
+    "_OptionalCustomConnectorSourcePropertiesTypeDef",
+    {
+        "customProperties": Mapping[str, str],
+        "dataTransferApi": DataTransferApiTypeDef,
+    },
+    total=False,
+)
+
+class CustomConnectorSourcePropertiesTypeDef(
+    _RequiredCustomConnectorSourcePropertiesTypeDef, _OptionalCustomConnectorSourcePropertiesTypeDef
+):
+    pass
+
 FlowDefinitionTypeDef = TypedDict(
     "FlowDefinitionTypeDef",
     {
         "flowArn": str,
         "description": str,
         "flowName": str,
         "flowStatus": FlowStatusType,
@@ -1920,18 +2593,24 @@
         "supportedDateFormat": str,
         "fieldValueRange": RangeTypeDef,
         "fieldLengthRange": RangeTypeDef,
     },
     total=False,
 )
 
-
 class FieldTypeDetailsTypeDef(_RequiredFieldTypeDetailsTypeDef, _OptionalFieldTypeDetailsTypeDef):
     pass
 
+MetadataCatalogConfigOutputTypeDef = TypedDict(
+    "MetadataCatalogConfigOutputTypeDef",
+    {
+        "glueDataCatalog": GlueDataCatalogConfigOutputTypeDef,
+    },
+    total=False,
+)
 
 MetadataCatalogConfigTypeDef = TypedDict(
     "MetadataCatalogConfigTypeDef",
     {
         "glueDataCatalog": GlueDataCatalogConfigTypeDef,
     },
     total=False,
@@ -1956,14 +2635,40 @@
         "authCodeUrls": List[str],
         "oauth2GrantTypesSupported": List[OAuth2GrantTypeType],
         "oauth2CustomProperties": List[OAuth2CustomParameterTypeDef],
     },
     total=False,
 )
 
+_RequiredSAPODataConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_RequiredSAPODataConnectorProfilePropertiesOutputTypeDef",
+    {
+        "applicationHostUrl": str,
+        "applicationServicePath": str,
+        "portNumber": int,
+        "clientNumber": str,
+    },
+)
+_OptionalSAPODataConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_OptionalSAPODataConnectorProfilePropertiesOutputTypeDef",
+    {
+        "logonLanguage": str,
+        "privateLinkServiceName": str,
+        "oAuthProperties": OAuthPropertiesOutputTypeDef,
+        "disableSSO": bool,
+    },
+    total=False,
+)
+
+class SAPODataConnectorProfilePropertiesOutputTypeDef(
+    _RequiredSAPODataConnectorProfilePropertiesOutputTypeDef,
+    _OptionalSAPODataConnectorProfilePropertiesOutputTypeDef,
+):
+    pass
+
 _RequiredSAPODataConnectorProfilePropertiesTypeDef = TypedDict(
     "_RequiredSAPODataConnectorProfilePropertiesTypeDef",
     {
         "applicationHostUrl": str,
         "applicationServicePath": str,
         "portNumber": int,
         "clientNumber": str,
@@ -1976,21 +2681,51 @@
         "privateLinkServiceName": str,
         "oAuthProperties": OAuthPropertiesTypeDef,
         "disableSSO": bool,
     },
     total=False,
 )
 
-
 class SAPODataConnectorProfilePropertiesTypeDef(
     _RequiredSAPODataConnectorProfilePropertiesTypeDef,
     _OptionalSAPODataConnectorProfilePropertiesTypeDef,
 ):
     pass
 
+S3OutputFormatConfigOutputTypeDef = TypedDict(
+    "S3OutputFormatConfigOutputTypeDef",
+    {
+        "fileType": FileTypeType,
+        "prefixConfig": PrefixConfigOutputTypeDef,
+        "aggregationConfig": AggregationConfigOutputTypeDef,
+        "preserveSourceDataTyping": bool,
+    },
+    total=False,
+)
+
+_RequiredUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
+    "_RequiredUpsolverS3OutputFormatConfigOutputTypeDef",
+    {
+        "prefixConfig": PrefixConfigOutputTypeDef,
+    },
+)
+_OptionalUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
+    "_OptionalUpsolverS3OutputFormatConfigOutputTypeDef",
+    {
+        "fileType": FileTypeType,
+        "aggregationConfig": AggregationConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class UpsolverS3OutputFormatConfigOutputTypeDef(
+    _RequiredUpsolverS3OutputFormatConfigOutputTypeDef,
+    _OptionalUpsolverS3OutputFormatConfigOutputTypeDef,
+):
+    pass
 
 S3OutputFormatConfigTypeDef = TypedDict(
     "S3OutputFormatConfigTypeDef",
     {
         "fileType": FileTypeType,
         "prefixConfig": PrefixConfigTypeDef,
         "aggregationConfig": AggregationConfigTypeDef,
@@ -2010,20 +2745,38 @@
     {
         "fileType": FileTypeType,
         "aggregationConfig": AggregationConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpsolverS3OutputFormatConfigTypeDef(
     _RequiredUpsolverS3OutputFormatConfigTypeDef, _OptionalUpsolverS3OutputFormatConfigTypeDef
 ):
     pass
 
+_RequiredS3SourcePropertiesOutputTypeDef = TypedDict(
+    "_RequiredS3SourcePropertiesOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+_OptionalS3SourcePropertiesOutputTypeDef = TypedDict(
+    "_OptionalS3SourcePropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+        "s3InputFormatConfig": S3InputFormatConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class S3SourcePropertiesOutputTypeDef(
+    _RequiredS3SourcePropertiesOutputTypeDef, _OptionalS3SourcePropertiesOutputTypeDef
+):
+    pass
 
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "bucketName": str,
     },
 )
@@ -2032,20 +2785,41 @@
     {
         "bucketPrefix": str,
         "s3InputFormatConfig": S3InputFormatConfigTypeDef,
     },
     total=False,
 )
 
-
 class S3SourcePropertiesTypeDef(
     _RequiredS3SourcePropertiesTypeDef, _OptionalS3SourcePropertiesTypeDef
 ):
     pass
 
+_RequiredSAPODataDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredSAPODataDestinationPropertiesOutputTypeDef",
+    {
+        "objectPath": str,
+    },
+)
+_OptionalSAPODataDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalSAPODataDestinationPropertiesOutputTypeDef",
+    {
+        "successResponseHandlingConfig": SuccessResponseHandlingConfigOutputTypeDef,
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+    },
+    total=False,
+)
+
+class SAPODataDestinationPropertiesOutputTypeDef(
+    _RequiredSAPODataDestinationPropertiesOutputTypeDef,
+    _OptionalSAPODataDestinationPropertiesOutputTypeDef,
+):
+    pass
 
 _RequiredSAPODataDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSAPODataDestinationPropertiesTypeDef",
     {
         "objectPath": str,
     },
 )
@@ -2056,20 +2830,26 @@
         "idFieldNames": Sequence[str],
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
     },
     total=False,
 )
 
-
 class SAPODataDestinationPropertiesTypeDef(
     _RequiredSAPODataDestinationPropertiesTypeDef, _OptionalSAPODataDestinationPropertiesTypeDef
 ):
     pass
 
+TriggerPropertiesOutputTypeDef = TypedDict(
+    "TriggerPropertiesOutputTypeDef",
+    {
+        "Scheduled": ScheduledTriggerPropertiesOutputTypeDef,
+    },
+    total=False,
+)
 
 TriggerPropertiesTypeDef = TypedDict(
     "TriggerPropertiesTypeDef",
     {
         "Scheduled": ScheduledTriggerPropertiesTypeDef,
     },
     total=False,
@@ -2088,22 +2868,20 @@
         "oauth2": OAuth2CredentialsTypeDef,
         "apiKey": ApiKeyCredentialsTypeDef,
         "custom": CustomAuthCredentialsTypeDef,
     },
     total=False,
 )
 
-
 class CustomConnectorProfileCredentialsTypeDef(
     _RequiredCustomConnectorProfileCredentialsTypeDef,
     _OptionalCustomConnectorProfileCredentialsTypeDef,
 ):
     pass
 
-
 SAPODataConnectorProfileCredentialsTypeDef = TypedDict(
     "SAPODataConnectorProfileCredentialsTypeDef",
     {
         "basicAuthCredentials": BasicAuthCredentialsTypeDef,
         "oAuthCredentials": OAuthCredentialsTypeDef,
     },
     total=False,
@@ -2133,22 +2911,20 @@
         "description": str,
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateConnectorRegistrationRequestRequestTypeDef(
     _RequiredUpdateConnectorRegistrationRequestRequestTypeDef,
     _OptionalUpdateConnectorRegistrationRequestRequestTypeDef,
 ):
     pass
 
-
 ListFlowsResponseTypeDef = TypedDict(
     "ListFlowsResponseTypeDef",
     {
         "flows": List[FlowDefinitionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2185,14 +2961,40 @@
         "isCustomAuthSupported": bool,
         "oAuth2Defaults": OAuth2DefaultsTypeDef,
         "customAuthConfigs": List[CustomAuthConfigTypeDef],
     },
     total=False,
 )
 
+ConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "ConnectorProfilePropertiesOutputTypeDef",
+    {
+        "Amplitude": Dict[str, Any],
+        "Datadog": DatadogConnectorProfilePropertiesOutputTypeDef,
+        "Dynatrace": DynatraceConnectorProfilePropertiesOutputTypeDef,
+        "GoogleAnalytics": Dict[str, Any],
+        "Honeycode": Dict[str, Any],
+        "InforNexus": InforNexusConnectorProfilePropertiesOutputTypeDef,
+        "Marketo": MarketoConnectorProfilePropertiesOutputTypeDef,
+        "Redshift": RedshiftConnectorProfilePropertiesOutputTypeDef,
+        "Salesforce": SalesforceConnectorProfilePropertiesOutputTypeDef,
+        "ServiceNow": ServiceNowConnectorProfilePropertiesOutputTypeDef,
+        "Singular": Dict[str, Any],
+        "Slack": SlackConnectorProfilePropertiesOutputTypeDef,
+        "Snowflake": SnowflakeConnectorProfilePropertiesOutputTypeDef,
+        "Trendmicro": Dict[str, Any],
+        "Veeva": VeevaConnectorProfilePropertiesOutputTypeDef,
+        "Zendesk": ZendeskConnectorProfilePropertiesOutputTypeDef,
+        "SAPOData": SAPODataConnectorProfilePropertiesOutputTypeDef,
+        "CustomConnector": CustomConnectorProfilePropertiesOutputTypeDef,
+        "Pardot": PardotConnectorProfilePropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 ConnectorProfilePropertiesTypeDef = TypedDict(
     "ConnectorProfilePropertiesTypeDef",
     {
         "Amplitude": Mapping[str, Any],
         "Datadog": DatadogConnectorProfilePropertiesTypeDef,
         "Dynatrace": DynatraceConnectorProfilePropertiesTypeDef,
         "GoogleAnalytics": Mapping[str, Any],
@@ -2211,14 +3013,55 @@
         "SAPOData": SAPODataConnectorProfilePropertiesTypeDef,
         "CustomConnector": CustomConnectorProfilePropertiesTypeDef,
         "Pardot": PardotConnectorProfilePropertiesTypeDef,
     },
     total=False,
 )
 
+_RequiredS3DestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredS3DestinationPropertiesOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+_OptionalS3DestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalS3DestinationPropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+        "s3OutputFormatConfig": S3OutputFormatConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class S3DestinationPropertiesOutputTypeDef(
+    _RequiredS3DestinationPropertiesOutputTypeDef, _OptionalS3DestinationPropertiesOutputTypeDef
+):
+    pass
+
+_RequiredUpsolverDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredUpsolverDestinationPropertiesOutputTypeDef",
+    {
+        "bucketName": str,
+        "s3OutputFormatConfig": UpsolverS3OutputFormatConfigOutputTypeDef,
+    },
+)
+_OptionalUpsolverDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalUpsolverDestinationPropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+    },
+    total=False,
+)
+
+class UpsolverDestinationPropertiesOutputTypeDef(
+    _RequiredUpsolverDestinationPropertiesOutputTypeDef,
+    _OptionalUpsolverDestinationPropertiesOutputTypeDef,
+):
+    pass
+
 _RequiredS3DestinationPropertiesTypeDef = TypedDict(
     "_RequiredS3DestinationPropertiesTypeDef",
     {
         "bucketName": str,
     },
 )
 _OptionalS3DestinationPropertiesTypeDef = TypedDict(
@@ -2226,21 +3069,19 @@
     {
         "bucketPrefix": str,
         "s3OutputFormatConfig": S3OutputFormatConfigTypeDef,
     },
     total=False,
 )
 
-
 class S3DestinationPropertiesTypeDef(
     _RequiredS3DestinationPropertiesTypeDef, _OptionalS3DestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredUpsolverDestinationPropertiesTypeDef = TypedDict(
     "_RequiredUpsolverDestinationPropertiesTypeDef",
     {
         "bucketName": str,
         "s3OutputFormatConfig": UpsolverS3OutputFormatConfigTypeDef,
     },
 )
@@ -2248,20 +3089,42 @@
     "_OptionalUpsolverDestinationPropertiesTypeDef",
     {
         "bucketPrefix": str,
     },
     total=False,
 )
 
-
 class UpsolverDestinationPropertiesTypeDef(
     _RequiredUpsolverDestinationPropertiesTypeDef, _OptionalUpsolverDestinationPropertiesTypeDef
 ):
     pass
 
+SourceConnectorPropertiesOutputTypeDef = TypedDict(
+    "SourceConnectorPropertiesOutputTypeDef",
+    {
+        "Amplitude": AmplitudeSourcePropertiesOutputTypeDef,
+        "Datadog": DatadogSourcePropertiesOutputTypeDef,
+        "Dynatrace": DynatraceSourcePropertiesOutputTypeDef,
+        "GoogleAnalytics": GoogleAnalyticsSourcePropertiesOutputTypeDef,
+        "InforNexus": InforNexusSourcePropertiesOutputTypeDef,
+        "Marketo": MarketoSourcePropertiesOutputTypeDef,
+        "S3": S3SourcePropertiesOutputTypeDef,
+        "Salesforce": SalesforceSourcePropertiesOutputTypeDef,
+        "ServiceNow": ServiceNowSourcePropertiesOutputTypeDef,
+        "Singular": SingularSourcePropertiesOutputTypeDef,
+        "Slack": SlackSourcePropertiesOutputTypeDef,
+        "Trendmicro": TrendmicroSourcePropertiesOutputTypeDef,
+        "Veeva": VeevaSourcePropertiesOutputTypeDef,
+        "Zendesk": ZendeskSourcePropertiesOutputTypeDef,
+        "SAPOData": SAPODataSourcePropertiesOutputTypeDef,
+        "CustomConnector": CustomConnectorSourcePropertiesOutputTypeDef,
+        "Pardot": PardotSourcePropertiesOutputTypeDef,
+    },
+    total=False,
+)
 
 SourceConnectorPropertiesTypeDef = TypedDict(
     "SourceConnectorPropertiesTypeDef",
     {
         "Amplitude": AmplitudeSourcePropertiesTypeDef,
         "Datadog": DatadogSourcePropertiesTypeDef,
         "Dynatrace": DynatraceSourcePropertiesTypeDef,
@@ -2279,33 +3142,50 @@
         "SAPOData": SAPODataSourcePropertiesTypeDef,
         "CustomConnector": CustomConnectorSourcePropertiesTypeDef,
         "Pardot": PardotSourcePropertiesTypeDef,
     },
     total=False,
 )
 
+_RequiredTriggerConfigOutputTypeDef = TypedDict(
+    "_RequiredTriggerConfigOutputTypeDef",
+    {
+        "triggerType": TriggerTypeType,
+    },
+)
+_OptionalTriggerConfigOutputTypeDef = TypedDict(
+    "_OptionalTriggerConfigOutputTypeDef",
+    {
+        "triggerProperties": TriggerPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
+class TriggerConfigOutputTypeDef(
+    _RequiredTriggerConfigOutputTypeDef, _OptionalTriggerConfigOutputTypeDef
+):
+    pass
+
 _RequiredTriggerConfigTypeDef = TypedDict(
     "_RequiredTriggerConfigTypeDef",
     {
         "triggerType": TriggerTypeType,
     },
 )
 _OptionalTriggerConfigTypeDef = TypedDict(
     "_OptionalTriggerConfigTypeDef",
     {
         "triggerProperties": TriggerPropertiesTypeDef,
     },
     total=False,
 )
 
-
 class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
     pass
 
-
 ConnectorProfileCredentialsTypeDef = TypedDict(
     "ConnectorProfileCredentialsTypeDef",
     {
         "Amplitude": AmplitudeConnectorProfileCredentialsTypeDef,
         "Datadog": DatadogConnectorProfileCredentialsTypeDef,
         "Dynatrace": DynatraceConnectorProfileCredentialsTypeDef,
         "GoogleAnalytics": GoogleAnalyticsConnectorProfileCredentialsTypeDef,
@@ -2347,21 +3227,19 @@
         "sourceProperties": SourceFieldPropertiesTypeDef,
         "destinationProperties": DestinationFieldPropertiesTypeDef,
         "customProperties": Dict[str, str],
     },
     total=False,
 )
 
-
 class ConnectorEntityFieldTypeDef(
     _RequiredConnectorEntityFieldTypeDef, _OptionalConnectorEntityFieldTypeDef
 ):
     pass
 
-
 DescribeFlowExecutionRecordsResponseTypeDef = TypedDict(
     "DescribeFlowExecutionRecordsResponseTypeDef",
     {
         "flowExecutions": List[ExecutionRecordTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2388,41 +3266,61 @@
         "connectorModes": List[str],
         "authenticationConfig": AuthenticationConfigTypeDef,
         "connectorRuntimeSettings": List[ConnectorRuntimeSettingTypeDef],
         "supportedApiVersions": List[str],
         "supportedOperators": List[OperatorsType],
         "supportedWriteOperations": List[WriteOperationTypeType],
         "connectorProvisioningType": Literal["LAMBDA"],
-        "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
+        "connectorProvisioningConfig": ConnectorProvisioningConfigOutputTypeDef,
         "logoURL": str,
         "registeredAt": datetime,
         "registeredBy": str,
         "supportedDataTransferTypes": List[SupportedDataTransferTypeType],
-        "supportedDataTransferApis": List[DataTransferApiTypeDef],
+        "supportedDataTransferApis": List[DataTransferApiOutputTypeDef],
     },
     total=False,
 )
 
 ConnectorProfileTypeDef = TypedDict(
     "ConnectorProfileTypeDef",
     {
         "connectorProfileArn": str,
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectorLabel": str,
         "connectionMode": ConnectionModeType,
         "credentialsArn": str,
-        "connectorProfileProperties": ConnectorProfilePropertiesTypeDef,
+        "connectorProfileProperties": ConnectorProfilePropertiesOutputTypeDef,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "privateConnectionProvisioningState": PrivateConnectionProvisioningStateTypeDef,
     },
     total=False,
 )
 
+DestinationConnectorPropertiesOutputTypeDef = TypedDict(
+    "DestinationConnectorPropertiesOutputTypeDef",
+    {
+        "Redshift": RedshiftDestinationPropertiesOutputTypeDef,
+        "S3": S3DestinationPropertiesOutputTypeDef,
+        "Salesforce": SalesforceDestinationPropertiesOutputTypeDef,
+        "Snowflake": SnowflakeDestinationPropertiesOutputTypeDef,
+        "EventBridge": EventBridgeDestinationPropertiesOutputTypeDef,
+        "LookoutMetrics": Dict[str, Any],
+        "Upsolver": UpsolverDestinationPropertiesOutputTypeDef,
+        "Honeycode": HoneycodeDestinationPropertiesOutputTypeDef,
+        "CustomerProfiles": CustomerProfilesDestinationPropertiesOutputTypeDef,
+        "Zendesk": ZendeskDestinationPropertiesOutputTypeDef,
+        "Marketo": MarketoDestinationPropertiesOutputTypeDef,
+        "CustomConnector": CustomConnectorDestinationPropertiesOutputTypeDef,
+        "SAPOData": SAPODataDestinationPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 DestinationConnectorPropertiesTypeDef = TypedDict(
     "DestinationConnectorPropertiesTypeDef",
     {
         "Redshift": RedshiftDestinationPropertiesTypeDef,
         "S3": S3DestinationPropertiesTypeDef,
         "Salesforce": SalesforceDestinationPropertiesTypeDef,
         "Snowflake": SnowflakeDestinationPropertiesTypeDef,
@@ -2435,14 +3333,36 @@
         "Marketo": MarketoDestinationPropertiesTypeDef,
         "CustomConnector": CustomConnectorDestinationPropertiesTypeDef,
         "SAPOData": SAPODataDestinationPropertiesTypeDef,
     },
     total=False,
 )
 
+_RequiredSourceFlowConfigOutputTypeDef = TypedDict(
+    "_RequiredSourceFlowConfigOutputTypeDef",
+    {
+        "connectorType": ConnectorTypeType,
+        "sourceConnectorProperties": SourceConnectorPropertiesOutputTypeDef,
+    },
+)
+_OptionalSourceFlowConfigOutputTypeDef = TypedDict(
+    "_OptionalSourceFlowConfigOutputTypeDef",
+    {
+        "apiVersion": str,
+        "connectorProfileName": str,
+        "incrementalPullConfig": IncrementalPullConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class SourceFlowConfigOutputTypeDef(
+    _RequiredSourceFlowConfigOutputTypeDef, _OptionalSourceFlowConfigOutputTypeDef
+):
+    pass
+
 _RequiredSourceFlowConfigTypeDef = TypedDict(
     "_RequiredSourceFlowConfigTypeDef",
     {
         "connectorType": ConnectorTypeType,
         "sourceConnectorProperties": SourceConnectorPropertiesTypeDef,
     },
 )
@@ -2452,40 +3372,36 @@
         "apiVersion": str,
         "connectorProfileName": str,
         "incrementalPullConfig": IncrementalPullConfigTypeDef,
     },
     total=False,
 )
 
-
 class SourceFlowConfigTypeDef(_RequiredSourceFlowConfigTypeDef, _OptionalSourceFlowConfigTypeDef):
     pass
 
-
 _RequiredConnectorProfileConfigTypeDef = TypedDict(
     "_RequiredConnectorProfileConfigTypeDef",
     {
         "connectorProfileProperties": ConnectorProfilePropertiesTypeDef,
     },
 )
 _OptionalConnectorProfileConfigTypeDef = TypedDict(
     "_OptionalConnectorProfileConfigTypeDef",
     {
         "connectorProfileCredentials": ConnectorProfileCredentialsTypeDef,
     },
     total=False,
 )
 
-
 class ConnectorProfileConfigTypeDef(
     _RequiredConnectorProfileConfigTypeDef, _OptionalConnectorProfileConfigTypeDef
 ):
     pass
 
-
 DescribeConnectorEntityResponseTypeDef = TypedDict(
     "DescribeConnectorEntityResponseTypeDef",
     {
         "connectorEntityFields": List[ConnectorEntityFieldTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2513,14 +3429,35 @@
     {
         "connectorProfileDetails": List[ConnectorProfileTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDestinationFlowConfigOutputTypeDef = TypedDict(
+    "_RequiredDestinationFlowConfigOutputTypeDef",
+    {
+        "connectorType": ConnectorTypeType,
+        "destinationConnectorProperties": DestinationConnectorPropertiesOutputTypeDef,
+    },
+)
+_OptionalDestinationFlowConfigOutputTypeDef = TypedDict(
+    "_OptionalDestinationFlowConfigOutputTypeDef",
+    {
+        "apiVersion": str,
+        "connectorProfileName": str,
+    },
+    total=False,
+)
+
+class DestinationFlowConfigOutputTypeDef(
+    _RequiredDestinationFlowConfigOutputTypeDef, _OptionalDestinationFlowConfigOutputTypeDef
+):
+    pass
+
 _RequiredDestinationFlowConfigTypeDef = TypedDict(
     "_RequiredDestinationFlowConfigTypeDef",
     {
         "connectorType": ConnectorTypeType,
         "destinationConnectorProperties": DestinationConnectorPropertiesTypeDef,
     },
 )
@@ -2529,21 +3466,19 @@
     {
         "apiVersion": str,
         "connectorProfileName": str,
     },
     total=False,
 )
 
-
 class DestinationFlowConfigTypeDef(
     _RequiredDestinationFlowConfigTypeDef, _OptionalDestinationFlowConfigTypeDef
 ):
     pass
 
-
 _RequiredCreateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
@@ -2555,22 +3490,20 @@
         "kmsArn": str,
         "connectorLabel": str,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateConnectorProfileRequestRequestTypeDef(
     _RequiredCreateConnectorProfileRequestRequestTypeDef,
     _OptionalCreateConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
     },
@@ -2579,21 +3512,45 @@
     "_OptionalUpdateConnectorProfileRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateConnectorProfileRequestRequestTypeDef(
     _RequiredUpdateConnectorProfileRequestRequestTypeDef,
     _OptionalUpdateConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
+DescribeFlowResponseTypeDef = TypedDict(
+    "DescribeFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "description": str,
+        "flowName": str,
+        "kmsArn": str,
+        "flowStatus": FlowStatusType,
+        "flowStatusMessage": str,
+        "sourceFlowConfig": SourceFlowConfigOutputTypeDef,
+        "destinationFlowConfigList": List[DestinationFlowConfigOutputTypeDef],
+        "lastRunExecutionDetails": ExecutionDetailsTypeDef,
+        "triggerConfig": TriggerConfigOutputTypeDef,
+        "tasks": List[TaskOutputTypeDef],
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "createdBy": str,
+        "lastUpdatedBy": str,
+        "tags": Dict[str, str],
+        "metadataCatalogConfig": MetadataCatalogConfigOutputTypeDef,
+        "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
+        "schemaVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredCreateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
@@ -2609,47 +3566,19 @@
         "tags": Mapping[str, str],
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateFlowRequestRequestTypeDef(
     _RequiredCreateFlowRequestRequestTypeDef, _OptionalCreateFlowRequestRequestTypeDef
 ):
     pass
 
-
-DescribeFlowResponseTypeDef = TypedDict(
-    "DescribeFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "description": str,
-        "flowName": str,
-        "kmsArn": str,
-        "flowStatus": FlowStatusType,
-        "flowStatusMessage": str,
-        "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": List[DestinationFlowConfigTypeDef],
-        "lastRunExecutionDetails": ExecutionDetailsTypeDef,
-        "triggerConfig": TriggerConfigTypeDef,
-        "tasks": List[TaskTypeDef],
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "createdBy": str,
-        "lastUpdatedBy": str,
-        "tags": Dict[str, str],
-        "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
-        "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
-        "schemaVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
         "destinationFlowConfigList": Sequence[DestinationFlowConfigTypeDef],
@@ -2662,12 +3591,11 @@
         "description": str,
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateFlowRequestRequestTypeDef(
     _RequiredUpdateFlowRequestRequestTypeDef, _OptionalUpdateFlowRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-appflow-1.28.0/mypy_boto3_appflow/type_defs.pyi` & `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow/type_defs.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for appflow service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_appflow.type_defs import AggregationConfigTypeDef
+    from mypy_boto3_appflow.type_defs import AggregationConfigOutputTypeDef
 
-    data: AggregationConfigTypeDef = {...}
+    data: AggregationConfigOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -64,188 +64,266 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AggregationConfigOutputTypeDef",
     "AggregationConfigTypeDef",
     "AmplitudeConnectorProfileCredentialsTypeDef",
+    "AmplitudeSourcePropertiesOutputTypeDef",
     "AmplitudeSourcePropertiesTypeDef",
     "ApiKeyCredentialsTypeDef",
     "AuthParameterTypeDef",
     "BasicAuthCredentialsTypeDef",
     "CancelFlowExecutionsRequestRequestTypeDef",
     "CancelFlowExecutionsResponseTypeDef",
     "ConnectorRuntimeSettingTypeDef",
-    "DataTransferApiTypeDef",
+    "DataTransferApiOutputTypeDef",
     "ConnectorDetailTypeDef",
     "DestinationFieldPropertiesTypeDef",
     "SourceFieldPropertiesTypeDef",
     "ConnectorEntityTypeDef",
     "GoogleAnalyticsMetadataTypeDef",
     "HoneycodeMetadataTypeDef",
     "SalesforceMetadataTypeDef",
     "SlackMetadataTypeDef",
     "SnowflakeMetadataTypeDef",
     "ZendeskMetadataTypeDef",
     "ConnectorOAuthRequestTypeDef",
+    "ConnectorOperatorOutputTypeDef",
     "ConnectorOperatorTypeDef",
     "DatadogConnectorProfileCredentialsTypeDef",
     "DynatraceConnectorProfileCredentialsTypeDef",
     "InforNexusConnectorProfileCredentialsTypeDef",
     "RedshiftConnectorProfileCredentialsTypeDef",
     "ServiceNowConnectorProfileCredentialsTypeDef",
     "SingularConnectorProfileCredentialsTypeDef",
     "SnowflakeConnectorProfileCredentialsTypeDef",
     "TrendmicroConnectorProfileCredentialsTypeDef",
     "VeevaConnectorProfileCredentialsTypeDef",
+    "DatadogConnectorProfilePropertiesOutputTypeDef",
+    "DynatraceConnectorProfilePropertiesOutputTypeDef",
+    "InforNexusConnectorProfilePropertiesOutputTypeDef",
+    "MarketoConnectorProfilePropertiesOutputTypeDef",
+    "PardotConnectorProfilePropertiesOutputTypeDef",
+    "RedshiftConnectorProfilePropertiesOutputTypeDef",
+    "SalesforceConnectorProfilePropertiesOutputTypeDef",
+    "ServiceNowConnectorProfilePropertiesOutputTypeDef",
+    "SlackConnectorProfilePropertiesOutputTypeDef",
+    "SnowflakeConnectorProfilePropertiesOutputTypeDef",
+    "VeevaConnectorProfilePropertiesOutputTypeDef",
+    "ZendeskConnectorProfilePropertiesOutputTypeDef",
     "DatadogConnectorProfilePropertiesTypeDef",
     "DynatraceConnectorProfilePropertiesTypeDef",
     "InforNexusConnectorProfilePropertiesTypeDef",
     "MarketoConnectorProfilePropertiesTypeDef",
     "PardotConnectorProfilePropertiesTypeDef",
     "RedshiftConnectorProfilePropertiesTypeDef",
     "SalesforceConnectorProfilePropertiesTypeDef",
     "ServiceNowConnectorProfilePropertiesTypeDef",
     "SlackConnectorProfilePropertiesTypeDef",
     "SnowflakeConnectorProfilePropertiesTypeDef",
     "VeevaConnectorProfilePropertiesTypeDef",
     "ZendeskConnectorProfilePropertiesTypeDef",
     "PrivateConnectionProvisioningStateTypeDef",
+    "LambdaConnectorProvisioningConfigOutputTypeDef",
     "LambdaConnectorProvisioningConfigTypeDef",
     "CreateConnectorProfileResponseTypeDef",
     "CreateFlowResponseTypeDef",
     "CustomAuthCredentialsTypeDef",
+    "ErrorHandlingConfigOutputTypeDef",
     "ErrorHandlingConfigTypeDef",
+    "OAuth2PropertiesOutputTypeDef",
     "OAuth2PropertiesTypeDef",
+    "DataTransferApiTypeDef",
+    "CustomerProfilesDestinationPropertiesOutputTypeDef",
     "CustomerProfilesDestinationPropertiesTypeDef",
+    "DatadogSourcePropertiesOutputTypeDef",
     "DatadogSourcePropertiesTypeDef",
     "DeleteConnectorProfileRequestRequestTypeDef",
     "DeleteFlowRequestRequestTypeDef",
     "DescribeConnectorEntityRequestRequestTypeDef",
     "DescribeConnectorProfilesRequestRequestTypeDef",
     "DescribeConnectorRequestRequestTypeDef",
     "DescribeConnectorsRequestRequestTypeDef",
     "DescribeFlowExecutionRecordsRequestRequestTypeDef",
     "DescribeFlowRequestRequestTypeDef",
     "ExecutionDetailsTypeDef",
+    "DynatraceSourcePropertiesOutputTypeDef",
     "DynatraceSourcePropertiesTypeDef",
     "ErrorInfoTypeDef",
     "RangeTypeDef",
+    "GlueDataCatalogConfigOutputTypeDef",
     "GlueDataCatalogConfigTypeDef",
+    "GoogleAnalyticsSourcePropertiesOutputTypeDef",
     "GoogleAnalyticsSourcePropertiesTypeDef",
+    "IncrementalPullConfigOutputTypeDef",
     "IncrementalPullConfigTypeDef",
+    "InforNexusSourcePropertiesOutputTypeDef",
     "InforNexusSourcePropertiesTypeDef",
     "ListConnectorEntitiesRequestRequestTypeDef",
     "ListConnectorsRequestRequestTypeDef",
     "ListFlowsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "MarketoSourcePropertiesOutputTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "RegistrationOutputTypeDef",
     "OAuth2CustomParameterTypeDef",
+    "OAuthPropertiesOutputTypeDef",
     "OAuthPropertiesTypeDef",
+    "PardotSourcePropertiesOutputTypeDef",
     "PardotSourcePropertiesTypeDef",
+    "PrefixConfigOutputTypeDef",
     "PrefixConfigTypeDef",
     "RegisterConnectorResponseTypeDef",
     "ResetConnectorMetadataCacheRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "S3InputFormatConfigOutputTypeDef",
     "S3InputFormatConfigTypeDef",
+    "SuccessResponseHandlingConfigOutputTypeDef",
     "SuccessResponseHandlingConfigTypeDef",
+    "SAPODataSourcePropertiesOutputTypeDef",
     "SAPODataSourcePropertiesTypeDef",
+    "SalesforceSourcePropertiesOutputTypeDef",
     "SalesforceSourcePropertiesTypeDef",
+    "ScheduledTriggerPropertiesOutputTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
+    "ServiceNowSourcePropertiesOutputTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
+    "SingularSourcePropertiesOutputTypeDef",
     "SingularSourcePropertiesTypeDef",
+    "SlackSourcePropertiesOutputTypeDef",
     "SlackSourcePropertiesTypeDef",
+    "TrendmicroSourcePropertiesOutputTypeDef",
+    "VeevaSourcePropertiesOutputTypeDef",
+    "ZendeskSourcePropertiesOutputTypeDef",
     "TrendmicroSourcePropertiesTypeDef",
     "VeevaSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "StartFlowRequestRequestTypeDef",
     "StartFlowResponseTypeDef",
     "StopFlowRequestRequestTypeDef",
     "StopFlowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnregisterConnectorRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateConnectorProfileResponseTypeDef",
     "UpdateConnectorRegistrationResponseTypeDef",
     "UpdateFlowResponseTypeDef",
     "CustomAuthConfigTypeDef",
-    "CustomConnectorSourcePropertiesTypeDef",
+    "CustomConnectorSourcePropertiesOutputTypeDef",
     "ListConnectorsResponseTypeDef",
     "ListConnectorEntitiesResponseTypeDef",
     "ConnectorMetadataTypeDef",
     "GoogleAnalyticsConnectorProfileCredentialsTypeDef",
     "HoneycodeConnectorProfileCredentialsTypeDef",
     "MarketoConnectorProfileCredentialsTypeDef",
     "OAuth2CredentialsTypeDef",
     "OAuthCredentialsTypeDef",
     "PardotConnectorProfileCredentialsTypeDef",
     "SalesforceConnectorProfileCredentialsTypeDef",
     "SlackConnectorProfileCredentialsTypeDef",
     "ZendeskConnectorProfileCredentialsTypeDef",
+    "TaskOutputTypeDef",
     "TaskTypeDef",
+    "ConnectorProvisioningConfigOutputTypeDef",
     "ConnectorProvisioningConfigTypeDef",
+    "CustomConnectorDestinationPropertiesOutputTypeDef",
+    "EventBridgeDestinationPropertiesOutputTypeDef",
+    "HoneycodeDestinationPropertiesOutputTypeDef",
+    "MarketoDestinationPropertiesOutputTypeDef",
+    "RedshiftDestinationPropertiesOutputTypeDef",
+    "SalesforceDestinationPropertiesOutputTypeDef",
+    "SnowflakeDestinationPropertiesOutputTypeDef",
+    "ZendeskDestinationPropertiesOutputTypeDef",
     "CustomConnectorDestinationPropertiesTypeDef",
     "EventBridgeDestinationPropertiesTypeDef",
     "HoneycodeDestinationPropertiesTypeDef",
     "MarketoDestinationPropertiesTypeDef",
     "RedshiftDestinationPropertiesTypeDef",
     "SalesforceDestinationPropertiesTypeDef",
     "SnowflakeDestinationPropertiesTypeDef",
     "ZendeskDestinationPropertiesTypeDef",
+    "CustomConnectorProfilePropertiesOutputTypeDef",
     "CustomConnectorProfilePropertiesTypeDef",
+    "CustomConnectorSourcePropertiesTypeDef",
     "FlowDefinitionTypeDef",
     "ExecutionResultTypeDef",
     "FieldTypeDetailsTypeDef",
+    "MetadataCatalogConfigOutputTypeDef",
     "MetadataCatalogConfigTypeDef",
     "MetadataCatalogDetailTypeDef",
     "OAuth2DefaultsTypeDef",
+    "SAPODataConnectorProfilePropertiesOutputTypeDef",
     "SAPODataConnectorProfilePropertiesTypeDef",
+    "S3OutputFormatConfigOutputTypeDef",
+    "UpsolverS3OutputFormatConfigOutputTypeDef",
     "S3OutputFormatConfigTypeDef",
     "UpsolverS3OutputFormatConfigTypeDef",
+    "S3SourcePropertiesOutputTypeDef",
     "S3SourcePropertiesTypeDef",
+    "SAPODataDestinationPropertiesOutputTypeDef",
     "SAPODataDestinationPropertiesTypeDef",
+    "TriggerPropertiesOutputTypeDef",
     "TriggerPropertiesTypeDef",
     "CustomConnectorProfileCredentialsTypeDef",
     "SAPODataConnectorProfileCredentialsTypeDef",
     "RegisterConnectorRequestRequestTypeDef",
     "UpdateConnectorRegistrationRequestRequestTypeDef",
     "ListFlowsResponseTypeDef",
     "SupportedFieldTypeDetailsTypeDef",
     "ExecutionRecordTypeDef",
     "AuthenticationConfigTypeDef",
+    "ConnectorProfilePropertiesOutputTypeDef",
     "ConnectorProfilePropertiesTypeDef",
+    "S3DestinationPropertiesOutputTypeDef",
+    "UpsolverDestinationPropertiesOutputTypeDef",
     "S3DestinationPropertiesTypeDef",
     "UpsolverDestinationPropertiesTypeDef",
+    "SourceConnectorPropertiesOutputTypeDef",
     "SourceConnectorPropertiesTypeDef",
+    "TriggerConfigOutputTypeDef",
     "TriggerConfigTypeDef",
     "ConnectorProfileCredentialsTypeDef",
     "ConnectorEntityFieldTypeDef",
     "DescribeFlowExecutionRecordsResponseTypeDef",
     "ConnectorConfigurationTypeDef",
     "ConnectorProfileTypeDef",
+    "DestinationConnectorPropertiesOutputTypeDef",
     "DestinationConnectorPropertiesTypeDef",
+    "SourceFlowConfigOutputTypeDef",
     "SourceFlowConfigTypeDef",
     "ConnectorProfileConfigTypeDef",
     "DescribeConnectorEntityResponseTypeDef",
     "DescribeConnectorResponseTypeDef",
     "DescribeConnectorsResponseTypeDef",
     "DescribeConnectorProfilesResponseTypeDef",
+    "DestinationFlowConfigOutputTypeDef",
     "DestinationFlowConfigTypeDef",
     "CreateConnectorProfileRequestRequestTypeDef",
     "UpdateConnectorProfileRequestRequestTypeDef",
-    "CreateFlowRequestRequestTypeDef",
     "DescribeFlowResponseTypeDef",
+    "CreateFlowRequestRequestTypeDef",
     "UpdateFlowRequestRequestTypeDef",
 )
 
+AggregationConfigOutputTypeDef = TypedDict(
+    "AggregationConfigOutputTypeDef",
+    {
+        "aggregationType": AggregationTypeType,
+        "targetFileSize": int,
+    },
+    total=False,
+)
+
 AggregationConfigTypeDef = TypedDict(
     "AggregationConfigTypeDef",
     {
         "aggregationType": AggregationTypeType,
         "targetFileSize": int,
     },
     total=False,
@@ -255,14 +333,21 @@
     "AmplitudeConnectorProfileCredentialsTypeDef",
     {
         "apiKey": str,
         "secretKey": str,
     },
 )
 
+AmplitudeSourcePropertiesOutputTypeDef = TypedDict(
+    "AmplitudeSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 AmplitudeSourcePropertiesTypeDef = TypedDict(
     "AmplitudeSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -276,19 +361,21 @@
     "_OptionalApiKeyCredentialsTypeDef",
     {
         "apiSecretKey": str,
     },
     total=False,
 )
 
+
 class ApiKeyCredentialsTypeDef(
     _RequiredApiKeyCredentialsTypeDef, _OptionalApiKeyCredentialsTypeDef
 ):
     pass
 
+
 AuthParameterTypeDef = TypedDict(
     "AuthParameterTypeDef",
     {
         "key": str,
         "isRequired": bool,
         "label": str,
         "description": str,
@@ -316,20 +403,22 @@
     "_OptionalCancelFlowExecutionsRequestRequestTypeDef",
     {
         "executionIds": Sequence[str],
     },
     total=False,
 )
 
+
 class CancelFlowExecutionsRequestRequestTypeDef(
     _RequiredCancelFlowExecutionsRequestRequestTypeDef,
     _OptionalCancelFlowExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 CancelFlowExecutionsResponseTypeDef = TypedDict(
     "CancelFlowExecutionsResponseTypeDef",
     {
         "invalidExecutions": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -344,16 +433,16 @@
         "description": str,
         "scope": str,
         "connectorSuppliedValueOptions": List[str],
     },
     total=False,
 )
 
-DataTransferApiTypeDef = TypedDict(
-    "DataTransferApiTypeDef",
+DataTransferApiOutputTypeDef = TypedDict(
+    "DataTransferApiOutputTypeDef",
     {
         "Name": str,
         "Type": DataTransferApiTypeType,
     },
     total=False,
 )
 
@@ -410,17 +499,19 @@
     {
         "label": str,
         "hasNestedEntities": bool,
     },
     total=False,
 )
 
+
 class ConnectorEntityTypeDef(_RequiredConnectorEntityTypeDef, _OptionalConnectorEntityTypeDef):
     pass
 
+
 GoogleAnalyticsMetadataTypeDef = TypedDict(
     "GoogleAnalyticsMetadataTypeDef",
     {
         "oAuthScopes": List[str],
     },
     total=False,
 )
@@ -472,14 +563,38 @@
     {
         "authCode": str,
         "redirectUri": str,
     },
     total=False,
 )
 
+ConnectorOperatorOutputTypeDef = TypedDict(
+    "ConnectorOperatorOutputTypeDef",
+    {
+        "Amplitude": Literal["BETWEEN"],
+        "Datadog": DatadogConnectorOperatorType,
+        "Dynatrace": DynatraceConnectorOperatorType,
+        "GoogleAnalytics": GoogleAnalyticsConnectorOperatorType,
+        "InforNexus": InforNexusConnectorOperatorType,
+        "Marketo": MarketoConnectorOperatorType,
+        "S3": S3ConnectorOperatorType,
+        "Salesforce": SalesforceConnectorOperatorType,
+        "ServiceNow": ServiceNowConnectorOperatorType,
+        "Singular": SingularConnectorOperatorType,
+        "Slack": SlackConnectorOperatorType,
+        "Trendmicro": TrendmicroConnectorOperatorType,
+        "Veeva": VeevaConnectorOperatorType,
+        "Zendesk": ZendeskConnectorOperatorType,
+        "SAPOData": SAPODataConnectorOperatorType,
+        "CustomConnector": OperatorType,
+        "Pardot": PardotConnectorOperatorType,
+    },
+    total=False,
+)
+
 ConnectorOperatorTypeDef = TypedDict(
     "ConnectorOperatorTypeDef",
     {
         "Amplitude": Literal["BETWEEN"],
         "Datadog": DatadogConnectorOperatorType,
         "Dynatrace": DynatraceConnectorOperatorType,
         "GoogleAnalytics": GoogleAnalyticsConnectorOperatorType,
@@ -568,14 +683,146 @@
     "VeevaConnectorProfileCredentialsTypeDef",
     {
         "username": str,
         "password": str,
     },
 )
 
+DatadogConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "DatadogConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
+DynatraceConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "DynatraceConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
+InforNexusConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "InforNexusConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
+MarketoConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "MarketoConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
+PardotConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "PardotConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+        "isSandboxEnvironment": bool,
+        "businessUnitId": str,
+    },
+    total=False,
+)
+
+_RequiredRedshiftConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_RequiredRedshiftConnectorProfilePropertiesOutputTypeDef",
+    {
+        "bucketName": str,
+        "roleArn": str,
+    },
+)
+_OptionalRedshiftConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_OptionalRedshiftConnectorProfilePropertiesOutputTypeDef",
+    {
+        "databaseUrl": str,
+        "bucketPrefix": str,
+        "dataApiRoleArn": str,
+        "isRedshiftServerless": bool,
+        "clusterIdentifier": str,
+        "workgroupName": str,
+        "databaseName": str,
+    },
+    total=False,
+)
+
+
+class RedshiftConnectorProfilePropertiesOutputTypeDef(
+    _RequiredRedshiftConnectorProfilePropertiesOutputTypeDef,
+    _OptionalRedshiftConnectorProfilePropertiesOutputTypeDef,
+):
+    pass
+
+
+SalesforceConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "SalesforceConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+        "isSandboxEnvironment": bool,
+        "usePrivateLinkForMetadataAndAuthorization": bool,
+    },
+    total=False,
+)
+
+ServiceNowConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "ServiceNowConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
+SlackConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "SlackConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
+_RequiredSnowflakeConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_RequiredSnowflakeConnectorProfilePropertiesOutputTypeDef",
+    {
+        "warehouse": str,
+        "stage": str,
+        "bucketName": str,
+    },
+)
+_OptionalSnowflakeConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_OptionalSnowflakeConnectorProfilePropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+        "privateLinkServiceName": str,
+        "accountName": str,
+        "region": str,
+    },
+    total=False,
+)
+
+
+class SnowflakeConnectorProfilePropertiesOutputTypeDef(
+    _RequiredSnowflakeConnectorProfilePropertiesOutputTypeDef,
+    _OptionalSnowflakeConnectorProfilePropertiesOutputTypeDef,
+):
+    pass
+
+
+VeevaConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "VeevaConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
+ZendeskConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "ZendeskConnectorProfilePropertiesOutputTypeDef",
+    {
+        "instanceUrl": str,
+    },
+)
+
 DatadogConnectorProfilePropertiesTypeDef = TypedDict(
     "DatadogConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
     },
 )
 
@@ -627,20 +874,22 @@
         "clusterIdentifier": str,
         "workgroupName": str,
         "databaseName": str,
     },
     total=False,
 )
 
+
 class RedshiftConnectorProfilePropertiesTypeDef(
     _RequiredRedshiftConnectorProfilePropertiesTypeDef,
     _OptionalRedshiftConnectorProfilePropertiesTypeDef,
 ):
     pass
 
+
 SalesforceConnectorProfilePropertiesTypeDef = TypedDict(
     "SalesforceConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
         "isSandboxEnvironment": bool,
         "usePrivateLinkForMetadataAndAuthorization": bool,
     },
@@ -676,20 +925,22 @@
         "privateLinkServiceName": str,
         "accountName": str,
         "region": str,
     },
     total=False,
 )
 
+
 class SnowflakeConnectorProfilePropertiesTypeDef(
     _RequiredSnowflakeConnectorProfilePropertiesTypeDef,
     _OptionalSnowflakeConnectorProfilePropertiesTypeDef,
 ):
     pass
 
+
 VeevaConnectorProfilePropertiesTypeDef = TypedDict(
     "VeevaConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
     },
 )
 
@@ -706,14 +957,21 @@
         "status": PrivateConnectionProvisioningStatusType,
         "failureMessage": str,
         "failureCause": PrivateConnectionProvisioningFailureCauseType,
     },
     total=False,
 )
 
+LambdaConnectorProvisioningConfigOutputTypeDef = TypedDict(
+    "LambdaConnectorProvisioningConfigOutputTypeDef",
+    {
+        "lambdaArn": str,
+    },
+)
+
 LambdaConnectorProvisioningConfigTypeDef = TypedDict(
     "LambdaConnectorProvisioningConfigTypeDef",
     {
         "lambdaArn": str,
     },
 )
 
@@ -744,29 +1002,63 @@
     "_OptionalCustomAuthCredentialsTypeDef",
     {
         "credentialsMap": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CustomAuthCredentialsTypeDef(
     _RequiredCustomAuthCredentialsTypeDef, _OptionalCustomAuthCredentialsTypeDef
 ):
     pass
 
+
+ErrorHandlingConfigOutputTypeDef = TypedDict(
+    "ErrorHandlingConfigOutputTypeDef",
+    {
+        "failOnFirstDestinationError": bool,
+        "bucketPrefix": str,
+        "bucketName": str,
+    },
+    total=False,
+)
+
 ErrorHandlingConfigTypeDef = TypedDict(
     "ErrorHandlingConfigTypeDef",
     {
         "failOnFirstDestinationError": bool,
         "bucketPrefix": str,
         "bucketName": str,
     },
     total=False,
 )
 
+_RequiredOAuth2PropertiesOutputTypeDef = TypedDict(
+    "_RequiredOAuth2PropertiesOutputTypeDef",
+    {
+        "tokenUrl": str,
+        "oAuth2GrantType": OAuth2GrantTypeType,
+    },
+)
+_OptionalOAuth2PropertiesOutputTypeDef = TypedDict(
+    "_OptionalOAuth2PropertiesOutputTypeDef",
+    {
+        "tokenUrlCustomProperties": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class OAuth2PropertiesOutputTypeDef(
+    _RequiredOAuth2PropertiesOutputTypeDef, _OptionalOAuth2PropertiesOutputTypeDef
+):
+    pass
+
+
 _RequiredOAuth2PropertiesTypeDef = TypedDict(
     "_RequiredOAuth2PropertiesTypeDef",
     {
         "tokenUrl": str,
         "oAuth2GrantType": OAuth2GrantTypeType,
     },
 )
@@ -774,37 +1066,79 @@
     "_OptionalOAuth2PropertiesTypeDef",
     {
         "tokenUrlCustomProperties": Mapping[str, str],
     },
     total=False,
 )
 
+
 class OAuth2PropertiesTypeDef(_RequiredOAuth2PropertiesTypeDef, _OptionalOAuth2PropertiesTypeDef):
     pass
 
+
+DataTransferApiTypeDef = TypedDict(
+    "DataTransferApiTypeDef",
+    {
+        "Name": str,
+        "Type": DataTransferApiTypeType,
+    },
+    total=False,
+)
+
+_RequiredCustomerProfilesDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredCustomerProfilesDestinationPropertiesOutputTypeDef",
+    {
+        "domainName": str,
+    },
+)
+_OptionalCustomerProfilesDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalCustomerProfilesDestinationPropertiesOutputTypeDef",
+    {
+        "objectTypeName": str,
+    },
+    total=False,
+)
+
+
+class CustomerProfilesDestinationPropertiesOutputTypeDef(
+    _RequiredCustomerProfilesDestinationPropertiesOutputTypeDef,
+    _OptionalCustomerProfilesDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredCustomerProfilesDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomerProfilesDestinationPropertiesTypeDef",
     {
         "domainName": str,
     },
 )
 _OptionalCustomerProfilesDestinationPropertiesTypeDef = TypedDict(
     "_OptionalCustomerProfilesDestinationPropertiesTypeDef",
     {
         "objectTypeName": str,
     },
     total=False,
 )
 
+
 class CustomerProfilesDestinationPropertiesTypeDef(
     _RequiredCustomerProfilesDestinationPropertiesTypeDef,
     _OptionalCustomerProfilesDestinationPropertiesTypeDef,
 ):
     pass
 
+
+DatadogSourcePropertiesOutputTypeDef = TypedDict(
+    "DatadogSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 DatadogSourcePropertiesTypeDef = TypedDict(
     "DatadogSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -818,39 +1152,43 @@
     "_OptionalDeleteConnectorProfileRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
+
 class DeleteConnectorProfileRequestRequestTypeDef(
     _RequiredDeleteConnectorProfileRequestRequestTypeDef,
     _OptionalDeleteConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteFlowRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 _OptionalDeleteFlowRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFlowRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
+
 class DeleteFlowRequestRequestTypeDef(
     _RequiredDeleteFlowRequestRequestTypeDef, _OptionalDeleteFlowRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeConnectorEntityRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConnectorEntityRequestRequestTypeDef",
     {
         "connectorEntityName": str,
     },
 )
 _OptionalDescribeConnectorEntityRequestRequestTypeDef = TypedDict(
@@ -859,20 +1197,22 @@
         "connectorType": ConnectorTypeType,
         "connectorProfileName": str,
         "apiVersion": str,
     },
     total=False,
 )
 
+
 class DescribeConnectorEntityRequestRequestTypeDef(
     _RequiredDescribeConnectorEntityRequestRequestTypeDef,
     _OptionalDescribeConnectorEntityRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeConnectorProfilesRequestRequestTypeDef = TypedDict(
     "DescribeConnectorProfilesRequestRequestTypeDef",
     {
         "connectorProfileNames": Sequence[str],
         "connectorType": ConnectorTypeType,
         "connectorLabel": str,
         "maxResults": int,
@@ -891,19 +1231,21 @@
     "_OptionalDescribeConnectorRequestRequestTypeDef",
     {
         "connectorLabel": str,
     },
     total=False,
 )
 
+
 class DescribeConnectorRequestRequestTypeDef(
     _RequiredDescribeConnectorRequestRequestTypeDef, _OptionalDescribeConnectorRequestRequestTypeDef
 ):
     pass
 
+
 DescribeConnectorsRequestRequestTypeDef = TypedDict(
     "DescribeConnectorsRequestRequestTypeDef",
     {
         "connectorTypes": Sequence[ConnectorTypeType],
         "maxResults": int,
         "nextToken": str,
     },
@@ -921,20 +1263,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class DescribeFlowExecutionRecordsRequestRequestTypeDef(
     _RequiredDescribeFlowExecutionRecordsRequestRequestTypeDef,
     _OptionalDescribeFlowExecutionRecordsRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeFlowRequestRequestTypeDef = TypedDict(
     "DescribeFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 
@@ -944,14 +1288,21 @@
         "mostRecentExecutionMessage": str,
         "mostRecentExecutionTime": datetime,
         "mostRecentExecutionStatus": ExecutionStatusType,
     },
     total=False,
 )
 
+DynatraceSourcePropertiesOutputTypeDef = TypedDict(
+    "DynatraceSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 DynatraceSourcePropertiesTypeDef = TypedDict(
     "DynatraceSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -969,38 +1320,69 @@
     {
         "maximum": float,
         "minimum": float,
     },
     total=False,
 )
 
+GlueDataCatalogConfigOutputTypeDef = TypedDict(
+    "GlueDataCatalogConfigOutputTypeDef",
+    {
+        "roleArn": str,
+        "databaseName": str,
+        "tablePrefix": str,
+    },
+)
+
 GlueDataCatalogConfigTypeDef = TypedDict(
     "GlueDataCatalogConfigTypeDef",
     {
         "roleArn": str,
         "databaseName": str,
         "tablePrefix": str,
     },
 )
 
+GoogleAnalyticsSourcePropertiesOutputTypeDef = TypedDict(
+    "GoogleAnalyticsSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 GoogleAnalyticsSourcePropertiesTypeDef = TypedDict(
     "GoogleAnalyticsSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
+IncrementalPullConfigOutputTypeDef = TypedDict(
+    "IncrementalPullConfigOutputTypeDef",
+    {
+        "datetimeTypeFieldName": str,
+    },
+    total=False,
+)
+
 IncrementalPullConfigTypeDef = TypedDict(
     "IncrementalPullConfigTypeDef",
     {
         "datetimeTypeFieldName": str,
     },
     total=False,
 )
 
+InforNexusSourcePropertiesOutputTypeDef = TypedDict(
+    "InforNexusSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 InforNexusSourcePropertiesTypeDef = TypedDict(
     "InforNexusSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1046,14 +1428,21 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MarketoSourcePropertiesOutputTypeDef = TypedDict(
+    "MarketoSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1077,30 +1466,56 @@
         "isSensitiveField": bool,
         "connectorSuppliedValues": List[str],
         "type": OAuth2CustomPropTypeType,
     },
     total=False,
 )
 
+OAuthPropertiesOutputTypeDef = TypedDict(
+    "OAuthPropertiesOutputTypeDef",
+    {
+        "tokenUrl": str,
+        "authCodeUrl": str,
+        "oAuthScopes": List[str],
+    },
+)
+
 OAuthPropertiesTypeDef = TypedDict(
     "OAuthPropertiesTypeDef",
     {
         "tokenUrl": str,
         "authCodeUrl": str,
         "oAuthScopes": Sequence[str],
     },
 )
 
+PardotSourcePropertiesOutputTypeDef = TypedDict(
+    "PardotSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 PardotSourcePropertiesTypeDef = TypedDict(
     "PardotSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
+PrefixConfigOutputTypeDef = TypedDict(
+    "PrefixConfigOutputTypeDef",
+    {
+        "prefixType": PrefixTypeType,
+        "prefixFormat": PrefixFormatType,
+        "pathPrefixHierarchy": List[PathPrefixType],
+    },
+    total=False,
+)
+
 PrefixConfigTypeDef = TypedDict(
     "PrefixConfigTypeDef",
     {
         "prefixType": PrefixTypeType,
         "prefixFormat": PrefixFormatType,
         "pathPrefixHierarchy": Sequence[PathPrefixType],
     },
@@ -1134,39 +1549,88 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+S3InputFormatConfigOutputTypeDef = TypedDict(
+    "S3InputFormatConfigOutputTypeDef",
+    {
+        "s3InputFileType": S3InputFileTypeType,
+    },
+    total=False,
+)
+
 S3InputFormatConfigTypeDef = TypedDict(
     "S3InputFormatConfigTypeDef",
     {
         "s3InputFileType": S3InputFileTypeType,
     },
     total=False,
 )
 
+SuccessResponseHandlingConfigOutputTypeDef = TypedDict(
+    "SuccessResponseHandlingConfigOutputTypeDef",
+    {
+        "bucketPrefix": str,
+        "bucketName": str,
+    },
+    total=False,
+)
+
 SuccessResponseHandlingConfigTypeDef = TypedDict(
     "SuccessResponseHandlingConfigTypeDef",
     {
         "bucketPrefix": str,
         "bucketName": str,
     },
     total=False,
 )
 
+SAPODataSourcePropertiesOutputTypeDef = TypedDict(
+    "SAPODataSourcePropertiesOutputTypeDef",
+    {
+        "objectPath": str,
+    },
+    total=False,
+)
+
 SAPODataSourcePropertiesTypeDef = TypedDict(
     "SAPODataSourcePropertiesTypeDef",
     {
         "objectPath": str,
     },
     total=False,
 )
 
+_RequiredSalesforceSourcePropertiesOutputTypeDef = TypedDict(
+    "_RequiredSalesforceSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalSalesforceSourcePropertiesOutputTypeDef = TypedDict(
+    "_OptionalSalesforceSourcePropertiesOutputTypeDef",
+    {
+        "enableDynamicFieldUpdate": bool,
+        "includeDeletedRecords": bool,
+        "dataTransferApi": SalesforceDataTransferApiType,
+    },
+    total=False,
+)
+
+
+class SalesforceSourcePropertiesOutputTypeDef(
+    _RequiredSalesforceSourcePropertiesOutputTypeDef,
+    _OptionalSalesforceSourcePropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredSalesforceSourcePropertiesTypeDef = TypedDict(
     "_RequiredSalesforceSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalSalesforceSourcePropertiesTypeDef = TypedDict(
@@ -1175,19 +1639,49 @@
         "enableDynamicFieldUpdate": bool,
         "includeDeletedRecords": bool,
         "dataTransferApi": SalesforceDataTransferApiType,
     },
     total=False,
 )
 
+
 class SalesforceSourcePropertiesTypeDef(
     _RequiredSalesforceSourcePropertiesTypeDef, _OptionalSalesforceSourcePropertiesTypeDef
 ):
     pass
 
+
+_RequiredScheduledTriggerPropertiesOutputTypeDef = TypedDict(
+    "_RequiredScheduledTriggerPropertiesOutputTypeDef",
+    {
+        "scheduleExpression": str,
+    },
+)
+_OptionalScheduledTriggerPropertiesOutputTypeDef = TypedDict(
+    "_OptionalScheduledTriggerPropertiesOutputTypeDef",
+    {
+        "dataPullMode": DataPullModeType,
+        "scheduleStartTime": datetime,
+        "scheduleEndTime": datetime,
+        "timezone": str,
+        "scheduleOffset": int,
+        "firstExecutionFrom": datetime,
+        "flowErrorDeactivationThreshold": int,
+    },
+    total=False,
+)
+
+
+class ScheduledTriggerPropertiesOutputTypeDef(
+    _RequiredScheduledTriggerPropertiesOutputTypeDef,
+    _OptionalScheduledTriggerPropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
     "_RequiredScheduledTriggerPropertiesTypeDef",
     {
         "scheduleExpression": str,
     },
 )
 _OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
@@ -1200,40 +1694,101 @@
         "scheduleOffset": int,
         "firstExecutionFrom": Union[datetime, str],
         "flowErrorDeactivationThreshold": int,
     },
     total=False,
 )
 
+
 class ScheduledTriggerPropertiesTypeDef(
     _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
 ):
     pass
 
+
+ServiceNowSourcePropertiesOutputTypeDef = TypedDict(
+    "ServiceNowSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 ServiceNowSourcePropertiesTypeDef = TypedDict(
     "ServiceNowSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
+SingularSourcePropertiesOutputTypeDef = TypedDict(
+    "SingularSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 SingularSourcePropertiesTypeDef = TypedDict(
     "SingularSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
+SlackSourcePropertiesOutputTypeDef = TypedDict(
+    "SlackSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 SlackSourcePropertiesTypeDef = TypedDict(
     "SlackSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
+TrendmicroSourcePropertiesOutputTypeDef = TypedDict(
+    "TrendmicroSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
+_RequiredVeevaSourcePropertiesOutputTypeDef = TypedDict(
+    "_RequiredVeevaSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalVeevaSourcePropertiesOutputTypeDef = TypedDict(
+    "_OptionalVeevaSourcePropertiesOutputTypeDef",
+    {
+        "documentType": str,
+        "includeSourceFiles": bool,
+        "includeRenditions": bool,
+        "includeAllVersions": bool,
+    },
+    total=False,
+)
+
+
+class VeevaSourcePropertiesOutputTypeDef(
+    _RequiredVeevaSourcePropertiesOutputTypeDef, _OptionalVeevaSourcePropertiesOutputTypeDef
+):
+    pass
+
+
+ZendeskSourcePropertiesOutputTypeDef = TypedDict(
+    "ZendeskSourcePropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+
 TrendmicroSourcePropertiesTypeDef = TypedDict(
     "TrendmicroSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1250,19 +1805,21 @@
         "includeSourceFiles": bool,
         "includeRenditions": bool,
         "includeAllVersions": bool,
     },
     total=False,
 )
 
+
 class VeevaSourcePropertiesTypeDef(
     _RequiredVeevaSourcePropertiesTypeDef, _OptionalVeevaSourcePropertiesTypeDef
 ):
     pass
 
+
 ZendeskSourcePropertiesTypeDef = TypedDict(
     "ZendeskSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1276,19 +1833,21 @@
     "_OptionalStartFlowRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class StartFlowRequestRequestTypeDef(
     _RequiredStartFlowRequestRequestTypeDef, _OptionalStartFlowRequestRequestTypeDef
 ):
     pass
 
+
 StartFlowResponseTypeDef = TypedDict(
     "StartFlowResponseTypeDef",
     {
         "flowArn": str,
         "flowStatus": FlowStatusType,
         "executionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1329,20 +1888,22 @@
     "_OptionalUnregisterConnectorRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
+
 class UnregisterConnectorRequestRequestTypeDef(
     _RequiredUnregisterConnectorRequestRequestTypeDef,
     _OptionalUnregisterConnectorRequestRequestTypeDef,
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1376,34 +1937,37 @@
     {
         "customAuthenticationType": str,
         "authParameters": List[AuthParameterTypeDef],
     },
     total=False,
 )
 
-_RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
-    "_RequiredCustomConnectorSourcePropertiesTypeDef",
+_RequiredCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
+    "_RequiredCustomConnectorSourcePropertiesOutputTypeDef",
     {
         "entityName": str,
     },
 )
-_OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
-    "_OptionalCustomConnectorSourcePropertiesTypeDef",
+_OptionalCustomConnectorSourcePropertiesOutputTypeDef = TypedDict(
+    "_OptionalCustomConnectorSourcePropertiesOutputTypeDef",
     {
-        "customProperties": Mapping[str, str],
-        "dataTransferApi": DataTransferApiTypeDef,
+        "customProperties": Dict[str, str],
+        "dataTransferApi": DataTransferApiOutputTypeDef,
     },
     total=False,
 )
 
-class CustomConnectorSourcePropertiesTypeDef(
-    _RequiredCustomConnectorSourcePropertiesTypeDef, _OptionalCustomConnectorSourcePropertiesTypeDef
+
+class CustomConnectorSourcePropertiesOutputTypeDef(
+    _RequiredCustomConnectorSourcePropertiesOutputTypeDef,
+    _OptionalCustomConnectorSourcePropertiesOutputTypeDef,
 ):
     pass
 
+
 ListConnectorsResponseTypeDef = TypedDict(
     "ListConnectorsResponseTypeDef",
     {
         "connectors": List[ConnectorDetailTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1460,20 +2024,22 @@
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
+
 class GoogleAnalyticsConnectorProfileCredentialsTypeDef(
     _RequiredGoogleAnalyticsConnectorProfileCredentialsTypeDef,
     _OptionalGoogleAnalyticsConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+
 HoneycodeConnectorProfileCredentialsTypeDef = TypedDict(
     "HoneycodeConnectorProfileCredentialsTypeDef",
     {
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
@@ -1492,20 +2058,22 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
+
 class MarketoConnectorProfileCredentialsTypeDef(
     _RequiredMarketoConnectorProfileCredentialsTypeDef,
     _OptionalMarketoConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+
 OAuth2CredentialsTypeDef = TypedDict(
     "OAuth2CredentialsTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
         "accessToken": str,
         "refreshToken": str,
@@ -1527,17 +2095,19 @@
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
+
 class OAuthCredentialsTypeDef(_RequiredOAuthCredentialsTypeDef, _OptionalOAuthCredentialsTypeDef):
     pass
 
+
 PardotConnectorProfileCredentialsTypeDef = TypedDict(
     "PardotConnectorProfileCredentialsTypeDef",
     {
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
         "clientCredentialsArn": str,
@@ -1570,20 +2140,22 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
+
 class SlackConnectorProfileCredentialsTypeDef(
     _RequiredSlackConnectorProfileCredentialsTypeDef,
     _OptionalSlackConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+
 _RequiredZendeskConnectorProfileCredentialsTypeDef = TypedDict(
     "_RequiredZendeskConnectorProfileCredentialsTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
     },
 )
@@ -1592,20 +2164,44 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
+
 class ZendeskConnectorProfileCredentialsTypeDef(
     _RequiredZendeskConnectorProfileCredentialsTypeDef,
     _OptionalZendeskConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+
+_RequiredTaskOutputTypeDef = TypedDict(
+    "_RequiredTaskOutputTypeDef",
+    {
+        "sourceFields": List[str],
+        "taskType": TaskTypeType,
+    },
+)
+_OptionalTaskOutputTypeDef = TypedDict(
+    "_OptionalTaskOutputTypeDef",
+    {
+        "connectorOperator": ConnectorOperatorOutputTypeDef,
+        "destinationField": str,
+        "taskProperties": Dict[OperatorPropertiesKeysType, str],
+    },
+    total=False,
+)
+
+
+class TaskOutputTypeDef(_RequiredTaskOutputTypeDef, _OptionalTaskOutputTypeDef):
+    pass
+
+
 _RequiredTaskTypeDef = TypedDict(
     "_RequiredTaskTypeDef",
     {
         "sourceFields": Sequence[str],
         "taskType": TaskTypeType,
     },
 )
@@ -1615,25 +2211,223 @@
         "connectorOperator": ConnectorOperatorTypeDef,
         "destinationField": str,
         "taskProperties": Mapping[OperatorPropertiesKeysType, str],
     },
     total=False,
 )
 
+
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
+
+ConnectorProvisioningConfigOutputTypeDef = TypedDict(
+    "ConnectorProvisioningConfigOutputTypeDef",
+    {
+        "lambda": LambdaConnectorProvisioningConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 ConnectorProvisioningConfigTypeDef = TypedDict(
     "ConnectorProvisioningConfigTypeDef",
     {
         "lambda": LambdaConnectorProvisioningConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredCustomConnectorDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredCustomConnectorDestinationPropertiesOutputTypeDef",
+    {
+        "entityName": str,
+    },
+)
+_OptionalCustomConnectorDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalCustomConnectorDestinationPropertiesOutputTypeDef",
+    {
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+        "idFieldNames": List[str],
+        "customProperties": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class CustomConnectorDestinationPropertiesOutputTypeDef(
+    _RequiredCustomConnectorDestinationPropertiesOutputTypeDef,
+    _OptionalCustomConnectorDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
+_RequiredEventBridgeDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredEventBridgeDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalEventBridgeDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalEventBridgeDestinationPropertiesOutputTypeDef",
+    {
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class EventBridgeDestinationPropertiesOutputTypeDef(
+    _RequiredEventBridgeDestinationPropertiesOutputTypeDef,
+    _OptionalEventBridgeDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
+_RequiredHoneycodeDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredHoneycodeDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalHoneycodeDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalHoneycodeDestinationPropertiesOutputTypeDef",
+    {
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class HoneycodeDestinationPropertiesOutputTypeDef(
+    _RequiredHoneycodeDestinationPropertiesOutputTypeDef,
+    _OptionalHoneycodeDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
+_RequiredMarketoDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredMarketoDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalMarketoDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalMarketoDestinationPropertiesOutputTypeDef",
+    {
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class MarketoDestinationPropertiesOutputTypeDef(
+    _RequiredMarketoDestinationPropertiesOutputTypeDef,
+    _OptionalMarketoDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
+_RequiredRedshiftDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredRedshiftDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+        "intermediateBucketName": str,
+    },
+)
+_OptionalRedshiftDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalRedshiftDestinationPropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class RedshiftDestinationPropertiesOutputTypeDef(
+    _RequiredRedshiftDestinationPropertiesOutputTypeDef,
+    _OptionalRedshiftDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
+_RequiredSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredSalesforceDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalSalesforceDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalSalesforceDestinationPropertiesOutputTypeDef",
+    {
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+        "dataTransferApi": SalesforceDataTransferApiType,
+    },
+    total=False,
+)
+
+
+class SalesforceDestinationPropertiesOutputTypeDef(
+    _RequiredSalesforceDestinationPropertiesOutputTypeDef,
+    _OptionalSalesforceDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
+_RequiredSnowflakeDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredSnowflakeDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+        "intermediateBucketName": str,
+    },
+)
+_OptionalSnowflakeDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalSnowflakeDestinationPropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class SnowflakeDestinationPropertiesOutputTypeDef(
+    _RequiredSnowflakeDestinationPropertiesOutputTypeDef,
+    _OptionalSnowflakeDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
+_RequiredZendeskDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredZendeskDestinationPropertiesOutputTypeDef",
+    {
+        "object": str,
+    },
+)
+_OptionalZendeskDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalZendeskDestinationPropertiesOutputTypeDef",
+    {
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+    },
+    total=False,
+)
+
+
+class ZendeskDestinationPropertiesOutputTypeDef(
+    _RequiredZendeskDestinationPropertiesOutputTypeDef,
+    _OptionalZendeskDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredCustomConnectorDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomConnectorDestinationPropertiesTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorDestinationPropertiesTypeDef = TypedDict(
@@ -1643,78 +2437,86 @@
         "writeOperationType": WriteOperationTypeType,
         "idFieldNames": Sequence[str],
         "customProperties": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CustomConnectorDestinationPropertiesTypeDef(
     _RequiredCustomConnectorDestinationPropertiesTypeDef,
     _OptionalCustomConnectorDestinationPropertiesTypeDef,
 ):
     pass
 
+
 _RequiredEventBridgeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredEventBridgeDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalEventBridgeDestinationPropertiesTypeDef = TypedDict(
     "_OptionalEventBridgeDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
+
 class EventBridgeDestinationPropertiesTypeDef(
     _RequiredEventBridgeDestinationPropertiesTypeDef,
     _OptionalEventBridgeDestinationPropertiesTypeDef,
 ):
     pass
 
+
 _RequiredHoneycodeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredHoneycodeDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalHoneycodeDestinationPropertiesTypeDef = TypedDict(
     "_OptionalHoneycodeDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
+
 class HoneycodeDestinationPropertiesTypeDef(
     _RequiredHoneycodeDestinationPropertiesTypeDef, _OptionalHoneycodeDestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredMarketoDestinationPropertiesTypeDef = TypedDict(
     "_RequiredMarketoDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalMarketoDestinationPropertiesTypeDef = TypedDict(
     "_OptionalMarketoDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
+
 class MarketoDestinationPropertiesTypeDef(
     _RequiredMarketoDestinationPropertiesTypeDef, _OptionalMarketoDestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredRedshiftDestinationPropertiesTypeDef = TypedDict(
     "_RequiredRedshiftDestinationPropertiesTypeDef",
     {
         "object": str,
         "intermediateBucketName": str,
     },
 )
@@ -1723,19 +2525,21 @@
     {
         "bucketPrefix": str,
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
+
 class RedshiftDestinationPropertiesTypeDef(
     _RequiredRedshiftDestinationPropertiesTypeDef, _OptionalRedshiftDestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredSalesforceDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSalesforceDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalSalesforceDestinationPropertiesTypeDef = TypedDict(
@@ -1745,19 +2549,21 @@
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
         "dataTransferApi": SalesforceDataTransferApiType,
     },
     total=False,
 )
 
+
 class SalesforceDestinationPropertiesTypeDef(
     _RequiredSalesforceDestinationPropertiesTypeDef, _OptionalSalesforceDestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredSnowflakeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSnowflakeDestinationPropertiesTypeDef",
     {
         "object": str,
         "intermediateBucketName": str,
     },
 )
@@ -1766,19 +2572,21 @@
     {
         "bucketPrefix": str,
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
+
 class SnowflakeDestinationPropertiesTypeDef(
     _RequiredSnowflakeDestinationPropertiesTypeDef, _OptionalSnowflakeDestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredZendeskDestinationPropertiesTypeDef = TypedDict(
     "_RequiredZendeskDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalZendeskDestinationPropertiesTypeDef = TypedDict(
@@ -1787,28 +2595,61 @@
         "idFieldNames": Sequence[str],
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
     },
     total=False,
 )
 
+
 class ZendeskDestinationPropertiesTypeDef(
     _RequiredZendeskDestinationPropertiesTypeDef, _OptionalZendeskDestinationPropertiesTypeDef
 ):
     pass
 
+
+CustomConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "CustomConnectorProfilePropertiesOutputTypeDef",
+    {
+        "profileProperties": Dict[str, str],
+        "oAuth2Properties": OAuth2PropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 CustomConnectorProfilePropertiesTypeDef = TypedDict(
     "CustomConnectorProfilePropertiesTypeDef",
     {
         "profileProperties": Mapping[str, str],
         "oAuth2Properties": OAuth2PropertiesTypeDef,
     },
     total=False,
 )
 
+_RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
+    "_RequiredCustomConnectorSourcePropertiesTypeDef",
+    {
+        "entityName": str,
+    },
+)
+_OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
+    "_OptionalCustomConnectorSourcePropertiesTypeDef",
+    {
+        "customProperties": Mapping[str, str],
+        "dataTransferApi": DataTransferApiTypeDef,
+    },
+    total=False,
+)
+
+
+class CustomConnectorSourcePropertiesTypeDef(
+    _RequiredCustomConnectorSourcePropertiesTypeDef, _OptionalCustomConnectorSourcePropertiesTypeDef
+):
+    pass
+
+
 FlowDefinitionTypeDef = TypedDict(
     "FlowDefinitionTypeDef",
     {
         "flowArn": str,
         "description": str,
         "flowName": str,
         "flowStatus": FlowStatusType,
@@ -1853,17 +2694,27 @@
         "supportedDateFormat": str,
         "fieldValueRange": RangeTypeDef,
         "fieldLengthRange": RangeTypeDef,
     },
     total=False,
 )
 
+
 class FieldTypeDetailsTypeDef(_RequiredFieldTypeDetailsTypeDef, _OptionalFieldTypeDetailsTypeDef):
     pass
 
+
+MetadataCatalogConfigOutputTypeDef = TypedDict(
+    "MetadataCatalogConfigOutputTypeDef",
+    {
+        "glueDataCatalog": GlueDataCatalogConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 MetadataCatalogConfigTypeDef = TypedDict(
     "MetadataCatalogConfigTypeDef",
     {
         "glueDataCatalog": GlueDataCatalogConfigTypeDef,
     },
     total=False,
 )
@@ -1887,14 +2738,42 @@
         "authCodeUrls": List[str],
         "oauth2GrantTypesSupported": List[OAuth2GrantTypeType],
         "oauth2CustomProperties": List[OAuth2CustomParameterTypeDef],
     },
     total=False,
 )
 
+_RequiredSAPODataConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_RequiredSAPODataConnectorProfilePropertiesOutputTypeDef",
+    {
+        "applicationHostUrl": str,
+        "applicationServicePath": str,
+        "portNumber": int,
+        "clientNumber": str,
+    },
+)
+_OptionalSAPODataConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "_OptionalSAPODataConnectorProfilePropertiesOutputTypeDef",
+    {
+        "logonLanguage": str,
+        "privateLinkServiceName": str,
+        "oAuthProperties": OAuthPropertiesOutputTypeDef,
+        "disableSSO": bool,
+    },
+    total=False,
+)
+
+
+class SAPODataConnectorProfilePropertiesOutputTypeDef(
+    _RequiredSAPODataConnectorProfilePropertiesOutputTypeDef,
+    _OptionalSAPODataConnectorProfilePropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredSAPODataConnectorProfilePropertiesTypeDef = TypedDict(
     "_RequiredSAPODataConnectorProfilePropertiesTypeDef",
     {
         "applicationHostUrl": str,
         "applicationServicePath": str,
         "portNumber": int,
         "clientNumber": str,
@@ -1907,20 +2786,56 @@
         "privateLinkServiceName": str,
         "oAuthProperties": OAuthPropertiesTypeDef,
         "disableSSO": bool,
     },
     total=False,
 )
 
+
 class SAPODataConnectorProfilePropertiesTypeDef(
     _RequiredSAPODataConnectorProfilePropertiesTypeDef,
     _OptionalSAPODataConnectorProfilePropertiesTypeDef,
 ):
     pass
 
+
+S3OutputFormatConfigOutputTypeDef = TypedDict(
+    "S3OutputFormatConfigOutputTypeDef",
+    {
+        "fileType": FileTypeType,
+        "prefixConfig": PrefixConfigOutputTypeDef,
+        "aggregationConfig": AggregationConfigOutputTypeDef,
+        "preserveSourceDataTyping": bool,
+    },
+    total=False,
+)
+
+_RequiredUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
+    "_RequiredUpsolverS3OutputFormatConfigOutputTypeDef",
+    {
+        "prefixConfig": PrefixConfigOutputTypeDef,
+    },
+)
+_OptionalUpsolverS3OutputFormatConfigOutputTypeDef = TypedDict(
+    "_OptionalUpsolverS3OutputFormatConfigOutputTypeDef",
+    {
+        "fileType": FileTypeType,
+        "aggregationConfig": AggregationConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class UpsolverS3OutputFormatConfigOutputTypeDef(
+    _RequiredUpsolverS3OutputFormatConfigOutputTypeDef,
+    _OptionalUpsolverS3OutputFormatConfigOutputTypeDef,
+):
+    pass
+
+
 S3OutputFormatConfigTypeDef = TypedDict(
     "S3OutputFormatConfigTypeDef",
     {
         "fileType": FileTypeType,
         "prefixConfig": PrefixConfigTypeDef,
         "aggregationConfig": AggregationConfigTypeDef,
         "preserveSourceDataTyping": bool,
@@ -1939,19 +2854,43 @@
     {
         "fileType": FileTypeType,
         "aggregationConfig": AggregationConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpsolverS3OutputFormatConfigTypeDef(
     _RequiredUpsolverS3OutputFormatConfigTypeDef, _OptionalUpsolverS3OutputFormatConfigTypeDef
 ):
     pass
 
+
+_RequiredS3SourcePropertiesOutputTypeDef = TypedDict(
+    "_RequiredS3SourcePropertiesOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+_OptionalS3SourcePropertiesOutputTypeDef = TypedDict(
+    "_OptionalS3SourcePropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+        "s3InputFormatConfig": S3InputFormatConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class S3SourcePropertiesOutputTypeDef(
+    _RequiredS3SourcePropertiesOutputTypeDef, _OptionalS3SourcePropertiesOutputTypeDef
+):
+    pass
+
+
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "bucketName": str,
     },
 )
 _OptionalS3SourcePropertiesTypeDef = TypedDict(
@@ -1959,19 +2898,46 @@
     {
         "bucketPrefix": str,
         "s3InputFormatConfig": S3InputFormatConfigTypeDef,
     },
     total=False,
 )
 
+
 class S3SourcePropertiesTypeDef(
     _RequiredS3SourcePropertiesTypeDef, _OptionalS3SourcePropertiesTypeDef
 ):
     pass
 
+
+_RequiredSAPODataDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredSAPODataDestinationPropertiesOutputTypeDef",
+    {
+        "objectPath": str,
+    },
+)
+_OptionalSAPODataDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalSAPODataDestinationPropertiesOutputTypeDef",
+    {
+        "successResponseHandlingConfig": SuccessResponseHandlingConfigOutputTypeDef,
+        "idFieldNames": List[str],
+        "errorHandlingConfig": ErrorHandlingConfigOutputTypeDef,
+        "writeOperationType": WriteOperationTypeType,
+    },
+    total=False,
+)
+
+
+class SAPODataDestinationPropertiesOutputTypeDef(
+    _RequiredSAPODataDestinationPropertiesOutputTypeDef,
+    _OptionalSAPODataDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredSAPODataDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSAPODataDestinationPropertiesTypeDef",
     {
         "objectPath": str,
     },
 )
 _OptionalSAPODataDestinationPropertiesTypeDef = TypedDict(
@@ -1981,19 +2947,29 @@
         "idFieldNames": Sequence[str],
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
     },
     total=False,
 )
 
+
 class SAPODataDestinationPropertiesTypeDef(
     _RequiredSAPODataDestinationPropertiesTypeDef, _OptionalSAPODataDestinationPropertiesTypeDef
 ):
     pass
 
+
+TriggerPropertiesOutputTypeDef = TypedDict(
+    "TriggerPropertiesOutputTypeDef",
+    {
+        "Scheduled": ScheduledTriggerPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 TriggerPropertiesTypeDef = TypedDict(
     "TriggerPropertiesTypeDef",
     {
         "Scheduled": ScheduledTriggerPropertiesTypeDef,
     },
     total=False,
 )
@@ -2011,20 +2987,22 @@
         "oauth2": OAuth2CredentialsTypeDef,
         "apiKey": ApiKeyCredentialsTypeDef,
         "custom": CustomAuthCredentialsTypeDef,
     },
     total=False,
 )
 
+
 class CustomConnectorProfileCredentialsTypeDef(
     _RequiredCustomConnectorProfileCredentialsTypeDef,
     _OptionalCustomConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+
 SAPODataConnectorProfileCredentialsTypeDef = TypedDict(
     "SAPODataConnectorProfileCredentialsTypeDef",
     {
         "basicAuthCredentials": BasicAuthCredentialsTypeDef,
         "oAuthCredentials": OAuthCredentialsTypeDef,
     },
     total=False,
@@ -2054,20 +3032,22 @@
         "description": str,
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateConnectorRegistrationRequestRequestTypeDef(
     _RequiredUpdateConnectorRegistrationRequestRequestTypeDef,
     _OptionalUpdateConnectorRegistrationRequestRequestTypeDef,
 ):
     pass
 
+
 ListFlowsResponseTypeDef = TypedDict(
     "ListFlowsResponseTypeDef",
     {
         "flows": List[FlowDefinitionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2104,14 +3084,40 @@
         "isCustomAuthSupported": bool,
         "oAuth2Defaults": OAuth2DefaultsTypeDef,
         "customAuthConfigs": List[CustomAuthConfigTypeDef],
     },
     total=False,
 )
 
+ConnectorProfilePropertiesOutputTypeDef = TypedDict(
+    "ConnectorProfilePropertiesOutputTypeDef",
+    {
+        "Amplitude": Dict[str, Any],
+        "Datadog": DatadogConnectorProfilePropertiesOutputTypeDef,
+        "Dynatrace": DynatraceConnectorProfilePropertiesOutputTypeDef,
+        "GoogleAnalytics": Dict[str, Any],
+        "Honeycode": Dict[str, Any],
+        "InforNexus": InforNexusConnectorProfilePropertiesOutputTypeDef,
+        "Marketo": MarketoConnectorProfilePropertiesOutputTypeDef,
+        "Redshift": RedshiftConnectorProfilePropertiesOutputTypeDef,
+        "Salesforce": SalesforceConnectorProfilePropertiesOutputTypeDef,
+        "ServiceNow": ServiceNowConnectorProfilePropertiesOutputTypeDef,
+        "Singular": Dict[str, Any],
+        "Slack": SlackConnectorProfilePropertiesOutputTypeDef,
+        "Snowflake": SnowflakeConnectorProfilePropertiesOutputTypeDef,
+        "Trendmicro": Dict[str, Any],
+        "Veeva": VeevaConnectorProfilePropertiesOutputTypeDef,
+        "Zendesk": ZendeskConnectorProfilePropertiesOutputTypeDef,
+        "SAPOData": SAPODataConnectorProfilePropertiesOutputTypeDef,
+        "CustomConnector": CustomConnectorProfilePropertiesOutputTypeDef,
+        "Pardot": PardotConnectorProfilePropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 ConnectorProfilePropertiesTypeDef = TypedDict(
     "ConnectorProfilePropertiesTypeDef",
     {
         "Amplitude": Mapping[str, Any],
         "Datadog": DatadogConnectorProfilePropertiesTypeDef,
         "Dynatrace": DynatraceConnectorProfilePropertiesTypeDef,
         "GoogleAnalytics": Mapping[str, Any],
@@ -2130,14 +3136,59 @@
         "SAPOData": SAPODataConnectorProfilePropertiesTypeDef,
         "CustomConnector": CustomConnectorProfilePropertiesTypeDef,
         "Pardot": PardotConnectorProfilePropertiesTypeDef,
     },
     total=False,
 )
 
+_RequiredS3DestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredS3DestinationPropertiesOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+_OptionalS3DestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalS3DestinationPropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+        "s3OutputFormatConfig": S3OutputFormatConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class S3DestinationPropertiesOutputTypeDef(
+    _RequiredS3DestinationPropertiesOutputTypeDef, _OptionalS3DestinationPropertiesOutputTypeDef
+):
+    pass
+
+
+_RequiredUpsolverDestinationPropertiesOutputTypeDef = TypedDict(
+    "_RequiredUpsolverDestinationPropertiesOutputTypeDef",
+    {
+        "bucketName": str,
+        "s3OutputFormatConfig": UpsolverS3OutputFormatConfigOutputTypeDef,
+    },
+)
+_OptionalUpsolverDestinationPropertiesOutputTypeDef = TypedDict(
+    "_OptionalUpsolverDestinationPropertiesOutputTypeDef",
+    {
+        "bucketPrefix": str,
+    },
+    total=False,
+)
+
+
+class UpsolverDestinationPropertiesOutputTypeDef(
+    _RequiredUpsolverDestinationPropertiesOutputTypeDef,
+    _OptionalUpsolverDestinationPropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredS3DestinationPropertiesTypeDef = TypedDict(
     "_RequiredS3DestinationPropertiesTypeDef",
     {
         "bucketName": str,
     },
 )
 _OptionalS3DestinationPropertiesTypeDef = TypedDict(
@@ -2145,19 +3196,21 @@
     {
         "bucketPrefix": str,
         "s3OutputFormatConfig": S3OutputFormatConfigTypeDef,
     },
     total=False,
 )
 
+
 class S3DestinationPropertiesTypeDef(
     _RequiredS3DestinationPropertiesTypeDef, _OptionalS3DestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredUpsolverDestinationPropertiesTypeDef = TypedDict(
     "_RequiredUpsolverDestinationPropertiesTypeDef",
     {
         "bucketName": str,
         "s3OutputFormatConfig": UpsolverS3OutputFormatConfigTypeDef,
     },
 )
@@ -2165,19 +3218,45 @@
     "_OptionalUpsolverDestinationPropertiesTypeDef",
     {
         "bucketPrefix": str,
     },
     total=False,
 )
 
+
 class UpsolverDestinationPropertiesTypeDef(
     _RequiredUpsolverDestinationPropertiesTypeDef, _OptionalUpsolverDestinationPropertiesTypeDef
 ):
     pass
 
+
+SourceConnectorPropertiesOutputTypeDef = TypedDict(
+    "SourceConnectorPropertiesOutputTypeDef",
+    {
+        "Amplitude": AmplitudeSourcePropertiesOutputTypeDef,
+        "Datadog": DatadogSourcePropertiesOutputTypeDef,
+        "Dynatrace": DynatraceSourcePropertiesOutputTypeDef,
+        "GoogleAnalytics": GoogleAnalyticsSourcePropertiesOutputTypeDef,
+        "InforNexus": InforNexusSourcePropertiesOutputTypeDef,
+        "Marketo": MarketoSourcePropertiesOutputTypeDef,
+        "S3": S3SourcePropertiesOutputTypeDef,
+        "Salesforce": SalesforceSourcePropertiesOutputTypeDef,
+        "ServiceNow": ServiceNowSourcePropertiesOutputTypeDef,
+        "Singular": SingularSourcePropertiesOutputTypeDef,
+        "Slack": SlackSourcePropertiesOutputTypeDef,
+        "Trendmicro": TrendmicroSourcePropertiesOutputTypeDef,
+        "Veeva": VeevaSourcePropertiesOutputTypeDef,
+        "Zendesk": ZendeskSourcePropertiesOutputTypeDef,
+        "SAPOData": SAPODataSourcePropertiesOutputTypeDef,
+        "CustomConnector": CustomConnectorSourcePropertiesOutputTypeDef,
+        "Pardot": PardotSourcePropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 SourceConnectorPropertiesTypeDef = TypedDict(
     "SourceConnectorPropertiesTypeDef",
     {
         "Amplitude": AmplitudeSourcePropertiesTypeDef,
         "Datadog": DatadogSourcePropertiesTypeDef,
         "Dynatrace": DynatraceSourcePropertiesTypeDef,
         "GoogleAnalytics": GoogleAnalyticsSourcePropertiesTypeDef,
@@ -2194,31 +3273,54 @@
         "SAPOData": SAPODataSourcePropertiesTypeDef,
         "CustomConnector": CustomConnectorSourcePropertiesTypeDef,
         "Pardot": PardotSourcePropertiesTypeDef,
     },
     total=False,
 )
 
+_RequiredTriggerConfigOutputTypeDef = TypedDict(
+    "_RequiredTriggerConfigOutputTypeDef",
+    {
+        "triggerType": TriggerTypeType,
+    },
+)
+_OptionalTriggerConfigOutputTypeDef = TypedDict(
+    "_OptionalTriggerConfigOutputTypeDef",
+    {
+        "triggerProperties": TriggerPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class TriggerConfigOutputTypeDef(
+    _RequiredTriggerConfigOutputTypeDef, _OptionalTriggerConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredTriggerConfigTypeDef = TypedDict(
     "_RequiredTriggerConfigTypeDef",
     {
         "triggerType": TriggerTypeType,
     },
 )
 _OptionalTriggerConfigTypeDef = TypedDict(
     "_OptionalTriggerConfigTypeDef",
     {
         "triggerProperties": TriggerPropertiesTypeDef,
     },
     total=False,
 )
 
+
 class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
     pass
 
+
 ConnectorProfileCredentialsTypeDef = TypedDict(
     "ConnectorProfileCredentialsTypeDef",
     {
         "Amplitude": AmplitudeConnectorProfileCredentialsTypeDef,
         "Datadog": DatadogConnectorProfileCredentialsTypeDef,
         "Dynatrace": DynatraceConnectorProfileCredentialsTypeDef,
         "GoogleAnalytics": GoogleAnalyticsConnectorProfileCredentialsTypeDef,
@@ -2260,19 +3362,21 @@
         "sourceProperties": SourceFieldPropertiesTypeDef,
         "destinationProperties": DestinationFieldPropertiesTypeDef,
         "customProperties": Dict[str, str],
     },
     total=False,
 )
 
+
 class ConnectorEntityFieldTypeDef(
     _RequiredConnectorEntityFieldTypeDef, _OptionalConnectorEntityFieldTypeDef
 ):
     pass
 
+
 DescribeFlowExecutionRecordsResponseTypeDef = TypedDict(
     "DescribeFlowExecutionRecordsResponseTypeDef",
     {
         "flowExecutions": List[ExecutionRecordTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2299,41 +3403,61 @@
         "connectorModes": List[str],
         "authenticationConfig": AuthenticationConfigTypeDef,
         "connectorRuntimeSettings": List[ConnectorRuntimeSettingTypeDef],
         "supportedApiVersions": List[str],
         "supportedOperators": List[OperatorsType],
         "supportedWriteOperations": List[WriteOperationTypeType],
         "connectorProvisioningType": Literal["LAMBDA"],
-        "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
+        "connectorProvisioningConfig": ConnectorProvisioningConfigOutputTypeDef,
         "logoURL": str,
         "registeredAt": datetime,
         "registeredBy": str,
         "supportedDataTransferTypes": List[SupportedDataTransferTypeType],
-        "supportedDataTransferApis": List[DataTransferApiTypeDef],
+        "supportedDataTransferApis": List[DataTransferApiOutputTypeDef],
     },
     total=False,
 )
 
 ConnectorProfileTypeDef = TypedDict(
     "ConnectorProfileTypeDef",
     {
         "connectorProfileArn": str,
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectorLabel": str,
         "connectionMode": ConnectionModeType,
         "credentialsArn": str,
-        "connectorProfileProperties": ConnectorProfilePropertiesTypeDef,
+        "connectorProfileProperties": ConnectorProfilePropertiesOutputTypeDef,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "privateConnectionProvisioningState": PrivateConnectionProvisioningStateTypeDef,
     },
     total=False,
 )
 
+DestinationConnectorPropertiesOutputTypeDef = TypedDict(
+    "DestinationConnectorPropertiesOutputTypeDef",
+    {
+        "Redshift": RedshiftDestinationPropertiesOutputTypeDef,
+        "S3": S3DestinationPropertiesOutputTypeDef,
+        "Salesforce": SalesforceDestinationPropertiesOutputTypeDef,
+        "Snowflake": SnowflakeDestinationPropertiesOutputTypeDef,
+        "EventBridge": EventBridgeDestinationPropertiesOutputTypeDef,
+        "LookoutMetrics": Dict[str, Any],
+        "Upsolver": UpsolverDestinationPropertiesOutputTypeDef,
+        "Honeycode": HoneycodeDestinationPropertiesOutputTypeDef,
+        "CustomerProfiles": CustomerProfilesDestinationPropertiesOutputTypeDef,
+        "Zendesk": ZendeskDestinationPropertiesOutputTypeDef,
+        "Marketo": MarketoDestinationPropertiesOutputTypeDef,
+        "CustomConnector": CustomConnectorDestinationPropertiesOutputTypeDef,
+        "SAPOData": SAPODataDestinationPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 DestinationConnectorPropertiesTypeDef = TypedDict(
     "DestinationConnectorPropertiesTypeDef",
     {
         "Redshift": RedshiftDestinationPropertiesTypeDef,
         "S3": S3DestinationPropertiesTypeDef,
         "Salesforce": SalesforceDestinationPropertiesTypeDef,
         "Snowflake": SnowflakeDestinationPropertiesTypeDef,
@@ -2346,14 +3470,38 @@
         "Marketo": MarketoDestinationPropertiesTypeDef,
         "CustomConnector": CustomConnectorDestinationPropertiesTypeDef,
         "SAPOData": SAPODataDestinationPropertiesTypeDef,
     },
     total=False,
 )
 
+_RequiredSourceFlowConfigOutputTypeDef = TypedDict(
+    "_RequiredSourceFlowConfigOutputTypeDef",
+    {
+        "connectorType": ConnectorTypeType,
+        "sourceConnectorProperties": SourceConnectorPropertiesOutputTypeDef,
+    },
+)
+_OptionalSourceFlowConfigOutputTypeDef = TypedDict(
+    "_OptionalSourceFlowConfigOutputTypeDef",
+    {
+        "apiVersion": str,
+        "connectorProfileName": str,
+        "incrementalPullConfig": IncrementalPullConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class SourceFlowConfigOutputTypeDef(
+    _RequiredSourceFlowConfigOutputTypeDef, _OptionalSourceFlowConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredSourceFlowConfigTypeDef = TypedDict(
     "_RequiredSourceFlowConfigTypeDef",
     {
         "connectorType": ConnectorTypeType,
         "sourceConnectorProperties": SourceConnectorPropertiesTypeDef,
     },
 )
@@ -2363,36 +3511,40 @@
         "apiVersion": str,
         "connectorProfileName": str,
         "incrementalPullConfig": IncrementalPullConfigTypeDef,
     },
     total=False,
 )
 
+
 class SourceFlowConfigTypeDef(_RequiredSourceFlowConfigTypeDef, _OptionalSourceFlowConfigTypeDef):
     pass
 
+
 _RequiredConnectorProfileConfigTypeDef = TypedDict(
     "_RequiredConnectorProfileConfigTypeDef",
     {
         "connectorProfileProperties": ConnectorProfilePropertiesTypeDef,
     },
 )
 _OptionalConnectorProfileConfigTypeDef = TypedDict(
     "_OptionalConnectorProfileConfigTypeDef",
     {
         "connectorProfileCredentials": ConnectorProfileCredentialsTypeDef,
     },
     total=False,
 )
 
+
 class ConnectorProfileConfigTypeDef(
     _RequiredConnectorProfileConfigTypeDef, _OptionalConnectorProfileConfigTypeDef
 ):
     pass
 
+
 DescribeConnectorEntityResponseTypeDef = TypedDict(
     "DescribeConnectorEntityResponseTypeDef",
     {
         "connectorEntityFields": List[ConnectorEntityFieldTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2420,14 +3572,37 @@
     {
         "connectorProfileDetails": List[ConnectorProfileTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDestinationFlowConfigOutputTypeDef = TypedDict(
+    "_RequiredDestinationFlowConfigOutputTypeDef",
+    {
+        "connectorType": ConnectorTypeType,
+        "destinationConnectorProperties": DestinationConnectorPropertiesOutputTypeDef,
+    },
+)
+_OptionalDestinationFlowConfigOutputTypeDef = TypedDict(
+    "_OptionalDestinationFlowConfigOutputTypeDef",
+    {
+        "apiVersion": str,
+        "connectorProfileName": str,
+    },
+    total=False,
+)
+
+
+class DestinationFlowConfigOutputTypeDef(
+    _RequiredDestinationFlowConfigOutputTypeDef, _OptionalDestinationFlowConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredDestinationFlowConfigTypeDef = TypedDict(
     "_RequiredDestinationFlowConfigTypeDef",
     {
         "connectorType": ConnectorTypeType,
         "destinationConnectorProperties": DestinationConnectorPropertiesTypeDef,
     },
 )
@@ -2436,19 +3611,21 @@
     {
         "apiVersion": str,
         "connectorProfileName": str,
     },
     total=False,
 )
 
+
 class DestinationFlowConfigTypeDef(
     _RequiredDestinationFlowConfigTypeDef, _OptionalDestinationFlowConfigTypeDef
 ):
     pass
 
+
 _RequiredCreateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
@@ -2460,20 +3637,22 @@
         "kmsArn": str,
         "connectorLabel": str,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateConnectorProfileRequestRequestTypeDef(
     _RequiredCreateConnectorProfileRequestRequestTypeDef,
     _OptionalCreateConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
     },
@@ -2482,20 +3661,48 @@
     "_OptionalUpdateConnectorProfileRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateConnectorProfileRequestRequestTypeDef(
     _RequiredUpdateConnectorProfileRequestRequestTypeDef,
     _OptionalUpdateConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
+
+DescribeFlowResponseTypeDef = TypedDict(
+    "DescribeFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "description": str,
+        "flowName": str,
+        "kmsArn": str,
+        "flowStatus": FlowStatusType,
+        "flowStatusMessage": str,
+        "sourceFlowConfig": SourceFlowConfigOutputTypeDef,
+        "destinationFlowConfigList": List[DestinationFlowConfigOutputTypeDef],
+        "lastRunExecutionDetails": ExecutionDetailsTypeDef,
+        "triggerConfig": TriggerConfigOutputTypeDef,
+        "tasks": List[TaskOutputTypeDef],
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "createdBy": str,
+        "lastUpdatedBy": str,
+        "tags": Dict[str, str],
+        "metadataCatalogConfig": MetadataCatalogConfigOutputTypeDef,
+        "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
+        "schemaVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
         "destinationFlowConfigList": Sequence[DestinationFlowConfigTypeDef],
@@ -2510,44 +3717,20 @@
         "tags": Mapping[str, str],
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateFlowRequestRequestTypeDef(
     _RequiredCreateFlowRequestRequestTypeDef, _OptionalCreateFlowRequestRequestTypeDef
 ):
     pass
 
-DescribeFlowResponseTypeDef = TypedDict(
-    "DescribeFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "description": str,
-        "flowName": str,
-        "kmsArn": str,
-        "flowStatus": FlowStatusType,
-        "flowStatusMessage": str,
-        "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": List[DestinationFlowConfigTypeDef],
-        "lastRunExecutionDetails": ExecutionDetailsTypeDef,
-        "triggerConfig": TriggerConfigTypeDef,
-        "tasks": List[TaskTypeDef],
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "createdBy": str,
-        "lastUpdatedBy": str,
-        "tags": Dict[str, str],
-        "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
-        "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
-        "schemaVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
@@ -2561,11 +3744,12 @@
         "description": str,
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateFlowRequestRequestTypeDef(
     _RequiredUpdateFlowRequestRequestTypeDef, _OptionalUpdateFlowRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-appflow-1.28.0/mypy_boto3_appflow.egg-info/PKG-INFO` & `mypy-boto3-appflow-1.28.12/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-appflow
-Version: 1.28.0
-Summary: Type annotations for boto3.Appflow 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appflow type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-appflow"></a>
 
 # mypy-boto3-appflow
 
 [![PyPI - mypy-boto3-appflow](https://img.shields.io/pypi/v/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appflow?color=blue)](https://pypistats.org/packages/mypy-boto3-appflow)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appflow)](https://pepy.tech/project/mypy-boto3-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Appflow 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[boto3.Appflow 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,189 +307,257 @@
 ### Typed dictionaries
 
 `mypy_boto3_appflow.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appflow.type_defs import (
+    AggregationConfigOutputTypeDef,
     AggregationConfigTypeDef,
     AmplitudeConnectorProfileCredentialsTypeDef,
+    AmplitudeSourcePropertiesOutputTypeDef,
     AmplitudeSourcePropertiesTypeDef,
     ApiKeyCredentialsTypeDef,
     AuthParameterTypeDef,
     BasicAuthCredentialsTypeDef,
     CancelFlowExecutionsRequestRequestTypeDef,
     CancelFlowExecutionsResponseTypeDef,
     ConnectorRuntimeSettingTypeDef,
-    DataTransferApiTypeDef,
+    DataTransferApiOutputTypeDef,
     ConnectorDetailTypeDef,
     DestinationFieldPropertiesTypeDef,
     SourceFieldPropertiesTypeDef,
     ConnectorEntityTypeDef,
     GoogleAnalyticsMetadataTypeDef,
     HoneycodeMetadataTypeDef,
     SalesforceMetadataTypeDef,
     SlackMetadataTypeDef,
     SnowflakeMetadataTypeDef,
     ZendeskMetadataTypeDef,
     ConnectorOAuthRequestTypeDef,
+    ConnectorOperatorOutputTypeDef,
     ConnectorOperatorTypeDef,
     DatadogConnectorProfileCredentialsTypeDef,
     DynatraceConnectorProfileCredentialsTypeDef,
     InforNexusConnectorProfileCredentialsTypeDef,
     RedshiftConnectorProfileCredentialsTypeDef,
     ServiceNowConnectorProfileCredentialsTypeDef,
     SingularConnectorProfileCredentialsTypeDef,
     SnowflakeConnectorProfileCredentialsTypeDef,
     TrendmicroConnectorProfileCredentialsTypeDef,
     VeevaConnectorProfileCredentialsTypeDef,
+    DatadogConnectorProfilePropertiesOutputTypeDef,
+    DynatraceConnectorProfilePropertiesOutputTypeDef,
+    InforNexusConnectorProfilePropertiesOutputTypeDef,
+    MarketoConnectorProfilePropertiesOutputTypeDef,
+    PardotConnectorProfilePropertiesOutputTypeDef,
+    RedshiftConnectorProfilePropertiesOutputTypeDef,
+    SalesforceConnectorProfilePropertiesOutputTypeDef,
+    ServiceNowConnectorProfilePropertiesOutputTypeDef,
+    SlackConnectorProfilePropertiesOutputTypeDef,
+    SnowflakeConnectorProfilePropertiesOutputTypeDef,
+    VeevaConnectorProfilePropertiesOutputTypeDef,
+    ZendeskConnectorProfilePropertiesOutputTypeDef,
     DatadogConnectorProfilePropertiesTypeDef,
     DynatraceConnectorProfilePropertiesTypeDef,
     InforNexusConnectorProfilePropertiesTypeDef,
     MarketoConnectorProfilePropertiesTypeDef,
     PardotConnectorProfilePropertiesTypeDef,
     RedshiftConnectorProfilePropertiesTypeDef,
     SalesforceConnectorProfilePropertiesTypeDef,
     ServiceNowConnectorProfilePropertiesTypeDef,
     SlackConnectorProfilePropertiesTypeDef,
     SnowflakeConnectorProfilePropertiesTypeDef,
     VeevaConnectorProfilePropertiesTypeDef,
     ZendeskConnectorProfilePropertiesTypeDef,
     PrivateConnectionProvisioningStateTypeDef,
+    LambdaConnectorProvisioningConfigOutputTypeDef,
     LambdaConnectorProvisioningConfigTypeDef,
     CreateConnectorProfileResponseTypeDef,
     CreateFlowResponseTypeDef,
     CustomAuthCredentialsTypeDef,
+    ErrorHandlingConfigOutputTypeDef,
     ErrorHandlingConfigTypeDef,
+    OAuth2PropertiesOutputTypeDef,
     OAuth2PropertiesTypeDef,
+    DataTransferApiTypeDef,
+    CustomerProfilesDestinationPropertiesOutputTypeDef,
     CustomerProfilesDestinationPropertiesTypeDef,
+    DatadogSourcePropertiesOutputTypeDef,
     DatadogSourcePropertiesTypeDef,
     DeleteConnectorProfileRequestRequestTypeDef,
     DeleteFlowRequestRequestTypeDef,
     DescribeConnectorEntityRequestRequestTypeDef,
     DescribeConnectorProfilesRequestRequestTypeDef,
     DescribeConnectorRequestRequestTypeDef,
     DescribeConnectorsRequestRequestTypeDef,
     DescribeFlowExecutionRecordsRequestRequestTypeDef,
     DescribeFlowRequestRequestTypeDef,
     ExecutionDetailsTypeDef,
+    DynatraceSourcePropertiesOutputTypeDef,
     DynatraceSourcePropertiesTypeDef,
     ErrorInfoTypeDef,
     RangeTypeDef,
+    GlueDataCatalogConfigOutputTypeDef,
     GlueDataCatalogConfigTypeDef,
+    GoogleAnalyticsSourcePropertiesOutputTypeDef,
     GoogleAnalyticsSourcePropertiesTypeDef,
+    IncrementalPullConfigOutputTypeDef,
     IncrementalPullConfigTypeDef,
+    InforNexusSourcePropertiesOutputTypeDef,
     InforNexusSourcePropertiesTypeDef,
     ListConnectorEntitiesRequestRequestTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListFlowsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    MarketoSourcePropertiesOutputTypeDef,
     MarketoSourcePropertiesTypeDef,
     RegistrationOutputTypeDef,
     OAuth2CustomParameterTypeDef,
+    OAuthPropertiesOutputTypeDef,
     OAuthPropertiesTypeDef,
+    PardotSourcePropertiesOutputTypeDef,
     PardotSourcePropertiesTypeDef,
+    PrefixConfigOutputTypeDef,
     PrefixConfigTypeDef,
     RegisterConnectorResponseTypeDef,
     ResetConnectorMetadataCacheRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    S3InputFormatConfigOutputTypeDef,
     S3InputFormatConfigTypeDef,
+    SuccessResponseHandlingConfigOutputTypeDef,
     SuccessResponseHandlingConfigTypeDef,
+    SAPODataSourcePropertiesOutputTypeDef,
     SAPODataSourcePropertiesTypeDef,
+    SalesforceSourcePropertiesOutputTypeDef,
     SalesforceSourcePropertiesTypeDef,
+    ScheduledTriggerPropertiesOutputTypeDef,
     ScheduledTriggerPropertiesTypeDef,
+    ServiceNowSourcePropertiesOutputTypeDef,
     ServiceNowSourcePropertiesTypeDef,
+    SingularSourcePropertiesOutputTypeDef,
     SingularSourcePropertiesTypeDef,
+    SlackSourcePropertiesOutputTypeDef,
     SlackSourcePropertiesTypeDef,
+    TrendmicroSourcePropertiesOutputTypeDef,
+    VeevaSourcePropertiesOutputTypeDef,
+    ZendeskSourcePropertiesOutputTypeDef,
     TrendmicroSourcePropertiesTypeDef,
     VeevaSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     StartFlowRequestRequestTypeDef,
     StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
     StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UnregisterConnectorRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
     CustomAuthConfigTypeDef,
-    CustomConnectorSourcePropertiesTypeDef,
+    CustomConnectorSourcePropertiesOutputTypeDef,
     ListConnectorsResponseTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ConnectorMetadataTypeDef,
     GoogleAnalyticsConnectorProfileCredentialsTypeDef,
     HoneycodeConnectorProfileCredentialsTypeDef,
     MarketoConnectorProfileCredentialsTypeDef,
     OAuth2CredentialsTypeDef,
     OAuthCredentialsTypeDef,
     PardotConnectorProfileCredentialsTypeDef,
     SalesforceConnectorProfileCredentialsTypeDef,
     SlackConnectorProfileCredentialsTypeDef,
     ZendeskConnectorProfileCredentialsTypeDef,
+    TaskOutputTypeDef,
     TaskTypeDef,
+    ConnectorProvisioningConfigOutputTypeDef,
     ConnectorProvisioningConfigTypeDef,
+    CustomConnectorDestinationPropertiesOutputTypeDef,
+    EventBridgeDestinationPropertiesOutputTypeDef,
+    HoneycodeDestinationPropertiesOutputTypeDef,
+    MarketoDestinationPropertiesOutputTypeDef,
+    RedshiftDestinationPropertiesOutputTypeDef,
+    SalesforceDestinationPropertiesOutputTypeDef,
+    SnowflakeDestinationPropertiesOutputTypeDef,
+    ZendeskDestinationPropertiesOutputTypeDef,
     CustomConnectorDestinationPropertiesTypeDef,
     EventBridgeDestinationPropertiesTypeDef,
     HoneycodeDestinationPropertiesTypeDef,
     MarketoDestinationPropertiesTypeDef,
     RedshiftDestinationPropertiesTypeDef,
     SalesforceDestinationPropertiesTypeDef,
     SnowflakeDestinationPropertiesTypeDef,
     ZendeskDestinationPropertiesTypeDef,
+    CustomConnectorProfilePropertiesOutputTypeDef,
     CustomConnectorProfilePropertiesTypeDef,
+    CustomConnectorSourcePropertiesTypeDef,
     FlowDefinitionTypeDef,
     ExecutionResultTypeDef,
     FieldTypeDetailsTypeDef,
+    MetadataCatalogConfigOutputTypeDef,
     MetadataCatalogConfigTypeDef,
     MetadataCatalogDetailTypeDef,
     OAuth2DefaultsTypeDef,
+    SAPODataConnectorProfilePropertiesOutputTypeDef,
     SAPODataConnectorProfilePropertiesTypeDef,
+    S3OutputFormatConfigOutputTypeDef,
+    UpsolverS3OutputFormatConfigOutputTypeDef,
     S3OutputFormatConfigTypeDef,
     UpsolverS3OutputFormatConfigTypeDef,
+    S3SourcePropertiesOutputTypeDef,
     S3SourcePropertiesTypeDef,
+    SAPODataDestinationPropertiesOutputTypeDef,
     SAPODataDestinationPropertiesTypeDef,
+    TriggerPropertiesOutputTypeDef,
     TriggerPropertiesTypeDef,
     CustomConnectorProfileCredentialsTypeDef,
     SAPODataConnectorProfileCredentialsTypeDef,
     RegisterConnectorRequestRequestTypeDef,
     UpdateConnectorRegistrationRequestRequestTypeDef,
     ListFlowsResponseTypeDef,
     SupportedFieldTypeDetailsTypeDef,
     ExecutionRecordTypeDef,
     AuthenticationConfigTypeDef,
+    ConnectorProfilePropertiesOutputTypeDef,
     ConnectorProfilePropertiesTypeDef,
+    S3DestinationPropertiesOutputTypeDef,
+    UpsolverDestinationPropertiesOutputTypeDef,
     S3DestinationPropertiesTypeDef,
     UpsolverDestinationPropertiesTypeDef,
+    SourceConnectorPropertiesOutputTypeDef,
     SourceConnectorPropertiesTypeDef,
+    TriggerConfigOutputTypeDef,
     TriggerConfigTypeDef,
     ConnectorProfileCredentialsTypeDef,
     ConnectorEntityFieldTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     ConnectorConfigurationTypeDef,
     ConnectorProfileTypeDef,
+    DestinationConnectorPropertiesOutputTypeDef,
     DestinationConnectorPropertiesTypeDef,
+    SourceFlowConfigOutputTypeDef,
     SourceFlowConfigTypeDef,
     ConnectorProfileConfigTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
+    DestinationFlowConfigOutputTypeDef,
     DestinationFlowConfigTypeDef,
     CreateConnectorProfileRequestRequestTypeDef,
     UpdateConnectorProfileRequestRequestTypeDef,
-    CreateFlowRequestRequestTypeDef,
     DescribeFlowResponseTypeDef,
+    CreateFlowRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AggregationConfigTypeDef:
+def get_structure() -> AggregationConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appflow-1.28.0/mypy_boto3_appflow.egg-info/SOURCES.txt` & `mypy-boto3-appflow-1.28.12/mypy_boto3_appflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.0/setup.py` & `mypy-boto3-appflow-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appflow",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_appflow"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Appflow 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Appflow 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

