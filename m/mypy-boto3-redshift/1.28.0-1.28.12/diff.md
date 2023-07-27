# Comparing `tmp/mypy-boto3-redshift-1.28.0.tar.gz` & `tmp/mypy-boto3-redshift-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-redshift-1.28.0.tar", last modified: Thu Jul  6 21:00:25 2023, max compression
+gzip compressed data, was "mypy-boto3-redshift-1.28.12.tar", last modified: Thu Jul 27 11:49:27 2023, max compression
```

## Comparing `mypy-boto3-redshift-1.28.0.tar` & `mypy-boto3-redshift-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:25.342406 mypy-boto3-redshift-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:52:47.000000 mypy-boto3-redshift-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36979 2023-07-06 21:00:25.338406 mypy-boto3-redshift-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35490 2023-07-06 20:52:47.000000 mypy-boto3-redshift-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:25.330406 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-06 20:52:47.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-06 20:52:47.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:52:47.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115402 2023-07-06 20:52:49.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   115235 2023-07-06 20:52:48.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-07-06 20:52:53.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-07-06 20:52:49.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    43616 2023-07-06 20:52:49.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43581 2023-07-06 20:52:49.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:52:47.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   134445 2023-07-06 20:52:57.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   134326 2023-07-06 20:52:55.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:52:47.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-06 20:52:49.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-06 20:52:49.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:25.338406 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36979 2023-07-06 21:00:25.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-06 21:00:25.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:25.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:25.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:25.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:25.000000 mypy-boto3-redshift-1.28.0/mypy_boto3_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:25.342406 mypy-boto3-redshift-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:52:47.000000 mypy-boto3-redshift-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.825190 mypy-boto3-redshift-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-07-27 11:49:27.825190 mypy-boto3-redshift-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35679 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.821190 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115402 2023-07-27 11:44:17.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115235 2023-07-27 11:44:16.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17351 2023-07-27 11:44:19.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-07-27 11:44:19.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    43550 2023-07-27 11:44:17.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43515 2023-07-27 11:44:17.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   136230 2023-07-27 11:44:22.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136109 2023-07-27 11:44:20.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-27 11:44:17.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-27 11:44:17.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.825190 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-07-27 11:49:27.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-27 11:49:27.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:27.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:27.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:27.825190 mypy-boto3-redshift-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/setup.py
```

### Comparing `mypy-boto3-redshift-1.28.0/LICENSE` & `mypy-boto3-redshift-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.0/PKG-INFO` & `mypy-boto3-redshift-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift
-Version: 1.28.0
-Summary: Type annotations for boto3.Redshift 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Redshift 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-redshift"></a>
 
 # mypy-boto3-redshift
 
 [![PyPI - mypy-boto3-redshift](https://img.shields.io/pypi/v/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift)](https://pepy.tech/project/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
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
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -538,14 +538,15 @@
 
 `mypy_boto3_redshift.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift.type_defs import (
     AcceptReservedNodeExchangeInputMessageRequestTypeDef,
+    ResponseMetadataTypeDef,
     AttributeValueTargetTypeDef,
     AccountWithRestoreAccessTypeDef,
     AquaConfigurationTypeDef,
     AssociateDataShareConsumerMessageRequestTypeDef,
     CertificateAssociationTypeDef,
     AuthenticationProfileTypeDef,
     AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
@@ -554,46 +555,40 @@
     AuthorizeSnapshotAccessMessageRequestTypeDef,
     SupportedPlatformTypeDef,
     DeleteClusterSnapshotMessageTypeDef,
     SnapshotErrorMessageTypeDef,
     BatchModifyClusterSnapshotsMessageRequestTypeDef,
     CancelResizeMessageRequestTypeDef,
     ClusterAssociatedToScheduleTypeDef,
-    ClusterCredentialsTypeDef,
     RevisionTargetTypeDef,
-    ClusterExtendedCredentialsTypeDef,
     ClusterIamRoleTypeDef,
     ClusterNodeTypeDef,
-    ParameterTypeDef,
-    ClusterParameterGroupNameMessageTypeDef,
+    ParameterOutputTypeDef,
     ClusterParameterStatusTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ClusterSecurityGroupMembershipTypeDef,
     ClusterSnapshotCopyStatusTypeDef,
     DataTransferProgressTypeDef,
     DeferredMaintenanceWindowTypeDef,
     ElasticIpStatusTypeDef,
     HsmStatusTypeDef,
     PendingModifiedValuesTypeDef,
     ReservedNodeExchangeStatusTypeDef,
     ResizeInfoTypeDef,
     RestoreStatusTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ClusterVersionTypeDef,
     CopyClusterSnapshotMessageRequestTypeDef,
     CreateAuthenticationProfileMessageRequestTypeDef,
-    CreateAuthenticationProfileResultTypeDef,
+    TagTypeDef,
     CreateCustomDomainAssociationMessageRequestTypeDef,
-    CreateCustomDomainAssociationResultTypeDef,
     CreateEndpointAccessMessageRequestTypeDef,
-    CustomerStorageMessageTypeDef,
     DataShareAssociationTypeDef,
     DeauthorizeDataShareMessageRequestTypeDef,
     DeleteAuthenticationProfileMessageRequestTypeDef,
-    DeleteAuthenticationProfileResultTypeDef,
     DeleteClusterMessageRequestTypeDef,
     DeleteClusterParameterGroupMessageRequestTypeDef,
     DeleteClusterSecurityGroupMessageRequestTypeDef,
     DeleteClusterSnapshotMessageRequestTypeDef,
     DeleteClusterSubnetGroupMessageRequestTypeDef,
     DeleteCustomDomainAssociationMessageRequestTypeDef,
     DeleteEndpointAccessMessageRequestTypeDef,
@@ -603,202 +598,213 @@
     DeleteScheduledActionMessageRequestTypeDef,
     DeleteSnapshotCopyGrantMessageRequestTypeDef,
     DeleteSnapshotScheduleMessageRequestTypeDef,
     DeleteTagsMessageRequestTypeDef,
     DeleteUsageLimitMessageRequestTypeDef,
     DescribeAccountAttributesMessageRequestTypeDef,
     DescribeAuthenticationProfilesMessageRequestTypeDef,
-    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClusterDbRevisionsMessageRequestTypeDef,
-    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
     DescribeClusterParameterGroupsMessageRequestTypeDef,
-    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
     DescribeClusterParametersMessageRequestTypeDef,
-    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
     DescribeClusterSecurityGroupsMessageRequestTypeDef,
     SnapshotSortingEntityTypeDef,
     WaiterConfigTypeDef,
-    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
     DescribeClusterSubnetGroupsMessageRequestTypeDef,
-    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
     DescribeClusterTracksMessageRequestTypeDef,
-    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
     DescribeClusterVersionsMessageRequestTypeDef,
-    DescribeClustersMessageDescribeClustersPaginateTypeDef,
     DescribeClustersMessageRequestTypeDef,
-    DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef,
     DescribeCustomDomainAssociationsMessageRequestTypeDef,
-    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
     DescribeDataSharesForConsumerMessageRequestTypeDef,
-    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
     DescribeDataSharesForProducerMessageRequestTypeDef,
-    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
     DescribeDataSharesMessageRequestTypeDef,
-    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
     DescribeDefaultClusterParametersMessageRequestTypeDef,
-    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
     DescribeEndpointAccessMessageRequestTypeDef,
-    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
     DescribeEndpointAuthorizationMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
-    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
     DescribeHsmClientCertificatesMessageRequestTypeDef,
-    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
     DescribeHsmConfigurationsMessageRequestTypeDef,
     DescribeLoggingStatusMessageRequestTypeDef,
     NodeConfigurationOptionsFilterTypeDef,
-    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
     DescribeOrderableClusterOptionsMessageRequestTypeDef,
     DescribePartnersInputMessageRequestTypeDef,
     PartnerIntegrationInfoTypeDef,
-    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
     DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef,
-    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
     DescribeReservedNodeOfferingsMessageRequestTypeDef,
-    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
     DescribeReservedNodesMessageRequestTypeDef,
     DescribeResizeMessageRequestTypeDef,
     ScheduledActionFilterTypeDef,
-    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
     DescribeSnapshotCopyGrantsMessageRequestTypeDef,
-    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
     DescribeSnapshotSchedulesMessageRequestTypeDef,
-    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
     DescribeTableRestoreStatusMessageRequestTypeDef,
-    DescribeTagsMessageDescribeTagsPaginateTypeDef,
     DescribeTagsMessageRequestTypeDef,
-    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
     DescribeUsageLimitsMessageRequestTypeDef,
     DisableLoggingMessageRequestTypeDef,
     DisableSnapshotCopyMessageRequestTypeDef,
     DisassociateDataShareConsumerMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableLoggingMessageRequestTypeDef,
     EnableSnapshotCopyMessageRequestTypeDef,
     EndpointAuthorizationTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
     EventInfoMapTypeDef,
     EventTypeDef,
     GetClusterCredentialsMessageRequestTypeDef,
     GetClusterCredentialsWithIAMMessageRequestTypeDef,
-    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
     GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
-    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
-    LoggingStatusTypeDef,
     ModifyAquaInputMessageRequestTypeDef,
     ModifyAuthenticationProfileMessageRequestTypeDef,
-    ModifyAuthenticationProfileResultTypeDef,
     ModifyClusterDbRevisionMessageRequestTypeDef,
     ModifyClusterIamRolesMessageRequestTypeDef,
     ModifyClusterMaintenanceMessageRequestTypeDef,
     ModifyClusterMessageRequestTypeDef,
+    ParameterTypeDef,
     ModifyClusterSnapshotMessageRequestTypeDef,
     ModifyClusterSnapshotScheduleMessageRequestTypeDef,
     ModifyClusterSubnetGroupMessageRequestTypeDef,
     ModifyCustomDomainAssociationMessageRequestTypeDef,
-    ModifyCustomDomainAssociationResultTypeDef,
     ModifyEndpointAccessMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     ModifySnapshotScheduleMessageRequestTypeDef,
     ModifyUsageLimitMessageRequestTypeDef,
     NetworkInterfaceTypeDef,
     NodeConfigurationOptionTypeDef,
-    PaginatorConfigTypeDef,
     PartnerIntegrationInputMessageRequestTypeDef,
-    PartnerIntegrationOutputMessageTypeDef,
+    PauseClusterMessageOutputTypeDef,
     PauseClusterMessageRequestTypeDef,
     PauseClusterMessageTypeDef,
     PurchaseReservedNodeOfferingMessageRequestTypeDef,
     RebootClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RejectDataShareMessageRequestTypeDef,
+    ResizeClusterMessageOutputTypeDef,
     ResizeClusterMessageRequestTypeDef,
     ResizeClusterMessageTypeDef,
-    ResizeProgressMessageTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromClusterSnapshotMessageRequestTypeDef,
     RestoreTableFromClusterSnapshotMessageRequestTypeDef,
     TableRestoreStatusTypeDef,
+    ResumeClusterMessageOutputTypeDef,
     ResumeClusterMessageRequestTypeDef,
     ResumeClusterMessageTypeDef,
     RevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     RevokeEndpointAccessMessageRequestTypeDef,
     RevokeSnapshotAccessMessageRequestTypeDef,
     RotateEncryptionKeyMessageRequestTypeDef,
     SupportedOperationTypeDef,
     UpdatePartnerStatusInputMessageRequestTypeDef,
+    ClusterCredentialsTypeDef,
+    ClusterExtendedCredentialsTypeDef,
+    ClusterParameterGroupNameMessageTypeDef,
+    CreateAuthenticationProfileResultTypeDef,
+    CreateCustomDomainAssociationResultTypeDef,
+    CustomerStorageMessageTypeDef,
+    DeleteAuthenticationProfileResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EndpointAuthorizationResponseMetadataTypeDef,
+    LoggingStatusTypeDef,
+    ModifyAuthenticationProfileResultTypeDef,
+    ModifyCustomDomainAssociationResultTypeDef,
+    PartnerIntegrationOutputMessageTypeDef,
+    ResizeProgressMessageTypeDef,
     AccountAttributeTypeDef,
     ModifyAquaOutputMessageTypeDef,
     AssociationTypeDef,
     DescribeAuthenticationProfilesResultTypeDef,
     AvailabilityZoneTypeDef,
     BatchDeleteClusterSnapshotsRequestRequestTypeDef,
     BatchDeleteClusterSnapshotsResultTypeDef,
     BatchModifyClusterSnapshotsOutputMessageTypeDef,
     ClusterDbRevisionTypeDef,
     ClusterParameterGroupDetailsTypeDef,
     DefaultClusterParametersTypeDef,
-    ModifyClusterParameterGroupMessageRequestTypeDef,
-    ResetClusterParameterGroupMessageRequestTypeDef,
     ClusterParameterGroupStatusTypeDef,
     ClusterParameterGroupTypeDef,
-    CreateClusterMessageRequestTypeDef,
-    CreateClusterParameterGroupMessageRequestTypeDef,
-    CreateClusterSecurityGroupMessageRequestTypeDef,
-    CreateClusterSnapshotMessageRequestTypeDef,
-    CreateClusterSubnetGroupMessageRequestTypeDef,
-    CreateEventSubscriptionMessageRequestTypeDef,
-    CreateHsmClientCertificateMessageRequestTypeDef,
-    CreateHsmConfigurationMessageRequestTypeDef,
-    CreateSnapshotCopyGrantMessageRequestTypeDef,
-    CreateSnapshotScheduleMessageRequestTypeDef,
-    CreateTagsMessageRequestTypeDef,
-    CreateUsageLimitMessageRequestTypeDef,
     EC2SecurityGroupTypeDef,
     EventSubscriptionTypeDef,
     HsmClientCertificateTypeDef,
     HsmConfigurationTypeDef,
     IPRangeTypeDef,
     SnapshotCopyGrantTypeDef,
     SnapshotScheduleResponseMetadataTypeDef,
     SnapshotScheduleTypeDef,
     SnapshotTypeDef,
     TaggedResourceTypeDef,
     UsageLimitResponseMetadataTypeDef,
     UsageLimitTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     ClusterVersionsMessageTypeDef,
+    CreateClusterMessageRequestTypeDef,
+    CreateClusterParameterGroupMessageRequestTypeDef,
+    CreateClusterSecurityGroupMessageRequestTypeDef,
+    CreateClusterSnapshotMessageRequestTypeDef,
+    CreateClusterSubnetGroupMessageRequestTypeDef,
+    CreateEventSubscriptionMessageRequestTypeDef,
+    CreateHsmClientCertificateMessageRequestTypeDef,
+    CreateHsmConfigurationMessageRequestTypeDef,
+    CreateSnapshotCopyGrantMessageRequestTypeDef,
+    CreateSnapshotScheduleMessageRequestTypeDef,
+    CreateTagsMessageRequestTypeDef,
+    CreateUsageLimitMessageRequestTypeDef,
     DataShareResponseMetadataTypeDef,
     DataShareTypeDef,
+    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
+    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
+    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
+    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
+    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
+    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
+    DescribeClustersMessageDescribeClustersPaginateTypeDef,
+    DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef,
+    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
+    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
+    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
+    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
+    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
+    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
+    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
+    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
+    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
+    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
+    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
+    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
+    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
+    DescribeTagsMessageDescribeTagsPaginateTypeDef,
+    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
+    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef,
     DescribeClusterSnapshotsMessageRequestTypeDef,
     DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef,
     DescribeClustersMessageClusterAvailableWaitTypeDef,
     DescribeClustersMessageClusterDeletedWaitTypeDef,
     DescribeClustersMessageClusterRestoredWaitTypeDef,
     DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
     DescribeNodeConfigurationOptionsMessageRequestTypeDef,
     DescribePartnersOutputMessageTypeDef,
     DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsMessageRequestTypeDef,
     EndpointAuthorizationListTypeDef,
     EventCategoriesMapTypeDef,
     EventsMessageTypeDef,
+    ModifyClusterParameterGroupMessageRequestTypeDef,
+    ResetClusterParameterGroupMessageRequestTypeDef,
     VpcEndpointTypeDef,
     NodeConfigurationOptionsMessageTypeDef,
     ReservedNodeOfferingTypeDef,
     ReservedNodeTypeDef,
     RestoreTableFromClusterSnapshotResultTypeDef,
     TableRestoreStatusMessageTypeDef,
+    ScheduledActionTypeOutputTypeDef,
     ScheduledActionTypeTypeDef,
     UpdateTargetTypeDef,
     AccountAttributeListTypeDef,
     CustomDomainAssociationsMessageTypeDef,
     OrderableClusterOptionTypeDef,
     SubnetTypeDef,
     ClusterDbRevisionsMessageTypeDef,
@@ -834,18 +840,18 @@
     EndpointTypeDef,
     GetReservedNodeExchangeOfferingsOutputMessageTypeDef,
     ReservedNodeOfferingsMessageTypeDef,
     AcceptReservedNodeExchangeOutputMessageTypeDef,
     PurchaseReservedNodeOfferingResultTypeDef,
     ReservedNodeConfigurationOptionTypeDef,
     ReservedNodesMessageTypeDef,
-    CreateScheduledActionMessageRequestTypeDef,
-    ModifyScheduledActionMessageRequestTypeDef,
     ScheduledActionResponseMetadataTypeDef,
     ScheduledActionTypeDef,
+    CreateScheduledActionMessageRequestTypeDef,
+    ModifyScheduledActionMessageRequestTypeDef,
     MaintenanceTrackTypeDef,
     OrderableClusterOptionsMessageTypeDef,
     ClusterSubnetGroupTypeDef,
     AuthorizeClusterSecurityGroupIngressResultTypeDef,
     ClusterSecurityGroupMessageTypeDef,
     CreateClusterSecurityGroupResultTypeDef,
     RevokeClusterSecurityGroupIngressResultTypeDef,
```

### Comparing `mypy-boto3-redshift-1.28.0/README.md` & `mypy-boto3-redshift-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-redshift"></a>
 
 # mypy-boto3-redshift
 
 [![PyPI - mypy-boto3-redshift](https://img.shields.io/pypi/v/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift)](https://pepy.tech/project/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
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
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -506,14 +506,15 @@
 
 `mypy_boto3_redshift.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift.type_defs import (
     AcceptReservedNodeExchangeInputMessageRequestTypeDef,
+    ResponseMetadataTypeDef,
     AttributeValueTargetTypeDef,
     AccountWithRestoreAccessTypeDef,
     AquaConfigurationTypeDef,
     AssociateDataShareConsumerMessageRequestTypeDef,
     CertificateAssociationTypeDef,
     AuthenticationProfileTypeDef,
     AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
@@ -522,46 +523,40 @@
     AuthorizeSnapshotAccessMessageRequestTypeDef,
     SupportedPlatformTypeDef,
     DeleteClusterSnapshotMessageTypeDef,
     SnapshotErrorMessageTypeDef,
     BatchModifyClusterSnapshotsMessageRequestTypeDef,
     CancelResizeMessageRequestTypeDef,
     ClusterAssociatedToScheduleTypeDef,
-    ClusterCredentialsTypeDef,
     RevisionTargetTypeDef,
-    ClusterExtendedCredentialsTypeDef,
     ClusterIamRoleTypeDef,
     ClusterNodeTypeDef,
-    ParameterTypeDef,
-    ClusterParameterGroupNameMessageTypeDef,
+    ParameterOutputTypeDef,
     ClusterParameterStatusTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ClusterSecurityGroupMembershipTypeDef,
     ClusterSnapshotCopyStatusTypeDef,
     DataTransferProgressTypeDef,
     DeferredMaintenanceWindowTypeDef,
     ElasticIpStatusTypeDef,
     HsmStatusTypeDef,
     PendingModifiedValuesTypeDef,
     ReservedNodeExchangeStatusTypeDef,
     ResizeInfoTypeDef,
     RestoreStatusTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ClusterVersionTypeDef,
     CopyClusterSnapshotMessageRequestTypeDef,
     CreateAuthenticationProfileMessageRequestTypeDef,
-    CreateAuthenticationProfileResultTypeDef,
+    TagTypeDef,
     CreateCustomDomainAssociationMessageRequestTypeDef,
-    CreateCustomDomainAssociationResultTypeDef,
     CreateEndpointAccessMessageRequestTypeDef,
-    CustomerStorageMessageTypeDef,
     DataShareAssociationTypeDef,
     DeauthorizeDataShareMessageRequestTypeDef,
     DeleteAuthenticationProfileMessageRequestTypeDef,
-    DeleteAuthenticationProfileResultTypeDef,
     DeleteClusterMessageRequestTypeDef,
     DeleteClusterParameterGroupMessageRequestTypeDef,
     DeleteClusterSecurityGroupMessageRequestTypeDef,
     DeleteClusterSnapshotMessageRequestTypeDef,
     DeleteClusterSubnetGroupMessageRequestTypeDef,
     DeleteCustomDomainAssociationMessageRequestTypeDef,
     DeleteEndpointAccessMessageRequestTypeDef,
@@ -571,202 +566,213 @@
     DeleteScheduledActionMessageRequestTypeDef,
     DeleteSnapshotCopyGrantMessageRequestTypeDef,
     DeleteSnapshotScheduleMessageRequestTypeDef,
     DeleteTagsMessageRequestTypeDef,
     DeleteUsageLimitMessageRequestTypeDef,
     DescribeAccountAttributesMessageRequestTypeDef,
     DescribeAuthenticationProfilesMessageRequestTypeDef,
-    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClusterDbRevisionsMessageRequestTypeDef,
-    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
     DescribeClusterParameterGroupsMessageRequestTypeDef,
-    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
     DescribeClusterParametersMessageRequestTypeDef,
-    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
     DescribeClusterSecurityGroupsMessageRequestTypeDef,
     SnapshotSortingEntityTypeDef,
     WaiterConfigTypeDef,
-    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
     DescribeClusterSubnetGroupsMessageRequestTypeDef,
-    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
     DescribeClusterTracksMessageRequestTypeDef,
-    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
     DescribeClusterVersionsMessageRequestTypeDef,
-    DescribeClustersMessageDescribeClustersPaginateTypeDef,
     DescribeClustersMessageRequestTypeDef,
-    DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef,
     DescribeCustomDomainAssociationsMessageRequestTypeDef,
-    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
     DescribeDataSharesForConsumerMessageRequestTypeDef,
-    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
     DescribeDataSharesForProducerMessageRequestTypeDef,
-    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
     DescribeDataSharesMessageRequestTypeDef,
-    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
     DescribeDefaultClusterParametersMessageRequestTypeDef,
-    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
     DescribeEndpointAccessMessageRequestTypeDef,
-    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
     DescribeEndpointAuthorizationMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
-    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
     DescribeHsmClientCertificatesMessageRequestTypeDef,
-    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
     DescribeHsmConfigurationsMessageRequestTypeDef,
     DescribeLoggingStatusMessageRequestTypeDef,
     NodeConfigurationOptionsFilterTypeDef,
-    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
     DescribeOrderableClusterOptionsMessageRequestTypeDef,
     DescribePartnersInputMessageRequestTypeDef,
     PartnerIntegrationInfoTypeDef,
-    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
     DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef,
-    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
     DescribeReservedNodeOfferingsMessageRequestTypeDef,
-    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
     DescribeReservedNodesMessageRequestTypeDef,
     DescribeResizeMessageRequestTypeDef,
     ScheduledActionFilterTypeDef,
-    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
     DescribeSnapshotCopyGrantsMessageRequestTypeDef,
-    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
     DescribeSnapshotSchedulesMessageRequestTypeDef,
-    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
     DescribeTableRestoreStatusMessageRequestTypeDef,
-    DescribeTagsMessageDescribeTagsPaginateTypeDef,
     DescribeTagsMessageRequestTypeDef,
-    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
     DescribeUsageLimitsMessageRequestTypeDef,
     DisableLoggingMessageRequestTypeDef,
     DisableSnapshotCopyMessageRequestTypeDef,
     DisassociateDataShareConsumerMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableLoggingMessageRequestTypeDef,
     EnableSnapshotCopyMessageRequestTypeDef,
     EndpointAuthorizationTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
     EventInfoMapTypeDef,
     EventTypeDef,
     GetClusterCredentialsMessageRequestTypeDef,
     GetClusterCredentialsWithIAMMessageRequestTypeDef,
-    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
     GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
-    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
-    LoggingStatusTypeDef,
     ModifyAquaInputMessageRequestTypeDef,
     ModifyAuthenticationProfileMessageRequestTypeDef,
-    ModifyAuthenticationProfileResultTypeDef,
     ModifyClusterDbRevisionMessageRequestTypeDef,
     ModifyClusterIamRolesMessageRequestTypeDef,
     ModifyClusterMaintenanceMessageRequestTypeDef,
     ModifyClusterMessageRequestTypeDef,
+    ParameterTypeDef,
     ModifyClusterSnapshotMessageRequestTypeDef,
     ModifyClusterSnapshotScheduleMessageRequestTypeDef,
     ModifyClusterSubnetGroupMessageRequestTypeDef,
     ModifyCustomDomainAssociationMessageRequestTypeDef,
-    ModifyCustomDomainAssociationResultTypeDef,
     ModifyEndpointAccessMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     ModifySnapshotScheduleMessageRequestTypeDef,
     ModifyUsageLimitMessageRequestTypeDef,
     NetworkInterfaceTypeDef,
     NodeConfigurationOptionTypeDef,
-    PaginatorConfigTypeDef,
     PartnerIntegrationInputMessageRequestTypeDef,
-    PartnerIntegrationOutputMessageTypeDef,
+    PauseClusterMessageOutputTypeDef,
     PauseClusterMessageRequestTypeDef,
     PauseClusterMessageTypeDef,
     PurchaseReservedNodeOfferingMessageRequestTypeDef,
     RebootClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RejectDataShareMessageRequestTypeDef,
+    ResizeClusterMessageOutputTypeDef,
     ResizeClusterMessageRequestTypeDef,
     ResizeClusterMessageTypeDef,
-    ResizeProgressMessageTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromClusterSnapshotMessageRequestTypeDef,
     RestoreTableFromClusterSnapshotMessageRequestTypeDef,
     TableRestoreStatusTypeDef,
+    ResumeClusterMessageOutputTypeDef,
     ResumeClusterMessageRequestTypeDef,
     ResumeClusterMessageTypeDef,
     RevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     RevokeEndpointAccessMessageRequestTypeDef,
     RevokeSnapshotAccessMessageRequestTypeDef,
     RotateEncryptionKeyMessageRequestTypeDef,
     SupportedOperationTypeDef,
     UpdatePartnerStatusInputMessageRequestTypeDef,
+    ClusterCredentialsTypeDef,
+    ClusterExtendedCredentialsTypeDef,
+    ClusterParameterGroupNameMessageTypeDef,
+    CreateAuthenticationProfileResultTypeDef,
+    CreateCustomDomainAssociationResultTypeDef,
+    CustomerStorageMessageTypeDef,
+    DeleteAuthenticationProfileResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EndpointAuthorizationResponseMetadataTypeDef,
+    LoggingStatusTypeDef,
+    ModifyAuthenticationProfileResultTypeDef,
+    ModifyCustomDomainAssociationResultTypeDef,
+    PartnerIntegrationOutputMessageTypeDef,
+    ResizeProgressMessageTypeDef,
     AccountAttributeTypeDef,
     ModifyAquaOutputMessageTypeDef,
     AssociationTypeDef,
     DescribeAuthenticationProfilesResultTypeDef,
     AvailabilityZoneTypeDef,
     BatchDeleteClusterSnapshotsRequestRequestTypeDef,
     BatchDeleteClusterSnapshotsResultTypeDef,
     BatchModifyClusterSnapshotsOutputMessageTypeDef,
     ClusterDbRevisionTypeDef,
     ClusterParameterGroupDetailsTypeDef,
     DefaultClusterParametersTypeDef,
-    ModifyClusterParameterGroupMessageRequestTypeDef,
-    ResetClusterParameterGroupMessageRequestTypeDef,
     ClusterParameterGroupStatusTypeDef,
     ClusterParameterGroupTypeDef,
-    CreateClusterMessageRequestTypeDef,
-    CreateClusterParameterGroupMessageRequestTypeDef,
-    CreateClusterSecurityGroupMessageRequestTypeDef,
-    CreateClusterSnapshotMessageRequestTypeDef,
-    CreateClusterSubnetGroupMessageRequestTypeDef,
-    CreateEventSubscriptionMessageRequestTypeDef,
-    CreateHsmClientCertificateMessageRequestTypeDef,
-    CreateHsmConfigurationMessageRequestTypeDef,
-    CreateSnapshotCopyGrantMessageRequestTypeDef,
-    CreateSnapshotScheduleMessageRequestTypeDef,
-    CreateTagsMessageRequestTypeDef,
-    CreateUsageLimitMessageRequestTypeDef,
     EC2SecurityGroupTypeDef,
     EventSubscriptionTypeDef,
     HsmClientCertificateTypeDef,
     HsmConfigurationTypeDef,
     IPRangeTypeDef,
     SnapshotCopyGrantTypeDef,
     SnapshotScheduleResponseMetadataTypeDef,
     SnapshotScheduleTypeDef,
     SnapshotTypeDef,
     TaggedResourceTypeDef,
     UsageLimitResponseMetadataTypeDef,
     UsageLimitTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     ClusterVersionsMessageTypeDef,
+    CreateClusterMessageRequestTypeDef,
+    CreateClusterParameterGroupMessageRequestTypeDef,
+    CreateClusterSecurityGroupMessageRequestTypeDef,
+    CreateClusterSnapshotMessageRequestTypeDef,
+    CreateClusterSubnetGroupMessageRequestTypeDef,
+    CreateEventSubscriptionMessageRequestTypeDef,
+    CreateHsmClientCertificateMessageRequestTypeDef,
+    CreateHsmConfigurationMessageRequestTypeDef,
+    CreateSnapshotCopyGrantMessageRequestTypeDef,
+    CreateSnapshotScheduleMessageRequestTypeDef,
+    CreateTagsMessageRequestTypeDef,
+    CreateUsageLimitMessageRequestTypeDef,
     DataShareResponseMetadataTypeDef,
     DataShareTypeDef,
+    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
+    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
+    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
+    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
+    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
+    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
+    DescribeClustersMessageDescribeClustersPaginateTypeDef,
+    DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef,
+    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
+    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
+    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
+    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
+    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
+    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
+    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
+    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
+    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
+    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
+    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
+    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
+    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
+    DescribeTagsMessageDescribeTagsPaginateTypeDef,
+    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
+    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef,
     DescribeClusterSnapshotsMessageRequestTypeDef,
     DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef,
     DescribeClustersMessageClusterAvailableWaitTypeDef,
     DescribeClustersMessageClusterDeletedWaitTypeDef,
     DescribeClustersMessageClusterRestoredWaitTypeDef,
     DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
     DescribeNodeConfigurationOptionsMessageRequestTypeDef,
     DescribePartnersOutputMessageTypeDef,
     DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsMessageRequestTypeDef,
     EndpointAuthorizationListTypeDef,
     EventCategoriesMapTypeDef,
     EventsMessageTypeDef,
+    ModifyClusterParameterGroupMessageRequestTypeDef,
+    ResetClusterParameterGroupMessageRequestTypeDef,
     VpcEndpointTypeDef,
     NodeConfigurationOptionsMessageTypeDef,
     ReservedNodeOfferingTypeDef,
     ReservedNodeTypeDef,
     RestoreTableFromClusterSnapshotResultTypeDef,
     TableRestoreStatusMessageTypeDef,
+    ScheduledActionTypeOutputTypeDef,
     ScheduledActionTypeTypeDef,
     UpdateTargetTypeDef,
     AccountAttributeListTypeDef,
     CustomDomainAssociationsMessageTypeDef,
     OrderableClusterOptionTypeDef,
     SubnetTypeDef,
     ClusterDbRevisionsMessageTypeDef,
@@ -802,18 +808,18 @@
     EndpointTypeDef,
     GetReservedNodeExchangeOfferingsOutputMessageTypeDef,
     ReservedNodeOfferingsMessageTypeDef,
     AcceptReservedNodeExchangeOutputMessageTypeDef,
     PurchaseReservedNodeOfferingResultTypeDef,
     ReservedNodeConfigurationOptionTypeDef,
     ReservedNodesMessageTypeDef,
-    CreateScheduledActionMessageRequestTypeDef,
-    ModifyScheduledActionMessageRequestTypeDef,
     ScheduledActionResponseMetadataTypeDef,
     ScheduledActionTypeDef,
+    CreateScheduledActionMessageRequestTypeDef,
+    ModifyScheduledActionMessageRequestTypeDef,
     MaintenanceTrackTypeDef,
     OrderableClusterOptionsMessageTypeDef,
     ClusterSubnetGroupTypeDef,
     AuthorizeClusterSecurityGroupIngressResultTypeDef,
     ClusterSecurityGroupMessageTypeDef,
     CreateClusterSecurityGroupResultTypeDef,
     RevokeClusterSecurityGroupIngressResultTypeDef,
```

### Comparing `mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/__init__.py` & `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/__init__.pyi` & `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/__main__.py` & `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Redshift 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Redshift 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift\nOther"
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

### Comparing `mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/client.py` & `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/client.pyi` & `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/literals.py` & `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,14 +291,15 @@
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
@@ -377,26 +378,28 @@
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

### Comparing `mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/literals.pyi` & `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -289,14 +289,15 @@
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
@@ -375,26 +376,28 @@
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

### Comparing `mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/paginator.py` & `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 class DescribeClusterDbRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterDbRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterdbrevisionspaginator)
     """
 
     def paginate(
-        self, *, ClusterIdentifier: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterIdentifier: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ClusterDbRevisionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterDbRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterdbrevisionspaginator)
         """
 
 
@@ -207,15 +207,15 @@
 
     def paginate(
         self,
         *,
         ParameterGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterparametergroupspaginator)
         """
 
 
@@ -226,15 +226,15 @@
     """
 
     def paginate(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterparameterspaginator)
         """
 
 
@@ -246,15 +246,15 @@
 
     def paginate(
         self,
         *,
         ClusterSecurityGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ClusterSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustersecuritygroupspaginator)
         """
 
 
@@ -274,15 +274,15 @@
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustersnapshotspaginator)
         """
 
 
@@ -294,30 +294,30 @@
 
     def paginate(
         self,
         *,
         ClusterSubnetGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ClusterSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustersubnetgroupspaginator)
         """
 
 
 class DescribeClusterTracksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterTracks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustertrackspaginator)
     """
 
     def paginate(
-        self, *, MaintenanceTrackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, MaintenanceTrackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[TrackListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterTracks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustertrackspaginator)
         """
 
 
@@ -328,15 +328,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         ClusterParameterGroupFamily: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ClusterVersionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterversionspaginator)
         """
 
 
@@ -348,15 +348,15 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterspaginator)
         """
 
 
@@ -367,30 +367,30 @@
     """
 
     def paginate(
         self,
         *,
         CustomDomainName: str = ...,
         CustomDomainCertificateArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CustomDomainAssociationsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeCustomDomainAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describecustomdomainassociationspaginator)
         """
 
 
 class DescribeDataSharesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataShares)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharespaginator)
     """
 
     def paginate(
-        self, *, DataShareArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DataShareArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDataSharesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharespaginator)
         """
 
 
