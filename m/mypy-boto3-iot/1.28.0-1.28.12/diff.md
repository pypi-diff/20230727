# Comparing `tmp/mypy-boto3-iot-1.28.0.tar.gz` & `tmp/mypy-boto3-iot-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot-1.28.0.tar", last modified: Thu Jul  6 20:59:47 2023, max compression
+gzip compressed data, was "mypy-boto3-iot-1.28.12.tar", last modified: Thu Jul 27 05:34:48 2023, max compression
```

## Comparing `mypy-boto3-iot-1.28.0.tar` & `mypy-boto3-iot-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:47.306328 mypy-boto3-iot-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    54325 2023-07-06 20:59:47.306328 mypy-boto3-iot-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    52856 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:47.302328 mypy-boto3-iot-1.28.0/mypy_boto3_iot/
--rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   181667 2023-07-06 20:43:17.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   181351 2023-07-06 20:43:16.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24959 2023-07-06 20:43:18.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    24957 2023-07-06 20:43:18.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    69164 2023-07-06 20:43:17.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    69103 2023-07-06 20:43:17.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   257086 2023-07-06 20:43:27.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   256759 2023-07-06 20:43:23.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:47.306328 mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    54325 2023-07-06 20:59:47.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 20:59:47.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:47.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:47.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:47.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:47.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:47.306328 mypy-boto3-iot-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:48.856485 mypy-boto3-iot-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    58207 2023-07-27 05:34:48.852485 mypy-boto3-iot-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    56736 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:48.848485 mypy-boto3-iot-1.28.12/mypy_boto3_iot/
+-rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   181667 2023-07-27 05:23:45.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   181351 2023-07-27 05:23:43.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25037 2023-07-27 05:23:46.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-07-27 05:23:45.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    69164 2023-07-27 05:23:45.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69103 2023-07-27 05:23:45.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   293163 2023-07-27 05:23:52.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   292776 2023-07-27 05:23:48.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:48.848485 mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    58207 2023-07-27 05:34:48.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:34:48.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:48.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:48.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:48.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:48.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:48.856485 mypy-boto3-iot-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/setup.py
```

### Comparing `mypy-boto3-iot-1.28.0/LICENSE` & `mypy-boto3-iot-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.0/PKG-INFO` & `mypy-boto3-iot-1.28.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot
-Version: 1.28.0
-Summary: Type annotations for boto3.IoT 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoT 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iot"></a>
 
 # mypy-boto3-iot
 
 [![PyPI - mypy-boto3-iot](https://img.shields.io/pypi/v/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot?color=blue)](https://pypistats.org/packages/mypy-boto3-iot)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot)](https://pepy.tech/project/mypy-boto3-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[boto3.IoT 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
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
 [mypy-boto3-iot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/).
 
 See how it helps to find and fix potential bugs:
 
@@ -645,16 +645,34 @@
 ### Typed dictionaries
 
 `mypy_boto3_iot.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot.type_defs import (
+    AbortCriteriaOutputTypeDef,
     AbortCriteriaTypeDef,
     AcceptCertificateTransferRequestRequestTypeDef,
+    CloudwatchAlarmActionOutputTypeDef,
+    CloudwatchLogsActionOutputTypeDef,
+    CloudwatchMetricActionOutputTypeDef,
+    DynamoDBActionOutputTypeDef,
+    ElasticsearchActionOutputTypeDef,
+    FirehoseActionOutputTypeDef,
+    IotAnalyticsActionOutputTypeDef,
+    IotEventsActionOutputTypeDef,
+    KafkaActionOutputTypeDef,
+    KinesisActionOutputTypeDef,
+    LambdaActionOutputTypeDef,
+    OpenSearchActionOutputTypeDef,
+    S3ActionOutputTypeDef,
+    SalesforceActionOutputTypeDef,
+    SnsActionOutputTypeDef,
+    SqsActionOutputTypeDef,
+    StepFunctionsActionOutputTypeDef,
     CloudwatchAlarmActionTypeDef,
     CloudwatchLogsActionTypeDef,
     CloudwatchMetricActionTypeDef,
     DynamoDBActionTypeDef,
     ElasticsearchActionTypeDef,
     FirehoseActionTypeDef,
     IotAnalyticsActionTypeDef,
@@ -664,67 +682,88 @@
     LambdaActionTypeDef,
     OpenSearchActionTypeDef,
     S3ActionTypeDef,
     SalesforceActionTypeDef,
     SnsActionTypeDef,
     SqsActionTypeDef,
     StepFunctionsActionTypeDef,
-    MetricValueTypeDef,
+    MetricValueOutputTypeDef,
     ViolationEventAdditionalInfoTypeDef,
     AddThingToBillingGroupRequestRequestTypeDef,
     AddThingToThingGroupRequestRequestTypeDef,
+    AddThingsToThingGroupParamsOutputTypeDef,
     AddThingsToThingGroupParamsTypeDef,
+    AggregationTypeOutputTypeDef,
     AggregationTypeTypeDef,
+    AlertTargetOutputTypeDef,
     AlertTargetTypeDef,
     PolicyTypeDef,
+    AssetPropertyTimestampOutputTypeDef,
     AssetPropertyTimestampTypeDef,
+    AssetPropertyVariantOutputTypeDef,
     AssetPropertyVariantTypeDef,
     AssociateTargetsWithJobRequestRequestTypeDef,
     AssociateTargetsWithJobResponseTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachPrincipalPolicyRequestRequestTypeDef,
     AttachSecurityProfileRequestRequestTypeDef,
     AttachThingPrincipalRequestRequestTypeDef,
+    AttributePayloadOutputTypeDef,
     AttributePayloadTypeDef,
+    AuditCheckConfigurationOutputTypeDef,
     AuditCheckConfigurationTypeDef,
     AuditCheckDetailsTypeDef,
     AuditMitigationActionExecutionMetadataTypeDef,
     AuditMitigationActionsTaskMetadataTypeDef,
+    AuditMitigationActionsTaskTargetOutputTypeDef,
     AuditMitigationActionsTaskTargetTypeDef,
+    AuditNotificationTargetOutputTypeDef,
     AuditNotificationTargetTypeDef,
     AuditTaskMetadataTypeDef,
+    AuthInfoOutputTypeDef,
     AuthInfoTypeDef,
+    AuthorizerConfigOutputTypeDef,
     AuthorizerConfigTypeDef,
     AuthorizerDescriptionTypeDef,
     AuthorizerSummaryTypeDef,
     AwsJobAbortCriteriaTypeDef,
+    AwsJobRateIncreaseCriteriaOutputTypeDef,
     AwsJobRateIncreaseCriteriaTypeDef,
+    AwsJobPresignedUrlConfigOutputTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
+    MachineLearningDetectionConfigOutputTypeDef,
+    StatisticalThresholdOutputTypeDef,
     MachineLearningDetectionConfigTypeDef,
+    MetricValueTypeDef,
     StatisticalThresholdTypeDef,
     BehaviorModelTrainingSummaryTypeDef,
+    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     BillingGroupMetadataTypeDef,
+    BillingGroupPropertiesOutputTypeDef,
     BillingGroupPropertiesTypeDef,
     BucketTypeDef,
     TermsAggregationTypeDef,
     CertificateValidityTypeDef,
     CACertificateTypeDef,
     CancelAuditMitigationActionsTaskRequestRequestTypeDef,
     CancelAuditTaskRequestRequestTypeDef,
     CancelCertificateTransferRequestRequestTypeDef,
     CancelDetectMitigationActionsTaskRequestRequestTypeDef,
     CancelJobExecutionRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     CancelJobResponseTypeDef,
     TransferDataTypeDef,
     CertificateTypeDef,
+    CodeSigningCertificateChainOutputTypeDef,
     CodeSigningCertificateChainTypeDef,
+    CodeSigningSignatureOutputTypeDef,
     CodeSigningSignatureTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ConfirmTopicRuleDestinationRequestRequestTypeDef,
     TagTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateBillingGroupResponseTypeDef,
     CreateCertificateFromCsrRequestRequestTypeDef,
     CreateCertificateFromCsrResponseTypeDef,
@@ -799,35 +838,40 @@
     DescribeAuditMitigationActionsTaskRequestRequestTypeDef,
     TaskStatisticsForAuditCheckTypeDef,
     DescribeAuditTaskRequestRequestTypeDef,
     TaskStatisticsTypeDef,
     DescribeAuthorizerRequestRequestTypeDef,
     DescribeBillingGroupRequestRequestTypeDef,
     DescribeCACertificateRequestRequestTypeDef,
-    RegistrationConfigTypeDef,
+    RegistrationConfigOutputTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     DescribeCustomMetricRequestRequestTypeDef,
     DescribeCustomMetricResponseTypeDef,
     DescribeDetectMitigationActionsTaskRequestRequestTypeDef,
     DescribeDimensionRequestRequestTypeDef,
     DescribeDimensionResponseTypeDef,
     DescribeDomainConfigurationRequestRequestTypeDef,
     ServerCertificateSummaryTypeDef,
+    TlsConfigOutputTypeDef,
     DescribeEndpointRequestRequestTypeDef,
     DescribeEndpointResponseTypeDef,
     DescribeFleetMetricRequestRequestTypeDef,
     DescribeIndexRequestRequestTypeDef,
     DescribeIndexResponseTypeDef,
     DescribeJobExecutionRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
+    MaintenanceWindowOutputTypeDef,
+    PresignedUrlConfigOutputTypeDef,
+    TimeoutConfigOutputTypeDef,
     DescribeManagedJobTemplateRequestRequestTypeDef,
     DocumentParameterTypeDef,
     DescribeMitigationActionRequestRequestTypeDef,
     DescribeProvisioningTemplateRequestRequestTypeDef,
+    ProvisioningHookOutputTypeDef,
     DescribeProvisioningTemplateVersionRequestRequestTypeDef,
     DescribeProvisioningTemplateVersionResponseTypeDef,
     DescribeRoleAliasRequestRequestTypeDef,
     RoleAliasDescriptionTypeDef,
     DescribeScheduledAuditRequestRequestTypeDef,
     DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileRequestRequestTypeDef,
@@ -835,46 +879,55 @@
     DescribeThingGroupRequestRequestTypeDef,
     DescribeThingRegistrationTaskRequestRequestTypeDef,
     DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingRequestRequestTypeDef,
     DescribeThingResponseTypeDef,
     DescribeThingTypeRequestRequestTypeDef,
     ThingTypeMetadataTypeDef,
+    ThingTypePropertiesOutputTypeDef,
+    S3DestinationOutputTypeDef,
     S3DestinationTypeDef,
     DetachPolicyRequestRequestTypeDef,
     DetachPrincipalPolicyRequestRequestTypeDef,
     DetachSecurityProfileRequestRequestTypeDef,
     DetachThingPrincipalRequestRequestTypeDef,
     DetectMitigationActionExecutionTypeDef,
     DetectMitigationActionsTaskStatisticsTypeDef,
+    DetectMitigationActionsTaskTargetOutputTypeDef,
+    ViolationEventOccurrenceRangeOutputTypeDef,
     DetectMitigationActionsTaskTargetTypeDef,
-    ViolationEventOccurrenceRangeTypeDef,
     DisableTopicRuleRequestRequestTypeDef,
     DomainConfigurationSummaryTypeDef,
+    PutItemInputOutputTypeDef,
     PutItemInputTypeDef,
     EffectivePolicyTypeDef,
     EmptyResponseMetadataTypeDef,
+    EnableIoTLoggingParamsOutputTypeDef,
     EnableIoTLoggingParamsTypeDef,
     EnableTopicRuleRequestRequestTypeDef,
     ErrorInfoTypeDef,
+    RateIncreaseCriteriaOutputTypeDef,
     RateIncreaseCriteriaTypeDef,
+    FieldOutputTypeDef,
     FieldTypeDef,
+    S3LocationOutputTypeDef,
+    StreamOutputTypeDef,
     S3LocationTypeDef,
     StreamTypeDef,
     FleetMetricNameAndArnTypeDef,
     GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef,
     GetBehaviorModelTrainingSummariesRequestRequestTypeDef,
     GetCardinalityRequestRequestTypeDef,
     GetCardinalityResponseTypeDef,
     GetEffectivePoliciesRequestRequestTypeDef,
     GetJobDocumentRequestRequestTypeDef,
     GetJobDocumentResponseTypeDef,
     GetLoggingOptionsResponseTypeDef,
     GetOTAUpdateRequestRequestTypeDef,
-    VersionUpdateByJobsConfigTypeDef,
+    VersionUpdateByJobsConfigOutputTypeDef,
     GetPackageRequestRequestTypeDef,
     GetPackageResponseTypeDef,
     GetPackageVersionRequestRequestTypeDef,
     GetPackageVersionResponseTypeDef,
     GetPercentilesRequestRequestTypeDef,
     PercentPairTypeDef,
     GetPolicyRequestRequestTypeDef,
@@ -884,24 +937,29 @@
     GetRegistrationCodeResponseTypeDef,
     GetStatisticsRequestRequestTypeDef,
     StatisticsTypeDef,
     GetTopicRuleDestinationRequestRequestTypeDef,
     GetTopicRuleRequestRequestTypeDef,
     GetV2LoggingOptionsResponseTypeDef,
     GroupNameAndArnTypeDef,
+    HttpActionHeaderOutputTypeDef,
     HttpActionHeaderTypeDef,
+    SigV4AuthorizationOutputTypeDef,
     SigV4AuthorizationTypeDef,
     HttpContextTypeDef,
     HttpUrlDestinationConfigurationTypeDef,
     HttpUrlDestinationPropertiesTypeDef,
     HttpUrlDestinationSummaryTypeDef,
+    IndexingFilterOutputTypeDef,
     IndexingFilterTypeDef,
+    IssuerCertificateIdentifierOutputTypeDef,
     IssuerCertificateIdentifierTypeDef,
     JobExecutionStatusDetailsTypeDef,
     JobExecutionSummaryTypeDef,
+    RetryCriteriaOutputTypeDef,
     RetryCriteriaTypeDef,
     JobProcessDetailsTypeDef,
     JobSummaryTypeDef,
     JobTemplateSummaryTypeDef,
     ScheduledJobRolloutTypeDef,
     ListActiveViolationsRequestListActiveViolationsPaginateTypeDef,
     ListActiveViolationsRequestRequestTypeDef,
@@ -1000,14 +1058,15 @@
     ListSecurityProfilesRequestRequestTypeDef,
     SecurityProfileIdentifierTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     StreamSummaryTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
     ListTargetsForPolicyRequestRequestTypeDef,
     ListTargetsForPolicyResponseTypeDef,
     ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
     ListTargetsForSecurityProfileRequestRequestTypeDef,
     SecurityProfileTargetTypeDef,
     ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
@@ -1039,26 +1098,35 @@
     ListTopicRulesRequestListTopicRulesPaginateTypeDef,
     ListTopicRulesRequestRequestTypeDef,
     TopicRuleListItemTypeDef,
     ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef,
     ListV2LoggingLevelsRequestRequestTypeDef,
     ListViolationEventsRequestListViolationEventsPaginateTypeDef,
     ListViolationEventsRequestRequestTypeDef,
+    LocationTimestampOutputTypeDef,
     LocationTimestampTypeDef,
+    LogTargetOutputTypeDef,
     LogTargetTypeDef,
     LoggingOptionsPayloadTypeDef,
+    PublishFindingToSnsParamsOutputTypeDef,
+    ReplaceDefaultPolicyVersionParamsOutputTypeDef,
+    UpdateCACertificateParamsOutputTypeDef,
+    UpdateDeviceCertificateParamsOutputTypeDef,
     PublishFindingToSnsParamsTypeDef,
     ReplaceDefaultPolicyVersionParamsTypeDef,
     UpdateCACertificateParamsTypeDef,
     UpdateDeviceCertificateParamsTypeDef,
     MqttContextTypeDef,
+    UserPropertyOutputTypeDef,
     UserPropertyTypeDef,
     PaginatorConfigTypeDef,
+    PolicyVersionIdentifierOutputTypeDef,
     PolicyVersionIdentifierTypeDef,
     PutVerificationStateOnViolationRequestRequestTypeDef,
+    RegistrationConfigTypeDef,
     RegisterCACertificateResponseTypeDef,
     RegisterCertificateRequestRequestTypeDef,
     RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCARequestRequestTypeDef,
     RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingRequestRequestTypeDef,
     RegisterThingResponseTypeDef,
@@ -1068,25 +1136,29 @@
     ResponseMetadataTypeDef,
     SearchIndexRequestRequestTypeDef,
     ThingGroupDocumentTypeDef,
     SetDefaultAuthorizerRequestRequestTypeDef,
     SetDefaultAuthorizerResponseTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetV2LoggingOptionsRequestRequestTypeDef,
+    SigningProfileParameterOutputTypeDef,
     SigningProfileParameterTypeDef,
     StartAuditMitigationActionsTaskResponseTypeDef,
+    ViolationEventOccurrenceRangeTypeDef,
     StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskRequestRequestTypeDef,
     StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskRequestRequestTypeDef,
     StartThingRegistrationTaskResponseTypeDef,
     StopThingRegistrationTaskRequestRequestTypeDef,
     TlsContextTypeDef,
     TestInvokeAuthorizerResponseTypeDef,
     ThingConnectivityTypeDef,
+    TimestreamDimensionOutputTypeDef,
+    TimestreamTimestampOutputTypeDef,
     TimestreamDimensionTypeDef,
     TimestreamTimestampTypeDef,
     VpcDestinationConfigurationTypeDef,
     VpcDestinationSummaryTypeDef,
     VpcDestinationPropertiesTypeDef,
     TransferCertificateRequestRequestTypeDef,
     TransferCertificateResponseTypeDef,
@@ -1098,117 +1170,130 @@
     UpdateCustomMetricRequestRequestTypeDef,
     UpdateCustomMetricResponseTypeDef,
     UpdateDimensionRequestRequestTypeDef,
     UpdateDimensionResponseTypeDef,
     UpdateDomainConfigurationResponseTypeDef,
     UpdateDynamicThingGroupResponseTypeDef,
     UpdateMitigationActionResponseTypeDef,
+    VersionUpdateByJobsConfigTypeDef,
     UpdatePackageRequestRequestTypeDef,
     UpdatePackageVersionRequestRequestTypeDef,
     UpdateRoleAliasRequestRequestTypeDef,
     UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditRequestRequestTypeDef,
     UpdateScheduledAuditResponseTypeDef,
     UpdateStreamResponseTypeDef,
     UpdateThingGroupResponseTypeDef,
     UpdateThingGroupsForThingRequestRequestTypeDef,
     UpdateTopicRuleDestinationRequestRequestTypeDef,
     ValidationErrorTypeDef,
+    AbortConfigOutputTypeDef,
     AbortConfigTypeDef,
     MetricDatumTypeDef,
     DescribeFleetMetricResponseTypeDef,
     UpdateFleetMetricRequestRequestTypeDef,
     AllowedTypeDef,
     ExplicitDenyTypeDef,
     ImplicitDenyTypeDef,
     ListAttachedPoliciesResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListPrincipalPoliciesResponseTypeDef,
+    AssetPropertyValueOutputTypeDef,
     AssetPropertyValueTypeDef,
+    ThingGroupPropertiesOutputTypeDef,
     CreateThingRequestRequestTypeDef,
     ThingGroupPropertiesTypeDef,
     UpdateThingRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
     StartAuditMitigationActionsTaskRequestRequestTypeDef,
     DescribeAccountAuditConfigurationResponseTypeDef,
     UpdateAccountAuditConfigurationRequestRequestTypeDef,
     ListAuditTasksResponseTypeDef,
     TestAuthorizationRequestRequestTypeDef,
     DescribeAuthorizerResponseTypeDef,
     DescribeDefaultAuthorizerResponseTypeDef,
     ListAuthorizersResponseTypeDef,
     AwsJobAbortConfigTypeDef,
+    AwsJobExponentialRolloutRateOutputTypeDef,
     AwsJobExponentialRolloutRateTypeDef,
+    BehaviorCriteriaOutputTypeDef,
     BehaviorCriteriaTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
+    MetricToRetainOutputTypeDef,
     MetricToRetainTypeDef,
     DescribeBillingGroupResponseTypeDef,
     UpdateBillingGroupRequestRequestTypeDef,
     GetBucketsAggregationResponseTypeDef,
     BucketsAggregationTypeTypeDef,
     CACertificateDescriptionTypeDef,
     ListCACertificatesResponseTypeDef,
     CertificateDescriptionTypeDef,
     ListCertificatesByCAResponseTypeDef,
     ListCertificatesResponseTypeDef,
+    CustomCodeSigningOutputTypeDef,
     CustomCodeSigningTypeDef,
     DescribeEventConfigurationsResponseTypeDef,
     UpdateEventConfigurationsRequestRequestTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     CreateBillingGroupRequestRequestTypeDef,
     CreateCustomMetricRequestRequestTypeDef,
     CreateDimensionRequestRequestTypeDef,
     CreateFleetMetricRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreateRoleAliasRequestRequestTypeDef,
     CreateScheduledAuditRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainConfigurationRequestRequestTypeDef,
     UpdateDomainConfigurationRequestRequestTypeDef,
     SchedulingConfigTypeDef,
     CreateKeysAndCertificateResponseTypeDef,
     CreateProvisioningClaimResponseTypeDef,
     CreateProvisioningTemplateRequestRequestTypeDef,
-    DescribeProvisioningTemplateResponseTypeDef,
     UpdateProvisioningTemplateRequestRequestTypeDef,
     CreateThingTypeRequestRequestTypeDef,
     DescribeAuditTaskResponseTypeDef,
-    RegisterCACertificateRequestRequestTypeDef,
-    UpdateCACertificateRequestRequestTypeDef,
     DescribeDomainConfigurationResponseTypeDef,
+    SchedulingConfigOutputTypeDef,
     DescribeManagedJobTemplateResponseTypeDef,
+    DescribeProvisioningTemplateResponseTypeDef,
     DescribeRoleAliasResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
     ThingTypeDefinitionTypeDef,
+    DestinationOutputTypeDef,
     DestinationTypeDef,
     ListDetectMitigationActionsExecutionsResponseTypeDef,
-    StartDetectMitigationActionsTaskRequestRequestTypeDef,
     ListDomainConfigurationsResponseTypeDef,
+    DynamoDBv2ActionOutputTypeDef,
     DynamoDBv2ActionTypeDef,
     GetEffectivePoliciesResponseTypeDef,
+    ExponentialRolloutRateOutputTypeDef,
     ExponentialRolloutRateTypeDef,
+    ThingGroupIndexingConfigurationOutputTypeDef,
     ThingGroupIndexingConfigurationTypeDef,
+    StreamFileOutputTypeDef,
+    FileLocationOutputTypeDef,
     StreamFileTypeDef,
     FileLocationTypeDef,
     ListFleetMetricsResponseTypeDef,
     GetPackageConfigurationResponseTypeDef,
-    UpdatePackageConfigurationRequestRequestTypeDef,
     GetPercentilesResponseTypeDef,
     GetStatisticsResponseTypeDef,
     ListBillingGroupsResponseTypeDef,
     ListThingGroupsForThingResponseTypeDef,
     ListThingGroupsResponseTypeDef,
     ThingGroupMetadataTypeDef,
+    HttpAuthorizationOutputTypeDef,
     HttpAuthorizationTypeDef,
+    ThingIndexingConfigurationOutputTypeDef,
     ThingIndexingConfigurationTypeDef,
     JobExecutionTypeDef,
     JobExecutionSummaryForJobTypeDef,
     JobExecutionSummaryForThingTypeDef,
+    JobExecutionsRetryConfigOutputTypeDef,
     JobExecutionsRetryConfigTypeDef,
     ListJobsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedJobTemplatesResponseTypeDef,
     ListMitigationActionsResponseTypeDef,
     ListOTAUpdatesResponseTypeDef,
     ListOutgoingCertificatesResponseTypeDef,
@@ -1216,124 +1301,145 @@
     ListPackagesResponseTypeDef,
     ListPolicyVersionsResponseTypeDef,
     ListProvisioningTemplateVersionsResponseTypeDef,
     ListProvisioningTemplatesResponseTypeDef,
     ListScheduledAuditsResponseTypeDef,
     ListSecurityProfilesResponseTypeDef,
     ListStreamsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTargetsForSecurityProfileResponseTypeDef,
     SecurityProfileTargetMappingTypeDef,
     ListThingsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
+    LocationActionOutputTypeDef,
     LocationActionTypeDef,
     LogTargetConfigurationTypeDef,
     SetV2LoggingLevelRequestRequestTypeDef,
     SetLoggingOptionsRequestRequestTypeDef,
+    MitigationActionParamsOutputTypeDef,
     MitigationActionParamsTypeDef,
+    MqttHeadersOutputTypeDef,
     MqttHeadersTypeDef,
+    ResourceIdentifierOutputTypeDef,
     ResourceIdentifierTypeDef,
+    RegisterCACertificateRequestRequestTypeDef,
+    UpdateCACertificateRequestRequestTypeDef,
+    StartDetectMitigationActionsTaskRequestRequestTypeDef,
     TestInvokeAuthorizerRequestRequestTypeDef,
     ThingDocumentTypeDef,
+    TimestreamActionOutputTypeDef,
     TimestreamActionTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRuleDestinationSummaryTypeDef,
     TopicRuleDestinationTypeDef,
+    UpdatePackageConfigurationRequestRequestTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
     ListMetricValuesResponseTypeDef,
     DeniedTypeDef,
+    PutAssetPropertyValueEntryOutputTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     CreateDynamicThingGroupRequestRequestTypeDef,
     CreateThingGroupRequestRequestTypeDef,
     UpdateDynamicThingGroupRequestRequestTypeDef,
     UpdateThingGroupRequestRequestTypeDef,
+    AwsJobExecutionsRolloutConfigOutputTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
+    BehaviorOutputTypeDef,
     BehaviorTypeDef,
     GetBucketsAggregationRequestRequestTypeDef,
     DescribeCACertificateResponseTypeDef,
     DescribeCertificateResponseTypeDef,
     ListThingTypesResponseTypeDef,
+    StartSigningJobParameterOutputTypeDef,
     StartSigningJobParameterTypeDef,
+    JobExecutionsRolloutConfigOutputTypeDef,
     JobExecutionsRolloutConfigTypeDef,
-    CreateStreamRequestRequestTypeDef,
     StreamInfoTypeDef,
+    CreateStreamRequestRequestTypeDef,
     UpdateStreamRequestRequestTypeDef,
     DescribeThingGroupResponseTypeDef,
+    HttpActionOutputTypeDef,
     HttpActionTypeDef,
     GetIndexingConfigurationResponseTypeDef,
     UpdateIndexingConfigurationRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
     ListJobExecutionsForJobResponseTypeDef,
     ListJobExecutionsForThingResponseTypeDef,
     ListSecurityProfilesForTargetResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
-    CreateMitigationActionRequestRequestTypeDef,
     DescribeMitigationActionResponseTypeDef,
     MitigationActionTypeDef,
+    CreateMitigationActionRequestRequestTypeDef,
     UpdateMitigationActionRequestRequestTypeDef,
+    RepublishActionOutputTypeDef,
     RepublishActionTypeDef,
     AuditSuppressionTypeDef,
+    DescribeAuditSuppressionResponseTypeDef,
+    NonCompliantResourceTypeDef,
+    RelatedResourceTypeDef,
     CreateAuditSuppressionRequestRequestTypeDef,
     DeleteAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionRequestRequestTypeDef,
-    DescribeAuditSuppressionResponseTypeDef,
     ListAuditFindingsRequestListAuditFindingsPaginateTypeDef,
     ListAuditFindingsRequestRequestTypeDef,
     ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef,
     ListAuditSuppressionsRequestRequestTypeDef,
-    NonCompliantResourceTypeDef,
-    RelatedResourceTypeDef,
     UpdateAuditSuppressionRequestRequestTypeDef,
     SearchIndexResponseTypeDef,
     CreateTopicRuleDestinationRequestRequestTypeDef,
     ListTopicRuleDestinationsResponseTypeDef,
     CreateTopicRuleDestinationResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     AuthResultTypeDef,
+    IotSiteWiseActionOutputTypeDef,
     IotSiteWiseActionTypeDef,
     ActiveViolationTypeDef,
-    CreateSecurityProfileRequestRequestTypeDef,
     DescribeSecurityProfileResponseTypeDef,
-    UpdateSecurityProfileRequestRequestTypeDef,
     UpdateSecurityProfileResponseTypeDef,
-    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
     ViolationEventTypeDef,
+    CreateSecurityProfileRequestRequestTypeDef,
+    UpdateSecurityProfileRequestRequestTypeDef,
+    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
+    CodeSigningOutputTypeDef,
     CodeSigningTypeDef,
-    CreateJobRequestRequestTypeDef,
-    CreateJobTemplateRequestRequestTypeDef,
     DescribeJobTemplateResponseTypeDef,
     JobTypeDef,
+    CreateJobRequestRequestTypeDef,
+    CreateJobTemplateRequestRequestTypeDef,
     UpdateJobRequestRequestTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeAuditMitigationActionsTaskResponseTypeDef,
     DetectMitigationActionsTaskSummaryTypeDef,
     ListAuditSuppressionsResponseTypeDef,
     AuditFindingTypeDef,
     ListRelatedResourcesForAuditFindingResponseTypeDef,
     TestAuthorizationResponseTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
+    OTAUpdateFileOutputTypeDef,
     OTAUpdateFileTypeDef,
     DescribeJobResponseTypeDef,
     DescribeDetectMitigationActionsTaskResponseTypeDef,
     ListDetectMitigationActionsTasksResponseTypeDef,
     DescribeAuditFindingResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
-    TopicRulePayloadTypeDef,
     TopicRuleTypeDef,
-    CreateOTAUpdateRequestRequestTypeDef,
+    TopicRulePayloadTypeDef,
     OTAUpdateInfoTypeDef,
+    CreateOTAUpdateRequestRequestTypeDef,
+    GetTopicRuleResponseTypeDef,
     CreateTopicRuleRequestRequestTypeDef,
     ReplaceTopicRuleRequestRequestTypeDef,
-    GetTopicRuleResponseTypeDef,
     GetOTAUpdateResponseTypeDef,
 )
 
 
-def get_structure() -> AbortCriteriaTypeDef:
+def get_structure() -> AbortCriteriaOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-1.28.0/README.md` & `mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-iot
+Version: 1.28.12
+Summary: Type annotations for boto3.IoT 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 iot type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iot"></a>
 
 # mypy-boto3-iot
 
 [![PyPI - mypy-boto3-iot](https://img.shields.io/pypi/v/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot?color=blue)](https://pypistats.org/packages/mypy-boto3-iot)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot)](https://pepy.tech/project/mypy-boto3-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[boto3.IoT 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
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
 [mypy-boto3-iot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/).
 
 See how it helps to find and fix potential bugs:
 
@@ -613,16 +645,34 @@
 ### Typed dictionaries
 
 `mypy_boto3_iot.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot.type_defs import (
+    AbortCriteriaOutputTypeDef,
     AbortCriteriaTypeDef,
     AcceptCertificateTransferRequestRequestTypeDef,
+    CloudwatchAlarmActionOutputTypeDef,
+    CloudwatchLogsActionOutputTypeDef,
+    CloudwatchMetricActionOutputTypeDef,
+    DynamoDBActionOutputTypeDef,
+    ElasticsearchActionOutputTypeDef,
+    FirehoseActionOutputTypeDef,
+    IotAnalyticsActionOutputTypeDef,
+    IotEventsActionOutputTypeDef,
+    KafkaActionOutputTypeDef,
+    KinesisActionOutputTypeDef,
+    LambdaActionOutputTypeDef,
+    OpenSearchActionOutputTypeDef,
+    S3ActionOutputTypeDef,
+    SalesforceActionOutputTypeDef,
+    SnsActionOutputTypeDef,
+    SqsActionOutputTypeDef,
+    StepFunctionsActionOutputTypeDef,
     CloudwatchAlarmActionTypeDef,
     CloudwatchLogsActionTypeDef,
     CloudwatchMetricActionTypeDef,
     DynamoDBActionTypeDef,
     ElasticsearchActionTypeDef,
     FirehoseActionTypeDef,
     IotAnalyticsActionTypeDef,
@@ -632,67 +682,88 @@
     LambdaActionTypeDef,
     OpenSearchActionTypeDef,
     S3ActionTypeDef,
     SalesforceActionTypeDef,
     SnsActionTypeDef,
     SqsActionTypeDef,
     StepFunctionsActionTypeDef,
-    MetricValueTypeDef,
+    MetricValueOutputTypeDef,
     ViolationEventAdditionalInfoTypeDef,
     AddThingToBillingGroupRequestRequestTypeDef,
     AddThingToThingGroupRequestRequestTypeDef,
+    AddThingsToThingGroupParamsOutputTypeDef,
     AddThingsToThingGroupParamsTypeDef,
+    AggregationTypeOutputTypeDef,
     AggregationTypeTypeDef,
+    AlertTargetOutputTypeDef,
     AlertTargetTypeDef,
     PolicyTypeDef,
+    AssetPropertyTimestampOutputTypeDef,
     AssetPropertyTimestampTypeDef,
+    AssetPropertyVariantOutputTypeDef,
     AssetPropertyVariantTypeDef,
     AssociateTargetsWithJobRequestRequestTypeDef,
     AssociateTargetsWithJobResponseTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachPrincipalPolicyRequestRequestTypeDef,
     AttachSecurityProfileRequestRequestTypeDef,
     AttachThingPrincipalRequestRequestTypeDef,
+    AttributePayloadOutputTypeDef,
     AttributePayloadTypeDef,
+    AuditCheckConfigurationOutputTypeDef,
     AuditCheckConfigurationTypeDef,
     AuditCheckDetailsTypeDef,
     AuditMitigationActionExecutionMetadataTypeDef,
     AuditMitigationActionsTaskMetadataTypeDef,
+    AuditMitigationActionsTaskTargetOutputTypeDef,
     AuditMitigationActionsTaskTargetTypeDef,
+    AuditNotificationTargetOutputTypeDef,
     AuditNotificationTargetTypeDef,
     AuditTaskMetadataTypeDef,
+    AuthInfoOutputTypeDef,
     AuthInfoTypeDef,
+    AuthorizerConfigOutputTypeDef,
     AuthorizerConfigTypeDef,
     AuthorizerDescriptionTypeDef,
     AuthorizerSummaryTypeDef,
     AwsJobAbortCriteriaTypeDef,
+    AwsJobRateIncreaseCriteriaOutputTypeDef,
     AwsJobRateIncreaseCriteriaTypeDef,
+    AwsJobPresignedUrlConfigOutputTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
+    MachineLearningDetectionConfigOutputTypeDef,
+    StatisticalThresholdOutputTypeDef,
     MachineLearningDetectionConfigTypeDef,
+    MetricValueTypeDef,
     StatisticalThresholdTypeDef,
     BehaviorModelTrainingSummaryTypeDef,
+    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     BillingGroupMetadataTypeDef,
+    BillingGroupPropertiesOutputTypeDef,
     BillingGroupPropertiesTypeDef,
     BucketTypeDef,
     TermsAggregationTypeDef,
     CertificateValidityTypeDef,
     CACertificateTypeDef,
     CancelAuditMitigationActionsTaskRequestRequestTypeDef,
     CancelAuditTaskRequestRequestTypeDef,
     CancelCertificateTransferRequestRequestTypeDef,
     CancelDetectMitigationActionsTaskRequestRequestTypeDef,
     CancelJobExecutionRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     CancelJobResponseTypeDef,
     TransferDataTypeDef,
     CertificateTypeDef,
+    CodeSigningCertificateChainOutputTypeDef,
     CodeSigningCertificateChainTypeDef,
+    CodeSigningSignatureOutputTypeDef,
     CodeSigningSignatureTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ConfirmTopicRuleDestinationRequestRequestTypeDef,
     TagTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateBillingGroupResponseTypeDef,
     CreateCertificateFromCsrRequestRequestTypeDef,
     CreateCertificateFromCsrResponseTypeDef,
@@ -767,35 +838,40 @@
     DescribeAuditMitigationActionsTaskRequestRequestTypeDef,
     TaskStatisticsForAuditCheckTypeDef,
     DescribeAuditTaskRequestRequestTypeDef,
     TaskStatisticsTypeDef,
     DescribeAuthorizerRequestRequestTypeDef,
     DescribeBillingGroupRequestRequestTypeDef,
     DescribeCACertificateRequestRequestTypeDef,
-    RegistrationConfigTypeDef,
+    RegistrationConfigOutputTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     DescribeCustomMetricRequestRequestTypeDef,
     DescribeCustomMetricResponseTypeDef,
     DescribeDetectMitigationActionsTaskRequestRequestTypeDef,
     DescribeDimensionRequestRequestTypeDef,
     DescribeDimensionResponseTypeDef,
     DescribeDomainConfigurationRequestRequestTypeDef,
     ServerCertificateSummaryTypeDef,
+    TlsConfigOutputTypeDef,
     DescribeEndpointRequestRequestTypeDef,
     DescribeEndpointResponseTypeDef,
     DescribeFleetMetricRequestRequestTypeDef,
     DescribeIndexRequestRequestTypeDef,
     DescribeIndexResponseTypeDef,
     DescribeJobExecutionRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
+    MaintenanceWindowOutputTypeDef,
+    PresignedUrlConfigOutputTypeDef,
+    TimeoutConfigOutputTypeDef,
     DescribeManagedJobTemplateRequestRequestTypeDef,
     DocumentParameterTypeDef,
     DescribeMitigationActionRequestRequestTypeDef,
     DescribeProvisioningTemplateRequestRequestTypeDef,
+    ProvisioningHookOutputTypeDef,
     DescribeProvisioningTemplateVersionRequestRequestTypeDef,
     DescribeProvisioningTemplateVersionResponseTypeDef,
     DescribeRoleAliasRequestRequestTypeDef,
     RoleAliasDescriptionTypeDef,
     DescribeScheduledAuditRequestRequestTypeDef,
     DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileRequestRequestTypeDef,
@@ -803,46 +879,55 @@
     DescribeThingGroupRequestRequestTypeDef,
     DescribeThingRegistrationTaskRequestRequestTypeDef,
     DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingRequestRequestTypeDef,
     DescribeThingResponseTypeDef,
     DescribeThingTypeRequestRequestTypeDef,
     ThingTypeMetadataTypeDef,
+    ThingTypePropertiesOutputTypeDef,
+    S3DestinationOutputTypeDef,
     S3DestinationTypeDef,
     DetachPolicyRequestRequestTypeDef,
     DetachPrincipalPolicyRequestRequestTypeDef,
     DetachSecurityProfileRequestRequestTypeDef,
     DetachThingPrincipalRequestRequestTypeDef,
     DetectMitigationActionExecutionTypeDef,
     DetectMitigationActionsTaskStatisticsTypeDef,
+    DetectMitigationActionsTaskTargetOutputTypeDef,
+    ViolationEventOccurrenceRangeOutputTypeDef,
     DetectMitigationActionsTaskTargetTypeDef,
-    ViolationEventOccurrenceRangeTypeDef,
     DisableTopicRuleRequestRequestTypeDef,
     DomainConfigurationSummaryTypeDef,
+    PutItemInputOutputTypeDef,
     PutItemInputTypeDef,
     EffectivePolicyTypeDef,
     EmptyResponseMetadataTypeDef,
+    EnableIoTLoggingParamsOutputTypeDef,
     EnableIoTLoggingParamsTypeDef,
     EnableTopicRuleRequestRequestTypeDef,
     ErrorInfoTypeDef,
+    RateIncreaseCriteriaOutputTypeDef,
     RateIncreaseCriteriaTypeDef,
+    FieldOutputTypeDef,
     FieldTypeDef,
+    S3LocationOutputTypeDef,
+    StreamOutputTypeDef,
     S3LocationTypeDef,
     StreamTypeDef,
     FleetMetricNameAndArnTypeDef,
     GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef,
     GetBehaviorModelTrainingSummariesRequestRequestTypeDef,
     GetCardinalityRequestRequestTypeDef,
     GetCardinalityResponseTypeDef,
     GetEffectivePoliciesRequestRequestTypeDef,
     GetJobDocumentRequestRequestTypeDef,
     GetJobDocumentResponseTypeDef,
     GetLoggingOptionsResponseTypeDef,
     GetOTAUpdateRequestRequestTypeDef,
-    VersionUpdateByJobsConfigTypeDef,
+    VersionUpdateByJobsConfigOutputTypeDef,
     GetPackageRequestRequestTypeDef,
     GetPackageResponseTypeDef,
     GetPackageVersionRequestRequestTypeDef,
     GetPackageVersionResponseTypeDef,
     GetPercentilesRequestRequestTypeDef,
     PercentPairTypeDef,
     GetPolicyRequestRequestTypeDef,
@@ -852,24 +937,29 @@
     GetRegistrationCodeResponseTypeDef,
     GetStatisticsRequestRequestTypeDef,
     StatisticsTypeDef,
     GetTopicRuleDestinationRequestRequestTypeDef,
     GetTopicRuleRequestRequestTypeDef,
     GetV2LoggingOptionsResponseTypeDef,
     GroupNameAndArnTypeDef,
+    HttpActionHeaderOutputTypeDef,
     HttpActionHeaderTypeDef,
+    SigV4AuthorizationOutputTypeDef,
     SigV4AuthorizationTypeDef,
     HttpContextTypeDef,
     HttpUrlDestinationConfigurationTypeDef,
     HttpUrlDestinationPropertiesTypeDef,
     HttpUrlDestinationSummaryTypeDef,
+    IndexingFilterOutputTypeDef,
     IndexingFilterTypeDef,
+    IssuerCertificateIdentifierOutputTypeDef,
     IssuerCertificateIdentifierTypeDef,
     JobExecutionStatusDetailsTypeDef,
     JobExecutionSummaryTypeDef,
+    RetryCriteriaOutputTypeDef,
     RetryCriteriaTypeDef,
     JobProcessDetailsTypeDef,
     JobSummaryTypeDef,
     JobTemplateSummaryTypeDef,
     ScheduledJobRolloutTypeDef,
     ListActiveViolationsRequestListActiveViolationsPaginateTypeDef,
     ListActiveViolationsRequestRequestTypeDef,
@@ -968,14 +1058,15 @@
     ListSecurityProfilesRequestRequestTypeDef,
     SecurityProfileIdentifierTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     StreamSummaryTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
     ListTargetsForPolicyRequestRequestTypeDef,
     ListTargetsForPolicyResponseTypeDef,
     ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
     ListTargetsForSecurityProfileRequestRequestTypeDef,
     SecurityProfileTargetTypeDef,
     ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
@@ -1007,26 +1098,35 @@
     ListTopicRulesRequestListTopicRulesPaginateTypeDef,
     ListTopicRulesRequestRequestTypeDef,
     TopicRuleListItemTypeDef,
     ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef,
     ListV2LoggingLevelsRequestRequestTypeDef,
     ListViolationEventsRequestListViolationEventsPaginateTypeDef,
     ListViolationEventsRequestRequestTypeDef,
+    LocationTimestampOutputTypeDef,
     LocationTimestampTypeDef,
+    LogTargetOutputTypeDef,
     LogTargetTypeDef,
     LoggingOptionsPayloadTypeDef,
+    PublishFindingToSnsParamsOutputTypeDef,
+    ReplaceDefaultPolicyVersionParamsOutputTypeDef,
+    UpdateCACertificateParamsOutputTypeDef,
+    UpdateDeviceCertificateParamsOutputTypeDef,
     PublishFindingToSnsParamsTypeDef,
     ReplaceDefaultPolicyVersionParamsTypeDef,
     UpdateCACertificateParamsTypeDef,
     UpdateDeviceCertificateParamsTypeDef,
     MqttContextTypeDef,
+    UserPropertyOutputTypeDef,
     UserPropertyTypeDef,
     PaginatorConfigTypeDef,
+    PolicyVersionIdentifierOutputTypeDef,
     PolicyVersionIdentifierTypeDef,
     PutVerificationStateOnViolationRequestRequestTypeDef,
+    RegistrationConfigTypeDef,
     RegisterCACertificateResponseTypeDef,
     RegisterCertificateRequestRequestTypeDef,
     RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCARequestRequestTypeDef,
     RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingRequestRequestTypeDef,
     RegisterThingResponseTypeDef,
@@ -1036,25 +1136,29 @@
     ResponseMetadataTypeDef,
     SearchIndexRequestRequestTypeDef,
     ThingGroupDocumentTypeDef,
     SetDefaultAuthorizerRequestRequestTypeDef,
     SetDefaultAuthorizerResponseTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetV2LoggingOptionsRequestRequestTypeDef,
+    SigningProfileParameterOutputTypeDef,
     SigningProfileParameterTypeDef,
     StartAuditMitigationActionsTaskResponseTypeDef,
+    ViolationEventOccurrenceRangeTypeDef,
     StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskRequestRequestTypeDef,
     StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskRequestRequestTypeDef,
     StartThingRegistrationTaskResponseTypeDef,
     StopThingRegistrationTaskRequestRequestTypeDef,
     TlsContextTypeDef,
     TestInvokeAuthorizerResponseTypeDef,
     ThingConnectivityTypeDef,
+    TimestreamDimensionOutputTypeDef,
+    TimestreamTimestampOutputTypeDef,
     TimestreamDimensionTypeDef,
     TimestreamTimestampTypeDef,
     VpcDestinationConfigurationTypeDef,
     VpcDestinationSummaryTypeDef,
     VpcDestinationPropertiesTypeDef,
     TransferCertificateRequestRequestTypeDef,
     TransferCertificateResponseTypeDef,
@@ -1066,117 +1170,130 @@
     UpdateCustomMetricRequestRequestTypeDef,
     UpdateCustomMetricResponseTypeDef,
     UpdateDimensionRequestRequestTypeDef,
     UpdateDimensionResponseTypeDef,
     UpdateDomainConfigurationResponseTypeDef,
     UpdateDynamicThingGroupResponseTypeDef,
     UpdateMitigationActionResponseTypeDef,
+    VersionUpdateByJobsConfigTypeDef,
     UpdatePackageRequestRequestTypeDef,
     UpdatePackageVersionRequestRequestTypeDef,
     UpdateRoleAliasRequestRequestTypeDef,
     UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditRequestRequestTypeDef,
     UpdateScheduledAuditResponseTypeDef,
     UpdateStreamResponseTypeDef,
     UpdateThingGroupResponseTypeDef,
     UpdateThingGroupsForThingRequestRequestTypeDef,
     UpdateTopicRuleDestinationRequestRequestTypeDef,
     ValidationErrorTypeDef,
+    AbortConfigOutputTypeDef,
     AbortConfigTypeDef,
     MetricDatumTypeDef,
     DescribeFleetMetricResponseTypeDef,
     UpdateFleetMetricRequestRequestTypeDef,
     AllowedTypeDef,
     ExplicitDenyTypeDef,
     ImplicitDenyTypeDef,
     ListAttachedPoliciesResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListPrincipalPoliciesResponseTypeDef,
+    AssetPropertyValueOutputTypeDef,
     AssetPropertyValueTypeDef,
+    ThingGroupPropertiesOutputTypeDef,
     CreateThingRequestRequestTypeDef,
     ThingGroupPropertiesTypeDef,
     UpdateThingRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
     StartAuditMitigationActionsTaskRequestRequestTypeDef,
     DescribeAccountAuditConfigurationResponseTypeDef,
     UpdateAccountAuditConfigurationRequestRequestTypeDef,
     ListAuditTasksResponseTypeDef,
     TestAuthorizationRequestRequestTypeDef,
     DescribeAuthorizerResponseTypeDef,
     DescribeDefaultAuthorizerResponseTypeDef,
     ListAuthorizersResponseTypeDef,
     AwsJobAbortConfigTypeDef,
+    AwsJobExponentialRolloutRateOutputTypeDef,
     AwsJobExponentialRolloutRateTypeDef,
+    BehaviorCriteriaOutputTypeDef,
     BehaviorCriteriaTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
+    MetricToRetainOutputTypeDef,
     MetricToRetainTypeDef,
     DescribeBillingGroupResponseTypeDef,
     UpdateBillingGroupRequestRequestTypeDef,
     GetBucketsAggregationResponseTypeDef,
     BucketsAggregationTypeTypeDef,
     CACertificateDescriptionTypeDef,
     ListCACertificatesResponseTypeDef,
     CertificateDescriptionTypeDef,
     ListCertificatesByCAResponseTypeDef,
     ListCertificatesResponseTypeDef,
+    CustomCodeSigningOutputTypeDef,
     CustomCodeSigningTypeDef,
     DescribeEventConfigurationsResponseTypeDef,
     UpdateEventConfigurationsRequestRequestTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     CreateBillingGroupRequestRequestTypeDef,
     CreateCustomMetricRequestRequestTypeDef,
     CreateDimensionRequestRequestTypeDef,
     CreateFleetMetricRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreateRoleAliasRequestRequestTypeDef,
     CreateScheduledAuditRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainConfigurationRequestRequestTypeDef,
     UpdateDomainConfigurationRequestRequestTypeDef,
     SchedulingConfigTypeDef,
     CreateKeysAndCertificateResponseTypeDef,
     CreateProvisioningClaimResponseTypeDef,
     CreateProvisioningTemplateRequestRequestTypeDef,
-    DescribeProvisioningTemplateResponseTypeDef,
     UpdateProvisioningTemplateRequestRequestTypeDef,
     CreateThingTypeRequestRequestTypeDef,
     DescribeAuditTaskResponseTypeDef,
-    RegisterCACertificateRequestRequestTypeDef,
-    UpdateCACertificateRequestRequestTypeDef,
     DescribeDomainConfigurationResponseTypeDef,
+    SchedulingConfigOutputTypeDef,
     DescribeManagedJobTemplateResponseTypeDef,
+    DescribeProvisioningTemplateResponseTypeDef,
     DescribeRoleAliasResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
     ThingTypeDefinitionTypeDef,
+    DestinationOutputTypeDef,
     DestinationTypeDef,
     ListDetectMitigationActionsExecutionsResponseTypeDef,
-    StartDetectMitigationActionsTaskRequestRequestTypeDef,
     ListDomainConfigurationsResponseTypeDef,
+    DynamoDBv2ActionOutputTypeDef,
     DynamoDBv2ActionTypeDef,
     GetEffectivePoliciesResponseTypeDef,
+    ExponentialRolloutRateOutputTypeDef,
     ExponentialRolloutRateTypeDef,
+    ThingGroupIndexingConfigurationOutputTypeDef,
     ThingGroupIndexingConfigurationTypeDef,
+    StreamFileOutputTypeDef,
+    FileLocationOutputTypeDef,
     StreamFileTypeDef,
     FileLocationTypeDef,
     ListFleetMetricsResponseTypeDef,
     GetPackageConfigurationResponseTypeDef,
-    UpdatePackageConfigurationRequestRequestTypeDef,
     GetPercentilesResponseTypeDef,
     GetStatisticsResponseTypeDef,
     ListBillingGroupsResponseTypeDef,
     ListThingGroupsForThingResponseTypeDef,
     ListThingGroupsResponseTypeDef,
     ThingGroupMetadataTypeDef,
+    HttpAuthorizationOutputTypeDef,
     HttpAuthorizationTypeDef,
+    ThingIndexingConfigurationOutputTypeDef,
     ThingIndexingConfigurationTypeDef,
     JobExecutionTypeDef,
     JobExecutionSummaryForJobTypeDef,
     JobExecutionSummaryForThingTypeDef,
+    JobExecutionsRetryConfigOutputTypeDef,
     JobExecutionsRetryConfigTypeDef,
     ListJobsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedJobTemplatesResponseTypeDef,
     ListMitigationActionsResponseTypeDef,
     ListOTAUpdatesResponseTypeDef,
     ListOutgoingCertificatesResponseTypeDef,
@@ -1184,124 +1301,145 @@
     ListPackagesResponseTypeDef,
     ListPolicyVersionsResponseTypeDef,
     ListProvisioningTemplateVersionsResponseTypeDef,
     ListProvisioningTemplatesResponseTypeDef,
     ListScheduledAuditsResponseTypeDef,
     ListSecurityProfilesResponseTypeDef,
     ListStreamsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTargetsForSecurityProfileResponseTypeDef,
     SecurityProfileTargetMappingTypeDef,
     ListThingsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
+    LocationActionOutputTypeDef,
     LocationActionTypeDef,
     LogTargetConfigurationTypeDef,
     SetV2LoggingLevelRequestRequestTypeDef,
     SetLoggingOptionsRequestRequestTypeDef,
+    MitigationActionParamsOutputTypeDef,
     MitigationActionParamsTypeDef,
+    MqttHeadersOutputTypeDef,
     MqttHeadersTypeDef,
+    ResourceIdentifierOutputTypeDef,
     ResourceIdentifierTypeDef,
+    RegisterCACertificateRequestRequestTypeDef,
+    UpdateCACertificateRequestRequestTypeDef,
+    StartDetectMitigationActionsTaskRequestRequestTypeDef,
     TestInvokeAuthorizerRequestRequestTypeDef,
     ThingDocumentTypeDef,
+    TimestreamActionOutputTypeDef,
     TimestreamActionTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRuleDestinationSummaryTypeDef,
     TopicRuleDestinationTypeDef,
+    UpdatePackageConfigurationRequestRequestTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
     ListMetricValuesResponseTypeDef,
     DeniedTypeDef,
+    PutAssetPropertyValueEntryOutputTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     CreateDynamicThingGroupRequestRequestTypeDef,
     CreateThingGroupRequestRequestTypeDef,
     UpdateDynamicThingGroupRequestRequestTypeDef,
     UpdateThingGroupRequestRequestTypeDef,
+    AwsJobExecutionsRolloutConfigOutputTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
+    BehaviorOutputTypeDef,
     BehaviorTypeDef,
     GetBucketsAggregationRequestRequestTypeDef,
     DescribeCACertificateResponseTypeDef,
     DescribeCertificateResponseTypeDef,
     ListThingTypesResponseTypeDef,
+    StartSigningJobParameterOutputTypeDef,
     StartSigningJobParameterTypeDef,
+    JobExecutionsRolloutConfigOutputTypeDef,
     JobExecutionsRolloutConfigTypeDef,
-    CreateStreamRequestRequestTypeDef,
     StreamInfoTypeDef,
+    CreateStreamRequestRequestTypeDef,
     UpdateStreamRequestRequestTypeDef,
     DescribeThingGroupResponseTypeDef,
+    HttpActionOutputTypeDef,
     HttpActionTypeDef,
     GetIndexingConfigurationResponseTypeDef,
     UpdateIndexingConfigurationRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
     ListJobExecutionsForJobResponseTypeDef,
     ListJobExecutionsForThingResponseTypeDef,
     ListSecurityProfilesForTargetResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
-    CreateMitigationActionRequestRequestTypeDef,
     DescribeMitigationActionResponseTypeDef,
     MitigationActionTypeDef,
+    CreateMitigationActionRequestRequestTypeDef,
     UpdateMitigationActionRequestRequestTypeDef,
+    RepublishActionOutputTypeDef,
     RepublishActionTypeDef,
     AuditSuppressionTypeDef,
+    DescribeAuditSuppressionResponseTypeDef,
+    NonCompliantResourceTypeDef,
+    RelatedResourceTypeDef,
     CreateAuditSuppressionRequestRequestTypeDef,
     DeleteAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionRequestRequestTypeDef,
-    DescribeAuditSuppressionResponseTypeDef,
     ListAuditFindingsRequestListAuditFindingsPaginateTypeDef,
     ListAuditFindingsRequestRequestTypeDef,
     ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef,
     ListAuditSuppressionsRequestRequestTypeDef,
-    NonCompliantResourceTypeDef,
-    RelatedResourceTypeDef,
     UpdateAuditSuppressionRequestRequestTypeDef,
     SearchIndexResponseTypeDef,
     CreateTopicRuleDestinationRequestRequestTypeDef,
     ListTopicRuleDestinationsResponseTypeDef,
     CreateTopicRuleDestinationResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     AuthResultTypeDef,
+    IotSiteWiseActionOutputTypeDef,
     IotSiteWiseActionTypeDef,
     ActiveViolationTypeDef,
-    CreateSecurityProfileRequestRequestTypeDef,
     DescribeSecurityProfileResponseTypeDef,
-    UpdateSecurityProfileRequestRequestTypeDef,
     UpdateSecurityProfileResponseTypeDef,
-    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
     ViolationEventTypeDef,
+    CreateSecurityProfileRequestRequestTypeDef,
+    UpdateSecurityProfileRequestRequestTypeDef,
+    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
+    CodeSigningOutputTypeDef,
     CodeSigningTypeDef,
-    CreateJobRequestRequestTypeDef,
-    CreateJobTemplateRequestRequestTypeDef,
     DescribeJobTemplateResponseTypeDef,
     JobTypeDef,
+    CreateJobRequestRequestTypeDef,
+    CreateJobTemplateRequestRequestTypeDef,
     UpdateJobRequestRequestTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeAuditMitigationActionsTaskResponseTypeDef,
     DetectMitigationActionsTaskSummaryTypeDef,
     ListAuditSuppressionsResponseTypeDef,
     AuditFindingTypeDef,
     ListRelatedResourcesForAuditFindingResponseTypeDef,
     TestAuthorizationResponseTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
+    OTAUpdateFileOutputTypeDef,
     OTAUpdateFileTypeDef,
     DescribeJobResponseTypeDef,
     DescribeDetectMitigationActionsTaskResponseTypeDef,
     ListDetectMitigationActionsTasksResponseTypeDef,
     DescribeAuditFindingResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
-    TopicRulePayloadTypeDef,
     TopicRuleTypeDef,
-    CreateOTAUpdateRequestRequestTypeDef,
+    TopicRulePayloadTypeDef,
     OTAUpdateInfoTypeDef,
+    CreateOTAUpdateRequestRequestTypeDef,
+    GetTopicRuleResponseTypeDef,
     CreateTopicRuleRequestRequestTypeDef,
     ReplaceTopicRuleRequestRequestTypeDef,
-    GetTopicRuleResponseTypeDef,
     GetOTAUpdateResponseTypeDef,
 )
 
 
-def get_structure() -> AbortCriteriaTypeDef:
+def get_structure() -> AbortCriteriaOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-1.28.0/mypy_boto3_iot/__init__.py` & `mypy-boto3-iot-1.28.12/mypy_boto3_iot/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.0/mypy_boto3_iot/__init__.pyi` & `mypy-boto3-iot-1.28.12/mypy_boto3_iot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.0/mypy_boto3_iot/__main__.py` & `mypy-boto3-iot-1.28.12/mypy_boto3_iot/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoT 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.IoT 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT\nOther"
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

### Comparing `mypy-boto3-iot-1.28.0/mypy_boto3_iot/client.py` & `mypy-boto3-iot-1.28.12/mypy_boto3_iot/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.0/mypy_boto3_iot/client.pyi` & `mypy-boto3-iot-1.28.12/mypy_boto3_iot/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.0/mypy_boto3_iot/literals.py` & `mypy-boto3-iot-1.28.12/mypy_boto3_iot/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -507,14 +507,15 @@
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
@@ -593,26 +594,28 @@
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

### Comparing `mypy-boto3-iot-1.28.0/mypy_boto3_iot/literals.pyi` & `mypy-boto3-iot-1.28.12/mypy_boto3_iot/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -505,14 +505,15 @@
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
@@ -591,26 +592,28 @@
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

### Comparing `mypy-boto3-iot-1.28.0/mypy_boto3_iot/paginator.py` & `mypy-boto3-iot-1.28.12/mypy_boto3_iot/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.0/mypy_boto3_iot/paginator.pyi` & `mypy-boto3-iot-1.28.12/mypy_boto3_iot/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.0/mypy_boto3_iot/type_defs.py` & `mypy-boto3-iot-1.28.12/mypy_boto3_iot/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iot service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iot.type_defs import AbortCriteriaTypeDef
+    from mypy_boto3_iot.type_defs import AbortCriteriaOutputTypeDef
 
-    data: AbortCriteriaTypeDef = {...}
+    data: AbortCriteriaOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -89,16 +89,34 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AbortCriteriaOutputTypeDef",
     "AbortCriteriaTypeDef",
     "AcceptCertificateTransferRequestRequestTypeDef",
+    "CloudwatchAlarmActionOutputTypeDef",
+    "CloudwatchLogsActionOutputTypeDef",
+    "CloudwatchMetricActionOutputTypeDef",
+    "DynamoDBActionOutputTypeDef",
+    "ElasticsearchActionOutputTypeDef",
+    "FirehoseActionOutputTypeDef",
+    "IotAnalyticsActionOutputTypeDef",
+    "IotEventsActionOutputTypeDef",
+    "KafkaActionOutputTypeDef",
+    "KinesisActionOutputTypeDef",
+    "LambdaActionOutputTypeDef",
+    "OpenSearchActionOutputTypeDef",
+    "S3ActionOutputTypeDef",
+    "SalesforceActionOutputTypeDef",
+    "SnsActionOutputTypeDef",
+    "SqsActionOutputTypeDef",
+    "StepFunctionsActionOutputTypeDef",
     "CloudwatchAlarmActionTypeDef",
     "CloudwatchLogsActionTypeDef",
     "CloudwatchMetricActionTypeDef",
     "DynamoDBActionTypeDef",
     "ElasticsearchActionTypeDef",
     "FirehoseActionTypeDef",
     "IotAnalyticsActionTypeDef",
@@ -108,67 +126,88 @@
     "LambdaActionTypeDef",
     "OpenSearchActionTypeDef",
     "S3ActionTypeDef",
     "SalesforceActionTypeDef",
     "SnsActionTypeDef",
     "SqsActionTypeDef",
     "StepFunctionsActionTypeDef",
-    "MetricValueTypeDef",
+    "MetricValueOutputTypeDef",
     "ViolationEventAdditionalInfoTypeDef",
     "AddThingToBillingGroupRequestRequestTypeDef",
     "AddThingToThingGroupRequestRequestTypeDef",
+    "AddThingsToThingGroupParamsOutputTypeDef",
     "AddThingsToThingGroupParamsTypeDef",
+    "AggregationTypeOutputTypeDef",
     "AggregationTypeTypeDef",
+    "AlertTargetOutputTypeDef",
     "AlertTargetTypeDef",
     "PolicyTypeDef",
+    "AssetPropertyTimestampOutputTypeDef",
     "AssetPropertyTimestampTypeDef",
+    "AssetPropertyVariantOutputTypeDef",
     "AssetPropertyVariantTypeDef",
     "AssociateTargetsWithJobRequestRequestTypeDef",
     "AssociateTargetsWithJobResponseTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachPrincipalPolicyRequestRequestTypeDef",
     "AttachSecurityProfileRequestRequestTypeDef",
     "AttachThingPrincipalRequestRequestTypeDef",
+    "AttributePayloadOutputTypeDef",
     "AttributePayloadTypeDef",
+    "AuditCheckConfigurationOutputTypeDef",
     "AuditCheckConfigurationTypeDef",
     "AuditCheckDetailsTypeDef",
     "AuditMitigationActionExecutionMetadataTypeDef",
     "AuditMitigationActionsTaskMetadataTypeDef",
+    "AuditMitigationActionsTaskTargetOutputTypeDef",
     "AuditMitigationActionsTaskTargetTypeDef",
+    "AuditNotificationTargetOutputTypeDef",
     "AuditNotificationTargetTypeDef",
     "AuditTaskMetadataTypeDef",
+    "AuthInfoOutputTypeDef",
     "AuthInfoTypeDef",
+    "AuthorizerConfigOutputTypeDef",
     "AuthorizerConfigTypeDef",
     "AuthorizerDescriptionTypeDef",
     "AuthorizerSummaryTypeDef",
     "AwsJobAbortCriteriaTypeDef",
+    "AwsJobRateIncreaseCriteriaOutputTypeDef",
     "AwsJobRateIncreaseCriteriaTypeDef",
+    "AwsJobPresignedUrlConfigOutputTypeDef",
     "AwsJobPresignedUrlConfigTypeDef",
     "AwsJobTimeoutConfigTypeDef",
+    "MachineLearningDetectionConfigOutputTypeDef",
+    "StatisticalThresholdOutputTypeDef",
     "MachineLearningDetectionConfigTypeDef",
+    "MetricValueTypeDef",
     "StatisticalThresholdTypeDef",
     "BehaviorModelTrainingSummaryTypeDef",
+    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "BillingGroupMetadataTypeDef",
+    "BillingGroupPropertiesOutputTypeDef",
     "BillingGroupPropertiesTypeDef",
     "BucketTypeDef",
     "TermsAggregationTypeDef",
     "CertificateValidityTypeDef",
     "CACertificateTypeDef",
     "CancelAuditMitigationActionsTaskRequestRequestTypeDef",
     "CancelAuditTaskRequestRequestTypeDef",
     "CancelCertificateTransferRequestRequestTypeDef",
     "CancelDetectMitigationActionsTaskRequestRequestTypeDef",
     "CancelJobExecutionRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "CancelJobResponseTypeDef",
     "TransferDataTypeDef",
     "CertificateTypeDef",
+    "CodeSigningCertificateChainOutputTypeDef",
     "CodeSigningCertificateChainTypeDef",
+    "CodeSigningSignatureOutputTypeDef",
     "CodeSigningSignatureTypeDef",
+    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
     "TagTypeDef",
     "CreateAuthorizerResponseTypeDef",
     "CreateBillingGroupResponseTypeDef",
     "CreateCertificateFromCsrRequestRequestTypeDef",
     "CreateCertificateFromCsrResponseTypeDef",
@@ -243,35 +282,40 @@
     "DescribeAuditMitigationActionsTaskRequestRequestTypeDef",
     "TaskStatisticsForAuditCheckTypeDef",
     "DescribeAuditTaskRequestRequestTypeDef",
     "TaskStatisticsTypeDef",
     "DescribeAuthorizerRequestRequestTypeDef",
     "DescribeBillingGroupRequestRequestTypeDef",
     "DescribeCACertificateRequestRequestTypeDef",
-    "RegistrationConfigTypeDef",
+    "RegistrationConfigOutputTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "DescribeCustomMetricRequestRequestTypeDef",
     "DescribeCustomMetricResponseTypeDef",
     "DescribeDetectMitigationActionsTaskRequestRequestTypeDef",
     "DescribeDimensionRequestRequestTypeDef",
     "DescribeDimensionResponseTypeDef",
     "DescribeDomainConfigurationRequestRequestTypeDef",
     "ServerCertificateSummaryTypeDef",
+    "TlsConfigOutputTypeDef",
     "DescribeEndpointRequestRequestTypeDef",
     "DescribeEndpointResponseTypeDef",
     "DescribeFleetMetricRequestRequestTypeDef",
     "DescribeIndexRequestRequestTypeDef",
     "DescribeIndexResponseTypeDef",
     "DescribeJobExecutionRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
+    "MaintenanceWindowOutputTypeDef",
+    "PresignedUrlConfigOutputTypeDef",
+    "TimeoutConfigOutputTypeDef",
     "DescribeManagedJobTemplateRequestRequestTypeDef",
     "DocumentParameterTypeDef",
     "DescribeMitigationActionRequestRequestTypeDef",
     "DescribeProvisioningTemplateRequestRequestTypeDef",
+    "ProvisioningHookOutputTypeDef",
     "DescribeProvisioningTemplateVersionRequestRequestTypeDef",
     "DescribeProvisioningTemplateVersionResponseTypeDef",
     "DescribeRoleAliasRequestRequestTypeDef",
     "RoleAliasDescriptionTypeDef",
     "DescribeScheduledAuditRequestRequestTypeDef",
     "DescribeScheduledAuditResponseTypeDef",
     "DescribeSecurityProfileRequestRequestTypeDef",
@@ -279,46 +323,55 @@
     "DescribeThingGroupRequestRequestTypeDef",
     "DescribeThingRegistrationTaskRequestRequestTypeDef",
     "DescribeThingRegistrationTaskResponseTypeDef",
     "DescribeThingRequestRequestTypeDef",
     "DescribeThingResponseTypeDef",
     "DescribeThingTypeRequestRequestTypeDef",
     "ThingTypeMetadataTypeDef",
+    "ThingTypePropertiesOutputTypeDef",
+    "S3DestinationOutputTypeDef",
     "S3DestinationTypeDef",
     "DetachPolicyRequestRequestTypeDef",
     "DetachPrincipalPolicyRequestRequestTypeDef",
     "DetachSecurityProfileRequestRequestTypeDef",
     "DetachThingPrincipalRequestRequestTypeDef",
     "DetectMitigationActionExecutionTypeDef",
     "DetectMitigationActionsTaskStatisticsTypeDef",
+    "DetectMitigationActionsTaskTargetOutputTypeDef",
+    "ViolationEventOccurrenceRangeOutputTypeDef",
     "DetectMitigationActionsTaskTargetTypeDef",
-    "ViolationEventOccurrenceRangeTypeDef",
     "DisableTopicRuleRequestRequestTypeDef",
     "DomainConfigurationSummaryTypeDef",
+    "PutItemInputOutputTypeDef",
     "PutItemInputTypeDef",
     "EffectivePolicyTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EnableIoTLoggingParamsOutputTypeDef",
     "EnableIoTLoggingParamsTypeDef",
     "EnableTopicRuleRequestRequestTypeDef",
     "ErrorInfoTypeDef",
+    "RateIncreaseCriteriaOutputTypeDef",
     "RateIncreaseCriteriaTypeDef",
+    "FieldOutputTypeDef",
     "FieldTypeDef",
+    "S3LocationOutputTypeDef",
+    "StreamOutputTypeDef",
     "S3LocationTypeDef",
     "StreamTypeDef",
     "FleetMetricNameAndArnTypeDef",
     "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
     "GetBehaviorModelTrainingSummariesRequestRequestTypeDef",
     "GetCardinalityRequestRequestTypeDef",
     "GetCardinalityResponseTypeDef",
     "GetEffectivePoliciesRequestRequestTypeDef",
     "GetJobDocumentRequestRequestTypeDef",
     "GetJobDocumentResponseTypeDef",
     "GetLoggingOptionsResponseTypeDef",
     "GetOTAUpdateRequestRequestTypeDef",
-    "VersionUpdateByJobsConfigTypeDef",
+    "VersionUpdateByJobsConfigOutputTypeDef",
     "GetPackageRequestRequestTypeDef",
     "GetPackageResponseTypeDef",
     "GetPackageVersionRequestRequestTypeDef",
     "GetPackageVersionResponseTypeDef",
     "GetPercentilesRequestRequestTypeDef",
     "PercentPairTypeDef",
     "GetPolicyRequestRequestTypeDef",
@@ -328,24 +381,29 @@
     "GetRegistrationCodeResponseTypeDef",
     "GetStatisticsRequestRequestTypeDef",
     "StatisticsTypeDef",
     "GetTopicRuleDestinationRequestRequestTypeDef",
     "GetTopicRuleRequestRequestTypeDef",
     "GetV2LoggingOptionsResponseTypeDef",
     "GroupNameAndArnTypeDef",
+    "HttpActionHeaderOutputTypeDef",
     "HttpActionHeaderTypeDef",
+    "SigV4AuthorizationOutputTypeDef",
     "SigV4AuthorizationTypeDef",
     "HttpContextTypeDef",
     "HttpUrlDestinationConfigurationTypeDef",
     "HttpUrlDestinationPropertiesTypeDef",
     "HttpUrlDestinationSummaryTypeDef",
+    "IndexingFilterOutputTypeDef",
     "IndexingFilterTypeDef",
+    "IssuerCertificateIdentifierOutputTypeDef",
     "IssuerCertificateIdentifierTypeDef",
     "JobExecutionStatusDetailsTypeDef",
     "JobExecutionSummaryTypeDef",
+    "RetryCriteriaOutputTypeDef",
     "RetryCriteriaTypeDef",
     "JobProcessDetailsTypeDef",
     "JobSummaryTypeDef",
     "JobTemplateSummaryTypeDef",
     "ScheduledJobRolloutTypeDef",
     "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
     "ListActiveViolationsRequestRequestTypeDef",
@@ -444,14 +502,15 @@
     "ListSecurityProfilesRequestRequestTypeDef",
     "SecurityProfileIdentifierTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "StreamSummaryTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
     "ListTargetsForPolicyRequestRequestTypeDef",
     "ListTargetsForPolicyResponseTypeDef",
     "ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
     "ListTargetsForSecurityProfileRequestRequestTypeDef",
     "SecurityProfileTargetTypeDef",
     "ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
@@ -483,26 +542,35 @@
     "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
     "ListTopicRulesRequestRequestTypeDef",
     "TopicRuleListItemTypeDef",
     "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
     "ListV2LoggingLevelsRequestRequestTypeDef",
     "ListViolationEventsRequestListViolationEventsPaginateTypeDef",
     "ListViolationEventsRequestRequestTypeDef",
+    "LocationTimestampOutputTypeDef",
     "LocationTimestampTypeDef",
+    "LogTargetOutputTypeDef",
     "LogTargetTypeDef",
     "LoggingOptionsPayloadTypeDef",
+    "PublishFindingToSnsParamsOutputTypeDef",
+    "ReplaceDefaultPolicyVersionParamsOutputTypeDef",
+    "UpdateCACertificateParamsOutputTypeDef",
+    "UpdateDeviceCertificateParamsOutputTypeDef",
     "PublishFindingToSnsParamsTypeDef",
     "ReplaceDefaultPolicyVersionParamsTypeDef",
     "UpdateCACertificateParamsTypeDef",
     "UpdateDeviceCertificateParamsTypeDef",
     "MqttContextTypeDef",
+    "UserPropertyOutputTypeDef",
     "UserPropertyTypeDef",
     "PaginatorConfigTypeDef",
+    "PolicyVersionIdentifierOutputTypeDef",
     "PolicyVersionIdentifierTypeDef",
     "PutVerificationStateOnViolationRequestRequestTypeDef",
+    "RegistrationConfigTypeDef",
     "RegisterCACertificateResponseTypeDef",
     "RegisterCertificateRequestRequestTypeDef",
     "RegisterCertificateResponseTypeDef",
     "RegisterCertificateWithoutCARequestRequestTypeDef",
     "RegisterCertificateWithoutCAResponseTypeDef",
     "RegisterThingRequestRequestTypeDef",
     "RegisterThingResponseTypeDef",
@@ -512,25 +580,29 @@
     "ResponseMetadataTypeDef",
     "SearchIndexRequestRequestTypeDef",
     "ThingGroupDocumentTypeDef",
     "SetDefaultAuthorizerRequestRequestTypeDef",
     "SetDefaultAuthorizerResponseTypeDef",
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     "SetV2LoggingOptionsRequestRequestTypeDef",
+    "SigningProfileParameterOutputTypeDef",
     "SigningProfileParameterTypeDef",
     "StartAuditMitigationActionsTaskResponseTypeDef",
+    "ViolationEventOccurrenceRangeTypeDef",
     "StartDetectMitigationActionsTaskResponseTypeDef",
     "StartOnDemandAuditTaskRequestRequestTypeDef",
     "StartOnDemandAuditTaskResponseTypeDef",
     "StartThingRegistrationTaskRequestRequestTypeDef",
     "StartThingRegistrationTaskResponseTypeDef",
     "StopThingRegistrationTaskRequestRequestTypeDef",
     "TlsContextTypeDef",
     "TestInvokeAuthorizerResponseTypeDef",
     "ThingConnectivityTypeDef",
+    "TimestreamDimensionOutputTypeDef",
+    "TimestreamTimestampOutputTypeDef",
     "TimestreamDimensionTypeDef",
     "TimestreamTimestampTypeDef",
     "VpcDestinationConfigurationTypeDef",
     "VpcDestinationSummaryTypeDef",
     "VpcDestinationPropertiesTypeDef",
     "TransferCertificateRequestRequestTypeDef",
     "TransferCertificateResponseTypeDef",
@@ -542,117 +614,130 @@
     "UpdateCustomMetricRequestRequestTypeDef",
     "UpdateCustomMetricResponseTypeDef",
     "UpdateDimensionRequestRequestTypeDef",
     "UpdateDimensionResponseTypeDef",
     "UpdateDomainConfigurationResponseTypeDef",
     "UpdateDynamicThingGroupResponseTypeDef",
     "UpdateMitigationActionResponseTypeDef",
+    "VersionUpdateByJobsConfigTypeDef",
     "UpdatePackageRequestRequestTypeDef",
     "UpdatePackageVersionRequestRequestTypeDef",
     "UpdateRoleAliasRequestRequestTypeDef",
     "UpdateRoleAliasResponseTypeDef",
     "UpdateScheduledAuditRequestRequestTypeDef",
     "UpdateScheduledAuditResponseTypeDef",
     "UpdateStreamResponseTypeDef",
     "UpdateThingGroupResponseTypeDef",
     "UpdateThingGroupsForThingRequestRequestTypeDef",
     "UpdateTopicRuleDestinationRequestRequestTypeDef",
     "ValidationErrorTypeDef",
+    "AbortConfigOutputTypeDef",
     "AbortConfigTypeDef",
     "MetricDatumTypeDef",
     "DescribeFleetMetricResponseTypeDef",
     "UpdateFleetMetricRequestRequestTypeDef",
     "AllowedTypeDef",
     "ExplicitDenyTypeDef",
     "ImplicitDenyTypeDef",
     "ListAttachedPoliciesResponseTypeDef",
     "ListPoliciesResponseTypeDef",
     "ListPrincipalPoliciesResponseTypeDef",
+    "AssetPropertyValueOutputTypeDef",
     "AssetPropertyValueTypeDef",
+    "ThingGroupPropertiesOutputTypeDef",
     "CreateThingRequestRequestTypeDef",
     "ThingGroupPropertiesTypeDef",
     "UpdateThingRequestRequestTypeDef",
     "ListAuditMitigationActionsExecutionsResponseTypeDef",
     "ListAuditMitigationActionsTasksResponseTypeDef",
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     "DescribeAccountAuditConfigurationResponseTypeDef",
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     "ListAuditTasksResponseTypeDef",
     "TestAuthorizationRequestRequestTypeDef",
     "DescribeAuthorizerResponseTypeDef",
     "DescribeDefaultAuthorizerResponseTypeDef",
     "ListAuthorizersResponseTypeDef",
     "AwsJobAbortConfigTypeDef",
+    "AwsJobExponentialRolloutRateOutputTypeDef",
     "AwsJobExponentialRolloutRateTypeDef",
+    "BehaviorCriteriaOutputTypeDef",
     "BehaviorCriteriaTypeDef",
     "GetBehaviorModelTrainingSummariesResponseTypeDef",
+    "MetricToRetainOutputTypeDef",
     "MetricToRetainTypeDef",
     "DescribeBillingGroupResponseTypeDef",
     "UpdateBillingGroupRequestRequestTypeDef",
     "GetBucketsAggregationResponseTypeDef",
     "BucketsAggregationTypeTypeDef",
     "CACertificateDescriptionTypeDef",
     "ListCACertificatesResponseTypeDef",
     "CertificateDescriptionTypeDef",
     "ListCertificatesByCAResponseTypeDef",
     "ListCertificatesResponseTypeDef",
+    "CustomCodeSigningOutputTypeDef",
     "CustomCodeSigningTypeDef",
     "DescribeEventConfigurationsResponseTypeDef",
     "UpdateEventConfigurationsRequestRequestTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
     "CreateBillingGroupRequestRequestTypeDef",
     "CreateCustomMetricRequestRequestTypeDef",
     "CreateDimensionRequestRequestTypeDef",
     "CreateFleetMetricRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreateRoleAliasRequestRequestTypeDef",
     "CreateScheduledAuditRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainConfigurationRequestRequestTypeDef",
     "UpdateDomainConfigurationRequestRequestTypeDef",
     "SchedulingConfigTypeDef",
     "CreateKeysAndCertificateResponseTypeDef",
     "CreateProvisioningClaimResponseTypeDef",
     "CreateProvisioningTemplateRequestRequestTypeDef",
-    "DescribeProvisioningTemplateResponseTypeDef",
     "UpdateProvisioningTemplateRequestRequestTypeDef",
     "CreateThingTypeRequestRequestTypeDef",
     "DescribeAuditTaskResponseTypeDef",
-    "RegisterCACertificateRequestRequestTypeDef",
-    "UpdateCACertificateRequestRequestTypeDef",
     "DescribeDomainConfigurationResponseTypeDef",
+    "SchedulingConfigOutputTypeDef",
     "DescribeManagedJobTemplateResponseTypeDef",
+    "DescribeProvisioningTemplateResponseTypeDef",
     "DescribeRoleAliasResponseTypeDef",
     "DescribeThingTypeResponseTypeDef",
     "ThingTypeDefinitionTypeDef",
+    "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "ListDetectMitigationActionsExecutionsResponseTypeDef",
-    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
     "ListDomainConfigurationsResponseTypeDef",
+    "DynamoDBv2ActionOutputTypeDef",
     "DynamoDBv2ActionTypeDef",
     "GetEffectivePoliciesResponseTypeDef",
+    "ExponentialRolloutRateOutputTypeDef",
     "ExponentialRolloutRateTypeDef",
+    "ThingGroupIndexingConfigurationOutputTypeDef",
     "ThingGroupIndexingConfigurationTypeDef",
+    "StreamFileOutputTypeDef",
+    "FileLocationOutputTypeDef",
     "StreamFileTypeDef",
     "FileLocationTypeDef",
     "ListFleetMetricsResponseTypeDef",
     "GetPackageConfigurationResponseTypeDef",
-    "UpdatePackageConfigurationRequestRequestTypeDef",
     "GetPercentilesResponseTypeDef",
     "GetStatisticsResponseTypeDef",
     "ListBillingGroupsResponseTypeDef",
     "ListThingGroupsForThingResponseTypeDef",
     "ListThingGroupsResponseTypeDef",
     "ThingGroupMetadataTypeDef",
+    "HttpAuthorizationOutputTypeDef",
     "HttpAuthorizationTypeDef",
+    "ThingIndexingConfigurationOutputTypeDef",
     "ThingIndexingConfigurationTypeDef",
     "JobExecutionTypeDef",
     "JobExecutionSummaryForJobTypeDef",
     "JobExecutionSummaryForThingTypeDef",
+    "JobExecutionsRetryConfigOutputTypeDef",
     "JobExecutionsRetryConfigTypeDef",
     "ListJobsResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
     "ListManagedJobTemplatesResponseTypeDef",
     "ListMitigationActionsResponseTypeDef",
     "ListOTAUpdatesResponseTypeDef",
     "ListOutgoingCertificatesResponseTypeDef",
@@ -660,122 +745,153 @@
     "ListPackagesResponseTypeDef",
     "ListPolicyVersionsResponseTypeDef",
     "ListProvisioningTemplateVersionsResponseTypeDef",
     "ListProvisioningTemplatesResponseTypeDef",
     "ListScheduledAuditsResponseTypeDef",
     "ListSecurityProfilesResponseTypeDef",
     "ListStreamsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTargetsForSecurityProfileResponseTypeDef",
     "SecurityProfileTargetMappingTypeDef",
     "ListThingsResponseTypeDef",
     "ListTopicRulesResponseTypeDef",
+    "LocationActionOutputTypeDef",
     "LocationActionTypeDef",
     "LogTargetConfigurationTypeDef",
     "SetV2LoggingLevelRequestRequestTypeDef",
     "SetLoggingOptionsRequestRequestTypeDef",
+    "MitigationActionParamsOutputTypeDef",
     "MitigationActionParamsTypeDef",
+    "MqttHeadersOutputTypeDef",
     "MqttHeadersTypeDef",
+    "ResourceIdentifierOutputTypeDef",
     "ResourceIdentifierTypeDef",
+    "RegisterCACertificateRequestRequestTypeDef",
+    "UpdateCACertificateRequestRequestTypeDef",
+    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
     "TestInvokeAuthorizerRequestRequestTypeDef",
     "ThingDocumentTypeDef",
+    "TimestreamActionOutputTypeDef",
     "TimestreamActionTypeDef",
     "TopicRuleDestinationConfigurationTypeDef",
     "TopicRuleDestinationSummaryTypeDef",
     "TopicRuleDestinationTypeDef",
+    "UpdatePackageConfigurationRequestRequestTypeDef",
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
     "ListMetricValuesResponseTypeDef",
     "DeniedTypeDef",
+    "PutAssetPropertyValueEntryOutputTypeDef",
     "PutAssetPropertyValueEntryTypeDef",
     "CreateDynamicThingGroupRequestRequestTypeDef",
     "CreateThingGroupRequestRequestTypeDef",
     "UpdateDynamicThingGroupRequestRequestTypeDef",
     "UpdateThingGroupRequestRequestTypeDef",
+    "AwsJobExecutionsRolloutConfigOutputTypeDef",
     "AwsJobExecutionsRolloutConfigTypeDef",
+    "BehaviorOutputTypeDef",
     "BehaviorTypeDef",
     "GetBucketsAggregationRequestRequestTypeDef",
     "DescribeCACertificateResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
     "ListThingTypesResponseTypeDef",
+    "StartSigningJobParameterOutputTypeDef",
     "StartSigningJobParameterTypeDef",
+    "JobExecutionsRolloutConfigOutputTypeDef",
     "JobExecutionsRolloutConfigTypeDef",
-    "CreateStreamRequestRequestTypeDef",
     "StreamInfoTypeDef",
+    "CreateStreamRequestRequestTypeDef",
     "UpdateStreamRequestRequestTypeDef",
     "DescribeThingGroupResponseTypeDef",
+    "HttpActionOutputTypeDef",
     "HttpActionTypeDef",
     "GetIndexingConfigurationResponseTypeDef",
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     "DescribeJobExecutionResponseTypeDef",
     "ListJobExecutionsForJobResponseTypeDef",
     "ListJobExecutionsForThingResponseTypeDef",
     "ListSecurityProfilesForTargetResponseTypeDef",
     "ListV2LoggingLevelsResponseTypeDef",
-    "CreateMitigationActionRequestRequestTypeDef",
     "DescribeMitigationActionResponseTypeDef",
     "MitigationActionTypeDef",
+    "CreateMitigationActionRequestRequestTypeDef",
     "UpdateMitigationActionRequestRequestTypeDef",
+    "RepublishActionOutputTypeDef",
     "RepublishActionTypeDef",
     "AuditSuppressionTypeDef",
+    "DescribeAuditSuppressionResponseTypeDef",
+    "NonCompliantResourceTypeDef",
+    "RelatedResourceTypeDef",
     "CreateAuditSuppressionRequestRequestTypeDef",
     "DeleteAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionRequestRequestTypeDef",
-    "DescribeAuditSuppressionResponseTypeDef",
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
     "ListAuditFindingsRequestRequestTypeDef",
     "ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef",
     "ListAuditSuppressionsRequestRequestTypeDef",
-    "NonCompliantResourceTypeDef",
-    "RelatedResourceTypeDef",
     "UpdateAuditSuppressionRequestRequestTypeDef",
     "SearchIndexResponseTypeDef",
     "CreateTopicRuleDestinationRequestRequestTypeDef",
     "ListTopicRuleDestinationsResponseTypeDef",
     "CreateTopicRuleDestinationResponseTypeDef",
     "GetTopicRuleDestinationResponseTypeDef",
     "AuthResultTypeDef",
+    "IotSiteWiseActionOutputTypeDef",
     "IotSiteWiseActionTypeDef",
     "ActiveViolationTypeDef",
-    "CreateSecurityProfileRequestRequestTypeDef",
     "DescribeSecurityProfileResponseTypeDef",
-    "UpdateSecurityProfileRequestRequestTypeDef",
     "UpdateSecurityProfileResponseTypeDef",
-    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
     "ViolationEventTypeDef",
+    "CreateSecurityProfileRequestRequestTypeDef",
+    "UpdateSecurityProfileRequestRequestTypeDef",
+    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
+    "CodeSigningOutputTypeDef",
     "CodeSigningTypeDef",
-    "CreateJobRequestRequestTypeDef",
-    "CreateJobTemplateRequestRequestTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "JobTypeDef",
+    "CreateJobRequestRequestTypeDef",
+    "CreateJobTemplateRequestRequestTypeDef",
     "UpdateJobRequestRequestTypeDef",
     "DescribeStreamResponseTypeDef",
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     "DetectMitigationActionsTaskSummaryTypeDef",
     "ListAuditSuppressionsResponseTypeDef",
     "AuditFindingTypeDef",
     "ListRelatedResourcesForAuditFindingResponseTypeDef",
     "TestAuthorizationResponseTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListActiveViolationsResponseTypeDef",
     "ListViolationEventsResponseTypeDef",
+    "OTAUpdateFileOutputTypeDef",
     "OTAUpdateFileTypeDef",
     "DescribeJobResponseTypeDef",
     "DescribeDetectMitigationActionsTaskResponseTypeDef",
     "ListDetectMitigationActionsTasksResponseTypeDef",
     "DescribeAuditFindingResponseTypeDef",
     "ListAuditFindingsResponseTypeDef",
-    "TopicRulePayloadTypeDef",
     "TopicRuleTypeDef",
-    "CreateOTAUpdateRequestRequestTypeDef",
+    "TopicRulePayloadTypeDef",
     "OTAUpdateInfoTypeDef",
+    "CreateOTAUpdateRequestRequestTypeDef",
+    "GetTopicRuleResponseTypeDef",
     "CreateTopicRuleRequestRequestTypeDef",
     "ReplaceTopicRuleRequestRequestTypeDef",
-    "GetTopicRuleResponseTypeDef",
     "GetOTAUpdateResponseTypeDef",
 )
 
+AbortCriteriaOutputTypeDef = TypedDict(
+    "AbortCriteriaOutputTypeDef",
+    {
+        "failureType": JobExecutionFailureTypeType,
+        "action": Literal["CANCEL"],
+        "thresholdPercentage": float,
+        "minNumberOfExecutedThings": int,
+    },
+)
+
 AbortCriteriaTypeDef = TypedDict(
     "AbortCriteriaTypeDef",
     {
         "failureType": JobExecutionFailureTypeType,
         "action": Literal["CANCEL"],
         "thresholdPercentage": float,
         "minNumberOfExecutedThings": int,
@@ -800,14 +916,323 @@
 class AcceptCertificateTransferRequestRequestTypeDef(
     _RequiredAcceptCertificateTransferRequestRequestTypeDef,
     _OptionalAcceptCertificateTransferRequestRequestTypeDef,
 ):
     pass
 
 
+CloudwatchAlarmActionOutputTypeDef = TypedDict(
+    "CloudwatchAlarmActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "alarmName": str,
+        "stateReason": str,
+        "stateValue": str,
+    },
+)
+
+_RequiredCloudwatchLogsActionOutputTypeDef = TypedDict(
+    "_RequiredCloudwatchLogsActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "logGroupName": str,
+    },
+)
+_OptionalCloudwatchLogsActionOutputTypeDef = TypedDict(
+    "_OptionalCloudwatchLogsActionOutputTypeDef",
+    {
+        "batchMode": bool,
+    },
+    total=False,
+)
+
+
+class CloudwatchLogsActionOutputTypeDef(
+    _RequiredCloudwatchLogsActionOutputTypeDef, _OptionalCloudwatchLogsActionOutputTypeDef
+):
+    pass
+
+
+_RequiredCloudwatchMetricActionOutputTypeDef = TypedDict(
+    "_RequiredCloudwatchMetricActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "metricNamespace": str,
+        "metricName": str,
+        "metricValue": str,
+        "metricUnit": str,
+    },
+)
+_OptionalCloudwatchMetricActionOutputTypeDef = TypedDict(
+    "_OptionalCloudwatchMetricActionOutputTypeDef",
+    {
+        "metricTimestamp": str,
+    },
+    total=False,
+)
+
+
+class CloudwatchMetricActionOutputTypeDef(
+    _RequiredCloudwatchMetricActionOutputTypeDef, _OptionalCloudwatchMetricActionOutputTypeDef
+):
+    pass
+
+
+_RequiredDynamoDBActionOutputTypeDef = TypedDict(
+    "_RequiredDynamoDBActionOutputTypeDef",
+    {
+        "tableName": str,
+        "roleArn": str,
+        "hashKeyField": str,
+        "hashKeyValue": str,
+    },
+)
+_OptionalDynamoDBActionOutputTypeDef = TypedDict(
+    "_OptionalDynamoDBActionOutputTypeDef",
+    {
+        "operation": str,
+        "hashKeyType": DynamoKeyTypeType,
+        "rangeKeyField": str,
+        "rangeKeyValue": str,
+        "rangeKeyType": DynamoKeyTypeType,
+        "payloadField": str,
+    },
+    total=False,
+)
+
+
+class DynamoDBActionOutputTypeDef(
+    _RequiredDynamoDBActionOutputTypeDef, _OptionalDynamoDBActionOutputTypeDef
+):
+    pass
+
+
+ElasticsearchActionOutputTypeDef = TypedDict(
+    "ElasticsearchActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "endpoint": str,
+        "index": str,
+        "type": str,
+        "id": str,
+    },
+)
+
+_RequiredFirehoseActionOutputTypeDef = TypedDict(
+    "_RequiredFirehoseActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "deliveryStreamName": str,
+    },
+)
+_OptionalFirehoseActionOutputTypeDef = TypedDict(
+    "_OptionalFirehoseActionOutputTypeDef",
+    {
+        "separator": str,
+        "batchMode": bool,
+    },
+    total=False,
+)
+
+
+class FirehoseActionOutputTypeDef(
+    _RequiredFirehoseActionOutputTypeDef, _OptionalFirehoseActionOutputTypeDef
+):
+    pass
+
+
+IotAnalyticsActionOutputTypeDef = TypedDict(
+    "IotAnalyticsActionOutputTypeDef",
+    {
+        "channelArn": str,
+        "channelName": str,
+        "batchMode": bool,
+        "roleArn": str,
+    },
+    total=False,
+)
+
+_RequiredIotEventsActionOutputTypeDef = TypedDict(
+    "_RequiredIotEventsActionOutputTypeDef",
+    {
+        "inputName": str,
+        "roleArn": str,
+    },
+)
+_OptionalIotEventsActionOutputTypeDef = TypedDict(
+    "_OptionalIotEventsActionOutputTypeDef",
+    {
+        "messageId": str,
+        "batchMode": bool,
+    },
+    total=False,
+)
+
+
+class IotEventsActionOutputTypeDef(
+    _RequiredIotEventsActionOutputTypeDef, _OptionalIotEventsActionOutputTypeDef
+):
+    pass
+
+
+_RequiredKafkaActionOutputTypeDef = TypedDict(
+    "_RequiredKafkaActionOutputTypeDef",
+    {
+        "destinationArn": str,
+        "topic": str,
+        "clientProperties": Dict[str, str],
+    },
+)
+_OptionalKafkaActionOutputTypeDef = TypedDict(
+    "_OptionalKafkaActionOutputTypeDef",
+    {
+        "key": str,
+        "partition": str,
+    },
+    total=False,
+)
+
+
+class KafkaActionOutputTypeDef(
+    _RequiredKafkaActionOutputTypeDef, _OptionalKafkaActionOutputTypeDef
+):
+    pass
+
+
+_RequiredKinesisActionOutputTypeDef = TypedDict(
+    "_RequiredKinesisActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "streamName": str,
+    },
+)
+_OptionalKinesisActionOutputTypeDef = TypedDict(
+    "_OptionalKinesisActionOutputTypeDef",
+    {
+        "partitionKey": str,
+    },
+    total=False,
+)
+
+
+class KinesisActionOutputTypeDef(
+    _RequiredKinesisActionOutputTypeDef, _OptionalKinesisActionOutputTypeDef
+):
+    pass
+
+
+LambdaActionOutputTypeDef = TypedDict(
+    "LambdaActionOutputTypeDef",
+    {
+        "functionArn": str,
+    },
+)
+
+OpenSearchActionOutputTypeDef = TypedDict(
+    "OpenSearchActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "endpoint": str,
+        "index": str,
+        "type": str,
+        "id": str,
+    },
+)
+
+_RequiredS3ActionOutputTypeDef = TypedDict(
+    "_RequiredS3ActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "bucketName": str,
+        "key": str,
+    },
+)
+_OptionalS3ActionOutputTypeDef = TypedDict(
+    "_OptionalS3ActionOutputTypeDef",
+    {
+        "cannedAcl": CannedAccessControlListType,
+    },
+    total=False,
+)
+
+
+class S3ActionOutputTypeDef(_RequiredS3ActionOutputTypeDef, _OptionalS3ActionOutputTypeDef):
+    pass
+
+
+SalesforceActionOutputTypeDef = TypedDict(
+    "SalesforceActionOutputTypeDef",
+    {
+        "token": str,
+        "url": str,
+    },
+)
+
+_RequiredSnsActionOutputTypeDef = TypedDict(
+    "_RequiredSnsActionOutputTypeDef",
+    {
+        "targetArn": str,
+        "roleArn": str,
+    },
+)
+_OptionalSnsActionOutputTypeDef = TypedDict(
+    "_OptionalSnsActionOutputTypeDef",
+    {
+        "messageFormat": MessageFormatType,
+    },
+    total=False,
+)
+
+
+class SnsActionOutputTypeDef(_RequiredSnsActionOutputTypeDef, _OptionalSnsActionOutputTypeDef):
+    pass
+
+
+_RequiredSqsActionOutputTypeDef = TypedDict(
+    "_RequiredSqsActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "queueUrl": str,
+    },
+)
+_OptionalSqsActionOutputTypeDef = TypedDict(
+    "_OptionalSqsActionOutputTypeDef",
+    {
+        "useBase64": bool,
+    },
+    total=False,
+)
+
+
+class SqsActionOutputTypeDef(_RequiredSqsActionOutputTypeDef, _OptionalSqsActionOutputTypeDef):
+    pass
+
+
+_RequiredStepFunctionsActionOutputTypeDef = TypedDict(
+    "_RequiredStepFunctionsActionOutputTypeDef",
+    {
+        "stateMachineName": str,
+        "roleArn": str,
+    },
+)
+_OptionalStepFunctionsActionOutputTypeDef = TypedDict(
+    "_OptionalStepFunctionsActionOutputTypeDef",
+    {
+        "executionNamePrefix": str,
+    },
+    total=False,
+)
+
+
+class StepFunctionsActionOutputTypeDef(
+    _RequiredStepFunctionsActionOutputTypeDef, _OptionalStepFunctionsActionOutputTypeDef
+):
+    pass
+
+
 CloudwatchAlarmActionTypeDef = TypedDict(
     "CloudwatchAlarmActionTypeDef",
     {
         "roleArn": str,
         "alarmName": str,
         "stateReason": str,
         "stateValue": str,
@@ -1099,23 +1524,23 @@
 
 class StepFunctionsActionTypeDef(
     _RequiredStepFunctionsActionTypeDef, _OptionalStepFunctionsActionTypeDef
 ):
     pass
 
 
-MetricValueTypeDef = TypedDict(
-    "MetricValueTypeDef",
+MetricValueOutputTypeDef = TypedDict(
+    "MetricValueOutputTypeDef",
     {
         "count": int,
-        "cidrs": Sequence[str],
-        "ports": Sequence[int],
+        "cidrs": List[str],
+        "ports": List[int],
         "number": float,
-        "numbers": Sequence[float],
-        "strings": Sequence[str],
+        "numbers": List[float],
+        "strings": List[str],
     },
     total=False,
 )
 
 ViolationEventAdditionalInfoTypeDef = TypedDict(
     "ViolationEventAdditionalInfoTypeDef",
     {
@@ -1143,14 +1568,36 @@
         "thingName": str,
         "thingArn": str,
         "overrideDynamicGroups": bool,
     },
     total=False,
 )
 
+_RequiredAddThingsToThingGroupParamsOutputTypeDef = TypedDict(
+    "_RequiredAddThingsToThingGroupParamsOutputTypeDef",
+    {
+        "thingGroupNames": List[str],
+    },
+)
+_OptionalAddThingsToThingGroupParamsOutputTypeDef = TypedDict(
+    "_OptionalAddThingsToThingGroupParamsOutputTypeDef",
+    {
+        "overrideDynamicGroups": bool,
+    },
+    total=False,
+)
+
+
+class AddThingsToThingGroupParamsOutputTypeDef(
+    _RequiredAddThingsToThingGroupParamsOutputTypeDef,
+    _OptionalAddThingsToThingGroupParamsOutputTypeDef,
+):
+    pass
+
+
 _RequiredAddThingsToThingGroupParamsTypeDef = TypedDict(
     "_RequiredAddThingsToThingGroupParamsTypeDef",
     {
         "thingGroupNames": Sequence[str],
     },
 )
 _OptionalAddThingsToThingGroupParamsTypeDef = TypedDict(
@@ -1164,14 +1611,35 @@
 
 class AddThingsToThingGroupParamsTypeDef(
     _RequiredAddThingsToThingGroupParamsTypeDef, _OptionalAddThingsToThingGroupParamsTypeDef
 ):
     pass
 
 
+_RequiredAggregationTypeOutputTypeDef = TypedDict(
+    "_RequiredAggregationTypeOutputTypeDef",
+    {
+        "name": AggregationTypeNameType,
+    },
+)
+_OptionalAggregationTypeOutputTypeDef = TypedDict(
+    "_OptionalAggregationTypeOutputTypeDef",
+    {
+        "values": List[str],
+    },
+    total=False,
+)
+
+
+class AggregationTypeOutputTypeDef(
+    _RequiredAggregationTypeOutputTypeDef, _OptionalAggregationTypeOutputTypeDef
+):
+    pass
+
+
 _RequiredAggregationTypeTypeDef = TypedDict(
     "_RequiredAggregationTypeTypeDef",
     {
         "name": AggregationTypeNameType,
     },
 )
 _OptionalAggregationTypeTypeDef = TypedDict(
@@ -1183,14 +1651,22 @@
 )
 
 
 class AggregationTypeTypeDef(_RequiredAggregationTypeTypeDef, _OptionalAggregationTypeTypeDef):
     pass
 
 
+AlertTargetOutputTypeDef = TypedDict(
+    "AlertTargetOutputTypeDef",
+    {
+        "alertTargetArn": str,
+        "roleArn": str,
+    },
+)
+
 AlertTargetTypeDef = TypedDict(
     "AlertTargetTypeDef",
     {
         "alertTargetArn": str,
         "roleArn": str,
     },
 )
@@ -1200,14 +1676,35 @@
     {
         "policyName": str,
         "policyArn": str,
     },
     total=False,
 )
 
+_RequiredAssetPropertyTimestampOutputTypeDef = TypedDict(
+    "_RequiredAssetPropertyTimestampOutputTypeDef",
+    {
+        "timeInSeconds": str,
+    },
+)
+_OptionalAssetPropertyTimestampOutputTypeDef = TypedDict(
+    "_OptionalAssetPropertyTimestampOutputTypeDef",
+    {
+        "offsetInNanos": str,
+    },
+    total=False,
+)
+
+
+class AssetPropertyTimestampOutputTypeDef(
+    _RequiredAssetPropertyTimestampOutputTypeDef, _OptionalAssetPropertyTimestampOutputTypeDef
+):
+    pass
+
+
 _RequiredAssetPropertyTimestampTypeDef = TypedDict(
     "_RequiredAssetPropertyTimestampTypeDef",
     {
         "timeInSeconds": str,
     },
 )
 _OptionalAssetPropertyTimestampTypeDef = TypedDict(
@@ -1221,14 +1718,25 @@
 
 class AssetPropertyTimestampTypeDef(
     _RequiredAssetPropertyTimestampTypeDef, _OptionalAssetPropertyTimestampTypeDef
 ):
     pass
 
 
+AssetPropertyVariantOutputTypeDef = TypedDict(
+    "AssetPropertyVariantOutputTypeDef",
+    {
+        "stringValue": str,
+        "integerValue": str,
+        "doubleValue": str,
+        "booleanValue": str,
+    },
+    total=False,
+)
+
 AssetPropertyVariantTypeDef = TypedDict(
     "AssetPropertyVariantTypeDef",
     {
         "stringValue": str,
         "integerValue": str,
         "doubleValue": str,
         "booleanValue": str,
@@ -1298,23 +1806,40 @@
     "AttachThingPrincipalRequestRequestTypeDef",
     {
         "thingName": str,
         "principal": str,
     },
 )
 
+AttributePayloadOutputTypeDef = TypedDict(
+    "AttributePayloadOutputTypeDef",
+    {
+        "attributes": Dict[str, str],
+        "merge": bool,
+    },
+    total=False,
+)
+
 AttributePayloadTypeDef = TypedDict(
     "AttributePayloadTypeDef",
     {
         "attributes": Mapping[str, str],
         "merge": bool,
     },
     total=False,
 )
 
+AuditCheckConfigurationOutputTypeDef = TypedDict(
+    "AuditCheckConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+    total=False,
+)
+
 AuditCheckConfigurationTypeDef = TypedDict(
     "AuditCheckConfigurationTypeDef",
     {
         "enabled": bool,
     },
     total=False,
 )
@@ -1355,24 +1880,44 @@
         "taskId": str,
         "startTime": datetime,
         "taskStatus": AuditMitigationActionsTaskStatusType,
     },
     total=False,
 )
 
-AuditMitigationActionsTaskTargetTypeDef = TypedDict(
-    "AuditMitigationActionsTaskTargetTypeDef",
+AuditMitigationActionsTaskTargetOutputTypeDef = TypedDict(
+    "AuditMitigationActionsTaskTargetOutputTypeDef",
     {
         "auditTaskId": str,
         "findingIds": List[str],
         "auditCheckToReasonCodeFilter": Dict[str, List[str]],
     },
     total=False,
 )
 
+AuditMitigationActionsTaskTargetTypeDef = TypedDict(
+    "AuditMitigationActionsTaskTargetTypeDef",
+    {
+        "auditTaskId": str,
+        "findingIds": Sequence[str],
+        "auditCheckToReasonCodeFilter": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
+AuditNotificationTargetOutputTypeDef = TypedDict(
+    "AuditNotificationTargetOutputTypeDef",
+    {
+        "targetArn": str,
+        "roleArn": str,
+        "enabled": bool,
+    },
+    total=False,
+)
+
 AuditNotificationTargetTypeDef = TypedDict(
     "AuditNotificationTargetTypeDef",
     {
         "targetArn": str,
         "roleArn": str,
         "enabled": bool,
     },
@@ -1385,14 +1930,33 @@
         "taskId": str,
         "taskStatus": AuditTaskStatusType,
         "taskType": AuditTaskTypeType,
     },
     total=False,
 )
 
+_RequiredAuthInfoOutputTypeDef = TypedDict(
+    "_RequiredAuthInfoOutputTypeDef",
+    {
+        "resources": List[str],
+    },
+)
+_OptionalAuthInfoOutputTypeDef = TypedDict(
+    "_OptionalAuthInfoOutputTypeDef",
+    {
+        "actionType": ActionTypeType,
+    },
+    total=False,
+)
+
+
+class AuthInfoOutputTypeDef(_RequiredAuthInfoOutputTypeDef, _OptionalAuthInfoOutputTypeDef):
+    pass
+
+
 _RequiredAuthInfoTypeDef = TypedDict(
     "_RequiredAuthInfoTypeDef",
     {
         "resources": Sequence[str],
     },
 )
 _OptionalAuthInfoTypeDef = TypedDict(
@@ -1404,14 +1968,23 @@
 )
 
 
 class AuthInfoTypeDef(_RequiredAuthInfoTypeDef, _OptionalAuthInfoTypeDef):
     pass
 
 
+AuthorizerConfigOutputTypeDef = TypedDict(
+    "AuthorizerConfigOutputTypeDef",
+    {
+        "defaultAuthorizerName": str,
+        "allowAuthorizerOverride": bool,
+    },
+    total=False,
+)
+
 AuthorizerConfigTypeDef = TypedDict(
     "AuthorizerConfigTypeDef",
     {
         "defaultAuthorizerName": str,
         "allowAuthorizerOverride": bool,
     },
     total=False,
@@ -1449,23 +2022,40 @@
         "failureType": AwsJobAbortCriteriaFailureTypeType,
         "action": Literal["CANCEL"],
         "thresholdPercentage": float,
         "minNumberOfExecutedThings": int,
     },
 )
 
+AwsJobRateIncreaseCriteriaOutputTypeDef = TypedDict(
+    "AwsJobRateIncreaseCriteriaOutputTypeDef",
+    {
+        "numberOfNotifiedThings": int,
+        "numberOfSucceededThings": int,
+    },
+    total=False,
+)
+
 AwsJobRateIncreaseCriteriaTypeDef = TypedDict(
     "AwsJobRateIncreaseCriteriaTypeDef",
     {
         "numberOfNotifiedThings": int,
         "numberOfSucceededThings": int,
     },
     total=False,
 )
 
+AwsJobPresignedUrlConfigOutputTypeDef = TypedDict(
+    "AwsJobPresignedUrlConfigOutputTypeDef",
+    {
+        "expiresInSec": int,
+    },
+    total=False,
+)
+
 AwsJobPresignedUrlConfigTypeDef = TypedDict(
     "AwsJobPresignedUrlConfigTypeDef",
     {
         "expiresInSec": int,
     },
     total=False,
 )
@@ -1474,21 +2064,49 @@
     "AwsJobTimeoutConfigTypeDef",
     {
         "inProgressTimeoutInMinutes": int,
     },
     total=False,
 )
 
+MachineLearningDetectionConfigOutputTypeDef = TypedDict(
+    "MachineLearningDetectionConfigOutputTypeDef",
+    {
+        "confidenceLevel": ConfidenceLevelType,
+    },
+)
+
+StatisticalThresholdOutputTypeDef = TypedDict(
+    "StatisticalThresholdOutputTypeDef",
+    {
+        "statistic": str,
+    },
+    total=False,
+)
+
 MachineLearningDetectionConfigTypeDef = TypedDict(
     "MachineLearningDetectionConfigTypeDef",
     {
         "confidenceLevel": ConfidenceLevelType,
     },
 )
 
+MetricValueTypeDef = TypedDict(
+    "MetricValueTypeDef",
+    {
+        "count": int,
+        "cidrs": Sequence[str],
+        "ports": Sequence[int],
+        "number": float,
+        "numbers": Sequence[float],
+        "strings": Sequence[str],
+    },
+    total=False,
+)
+
 StatisticalThresholdTypeDef = TypedDict(
     "StatisticalThresholdTypeDef",
     {
         "statistic": str,
     },
     total=False,
 )
@@ -1502,14 +2120,35 @@
         "modelStatus": ModelStatusType,
         "datapointsCollectionPercentage": float,
         "lastModelRefreshDate": datetime,
     },
     total=False,
 )
 
+_RequiredMetricDimensionOutputTypeDef = TypedDict(
+    "_RequiredMetricDimensionOutputTypeDef",
+    {
+        "dimensionName": str,
+    },
+)
+_OptionalMetricDimensionOutputTypeDef = TypedDict(
+    "_OptionalMetricDimensionOutputTypeDef",
+    {
+        "operator": DimensionValueOperatorType,
+    },
+    total=False,
+)
+
+
+class MetricDimensionOutputTypeDef(
+    _RequiredMetricDimensionOutputTypeDef, _OptionalMetricDimensionOutputTypeDef
+):
+    pass
+
+
 _RequiredMetricDimensionTypeDef = TypedDict(
     "_RequiredMetricDimensionTypeDef",
     {
         "dimensionName": str,
     },
 )
 _OptionalMetricDimensionTypeDef = TypedDict(
@@ -1529,14 +2168,22 @@
     "BillingGroupMetadataTypeDef",
     {
         "creationDate": datetime,
     },
     total=False,
 )
 
+BillingGroupPropertiesOutputTypeDef = TypedDict(
+    "BillingGroupPropertiesOutputTypeDef",
+    {
+        "billingGroupDescription": str,
+    },
+    total=False,
+)
+
 BillingGroupPropertiesTypeDef = TypedDict(
     "BillingGroupPropertiesTypeDef",
     {
         "billingGroupDescription": str,
     },
     total=False,
 )
@@ -1684,31 +2331,56 @@
         "status": CertificateStatusType,
         "certificateMode": CertificateModeType,
         "creationDate": datetime,
     },
     total=False,
 )
 
+CodeSigningCertificateChainOutputTypeDef = TypedDict(
+    "CodeSigningCertificateChainOutputTypeDef",
+    {
+        "certificateName": str,
+        "inlineDocument": str,
+    },
+    total=False,
+)
+
 CodeSigningCertificateChainTypeDef = TypedDict(
     "CodeSigningCertificateChainTypeDef",
     {
         "certificateName": str,
         "inlineDocument": str,
     },
     total=False,
 )
 
+CodeSigningSignatureOutputTypeDef = TypedDict(
+    "CodeSigningSignatureOutputTypeDef",
+    {
+        "inlineDocument": bytes,
+    },
+    total=False,
+)
+
 CodeSigningSignatureTypeDef = TypedDict(
     "CodeSigningSignatureTypeDef",
     {
         "inlineDocument": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
+ConfigurationOutputTypeDef = TypedDict(
+    "ConfigurationOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -2679,16 +3351,16 @@
 DescribeCACertificateRequestRequestTypeDef = TypedDict(
     "DescribeCACertificateRequestRequestTypeDef",
     {
         "certificateId": str,
     },
 )
 
-RegistrationConfigTypeDef = TypedDict(
-    "RegistrationConfigTypeDef",
+RegistrationConfigOutputTypeDef = TypedDict(
+    "RegistrationConfigOutputTypeDef",
     {
         "templateBody": str,
         "roleArn": str,
         "templateName": str,
     },
     total=False,
 )
@@ -2760,14 +3432,22 @@
         "serverCertificateArn": str,
         "serverCertificateStatus": ServerCertificateStatusType,
         "serverCertificateStatusDetail": str,
     },
     total=False,
 )
 
+TlsConfigOutputTypeDef = TypedDict(
+    "TlsConfigOutputTypeDef",
+    {
+        "securityPolicy": str,
+    },
+    total=False,
+)
+
 DescribeEndpointRequestRequestTypeDef = TypedDict(
     "DescribeEndpointRequestRequestTypeDef",
     {
         "endpointType": str,
     },
     total=False,
 )
@@ -2837,14 +3517,39 @@
 DescribeJobTemplateRequestRequestTypeDef = TypedDict(
     "DescribeJobTemplateRequestRequestTypeDef",
     {
         "jobTemplateId": str,
     },
 )
 
+MaintenanceWindowOutputTypeDef = TypedDict(
+    "MaintenanceWindowOutputTypeDef",
+    {
+        "startTime": str,
+        "durationInMinutes": int,
+    },
+)
+
+PresignedUrlConfigOutputTypeDef = TypedDict(
+    "PresignedUrlConfigOutputTypeDef",
+    {
+        "roleArn": str,
+        "expiresInSec": int,
+    },
+    total=False,
+)
+
+TimeoutConfigOutputTypeDef = TypedDict(
+    "TimeoutConfigOutputTypeDef",
+    {
+        "inProgressTimeoutInMinutes": int,
+    },
+    total=False,
+)
+
 _RequiredDescribeManagedJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeManagedJobTemplateRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 _OptionalDescribeManagedJobTemplateRequestRequestTypeDef = TypedDict(
@@ -2885,14 +3590,35 @@
 DescribeProvisioningTemplateRequestRequestTypeDef = TypedDict(
     "DescribeProvisioningTemplateRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 
+_RequiredProvisioningHookOutputTypeDef = TypedDict(
+    "_RequiredProvisioningHookOutputTypeDef",
+    {
+        "targetArn": str,
+    },
+)
+_OptionalProvisioningHookOutputTypeDef = TypedDict(
+    "_OptionalProvisioningHookOutputTypeDef",
+    {
+        "payloadVersion": str,
+    },
+    total=False,
+)
+
+
+class ProvisioningHookOutputTypeDef(
+    _RequiredProvisioningHookOutputTypeDef, _OptionalProvisioningHookOutputTypeDef
+):
+    pass
+
+
 DescribeProvisioningTemplateVersionRequestRequestTypeDef = TypedDict(
     "DescribeProvisioningTemplateVersionRequestRequestTypeDef",
     {
         "templateName": str,
         "versionId": int,
     },
 )
@@ -3031,14 +3757,32 @@
         "deprecated": bool,
         "deprecationDate": datetime,
         "creationDate": datetime,
     },
     total=False,
 )
 
+ThingTypePropertiesOutputTypeDef = TypedDict(
+    "ThingTypePropertiesOutputTypeDef",
+    {
+        "thingTypeDescription": str,
+        "searchableAttributes": List[str],
+    },
+    total=False,
+)
+
+S3DestinationOutputTypeDef = TypedDict(
+    "S3DestinationOutputTypeDef",
+    {
+        "bucket": str,
+        "prefix": str,
+    },
+    total=False,
+)
+
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
@@ -3098,32 +3842,42 @@
         "actionsExecuted": int,
         "actionsSkipped": int,
         "actionsFailed": int,
     },
     total=False,
 )
 
-DetectMitigationActionsTaskTargetTypeDef = TypedDict(
-    "DetectMitigationActionsTaskTargetTypeDef",
+DetectMitigationActionsTaskTargetOutputTypeDef = TypedDict(
+    "DetectMitigationActionsTaskTargetOutputTypeDef",
     {
         "violationIds": List[str],
         "securityProfileName": str,
         "behaviorName": str,
     },
     total=False,
 )
 
-ViolationEventOccurrenceRangeTypeDef = TypedDict(
-    "ViolationEventOccurrenceRangeTypeDef",
+ViolationEventOccurrenceRangeOutputTypeDef = TypedDict(
+    "ViolationEventOccurrenceRangeOutputTypeDef",
     {
         "startTime": datetime,
         "endTime": datetime,
     },
 )
 
+DetectMitigationActionsTaskTargetTypeDef = TypedDict(
+    "DetectMitigationActionsTaskTargetTypeDef",
+    {
+        "violationIds": Sequence[str],
+        "securityProfileName": str,
+        "behaviorName": str,
+    },
+    total=False,
+)
+
 DisableTopicRuleRequestRequestTypeDef = TypedDict(
     "DisableTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
     },
 )
 
@@ -3133,14 +3887,21 @@
         "domainConfigurationName": str,
         "domainConfigurationArn": str,
         "serviceType": ServiceTypeType,
     },
     total=False,
 )
 
+PutItemInputOutputTypeDef = TypedDict(
+    "PutItemInputOutputTypeDef",
+    {
+        "tableName": str,
+    },
+)
+
 PutItemInputTypeDef = TypedDict(
     "PutItemInputTypeDef",
     {
         "tableName": str,
     },
 )
 
@@ -3157,14 +3918,22 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EnableIoTLoggingParamsOutputTypeDef = TypedDict(
+    "EnableIoTLoggingParamsOutputTypeDef",
+    {
+        "roleArnForLogging": str,
+        "logLevel": LogLevelType,
+    },
+)
+
 EnableIoTLoggingParamsTypeDef = TypedDict(
     "EnableIoTLoggingParamsTypeDef",
     {
         "roleArnForLogging": str,
         "logLevel": LogLevelType,
     },
 )
@@ -3181,32 +3950,69 @@
     {
         "code": str,
         "message": str,
     },
     total=False,
 )
 
+RateIncreaseCriteriaOutputTypeDef = TypedDict(
+    "RateIncreaseCriteriaOutputTypeDef",
+    {
+        "numberOfNotifiedThings": int,
+        "numberOfSucceededThings": int,
+    },
+    total=False,
+)
+
 RateIncreaseCriteriaTypeDef = TypedDict(
     "RateIncreaseCriteriaTypeDef",
     {
         "numberOfNotifiedThings": int,
         "numberOfSucceededThings": int,
     },
     total=False,
 )
 
+FieldOutputTypeDef = TypedDict(
+    "FieldOutputTypeDef",
+    {
+        "name": str,
+        "type": FieldTypeType,
+    },
+    total=False,
+)
+
 FieldTypeDef = TypedDict(
     "FieldTypeDef",
     {
         "name": str,
         "type": FieldTypeType,
     },
     total=False,
 )
 
+S3LocationOutputTypeDef = TypedDict(
+    "S3LocationOutputTypeDef",
+    {
+        "bucket": str,
+        "key": str,
+        "version": str,
+    },
+    total=False,
+)
+
+StreamOutputTypeDef = TypedDict(
+    "StreamOutputTypeDef",
+    {
+        "streamId": str,
+        "fileId": int,
+    },
+    total=False,
+)
+
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
         "version": str,
     },
@@ -3320,16 +4126,16 @@
 GetOTAUpdateRequestRequestTypeDef = TypedDict(
     "GetOTAUpdateRequestRequestTypeDef",
     {
         "otaUpdateId": str,
     },
 )
 
-VersionUpdateByJobsConfigTypeDef = TypedDict(
-    "VersionUpdateByJobsConfigTypeDef",
+VersionUpdateByJobsConfigOutputTypeDef = TypedDict(
+    "VersionUpdateByJobsConfigOutputTypeDef",
     {
         "enabled": bool,
         "roleArn": str,
     },
     total=False,
 )
 
@@ -3529,22 +4335,39 @@
     {
         "groupName": str,
         "groupArn": str,
     },
     total=False,
 )
 
+HttpActionHeaderOutputTypeDef = TypedDict(
+    "HttpActionHeaderOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 HttpActionHeaderTypeDef = TypedDict(
     "HttpActionHeaderTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
+SigV4AuthorizationOutputTypeDef = TypedDict(
+    "SigV4AuthorizationOutputTypeDef",
+    {
+        "signingRegion": str,
+        "serviceName": str,
+        "roleArn": str,
+    },
+)
+
 SigV4AuthorizationTypeDef = TypedDict(
     "SigV4AuthorizationTypeDef",
     {
         "signingRegion": str,
         "serviceName": str,
         "roleArn": str,
     },
@@ -3578,18 +4401,36 @@
     "HttpUrlDestinationSummaryTypeDef",
     {
         "confirmationUrl": str,
     },
     total=False,
 )
 
+IndexingFilterOutputTypeDef = TypedDict(
+    "IndexingFilterOutputTypeDef",
+    {
+        "namedShadowNames": List[str],
+    },
+    total=False,
+)
+
 IndexingFilterTypeDef = TypedDict(
     "IndexingFilterTypeDef",
     {
-        "namedShadowNames": List[str],
+        "namedShadowNames": Sequence[str],
+    },
+    total=False,
+)
+
+IssuerCertificateIdentifierOutputTypeDef = TypedDict(
+    "IssuerCertificateIdentifierOutputTypeDef",
+    {
+        "issuerCertificateSubject": str,
+        "issuerId": str,
+        "issuerCertificateSerialNumber": str,
     },
     total=False,
 )
 
 IssuerCertificateIdentifierTypeDef = TypedDict(
     "IssuerCertificateIdentifierTypeDef",
     {
@@ -3617,14 +4458,22 @@
         "lastUpdatedAt": datetime,
         "executionNumber": int,
         "retryAttempt": int,
     },
     total=False,
 )
 
+RetryCriteriaOutputTypeDef = TypedDict(
+    "RetryCriteriaOutputTypeDef",
+    {
+        "failureType": RetryableFailureTypeType,
+        "numberOfRetries": int,
+    },
+)
+
 RetryCriteriaTypeDef = TypedDict(
     "RetryCriteriaTypeDef",
     {
         "failureType": RetryableFailureTypeType,
         "numberOfRetries": int,
     },
 )
@@ -5156,14 +6005,33 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
+
 _RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
     "_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
     {
         "policyName": str,
     },
 )
 _OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
@@ -5765,14 +6633,35 @@
 class ListViolationEventsRequestRequestTypeDef(
     _RequiredListViolationEventsRequestRequestTypeDef,
     _OptionalListViolationEventsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredLocationTimestampOutputTypeDef = TypedDict(
+    "_RequiredLocationTimestampOutputTypeDef",
+    {
+        "value": str,
+    },
+)
+_OptionalLocationTimestampOutputTypeDef = TypedDict(
+    "_OptionalLocationTimestampOutputTypeDef",
+    {
+        "unit": str,
+    },
+    total=False,
+)
+
+
+class LocationTimestampOutputTypeDef(
+    _RequiredLocationTimestampOutputTypeDef, _OptionalLocationTimestampOutputTypeDef
+):
+    pass
+
+
 _RequiredLocationTimestampTypeDef = TypedDict(
     "_RequiredLocationTimestampTypeDef",
     {
         "value": str,
     },
 )
 _OptionalLocationTimestampTypeDef = TypedDict(
@@ -5786,14 +6675,33 @@
 
 class LocationTimestampTypeDef(
     _RequiredLocationTimestampTypeDef, _OptionalLocationTimestampTypeDef
 ):
     pass
 
 
+_RequiredLogTargetOutputTypeDef = TypedDict(
+    "_RequiredLogTargetOutputTypeDef",
+    {
+        "targetType": LogTargetTypeType,
+    },
+)
+_OptionalLogTargetOutputTypeDef = TypedDict(
+    "_OptionalLogTargetOutputTypeDef",
+    {
+        "targetName": str,
+    },
+    total=False,
+)
+
+
+class LogTargetOutputTypeDef(_RequiredLogTargetOutputTypeDef, _OptionalLogTargetOutputTypeDef):
+    pass
+
+
 _RequiredLogTargetTypeDef = TypedDict(
     "_RequiredLogTargetTypeDef",
     {
         "targetType": LogTargetTypeType,
     },
 )
 _OptionalLogTargetTypeDef = TypedDict(
@@ -5826,14 +6734,42 @@
 
 class LoggingOptionsPayloadTypeDef(
     _RequiredLoggingOptionsPayloadTypeDef, _OptionalLoggingOptionsPayloadTypeDef
 ):
     pass
 
 
+PublishFindingToSnsParamsOutputTypeDef = TypedDict(
+    "PublishFindingToSnsParamsOutputTypeDef",
+    {
+        "topicArn": str,
+    },
+)
+
+ReplaceDefaultPolicyVersionParamsOutputTypeDef = TypedDict(
+    "ReplaceDefaultPolicyVersionParamsOutputTypeDef",
+    {
+        "templateName": Literal["BLANK_POLICY"],
+    },
+)
+
+UpdateCACertificateParamsOutputTypeDef = TypedDict(
+    "UpdateCACertificateParamsOutputTypeDef",
+    {
+        "action": Literal["DEACTIVATE"],
+    },
+)
+
+UpdateDeviceCertificateParamsOutputTypeDef = TypedDict(
+    "UpdateDeviceCertificateParamsOutputTypeDef",
+    {
+        "action": Literal["DEACTIVATE"],
+    },
+)
+
 PublishFindingToSnsParamsTypeDef = TypedDict(
     "PublishFindingToSnsParamsTypeDef",
     {
         "topicArn": str,
     },
 )
 
@@ -5864,14 +6800,22 @@
         "username": str,
         "password": Union[str, bytes, IO[Any], StreamingBody],
         "clientId": str,
     },
     total=False,
 )
 
+UserPropertyOutputTypeDef = TypedDict(
+    "UserPropertyOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 UserPropertyTypeDef = TypedDict(
     "UserPropertyTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -5882,14 +6826,23 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PolicyVersionIdentifierOutputTypeDef = TypedDict(
+    "PolicyVersionIdentifierOutputTypeDef",
+    {
+        "policyName": str,
+        "policyVersionId": str,
+    },
+    total=False,
+)
+
 PolicyVersionIdentifierTypeDef = TypedDict(
     "PolicyVersionIdentifierTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
     total=False,
@@ -5914,14 +6867,24 @@
 class PutVerificationStateOnViolationRequestRequestTypeDef(
     _RequiredPutVerificationStateOnViolationRequestRequestTypeDef,
     _OptionalPutVerificationStateOnViolationRequestRequestTypeDef,
 ):
     pass
 
 
+RegistrationConfigTypeDef = TypedDict(
+    "RegistrationConfigTypeDef",
+    {
+        "templateBody": str,
+        "roleArn": str,
+        "templateName": str,
+    },
+    total=False,
+)
+
 RegisterCACertificateResponseTypeDef = TypedDict(
     "RegisterCACertificateResponseTypeDef",
     {
         "certificateArn": str,
         "certificateId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -6142,14 +7105,24 @@
         "roleArn": str,
         "defaultLogLevel": LogLevelType,
         "disableAllLogs": bool,
     },
     total=False,
 )
 
+SigningProfileParameterOutputTypeDef = TypedDict(
+    "SigningProfileParameterOutputTypeDef",
+    {
+        "certificateArn": str,
+        "platform": str,
+        "certificatePathOnDevice": str,
+    },
+    total=False,
+)
+
 SigningProfileParameterTypeDef = TypedDict(
     "SigningProfileParameterTypeDef",
     {
         "certificateArn": str,
         "platform": str,
         "certificatePathOnDevice": str,
     },
@@ -6160,14 +7133,22 @@
     "StartAuditMitigationActionsTaskResponseTypeDef",
     {
         "taskId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ViolationEventOccurrenceRangeTypeDef = TypedDict(
+    "ViolationEventOccurrenceRangeTypeDef",
+    {
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+
 StartDetectMitigationActionsTaskResponseTypeDef = TypedDict(
     "StartDetectMitigationActionsTaskResponseTypeDef",
     {
         "taskId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -6238,14 +7219,30 @@
         "connected": bool,
         "timestamp": int,
         "disconnectReason": str,
     },
     total=False,
 )
 
+TimestreamDimensionOutputTypeDef = TypedDict(
+    "TimestreamDimensionOutputTypeDef",
+    {
+        "name": str,
+        "value": str,
+    },
+)
+
+TimestreamTimestampOutputTypeDef = TypedDict(
+    "TimestreamTimestampOutputTypeDef",
+    {
+        "value": str,
+        "unit": str,
+    },
+)
+
 TimestreamDimensionTypeDef = TypedDict(
     "TimestreamDimensionTypeDef",
     {
         "name": str,
         "value": str,
     },
 )
@@ -6456,14 +7453,23 @@
     {
         "actionArn": str,
         "actionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+VersionUpdateByJobsConfigTypeDef = TypedDict(
+    "VersionUpdateByJobsConfigTypeDef",
+    {
+        "enabled": bool,
+        "roleArn": str,
+    },
+    total=False,
+)
+
 _RequiredUpdatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePackageRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 _OptionalUpdatePackageRequestRequestTypeDef = TypedDict(
@@ -6616,36 +7622,43 @@
     "ValidationErrorTypeDef",
     {
         "errorMessage": str,
     },
     total=False,
 )
 
+AbortConfigOutputTypeDef = TypedDict(
+    "AbortConfigOutputTypeDef",
+    {
+        "criteriaList": List[AbortCriteriaOutputTypeDef],
+    },
+)
+
 AbortConfigTypeDef = TypedDict(
     "AbortConfigTypeDef",
     {
         "criteriaList": Sequence[AbortCriteriaTypeDef],
     },
 )
 
 MetricDatumTypeDef = TypedDict(
     "MetricDatumTypeDef",
     {
         "timestamp": datetime,
-        "value": MetricValueTypeDef,
+        "value": MetricValueOutputTypeDef,
     },
     total=False,
 )
 
 DescribeFleetMetricResponseTypeDef = TypedDict(
     "DescribeFleetMetricResponseTypeDef",
     {
         "metricName": str,
         "queryString": str,
-        "aggregationType": AggregationTypeTypeDef,
+        "aggregationType": AggregationTypeOutputTypeDef,
         "period": int,
         "aggregationField": str,
         "description": str,
         "queryVersion": str,
         "indexName": str,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
@@ -6732,14 +7745,36 @@
     {
         "policies": List[PolicyTypeDef],
         "nextMarker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredAssetPropertyValueOutputTypeDef = TypedDict(
+    "_RequiredAssetPropertyValueOutputTypeDef",
+    {
+        "value": AssetPropertyVariantOutputTypeDef,
+        "timestamp": AssetPropertyTimestampOutputTypeDef,
+    },
+)
+_OptionalAssetPropertyValueOutputTypeDef = TypedDict(
+    "_OptionalAssetPropertyValueOutputTypeDef",
+    {
+        "quality": str,
+    },
+    total=False,
+)
+
+
+class AssetPropertyValueOutputTypeDef(
+    _RequiredAssetPropertyValueOutputTypeDef, _OptionalAssetPropertyValueOutputTypeDef
+):
+    pass
+
+
 _RequiredAssetPropertyValueTypeDef = TypedDict(
     "_RequiredAssetPropertyValueTypeDef",
     {
         "value": AssetPropertyVariantTypeDef,
         "timestamp": AssetPropertyTimestampTypeDef,
     },
 )
@@ -6754,14 +7789,23 @@
 
 class AssetPropertyValueTypeDef(
     _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
 ):
     pass
 
 
+ThingGroupPropertiesOutputTypeDef = TypedDict(
+    "ThingGroupPropertiesOutputTypeDef",
+    {
+        "thingGroupDescription": str,
+        "attributePayload": AttributePayloadOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateThingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalCreateThingRequestRequestTypeDef = TypedDict(
@@ -6843,17 +7887,17 @@
 )
 
 DescribeAccountAuditConfigurationResponseTypeDef = TypedDict(
     "DescribeAccountAuditConfigurationResponseTypeDef",
     {
         "roleArn": str,
         "auditNotificationTargetConfigurations": Dict[
-            Literal["SNS"], AuditNotificationTargetTypeDef
+            Literal["SNS"], AuditNotificationTargetOutputTypeDef
         ],
-        "auditCheckConfigurations": Dict[str, AuditCheckConfigurationTypeDef],
+        "auditCheckConfigurations": Dict[str, AuditCheckConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAccountAuditConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     {
@@ -6928,23 +7972,46 @@
 AwsJobAbortConfigTypeDef = TypedDict(
     "AwsJobAbortConfigTypeDef",
     {
         "abortCriteriaList": Sequence[AwsJobAbortCriteriaTypeDef],
     },
 )
 
+AwsJobExponentialRolloutRateOutputTypeDef = TypedDict(
+    "AwsJobExponentialRolloutRateOutputTypeDef",
+    {
+        "baseRatePerMinute": int,
+        "incrementFactor": float,
+        "rateIncreaseCriteria": AwsJobRateIncreaseCriteriaOutputTypeDef,
+    },
+)
+
 AwsJobExponentialRolloutRateTypeDef = TypedDict(
     "AwsJobExponentialRolloutRateTypeDef",
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": AwsJobRateIncreaseCriteriaTypeDef,
     },
 )
 
+BehaviorCriteriaOutputTypeDef = TypedDict(
+    "BehaviorCriteriaOutputTypeDef",
+    {
+        "comparisonOperator": ComparisonOperatorType,
+        "value": MetricValueOutputTypeDef,
+        "durationSeconds": int,
+        "consecutiveDatapointsToAlarm": int,
+        "consecutiveDatapointsToClear": int,
+        "statisticalThreshold": StatisticalThresholdOutputTypeDef,
+        "mlDetectionConfig": MachineLearningDetectionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 BehaviorCriteriaTypeDef = TypedDict(
     "BehaviorCriteriaTypeDef",
     {
         "comparisonOperator": ComparisonOperatorType,
         "value": MetricValueTypeDef,
         "durationSeconds": int,
         "consecutiveDatapointsToAlarm": int,
@@ -6960,14 +8027,35 @@
     {
         "summaries": List[BehaviorModelTrainingSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredMetricToRetainOutputTypeDef = TypedDict(
+    "_RequiredMetricToRetainOutputTypeDef",
+    {
+        "metric": str,
+    },
+)
+_OptionalMetricToRetainOutputTypeDef = TypedDict(
+    "_OptionalMetricToRetainOutputTypeDef",
+    {
+        "metricDimension": MetricDimensionOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class MetricToRetainOutputTypeDef(
+    _RequiredMetricToRetainOutputTypeDef, _OptionalMetricToRetainOutputTypeDef
+):
+    pass
+
+
 _RequiredMetricToRetainTypeDef = TypedDict(
     "_RequiredMetricToRetainTypeDef",
     {
         "metric": str,
     },
 )
 _OptionalMetricToRetainTypeDef = TypedDict(
@@ -6986,15 +8074,15 @@
 DescribeBillingGroupResponseTypeDef = TypedDict(
     "DescribeBillingGroupResponseTypeDef",
     {
         "billingGroupName": str,
         "billingGroupId": str,
         "billingGroupArn": str,
         "version": int,
-        "billingGroupProperties": BillingGroupPropertiesTypeDef,
+        "billingGroupProperties": BillingGroupPropertiesOutputTypeDef,
         "billingGroupMetadata": BillingGroupMetadataTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateBillingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBillingGroupRequestRequestTypeDef",
@@ -7099,29 +8187,40 @@
     {
         "certificates": List[CertificateTypeDef],
         "nextMarker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CustomCodeSigningOutputTypeDef = TypedDict(
+    "CustomCodeSigningOutputTypeDef",
+    {
+        "signature": CodeSigningSignatureOutputTypeDef,
+        "certificateChain": CodeSigningCertificateChainOutputTypeDef,
+        "hashAlgorithm": str,
+        "signatureAlgorithm": str,
+    },
+    total=False,
+)
+
 CustomCodeSigningTypeDef = TypedDict(
     "CustomCodeSigningTypeDef",
     {
         "signature": CodeSigningSignatureTypeDef,
         "certificateChain": CodeSigningCertificateChainTypeDef,
         "hashAlgorithm": str,
         "signatureAlgorithm": str,
     },
     total=False,
 )
 
 DescribeEventConfigurationsResponseTypeDef = TypedDict(
     "DescribeEventConfigurationsResponseTypeDef",
     {
-        "eventConfigurations": Dict[EventTypeType, ConfigurationTypeDef],
+        "eventConfigurations": Dict[EventTypeType, ConfigurationOutputTypeDef],
         "creationDate": datetime,
         "lastModifiedDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEventConfigurationsRequestRequestTypeDef = TypedDict(
@@ -7327,23 +8426,14 @@
 class CreateScheduledAuditRequestRequestTypeDef(
     _RequiredCreateScheduledAuditRequestRequestTypeDef,
     _OptionalCreateScheduledAuditRequestRequestTypeDef,
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -7458,32 +8548,14 @@
 class CreateProvisioningTemplateRequestRequestTypeDef(
     _RequiredCreateProvisioningTemplateRequestRequestTypeDef,
     _OptionalCreateProvisioningTemplateRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeProvisioningTemplateResponseTypeDef = TypedDict(
-    "DescribeProvisioningTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateName": str,
-        "description": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "defaultVersionId": int,
-        "templateBody": str,
-        "enabled": bool,
-        "provisioningRoleArn": str,
-        "preProvisioningHook": ProvisioningHookTypeDef,
-        "type": TemplateTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateProvisioningTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProvisioningTemplateRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 _OptionalUpdateProvisioningTemplateRequestRequestTypeDef = TypedDict(
@@ -7538,128 +8610,113 @@
         "taskStatistics": TaskStatisticsTypeDef,
         "scheduledAuditName": str,
         "auditDetails": Dict[str, AuditCheckDetailsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredRegisterCACertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterCACertificateRequestRequestTypeDef",
-    {
-        "caCertificate": str,
-    },
-)
-_OptionalRegisterCACertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterCACertificateRequestRequestTypeDef",
-    {
-        "verificationCertificate": str,
-        "setAsActive": bool,
-        "allowAutoRegistration": bool,
-        "registrationConfig": RegistrationConfigTypeDef,
-        "tags": Sequence[TagTypeDef],
-        "certificateMode": CertificateModeType,
-    },
-    total=False,
-)
-
-
-class RegisterCACertificateRequestRequestTypeDef(
-    _RequiredRegisterCACertificateRequestRequestTypeDef,
-    _OptionalRegisterCACertificateRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateCACertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCACertificateRequestRequestTypeDef",
-    {
-        "certificateId": str,
-    },
-)
-_OptionalUpdateCACertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCACertificateRequestRequestTypeDef",
-    {
-        "newStatus": CACertificateStatusType,
-        "newAutoRegistrationStatus": AutoRegistrationStatusType,
-        "registrationConfig": RegistrationConfigTypeDef,
-        "removeAutoRegistration": bool,
-    },
-    total=False,
-)
-
-
-class UpdateCACertificateRequestRequestTypeDef(
-    _RequiredUpdateCACertificateRequestRequestTypeDef,
-    _OptionalUpdateCACertificateRequestRequestTypeDef,
-):
-    pass
-
-
 DescribeDomainConfigurationResponseTypeDef = TypedDict(
     "DescribeDomainConfigurationResponseTypeDef",
     {
         "domainConfigurationName": str,
         "domainConfigurationArn": str,
         "domainName": str,
         "serverCertificates": List[ServerCertificateSummaryTypeDef],
-        "authorizerConfig": AuthorizerConfigTypeDef,
+        "authorizerConfig": AuthorizerConfigOutputTypeDef,
         "domainConfigurationStatus": DomainConfigurationStatusType,
         "serviceType": ServiceTypeType,
         "domainType": DomainTypeType,
         "lastStatusChangeDate": datetime,
-        "tlsConfig": TlsConfigTypeDef,
+        "tlsConfig": TlsConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SchedulingConfigOutputTypeDef = TypedDict(
+    "SchedulingConfigOutputTypeDef",
+    {
+        "startTime": str,
+        "endTime": str,
+        "endBehavior": JobEndBehaviorType,
+        "maintenanceWindows": List[MaintenanceWindowOutputTypeDef],
+    },
+    total=False,
+)
+
 DescribeManagedJobTemplateResponseTypeDef = TypedDict(
     "DescribeManagedJobTemplateResponseTypeDef",
     {
         "templateName": str,
         "templateArn": str,
         "description": str,
         "templateVersion": str,
         "environments": List[str],
         "documentParameters": List[DocumentParameterTypeDef],
         "document": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DescribeProvisioningTemplateResponseTypeDef = TypedDict(
+    "DescribeProvisioningTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateName": str,
+        "description": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "defaultVersionId": int,
+        "templateBody": str,
+        "enabled": bool,
+        "provisioningRoleArn": str,
+        "preProvisioningHook": ProvisioningHookOutputTypeDef,
+        "type": TemplateTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeRoleAliasResponseTypeDef = TypedDict(
     "DescribeRoleAliasResponseTypeDef",
     {
         "roleAliasDescription": RoleAliasDescriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeThingTypeResponseTypeDef = TypedDict(
     "DescribeThingTypeResponseTypeDef",
     {
         "thingTypeName": str,
         "thingTypeId": str,
         "thingTypeArn": str,
-        "thingTypeProperties": ThingTypePropertiesTypeDef,
+        "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ThingTypeDefinitionTypeDef = TypedDict(
     "ThingTypeDefinitionTypeDef",
     {
         "thingTypeName": str,
         "thingTypeArn": str,
-        "thingTypeProperties": ThingTypePropertiesTypeDef,
+        "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
     },
     total=False,
 )
 
+DestinationOutputTypeDef = TypedDict(
+    "DestinationOutputTypeDef",
+    {
+        "s3Destination": S3DestinationOutputTypeDef,
+    },
+    total=False,
+)
+
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3Destination": S3DestinationTypeDef,
     },
     total=False,
 )
@@ -7669,50 +8726,31 @@
     {
         "actionsExecutions": List[DetectMitigationActionExecutionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "taskId": str,
-        "target": DetectMitigationActionsTaskTargetTypeDef,
-        "actions": Sequence[str],
-        "clientRequestToken": str,
-    },
-)
-_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
-        "includeOnlyActiveViolations": bool,
-        "includeSuppressedAlerts": bool,
-    },
-    total=False,
-)
-
-
-class StartDetectMitigationActionsTaskRequestRequestTypeDef(
-    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
-    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
-):
-    pass
-
-
 ListDomainConfigurationsResponseTypeDef = TypedDict(
     "ListDomainConfigurationsResponseTypeDef",
     {
         "domainConfigurations": List[DomainConfigurationSummaryTypeDef],
         "nextMarker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DynamoDBv2ActionOutputTypeDef = TypedDict(
+    "DynamoDBv2ActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "putItem": PutItemInputOutputTypeDef,
+    },
+)
+
 DynamoDBv2ActionTypeDef = TypedDict(
     "DynamoDBv2ActionTypeDef",
     {
         "roleArn": str,
         "putItem": PutItemInputTypeDef,
     },
 )
@@ -7721,45 +8759,95 @@
     "GetEffectivePoliciesResponseTypeDef",
     {
         "effectivePolicies": List[EffectivePolicyTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ExponentialRolloutRateOutputTypeDef = TypedDict(
+    "ExponentialRolloutRateOutputTypeDef",
+    {
+        "baseRatePerMinute": int,
+        "incrementFactor": float,
+        "rateIncreaseCriteria": RateIncreaseCriteriaOutputTypeDef,
+    },
+)
+
 ExponentialRolloutRateTypeDef = TypedDict(
     "ExponentialRolloutRateTypeDef",
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": RateIncreaseCriteriaTypeDef,
     },
 )
 
+_RequiredThingGroupIndexingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredThingGroupIndexingConfigurationOutputTypeDef",
+    {
+        "thingGroupIndexingMode": ThingGroupIndexingModeType,
+    },
+)
+_OptionalThingGroupIndexingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalThingGroupIndexingConfigurationOutputTypeDef",
+    {
+        "managedFields": List[FieldOutputTypeDef],
+        "customFields": List[FieldOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class ThingGroupIndexingConfigurationOutputTypeDef(
+    _RequiredThingGroupIndexingConfigurationOutputTypeDef,
+    _OptionalThingGroupIndexingConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredThingGroupIndexingConfigurationTypeDef = TypedDict(
     "_RequiredThingGroupIndexingConfigurationTypeDef",
     {
         "thingGroupIndexingMode": ThingGroupIndexingModeType,
     },
 )
 _OptionalThingGroupIndexingConfigurationTypeDef = TypedDict(
     "_OptionalThingGroupIndexingConfigurationTypeDef",
     {
-        "managedFields": List[FieldTypeDef],
-        "customFields": List[FieldTypeDef],
+        "managedFields": Sequence[FieldTypeDef],
+        "customFields": Sequence[FieldTypeDef],
     },
     total=False,
 )
 
 
 class ThingGroupIndexingConfigurationTypeDef(
     _RequiredThingGroupIndexingConfigurationTypeDef, _OptionalThingGroupIndexingConfigurationTypeDef
 ):
     pass
 
 
+StreamFileOutputTypeDef = TypedDict(
+    "StreamFileOutputTypeDef",
+    {
+        "fileId": int,
+        "s3Location": S3LocationOutputTypeDef,
+    },
+    total=False,
+)
+
+FileLocationOutputTypeDef = TypedDict(
+    "FileLocationOutputTypeDef",
+    {
+        "stream": StreamOutputTypeDef,
+        "s3Location": S3LocationOutputTypeDef,
+    },
+    total=False,
+)
+
 StreamFileTypeDef = TypedDict(
     "StreamFileTypeDef",
     {
         "fileId": int,
         "s3Location": S3LocationTypeDef,
     },
     total=False,
@@ -7782,28 +8870,19 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPackageConfigurationResponseTypeDef = TypedDict(
     "GetPackageConfigurationResponseTypeDef",
     {
-        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
+        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdatePackageConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdatePackageConfigurationRequestRequestTypeDef",
-    {
-        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
-        "clientToken": str,
-    },
-    total=False,
-)
-
 GetPercentilesResponseTypeDef = TypedDict(
     "GetPercentilesResponseTypeDef",
     {
         "percentiles": List[PercentPairTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -7849,36 +8928,71 @@
         "parentGroupName": str,
         "rootToParentThingGroups": List[GroupNameAndArnTypeDef],
         "creationDate": datetime,
     },
     total=False,
 )
 
+HttpAuthorizationOutputTypeDef = TypedDict(
+    "HttpAuthorizationOutputTypeDef",
+    {
+        "sigv4": SigV4AuthorizationOutputTypeDef,
+    },
+    total=False,
+)
+
 HttpAuthorizationTypeDef = TypedDict(
     "HttpAuthorizationTypeDef",
     {
         "sigv4": SigV4AuthorizationTypeDef,
     },
     total=False,
 )
 
+_RequiredThingIndexingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredThingIndexingConfigurationOutputTypeDef",
+    {
+        "thingIndexingMode": ThingIndexingModeType,
+    },
+)
+_OptionalThingIndexingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalThingIndexingConfigurationOutputTypeDef",
+    {
+        "thingConnectivityIndexingMode": ThingConnectivityIndexingModeType,
+        "deviceDefenderIndexingMode": DeviceDefenderIndexingModeType,
+        "namedShadowIndexingMode": NamedShadowIndexingModeType,
+        "managedFields": List[FieldOutputTypeDef],
+        "customFields": List[FieldOutputTypeDef],
+        "filter": IndexingFilterOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ThingIndexingConfigurationOutputTypeDef(
+    _RequiredThingIndexingConfigurationOutputTypeDef,
+    _OptionalThingIndexingConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredThingIndexingConfigurationTypeDef = TypedDict(
     "_RequiredThingIndexingConfigurationTypeDef",
     {
         "thingIndexingMode": ThingIndexingModeType,
     },
 )
 _OptionalThingIndexingConfigurationTypeDef = TypedDict(
     "_OptionalThingIndexingConfigurationTypeDef",
     {
         "thingConnectivityIndexingMode": ThingConnectivityIndexingModeType,
         "deviceDefenderIndexingMode": DeviceDefenderIndexingModeType,
         "namedShadowIndexingMode": NamedShadowIndexingModeType,
-        "managedFields": List[FieldTypeDef],
-        "customFields": List[FieldTypeDef],
+        "managedFields": Sequence[FieldTypeDef],
+        "customFields": Sequence[FieldTypeDef],
         "filter": IndexingFilterTypeDef,
     },
     total=False,
 )
 
 
 class ThingIndexingConfigurationTypeDef(
@@ -7919,14 +9033,21 @@
     {
         "jobId": str,
         "jobExecutionSummary": JobExecutionSummaryTypeDef,
     },
     total=False,
 )
 
+JobExecutionsRetryConfigOutputTypeDef = TypedDict(
+    "JobExecutionsRetryConfigOutputTypeDef",
+    {
+        "criteriaList": List[RetryCriteriaOutputTypeDef],
+    },
+)
+
 JobExecutionsRetryConfigTypeDef = TypedDict(
     "JobExecutionsRetryConfigTypeDef",
     {
         "criteriaList": Sequence[RetryCriteriaTypeDef],
     },
 )
 
@@ -8051,14 +9172,23 @@
     {
         "streams": List[StreamSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTargetsForSecurityProfileResponseTypeDef = TypedDict(
     "ListTargetsForSecurityProfileResponseTypeDef",
     {
         "securityProfileTargets": List[SecurityProfileTargetTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -8087,14 +9217,39 @@
     {
         "rules": List[TopicRuleListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredLocationActionOutputTypeDef = TypedDict(
+    "_RequiredLocationActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "trackerName": str,
+        "deviceId": str,
+        "latitude": str,
+        "longitude": str,
+    },
+)
+_OptionalLocationActionOutputTypeDef = TypedDict(
+    "_OptionalLocationActionOutputTypeDef",
+    {
+        "timestamp": LocationTimestampOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class LocationActionOutputTypeDef(
+    _RequiredLocationActionOutputTypeDef, _OptionalLocationActionOutputTypeDef
+):
+    pass
+
+
 _RequiredLocationActionTypeDef = TypedDict(
     "_RequiredLocationActionTypeDef",
     {
         "roleArn": str,
         "trackerName": str,
         "deviceId": str,
         "latitude": str,
@@ -8113,15 +9268,15 @@
 class LocationActionTypeDef(_RequiredLocationActionTypeDef, _OptionalLocationActionTypeDef):
     pass
 
 
 LogTargetConfigurationTypeDef = TypedDict(
     "LogTargetConfigurationTypeDef",
     {
-        "logTarget": LogTargetTypeDef,
+        "logTarget": LogTargetOutputTypeDef,
         "logLevel": LogLevelType,
     },
     total=False,
 )
 
 SetV2LoggingLevelRequestRequestTypeDef = TypedDict(
     "SetV2LoggingLevelRequestRequestTypeDef",
@@ -8134,40 +9289,83 @@
 SetLoggingOptionsRequestRequestTypeDef = TypedDict(
     "SetLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptionsPayload": LoggingOptionsPayloadTypeDef,
     },
 )
 
+MitigationActionParamsOutputTypeDef = TypedDict(
+    "MitigationActionParamsOutputTypeDef",
+    {
+        "updateDeviceCertificateParams": UpdateDeviceCertificateParamsOutputTypeDef,
+        "updateCACertificateParams": UpdateCACertificateParamsOutputTypeDef,
+        "addThingsToThingGroupParams": AddThingsToThingGroupParamsOutputTypeDef,
+        "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsOutputTypeDef,
+        "enableIoTLoggingParams": EnableIoTLoggingParamsOutputTypeDef,
+        "publishFindingToSnsParams": PublishFindingToSnsParamsOutputTypeDef,
+    },
+    total=False,
+)
+
 MitigationActionParamsTypeDef = TypedDict(
     "MitigationActionParamsTypeDef",
     {
         "updateDeviceCertificateParams": UpdateDeviceCertificateParamsTypeDef,
         "updateCACertificateParams": UpdateCACertificateParamsTypeDef,
         "addThingsToThingGroupParams": AddThingsToThingGroupParamsTypeDef,
         "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsTypeDef,
         "enableIoTLoggingParams": EnableIoTLoggingParamsTypeDef,
         "publishFindingToSnsParams": PublishFindingToSnsParamsTypeDef,
     },
     total=False,
 )
 
+MqttHeadersOutputTypeDef = TypedDict(
+    "MqttHeadersOutputTypeDef",
+    {
+        "payloadFormatIndicator": str,
+        "contentType": str,
+        "responseTopic": str,
+        "correlationData": str,
+        "messageExpiry": str,
+        "userProperties": List[UserPropertyOutputTypeDef],
+    },
+    total=False,
+)
+
 MqttHeadersTypeDef = TypedDict(
     "MqttHeadersTypeDef",
     {
         "payloadFormatIndicator": str,
         "contentType": str,
         "responseTopic": str,
         "correlationData": str,
         "messageExpiry": str,
         "userProperties": Sequence[UserPropertyTypeDef],
     },
     total=False,
 )
 
+ResourceIdentifierOutputTypeDef = TypedDict(
+    "ResourceIdentifierOutputTypeDef",
+    {
+        "deviceCertificateId": str,
+        "caCertificateId": str,
+        "cognitoIdentityPoolId": str,
+        "clientId": str,
+        "policyVersionIdentifier": PolicyVersionIdentifierOutputTypeDef,
+        "account": str,
+        "iamRoleArn": str,
+        "roleAliasArn": str,
+        "issuerCertificateIdentifier": IssuerCertificateIdentifierOutputTypeDef,
+        "deviceCertificateArn": str,
+    },
+    total=False,
+)
+
 ResourceIdentifierTypeDef = TypedDict(
     "ResourceIdentifierTypeDef",
     {
         "deviceCertificateId": str,
         "caCertificateId": str,
         "cognitoIdentityPoolId": str,
         "clientId": str,
@@ -8177,14 +9375,93 @@
         "roleAliasArn": str,
         "issuerCertificateIdentifier": IssuerCertificateIdentifierTypeDef,
         "deviceCertificateArn": str,
     },
     total=False,
 )
 
+_RequiredRegisterCACertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterCACertificateRequestRequestTypeDef",
+    {
+        "caCertificate": str,
+    },
+)
+_OptionalRegisterCACertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterCACertificateRequestRequestTypeDef",
+    {
+        "verificationCertificate": str,
+        "setAsActive": bool,
+        "allowAutoRegistration": bool,
+        "registrationConfig": RegistrationConfigTypeDef,
+        "tags": Sequence[TagTypeDef],
+        "certificateMode": CertificateModeType,
+    },
+    total=False,
+)
+
+
+class RegisterCACertificateRequestRequestTypeDef(
+    _RequiredRegisterCACertificateRequestRequestTypeDef,
+    _OptionalRegisterCACertificateRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateCACertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCACertificateRequestRequestTypeDef",
+    {
+        "certificateId": str,
+    },
+)
+_OptionalUpdateCACertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCACertificateRequestRequestTypeDef",
+    {
+        "newStatus": CACertificateStatusType,
+        "newAutoRegistrationStatus": AutoRegistrationStatusType,
+        "registrationConfig": RegistrationConfigTypeDef,
+        "removeAutoRegistration": bool,
+    },
+    total=False,
+)
+
+
+class UpdateCACertificateRequestRequestTypeDef(
+    _RequiredUpdateCACertificateRequestRequestTypeDef,
+    _OptionalUpdateCACertificateRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "taskId": str,
+        "target": DetectMitigationActionsTaskTargetTypeDef,
+        "actions": Sequence[str],
+        "clientRequestToken": str,
+    },
+)
+_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
+        "includeOnlyActiveViolations": bool,
+        "includeSuppressedAlerts": bool,
+    },
+    total=False,
+)
+
+
+class StartDetectMitigationActionsTaskRequestRequestTypeDef(
+    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
+    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredTestInvokeAuthorizerRequestRequestTypeDef",
     {
         "authorizerName": str,
     },
 )
 _OptionalTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
@@ -8218,14 +9495,38 @@
         "shadow": str,
         "deviceDefender": str,
         "connectivity": ThingConnectivityTypeDef,
     },
     total=False,
 )
 
+_RequiredTimestreamActionOutputTypeDef = TypedDict(
+    "_RequiredTimestreamActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "databaseName": str,
+        "tableName": str,
+        "dimensions": List[TimestreamDimensionOutputTypeDef],
+    },
+)
+_OptionalTimestreamActionOutputTypeDef = TypedDict(
+    "_OptionalTimestreamActionOutputTypeDef",
+    {
+        "timestamp": TimestreamTimestampOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class TimestreamActionOutputTypeDef(
+    _RequiredTimestreamActionOutputTypeDef, _OptionalTimestreamActionOutputTypeDef
+):
+    pass
+
+
 _RequiredTimestreamActionTypeDef = TypedDict(
     "_RequiredTimestreamActionTypeDef",
     {
         "roleArn": str,
         "databaseName": str,
         "tableName": str,
         "dimensions": Sequence[TimestreamDimensionTypeDef],
@@ -8277,14 +9578,23 @@
         "statusReason": str,
         "httpUrlProperties": HttpUrlDestinationPropertiesTypeDef,
         "vpcProperties": VpcDestinationPropertiesTypeDef,
     },
     total=False,
 )
 
+UpdatePackageConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdatePackageConfigurationRequestRequestTypeDef",
+    {
+        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
+        "clientToken": str,
+    },
+    total=False,
+)
+
 ValidateSecurityProfileBehaviorsResponseTypeDef = TypedDict(
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
     {
         "valid": bool,
         "validationErrors": List[ValidationErrorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -8304,14 +9614,39 @@
     {
         "implicitDeny": ImplicitDenyTypeDef,
         "explicitDeny": ExplicitDenyTypeDef,
     },
     total=False,
 )
 
+_RequiredPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
+    "_RequiredPutAssetPropertyValueEntryOutputTypeDef",
+    {
+        "propertyValues": List[AssetPropertyValueOutputTypeDef],
+    },
+)
+_OptionalPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
+    "_OptionalPutAssetPropertyValueEntryOutputTypeDef",
+    {
+        "entryId": str,
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+    },
+    total=False,
+)
+
+
+class PutAssetPropertyValueEntryOutputTypeDef(
+    _RequiredPutAssetPropertyValueEntryOutputTypeDef,
+    _OptionalPutAssetPropertyValueEntryOutputTypeDef,
+):
+    pass
+
+
 _RequiredPutAssetPropertyValueEntryTypeDef = TypedDict(
     "_RequiredPutAssetPropertyValueEntryTypeDef",
     {
         "propertyValues": Sequence[AssetPropertyValueTypeDef],
     },
 )
 _OptionalPutAssetPropertyValueEntryTypeDef = TypedDict(
@@ -8425,23 +9760,54 @@
 
 class UpdateThingGroupRequestRequestTypeDef(
     _RequiredUpdateThingGroupRequestRequestTypeDef, _OptionalUpdateThingGroupRequestRequestTypeDef
 ):
     pass
 
 
+AwsJobExecutionsRolloutConfigOutputTypeDef = TypedDict(
+    "AwsJobExecutionsRolloutConfigOutputTypeDef",
+    {
+        "maximumPerMinute": int,
+        "exponentialRate": AwsJobExponentialRolloutRateOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsJobExecutionsRolloutConfigTypeDef = TypedDict(
     "AwsJobExecutionsRolloutConfigTypeDef",
     {
         "maximumPerMinute": int,
         "exponentialRate": AwsJobExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
+_RequiredBehaviorOutputTypeDef = TypedDict(
+    "_RequiredBehaviorOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalBehaviorOutputTypeDef = TypedDict(
+    "_OptionalBehaviorOutputTypeDef",
+    {
+        "metric": str,
+        "metricDimension": MetricDimensionOutputTypeDef,
+        "criteria": BehaviorCriteriaOutputTypeDef,
+        "suppressAlerts": bool,
+    },
+    total=False,
+)
+
+
+class BehaviorOutputTypeDef(_RequiredBehaviorOutputTypeDef, _OptionalBehaviorOutputTypeDef):
+    pass
+
+
 _RequiredBehaviorTypeDef = TypedDict(
     "_RequiredBehaviorTypeDef",
     {
         "name": str,
     },
 )
 _OptionalBehaviorTypeDef = TypedDict(
@@ -8485,15 +9851,15 @@
     pass
 
 
 DescribeCACertificateResponseTypeDef = TypedDict(
     "DescribeCACertificateResponseTypeDef",
     {
         "certificateDescription": CACertificateDescriptionTypeDef,
-        "registrationConfig": RegistrationConfigTypeDef,
+        "registrationConfig": RegistrationConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCertificateResponseTypeDef = TypedDict(
     "DescribeCertificateResponseTypeDef",
     {
@@ -8507,33 +9873,67 @@
     {
         "thingTypes": List[ThingTypeDefinitionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StartSigningJobParameterOutputTypeDef = TypedDict(
+    "StartSigningJobParameterOutputTypeDef",
+    {
+        "signingProfileParameter": SigningProfileParameterOutputTypeDef,
+        "signingProfileName": str,
+        "destination": DestinationOutputTypeDef,
+    },
+    total=False,
+)
+
 StartSigningJobParameterTypeDef = TypedDict(
     "StartSigningJobParameterTypeDef",
     {
         "signingProfileParameter": SigningProfileParameterTypeDef,
         "signingProfileName": str,
         "destination": DestinationTypeDef,
     },
     total=False,
 )
 
+JobExecutionsRolloutConfigOutputTypeDef = TypedDict(
+    "JobExecutionsRolloutConfigOutputTypeDef",
+    {
+        "maximumPerMinute": int,
+        "exponentialRate": ExponentialRolloutRateOutputTypeDef,
+    },
+    total=False,
+)
+
 JobExecutionsRolloutConfigTypeDef = TypedDict(
     "JobExecutionsRolloutConfigTypeDef",
     {
         "maximumPerMinute": int,
         "exponentialRate": ExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
+StreamInfoTypeDef = TypedDict(
+    "StreamInfoTypeDef",
+    {
+        "streamId": str,
+        "streamArn": str,
+        "streamVersion": int,
+        "description": str,
+        "files": List[StreamFileOutputTypeDef],
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "roleArn": str,
+    },
+    total=False,
+)
+
 _RequiredCreateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamRequestRequestTypeDef",
     {
         "streamId": str,
         "files": Sequence[StreamFileTypeDef],
         "roleArn": str,
     },
@@ -8550,29 +9950,14 @@
 
 class CreateStreamRequestRequestTypeDef(
     _RequiredCreateStreamRequestRequestTypeDef, _OptionalCreateStreamRequestRequestTypeDef
 ):
     pass
 
 
-StreamInfoTypeDef = TypedDict(
-    "StreamInfoTypeDef",
-    {
-        "streamId": str,
-        "streamArn": str,
-        "streamVersion": int,
-        "description": str,
-        "files": List[StreamFileTypeDef],
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "roleArn": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamRequestRequestTypeDef",
     {
         "streamId": str,
     },
 )
 _OptionalUpdateStreamRequestRequestTypeDef = TypedDict(
@@ -8595,24 +9980,45 @@
 DescribeThingGroupResponseTypeDef = TypedDict(
     "DescribeThingGroupResponseTypeDef",
     {
         "thingGroupName": str,
         "thingGroupId": str,
         "thingGroupArn": str,
         "version": int,
-        "thingGroupProperties": ThingGroupPropertiesTypeDef,
+        "thingGroupProperties": ThingGroupPropertiesOutputTypeDef,
         "thingGroupMetadata": ThingGroupMetadataTypeDef,
         "indexName": str,
         "queryString": str,
         "queryVersion": str,
         "status": DynamicGroupStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredHttpActionOutputTypeDef = TypedDict(
+    "_RequiredHttpActionOutputTypeDef",
+    {
+        "url": str,
+    },
+)
+_OptionalHttpActionOutputTypeDef = TypedDict(
+    "_OptionalHttpActionOutputTypeDef",
+    {
+        "confirmationUrl": str,
+        "headers": List[HttpActionHeaderOutputTypeDef],
+        "auth": HttpAuthorizationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class HttpActionOutputTypeDef(_RequiredHttpActionOutputTypeDef, _OptionalHttpActionOutputTypeDef):
+    pass
+
+
 _RequiredHttpActionTypeDef = TypedDict(
     "_RequiredHttpActionTypeDef",
     {
         "url": str,
     },
 )
 _OptionalHttpActionTypeDef = TypedDict(
@@ -8629,16 +10035,16 @@
 class HttpActionTypeDef(_RequiredHttpActionTypeDef, _OptionalHttpActionTypeDef):
     pass
 
 
 GetIndexingConfigurationResponseTypeDef = TypedDict(
     "GetIndexingConfigurationResponseTypeDef",
     {
-        "thingIndexingConfiguration": ThingIndexingConfigurationTypeDef,
-        "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationTypeDef,
+        "thingIndexingConfiguration": ThingIndexingConfigurationOutputTypeDef,
+        "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateIndexingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     {
@@ -8688,64 +10094,64 @@
     {
         "logTargetConfigurations": List[LogTargetConfigurationTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateMitigationActionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMitigationActionRequestRequestTypeDef",
-    {
-        "actionName": str,
-        "roleArn": str,
-        "actionParams": MitigationActionParamsTypeDef,
-    },
-)
-_OptionalCreateMitigationActionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMitigationActionRequestRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateMitigationActionRequestRequestTypeDef(
-    _RequiredCreateMitigationActionRequestRequestTypeDef,
-    _OptionalCreateMitigationActionRequestRequestTypeDef,
-):
-    pass
-
-
 DescribeMitigationActionResponseTypeDef = TypedDict(
     "DescribeMitigationActionResponseTypeDef",
     {
         "actionName": str,
         "actionType": MitigationActionTypeType,
         "actionArn": str,
         "actionId": str,
         "roleArn": str,
-        "actionParams": MitigationActionParamsTypeDef,
+        "actionParams": MitigationActionParamsOutputTypeDef,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MitigationActionTypeDef = TypedDict(
     "MitigationActionTypeDef",
     {
         "name": str,
         "id": str,
         "roleArn": str,
+        "actionParams": MitigationActionParamsOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateMitigationActionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMitigationActionRequestRequestTypeDef",
+    {
+        "actionName": str,
+        "roleArn": str,
         "actionParams": MitigationActionParamsTypeDef,
     },
+)
+_OptionalCreateMitigationActionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMitigationActionRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
     total=False,
 )
 
+
+class CreateMitigationActionRequestRequestTypeDef(
+    _RequiredCreateMitigationActionRequestRequestTypeDef,
+    _OptionalCreateMitigationActionRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredUpdateMitigationActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMitigationActionRequestRequestTypeDef",
     {
         "actionName": str,
     },
 )
 _OptionalUpdateMitigationActionRequestRequestTypeDef = TypedDict(
@@ -8761,14 +10167,37 @@
 class UpdateMitigationActionRequestRequestTypeDef(
     _RequiredUpdateMitigationActionRequestRequestTypeDef,
     _OptionalUpdateMitigationActionRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredRepublishActionOutputTypeDef = TypedDict(
+    "_RequiredRepublishActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "topic": str,
+    },
+)
+_OptionalRepublishActionOutputTypeDef = TypedDict(
+    "_OptionalRepublishActionOutputTypeDef",
+    {
+        "qos": int,
+        "headers": MqttHeadersOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class RepublishActionOutputTypeDef(
+    _RequiredRepublishActionOutputTypeDef, _OptionalRepublishActionOutputTypeDef
+):
+    pass
+
+
 _RequiredRepublishActionTypeDef = TypedDict(
     "_RequiredRepublishActionTypeDef",
     {
         "roleArn": str,
         "topic": str,
     },
 )
@@ -8786,15 +10215,15 @@
     pass
 
 
 _RequiredAuditSuppressionTypeDef = TypedDict(
     "_RequiredAuditSuppressionTypeDef",
     {
         "checkName": str,
-        "resourceIdentifier": ResourceIdentifierTypeDef,
+        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
     },
 )
 _OptionalAuditSuppressionTypeDef = TypedDict(
     "_OptionalAuditSuppressionTypeDef",
     {
         "expirationDate": datetime,
         "suppressIndefinitely": bool,
@@ -8804,14 +10233,46 @@
 )
 
 
 class AuditSuppressionTypeDef(_RequiredAuditSuppressionTypeDef, _OptionalAuditSuppressionTypeDef):
     pass
 
 
+DescribeAuditSuppressionResponseTypeDef = TypedDict(
+    "DescribeAuditSuppressionResponseTypeDef",
+    {
+        "checkName": str,
+        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
+        "expirationDate": datetime,
+        "suppressIndefinitely": bool,
+        "description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+NonCompliantResourceTypeDef = TypedDict(
+    "NonCompliantResourceTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
+        "additionalInfo": Dict[str, str],
+    },
+    total=False,
+)
+
+RelatedResourceTypeDef = TypedDict(
+    "RelatedResourceTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
+        "additionalInfo": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredCreateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuditSuppressionRequestRequestTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "clientRequestToken": str,
     },
@@ -8846,26 +10307,14 @@
     "DescribeAuditSuppressionRequestRequestTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
 
-DescribeAuditSuppressionResponseTypeDef = TypedDict(
-    "DescribeAuditSuppressionResponseTypeDef",
-    {
-        "checkName": str,
-        "resourceIdentifier": ResourceIdentifierTypeDef,
-        "expirationDate": datetime,
-        "suppressIndefinitely": bool,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListAuditFindingsRequestListAuditFindingsPaginateTypeDef = TypedDict(
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
     {
         "taskId": str,
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "startTime": Union[datetime, str],
@@ -8910,34 +10359,14 @@
         "ascendingOrder": bool,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-NonCompliantResourceTypeDef = TypedDict(
-    "NonCompliantResourceTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceIdentifier": ResourceIdentifierTypeDef,
-        "additionalInfo": Dict[str, str],
-    },
-    total=False,
-)
-
-RelatedResourceTypeDef = TypedDict(
-    "RelatedResourceTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceIdentifier": ResourceIdentifierTypeDef,
-        "additionalInfo": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredUpdateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAuditSuppressionRequestRequestTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
@@ -9000,48 +10429,107 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AuthResultTypeDef = TypedDict(
     "AuthResultTypeDef",
     {
-        "authInfo": AuthInfoTypeDef,
+        "authInfo": AuthInfoOutputTypeDef,
         "allowed": AllowedTypeDef,
         "denied": DeniedTypeDef,
         "authDecision": AuthDecisionType,
         "missingContextValues": List[str],
     },
     total=False,
 )
 
+IotSiteWiseActionOutputTypeDef = TypedDict(
+    "IotSiteWiseActionOutputTypeDef",
+    {
+        "putAssetPropertyValueEntries": List[PutAssetPropertyValueEntryOutputTypeDef],
+        "roleArn": str,
+    },
+)
+
 IotSiteWiseActionTypeDef = TypedDict(
     "IotSiteWiseActionTypeDef",
     {
         "putAssetPropertyValueEntries": Sequence[PutAssetPropertyValueEntryTypeDef],
         "roleArn": str,
     },
 )
 
 ActiveViolationTypeDef = TypedDict(
     "ActiveViolationTypeDef",
     {
         "violationId": str,
         "thingName": str,
         "securityProfileName": str,
-        "behavior": BehaviorTypeDef,
-        "lastViolationValue": MetricValueTypeDef,
+        "behavior": BehaviorOutputTypeDef,
+        "lastViolationValue": MetricValueOutputTypeDef,
         "violationEventAdditionalInfo": ViolationEventAdditionalInfoTypeDef,
         "verificationState": VerificationStateType,
         "verificationStateDescription": str,
         "lastViolationTime": datetime,
         "violationStartTime": datetime,
     },
     total=False,
 )
 
+DescribeSecurityProfileResponseTypeDef = TypedDict(
+    "DescribeSecurityProfileResponseTypeDef",
+    {
+        "securityProfileName": str,
+        "securityProfileArn": str,
+        "securityProfileDescription": str,
+        "behaviors": List[BehaviorOutputTypeDef],
+        "alertTargets": Dict[Literal["SNS"], AlertTargetOutputTypeDef],
+        "additionalMetricsToRetain": List[str],
+        "additionalMetricsToRetainV2": List[MetricToRetainOutputTypeDef],
+        "version": int,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSecurityProfileResponseTypeDef = TypedDict(
+    "UpdateSecurityProfileResponseTypeDef",
+    {
+        "securityProfileName": str,
+        "securityProfileArn": str,
+        "securityProfileDescription": str,
+        "behaviors": List[BehaviorOutputTypeDef],
+        "alertTargets": Dict[Literal["SNS"], AlertTargetOutputTypeDef],
+        "additionalMetricsToRetain": List[str],
+        "additionalMetricsToRetainV2": List[MetricToRetainOutputTypeDef],
+        "version": int,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ViolationEventTypeDef = TypedDict(
+    "ViolationEventTypeDef",
+    {
+        "violationId": str,
+        "thingName": str,
+        "securityProfileName": str,
+        "behavior": BehaviorOutputTypeDef,
+        "metricValue": MetricValueOutputTypeDef,
+        "violationEventAdditionalInfo": ViolationEventAdditionalInfoTypeDef,
+        "violationEventType": ViolationEventTypeType,
+        "verificationState": VerificationStateType,
+        "verificationStateDescription": str,
+        "violationEventTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileName": str,
     },
 )
 _OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
@@ -9061,31 +10549,14 @@
 class CreateSecurityProfileRequestRequestTypeDef(
     _RequiredCreateSecurityProfileRequestRequestTypeDef,
     _OptionalCreateSecurityProfileRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeSecurityProfileResponseTypeDef = TypedDict(
-    "DescribeSecurityProfileResponseTypeDef",
-    {
-        "securityProfileName": str,
-        "securityProfileArn": str,
-        "securityProfileDescription": str,
-        "behaviors": List[BehaviorTypeDef],
-        "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": List[str],
-        "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
-        "version": int,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileName": str,
     },
 )
 _OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
@@ -9108,65 +10579,93 @@
 class UpdateSecurityProfileRequestRequestTypeDef(
     _RequiredUpdateSecurityProfileRequestRequestTypeDef,
     _OptionalUpdateSecurityProfileRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateSecurityProfileResponseTypeDef = TypedDict(
-    "UpdateSecurityProfileResponseTypeDef",
-    {
-        "securityProfileName": str,
-        "securityProfileArn": str,
-        "securityProfileDescription": str,
-        "behaviors": List[BehaviorTypeDef],
-        "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": List[str],
-        "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
-        "version": int,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
     "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
     {
         "behaviors": Sequence[BehaviorTypeDef],
     },
 )
 
-ViolationEventTypeDef = TypedDict(
-    "ViolationEventTypeDef",
+CodeSigningOutputTypeDef = TypedDict(
+    "CodeSigningOutputTypeDef",
     {
-        "violationId": str,
-        "thingName": str,
-        "securityProfileName": str,
-        "behavior": BehaviorTypeDef,
-        "metricValue": MetricValueTypeDef,
-        "violationEventAdditionalInfo": ViolationEventAdditionalInfoTypeDef,
-        "violationEventType": ViolationEventTypeType,
-        "verificationState": VerificationStateType,
-        "verificationStateDescription": str,
-        "violationEventTime": datetime,
+        "awsSignerJobId": str,
+        "startSigningJobParameter": StartSigningJobParameterOutputTypeDef,
+        "customCodeSigning": CustomCodeSigningOutputTypeDef,
     },
     total=False,
 )
 
 CodeSigningTypeDef = TypedDict(
     "CodeSigningTypeDef",
     {
         "awsSignerJobId": str,
         "startSigningJobParameter": StartSigningJobParameterTypeDef,
         "customCodeSigning": CustomCodeSigningTypeDef,
     },
     total=False,
 )
 
+DescribeJobTemplateResponseTypeDef = TypedDict(
+    "DescribeJobTemplateResponseTypeDef",
+    {
+        "jobTemplateArn": str,
+        "jobTemplateId": str,
+        "description": str,
+        "documentSource": str,
+        "document": str,
+        "createdAt": datetime,
+        "presignedUrlConfig": PresignedUrlConfigOutputTypeDef,
+        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigOutputTypeDef,
+        "abortConfig": AbortConfigOutputTypeDef,
+        "timeoutConfig": TimeoutConfigOutputTypeDef,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
+        "maintenanceWindows": List[MaintenanceWindowOutputTypeDef],
+        "destinationPackageVersions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+JobTypeDef = TypedDict(
+    "JobTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "targetSelection": TargetSelectionType,
+        "status": JobStatusType,
+        "forceCanceled": bool,
+        "reasonCode": str,
+        "comment": str,
+        "targets": List[str],
+        "description": str,
+        "presignedUrlConfig": PresignedUrlConfigOutputTypeDef,
+        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigOutputTypeDef,
+        "abortConfig": AbortConfigOutputTypeDef,
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "completedAt": datetime,
+        "jobProcessDetails": JobProcessDetailsTypeDef,
+        "timeoutConfig": TimeoutConfigOutputTypeDef,
+        "namespaceId": str,
+        "jobTemplateArn": str,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
+        "documentParameters": Dict[str, str],
+        "isConcurrent": bool,
+        "schedulingConfig": SchedulingConfigOutputTypeDef,
+        "scheduledJobRollouts": List[ScheduledJobRolloutTypeDef],
+        "destinationPackageVersions": List[str],
+    },
+    total=False,
+)
+
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "jobId": str,
         "targets": Sequence[str],
     },
 )
@@ -9227,66 +10726,14 @@
 
 class CreateJobTemplateRequestRequestTypeDef(
     _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
     pass
 
 
-DescribeJobTemplateResponseTypeDef = TypedDict(
-    "DescribeJobTemplateResponseTypeDef",
-    {
-        "jobTemplateArn": str,
-        "jobTemplateId": str,
-        "description": str,
-        "documentSource": str,
-        "document": str,
-        "createdAt": datetime,
-        "presignedUrlConfig": PresignedUrlConfigTypeDef,
-        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
-        "abortConfig": AbortConfigTypeDef,
-        "timeoutConfig": TimeoutConfigTypeDef,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
-        "maintenanceWindows": List[MaintenanceWindowTypeDef],
-        "destinationPackageVersions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-JobTypeDef = TypedDict(
-    "JobTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "targetSelection": TargetSelectionType,
-        "status": JobStatusType,
-        "forceCanceled": bool,
-        "reasonCode": str,
-        "comment": str,
-        "targets": List[str],
-        "description": str,
-        "presignedUrlConfig": PresignedUrlConfigTypeDef,
-        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
-        "abortConfig": AbortConfigTypeDef,
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "completedAt": datetime,
-        "jobProcessDetails": JobProcessDetailsTypeDef,
-        "timeoutConfig": TimeoutConfigTypeDef,
-        "namespaceId": str,
-        "jobTemplateArn": str,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
-        "documentParameters": Dict[str, str],
-        "isConcurrent": bool,
-        "schedulingConfig": SchedulingConfigTypeDef,
-        "scheduledJobRollouts": List[ScheduledJobRolloutTypeDef],
-        "destinationPackageVersions": List[str],
-    },
-    total=False,
-)
-
 _RequiredUpdateJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalUpdateJobRequestRequestTypeDef = TypedDict(
@@ -9321,30 +10768,30 @@
 DescribeAuditMitigationActionsTaskResponseTypeDef = TypedDict(
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     {
         "taskStatus": AuditMitigationActionsTaskStatusType,
         "startTime": datetime,
         "endTime": datetime,
         "taskStatistics": Dict[str, TaskStatisticsForAuditCheckTypeDef],
-        "target": AuditMitigationActionsTaskTargetTypeDef,
+        "target": AuditMitigationActionsTaskTargetOutputTypeDef,
         "auditCheckToActionsMapping": Dict[str, List[str]],
         "actionsDefinition": List[MitigationActionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectMitigationActionsTaskSummaryTypeDef = TypedDict(
     "DetectMitigationActionsTaskSummaryTypeDef",
     {
         "taskId": str,
         "taskStatus": DetectMitigationActionsTaskStatusType,
         "taskStartTime": datetime,
         "taskEndTime": datetime,
-        "target": DetectMitigationActionsTaskTargetTypeDef,
-        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
+        "target": DetectMitigationActionsTaskTargetOutputTypeDef,
+        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeOutputTypeDef,
         "onlyActiveViolationsIncluded": bool,
         "suppressedAlertsIncluded": bool,
         "actionsDefinition": List[MitigationActionTypeDef],
         "taskStatistics": DetectMitigationActionsTaskStatisticsTypeDef,
     },
     total=False,
 )
@@ -9389,14 +10836,44 @@
     "TestAuthorizationResponseTypeDef",
     {
         "authResults": List[AuthResultTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "dynamoDB": DynamoDBActionOutputTypeDef,
+        "dynamoDBv2": DynamoDBv2ActionOutputTypeDef,
+        "lambda": LambdaActionOutputTypeDef,
+        "sns": SnsActionOutputTypeDef,
+        "sqs": SqsActionOutputTypeDef,
+        "kinesis": KinesisActionOutputTypeDef,
+        "republish": RepublishActionOutputTypeDef,
+        "s3": S3ActionOutputTypeDef,
+        "firehose": FirehoseActionOutputTypeDef,
+        "cloudwatchMetric": CloudwatchMetricActionOutputTypeDef,
+        "cloudwatchAlarm": CloudwatchAlarmActionOutputTypeDef,
+        "cloudwatchLogs": CloudwatchLogsActionOutputTypeDef,
+        "elasticsearch": ElasticsearchActionOutputTypeDef,
+        "salesforce": SalesforceActionOutputTypeDef,
+        "iotAnalytics": IotAnalyticsActionOutputTypeDef,
+        "iotEvents": IotEventsActionOutputTypeDef,
+        "iotSiteWise": IotSiteWiseActionOutputTypeDef,
+        "stepFunctions": StepFunctionsActionOutputTypeDef,
+        "timestream": TimestreamActionOutputTypeDef,
+        "http": HttpActionOutputTypeDef,
+        "kafka": KafkaActionOutputTypeDef,
+        "openSearch": OpenSearchActionOutputTypeDef,
+        "location": LocationActionOutputTypeDef,
+    },
+    total=False,
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "dynamoDB": DynamoDBActionTypeDef,
         "dynamoDBv2": DynamoDBv2ActionTypeDef,
         "lambda": LambdaActionTypeDef,
         "sns": SnsActionTypeDef,
@@ -9437,14 +10914,27 @@
     {
         "violationEvents": List[ViolationEventTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+OTAUpdateFileOutputTypeDef = TypedDict(
+    "OTAUpdateFileOutputTypeDef",
+    {
+        "fileName": str,
+        "fileType": int,
+        "fileVersion": str,
+        "fileLocation": FileLocationOutputTypeDef,
+        "codeSigning": CodeSigningOutputTypeDef,
+        "attributes": Dict[str, str],
+    },
+    total=False,
+)
+
 OTAUpdateFileTypeDef = TypedDict(
     "OTAUpdateFileTypeDef",
     {
         "fileName": str,
         "fileType": int,
         "fileVersion": str,
         "fileLocation": FileLocationTypeDef,
@@ -9493,14 +10983,29 @@
     {
         "findings": List[AuditFindingTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TopicRuleTypeDef = TypedDict(
+    "TopicRuleTypeDef",
+    {
+        "ruleName": str,
+        "sql": str,
+        "description": str,
+        "createdAt": datetime,
+        "actions": List[ActionOutputTypeDef],
+        "ruleDisabled": bool,
+        "awsIotSqlVersion": str,
+        "errorAction": ActionOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredTopicRulePayloadTypeDef = TypedDict(
     "_RequiredTopicRulePayloadTypeDef",
     {
         "sql": str,
         "actions": Sequence[ActionTypeDef],
     },
 )
@@ -9516,25 +11021,33 @@
 )
 
 
 class TopicRulePayloadTypeDef(_RequiredTopicRulePayloadTypeDef, _OptionalTopicRulePayloadTypeDef):
     pass
 
 
-TopicRuleTypeDef = TypedDict(
-    "TopicRuleTypeDef",
+OTAUpdateInfoTypeDef = TypedDict(
+    "OTAUpdateInfoTypeDef",
     {
-        "ruleName": str,
-        "sql": str,
+        "otaUpdateId": str,
+        "otaUpdateArn": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
         "description": str,
-        "createdAt": datetime,
-        "actions": List[ActionTypeDef],
-        "ruleDisabled": bool,
-        "awsIotSqlVersion": str,
-        "errorAction": ActionTypeDef,
+        "targets": List[str],
+        "protocols": List[ProtocolType],
+        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigOutputTypeDef,
+        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigOutputTypeDef,
+        "targetSelection": TargetSelectionType,
+        "otaUpdateFiles": List[OTAUpdateFileOutputTypeDef],
+        "otaUpdateStatus": OTAUpdateStatusType,
+        "awsIotJobId": str,
+        "awsIotJobArn": str,
+        "errorInfo": ErrorInfoTypeDef,
+        "additionalParameters": Dict[str, str],
     },
     total=False,
 )
 
 _RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOTAUpdateRequestRequestTypeDef",
     {
@@ -9563,35 +11076,21 @@
 
 class CreateOTAUpdateRequestRequestTypeDef(
     _RequiredCreateOTAUpdateRequestRequestTypeDef, _OptionalCreateOTAUpdateRequestRequestTypeDef
 ):
     pass
 
 
-OTAUpdateInfoTypeDef = TypedDict(
-    "OTAUpdateInfoTypeDef",
+GetTopicRuleResponseTypeDef = TypedDict(
+    "GetTopicRuleResponseTypeDef",
     {
-        "otaUpdateId": str,
-        "otaUpdateArn": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "description": str,
-        "targets": List[str],
-        "protocols": List[ProtocolType],
-        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
-        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
-        "targetSelection": TargetSelectionType,
-        "otaUpdateFiles": List[OTAUpdateFileTypeDef],
-        "otaUpdateStatus": OTAUpdateStatusType,
-        "awsIotJobId": str,
-        "awsIotJobArn": str,
-        "errorInfo": ErrorInfoTypeDef,
-        "additionalParameters": Dict[str, str],
+        "ruleArn": str,
+        "rule": TopicRuleTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 _RequiredCreateTopicRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
         "topicRulePayload": TopicRulePayloadTypeDef,
@@ -9616,23 +11115,14 @@
     "ReplaceTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
         "topicRulePayload": TopicRulePayloadTypeDef,
     },
 )
 
-GetTopicRuleResponseTypeDef = TypedDict(
-    "GetTopicRuleResponseTypeDef",
-    {
-        "ruleArn": str,
-        "rule": TopicRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetOTAUpdateResponseTypeDef = TypedDict(
     "GetOTAUpdateResponseTypeDef",
     {
         "otaUpdateInfo": OTAUpdateInfoTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iot-1.28.0/mypy_boto3_iot/type_defs.pyi` & `mypy-boto3-iot-1.28.12/mypy_boto3_iot/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iot service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iot.type_defs import AbortCriteriaTypeDef
+    from mypy_boto3_iot.type_defs import AbortCriteriaOutputTypeDef
 
-    data: AbortCriteriaTypeDef = {...}
+    data: AbortCriteriaOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -88,16 +88,34 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AbortCriteriaOutputTypeDef",
     "AbortCriteriaTypeDef",
     "AcceptCertificateTransferRequestRequestTypeDef",
+    "CloudwatchAlarmActionOutputTypeDef",
+    "CloudwatchLogsActionOutputTypeDef",
+    "CloudwatchMetricActionOutputTypeDef",
+    "DynamoDBActionOutputTypeDef",
+    "ElasticsearchActionOutputTypeDef",
+    "FirehoseActionOutputTypeDef",
+    "IotAnalyticsActionOutputTypeDef",
+    "IotEventsActionOutputTypeDef",
+    "KafkaActionOutputTypeDef",
+    "KinesisActionOutputTypeDef",
+    "LambdaActionOutputTypeDef",
+    "OpenSearchActionOutputTypeDef",
+    "S3ActionOutputTypeDef",
+    "SalesforceActionOutputTypeDef",
+    "SnsActionOutputTypeDef",
+    "SqsActionOutputTypeDef",
+    "StepFunctionsActionOutputTypeDef",
     "CloudwatchAlarmActionTypeDef",
     "CloudwatchLogsActionTypeDef",
     "CloudwatchMetricActionTypeDef",
     "DynamoDBActionTypeDef",
     "ElasticsearchActionTypeDef",
     "FirehoseActionTypeDef",
     "IotAnalyticsActionTypeDef",
@@ -107,67 +125,88 @@
     "LambdaActionTypeDef",
     "OpenSearchActionTypeDef",
     "S3ActionTypeDef",
     "SalesforceActionTypeDef",
     "SnsActionTypeDef",
     "SqsActionTypeDef",
     "StepFunctionsActionTypeDef",
-    "MetricValueTypeDef",
+    "MetricValueOutputTypeDef",
     "ViolationEventAdditionalInfoTypeDef",
     "AddThingToBillingGroupRequestRequestTypeDef",
     "AddThingToThingGroupRequestRequestTypeDef",
+    "AddThingsToThingGroupParamsOutputTypeDef",
     "AddThingsToThingGroupParamsTypeDef",
+    "AggregationTypeOutputTypeDef",
     "AggregationTypeTypeDef",
+    "AlertTargetOutputTypeDef",
     "AlertTargetTypeDef",
     "PolicyTypeDef",
+    "AssetPropertyTimestampOutputTypeDef",
     "AssetPropertyTimestampTypeDef",
+    "AssetPropertyVariantOutputTypeDef",
     "AssetPropertyVariantTypeDef",
     "AssociateTargetsWithJobRequestRequestTypeDef",
     "AssociateTargetsWithJobResponseTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachPrincipalPolicyRequestRequestTypeDef",
     "AttachSecurityProfileRequestRequestTypeDef",
     "AttachThingPrincipalRequestRequestTypeDef",
+    "AttributePayloadOutputTypeDef",
     "AttributePayloadTypeDef",
+    "AuditCheckConfigurationOutputTypeDef",
     "AuditCheckConfigurationTypeDef",
     "AuditCheckDetailsTypeDef",
     "AuditMitigationActionExecutionMetadataTypeDef",
     "AuditMitigationActionsTaskMetadataTypeDef",
+    "AuditMitigationActionsTaskTargetOutputTypeDef",
     "AuditMitigationActionsTaskTargetTypeDef",
+    "AuditNotificationTargetOutputTypeDef",
     "AuditNotificationTargetTypeDef",
     "AuditTaskMetadataTypeDef",
+    "AuthInfoOutputTypeDef",
     "AuthInfoTypeDef",
+    "AuthorizerConfigOutputTypeDef",
     "AuthorizerConfigTypeDef",
     "AuthorizerDescriptionTypeDef",
     "AuthorizerSummaryTypeDef",
     "AwsJobAbortCriteriaTypeDef",
+    "AwsJobRateIncreaseCriteriaOutputTypeDef",
     "AwsJobRateIncreaseCriteriaTypeDef",
+    "AwsJobPresignedUrlConfigOutputTypeDef",
     "AwsJobPresignedUrlConfigTypeDef",
     "AwsJobTimeoutConfigTypeDef",
+    "MachineLearningDetectionConfigOutputTypeDef",
+    "StatisticalThresholdOutputTypeDef",
     "MachineLearningDetectionConfigTypeDef",
+    "MetricValueTypeDef",
     "StatisticalThresholdTypeDef",
     "BehaviorModelTrainingSummaryTypeDef",
+    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "BillingGroupMetadataTypeDef",
+    "BillingGroupPropertiesOutputTypeDef",
     "BillingGroupPropertiesTypeDef",
     "BucketTypeDef",
     "TermsAggregationTypeDef",
     "CertificateValidityTypeDef",
     "CACertificateTypeDef",
     "CancelAuditMitigationActionsTaskRequestRequestTypeDef",
     "CancelAuditTaskRequestRequestTypeDef",
     "CancelCertificateTransferRequestRequestTypeDef",
     "CancelDetectMitigationActionsTaskRequestRequestTypeDef",
     "CancelJobExecutionRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "CancelJobResponseTypeDef",
     "TransferDataTypeDef",
     "CertificateTypeDef",
+    "CodeSigningCertificateChainOutputTypeDef",
     "CodeSigningCertificateChainTypeDef",
+    "CodeSigningSignatureOutputTypeDef",
     "CodeSigningSignatureTypeDef",
+    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
     "TagTypeDef",
     "CreateAuthorizerResponseTypeDef",
     "CreateBillingGroupResponseTypeDef",
     "CreateCertificateFromCsrRequestRequestTypeDef",
     "CreateCertificateFromCsrResponseTypeDef",
@@ -242,35 +281,40 @@
     "DescribeAuditMitigationActionsTaskRequestRequestTypeDef",
     "TaskStatisticsForAuditCheckTypeDef",
     "DescribeAuditTaskRequestRequestTypeDef",
     "TaskStatisticsTypeDef",
     "DescribeAuthorizerRequestRequestTypeDef",
     "DescribeBillingGroupRequestRequestTypeDef",
     "DescribeCACertificateRequestRequestTypeDef",
-    "RegistrationConfigTypeDef",
+    "RegistrationConfigOutputTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "DescribeCustomMetricRequestRequestTypeDef",
     "DescribeCustomMetricResponseTypeDef",
     "DescribeDetectMitigationActionsTaskRequestRequestTypeDef",
     "DescribeDimensionRequestRequestTypeDef",
     "DescribeDimensionResponseTypeDef",
     "DescribeDomainConfigurationRequestRequestTypeDef",
     "ServerCertificateSummaryTypeDef",
+    "TlsConfigOutputTypeDef",
     "DescribeEndpointRequestRequestTypeDef",
     "DescribeEndpointResponseTypeDef",
     "DescribeFleetMetricRequestRequestTypeDef",
     "DescribeIndexRequestRequestTypeDef",
     "DescribeIndexResponseTypeDef",
     "DescribeJobExecutionRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
+    "MaintenanceWindowOutputTypeDef",
+    "PresignedUrlConfigOutputTypeDef",
+    "TimeoutConfigOutputTypeDef",
     "DescribeManagedJobTemplateRequestRequestTypeDef",
     "DocumentParameterTypeDef",
     "DescribeMitigationActionRequestRequestTypeDef",
     "DescribeProvisioningTemplateRequestRequestTypeDef",
+    "ProvisioningHookOutputTypeDef",
     "DescribeProvisioningTemplateVersionRequestRequestTypeDef",
     "DescribeProvisioningTemplateVersionResponseTypeDef",
     "DescribeRoleAliasRequestRequestTypeDef",
     "RoleAliasDescriptionTypeDef",
     "DescribeScheduledAuditRequestRequestTypeDef",
     "DescribeScheduledAuditResponseTypeDef",
     "DescribeSecurityProfileRequestRequestTypeDef",
@@ -278,46 +322,55 @@
     "DescribeThingGroupRequestRequestTypeDef",
     "DescribeThingRegistrationTaskRequestRequestTypeDef",
     "DescribeThingRegistrationTaskResponseTypeDef",
     "DescribeThingRequestRequestTypeDef",
     "DescribeThingResponseTypeDef",
     "DescribeThingTypeRequestRequestTypeDef",
     "ThingTypeMetadataTypeDef",
+    "ThingTypePropertiesOutputTypeDef",
+    "S3DestinationOutputTypeDef",
     "S3DestinationTypeDef",
     "DetachPolicyRequestRequestTypeDef",
     "DetachPrincipalPolicyRequestRequestTypeDef",
     "DetachSecurityProfileRequestRequestTypeDef",
     "DetachThingPrincipalRequestRequestTypeDef",
     "DetectMitigationActionExecutionTypeDef",
     "DetectMitigationActionsTaskStatisticsTypeDef",
+    "DetectMitigationActionsTaskTargetOutputTypeDef",
+    "ViolationEventOccurrenceRangeOutputTypeDef",
     "DetectMitigationActionsTaskTargetTypeDef",
-    "ViolationEventOccurrenceRangeTypeDef",
     "DisableTopicRuleRequestRequestTypeDef",
     "DomainConfigurationSummaryTypeDef",
+    "PutItemInputOutputTypeDef",
     "PutItemInputTypeDef",
     "EffectivePolicyTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EnableIoTLoggingParamsOutputTypeDef",
     "EnableIoTLoggingParamsTypeDef",
     "EnableTopicRuleRequestRequestTypeDef",
     "ErrorInfoTypeDef",
+    "RateIncreaseCriteriaOutputTypeDef",
     "RateIncreaseCriteriaTypeDef",
+    "FieldOutputTypeDef",
     "FieldTypeDef",
+    "S3LocationOutputTypeDef",
+    "StreamOutputTypeDef",
     "S3LocationTypeDef",
     "StreamTypeDef",
     "FleetMetricNameAndArnTypeDef",
     "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
     "GetBehaviorModelTrainingSummariesRequestRequestTypeDef",
     "GetCardinalityRequestRequestTypeDef",
     "GetCardinalityResponseTypeDef",
     "GetEffectivePoliciesRequestRequestTypeDef",
     "GetJobDocumentRequestRequestTypeDef",
     "GetJobDocumentResponseTypeDef",
     "GetLoggingOptionsResponseTypeDef",
     "GetOTAUpdateRequestRequestTypeDef",
-    "VersionUpdateByJobsConfigTypeDef",
+    "VersionUpdateByJobsConfigOutputTypeDef",
     "GetPackageRequestRequestTypeDef",
     "GetPackageResponseTypeDef",
     "GetPackageVersionRequestRequestTypeDef",
     "GetPackageVersionResponseTypeDef",
     "GetPercentilesRequestRequestTypeDef",
     "PercentPairTypeDef",
     "GetPolicyRequestRequestTypeDef",
@@ -327,24 +380,29 @@
     "GetRegistrationCodeResponseTypeDef",
     "GetStatisticsRequestRequestTypeDef",
     "StatisticsTypeDef",
     "GetTopicRuleDestinationRequestRequestTypeDef",
     "GetTopicRuleRequestRequestTypeDef",
     "GetV2LoggingOptionsResponseTypeDef",
     "GroupNameAndArnTypeDef",
+    "HttpActionHeaderOutputTypeDef",
     "HttpActionHeaderTypeDef",
+    "SigV4AuthorizationOutputTypeDef",
     "SigV4AuthorizationTypeDef",
     "HttpContextTypeDef",
     "HttpUrlDestinationConfigurationTypeDef",
     "HttpUrlDestinationPropertiesTypeDef",
     "HttpUrlDestinationSummaryTypeDef",
+    "IndexingFilterOutputTypeDef",
     "IndexingFilterTypeDef",
+    "IssuerCertificateIdentifierOutputTypeDef",
     "IssuerCertificateIdentifierTypeDef",
     "JobExecutionStatusDetailsTypeDef",
     "JobExecutionSummaryTypeDef",
+    "RetryCriteriaOutputTypeDef",
     "RetryCriteriaTypeDef",
     "JobProcessDetailsTypeDef",
     "JobSummaryTypeDef",
     "JobTemplateSummaryTypeDef",
     "ScheduledJobRolloutTypeDef",
     "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
     "ListActiveViolationsRequestRequestTypeDef",
@@ -443,14 +501,15 @@
     "ListSecurityProfilesRequestRequestTypeDef",
     "SecurityProfileIdentifierTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "StreamSummaryTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
     "ListTargetsForPolicyRequestRequestTypeDef",
     "ListTargetsForPolicyResponseTypeDef",
     "ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
     "ListTargetsForSecurityProfileRequestRequestTypeDef",
     "SecurityProfileTargetTypeDef",
     "ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
@@ -482,26 +541,35 @@
     "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
     "ListTopicRulesRequestRequestTypeDef",
     "TopicRuleListItemTypeDef",
     "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
     "ListV2LoggingLevelsRequestRequestTypeDef",
     "ListViolationEventsRequestListViolationEventsPaginateTypeDef",
     "ListViolationEventsRequestRequestTypeDef",
+    "LocationTimestampOutputTypeDef",
     "LocationTimestampTypeDef",
+    "LogTargetOutputTypeDef",
     "LogTargetTypeDef",
     "LoggingOptionsPayloadTypeDef",
+    "PublishFindingToSnsParamsOutputTypeDef",
+    "ReplaceDefaultPolicyVersionParamsOutputTypeDef",
+    "UpdateCACertificateParamsOutputTypeDef",
+    "UpdateDeviceCertificateParamsOutputTypeDef",
     "PublishFindingToSnsParamsTypeDef",
     "ReplaceDefaultPolicyVersionParamsTypeDef",
     "UpdateCACertificateParamsTypeDef",
     "UpdateDeviceCertificateParamsTypeDef",
     "MqttContextTypeDef",
+    "UserPropertyOutputTypeDef",
     "UserPropertyTypeDef",
     "PaginatorConfigTypeDef",
+    "PolicyVersionIdentifierOutputTypeDef",
     "PolicyVersionIdentifierTypeDef",
     "PutVerificationStateOnViolationRequestRequestTypeDef",
+    "RegistrationConfigTypeDef",
     "RegisterCACertificateResponseTypeDef",
     "RegisterCertificateRequestRequestTypeDef",
     "RegisterCertificateResponseTypeDef",
     "RegisterCertificateWithoutCARequestRequestTypeDef",
     "RegisterCertificateWithoutCAResponseTypeDef",
     "RegisterThingRequestRequestTypeDef",
     "RegisterThingResponseTypeDef",
@@ -511,25 +579,29 @@
     "ResponseMetadataTypeDef",
     "SearchIndexRequestRequestTypeDef",
     "ThingGroupDocumentTypeDef",
     "SetDefaultAuthorizerRequestRequestTypeDef",
     "SetDefaultAuthorizerResponseTypeDef",
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     "SetV2LoggingOptionsRequestRequestTypeDef",
+    "SigningProfileParameterOutputTypeDef",
     "SigningProfileParameterTypeDef",
     "StartAuditMitigationActionsTaskResponseTypeDef",
+    "ViolationEventOccurrenceRangeTypeDef",
     "StartDetectMitigationActionsTaskResponseTypeDef",
     "StartOnDemandAuditTaskRequestRequestTypeDef",
     "StartOnDemandAuditTaskResponseTypeDef",
     "StartThingRegistrationTaskRequestRequestTypeDef",
     "StartThingRegistrationTaskResponseTypeDef",
     "StopThingRegistrationTaskRequestRequestTypeDef",
     "TlsContextTypeDef",
     "TestInvokeAuthorizerResponseTypeDef",
     "ThingConnectivityTypeDef",
+    "TimestreamDimensionOutputTypeDef",
+    "TimestreamTimestampOutputTypeDef",
     "TimestreamDimensionTypeDef",
     "TimestreamTimestampTypeDef",
     "VpcDestinationConfigurationTypeDef",
     "VpcDestinationSummaryTypeDef",
     "VpcDestinationPropertiesTypeDef",
     "TransferCertificateRequestRequestTypeDef",
     "TransferCertificateResponseTypeDef",
@@ -541,117 +613,130 @@
     "UpdateCustomMetricRequestRequestTypeDef",
     "UpdateCustomMetricResponseTypeDef",
     "UpdateDimensionRequestRequestTypeDef",
     "UpdateDimensionResponseTypeDef",
     "UpdateDomainConfigurationResponseTypeDef",
     "UpdateDynamicThingGroupResponseTypeDef",
     "UpdateMitigationActionResponseTypeDef",
+    "VersionUpdateByJobsConfigTypeDef",
     "UpdatePackageRequestRequestTypeDef",
     "UpdatePackageVersionRequestRequestTypeDef",
     "UpdateRoleAliasRequestRequestTypeDef",
     "UpdateRoleAliasResponseTypeDef",
     "UpdateScheduledAuditRequestRequestTypeDef",
     "UpdateScheduledAuditResponseTypeDef",
     "UpdateStreamResponseTypeDef",
     "UpdateThingGroupResponseTypeDef",
     "UpdateThingGroupsForThingRequestRequestTypeDef",
     "UpdateTopicRuleDestinationRequestRequestTypeDef",
     "ValidationErrorTypeDef",
+    "AbortConfigOutputTypeDef",
     "AbortConfigTypeDef",
     "MetricDatumTypeDef",
     "DescribeFleetMetricResponseTypeDef",
     "UpdateFleetMetricRequestRequestTypeDef",
     "AllowedTypeDef",
     "ExplicitDenyTypeDef",
     "ImplicitDenyTypeDef",
     "ListAttachedPoliciesResponseTypeDef",
     "ListPoliciesResponseTypeDef",
     "ListPrincipalPoliciesResponseTypeDef",
+    "AssetPropertyValueOutputTypeDef",
     "AssetPropertyValueTypeDef",
+    "ThingGroupPropertiesOutputTypeDef",
     "CreateThingRequestRequestTypeDef",
     "ThingGroupPropertiesTypeDef",
     "UpdateThingRequestRequestTypeDef",
     "ListAuditMitigationActionsExecutionsResponseTypeDef",
     "ListAuditMitigationActionsTasksResponseTypeDef",
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     "DescribeAccountAuditConfigurationResponseTypeDef",
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     "ListAuditTasksResponseTypeDef",
     "TestAuthorizationRequestRequestTypeDef",
     "DescribeAuthorizerResponseTypeDef",
     "DescribeDefaultAuthorizerResponseTypeDef",
     "ListAuthorizersResponseTypeDef",
     "AwsJobAbortConfigTypeDef",
+    "AwsJobExponentialRolloutRateOutputTypeDef",
     "AwsJobExponentialRolloutRateTypeDef",
+    "BehaviorCriteriaOutputTypeDef",
     "BehaviorCriteriaTypeDef",
     "GetBehaviorModelTrainingSummariesResponseTypeDef",
+    "MetricToRetainOutputTypeDef",
     "MetricToRetainTypeDef",
     "DescribeBillingGroupResponseTypeDef",
     "UpdateBillingGroupRequestRequestTypeDef",
     "GetBucketsAggregationResponseTypeDef",
     "BucketsAggregationTypeTypeDef",
     "CACertificateDescriptionTypeDef",
     "ListCACertificatesResponseTypeDef",
     "CertificateDescriptionTypeDef",
     "ListCertificatesByCAResponseTypeDef",
     "ListCertificatesResponseTypeDef",
+    "CustomCodeSigningOutputTypeDef",
     "CustomCodeSigningTypeDef",
     "DescribeEventConfigurationsResponseTypeDef",
     "UpdateEventConfigurationsRequestRequestTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
     "CreateBillingGroupRequestRequestTypeDef",
     "CreateCustomMetricRequestRequestTypeDef",
     "CreateDimensionRequestRequestTypeDef",
     "CreateFleetMetricRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreateRoleAliasRequestRequestTypeDef",
     "CreateScheduledAuditRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainConfigurationRequestRequestTypeDef",
     "UpdateDomainConfigurationRequestRequestTypeDef",
     "SchedulingConfigTypeDef",
     "CreateKeysAndCertificateResponseTypeDef",
     "CreateProvisioningClaimResponseTypeDef",
     "CreateProvisioningTemplateRequestRequestTypeDef",
-    "DescribeProvisioningTemplateResponseTypeDef",
     "UpdateProvisioningTemplateRequestRequestTypeDef",
     "CreateThingTypeRequestRequestTypeDef",
     "DescribeAuditTaskResponseTypeDef",
-    "RegisterCACertificateRequestRequestTypeDef",
-    "UpdateCACertificateRequestRequestTypeDef",
     "DescribeDomainConfigurationResponseTypeDef",
+    "SchedulingConfigOutputTypeDef",
     "DescribeManagedJobTemplateResponseTypeDef",
+    "DescribeProvisioningTemplateResponseTypeDef",
     "DescribeRoleAliasResponseTypeDef",
     "DescribeThingTypeResponseTypeDef",
     "ThingTypeDefinitionTypeDef",
+    "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "ListDetectMitigationActionsExecutionsResponseTypeDef",
-    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
     "ListDomainConfigurationsResponseTypeDef",
+    "DynamoDBv2ActionOutputTypeDef",
     "DynamoDBv2ActionTypeDef",
     "GetEffectivePoliciesResponseTypeDef",
+    "ExponentialRolloutRateOutputTypeDef",
     "ExponentialRolloutRateTypeDef",
+    "ThingGroupIndexingConfigurationOutputTypeDef",
     "ThingGroupIndexingConfigurationTypeDef",
+    "StreamFileOutputTypeDef",
+    "FileLocationOutputTypeDef",
     "StreamFileTypeDef",
     "FileLocationTypeDef",
     "ListFleetMetricsResponseTypeDef",
     "GetPackageConfigurationResponseTypeDef",
-    "UpdatePackageConfigurationRequestRequestTypeDef",
     "GetPercentilesResponseTypeDef",
     "GetStatisticsResponseTypeDef",
     "ListBillingGroupsResponseTypeDef",
     "ListThingGroupsForThingResponseTypeDef",
     "ListThingGroupsResponseTypeDef",
     "ThingGroupMetadataTypeDef",
+    "HttpAuthorizationOutputTypeDef",
     "HttpAuthorizationTypeDef",
+    "ThingIndexingConfigurationOutputTypeDef",
     "ThingIndexingConfigurationTypeDef",
     "JobExecutionTypeDef",
     "JobExecutionSummaryForJobTypeDef",
     "JobExecutionSummaryForThingTypeDef",
+    "JobExecutionsRetryConfigOutputTypeDef",
     "JobExecutionsRetryConfigTypeDef",
     "ListJobsResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
     "ListManagedJobTemplatesResponseTypeDef",
     "ListMitigationActionsResponseTypeDef",
     "ListOTAUpdatesResponseTypeDef",
     "ListOutgoingCertificatesResponseTypeDef",
@@ -659,122 +744,153 @@
     "ListPackagesResponseTypeDef",
     "ListPolicyVersionsResponseTypeDef",
     "ListProvisioningTemplateVersionsResponseTypeDef",
     "ListProvisioningTemplatesResponseTypeDef",
     "ListScheduledAuditsResponseTypeDef",
     "ListSecurityProfilesResponseTypeDef",
     "ListStreamsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTargetsForSecurityProfileResponseTypeDef",
     "SecurityProfileTargetMappingTypeDef",
     "ListThingsResponseTypeDef",
     "ListTopicRulesResponseTypeDef",
+    "LocationActionOutputTypeDef",
     "LocationActionTypeDef",
     "LogTargetConfigurationTypeDef",
     "SetV2LoggingLevelRequestRequestTypeDef",
     "SetLoggingOptionsRequestRequestTypeDef",
+    "MitigationActionParamsOutputTypeDef",
     "MitigationActionParamsTypeDef",
+    "MqttHeadersOutputTypeDef",
     "MqttHeadersTypeDef",
+    "ResourceIdentifierOutputTypeDef",
     "ResourceIdentifierTypeDef",
+    "RegisterCACertificateRequestRequestTypeDef",
+    "UpdateCACertificateRequestRequestTypeDef",
+    "StartDetectMitigationActionsTaskRequestRequestTypeDef",
     "TestInvokeAuthorizerRequestRequestTypeDef",
     "ThingDocumentTypeDef",
+    "TimestreamActionOutputTypeDef",
     "TimestreamActionTypeDef",
     "TopicRuleDestinationConfigurationTypeDef",
     "TopicRuleDestinationSummaryTypeDef",
     "TopicRuleDestinationTypeDef",
+    "UpdatePackageConfigurationRequestRequestTypeDef",
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
     "ListMetricValuesResponseTypeDef",
     "DeniedTypeDef",
+    "PutAssetPropertyValueEntryOutputTypeDef",
     "PutAssetPropertyValueEntryTypeDef",
     "CreateDynamicThingGroupRequestRequestTypeDef",
     "CreateThingGroupRequestRequestTypeDef",
     "UpdateDynamicThingGroupRequestRequestTypeDef",
     "UpdateThingGroupRequestRequestTypeDef",
+    "AwsJobExecutionsRolloutConfigOutputTypeDef",
     "AwsJobExecutionsRolloutConfigTypeDef",
+    "BehaviorOutputTypeDef",
     "BehaviorTypeDef",
     "GetBucketsAggregationRequestRequestTypeDef",
     "DescribeCACertificateResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
     "ListThingTypesResponseTypeDef",
+    "StartSigningJobParameterOutputTypeDef",
     "StartSigningJobParameterTypeDef",
+    "JobExecutionsRolloutConfigOutputTypeDef",
     "JobExecutionsRolloutConfigTypeDef",
-    "CreateStreamRequestRequestTypeDef",
     "StreamInfoTypeDef",
+    "CreateStreamRequestRequestTypeDef",
     "UpdateStreamRequestRequestTypeDef",
     "DescribeThingGroupResponseTypeDef",
+    "HttpActionOutputTypeDef",
     "HttpActionTypeDef",
     "GetIndexingConfigurationResponseTypeDef",
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     "DescribeJobExecutionResponseTypeDef",
     "ListJobExecutionsForJobResponseTypeDef",
     "ListJobExecutionsForThingResponseTypeDef",
     "ListSecurityProfilesForTargetResponseTypeDef",
     "ListV2LoggingLevelsResponseTypeDef",
-    "CreateMitigationActionRequestRequestTypeDef",
     "DescribeMitigationActionResponseTypeDef",
     "MitigationActionTypeDef",
+    "CreateMitigationActionRequestRequestTypeDef",
     "UpdateMitigationActionRequestRequestTypeDef",
+    "RepublishActionOutputTypeDef",
     "RepublishActionTypeDef",
     "AuditSuppressionTypeDef",
+    "DescribeAuditSuppressionResponseTypeDef",
+    "NonCompliantResourceTypeDef",
+    "RelatedResourceTypeDef",
     "CreateAuditSuppressionRequestRequestTypeDef",
     "DeleteAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionRequestRequestTypeDef",
-    "DescribeAuditSuppressionResponseTypeDef",
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
     "ListAuditFindingsRequestRequestTypeDef",
     "ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef",
     "ListAuditSuppressionsRequestRequestTypeDef",
-    "NonCompliantResourceTypeDef",
-    "RelatedResourceTypeDef",
     "UpdateAuditSuppressionRequestRequestTypeDef",
     "SearchIndexResponseTypeDef",
     "CreateTopicRuleDestinationRequestRequestTypeDef",
     "ListTopicRuleDestinationsResponseTypeDef",
     "CreateTopicRuleDestinationResponseTypeDef",
     "GetTopicRuleDestinationResponseTypeDef",
     "AuthResultTypeDef",
+    "IotSiteWiseActionOutputTypeDef",
     "IotSiteWiseActionTypeDef",
     "ActiveViolationTypeDef",
-    "CreateSecurityProfileRequestRequestTypeDef",
     "DescribeSecurityProfileResponseTypeDef",
-    "UpdateSecurityProfileRequestRequestTypeDef",
     "UpdateSecurityProfileResponseTypeDef",
-    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
     "ViolationEventTypeDef",
+    "CreateSecurityProfileRequestRequestTypeDef",
+    "UpdateSecurityProfileRequestRequestTypeDef",
+    "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
+    "CodeSigningOutputTypeDef",
     "CodeSigningTypeDef",
-    "CreateJobRequestRequestTypeDef",
-    "CreateJobTemplateRequestRequestTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "JobTypeDef",
+    "CreateJobRequestRequestTypeDef",
+    "CreateJobTemplateRequestRequestTypeDef",
     "UpdateJobRequestRequestTypeDef",
     "DescribeStreamResponseTypeDef",
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     "DetectMitigationActionsTaskSummaryTypeDef",
     "ListAuditSuppressionsResponseTypeDef",
     "AuditFindingTypeDef",
     "ListRelatedResourcesForAuditFindingResponseTypeDef",
     "TestAuthorizationResponseTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListActiveViolationsResponseTypeDef",
     "ListViolationEventsResponseTypeDef",
+    "OTAUpdateFileOutputTypeDef",
     "OTAUpdateFileTypeDef",
     "DescribeJobResponseTypeDef",
     "DescribeDetectMitigationActionsTaskResponseTypeDef",
     "ListDetectMitigationActionsTasksResponseTypeDef",
     "DescribeAuditFindingResponseTypeDef",
     "ListAuditFindingsResponseTypeDef",
-    "TopicRulePayloadTypeDef",
     "TopicRuleTypeDef",
-    "CreateOTAUpdateRequestRequestTypeDef",
+    "TopicRulePayloadTypeDef",
     "OTAUpdateInfoTypeDef",
+    "CreateOTAUpdateRequestRequestTypeDef",
+    "GetTopicRuleResponseTypeDef",
     "CreateTopicRuleRequestRequestTypeDef",
     "ReplaceTopicRuleRequestRequestTypeDef",
-    "GetTopicRuleResponseTypeDef",
     "GetOTAUpdateResponseTypeDef",
 )
 
+AbortCriteriaOutputTypeDef = TypedDict(
+    "AbortCriteriaOutputTypeDef",
+    {
+        "failureType": JobExecutionFailureTypeType,
+        "action": Literal["CANCEL"],
+        "thresholdPercentage": float,
+        "minNumberOfExecutedThings": int,
+    },
+)
+
 AbortCriteriaTypeDef = TypedDict(
     "AbortCriteriaTypeDef",
     {
         "failureType": JobExecutionFailureTypeType,
         "action": Literal["CANCEL"],
         "thresholdPercentage": float,
         "minNumberOfExecutedThings": int,
@@ -797,14 +913,301 @@
 
 class AcceptCertificateTransferRequestRequestTypeDef(
     _RequiredAcceptCertificateTransferRequestRequestTypeDef,
     _OptionalAcceptCertificateTransferRequestRequestTypeDef,
 ):
     pass
 
+CloudwatchAlarmActionOutputTypeDef = TypedDict(
+    "CloudwatchAlarmActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "alarmName": str,
+        "stateReason": str,
+        "stateValue": str,
+    },
+)
+
+_RequiredCloudwatchLogsActionOutputTypeDef = TypedDict(
+    "_RequiredCloudwatchLogsActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "logGroupName": str,
+    },
+)
+_OptionalCloudwatchLogsActionOutputTypeDef = TypedDict(
+    "_OptionalCloudwatchLogsActionOutputTypeDef",
+    {
+        "batchMode": bool,
+    },
+    total=False,
+)
+
+class CloudwatchLogsActionOutputTypeDef(
+    _RequiredCloudwatchLogsActionOutputTypeDef, _OptionalCloudwatchLogsActionOutputTypeDef
+):
+    pass
+
+_RequiredCloudwatchMetricActionOutputTypeDef = TypedDict(
+    "_RequiredCloudwatchMetricActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "metricNamespace": str,
+        "metricName": str,
+        "metricValue": str,
+        "metricUnit": str,
+    },
+)
+_OptionalCloudwatchMetricActionOutputTypeDef = TypedDict(
+    "_OptionalCloudwatchMetricActionOutputTypeDef",
+    {
+        "metricTimestamp": str,
+    },
+    total=False,
+)
+
+class CloudwatchMetricActionOutputTypeDef(
+    _RequiredCloudwatchMetricActionOutputTypeDef, _OptionalCloudwatchMetricActionOutputTypeDef
+):
+    pass
+
+_RequiredDynamoDBActionOutputTypeDef = TypedDict(
+    "_RequiredDynamoDBActionOutputTypeDef",
+    {
+        "tableName": str,
+        "roleArn": str,
+        "hashKeyField": str,
+        "hashKeyValue": str,
+    },
+)
+_OptionalDynamoDBActionOutputTypeDef = TypedDict(
+    "_OptionalDynamoDBActionOutputTypeDef",
+    {
+        "operation": str,
+        "hashKeyType": DynamoKeyTypeType,
+        "rangeKeyField": str,
+        "rangeKeyValue": str,
+        "rangeKeyType": DynamoKeyTypeType,
+        "payloadField": str,
+    },
+    total=False,
+)
+
+class DynamoDBActionOutputTypeDef(
+    _RequiredDynamoDBActionOutputTypeDef, _OptionalDynamoDBActionOutputTypeDef
+):
+    pass
+
+ElasticsearchActionOutputTypeDef = TypedDict(
+    "ElasticsearchActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "endpoint": str,
+        "index": str,
+        "type": str,
+        "id": str,
+    },
+)
+
+_RequiredFirehoseActionOutputTypeDef = TypedDict(
+    "_RequiredFirehoseActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "deliveryStreamName": str,
+    },
+)
+_OptionalFirehoseActionOutputTypeDef = TypedDict(
+    "_OptionalFirehoseActionOutputTypeDef",
+    {
+        "separator": str,
+        "batchMode": bool,
+    },
+    total=False,
+)
+
+class FirehoseActionOutputTypeDef(
+    _RequiredFirehoseActionOutputTypeDef, _OptionalFirehoseActionOutputTypeDef
+):
+    pass
+
+IotAnalyticsActionOutputTypeDef = TypedDict(
+    "IotAnalyticsActionOutputTypeDef",
+    {
+        "channelArn": str,
+        "channelName": str,
+        "batchMode": bool,
+        "roleArn": str,
+    },
+    total=False,
+)
+
+_RequiredIotEventsActionOutputTypeDef = TypedDict(
+    "_RequiredIotEventsActionOutputTypeDef",
+    {
+        "inputName": str,
+        "roleArn": str,
+    },
+)
+_OptionalIotEventsActionOutputTypeDef = TypedDict(
+    "_OptionalIotEventsActionOutputTypeDef",
+    {
+        "messageId": str,
+        "batchMode": bool,
+    },
+    total=False,
+)
+
+class IotEventsActionOutputTypeDef(
+    _RequiredIotEventsActionOutputTypeDef, _OptionalIotEventsActionOutputTypeDef
+):
+    pass
+
+_RequiredKafkaActionOutputTypeDef = TypedDict(
+    "_RequiredKafkaActionOutputTypeDef",
+    {
+        "destinationArn": str,
+        "topic": str,
+        "clientProperties": Dict[str, str],
+    },
+)
+_OptionalKafkaActionOutputTypeDef = TypedDict(
+    "_OptionalKafkaActionOutputTypeDef",
+    {
+        "key": str,
+        "partition": str,
+    },
+    total=False,
+)
+
+class KafkaActionOutputTypeDef(
+    _RequiredKafkaActionOutputTypeDef, _OptionalKafkaActionOutputTypeDef
+):
+    pass
+
+_RequiredKinesisActionOutputTypeDef = TypedDict(
+    "_RequiredKinesisActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "streamName": str,
+    },
+)
+_OptionalKinesisActionOutputTypeDef = TypedDict(
+    "_OptionalKinesisActionOutputTypeDef",
+    {
+        "partitionKey": str,
+    },
+    total=False,
+)
+
+class KinesisActionOutputTypeDef(
+    _RequiredKinesisActionOutputTypeDef, _OptionalKinesisActionOutputTypeDef
+):
+    pass
+
+LambdaActionOutputTypeDef = TypedDict(
+    "LambdaActionOutputTypeDef",
+    {
+        "functionArn": str,
+    },
+)
+
+OpenSearchActionOutputTypeDef = TypedDict(
+    "OpenSearchActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "endpoint": str,
+        "index": str,
+        "type": str,
+        "id": str,
+    },
+)
+
+_RequiredS3ActionOutputTypeDef = TypedDict(
+    "_RequiredS3ActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "bucketName": str,
+        "key": str,
+    },
+)
+_OptionalS3ActionOutputTypeDef = TypedDict(
+    "_OptionalS3ActionOutputTypeDef",
+    {
+        "cannedAcl": CannedAccessControlListType,
+    },
+    total=False,
+)
+
+class S3ActionOutputTypeDef(_RequiredS3ActionOutputTypeDef, _OptionalS3ActionOutputTypeDef):
+    pass
+
+SalesforceActionOutputTypeDef = TypedDict(
+    "SalesforceActionOutputTypeDef",
+    {
+        "token": str,
+        "url": str,
+    },
+)
+
+_RequiredSnsActionOutputTypeDef = TypedDict(
+    "_RequiredSnsActionOutputTypeDef",
+    {
+        "targetArn": str,
+        "roleArn": str,
+    },
+)
+_OptionalSnsActionOutputTypeDef = TypedDict(
+    "_OptionalSnsActionOutputTypeDef",
+    {
+        "messageFormat": MessageFormatType,
+    },
+    total=False,
+)
+
+class SnsActionOutputTypeDef(_RequiredSnsActionOutputTypeDef, _OptionalSnsActionOutputTypeDef):
+    pass
+
+_RequiredSqsActionOutputTypeDef = TypedDict(
+    "_RequiredSqsActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "queueUrl": str,
+    },
+)
+_OptionalSqsActionOutputTypeDef = TypedDict(
+    "_OptionalSqsActionOutputTypeDef",
+    {
+        "useBase64": bool,
+    },
+    total=False,
+)
+
+class SqsActionOutputTypeDef(_RequiredSqsActionOutputTypeDef, _OptionalSqsActionOutputTypeDef):
+    pass
+
+_RequiredStepFunctionsActionOutputTypeDef = TypedDict(
+    "_RequiredStepFunctionsActionOutputTypeDef",
+    {
+        "stateMachineName": str,
+        "roleArn": str,
+    },
+)
+_OptionalStepFunctionsActionOutputTypeDef = TypedDict(
+    "_OptionalStepFunctionsActionOutputTypeDef",
+    {
+        "executionNamePrefix": str,
+    },
+    total=False,
+)
+
+class StepFunctionsActionOutputTypeDef(
+    _RequiredStepFunctionsActionOutputTypeDef, _OptionalStepFunctionsActionOutputTypeDef
+):
+    pass
+
 CloudwatchAlarmActionTypeDef = TypedDict(
     "CloudwatchAlarmActionTypeDef",
     {
         "roleArn": str,
         "alarmName": str,
         "stateReason": str,
         "stateValue": str,
@@ -1074,23 +1477,23 @@
 )
 
 class StepFunctionsActionTypeDef(
     _RequiredStepFunctionsActionTypeDef, _OptionalStepFunctionsActionTypeDef
 ):
     pass
 
-MetricValueTypeDef = TypedDict(
-    "MetricValueTypeDef",
+MetricValueOutputTypeDef = TypedDict(
+    "MetricValueOutputTypeDef",
     {
         "count": int,
-        "cidrs": Sequence[str],
-        "ports": Sequence[int],
+        "cidrs": List[str],
+        "ports": List[int],
         "number": float,
-        "numbers": Sequence[float],
-        "strings": Sequence[str],
+        "numbers": List[float],
+        "strings": List[str],
     },
     total=False,
 )
 
 ViolationEventAdditionalInfoTypeDef = TypedDict(
     "ViolationEventAdditionalInfoTypeDef",
     {
@@ -1118,14 +1521,34 @@
         "thingName": str,
         "thingArn": str,
         "overrideDynamicGroups": bool,
     },
     total=False,
 )
 
+_RequiredAddThingsToThingGroupParamsOutputTypeDef = TypedDict(
+    "_RequiredAddThingsToThingGroupParamsOutputTypeDef",
+    {
+        "thingGroupNames": List[str],
+    },
+)
+_OptionalAddThingsToThingGroupParamsOutputTypeDef = TypedDict(
+    "_OptionalAddThingsToThingGroupParamsOutputTypeDef",
+    {
+        "overrideDynamicGroups": bool,
+    },
+    total=False,
+)
+
+class AddThingsToThingGroupParamsOutputTypeDef(
+    _RequiredAddThingsToThingGroupParamsOutputTypeDef,
+    _OptionalAddThingsToThingGroupParamsOutputTypeDef,
+):
+    pass
+
 _RequiredAddThingsToThingGroupParamsTypeDef = TypedDict(
     "_RequiredAddThingsToThingGroupParamsTypeDef",
     {
         "thingGroupNames": Sequence[str],
     },
 )
 _OptionalAddThingsToThingGroupParamsTypeDef = TypedDict(
@@ -1137,14 +1560,33 @@
 )
 
 class AddThingsToThingGroupParamsTypeDef(
     _RequiredAddThingsToThingGroupParamsTypeDef, _OptionalAddThingsToThingGroupParamsTypeDef
 ):
     pass
 
+_RequiredAggregationTypeOutputTypeDef = TypedDict(
+    "_RequiredAggregationTypeOutputTypeDef",
+    {
+        "name": AggregationTypeNameType,
+    },
+)
+_OptionalAggregationTypeOutputTypeDef = TypedDict(
+    "_OptionalAggregationTypeOutputTypeDef",
+    {
+        "values": List[str],
+    },
+    total=False,
+)
+
+class AggregationTypeOutputTypeDef(
+    _RequiredAggregationTypeOutputTypeDef, _OptionalAggregationTypeOutputTypeDef
+):
+    pass
+
 _RequiredAggregationTypeTypeDef = TypedDict(
     "_RequiredAggregationTypeTypeDef",
     {
         "name": AggregationTypeNameType,
     },
 )
 _OptionalAggregationTypeTypeDef = TypedDict(
@@ -1154,14 +1596,22 @@
     },
     total=False,
 )
 
 class AggregationTypeTypeDef(_RequiredAggregationTypeTypeDef, _OptionalAggregationTypeTypeDef):
     pass
 
+AlertTargetOutputTypeDef = TypedDict(
+    "AlertTargetOutputTypeDef",
+    {
+        "alertTargetArn": str,
+        "roleArn": str,
+    },
+)
+
 AlertTargetTypeDef = TypedDict(
     "AlertTargetTypeDef",
     {
         "alertTargetArn": str,
         "roleArn": str,
     },
 )
@@ -1171,14 +1621,33 @@
     {
         "policyName": str,
         "policyArn": str,
     },
     total=False,
 )
 
+_RequiredAssetPropertyTimestampOutputTypeDef = TypedDict(
+    "_RequiredAssetPropertyTimestampOutputTypeDef",
+    {
+        "timeInSeconds": str,
+    },
+)
+_OptionalAssetPropertyTimestampOutputTypeDef = TypedDict(
+    "_OptionalAssetPropertyTimestampOutputTypeDef",
+    {
+        "offsetInNanos": str,
+    },
+    total=False,
+)
+
+class AssetPropertyTimestampOutputTypeDef(
+    _RequiredAssetPropertyTimestampOutputTypeDef, _OptionalAssetPropertyTimestampOutputTypeDef
+):
+    pass
+
 _RequiredAssetPropertyTimestampTypeDef = TypedDict(
     "_RequiredAssetPropertyTimestampTypeDef",
     {
         "timeInSeconds": str,
     },
 )
 _OptionalAssetPropertyTimestampTypeDef = TypedDict(
@@ -1190,14 +1659,25 @@
 )
 
 class AssetPropertyTimestampTypeDef(
     _RequiredAssetPropertyTimestampTypeDef, _OptionalAssetPropertyTimestampTypeDef
 ):
     pass
 
+AssetPropertyVariantOutputTypeDef = TypedDict(
+    "AssetPropertyVariantOutputTypeDef",
+    {
+        "stringValue": str,
+        "integerValue": str,
+        "doubleValue": str,
+        "booleanValue": str,
+    },
+    total=False,
+)
+
 AssetPropertyVariantTypeDef = TypedDict(
     "AssetPropertyVariantTypeDef",
     {
         "stringValue": str,
         "integerValue": str,
         "doubleValue": str,
         "booleanValue": str,
@@ -1265,23 +1745,40 @@
     "AttachThingPrincipalRequestRequestTypeDef",
     {
         "thingName": str,
         "principal": str,
     },
 )
 
+AttributePayloadOutputTypeDef = TypedDict(
+    "AttributePayloadOutputTypeDef",
+    {
+        "attributes": Dict[str, str],
+        "merge": bool,
+    },
+    total=False,
+)
+
 AttributePayloadTypeDef = TypedDict(
     "AttributePayloadTypeDef",
     {
         "attributes": Mapping[str, str],
         "merge": bool,
     },
     total=False,
 )
 
+AuditCheckConfigurationOutputTypeDef = TypedDict(
+    "AuditCheckConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+    total=False,
+)
+
 AuditCheckConfigurationTypeDef = TypedDict(
     "AuditCheckConfigurationTypeDef",
     {
         "enabled": bool,
     },
     total=False,
 )
@@ -1322,24 +1819,44 @@
         "taskId": str,
         "startTime": datetime,
         "taskStatus": AuditMitigationActionsTaskStatusType,
     },
     total=False,
 )
 
-AuditMitigationActionsTaskTargetTypeDef = TypedDict(
-    "AuditMitigationActionsTaskTargetTypeDef",
+AuditMitigationActionsTaskTargetOutputTypeDef = TypedDict(
+    "AuditMitigationActionsTaskTargetOutputTypeDef",
     {
         "auditTaskId": str,
         "findingIds": List[str],
         "auditCheckToReasonCodeFilter": Dict[str, List[str]],
     },
     total=False,
 )
 
+AuditMitigationActionsTaskTargetTypeDef = TypedDict(
+    "AuditMitigationActionsTaskTargetTypeDef",
+    {
+        "auditTaskId": str,
+        "findingIds": Sequence[str],
+        "auditCheckToReasonCodeFilter": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
+AuditNotificationTargetOutputTypeDef = TypedDict(
+    "AuditNotificationTargetOutputTypeDef",
+    {
+        "targetArn": str,
+        "roleArn": str,
+        "enabled": bool,
+    },
+    total=False,
+)
+
 AuditNotificationTargetTypeDef = TypedDict(
     "AuditNotificationTargetTypeDef",
     {
         "targetArn": str,
         "roleArn": str,
         "enabled": bool,
     },
@@ -1352,14 +1869,31 @@
         "taskId": str,
         "taskStatus": AuditTaskStatusType,
         "taskType": AuditTaskTypeType,
     },
     total=False,
 )
 
+_RequiredAuthInfoOutputTypeDef = TypedDict(
+    "_RequiredAuthInfoOutputTypeDef",
+    {
+        "resources": List[str],
+    },
+)
+_OptionalAuthInfoOutputTypeDef = TypedDict(
+    "_OptionalAuthInfoOutputTypeDef",
+    {
+        "actionType": ActionTypeType,
+    },
+    total=False,
+)
+
+class AuthInfoOutputTypeDef(_RequiredAuthInfoOutputTypeDef, _OptionalAuthInfoOutputTypeDef):
+    pass
+
 _RequiredAuthInfoTypeDef = TypedDict(
     "_RequiredAuthInfoTypeDef",
     {
         "resources": Sequence[str],
     },
 )
 _OptionalAuthInfoTypeDef = TypedDict(
@@ -1369,14 +1903,23 @@
     },
     total=False,
 )
 
 class AuthInfoTypeDef(_RequiredAuthInfoTypeDef, _OptionalAuthInfoTypeDef):
     pass
 
+AuthorizerConfigOutputTypeDef = TypedDict(
+    "AuthorizerConfigOutputTypeDef",
+    {
+        "defaultAuthorizerName": str,
+        "allowAuthorizerOverride": bool,
+    },
+    total=False,
+)
+
 AuthorizerConfigTypeDef = TypedDict(
     "AuthorizerConfigTypeDef",
     {
         "defaultAuthorizerName": str,
         "allowAuthorizerOverride": bool,
     },
     total=False,
@@ -1414,23 +1957,40 @@
         "failureType": AwsJobAbortCriteriaFailureTypeType,
         "action": Literal["CANCEL"],
         "thresholdPercentage": float,
         "minNumberOfExecutedThings": int,
     },
 )
 
+AwsJobRateIncreaseCriteriaOutputTypeDef = TypedDict(
+    "AwsJobRateIncreaseCriteriaOutputTypeDef",
+    {
+        "numberOfNotifiedThings": int,
+        "numberOfSucceededThings": int,
+    },
+    total=False,
+)
+
 AwsJobRateIncreaseCriteriaTypeDef = TypedDict(
     "AwsJobRateIncreaseCriteriaTypeDef",
     {
         "numberOfNotifiedThings": int,
         "numberOfSucceededThings": int,
     },
     total=False,
 )
 
+AwsJobPresignedUrlConfigOutputTypeDef = TypedDict(
+    "AwsJobPresignedUrlConfigOutputTypeDef",
+    {
+        "expiresInSec": int,
+    },
+    total=False,
+)
+
 AwsJobPresignedUrlConfigTypeDef = TypedDict(
     "AwsJobPresignedUrlConfigTypeDef",
     {
         "expiresInSec": int,
     },
     total=False,
 )
@@ -1439,21 +1999,49 @@
     "AwsJobTimeoutConfigTypeDef",
     {
         "inProgressTimeoutInMinutes": int,
     },
     total=False,
 )
 
+MachineLearningDetectionConfigOutputTypeDef = TypedDict(
+    "MachineLearningDetectionConfigOutputTypeDef",
+    {
+        "confidenceLevel": ConfidenceLevelType,
+    },
+)
+
+StatisticalThresholdOutputTypeDef = TypedDict(
+    "StatisticalThresholdOutputTypeDef",
+    {
+        "statistic": str,
+    },
+    total=False,
+)
+
 MachineLearningDetectionConfigTypeDef = TypedDict(
     "MachineLearningDetectionConfigTypeDef",
     {
         "confidenceLevel": ConfidenceLevelType,
     },
 )
 
+MetricValueTypeDef = TypedDict(
+    "MetricValueTypeDef",
+    {
+        "count": int,
+        "cidrs": Sequence[str],
+        "ports": Sequence[int],
+        "number": float,
+        "numbers": Sequence[float],
+        "strings": Sequence[str],
+    },
+    total=False,
+)
+
 StatisticalThresholdTypeDef = TypedDict(
     "StatisticalThresholdTypeDef",
     {
         "statistic": str,
     },
     total=False,
 )
@@ -1467,14 +2055,33 @@
         "modelStatus": ModelStatusType,
         "datapointsCollectionPercentage": float,
         "lastModelRefreshDate": datetime,
     },
     total=False,
 )
 
+_RequiredMetricDimensionOutputTypeDef = TypedDict(
+    "_RequiredMetricDimensionOutputTypeDef",
+    {
+        "dimensionName": str,
+    },
+)
+_OptionalMetricDimensionOutputTypeDef = TypedDict(
+    "_OptionalMetricDimensionOutputTypeDef",
+    {
+        "operator": DimensionValueOperatorType,
+    },
+    total=False,
+)
+
+class MetricDimensionOutputTypeDef(
+    _RequiredMetricDimensionOutputTypeDef, _OptionalMetricDimensionOutputTypeDef
+):
+    pass
+
 _RequiredMetricDimensionTypeDef = TypedDict(
     "_RequiredMetricDimensionTypeDef",
     {
         "dimensionName": str,
     },
 )
 _OptionalMetricDimensionTypeDef = TypedDict(
@@ -1492,14 +2099,22 @@
     "BillingGroupMetadataTypeDef",
     {
         "creationDate": datetime,
     },
     total=False,
 )
 
+BillingGroupPropertiesOutputTypeDef = TypedDict(
+    "BillingGroupPropertiesOutputTypeDef",
+    {
+        "billingGroupDescription": str,
+    },
+    total=False,
+)
+
 BillingGroupPropertiesTypeDef = TypedDict(
     "BillingGroupPropertiesTypeDef",
     {
         "billingGroupDescription": str,
     },
     total=False,
 )
@@ -1643,31 +2258,56 @@
         "status": CertificateStatusType,
         "certificateMode": CertificateModeType,
         "creationDate": datetime,
     },
     total=False,
 )
 
+CodeSigningCertificateChainOutputTypeDef = TypedDict(
+    "CodeSigningCertificateChainOutputTypeDef",
+    {
+        "certificateName": str,
+        "inlineDocument": str,
+    },
+    total=False,
+)
+
 CodeSigningCertificateChainTypeDef = TypedDict(
     "CodeSigningCertificateChainTypeDef",
     {
         "certificateName": str,
         "inlineDocument": str,
     },
     total=False,
 )
 
+CodeSigningSignatureOutputTypeDef = TypedDict(
+    "CodeSigningSignatureOutputTypeDef",
+    {
+        "inlineDocument": bytes,
+    },
+    total=False,
+)
+
 CodeSigningSignatureTypeDef = TypedDict(
     "CodeSigningSignatureTypeDef",
     {
         "inlineDocument": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
+ConfigurationOutputTypeDef = TypedDict(
+    "ConfigurationOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -2598,16 +3238,16 @@
 DescribeCACertificateRequestRequestTypeDef = TypedDict(
     "DescribeCACertificateRequestRequestTypeDef",
     {
         "certificateId": str,
     },
 )
 
-RegistrationConfigTypeDef = TypedDict(
-    "RegistrationConfigTypeDef",
+RegistrationConfigOutputTypeDef = TypedDict(
+    "RegistrationConfigOutputTypeDef",
     {
         "templateBody": str,
         "roleArn": str,
         "templateName": str,
     },
     total=False,
 )
@@ -2679,14 +3319,22 @@
         "serverCertificateArn": str,
         "serverCertificateStatus": ServerCertificateStatusType,
         "serverCertificateStatusDetail": str,
     },
     total=False,
 )
 
+TlsConfigOutputTypeDef = TypedDict(
+    "TlsConfigOutputTypeDef",
+    {
+        "securityPolicy": str,
+    },
+    total=False,
+)
+
 DescribeEndpointRequestRequestTypeDef = TypedDict(
     "DescribeEndpointRequestRequestTypeDef",
     {
         "endpointType": str,
     },
     total=False,
 )
@@ -2754,14 +3402,39 @@
 DescribeJobTemplateRequestRequestTypeDef = TypedDict(
     "DescribeJobTemplateRequestRequestTypeDef",
     {
         "jobTemplateId": str,
     },
 )
 
+MaintenanceWindowOutputTypeDef = TypedDict(
+    "MaintenanceWindowOutputTypeDef",
+    {
+        "startTime": str,
+        "durationInMinutes": int,
+    },
+)
+
+PresignedUrlConfigOutputTypeDef = TypedDict(
+    "PresignedUrlConfigOutputTypeDef",
+    {
+        "roleArn": str,
+        "expiresInSec": int,
+    },
+    total=False,
+)
+
+TimeoutConfigOutputTypeDef = TypedDict(
+    "TimeoutConfigOutputTypeDef",
+    {
+        "inProgressTimeoutInMinutes": int,
+    },
+    total=False,
+)
+
 _RequiredDescribeManagedJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeManagedJobTemplateRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 _OptionalDescribeManagedJobTemplateRequestRequestTypeDef = TypedDict(
@@ -2800,14 +3473,33 @@
 DescribeProvisioningTemplateRequestRequestTypeDef = TypedDict(
     "DescribeProvisioningTemplateRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 
+_RequiredProvisioningHookOutputTypeDef = TypedDict(
+    "_RequiredProvisioningHookOutputTypeDef",
+    {
+        "targetArn": str,
+    },
+)
+_OptionalProvisioningHookOutputTypeDef = TypedDict(
+    "_OptionalProvisioningHookOutputTypeDef",
+    {
+        "payloadVersion": str,
+    },
+    total=False,
+)
+
+class ProvisioningHookOutputTypeDef(
+    _RequiredProvisioningHookOutputTypeDef, _OptionalProvisioningHookOutputTypeDef
+):
+    pass
+
 DescribeProvisioningTemplateVersionRequestRequestTypeDef = TypedDict(
     "DescribeProvisioningTemplateVersionRequestRequestTypeDef",
     {
         "templateName": str,
         "versionId": int,
     },
 )
@@ -2946,14 +3638,32 @@
         "deprecated": bool,
         "deprecationDate": datetime,
         "creationDate": datetime,
     },
     total=False,
 )
 
+ThingTypePropertiesOutputTypeDef = TypedDict(
+    "ThingTypePropertiesOutputTypeDef",
+    {
+        "thingTypeDescription": str,
+        "searchableAttributes": List[str],
+    },
+    total=False,
+)
+
+S3DestinationOutputTypeDef = TypedDict(
+    "S3DestinationOutputTypeDef",
+    {
+        "bucket": str,
+        "prefix": str,
+    },
+    total=False,
+)
+
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
@@ -3013,32 +3723,42 @@
         "actionsExecuted": int,
         "actionsSkipped": int,
         "actionsFailed": int,
     },
     total=False,
 )
 
-DetectMitigationActionsTaskTargetTypeDef = TypedDict(
-    "DetectMitigationActionsTaskTargetTypeDef",
+DetectMitigationActionsTaskTargetOutputTypeDef = TypedDict(
+    "DetectMitigationActionsTaskTargetOutputTypeDef",
     {
         "violationIds": List[str],
         "securityProfileName": str,
         "behaviorName": str,
     },
     total=False,
 )
 
-ViolationEventOccurrenceRangeTypeDef = TypedDict(
-    "ViolationEventOccurrenceRangeTypeDef",
+ViolationEventOccurrenceRangeOutputTypeDef = TypedDict(
+    "ViolationEventOccurrenceRangeOutputTypeDef",
     {
         "startTime": datetime,
         "endTime": datetime,
     },
 )
 
+DetectMitigationActionsTaskTargetTypeDef = TypedDict(
+    "DetectMitigationActionsTaskTargetTypeDef",
+    {
+        "violationIds": Sequence[str],
+        "securityProfileName": str,
+        "behaviorName": str,
+    },
+    total=False,
+)
+
 DisableTopicRuleRequestRequestTypeDef = TypedDict(
     "DisableTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
     },
 )
 
@@ -3048,14 +3768,21 @@
         "domainConfigurationName": str,
         "domainConfigurationArn": str,
         "serviceType": ServiceTypeType,
     },
     total=False,
 )
 
+PutItemInputOutputTypeDef = TypedDict(
+    "PutItemInputOutputTypeDef",
+    {
+        "tableName": str,
+    },
+)
+
 PutItemInputTypeDef = TypedDict(
     "PutItemInputTypeDef",
     {
         "tableName": str,
     },
 )
 
@@ -3072,14 +3799,22 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EnableIoTLoggingParamsOutputTypeDef = TypedDict(
+    "EnableIoTLoggingParamsOutputTypeDef",
+    {
+        "roleArnForLogging": str,
+        "logLevel": LogLevelType,
+    },
+)
+
 EnableIoTLoggingParamsTypeDef = TypedDict(
     "EnableIoTLoggingParamsTypeDef",
     {
         "roleArnForLogging": str,
         "logLevel": LogLevelType,
     },
 )
@@ -3096,32 +3831,69 @@
     {
         "code": str,
         "message": str,
     },
     total=False,
 )
 
+RateIncreaseCriteriaOutputTypeDef = TypedDict(
+    "RateIncreaseCriteriaOutputTypeDef",
+    {
+        "numberOfNotifiedThings": int,
+        "numberOfSucceededThings": int,
+    },
+    total=False,
+)
+
 RateIncreaseCriteriaTypeDef = TypedDict(
     "RateIncreaseCriteriaTypeDef",
     {
         "numberOfNotifiedThings": int,
         "numberOfSucceededThings": int,
     },
     total=False,
 )
 
+FieldOutputTypeDef = TypedDict(
+    "FieldOutputTypeDef",
+    {
+        "name": str,
+        "type": FieldTypeType,
+    },
+    total=False,
+)
+
 FieldTypeDef = TypedDict(
     "FieldTypeDef",
     {
         "name": str,
         "type": FieldTypeType,
     },
     total=False,
 )
 
+S3LocationOutputTypeDef = TypedDict(
+    "S3LocationOutputTypeDef",
+    {
+        "bucket": str,
+        "key": str,
+        "version": str,
+    },
+    total=False,
+)
+
+StreamOutputTypeDef = TypedDict(
+    "StreamOutputTypeDef",
+    {
+        "streamId": str,
+        "fileId": int,
+    },
+    total=False,
+)
+
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
         "version": str,
     },
@@ -3233,16 +4005,16 @@
 GetOTAUpdateRequestRequestTypeDef = TypedDict(
     "GetOTAUpdateRequestRequestTypeDef",
     {
         "otaUpdateId": str,
     },
 )
 
-VersionUpdateByJobsConfigTypeDef = TypedDict(
-    "VersionUpdateByJobsConfigTypeDef",
+VersionUpdateByJobsConfigOutputTypeDef = TypedDict(
+    "VersionUpdateByJobsConfigOutputTypeDef",
     {
         "enabled": bool,
         "roleArn": str,
     },
     total=False,
 )
 
@@ -3438,22 +4210,39 @@
     {
         "groupName": str,
         "groupArn": str,
     },
     total=False,
 )
 
+HttpActionHeaderOutputTypeDef = TypedDict(
+    "HttpActionHeaderOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 HttpActionHeaderTypeDef = TypedDict(
     "HttpActionHeaderTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
+SigV4AuthorizationOutputTypeDef = TypedDict(
+    "SigV4AuthorizationOutputTypeDef",
+    {
+        "signingRegion": str,
+        "serviceName": str,
+        "roleArn": str,
+    },
+)
+
 SigV4AuthorizationTypeDef = TypedDict(
     "SigV4AuthorizationTypeDef",
     {
         "signingRegion": str,
         "serviceName": str,
         "roleArn": str,
     },
@@ -3487,18 +4276,36 @@
     "HttpUrlDestinationSummaryTypeDef",
     {
         "confirmationUrl": str,
     },
     total=False,
 )
 
+IndexingFilterOutputTypeDef = TypedDict(
+    "IndexingFilterOutputTypeDef",
+    {
+        "namedShadowNames": List[str],
+    },
+    total=False,
+)
+
 IndexingFilterTypeDef = TypedDict(
     "IndexingFilterTypeDef",
     {
-        "namedShadowNames": List[str],
+        "namedShadowNames": Sequence[str],
+    },
+    total=False,
+)
+
+IssuerCertificateIdentifierOutputTypeDef = TypedDict(
+    "IssuerCertificateIdentifierOutputTypeDef",
+    {
+        "issuerCertificateSubject": str,
+        "issuerId": str,
+        "issuerCertificateSerialNumber": str,
     },
     total=False,
 )
 
 IssuerCertificateIdentifierTypeDef = TypedDict(
     "IssuerCertificateIdentifierTypeDef",
     {
@@ -3526,14 +4333,22 @@
         "lastUpdatedAt": datetime,
         "executionNumber": int,
         "retryAttempt": int,
     },
     total=False,
 )
 
+RetryCriteriaOutputTypeDef = TypedDict(
+    "RetryCriteriaOutputTypeDef",
+    {
+        "failureType": RetryableFailureTypeType,
+        "numberOfRetries": int,
+    },
+)
+
 RetryCriteriaTypeDef = TypedDict(
     "RetryCriteriaTypeDef",
     {
         "failureType": RetryableFailureTypeType,
         "numberOfRetries": int,
     },
 )
@@ -4997,14 +5812,31 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
 _RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
     "_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
     {
         "policyName": str,
     },
 )
 _OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
@@ -5574,14 +6406,33 @@
 
 class ListViolationEventsRequestRequestTypeDef(
     _RequiredListViolationEventsRequestRequestTypeDef,
     _OptionalListViolationEventsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredLocationTimestampOutputTypeDef = TypedDict(
+    "_RequiredLocationTimestampOutputTypeDef",
+    {
+        "value": str,
+    },
+)
+_OptionalLocationTimestampOutputTypeDef = TypedDict(
+    "_OptionalLocationTimestampOutputTypeDef",
+    {
+        "unit": str,
+    },
+    total=False,
+)
+
+class LocationTimestampOutputTypeDef(
+    _RequiredLocationTimestampOutputTypeDef, _OptionalLocationTimestampOutputTypeDef
+):
+    pass
+
 _RequiredLocationTimestampTypeDef = TypedDict(
     "_RequiredLocationTimestampTypeDef",
     {
         "value": str,
     },
 )
 _OptionalLocationTimestampTypeDef = TypedDict(
@@ -5593,14 +6444,31 @@
 )
 
 class LocationTimestampTypeDef(
     _RequiredLocationTimestampTypeDef, _OptionalLocationTimestampTypeDef
 ):
     pass
 
+_RequiredLogTargetOutputTypeDef = TypedDict(
+    "_RequiredLogTargetOutputTypeDef",
+    {
+        "targetType": LogTargetTypeType,
+    },
+)
+_OptionalLogTargetOutputTypeDef = TypedDict(
+    "_OptionalLogTargetOutputTypeDef",
+    {
+        "targetName": str,
+    },
+    total=False,
+)
+
+class LogTargetOutputTypeDef(_RequiredLogTargetOutputTypeDef, _OptionalLogTargetOutputTypeDef):
+    pass
+
 _RequiredLogTargetTypeDef = TypedDict(
     "_RequiredLogTargetTypeDef",
     {
         "targetType": LogTargetTypeType,
     },
 )
 _OptionalLogTargetTypeDef = TypedDict(
@@ -5629,14 +6497,42 @@
 )
 
 class LoggingOptionsPayloadTypeDef(
     _RequiredLoggingOptionsPayloadTypeDef, _OptionalLoggingOptionsPayloadTypeDef
 ):
     pass
 
+PublishFindingToSnsParamsOutputTypeDef = TypedDict(
+    "PublishFindingToSnsParamsOutputTypeDef",
+    {
+        "topicArn": str,
+    },
+)
+
+ReplaceDefaultPolicyVersionParamsOutputTypeDef = TypedDict(
+    "ReplaceDefaultPolicyVersionParamsOutputTypeDef",
+    {
+        "templateName": Literal["BLANK_POLICY"],
+    },
+)
+
+UpdateCACertificateParamsOutputTypeDef = TypedDict(
+    "UpdateCACertificateParamsOutputTypeDef",
+    {
+        "action": Literal["DEACTIVATE"],
+    },
+)
+
+UpdateDeviceCertificateParamsOutputTypeDef = TypedDict(
+    "UpdateDeviceCertificateParamsOutputTypeDef",
+    {
+        "action": Literal["DEACTIVATE"],
+    },
+)
+
 PublishFindingToSnsParamsTypeDef = TypedDict(
     "PublishFindingToSnsParamsTypeDef",
     {
         "topicArn": str,
     },
 )
 
@@ -5667,14 +6563,22 @@
         "username": str,
         "password": Union[str, bytes, IO[Any], StreamingBody],
         "clientId": str,
     },
     total=False,
 )
 
+UserPropertyOutputTypeDef = TypedDict(
+    "UserPropertyOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 UserPropertyTypeDef = TypedDict(
     "UserPropertyTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -5685,14 +6589,23 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PolicyVersionIdentifierOutputTypeDef = TypedDict(
+    "PolicyVersionIdentifierOutputTypeDef",
+    {
+        "policyName": str,
+        "policyVersionId": str,
+    },
+    total=False,
+)
+
 PolicyVersionIdentifierTypeDef = TypedDict(
     "PolicyVersionIdentifierTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
     total=False,
@@ -5715,14 +6628,24 @@
 
 class PutVerificationStateOnViolationRequestRequestTypeDef(
     _RequiredPutVerificationStateOnViolationRequestRequestTypeDef,
     _OptionalPutVerificationStateOnViolationRequestRequestTypeDef,
 ):
     pass
 
+RegistrationConfigTypeDef = TypedDict(
+    "RegistrationConfigTypeDef",
+    {
+        "templateBody": str,
+        "roleArn": str,
+        "templateName": str,
+    },
+    total=False,
+)
+
 RegisterCACertificateResponseTypeDef = TypedDict(
     "RegisterCACertificateResponseTypeDef",
     {
         "certificateArn": str,
         "certificateId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -5933,14 +6856,24 @@
         "roleArn": str,
         "defaultLogLevel": LogLevelType,
         "disableAllLogs": bool,
     },
     total=False,
 )
 
+SigningProfileParameterOutputTypeDef = TypedDict(
+    "SigningProfileParameterOutputTypeDef",
+    {
+        "certificateArn": str,
+        "platform": str,
+        "certificatePathOnDevice": str,
+    },
+    total=False,
+)
+
 SigningProfileParameterTypeDef = TypedDict(
     "SigningProfileParameterTypeDef",
     {
         "certificateArn": str,
         "platform": str,
         "certificatePathOnDevice": str,
     },
@@ -5951,14 +6884,22 @@
     "StartAuditMitigationActionsTaskResponseTypeDef",
     {
         "taskId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ViolationEventOccurrenceRangeTypeDef = TypedDict(
+    "ViolationEventOccurrenceRangeTypeDef",
+    {
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+
 StartDetectMitigationActionsTaskResponseTypeDef = TypedDict(
     "StartDetectMitigationActionsTaskResponseTypeDef",
     {
         "taskId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -6029,14 +6970,30 @@
         "connected": bool,
         "timestamp": int,
         "disconnectReason": str,
     },
     total=False,
 )
 
+TimestreamDimensionOutputTypeDef = TypedDict(
+    "TimestreamDimensionOutputTypeDef",
+    {
+        "name": str,
+        "value": str,
+    },
+)
+
+TimestreamTimestampOutputTypeDef = TypedDict(
+    "TimestreamTimestampOutputTypeDef",
+    {
+        "value": str,
+        "unit": str,
+    },
+)
+
 TimestreamDimensionTypeDef = TypedDict(
     "TimestreamDimensionTypeDef",
     {
         "name": str,
         "value": str,
     },
 )
@@ -6241,14 +7198,23 @@
     {
         "actionArn": str,
         "actionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+VersionUpdateByJobsConfigTypeDef = TypedDict(
+    "VersionUpdateByJobsConfigTypeDef",
+    {
+        "enabled": bool,
+        "roleArn": str,
+    },
+    total=False,
+)
+
 _RequiredUpdatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePackageRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 _OptionalUpdatePackageRequestRequestTypeDef = TypedDict(
@@ -6393,36 +7359,43 @@
     "ValidationErrorTypeDef",
     {
         "errorMessage": str,
     },
     total=False,
 )
 
+AbortConfigOutputTypeDef = TypedDict(
+    "AbortConfigOutputTypeDef",
+    {
+        "criteriaList": List[AbortCriteriaOutputTypeDef],
+    },
+)
+
 AbortConfigTypeDef = TypedDict(
     "AbortConfigTypeDef",
     {
         "criteriaList": Sequence[AbortCriteriaTypeDef],
     },
 )
 
 MetricDatumTypeDef = TypedDict(
     "MetricDatumTypeDef",
     {
         "timestamp": datetime,
-        "value": MetricValueTypeDef,
+        "value": MetricValueOutputTypeDef,
     },
     total=False,
 )
 
 DescribeFleetMetricResponseTypeDef = TypedDict(
     "DescribeFleetMetricResponseTypeDef",
     {
         "metricName": str,
         "queryString": str,
-        "aggregationType": AggregationTypeTypeDef,
+        "aggregationType": AggregationTypeOutputTypeDef,
         "period": int,
         "aggregationField": str,
         "description": str,
         "queryVersion": str,
         "indexName": str,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
@@ -6507,14 +7480,34 @@
     {
         "policies": List[PolicyTypeDef],
         "nextMarker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredAssetPropertyValueOutputTypeDef = TypedDict(
+    "_RequiredAssetPropertyValueOutputTypeDef",
+    {
+        "value": AssetPropertyVariantOutputTypeDef,
+        "timestamp": AssetPropertyTimestampOutputTypeDef,
+    },
+)
+_OptionalAssetPropertyValueOutputTypeDef = TypedDict(
+    "_OptionalAssetPropertyValueOutputTypeDef",
+    {
+        "quality": str,
+    },
+    total=False,
+)
+
+class AssetPropertyValueOutputTypeDef(
+    _RequiredAssetPropertyValueOutputTypeDef, _OptionalAssetPropertyValueOutputTypeDef
+):
+    pass
+
 _RequiredAssetPropertyValueTypeDef = TypedDict(
     "_RequiredAssetPropertyValueTypeDef",
     {
         "value": AssetPropertyVariantTypeDef,
         "timestamp": AssetPropertyTimestampTypeDef,
     },
 )
@@ -6527,14 +7520,23 @@
 )
 
 class AssetPropertyValueTypeDef(
     _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
 ):
     pass
 
+ThingGroupPropertiesOutputTypeDef = TypedDict(
+    "ThingGroupPropertiesOutputTypeDef",
+    {
+        "thingGroupDescription": str,
+        "attributePayload": AttributePayloadOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateThingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalCreateThingRequestRequestTypeDef = TypedDict(
@@ -6612,17 +7614,17 @@
 )
 
 DescribeAccountAuditConfigurationResponseTypeDef = TypedDict(
     "DescribeAccountAuditConfigurationResponseTypeDef",
     {
         "roleArn": str,
         "auditNotificationTargetConfigurations": Dict[
-            Literal["SNS"], AuditNotificationTargetTypeDef
+            Literal["SNS"], AuditNotificationTargetOutputTypeDef
         ],
-        "auditCheckConfigurations": Dict[str, AuditCheckConfigurationTypeDef],
+        "auditCheckConfigurations": Dict[str, AuditCheckConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAccountAuditConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     {
@@ -6695,23 +7697,46 @@
 AwsJobAbortConfigTypeDef = TypedDict(
     "AwsJobAbortConfigTypeDef",
     {
         "abortCriteriaList": Sequence[AwsJobAbortCriteriaTypeDef],
     },
 )
 
+AwsJobExponentialRolloutRateOutputTypeDef = TypedDict(
+    "AwsJobExponentialRolloutRateOutputTypeDef",
+    {
+        "baseRatePerMinute": int,
+        "incrementFactor": float,
+        "rateIncreaseCriteria": AwsJobRateIncreaseCriteriaOutputTypeDef,
+    },
+)
+
 AwsJobExponentialRolloutRateTypeDef = TypedDict(
     "AwsJobExponentialRolloutRateTypeDef",
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": AwsJobRateIncreaseCriteriaTypeDef,
     },
 )
 
+BehaviorCriteriaOutputTypeDef = TypedDict(
+    "BehaviorCriteriaOutputTypeDef",
+    {
+        "comparisonOperator": ComparisonOperatorType,
+        "value": MetricValueOutputTypeDef,
+        "durationSeconds": int,
+        "consecutiveDatapointsToAlarm": int,
+        "consecutiveDatapointsToClear": int,
+        "statisticalThreshold": StatisticalThresholdOutputTypeDef,
+        "mlDetectionConfig": MachineLearningDetectionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 BehaviorCriteriaTypeDef = TypedDict(
     "BehaviorCriteriaTypeDef",
     {
         "comparisonOperator": ComparisonOperatorType,
         "value": MetricValueTypeDef,
         "durationSeconds": int,
         "consecutiveDatapointsToAlarm": int,
@@ -6727,14 +7752,33 @@
     {
         "summaries": List[BehaviorModelTrainingSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredMetricToRetainOutputTypeDef = TypedDict(
+    "_RequiredMetricToRetainOutputTypeDef",
+    {
+        "metric": str,
+    },
+)
+_OptionalMetricToRetainOutputTypeDef = TypedDict(
+    "_OptionalMetricToRetainOutputTypeDef",
+    {
+        "metricDimension": MetricDimensionOutputTypeDef,
+    },
+    total=False,
+)
+
+class MetricToRetainOutputTypeDef(
+    _RequiredMetricToRetainOutputTypeDef, _OptionalMetricToRetainOutputTypeDef
+):
+    pass
+
 _RequiredMetricToRetainTypeDef = TypedDict(
     "_RequiredMetricToRetainTypeDef",
     {
         "metric": str,
     },
 )
 _OptionalMetricToRetainTypeDef = TypedDict(
@@ -6751,15 +7795,15 @@
 DescribeBillingGroupResponseTypeDef = TypedDict(
     "DescribeBillingGroupResponseTypeDef",
     {
         "billingGroupName": str,
         "billingGroupId": str,
         "billingGroupArn": str,
         "version": int,
-        "billingGroupProperties": BillingGroupPropertiesTypeDef,
+        "billingGroupProperties": BillingGroupPropertiesOutputTypeDef,
         "billingGroupMetadata": BillingGroupMetadataTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateBillingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBillingGroupRequestRequestTypeDef",
@@ -6862,29 +7906,40 @@
     {
         "certificates": List[CertificateTypeDef],
         "nextMarker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CustomCodeSigningOutputTypeDef = TypedDict(
+    "CustomCodeSigningOutputTypeDef",
+    {
+        "signature": CodeSigningSignatureOutputTypeDef,
+        "certificateChain": CodeSigningCertificateChainOutputTypeDef,
+        "hashAlgorithm": str,
+        "signatureAlgorithm": str,
+    },
+    total=False,
+)
+
 CustomCodeSigningTypeDef = TypedDict(
     "CustomCodeSigningTypeDef",
     {
         "signature": CodeSigningSignatureTypeDef,
         "certificateChain": CodeSigningCertificateChainTypeDef,
         "hashAlgorithm": str,
         "signatureAlgorithm": str,
     },
     total=False,
 )
 
 DescribeEventConfigurationsResponseTypeDef = TypedDict(
     "DescribeEventConfigurationsResponseTypeDef",
     {
-        "eventConfigurations": Dict[EventTypeType, ConfigurationTypeDef],
+        "eventConfigurations": Dict[EventTypeType, ConfigurationOutputTypeDef],
         "creationDate": datetime,
         "lastModifiedDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEventConfigurationsRequestRequestTypeDef = TypedDict(
@@ -7074,23 +8129,14 @@
 
 class CreateScheduledAuditRequestRequestTypeDef(
     _RequiredCreateScheduledAuditRequestRequestTypeDef,
     _OptionalCreateScheduledAuditRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -7199,32 +8245,14 @@
 
 class CreateProvisioningTemplateRequestRequestTypeDef(
     _RequiredCreateProvisioningTemplateRequestRequestTypeDef,
     _OptionalCreateProvisioningTemplateRequestRequestTypeDef,
 ):
     pass
 
-DescribeProvisioningTemplateResponseTypeDef = TypedDict(
-    "DescribeProvisioningTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateName": str,
-        "description": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "defaultVersionId": int,
-        "templateBody": str,
-        "enabled": bool,
-        "provisioningRoleArn": str,
-        "preProvisioningHook": ProvisioningHookTypeDef,
-        "type": TemplateTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateProvisioningTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProvisioningTemplateRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 _OptionalUpdateProvisioningTemplateRequestRequestTypeDef = TypedDict(
@@ -7275,124 +8303,113 @@
         "taskStatistics": TaskStatisticsTypeDef,
         "scheduledAuditName": str,
         "auditDetails": Dict[str, AuditCheckDetailsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredRegisterCACertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterCACertificateRequestRequestTypeDef",
-    {
-        "caCertificate": str,
-    },
-)
-_OptionalRegisterCACertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterCACertificateRequestRequestTypeDef",
-    {
-        "verificationCertificate": str,
-        "setAsActive": bool,
-        "allowAutoRegistration": bool,
-        "registrationConfig": RegistrationConfigTypeDef,
-        "tags": Sequence[TagTypeDef],
-        "certificateMode": CertificateModeType,
-    },
-    total=False,
-)
-
-class RegisterCACertificateRequestRequestTypeDef(
-    _RequiredRegisterCACertificateRequestRequestTypeDef,
-    _OptionalRegisterCACertificateRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateCACertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCACertificateRequestRequestTypeDef",
-    {
-        "certificateId": str,
-    },
-)
-_OptionalUpdateCACertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCACertificateRequestRequestTypeDef",
-    {
-        "newStatus": CACertificateStatusType,
-        "newAutoRegistrationStatus": AutoRegistrationStatusType,
-        "registrationConfig": RegistrationConfigTypeDef,
-        "removeAutoRegistration": bool,
-    },
-    total=False,
-)
-
-class UpdateCACertificateRequestRequestTypeDef(
-    _RequiredUpdateCACertificateRequestRequestTypeDef,
-    _OptionalUpdateCACertificateRequestRequestTypeDef,
-):
-    pass
-
 DescribeDomainConfigurationResponseTypeDef = TypedDict(
     "DescribeDomainConfigurationResponseTypeDef",
     {
         "domainConfigurationName": str,
         "domainConfigurationArn": str,
         "domainName": str,
         "serverCertificates": List[ServerCertificateSummaryTypeDef],
-        "authorizerConfig": AuthorizerConfigTypeDef,
+        "authorizerConfig": AuthorizerConfigOutputTypeDef,
         "domainConfigurationStatus": DomainConfigurationStatusType,
         "serviceType": ServiceTypeType,
         "domainType": DomainTypeType,
         "lastStatusChangeDate": datetime,
-        "tlsConfig": TlsConfigTypeDef,
+        "tlsConfig": TlsConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SchedulingConfigOutputTypeDef = TypedDict(
+    "SchedulingConfigOutputTypeDef",
+    {
+        "startTime": str,
+        "endTime": str,
+        "endBehavior": JobEndBehaviorType,
+        "maintenanceWindows": List[MaintenanceWindowOutputTypeDef],
+    },
+    total=False,
+)
+
 DescribeManagedJobTemplateResponseTypeDef = TypedDict(
     "DescribeManagedJobTemplateResponseTypeDef",
     {
         "templateName": str,
         "templateArn": str,
         "description": str,
         "templateVersion": str,
         "environments": List[str],
         "documentParameters": List[DocumentParameterTypeDef],
         "document": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DescribeProvisioningTemplateResponseTypeDef = TypedDict(
+    "DescribeProvisioningTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateName": str,
+        "description": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "defaultVersionId": int,
+        "templateBody": str,
+        "enabled": bool,
+        "provisioningRoleArn": str,
+        "preProvisioningHook": ProvisioningHookOutputTypeDef,
+        "type": TemplateTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeRoleAliasResponseTypeDef = TypedDict(
     "DescribeRoleAliasResponseTypeDef",
     {
         "roleAliasDescription": RoleAliasDescriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeThingTypeResponseTypeDef = TypedDict(
     "DescribeThingTypeResponseTypeDef",
     {
         "thingTypeName": str,
         "thingTypeId": str,
         "thingTypeArn": str,
-        "thingTypeProperties": ThingTypePropertiesTypeDef,
+        "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ThingTypeDefinitionTypeDef = TypedDict(
     "ThingTypeDefinitionTypeDef",
     {
         "thingTypeName": str,
         "thingTypeArn": str,
-        "thingTypeProperties": ThingTypePropertiesTypeDef,
+        "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
     },
     total=False,
 )
 
+DestinationOutputTypeDef = TypedDict(
+    "DestinationOutputTypeDef",
+    {
+        "s3Destination": S3DestinationOutputTypeDef,
+    },
+    total=False,
+)
+
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3Destination": S3DestinationTypeDef,
     },
     total=False,
 )
@@ -7402,48 +8419,31 @@
     {
         "actionsExecutions": List[DetectMitigationActionExecutionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "taskId": str,
-        "target": DetectMitigationActionsTaskTargetTypeDef,
-        "actions": Sequence[str],
-        "clientRequestToken": str,
-    },
-)
-_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
-    {
-        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
-        "includeOnlyActiveViolations": bool,
-        "includeSuppressedAlerts": bool,
-    },
-    total=False,
-)
-
-class StartDetectMitigationActionsTaskRequestRequestTypeDef(
-    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
-    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
-):
-    pass
-
 ListDomainConfigurationsResponseTypeDef = TypedDict(
     "ListDomainConfigurationsResponseTypeDef",
     {
         "domainConfigurations": List[DomainConfigurationSummaryTypeDef],
         "nextMarker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DynamoDBv2ActionOutputTypeDef = TypedDict(
+    "DynamoDBv2ActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "putItem": PutItemInputOutputTypeDef,
+    },
+)
+
 DynamoDBv2ActionTypeDef = TypedDict(
     "DynamoDBv2ActionTypeDef",
     {
         "roleArn": str,
         "putItem": PutItemInputTypeDef,
     },
 )
@@ -7452,43 +8452,91 @@
     "GetEffectivePoliciesResponseTypeDef",
     {
         "effectivePolicies": List[EffectivePolicyTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ExponentialRolloutRateOutputTypeDef = TypedDict(
+    "ExponentialRolloutRateOutputTypeDef",
+    {
+        "baseRatePerMinute": int,
+        "incrementFactor": float,
+        "rateIncreaseCriteria": RateIncreaseCriteriaOutputTypeDef,
+    },
+)
+
 ExponentialRolloutRateTypeDef = TypedDict(
     "ExponentialRolloutRateTypeDef",
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": RateIncreaseCriteriaTypeDef,
     },
 )
 
+_RequiredThingGroupIndexingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredThingGroupIndexingConfigurationOutputTypeDef",
+    {
+        "thingGroupIndexingMode": ThingGroupIndexingModeType,
+    },
+)
+_OptionalThingGroupIndexingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalThingGroupIndexingConfigurationOutputTypeDef",
+    {
+        "managedFields": List[FieldOutputTypeDef],
+        "customFields": List[FieldOutputTypeDef],
+    },
+    total=False,
+)
+
+class ThingGroupIndexingConfigurationOutputTypeDef(
+    _RequiredThingGroupIndexingConfigurationOutputTypeDef,
+    _OptionalThingGroupIndexingConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredThingGroupIndexingConfigurationTypeDef = TypedDict(
     "_RequiredThingGroupIndexingConfigurationTypeDef",
     {
         "thingGroupIndexingMode": ThingGroupIndexingModeType,
     },
 )
 _OptionalThingGroupIndexingConfigurationTypeDef = TypedDict(
     "_OptionalThingGroupIndexingConfigurationTypeDef",
     {
-        "managedFields": List[FieldTypeDef],
-        "customFields": List[FieldTypeDef],
+        "managedFields": Sequence[FieldTypeDef],
+        "customFields": Sequence[FieldTypeDef],
     },
     total=False,
 )
 
 class ThingGroupIndexingConfigurationTypeDef(
     _RequiredThingGroupIndexingConfigurationTypeDef, _OptionalThingGroupIndexingConfigurationTypeDef
 ):
     pass
 
+StreamFileOutputTypeDef = TypedDict(
+    "StreamFileOutputTypeDef",
+    {
+        "fileId": int,
+        "s3Location": S3LocationOutputTypeDef,
+    },
+    total=False,
+)
+
+FileLocationOutputTypeDef = TypedDict(
+    "FileLocationOutputTypeDef",
+    {
+        "stream": StreamOutputTypeDef,
+        "s3Location": S3LocationOutputTypeDef,
+    },
+    total=False,
+)
+
 StreamFileTypeDef = TypedDict(
     "StreamFileTypeDef",
     {
         "fileId": int,
         "s3Location": S3LocationTypeDef,
     },
     total=False,
@@ -7511,28 +8559,19 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPackageConfigurationResponseTypeDef = TypedDict(
     "GetPackageConfigurationResponseTypeDef",
     {
-        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
+        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdatePackageConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdatePackageConfigurationRequestRequestTypeDef",
-    {
-        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
-        "clientToken": str,
-    },
-    total=False,
-)
-
 GetPercentilesResponseTypeDef = TypedDict(
     "GetPercentilesResponseTypeDef",
     {
         "percentiles": List[PercentPairTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -7578,36 +8617,69 @@
         "parentGroupName": str,
         "rootToParentThingGroups": List[GroupNameAndArnTypeDef],
         "creationDate": datetime,
     },
     total=False,
 )
 
+HttpAuthorizationOutputTypeDef = TypedDict(
+    "HttpAuthorizationOutputTypeDef",
+    {
+        "sigv4": SigV4AuthorizationOutputTypeDef,
+    },
+    total=False,
+)
+
 HttpAuthorizationTypeDef = TypedDict(
     "HttpAuthorizationTypeDef",
     {
         "sigv4": SigV4AuthorizationTypeDef,
     },
     total=False,
 )
 
+_RequiredThingIndexingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredThingIndexingConfigurationOutputTypeDef",
+    {
+        "thingIndexingMode": ThingIndexingModeType,
+    },
+)
+_OptionalThingIndexingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalThingIndexingConfigurationOutputTypeDef",
+    {
+        "thingConnectivityIndexingMode": ThingConnectivityIndexingModeType,
+        "deviceDefenderIndexingMode": DeviceDefenderIndexingModeType,
+        "namedShadowIndexingMode": NamedShadowIndexingModeType,
+        "managedFields": List[FieldOutputTypeDef],
+        "customFields": List[FieldOutputTypeDef],
+        "filter": IndexingFilterOutputTypeDef,
+    },
+    total=False,
+)
+
+class ThingIndexingConfigurationOutputTypeDef(
+    _RequiredThingIndexingConfigurationOutputTypeDef,
+    _OptionalThingIndexingConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredThingIndexingConfigurationTypeDef = TypedDict(
     "_RequiredThingIndexingConfigurationTypeDef",
     {
         "thingIndexingMode": ThingIndexingModeType,
     },
 )
 _OptionalThingIndexingConfigurationTypeDef = TypedDict(
     "_OptionalThingIndexingConfigurationTypeDef",
     {
         "thingConnectivityIndexingMode": ThingConnectivityIndexingModeType,
         "deviceDefenderIndexingMode": DeviceDefenderIndexingModeType,
         "namedShadowIndexingMode": NamedShadowIndexingModeType,
-        "managedFields": List[FieldTypeDef],
-        "customFields": List[FieldTypeDef],
+        "managedFields": Sequence[FieldTypeDef],
+        "customFields": Sequence[FieldTypeDef],
         "filter": IndexingFilterTypeDef,
     },
     total=False,
 )
 
 class ThingIndexingConfigurationTypeDef(
     _RequiredThingIndexingConfigurationTypeDef, _OptionalThingIndexingConfigurationTypeDef
@@ -7646,14 +8718,21 @@
     {
         "jobId": str,
         "jobExecutionSummary": JobExecutionSummaryTypeDef,
     },
     total=False,
 )
 
+JobExecutionsRetryConfigOutputTypeDef = TypedDict(
+    "JobExecutionsRetryConfigOutputTypeDef",
+    {
+        "criteriaList": List[RetryCriteriaOutputTypeDef],
+    },
+)
+
 JobExecutionsRetryConfigTypeDef = TypedDict(
     "JobExecutionsRetryConfigTypeDef",
     {
         "criteriaList": Sequence[RetryCriteriaTypeDef],
     },
 )
 
@@ -7778,14 +8857,23 @@
     {
         "streams": List[StreamSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTargetsForSecurityProfileResponseTypeDef = TypedDict(
     "ListTargetsForSecurityProfileResponseTypeDef",
     {
         "securityProfileTargets": List[SecurityProfileTargetTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -7814,14 +8902,37 @@
     {
         "rules": List[TopicRuleListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredLocationActionOutputTypeDef = TypedDict(
+    "_RequiredLocationActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "trackerName": str,
+        "deviceId": str,
+        "latitude": str,
+        "longitude": str,
+    },
+)
+_OptionalLocationActionOutputTypeDef = TypedDict(
+    "_OptionalLocationActionOutputTypeDef",
+    {
+        "timestamp": LocationTimestampOutputTypeDef,
+    },
+    total=False,
+)
+
+class LocationActionOutputTypeDef(
+    _RequiredLocationActionOutputTypeDef, _OptionalLocationActionOutputTypeDef
+):
+    pass
+
 _RequiredLocationActionTypeDef = TypedDict(
     "_RequiredLocationActionTypeDef",
     {
         "roleArn": str,
         "trackerName": str,
         "deviceId": str,
         "latitude": str,
@@ -7838,15 +8949,15 @@
 
 class LocationActionTypeDef(_RequiredLocationActionTypeDef, _OptionalLocationActionTypeDef):
     pass
 
 LogTargetConfigurationTypeDef = TypedDict(
     "LogTargetConfigurationTypeDef",
     {
-        "logTarget": LogTargetTypeDef,
+        "logTarget": LogTargetOutputTypeDef,
         "logLevel": LogLevelType,
     },
     total=False,
 )
 
 SetV2LoggingLevelRequestRequestTypeDef = TypedDict(
     "SetV2LoggingLevelRequestRequestTypeDef",
@@ -7859,40 +8970,83 @@
 SetLoggingOptionsRequestRequestTypeDef = TypedDict(
     "SetLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptionsPayload": LoggingOptionsPayloadTypeDef,
     },
 )
 
+MitigationActionParamsOutputTypeDef = TypedDict(
+    "MitigationActionParamsOutputTypeDef",
+    {
+        "updateDeviceCertificateParams": UpdateDeviceCertificateParamsOutputTypeDef,
+        "updateCACertificateParams": UpdateCACertificateParamsOutputTypeDef,
+        "addThingsToThingGroupParams": AddThingsToThingGroupParamsOutputTypeDef,
+        "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsOutputTypeDef,
+        "enableIoTLoggingParams": EnableIoTLoggingParamsOutputTypeDef,
+        "publishFindingToSnsParams": PublishFindingToSnsParamsOutputTypeDef,
+    },
+    total=False,
+)
+
 MitigationActionParamsTypeDef = TypedDict(
     "MitigationActionParamsTypeDef",
     {
         "updateDeviceCertificateParams": UpdateDeviceCertificateParamsTypeDef,
         "updateCACertificateParams": UpdateCACertificateParamsTypeDef,
         "addThingsToThingGroupParams": AddThingsToThingGroupParamsTypeDef,
         "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsTypeDef,
         "enableIoTLoggingParams": EnableIoTLoggingParamsTypeDef,
         "publishFindingToSnsParams": PublishFindingToSnsParamsTypeDef,
     },
     total=False,
 )
 
+MqttHeadersOutputTypeDef = TypedDict(
+    "MqttHeadersOutputTypeDef",
+    {
+        "payloadFormatIndicator": str,
+        "contentType": str,
+        "responseTopic": str,
+        "correlationData": str,
+        "messageExpiry": str,
+        "userProperties": List[UserPropertyOutputTypeDef],
+    },
+    total=False,
+)
+
 MqttHeadersTypeDef = TypedDict(
     "MqttHeadersTypeDef",
     {
         "payloadFormatIndicator": str,
         "contentType": str,
         "responseTopic": str,
         "correlationData": str,
         "messageExpiry": str,
         "userProperties": Sequence[UserPropertyTypeDef],
     },
     total=False,
 )
 
+ResourceIdentifierOutputTypeDef = TypedDict(
+    "ResourceIdentifierOutputTypeDef",
+    {
+        "deviceCertificateId": str,
+        "caCertificateId": str,
+        "cognitoIdentityPoolId": str,
+        "clientId": str,
+        "policyVersionIdentifier": PolicyVersionIdentifierOutputTypeDef,
+        "account": str,
+        "iamRoleArn": str,
+        "roleAliasArn": str,
+        "issuerCertificateIdentifier": IssuerCertificateIdentifierOutputTypeDef,
+        "deviceCertificateArn": str,
+    },
+    total=False,
+)
+
 ResourceIdentifierTypeDef = TypedDict(
     "ResourceIdentifierTypeDef",
     {
         "deviceCertificateId": str,
         "caCertificateId": str,
         "cognitoIdentityPoolId": str,
         "clientId": str,
@@ -7902,14 +9056,87 @@
         "roleAliasArn": str,
         "issuerCertificateIdentifier": IssuerCertificateIdentifierTypeDef,
         "deviceCertificateArn": str,
     },
     total=False,
 )
 
+_RequiredRegisterCACertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterCACertificateRequestRequestTypeDef",
+    {
+        "caCertificate": str,
+    },
+)
+_OptionalRegisterCACertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterCACertificateRequestRequestTypeDef",
+    {
+        "verificationCertificate": str,
+        "setAsActive": bool,
+        "allowAutoRegistration": bool,
+        "registrationConfig": RegistrationConfigTypeDef,
+        "tags": Sequence[TagTypeDef],
+        "certificateMode": CertificateModeType,
+    },
+    total=False,
+)
+
+class RegisterCACertificateRequestRequestTypeDef(
+    _RequiredRegisterCACertificateRequestRequestTypeDef,
+    _OptionalRegisterCACertificateRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateCACertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCACertificateRequestRequestTypeDef",
+    {
+        "certificateId": str,
+    },
+)
+_OptionalUpdateCACertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCACertificateRequestRequestTypeDef",
+    {
+        "newStatus": CACertificateStatusType,
+        "newAutoRegistrationStatus": AutoRegistrationStatusType,
+        "registrationConfig": RegistrationConfigTypeDef,
+        "removeAutoRegistration": bool,
+    },
+    total=False,
+)
+
+class UpdateCACertificateRequestRequestTypeDef(
+    _RequiredUpdateCACertificateRequestRequestTypeDef,
+    _OptionalUpdateCACertificateRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "taskId": str,
+        "target": DetectMitigationActionsTaskTargetTypeDef,
+        "actions": Sequence[str],
+        "clientRequestToken": str,
+    },
+)
+_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef",
+    {
+        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
+        "includeOnlyActiveViolations": bool,
+        "includeSuppressedAlerts": bool,
+    },
+    total=False,
+)
+
+class StartDetectMitigationActionsTaskRequestRequestTypeDef(
+    _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef,
+    _OptionalStartDetectMitigationActionsTaskRequestRequestTypeDef,
+):
+    pass
+
 _RequiredTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredTestInvokeAuthorizerRequestRequestTypeDef",
     {
         "authorizerName": str,
     },
 )
 _OptionalTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
@@ -7941,14 +9168,36 @@
         "shadow": str,
         "deviceDefender": str,
         "connectivity": ThingConnectivityTypeDef,
     },
     total=False,
 )
 
+_RequiredTimestreamActionOutputTypeDef = TypedDict(
+    "_RequiredTimestreamActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "databaseName": str,
+        "tableName": str,
+        "dimensions": List[TimestreamDimensionOutputTypeDef],
+    },
+)
+_OptionalTimestreamActionOutputTypeDef = TypedDict(
+    "_OptionalTimestreamActionOutputTypeDef",
+    {
+        "timestamp": TimestreamTimestampOutputTypeDef,
+    },
+    total=False,
+)
+
+class TimestreamActionOutputTypeDef(
+    _RequiredTimestreamActionOutputTypeDef, _OptionalTimestreamActionOutputTypeDef
+):
+    pass
+
 _RequiredTimestreamActionTypeDef = TypedDict(
     "_RequiredTimestreamActionTypeDef",
     {
         "roleArn": str,
         "databaseName": str,
         "tableName": str,
         "dimensions": Sequence[TimestreamDimensionTypeDef],
@@ -7998,14 +9247,23 @@
         "statusReason": str,
         "httpUrlProperties": HttpUrlDestinationPropertiesTypeDef,
         "vpcProperties": VpcDestinationPropertiesTypeDef,
     },
     total=False,
 )
 
+UpdatePackageConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdatePackageConfigurationRequestRequestTypeDef",
+    {
+        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
+        "clientToken": str,
+    },
+    total=False,
+)
+
 ValidateSecurityProfileBehaviorsResponseTypeDef = TypedDict(
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
     {
         "valid": bool,
         "validationErrors": List[ValidationErrorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -8025,14 +9283,37 @@
     {
         "implicitDeny": ImplicitDenyTypeDef,
         "explicitDeny": ExplicitDenyTypeDef,
     },
     total=False,
 )
 
+_RequiredPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
+    "_RequiredPutAssetPropertyValueEntryOutputTypeDef",
+    {
+        "propertyValues": List[AssetPropertyValueOutputTypeDef],
+    },
+)
+_OptionalPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
+    "_OptionalPutAssetPropertyValueEntryOutputTypeDef",
+    {
+        "entryId": str,
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+    },
+    total=False,
+)
+
+class PutAssetPropertyValueEntryOutputTypeDef(
+    _RequiredPutAssetPropertyValueEntryOutputTypeDef,
+    _OptionalPutAssetPropertyValueEntryOutputTypeDef,
+):
+    pass
+
 _RequiredPutAssetPropertyValueEntryTypeDef = TypedDict(
     "_RequiredPutAssetPropertyValueEntryTypeDef",
     {
         "propertyValues": Sequence[AssetPropertyValueTypeDef],
     },
 )
 _OptionalPutAssetPropertyValueEntryTypeDef = TypedDict(
@@ -8136,23 +9417,52 @@
 )
 
 class UpdateThingGroupRequestRequestTypeDef(
     _RequiredUpdateThingGroupRequestRequestTypeDef, _OptionalUpdateThingGroupRequestRequestTypeDef
 ):
     pass
 
+AwsJobExecutionsRolloutConfigOutputTypeDef = TypedDict(
+    "AwsJobExecutionsRolloutConfigOutputTypeDef",
+    {
+        "maximumPerMinute": int,
+        "exponentialRate": AwsJobExponentialRolloutRateOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsJobExecutionsRolloutConfigTypeDef = TypedDict(
     "AwsJobExecutionsRolloutConfigTypeDef",
     {
         "maximumPerMinute": int,
         "exponentialRate": AwsJobExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
+_RequiredBehaviorOutputTypeDef = TypedDict(
+    "_RequiredBehaviorOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalBehaviorOutputTypeDef = TypedDict(
+    "_OptionalBehaviorOutputTypeDef",
+    {
+        "metric": str,
+        "metricDimension": MetricDimensionOutputTypeDef,
+        "criteria": BehaviorCriteriaOutputTypeDef,
+        "suppressAlerts": bool,
+    },
+    total=False,
+)
+
+class BehaviorOutputTypeDef(_RequiredBehaviorOutputTypeDef, _OptionalBehaviorOutputTypeDef):
+    pass
+
 _RequiredBehaviorTypeDef = TypedDict(
     "_RequiredBehaviorTypeDef",
     {
         "name": str,
     },
 )
 _OptionalBehaviorTypeDef = TypedDict(
@@ -8192,15 +9502,15 @@
 ):
     pass
 
 DescribeCACertificateResponseTypeDef = TypedDict(
     "DescribeCACertificateResponseTypeDef",
     {
         "certificateDescription": CACertificateDescriptionTypeDef,
-        "registrationConfig": RegistrationConfigTypeDef,
+        "registrationConfig": RegistrationConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCertificateResponseTypeDef = TypedDict(
     "DescribeCertificateResponseTypeDef",
     {
@@ -8214,33 +9524,67 @@
     {
         "thingTypes": List[ThingTypeDefinitionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StartSigningJobParameterOutputTypeDef = TypedDict(
+    "StartSigningJobParameterOutputTypeDef",
+    {
+        "signingProfileParameter": SigningProfileParameterOutputTypeDef,
+        "signingProfileName": str,
+        "destination": DestinationOutputTypeDef,
+    },
+    total=False,
+)
+
 StartSigningJobParameterTypeDef = TypedDict(
     "StartSigningJobParameterTypeDef",
     {
         "signingProfileParameter": SigningProfileParameterTypeDef,
         "signingProfileName": str,
         "destination": DestinationTypeDef,
     },
     total=False,
 )
 
+JobExecutionsRolloutConfigOutputTypeDef = TypedDict(
+    "JobExecutionsRolloutConfigOutputTypeDef",
+    {
+        "maximumPerMinute": int,
+        "exponentialRate": ExponentialRolloutRateOutputTypeDef,
+    },
+    total=False,
+)
+
 JobExecutionsRolloutConfigTypeDef = TypedDict(
     "JobExecutionsRolloutConfigTypeDef",
     {
         "maximumPerMinute": int,
         "exponentialRate": ExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
+StreamInfoTypeDef = TypedDict(
+    "StreamInfoTypeDef",
+    {
+        "streamId": str,
+        "streamArn": str,
+        "streamVersion": int,
+        "description": str,
+        "files": List[StreamFileOutputTypeDef],
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "roleArn": str,
+    },
+    total=False,
+)
+
 _RequiredCreateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamRequestRequestTypeDef",
     {
         "streamId": str,
         "files": Sequence[StreamFileTypeDef],
         "roleArn": str,
     },
@@ -8255,29 +9599,14 @@
 )
 
 class CreateStreamRequestRequestTypeDef(
     _RequiredCreateStreamRequestRequestTypeDef, _OptionalCreateStreamRequestRequestTypeDef
 ):
     pass
 
-StreamInfoTypeDef = TypedDict(
-    "StreamInfoTypeDef",
-    {
-        "streamId": str,
-        "streamArn": str,
-        "streamVersion": int,
-        "description": str,
-        "files": List[StreamFileTypeDef],
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "roleArn": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamRequestRequestTypeDef",
     {
         "streamId": str,
     },
 )
 _OptionalUpdateStreamRequestRequestTypeDef = TypedDict(
@@ -8298,24 +9627,43 @@
 DescribeThingGroupResponseTypeDef = TypedDict(
     "DescribeThingGroupResponseTypeDef",
     {
         "thingGroupName": str,
         "thingGroupId": str,
         "thingGroupArn": str,
         "version": int,
-        "thingGroupProperties": ThingGroupPropertiesTypeDef,
+        "thingGroupProperties": ThingGroupPropertiesOutputTypeDef,
         "thingGroupMetadata": ThingGroupMetadataTypeDef,
         "indexName": str,
         "queryString": str,
         "queryVersion": str,
         "status": DynamicGroupStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredHttpActionOutputTypeDef = TypedDict(
+    "_RequiredHttpActionOutputTypeDef",
+    {
+        "url": str,
+    },
+)
+_OptionalHttpActionOutputTypeDef = TypedDict(
+    "_OptionalHttpActionOutputTypeDef",
+    {
+        "confirmationUrl": str,
+        "headers": List[HttpActionHeaderOutputTypeDef],
+        "auth": HttpAuthorizationOutputTypeDef,
+    },
+    total=False,
+)
+
+class HttpActionOutputTypeDef(_RequiredHttpActionOutputTypeDef, _OptionalHttpActionOutputTypeDef):
+    pass
+
 _RequiredHttpActionTypeDef = TypedDict(
     "_RequiredHttpActionTypeDef",
     {
         "url": str,
     },
 )
 _OptionalHttpActionTypeDef = TypedDict(
@@ -8330,16 +9678,16 @@
 
 class HttpActionTypeDef(_RequiredHttpActionTypeDef, _OptionalHttpActionTypeDef):
     pass
 
 GetIndexingConfigurationResponseTypeDef = TypedDict(
     "GetIndexingConfigurationResponseTypeDef",
     {
-        "thingIndexingConfiguration": ThingIndexingConfigurationTypeDef,
-        "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationTypeDef,
+        "thingIndexingConfiguration": ThingIndexingConfigurationOutputTypeDef,
+        "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateIndexingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     {
@@ -8389,62 +9737,62 @@
     {
         "logTargetConfigurations": List[LogTargetConfigurationTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateMitigationActionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMitigationActionRequestRequestTypeDef",
-    {
-        "actionName": str,
-        "roleArn": str,
-        "actionParams": MitigationActionParamsTypeDef,
-    },
-)
-_OptionalCreateMitigationActionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMitigationActionRequestRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateMitigationActionRequestRequestTypeDef(
-    _RequiredCreateMitigationActionRequestRequestTypeDef,
-    _OptionalCreateMitigationActionRequestRequestTypeDef,
-):
-    pass
-
 DescribeMitigationActionResponseTypeDef = TypedDict(
     "DescribeMitigationActionResponseTypeDef",
     {
         "actionName": str,
         "actionType": MitigationActionTypeType,
         "actionArn": str,
         "actionId": str,
         "roleArn": str,
-        "actionParams": MitigationActionParamsTypeDef,
+        "actionParams": MitigationActionParamsOutputTypeDef,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MitigationActionTypeDef = TypedDict(
     "MitigationActionTypeDef",
     {
         "name": str,
         "id": str,
         "roleArn": str,
+        "actionParams": MitigationActionParamsOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateMitigationActionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMitigationActionRequestRequestTypeDef",
+    {
+        "actionName": str,
+        "roleArn": str,
         "actionParams": MitigationActionParamsTypeDef,
     },
+)
+_OptionalCreateMitigationActionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMitigationActionRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
     total=False,
 )
 
+class CreateMitigationActionRequestRequestTypeDef(
+    _RequiredCreateMitigationActionRequestRequestTypeDef,
+    _OptionalCreateMitigationActionRequestRequestTypeDef,
+):
+    pass
+
 _RequiredUpdateMitigationActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMitigationActionRequestRequestTypeDef",
     {
         "actionName": str,
     },
 )
 _OptionalUpdateMitigationActionRequestRequestTypeDef = TypedDict(
@@ -8458,14 +9806,35 @@
 
 class UpdateMitigationActionRequestRequestTypeDef(
     _RequiredUpdateMitigationActionRequestRequestTypeDef,
     _OptionalUpdateMitigationActionRequestRequestTypeDef,
 ):
     pass
 
+_RequiredRepublishActionOutputTypeDef = TypedDict(
+    "_RequiredRepublishActionOutputTypeDef",
+    {
+        "roleArn": str,
+        "topic": str,
+    },
+)
+_OptionalRepublishActionOutputTypeDef = TypedDict(
+    "_OptionalRepublishActionOutputTypeDef",
+    {
+        "qos": int,
+        "headers": MqttHeadersOutputTypeDef,
+    },
+    total=False,
+)
+
+class RepublishActionOutputTypeDef(
+    _RequiredRepublishActionOutputTypeDef, _OptionalRepublishActionOutputTypeDef
+):
+    pass
+
 _RequiredRepublishActionTypeDef = TypedDict(
     "_RequiredRepublishActionTypeDef",
     {
         "roleArn": str,
         "topic": str,
     },
 )
@@ -8481,15 +9850,15 @@
 class RepublishActionTypeDef(_RequiredRepublishActionTypeDef, _OptionalRepublishActionTypeDef):
     pass
 
 _RequiredAuditSuppressionTypeDef = TypedDict(
     "_RequiredAuditSuppressionTypeDef",
     {
         "checkName": str,
-        "resourceIdentifier": ResourceIdentifierTypeDef,
+        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
     },
 )
 _OptionalAuditSuppressionTypeDef = TypedDict(
     "_OptionalAuditSuppressionTypeDef",
     {
         "expirationDate": datetime,
         "suppressIndefinitely": bool,
@@ -8497,14 +9866,46 @@
     },
     total=False,
 )
 
 class AuditSuppressionTypeDef(_RequiredAuditSuppressionTypeDef, _OptionalAuditSuppressionTypeDef):
     pass
 
+DescribeAuditSuppressionResponseTypeDef = TypedDict(
+    "DescribeAuditSuppressionResponseTypeDef",
+    {
+        "checkName": str,
+        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
+        "expirationDate": datetime,
+        "suppressIndefinitely": bool,
+        "description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+NonCompliantResourceTypeDef = TypedDict(
+    "NonCompliantResourceTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
+        "additionalInfo": Dict[str, str],
+    },
+    total=False,
+)
+
+RelatedResourceTypeDef = TypedDict(
+    "RelatedResourceTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
+        "additionalInfo": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredCreateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuditSuppressionRequestRequestTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "clientRequestToken": str,
     },
@@ -8537,26 +9938,14 @@
     "DescribeAuditSuppressionRequestRequestTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
 
-DescribeAuditSuppressionResponseTypeDef = TypedDict(
-    "DescribeAuditSuppressionResponseTypeDef",
-    {
-        "checkName": str,
-        "resourceIdentifier": ResourceIdentifierTypeDef,
-        "expirationDate": datetime,
-        "suppressIndefinitely": bool,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListAuditFindingsRequestListAuditFindingsPaginateTypeDef = TypedDict(
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
     {
         "taskId": str,
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "startTime": Union[datetime, str],
@@ -8601,34 +9990,14 @@
         "ascendingOrder": bool,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-NonCompliantResourceTypeDef = TypedDict(
-    "NonCompliantResourceTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceIdentifier": ResourceIdentifierTypeDef,
-        "additionalInfo": Dict[str, str],
-    },
-    total=False,
-)
-
-RelatedResourceTypeDef = TypedDict(
-    "RelatedResourceTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceIdentifier": ResourceIdentifierTypeDef,
-        "additionalInfo": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredUpdateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAuditSuppressionRequestRequestTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
@@ -8689,48 +10058,107 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AuthResultTypeDef = TypedDict(
     "AuthResultTypeDef",
     {
-        "authInfo": AuthInfoTypeDef,
+        "authInfo": AuthInfoOutputTypeDef,
         "allowed": AllowedTypeDef,
         "denied": DeniedTypeDef,
         "authDecision": AuthDecisionType,
         "missingContextValues": List[str],
     },
     total=False,
 )
 
+IotSiteWiseActionOutputTypeDef = TypedDict(
+    "IotSiteWiseActionOutputTypeDef",
+    {
+        "putAssetPropertyValueEntries": List[PutAssetPropertyValueEntryOutputTypeDef],
+        "roleArn": str,
+    },
+)
+
 IotSiteWiseActionTypeDef = TypedDict(
     "IotSiteWiseActionTypeDef",
     {
         "putAssetPropertyValueEntries": Sequence[PutAssetPropertyValueEntryTypeDef],
         "roleArn": str,
     },
 )
 
 ActiveViolationTypeDef = TypedDict(
     "ActiveViolationTypeDef",
     {
         "violationId": str,
         "thingName": str,
         "securityProfileName": str,
-        "behavior": BehaviorTypeDef,
-        "lastViolationValue": MetricValueTypeDef,
+        "behavior": BehaviorOutputTypeDef,
+        "lastViolationValue": MetricValueOutputTypeDef,
         "violationEventAdditionalInfo": ViolationEventAdditionalInfoTypeDef,
         "verificationState": VerificationStateType,
         "verificationStateDescription": str,
         "lastViolationTime": datetime,
         "violationStartTime": datetime,
     },
     total=False,
 )
 
+DescribeSecurityProfileResponseTypeDef = TypedDict(
+    "DescribeSecurityProfileResponseTypeDef",
+    {
+        "securityProfileName": str,
+        "securityProfileArn": str,
+        "securityProfileDescription": str,
+        "behaviors": List[BehaviorOutputTypeDef],
+        "alertTargets": Dict[Literal["SNS"], AlertTargetOutputTypeDef],
+        "additionalMetricsToRetain": List[str],
+        "additionalMetricsToRetainV2": List[MetricToRetainOutputTypeDef],
+        "version": int,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSecurityProfileResponseTypeDef = TypedDict(
+    "UpdateSecurityProfileResponseTypeDef",
+    {
+        "securityProfileName": str,
+        "securityProfileArn": str,
+        "securityProfileDescription": str,
+        "behaviors": List[BehaviorOutputTypeDef],
+        "alertTargets": Dict[Literal["SNS"], AlertTargetOutputTypeDef],
+        "additionalMetricsToRetain": List[str],
+        "additionalMetricsToRetainV2": List[MetricToRetainOutputTypeDef],
+        "version": int,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ViolationEventTypeDef = TypedDict(
+    "ViolationEventTypeDef",
+    {
+        "violationId": str,
+        "thingName": str,
+        "securityProfileName": str,
+        "behavior": BehaviorOutputTypeDef,
+        "metricValue": MetricValueOutputTypeDef,
+        "violationEventAdditionalInfo": ViolationEventAdditionalInfoTypeDef,
+        "violationEventType": ViolationEventTypeType,
+        "verificationState": VerificationStateType,
+        "verificationStateDescription": str,
+        "violationEventTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredCreateSecurityProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileName": str,
     },
 )
 _OptionalCreateSecurityProfileRequestRequestTypeDef = TypedDict(
@@ -8748,31 +10176,14 @@
 
 class CreateSecurityProfileRequestRequestTypeDef(
     _RequiredCreateSecurityProfileRequestRequestTypeDef,
     _OptionalCreateSecurityProfileRequestRequestTypeDef,
 ):
     pass
 
-DescribeSecurityProfileResponseTypeDef = TypedDict(
-    "DescribeSecurityProfileResponseTypeDef",
-    {
-        "securityProfileName": str,
-        "securityProfileArn": str,
-        "securityProfileDescription": str,
-        "behaviors": List[BehaviorTypeDef],
-        "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": List[str],
-        "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
-        "version": int,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileName": str,
     },
 )
 _OptionalUpdateSecurityProfileRequestRequestTypeDef = TypedDict(
@@ -8793,65 +10204,93 @@
 
 class UpdateSecurityProfileRequestRequestTypeDef(
     _RequiredUpdateSecurityProfileRequestRequestTypeDef,
     _OptionalUpdateSecurityProfileRequestRequestTypeDef,
 ):
     pass
 
-UpdateSecurityProfileResponseTypeDef = TypedDict(
-    "UpdateSecurityProfileResponseTypeDef",
-    {
-        "securityProfileName": str,
-        "securityProfileArn": str,
-        "securityProfileDescription": str,
-        "behaviors": List[BehaviorTypeDef],
-        "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
-        "additionalMetricsToRetain": List[str],
-        "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
-        "version": int,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ValidateSecurityProfileBehaviorsRequestRequestTypeDef = TypedDict(
     "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
     {
         "behaviors": Sequence[BehaviorTypeDef],
     },
 )
 
-ViolationEventTypeDef = TypedDict(
-    "ViolationEventTypeDef",
+CodeSigningOutputTypeDef = TypedDict(
+    "CodeSigningOutputTypeDef",
     {
-        "violationId": str,
-        "thingName": str,
-        "securityProfileName": str,
-        "behavior": BehaviorTypeDef,
-        "metricValue": MetricValueTypeDef,
-        "violationEventAdditionalInfo": ViolationEventAdditionalInfoTypeDef,
-        "violationEventType": ViolationEventTypeType,
-        "verificationState": VerificationStateType,
-        "verificationStateDescription": str,
-        "violationEventTime": datetime,
+        "awsSignerJobId": str,
+        "startSigningJobParameter": StartSigningJobParameterOutputTypeDef,
+        "customCodeSigning": CustomCodeSigningOutputTypeDef,
     },
     total=False,
 )
 
 CodeSigningTypeDef = TypedDict(
     "CodeSigningTypeDef",
     {
         "awsSignerJobId": str,
         "startSigningJobParameter": StartSigningJobParameterTypeDef,
         "customCodeSigning": CustomCodeSigningTypeDef,
     },
     total=False,
 )
 
+DescribeJobTemplateResponseTypeDef = TypedDict(
+    "DescribeJobTemplateResponseTypeDef",
+    {
+        "jobTemplateArn": str,
+        "jobTemplateId": str,
+        "description": str,
+        "documentSource": str,
+        "document": str,
+        "createdAt": datetime,
+        "presignedUrlConfig": PresignedUrlConfigOutputTypeDef,
+        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigOutputTypeDef,
+        "abortConfig": AbortConfigOutputTypeDef,
+        "timeoutConfig": TimeoutConfigOutputTypeDef,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
+        "maintenanceWindows": List[MaintenanceWindowOutputTypeDef],
+        "destinationPackageVersions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+JobTypeDef = TypedDict(
+    "JobTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "targetSelection": TargetSelectionType,
+        "status": JobStatusType,
+        "forceCanceled": bool,
+        "reasonCode": str,
+        "comment": str,
+        "targets": List[str],
+        "description": str,
+        "presignedUrlConfig": PresignedUrlConfigOutputTypeDef,
+        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigOutputTypeDef,
+        "abortConfig": AbortConfigOutputTypeDef,
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "completedAt": datetime,
+        "jobProcessDetails": JobProcessDetailsTypeDef,
+        "timeoutConfig": TimeoutConfigOutputTypeDef,
+        "namespaceId": str,
+        "jobTemplateArn": str,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
+        "documentParameters": Dict[str, str],
+        "isConcurrent": bool,
+        "schedulingConfig": SchedulingConfigOutputTypeDef,
+        "scheduledJobRollouts": List[ScheduledJobRolloutTypeDef],
+        "destinationPackageVersions": List[str],
+    },
+    total=False,
+)
+
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "jobId": str,
         "targets": Sequence[str],
     },
 )
@@ -8908,66 +10347,14 @@
 )
 
 class CreateJobTemplateRequestRequestTypeDef(
     _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
     pass
 
-DescribeJobTemplateResponseTypeDef = TypedDict(
-    "DescribeJobTemplateResponseTypeDef",
-    {
-        "jobTemplateArn": str,
-        "jobTemplateId": str,
-        "description": str,
-        "documentSource": str,
-        "document": str,
-        "createdAt": datetime,
-        "presignedUrlConfig": PresignedUrlConfigTypeDef,
-        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
-        "abortConfig": AbortConfigTypeDef,
-        "timeoutConfig": TimeoutConfigTypeDef,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
-        "maintenanceWindows": List[MaintenanceWindowTypeDef],
-        "destinationPackageVersions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-JobTypeDef = TypedDict(
-    "JobTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "targetSelection": TargetSelectionType,
-        "status": JobStatusType,
-        "forceCanceled": bool,
-        "reasonCode": str,
-        "comment": str,
-        "targets": List[str],
-        "description": str,
-        "presignedUrlConfig": PresignedUrlConfigTypeDef,
-        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
-        "abortConfig": AbortConfigTypeDef,
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "completedAt": datetime,
-        "jobProcessDetails": JobProcessDetailsTypeDef,
-        "timeoutConfig": TimeoutConfigTypeDef,
-        "namespaceId": str,
-        "jobTemplateArn": str,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigTypeDef,
-        "documentParameters": Dict[str, str],
-        "isConcurrent": bool,
-        "schedulingConfig": SchedulingConfigTypeDef,
-        "scheduledJobRollouts": List[ScheduledJobRolloutTypeDef],
-        "destinationPackageVersions": List[str],
-    },
-    total=False,
-)
-
 _RequiredUpdateJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalUpdateJobRequestRequestTypeDef = TypedDict(
@@ -9000,30 +10387,30 @@
 DescribeAuditMitigationActionsTaskResponseTypeDef = TypedDict(
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     {
         "taskStatus": AuditMitigationActionsTaskStatusType,
         "startTime": datetime,
         "endTime": datetime,
         "taskStatistics": Dict[str, TaskStatisticsForAuditCheckTypeDef],
-        "target": AuditMitigationActionsTaskTargetTypeDef,
+        "target": AuditMitigationActionsTaskTargetOutputTypeDef,
         "auditCheckToActionsMapping": Dict[str, List[str]],
         "actionsDefinition": List[MitigationActionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectMitigationActionsTaskSummaryTypeDef = TypedDict(
     "DetectMitigationActionsTaskSummaryTypeDef",
     {
         "taskId": str,
         "taskStatus": DetectMitigationActionsTaskStatusType,
         "taskStartTime": datetime,
         "taskEndTime": datetime,
-        "target": DetectMitigationActionsTaskTargetTypeDef,
-        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeTypeDef,
+        "target": DetectMitigationActionsTaskTargetOutputTypeDef,
+        "violationEventOccurrenceRange": ViolationEventOccurrenceRangeOutputTypeDef,
         "onlyActiveViolationsIncluded": bool,
         "suppressedAlertsIncluded": bool,
         "actionsDefinition": List[MitigationActionTypeDef],
         "taskStatistics": DetectMitigationActionsTaskStatisticsTypeDef,
     },
     total=False,
 )
@@ -9068,14 +10455,44 @@
     "TestAuthorizationResponseTypeDef",
     {
         "authResults": List[AuthResultTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "dynamoDB": DynamoDBActionOutputTypeDef,
+        "dynamoDBv2": DynamoDBv2ActionOutputTypeDef,
+        "lambda": LambdaActionOutputTypeDef,
+        "sns": SnsActionOutputTypeDef,
+        "sqs": SqsActionOutputTypeDef,
+        "kinesis": KinesisActionOutputTypeDef,
+        "republish": RepublishActionOutputTypeDef,
+        "s3": S3ActionOutputTypeDef,
+        "firehose": FirehoseActionOutputTypeDef,
+        "cloudwatchMetric": CloudwatchMetricActionOutputTypeDef,
+        "cloudwatchAlarm": CloudwatchAlarmActionOutputTypeDef,
+        "cloudwatchLogs": CloudwatchLogsActionOutputTypeDef,
+        "elasticsearch": ElasticsearchActionOutputTypeDef,
+        "salesforce": SalesforceActionOutputTypeDef,
+        "iotAnalytics": IotAnalyticsActionOutputTypeDef,
+        "iotEvents": IotEventsActionOutputTypeDef,
+        "iotSiteWise": IotSiteWiseActionOutputTypeDef,
+        "stepFunctions": StepFunctionsActionOutputTypeDef,
+        "timestream": TimestreamActionOutputTypeDef,
+        "http": HttpActionOutputTypeDef,
+        "kafka": KafkaActionOutputTypeDef,
+        "openSearch": OpenSearchActionOutputTypeDef,
+        "location": LocationActionOutputTypeDef,
+    },
+    total=False,
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "dynamoDB": DynamoDBActionTypeDef,
         "dynamoDBv2": DynamoDBv2ActionTypeDef,
         "lambda": LambdaActionTypeDef,
         "sns": SnsActionTypeDef,
@@ -9116,14 +10533,27 @@
     {
         "violationEvents": List[ViolationEventTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+OTAUpdateFileOutputTypeDef = TypedDict(
+    "OTAUpdateFileOutputTypeDef",
+    {
+        "fileName": str,
+        "fileType": int,
+        "fileVersion": str,
+        "fileLocation": FileLocationOutputTypeDef,
+        "codeSigning": CodeSigningOutputTypeDef,
+        "attributes": Dict[str, str],
+    },
+    total=False,
+)
+
 OTAUpdateFileTypeDef = TypedDict(
     "OTAUpdateFileTypeDef",
     {
         "fileName": str,
         "fileType": int,
         "fileVersion": str,
         "fileLocation": FileLocationTypeDef,
@@ -9172,14 +10602,29 @@
     {
         "findings": List[AuditFindingTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TopicRuleTypeDef = TypedDict(
+    "TopicRuleTypeDef",
+    {
+        "ruleName": str,
+        "sql": str,
+        "description": str,
+        "createdAt": datetime,
+        "actions": List[ActionOutputTypeDef],
+        "ruleDisabled": bool,
+        "awsIotSqlVersion": str,
+        "errorAction": ActionOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredTopicRulePayloadTypeDef = TypedDict(
     "_RequiredTopicRulePayloadTypeDef",
     {
         "sql": str,
         "actions": Sequence[ActionTypeDef],
     },
 )
@@ -9193,25 +10638,33 @@
     },
     total=False,
 )
 
 class TopicRulePayloadTypeDef(_RequiredTopicRulePayloadTypeDef, _OptionalTopicRulePayloadTypeDef):
     pass
 
-TopicRuleTypeDef = TypedDict(
-    "TopicRuleTypeDef",
+OTAUpdateInfoTypeDef = TypedDict(
+    "OTAUpdateInfoTypeDef",
     {
-        "ruleName": str,
-        "sql": str,
+        "otaUpdateId": str,
+        "otaUpdateArn": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
         "description": str,
-        "createdAt": datetime,
-        "actions": List[ActionTypeDef],
-        "ruleDisabled": bool,
-        "awsIotSqlVersion": str,
-        "errorAction": ActionTypeDef,
+        "targets": List[str],
+        "protocols": List[ProtocolType],
+        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigOutputTypeDef,
+        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigOutputTypeDef,
+        "targetSelection": TargetSelectionType,
+        "otaUpdateFiles": List[OTAUpdateFileOutputTypeDef],
+        "otaUpdateStatus": OTAUpdateStatusType,
+        "awsIotJobId": str,
+        "awsIotJobArn": str,
+        "errorInfo": ErrorInfoTypeDef,
+        "additionalParameters": Dict[str, str],
     },
     total=False,
 )
 
 _RequiredCreateOTAUpdateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOTAUpdateRequestRequestTypeDef",
     {
@@ -9238,35 +10691,21 @@
 )
 
 class CreateOTAUpdateRequestRequestTypeDef(
     _RequiredCreateOTAUpdateRequestRequestTypeDef, _OptionalCreateOTAUpdateRequestRequestTypeDef
 ):
     pass
 
-OTAUpdateInfoTypeDef = TypedDict(
-    "OTAUpdateInfoTypeDef",
+GetTopicRuleResponseTypeDef = TypedDict(
+    "GetTopicRuleResponseTypeDef",
     {
-        "otaUpdateId": str,
-        "otaUpdateArn": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "description": str,
-        "targets": List[str],
-        "protocols": List[ProtocolType],
-        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
-        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
-        "targetSelection": TargetSelectionType,
-        "otaUpdateFiles": List[OTAUpdateFileTypeDef],
-        "otaUpdateStatus": OTAUpdateStatusType,
-        "awsIotJobId": str,
-        "awsIotJobArn": str,
-        "errorInfo": ErrorInfoTypeDef,
-        "additionalParameters": Dict[str, str],
+        "ruleArn": str,
+        "rule": TopicRuleTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 _RequiredCreateTopicRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
         "topicRulePayload": TopicRulePayloadTypeDef,
@@ -9289,23 +10728,14 @@
     "ReplaceTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
         "topicRulePayload": TopicRulePayloadTypeDef,
     },
 )
 
-GetTopicRuleResponseTypeDef = TypedDict(
-    "GetTopicRuleResponseTypeDef",
-    {
-        "ruleArn": str,
-        "rule": TopicRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetOTAUpdateResponseTypeDef = TypedDict(
     "GetOTAUpdateResponseTypeDef",
     {
         "otaUpdateInfo": OTAUpdateInfoTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/PKG-INFO` & `mypy-boto3-iot-1.28.12/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-iot
-Version: 1.28.0
-Summary: Type annotations for boto3.IoT 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iot type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iot"></a>
 
 # mypy-boto3-iot
 
 [![PyPI - mypy-boto3-iot](https://img.shields.io/pypi/v/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot?color=blue)](https://pypistats.org/packages/mypy-boto3-iot)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot)](https://pepy.tech/project/mypy-boto3-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[boto3.IoT 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
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
 [mypy-boto3-iot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/).
 
 See how it helps to find and fix potential bugs:
 
@@ -645,16 +613,34 @@
 ### Typed dictionaries
 
 `mypy_boto3_iot.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot.type_defs import (
+    AbortCriteriaOutputTypeDef,
     AbortCriteriaTypeDef,
     AcceptCertificateTransferRequestRequestTypeDef,
+    CloudwatchAlarmActionOutputTypeDef,
+    CloudwatchLogsActionOutputTypeDef,
+    CloudwatchMetricActionOutputTypeDef,
+    DynamoDBActionOutputTypeDef,
+    ElasticsearchActionOutputTypeDef,
+    FirehoseActionOutputTypeDef,
+    IotAnalyticsActionOutputTypeDef,
+    IotEventsActionOutputTypeDef,
+    KafkaActionOutputTypeDef,
+    KinesisActionOutputTypeDef,
+    LambdaActionOutputTypeDef,
+    OpenSearchActionOutputTypeDef,
+    S3ActionOutputTypeDef,
+    SalesforceActionOutputTypeDef,
+    SnsActionOutputTypeDef,
+    SqsActionOutputTypeDef,
+    StepFunctionsActionOutputTypeDef,
     CloudwatchAlarmActionTypeDef,
     CloudwatchLogsActionTypeDef,
     CloudwatchMetricActionTypeDef,
     DynamoDBActionTypeDef,
     ElasticsearchActionTypeDef,
     FirehoseActionTypeDef,
     IotAnalyticsActionTypeDef,
@@ -664,67 +650,88 @@
     LambdaActionTypeDef,
     OpenSearchActionTypeDef,
     S3ActionTypeDef,
     SalesforceActionTypeDef,
     SnsActionTypeDef,
     SqsActionTypeDef,
     StepFunctionsActionTypeDef,
-    MetricValueTypeDef,
+    MetricValueOutputTypeDef,
     ViolationEventAdditionalInfoTypeDef,
     AddThingToBillingGroupRequestRequestTypeDef,
     AddThingToThingGroupRequestRequestTypeDef,
+    AddThingsToThingGroupParamsOutputTypeDef,
     AddThingsToThingGroupParamsTypeDef,
+    AggregationTypeOutputTypeDef,
     AggregationTypeTypeDef,
+    AlertTargetOutputTypeDef,
     AlertTargetTypeDef,
     PolicyTypeDef,
+    AssetPropertyTimestampOutputTypeDef,
     AssetPropertyTimestampTypeDef,
+    AssetPropertyVariantOutputTypeDef,
     AssetPropertyVariantTypeDef,
     AssociateTargetsWithJobRequestRequestTypeDef,
     AssociateTargetsWithJobResponseTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachPrincipalPolicyRequestRequestTypeDef,
     AttachSecurityProfileRequestRequestTypeDef,
     AttachThingPrincipalRequestRequestTypeDef,
+    AttributePayloadOutputTypeDef,
     AttributePayloadTypeDef,
+    AuditCheckConfigurationOutputTypeDef,
     AuditCheckConfigurationTypeDef,
     AuditCheckDetailsTypeDef,
     AuditMitigationActionExecutionMetadataTypeDef,
     AuditMitigationActionsTaskMetadataTypeDef,
+    AuditMitigationActionsTaskTargetOutputTypeDef,
     AuditMitigationActionsTaskTargetTypeDef,
+    AuditNotificationTargetOutputTypeDef,
     AuditNotificationTargetTypeDef,
     AuditTaskMetadataTypeDef,
+    AuthInfoOutputTypeDef,
     AuthInfoTypeDef,
+    AuthorizerConfigOutputTypeDef,
     AuthorizerConfigTypeDef,
     AuthorizerDescriptionTypeDef,
     AuthorizerSummaryTypeDef,
     AwsJobAbortCriteriaTypeDef,
+    AwsJobRateIncreaseCriteriaOutputTypeDef,
     AwsJobRateIncreaseCriteriaTypeDef,
+    AwsJobPresignedUrlConfigOutputTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
+    MachineLearningDetectionConfigOutputTypeDef,
+    StatisticalThresholdOutputTypeDef,
     MachineLearningDetectionConfigTypeDef,
+    MetricValueTypeDef,
     StatisticalThresholdTypeDef,
     BehaviorModelTrainingSummaryTypeDef,
+    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     BillingGroupMetadataTypeDef,
+    BillingGroupPropertiesOutputTypeDef,
     BillingGroupPropertiesTypeDef,
     BucketTypeDef,
     TermsAggregationTypeDef,
     CertificateValidityTypeDef,
     CACertificateTypeDef,
     CancelAuditMitigationActionsTaskRequestRequestTypeDef,
     CancelAuditTaskRequestRequestTypeDef,
     CancelCertificateTransferRequestRequestTypeDef,
     CancelDetectMitigationActionsTaskRequestRequestTypeDef,
     CancelJobExecutionRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     CancelJobResponseTypeDef,
     TransferDataTypeDef,
     CertificateTypeDef,
+    CodeSigningCertificateChainOutputTypeDef,
     CodeSigningCertificateChainTypeDef,
+    CodeSigningSignatureOutputTypeDef,
     CodeSigningSignatureTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ConfirmTopicRuleDestinationRequestRequestTypeDef,
     TagTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateBillingGroupResponseTypeDef,
     CreateCertificateFromCsrRequestRequestTypeDef,
     CreateCertificateFromCsrResponseTypeDef,
@@ -799,35 +806,40 @@
     DescribeAuditMitigationActionsTaskRequestRequestTypeDef,
     TaskStatisticsForAuditCheckTypeDef,
     DescribeAuditTaskRequestRequestTypeDef,
     TaskStatisticsTypeDef,
     DescribeAuthorizerRequestRequestTypeDef,
     DescribeBillingGroupRequestRequestTypeDef,
     DescribeCACertificateRequestRequestTypeDef,
-    RegistrationConfigTypeDef,
+    RegistrationConfigOutputTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     DescribeCustomMetricRequestRequestTypeDef,
     DescribeCustomMetricResponseTypeDef,
     DescribeDetectMitigationActionsTaskRequestRequestTypeDef,
     DescribeDimensionRequestRequestTypeDef,
     DescribeDimensionResponseTypeDef,
     DescribeDomainConfigurationRequestRequestTypeDef,
     ServerCertificateSummaryTypeDef,
+    TlsConfigOutputTypeDef,
     DescribeEndpointRequestRequestTypeDef,
     DescribeEndpointResponseTypeDef,
     DescribeFleetMetricRequestRequestTypeDef,
     DescribeIndexRequestRequestTypeDef,
     DescribeIndexResponseTypeDef,
     DescribeJobExecutionRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
+    MaintenanceWindowOutputTypeDef,
+    PresignedUrlConfigOutputTypeDef,
+    TimeoutConfigOutputTypeDef,
     DescribeManagedJobTemplateRequestRequestTypeDef,
     DocumentParameterTypeDef,
     DescribeMitigationActionRequestRequestTypeDef,
     DescribeProvisioningTemplateRequestRequestTypeDef,
+    ProvisioningHookOutputTypeDef,
     DescribeProvisioningTemplateVersionRequestRequestTypeDef,
     DescribeProvisioningTemplateVersionResponseTypeDef,
     DescribeRoleAliasRequestRequestTypeDef,
     RoleAliasDescriptionTypeDef,
     DescribeScheduledAuditRequestRequestTypeDef,
     DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileRequestRequestTypeDef,
@@ -835,46 +847,55 @@
     DescribeThingGroupRequestRequestTypeDef,
     DescribeThingRegistrationTaskRequestRequestTypeDef,
     DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingRequestRequestTypeDef,
     DescribeThingResponseTypeDef,
     DescribeThingTypeRequestRequestTypeDef,
     ThingTypeMetadataTypeDef,
+    ThingTypePropertiesOutputTypeDef,
+    S3DestinationOutputTypeDef,
     S3DestinationTypeDef,
     DetachPolicyRequestRequestTypeDef,
     DetachPrincipalPolicyRequestRequestTypeDef,
     DetachSecurityProfileRequestRequestTypeDef,
     DetachThingPrincipalRequestRequestTypeDef,
     DetectMitigationActionExecutionTypeDef,
     DetectMitigationActionsTaskStatisticsTypeDef,
+    DetectMitigationActionsTaskTargetOutputTypeDef,
+    ViolationEventOccurrenceRangeOutputTypeDef,
     DetectMitigationActionsTaskTargetTypeDef,
-    ViolationEventOccurrenceRangeTypeDef,
     DisableTopicRuleRequestRequestTypeDef,
     DomainConfigurationSummaryTypeDef,
+    PutItemInputOutputTypeDef,
     PutItemInputTypeDef,
     EffectivePolicyTypeDef,
     EmptyResponseMetadataTypeDef,
+    EnableIoTLoggingParamsOutputTypeDef,
     EnableIoTLoggingParamsTypeDef,
     EnableTopicRuleRequestRequestTypeDef,
     ErrorInfoTypeDef,
+    RateIncreaseCriteriaOutputTypeDef,
     RateIncreaseCriteriaTypeDef,
+    FieldOutputTypeDef,
     FieldTypeDef,
+    S3LocationOutputTypeDef,
+    StreamOutputTypeDef,
     S3LocationTypeDef,
     StreamTypeDef,
     FleetMetricNameAndArnTypeDef,
     GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef,
     GetBehaviorModelTrainingSummariesRequestRequestTypeDef,
     GetCardinalityRequestRequestTypeDef,
     GetCardinalityResponseTypeDef,
     GetEffectivePoliciesRequestRequestTypeDef,
     GetJobDocumentRequestRequestTypeDef,
     GetJobDocumentResponseTypeDef,
     GetLoggingOptionsResponseTypeDef,
     GetOTAUpdateRequestRequestTypeDef,
-    VersionUpdateByJobsConfigTypeDef,
+    VersionUpdateByJobsConfigOutputTypeDef,
     GetPackageRequestRequestTypeDef,
     GetPackageResponseTypeDef,
     GetPackageVersionRequestRequestTypeDef,
     GetPackageVersionResponseTypeDef,
     GetPercentilesRequestRequestTypeDef,
     PercentPairTypeDef,
     GetPolicyRequestRequestTypeDef,
@@ -884,24 +905,29 @@
     GetRegistrationCodeResponseTypeDef,
     GetStatisticsRequestRequestTypeDef,
     StatisticsTypeDef,
     GetTopicRuleDestinationRequestRequestTypeDef,
     GetTopicRuleRequestRequestTypeDef,
     GetV2LoggingOptionsResponseTypeDef,
     GroupNameAndArnTypeDef,
+    HttpActionHeaderOutputTypeDef,
     HttpActionHeaderTypeDef,
+    SigV4AuthorizationOutputTypeDef,
     SigV4AuthorizationTypeDef,
     HttpContextTypeDef,
     HttpUrlDestinationConfigurationTypeDef,
     HttpUrlDestinationPropertiesTypeDef,
     HttpUrlDestinationSummaryTypeDef,
+    IndexingFilterOutputTypeDef,
     IndexingFilterTypeDef,
+    IssuerCertificateIdentifierOutputTypeDef,
     IssuerCertificateIdentifierTypeDef,
     JobExecutionStatusDetailsTypeDef,
     JobExecutionSummaryTypeDef,
+    RetryCriteriaOutputTypeDef,
     RetryCriteriaTypeDef,
     JobProcessDetailsTypeDef,
     JobSummaryTypeDef,
     JobTemplateSummaryTypeDef,
     ScheduledJobRolloutTypeDef,
     ListActiveViolationsRequestListActiveViolationsPaginateTypeDef,
     ListActiveViolationsRequestRequestTypeDef,
@@ -1000,14 +1026,15 @@
     ListSecurityProfilesRequestRequestTypeDef,
     SecurityProfileIdentifierTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     StreamSummaryTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
     ListTargetsForPolicyRequestRequestTypeDef,
     ListTargetsForPolicyResponseTypeDef,
     ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
     ListTargetsForSecurityProfileRequestRequestTypeDef,
     SecurityProfileTargetTypeDef,
     ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
@@ -1039,26 +1066,35 @@
     ListTopicRulesRequestListTopicRulesPaginateTypeDef,
     ListTopicRulesRequestRequestTypeDef,
     TopicRuleListItemTypeDef,
     ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef,
     ListV2LoggingLevelsRequestRequestTypeDef,
     ListViolationEventsRequestListViolationEventsPaginateTypeDef,
     ListViolationEventsRequestRequestTypeDef,
+    LocationTimestampOutputTypeDef,
     LocationTimestampTypeDef,
+    LogTargetOutputTypeDef,
     LogTargetTypeDef,
     LoggingOptionsPayloadTypeDef,
+    PublishFindingToSnsParamsOutputTypeDef,
+    ReplaceDefaultPolicyVersionParamsOutputTypeDef,
+    UpdateCACertificateParamsOutputTypeDef,
+    UpdateDeviceCertificateParamsOutputTypeDef,
     PublishFindingToSnsParamsTypeDef,
     ReplaceDefaultPolicyVersionParamsTypeDef,
     UpdateCACertificateParamsTypeDef,
     UpdateDeviceCertificateParamsTypeDef,
     MqttContextTypeDef,
+    UserPropertyOutputTypeDef,
     UserPropertyTypeDef,
     PaginatorConfigTypeDef,
+    PolicyVersionIdentifierOutputTypeDef,
     PolicyVersionIdentifierTypeDef,
     PutVerificationStateOnViolationRequestRequestTypeDef,
+    RegistrationConfigTypeDef,
     RegisterCACertificateResponseTypeDef,
     RegisterCertificateRequestRequestTypeDef,
     RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCARequestRequestTypeDef,
     RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingRequestRequestTypeDef,
     RegisterThingResponseTypeDef,
@@ -1068,25 +1104,29 @@
     ResponseMetadataTypeDef,
     SearchIndexRequestRequestTypeDef,
     ThingGroupDocumentTypeDef,
     SetDefaultAuthorizerRequestRequestTypeDef,
     SetDefaultAuthorizerResponseTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetV2LoggingOptionsRequestRequestTypeDef,
+    SigningProfileParameterOutputTypeDef,
     SigningProfileParameterTypeDef,
     StartAuditMitigationActionsTaskResponseTypeDef,
+    ViolationEventOccurrenceRangeTypeDef,
     StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskRequestRequestTypeDef,
     StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskRequestRequestTypeDef,
     StartThingRegistrationTaskResponseTypeDef,
     StopThingRegistrationTaskRequestRequestTypeDef,
     TlsContextTypeDef,
     TestInvokeAuthorizerResponseTypeDef,
     ThingConnectivityTypeDef,
+    TimestreamDimensionOutputTypeDef,
+    TimestreamTimestampOutputTypeDef,
     TimestreamDimensionTypeDef,
     TimestreamTimestampTypeDef,
     VpcDestinationConfigurationTypeDef,
     VpcDestinationSummaryTypeDef,
     VpcDestinationPropertiesTypeDef,
     TransferCertificateRequestRequestTypeDef,
     TransferCertificateResponseTypeDef,
@@ -1098,117 +1138,130 @@
     UpdateCustomMetricRequestRequestTypeDef,
     UpdateCustomMetricResponseTypeDef,
     UpdateDimensionRequestRequestTypeDef,
     UpdateDimensionResponseTypeDef,
     UpdateDomainConfigurationResponseTypeDef,
     UpdateDynamicThingGroupResponseTypeDef,
     UpdateMitigationActionResponseTypeDef,
+    VersionUpdateByJobsConfigTypeDef,
     UpdatePackageRequestRequestTypeDef,
     UpdatePackageVersionRequestRequestTypeDef,
     UpdateRoleAliasRequestRequestTypeDef,
     UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditRequestRequestTypeDef,
     UpdateScheduledAuditResponseTypeDef,
     UpdateStreamResponseTypeDef,
     UpdateThingGroupResponseTypeDef,
     UpdateThingGroupsForThingRequestRequestTypeDef,
     UpdateTopicRuleDestinationRequestRequestTypeDef,
     ValidationErrorTypeDef,
+    AbortConfigOutputTypeDef,
     AbortConfigTypeDef,
     MetricDatumTypeDef,
     DescribeFleetMetricResponseTypeDef,
     UpdateFleetMetricRequestRequestTypeDef,
     AllowedTypeDef,
     ExplicitDenyTypeDef,
     ImplicitDenyTypeDef,
     ListAttachedPoliciesResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListPrincipalPoliciesResponseTypeDef,
+    AssetPropertyValueOutputTypeDef,
     AssetPropertyValueTypeDef,
+    ThingGroupPropertiesOutputTypeDef,
     CreateThingRequestRequestTypeDef,
     ThingGroupPropertiesTypeDef,
     UpdateThingRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
     StartAuditMitigationActionsTaskRequestRequestTypeDef,
     DescribeAccountAuditConfigurationResponseTypeDef,
     UpdateAccountAuditConfigurationRequestRequestTypeDef,
     ListAuditTasksResponseTypeDef,
     TestAuthorizationRequestRequestTypeDef,
     DescribeAuthorizerResponseTypeDef,
     DescribeDefaultAuthorizerResponseTypeDef,
     ListAuthorizersResponseTypeDef,
     AwsJobAbortConfigTypeDef,
+    AwsJobExponentialRolloutRateOutputTypeDef,
     AwsJobExponentialRolloutRateTypeDef,
+    BehaviorCriteriaOutputTypeDef,
     BehaviorCriteriaTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
+    MetricToRetainOutputTypeDef,
     MetricToRetainTypeDef,
     DescribeBillingGroupResponseTypeDef,
     UpdateBillingGroupRequestRequestTypeDef,
     GetBucketsAggregationResponseTypeDef,
     BucketsAggregationTypeTypeDef,
     CACertificateDescriptionTypeDef,
     ListCACertificatesResponseTypeDef,
     CertificateDescriptionTypeDef,
     ListCertificatesByCAResponseTypeDef,
     ListCertificatesResponseTypeDef,
+    CustomCodeSigningOutputTypeDef,
     CustomCodeSigningTypeDef,
     DescribeEventConfigurationsResponseTypeDef,
     UpdateEventConfigurationsRequestRequestTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     CreateBillingGroupRequestRequestTypeDef,
     CreateCustomMetricRequestRequestTypeDef,
     CreateDimensionRequestRequestTypeDef,
     CreateFleetMetricRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreateRoleAliasRequestRequestTypeDef,
     CreateScheduledAuditRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainConfigurationRequestRequestTypeDef,
     UpdateDomainConfigurationRequestRequestTypeDef,
     SchedulingConfigTypeDef,
     CreateKeysAndCertificateResponseTypeDef,
     CreateProvisioningClaimResponseTypeDef,
     CreateProvisioningTemplateRequestRequestTypeDef,
-    DescribeProvisioningTemplateResponseTypeDef,
     UpdateProvisioningTemplateRequestRequestTypeDef,
     CreateThingTypeRequestRequestTypeDef,
     DescribeAuditTaskResponseTypeDef,
-    RegisterCACertificateRequestRequestTypeDef,
-    UpdateCACertificateRequestRequestTypeDef,
     DescribeDomainConfigurationResponseTypeDef,
+    SchedulingConfigOutputTypeDef,
     DescribeManagedJobTemplateResponseTypeDef,
+    DescribeProvisioningTemplateResponseTypeDef,
     DescribeRoleAliasResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
     ThingTypeDefinitionTypeDef,
+    DestinationOutputTypeDef,
     DestinationTypeDef,
     ListDetectMitigationActionsExecutionsResponseTypeDef,
-    StartDetectMitigationActionsTaskRequestRequestTypeDef,
     ListDomainConfigurationsResponseTypeDef,
+    DynamoDBv2ActionOutputTypeDef,
     DynamoDBv2ActionTypeDef,
     GetEffectivePoliciesResponseTypeDef,
+    ExponentialRolloutRateOutputTypeDef,
     ExponentialRolloutRateTypeDef,
+    ThingGroupIndexingConfigurationOutputTypeDef,
     ThingGroupIndexingConfigurationTypeDef,
+    StreamFileOutputTypeDef,
+    FileLocationOutputTypeDef,
     StreamFileTypeDef,
     FileLocationTypeDef,
     ListFleetMetricsResponseTypeDef,
     GetPackageConfigurationResponseTypeDef,
-    UpdatePackageConfigurationRequestRequestTypeDef,
     GetPercentilesResponseTypeDef,
     GetStatisticsResponseTypeDef,
     ListBillingGroupsResponseTypeDef,
     ListThingGroupsForThingResponseTypeDef,
     ListThingGroupsResponseTypeDef,
     ThingGroupMetadataTypeDef,
+    HttpAuthorizationOutputTypeDef,
     HttpAuthorizationTypeDef,
+    ThingIndexingConfigurationOutputTypeDef,
     ThingIndexingConfigurationTypeDef,
     JobExecutionTypeDef,
     JobExecutionSummaryForJobTypeDef,
     JobExecutionSummaryForThingTypeDef,
+    JobExecutionsRetryConfigOutputTypeDef,
     JobExecutionsRetryConfigTypeDef,
     ListJobsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedJobTemplatesResponseTypeDef,
     ListMitigationActionsResponseTypeDef,
     ListOTAUpdatesResponseTypeDef,
     ListOutgoingCertificatesResponseTypeDef,
@@ -1216,124 +1269,145 @@
     ListPackagesResponseTypeDef,
     ListPolicyVersionsResponseTypeDef,
     ListProvisioningTemplateVersionsResponseTypeDef,
     ListProvisioningTemplatesResponseTypeDef,
     ListScheduledAuditsResponseTypeDef,
     ListSecurityProfilesResponseTypeDef,
     ListStreamsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTargetsForSecurityProfileResponseTypeDef,
     SecurityProfileTargetMappingTypeDef,
     ListThingsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
+    LocationActionOutputTypeDef,
     LocationActionTypeDef,
     LogTargetConfigurationTypeDef,
     SetV2LoggingLevelRequestRequestTypeDef,
     SetLoggingOptionsRequestRequestTypeDef,
+    MitigationActionParamsOutputTypeDef,
     MitigationActionParamsTypeDef,
+    MqttHeadersOutputTypeDef,
     MqttHeadersTypeDef,
+    ResourceIdentifierOutputTypeDef,
     ResourceIdentifierTypeDef,
+    RegisterCACertificateRequestRequestTypeDef,
+    UpdateCACertificateRequestRequestTypeDef,
+    StartDetectMitigationActionsTaskRequestRequestTypeDef,
     TestInvokeAuthorizerRequestRequestTypeDef,
     ThingDocumentTypeDef,
+    TimestreamActionOutputTypeDef,
     TimestreamActionTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRuleDestinationSummaryTypeDef,
     TopicRuleDestinationTypeDef,
+    UpdatePackageConfigurationRequestRequestTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
     ListMetricValuesResponseTypeDef,
     DeniedTypeDef,
+    PutAssetPropertyValueEntryOutputTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     CreateDynamicThingGroupRequestRequestTypeDef,
     CreateThingGroupRequestRequestTypeDef,
     UpdateDynamicThingGroupRequestRequestTypeDef,
     UpdateThingGroupRequestRequestTypeDef,
+    AwsJobExecutionsRolloutConfigOutputTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
+    BehaviorOutputTypeDef,
     BehaviorTypeDef,
     GetBucketsAggregationRequestRequestTypeDef,
     DescribeCACertificateResponseTypeDef,
     DescribeCertificateResponseTypeDef,
     ListThingTypesResponseTypeDef,
+    StartSigningJobParameterOutputTypeDef,
     StartSigningJobParameterTypeDef,
+    JobExecutionsRolloutConfigOutputTypeDef,
     JobExecutionsRolloutConfigTypeDef,
-    CreateStreamRequestRequestTypeDef,
     StreamInfoTypeDef,
+    CreateStreamRequestRequestTypeDef,
     UpdateStreamRequestRequestTypeDef,
     DescribeThingGroupResponseTypeDef,
+    HttpActionOutputTypeDef,
     HttpActionTypeDef,
     GetIndexingConfigurationResponseTypeDef,
     UpdateIndexingConfigurationRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
     ListJobExecutionsForJobResponseTypeDef,
     ListJobExecutionsForThingResponseTypeDef,
     ListSecurityProfilesForTargetResponseTypeDef,
     ListV2LoggingLevelsResponseTypeDef,
-    CreateMitigationActionRequestRequestTypeDef,
     DescribeMitigationActionResponseTypeDef,
     MitigationActionTypeDef,
+    CreateMitigationActionRequestRequestTypeDef,
     UpdateMitigationActionRequestRequestTypeDef,
+    RepublishActionOutputTypeDef,
     RepublishActionTypeDef,
     AuditSuppressionTypeDef,
+    DescribeAuditSuppressionResponseTypeDef,
+    NonCompliantResourceTypeDef,
+    RelatedResourceTypeDef,
     CreateAuditSuppressionRequestRequestTypeDef,
     DeleteAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionRequestRequestTypeDef,
-    DescribeAuditSuppressionResponseTypeDef,
     ListAuditFindingsRequestListAuditFindingsPaginateTypeDef,
     ListAuditFindingsRequestRequestTypeDef,
     ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef,
     ListAuditSuppressionsRequestRequestTypeDef,
-    NonCompliantResourceTypeDef,
-    RelatedResourceTypeDef,
     UpdateAuditSuppressionRequestRequestTypeDef,
     SearchIndexResponseTypeDef,
     CreateTopicRuleDestinationRequestRequestTypeDef,
     ListTopicRuleDestinationsResponseTypeDef,
     CreateTopicRuleDestinationResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     AuthResultTypeDef,
+    IotSiteWiseActionOutputTypeDef,
     IotSiteWiseActionTypeDef,
     ActiveViolationTypeDef,
-    CreateSecurityProfileRequestRequestTypeDef,
     DescribeSecurityProfileResponseTypeDef,
-    UpdateSecurityProfileRequestRequestTypeDef,
     UpdateSecurityProfileResponseTypeDef,
-    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
     ViolationEventTypeDef,
+    CreateSecurityProfileRequestRequestTypeDef,
+    UpdateSecurityProfileRequestRequestTypeDef,
+    ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
+    CodeSigningOutputTypeDef,
     CodeSigningTypeDef,
-    CreateJobRequestRequestTypeDef,
-    CreateJobTemplateRequestRequestTypeDef,
     DescribeJobTemplateResponseTypeDef,
     JobTypeDef,
+    CreateJobRequestRequestTypeDef,
+    CreateJobTemplateRequestRequestTypeDef,
     UpdateJobRequestRequestTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeAuditMitigationActionsTaskResponseTypeDef,
     DetectMitigationActionsTaskSummaryTypeDef,
     ListAuditSuppressionsResponseTypeDef,
     AuditFindingTypeDef,
     ListRelatedResourcesForAuditFindingResponseTypeDef,
     TestAuthorizationResponseTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
     ListActiveViolationsResponseTypeDef,
     ListViolationEventsResponseTypeDef,
+    OTAUpdateFileOutputTypeDef,
     OTAUpdateFileTypeDef,
     DescribeJobResponseTypeDef,
     DescribeDetectMitigationActionsTaskResponseTypeDef,
     ListDetectMitigationActionsTasksResponseTypeDef,
     DescribeAuditFindingResponseTypeDef,
     ListAuditFindingsResponseTypeDef,
-    TopicRulePayloadTypeDef,
     TopicRuleTypeDef,
-    CreateOTAUpdateRequestRequestTypeDef,
+    TopicRulePayloadTypeDef,
     OTAUpdateInfoTypeDef,
+    CreateOTAUpdateRequestRequestTypeDef,
+    GetTopicRuleResponseTypeDef,
     CreateTopicRuleRequestRequestTypeDef,
     ReplaceTopicRuleRequestRequestTypeDef,
-    GetTopicRuleResponseTypeDef,
     GetOTAUpdateResponseTypeDef,
 )
 
 
-def get_structure() -> AbortCriteriaTypeDef:
+def get_structure() -> AbortCriteriaOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/SOURCES.txt` & `mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.0/setup.py` & `mypy-boto3-iot-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_iot"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoT 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.IoT 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

