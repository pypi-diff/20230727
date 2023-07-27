# Comparing `tmp/mypy-boto3-kafka-1.28.0.tar.gz` & `tmp/mypy-boto3-kafka-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kafka-1.28.0.tar", last modified: Thu Jul  6 20:59:52 2023, max compression
+gzip compressed data, was "mypy-boto3-kafka-1.28.12.tar", last modified: Thu Jul 27 05:34:51 2023, max compression
```

## Comparing `mypy-boto3-kafka-1.28.0.tar` & `mypy-boto3-kafka-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:52.082338 mypy-boto3-kafka-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:23.000000 mypy-boto3-kafka-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-07-06 20:59:52.082338 mypy-boto3-kafka-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18967 2023-07-06 20:44:23.000000 mypy-boto3-kafka-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:52.082338 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-06 20:44:23.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-06 20:44:23.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 20:44:23.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34876 2023-07-06 20:44:24.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34814 2023-07-06 20:44:24.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-07-06 20:44:24.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-07-06 20:44:24.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-07-06 20:44:24.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11460 2023-07-06 20:44:24.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:23.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55042 2023-07-06 20:44:28.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54973 2023-07-06 20:44:27.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:23.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:52.082338 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-07-06 20:59:51.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-06 20:59:51.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:51.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:51.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:51.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 20:59:51.000000 mypy-boto3-kafka-1.28.0/mypy_boto3_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:52.082338 mypy-boto3-kafka-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-06 20:44:23.000000 mypy-boto3-kafka-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.796474 mypy-boto3-kafka-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21610 2023-07-27 05:34:51.796474 mypy-boto3-kafka-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20131 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.792474 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34876 2023-07-27 05:24:27.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34814 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-07-27 05:24:27.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-07-27 05:24:27.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-07-27 05:24:27.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11460 2023-07-27 05:24:27.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64069 2023-07-27 05:24:29.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63988 2023-07-27 05:24:27.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.796474 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21610 2023-07-27 05:34:51.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 05:34:51.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:51.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:34:51.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:51.796474 mypy-boto3-kafka-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/setup.py
```

### Comparing `mypy-boto3-kafka-1.28.0/LICENSE` & `mypy-boto3-kafka-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.0/PKG-INFO` & `mypy-boto3-kafka-1.28.12/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-kafka
-Version: 1.28.0
-Summary: Type annotations for boto3.Kafka 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kafka type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-kafka"></a>
 
 # mypy-boto3-kafka
 
 [![PyPI - mypy-boto3-kafka](https://img.shields.io/pypi/v/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kafka?color=blue)](https://pypistats.org/packages/mypy-boto3-kafka)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kafka)](https://pepy.tech/project/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
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
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
 
@@ -373,28 +341,36 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kafka.type_defs import (
     BatchAssociateScramSecretRequestRequestTypeDef,
     UnprocessedScramSecretTypeDef,
     BatchDisassociateScramSecretRequestRequestTypeDef,
+    ProvisionedThroughputOutputTypeDef,
     ProvisionedThroughputTypeDef,
+    CloudWatchLogsOutputTypeDef,
+    FirehoseOutputTypeDef,
+    S3OutputTypeDef,
     CloudWatchLogsTypeDef,
     FirehoseTypeDef,
     S3TypeDef,
     BrokerSoftwareInfoTypeDef,
+    TlsOutputTypeDef,
+    UnauthenticatedOutputTypeDef,
     TlsTypeDef,
     UnauthenticatedTypeDef,
     ClientVpcConnectionTypeDef,
     StateInfoTypeDef,
     ErrorInfoTypeDef,
     ClusterOperationStepInfoTypeDef,
     CompatibleKafkaVersionTypeDef,
+    ConfigurationInfoOutputTypeDef,
     ConfigurationInfoTypeDef,
     ConfigurationRevisionTypeDef,
+    PublicAccessOutputTypeDef,
     PublicAccessTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationRequestRequestTypeDef,
     CreateVpcConnectionRequestRequestTypeDef,
     CreateVpcConnectionResponseTypeDef,
     DeleteClusterPolicyRequestRequestTypeDef,
@@ -409,22 +385,26 @@
     DescribeClusterV2RequestRequestTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
     DescribeVpcConnectionRequestRequestTypeDef,
     DescribeVpcConnectionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionAtRestOutputTypeDef,
     EncryptionAtRestTypeDef,
+    EncryptionInTransitOutputTypeDef,
     EncryptionInTransitTypeDef,
     GetBootstrapBrokersRequestRequestTypeDef,
     GetBootstrapBrokersResponseTypeDef,
     GetClusterPolicyRequestRequestTypeDef,
     GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsRequestRequestTypeDef,
+    IamOutputTypeDef,
     IamTypeDef,
+    JmxExporterInfoOutputTypeDef,
     JmxExporterInfoTypeDef,
     JmxExporterTypeDef,
     KafkaVersionTypeDef,
     ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
     ListClientVpcConnectionsRequestRequestTypeDef,
     ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     ListClusterOperationsRequestRequestTypeDef,
@@ -444,26 +424,29 @@
     ListScramSecretsRequestRequestTypeDef,
     ListScramSecretsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef,
     ListVpcConnectionsRequestRequestTypeDef,
     VpcConnectionTypeDef,
+    NodeExporterInfoOutputTypeDef,
     NodeExporterInfoTypeDef,
     NodeExporterTypeDef,
     ZookeeperNodeInfoTypeDef,
     PaginatorConfigTypeDef,
     PutClusterPolicyRequestRequestTypeDef,
     PutClusterPolicyResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
     RebootBrokerResponseTypeDef,
     RejectClientVpcConnectionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    ScramOutputTypeDef,
     ScramTypeDef,
     VpcConfigTypeDef,
+    VpcConfigOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrokerCountRequestRequestTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
     UpdateBrokerTypeRequestRequestTypeDef,
     UpdateBrokerTypeResponseTypeDef,
@@ -471,74 +454,94 @@
     UpdateClusterKafkaVersionResponseTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     UpdateConnectivityResponseTypeDef,
     UpdateMonitoringResponseTypeDef,
     UpdateSecurityResponseTypeDef,
     UpdateStorageResponseTypeDef,
     UserIdentityTypeDef,
+    VpcConnectivityTlsOutputTypeDef,
     VpcConnectivityTlsTypeDef,
+    VpcConnectivityIamOutputTypeDef,
     VpcConnectivityIamTypeDef,
+    VpcConnectivityScramOutputTypeDef,
     VpcConnectivityScramTypeDef,
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
+    BrokerEBSVolumeInfoOutputTypeDef,
+    EBSStorageInfoOutputTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     EBSStorageInfoTypeDef,
     UpdateStorageRequestRequestTypeDef,
+    BrokerLogsOutputTypeDef,
     BrokerLogsTypeDef,
     BrokerNodeInfoTypeDef,
     ListClientVpcConnectionsResponseTypeDef,
     ClusterOperationStepTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     UpdateClusterConfigurationRequestRequestTypeDef,
     UpdateClusterKafkaVersionRequestRequestTypeDef,
     ConfigurationTypeDef,
     CreateConfigurationResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     UpdateConfigurationResponseTypeDef,
+    EncryptionInfoOutputTypeDef,
     EncryptionInfoTypeDef,
+    ServerlessSaslOutputTypeDef,
     ServerlessSaslTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListVpcConnectionsResponseTypeDef,
+    PrometheusInfoOutputTypeDef,
     PrometheusInfoTypeDef,
     PrometheusTypeDef,
+    SaslOutputTypeDef,
     SaslTypeDef,
     VpcConnectionInfoTypeDef,
+    VpcConnectivitySaslOutputTypeDef,
     VpcConnectivitySaslTypeDef,
+    StorageInfoOutputTypeDef,
     UpdateBrokerStorageRequestRequestTypeDef,
     StorageInfoTypeDef,
+    LoggingInfoOutputTypeDef,
     LoggingInfoTypeDef,
     NodeInfoTypeDef,
     ListConfigurationsResponseTypeDef,
+    ServerlessClientAuthenticationOutputTypeDef,
     ServerlessClientAuthenticationTypeDef,
+    OpenMonitoringInfoOutputTypeDef,
     OpenMonitoringInfoTypeDef,
     OpenMonitoringTypeDef,
+    ClientAuthenticationOutputTypeDef,
     ClientAuthenticationTypeDef,
+    VpcConnectivityClientAuthenticationOutputTypeDef,
     VpcConnectivityClientAuthenticationTypeDef,
     ListNodesResponseTypeDef,
-    ServerlessRequestTypeDef,
     ServerlessTypeDef,
+    ServerlessRequestTypeDef,
     UpdateMonitoringRequestRequestTypeDef,
     UpdateSecurityRequestRequestTypeDef,
+    VpcConnectivityOutputTypeDef,
     VpcConnectivityTypeDef,
+    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
-    BrokerNodeGroupInfoTypeDef,
+    BrokerNodeGroupInfoOutputTypeDef,
     MutableClusterInfoTypeDef,
+    BrokerNodeGroupInfoTypeDef,
     UpdateConnectivityRequestRequestTypeDef,
     ClusterInfoTypeDef,
-    CreateClusterRequestRequestTypeDef,
-    ProvisionedRequestTypeDef,
     ProvisionedTypeDef,
     ClusterOperationInfoTypeDef,
+    CreateClusterRequestRequestTypeDef,
+    ProvisionedRequestTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
-    CreateClusterV2RequestRequestTypeDef,
     ClusterTypeDef,
     DescribeClusterOperationResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
+    CreateClusterV2RequestRequestTypeDef,
     DescribeClusterV2ResponseTypeDef,
     ListClustersV2ResponseTypeDef,
 )
 
 
 def get_structure() -> BatchAssociateScramSecretRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-kafka-1.28.0/README.md` & `mypy-boto3-kafka-1.28.12/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-kafka
+Version: 1.28.12
+Summary: Type annotations for boto3.Kafka 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 kafka type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-kafka"></a>
 
 # mypy-boto3-kafka
 
 [![PyPI - mypy-boto3-kafka](https://img.shields.io/pypi/v/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kafka?color=blue)](https://pypistats.org/packages/mypy-boto3-kafka)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kafka)](https://pepy.tech/project/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
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
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,28 +373,36 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kafka.type_defs import (
     BatchAssociateScramSecretRequestRequestTypeDef,
     UnprocessedScramSecretTypeDef,
     BatchDisassociateScramSecretRequestRequestTypeDef,
+    ProvisionedThroughputOutputTypeDef,
     ProvisionedThroughputTypeDef,
+    CloudWatchLogsOutputTypeDef,
+    FirehoseOutputTypeDef,
+    S3OutputTypeDef,
     CloudWatchLogsTypeDef,
     FirehoseTypeDef,
     S3TypeDef,
     BrokerSoftwareInfoTypeDef,
+    TlsOutputTypeDef,
+    UnauthenticatedOutputTypeDef,
     TlsTypeDef,
     UnauthenticatedTypeDef,
     ClientVpcConnectionTypeDef,
     StateInfoTypeDef,
     ErrorInfoTypeDef,
     ClusterOperationStepInfoTypeDef,
     CompatibleKafkaVersionTypeDef,
+    ConfigurationInfoOutputTypeDef,
     ConfigurationInfoTypeDef,
     ConfigurationRevisionTypeDef,
+    PublicAccessOutputTypeDef,
     PublicAccessTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationRequestRequestTypeDef,
     CreateVpcConnectionRequestRequestTypeDef,
     CreateVpcConnectionResponseTypeDef,
     DeleteClusterPolicyRequestRequestTypeDef,
@@ -377,22 +417,26 @@
     DescribeClusterV2RequestRequestTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
     DescribeVpcConnectionRequestRequestTypeDef,
     DescribeVpcConnectionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionAtRestOutputTypeDef,
     EncryptionAtRestTypeDef,
+    EncryptionInTransitOutputTypeDef,
     EncryptionInTransitTypeDef,
     GetBootstrapBrokersRequestRequestTypeDef,
     GetBootstrapBrokersResponseTypeDef,
     GetClusterPolicyRequestRequestTypeDef,
     GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsRequestRequestTypeDef,
+    IamOutputTypeDef,
     IamTypeDef,
+    JmxExporterInfoOutputTypeDef,
     JmxExporterInfoTypeDef,
     JmxExporterTypeDef,
     KafkaVersionTypeDef,
     ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
     ListClientVpcConnectionsRequestRequestTypeDef,
     ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     ListClusterOperationsRequestRequestTypeDef,
@@ -412,26 +456,29 @@
     ListScramSecretsRequestRequestTypeDef,
     ListScramSecretsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef,
     ListVpcConnectionsRequestRequestTypeDef,
     VpcConnectionTypeDef,
+    NodeExporterInfoOutputTypeDef,
     NodeExporterInfoTypeDef,
     NodeExporterTypeDef,
     ZookeeperNodeInfoTypeDef,
     PaginatorConfigTypeDef,
     PutClusterPolicyRequestRequestTypeDef,
     PutClusterPolicyResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
     RebootBrokerResponseTypeDef,
     RejectClientVpcConnectionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    ScramOutputTypeDef,
     ScramTypeDef,
     VpcConfigTypeDef,
+    VpcConfigOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrokerCountRequestRequestTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
     UpdateBrokerTypeRequestRequestTypeDef,
     UpdateBrokerTypeResponseTypeDef,
@@ -439,74 +486,94 @@
     UpdateClusterKafkaVersionResponseTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     UpdateConnectivityResponseTypeDef,
     UpdateMonitoringResponseTypeDef,
     UpdateSecurityResponseTypeDef,
     UpdateStorageResponseTypeDef,
     UserIdentityTypeDef,
+    VpcConnectivityTlsOutputTypeDef,
     VpcConnectivityTlsTypeDef,
+    VpcConnectivityIamOutputTypeDef,
     VpcConnectivityIamTypeDef,
+    VpcConnectivityScramOutputTypeDef,
     VpcConnectivityScramTypeDef,
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
+    BrokerEBSVolumeInfoOutputTypeDef,
+    EBSStorageInfoOutputTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     EBSStorageInfoTypeDef,
     UpdateStorageRequestRequestTypeDef,
+    BrokerLogsOutputTypeDef,
     BrokerLogsTypeDef,
     BrokerNodeInfoTypeDef,
     ListClientVpcConnectionsResponseTypeDef,
     ClusterOperationStepTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     UpdateClusterConfigurationRequestRequestTypeDef,
     UpdateClusterKafkaVersionRequestRequestTypeDef,
     ConfigurationTypeDef,
     CreateConfigurationResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     UpdateConfigurationResponseTypeDef,
+    EncryptionInfoOutputTypeDef,
     EncryptionInfoTypeDef,
+    ServerlessSaslOutputTypeDef,
     ServerlessSaslTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListVpcConnectionsResponseTypeDef,
+    PrometheusInfoOutputTypeDef,
     PrometheusInfoTypeDef,
     PrometheusTypeDef,
+    SaslOutputTypeDef,
     SaslTypeDef,
     VpcConnectionInfoTypeDef,
+    VpcConnectivitySaslOutputTypeDef,
     VpcConnectivitySaslTypeDef,
+    StorageInfoOutputTypeDef,
     UpdateBrokerStorageRequestRequestTypeDef,
     StorageInfoTypeDef,
+    LoggingInfoOutputTypeDef,
     LoggingInfoTypeDef,
     NodeInfoTypeDef,
     ListConfigurationsResponseTypeDef,
+    ServerlessClientAuthenticationOutputTypeDef,
     ServerlessClientAuthenticationTypeDef,
+    OpenMonitoringInfoOutputTypeDef,
     OpenMonitoringInfoTypeDef,
     OpenMonitoringTypeDef,
+    ClientAuthenticationOutputTypeDef,
     ClientAuthenticationTypeDef,
+    VpcConnectivityClientAuthenticationOutputTypeDef,
     VpcConnectivityClientAuthenticationTypeDef,
     ListNodesResponseTypeDef,
-    ServerlessRequestTypeDef,
     ServerlessTypeDef,
+    ServerlessRequestTypeDef,
     UpdateMonitoringRequestRequestTypeDef,
     UpdateSecurityRequestRequestTypeDef,
+    VpcConnectivityOutputTypeDef,
     VpcConnectivityTypeDef,
+    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
-    BrokerNodeGroupInfoTypeDef,
+    BrokerNodeGroupInfoOutputTypeDef,
     MutableClusterInfoTypeDef,
+    BrokerNodeGroupInfoTypeDef,
     UpdateConnectivityRequestRequestTypeDef,
     ClusterInfoTypeDef,
-    CreateClusterRequestRequestTypeDef,
-    ProvisionedRequestTypeDef,
     ProvisionedTypeDef,
     ClusterOperationInfoTypeDef,
+    CreateClusterRequestRequestTypeDef,
+    ProvisionedRequestTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
-    CreateClusterV2RequestRequestTypeDef,
     ClusterTypeDef,
     DescribeClusterOperationResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
+    CreateClusterV2RequestRequestTypeDef,
     DescribeClusterV2ResponseTypeDef,
     ListClustersV2ResponseTypeDef,
 )
 
 
 def get_structure() -> BatchAssociateScramSecretRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/__init__.py` & `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/__init__.pyi` & `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/__main__.py` & `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Kafka 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Kafka 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka\nOther"
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

### Comparing `mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/client.py` & `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/client.pyi` & `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/literals.py` & `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -206,14 +206,15 @@
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
@@ -292,26 +293,28 @@
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

### Comparing `mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/literals.pyi` & `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -204,14 +204,15 @@
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
@@ -290,26 +291,28 @@
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

### Comparing `mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/paginator.py` & `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/paginator.pyi` & `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/type_defs.py` & `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,28 +39,36 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BatchAssociateScramSecretRequestRequestTypeDef",
     "UnprocessedScramSecretTypeDef",
     "BatchDisassociateScramSecretRequestRequestTypeDef",
+    "ProvisionedThroughputOutputTypeDef",
     "ProvisionedThroughputTypeDef",
+    "CloudWatchLogsOutputTypeDef",
+    "FirehoseOutputTypeDef",
+    "S3OutputTypeDef",
     "CloudWatchLogsTypeDef",
     "FirehoseTypeDef",
     "S3TypeDef",
     "BrokerSoftwareInfoTypeDef",
+    "TlsOutputTypeDef",
+    "UnauthenticatedOutputTypeDef",
     "TlsTypeDef",
     "UnauthenticatedTypeDef",
     "ClientVpcConnectionTypeDef",
     "StateInfoTypeDef",
     "ErrorInfoTypeDef",
     "ClusterOperationStepInfoTypeDef",
     "CompatibleKafkaVersionTypeDef",
+    "ConfigurationInfoOutputTypeDef",
     "ConfigurationInfoTypeDef",
     "ConfigurationRevisionTypeDef",
+    "PublicAccessOutputTypeDef",
     "PublicAccessTypeDef",
     "CreateClusterResponseTypeDef",
     "CreateClusterV2ResponseTypeDef",
     "CreateConfigurationRequestRequestTypeDef",
     "CreateVpcConnectionRequestRequestTypeDef",
     "CreateVpcConnectionResponseTypeDef",
     "DeleteClusterPolicyRequestRequestTypeDef",
@@ -75,22 +83,26 @@
     "DescribeClusterV2RequestRequestTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     "DescribeConfigurationRevisionResponseTypeDef",
     "DescribeVpcConnectionRequestRequestTypeDef",
     "DescribeVpcConnectionResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionAtRestOutputTypeDef",
     "EncryptionAtRestTypeDef",
+    "EncryptionInTransitOutputTypeDef",
     "EncryptionInTransitTypeDef",
     "GetBootstrapBrokersRequestRequestTypeDef",
     "GetBootstrapBrokersResponseTypeDef",
     "GetClusterPolicyRequestRequestTypeDef",
     "GetClusterPolicyResponseTypeDef",
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
+    "IamOutputTypeDef",
     "IamTypeDef",
+    "JmxExporterInfoOutputTypeDef",
     "JmxExporterInfoTypeDef",
     "JmxExporterTypeDef",
     "KafkaVersionTypeDef",
     "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
     "ListClientVpcConnectionsRequestRequestTypeDef",
     "ListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
     "ListClusterOperationsRequestRequestTypeDef",
@@ -110,26 +122,29 @@
     "ListScramSecretsRequestRequestTypeDef",
     "ListScramSecretsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
     "ListVpcConnectionsRequestRequestTypeDef",
     "VpcConnectionTypeDef",
+    "NodeExporterInfoOutputTypeDef",
     "NodeExporterInfoTypeDef",
     "NodeExporterTypeDef",
     "ZookeeperNodeInfoTypeDef",
     "PaginatorConfigTypeDef",
     "PutClusterPolicyRequestRequestTypeDef",
     "PutClusterPolicyResponseTypeDef",
     "RebootBrokerRequestRequestTypeDef",
     "RebootBrokerResponseTypeDef",
     "RejectClientVpcConnectionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "ScramOutputTypeDef",
     "ScramTypeDef",
     "VpcConfigTypeDef",
+    "VpcConfigOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrokerCountRequestRequestTypeDef",
     "UpdateBrokerCountResponseTypeDef",
     "UpdateBrokerStorageResponseTypeDef",
     "UpdateBrokerTypeRequestRequestTypeDef",
     "UpdateBrokerTypeResponseTypeDef",
@@ -137,74 +152,94 @@
     "UpdateClusterKafkaVersionResponseTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "UpdateConnectivityResponseTypeDef",
     "UpdateMonitoringResponseTypeDef",
     "UpdateSecurityResponseTypeDef",
     "UpdateStorageResponseTypeDef",
     "UserIdentityTypeDef",
+    "VpcConnectivityTlsOutputTypeDef",
     "VpcConnectivityTlsTypeDef",
+    "VpcConnectivityIamOutputTypeDef",
     "VpcConnectivityIamTypeDef",
+    "VpcConnectivityScramOutputTypeDef",
     "VpcConnectivityScramTypeDef",
     "BatchAssociateScramSecretResponseTypeDef",
     "BatchDisassociateScramSecretResponseTypeDef",
+    "BrokerEBSVolumeInfoOutputTypeDef",
+    "EBSStorageInfoOutputTypeDef",
     "BrokerEBSVolumeInfoTypeDef",
     "EBSStorageInfoTypeDef",
     "UpdateStorageRequestRequestTypeDef",
+    "BrokerLogsOutputTypeDef",
     "BrokerLogsTypeDef",
     "BrokerNodeInfoTypeDef",
     "ListClientVpcConnectionsResponseTypeDef",
     "ClusterOperationStepTypeDef",
     "GetCompatibleKafkaVersionsResponseTypeDef",
     "UpdateClusterConfigurationRequestRequestTypeDef",
     "UpdateClusterKafkaVersionRequestRequestTypeDef",
     "ConfigurationTypeDef",
     "CreateConfigurationResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
     "UpdateConfigurationResponseTypeDef",
+    "EncryptionInfoOutputTypeDef",
     "EncryptionInfoTypeDef",
+    "ServerlessSaslOutputTypeDef",
     "ServerlessSaslTypeDef",
     "ListKafkaVersionsResponseTypeDef",
     "ListVpcConnectionsResponseTypeDef",
+    "PrometheusInfoOutputTypeDef",
     "PrometheusInfoTypeDef",
     "PrometheusTypeDef",
+    "SaslOutputTypeDef",
     "SaslTypeDef",
     "VpcConnectionInfoTypeDef",
+    "VpcConnectivitySaslOutputTypeDef",
     "VpcConnectivitySaslTypeDef",
+    "StorageInfoOutputTypeDef",
     "UpdateBrokerStorageRequestRequestTypeDef",
     "StorageInfoTypeDef",
+    "LoggingInfoOutputTypeDef",
     "LoggingInfoTypeDef",
     "NodeInfoTypeDef",
     "ListConfigurationsResponseTypeDef",
+    "ServerlessClientAuthenticationOutputTypeDef",
     "ServerlessClientAuthenticationTypeDef",
+    "OpenMonitoringInfoOutputTypeDef",
     "OpenMonitoringInfoTypeDef",
     "OpenMonitoringTypeDef",
+    "ClientAuthenticationOutputTypeDef",
     "ClientAuthenticationTypeDef",
+    "VpcConnectivityClientAuthenticationOutputTypeDef",
     "VpcConnectivityClientAuthenticationTypeDef",
     "ListNodesResponseTypeDef",
-    "ServerlessRequestTypeDef",
     "ServerlessTypeDef",
+    "ServerlessRequestTypeDef",
     "UpdateMonitoringRequestRequestTypeDef",
     "UpdateSecurityRequestRequestTypeDef",
+    "VpcConnectivityOutputTypeDef",
     "VpcConnectivityTypeDef",
+    "ConnectivityInfoOutputTypeDef",
     "ConnectivityInfoTypeDef",
-    "BrokerNodeGroupInfoTypeDef",
+    "BrokerNodeGroupInfoOutputTypeDef",
     "MutableClusterInfoTypeDef",
+    "BrokerNodeGroupInfoTypeDef",
     "UpdateConnectivityRequestRequestTypeDef",
     "ClusterInfoTypeDef",
-    "CreateClusterRequestRequestTypeDef",
-    "ProvisionedRequestTypeDef",
     "ProvisionedTypeDef",
     "ClusterOperationInfoTypeDef",
+    "CreateClusterRequestRequestTypeDef",
+    "ProvisionedRequestTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
-    "CreateClusterV2RequestRequestTypeDef",
     "ClusterTypeDef",
     "DescribeClusterOperationResponseTypeDef",
     "ListClusterOperationsResponseTypeDef",
+    "CreateClusterV2RequestRequestTypeDef",
     "DescribeClusterV2ResponseTypeDef",
     "ListClustersV2ResponseTypeDef",
 )
 
 BatchAssociateScramSecretRequestRequestTypeDef = TypedDict(
     "BatchAssociateScramSecretRequestRequestTypeDef",
     {
@@ -227,23 +262,92 @@
     "BatchDisassociateScramSecretRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "SecretArnList": Sequence[str],
     },
 )
 
+ProvisionedThroughputOutputTypeDef = TypedDict(
+    "ProvisionedThroughputOutputTypeDef",
+    {
+        "Enabled": bool,
+        "VolumeThroughput": int,
+    },
+    total=False,
+)
+
 ProvisionedThroughputTypeDef = TypedDict(
     "ProvisionedThroughputTypeDef",
     {
         "Enabled": bool,
         "VolumeThroughput": int,
     },
     total=False,
 )
 
+_RequiredCloudWatchLogsOutputTypeDef = TypedDict(
+    "_RequiredCloudWatchLogsOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalCloudWatchLogsOutputTypeDef = TypedDict(
+    "_OptionalCloudWatchLogsOutputTypeDef",
+    {
+        "LogGroup": str,
+    },
+    total=False,
+)
+
+
+class CloudWatchLogsOutputTypeDef(
+    _RequiredCloudWatchLogsOutputTypeDef, _OptionalCloudWatchLogsOutputTypeDef
+):
+    pass
+
+
+_RequiredFirehoseOutputTypeDef = TypedDict(
+    "_RequiredFirehoseOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalFirehoseOutputTypeDef = TypedDict(
+    "_OptionalFirehoseOutputTypeDef",
+    {
+        "DeliveryStream": str,
+    },
+    total=False,
+)
+
+
+class FirehoseOutputTypeDef(_RequiredFirehoseOutputTypeDef, _OptionalFirehoseOutputTypeDef):
+    pass
+
+
+_RequiredS3OutputTypeDef = TypedDict(
+    "_RequiredS3OutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalS3OutputTypeDef = TypedDict(
+    "_OptionalS3OutputTypeDef",
+    {
+        "Bucket": str,
+        "Prefix": str,
+    },
+    total=False,
+)
+
+
+class S3OutputTypeDef(_RequiredS3OutputTypeDef, _OptionalS3OutputTypeDef):
+    pass
+
+
 _RequiredCloudWatchLogsTypeDef = TypedDict(
     "_RequiredCloudWatchLogsTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalCloudWatchLogsTypeDef = TypedDict(
@@ -304,14 +408,31 @@
         "ConfigurationArn": str,
         "ConfigurationRevision": int,
         "KafkaVersion": str,
     },
     total=False,
 )
 
+TlsOutputTypeDef = TypedDict(
+    "TlsOutputTypeDef",
+    {
+        "CertificateAuthorityArnList": List[str],
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+UnauthenticatedOutputTypeDef = TypedDict(
+    "UnauthenticatedOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 TlsTypeDef = TypedDict(
     "TlsTypeDef",
     {
         "CertificateAuthorityArnList": Sequence[str],
         "Enabled": bool,
     },
     total=False,
@@ -380,14 +501,22 @@
     {
         "SourceVersion": str,
         "TargetVersions": List[str],
     },
     total=False,
 )
 
+ConfigurationInfoOutputTypeDef = TypedDict(
+    "ConfigurationInfoOutputTypeDef",
+    {
+        "Arn": str,
+        "Revision": int,
+    },
+)
+
 ConfigurationInfoTypeDef = TypedDict(
     "ConfigurationInfoTypeDef",
     {
         "Arn": str,
         "Revision": int,
     },
 )
@@ -410,14 +539,22 @@
 
 class ConfigurationRevisionTypeDef(
     _RequiredConfigurationRevisionTypeDef, _OptionalConfigurationRevisionTypeDef
 ):
     pass
 
 
+PublicAccessOutputTypeDef = TypedDict(
+    "PublicAccessOutputTypeDef",
+    {
+        "Type": str,
+    },
+    total=False,
+)
+
 PublicAccessTypeDef = TypedDict(
     "PublicAccessTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
@@ -651,21 +788,37 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionAtRestOutputTypeDef = TypedDict(
+    "EncryptionAtRestOutputTypeDef",
+    {
+        "DataVolumeKMSKeyId": str,
+    },
+)
+
 EncryptionAtRestTypeDef = TypedDict(
     "EncryptionAtRestTypeDef",
     {
         "DataVolumeKMSKeyId": str,
     },
 )
 
+EncryptionInTransitOutputTypeDef = TypedDict(
+    "EncryptionInTransitOutputTypeDef",
+    {
+        "ClientBroker": ClientBrokerType,
+        "InCluster": bool,
+    },
+    total=False,
+)
+
 EncryptionInTransitTypeDef = TypedDict(
     "EncryptionInTransitTypeDef",
     {
         "ClientBroker": ClientBrokerType,
         "InCluster": bool,
     },
     total=False,
@@ -715,22 +868,37 @@
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
     total=False,
 )
 
+IamOutputTypeDef = TypedDict(
+    "IamOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 IamTypeDef = TypedDict(
     "IamTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+JmxExporterInfoOutputTypeDef = TypedDict(
+    "JmxExporterInfoOutputTypeDef",
+    {
+        "EnabledInBroker": bool,
+    },
+)
+
 JmxExporterInfoTypeDef = TypedDict(
     "JmxExporterInfoTypeDef",
     {
         "EnabledInBroker": bool,
     },
 )
 
@@ -1107,14 +1275,21 @@
 )
 
 
 class VpcConnectionTypeDef(_RequiredVpcConnectionTypeDef, _OptionalVpcConnectionTypeDef):
     pass
 
 
+NodeExporterInfoOutputTypeDef = TypedDict(
+    "NodeExporterInfoOutputTypeDef",
+    {
+        "EnabledInBroker": bool,
+    },
+)
+
 NodeExporterInfoTypeDef = TypedDict(
     "NodeExporterInfoTypeDef",
     {
         "EnabledInBroker": bool,
     },
 )
 
@@ -1209,14 +1384,22 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+ScramOutputTypeDef = TypedDict(
+    "ScramOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 ScramTypeDef = TypedDict(
     "ScramTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -1236,14 +1419,33 @@
 )
 
 
 class VpcConfigTypeDef(_RequiredVpcConfigTypeDef, _OptionalVpcConfigTypeDef):
     pass
 
 
+_RequiredVpcConfigOutputTypeDef = TypedDict(
+    "_RequiredVpcConfigOutputTypeDef",
+    {
+        "SubnetIds": List[str],
+    },
+)
+_OptionalVpcConfigOutputTypeDef = TypedDict(
+    "_OptionalVpcConfigOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+    },
+    total=False,
+)
+
+
+class VpcConfigOutputTypeDef(_RequiredVpcConfigOutputTypeDef, _OptionalVpcConfigOutputTypeDef):
+    pass
+
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1383,30 +1585,54 @@
     {
         "Type": UserIdentityTypeType,
         "PrincipalId": str,
     },
     total=False,
 )
 
+VpcConnectivityTlsOutputTypeDef = TypedDict(
+    "VpcConnectivityTlsOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 VpcConnectivityTlsTypeDef = TypedDict(
     "VpcConnectivityTlsTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+VpcConnectivityIamOutputTypeDef = TypedDict(
+    "VpcConnectivityIamOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 VpcConnectivityIamTypeDef = TypedDict(
     "VpcConnectivityIamTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+VpcConnectivityScramOutputTypeDef = TypedDict(
+    "VpcConnectivityScramOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 VpcConnectivityScramTypeDef = TypedDict(
     "VpcConnectivityScramTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -1425,14 +1651,45 @@
     {
         "ClusterArn": str,
         "UnprocessedScramSecrets": List[UnprocessedScramSecretTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredBrokerEBSVolumeInfoOutputTypeDef = TypedDict(
+    "_RequiredBrokerEBSVolumeInfoOutputTypeDef",
+    {
+        "KafkaBrokerNodeId": str,
+    },
+)
+_OptionalBrokerEBSVolumeInfoOutputTypeDef = TypedDict(
+    "_OptionalBrokerEBSVolumeInfoOutputTypeDef",
+    {
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "VolumeSizeGB": int,
+    },
+    total=False,
+)
+
+
+class BrokerEBSVolumeInfoOutputTypeDef(
+    _RequiredBrokerEBSVolumeInfoOutputTypeDef, _OptionalBrokerEBSVolumeInfoOutputTypeDef
+):
+    pass
+
+
+EBSStorageInfoOutputTypeDef = TypedDict(
+    "EBSStorageInfoOutputTypeDef",
+    {
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "VolumeSize": int,
+    },
+    total=False,
+)
+
 _RequiredBrokerEBSVolumeInfoTypeDef = TypedDict(
     "_RequiredBrokerEBSVolumeInfoTypeDef",
     {
         "KafkaBrokerNodeId": str,
     },
 )
 _OptionalBrokerEBSVolumeInfoTypeDef = TypedDict(
@@ -1480,14 +1737,24 @@
 
 class UpdateStorageRequestRequestTypeDef(
     _RequiredUpdateStorageRequestRequestTypeDef, _OptionalUpdateStorageRequestRequestTypeDef
 ):
     pass
 
 
+BrokerLogsOutputTypeDef = TypedDict(
+    "BrokerLogsOutputTypeDef",
+    {
+        "CloudWatchLogs": CloudWatchLogsOutputTypeDef,
+        "Firehose": FirehoseOutputTypeDef,
+        "S3": S3OutputTypeDef,
+    },
+    total=False,
+)
+
 BrokerLogsTypeDef = TypedDict(
     "BrokerLogsTypeDef",
     {
         "CloudWatchLogs": CloudWatchLogsTypeDef,
         "Firehose": FirehoseTypeDef,
         "S3": S3TypeDef,
     },
@@ -1619,23 +1886,40 @@
     {
         "Arn": str,
         "LatestRevision": ConfigurationRevisionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionInfoOutputTypeDef = TypedDict(
+    "EncryptionInfoOutputTypeDef",
+    {
+        "EncryptionAtRest": EncryptionAtRestOutputTypeDef,
+        "EncryptionInTransit": EncryptionInTransitOutputTypeDef,
+    },
+    total=False,
+)
+
 EncryptionInfoTypeDef = TypedDict(
     "EncryptionInfoTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "EncryptionInTransit": EncryptionInTransitTypeDef,
     },
     total=False,
 )
 
+ServerlessSaslOutputTypeDef = TypedDict(
+    "ServerlessSaslOutputTypeDef",
+    {
+        "Iam": IamOutputTypeDef,
+    },
+    total=False,
+)
+
 ServerlessSaslTypeDef = TypedDict(
     "ServerlessSaslTypeDef",
     {
         "Iam": IamTypeDef,
     },
     total=False,
 )
@@ -1654,14 +1938,23 @@
     {
         "VpcConnections": List[VpcConnectionTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PrometheusInfoOutputTypeDef = TypedDict(
+    "PrometheusInfoOutputTypeDef",
+    {
+        "JmxExporter": JmxExporterInfoOutputTypeDef,
+        "NodeExporter": NodeExporterInfoOutputTypeDef,
+    },
+    total=False,
+)
+
 PrometheusInfoTypeDef = TypedDict(
     "PrometheusInfoTypeDef",
     {
         "JmxExporter": JmxExporterInfoTypeDef,
         "NodeExporter": NodeExporterInfoTypeDef,
     },
     total=False,
@@ -1672,14 +1965,23 @@
     {
         "JmxExporter": JmxExporterTypeDef,
         "NodeExporter": NodeExporterTypeDef,
     },
     total=False,
 )
 
+SaslOutputTypeDef = TypedDict(
+    "SaslOutputTypeDef",
+    {
+        "Scram": ScramOutputTypeDef,
+        "Iam": IamOutputTypeDef,
+    },
+    total=False,
+)
+
 SaslTypeDef = TypedDict(
     "SaslTypeDef",
     {
         "Scram": ScramTypeDef,
         "Iam": IamTypeDef,
     },
     total=False,
@@ -1692,23 +1994,40 @@
         "Owner": str,
         "UserIdentity": UserIdentityTypeDef,
         "CreationTime": datetime,
     },
     total=False,
 )
 
+VpcConnectivitySaslOutputTypeDef = TypedDict(
+    "VpcConnectivitySaslOutputTypeDef",
+    {
+        "Scram": VpcConnectivityScramOutputTypeDef,
+        "Iam": VpcConnectivityIamOutputTypeDef,
+    },
+    total=False,
+)
+
 VpcConnectivitySaslTypeDef = TypedDict(
     "VpcConnectivitySaslTypeDef",
     {
         "Scram": VpcConnectivityScramTypeDef,
         "Iam": VpcConnectivityIamTypeDef,
     },
     total=False,
 )
 
+StorageInfoOutputTypeDef = TypedDict(
+    "StorageInfoOutputTypeDef",
+    {
+        "EbsStorageInfo": EBSStorageInfoOutputTypeDef,
+    },
+    total=False,
+)
+
 UpdateBrokerStorageRequestRequestTypeDef = TypedDict(
     "UpdateBrokerStorageRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
         "TargetBrokerEBSVolumeInfo": Sequence[BrokerEBSVolumeInfoTypeDef],
     },
@@ -1718,14 +2037,21 @@
     "StorageInfoTypeDef",
     {
         "EbsStorageInfo": EBSStorageInfoTypeDef,
     },
     total=False,
 )
 
+LoggingInfoOutputTypeDef = TypedDict(
+    "LoggingInfoOutputTypeDef",
+    {
+        "BrokerLogs": BrokerLogsOutputTypeDef,
+    },
+)
+
 LoggingInfoTypeDef = TypedDict(
     "LoggingInfoTypeDef",
     {
         "BrokerLogs": BrokerLogsTypeDef,
     },
 )
 
@@ -1747,46 +2073,80 @@
     {
         "Configurations": List[ConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ServerlessClientAuthenticationOutputTypeDef = TypedDict(
+    "ServerlessClientAuthenticationOutputTypeDef",
+    {
+        "Sasl": ServerlessSaslOutputTypeDef,
+    },
+    total=False,
+)
+
 ServerlessClientAuthenticationTypeDef = TypedDict(
     "ServerlessClientAuthenticationTypeDef",
     {
         "Sasl": ServerlessSaslTypeDef,
     },
     total=False,
 )
 
+OpenMonitoringInfoOutputTypeDef = TypedDict(
+    "OpenMonitoringInfoOutputTypeDef",
+    {
+        "Prometheus": PrometheusInfoOutputTypeDef,
+    },
+)
+
 OpenMonitoringInfoTypeDef = TypedDict(
     "OpenMonitoringInfoTypeDef",
     {
         "Prometheus": PrometheusInfoTypeDef,
     },
 )
 
 OpenMonitoringTypeDef = TypedDict(
     "OpenMonitoringTypeDef",
     {
         "Prometheus": PrometheusTypeDef,
     },
 )
 
+ClientAuthenticationOutputTypeDef = TypedDict(
+    "ClientAuthenticationOutputTypeDef",
+    {
+        "Sasl": SaslOutputTypeDef,
+        "Tls": TlsOutputTypeDef,
+        "Unauthenticated": UnauthenticatedOutputTypeDef,
+    },
+    total=False,
+)
+
 ClientAuthenticationTypeDef = TypedDict(
     "ClientAuthenticationTypeDef",
     {
         "Sasl": SaslTypeDef,
         "Tls": TlsTypeDef,
         "Unauthenticated": UnauthenticatedTypeDef,
     },
     total=False,
 )
 
+VpcConnectivityClientAuthenticationOutputTypeDef = TypedDict(
+    "VpcConnectivityClientAuthenticationOutputTypeDef",
+    {
+        "Sasl": VpcConnectivitySaslOutputTypeDef,
+        "Tls": VpcConnectivityTlsOutputTypeDef,
+    },
+    total=False,
+)
+
 VpcConnectivityClientAuthenticationTypeDef = TypedDict(
     "VpcConnectivityClientAuthenticationTypeDef",
     {
         "Sasl": VpcConnectivitySaslTypeDef,
         "Tls": VpcConnectivityTlsTypeDef,
     },
     total=False,
@@ -1797,51 +2157,51 @@
     {
         "NextToken": str,
         "NodeInfoList": List[NodeInfoTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredServerlessRequestTypeDef = TypedDict(
-    "_RequiredServerlessRequestTypeDef",
+_RequiredServerlessTypeDef = TypedDict(
+    "_RequiredServerlessTypeDef",
     {
-        "VpcConfigs": Sequence[VpcConfigTypeDef],
+        "VpcConfigs": List[VpcConfigOutputTypeDef],
     },
 )
-_OptionalServerlessRequestTypeDef = TypedDict(
-    "_OptionalServerlessRequestTypeDef",
+_OptionalServerlessTypeDef = TypedDict(
+    "_OptionalServerlessTypeDef",
     {
-        "ClientAuthentication": ServerlessClientAuthenticationTypeDef,
+        "ClientAuthentication": ServerlessClientAuthenticationOutputTypeDef,
     },
     total=False,
 )
 
 
-class ServerlessRequestTypeDef(
-    _RequiredServerlessRequestTypeDef, _OptionalServerlessRequestTypeDef
-):
+class ServerlessTypeDef(_RequiredServerlessTypeDef, _OptionalServerlessTypeDef):
     pass
 
 
-_RequiredServerlessTypeDef = TypedDict(
-    "_RequiredServerlessTypeDef",
+_RequiredServerlessRequestTypeDef = TypedDict(
+    "_RequiredServerlessRequestTypeDef",
     {
-        "VpcConfigs": List[VpcConfigTypeDef],
+        "VpcConfigs": Sequence[VpcConfigTypeDef],
     },
 )
-_OptionalServerlessTypeDef = TypedDict(
-    "_OptionalServerlessTypeDef",
+_OptionalServerlessRequestTypeDef = TypedDict(
+    "_OptionalServerlessRequestTypeDef",
     {
         "ClientAuthentication": ServerlessClientAuthenticationTypeDef,
     },
     total=False,
 )
 
 
-class ServerlessTypeDef(_RequiredServerlessTypeDef, _OptionalServerlessTypeDef):
+class ServerlessRequestTypeDef(
+    _RequiredServerlessRequestTypeDef, _OptionalServerlessRequestTypeDef
+):
     pass
 
 
 _RequiredUpdateMonitoringRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMonitoringRequestRequestTypeDef",
     {
         "ClusterArn": str,
@@ -1884,111 +2244,201 @@
 
 class UpdateSecurityRequestRequestTypeDef(
     _RequiredUpdateSecurityRequestRequestTypeDef, _OptionalUpdateSecurityRequestRequestTypeDef
 ):
     pass
 
 
+VpcConnectivityOutputTypeDef = TypedDict(
+    "VpcConnectivityOutputTypeDef",
+    {
+        "ClientAuthentication": VpcConnectivityClientAuthenticationOutputTypeDef,
+    },
+    total=False,
+)
+
 VpcConnectivityTypeDef = TypedDict(
     "VpcConnectivityTypeDef",
     {
         "ClientAuthentication": VpcConnectivityClientAuthenticationTypeDef,
     },
     total=False,
 )
 
+ConnectivityInfoOutputTypeDef = TypedDict(
+    "ConnectivityInfoOutputTypeDef",
+    {
+        "PublicAccess": PublicAccessOutputTypeDef,
+        "VpcConnectivity": VpcConnectivityOutputTypeDef,
+    },
+    total=False,
+)
+
 ConnectivityInfoTypeDef = TypedDict(
     "ConnectivityInfoTypeDef",
     {
         "PublicAccess": PublicAccessTypeDef,
         "VpcConnectivity": VpcConnectivityTypeDef,
     },
     total=False,
 )
 
-_RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
-    "_RequiredBrokerNodeGroupInfoTypeDef",
+_RequiredBrokerNodeGroupInfoOutputTypeDef = TypedDict(
+    "_RequiredBrokerNodeGroupInfoOutputTypeDef",
     {
-        "ClientSubnets": Sequence[str],
+        "ClientSubnets": List[str],
         "InstanceType": str,
     },
 )
-_OptionalBrokerNodeGroupInfoTypeDef = TypedDict(
-    "_OptionalBrokerNodeGroupInfoTypeDef",
+_OptionalBrokerNodeGroupInfoOutputTypeDef = TypedDict(
+    "_OptionalBrokerNodeGroupInfoOutputTypeDef",
     {
         "BrokerAZDistribution": Literal["DEFAULT"],
-        "SecurityGroups": Sequence[str],
-        "StorageInfo": StorageInfoTypeDef,
-        "ConnectivityInfo": ConnectivityInfoTypeDef,
-        "ZoneIds": Sequence[str],
+        "SecurityGroups": List[str],
+        "StorageInfo": StorageInfoOutputTypeDef,
+        "ConnectivityInfo": ConnectivityInfoOutputTypeDef,
+        "ZoneIds": List[str],
     },
     total=False,
 )
 
 
-class BrokerNodeGroupInfoTypeDef(
-    _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
+class BrokerNodeGroupInfoOutputTypeDef(
+    _RequiredBrokerNodeGroupInfoOutputTypeDef, _OptionalBrokerNodeGroupInfoOutputTypeDef
 ):
     pass
 
 
 MutableClusterInfoTypeDef = TypedDict(
     "MutableClusterInfoTypeDef",
     {
-        "BrokerEBSVolumeInfo": List[BrokerEBSVolumeInfoTypeDef],
-        "ConfigurationInfo": ConfigurationInfoTypeDef,
+        "BrokerEBSVolumeInfo": List[BrokerEBSVolumeInfoOutputTypeDef],
+        "ConfigurationInfo": ConfigurationInfoOutputTypeDef,
         "NumberOfBrokerNodes": int,
         "EnhancedMonitoring": EnhancedMonitoringType,
         "OpenMonitoring": OpenMonitoringTypeDef,
         "KafkaVersion": str,
-        "LoggingInfo": LoggingInfoTypeDef,
+        "LoggingInfo": LoggingInfoOutputTypeDef,
         "InstanceType": str,
-        "ClientAuthentication": ClientAuthenticationTypeDef,
-        "EncryptionInfo": EncryptionInfoTypeDef,
-        "ConnectivityInfo": ConnectivityInfoTypeDef,
+        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
+        "EncryptionInfo": EncryptionInfoOutputTypeDef,
+        "ConnectivityInfo": ConnectivityInfoOutputTypeDef,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
+_RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
+    "_RequiredBrokerNodeGroupInfoTypeDef",
+    {
+        "ClientSubnets": Sequence[str],
+        "InstanceType": str,
+    },
+)
+_OptionalBrokerNodeGroupInfoTypeDef = TypedDict(
+    "_OptionalBrokerNodeGroupInfoTypeDef",
+    {
+        "BrokerAZDistribution": Literal["DEFAULT"],
+        "SecurityGroups": Sequence[str],
+        "StorageInfo": StorageInfoTypeDef,
+        "ConnectivityInfo": ConnectivityInfoTypeDef,
+        "ZoneIds": Sequence[str],
+    },
+    total=False,
+)
+
+
+class BrokerNodeGroupInfoTypeDef(
+    _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
+):
+    pass
+
+
 UpdateConnectivityRequestRequestTypeDef = TypedDict(
     "UpdateConnectivityRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "CurrentVersion": str,
     },
 )
 
 ClusterInfoTypeDef = TypedDict(
     "ClusterInfoTypeDef",
     {
         "ActiveOperationArn": str,
-        "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
-        "ClientAuthentication": ClientAuthenticationTypeDef,
+        "BrokerNodeGroupInfo": BrokerNodeGroupInfoOutputTypeDef,
+        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
         "ClusterArn": str,
         "ClusterName": str,
         "CreationTime": datetime,
         "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
         "CurrentVersion": str,
-        "EncryptionInfo": EncryptionInfoTypeDef,
+        "EncryptionInfo": EncryptionInfoOutputTypeDef,
         "EnhancedMonitoring": EnhancedMonitoringType,
         "OpenMonitoring": OpenMonitoringTypeDef,
-        "LoggingInfo": LoggingInfoTypeDef,
+        "LoggingInfo": LoggingInfoOutputTypeDef,
         "NumberOfBrokerNodes": int,
         "State": ClusterStateType,
         "StateInfo": StateInfoTypeDef,
         "Tags": Dict[str, str],
         "ZookeeperConnectString": str,
         "ZookeeperConnectStringTls": str,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
+_RequiredProvisionedTypeDef = TypedDict(
+    "_RequiredProvisionedTypeDef",
+    {
+        "BrokerNodeGroupInfo": BrokerNodeGroupInfoOutputTypeDef,
+        "NumberOfBrokerNodes": int,
+    },
+)
+_OptionalProvisionedTypeDef = TypedDict(
+    "_OptionalProvisionedTypeDef",
+    {
+        "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
+        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
+        "EncryptionInfo": EncryptionInfoOutputTypeDef,
+        "EnhancedMonitoring": EnhancedMonitoringType,
+        "OpenMonitoring": OpenMonitoringInfoOutputTypeDef,
+        "LoggingInfo": LoggingInfoOutputTypeDef,
+        "ZookeeperConnectString": str,
+        "ZookeeperConnectStringTls": str,
+        "StorageMode": StorageModeType,
+    },
+    total=False,
+)
+
+
+class ProvisionedTypeDef(_RequiredProvisionedTypeDef, _OptionalProvisionedTypeDef):
+    pass
+
+
+ClusterOperationInfoTypeDef = TypedDict(
+    "ClusterOperationInfoTypeDef",
+    {
+        "ClientRequestId": str,
+        "ClusterArn": str,
+        "CreationTime": datetime,
+        "EndTime": datetime,
+        "ErrorInfo": ErrorInfoTypeDef,
+        "OperationArn": str,
+        "OperationState": str,
+        "OperationSteps": List[ClusterOperationStepTypeDef],
+        "OperationType": str,
+        "SourceClusterInfo": MutableClusterInfoTypeDef,
+        "TargetClusterInfo": MutableClusterInfoTypeDef,
+        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "ClusterName": str,
         "KafkaVersion": str,
         "NumberOfBrokerNodes": int,
@@ -2041,61 +2491,14 @@
 
 class ProvisionedRequestTypeDef(
     _RequiredProvisionedRequestTypeDef, _OptionalProvisionedRequestTypeDef
 ):
     pass
 
 
-_RequiredProvisionedTypeDef = TypedDict(
-    "_RequiredProvisionedTypeDef",
-    {
-        "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
-        "NumberOfBrokerNodes": int,
-    },
-)
-_OptionalProvisionedTypeDef = TypedDict(
-    "_OptionalProvisionedTypeDef",
-    {
-        "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
-        "ClientAuthentication": ClientAuthenticationTypeDef,
-        "EncryptionInfo": EncryptionInfoTypeDef,
-        "EnhancedMonitoring": EnhancedMonitoringType,
-        "OpenMonitoring": OpenMonitoringInfoTypeDef,
-        "LoggingInfo": LoggingInfoTypeDef,
-        "ZookeeperConnectString": str,
-        "ZookeeperConnectStringTls": str,
-        "StorageMode": StorageModeType,
-    },
-    total=False,
-)
-
-
-class ProvisionedTypeDef(_RequiredProvisionedTypeDef, _OptionalProvisionedTypeDef):
-    pass
-
-
-ClusterOperationInfoTypeDef = TypedDict(
-    "ClusterOperationInfoTypeDef",
-    {
-        "ClientRequestId": str,
-        "ClusterArn": str,
-        "CreationTime": datetime,
-        "EndTime": datetime,
-        "ErrorInfo": ErrorInfoTypeDef,
-        "OperationArn": str,
-        "OperationState": str,
-        "OperationSteps": List[ClusterOperationStepTypeDef],
-        "OperationType": str,
-        "SourceClusterInfo": MutableClusterInfoTypeDef,
-        "TargetClusterInfo": MutableClusterInfoTypeDef,
-        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
-    },
-    total=False,
-)
-
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "ClusterInfo": ClusterInfoTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2105,37 +2508,14 @@
     {
         "ClusterInfoList": List[ClusterInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateClusterV2RequestRequestTypeDef = TypedDict(
-    "_RequiredCreateClusterV2RequestRequestTypeDef",
-    {
-        "ClusterName": str,
-    },
-)
-_OptionalCreateClusterV2RequestRequestTypeDef = TypedDict(
-    "_OptionalCreateClusterV2RequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-        "Provisioned": ProvisionedRequestTypeDef,
-        "Serverless": ServerlessRequestTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateClusterV2RequestRequestTypeDef(
-    _RequiredCreateClusterV2RequestRequestTypeDef, _OptionalCreateClusterV2RequestRequestTypeDef
-):
-    pass
-
-
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "ActiveOperationArn": str,
         "ClusterType": ClusterTypeType,
         "ClusterArn": str,
         "ClusterName": str,
@@ -2163,14 +2543,37 @@
     {
         "ClusterOperationInfoList": List[ClusterOperationInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateClusterV2RequestRequestTypeDef = TypedDict(
+    "_RequiredCreateClusterV2RequestRequestTypeDef",
+    {
+        "ClusterName": str,
+    },
+)
+_OptionalCreateClusterV2RequestRequestTypeDef = TypedDict(
+    "_OptionalCreateClusterV2RequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "Provisioned": ProvisionedRequestTypeDef,
+        "Serverless": ServerlessRequestTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateClusterV2RequestRequestTypeDef(
+    _RequiredCreateClusterV2RequestRequestTypeDef, _OptionalCreateClusterV2RequestRequestTypeDef
+):
+    pass
+
+
 DescribeClusterV2ResponseTypeDef = TypedDict(
     "DescribeClusterV2ResponseTypeDef",
     {
         "ClusterInfo": ClusterTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kafka-1.28.0/mypy_boto3_kafka/type_defs.pyi` & `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -38,28 +38,36 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BatchAssociateScramSecretRequestRequestTypeDef",
     "UnprocessedScramSecretTypeDef",
     "BatchDisassociateScramSecretRequestRequestTypeDef",
+    "ProvisionedThroughputOutputTypeDef",
     "ProvisionedThroughputTypeDef",
+    "CloudWatchLogsOutputTypeDef",
+    "FirehoseOutputTypeDef",
+    "S3OutputTypeDef",
     "CloudWatchLogsTypeDef",
     "FirehoseTypeDef",
     "S3TypeDef",
     "BrokerSoftwareInfoTypeDef",
+    "TlsOutputTypeDef",
+    "UnauthenticatedOutputTypeDef",
     "TlsTypeDef",
     "UnauthenticatedTypeDef",
     "ClientVpcConnectionTypeDef",
     "StateInfoTypeDef",
     "ErrorInfoTypeDef",
     "ClusterOperationStepInfoTypeDef",
     "CompatibleKafkaVersionTypeDef",
+    "ConfigurationInfoOutputTypeDef",
     "ConfigurationInfoTypeDef",
     "ConfigurationRevisionTypeDef",
+    "PublicAccessOutputTypeDef",
     "PublicAccessTypeDef",
     "CreateClusterResponseTypeDef",
     "CreateClusterV2ResponseTypeDef",
     "CreateConfigurationRequestRequestTypeDef",
     "CreateVpcConnectionRequestRequestTypeDef",
     "CreateVpcConnectionResponseTypeDef",
     "DeleteClusterPolicyRequestRequestTypeDef",
@@ -74,22 +82,26 @@
     "DescribeClusterV2RequestRequestTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     "DescribeConfigurationRevisionResponseTypeDef",
     "DescribeVpcConnectionRequestRequestTypeDef",
     "DescribeVpcConnectionResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionAtRestOutputTypeDef",
     "EncryptionAtRestTypeDef",
+    "EncryptionInTransitOutputTypeDef",
     "EncryptionInTransitTypeDef",
     "GetBootstrapBrokersRequestRequestTypeDef",
     "GetBootstrapBrokersResponseTypeDef",
     "GetClusterPolicyRequestRequestTypeDef",
     "GetClusterPolicyResponseTypeDef",
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
+    "IamOutputTypeDef",
     "IamTypeDef",
+    "JmxExporterInfoOutputTypeDef",
     "JmxExporterInfoTypeDef",
     "JmxExporterTypeDef",
     "KafkaVersionTypeDef",
     "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
     "ListClientVpcConnectionsRequestRequestTypeDef",
     "ListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
     "ListClusterOperationsRequestRequestTypeDef",
@@ -109,26 +121,29 @@
     "ListScramSecretsRequestRequestTypeDef",
     "ListScramSecretsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
     "ListVpcConnectionsRequestRequestTypeDef",
     "VpcConnectionTypeDef",
+    "NodeExporterInfoOutputTypeDef",
     "NodeExporterInfoTypeDef",
     "NodeExporterTypeDef",
     "ZookeeperNodeInfoTypeDef",
     "PaginatorConfigTypeDef",
     "PutClusterPolicyRequestRequestTypeDef",
     "PutClusterPolicyResponseTypeDef",
     "RebootBrokerRequestRequestTypeDef",
     "RebootBrokerResponseTypeDef",
     "RejectClientVpcConnectionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "ScramOutputTypeDef",
     "ScramTypeDef",
     "VpcConfigTypeDef",
+    "VpcConfigOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrokerCountRequestRequestTypeDef",
     "UpdateBrokerCountResponseTypeDef",
     "UpdateBrokerStorageResponseTypeDef",
     "UpdateBrokerTypeRequestRequestTypeDef",
     "UpdateBrokerTypeResponseTypeDef",
@@ -136,74 +151,94 @@
     "UpdateClusterKafkaVersionResponseTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "UpdateConnectivityResponseTypeDef",
     "UpdateMonitoringResponseTypeDef",
     "UpdateSecurityResponseTypeDef",
     "UpdateStorageResponseTypeDef",
     "UserIdentityTypeDef",
+    "VpcConnectivityTlsOutputTypeDef",
     "VpcConnectivityTlsTypeDef",
+    "VpcConnectivityIamOutputTypeDef",
     "VpcConnectivityIamTypeDef",
+    "VpcConnectivityScramOutputTypeDef",
     "VpcConnectivityScramTypeDef",
     "BatchAssociateScramSecretResponseTypeDef",
     "BatchDisassociateScramSecretResponseTypeDef",
+    "BrokerEBSVolumeInfoOutputTypeDef",
+    "EBSStorageInfoOutputTypeDef",
     "BrokerEBSVolumeInfoTypeDef",
     "EBSStorageInfoTypeDef",
     "UpdateStorageRequestRequestTypeDef",
+    "BrokerLogsOutputTypeDef",
     "BrokerLogsTypeDef",
     "BrokerNodeInfoTypeDef",
     "ListClientVpcConnectionsResponseTypeDef",
     "ClusterOperationStepTypeDef",
     "GetCompatibleKafkaVersionsResponseTypeDef",
     "UpdateClusterConfigurationRequestRequestTypeDef",
     "UpdateClusterKafkaVersionRequestRequestTypeDef",
     "ConfigurationTypeDef",
     "CreateConfigurationResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
     "UpdateConfigurationResponseTypeDef",
+    "EncryptionInfoOutputTypeDef",
     "EncryptionInfoTypeDef",
+    "ServerlessSaslOutputTypeDef",
     "ServerlessSaslTypeDef",
     "ListKafkaVersionsResponseTypeDef",
     "ListVpcConnectionsResponseTypeDef",
+    "PrometheusInfoOutputTypeDef",
     "PrometheusInfoTypeDef",
     "PrometheusTypeDef",
+    "SaslOutputTypeDef",
     "SaslTypeDef",
     "VpcConnectionInfoTypeDef",
+    "VpcConnectivitySaslOutputTypeDef",
     "VpcConnectivitySaslTypeDef",
+    "StorageInfoOutputTypeDef",
     "UpdateBrokerStorageRequestRequestTypeDef",
     "StorageInfoTypeDef",
+    "LoggingInfoOutputTypeDef",
     "LoggingInfoTypeDef",
     "NodeInfoTypeDef",
     "ListConfigurationsResponseTypeDef",
+    "ServerlessClientAuthenticationOutputTypeDef",
     "ServerlessClientAuthenticationTypeDef",
+    "OpenMonitoringInfoOutputTypeDef",
     "OpenMonitoringInfoTypeDef",
     "OpenMonitoringTypeDef",
+    "ClientAuthenticationOutputTypeDef",
     "ClientAuthenticationTypeDef",
+    "VpcConnectivityClientAuthenticationOutputTypeDef",
     "VpcConnectivityClientAuthenticationTypeDef",
     "ListNodesResponseTypeDef",
-    "ServerlessRequestTypeDef",
     "ServerlessTypeDef",
+    "ServerlessRequestTypeDef",
     "UpdateMonitoringRequestRequestTypeDef",
     "UpdateSecurityRequestRequestTypeDef",
+    "VpcConnectivityOutputTypeDef",
     "VpcConnectivityTypeDef",
+    "ConnectivityInfoOutputTypeDef",
     "ConnectivityInfoTypeDef",
-    "BrokerNodeGroupInfoTypeDef",
+    "BrokerNodeGroupInfoOutputTypeDef",
     "MutableClusterInfoTypeDef",
+    "BrokerNodeGroupInfoTypeDef",
     "UpdateConnectivityRequestRequestTypeDef",
     "ClusterInfoTypeDef",
-    "CreateClusterRequestRequestTypeDef",
-    "ProvisionedRequestTypeDef",
     "ProvisionedTypeDef",
     "ClusterOperationInfoTypeDef",
+    "CreateClusterRequestRequestTypeDef",
+    "ProvisionedRequestTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
-    "CreateClusterV2RequestRequestTypeDef",
     "ClusterTypeDef",
     "DescribeClusterOperationResponseTypeDef",
     "ListClusterOperationsResponseTypeDef",
+    "CreateClusterV2RequestRequestTypeDef",
     "DescribeClusterV2ResponseTypeDef",
     "ListClustersV2ResponseTypeDef",
 )
 
 BatchAssociateScramSecretRequestRequestTypeDef = TypedDict(
     "BatchAssociateScramSecretRequestRequestTypeDef",
     {
@@ -226,23 +261,86 @@
     "BatchDisassociateScramSecretRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "SecretArnList": Sequence[str],
     },
 )
 
+ProvisionedThroughputOutputTypeDef = TypedDict(
+    "ProvisionedThroughputOutputTypeDef",
+    {
+        "Enabled": bool,
+        "VolumeThroughput": int,
+    },
+    total=False,
+)
+
 ProvisionedThroughputTypeDef = TypedDict(
     "ProvisionedThroughputTypeDef",
     {
         "Enabled": bool,
         "VolumeThroughput": int,
     },
     total=False,
 )
 
+_RequiredCloudWatchLogsOutputTypeDef = TypedDict(
+    "_RequiredCloudWatchLogsOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalCloudWatchLogsOutputTypeDef = TypedDict(
+    "_OptionalCloudWatchLogsOutputTypeDef",
+    {
+        "LogGroup": str,
+    },
+    total=False,
+)
+
+class CloudWatchLogsOutputTypeDef(
+    _RequiredCloudWatchLogsOutputTypeDef, _OptionalCloudWatchLogsOutputTypeDef
+):
+    pass
+
+_RequiredFirehoseOutputTypeDef = TypedDict(
+    "_RequiredFirehoseOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalFirehoseOutputTypeDef = TypedDict(
+    "_OptionalFirehoseOutputTypeDef",
+    {
+        "DeliveryStream": str,
+    },
+    total=False,
+)
+
+class FirehoseOutputTypeDef(_RequiredFirehoseOutputTypeDef, _OptionalFirehoseOutputTypeDef):
+    pass
+
+_RequiredS3OutputTypeDef = TypedDict(
+    "_RequiredS3OutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalS3OutputTypeDef = TypedDict(
+    "_OptionalS3OutputTypeDef",
+    {
+        "Bucket": str,
+        "Prefix": str,
+    },
+    total=False,
+)
+
+class S3OutputTypeDef(_RequiredS3OutputTypeDef, _OptionalS3OutputTypeDef):
+    pass
+
 _RequiredCloudWatchLogsTypeDef = TypedDict(
     "_RequiredCloudWatchLogsTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalCloudWatchLogsTypeDef = TypedDict(
@@ -297,14 +395,31 @@
         "ConfigurationArn": str,
         "ConfigurationRevision": int,
         "KafkaVersion": str,
     },
     total=False,
 )
 
+TlsOutputTypeDef = TypedDict(
+    "TlsOutputTypeDef",
+    {
+        "CertificateAuthorityArnList": List[str],
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+UnauthenticatedOutputTypeDef = TypedDict(
+    "UnauthenticatedOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 TlsTypeDef = TypedDict(
     "TlsTypeDef",
     {
         "CertificateAuthorityArnList": Sequence[str],
         "Enabled": bool,
     },
     total=False,
@@ -371,14 +486,22 @@
     {
         "SourceVersion": str,
         "TargetVersions": List[str],
     },
     total=False,
 )
 
+ConfigurationInfoOutputTypeDef = TypedDict(
+    "ConfigurationInfoOutputTypeDef",
+    {
+        "Arn": str,
+        "Revision": int,
+    },
+)
+
 ConfigurationInfoTypeDef = TypedDict(
     "ConfigurationInfoTypeDef",
     {
         "Arn": str,
         "Revision": int,
     },
 )
@@ -399,14 +522,22 @@
 )
 
 class ConfigurationRevisionTypeDef(
     _RequiredConfigurationRevisionTypeDef, _OptionalConfigurationRevisionTypeDef
 ):
     pass
 
+PublicAccessOutputTypeDef = TypedDict(
+    "PublicAccessOutputTypeDef",
+    {
+        "Type": str,
+    },
+    total=False,
+)
+
 PublicAccessTypeDef = TypedDict(
     "PublicAccessTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
@@ -634,21 +765,37 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionAtRestOutputTypeDef = TypedDict(
+    "EncryptionAtRestOutputTypeDef",
+    {
+        "DataVolumeKMSKeyId": str,
+    },
+)
+
 EncryptionAtRestTypeDef = TypedDict(
     "EncryptionAtRestTypeDef",
     {
         "DataVolumeKMSKeyId": str,
     },
 )
 
+EncryptionInTransitOutputTypeDef = TypedDict(
+    "EncryptionInTransitOutputTypeDef",
+    {
+        "ClientBroker": ClientBrokerType,
+        "InCluster": bool,
+    },
+    total=False,
+)
+
 EncryptionInTransitTypeDef = TypedDict(
     "EncryptionInTransitTypeDef",
     {
         "ClientBroker": ClientBrokerType,
         "InCluster": bool,
     },
     total=False,
@@ -698,22 +845,37 @@
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
     total=False,
 )
 
+IamOutputTypeDef = TypedDict(
+    "IamOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 IamTypeDef = TypedDict(
     "IamTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+JmxExporterInfoOutputTypeDef = TypedDict(
+    "JmxExporterInfoOutputTypeDef",
+    {
+        "EnabledInBroker": bool,
+    },
+)
+
 JmxExporterInfoTypeDef = TypedDict(
     "JmxExporterInfoTypeDef",
     {
         "EnabledInBroker": bool,
     },
 )
 
@@ -1068,14 +1230,21 @@
     },
     total=False,
 )
 
 class VpcConnectionTypeDef(_RequiredVpcConnectionTypeDef, _OptionalVpcConnectionTypeDef):
     pass
 
+NodeExporterInfoOutputTypeDef = TypedDict(
+    "NodeExporterInfoOutputTypeDef",
+    {
+        "EnabledInBroker": bool,
+    },
+)
+
 NodeExporterInfoTypeDef = TypedDict(
     "NodeExporterInfoTypeDef",
     {
         "EnabledInBroker": bool,
     },
 )
 
@@ -1168,14 +1337,22 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+ScramOutputTypeDef = TypedDict(
+    "ScramOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 ScramTypeDef = TypedDict(
     "ScramTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -1193,14 +1370,31 @@
     },
     total=False,
 )
 
 class VpcConfigTypeDef(_RequiredVpcConfigTypeDef, _OptionalVpcConfigTypeDef):
     pass
 
+_RequiredVpcConfigOutputTypeDef = TypedDict(
+    "_RequiredVpcConfigOutputTypeDef",
+    {
+        "SubnetIds": List[str],
+    },
+)
+_OptionalVpcConfigOutputTypeDef = TypedDict(
+    "_OptionalVpcConfigOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+    },
+    total=False,
+)
+
+class VpcConfigOutputTypeDef(_RequiredVpcConfigOutputTypeDef, _OptionalVpcConfigOutputTypeDef):
+    pass
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1338,30 +1532,54 @@
     {
         "Type": UserIdentityTypeType,
         "PrincipalId": str,
     },
     total=False,
 )
 
+VpcConnectivityTlsOutputTypeDef = TypedDict(
+    "VpcConnectivityTlsOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 VpcConnectivityTlsTypeDef = TypedDict(
     "VpcConnectivityTlsTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+VpcConnectivityIamOutputTypeDef = TypedDict(
+    "VpcConnectivityIamOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 VpcConnectivityIamTypeDef = TypedDict(
     "VpcConnectivityIamTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+VpcConnectivityScramOutputTypeDef = TypedDict(
+    "VpcConnectivityScramOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
 VpcConnectivityScramTypeDef = TypedDict(
     "VpcConnectivityScramTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -1380,14 +1598,43 @@
     {
         "ClusterArn": str,
         "UnprocessedScramSecrets": List[UnprocessedScramSecretTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredBrokerEBSVolumeInfoOutputTypeDef = TypedDict(
+    "_RequiredBrokerEBSVolumeInfoOutputTypeDef",
+    {
+        "KafkaBrokerNodeId": str,
+    },
+)
+_OptionalBrokerEBSVolumeInfoOutputTypeDef = TypedDict(
+    "_OptionalBrokerEBSVolumeInfoOutputTypeDef",
+    {
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "VolumeSizeGB": int,
+    },
+    total=False,
+)
+
+class BrokerEBSVolumeInfoOutputTypeDef(
+    _RequiredBrokerEBSVolumeInfoOutputTypeDef, _OptionalBrokerEBSVolumeInfoOutputTypeDef
+):
+    pass
+
+EBSStorageInfoOutputTypeDef = TypedDict(
+    "EBSStorageInfoOutputTypeDef",
+    {
+        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "VolumeSize": int,
+    },
+    total=False,
+)
+
 _RequiredBrokerEBSVolumeInfoTypeDef = TypedDict(
     "_RequiredBrokerEBSVolumeInfoTypeDef",
     {
         "KafkaBrokerNodeId": str,
     },
 )
 _OptionalBrokerEBSVolumeInfoTypeDef = TypedDict(
@@ -1431,14 +1678,24 @@
 )
 
 class UpdateStorageRequestRequestTypeDef(
     _RequiredUpdateStorageRequestRequestTypeDef, _OptionalUpdateStorageRequestRequestTypeDef
 ):
     pass
 
+BrokerLogsOutputTypeDef = TypedDict(
+    "BrokerLogsOutputTypeDef",
+    {
+        "CloudWatchLogs": CloudWatchLogsOutputTypeDef,
+        "Firehose": FirehoseOutputTypeDef,
+        "S3": S3OutputTypeDef,
+    },
+    total=False,
+)
+
 BrokerLogsTypeDef = TypedDict(
     "BrokerLogsTypeDef",
     {
         "CloudWatchLogs": CloudWatchLogsTypeDef,
         "Firehose": FirehoseTypeDef,
         "S3": S3TypeDef,
     },
@@ -1568,23 +1825,40 @@
     {
         "Arn": str,
         "LatestRevision": ConfigurationRevisionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionInfoOutputTypeDef = TypedDict(
+    "EncryptionInfoOutputTypeDef",
+    {
+        "EncryptionAtRest": EncryptionAtRestOutputTypeDef,
+        "EncryptionInTransit": EncryptionInTransitOutputTypeDef,
+    },
+    total=False,
+)
+
 EncryptionInfoTypeDef = TypedDict(
     "EncryptionInfoTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "EncryptionInTransit": EncryptionInTransitTypeDef,
     },
     total=False,
 )
 
+ServerlessSaslOutputTypeDef = TypedDict(
+    "ServerlessSaslOutputTypeDef",
+    {
+        "Iam": IamOutputTypeDef,
+    },
+    total=False,
+)
+
 ServerlessSaslTypeDef = TypedDict(
     "ServerlessSaslTypeDef",
     {
         "Iam": IamTypeDef,
     },
     total=False,
 )
@@ -1603,14 +1877,23 @@
     {
         "VpcConnections": List[VpcConnectionTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PrometheusInfoOutputTypeDef = TypedDict(
+    "PrometheusInfoOutputTypeDef",
+    {
+        "JmxExporter": JmxExporterInfoOutputTypeDef,
+        "NodeExporter": NodeExporterInfoOutputTypeDef,
+    },
+    total=False,
+)
+
 PrometheusInfoTypeDef = TypedDict(
     "PrometheusInfoTypeDef",
     {
         "JmxExporter": JmxExporterInfoTypeDef,
         "NodeExporter": NodeExporterInfoTypeDef,
     },
     total=False,
@@ -1621,14 +1904,23 @@
     {
         "JmxExporter": JmxExporterTypeDef,
         "NodeExporter": NodeExporterTypeDef,
     },
     total=False,
 )
 
+SaslOutputTypeDef = TypedDict(
+    "SaslOutputTypeDef",
+    {
+        "Scram": ScramOutputTypeDef,
+        "Iam": IamOutputTypeDef,
+    },
+    total=False,
+)
+
 SaslTypeDef = TypedDict(
     "SaslTypeDef",
     {
         "Scram": ScramTypeDef,
         "Iam": IamTypeDef,
     },
     total=False,
@@ -1641,23 +1933,40 @@
         "Owner": str,
         "UserIdentity": UserIdentityTypeDef,
         "CreationTime": datetime,
     },
     total=False,
 )
 
+VpcConnectivitySaslOutputTypeDef = TypedDict(
+    "VpcConnectivitySaslOutputTypeDef",
+    {
+        "Scram": VpcConnectivityScramOutputTypeDef,
+        "Iam": VpcConnectivityIamOutputTypeDef,
+    },
+    total=False,
+)
+
 VpcConnectivitySaslTypeDef = TypedDict(
     "VpcConnectivitySaslTypeDef",
     {
         "Scram": VpcConnectivityScramTypeDef,
         "Iam": VpcConnectivityIamTypeDef,
     },
     total=False,
 )
 
+StorageInfoOutputTypeDef = TypedDict(
+    "StorageInfoOutputTypeDef",
+    {
+        "EbsStorageInfo": EBSStorageInfoOutputTypeDef,
+    },
+    total=False,
+)
+
 UpdateBrokerStorageRequestRequestTypeDef = TypedDict(
     "UpdateBrokerStorageRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
         "TargetBrokerEBSVolumeInfo": Sequence[BrokerEBSVolumeInfoTypeDef],
     },
@@ -1667,14 +1976,21 @@
     "StorageInfoTypeDef",
     {
         "EbsStorageInfo": EBSStorageInfoTypeDef,
     },
     total=False,
 )
 
+LoggingInfoOutputTypeDef = TypedDict(
+    "LoggingInfoOutputTypeDef",
+    {
+        "BrokerLogs": BrokerLogsOutputTypeDef,
+    },
+)
+
 LoggingInfoTypeDef = TypedDict(
     "LoggingInfoTypeDef",
     {
         "BrokerLogs": BrokerLogsTypeDef,
     },
 )
 
@@ -1696,46 +2012,80 @@
     {
         "Configurations": List[ConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ServerlessClientAuthenticationOutputTypeDef = TypedDict(
+    "ServerlessClientAuthenticationOutputTypeDef",
+    {
+        "Sasl": ServerlessSaslOutputTypeDef,
+    },
+    total=False,
+)
+
 ServerlessClientAuthenticationTypeDef = TypedDict(
     "ServerlessClientAuthenticationTypeDef",
     {
         "Sasl": ServerlessSaslTypeDef,
     },
     total=False,
 )
 
+OpenMonitoringInfoOutputTypeDef = TypedDict(
+    "OpenMonitoringInfoOutputTypeDef",
+    {
+        "Prometheus": PrometheusInfoOutputTypeDef,
+    },
+)
+
 OpenMonitoringInfoTypeDef = TypedDict(
     "OpenMonitoringInfoTypeDef",
     {
         "Prometheus": PrometheusInfoTypeDef,
     },
 )
 
 OpenMonitoringTypeDef = TypedDict(
     "OpenMonitoringTypeDef",
     {
         "Prometheus": PrometheusTypeDef,
     },
 )
 
+ClientAuthenticationOutputTypeDef = TypedDict(
+    "ClientAuthenticationOutputTypeDef",
+    {
+        "Sasl": SaslOutputTypeDef,
+        "Tls": TlsOutputTypeDef,
+        "Unauthenticated": UnauthenticatedOutputTypeDef,
+    },
+    total=False,
+)
+
 ClientAuthenticationTypeDef = TypedDict(
     "ClientAuthenticationTypeDef",
     {
         "Sasl": SaslTypeDef,
         "Tls": TlsTypeDef,
         "Unauthenticated": UnauthenticatedTypeDef,
     },
     total=False,
 )
 
+VpcConnectivityClientAuthenticationOutputTypeDef = TypedDict(
+    "VpcConnectivityClientAuthenticationOutputTypeDef",
+    {
+        "Sasl": VpcConnectivitySaslOutputTypeDef,
+        "Tls": VpcConnectivityTlsOutputTypeDef,
+    },
+    total=False,
+)
+
 VpcConnectivityClientAuthenticationTypeDef = TypedDict(
     "VpcConnectivityClientAuthenticationTypeDef",
     {
         "Sasl": VpcConnectivitySaslTypeDef,
         "Tls": VpcConnectivityTlsTypeDef,
     },
     total=False,
@@ -1746,48 +2096,48 @@
     {
         "NextToken": str,
         "NodeInfoList": List[NodeInfoTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredServerlessRequestTypeDef = TypedDict(
-    "_RequiredServerlessRequestTypeDef",
+_RequiredServerlessTypeDef = TypedDict(
+    "_RequiredServerlessTypeDef",
     {
-        "VpcConfigs": Sequence[VpcConfigTypeDef],
+        "VpcConfigs": List[VpcConfigOutputTypeDef],
     },
 )
-_OptionalServerlessRequestTypeDef = TypedDict(
-    "_OptionalServerlessRequestTypeDef",
+_OptionalServerlessTypeDef = TypedDict(
+    "_OptionalServerlessTypeDef",
     {
-        "ClientAuthentication": ServerlessClientAuthenticationTypeDef,
+        "ClientAuthentication": ServerlessClientAuthenticationOutputTypeDef,
     },
     total=False,
 )
 
-class ServerlessRequestTypeDef(
-    _RequiredServerlessRequestTypeDef, _OptionalServerlessRequestTypeDef
-):
+class ServerlessTypeDef(_RequiredServerlessTypeDef, _OptionalServerlessTypeDef):
     pass
 
-_RequiredServerlessTypeDef = TypedDict(
-    "_RequiredServerlessTypeDef",
+_RequiredServerlessRequestTypeDef = TypedDict(
+    "_RequiredServerlessRequestTypeDef",
     {
-        "VpcConfigs": List[VpcConfigTypeDef],
+        "VpcConfigs": Sequence[VpcConfigTypeDef],
     },
 )
-_OptionalServerlessTypeDef = TypedDict(
-    "_OptionalServerlessTypeDef",
+_OptionalServerlessRequestTypeDef = TypedDict(
+    "_OptionalServerlessRequestTypeDef",
     {
         "ClientAuthentication": ServerlessClientAuthenticationTypeDef,
     },
     total=False,
 )
 
-class ServerlessTypeDef(_RequiredServerlessTypeDef, _OptionalServerlessTypeDef):
+class ServerlessRequestTypeDef(
+    _RequiredServerlessRequestTypeDef, _OptionalServerlessRequestTypeDef
+):
     pass
 
 _RequiredUpdateMonitoringRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMonitoringRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
@@ -1825,109 +2175,195 @@
 )
 
 class UpdateSecurityRequestRequestTypeDef(
     _RequiredUpdateSecurityRequestRequestTypeDef, _OptionalUpdateSecurityRequestRequestTypeDef
 ):
     pass
 
+VpcConnectivityOutputTypeDef = TypedDict(
+    "VpcConnectivityOutputTypeDef",
+    {
+        "ClientAuthentication": VpcConnectivityClientAuthenticationOutputTypeDef,
+    },
+    total=False,
+)
+
 VpcConnectivityTypeDef = TypedDict(
     "VpcConnectivityTypeDef",
     {
         "ClientAuthentication": VpcConnectivityClientAuthenticationTypeDef,
     },
     total=False,
 )
 
+ConnectivityInfoOutputTypeDef = TypedDict(
+    "ConnectivityInfoOutputTypeDef",
+    {
+        "PublicAccess": PublicAccessOutputTypeDef,
+        "VpcConnectivity": VpcConnectivityOutputTypeDef,
+    },
+    total=False,
+)
+
 ConnectivityInfoTypeDef = TypedDict(
     "ConnectivityInfoTypeDef",
     {
         "PublicAccess": PublicAccessTypeDef,
         "VpcConnectivity": VpcConnectivityTypeDef,
     },
     total=False,
 )
 
-_RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
-    "_RequiredBrokerNodeGroupInfoTypeDef",
+_RequiredBrokerNodeGroupInfoOutputTypeDef = TypedDict(
+    "_RequiredBrokerNodeGroupInfoOutputTypeDef",
     {
-        "ClientSubnets": Sequence[str],
+        "ClientSubnets": List[str],
         "InstanceType": str,
     },
 )
-_OptionalBrokerNodeGroupInfoTypeDef = TypedDict(
-    "_OptionalBrokerNodeGroupInfoTypeDef",
+_OptionalBrokerNodeGroupInfoOutputTypeDef = TypedDict(
+    "_OptionalBrokerNodeGroupInfoOutputTypeDef",
     {
         "BrokerAZDistribution": Literal["DEFAULT"],
-        "SecurityGroups": Sequence[str],
-        "StorageInfo": StorageInfoTypeDef,
-        "ConnectivityInfo": ConnectivityInfoTypeDef,
-        "ZoneIds": Sequence[str],
+        "SecurityGroups": List[str],
+        "StorageInfo": StorageInfoOutputTypeDef,
+        "ConnectivityInfo": ConnectivityInfoOutputTypeDef,
+        "ZoneIds": List[str],
     },
     total=False,
 )
 
-class BrokerNodeGroupInfoTypeDef(
-    _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
+class BrokerNodeGroupInfoOutputTypeDef(
+    _RequiredBrokerNodeGroupInfoOutputTypeDef, _OptionalBrokerNodeGroupInfoOutputTypeDef
 ):
     pass
 
 MutableClusterInfoTypeDef = TypedDict(
     "MutableClusterInfoTypeDef",
     {
-        "BrokerEBSVolumeInfo": List[BrokerEBSVolumeInfoTypeDef],
-        "ConfigurationInfo": ConfigurationInfoTypeDef,
+        "BrokerEBSVolumeInfo": List[BrokerEBSVolumeInfoOutputTypeDef],
+        "ConfigurationInfo": ConfigurationInfoOutputTypeDef,
         "NumberOfBrokerNodes": int,
         "EnhancedMonitoring": EnhancedMonitoringType,
         "OpenMonitoring": OpenMonitoringTypeDef,
         "KafkaVersion": str,
-        "LoggingInfo": LoggingInfoTypeDef,
+        "LoggingInfo": LoggingInfoOutputTypeDef,
         "InstanceType": str,
-        "ClientAuthentication": ClientAuthenticationTypeDef,
-        "EncryptionInfo": EncryptionInfoTypeDef,
-        "ConnectivityInfo": ConnectivityInfoTypeDef,
+        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
+        "EncryptionInfo": EncryptionInfoOutputTypeDef,
+        "ConnectivityInfo": ConnectivityInfoOutputTypeDef,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
+_RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
+    "_RequiredBrokerNodeGroupInfoTypeDef",
+    {
+        "ClientSubnets": Sequence[str],
+        "InstanceType": str,
+    },
+)
+_OptionalBrokerNodeGroupInfoTypeDef = TypedDict(
+    "_OptionalBrokerNodeGroupInfoTypeDef",
+    {
+        "BrokerAZDistribution": Literal["DEFAULT"],
+        "SecurityGroups": Sequence[str],
+        "StorageInfo": StorageInfoTypeDef,
+        "ConnectivityInfo": ConnectivityInfoTypeDef,
+        "ZoneIds": Sequence[str],
+    },
+    total=False,
+)
+
+class BrokerNodeGroupInfoTypeDef(
+    _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
+):
+    pass
+
 UpdateConnectivityRequestRequestTypeDef = TypedDict(
     "UpdateConnectivityRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "CurrentVersion": str,
     },
 )
 
 ClusterInfoTypeDef = TypedDict(
     "ClusterInfoTypeDef",
     {
         "ActiveOperationArn": str,
-        "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
-        "ClientAuthentication": ClientAuthenticationTypeDef,
+        "BrokerNodeGroupInfo": BrokerNodeGroupInfoOutputTypeDef,
+        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
         "ClusterArn": str,
         "ClusterName": str,
         "CreationTime": datetime,
         "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
         "CurrentVersion": str,
-        "EncryptionInfo": EncryptionInfoTypeDef,
+        "EncryptionInfo": EncryptionInfoOutputTypeDef,
         "EnhancedMonitoring": EnhancedMonitoringType,
         "OpenMonitoring": OpenMonitoringTypeDef,
-        "LoggingInfo": LoggingInfoTypeDef,
+        "LoggingInfo": LoggingInfoOutputTypeDef,
         "NumberOfBrokerNodes": int,
         "State": ClusterStateType,
         "StateInfo": StateInfoTypeDef,
         "Tags": Dict[str, str],
         "ZookeeperConnectString": str,
         "ZookeeperConnectStringTls": str,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
+_RequiredProvisionedTypeDef = TypedDict(
+    "_RequiredProvisionedTypeDef",
+    {
+        "BrokerNodeGroupInfo": BrokerNodeGroupInfoOutputTypeDef,
+        "NumberOfBrokerNodes": int,
+    },
+)
+_OptionalProvisionedTypeDef = TypedDict(
+    "_OptionalProvisionedTypeDef",
+    {
+        "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
+        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
+        "EncryptionInfo": EncryptionInfoOutputTypeDef,
+        "EnhancedMonitoring": EnhancedMonitoringType,
+        "OpenMonitoring": OpenMonitoringInfoOutputTypeDef,
+        "LoggingInfo": LoggingInfoOutputTypeDef,
+        "ZookeeperConnectString": str,
+        "ZookeeperConnectStringTls": str,
+        "StorageMode": StorageModeType,
+    },
+    total=False,
+)
+
+class ProvisionedTypeDef(_RequiredProvisionedTypeDef, _OptionalProvisionedTypeDef):
+    pass
+
+ClusterOperationInfoTypeDef = TypedDict(
+    "ClusterOperationInfoTypeDef",
+    {
+        "ClientRequestId": str,
+        "ClusterArn": str,
+        "CreationTime": datetime,
+        "EndTime": datetime,
+        "ErrorInfo": ErrorInfoTypeDef,
+        "OperationArn": str,
+        "OperationState": str,
+        "OperationSteps": List[ClusterOperationStepTypeDef],
+        "OperationType": str,
+        "SourceClusterInfo": MutableClusterInfoTypeDef,
+        "TargetClusterInfo": MutableClusterInfoTypeDef,
+        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "ClusterName": str,
         "KafkaVersion": str,
         "NumberOfBrokerNodes": int,
@@ -1976,59 +2412,14 @@
 )
 
 class ProvisionedRequestTypeDef(
     _RequiredProvisionedRequestTypeDef, _OptionalProvisionedRequestTypeDef
 ):
     pass
 
-_RequiredProvisionedTypeDef = TypedDict(
-    "_RequiredProvisionedTypeDef",
-    {
-        "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
-        "NumberOfBrokerNodes": int,
-    },
-)
-_OptionalProvisionedTypeDef = TypedDict(
-    "_OptionalProvisionedTypeDef",
-    {
-        "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
-        "ClientAuthentication": ClientAuthenticationTypeDef,
-        "EncryptionInfo": EncryptionInfoTypeDef,
-        "EnhancedMonitoring": EnhancedMonitoringType,
-        "OpenMonitoring": OpenMonitoringInfoTypeDef,
-        "LoggingInfo": LoggingInfoTypeDef,
-        "ZookeeperConnectString": str,
-        "ZookeeperConnectStringTls": str,
-        "StorageMode": StorageModeType,
-    },
-    total=False,
-)
-
-class ProvisionedTypeDef(_RequiredProvisionedTypeDef, _OptionalProvisionedTypeDef):
-    pass
-
-ClusterOperationInfoTypeDef = TypedDict(
-    "ClusterOperationInfoTypeDef",
-    {
-        "ClientRequestId": str,
-        "ClusterArn": str,
-        "CreationTime": datetime,
-        "EndTime": datetime,
-        "ErrorInfo": ErrorInfoTypeDef,
-        "OperationArn": str,
-        "OperationState": str,
-        "OperationSteps": List[ClusterOperationStepTypeDef],
-        "OperationType": str,
-        "SourceClusterInfo": MutableClusterInfoTypeDef,
-        "TargetClusterInfo": MutableClusterInfoTypeDef,
-        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
-    },
-    total=False,
-)
-
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "ClusterInfo": ClusterInfoTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2038,35 +2429,14 @@
     {
         "ClusterInfoList": List[ClusterInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateClusterV2RequestRequestTypeDef = TypedDict(
-    "_RequiredCreateClusterV2RequestRequestTypeDef",
-    {
-        "ClusterName": str,
-    },
-)
-_OptionalCreateClusterV2RequestRequestTypeDef = TypedDict(
-    "_OptionalCreateClusterV2RequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-        "Provisioned": ProvisionedRequestTypeDef,
-        "Serverless": ServerlessRequestTypeDef,
-    },
-    total=False,
-)
-
-class CreateClusterV2RequestRequestTypeDef(
-    _RequiredCreateClusterV2RequestRequestTypeDef, _OptionalCreateClusterV2RequestRequestTypeDef
-):
-    pass
-
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "ActiveOperationArn": str,
         "ClusterType": ClusterTypeType,
         "ClusterArn": str,
         "ClusterName": str,
@@ -2094,14 +2464,35 @@
     {
         "ClusterOperationInfoList": List[ClusterOperationInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateClusterV2RequestRequestTypeDef = TypedDict(
+    "_RequiredCreateClusterV2RequestRequestTypeDef",
+    {
+        "ClusterName": str,
+    },
+)
+_OptionalCreateClusterV2RequestRequestTypeDef = TypedDict(
+    "_OptionalCreateClusterV2RequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "Provisioned": ProvisionedRequestTypeDef,
+        "Serverless": ServerlessRequestTypeDef,
+    },
+    total=False,
+)
+
+class CreateClusterV2RequestRequestTypeDef(
+    _RequiredCreateClusterV2RequestRequestTypeDef, _OptionalCreateClusterV2RequestRequestTypeDef
+):
+    pass
+
 DescribeClusterV2ResponseTypeDef = TypedDict(
     "DescribeClusterV2ResponseTypeDef",
     {
         "ClusterInfo": ClusterTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kafka-1.28.0/mypy_boto3_kafka.egg-info/PKG-INFO` & `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kafka
-Version: 1.28.0
-Summary: Type annotations for boto3.Kafka 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Kafka 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-kafka"></a>
 
 # mypy-boto3-kafka
 
 [![PyPI - mypy-boto3-kafka](https://img.shields.io/pypi/v/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kafka?color=blue)](https://pypistats.org/packages/mypy-boto3-kafka)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kafka)](https://pepy.tech/project/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
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
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
 
@@ -373,28 +373,36 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kafka.type_defs import (
     BatchAssociateScramSecretRequestRequestTypeDef,
     UnprocessedScramSecretTypeDef,
     BatchDisassociateScramSecretRequestRequestTypeDef,
+    ProvisionedThroughputOutputTypeDef,
     ProvisionedThroughputTypeDef,
+    CloudWatchLogsOutputTypeDef,
+    FirehoseOutputTypeDef,
+    S3OutputTypeDef,
     CloudWatchLogsTypeDef,
     FirehoseTypeDef,
     S3TypeDef,
     BrokerSoftwareInfoTypeDef,
+    TlsOutputTypeDef,
+    UnauthenticatedOutputTypeDef,
     TlsTypeDef,
     UnauthenticatedTypeDef,
     ClientVpcConnectionTypeDef,
     StateInfoTypeDef,
     ErrorInfoTypeDef,
     ClusterOperationStepInfoTypeDef,
     CompatibleKafkaVersionTypeDef,
+    ConfigurationInfoOutputTypeDef,
     ConfigurationInfoTypeDef,
     ConfigurationRevisionTypeDef,
+    PublicAccessOutputTypeDef,
     PublicAccessTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationRequestRequestTypeDef,
     CreateVpcConnectionRequestRequestTypeDef,
     CreateVpcConnectionResponseTypeDef,
     DeleteClusterPolicyRequestRequestTypeDef,
@@ -409,22 +417,26 @@
     DescribeClusterV2RequestRequestTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
     DescribeVpcConnectionRequestRequestTypeDef,
     DescribeVpcConnectionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionAtRestOutputTypeDef,
     EncryptionAtRestTypeDef,
+    EncryptionInTransitOutputTypeDef,
     EncryptionInTransitTypeDef,
     GetBootstrapBrokersRequestRequestTypeDef,
     GetBootstrapBrokersResponseTypeDef,
     GetClusterPolicyRequestRequestTypeDef,
     GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsRequestRequestTypeDef,
+    IamOutputTypeDef,
     IamTypeDef,
+    JmxExporterInfoOutputTypeDef,
     JmxExporterInfoTypeDef,
     JmxExporterTypeDef,
     KafkaVersionTypeDef,
     ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
     ListClientVpcConnectionsRequestRequestTypeDef,
     ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     ListClusterOperationsRequestRequestTypeDef,
@@ -444,26 +456,29 @@
     ListScramSecretsRequestRequestTypeDef,
     ListScramSecretsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef,
     ListVpcConnectionsRequestRequestTypeDef,
     VpcConnectionTypeDef,
+    NodeExporterInfoOutputTypeDef,
     NodeExporterInfoTypeDef,
     NodeExporterTypeDef,
     ZookeeperNodeInfoTypeDef,
     PaginatorConfigTypeDef,
     PutClusterPolicyRequestRequestTypeDef,
     PutClusterPolicyResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
     RebootBrokerResponseTypeDef,
     RejectClientVpcConnectionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    ScramOutputTypeDef,
     ScramTypeDef,
     VpcConfigTypeDef,
+    VpcConfigOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrokerCountRequestRequestTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
     UpdateBrokerTypeRequestRequestTypeDef,
     UpdateBrokerTypeResponseTypeDef,
@@ -471,74 +486,94 @@
     UpdateClusterKafkaVersionResponseTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     UpdateConnectivityResponseTypeDef,
     UpdateMonitoringResponseTypeDef,
     UpdateSecurityResponseTypeDef,
     UpdateStorageResponseTypeDef,
     UserIdentityTypeDef,
+    VpcConnectivityTlsOutputTypeDef,
     VpcConnectivityTlsTypeDef,
+    VpcConnectivityIamOutputTypeDef,
     VpcConnectivityIamTypeDef,
+    VpcConnectivityScramOutputTypeDef,
     VpcConnectivityScramTypeDef,
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
+    BrokerEBSVolumeInfoOutputTypeDef,
+    EBSStorageInfoOutputTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     EBSStorageInfoTypeDef,
     UpdateStorageRequestRequestTypeDef,
+    BrokerLogsOutputTypeDef,
     BrokerLogsTypeDef,
     BrokerNodeInfoTypeDef,
     ListClientVpcConnectionsResponseTypeDef,
     ClusterOperationStepTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     UpdateClusterConfigurationRequestRequestTypeDef,
     UpdateClusterKafkaVersionRequestRequestTypeDef,
     ConfigurationTypeDef,
     CreateConfigurationResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     UpdateConfigurationResponseTypeDef,
+    EncryptionInfoOutputTypeDef,
     EncryptionInfoTypeDef,
+    ServerlessSaslOutputTypeDef,
     ServerlessSaslTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListVpcConnectionsResponseTypeDef,
+    PrometheusInfoOutputTypeDef,
     PrometheusInfoTypeDef,
     PrometheusTypeDef,
+    SaslOutputTypeDef,
     SaslTypeDef,
     VpcConnectionInfoTypeDef,
+    VpcConnectivitySaslOutputTypeDef,
     VpcConnectivitySaslTypeDef,
+    StorageInfoOutputTypeDef,
     UpdateBrokerStorageRequestRequestTypeDef,
     StorageInfoTypeDef,
+    LoggingInfoOutputTypeDef,
     LoggingInfoTypeDef,
     NodeInfoTypeDef,
     ListConfigurationsResponseTypeDef,
+    ServerlessClientAuthenticationOutputTypeDef,
     ServerlessClientAuthenticationTypeDef,
+    OpenMonitoringInfoOutputTypeDef,
     OpenMonitoringInfoTypeDef,
     OpenMonitoringTypeDef,
+    ClientAuthenticationOutputTypeDef,
     ClientAuthenticationTypeDef,
+    VpcConnectivityClientAuthenticationOutputTypeDef,
     VpcConnectivityClientAuthenticationTypeDef,
     ListNodesResponseTypeDef,
-    ServerlessRequestTypeDef,
     ServerlessTypeDef,
+    ServerlessRequestTypeDef,
     UpdateMonitoringRequestRequestTypeDef,
     UpdateSecurityRequestRequestTypeDef,
+    VpcConnectivityOutputTypeDef,
     VpcConnectivityTypeDef,
+    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
-    BrokerNodeGroupInfoTypeDef,
+    BrokerNodeGroupInfoOutputTypeDef,
     MutableClusterInfoTypeDef,
+    BrokerNodeGroupInfoTypeDef,
     UpdateConnectivityRequestRequestTypeDef,
     ClusterInfoTypeDef,
-    CreateClusterRequestRequestTypeDef,
-    ProvisionedRequestTypeDef,
     ProvisionedTypeDef,
     ClusterOperationInfoTypeDef,
+    CreateClusterRequestRequestTypeDef,
+    ProvisionedRequestTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
-    CreateClusterV2RequestRequestTypeDef,
     ClusterTypeDef,
     DescribeClusterOperationResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
+    CreateClusterV2RequestRequestTypeDef,
     DescribeClusterV2ResponseTypeDef,
     ListClustersV2ResponseTypeDef,
 )
 
 
 def get_structure() -> BatchAssociateScramSecretRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-kafka-1.28.0/mypy_boto3_kafka.egg-info/SOURCES.txt` & `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.0/setup.py` & `mypy-boto3-kafka-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kafka",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_kafka"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Kafka 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Kafka 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