@@ -401,15 +401,15 @@
     """
 
     def paginate(
         self,
         *,
         ConsumerArn: str = ...,
         Status: DataShareStatusForConsumerType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDataSharesForConsumerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForConsumer.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharesforconsumerpaginator)
         """
 
 
@@ -420,30 +420,30 @@
     """
 
     def paginate(
         self,
         *,
         ProducerArn: str = ...,
         Status: DataShareStatusForProducerType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDataSharesForProducerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForProducer.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharesforproducerpaginator)
         """
 
 
 class DescribeDefaultClusterParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDefaultClusterParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedefaultclusterparameterspaginator)
     """
 
     def paginate(
-        self, *, ParameterGroupFamily: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ParameterGroupFamily: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDefaultClusterParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDefaultClusterParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedefaultclusterparameterspaginator)
         """
 
 
@@ -456,15 +456,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         EndpointName: str = ...,
         VpcId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EndpointAccessListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAccess.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeendpointaccesspaginator)
         """
 
 
@@ -476,15 +476,15 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         Grantee: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EndpointAuthorizationListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAuthorization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeendpointauthorizationpaginator)
         """
 
 
@@ -496,15 +496,15 @@
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeeventsubscriptionspaginator)
         """
 
 
@@ -518,15 +518,15 @@
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeeventspaginator)
         """
 
 
@@ -538,15 +538,15 @@
 
     def paginate(
         self,
         *,
         HsmClientCertificateIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[HsmClientCertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmClientCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describehsmclientcertificatespaginator)
         """
 
 
@@ -558,15 +558,15 @@
 
     def paginate(
         self,
         *,
         HsmConfigurationIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[HsmConfigurationMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describehsmconfigurationspaginator)
         """
 
 
@@ -581,15 +581,15 @@
         *,
         ActionType: ActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         OwnerAccount: str = ...,
         Filters: Sequence[NodeConfigurationOptionsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[NodeConfigurationOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeNodeConfigurationOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describenodeconfigurationoptionspaginator)
         """
 
 
@@ -600,15 +600,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         NodeType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[OrderableClusterOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeOrderableClusterOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeorderableclusteroptionspaginator)
         """
 
 
@@ -619,45 +619,45 @@
     """
 
     def paginate(
         self,
         *,
         ReservedNodeId: str = ...,
         ReservedNodeExchangeRequestId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeReservedNodeExchangeStatusOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeExchangeStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodeexchangestatuspaginator)
         """
 
 
 class DescribeReservedNodeOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodeofferingspaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeOfferingId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReservedNodeOfferingId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ReservedNodeOfferingsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodeofferingspaginator)
         """
 
 
 class DescribeReservedNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodespaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReservedNodeId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ReservedNodesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodespaginator)
         """
 
 
@@ -672,15 +672,15 @@
         *,
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ScheduledActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describescheduledactionspaginator)
         """
 
 
@@ -692,15 +692,15 @@
 
     def paginate(
         self,
         *,
         SnapshotCopyGrantName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SnapshotCopyGrantMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotCopyGrants.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describesnapshotcopygrantspaginator)
         """
 
 
@@ -713,15 +713,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ScheduleIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSnapshotSchedulesOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describesnapshotschedulespaginator)
         """
 
 
@@ -732,15 +732,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TableRestoreRequestId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[TableRestoreStatusMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTableRestoreStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describetablerestorestatuspaginator)
         """
 
 
@@ -753,15 +753,15 @@
     def paginate(
         self,
         *,
         ResourceName: str = ...,
         ResourceType: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[TaggedResourceListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describetagspaginator)
         """
 
 
@@ -775,15 +775,15 @@
         self,
         *,
         UsageLimitId: str = ...,
         ClusterIdentifier: str = ...,
         FeatureType: UsageLimitFeatureTypeType = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[UsageLimitListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeUsageLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeusagelimitspaginator)
         """
 
 
@@ -795,28 +795,28 @@
 
     def paginate(
         self,
         *,
         ActionType: ReservedNodeExchangeActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeConfigurationOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#getreservednodeexchangeconfigurationoptionspaginator)
         """
 
 
 class GetReservedNodeExchangeOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#getreservednodeexchangeofferingspaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReservedNodeId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetReservedNodeExchangeOfferingsOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#getreservednodeexchangeofferingspaginator)
         """
```

### Comparing `mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/paginator.pyi` & `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 class DescribeClusterDbRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterDbRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterdbrevisionspaginator)
     """
 
     def paginate(
-        self, *, ClusterIdentifier: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterIdentifier: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ClusterDbRevisionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterDbRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterdbrevisionspaginator)
         """
 
 class DescribeClusterParameterGroupsPaginator(Paginator):
@@ -203,15 +203,15 @@
 
     def paginate(
         self,
         *,
         ParameterGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterparametergroupspaginator)
         """
 
 class DescribeClusterParametersPaginator(Paginator):
@@ -221,15 +221,15 @@
     """
 
     def paginate(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterparameterspaginator)
         """
 
 class DescribeClusterSecurityGroupsPaginator(Paginator):
@@ -240,15 +240,15 @@
 
     def paginate(
         self,
         *,
         ClusterSecurityGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ClusterSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustersecuritygroupspaginator)
         """
 
 class DescribeClusterSnapshotsPaginator(Paginator):
@@ -267,15 +267,15 @@
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustersnapshotspaginator)
         """
 
 class DescribeClusterSubnetGroupsPaginator(Paginator):
@@ -286,29 +286,29 @@
 
     def paginate(
         self,
         *,
         ClusterSubnetGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ClusterSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustersubnetgroupspaginator)
         """
 
 class DescribeClusterTracksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterTracks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustertrackspaginator)
     """
 
     def paginate(
-        self, *, MaintenanceTrackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, MaintenanceTrackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[TrackListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterTracks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustertrackspaginator)
         """
 
 class DescribeClusterVersionsPaginator(Paginator):
@@ -318,15 +318,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         ClusterParameterGroupFamily: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ClusterVersionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterversionspaginator)
         """
 
 class DescribeClustersPaginator(Paginator):
@@ -337,15 +337,15 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterspaginator)
         """
 
 class DescribeCustomDomainAssociationsPaginator(Paginator):
@@ -355,29 +355,29 @@
     """
 
     def paginate(
         self,
         *,
         CustomDomainName: str = ...,
         CustomDomainCertificateArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CustomDomainAssociationsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeCustomDomainAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describecustomdomainassociationspaginator)
         """
 
 class DescribeDataSharesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataShares)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharespaginator)
     """
 
     def paginate(
-        self, *, DataShareArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DataShareArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDataSharesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharespaginator)
         """
 
 class DescribeDataSharesForConsumerPaginator(Paginator):
@@ -387,15 +387,15 @@
     """
 
     def paginate(
         self,
         *,
         ConsumerArn: str = ...,
         Status: DataShareStatusForConsumerType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDataSharesForConsumerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForConsumer.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharesforconsumerpaginator)
         """
 
 class DescribeDataSharesForProducerPaginator(Paginator):
@@ -405,29 +405,29 @@
     """
 
     def paginate(
         self,
         *,
         ProducerArn: str = ...,
         Status: DataShareStatusForProducerType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDataSharesForProducerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForProducer.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharesforproducerpaginator)
         """
 
 class DescribeDefaultClusterParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDefaultClusterParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedefaultclusterparameterspaginator)
     """
 
     def paginate(
-        self, *, ParameterGroupFamily: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ParameterGroupFamily: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDefaultClusterParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDefaultClusterParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedefaultclusterparameterspaginator)
         """
 
 class DescribeEndpointAccessPaginator(Paginator):
@@ -439,15 +439,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         EndpointName: str = ...,
         VpcId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EndpointAccessListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAccess.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeendpointaccesspaginator)
         """
 
 class DescribeEndpointAuthorizationPaginator(Paginator):
@@ -458,15 +458,15 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         Grantee: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EndpointAuthorizationListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAuthorization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeendpointauthorizationpaginator)
         """
 
 class DescribeEventSubscriptionsPaginator(Paginator):
@@ -477,15 +477,15 @@
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeeventsubscriptionspaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
@@ -498,15 +498,15 @@
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeeventspaginator)
         """
 
 class DescribeHsmClientCertificatesPaginator(Paginator):
@@ -517,15 +517,15 @@
 
     def paginate(
         self,
         *,
         HsmClientCertificateIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[HsmClientCertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmClientCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describehsmclientcertificatespaginator)
         """
 
 class DescribeHsmConfigurationsPaginator(Paginator):
@@ -536,15 +536,15 @@
 
     def paginate(
         self,
         *,
         HsmConfigurationIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[HsmConfigurationMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describehsmconfigurationspaginator)
         """
 
 class DescribeNodeConfigurationOptionsPaginator(Paginator):
@@ -558,15 +558,15 @@
         *,
         ActionType: ActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         OwnerAccount: str = ...,
         Filters: Sequence[NodeConfigurationOptionsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[NodeConfigurationOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeNodeConfigurationOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describenodeconfigurationoptionspaginator)
         """
 
 class DescribeOrderableClusterOptionsPaginator(Paginator):
@@ -576,15 +576,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         NodeType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[OrderableClusterOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeOrderableClusterOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeorderableclusteroptionspaginator)
         """
 
 class DescribeReservedNodeExchangeStatusPaginator(Paginator):
@@ -594,43 +594,43 @@
     """
 
     def paginate(
         self,
         *,
         ReservedNodeId: str = ...,
         ReservedNodeExchangeRequestId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeReservedNodeExchangeStatusOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeExchangeStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodeexchangestatuspaginator)
         """
 
 class DescribeReservedNodeOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodeofferingspaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeOfferingId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReservedNodeOfferingId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ReservedNodeOfferingsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodeofferingspaginator)
         """
 
 class DescribeReservedNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodespaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReservedNodeId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ReservedNodesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodespaginator)
         """
 
 class DescribeScheduledActionsPaginator(Paginator):
@@ -644,15 +644,15 @@
         *,
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ScheduledActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describescheduledactionspaginator)
         """
 
 class DescribeSnapshotCopyGrantsPaginator(Paginator):
@@ -663,15 +663,15 @@
 
     def paginate(
         self,
         *,
         SnapshotCopyGrantName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SnapshotCopyGrantMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotCopyGrants.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describesnapshotcopygrantspaginator)
         """
 
 class DescribeSnapshotSchedulesPaginator(Paginator):
@@ -683,15 +683,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ScheduleIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSnapshotSchedulesOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describesnapshotschedulespaginator)
         """
 
 class DescribeTableRestoreStatusPaginator(Paginator):
@@ -701,15 +701,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TableRestoreRequestId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[TableRestoreStatusMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTableRestoreStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describetablerestorestatuspaginator)
         """
 
 class DescribeTagsPaginator(Paginator):
@@ -721,15 +721,15 @@
     def paginate(
         self,
         *,
         ResourceName: str = ...,
         ResourceType: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[TaggedResourceListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describetagspaginator)
         """
 
 class DescribeUsageLimitsPaginator(Paginator):
@@ -742,15 +742,15 @@
         self,
         *,
         UsageLimitId: str = ...,
         ClusterIdentifier: str = ...,
         FeatureType: UsageLimitFeatureTypeType = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[UsageLimitListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeUsageLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeusagelimitspaginator)
         """
 
 class GetReservedNodeExchangeConfigurationOptionsPaginator(Paginator):
@@ -761,27 +761,27 @@
 
     def paginate(
         self,
         *,
         ActionType: ReservedNodeExchangeActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeConfigurationOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#getreservednodeexchangeconfigurationoptionspaginator)
         """
 
 class GetReservedNodeExchangeOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#getreservednodeexchangeofferingspaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReservedNodeId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetReservedNodeExchangeOfferingsOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#getreservednodeexchangeofferingspaginator)
         """
```

### Comparing `mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/type_defs.py` & `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -47,17 +47,17 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptReservedNodeExchangeInputMessageRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AttributeValueTargetTypeDef",
     "AccountWithRestoreAccessTypeDef",
     "AquaConfigurationTypeDef",
     "AssociateDataShareConsumerMessageRequestTypeDef",
     "CertificateAssociationTypeDef",
     "AuthenticationProfileTypeDef",
     "AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef",
@@ -66,46 +66,40 @@
     "AuthorizeSnapshotAccessMessageRequestTypeDef",
     "SupportedPlatformTypeDef",
     "DeleteClusterSnapshotMessageTypeDef",
     "SnapshotErrorMessageTypeDef",
     "BatchModifyClusterSnapshotsMessageRequestTypeDef",
     "CancelResizeMessageRequestTypeDef",
     "ClusterAssociatedToScheduleTypeDef",
-    "ClusterCredentialsTypeDef",
     "RevisionTargetTypeDef",
-    "ClusterExtendedCredentialsTypeDef",
     "ClusterIamRoleTypeDef",
     "ClusterNodeTypeDef",
-    "ParameterTypeDef",
-    "ClusterParameterGroupNameMessageTypeDef",
+    "ParameterOutputTypeDef",
     "ClusterParameterStatusTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "ClusterSecurityGroupMembershipTypeDef",
     "ClusterSnapshotCopyStatusTypeDef",
     "DataTransferProgressTypeDef",
     "DeferredMaintenanceWindowTypeDef",
     "ElasticIpStatusTypeDef",
     "HsmStatusTypeDef",
     "PendingModifiedValuesTypeDef",
     "ReservedNodeExchangeStatusTypeDef",
     "ResizeInfoTypeDef",
     "RestoreStatusTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ClusterVersionTypeDef",
     "CopyClusterSnapshotMessageRequestTypeDef",
     "CreateAuthenticationProfileMessageRequestTypeDef",
-    "CreateAuthenticationProfileResultTypeDef",
+    "TagTypeDef",
     "CreateCustomDomainAssociationMessageRequestTypeDef",
-    "CreateCustomDomainAssociationResultTypeDef",
     "CreateEndpointAccessMessageRequestTypeDef",
-    "CustomerStorageMessageTypeDef",
     "DataShareAssociationTypeDef",
     "DeauthorizeDataShareMessageRequestTypeDef",
     "DeleteAuthenticationProfileMessageRequestTypeDef",
-    "DeleteAuthenticationProfileResultTypeDef",
     "DeleteClusterMessageRequestTypeDef",
     "DeleteClusterParameterGroupMessageRequestTypeDef",
     "DeleteClusterSecurityGroupMessageRequestTypeDef",
     "DeleteClusterSnapshotMessageRequestTypeDef",
     "DeleteClusterSubnetGroupMessageRequestTypeDef",
     "DeleteCustomDomainAssociationMessageRequestTypeDef",
     "DeleteEndpointAccessMessageRequestTypeDef",
@@ -115,202 +109,213 @@
     "DeleteScheduledActionMessageRequestTypeDef",
     "DeleteSnapshotCopyGrantMessageRequestTypeDef",
     "DeleteSnapshotScheduleMessageRequestTypeDef",
     "DeleteTagsMessageRequestTypeDef",
     "DeleteUsageLimitMessageRequestTypeDef",
     "DescribeAccountAttributesMessageRequestTypeDef",
     "DescribeAuthenticationProfilesMessageRequestTypeDef",
-    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeClusterDbRevisionsMessageRequestTypeDef",
-    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
     "DescribeClusterParameterGroupsMessageRequestTypeDef",
-    "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
     "DescribeClusterParametersMessageRequestTypeDef",
-    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
     "DescribeClusterSecurityGroupsMessageRequestTypeDef",
     "SnapshotSortingEntityTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
     "DescribeClusterSubnetGroupsMessageRequestTypeDef",
-    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
     "DescribeClusterTracksMessageRequestTypeDef",
-    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
     "DescribeClusterVersionsMessageRequestTypeDef",
-    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
     "DescribeClustersMessageRequestTypeDef",
-    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
     "DescribeCustomDomainAssociationsMessageRequestTypeDef",
-    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
     "DescribeDataSharesForConsumerMessageRequestTypeDef",
-    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
     "DescribeDataSharesForProducerMessageRequestTypeDef",
-    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
     "DescribeDataSharesMessageRequestTypeDef",
-    "DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
     "DescribeDefaultClusterParametersMessageRequestTypeDef",
-    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
     "DescribeEndpointAccessMessageRequestTypeDef",
-    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
     "DescribeEndpointAuthorizationMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
-    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
-    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
     "DescribeHsmConfigurationsMessageRequestTypeDef",
     "DescribeLoggingStatusMessageRequestTypeDef",
     "NodeConfigurationOptionsFilterTypeDef",
-    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
     "DescribeOrderableClusterOptionsMessageRequestTypeDef",
     "DescribePartnersInputMessageRequestTypeDef",
     "PartnerIntegrationInfoTypeDef",
-    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
     "DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef",
-    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
     "DescribeReservedNodeOfferingsMessageRequestTypeDef",
-    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
     "DescribeReservedNodesMessageRequestTypeDef",
     "DescribeResizeMessageRequestTypeDef",
     "ScheduledActionFilterTypeDef",
-    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
     "DescribeSnapshotCopyGrantsMessageRequestTypeDef",
-    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
     "DescribeSnapshotSchedulesMessageRequestTypeDef",
-    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
     "DescribeTableRestoreStatusMessageRequestTypeDef",
-    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
     "DescribeTagsMessageRequestTypeDef",
-    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
     "DescribeUsageLimitsMessageRequestTypeDef",
     "DisableLoggingMessageRequestTypeDef",
     "DisableSnapshotCopyMessageRequestTypeDef",
     "DisassociateDataShareConsumerMessageRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableLoggingMessageRequestTypeDef",
     "EnableSnapshotCopyMessageRequestTypeDef",
     "EndpointAuthorizationTypeDef",
-    "EndpointAuthorizationResponseMetadataTypeDef",
     "EventInfoMapTypeDef",
     "EventTypeDef",
     "GetClusterCredentialsMessageRequestTypeDef",
     "GetClusterCredentialsWithIAMMessageRequestTypeDef",
-    "GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
     "GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef",
-    "GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
     "GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
-    "LoggingStatusTypeDef",
     "ModifyAquaInputMessageRequestTypeDef",
     "ModifyAuthenticationProfileMessageRequestTypeDef",
-    "ModifyAuthenticationProfileResultTypeDef",
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     "ModifyClusterIamRolesMessageRequestTypeDef",
     "ModifyClusterMaintenanceMessageRequestTypeDef",
     "ModifyClusterMessageRequestTypeDef",
+    "ParameterTypeDef",
     "ModifyClusterSnapshotMessageRequestTypeDef",
     "ModifyClusterSnapshotScheduleMessageRequestTypeDef",
     "ModifyClusterSubnetGroupMessageRequestTypeDef",
     "ModifyCustomDomainAssociationMessageRequestTypeDef",
-    "ModifyCustomDomainAssociationResultTypeDef",
     "ModifyEndpointAccessMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     "ModifySnapshotScheduleMessageRequestTypeDef",
     "ModifyUsageLimitMessageRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "NodeConfigurationOptionTypeDef",
-    "PaginatorConfigTypeDef",
     "PartnerIntegrationInputMessageRequestTypeDef",
-    "PartnerIntegrationOutputMessageTypeDef",
+    "PauseClusterMessageOutputTypeDef",
     "PauseClusterMessageRequestTypeDef",
     "PauseClusterMessageTypeDef",
     "PurchaseReservedNodeOfferingMessageRequestTypeDef",
     "RebootClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RejectDataShareMessageRequestTypeDef",
+    "ResizeClusterMessageOutputTypeDef",
     "ResizeClusterMessageRequestTypeDef",
     "ResizeClusterMessageTypeDef",
-    "ResizeProgressMessageTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreFromClusterSnapshotMessageRequestTypeDef",
     "RestoreTableFromClusterSnapshotMessageRequestTypeDef",
     "TableRestoreStatusTypeDef",
+    "ResumeClusterMessageOutputTypeDef",
     "ResumeClusterMessageRequestTypeDef",
     "ResumeClusterMessageTypeDef",
     "RevokeClusterSecurityGroupIngressMessageRequestTypeDef",
     "RevokeEndpointAccessMessageRequestTypeDef",
     "RevokeSnapshotAccessMessageRequestTypeDef",
     "RotateEncryptionKeyMessageRequestTypeDef",
     "SupportedOperationTypeDef",
     "UpdatePartnerStatusInputMessageRequestTypeDef",
+    "ClusterCredentialsTypeDef",
+    "ClusterExtendedCredentialsTypeDef",
+    "ClusterParameterGroupNameMessageTypeDef",
+    "CreateAuthenticationProfileResultTypeDef",
+    "CreateCustomDomainAssociationResultTypeDef",
+    "CustomerStorageMessageTypeDef",
+    "DeleteAuthenticationProfileResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EndpointAuthorizationResponseMetadataTypeDef",
+    "LoggingStatusTypeDef",
+    "ModifyAuthenticationProfileResultTypeDef",
+    "ModifyCustomDomainAssociationResultTypeDef",
+    "PartnerIntegrationOutputMessageTypeDef",
+    "ResizeProgressMessageTypeDef",
     "AccountAttributeTypeDef",
     "ModifyAquaOutputMessageTypeDef",
     "AssociationTypeDef",
     "DescribeAuthenticationProfilesResultTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchDeleteClusterSnapshotsRequestRequestTypeDef",
     "BatchDeleteClusterSnapshotsResultTypeDef",
     "BatchModifyClusterSnapshotsOutputMessageTypeDef",
     "ClusterDbRevisionTypeDef",
     "ClusterParameterGroupDetailsTypeDef",
     "DefaultClusterParametersTypeDef",
-    "ModifyClusterParameterGroupMessageRequestTypeDef",
-    "ResetClusterParameterGroupMessageRequestTypeDef",
     "ClusterParameterGroupStatusTypeDef",
     "ClusterParameterGroupTypeDef",
-    "CreateClusterMessageRequestTypeDef",
-    "CreateClusterParameterGroupMessageRequestTypeDef",
-    "CreateClusterSecurityGroupMessageRequestTypeDef",
-    "CreateClusterSnapshotMessageRequestTypeDef",
-    "CreateClusterSubnetGroupMessageRequestTypeDef",
-    "CreateEventSubscriptionMessageRequestTypeDef",
-    "CreateHsmClientCertificateMessageRequestTypeDef",
-    "CreateHsmConfigurationMessageRequestTypeDef",
-    "CreateSnapshotCopyGrantMessageRequestTypeDef",
-    "CreateSnapshotScheduleMessageRequestTypeDef",
-    "CreateTagsMessageRequestTypeDef",
-    "CreateUsageLimitMessageRequestTypeDef",
     "EC2SecurityGroupTypeDef",
     "EventSubscriptionTypeDef",
     "HsmClientCertificateTypeDef",
     "HsmConfigurationTypeDef",
     "IPRangeTypeDef",
     "SnapshotCopyGrantTypeDef",
     "SnapshotScheduleResponseMetadataTypeDef",
     "SnapshotScheduleTypeDef",
     "SnapshotTypeDef",
     "TaggedResourceTypeDef",
     "UsageLimitResponseMetadataTypeDef",
     "UsageLimitTypeDef",
     "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
     "ClusterVersionsMessageTypeDef",
+    "CreateClusterMessageRequestTypeDef",
+    "CreateClusterParameterGroupMessageRequestTypeDef",
+    "CreateClusterSecurityGroupMessageRequestTypeDef",
+    "CreateClusterSnapshotMessageRequestTypeDef",
+    "CreateClusterSubnetGroupMessageRequestTypeDef",
+    "CreateEventSubscriptionMessageRequestTypeDef",
+    "CreateHsmClientCertificateMessageRequestTypeDef",
+    "CreateHsmConfigurationMessageRequestTypeDef",
+    "CreateSnapshotCopyGrantMessageRequestTypeDef",
+    "CreateSnapshotScheduleMessageRequestTypeDef",
+    "CreateTagsMessageRequestTypeDef",
+    "CreateUsageLimitMessageRequestTypeDef",
     "DataShareResponseMetadataTypeDef",
     "DataShareTypeDef",
+    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
+    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
+    "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
+    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
+    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
+    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
+    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
+    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
+    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
+    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
+    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
+    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
+    "DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
+    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
+    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
+    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
+    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
+    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
+    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
+    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
+    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
+    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
+    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
+    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
+    "GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
+    "GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
     "DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef",
     "DescribeClusterSnapshotsMessageRequestTypeDef",
     "DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef",
     "DescribeClustersMessageClusterAvailableWaitTypeDef",
     "DescribeClustersMessageClusterDeletedWaitTypeDef",
     "DescribeClustersMessageClusterRestoredWaitTypeDef",
     "DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef",
     "DescribeNodeConfigurationOptionsMessageRequestTypeDef",
     "DescribePartnersOutputMessageTypeDef",
     "DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsMessageRequestTypeDef",
     "EndpointAuthorizationListTypeDef",
     "EventCategoriesMapTypeDef",
     "EventsMessageTypeDef",
+    "ModifyClusterParameterGroupMessageRequestTypeDef",
+    "ResetClusterParameterGroupMessageRequestTypeDef",
     "VpcEndpointTypeDef",
     "NodeConfigurationOptionsMessageTypeDef",
     "ReservedNodeOfferingTypeDef",
     "ReservedNodeTypeDef",
     "RestoreTableFromClusterSnapshotResultTypeDef",
     "TableRestoreStatusMessageTypeDef",
+    "ScheduledActionTypeOutputTypeDef",
     "ScheduledActionTypeTypeDef",
     "UpdateTargetTypeDef",
     "AccountAttributeListTypeDef",
     "CustomDomainAssociationsMessageTypeDef",
     "OrderableClusterOptionTypeDef",
     "SubnetTypeDef",
     "ClusterDbRevisionsMessageTypeDef",
@@ -346,18 +351,18 @@
     "EndpointTypeDef",
     "GetReservedNodeExchangeOfferingsOutputMessageTypeDef",
     "ReservedNodeOfferingsMessageTypeDef",
     "AcceptReservedNodeExchangeOutputMessageTypeDef",
     "PurchaseReservedNodeOfferingResultTypeDef",
     "ReservedNodeConfigurationOptionTypeDef",
     "ReservedNodesMessageTypeDef",
-    "CreateScheduledActionMessageRequestTypeDef",
-    "ModifyScheduledActionMessageRequestTypeDef",
     "ScheduledActionResponseMetadataTypeDef",
     "ScheduledActionTypeDef",
+    "CreateScheduledActionMessageRequestTypeDef",
+    "ModifyScheduledActionMessageRequestTypeDef",
     "MaintenanceTrackTypeDef",
     "OrderableClusterOptionsMessageTypeDef",
     "ClusterSubnetGroupTypeDef",
     "AuthorizeClusterSecurityGroupIngressResultTypeDef",
     "ClusterSecurityGroupMessageTypeDef",
     "CreateClusterSecurityGroupResultTypeDef",
     "RevokeClusterSecurityGroupIngressResultTypeDef",
@@ -391,14 +396,25 @@
     "AcceptReservedNodeExchangeInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
     },
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
 AttributeValueTargetTypeDef = TypedDict(
     "AttributeValueTargetTypeDef",
     {
         "AttributeValue": str,
     },
     total=False,
 )
@@ -433,22 +449,20 @@
         "AssociateEntireAccount": bool,
         "ConsumerArn": str,
         "ConsumerRegion": str,
     },
     total=False,
 )
 
-
 class AssociateDataShareConsumerMessageRequestTypeDef(
     _RequiredAssociateDataShareConsumerMessageRequestTypeDef,
     _OptionalAssociateDataShareConsumerMessageRequestTypeDef,
 ):
     pass
 
-
 CertificateAssociationTypeDef = TypedDict(
     "CertificateAssociationTypeDef",
     {
         "CustomDomainName": str,
         "ClusterIdentifier": str,
     },
     total=False,
@@ -475,22 +489,20 @@
         "CIDRIP": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
-
 class AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef(
     _RequiredAuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
     _OptionalAuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
-
 AuthorizeDataShareMessageRequestTypeDef = TypedDict(
     "AuthorizeDataShareMessageRequestTypeDef",
     {
         "DataShareArn": str,
         "ConsumerIdentifier": str,
     },
 )
@@ -506,22 +518,20 @@
     {
         "ClusterIdentifier": str,
         "VpcIds": Sequence[str],
     },
     total=False,
 )
 
-
 class AuthorizeEndpointAccessMessageRequestTypeDef(
     _RequiredAuthorizeEndpointAccessMessageRequestTypeDef,
     _OptionalAuthorizeEndpointAccessMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredAuthorizeSnapshotAccessMessageRequestTypeDef = TypedDict(
     "_RequiredAuthorizeSnapshotAccessMessageRequestTypeDef",
     {
         "AccountWithRestoreAccess": str,
     },
 )
 _OptionalAuthorizeSnapshotAccessMessageRequestTypeDef = TypedDict(
@@ -530,22 +540,20 @@
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
-
 class AuthorizeSnapshotAccessMessageRequestTypeDef(
     _RequiredAuthorizeSnapshotAccessMessageRequestTypeDef,
     _OptionalAuthorizeSnapshotAccessMessageRequestTypeDef,
 ):
     pass
 
-
 SupportedPlatformTypeDef = TypedDict(
     "SupportedPlatformTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -560,21 +568,19 @@
     "_OptionalDeleteClusterSnapshotMessageTypeDef",
     {
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
-
 class DeleteClusterSnapshotMessageTypeDef(
     _RequiredDeleteClusterSnapshotMessageTypeDef, _OptionalDeleteClusterSnapshotMessageTypeDef
 ):
     pass
 
-
 SnapshotErrorMessageTypeDef = TypedDict(
     "SnapshotErrorMessageTypeDef",
     {
         "SnapshotIdentifier": str,
         "SnapshotClusterIdentifier": str,
         "FailureCode": str,
         "FailureReason": str,
@@ -593,22 +599,20 @@
     {
         "ManualSnapshotRetentionPeriod": int,
         "Force": bool,
     },
     total=False,
 )
 
-
 class BatchModifyClusterSnapshotsMessageRequestTypeDef(
     _RequiredBatchModifyClusterSnapshotsMessageRequestTypeDef,
     _OptionalBatchModifyClusterSnapshotsMessageRequestTypeDef,
 ):
     pass
 
-
 CancelResizeMessageRequestTypeDef = TypedDict(
     "CancelResizeMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -617,45 +621,24 @@
     {
         "ClusterIdentifier": str,
         "ScheduleAssociationState": ScheduleStateType,
     },
     total=False,
 )
 
-ClusterCredentialsTypeDef = TypedDict(
-    "ClusterCredentialsTypeDef",
-    {
-        "DbUser": str,
-        "DbPassword": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RevisionTargetTypeDef = TypedDict(
     "RevisionTargetTypeDef",
     {
         "DatabaseRevision": str,
         "Description": str,
         "DatabaseRevisionReleaseDate": datetime,
     },
     total=False,
 )
 
-ClusterExtendedCredentialsTypeDef = TypedDict(
-    "ClusterExtendedCredentialsTypeDef",
-    {
-        "DbUser": str,
-        "DbPassword": str,
-        "Expiration": datetime,
-        "NextRefreshTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ClusterIamRoleTypeDef = TypedDict(
     "ClusterIamRoleTypeDef",
     {
         "IamRoleArn": str,
         "ApplyStatus": str,
     },
     total=False,
@@ -667,51 +650,42 @@
         "NodeRole": str,
         "PrivateIPAddress": str,
         "PublicIPAddress": str,
     },
     total=False,
 )
 
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
         "Description": str,
         "Source": str,
         "DataType": str,
         "AllowedValues": str,
         "ApplyType": ParameterApplyTypeType,
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
     },
     total=False,
 )
 
-ClusterParameterGroupNameMessageTypeDef = TypedDict(
-    "ClusterParameterGroupNameMessageTypeDef",
-    {
-        "ParameterGroupName": str,
-        "ParameterGroupStatus": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ClusterParameterStatusTypeDef = TypedDict(
     "ClusterParameterStatusTypeDef",
     {
         "ParameterName": str,
         "ParameterApplyStatus": str,
         "ParameterApplyErrorDescription": str,
     },
     total=False,
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
@@ -864,59 +838,46 @@
     {
         "SourceSnapshotClusterIdentifier": str,
         "ManualSnapshotRetentionPeriod": int,
     },
     total=False,
 )
 
-
 class CopyClusterSnapshotMessageRequestTypeDef(
     _RequiredCopyClusterSnapshotMessageRequestTypeDef,
     _OptionalCopyClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 CreateAuthenticationProfileMessageRequestTypeDef = TypedDict(
     "CreateAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
 )
 
-CreateAuthenticationProfileResultTypeDef = TypedDict(
-    "CreateAuthenticationProfileResultTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "AuthenticationProfileName": str,
-        "AuthenticationProfileContent": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Value": str,
     },
+    total=False,
 )
 
 CreateCustomDomainAssociationMessageRequestTypeDef = TypedDict(
     "CreateCustomDomainAssociationMessageRequestTypeDef",
     {
         "CustomDomainName": str,
         "CustomDomainCertificateArn": str,
         "ClusterIdentifier": str,
     },
 )
 
-CreateCustomDomainAssociationResultTypeDef = TypedDict(
-    "CreateCustomDomainAssociationResultTypeDef",
-    {
-        "CustomDomainName": str,
-        "CustomDomainCertificateArn": str,
-        "ClusterIdentifier": str,
-        "CustomDomainCertExpiryTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateEndpointAccessMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointAccessMessageRequestTypeDef",
     {
         "EndpointName": str,
         "SubnetGroupName": str,
     },
 )
@@ -926,31 +887,20 @@
         "ClusterIdentifier": str,
         "ResourceOwner": str,
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateEndpointAccessMessageRequestTypeDef(
     _RequiredCreateEndpointAccessMessageRequestTypeDef,
     _OptionalCreateEndpointAccessMessageRequestTypeDef,
 ):
     pass
 
-
-CustomerStorageMessageTypeDef = TypedDict(
-    "CustomerStorageMessageTypeDef",
-    {
-        "TotalBackupSizeInMegaBytes": float,
-        "TotalProvisionedStorageInMegaBytes": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataShareAssociationTypeDef = TypedDict(
     "DataShareAssociationTypeDef",
     {
         "ConsumerIdentifier": str,
         "Status": DataShareStatusType,
         "ConsumerRegion": str,
         "CreatedDate": datetime,
@@ -970,22 +920,14 @@
 DeleteAuthenticationProfileMessageRequestTypeDef = TypedDict(
     "DeleteAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
     },
 )
 
-DeleteAuthenticationProfileResultTypeDef = TypedDict(
-    "DeleteAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalDeleteClusterMessageRequestTypeDef = TypedDict(
@@ -994,21 +936,19 @@
         "SkipFinalClusterSnapshot": bool,
         "FinalClusterSnapshotIdentifier": str,
         "FinalClusterSnapshotRetentionPeriod": int,
     },
     total=False,
 )
 
-
 class DeleteClusterMessageRequestTypeDef(
     _RequiredDeleteClusterMessageRequestTypeDef, _OptionalDeleteClusterMessageRequestTypeDef
 ):
     pass
 
-
 DeleteClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteClusterParameterGroupMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 
@@ -1029,22 +969,20 @@
     "_OptionalDeleteClusterSnapshotMessageRequestTypeDef",
     {
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
-
 class DeleteClusterSnapshotMessageRequestTypeDef(
     _RequiredDeleteClusterSnapshotMessageRequestTypeDef,
     _OptionalDeleteClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 DeleteClusterSubnetGroupMessageRequestTypeDef = TypedDict(
     "DeleteClusterSubnetGroupMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
     },
 )
 
@@ -1131,79 +1069,46 @@
     "DescribeAuthenticationProfilesMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
     },
     total=False,
 )
 
-DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef = TypedDict(
-    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ClusterIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeClusterDbRevisionsMessageRequestTypeDef = TypedDict(
     "DescribeClusterDbRevisionsMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterParameterGroupsMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-    },
-)
-_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef(
-    _RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
-    _OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeClusterParametersMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalDescribeClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1212,33 +1117,20 @@
         "Source": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeClusterParametersMessageRequestTypeDef(
     _RequiredDescribeClusterParametersMessageRequestTypeDef,
     _OptionalDescribeClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-
-DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
-    {
-        "ClusterSecurityGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSecurityGroupsMessageRequestTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
@@ -1257,220 +1149,116 @@
     "_OptionalSnapshotSortingEntityTypeDef",
     {
         "SortOrder": SortByOrderType,
     },
     total=False,
 )
 
-
 class SnapshotSortingEntityTypeDef(
     _RequiredSnapshotSortingEntityTypeDef, _OptionalSnapshotSortingEntityTypeDef
 ):
     pass
 
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
-    {
-        "ClusterSubnetGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSubnetGroupsMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef = TypedDict(
-    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
-    {
-        "MaintenanceTrackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterTracksMessageRequestTypeDef = TypedDict(
     "DescribeClusterTracksMessageRequestTypeDef",
     {
         "MaintenanceTrackName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef = TypedDict(
-    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
-    {
-        "ClusterVersion": str,
-        "ClusterParameterGroupFamily": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterVersionsMessageRequestTypeDef = TypedDict(
     "DescribeClusterVersionsMessageRequestTypeDef",
     {
         "ClusterVersion": str,
         "ClusterParameterGroupFamily": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeClustersMessageDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClustersMessageRequestTypeDef = TypedDict(
     "DescribeClustersMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef = TypedDict(
-    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
-    {
-        "CustomDomainName": str,
-        "CustomDomainCertificateArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCustomDomainAssociationsMessageRequestTypeDef = TypedDict(
     "DescribeCustomDomainAssociationsMessageRequestTypeDef",
     {
         "CustomDomainName": str,
         "CustomDomainCertificateArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef = TypedDict(
-    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
-    {
-        "ConsumerArn": str,
-        "Status": DataShareStatusForConsumerType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSharesForConsumerMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesForConsumerMessageRequestTypeDef",
     {
         "ConsumerArn": str,
         "Status": DataShareStatusForConsumerType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef = TypedDict(
-    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
-    {
-        "ProducerArn": str,
-        "Status": DataShareStatusForProducerType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSharesForProducerMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesForProducerMessageRequestTypeDef",
     {
         "ProducerArn": str,
         "Status": DataShareStatusForProducerType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef = TypedDict(
-    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
-    {
-        "DataShareArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSharesMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesMessageRequestTypeDef",
     {
         "DataShareArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
-    {
-        "ParameterGroupFamily": str,
-    },
-)
-_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef(
-    _RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
-    _OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeDefaultClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDefaultClusterParametersMessageRequestTypeDef",
     {
         "ParameterGroupFamily": str,
     },
 )
 _OptionalDescribeDefaultClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1478,58 +1266,33 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeDefaultClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDefaultClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-
-DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef = TypedDict(
-    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ResourceOwner": str,
-        "EndpointName": str,
-        "VpcId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEndpointAccessMessageRequestTypeDef = TypedDict(
     "DescribeEndpointAccessMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "ResourceOwner": str,
         "EndpointName": str,
         "VpcId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef = TypedDict(
-    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "Account": str,
-        "Grantee": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEndpointAuthorizationMessageRequestTypeDef = TypedDict(
     "DescribeEndpointAuthorizationMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "Account": str,
         "Grantee": bool,
         "MaxRecords": int,
@@ -1542,98 +1305,52 @@
     "DescribeEventCategoriesMessageRequestTypeDef",
     {
         "SourceType": str,
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Duration": int,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef = TypedDict(
-    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
-    {
-        "HsmClientCertificateIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeHsmClientCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
     {
         "HsmClientCertificateIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
-    {
-        "HsmConfigurationIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeHsmConfigurationsMessageRequestTypeDef = TypedDict(
     "DescribeHsmConfigurationsMessageRequestTypeDef",
     {
         "HsmConfigurationIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
@@ -1655,24 +1372,14 @@
         "Name": NodeConfigurationOptionsFilterNameType,
         "Operator": OperatorTypeType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef = TypedDict(
-    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
-    {
-        "ClusterVersion": str,
-        "NodeType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrderableClusterOptionsMessageRequestTypeDef = TypedDict(
     "DescribeOrderableClusterOptionsMessageRequestTypeDef",
     {
         "ClusterVersion": str,
         "NodeType": str,
         "MaxRecords": int,
         "Marker": str,
@@ -1692,84 +1399,54 @@
     {
         "DatabaseName": str,
         "PartnerName": str,
     },
     total=False,
 )
 
-
 class DescribePartnersInputMessageRequestTypeDef(
     _RequiredDescribePartnersInputMessageRequestTypeDef,
     _OptionalDescribePartnersInputMessageRequestTypeDef,
 ):
     pass
 
-
 PartnerIntegrationInfoTypeDef = TypedDict(
     "PartnerIntegrationInfoTypeDef",
     {
         "DatabaseName": str,
         "PartnerName": str,
         "Status": PartnerIntegrationStatusType,
         "StatusMessage": str,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
-DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef = TypedDict(
-    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-        "ReservedNodeExchangeRequestId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "ReservedNodeExchangeRequestId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
-    {
-        "ReservedNodeOfferingId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedNodeOfferingsMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodeOfferingsMessageRequestTypeDef",
     {
         "ReservedNodeOfferingId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef = TypedDict(
-    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedNodesMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodesMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1787,121 +1464,63 @@
     "ScheduledActionFilterTypeDef",
     {
         "Name": ScheduledActionFilterNameType,
         "Values": Sequence[str],
     },
 )
 
-DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
-    {
-        "SnapshotCopyGrantName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSnapshotCopyGrantsMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotCopyGrantsMessageRequestTypeDef",
     {
         "SnapshotCopyGrantName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef = TypedDict(
-    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ScheduleIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSnapshotSchedulesMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotSchedulesMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "ScheduleIdentifier": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef = TypedDict(
-    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "TableRestoreRequestId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTableRestoreStatusMessageRequestTypeDef = TypedDict(
     "DescribeTableRestoreStatusMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "TableRestoreRequestId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeTagsMessageDescribeTagsPaginateTypeDef = TypedDict(
-    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
-    {
-        "ResourceName": str,
-        "ResourceType": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTagsMessageRequestTypeDef = TypedDict(
     "DescribeTagsMessageRequestTypeDef",
     {
         "ResourceName": str,
         "ResourceType": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef = TypedDict(
-    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
-    {
-        "UsageLimitId": str,
-        "ClusterIdentifier": str,
-        "FeatureType": UsageLimitFeatureTypeType,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeUsageLimitsMessageRequestTypeDef = TypedDict(
     "DescribeUsageLimitsMessageRequestTypeDef",
     {
         "UsageLimitId": str,
         "ClusterIdentifier": str,
         "FeatureType": UsageLimitFeatureTypeType,
         "MaxRecords": int,
@@ -1938,29 +1557,20 @@
         "DisassociateEntireAccount": bool,
         "ConsumerArn": str,
         "ConsumerRegion": str,
     },
     total=False,
 )
 
-
 class DisassociateDataShareConsumerMessageRequestTypeDef(
     _RequiredDisassociateDataShareConsumerMessageRequestTypeDef,
     _OptionalDisassociateDataShareConsumerMessageRequestTypeDef,
 ):
     pass
 
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEnableLoggingMessageRequestTypeDef = TypedDict(
     "_RequiredEnableLoggingMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalEnableLoggingMessageRequestTypeDef = TypedDict(
@@ -1970,21 +1580,19 @@
         "S3KeyPrefix": str,
         "LogDestinationType": LogDestinationTypeType,
         "LogExports": Sequence[str],
     },
     total=False,
 )
 
-
 class EnableLoggingMessageRequestTypeDef(
     _RequiredEnableLoggingMessageRequestTypeDef, _OptionalEnableLoggingMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredEnableSnapshotCopyMessageRequestTypeDef = TypedDict(
     "_RequiredEnableSnapshotCopyMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "DestinationRegion": str,
     },
 )
@@ -1994,22 +1602,20 @@
         "RetentionPeriod": int,
         "SnapshotCopyGrantName": str,
         "ManualSnapshotRetentionPeriod": int,
     },
     total=False,
 )
 
-
 class EnableSnapshotCopyMessageRequestTypeDef(
     _RequiredEnableSnapshotCopyMessageRequestTypeDef,
     _OptionalEnableSnapshotCopyMessageRequestTypeDef,
 ):
     pass
 
-
 EndpointAuthorizationTypeDef = TypedDict(
     "EndpointAuthorizationTypeDef",
     {
         "Grantor": str,
         "Grantee": str,
         "ClusterIdentifier": str,
         "AuthorizeTime": datetime,
@@ -2018,30 +1624,14 @@
         "AllowedAllVPCs": bool,
         "AllowedVPCs": List[str],
         "EndpointCount": int,
     },
     total=False,
 )
 
-EndpointAuthorizationResponseMetadataTypeDef = TypedDict(
-    "EndpointAuthorizationResponseMetadataTypeDef",
-    {
-        "Grantor": str,
-        "Grantee": str,
-        "ClusterIdentifier": str,
-        "AuthorizeTime": datetime,
-        "ClusterStatus": str,
-        "Status": AuthorizationStatusType,
-        "AllowedAllVPCs": bool,
-        "AllowedVPCs": List[str],
-        "EndpointCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventInfoMapTypeDef = TypedDict(
     "EventInfoMapTypeDef",
     {
         "EventId": str,
         "EventCategories": List[str],
         "EventDescription": str,
         "Severity": str,
@@ -2078,57 +1668,31 @@
         "AutoCreate": bool,
         "DbGroups": Sequence[str],
         "CustomDomainName": str,
     },
     total=False,
 )
 
-
 class GetClusterCredentialsMessageRequestTypeDef(
     _RequiredGetClusterCredentialsMessageRequestTypeDef,
     _OptionalGetClusterCredentialsMessageRequestTypeDef,
 ):
     pass
 
-
 GetClusterCredentialsWithIAMMessageRequestTypeDef = TypedDict(
     "GetClusterCredentialsWithIAMMessageRequestTypeDef",
     {
         "DbName": str,
         "ClusterIdentifier": str,
         "DurationSeconds": int,
         "CustomDomainName": str,
     },
     total=False,
 )
 
-_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
-    "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
-    {
-        "ActionType": ReservedNodeExchangeActionTypeType,
-    },
-)
-_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
-    "_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "SnapshotIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef(
-    _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
-    _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef = TypedDict(
     "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef",
     {
         "ActionType": ReservedNodeExchangeActionTypeType,
     },
 )
 _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef = TypedDict(
@@ -2138,44 +1702,20 @@
         "SnapshotIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef(
     _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
     _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
 ):
     pass
 
-
-_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
-    "_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-    },
-)
-_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
-    "_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef(
-    _RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
-    _OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef = TypedDict(
     "_RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
     },
 )
 _OptionalGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef = TypedDict(
@@ -2183,75 +1723,47 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef(
     _RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
     _OptionalGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
 ):
     pass
 
-
-LoggingStatusTypeDef = TypedDict(
-    "LoggingStatusTypeDef",
-    {
-        "LoggingEnabled": bool,
-        "BucketName": str,
-        "S3KeyPrefix": str,
-        "LastSuccessfulDeliveryTime": datetime,
-        "LastFailureTime": datetime,
-        "LastFailureMessage": str,
-        "LogDestinationType": LogDestinationTypeType,
-        "LogExports": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredModifyAquaInputMessageRequestTypeDef = TypedDict(
     "_RequiredModifyAquaInputMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyAquaInputMessageRequestTypeDef = TypedDict(
     "_OptionalModifyAquaInputMessageRequestTypeDef",
     {
         "AquaConfigurationStatus": AquaConfigurationStatusType,
     },
     total=False,
 )
 
-
 class ModifyAquaInputMessageRequestTypeDef(
     _RequiredModifyAquaInputMessageRequestTypeDef, _OptionalModifyAquaInputMessageRequestTypeDef
 ):
     pass
 
-
 ModifyAuthenticationProfileMessageRequestTypeDef = TypedDict(
     "ModifyAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
 )
 
-ModifyAuthenticationProfileResultTypeDef = TypedDict(
-    "ModifyAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "AuthenticationProfileContent": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ModifyClusterDbRevisionMessageRequestTypeDef = TypedDict(
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "RevisionTarget": str,
     },
 )
@@ -2268,22 +1780,20 @@
         "AddIamRoles": Sequence[str],
         "RemoveIamRoles": Sequence[str],
         "DefaultIamRoleArn": str,
     },
     total=False,
 )
 
-
 class ModifyClusterIamRolesMessageRequestTypeDef(
     _RequiredModifyClusterIamRolesMessageRequestTypeDef,
     _OptionalModifyClusterIamRolesMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterMaintenanceMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
@@ -2294,22 +1804,20 @@
         "DeferMaintenanceStartTime": Union[datetime, str],
         "DeferMaintenanceEndTime": Union[datetime, str],
         "DeferMaintenanceDuration": int,
     },
     total=False,
 )
 
-
 class ModifyClusterMaintenanceMessageRequestTypeDef(
     _RequiredModifyClusterMaintenanceMessageRequestTypeDef,
     _OptionalModifyClusterMaintenanceMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyClusterMessageRequestTypeDef = TypedDict(
@@ -2339,20 +1847,34 @@
         "AvailabilityZoneRelocation": bool,
         "AvailabilityZone": str,
         "Port": int,
     },
     total=False,
 )
 
-
 class ModifyClusterMessageRequestTypeDef(
     _RequiredModifyClusterMessageRequestTypeDef, _OptionalModifyClusterMessageRequestTypeDef
 ):
     pass
 
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
+    {
+        "ParameterName": str,
+        "ParameterValue": str,
+        "Description": str,
+        "Source": str,
+        "DataType": str,
+        "AllowedValues": str,
+        "ApplyType": ParameterApplyTypeType,
+        "IsModifiable": bool,
+        "MinimumEngineVersion": str,
+    },
+    total=False,
+)
 
 _RequiredModifyClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterSnapshotMessageRequestTypeDef",
     {
         "SnapshotIdentifier": str,
     },
 )
@@ -2361,22 +1883,20 @@
     {
         "ManualSnapshotRetentionPeriod": int,
         "Force": bool,
     },
     total=False,
 )
 
-
 class ModifyClusterSnapshotMessageRequestTypeDef(
     _RequiredModifyClusterSnapshotMessageRequestTypeDef,
     _OptionalModifyClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyClusterSnapshotScheduleMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterSnapshotScheduleMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyClusterSnapshotScheduleMessageRequestTypeDef = TypedDict(
@@ -2384,22 +1904,20 @@
     {
         "ScheduleIdentifier": str,
         "DisassociateSchedule": bool,
     },
     total=False,
 )
 
-
 class ModifyClusterSnapshotScheduleMessageRequestTypeDef(
     _RequiredModifyClusterSnapshotScheduleMessageRequestTypeDef,
     _OptionalModifyClusterSnapshotScheduleMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyClusterSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterSubnetGroupMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -2407,22 +1925,20 @@
     "_OptionalModifyClusterSubnetGroupMessageRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class ModifyClusterSubnetGroupMessageRequestTypeDef(
     _RequiredModifyClusterSubnetGroupMessageRequestTypeDef,
     _OptionalModifyClusterSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyCustomDomainAssociationMessageRequestTypeDef = TypedDict(
     "_RequiredModifyCustomDomainAssociationMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyCustomDomainAssociationMessageRequestTypeDef = TypedDict(
@@ -2430,55 +1946,40 @@
     {
         "CustomDomainName": str,
         "CustomDomainCertificateArn": str,
     },
     total=False,
 )
 
-
 class ModifyCustomDomainAssociationMessageRequestTypeDef(
     _RequiredModifyCustomDomainAssociationMessageRequestTypeDef,
     _OptionalModifyCustomDomainAssociationMessageRequestTypeDef,
 ):
     pass
 
-
-ModifyCustomDomainAssociationResultTypeDef = TypedDict(
-    "ModifyCustomDomainAssociationResultTypeDef",
-    {
-        "CustomDomainName": str,
-        "CustomDomainCertificateArn": str,
-        "ClusterIdentifier": str,
-        "CustomDomainCertExpiryTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredModifyEndpointAccessMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointAccessMessageRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
 _OptionalModifyEndpointAccessMessageRequestTypeDef = TypedDict(
     "_OptionalModifyEndpointAccessMessageRequestTypeDef",
     {
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyEndpointAccessMessageRequestTypeDef(
     _RequiredModifyEndpointAccessMessageRequestTypeDef,
     _OptionalModifyEndpointAccessMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
     },
 )
 _OptionalModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
@@ -2490,22 +1991,20 @@
         "EventCategories": Sequence[str],
         "Severity": str,
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class ModifyEventSubscriptionMessageRequestTypeDef(
     _RequiredModifyEventSubscriptionMessageRequestTypeDef,
     _OptionalModifyEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifySnapshotCopyRetentionPeriodMessageRequestTypeDef = TypedDict(
     "_RequiredModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "RetentionPeriod": int,
     },
 )
@@ -2513,22 +2012,20 @@
     "_OptionalModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     {
         "Manual": bool,
     },
     total=False,
 )
 
-
 class ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef(
     _RequiredModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     _OptionalModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
 ):
     pass
 
-
 ModifySnapshotScheduleMessageRequestTypeDef = TypedDict(
     "ModifySnapshotScheduleMessageRequestTypeDef",
     {
         "ScheduleIdentifier": str,
         "ScheduleDefinitions": Sequence[str],
     },
 )
@@ -2544,21 +2041,19 @@
     {
         "Amount": int,
         "BreachAction": UsageLimitBreachActionType,
     },
     total=False,
 )
 
-
 class ModifyUsageLimitMessageRequestTypeDef(
     _RequiredModifyUsageLimitMessageRequestTypeDef, _OptionalModifyUsageLimitMessageRequestTypeDef
 ):
     pass
 
-
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "NetworkInterfaceId": str,
         "SubnetId": str,
         "PrivateIpAddress": str,
         "AvailabilityZone": str,
@@ -2573,40 +2068,28 @@
         "NumberOfNodes": int,
         "EstimatedDiskUtilizationPercent": float,
         "Mode": ModeType,
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
 PartnerIntegrationInputMessageRequestTypeDef = TypedDict(
     "PartnerIntegrationInputMessageRequestTypeDef",
     {
         "AccountId": str,
         "ClusterIdentifier": str,
         "DatabaseName": str,
         "PartnerName": str,
     },
 )
 
-PartnerIntegrationOutputMessageTypeDef = TypedDict(
-    "PartnerIntegrationOutputMessageTypeDef",
+PauseClusterMessageOutputTypeDef = TypedDict(
+    "PauseClusterMessageOutputTypeDef",
     {
-        "DatabaseName": str,
-        "PartnerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterIdentifier": str,
     },
 )
 
 PauseClusterMessageRequestTypeDef = TypedDict(
     "PauseClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
@@ -2630,22 +2113,20 @@
     "_OptionalPurchaseReservedNodeOfferingMessageRequestTypeDef",
     {
         "NodeCount": int,
     },
     total=False,
 )
 
-
 class PurchaseReservedNodeOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedNodeOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedNodeOfferingMessageRequestTypeDef,
 ):
     pass
 
-
 RebootClusterMessageRequestTypeDef = TypedDict(
     "RebootClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2661,14 +2142,38 @@
 RejectDataShareMessageRequestTypeDef = TypedDict(
     "RejectDataShareMessageRequestTypeDef",
     {
         "DataShareArn": str,
     },
 )
 
+_RequiredResizeClusterMessageOutputTypeDef = TypedDict(
+    "_RequiredResizeClusterMessageOutputTypeDef",
+    {
+        "ClusterIdentifier": str,
+    },
+)
+_OptionalResizeClusterMessageOutputTypeDef = TypedDict(
+    "_OptionalResizeClusterMessageOutputTypeDef",
+    {
+        "ClusterType": str,
+        "NodeType": str,
+        "NumberOfNodes": int,
+        "Classic": bool,
+        "ReservedNodeId": str,
+        "TargetReservedNodeOfferingId": str,
+    },
+    total=False,
+)
+
+class ResizeClusterMessageOutputTypeDef(
+    _RequiredResizeClusterMessageOutputTypeDef, _OptionalResizeClusterMessageOutputTypeDef
+):
+    pass
+
 _RequiredResizeClusterMessageRequestTypeDef = TypedDict(
     "_RequiredResizeClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalResizeClusterMessageRequestTypeDef = TypedDict(
@@ -2680,21 +2185,19 @@
         "Classic": bool,
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
     },
     total=False,
 )
 
-
 class ResizeClusterMessageRequestTypeDef(
     _RequiredResizeClusterMessageRequestTypeDef, _OptionalResizeClusterMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredResizeClusterMessageTypeDef = TypedDict(
     "_RequiredResizeClusterMessageTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalResizeClusterMessageTypeDef = TypedDict(
@@ -2706,55 +2209,19 @@
         "Classic": bool,
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
     },
     total=False,
 )
 
-
 class ResizeClusterMessageTypeDef(
     _RequiredResizeClusterMessageTypeDef, _OptionalResizeClusterMessageTypeDef
 ):
     pass
 
-
-ResizeProgressMessageTypeDef = TypedDict(
-    "ResizeProgressMessageTypeDef",
-    {
-        "TargetNodeType": str,
-        "TargetNumberOfNodes": int,
-        "TargetClusterType": str,
-        "Status": str,
-        "ImportTablesCompleted": List[str],
-        "ImportTablesInProgress": List[str],
-        "ImportTablesNotStarted": List[str],
-        "AvgResizeRateInMegaBytesPerSecond": float,
-        "TotalResizeDataInMegaBytes": int,
-        "ProgressInMegaBytes": int,
-        "ElapsedTimeInSeconds": int,
-        "EstimatedTimeToCompletionInSeconds": int,
-        "ResizeType": str,
-        "Message": str,
-        "TargetEncryptionType": str,
-        "DataTransferProgressPercent": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 _RequiredRestoreFromClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreFromClusterSnapshotMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalRestoreFromClusterSnapshotMessageRequestTypeDef = TypedDict(
@@ -2792,22 +2259,20 @@
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
         "Encrypted": bool,
     },
     total=False,
 )
 
-
 class RestoreFromClusterSnapshotMessageRequestTypeDef(
     _RequiredRestoreFromClusterSnapshotMessageRequestTypeDef,
     _OptionalRestoreFromClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreTableFromClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreTableFromClusterSnapshotMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SourceDatabaseName": str,
         "SourceTableName": str,
@@ -2821,22 +2286,20 @@
         "TargetDatabaseName": str,
         "TargetSchemaName": str,
         "EnableCaseSensitiveIdentifier": bool,
     },
     total=False,
 )
 
-
 class RestoreTableFromClusterSnapshotMessageRequestTypeDef(
     _RequiredRestoreTableFromClusterSnapshotMessageRequestTypeDef,
     _OptionalRestoreTableFromClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 TableRestoreStatusTypeDef = TypedDict(
     "TableRestoreStatusTypeDef",
     {
         "TableRestoreRequestId": str,
         "Status": TableRestoreStatusTypeType,
         "Message": str,
         "RequestTime": datetime,
@@ -2850,14 +2313,21 @@
         "TargetDatabaseName": str,
         "TargetSchemaName": str,
         "NewTableName": str,
     },
     total=False,
 )
 
+ResumeClusterMessageOutputTypeDef = TypedDict(
+    "ResumeClusterMessageOutputTypeDef",
+    {
+        "ClusterIdentifier": str,
+    },
+)
+
 ResumeClusterMessageRequestTypeDef = TypedDict(
     "ResumeClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2880,22 +2350,20 @@
         "CIDRIP": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
-
 class RevokeClusterSecurityGroupIngressMessageRequestTypeDef(
     _RequiredRevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     _OptionalRevokeClusterSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
-
 RevokeEndpointAccessMessageRequestTypeDef = TypedDict(
     "RevokeEndpointAccessMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "Account": str,
         "VpcIds": Sequence[str],
         "Force": bool,
@@ -2915,22 +2383,20 @@
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
-
 class RevokeSnapshotAccessMessageRequestTypeDef(
     _RequiredRevokeSnapshotAccessMessageRequestTypeDef,
     _OptionalRevokeSnapshotAccessMessageRequestTypeDef,
 ):
     pass
 
-
 RotateEncryptionKeyMessageRequestTypeDef = TypedDict(
     "RotateEncryptionKeyMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2956,36 +2422,191 @@
     "_OptionalUpdatePartnerStatusInputMessageRequestTypeDef",
     {
         "StatusMessage": str,
     },
     total=False,
 )
 
-
 class UpdatePartnerStatusInputMessageRequestTypeDef(
     _RequiredUpdatePartnerStatusInputMessageRequestTypeDef,
     _OptionalUpdatePartnerStatusInputMessageRequestTypeDef,
 ):
     pass
 
+ClusterCredentialsTypeDef = TypedDict(
+    "ClusterCredentialsTypeDef",
+    {
+        "DbUser": str,
+        "DbPassword": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ClusterExtendedCredentialsTypeDef = TypedDict(
+    "ClusterExtendedCredentialsTypeDef",
+    {
+        "DbUser": str,
+        "DbPassword": str,
+        "Expiration": datetime,
+        "NextRefreshTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ClusterParameterGroupNameMessageTypeDef = TypedDict(
+    "ClusterParameterGroupNameMessageTypeDef",
+    {
+        "ParameterGroupName": str,
+        "ParameterGroupStatus": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAuthenticationProfileResultTypeDef = TypedDict(
+    "CreateAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "AuthenticationProfileContent": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomDomainAssociationResultTypeDef = TypedDict(
+    "CreateCustomDomainAssociationResultTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "ClusterIdentifier": str,
+        "CustomDomainCertExpiryTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CustomerStorageMessageTypeDef = TypedDict(
+    "CustomerStorageMessageTypeDef",
+    {
+        "TotalBackupSizeInMegaBytes": float,
+        "TotalProvisionedStorageInMegaBytes": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAuthenticationProfileResultTypeDef = TypedDict(
+    "DeleteAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EndpointAuthorizationResponseMetadataTypeDef = TypedDict(
+    "EndpointAuthorizationResponseMetadataTypeDef",
+    {
+        "Grantor": str,
+        "Grantee": str,
+        "ClusterIdentifier": str,
+        "AuthorizeTime": datetime,
+        "ClusterStatus": str,
+        "Status": AuthorizationStatusType,
+        "AllowedAllVPCs": bool,
+        "AllowedVPCs": List[str],
+        "EndpointCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LoggingStatusTypeDef = TypedDict(
+    "LoggingStatusTypeDef",
+    {
+        "LoggingEnabled": bool,
+        "BucketName": str,
+        "S3KeyPrefix": str,
+        "LastSuccessfulDeliveryTime": datetime,
+        "LastFailureTime": datetime,
+        "LastFailureMessage": str,
+        "LogDestinationType": LogDestinationTypeType,
+        "LogExports": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyAuthenticationProfileResultTypeDef = TypedDict(
+    "ModifyAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "AuthenticationProfileContent": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyCustomDomainAssociationResultTypeDef = TypedDict(
+    "ModifyCustomDomainAssociationResultTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "ClusterIdentifier": str,
+        "CustomDomainCertExpiryTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PartnerIntegrationOutputMessageTypeDef = TypedDict(
+    "PartnerIntegrationOutputMessageTypeDef",
+    {
+        "DatabaseName": str,
+        "PartnerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResizeProgressMessageTypeDef = TypedDict(
+    "ResizeProgressMessageTypeDef",
+    {
+        "TargetNodeType": str,
+        "TargetNumberOfNodes": int,
+        "TargetClusterType": str,
+        "Status": str,
+        "ImportTablesCompleted": List[str],
+        "ImportTablesInProgress": List[str],
+        "ImportTablesNotStarted": List[str],
+        "AvgResizeRateInMegaBytesPerSecond": float,
+        "TotalResizeDataInMegaBytes": int,
+        "ProgressInMegaBytes": int,
+        "ElapsedTimeInSeconds": int,
+        "EstimatedTimeToCompletionInSeconds": int,
+        "ResizeType": str,
+        "Message": str,
+        "TargetEncryptionType": str,
+        "DataTransferProgressPercent": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 AccountAttributeTypeDef = TypedDict(
     "AccountAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[AttributeValueTargetTypeDef],
     },
     total=False,
 )
 
 ModifyAquaOutputMessageTypeDef = TypedDict(
     "ModifyAquaOutputMessageTypeDef",
     {
         "AquaConfiguration": AquaConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociationTypeDef = TypedDict(
     "AssociationTypeDef",
     {
         "CustomDomainCertificateArn": str,
@@ -2995,15 +2616,15 @@
     total=False,
 )
 
 DescribeAuthenticationProfilesResultTypeDef = TypedDict(
     "DescribeAuthenticationProfilesResultTypeDef",
     {
         "AuthenticationProfiles": List[AuthenticationProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
@@ -3020,24 +2641,24 @@
 )
 
 BatchDeleteClusterSnapshotsResultTypeDef = TypedDict(
     "BatchDeleteClusterSnapshotsResultTypeDef",
     {
         "Resources": List[str],
         "Errors": List[SnapshotErrorMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchModifyClusterSnapshotsOutputMessageTypeDef = TypedDict(
     "BatchModifyClusterSnapshotsOutputMessageTypeDef",
     {
         "Resources": List[str],
         "Errors": List[SnapshotErrorMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterDbRevisionTypeDef = TypedDict(
     "ClusterDbRevisionTypeDef",
     {
         "ClusterIdentifier": str,
@@ -3047,82 +2668,249 @@
     },
     total=False,
 )
 
 ClusterParameterGroupDetailsTypeDef = TypedDict(
     "ClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefaultClusterParametersTypeDef = TypedDict(
     "DefaultClusterParametersTypeDef",
     {
         "ParameterGroupFamily": str,
         "Marker": str,
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
     },
     total=False,
 )
 
-ModifyClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyClusterParameterGroupMessageRequestTypeDef",
+ClusterParameterGroupStatusTypeDef = TypedDict(
+    "ClusterParameterGroupStatusTypeDef",
     {
         "ParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
+        "ParameterApplyStatus": str,
+        "ClusterParameterStatusList": List[ClusterParameterStatusTypeDef],
     },
+    total=False,
 )
 
-_RequiredResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetClusterParameterGroupMessageRequestTypeDef",
+ClusterParameterGroupTypeDef = TypedDict(
+    "ClusterParameterGroupTypeDef",
     {
         "ParameterGroupName": str,
+        "ParameterGroupFamily": str,
+        "Description": str,
+        "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
-_OptionalResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetClusterParameterGroupMessageRequestTypeDef",
+
+EC2SecurityGroupTypeDef = TypedDict(
+    "EC2SecurityGroupTypeDef",
     {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
+        "Status": str,
+        "EC2SecurityGroupName": str,
+        "EC2SecurityGroupOwnerId": str,
+        "Tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
+EventSubscriptionTypeDef = TypedDict(
+    "EventSubscriptionTypeDef",
+    {
+        "CustomerAwsId": str,
+        "CustSubscriptionId": str,
+        "SnsTopicArn": str,
+        "Status": str,
+        "SubscriptionCreationTime": datetime,
+        "SourceType": str,
+        "SourceIdsList": List[str],
+        "EventCategoriesList": List[str],
+        "Severity": str,
+        "Enabled": bool,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
 
-class ResetClusterParameterGroupMessageRequestTypeDef(
-    _RequiredResetClusterParameterGroupMessageRequestTypeDef,
-    _OptionalResetClusterParameterGroupMessageRequestTypeDef,
-):
-    pass
+HsmClientCertificateTypeDef = TypedDict(
+    "HsmClientCertificateTypeDef",
+    {
+        "HsmClientCertificateIdentifier": str,
+        "HsmClientCertificatePublicKey": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
 
+HsmConfigurationTypeDef = TypedDict(
+    "HsmConfigurationTypeDef",
+    {
+        "HsmConfigurationIdentifier": str,
+        "Description": str,
+        "HsmIpAddress": str,
+        "HsmPartitionName": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
 
-ClusterParameterGroupStatusTypeDef = TypedDict(
-    "ClusterParameterGroupStatusTypeDef",
+IPRangeTypeDef = TypedDict(
+    "IPRangeTypeDef",
     {
-        "ParameterGroupName": str,
-        "ParameterApplyStatus": str,
-        "ClusterParameterStatusList": List[ClusterParameterStatusTypeDef],
+        "Status": str,
+        "CIDRIP": str,
+        "Tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
-ClusterParameterGroupTypeDef = TypedDict(
-    "ClusterParameterGroupTypeDef",
+SnapshotCopyGrantTypeDef = TypedDict(
+    "SnapshotCopyGrantTypeDef",
     {
-        "ParameterGroupName": str,
-        "ParameterGroupFamily": str,
-        "Description": str,
-        "Tags": List[TagTypeDef],
+        "SnapshotCopyGrantName": str,
+        "KmsKeyId": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+SnapshotScheduleResponseMetadataTypeDef = TypedDict(
+    "SnapshotScheduleResponseMetadataTypeDef",
+    {
+        "ScheduleDefinitions": List[str],
+        "ScheduleIdentifier": str,
+        "ScheduleDescription": str,
+        "Tags": List[TagOutputTypeDef],
+        "NextInvocations": List[datetime],
+        "AssociatedClusterCount": int,
+        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SnapshotScheduleTypeDef = TypedDict(
+    "SnapshotScheduleTypeDef",
+    {
+        "ScheduleDefinitions": List[str],
+        "ScheduleIdentifier": str,
+        "ScheduleDescription": str,
+        "Tags": List[TagOutputTypeDef],
+        "NextInvocations": List[datetime],
+        "AssociatedClusterCount": int,
+        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
+    },
+    total=False,
+)
+
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotIdentifier": str,
+        "ClusterIdentifier": str,
+        "SnapshotCreateTime": datetime,
+        "Status": str,
+        "Port": int,
+        "AvailabilityZone": str,
+        "ClusterCreateTime": datetime,
+        "MasterUsername": str,
+        "ClusterVersion": str,
+        "EngineFullVersion": str,
+        "SnapshotType": str,
+        "NodeType": str,
+        "NumberOfNodes": int,
+        "DBName": str,
+        "VpcId": str,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "EncryptedWithHSM": bool,
+        "AccountsWithRestoreAccess": List[AccountWithRestoreAccessTypeDef],
+        "OwnerAccount": str,
+        "TotalBackupSizeInMegaBytes": float,
+        "ActualIncrementalBackupSizeInMegaBytes": float,
+        "BackupProgressInMegaBytes": float,
+        "CurrentBackupRateInMegaBytesPerSecond": float,
+        "EstimatedSecondsToCompletion": int,
+        "ElapsedTimeInSeconds": int,
+        "SourceRegion": str,
+        "Tags": List[TagOutputTypeDef],
+        "RestorableNodeTypes": List[str],
+        "EnhancedVpcRouting": bool,
+        "MaintenanceTrackName": str,
+        "ManualSnapshotRetentionPeriod": int,
+        "ManualSnapshotRemainingDays": int,
+        "SnapshotRetentionStartTime": datetime,
     },
     total=False,
 )
 
+TaggedResourceTypeDef = TypedDict(
+    "TaggedResourceTypeDef",
+    {
+        "Tag": TagOutputTypeDef,
+        "ResourceName": str,
+        "ResourceType": str,
+    },
+    total=False,
+)
+
+UsageLimitResponseMetadataTypeDef = TypedDict(
+    "UsageLimitResponseMetadataTypeDef",
+    {
+        "UsageLimitId": str,
+        "ClusterIdentifier": str,
+        "FeatureType": UsageLimitFeatureTypeType,
+        "LimitType": UsageLimitLimitTypeType,
+        "Amount": int,
+        "Period": UsageLimitPeriodType,
+        "BreachAction": UsageLimitBreachActionType,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UsageLimitTypeDef = TypedDict(
+    "UsageLimitTypeDef",
+    {
+        "UsageLimitId": str,
+        "ClusterIdentifier": str,
+        "FeatureType": UsageLimitFeatureTypeType,
+        "LimitType": UsageLimitLimitTypeType,
+        "Amount": int,
+        "Period": UsageLimitPeriodType,
+        "BreachAction": UsageLimitBreachActionType,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+DescribeReservedNodeExchangeStatusOutputMessageTypeDef = TypedDict(
+    "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
+    {
+        "ReservedNodeExchangeStatusDetails": List[ReservedNodeExchangeStatusTypeDef],
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ClusterVersionsMessageTypeDef = TypedDict(
+    "ClusterVersionsMessageTypeDef",
+    {
+        "Marker": str,
+        "ClusterVersions": List[ClusterVersionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "NodeType": str,
         "MasterUsername": str,
         "MasterUserPassword": str,
@@ -3161,21 +2949,19 @@
         "AquaConfigurationStatus": AquaConfigurationStatusType,
         "DefaultIamRoleArn": str,
         "LoadSampleData": str,
     },
     total=False,
 )
 
-
 class CreateClusterMessageRequestTypeDef(
     _RequiredCreateClusterMessageRequestTypeDef, _OptionalCreateClusterMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterParameterGroupMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
         "ParameterGroupFamily": str,
         "Description": str,
     },
@@ -3184,22 +2970,20 @@
     "_OptionalCreateClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateClusterParameterGroupMessageRequestTypeDef(
     _RequiredCreateClusterParameterGroupMessageRequestTypeDef,
     _OptionalCreateClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateClusterSecurityGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSecurityGroupMessageRequestTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "Description": str,
     },
 )
@@ -3207,22 +2991,20 @@
     "_OptionalCreateClusterSecurityGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateClusterSecurityGroupMessageRequestTypeDef(
     _RequiredCreateClusterSecurityGroupMessageRequestTypeDef,
     _OptionalCreateClusterSecurityGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSnapshotMessageRequestTypeDef",
     {
         "SnapshotIdentifier": str,
         "ClusterIdentifier": str,
     },
 )
@@ -3231,22 +3013,20 @@
     {
         "ManualSnapshotRetentionPeriod": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateClusterSnapshotMessageRequestTypeDef(
     _RequiredCreateClusterSnapshotMessageRequestTypeDef,
     _OptionalCreateClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateClusterSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSubnetGroupMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "Description": str,
         "SubnetIds": Sequence[str],
     },
@@ -3255,22 +3035,20 @@
     "_OptionalCreateClusterSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateClusterSubnetGroupMessageRequestTypeDef(
     _RequiredCreateClusterSubnetGroupMessageRequestTypeDef,
     _OptionalCreateClusterSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "SnsTopicArn": str,
     },
 )
@@ -3283,44 +3061,40 @@
         "Severity": str,
         "Enabled": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateEventSubscriptionMessageRequestTypeDef(
     _RequiredCreateEventSubscriptionMessageRequestTypeDef,
     _OptionalCreateEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateHsmClientCertificateMessageRequestTypeDef = TypedDict(
     "_RequiredCreateHsmClientCertificateMessageRequestTypeDef",
     {
         "HsmClientCertificateIdentifier": str,
     },
 )
 _OptionalCreateHsmClientCertificateMessageRequestTypeDef = TypedDict(
     "_OptionalCreateHsmClientCertificateMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateHsmClientCertificateMessageRequestTypeDef(
     _RequiredCreateHsmClientCertificateMessageRequestTypeDef,
     _OptionalCreateHsmClientCertificateMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateHsmConfigurationMessageRequestTypeDef = TypedDict(
     "_RequiredCreateHsmConfigurationMessageRequestTypeDef",
     {
         "HsmConfigurationIdentifier": str,
         "Description": str,
         "HsmIpAddress": str,
         "HsmPartitionName": str,
@@ -3332,22 +3106,20 @@
     "_OptionalCreateHsmConfigurationMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateHsmConfigurationMessageRequestTypeDef(
     _RequiredCreateHsmConfigurationMessageRequestTypeDef,
     _OptionalCreateHsmConfigurationMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateSnapshotCopyGrantMessageRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotCopyGrantMessageRequestTypeDef",
     {
         "SnapshotCopyGrantName": str,
     },
 )
 _OptionalCreateSnapshotCopyGrantMessageRequestTypeDef = TypedDict(
@@ -3355,22 +3127,20 @@
     {
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSnapshotCopyGrantMessageRequestTypeDef(
     _RequiredCreateSnapshotCopyGrantMessageRequestTypeDef,
     _OptionalCreateSnapshotCopyGrantMessageRequestTypeDef,
 ):
     pass
 
-
 CreateSnapshotScheduleMessageRequestTypeDef = TypedDict(
     "CreateSnapshotScheduleMessageRequestTypeDef",
     {
         "ScheduleDefinitions": Sequence[str],
         "ScheduleIdentifier": str,
         "ScheduleDescription": str,
         "Tags": Sequence[TagTypeDef],
@@ -3403,258 +3173,417 @@
         "Period": UsageLimitPeriodType,
         "BreachAction": UsageLimitBreachActionType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateUsageLimitMessageRequestTypeDef(
     _RequiredCreateUsageLimitMessageRequestTypeDef, _OptionalCreateUsageLimitMessageRequestTypeDef
 ):
     pass
 
+DataShareResponseMetadataTypeDef = TypedDict(
+    "DataShareResponseMetadataTypeDef",
+    {
+        "DataShareArn": str,
+        "ProducerArn": str,
+        "AllowPubliclyAccessibleConsumers": bool,
+        "DataShareAssociations": List[DataShareAssociationTypeDef],
+        "ManagedBy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-EC2SecurityGroupTypeDef = TypedDict(
-    "EC2SecurityGroupTypeDef",
+DataShareTypeDef = TypedDict(
+    "DataShareTypeDef",
     {
-        "Status": str,
-        "EC2SecurityGroupName": str,
-        "EC2SecurityGroupOwnerId": str,
-        "Tags": List[TagTypeDef],
+        "DataShareArn": str,
+        "ProducerArn": str,
+        "AllowPubliclyAccessibleConsumers": bool,
+        "DataShareAssociations": List[DataShareAssociationTypeDef],
+        "ManagedBy": str,
     },
     total=False,
 )
 
-EventSubscriptionTypeDef = TypedDict(
-    "EventSubscriptionTypeDef",
+DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef = TypedDict(
+    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
     {
-        "CustomerAwsId": str,
-        "CustSubscriptionId": str,
-        "SnsTopicArn": str,
-        "Status": str,
-        "SubscriptionCreationTime": datetime,
-        "SourceType": str,
-        "SourceIdsList": List[str],
-        "EventCategoriesList": List[str],
-        "Severity": str,
-        "Enabled": bool,
-        "Tags": List[TagTypeDef],
+        "ClusterIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-HsmClientCertificateTypeDef = TypedDict(
-    "HsmClientCertificateTypeDef",
+DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
     {
-        "HsmClientCertificateIdentifier": str,
-        "HsmClientCertificatePublicKey": str,
-        "Tags": List[TagTypeDef],
+        "ParameterGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-HsmConfigurationTypeDef = TypedDict(
-    "HsmConfigurationTypeDef",
+_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
     {
-        "HsmConfigurationIdentifier": str,
-        "Description": str,
-        "HsmIpAddress": str,
-        "HsmPartitionName": str,
-        "Tags": List[TagTypeDef],
+        "ParameterGroupName": str,
+    },
+)
+_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-IPRangeTypeDef = TypedDict(
-    "IPRangeTypeDef",
+class DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef(
+    _RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+    _OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+):
+    pass
+
+DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
     {
-        "Status": str,
-        "CIDRIP": str,
-        "Tags": List[TagTypeDef],
+        "ClusterSecurityGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-SnapshotCopyGrantTypeDef = TypedDict(
-    "SnapshotCopyGrantTypeDef",
+DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
     {
-        "SnapshotCopyGrantName": str,
-        "KmsKeyId": str,
-        "Tags": List[TagTypeDef],
+        "ClusterSubnetGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-SnapshotScheduleResponseMetadataTypeDef = TypedDict(
-    "SnapshotScheduleResponseMetadataTypeDef",
+DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef = TypedDict(
+    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
     {
-        "ScheduleDefinitions": List[str],
-        "ScheduleIdentifier": str,
-        "ScheduleDescription": str,
-        "Tags": List[TagTypeDef],
-        "NextInvocations": List[datetime],
-        "AssociatedClusterCount": int,
-        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaintenanceTrackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-SnapshotScheduleTypeDef = TypedDict(
-    "SnapshotScheduleTypeDef",
+DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef = TypedDict(
+    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
     {
-        "ScheduleDefinitions": List[str],
-        "ScheduleIdentifier": str,
-        "ScheduleDescription": str,
-        "Tags": List[TagTypeDef],
-        "NextInvocations": List[datetime],
-        "AssociatedClusterCount": int,
-        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
+        "ClusterVersion": str,
+        "ClusterParameterGroupFamily": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
+DescribeClustersMessageDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
     {
-        "SnapshotIdentifier": str,
         "ClusterIdentifier": str,
-        "SnapshotCreateTime": datetime,
-        "Status": str,
-        "Port": int,
-        "AvailabilityZone": str,
-        "ClusterCreateTime": datetime,
-        "MasterUsername": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef = TypedDict(
+    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef = TypedDict(
+    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
+    {
+        "ConsumerArn": str,
+        "Status": DataShareStatusForConsumerType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef = TypedDict(
+    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
+    {
+        "ProducerArn": str,
+        "Status": DataShareStatusForProducerType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef = TypedDict(
+    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
+    {
+        "DataShareArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    {
+        "ParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef(
+    _RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+    _OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+):
+    pass
+
+DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef = TypedDict(
+    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ResourceOwner": str,
+        "EndpointName": str,
+        "VpcId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef = TypedDict(
+    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "Account": str,
+        "Grantee": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef = TypedDict(
+    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
+    {
+        "HsmClientCertificateIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
+    {
+        "HsmConfigurationIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef = TypedDict(
+    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
+    {
         "ClusterVersion": str,
-        "EngineFullVersion": str,
-        "SnapshotType": str,
         "NodeType": str,
-        "NumberOfNodes": int,
-        "DBName": str,
-        "VpcId": str,
-        "Encrypted": bool,
-        "KmsKeyId": str,
-        "EncryptedWithHSM": bool,
-        "AccountsWithRestoreAccess": List[AccountWithRestoreAccessTypeDef],
-        "OwnerAccount": str,
-        "TotalBackupSizeInMegaBytes": float,
-        "ActualIncrementalBackupSizeInMegaBytes": float,
-        "BackupProgressInMegaBytes": float,
-        "CurrentBackupRateInMegaBytesPerSecond": float,
-        "EstimatedSecondsToCompletion": int,
-        "ElapsedTimeInSeconds": int,
-        "SourceRegion": str,
-        "Tags": List[TagTypeDef],
-        "RestorableNodeTypes": List[str],
-        "EnhancedVpcRouting": bool,
-        "MaintenanceTrackName": str,
-        "ManualSnapshotRetentionPeriod": int,
-        "ManualSnapshotRemainingDays": int,
-        "SnapshotRetentionStartTime": datetime,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-TaggedResourceTypeDef = TypedDict(
-    "TaggedResourceTypeDef",
+DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef = TypedDict(
+    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
     {
-        "Tag": TagTypeDef,
-        "ResourceName": str,
-        "ResourceType": str,
+        "ReservedNodeId": str,
+        "ReservedNodeExchangeRequestId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-UsageLimitResponseMetadataTypeDef = TypedDict(
-    "UsageLimitResponseMetadataTypeDef",
+DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
+    {
+        "ReservedNodeOfferingId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef = TypedDict(
+    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
+    {
+        "ReservedNodeId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
+    {
+        "SnapshotCopyGrantName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef = TypedDict(
+    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
     {
-        "UsageLimitId": str,
         "ClusterIdentifier": str,
-        "FeatureType": UsageLimitFeatureTypeType,
-        "LimitType": UsageLimitLimitTypeType,
-        "Amount": int,
-        "Period": UsageLimitPeriodType,
-        "BreachAction": UsageLimitBreachActionType,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ScheduleIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-UsageLimitTypeDef = TypedDict(
-    "UsageLimitTypeDef",
+DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef = TypedDict(
+    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
     {
-        "UsageLimitId": str,
         "ClusterIdentifier": str,
-        "FeatureType": UsageLimitFeatureTypeType,
-        "LimitType": UsageLimitLimitTypeType,
-        "Amount": int,
-        "Period": UsageLimitPeriodType,
-        "BreachAction": UsageLimitBreachActionType,
-        "Tags": List[TagTypeDef],
+        "TableRestoreRequestId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeReservedNodeExchangeStatusOutputMessageTypeDef = TypedDict(
-    "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
+DescribeTagsMessageDescribeTagsPaginateTypeDef = TypedDict(
+    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
     {
-        "ReservedNodeExchangeStatusDetails": List[ReservedNodeExchangeStatusTypeDef],
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceName": str,
+        "ResourceType": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ClusterVersionsMessageTypeDef = TypedDict(
-    "ClusterVersionsMessageTypeDef",
+DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef = TypedDict(
+    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
     {
-        "Marker": str,
-        "ClusterVersions": List[ClusterVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "UsageLimitId": str,
+        "ClusterIdentifier": str,
+        "FeatureType": UsageLimitFeatureTypeType,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-DataShareResponseMetadataTypeDef = TypedDict(
-    "DataShareResponseMetadataTypeDef",
+_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
+    "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
     {
-        "DataShareArn": str,
-        "ProducerArn": str,
-        "AllowPubliclyAccessibleConsumers": bool,
-        "DataShareAssociations": List[DataShareAssociationTypeDef],
-        "ManagedBy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ActionType": ReservedNodeExchangeActionTypeType,
+    },
+)
+_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
+    "_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "SnapshotIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-DataShareTypeDef = TypedDict(
-    "DataShareTypeDef",
+class GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef(
+    _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+    _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
+    "_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
     {
-        "DataShareArn": str,
-        "ProducerArn": str,
-        "AllowPubliclyAccessibleConsumers": bool,
-        "DataShareAssociations": List[DataShareAssociationTypeDef],
-        "ManagedBy": str,
+        "ReservedNodeId": str,
+    },
+)
+_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
+    "_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef(
+    _RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
+    _OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
+):
+    pass
+
 DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageRequestTypeDef",
     {
@@ -3745,27 +3674,25 @@
     "_OptionalDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "OwnerAccount": str,
         "Filters": Sequence[NodeConfigurationOptionsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef(
     _RequiredDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
     _OptionalDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeNodeConfigurationOptionsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeNodeConfigurationOptionsMessageRequestTypeDef",
     {
         "ActionType": ActionTypeType,
     },
 )
 _OptionalDescribeNodeConfigurationOptionsMessageRequestTypeDef = TypedDict(
@@ -3778,40 +3705,38 @@
         "Filters": Sequence[NodeConfigurationOptionsFilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-
 class DescribeNodeConfigurationOptionsMessageRequestTypeDef(
     _RequiredDescribeNodeConfigurationOptionsMessageRequestTypeDef,
     _OptionalDescribeNodeConfigurationOptionsMessageRequestTypeDef,
 ):
     pass
 
-
 DescribePartnersOutputMessageTypeDef = TypedDict(
     "DescribePartnersOutputMessageTypeDef",
     {
         "PartnerIntegrationInfoList": List[PartnerIntegrationInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef = TypedDict(
     "DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef",
     {
         "ScheduledActionName": str,
         "TargetActionType": ScheduledActionTypeValuesType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Active": bool,
         "Filters": Sequence[ScheduledActionFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeScheduledActionsMessageRequestTypeDef = TypedDict(
     "DescribeScheduledActionsMessageRequestTypeDef",
     {
@@ -3828,15 +3753,15 @@
 )
 
 EndpointAuthorizationListTypeDef = TypedDict(
     "EndpointAuthorizationListTypeDef",
     {
         "EndpointAuthorizationList": List[EndpointAuthorizationTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
@@ -3846,17 +3771,46 @@
 )
 
 EventsMessageTypeDef = TypedDict(
     "EventsMessageTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+_RequiredResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ParameterGroupName": str,
     },
 )
+_OptionalResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+    total=False,
+)
+
+class ResetClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
 
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "VpcEndpointId": str,
         "VpcId": str,
         "NetworkInterfaces": List[NetworkInterfaceTypeDef],
@@ -3865,15 +3819,15 @@
 )
 
 NodeConfigurationOptionsMessageTypeDef = TypedDict(
     "NodeConfigurationOptionsMessageTypeDef",
     {
         "NodeConfigurationOptionList": List[NodeConfigurationOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedNodeOfferingTypeDef = TypedDict(
     "ReservedNodeOfferingTypeDef",
     {
         "ReservedNodeOfferingId": str,
@@ -3909,27 +3863,37 @@
     total=False,
 )
 
 RestoreTableFromClusterSnapshotResultTypeDef = TypedDict(
     "RestoreTableFromClusterSnapshotResultTypeDef",
     {
         "TableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TableRestoreStatusMessageTypeDef = TypedDict(
     "TableRestoreStatusMessageTypeDef",
     {
         "TableRestoreStatusDetails": List[TableRestoreStatusTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ScheduledActionTypeOutputTypeDef = TypedDict(
+    "ScheduledActionTypeOutputTypeDef",
+    {
+        "ResizeCluster": ResizeClusterMessageOutputTypeDef,
+        "PauseCluster": PauseClusterMessageOutputTypeDef,
+        "ResumeCluster": ResumeClusterMessageOutputTypeDef,
+    },
+    total=False,
+)
+
 ScheduledActionTypeTypeDef = TypedDict(
     "ScheduledActionTypeTypeDef",
     {
         "ResizeCluster": ResizeClusterMessageTypeDef,
         "PauseCluster": PauseClusterMessageTypeDef,
         "ResumeCluster": ResumeClusterMessageTypeDef,
     },
@@ -3946,24 +3910,24 @@
     total=False,
 )
 
 AccountAttributeListTypeDef = TypedDict(
     "AccountAttributeListTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomDomainAssociationsMessageTypeDef = TypedDict(
     "CustomDomainAssociationsMessageTypeDef",
     {
         "Marker": str,
         "Associations": List[AssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OrderableClusterOptionTypeDef = TypedDict(
     "OrderableClusterOptionTypeDef",
     {
         "ClusterVersion": str,
@@ -3985,247 +3949,247 @@
 )
 
 ClusterDbRevisionsMessageTypeDef = TypedDict(
     "ClusterDbRevisionsMessageTypeDef",
     {
         "Marker": str,
         "ClusterDbRevisions": List[ClusterDbRevisionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeDefaultClusterParametersResultTypeDef",
     {
         "DefaultClusterParameters": DefaultClusterParametersTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterParameterGroupsMessageTypeDef = TypedDict(
     "ClusterParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "ParameterGroups": List[ClusterParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterParameterGroupResultTypeDef = TypedDict(
     "CreateClusterParameterGroupResultTypeDef",
     {
         "ClusterParameterGroup": ClusterParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEventSubscriptionResultTypeDef = TypedDict(
     "CreateEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventSubscriptionsMessageTypeDef = TypedDict(
     "EventSubscriptionsMessageTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyEventSubscriptionResultTypeDef = TypedDict(
     "ModifyEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHsmClientCertificateResultTypeDef = TypedDict(
     "CreateHsmClientCertificateResultTypeDef",
     {
         "HsmClientCertificate": HsmClientCertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HsmClientCertificateMessageTypeDef = TypedDict(
     "HsmClientCertificateMessageTypeDef",
     {
         "Marker": str,
         "HsmClientCertificates": List[HsmClientCertificateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHsmConfigurationResultTypeDef = TypedDict(
     "CreateHsmConfigurationResultTypeDef",
     {
         "HsmConfiguration": HsmConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HsmConfigurationMessageTypeDef = TypedDict(
     "HsmConfigurationMessageTypeDef",
     {
         "Marker": str,
         "HsmConfigurations": List[HsmConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSecurityGroupTypeDef = TypedDict(
     "ClusterSecurityGroupTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "Description": str,
         "EC2SecurityGroups": List[EC2SecurityGroupTypeDef],
         "IPRanges": List[IPRangeTypeDef],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 CreateSnapshotCopyGrantResultTypeDef = TypedDict(
     "CreateSnapshotCopyGrantResultTypeDef",
     {
         "SnapshotCopyGrant": SnapshotCopyGrantTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SnapshotCopyGrantMessageTypeDef = TypedDict(
     "SnapshotCopyGrantMessageTypeDef",
     {
         "Marker": str,
         "SnapshotCopyGrants": List[SnapshotCopyGrantTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSnapshotSchedulesOutputMessageTypeDef = TypedDict(
     "DescribeSnapshotSchedulesOutputMessageTypeDef",
     {
         "SnapshotSchedules": List[SnapshotScheduleTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthorizeSnapshotAccessResultTypeDef = TypedDict(
     "AuthorizeSnapshotAccessResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyClusterSnapshotResultTypeDef = TypedDict(
     "CopyClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterSnapshotResultTypeDef = TypedDict(
     "CreateClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterSnapshotResultTypeDef = TypedDict(
     "DeleteClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterSnapshotResultTypeDef = TypedDict(
     "ModifyClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RevokeSnapshotAccessResultTypeDef = TypedDict(
     "RevokeSnapshotAccessResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SnapshotMessageTypeDef = TypedDict(
     "SnapshotMessageTypeDef",
     {
         "Marker": str,
         "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaggedResourceListMessageTypeDef = TypedDict(
     "TaggedResourceListMessageTypeDef",
     {
         "TaggedResources": List[TaggedResourceTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UsageLimitListTypeDef = TypedDict(
     "UsageLimitListTypeDef",
     {
         "UsageLimits": List[UsageLimitTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSharesForConsumerResultTypeDef = TypedDict(
     "DescribeDataSharesForConsumerResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSharesForProducerResultTypeDef = TypedDict(
     "DescribeDataSharesForProducerResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSharesResultTypeDef = TypedDict(
     "DescribeDataSharesResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventCategoriesMessageTypeDef = TypedDict(
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointAccessResponseMetadataTypeDef = TypedDict(
     "EndpointAccessResponseMetadataTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4234,15 +4198,15 @@
         "EndpointStatus": str,
         "EndpointName": str,
         "EndpointCreateTime": datetime,
         "Port": int,
         "Address": str,
         "VpcSecurityGroups": List[VpcSecurityGroupMembershipTypeDef],
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointAccessTypeDef = TypedDict(
     "EndpointAccessTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4270,40 +4234,40 @@
 )
 
 GetReservedNodeExchangeOfferingsOutputMessageTypeDef = TypedDict(
     "GetReservedNodeExchangeOfferingsOutputMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeOfferings": List[ReservedNodeOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedNodeOfferingsMessageTypeDef = TypedDict(
     "ReservedNodeOfferingsMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeOfferings": List[ReservedNodeOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptReservedNodeExchangeOutputMessageTypeDef = TypedDict(
     "AcceptReservedNodeExchangeOutputMessageTypeDef",
     {
         "ExchangedReservedNode": ReservedNodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PurchaseReservedNodeOfferingResultTypeDef = TypedDict(
     "PurchaseReservedNodeOfferingResultTypeDef",
     {
         "ReservedNode": ReservedNodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedNodeConfigurationOptionTypeDef = TypedDict(
     "ReservedNodeConfigurationOptionTypeDef",
     {
         "SourceReservedNode": ReservedNodeTypeDef,
@@ -4314,18 +4278,50 @@
 )
 
 ReservedNodesMessageTypeDef = TypedDict(
     "ReservedNodesMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodes": List[ReservedNodeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ScheduledActionResponseMetadataTypeDef = TypedDict(
+    "ScheduledActionResponseMetadataTypeDef",
+    {
+        "ScheduledActionName": str,
+        "TargetAction": ScheduledActionTypeOutputTypeDef,
+        "Schedule": str,
+        "IamRole": str,
+        "ScheduledActionDescription": str,
+        "State": ScheduledActionStateType,
+        "NextInvocations": List[datetime],
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ScheduledActionTypeDef = TypedDict(
+    "ScheduledActionTypeDef",
+    {
+        "ScheduledActionName": str,
+        "TargetAction": ScheduledActionTypeOutputTypeDef,
+        "Schedule": str,
+        "IamRole": str,
+        "ScheduledActionDescription": str,
+        "State": ScheduledActionStateType,
+        "NextInvocations": List[datetime],
+        "StartTime": datetime,
+        "EndTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredCreateScheduledActionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
         "TargetAction": ScheduledActionTypeTypeDef,
         "Schedule": str,
         "IamRole": str,
@@ -4338,22 +4334,20 @@
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Enable": bool,
     },
     total=False,
 )
 
-
 class CreateScheduledActionMessageRequestTypeDef(
     _RequiredCreateScheduledActionMessageRequestTypeDef,
     _OptionalCreateScheduledActionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyScheduledActionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
     },
 )
 _OptionalModifyScheduledActionMessageRequestTypeDef = TypedDict(
@@ -4366,54 +4360,20 @@
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Enable": bool,
     },
     total=False,
 )
 
-
 class ModifyScheduledActionMessageRequestTypeDef(
     _RequiredModifyScheduledActionMessageRequestTypeDef,
     _OptionalModifyScheduledActionMessageRequestTypeDef,
 ):
     pass
 
-
-ScheduledActionResponseMetadataTypeDef = TypedDict(
-    "ScheduledActionResponseMetadataTypeDef",
-    {
-        "ScheduledActionName": str,
-        "TargetAction": ScheduledActionTypeTypeDef,
-        "Schedule": str,
-        "IamRole": str,
-        "ScheduledActionDescription": str,
-        "State": ScheduledActionStateType,
-        "NextInvocations": List[datetime],
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ScheduledActionTypeDef = TypedDict(
-    "ScheduledActionTypeDef",
-    {
-        "ScheduledActionName": str,
-        "TargetAction": ScheduledActionTypeTypeDef,
-        "Schedule": str,
-        "IamRole": str,
-        "ScheduledActionDescription": str,
-        "State": ScheduledActionStateType,
-        "NextInvocations": List[datetime],
-        "StartTime": datetime,
-        "EndTime": datetime,
-    },
-    total=False,
-)
-
 MaintenanceTrackTypeDef = TypedDict(
     "MaintenanceTrackTypeDef",
     {
         "MaintenanceTrackName": str,
         "DatabaseVersion": str,
         "UpdateTargets": List[UpdateTargetTypeDef],
     },
@@ -4421,70 +4381,70 @@
 )
 
 OrderableClusterOptionsMessageTypeDef = TypedDict(
     "OrderableClusterOptionsMessageTypeDef",
     {
         "OrderableClusterOptions": List[OrderableClusterOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSubnetGroupTypeDef = TypedDict(
     "ClusterSubnetGroupTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "Description": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[SubnetTypeDef],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 AuthorizeClusterSecurityGroupIngressResultTypeDef = TypedDict(
     "AuthorizeClusterSecurityGroupIngressResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSecurityGroupMessageTypeDef = TypedDict(
     "ClusterSecurityGroupMessageTypeDef",
     {
         "Marker": str,
         "ClusterSecurityGroups": List[ClusterSecurityGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterSecurityGroupResultTypeDef = TypedDict(
     "CreateClusterSecurityGroupResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RevokeClusterSecurityGroupIngressResultTypeDef = TypedDict(
     "RevokeClusterSecurityGroupIngressResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointAccessListTypeDef = TypedDict(
     "EndpointAccessListTypeDef",
     {
         "EndpointAccessList": List[EndpointAccessTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4515,15 +4475,15 @@
         "DataTransferProgress": DataTransferProgressTypeDef,
         "HsmStatus": HsmStatusTypeDef,
         "ClusterSnapshotCopyStatus": ClusterSnapshotCopyStatusTypeDef,
         "ClusterPublicKey": str,
         "ClusterNodes": List[ClusterNodeTypeDef],
         "ElasticIpStatus": ElasticIpStatusTypeDef,
         "ClusterRevisionNumber": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "KmsKeyId": str,
         "EnhancedVpcRouting": bool,
         "IamRoles": List[ClusterIamRoleTypeDef],
         "PendingActions": List[str],
         "MaintenanceTrackName": str,
         "ElasticResizeNumberOfNodeOptions": str,
         "DeferredMaintenanceWindows": List[DeferredMaintenanceWindowTypeDef],
@@ -4547,182 +4507,182 @@
 )
 
 GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef = TypedDict(
     "GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeConfigurationOptionList": List[ReservedNodeConfigurationOptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScheduledActionsMessageTypeDef = TypedDict(
     "ScheduledActionsMessageTypeDef",
     {
         "Marker": str,
         "ScheduledActions": List[ScheduledActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrackListMessageTypeDef = TypedDict(
     "TrackListMessageTypeDef",
     {
         "MaintenanceTracks": List[MaintenanceTrackTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSubnetGroupMessageTypeDef = TypedDict(
     "ClusterSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "ClusterSubnetGroups": List[ClusterSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterSubnetGroupResultTypeDef = TypedDict(
     "CreateClusterSubnetGroupResultTypeDef",
     {
         "ClusterSubnetGroup": ClusterSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterSubnetGroupResultTypeDef = TypedDict(
     "ModifyClusterSubnetGroupResultTypeDef",
     {
         "ClusterSubnetGroup": ClusterSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClustersMessageTypeDef = TypedDict(
     "ClustersMessageTypeDef",
     {
         "Marker": str,
         "Clusters": List[ClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResultTypeDef = TypedDict(
     "CreateClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResultTypeDef = TypedDict(
     "DeleteClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisableSnapshotCopyResultTypeDef = TypedDict(
     "DisableSnapshotCopyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnableSnapshotCopyResultTypeDef = TypedDict(
     "EnableSnapshotCopyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterDbRevisionResultTypeDef = TypedDict(
     "ModifyClusterDbRevisionResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterIamRolesResultTypeDef = TypedDict(
     "ModifyClusterIamRolesResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterMaintenanceResultTypeDef = TypedDict(
     "ModifyClusterMaintenanceResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterResultTypeDef = TypedDict(
     "ModifyClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifySnapshotCopyRetentionPeriodResultTypeDef = TypedDict(
     "ModifySnapshotCopyRetentionPeriodResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PauseClusterResultTypeDef = TypedDict(
     "PauseClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootClusterResultTypeDef = TypedDict(
     "RebootClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResizeClusterResultTypeDef = TypedDict(
     "ResizeClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreFromClusterSnapshotResultTypeDef = TypedDict(
     "RestoreFromClusterSnapshotResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResumeClusterResultTypeDef = TypedDict(
     "ResumeClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RotateEncryptionKeyResultTypeDef = TypedDict(
     "RotateEncryptionKeyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/type_defs.pyi` & `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/type_defs.py`

 * *Files 20% similar despite different names*

```diff
@@ -47,16 +47,18 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptReservedNodeExchangeInputMessageRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AttributeValueTargetTypeDef",
     "AccountWithRestoreAccessTypeDef",
     "AquaConfigurationTypeDef",
     "AssociateDataShareConsumerMessageRequestTypeDef",
     "CertificateAssociationTypeDef",
     "AuthenticationProfileTypeDef",
     "AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef",
@@ -65,46 +67,40 @@
     "AuthorizeSnapshotAccessMessageRequestTypeDef",
     "SupportedPlatformTypeDef",
     "DeleteClusterSnapshotMessageTypeDef",
     "SnapshotErrorMessageTypeDef",
     "BatchModifyClusterSnapshotsMessageRequestTypeDef",
     "CancelResizeMessageRequestTypeDef",
     "ClusterAssociatedToScheduleTypeDef",
-    "ClusterCredentialsTypeDef",
     "RevisionTargetTypeDef",
-    "ClusterExtendedCredentialsTypeDef",
     "ClusterIamRoleTypeDef",
     "ClusterNodeTypeDef",
-    "ParameterTypeDef",
-    "ClusterParameterGroupNameMessageTypeDef",
+    "ParameterOutputTypeDef",
     "ClusterParameterStatusTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "ClusterSecurityGroupMembershipTypeDef",
     "ClusterSnapshotCopyStatusTypeDef",
     "DataTransferProgressTypeDef",
     "DeferredMaintenanceWindowTypeDef",
     "ElasticIpStatusTypeDef",
     "HsmStatusTypeDef",
     "PendingModifiedValuesTypeDef",
     "ReservedNodeExchangeStatusTypeDef",
     "ResizeInfoTypeDef",
     "RestoreStatusTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ClusterVersionTypeDef",
     "CopyClusterSnapshotMessageRequestTypeDef",
     "CreateAuthenticationProfileMessageRequestTypeDef",
-    "CreateAuthenticationProfileResultTypeDef",
+    "TagTypeDef",
     "CreateCustomDomainAssociationMessageRequestTypeDef",
-    "CreateCustomDomainAssociationResultTypeDef",
     "CreateEndpointAccessMessageRequestTypeDef",
-    "CustomerStorageMessageTypeDef",
     "DataShareAssociationTypeDef",
     "DeauthorizeDataShareMessageRequestTypeDef",
     "DeleteAuthenticationProfileMessageRequestTypeDef",
-    "DeleteAuthenticationProfileResultTypeDef",
     "DeleteClusterMessageRequestTypeDef",
     "DeleteClusterParameterGroupMessageRequestTypeDef",
     "DeleteClusterSecurityGroupMessageRequestTypeDef",
     "DeleteClusterSnapshotMessageRequestTypeDef",
     "DeleteClusterSubnetGroupMessageRequestTypeDef",
     "DeleteCustomDomainAssociationMessageRequestTypeDef",
     "DeleteEndpointAccessMessageRequestTypeDef",
@@ -114,202 +110,213 @@
     "DeleteScheduledActionMessageRequestTypeDef",
     "DeleteSnapshotCopyGrantMessageRequestTypeDef",
     "DeleteSnapshotScheduleMessageRequestTypeDef",
     "DeleteTagsMessageRequestTypeDef",
     "DeleteUsageLimitMessageRequestTypeDef",
     "DescribeAccountAttributesMessageRequestTypeDef",
     "DescribeAuthenticationProfilesMessageRequestTypeDef",
-    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeClusterDbRevisionsMessageRequestTypeDef",
-    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
     "DescribeClusterParameterGroupsMessageRequestTypeDef",
-    "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
     "DescribeClusterParametersMessageRequestTypeDef",
-    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
     "DescribeClusterSecurityGroupsMessageRequestTypeDef",
     "SnapshotSortingEntityTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
     "DescribeClusterSubnetGroupsMessageRequestTypeDef",
-    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
     "DescribeClusterTracksMessageRequestTypeDef",
-    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
     "DescribeClusterVersionsMessageRequestTypeDef",
-    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
     "DescribeClustersMessageRequestTypeDef",
-    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
     "DescribeCustomDomainAssociationsMessageRequestTypeDef",
-    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
     "DescribeDataSharesForConsumerMessageRequestTypeDef",
-    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
     "DescribeDataSharesForProducerMessageRequestTypeDef",
-    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
     "DescribeDataSharesMessageRequestTypeDef",
-    "DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
     "DescribeDefaultClusterParametersMessageRequestTypeDef",
-    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
     "DescribeEndpointAccessMessageRequestTypeDef",
-    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
     "DescribeEndpointAuthorizationMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
-    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
-    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
     "DescribeHsmConfigurationsMessageRequestTypeDef",
     "DescribeLoggingStatusMessageRequestTypeDef",
     "NodeConfigurationOptionsFilterTypeDef",
-    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
     "DescribeOrderableClusterOptionsMessageRequestTypeDef",
     "DescribePartnersInputMessageRequestTypeDef",
     "PartnerIntegrationInfoTypeDef",
-    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
     "DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef",
-    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
     "DescribeReservedNodeOfferingsMessageRequestTypeDef",
-    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
     "DescribeReservedNodesMessageRequestTypeDef",
     "DescribeResizeMessageRequestTypeDef",
     "ScheduledActionFilterTypeDef",
-    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
     "DescribeSnapshotCopyGrantsMessageRequestTypeDef",
-    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
     "DescribeSnapshotSchedulesMessageRequestTypeDef",
-    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
     "DescribeTableRestoreStatusMessageRequestTypeDef",
-    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
     "DescribeTagsMessageRequestTypeDef",
-    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
     "DescribeUsageLimitsMessageRequestTypeDef",
     "DisableLoggingMessageRequestTypeDef",
     "DisableSnapshotCopyMessageRequestTypeDef",
     "DisassociateDataShareConsumerMessageRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableLoggingMessageRequestTypeDef",
     "EnableSnapshotCopyMessageRequestTypeDef",
     "EndpointAuthorizationTypeDef",
-    "EndpointAuthorizationResponseMetadataTypeDef",
     "EventInfoMapTypeDef",
     "EventTypeDef",
     "GetClusterCredentialsMessageRequestTypeDef",
     "GetClusterCredentialsWithIAMMessageRequestTypeDef",
-    "GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
     "GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef",
-    "GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
     "GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
-    "LoggingStatusTypeDef",
     "ModifyAquaInputMessageRequestTypeDef",
     "ModifyAuthenticationProfileMessageRequestTypeDef",
-    "ModifyAuthenticationProfileResultTypeDef",
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     "ModifyClusterIamRolesMessageRequestTypeDef",
     "ModifyClusterMaintenanceMessageRequestTypeDef",
     "ModifyClusterMessageRequestTypeDef",
+    "ParameterTypeDef",
     "ModifyClusterSnapshotMessageRequestTypeDef",
     "ModifyClusterSnapshotScheduleMessageRequestTypeDef",
     "ModifyClusterSubnetGroupMessageRequestTypeDef",
     "ModifyCustomDomainAssociationMessageRequestTypeDef",
-    "ModifyCustomDomainAssociationResultTypeDef",
     "ModifyEndpointAccessMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     "ModifySnapshotScheduleMessageRequestTypeDef",
     "ModifyUsageLimitMessageRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "NodeConfigurationOptionTypeDef",
-    "PaginatorConfigTypeDef",
     "PartnerIntegrationInputMessageRequestTypeDef",
-    "PartnerIntegrationOutputMessageTypeDef",
+    "PauseClusterMessageOutputTypeDef",
     "PauseClusterMessageRequestTypeDef",
     "PauseClusterMessageTypeDef",
     "PurchaseReservedNodeOfferingMessageRequestTypeDef",
     "RebootClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RejectDataShareMessageRequestTypeDef",
+    "ResizeClusterMessageOutputTypeDef",
     "ResizeClusterMessageRequestTypeDef",
     "ResizeClusterMessageTypeDef",
-    "ResizeProgressMessageTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreFromClusterSnapshotMessageRequestTypeDef",
     "RestoreTableFromClusterSnapshotMessageRequestTypeDef",
     "TableRestoreStatusTypeDef",
+    "ResumeClusterMessageOutputTypeDef",
     "ResumeClusterMessageRequestTypeDef",
     "ResumeClusterMessageTypeDef",
     "RevokeClusterSecurityGroupIngressMessageRequestTypeDef",
     "RevokeEndpointAccessMessageRequestTypeDef",
     "RevokeSnapshotAccessMessageRequestTypeDef",
     "RotateEncryptionKeyMessageRequestTypeDef",
     "SupportedOperationTypeDef",
     "UpdatePartnerStatusInputMessageRequestTypeDef",
+    "ClusterCredentialsTypeDef",
+    "ClusterExtendedCredentialsTypeDef",
+    "ClusterParameterGroupNameMessageTypeDef",
+    "CreateAuthenticationProfileResultTypeDef",
+    "CreateCustomDomainAssociationResultTypeDef",
+    "CustomerStorageMessageTypeDef",
+    "DeleteAuthenticationProfileResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EndpointAuthorizationResponseMetadataTypeDef",
+    "LoggingStatusTypeDef",
+    "ModifyAuthenticationProfileResultTypeDef",
+    "ModifyCustomDomainAssociationResultTypeDef",
+    "PartnerIntegrationOutputMessageTypeDef",
+    "ResizeProgressMessageTypeDef",
     "AccountAttributeTypeDef",
     "ModifyAquaOutputMessageTypeDef",
     "AssociationTypeDef",
     "DescribeAuthenticationProfilesResultTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchDeleteClusterSnapshotsRequestRequestTypeDef",
     "BatchDeleteClusterSnapshotsResultTypeDef",
     "BatchModifyClusterSnapshotsOutputMessageTypeDef",
     "ClusterDbRevisionTypeDef",
     "ClusterParameterGroupDetailsTypeDef",
     "DefaultClusterParametersTypeDef",
-    "ModifyClusterParameterGroupMessageRequestTypeDef",
-    "ResetClusterParameterGroupMessageRequestTypeDef",
     "ClusterParameterGroupStatusTypeDef",
     "ClusterParameterGroupTypeDef",
-    "CreateClusterMessageRequestTypeDef",
-    "CreateClusterParameterGroupMessageRequestTypeDef",
-    "CreateClusterSecurityGroupMessageRequestTypeDef",
-    "CreateClusterSnapshotMessageRequestTypeDef",
-    "CreateClusterSubnetGroupMessageRequestTypeDef",
-    "CreateEventSubscriptionMessageRequestTypeDef",
-    "CreateHsmClientCertificateMessageRequestTypeDef",
-    "CreateHsmConfigurationMessageRequestTypeDef",
-    "CreateSnapshotCopyGrantMessageRequestTypeDef",
-    "CreateSnapshotScheduleMessageRequestTypeDef",
-    "CreateTagsMessageRequestTypeDef",
-    "CreateUsageLimitMessageRequestTypeDef",
     "EC2SecurityGroupTypeDef",
     "EventSubscriptionTypeDef",
     "HsmClientCertificateTypeDef",
     "HsmConfigurationTypeDef",
     "IPRangeTypeDef",
     "SnapshotCopyGrantTypeDef",
     "SnapshotScheduleResponseMetadataTypeDef",
     "SnapshotScheduleTypeDef",
     "SnapshotTypeDef",
     "TaggedResourceTypeDef",
     "UsageLimitResponseMetadataTypeDef",
     "UsageLimitTypeDef",
     "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
     "ClusterVersionsMessageTypeDef",
+    "CreateClusterMessageRequestTypeDef",
+    "CreateClusterParameterGroupMessageRequestTypeDef",
+    "CreateClusterSecurityGroupMessageRequestTypeDef",
+    "CreateClusterSnapshotMessageRequestTypeDef",
+    "CreateClusterSubnetGroupMessageRequestTypeDef",
+    "CreateEventSubscriptionMessageRequestTypeDef",
+    "CreateHsmClientCertificateMessageRequestTypeDef",
+    "CreateHsmConfigurationMessageRequestTypeDef",
+    "CreateSnapshotCopyGrantMessageRequestTypeDef",
+    "CreateSnapshotScheduleMessageRequestTypeDef",
+    "CreateTagsMessageRequestTypeDef",
+    "CreateUsageLimitMessageRequestTypeDef",
     "DataShareResponseMetadataTypeDef",
     "DataShareTypeDef",
+    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
+    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
+    "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
+    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
+    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
+    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
+    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
+    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
+    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
+    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
+    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
+    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
+    "DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
+    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
+    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
+    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
+    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
+    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
+    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
+    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
+    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
+    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
+    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
+    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
+    "GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
+    "GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
     "DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef",
     "DescribeClusterSnapshotsMessageRequestTypeDef",
     "DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef",
     "DescribeClustersMessageClusterAvailableWaitTypeDef",
     "DescribeClustersMessageClusterDeletedWaitTypeDef",
     "DescribeClustersMessageClusterRestoredWaitTypeDef",
     "DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef",
     "DescribeNodeConfigurationOptionsMessageRequestTypeDef",
     "DescribePartnersOutputMessageTypeDef",
     "DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsMessageRequestTypeDef",
     "EndpointAuthorizationListTypeDef",
     "EventCategoriesMapTypeDef",
     "EventsMessageTypeDef",
+    "ModifyClusterParameterGroupMessageRequestTypeDef",
+    "ResetClusterParameterGroupMessageRequestTypeDef",
     "VpcEndpointTypeDef",
     "NodeConfigurationOptionsMessageTypeDef",
     "ReservedNodeOfferingTypeDef",
     "ReservedNodeTypeDef",
     "RestoreTableFromClusterSnapshotResultTypeDef",
     "TableRestoreStatusMessageTypeDef",
+    "ScheduledActionTypeOutputTypeDef",
     "ScheduledActionTypeTypeDef",
     "UpdateTargetTypeDef",
     "AccountAttributeListTypeDef",
     "CustomDomainAssociationsMessageTypeDef",
     "OrderableClusterOptionTypeDef",
     "SubnetTypeDef",
     "ClusterDbRevisionsMessageTypeDef",
@@ -345,18 +352,18 @@
     "EndpointTypeDef",
     "GetReservedNodeExchangeOfferingsOutputMessageTypeDef",
     "ReservedNodeOfferingsMessageTypeDef",
     "AcceptReservedNodeExchangeOutputMessageTypeDef",
     "PurchaseReservedNodeOfferingResultTypeDef",
     "ReservedNodeConfigurationOptionTypeDef",
     "ReservedNodesMessageTypeDef",
-    "CreateScheduledActionMessageRequestTypeDef",
-    "ModifyScheduledActionMessageRequestTypeDef",
     "ScheduledActionResponseMetadataTypeDef",
     "ScheduledActionTypeDef",
+    "CreateScheduledActionMessageRequestTypeDef",
+    "ModifyScheduledActionMessageRequestTypeDef",
     "MaintenanceTrackTypeDef",
     "OrderableClusterOptionsMessageTypeDef",
     "ClusterSubnetGroupTypeDef",
     "AuthorizeClusterSecurityGroupIngressResultTypeDef",
     "ClusterSecurityGroupMessageTypeDef",
     "CreateClusterSecurityGroupResultTypeDef",
     "RevokeClusterSecurityGroupIngressResultTypeDef",
@@ -390,14 +397,25 @@
     "AcceptReservedNodeExchangeInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
     },
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
 AttributeValueTargetTypeDef = TypedDict(
     "AttributeValueTargetTypeDef",
     {
         "AttributeValue": str,
     },
     total=False,
 )
@@ -432,20 +450,22 @@
         "AssociateEntireAccount": bool,
         "ConsumerArn": str,
         "ConsumerRegion": str,
     },
     total=False,
 )
 
+
 class AssociateDataShareConsumerMessageRequestTypeDef(
     _RequiredAssociateDataShareConsumerMessageRequestTypeDef,
     _OptionalAssociateDataShareConsumerMessageRequestTypeDef,
 ):
     pass
 
+
 CertificateAssociationTypeDef = TypedDict(
     "CertificateAssociationTypeDef",
     {
         "CustomDomainName": str,
         "ClusterIdentifier": str,
     },
     total=False,
@@ -472,20 +492,22 @@
         "CIDRIP": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+
 class AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef(
     _RequiredAuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
     _OptionalAuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
+
 AuthorizeDataShareMessageRequestTypeDef = TypedDict(
     "AuthorizeDataShareMessageRequestTypeDef",
     {
         "DataShareArn": str,
         "ConsumerIdentifier": str,
     },
 )
@@ -501,20 +523,22 @@
     {
         "ClusterIdentifier": str,
         "VpcIds": Sequence[str],
     },
     total=False,
 )
 
+
 class AuthorizeEndpointAccessMessageRequestTypeDef(
     _RequiredAuthorizeEndpointAccessMessageRequestTypeDef,
     _OptionalAuthorizeEndpointAccessMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredAuthorizeSnapshotAccessMessageRequestTypeDef = TypedDict(
     "_RequiredAuthorizeSnapshotAccessMessageRequestTypeDef",
     {
         "AccountWithRestoreAccess": str,
     },
 )
 _OptionalAuthorizeSnapshotAccessMessageRequestTypeDef = TypedDict(
@@ -523,20 +547,22 @@
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
+
 class AuthorizeSnapshotAccessMessageRequestTypeDef(
     _RequiredAuthorizeSnapshotAccessMessageRequestTypeDef,
     _OptionalAuthorizeSnapshotAccessMessageRequestTypeDef,
 ):
     pass
 
+
 SupportedPlatformTypeDef = TypedDict(
     "SupportedPlatformTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -551,19 +577,21 @@
     "_OptionalDeleteClusterSnapshotMessageTypeDef",
     {
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
+
 class DeleteClusterSnapshotMessageTypeDef(
     _RequiredDeleteClusterSnapshotMessageTypeDef, _OptionalDeleteClusterSnapshotMessageTypeDef
 ):
     pass
 
+
 SnapshotErrorMessageTypeDef = TypedDict(
     "SnapshotErrorMessageTypeDef",
     {
         "SnapshotIdentifier": str,
         "SnapshotClusterIdentifier": str,
         "FailureCode": str,
         "FailureReason": str,
@@ -582,20 +610,22 @@
     {
         "ManualSnapshotRetentionPeriod": int,
         "Force": bool,
     },
     total=False,
 )
 
+
 class BatchModifyClusterSnapshotsMessageRequestTypeDef(
     _RequiredBatchModifyClusterSnapshotsMessageRequestTypeDef,
     _OptionalBatchModifyClusterSnapshotsMessageRequestTypeDef,
 ):
     pass
 
+
 CancelResizeMessageRequestTypeDef = TypedDict(
     "CancelResizeMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -604,45 +634,24 @@
     {
         "ClusterIdentifier": str,
         "ScheduleAssociationState": ScheduleStateType,
     },
     total=False,
 )
 
-ClusterCredentialsTypeDef = TypedDict(
-    "ClusterCredentialsTypeDef",
-    {
-        "DbUser": str,
-        "DbPassword": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RevisionTargetTypeDef = TypedDict(
     "RevisionTargetTypeDef",
     {
         "DatabaseRevision": str,
         "Description": str,
         "DatabaseRevisionReleaseDate": datetime,
     },
     total=False,
 )
 
-ClusterExtendedCredentialsTypeDef = TypedDict(
-    "ClusterExtendedCredentialsTypeDef",
-    {
-        "DbUser": str,
-        "DbPassword": str,
-        "Expiration": datetime,
-        "NextRefreshTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ClusterIamRoleTypeDef = TypedDict(
     "ClusterIamRoleTypeDef",
     {
         "IamRoleArn": str,
         "ApplyStatus": str,
     },
     total=False,
@@ -654,51 +663,42 @@
         "NodeRole": str,
         "PrivateIPAddress": str,
         "PublicIPAddress": str,
     },
     total=False,
 )
 
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
         "Description": str,
         "Source": str,
         "DataType": str,
         "AllowedValues": str,
         "ApplyType": ParameterApplyTypeType,
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
     },
     total=False,
 )
 
-ClusterParameterGroupNameMessageTypeDef = TypedDict(
-    "ClusterParameterGroupNameMessageTypeDef",
-    {
-        "ParameterGroupName": str,
-        "ParameterGroupStatus": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ClusterParameterStatusTypeDef = TypedDict(
     "ClusterParameterStatusTypeDef",
     {
         "ParameterName": str,
         "ParameterApplyStatus": str,
         "ParameterApplyErrorDescription": str,
     },
     total=False,
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
@@ -851,57 +851,48 @@
     {
         "SourceSnapshotClusterIdentifier": str,
         "ManualSnapshotRetentionPeriod": int,
     },
     total=False,
 )
 
+
 class CopyClusterSnapshotMessageRequestTypeDef(
     _RequiredCopyClusterSnapshotMessageRequestTypeDef,
     _OptionalCopyClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 CreateAuthenticationProfileMessageRequestTypeDef = TypedDict(
     "CreateAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
 )
 
-CreateAuthenticationProfileResultTypeDef = TypedDict(
-    "CreateAuthenticationProfileResultTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "AuthenticationProfileName": str,
-        "AuthenticationProfileContent": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Value": str,
     },
+    total=False,
 )
 
 CreateCustomDomainAssociationMessageRequestTypeDef = TypedDict(
     "CreateCustomDomainAssociationMessageRequestTypeDef",
     {
         "CustomDomainName": str,
         "CustomDomainCertificateArn": str,
         "ClusterIdentifier": str,
     },
 )
 
-CreateCustomDomainAssociationResultTypeDef = TypedDict(
-    "CreateCustomDomainAssociationResultTypeDef",
-    {
-        "CustomDomainName": str,
-        "CustomDomainCertificateArn": str,
-        "ClusterIdentifier": str,
-        "CustomDomainCertExpiryTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateEndpointAccessMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointAccessMessageRequestTypeDef",
     {
         "EndpointName": str,
         "SubnetGroupName": str,
     },
 )
@@ -911,28 +902,21 @@
         "ClusterIdentifier": str,
         "ResourceOwner": str,
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateEndpointAccessMessageRequestTypeDef(
     _RequiredCreateEndpointAccessMessageRequestTypeDef,
     _OptionalCreateEndpointAccessMessageRequestTypeDef,
 ):
     pass
 
-CustomerStorageMessageTypeDef = TypedDict(
-    "CustomerStorageMessageTypeDef",
-    {
-        "TotalBackupSizeInMegaBytes": float,
-        "TotalProvisionedStorageInMegaBytes": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DataShareAssociationTypeDef = TypedDict(
     "DataShareAssociationTypeDef",
     {
         "ConsumerIdentifier": str,
         "Status": DataShareStatusType,
         "ConsumerRegion": str,
@@ -953,22 +937,14 @@
 DeleteAuthenticationProfileMessageRequestTypeDef = TypedDict(
     "DeleteAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
     },
 )
 
-DeleteAuthenticationProfileResultTypeDef = TypedDict(
-    "DeleteAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalDeleteClusterMessageRequestTypeDef = TypedDict(
@@ -977,19 +953,21 @@
         "SkipFinalClusterSnapshot": bool,
         "FinalClusterSnapshotIdentifier": str,
         "FinalClusterSnapshotRetentionPeriod": int,
     },
     total=False,
 )
 
+
 class DeleteClusterMessageRequestTypeDef(
     _RequiredDeleteClusterMessageRequestTypeDef, _OptionalDeleteClusterMessageRequestTypeDef
 ):
     pass
 
+
 DeleteClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteClusterParameterGroupMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 
@@ -1010,20 +988,22 @@
     "_OptionalDeleteClusterSnapshotMessageRequestTypeDef",
     {
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
+
 class DeleteClusterSnapshotMessageRequestTypeDef(
     _RequiredDeleteClusterSnapshotMessageRequestTypeDef,
     _OptionalDeleteClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 DeleteClusterSubnetGroupMessageRequestTypeDef = TypedDict(
     "DeleteClusterSubnetGroupMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
     },
 )
 
@@ -1110,77 +1090,46 @@
     "DescribeAuthenticationProfilesMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
     },
     total=False,
 )
 
-DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef = TypedDict(
-    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ClusterIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeClusterDbRevisionsMessageRequestTypeDef = TypedDict(
     "DescribeClusterDbRevisionsMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterParameterGroupsMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-    },
-)
-_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef(
-    _RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
-    _OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeClusterParametersMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalDescribeClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1189,30 +1138,21 @@
         "Source": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeClusterParametersMessageRequestTypeDef(
     _RequiredDescribeClusterParametersMessageRequestTypeDef,
     _OptionalDescribeClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
-    {
-        "ClusterSecurityGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 DescribeClusterSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSecurityGroupsMessageRequestTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "MaxRecords": int,
         "Marker": str,
@@ -1232,216 +1172,118 @@
     "_OptionalSnapshotSortingEntityTypeDef",
     {
         "SortOrder": SortByOrderType,
     },
     total=False,
 )
 
+
 class SnapshotSortingEntityTypeDef(
     _RequiredSnapshotSortingEntityTypeDef, _OptionalSnapshotSortingEntityTypeDef
 ):
     pass
 
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
-    {
-        "ClusterSubnetGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSubnetGroupsMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef = TypedDict(
-    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
-    {
-        "MaintenanceTrackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterTracksMessageRequestTypeDef = TypedDict(
     "DescribeClusterTracksMessageRequestTypeDef",
     {
         "MaintenanceTrackName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef = TypedDict(
-    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
-    {
-        "ClusterVersion": str,
-        "ClusterParameterGroupFamily": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterVersionsMessageRequestTypeDef = TypedDict(
     "DescribeClusterVersionsMessageRequestTypeDef",
     {
         "ClusterVersion": str,
         "ClusterParameterGroupFamily": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeClustersMessageDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClustersMessageRequestTypeDef = TypedDict(
     "DescribeClustersMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef = TypedDict(
-    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
-    {
-        "CustomDomainName": str,
-        "CustomDomainCertificateArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCustomDomainAssociationsMessageRequestTypeDef = TypedDict(
     "DescribeCustomDomainAssociationsMessageRequestTypeDef",
     {
         "CustomDomainName": str,
         "CustomDomainCertificateArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef = TypedDict(
-    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
-    {
-        "ConsumerArn": str,
-        "Status": DataShareStatusForConsumerType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSharesForConsumerMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesForConsumerMessageRequestTypeDef",
     {
         "ConsumerArn": str,
         "Status": DataShareStatusForConsumerType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef = TypedDict(
-    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
-    {
-        "ProducerArn": str,
-        "Status": DataShareStatusForProducerType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSharesForProducerMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesForProducerMessageRequestTypeDef",
     {
         "ProducerArn": str,
         "Status": DataShareStatusForProducerType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef = TypedDict(
-    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
-    {
-        "DataShareArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSharesMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesMessageRequestTypeDef",
     {
         "DataShareArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
-    {
-        "ParameterGroupFamily": str,
-    },
-)
-_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef(
-    _RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
-    _OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeDefaultClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDefaultClusterParametersMessageRequestTypeDef",
     {
         "ParameterGroupFamily": str,
     },
 )
 _OptionalDescribeDefaultClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1449,56 +1291,35 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeDefaultClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDefaultClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef = TypedDict(
-    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ResourceOwner": str,
-        "EndpointName": str,
-        "VpcId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 DescribeEndpointAccessMessageRequestTypeDef = TypedDict(
     "DescribeEndpointAccessMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "ResourceOwner": str,
         "EndpointName": str,
         "VpcId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef = TypedDict(
-    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "Account": str,
-        "Grantee": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEndpointAuthorizationMessageRequestTypeDef = TypedDict(
     "DescribeEndpointAuthorizationMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "Account": str,
         "Grantee": bool,
         "MaxRecords": int,
@@ -1511,98 +1332,52 @@
     "DescribeEventCategoriesMessageRequestTypeDef",
     {
         "SourceType": str,
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Duration": int,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef = TypedDict(
-    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
-    {
-        "HsmClientCertificateIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeHsmClientCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
     {
         "HsmClientCertificateIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
-    {
-        "HsmConfigurationIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeHsmConfigurationsMessageRequestTypeDef = TypedDict(
     "DescribeHsmConfigurationsMessageRequestTypeDef",
     {
         "HsmConfigurationIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
@@ -1624,24 +1399,14 @@
         "Name": NodeConfigurationOptionsFilterNameType,
         "Operator": OperatorTypeType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef = TypedDict(
-    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
-    {
-        "ClusterVersion": str,
-        "NodeType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrderableClusterOptionsMessageRequestTypeDef = TypedDict(
     "DescribeOrderableClusterOptionsMessageRequestTypeDef",
     {
         "ClusterVersion": str,
         "NodeType": str,
         "MaxRecords": int,
         "Marker": str,
@@ -1661,82 +1426,56 @@
     {
         "DatabaseName": str,
         "PartnerName": str,
     },
     total=False,
 )
 
+
 class DescribePartnersInputMessageRequestTypeDef(
     _RequiredDescribePartnersInputMessageRequestTypeDef,
     _OptionalDescribePartnersInputMessageRequestTypeDef,
 ):
     pass
 
+
 PartnerIntegrationInfoTypeDef = TypedDict(
     "PartnerIntegrationInfoTypeDef",
     {
         "DatabaseName": str,
         "PartnerName": str,
         "Status": PartnerIntegrationStatusType,
         "StatusMessage": str,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
-DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef = TypedDict(
-    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-        "ReservedNodeExchangeRequestId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "ReservedNodeExchangeRequestId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
-    {
-        "ReservedNodeOfferingId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedNodeOfferingsMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodeOfferingsMessageRequestTypeDef",
     {
         "ReservedNodeOfferingId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef = TypedDict(
-    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedNodesMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodesMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1754,121 +1493,63 @@
     "ScheduledActionFilterTypeDef",
     {
         "Name": ScheduledActionFilterNameType,
         "Values": Sequence[str],
     },
 )
 
-DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
-    {
-        "SnapshotCopyGrantName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSnapshotCopyGrantsMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotCopyGrantsMessageRequestTypeDef",
     {
         "SnapshotCopyGrantName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef = TypedDict(
-    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ScheduleIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSnapshotSchedulesMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotSchedulesMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "ScheduleIdentifier": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef = TypedDict(
-    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "TableRestoreRequestId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTableRestoreStatusMessageRequestTypeDef = TypedDict(
     "DescribeTableRestoreStatusMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "TableRestoreRequestId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeTagsMessageDescribeTagsPaginateTypeDef = TypedDict(
-    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
-    {
-        "ResourceName": str,
-        "ResourceType": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTagsMessageRequestTypeDef = TypedDict(
     "DescribeTagsMessageRequestTypeDef",
     {
         "ResourceName": str,
         "ResourceType": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef = TypedDict(
-    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
-    {
-        "UsageLimitId": str,
-        "ClusterIdentifier": str,
-        "FeatureType": UsageLimitFeatureTypeType,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeUsageLimitsMessageRequestTypeDef = TypedDict(
     "DescribeUsageLimitsMessageRequestTypeDef",
     {
         "UsageLimitId": str,
         "ClusterIdentifier": str,
         "FeatureType": UsageLimitFeatureTypeType,
         "MaxRecords": int,
@@ -1905,26 +1586,21 @@
         "DisassociateEntireAccount": bool,
         "ConsumerArn": str,
         "ConsumerRegion": str,
     },
     total=False,
 )
 
+
 class DisassociateDataShareConsumerMessageRequestTypeDef(
     _RequiredDisassociateDataShareConsumerMessageRequestTypeDef,
     _OptionalDisassociateDataShareConsumerMessageRequestTypeDef,
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredEnableLoggingMessageRequestTypeDef = TypedDict(
     "_RequiredEnableLoggingMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
@@ -1935,19 +1611,21 @@
         "S3KeyPrefix": str,
         "LogDestinationType": LogDestinationTypeType,
         "LogExports": Sequence[str],
     },
     total=False,
 )
 
+
 class EnableLoggingMessageRequestTypeDef(
     _RequiredEnableLoggingMessageRequestTypeDef, _OptionalEnableLoggingMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredEnableSnapshotCopyMessageRequestTypeDef = TypedDict(
     "_RequiredEnableSnapshotCopyMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "DestinationRegion": str,
     },
 )
@@ -1957,20 +1635,22 @@
         "RetentionPeriod": int,
         "SnapshotCopyGrantName": str,
         "ManualSnapshotRetentionPeriod": int,
     },
     total=False,
 )
 
+
 class EnableSnapshotCopyMessageRequestTypeDef(
     _RequiredEnableSnapshotCopyMessageRequestTypeDef,
     _OptionalEnableSnapshotCopyMessageRequestTypeDef,
 ):
     pass
 
+
 EndpointAuthorizationTypeDef = TypedDict(
     "EndpointAuthorizationTypeDef",
     {
         "Grantor": str,
         "Grantee": str,
         "ClusterIdentifier": str,
         "AuthorizeTime": datetime,
@@ -1979,30 +1659,14 @@
         "AllowedAllVPCs": bool,
         "AllowedVPCs": List[str],
         "EndpointCount": int,
     },
     total=False,
 )
 
-EndpointAuthorizationResponseMetadataTypeDef = TypedDict(
-    "EndpointAuthorizationResponseMetadataTypeDef",
-    {
-        "Grantor": str,
-        "Grantee": str,
-        "ClusterIdentifier": str,
-        "AuthorizeTime": datetime,
-        "ClusterStatus": str,
-        "Status": AuthorizationStatusType,
-        "AllowedAllVPCs": bool,
-        "AllowedVPCs": List[str],
-        "EndpointCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventInfoMapTypeDef = TypedDict(
     "EventInfoMapTypeDef",
     {
         "EventId": str,
         "EventCategories": List[str],
         "EventDescription": str,
         "Severity": str,
@@ -2039,53 +1703,33 @@
         "AutoCreate": bool,
         "DbGroups": Sequence[str],
         "CustomDomainName": str,
     },
     total=False,
 )
 
+
 class GetClusterCredentialsMessageRequestTypeDef(
     _RequiredGetClusterCredentialsMessageRequestTypeDef,
     _OptionalGetClusterCredentialsMessageRequestTypeDef,
 ):
     pass
 
+
 GetClusterCredentialsWithIAMMessageRequestTypeDef = TypedDict(
     "GetClusterCredentialsWithIAMMessageRequestTypeDef",
     {
         "DbName": str,
         "ClusterIdentifier": str,
         "DurationSeconds": int,
         "CustomDomainName": str,
     },
     total=False,
 )
 
-_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
-    "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
-    {
-        "ActionType": ReservedNodeExchangeActionTypeType,
-    },
-)
-_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
-    "_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "SnapshotIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef(
-    _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
-    _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef = TypedDict(
     "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef",
     {
         "ActionType": ReservedNodeExchangeActionTypeType,
     },
 )
 _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef = TypedDict(
@@ -2095,39 +1739,21 @@
         "SnapshotIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef(
     _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
     _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
 ):
     pass
 
-_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
-    "_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-    },
-)
-_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
-    "_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef(
-    _RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
-    _OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
-):
-    pass
 
 _RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef = TypedDict(
     "_RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
     },
 )
@@ -2136,34 +1762,21 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef(
     _RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
     _OptionalGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
 ):
     pass
 
-LoggingStatusTypeDef = TypedDict(
-    "LoggingStatusTypeDef",
-    {
-        "LoggingEnabled": bool,
-        "BucketName": str,
-        "S3KeyPrefix": str,
-        "LastSuccessfulDeliveryTime": datetime,
-        "LastFailureTime": datetime,
-        "LastFailureMessage": str,
-        "LogDestinationType": LogDestinationTypeType,
-        "LogExports": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredModifyAquaInputMessageRequestTypeDef = TypedDict(
     "_RequiredModifyAquaInputMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
@@ -2171,36 +1784,29 @@
     "_OptionalModifyAquaInputMessageRequestTypeDef",
     {
         "AquaConfigurationStatus": AquaConfigurationStatusType,
     },
     total=False,
 )
 
+
 class ModifyAquaInputMessageRequestTypeDef(
     _RequiredModifyAquaInputMessageRequestTypeDef, _OptionalModifyAquaInputMessageRequestTypeDef
 ):
     pass
 
+
 ModifyAuthenticationProfileMessageRequestTypeDef = TypedDict(
     "ModifyAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
 )
 
-ModifyAuthenticationProfileResultTypeDef = TypedDict(
-    "ModifyAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "AuthenticationProfileContent": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ModifyClusterDbRevisionMessageRequestTypeDef = TypedDict(
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "RevisionTarget": str,
     },
 )
@@ -2217,20 +1823,22 @@
         "AddIamRoles": Sequence[str],
         "RemoveIamRoles": Sequence[str],
         "DefaultIamRoleArn": str,
     },
     total=False,
 )
 
+
 class ModifyClusterIamRolesMessageRequestTypeDef(
     _RequiredModifyClusterIamRolesMessageRequestTypeDef,
     _OptionalModifyClusterIamRolesMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterMaintenanceMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
@@ -2241,20 +1849,22 @@
         "DeferMaintenanceStartTime": Union[datetime, str],
         "DeferMaintenanceEndTime": Union[datetime, str],
         "DeferMaintenanceDuration": int,
     },
     total=False,
 )
 
+
 class ModifyClusterMaintenanceMessageRequestTypeDef(
     _RequiredModifyClusterMaintenanceMessageRequestTypeDef,
     _OptionalModifyClusterMaintenanceMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyClusterMessageRequestTypeDef = TypedDict(
@@ -2284,19 +1894,37 @@
         "AvailabilityZoneRelocation": bool,
         "AvailabilityZone": str,
         "Port": int,
     },
     total=False,
 )
 
+
 class ModifyClusterMessageRequestTypeDef(
     _RequiredModifyClusterMessageRequestTypeDef, _OptionalModifyClusterMessageRequestTypeDef
 ):
     pass
 
+
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
+    {
+        "ParameterName": str,
+        "ParameterValue": str,
+        "Description": str,
+        "Source": str,
+        "DataType": str,
+        "AllowedValues": str,
+        "ApplyType": ParameterApplyTypeType,
+        "IsModifiable": bool,
+        "MinimumEngineVersion": str,
+    },
+    total=False,
+)
+
 _RequiredModifyClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterSnapshotMessageRequestTypeDef",
     {
         "SnapshotIdentifier": str,
     },
 )
 _OptionalModifyClusterSnapshotMessageRequestTypeDef = TypedDict(
@@ -2304,20 +1932,22 @@
     {
         "ManualSnapshotRetentionPeriod": int,
         "Force": bool,
     },
     total=False,
 )
 
+
 class ModifyClusterSnapshotMessageRequestTypeDef(
     _RequiredModifyClusterSnapshotMessageRequestTypeDef,
     _OptionalModifyClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyClusterSnapshotScheduleMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterSnapshotScheduleMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyClusterSnapshotScheduleMessageRequestTypeDef = TypedDict(
@@ -2325,20 +1955,22 @@
     {
         "ScheduleIdentifier": str,
         "DisassociateSchedule": bool,
     },
     total=False,
 )
 
+
 class ModifyClusterSnapshotScheduleMessageRequestTypeDef(
     _RequiredModifyClusterSnapshotScheduleMessageRequestTypeDef,
     _OptionalModifyClusterSnapshotScheduleMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyClusterSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterSubnetGroupMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -2346,20 +1978,22 @@
     "_OptionalModifyClusterSubnetGroupMessageRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class ModifyClusterSubnetGroupMessageRequestTypeDef(
     _RequiredModifyClusterSubnetGroupMessageRequestTypeDef,
     _OptionalModifyClusterSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyCustomDomainAssociationMessageRequestTypeDef = TypedDict(
     "_RequiredModifyCustomDomainAssociationMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyCustomDomainAssociationMessageRequestTypeDef = TypedDict(
@@ -2367,30 +2001,21 @@
     {
         "CustomDomainName": str,
         "CustomDomainCertificateArn": str,
     },
     total=False,
 )
 
+
 class ModifyCustomDomainAssociationMessageRequestTypeDef(
     _RequiredModifyCustomDomainAssociationMessageRequestTypeDef,
     _OptionalModifyCustomDomainAssociationMessageRequestTypeDef,
 ):
     pass
 
-ModifyCustomDomainAssociationResultTypeDef = TypedDict(
-    "ModifyCustomDomainAssociationResultTypeDef",
-    {
-        "CustomDomainName": str,
-        "CustomDomainCertificateArn": str,
-        "ClusterIdentifier": str,
-        "CustomDomainCertExpiryTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredModifyEndpointAccessMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointAccessMessageRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
@@ -2398,20 +2023,22 @@
     "_OptionalModifyEndpointAccessMessageRequestTypeDef",
     {
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyEndpointAccessMessageRequestTypeDef(
     _RequiredModifyEndpointAccessMessageRequestTypeDef,
     _OptionalModifyEndpointAccessMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
     },
 )
 _OptionalModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
@@ -2423,20 +2050,22 @@
         "EventCategories": Sequence[str],
         "Severity": str,
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class ModifyEventSubscriptionMessageRequestTypeDef(
     _RequiredModifyEventSubscriptionMessageRequestTypeDef,
     _OptionalModifyEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifySnapshotCopyRetentionPeriodMessageRequestTypeDef = TypedDict(
     "_RequiredModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "RetentionPeriod": int,
     },
 )
@@ -2444,20 +2073,22 @@
     "_OptionalModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     {
         "Manual": bool,
     },
     total=False,
 )
 
+
 class ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef(
     _RequiredModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     _OptionalModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
 ):
     pass
 
+
 ModifySnapshotScheduleMessageRequestTypeDef = TypedDict(
     "ModifySnapshotScheduleMessageRequestTypeDef",
     {
         "ScheduleIdentifier": str,
         "ScheduleDefinitions": Sequence[str],
     },
 )
@@ -2473,19 +2104,21 @@
     {
         "Amount": int,
         "BreachAction": UsageLimitBreachActionType,
     },
     total=False,
 )
 
+
 class ModifyUsageLimitMessageRequestTypeDef(
     _RequiredModifyUsageLimitMessageRequestTypeDef, _OptionalModifyUsageLimitMessageRequestTypeDef
 ):
     pass
 
+
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "NetworkInterfaceId": str,
         "SubnetId": str,
         "PrivateIpAddress": str,
         "AvailabilityZone": str,
@@ -2500,40 +2133,28 @@
         "NumberOfNodes": int,
         "EstimatedDiskUtilizationPercent": float,
         "Mode": ModeType,
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
 PartnerIntegrationInputMessageRequestTypeDef = TypedDict(
     "PartnerIntegrationInputMessageRequestTypeDef",
     {
         "AccountId": str,
         "ClusterIdentifier": str,
         "DatabaseName": str,
         "PartnerName": str,
     },
 )
 
-PartnerIntegrationOutputMessageTypeDef = TypedDict(
-    "PartnerIntegrationOutputMessageTypeDef",
+PauseClusterMessageOutputTypeDef = TypedDict(
+    "PauseClusterMessageOutputTypeDef",
     {
-        "DatabaseName": str,
-        "PartnerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterIdentifier": str,
     },
 )
 
 PauseClusterMessageRequestTypeDef = TypedDict(
     "PauseClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
@@ -2557,20 +2178,22 @@
     "_OptionalPurchaseReservedNodeOfferingMessageRequestTypeDef",
     {
         "NodeCount": int,
     },
     total=False,
 )
 
+
 class PurchaseReservedNodeOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedNodeOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedNodeOfferingMessageRequestTypeDef,
 ):
     pass
 
+
 RebootClusterMessageRequestTypeDef = TypedDict(
     "RebootClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2586,14 +2209,40 @@
 RejectDataShareMessageRequestTypeDef = TypedDict(
     "RejectDataShareMessageRequestTypeDef",
     {
         "DataShareArn": str,
     },
 )
 
+_RequiredResizeClusterMessageOutputTypeDef = TypedDict(
+    "_RequiredResizeClusterMessageOutputTypeDef",
+    {
+        "ClusterIdentifier": str,
+    },
+)
+_OptionalResizeClusterMessageOutputTypeDef = TypedDict(
+    "_OptionalResizeClusterMessageOutputTypeDef",
+    {
+        "ClusterType": str,
+        "NodeType": str,
+        "NumberOfNodes": int,
+        "Classic": bool,
+        "ReservedNodeId": str,
+        "TargetReservedNodeOfferingId": str,
+    },
+    total=False,
+)
+
+
+class ResizeClusterMessageOutputTypeDef(
+    _RequiredResizeClusterMessageOutputTypeDef, _OptionalResizeClusterMessageOutputTypeDef
+):
+    pass
+
+
 _RequiredResizeClusterMessageRequestTypeDef = TypedDict(
     "_RequiredResizeClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalResizeClusterMessageRequestTypeDef = TypedDict(
@@ -2605,19 +2254,21 @@
         "Classic": bool,
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
     },
     total=False,
 )
 
+
 class ResizeClusterMessageRequestTypeDef(
     _RequiredResizeClusterMessageRequestTypeDef, _OptionalResizeClusterMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredResizeClusterMessageTypeDef = TypedDict(
     "_RequiredResizeClusterMessageTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalResizeClusterMessageTypeDef = TypedDict(
@@ -2629,52 +2280,20 @@
         "Classic": bool,
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
     },
     total=False,
 )
 
+
 class ResizeClusterMessageTypeDef(
     _RequiredResizeClusterMessageTypeDef, _OptionalResizeClusterMessageTypeDef
 ):
     pass
 
-ResizeProgressMessageTypeDef = TypedDict(
-    "ResizeProgressMessageTypeDef",
-    {
-        "TargetNodeType": str,
-        "TargetNumberOfNodes": int,
-        "TargetClusterType": str,
-        "Status": str,
-        "ImportTablesCompleted": List[str],
-        "ImportTablesInProgress": List[str],
-        "ImportTablesNotStarted": List[str],
-        "AvgResizeRateInMegaBytesPerSecond": float,
-        "TotalResizeDataInMegaBytes": int,
-        "ProgressInMegaBytes": int,
-        "ElapsedTimeInSeconds": int,
-        "EstimatedTimeToCompletionInSeconds": int,
-        "ResizeType": str,
-        "Message": str,
-        "TargetEncryptionType": str,
-        "DataTransferProgressPercent": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 
 _RequiredRestoreFromClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreFromClusterSnapshotMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
@@ -2713,20 +2332,22 @@
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
         "Encrypted": bool,
     },
     total=False,
 )
 
+
 class RestoreFromClusterSnapshotMessageRequestTypeDef(
     _RequiredRestoreFromClusterSnapshotMessageRequestTypeDef,
     _OptionalRestoreFromClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreTableFromClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreTableFromClusterSnapshotMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SourceDatabaseName": str,
         "SourceTableName": str,
@@ -2740,20 +2361,22 @@
         "TargetDatabaseName": str,
         "TargetSchemaName": str,
         "EnableCaseSensitiveIdentifier": bool,
     },
     total=False,
 )
 
+
 class RestoreTableFromClusterSnapshotMessageRequestTypeDef(
     _RequiredRestoreTableFromClusterSnapshotMessageRequestTypeDef,
     _OptionalRestoreTableFromClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 TableRestoreStatusTypeDef = TypedDict(
     "TableRestoreStatusTypeDef",
     {
         "TableRestoreRequestId": str,
         "Status": TableRestoreStatusTypeType,
         "Message": str,
         "RequestTime": datetime,
@@ -2767,14 +2390,21 @@
         "TargetDatabaseName": str,
         "TargetSchemaName": str,
         "NewTableName": str,
     },
     total=False,
 )
 
+ResumeClusterMessageOutputTypeDef = TypedDict(
+    "ResumeClusterMessageOutputTypeDef",
+    {
+        "ClusterIdentifier": str,
+    },
+)
+
 ResumeClusterMessageRequestTypeDef = TypedDict(
     "ResumeClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2797,20 +2427,22 @@
         "CIDRIP": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+
 class RevokeClusterSecurityGroupIngressMessageRequestTypeDef(
     _RequiredRevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     _OptionalRevokeClusterSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
+
 RevokeEndpointAccessMessageRequestTypeDef = TypedDict(
     "RevokeEndpointAccessMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "Account": str,
         "VpcIds": Sequence[str],
         "Force": bool,
@@ -2830,20 +2462,22 @@
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
+
 class RevokeSnapshotAccessMessageRequestTypeDef(
     _RequiredRevokeSnapshotAccessMessageRequestTypeDef,
     _OptionalRevokeSnapshotAccessMessageRequestTypeDef,
 ):
     pass
 
+
 RotateEncryptionKeyMessageRequestTypeDef = TypedDict(
     "RotateEncryptionKeyMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2869,34 +2503,193 @@
     "_OptionalUpdatePartnerStatusInputMessageRequestTypeDef",
     {
         "StatusMessage": str,
     },
     total=False,
 )
 
+
 class UpdatePartnerStatusInputMessageRequestTypeDef(
     _RequiredUpdatePartnerStatusInputMessageRequestTypeDef,
     _OptionalUpdatePartnerStatusInputMessageRequestTypeDef,
 ):
     pass
 
+
+ClusterCredentialsTypeDef = TypedDict(
+    "ClusterCredentialsTypeDef",
+    {
+        "DbUser": str,
+        "DbPassword": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ClusterExtendedCredentialsTypeDef = TypedDict(
+    "ClusterExtendedCredentialsTypeDef",
+    {
+        "DbUser": str,
+        "DbPassword": str,
+        "Expiration": datetime,
+        "NextRefreshTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ClusterParameterGroupNameMessageTypeDef = TypedDict(
+    "ClusterParameterGroupNameMessageTypeDef",
+    {
+        "ParameterGroupName": str,
+        "ParameterGroupStatus": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAuthenticationProfileResultTypeDef = TypedDict(
+    "CreateAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "AuthenticationProfileContent": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomDomainAssociationResultTypeDef = TypedDict(
+    "CreateCustomDomainAssociationResultTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "ClusterIdentifier": str,
+        "CustomDomainCertExpiryTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CustomerStorageMessageTypeDef = TypedDict(
+    "CustomerStorageMessageTypeDef",
+    {
+        "TotalBackupSizeInMegaBytes": float,
+        "TotalProvisionedStorageInMegaBytes": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAuthenticationProfileResultTypeDef = TypedDict(
+    "DeleteAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EndpointAuthorizationResponseMetadataTypeDef = TypedDict(
+    "EndpointAuthorizationResponseMetadataTypeDef",
+    {
+        "Grantor": str,
+        "Grantee": str,
+        "ClusterIdentifier": str,
+        "AuthorizeTime": datetime,
+        "ClusterStatus": str,
+        "Status": AuthorizationStatusType,
+        "AllowedAllVPCs": bool,
+        "AllowedVPCs": List[str],
+        "EndpointCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LoggingStatusTypeDef = TypedDict(
+    "LoggingStatusTypeDef",
+    {
+        "LoggingEnabled": bool,
+        "BucketName": str,
+        "S3KeyPrefix": str,
+        "LastSuccessfulDeliveryTime": datetime,
+        "LastFailureTime": datetime,
+        "LastFailureMessage": str,
+        "LogDestinationType": LogDestinationTypeType,
+        "LogExports": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyAuthenticationProfileResultTypeDef = TypedDict(
+    "ModifyAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "AuthenticationProfileContent": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyCustomDomainAssociationResultTypeDef = TypedDict(
+    "ModifyCustomDomainAssociationResultTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "ClusterIdentifier": str,
+        "CustomDomainCertExpiryTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PartnerIntegrationOutputMessageTypeDef = TypedDict(
+    "PartnerIntegrationOutputMessageTypeDef",
+    {
+        "DatabaseName": str,
+        "PartnerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResizeProgressMessageTypeDef = TypedDict(
+    "ResizeProgressMessageTypeDef",
+    {
+        "TargetNodeType": str,
+        "TargetNumberOfNodes": int,
+        "TargetClusterType": str,
+        "Status": str,
+        "ImportTablesCompleted": List[str],
+        "ImportTablesInProgress": List[str],
+        "ImportTablesNotStarted": List[str],
+        "AvgResizeRateInMegaBytesPerSecond": float,
+        "TotalResizeDataInMegaBytes": int,
+        "ProgressInMegaBytes": int,
+        "ElapsedTimeInSeconds": int,
+        "EstimatedTimeToCompletionInSeconds": int,
+        "ResizeType": str,
+        "Message": str,
+        "TargetEncryptionType": str,
+        "DataTransferProgressPercent": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AccountAttributeTypeDef = TypedDict(
     "AccountAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[AttributeValueTargetTypeDef],
     },
     total=False,
 )
 
 ModifyAquaOutputMessageTypeDef = TypedDict(
     "ModifyAquaOutputMessageTypeDef",
     {
         "AquaConfiguration": AquaConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociationTypeDef = TypedDict(
     "AssociationTypeDef",
     {
         "CustomDomainCertificateArn": str,
@@ -2906,15 +2699,15 @@
     total=False,
 )
 
 DescribeAuthenticationProfilesResultTypeDef = TypedDict(
     "DescribeAuthenticationProfilesResultTypeDef",
     {
         "AuthenticationProfiles": List[AuthenticationProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
@@ -2931,24 +2724,24 @@
 )
 
 BatchDeleteClusterSnapshotsResultTypeDef = TypedDict(
     "BatchDeleteClusterSnapshotsResultTypeDef",
     {
         "Resources": List[str],
         "Errors": List[SnapshotErrorMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchModifyClusterSnapshotsOutputMessageTypeDef = TypedDict(
     "BatchModifyClusterSnapshotsOutputMessageTypeDef",
     {
         "Resources": List[str],
         "Errors": List[SnapshotErrorMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterDbRevisionTypeDef = TypedDict(
     "ClusterDbRevisionTypeDef",
     {
         "ClusterIdentifier": str,
@@ -2958,80 +2751,249 @@
     },
     total=False,
 )
 
 ClusterParameterGroupDetailsTypeDef = TypedDict(
     "ClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefaultClusterParametersTypeDef = TypedDict(
     "DefaultClusterParametersTypeDef",
     {
         "ParameterGroupFamily": str,
         "Marker": str,
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
     },
     total=False,
 )
 
-ModifyClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyClusterParameterGroupMessageRequestTypeDef",
+ClusterParameterGroupStatusTypeDef = TypedDict(
+    "ClusterParameterGroupStatusTypeDef",
     {
         "ParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
+        "ParameterApplyStatus": str,
+        "ClusterParameterStatusList": List[ClusterParameterStatusTypeDef],
     },
+    total=False,
 )
 
-_RequiredResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetClusterParameterGroupMessageRequestTypeDef",
+ClusterParameterGroupTypeDef = TypedDict(
+    "ClusterParameterGroupTypeDef",
     {
         "ParameterGroupName": str,
+        "ParameterGroupFamily": str,
+        "Description": str,
+        "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
-_OptionalResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetClusterParameterGroupMessageRequestTypeDef",
+
+EC2SecurityGroupTypeDef = TypedDict(
+    "EC2SecurityGroupTypeDef",
     {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
+        "Status": str,
+        "EC2SecurityGroupName": str,
+        "EC2SecurityGroupOwnerId": str,
+        "Tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
-class ResetClusterParameterGroupMessageRequestTypeDef(
-    _RequiredResetClusterParameterGroupMessageRequestTypeDef,
-    _OptionalResetClusterParameterGroupMessageRequestTypeDef,
-):
-    pass
+EventSubscriptionTypeDef = TypedDict(
+    "EventSubscriptionTypeDef",
+    {
+        "CustomerAwsId": str,
+        "CustSubscriptionId": str,
+        "SnsTopicArn": str,
+        "Status": str,
+        "SubscriptionCreationTime": datetime,
+        "SourceType": str,
+        "SourceIdsList": List[str],
+        "EventCategoriesList": List[str],
+        "Severity": str,
+        "Enabled": bool,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
 
-ClusterParameterGroupStatusTypeDef = TypedDict(
-    "ClusterParameterGroupStatusTypeDef",
+HsmClientCertificateTypeDef = TypedDict(
+    "HsmClientCertificateTypeDef",
     {
-        "ParameterGroupName": str,
-        "ParameterApplyStatus": str,
-        "ClusterParameterStatusList": List[ClusterParameterStatusTypeDef],
+        "HsmClientCertificateIdentifier": str,
+        "HsmClientCertificatePublicKey": str,
+        "Tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
-ClusterParameterGroupTypeDef = TypedDict(
-    "ClusterParameterGroupTypeDef",
+HsmConfigurationTypeDef = TypedDict(
+    "HsmConfigurationTypeDef",
     {
-        "ParameterGroupName": str,
-        "ParameterGroupFamily": str,
+        "HsmConfigurationIdentifier": str,
         "Description": str,
-        "Tags": List[TagTypeDef],
+        "HsmIpAddress": str,
+        "HsmPartitionName": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+IPRangeTypeDef = TypedDict(
+    "IPRangeTypeDef",
+    {
+        "Status": str,
+        "CIDRIP": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+SnapshotCopyGrantTypeDef = TypedDict(
+    "SnapshotCopyGrantTypeDef",
+    {
+        "SnapshotCopyGrantName": str,
+        "KmsKeyId": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+SnapshotScheduleResponseMetadataTypeDef = TypedDict(
+    "SnapshotScheduleResponseMetadataTypeDef",
+    {
+        "ScheduleDefinitions": List[str],
+        "ScheduleIdentifier": str,
+        "ScheduleDescription": str,
+        "Tags": List[TagOutputTypeDef],
+        "NextInvocations": List[datetime],
+        "AssociatedClusterCount": int,
+        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SnapshotScheduleTypeDef = TypedDict(
+    "SnapshotScheduleTypeDef",
+    {
+        "ScheduleDefinitions": List[str],
+        "ScheduleIdentifier": str,
+        "ScheduleDescription": str,
+        "Tags": List[TagOutputTypeDef],
+        "NextInvocations": List[datetime],
+        "AssociatedClusterCount": int,
+        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
+    },
+    total=False,
+)
+
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotIdentifier": str,
+        "ClusterIdentifier": str,
+        "SnapshotCreateTime": datetime,
+        "Status": str,
+        "Port": int,
+        "AvailabilityZone": str,
+        "ClusterCreateTime": datetime,
+        "MasterUsername": str,
+        "ClusterVersion": str,
+        "EngineFullVersion": str,
+        "SnapshotType": str,
+        "NodeType": str,
+        "NumberOfNodes": int,
+        "DBName": str,
+        "VpcId": str,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "EncryptedWithHSM": bool,
+        "AccountsWithRestoreAccess": List[AccountWithRestoreAccessTypeDef],
+        "OwnerAccount": str,
+        "TotalBackupSizeInMegaBytes": float,
+        "ActualIncrementalBackupSizeInMegaBytes": float,
+        "BackupProgressInMegaBytes": float,
+        "CurrentBackupRateInMegaBytesPerSecond": float,
+        "EstimatedSecondsToCompletion": int,
+        "ElapsedTimeInSeconds": int,
+        "SourceRegion": str,
+        "Tags": List[TagOutputTypeDef],
+        "RestorableNodeTypes": List[str],
+        "EnhancedVpcRouting": bool,
+        "MaintenanceTrackName": str,
+        "ManualSnapshotRetentionPeriod": int,
+        "ManualSnapshotRemainingDays": int,
+        "SnapshotRetentionStartTime": datetime,
     },
     total=False,
 )
 
+TaggedResourceTypeDef = TypedDict(
+    "TaggedResourceTypeDef",
+    {
+        "Tag": TagOutputTypeDef,
+        "ResourceName": str,
+        "ResourceType": str,
+    },
+    total=False,
+)
+
+UsageLimitResponseMetadataTypeDef = TypedDict(
+    "UsageLimitResponseMetadataTypeDef",
+    {
+        "UsageLimitId": str,
+        "ClusterIdentifier": str,
+        "FeatureType": UsageLimitFeatureTypeType,
+        "LimitType": UsageLimitLimitTypeType,
+        "Amount": int,
+        "Period": UsageLimitPeriodType,
+        "BreachAction": UsageLimitBreachActionType,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UsageLimitTypeDef = TypedDict(
+    "UsageLimitTypeDef",
+    {
+        "UsageLimitId": str,
+        "ClusterIdentifier": str,
+        "FeatureType": UsageLimitFeatureTypeType,
+        "LimitType": UsageLimitLimitTypeType,
+        "Amount": int,
+        "Period": UsageLimitPeriodType,
+        "BreachAction": UsageLimitBreachActionType,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+DescribeReservedNodeExchangeStatusOutputMessageTypeDef = TypedDict(
+    "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
+    {
+        "ReservedNodeExchangeStatusDetails": List[ReservedNodeExchangeStatusTypeDef],
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ClusterVersionsMessageTypeDef = TypedDict(
+    "ClusterVersionsMessageTypeDef",
+    {
+        "Marker": str,
+        "ClusterVersions": List[ClusterVersionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "NodeType": str,
         "MasterUsername": str,
         "MasterUserPassword": str,
@@ -3070,19 +3032,21 @@
         "AquaConfigurationStatus": AquaConfigurationStatusType,
         "DefaultIamRoleArn": str,
         "LoadSampleData": str,
     },
     total=False,
 )
 
+
 class CreateClusterMessageRequestTypeDef(
     _RequiredCreateClusterMessageRequestTypeDef, _OptionalCreateClusterMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterParameterGroupMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
         "ParameterGroupFamily": str,
         "Description": str,
     },
@@ -3091,20 +3055,22 @@
     "_OptionalCreateClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateClusterParameterGroupMessageRequestTypeDef(
     _RequiredCreateClusterParameterGroupMessageRequestTypeDef,
     _OptionalCreateClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateClusterSecurityGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSecurityGroupMessageRequestTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "Description": str,
     },
 )
@@ -3112,20 +3078,22 @@
     "_OptionalCreateClusterSecurityGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateClusterSecurityGroupMessageRequestTypeDef(
     _RequiredCreateClusterSecurityGroupMessageRequestTypeDef,
     _OptionalCreateClusterSecurityGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSnapshotMessageRequestTypeDef",
     {
         "SnapshotIdentifier": str,
         "ClusterIdentifier": str,
     },
 )
@@ -3134,20 +3102,22 @@
     {
         "ManualSnapshotRetentionPeriod": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateClusterSnapshotMessageRequestTypeDef(
     _RequiredCreateClusterSnapshotMessageRequestTypeDef,
     _OptionalCreateClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateClusterSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSubnetGroupMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "Description": str,
         "SubnetIds": Sequence[str],
     },
@@ -3156,20 +3126,22 @@
     "_OptionalCreateClusterSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateClusterSubnetGroupMessageRequestTypeDef(
     _RequiredCreateClusterSubnetGroupMessageRequestTypeDef,
     _OptionalCreateClusterSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "SnsTopicArn": str,
     },
 )
@@ -3182,40 +3154,44 @@
         "Severity": str,
         "Enabled": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateEventSubscriptionMessageRequestTypeDef(
     _RequiredCreateEventSubscriptionMessageRequestTypeDef,
     _OptionalCreateEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateHsmClientCertificateMessageRequestTypeDef = TypedDict(
     "_RequiredCreateHsmClientCertificateMessageRequestTypeDef",
     {
         "HsmClientCertificateIdentifier": str,
     },
 )
 _OptionalCreateHsmClientCertificateMessageRequestTypeDef = TypedDict(
     "_OptionalCreateHsmClientCertificateMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateHsmClientCertificateMessageRequestTypeDef(
     _RequiredCreateHsmClientCertificateMessageRequestTypeDef,
     _OptionalCreateHsmClientCertificateMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateHsmConfigurationMessageRequestTypeDef = TypedDict(
     "_RequiredCreateHsmConfigurationMessageRequestTypeDef",
     {
         "HsmConfigurationIdentifier": str,
         "Description": str,
         "HsmIpAddress": str,
         "HsmPartitionName": str,
@@ -3227,20 +3203,22 @@
     "_OptionalCreateHsmConfigurationMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateHsmConfigurationMessageRequestTypeDef(
     _RequiredCreateHsmConfigurationMessageRequestTypeDef,
     _OptionalCreateHsmConfigurationMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateSnapshotCopyGrantMessageRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotCopyGrantMessageRequestTypeDef",
     {
         "SnapshotCopyGrantName": str,
     },
 )
 _OptionalCreateSnapshotCopyGrantMessageRequestTypeDef = TypedDict(
@@ -3248,20 +3226,22 @@
     {
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSnapshotCopyGrantMessageRequestTypeDef(
     _RequiredCreateSnapshotCopyGrantMessageRequestTypeDef,
     _OptionalCreateSnapshotCopyGrantMessageRequestTypeDef,
 ):
     pass
 
+
 CreateSnapshotScheduleMessageRequestTypeDef = TypedDict(
     "CreateSnapshotScheduleMessageRequestTypeDef",
     {
         "ScheduleDefinitions": Sequence[str],
         "ScheduleIdentifier": str,
         "ScheduleDescription": str,
         "Tags": Sequence[TagTypeDef],
@@ -3294,256 +3274,427 @@
         "Period": UsageLimitPeriodType,
         "BreachAction": UsageLimitBreachActionType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateUsageLimitMessageRequestTypeDef(
     _RequiredCreateUsageLimitMessageRequestTypeDef, _OptionalCreateUsageLimitMessageRequestTypeDef
 ):
     pass
 
-EC2SecurityGroupTypeDef = TypedDict(
-    "EC2SecurityGroupTypeDef",
+
+DataShareResponseMetadataTypeDef = TypedDict(
+    "DataShareResponseMetadataTypeDef",
     {
-        "Status": str,
-        "EC2SecurityGroupName": str,
-        "EC2SecurityGroupOwnerId": str,
-        "Tags": List[TagTypeDef],
+        "DataShareArn": str,
+        "ProducerArn": str,
+        "AllowPubliclyAccessibleConsumers": bool,
+        "DataShareAssociations": List[DataShareAssociationTypeDef],
+        "ManagedBy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DataShareTypeDef = TypedDict(
+    "DataShareTypeDef",
+    {
+        "DataShareArn": str,
+        "ProducerArn": str,
+        "AllowPubliclyAccessibleConsumers": bool,
+        "DataShareAssociations": List[DataShareAssociationTypeDef],
+        "ManagedBy": str,
     },
     total=False,
 )
 
-EventSubscriptionTypeDef = TypedDict(
-    "EventSubscriptionTypeDef",
+DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef = TypedDict(
+    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
     {
-        "CustomerAwsId": str,
-        "CustSubscriptionId": str,
-        "SnsTopicArn": str,
-        "Status": str,
-        "SubscriptionCreationTime": datetime,
-        "SourceType": str,
-        "SourceIdsList": List[str],
-        "EventCategoriesList": List[str],
-        "Severity": str,
-        "Enabled": bool,
-        "Tags": List[TagTypeDef],
+        "ClusterIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-HsmClientCertificateTypeDef = TypedDict(
-    "HsmClientCertificateTypeDef",
+DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
     {
-        "HsmClientCertificateIdentifier": str,
-        "HsmClientCertificatePublicKey": str,
-        "Tags": List[TagTypeDef],
+        "ParameterGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-HsmConfigurationTypeDef = TypedDict(
-    "HsmConfigurationTypeDef",
+_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
     {
-        "HsmConfigurationIdentifier": str,
-        "Description": str,
-        "HsmIpAddress": str,
-        "HsmPartitionName": str,
-        "Tags": List[TagTypeDef],
+        "ParameterGroupName": str,
+    },
+)
+_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-IPRangeTypeDef = TypedDict(
-    "IPRangeTypeDef",
+
+class DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef(
+    _RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+    _OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+):
+    pass
+
+
+DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
     {
-        "Status": str,
-        "CIDRIP": str,
-        "Tags": List[TagTypeDef],
+        "ClusterSecurityGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-SnapshotCopyGrantTypeDef = TypedDict(
-    "SnapshotCopyGrantTypeDef",
+DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
     {
-        "SnapshotCopyGrantName": str,
-        "KmsKeyId": str,
-        "Tags": List[TagTypeDef],
+        "ClusterSubnetGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-SnapshotScheduleResponseMetadataTypeDef = TypedDict(
-    "SnapshotScheduleResponseMetadataTypeDef",
+DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef = TypedDict(
+    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
     {
-        "ScheduleDefinitions": List[str],
-        "ScheduleIdentifier": str,
-        "ScheduleDescription": str,
-        "Tags": List[TagTypeDef],
-        "NextInvocations": List[datetime],
-        "AssociatedClusterCount": int,
-        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaintenanceTrackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-SnapshotScheduleTypeDef = TypedDict(
-    "SnapshotScheduleTypeDef",
+DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef = TypedDict(
+    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
     {
-        "ScheduleDefinitions": List[str],
-        "ScheduleIdentifier": str,
-        "ScheduleDescription": str,
-        "Tags": List[TagTypeDef],
-        "NextInvocations": List[datetime],
-        "AssociatedClusterCount": int,
-        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
+        "ClusterVersion": str,
+        "ClusterParameterGroupFamily": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
+DescribeClustersMessageDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
     {
-        "SnapshotIdentifier": str,
         "ClusterIdentifier": str,
-        "SnapshotCreateTime": datetime,
-        "Status": str,
-        "Port": int,
-        "AvailabilityZone": str,
-        "ClusterCreateTime": datetime,
-        "MasterUsername": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef = TypedDict(
+    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef = TypedDict(
+    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
+    {
+        "ConsumerArn": str,
+        "Status": DataShareStatusForConsumerType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef = TypedDict(
+    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
+    {
+        "ProducerArn": str,
+        "Status": DataShareStatusForProducerType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef = TypedDict(
+    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
+    {
+        "DataShareArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    {
+        "ParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef(
+    _RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+    _OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+):
+    pass
+
+
+DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef = TypedDict(
+    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ResourceOwner": str,
+        "EndpointName": str,
+        "VpcId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef = TypedDict(
+    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "Account": str,
+        "Grantee": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef = TypedDict(
+    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
+    {
+        "HsmClientCertificateIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
+    {
+        "HsmConfigurationIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef = TypedDict(
+    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
+    {
         "ClusterVersion": str,
-        "EngineFullVersion": str,
-        "SnapshotType": str,
         "NodeType": str,
-        "NumberOfNodes": int,
-        "DBName": str,
-        "VpcId": str,
-        "Encrypted": bool,
-        "KmsKeyId": str,
-        "EncryptedWithHSM": bool,
-        "AccountsWithRestoreAccess": List[AccountWithRestoreAccessTypeDef],
-        "OwnerAccount": str,
-        "TotalBackupSizeInMegaBytes": float,
-        "ActualIncrementalBackupSizeInMegaBytes": float,
-        "BackupProgressInMegaBytes": float,
-        "CurrentBackupRateInMegaBytesPerSecond": float,
-        "EstimatedSecondsToCompletion": int,
-        "ElapsedTimeInSeconds": int,
-        "SourceRegion": str,
-        "Tags": List[TagTypeDef],
-        "RestorableNodeTypes": List[str],
-        "EnhancedVpcRouting": bool,
-        "MaintenanceTrackName": str,
-        "ManualSnapshotRetentionPeriod": int,
-        "ManualSnapshotRemainingDays": int,
-        "SnapshotRetentionStartTime": datetime,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-TaggedResourceTypeDef = TypedDict(
-    "TaggedResourceTypeDef",
+DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef = TypedDict(
+    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
     {
-        "Tag": TagTypeDef,
-        "ResourceName": str,
-        "ResourceType": str,
+        "ReservedNodeId": str,
+        "ReservedNodeExchangeRequestId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-UsageLimitResponseMetadataTypeDef = TypedDict(
-    "UsageLimitResponseMetadataTypeDef",
+DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
+    {
+        "ReservedNodeOfferingId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef = TypedDict(
+    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
+    {
+        "ReservedNodeId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
+    {
+        "SnapshotCopyGrantName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef = TypedDict(
+    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
     {
-        "UsageLimitId": str,
         "ClusterIdentifier": str,
-        "FeatureType": UsageLimitFeatureTypeType,
-        "LimitType": UsageLimitLimitTypeType,
-        "Amount": int,
-        "Period": UsageLimitPeriodType,
-        "BreachAction": UsageLimitBreachActionType,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ScheduleIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-UsageLimitTypeDef = TypedDict(
-    "UsageLimitTypeDef",
+DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef = TypedDict(
+    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
     {
-        "UsageLimitId": str,
         "ClusterIdentifier": str,
-        "FeatureType": UsageLimitFeatureTypeType,
-        "LimitType": UsageLimitLimitTypeType,
-        "Amount": int,
-        "Period": UsageLimitPeriodType,
-        "BreachAction": UsageLimitBreachActionType,
-        "Tags": List[TagTypeDef],
+        "TableRestoreRequestId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeReservedNodeExchangeStatusOutputMessageTypeDef = TypedDict(
-    "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
+DescribeTagsMessageDescribeTagsPaginateTypeDef = TypedDict(
+    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
     {
-        "ReservedNodeExchangeStatusDetails": List[ReservedNodeExchangeStatusTypeDef],
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceName": str,
+        "ResourceType": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ClusterVersionsMessageTypeDef = TypedDict(
-    "ClusterVersionsMessageTypeDef",
+DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef = TypedDict(
+    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
     {
-        "Marker": str,
-        "ClusterVersions": List[ClusterVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "UsageLimitId": str,
+        "ClusterIdentifier": str,
+        "FeatureType": UsageLimitFeatureTypeType,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-DataShareResponseMetadataTypeDef = TypedDict(
-    "DataShareResponseMetadataTypeDef",
+_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
+    "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
     {
-        "DataShareArn": str,
-        "ProducerArn": str,
-        "AllowPubliclyAccessibleConsumers": bool,
-        "DataShareAssociations": List[DataShareAssociationTypeDef],
-        "ManagedBy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ActionType": ReservedNodeExchangeActionTypeType,
     },
 )
+_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
+    "_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "SnapshotIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-DataShareTypeDef = TypedDict(
-    "DataShareTypeDef",
+
+class GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef(
+    _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+    _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
+    "_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
     {
-        "DataShareArn": str,
-        "ProducerArn": str,
-        "AllowPubliclyAccessibleConsumers": bool,
-        "DataShareAssociations": List[DataShareAssociationTypeDef],
-        "ManagedBy": str,
+        "ReservedNodeId": str,
+    },
+)
+_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
+    "_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
+class GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef(
+    _RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
+    _OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
+):
+    pass
+
+
 DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageRequestTypeDef",
     {
@@ -3634,25 +3785,27 @@
     "_OptionalDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "OwnerAccount": str,
         "Filters": Sequence[NodeConfigurationOptionsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef(
     _RequiredDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
     _OptionalDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeNodeConfigurationOptionsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeNodeConfigurationOptionsMessageRequestTypeDef",
     {
         "ActionType": ActionTypeType,
     },
 )
 _OptionalDescribeNodeConfigurationOptionsMessageRequestTypeDef = TypedDict(
@@ -3665,38 +3818,40 @@
         "Filters": Sequence[NodeConfigurationOptionsFilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+
 class DescribeNodeConfigurationOptionsMessageRequestTypeDef(
     _RequiredDescribeNodeConfigurationOptionsMessageRequestTypeDef,
     _OptionalDescribeNodeConfigurationOptionsMessageRequestTypeDef,
 ):
     pass
 
+
 DescribePartnersOutputMessageTypeDef = TypedDict(
     "DescribePartnersOutputMessageTypeDef",
     {
         "PartnerIntegrationInfoList": List[PartnerIntegrationInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef = TypedDict(
     "DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef",
     {
         "ScheduledActionName": str,
         "TargetActionType": ScheduledActionTypeValuesType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Active": bool,
         "Filters": Sequence[ScheduledActionFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeScheduledActionsMessageRequestTypeDef = TypedDict(
     "DescribeScheduledActionsMessageRequestTypeDef",
     {
@@ -3713,15 +3868,15 @@
 )
 
 EndpointAuthorizationListTypeDef = TypedDict(
     "EndpointAuthorizationListTypeDef",
     {
         "EndpointAuthorizationList": List[EndpointAuthorizationTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
@@ -3731,18 +3886,49 @@
 )
 
 EventsMessageTypeDef = TypedDict(
     "EventsMessageTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ModifyClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+_RequiredResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ParameterGroupName": str,
+    },
+)
+_OptionalResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+    total=False,
+)
+
+
+class ResetClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
+
+
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "VpcEndpointId": str,
         "VpcId": str,
         "NetworkInterfaces": List[NetworkInterfaceTypeDef],
     },
@@ -3750,15 +3936,15 @@
 )
 
 NodeConfigurationOptionsMessageTypeDef = TypedDict(
     "NodeConfigurationOptionsMessageTypeDef",
     {
         "NodeConfigurationOptionList": List[NodeConfigurationOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedNodeOfferingTypeDef = TypedDict(
     "ReservedNodeOfferingTypeDef",
     {
         "ReservedNodeOfferingId": str,
@@ -3794,25 +3980,35 @@
     total=False,
 )
 
 RestoreTableFromClusterSnapshotResultTypeDef = TypedDict(
     "RestoreTableFromClusterSnapshotResultTypeDef",
     {
         "TableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TableRestoreStatusMessageTypeDef = TypedDict(
     "TableRestoreStatusMessageTypeDef",
     {
         "TableRestoreStatusDetails": List[TableRestoreStatusTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ScheduledActionTypeOutputTypeDef = TypedDict(
+    "ScheduledActionTypeOutputTypeDef",
+    {
+        "ResizeCluster": ResizeClusterMessageOutputTypeDef,
+        "PauseCluster": PauseClusterMessageOutputTypeDef,
+        "ResumeCluster": ResumeClusterMessageOutputTypeDef,
     },
+    total=False,
 )
 
 ScheduledActionTypeTypeDef = TypedDict(
     "ScheduledActionTypeTypeDef",
     {
         "ResizeCluster": ResizeClusterMessageTypeDef,
         "PauseCluster": PauseClusterMessageTypeDef,
@@ -3831,24 +4027,24 @@
     total=False,
 )
 
 AccountAttributeListTypeDef = TypedDict(
     "AccountAttributeListTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomDomainAssociationsMessageTypeDef = TypedDict(
     "CustomDomainAssociationsMessageTypeDef",
     {
         "Marker": str,
         "Associations": List[AssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OrderableClusterOptionTypeDef = TypedDict(
     "OrderableClusterOptionTypeDef",
     {
         "ClusterVersion": str,
@@ -3870,247 +4066,247 @@
 )
 
 ClusterDbRevisionsMessageTypeDef = TypedDict(
     "ClusterDbRevisionsMessageTypeDef",
     {
         "Marker": str,
         "ClusterDbRevisions": List[ClusterDbRevisionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeDefaultClusterParametersResultTypeDef",
     {
         "DefaultClusterParameters": DefaultClusterParametersTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterParameterGroupsMessageTypeDef = TypedDict(
     "ClusterParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "ParameterGroups": List[ClusterParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterParameterGroupResultTypeDef = TypedDict(
     "CreateClusterParameterGroupResultTypeDef",
     {
         "ClusterParameterGroup": ClusterParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEventSubscriptionResultTypeDef = TypedDict(
     "CreateEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventSubscriptionsMessageTypeDef = TypedDict(
     "EventSubscriptionsMessageTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyEventSubscriptionResultTypeDef = TypedDict(
     "ModifyEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHsmClientCertificateResultTypeDef = TypedDict(
     "CreateHsmClientCertificateResultTypeDef",
     {
         "HsmClientCertificate": HsmClientCertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HsmClientCertificateMessageTypeDef = TypedDict(
     "HsmClientCertificateMessageTypeDef",
     {
         "Marker": str,
         "HsmClientCertificates": List[HsmClientCertificateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHsmConfigurationResultTypeDef = TypedDict(
     "CreateHsmConfigurationResultTypeDef",
     {
         "HsmConfiguration": HsmConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HsmConfigurationMessageTypeDef = TypedDict(
     "HsmConfigurationMessageTypeDef",
     {
         "Marker": str,
         "HsmConfigurations": List[HsmConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSecurityGroupTypeDef = TypedDict(
     "ClusterSecurityGroupTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "Description": str,
         "EC2SecurityGroups": List[EC2SecurityGroupTypeDef],
         "IPRanges": List[IPRangeTypeDef],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 CreateSnapshotCopyGrantResultTypeDef = TypedDict(
     "CreateSnapshotCopyGrantResultTypeDef",
     {
         "SnapshotCopyGrant": SnapshotCopyGrantTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SnapshotCopyGrantMessageTypeDef = TypedDict(
     "SnapshotCopyGrantMessageTypeDef",
     {
         "Marker": str,
         "SnapshotCopyGrants": List[SnapshotCopyGrantTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSnapshotSchedulesOutputMessageTypeDef = TypedDict(
     "DescribeSnapshotSchedulesOutputMessageTypeDef",
     {
         "SnapshotSchedules": List[SnapshotScheduleTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthorizeSnapshotAccessResultTypeDef = TypedDict(
     "AuthorizeSnapshotAccessResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyClusterSnapshotResultTypeDef = TypedDict(
     "CopyClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterSnapshotResultTypeDef = TypedDict(
     "CreateClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterSnapshotResultTypeDef = TypedDict(
     "DeleteClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterSnapshotResultTypeDef = TypedDict(
     "ModifyClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RevokeSnapshotAccessResultTypeDef = TypedDict(
     "RevokeSnapshotAccessResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SnapshotMessageTypeDef = TypedDict(
     "SnapshotMessageTypeDef",
     {
         "Marker": str,
         "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaggedResourceListMessageTypeDef = TypedDict(
     "TaggedResourceListMessageTypeDef",
     {
         "TaggedResources": List[TaggedResourceTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UsageLimitListTypeDef = TypedDict(
     "UsageLimitListTypeDef",
     {
         "UsageLimits": List[UsageLimitTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSharesForConsumerResultTypeDef = TypedDict(
     "DescribeDataSharesForConsumerResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSharesForProducerResultTypeDef = TypedDict(
     "DescribeDataSharesForProducerResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSharesResultTypeDef = TypedDict(
     "DescribeDataSharesResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventCategoriesMessageTypeDef = TypedDict(
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointAccessResponseMetadataTypeDef = TypedDict(
     "EndpointAccessResponseMetadataTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4119,15 +4315,15 @@
         "EndpointStatus": str,
         "EndpointName": str,
         "EndpointCreateTime": datetime,
         "Port": int,
         "Address": str,
         "VpcSecurityGroups": List[VpcSecurityGroupMembershipTypeDef],
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointAccessTypeDef = TypedDict(
     "EndpointAccessTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4155,40 +4351,40 @@
 )
 
 GetReservedNodeExchangeOfferingsOutputMessageTypeDef = TypedDict(
     "GetReservedNodeExchangeOfferingsOutputMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeOfferings": List[ReservedNodeOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedNodeOfferingsMessageTypeDef = TypedDict(
     "ReservedNodeOfferingsMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeOfferings": List[ReservedNodeOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptReservedNodeExchangeOutputMessageTypeDef = TypedDict(
     "AcceptReservedNodeExchangeOutputMessageTypeDef",
     {
         "ExchangedReservedNode": ReservedNodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PurchaseReservedNodeOfferingResultTypeDef = TypedDict(
     "PurchaseReservedNodeOfferingResultTypeDef",
     {
         "ReservedNode": ReservedNodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedNodeConfigurationOptionTypeDef = TypedDict(
     "ReservedNodeConfigurationOptionTypeDef",
     {
         "SourceReservedNode": ReservedNodeTypeDef,
@@ -4199,18 +4395,50 @@
 )
 
 ReservedNodesMessageTypeDef = TypedDict(
     "ReservedNodesMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodes": List[ReservedNodeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ScheduledActionResponseMetadataTypeDef = TypedDict(
+    "ScheduledActionResponseMetadataTypeDef",
+    {
+        "ScheduledActionName": str,
+        "TargetAction": ScheduledActionTypeOutputTypeDef,
+        "Schedule": str,
+        "IamRole": str,
+        "ScheduledActionDescription": str,
+        "State": ScheduledActionStateType,
+        "NextInvocations": List[datetime],
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ScheduledActionTypeDef = TypedDict(
+    "ScheduledActionTypeDef",
+    {
+        "ScheduledActionName": str,
+        "TargetAction": ScheduledActionTypeOutputTypeDef,
+        "Schedule": str,
+        "IamRole": str,
+        "ScheduledActionDescription": str,
+        "State": ScheduledActionStateType,
+        "NextInvocations": List[datetime],
+        "StartTime": datetime,
+        "EndTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredCreateScheduledActionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
         "TargetAction": ScheduledActionTypeTypeDef,
         "Schedule": str,
         "IamRole": str,
@@ -4223,20 +4451,22 @@
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Enable": bool,
     },
     total=False,
 )
 
+
 class CreateScheduledActionMessageRequestTypeDef(
     _RequiredCreateScheduledActionMessageRequestTypeDef,
     _OptionalCreateScheduledActionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyScheduledActionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
     },
 )
 _OptionalModifyScheduledActionMessageRequestTypeDef = TypedDict(
@@ -4249,51 +4479,21 @@
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Enable": bool,
     },
     total=False,
 )
 
+
 class ModifyScheduledActionMessageRequestTypeDef(
     _RequiredModifyScheduledActionMessageRequestTypeDef,
     _OptionalModifyScheduledActionMessageRequestTypeDef,
 ):
     pass
 
-ScheduledActionResponseMetadataTypeDef = TypedDict(
-    "ScheduledActionResponseMetadataTypeDef",
-    {
-        "ScheduledActionName": str,
-        "TargetAction": ScheduledActionTypeTypeDef,
-        "Schedule": str,
-        "IamRole": str,
-        "ScheduledActionDescription": str,
-        "State": ScheduledActionStateType,
-        "NextInvocations": List[datetime],
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ScheduledActionTypeDef = TypedDict(
-    "ScheduledActionTypeDef",
-    {
-        "ScheduledActionName": str,
-        "TargetAction": ScheduledActionTypeTypeDef,
-        "Schedule": str,
-        "IamRole": str,
-        "ScheduledActionDescription": str,
-        "State": ScheduledActionStateType,
-        "NextInvocations": List[datetime],
-        "StartTime": datetime,
-        "EndTime": datetime,
-    },
-    total=False,
-)
 
 MaintenanceTrackTypeDef = TypedDict(
     "MaintenanceTrackTypeDef",
     {
         "MaintenanceTrackName": str,
         "DatabaseVersion": str,
         "UpdateTargets": List[UpdateTargetTypeDef],
@@ -4302,70 +4502,70 @@
 )
 
 OrderableClusterOptionsMessageTypeDef = TypedDict(
     "OrderableClusterOptionsMessageTypeDef",
     {
         "OrderableClusterOptions": List[OrderableClusterOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSubnetGroupTypeDef = TypedDict(
     "ClusterSubnetGroupTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "Description": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[SubnetTypeDef],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 AuthorizeClusterSecurityGroupIngressResultTypeDef = TypedDict(
     "AuthorizeClusterSecurityGroupIngressResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSecurityGroupMessageTypeDef = TypedDict(
     "ClusterSecurityGroupMessageTypeDef",
     {
         "Marker": str,
         "ClusterSecurityGroups": List[ClusterSecurityGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterSecurityGroupResultTypeDef = TypedDict(
     "CreateClusterSecurityGroupResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RevokeClusterSecurityGroupIngressResultTypeDef = TypedDict(
     "RevokeClusterSecurityGroupIngressResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointAccessListTypeDef = TypedDict(
     "EndpointAccessListTypeDef",
     {
         "EndpointAccessList": List[EndpointAccessTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4396,15 +4596,15 @@
         "DataTransferProgress": DataTransferProgressTypeDef,
         "HsmStatus": HsmStatusTypeDef,
         "ClusterSnapshotCopyStatus": ClusterSnapshotCopyStatusTypeDef,
         "ClusterPublicKey": str,
         "ClusterNodes": List[ClusterNodeTypeDef],
         "ElasticIpStatus": ElasticIpStatusTypeDef,
         "ClusterRevisionNumber": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "KmsKeyId": str,
         "EnhancedVpcRouting": bool,
         "IamRoles": List[ClusterIamRoleTypeDef],
         "PendingActions": List[str],
         "MaintenanceTrackName": str,
         "ElasticResizeNumberOfNodeOptions": str,
         "DeferredMaintenanceWindows": List[DeferredMaintenanceWindowTypeDef],
@@ -4428,182 +4628,182 @@
 )
 
 GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef = TypedDict(
     "GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeConfigurationOptionList": List[ReservedNodeConfigurationOptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScheduledActionsMessageTypeDef = TypedDict(
     "ScheduledActionsMessageTypeDef",
     {
         "Marker": str,
         "ScheduledActions": List[ScheduledActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrackListMessageTypeDef = TypedDict(
     "TrackListMessageTypeDef",
     {
         "MaintenanceTracks": List[MaintenanceTrackTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSubnetGroupMessageTypeDef = TypedDict(
     "ClusterSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "ClusterSubnetGroups": List[ClusterSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterSubnetGroupResultTypeDef = TypedDict(
     "CreateClusterSubnetGroupResultTypeDef",
     {
         "ClusterSubnetGroup": ClusterSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterSubnetGroupResultTypeDef = TypedDict(
     "ModifyClusterSubnetGroupResultTypeDef",
     {
         "ClusterSubnetGroup": ClusterSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClustersMessageTypeDef = TypedDict(
     "ClustersMessageTypeDef",
     {
         "Marker": str,
         "Clusters": List[ClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResultTypeDef = TypedDict(
     "CreateClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResultTypeDef = TypedDict(
     "DeleteClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisableSnapshotCopyResultTypeDef = TypedDict(
     "DisableSnapshotCopyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnableSnapshotCopyResultTypeDef = TypedDict(
     "EnableSnapshotCopyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterDbRevisionResultTypeDef = TypedDict(
     "ModifyClusterDbRevisionResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterIamRolesResultTypeDef = TypedDict(
     "ModifyClusterIamRolesResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterMaintenanceResultTypeDef = TypedDict(
     "ModifyClusterMaintenanceResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterResultTypeDef = TypedDict(
     "ModifyClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifySnapshotCopyRetentionPeriodResultTypeDef = TypedDict(
     "ModifySnapshotCopyRetentionPeriodResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PauseClusterResultTypeDef = TypedDict(
     "PauseClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootClusterResultTypeDef = TypedDict(
     "RebootClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResizeClusterResultTypeDef = TypedDict(
     "ResizeClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreFromClusterSnapshotResultTypeDef = TypedDict(
     "RestoreFromClusterSnapshotResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResumeClusterResultTypeDef = TypedDict(
     "ResumeClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RotateEncryptionKeyResultTypeDef = TypedDict(
     "RotateEncryptionKeyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/waiter.py` & `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.0/mypy_boto3_redshift/waiter.pyi` & `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.0/mypy_boto3_redshift.egg-info/PKG-INFO` & `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift
-Version: 1.28.0
-Summary: Type annotations for boto3.Redshift 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Redshift 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-redshift"></a>
 
 # mypy-boto3-redshift
 
 [![PyPI - mypy-boto3-redshift](https://img.shields.io/pypi/v/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift)](https://pepy.tech/project/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
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
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -538,14 +538,15 @@
 
 `mypy_boto3_redshift.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift.type_defs import (
     AcceptReservedNodeExchangeInputMessageRequestTypeDef,
+    ResponseMetadataTypeDef,
     AttributeValueTargetTypeDef,
     AccountWithRestoreAccessTypeDef,
     AquaConfigurationTypeDef,
     AssociateDataShareConsumerMessageRequestTypeDef,
     CertificateAssociationTypeDef,
     AuthenticationProfileTypeDef,
     AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
@@ -554,46 +555,40 @@
     AuthorizeSnapshotAccessMessageRequestTypeDef,
     SupportedPlatformTypeDef,
     DeleteClusterSnapshotMessageTypeDef,
     SnapshotErrorMessageTypeDef,
     BatchModifyClusterSnapshotsMessageRequestTypeDef,
     CancelResizeMessageRequestTypeDef,
     ClusterAssociatedToScheduleTypeDef,
-    ClusterCredentialsTypeDef,
     RevisionTargetTypeDef,
-    ClusterExtendedCredentialsTypeDef,
     ClusterIamRoleTypeDef,
     ClusterNodeTypeDef,
-    ParameterTypeDef,
-    ClusterParameterGroupNameMessageTypeDef,
+    ParameterOutputTypeDef,
     ClusterParameterStatusTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ClusterSecurityGroupMembershipTypeDef,
     ClusterSnapshotCopyStatusTypeDef,
     DataTransferProgressTypeDef,
     DeferredMaintenanceWindowTypeDef,
     ElasticIpStatusTypeDef,
     HsmStatusTypeDef,
     PendingModifiedValuesTypeDef,
     ReservedNodeExchangeStatusTypeDef,
     ResizeInfoTypeDef,
     RestoreStatusTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ClusterVersionTypeDef,
     CopyClusterSnapshotMessageRequestTypeDef,
     CreateAuthenticationProfileMessageRequestTypeDef,
-    CreateAuthenticationProfileResultTypeDef,
+    TagTypeDef,
     CreateCustomDomainAssociationMessageRequestTypeDef,
-    CreateCustomDomainAssociationResultTypeDef,
     CreateEndpointAccessMessageRequestTypeDef,
-    CustomerStorageMessageTypeDef,
     DataShareAssociationTypeDef,
     DeauthorizeDataShareMessageRequestTypeDef,
     DeleteAuthenticationProfileMessageRequestTypeDef,
-    DeleteAuthenticationProfileResultTypeDef,
     DeleteClusterMessageRequestTypeDef,
     DeleteClusterParameterGroupMessageRequestTypeDef,
     DeleteClusterSecurityGroupMessageRequestTypeDef,
     DeleteClusterSnapshotMessageRequestTypeDef,
     DeleteClusterSubnetGroupMessageRequestTypeDef,
     DeleteCustomDomainAssociationMessageRequestTypeDef,
     DeleteEndpointAccessMessageRequestTypeDef,
@@ -603,202 +598,213 @@
     DeleteScheduledActionMessageRequestTypeDef,
     DeleteSnapshotCopyGrantMessageRequestTypeDef,
     DeleteSnapshotScheduleMessageRequestTypeDef,
     DeleteTagsMessageRequestTypeDef,
     DeleteUsageLimitMessageRequestTypeDef,
     DescribeAccountAttributesMessageRequestTypeDef,
     DescribeAuthenticationProfilesMessageRequestTypeDef,
-    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClusterDbRevisionsMessageRequestTypeDef,
-    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
     DescribeClusterParameterGroupsMessageRequestTypeDef,
-    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
     DescribeClusterParametersMessageRequestTypeDef,
-    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
     DescribeClusterSecurityGroupsMessageRequestTypeDef,
     SnapshotSortingEntityTypeDef,
     WaiterConfigTypeDef,
-    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
     DescribeClusterSubnetGroupsMessageRequestTypeDef,
-    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
     DescribeClusterTracksMessageRequestTypeDef,
-    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
     DescribeClusterVersionsMessageRequestTypeDef,
-    DescribeClustersMessageDescribeClustersPaginateTypeDef,
     DescribeClustersMessageRequestTypeDef,
-    DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef,
     DescribeCustomDomainAssociationsMessageRequestTypeDef,
-    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
     DescribeDataSharesForConsumerMessageRequestTypeDef,
-    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
     DescribeDataSharesForProducerMessageRequestTypeDef,
-    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
     DescribeDataSharesMessageRequestTypeDef,
-    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
     DescribeDefaultClusterParametersMessageRequestTypeDef,
-    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
     DescribeEndpointAccessMessageRequestTypeDef,
-    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
     DescribeEndpointAuthorizationMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
-    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
     DescribeHsmClientCertificatesMessageRequestTypeDef,
-    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
     DescribeHsmConfigurationsMessageRequestTypeDef,
     DescribeLoggingStatusMessageRequestTypeDef,
     NodeConfigurationOptionsFilterTypeDef,
-    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
     DescribeOrderableClusterOptionsMessageRequestTypeDef,
     DescribePartnersInputMessageRequestTypeDef,
     PartnerIntegrationInfoTypeDef,
-    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
     DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef,
-    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
     DescribeReservedNodeOfferingsMessageRequestTypeDef,
-    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
     DescribeReservedNodesMessageRequestTypeDef,
     DescribeResizeMessageRequestTypeDef,
     ScheduledActionFilterTypeDef,
-    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
     DescribeSnapshotCopyGrantsMessageRequestTypeDef,
-    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
     DescribeSnapshotSchedulesMessageRequestTypeDef,
-    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
     DescribeTableRestoreStatusMessageRequestTypeDef,
-    DescribeTagsMessageDescribeTagsPaginateTypeDef,
     DescribeTagsMessageRequestTypeDef,
-    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
     DescribeUsageLimitsMessageRequestTypeDef,
     DisableLoggingMessageRequestTypeDef,
     DisableSnapshotCopyMessageRequestTypeDef,
     DisassociateDataShareConsumerMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableLoggingMessageRequestTypeDef,
     EnableSnapshotCopyMessageRequestTypeDef,
     EndpointAuthorizationTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
     EventInfoMapTypeDef,
     EventTypeDef,
     GetClusterCredentialsMessageRequestTypeDef,
     GetClusterCredentialsWithIAMMessageRequestTypeDef,
-    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
     GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
-    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
-    LoggingStatusTypeDef,
     ModifyAquaInputMessageRequestTypeDef,
     ModifyAuthenticationProfileMessageRequestTypeDef,
-    ModifyAuthenticationProfileResultTypeDef,
     ModifyClusterDbRevisionMessageRequestTypeDef,
     ModifyClusterIamRolesMessageRequestTypeDef,
     ModifyClusterMaintenanceMessageRequestTypeDef,
     ModifyClusterMessageRequestTypeDef,
+    ParameterTypeDef,
     ModifyClusterSnapshotMessageRequestTypeDef,
     ModifyClusterSnapshotScheduleMessageRequestTypeDef,
     ModifyClusterSubnetGroupMessageRequestTypeDef,
     ModifyCustomDomainAssociationMessageRequestTypeDef,
-    ModifyCustomDomainAssociationResultTypeDef,
     ModifyEndpointAccessMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     ModifySnapshotScheduleMessageRequestTypeDef,
     ModifyUsageLimitMessageRequestTypeDef,
     NetworkInterfaceTypeDef,
     NodeConfigurationOptionTypeDef,
-    PaginatorConfigTypeDef,
     PartnerIntegrationInputMessageRequestTypeDef,
-    PartnerIntegrationOutputMessageTypeDef,
+    PauseClusterMessageOutputTypeDef,
     PauseClusterMessageRequestTypeDef,
     PauseClusterMessageTypeDef,
     PurchaseReservedNodeOfferingMessageRequestTypeDef,
     RebootClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RejectDataShareMessageRequestTypeDef,
+    ResizeClusterMessageOutputTypeDef,
     ResizeClusterMessageRequestTypeDef,
     ResizeClusterMessageTypeDef,
-    ResizeProgressMessageTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromClusterSnapshotMessageRequestTypeDef,
     RestoreTableFromClusterSnapshotMessageRequestTypeDef,
     TableRestoreStatusTypeDef,
+    ResumeClusterMessageOutputTypeDef,
     ResumeClusterMessageRequestTypeDef,
     ResumeClusterMessageTypeDef,
     RevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     RevokeEndpointAccessMessageRequestTypeDef,
     RevokeSnapshotAccessMessageRequestTypeDef,
     RotateEncryptionKeyMessageRequestTypeDef,
     SupportedOperationTypeDef,
     UpdatePartnerStatusInputMessageRequestTypeDef,
+    ClusterCredentialsTypeDef,
+    ClusterExtendedCredentialsTypeDef,
+    ClusterParameterGroupNameMessageTypeDef,
+    CreateAuthenticationProfileResultTypeDef,
+    CreateCustomDomainAssociationResultTypeDef,
+    CustomerStorageMessageTypeDef,
+    DeleteAuthenticationProfileResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EndpointAuthorizationResponseMetadataTypeDef,
+    LoggingStatusTypeDef,
+    ModifyAuthenticationProfileResultTypeDef,
+    ModifyCustomDomainAssociationResultTypeDef,
+    PartnerIntegrationOutputMessageTypeDef,
+    ResizeProgressMessageTypeDef,
     AccountAttributeTypeDef,
     ModifyAquaOutputMessageTypeDef,
     AssociationTypeDef,
     DescribeAuthenticationProfilesResultTypeDef,
     AvailabilityZoneTypeDef,
     BatchDeleteClusterSnapshotsRequestRequestTypeDef,
     BatchDeleteClusterSnapshotsResultTypeDef,
     BatchModifyClusterSnapshotsOutputMessageTypeDef,
     ClusterDbRevisionTypeDef,
     ClusterParameterGroupDetailsTypeDef,
     DefaultClusterParametersTypeDef,
-    ModifyClusterParameterGroupMessageRequestTypeDef,
-    ResetClusterParameterGroupMessageRequestTypeDef,
     ClusterParameterGroupStatusTypeDef,
     ClusterParameterGroupTypeDef,
-    CreateClusterMessageRequestTypeDef,
-    CreateClusterParameterGroupMessageRequestTypeDef,
-    CreateClusterSecurityGroupMessageRequestTypeDef,
-    CreateClusterSnapshotMessageRequestTypeDef,
-    CreateClusterSubnetGroupMessageRequestTypeDef,
-    CreateEventSubscriptionMessageRequestTypeDef,
-    CreateHsmClientCertificateMessageRequestTypeDef,
-    CreateHsmConfigurationMessageRequestTypeDef,
-    CreateSnapshotCopyGrantMessageRequestTypeDef,
-    CreateSnapshotScheduleMessageRequestTypeDef,
-    CreateTagsMessageRequestTypeDef,
-    CreateUsageLimitMessageRequestTypeDef,
     EC2SecurityGroupTypeDef,
     EventSubscriptionTypeDef,
     HsmClientCertificateTypeDef,
     HsmConfigurationTypeDef,
     IPRangeTypeDef,
     SnapshotCopyGrantTypeDef,
     SnapshotScheduleResponseMetadataTypeDef,
     SnapshotScheduleTypeDef,
     SnapshotTypeDef,
     TaggedResourceTypeDef,
     UsageLimitResponseMetadataTypeDef,
     UsageLimitTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     ClusterVersionsMessageTypeDef,
+    CreateClusterMessageRequestTypeDef,
+    CreateClusterParameterGroupMessageRequestTypeDef,
+    CreateClusterSecurityGroupMessageRequestTypeDef,
+    CreateClusterSnapshotMessageRequestTypeDef,
+    CreateClusterSubnetGroupMessageRequestTypeDef,
+    CreateEventSubscriptionMessageRequestTypeDef,
+    CreateHsmClientCertificateMessageRequestTypeDef,
+    CreateHsmConfigurationMessageRequestTypeDef,
+    CreateSnapshotCopyGrantMessageRequestTypeDef,
+    CreateSnapshotScheduleMessageRequestTypeDef,
+    CreateTagsMessageRequestTypeDef,
+    CreateUsageLimitMessageRequestTypeDef,
     DataShareResponseMetadataTypeDef,
     DataShareTypeDef,
+    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
+    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
+    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
+    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
+    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
+    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
+    DescribeClustersMessageDescribeClustersPaginateTypeDef,
+    DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef,
+    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
+    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
+    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
+    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
+    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
+    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
+    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
+    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
+    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
+    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
+    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
+    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
+    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
+    DescribeTagsMessageDescribeTagsPaginateTypeDef,
+    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
+    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef,
     DescribeClusterSnapshotsMessageRequestTypeDef,
     DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef,
     DescribeClustersMessageClusterAvailableWaitTypeDef,
     DescribeClustersMessageClusterDeletedWaitTypeDef,
     DescribeClustersMessageClusterRestoredWaitTypeDef,
     DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
     DescribeNodeConfigurationOptionsMessageRequestTypeDef,
     DescribePartnersOutputMessageTypeDef,
     DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsMessageRequestTypeDef,
     EndpointAuthorizationListTypeDef,
     EventCategoriesMapTypeDef,
     EventsMessageTypeDef,
+    ModifyClusterParameterGroupMessageRequestTypeDef,
+    ResetClusterParameterGroupMessageRequestTypeDef,
     VpcEndpointTypeDef,
     NodeConfigurationOptionsMessageTypeDef,
     ReservedNodeOfferingTypeDef,
     ReservedNodeTypeDef,
     RestoreTableFromClusterSnapshotResultTypeDef,
     TableRestoreStatusMessageTypeDef,
+    ScheduledActionTypeOutputTypeDef,
     ScheduledActionTypeTypeDef,
     UpdateTargetTypeDef,
     AccountAttributeListTypeDef,
     CustomDomainAssociationsMessageTypeDef,
     OrderableClusterOptionTypeDef,
     SubnetTypeDef,
     ClusterDbRevisionsMessageTypeDef,
@@ -834,18 +840,18 @@
     EndpointTypeDef,
     GetReservedNodeExchangeOfferingsOutputMessageTypeDef,
     ReservedNodeOfferingsMessageTypeDef,
     AcceptReservedNodeExchangeOutputMessageTypeDef,
     PurchaseReservedNodeOfferingResultTypeDef,
     ReservedNodeConfigurationOptionTypeDef,
     ReservedNodesMessageTypeDef,
-    CreateScheduledActionMessageRequestTypeDef,
-    ModifyScheduledActionMessageRequestTypeDef,
     ScheduledActionResponseMetadataTypeDef,
     ScheduledActionTypeDef,
+    CreateScheduledActionMessageRequestTypeDef,
+    ModifyScheduledActionMessageRequestTypeDef,
     MaintenanceTrackTypeDef,
     OrderableClusterOptionsMessageTypeDef,
     ClusterSubnetGroupTypeDef,
     AuthorizeClusterSecurityGroupIngressResultTypeDef,
     ClusterSecurityGroupMessageTypeDef,
     CreateClusterSecurityGroupResultTypeDef,
     RevokeClusterSecurityGroupIngressResultTypeDef,
```

### Comparing `mypy-boto3-redshift-1.28.0/mypy_boto3_redshift.egg-info/SOURCES.txt` & `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.0/setup.py` & `mypy-boto3-redshift-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-redshift",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_redshift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Redshift 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Redshift 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

