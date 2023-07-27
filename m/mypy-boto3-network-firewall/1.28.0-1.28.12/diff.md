# Comparing `tmp/mypy-boto3-network-firewall-1.28.0.tar.gz` & `tmp/mypy-boto3-network-firewall-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-network-firewall-1.28.0.tar", last modified: Thu Jul  6 21:00:12 2023, max compression
+gzip compressed data, was "mypy-boto3-network-firewall-1.28.12.tar", last modified: Thu Jul 27 05:35:05 2023, max compression
```

## Comparing `mypy-boto3-network-firewall-1.28.0.tar` & `mypy-boto3-network-firewall-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:12.398380 mypy-boto3-network-firewall-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:48:11.000000 mypy-boto3-network-firewall-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19449 2023-07-06 21:00:12.398380 mypy-boto3-network-firewall-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17929 2023-07-06 20:48:11.000000 mypy-boto3-network-firewall-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:12.390380 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-06 20:48:11.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-06 20:48:11.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 20:48:11.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32089 2023-07-06 20:48:12.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32041 2023-07-06 20:48:11.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-07-06 20:48:12.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-07-06 20:48:12.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-07-06 20:48:12.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-06 20:48:12.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:48:11.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    47527 2023-07-06 20:48:13.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47471 2023-07-06 20:48:13.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:48:11.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:12.398380 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19449 2023-07-06 21:00:12.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-06 21:00:12.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:12.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:12.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:12.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 21:00:12.000000 mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:12.398380 mypy-boto3-network-firewall-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-06 20:48:11.000000 mypy-boto3-network-firewall-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:05.136426 mypy-boto3-network-firewall-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-07-27 05:35:05.136426 mypy-boto3-network-firewall-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:05.132426 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32089 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32041 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59450 2023-07-27 05:26:58.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59378 2023-07-27 05:26:56.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:05.136426 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-07-27 05:35:04.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 05:35:04.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:04.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:35:04.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:05.136426 mypy-boto3-network-firewall-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/setup.py
```

### Comparing `mypy-boto3-network-firewall-1.28.0/LICENSE` & `mypy-boto3-network-firewall-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.0/PKG-INFO` & `mypy-boto3-network-firewall-1.28.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-network-firewall
-Version: 1.28.0
-Summary: Type annotations for boto3.NetworkFirewall 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.NetworkFirewall 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-network-firewall"></a>
 
 # mypy-boto3-network-firewall
 
 [![PyPI - mypy-boto3-network-firewall](https://img.shields.io/pypi/v/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-network-firewall?color=blue)](https://pypistats.org/packages/mypy-boto3-network-firewall)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-network-firewall)](https://pepy.tech/project/mypy-boto3-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NetworkFirewall 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[boto3.NetworkFirewall 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,18 +361,20 @@
 ### Typed dictionaries
 
 `mypy_boto3_network_firewall.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_network_firewall.type_defs import (
+    AddressOutputTypeDef,
     AddressTypeDef,
     AssociateFirewallPolicyRequestRequestTypeDef,
     AssociateFirewallPolicyResponseTypeDef,
     SubnetMappingTypeDef,
+    SubnetMappingOutputTypeDef,
     AttachmentTypeDef,
     IPSetMetadataTypeDef,
     EncryptionConfigurationTypeDef,
     TagTypeDef,
     SourceMetadataTypeDef,
     DeleteFirewallPolicyRequestRequestTypeDef,
     DeleteFirewallRequestRequestTypeDef,
@@ -381,49 +383,67 @@
     DeleteTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallRequestRequestTypeDef,
     DescribeLoggingConfigurationRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
     DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataRequestRequestTypeDef,
-    StatefulRuleOptionsTypeDef,
+    StatefulRuleOptionsOutputTypeDef,
     DescribeRuleGroupRequestRequestTypeDef,
     DescribeTLSInspectionConfigurationRequestRequestTypeDef,
+    DimensionOutputTypeDef,
     DimensionTypeDef,
     DisassociateSubnetsRequestRequestTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     FirewallMetadataTypeDef,
     FirewallPolicyMetadataTypeDef,
+    StatefulEngineOptionsOutputTypeDef,
+    StatelessRuleGroupReferenceOutputTypeDef,
+    TagOutputTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupReferenceTypeDef,
+    HeaderOutputTypeDef,
     HeaderTypeDef,
+    IPSetOutputTypeDef,
+    IPSetReferenceOutputTypeDef,
     IPSetReferenceTypeDef,
     IPSetTypeDef,
     ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
     ListFirewallPoliciesRequestRequestTypeDef,
     ListFirewallsRequestListFirewallsPaginateTypeDef,
     ListFirewallsRequestRequestTypeDef,
     ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupMetadataTypeDef,
     ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
     ListTLSInspectionConfigurationsRequestRequestTypeDef,
     TLSInspectionConfigurationMetadataTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    LogDestinationConfigOutputTypeDef,
     LogDestinationConfigTypeDef,
+    PortRangeOutputTypeDef,
+    TCPFlagFieldOutputTypeDef,
     PortRangeTypeDef,
     TCPFlagFieldTypeDef,
     PaginatorConfigTypeDef,
     PerObjectStatusTypeDef,
+    PortSetOutputTypeDef,
     PortSetTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    SourceMetadataOutputTypeDef,
+    StatefulRuleOptionsTypeDef,
+    RuleOptionOutputTypeDef,
     RuleOptionTypeDef,
+    RulesSourceListOutputTypeDef,
     RulesSourceListTypeDef,
+    ServerCertificateOutputTypeDef,
     ServerCertificateTypeDef,
+    StatefulRuleGroupOverrideOutputTypeDef,
     StatefulRuleGroupOverrideTypeDef,
     TlsCertificateDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallDeleteProtectionRequestRequestTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionRequestRequestTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
@@ -432,77 +452,96 @@
     UpdateSubnetChangeProtectionRequestRequestTypeDef,
     UpdateSubnetChangeProtectionResponseTypeDef,
     AssociateSubnetsRequestRequestTypeDef,
     AssociateSubnetsResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     CIDRSummaryTypeDef,
     UpdateFirewallEncryptionConfigurationRequestRequestTypeDef,
-    UpdateFirewallEncryptionConfigurationResponseTypeDef,
     CreateFirewallRequestRequestTypeDef,
-    FirewallPolicyResponseTypeDef,
-    FirewallTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    RuleGroupResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
+    PublishMetricActionOutputTypeDef,
     PublishMetricActionTypeDef,
+    UpdateFirewallEncryptionConfigurationResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListFirewallPoliciesResponseTypeDef,
+    FirewallPolicyResponseTypeDef,
+    FirewallTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PolicyVariablesOutputTypeDef,
+    ReferenceSetsOutputTypeDef,
     ReferenceSetsTypeDef,
     PolicyVariablesTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
+    ServerCertificateScopeOutputTypeDef,
+    MatchAttributesOutputTypeDef,
     ServerCertificateScopeTypeDef,
     MatchAttributesTypeDef,
     SyncStateTypeDef,
+    RuleVariablesOutputTypeDef,
     RuleVariablesTypeDef,
+    RuleGroupResponseTypeDef,
+    StatefulRuleOutputTypeDef,
     StatefulRuleTypeDef,
+    StatefulRuleGroupReferenceOutputTypeDef,
     StatefulRuleGroupReferenceTypeDef,
     TLSInspectionConfigurationResponseTypeDef,
     CapacityUsageSummaryTypeDef,
+    ActionDefinitionOutputTypeDef,
+    ActionDefinitionTypeDef,
     CreateFirewallPolicyResponseTypeDef,
     DeleteFirewallPolicyResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
-    CreateRuleGroupResponseTypeDef,
-    DeleteRuleGroupResponseTypeDef,
-    UpdateRuleGroupResponseTypeDef,
-    ActionDefinitionTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
-    UpdateLoggingConfigurationRequestRequestTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
+    UpdateLoggingConfigurationRequestRequestTypeDef,
+    ServerCertificateConfigurationOutputTypeDef,
+    RuleDefinitionOutputTypeDef,
     ServerCertificateConfigurationTypeDef,
     RuleDefinitionTypeDef,
+    CreateRuleGroupResponseTypeDef,
+    DeleteRuleGroupResponseTypeDef,
+    UpdateRuleGroupResponseTypeDef,
     CreateTLSInspectionConfigurationResponseTypeDef,
     DeleteTLSInspectionConfigurationResponseTypeDef,
     UpdateTLSInspectionConfigurationResponseTypeDef,
     FirewallStatusTypeDef,
+    CustomActionOutputTypeDef,
     CustomActionTypeDef,
+    TLSInspectionConfigurationOutputTypeDef,
+    StatelessRuleOutputTypeDef,
     TLSInspectionConfigurationTypeDef,
     StatelessRuleTypeDef,
     CreateFirewallResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DescribeFirewallResponseTypeDef,
+    FirewallPolicyOutputTypeDef,
     FirewallPolicyTypeDef,
-    CreateTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
+    StatelessRulesAndCustomActionsOutputTypeDef,
+    CreateTLSInspectionConfigurationRequestRequestTypeDef,
     UpdateTLSInspectionConfigurationRequestRequestTypeDef,
     StatelessRulesAndCustomActionsTypeDef,
-    CreateFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
+    CreateFirewallPolicyRequestRequestTypeDef,
     UpdateFirewallPolicyRequestRequestTypeDef,
+    RulesSourceOutputTypeDef,
     RulesSourceTypeDef,
+    RuleGroupOutputTypeDef,
     RuleGroupTypeDef,
-    CreateRuleGroupRequestRequestTypeDef,
     DescribeRuleGroupResponseTypeDef,
+    CreateRuleGroupRequestRequestTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_structure() -> AddressOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-network-firewall-1.28.0/README.md` & `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-network-firewall
+Version: 1.28.12
+Summary: Type annotations for boto3.NetworkFirewall 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 network-firewall type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-network-firewall"></a>
 
 # mypy-boto3-network-firewall
 
 [![PyPI - mypy-boto3-network-firewall](https://img.shields.io/pypi/v/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-network-firewall?color=blue)](https://pypistats.org/packages/mypy-boto3-network-firewall)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-network-firewall)](https://pepy.tech/project/mypy-boto3-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NetworkFirewall 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[boto3.NetworkFirewall 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,18 +361,20 @@
 ### Typed dictionaries
 
 `mypy_boto3_network_firewall.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_network_firewall.type_defs import (
+    AddressOutputTypeDef,
     AddressTypeDef,
     AssociateFirewallPolicyRequestRequestTypeDef,
     AssociateFirewallPolicyResponseTypeDef,
     SubnetMappingTypeDef,
+    SubnetMappingOutputTypeDef,
     AttachmentTypeDef,
     IPSetMetadataTypeDef,
     EncryptionConfigurationTypeDef,
     TagTypeDef,
     SourceMetadataTypeDef,
     DeleteFirewallPolicyRequestRequestTypeDef,
     DeleteFirewallRequestRequestTypeDef,
@@ -349,49 +383,67 @@
     DeleteTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallRequestRequestTypeDef,
     DescribeLoggingConfigurationRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
     DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataRequestRequestTypeDef,
-    StatefulRuleOptionsTypeDef,
+    StatefulRuleOptionsOutputTypeDef,
     DescribeRuleGroupRequestRequestTypeDef,
     DescribeTLSInspectionConfigurationRequestRequestTypeDef,
+    DimensionOutputTypeDef,
     DimensionTypeDef,
     DisassociateSubnetsRequestRequestTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     FirewallMetadataTypeDef,
     FirewallPolicyMetadataTypeDef,
+    StatefulEngineOptionsOutputTypeDef,
+    StatelessRuleGroupReferenceOutputTypeDef,
+    TagOutputTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupReferenceTypeDef,
+    HeaderOutputTypeDef,
     HeaderTypeDef,
+    IPSetOutputTypeDef,
+    IPSetReferenceOutputTypeDef,
     IPSetReferenceTypeDef,
     IPSetTypeDef,
     ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
     ListFirewallPoliciesRequestRequestTypeDef,
     ListFirewallsRequestListFirewallsPaginateTypeDef,
     ListFirewallsRequestRequestTypeDef,
     ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupMetadataTypeDef,
     ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
     ListTLSInspectionConfigurationsRequestRequestTypeDef,
     TLSInspectionConfigurationMetadataTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    LogDestinationConfigOutputTypeDef,
     LogDestinationConfigTypeDef,
+    PortRangeOutputTypeDef,
+    TCPFlagFieldOutputTypeDef,
     PortRangeTypeDef,
     TCPFlagFieldTypeDef,
     PaginatorConfigTypeDef,
     PerObjectStatusTypeDef,
+    PortSetOutputTypeDef,
     PortSetTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    SourceMetadataOutputTypeDef,
+    StatefulRuleOptionsTypeDef,
+    RuleOptionOutputTypeDef,
     RuleOptionTypeDef,
+    RulesSourceListOutputTypeDef,
     RulesSourceListTypeDef,
+    ServerCertificateOutputTypeDef,
     ServerCertificateTypeDef,
+    StatefulRuleGroupOverrideOutputTypeDef,
     StatefulRuleGroupOverrideTypeDef,
     TlsCertificateDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallDeleteProtectionRequestRequestTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionRequestRequestTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
@@ -400,77 +452,96 @@
     UpdateSubnetChangeProtectionRequestRequestTypeDef,
     UpdateSubnetChangeProtectionResponseTypeDef,
     AssociateSubnetsRequestRequestTypeDef,
     AssociateSubnetsResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     CIDRSummaryTypeDef,
     UpdateFirewallEncryptionConfigurationRequestRequestTypeDef,
-    UpdateFirewallEncryptionConfigurationResponseTypeDef,
     CreateFirewallRequestRequestTypeDef,
-    FirewallPolicyResponseTypeDef,
-    FirewallTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    RuleGroupResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
+    PublishMetricActionOutputTypeDef,
     PublishMetricActionTypeDef,
+    UpdateFirewallEncryptionConfigurationResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListFirewallPoliciesResponseTypeDef,
+    FirewallPolicyResponseTypeDef,
+    FirewallTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PolicyVariablesOutputTypeDef,
+    ReferenceSetsOutputTypeDef,
     ReferenceSetsTypeDef,
     PolicyVariablesTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
+    ServerCertificateScopeOutputTypeDef,
+    MatchAttributesOutputTypeDef,
     ServerCertificateScopeTypeDef,
     MatchAttributesTypeDef,
     SyncStateTypeDef,
+    RuleVariablesOutputTypeDef,
     RuleVariablesTypeDef,
+    RuleGroupResponseTypeDef,
+    StatefulRuleOutputTypeDef,
     StatefulRuleTypeDef,
+    StatefulRuleGroupReferenceOutputTypeDef,
     StatefulRuleGroupReferenceTypeDef,
     TLSInspectionConfigurationResponseTypeDef,
     CapacityUsageSummaryTypeDef,
+    ActionDefinitionOutputTypeDef,
+    ActionDefinitionTypeDef,
     CreateFirewallPolicyResponseTypeDef,
     DeleteFirewallPolicyResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
-    CreateRuleGroupResponseTypeDef,
-    DeleteRuleGroupResponseTypeDef,
-    UpdateRuleGroupResponseTypeDef,
-    ActionDefinitionTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
-    UpdateLoggingConfigurationRequestRequestTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
+    UpdateLoggingConfigurationRequestRequestTypeDef,
+    ServerCertificateConfigurationOutputTypeDef,
+    RuleDefinitionOutputTypeDef,
     ServerCertificateConfigurationTypeDef,
     RuleDefinitionTypeDef,
+    CreateRuleGroupResponseTypeDef,
+    DeleteRuleGroupResponseTypeDef,
+    UpdateRuleGroupResponseTypeDef,
     CreateTLSInspectionConfigurationResponseTypeDef,
     DeleteTLSInspectionConfigurationResponseTypeDef,
     UpdateTLSInspectionConfigurationResponseTypeDef,
     FirewallStatusTypeDef,
+    CustomActionOutputTypeDef,
     CustomActionTypeDef,
+    TLSInspectionConfigurationOutputTypeDef,
+    StatelessRuleOutputTypeDef,
     TLSInspectionConfigurationTypeDef,
     StatelessRuleTypeDef,
     CreateFirewallResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DescribeFirewallResponseTypeDef,
+    FirewallPolicyOutputTypeDef,
     FirewallPolicyTypeDef,
-    CreateTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
+    StatelessRulesAndCustomActionsOutputTypeDef,
+    CreateTLSInspectionConfigurationRequestRequestTypeDef,
     UpdateTLSInspectionConfigurationRequestRequestTypeDef,
     StatelessRulesAndCustomActionsTypeDef,
-    CreateFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
+    CreateFirewallPolicyRequestRequestTypeDef,
     UpdateFirewallPolicyRequestRequestTypeDef,
+    RulesSourceOutputTypeDef,
     RulesSourceTypeDef,
+    RuleGroupOutputTypeDef,
     RuleGroupTypeDef,
-    CreateRuleGroupRequestRequestTypeDef,
     DescribeRuleGroupResponseTypeDef,
+    CreateRuleGroupRequestRequestTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_structure() -> AddressOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/__init__.py` & `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/__init__.pyi` & `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/__main__.py` & `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.NetworkFirewall 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.NetworkFirewall 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall\nOther"
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

### Comparing `mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/client.py` & `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/client.pyi` & `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/literals.py` & `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/literals.py`

 * *Files 2% similar despite different names*

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
@@ -475,21 +478,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/literals.pyi` & `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/literals.pyi`

 * *Files 2% similar despite different names*

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
@@ -473,21 +476,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/paginator.py` & `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/paginator.pyi` & `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/type_defs.py` & `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for network-firewall service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_network_firewall.type_defs import AddressTypeDef
+    from mypy_boto3_network_firewall.type_defs import AddressOutputTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -45,18 +45,20 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AddressOutputTypeDef",
     "AddressTypeDef",
     "AssociateFirewallPolicyRequestRequestTypeDef",
     "AssociateFirewallPolicyResponseTypeDef",
     "SubnetMappingTypeDef",
+    "SubnetMappingOutputTypeDef",
     "AttachmentTypeDef",
     "IPSetMetadataTypeDef",
     "EncryptionConfigurationTypeDef",
     "TagTypeDef",
     "SourceMetadataTypeDef",
     "DeleteFirewallPolicyRequestRequestTypeDef",
     "DeleteFirewallRequestRequestTypeDef",
@@ -65,49 +67,67 @@
     "DeleteTLSInspectionConfigurationRequestRequestTypeDef",
     "DescribeFirewallPolicyRequestRequestTypeDef",
     "DescribeFirewallRequestRequestTypeDef",
     "DescribeLoggingConfigurationRequestRequestTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
     "DescribeResourcePolicyResponseTypeDef",
     "DescribeRuleGroupMetadataRequestRequestTypeDef",
-    "StatefulRuleOptionsTypeDef",
+    "StatefulRuleOptionsOutputTypeDef",
     "DescribeRuleGroupRequestRequestTypeDef",
     "DescribeTLSInspectionConfigurationRequestRequestTypeDef",
+    "DimensionOutputTypeDef",
     "DimensionTypeDef",
     "DisassociateSubnetsRequestRequestTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
     "FirewallMetadataTypeDef",
     "FirewallPolicyMetadataTypeDef",
+    "StatefulEngineOptionsOutputTypeDef",
+    "StatelessRuleGroupReferenceOutputTypeDef",
+    "TagOutputTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupReferenceTypeDef",
+    "HeaderOutputTypeDef",
     "HeaderTypeDef",
+    "IPSetOutputTypeDef",
+    "IPSetReferenceOutputTypeDef",
     "IPSetReferenceTypeDef",
     "IPSetTypeDef",
     "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
     "ListFirewallPoliciesRequestRequestTypeDef",
     "ListFirewallsRequestListFirewallsPaginateTypeDef",
     "ListFirewallsRequestRequestTypeDef",
     "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupMetadataTypeDef",
     "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
     "ListTLSInspectionConfigurationsRequestRequestTypeDef",
     "TLSInspectionConfigurationMetadataTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "LogDestinationConfigOutputTypeDef",
     "LogDestinationConfigTypeDef",
+    "PortRangeOutputTypeDef",
+    "TCPFlagFieldOutputTypeDef",
     "PortRangeTypeDef",
     "TCPFlagFieldTypeDef",
     "PaginatorConfigTypeDef",
     "PerObjectStatusTypeDef",
+    "PortSetOutputTypeDef",
     "PortSetTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "SourceMetadataOutputTypeDef",
+    "StatefulRuleOptionsTypeDef",
+    "RuleOptionOutputTypeDef",
     "RuleOptionTypeDef",
+    "RulesSourceListOutputTypeDef",
     "RulesSourceListTypeDef",
+    "ServerCertificateOutputTypeDef",
     "ServerCertificateTypeDef",
+    "StatefulRuleGroupOverrideOutputTypeDef",
     "StatefulRuleGroupOverrideTypeDef",
     "TlsCertificateDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallDeleteProtectionRequestRequestTypeDef",
     "UpdateFirewallDeleteProtectionResponseTypeDef",
     "UpdateFirewallDescriptionRequestRequestTypeDef",
     "UpdateFirewallDescriptionResponseTypeDef",
@@ -116,75 +136,101 @@
     "UpdateSubnetChangeProtectionRequestRequestTypeDef",
     "UpdateSubnetChangeProtectionResponseTypeDef",
     "AssociateSubnetsRequestRequestTypeDef",
     "AssociateSubnetsResponseTypeDef",
     "DisassociateSubnetsResponseTypeDef",
     "CIDRSummaryTypeDef",
     "UpdateFirewallEncryptionConfigurationRequestRequestTypeDef",
-    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
     "CreateFirewallRequestRequestTypeDef",
-    "FirewallPolicyResponseTypeDef",
-    "FirewallTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "RuleGroupResponseTypeDef",
     "DescribeRuleGroupMetadataResponseTypeDef",
+    "PublishMetricActionOutputTypeDef",
     "PublishMetricActionTypeDef",
+    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
     "ListFirewallsResponseTypeDef",
     "ListFirewallPoliciesResponseTypeDef",
+    "FirewallPolicyResponseTypeDef",
+    "FirewallTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PolicyVariablesOutputTypeDef",
+    "ReferenceSetsOutputTypeDef",
     "ReferenceSetsTypeDef",
     "PolicyVariablesTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "ListTLSInspectionConfigurationsResponseTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
+    "ServerCertificateScopeOutputTypeDef",
+    "MatchAttributesOutputTypeDef",
     "ServerCertificateScopeTypeDef",
     "MatchAttributesTypeDef",
     "SyncStateTypeDef",
+    "RuleVariablesOutputTypeDef",
     "RuleVariablesTypeDef",
+    "RuleGroupResponseTypeDef",
+    "StatefulRuleOutputTypeDef",
     "StatefulRuleTypeDef",
+    "StatefulRuleGroupReferenceOutputTypeDef",
     "StatefulRuleGroupReferenceTypeDef",
     "TLSInspectionConfigurationResponseTypeDef",
     "CapacityUsageSummaryTypeDef",
+    "ActionDefinitionOutputTypeDef",
+    "ActionDefinitionTypeDef",
     "CreateFirewallPolicyResponseTypeDef",
     "DeleteFirewallPolicyResponseTypeDef",
     "UpdateFirewallPolicyResponseTypeDef",
-    "CreateRuleGroupResponseTypeDef",
-    "DeleteRuleGroupResponseTypeDef",
-    "UpdateRuleGroupResponseTypeDef",
-    "ActionDefinitionTypeDef",
     "DescribeLoggingConfigurationResponseTypeDef",
-    "UpdateLoggingConfigurationRequestRequestTypeDef",
     "UpdateLoggingConfigurationResponseTypeDef",
+    "UpdateLoggingConfigurationRequestRequestTypeDef",
+    "ServerCertificateConfigurationOutputTypeDef",
+    "RuleDefinitionOutputTypeDef",
     "ServerCertificateConfigurationTypeDef",
     "RuleDefinitionTypeDef",
+    "CreateRuleGroupResponseTypeDef",
+    "DeleteRuleGroupResponseTypeDef",
+    "UpdateRuleGroupResponseTypeDef",
     "CreateTLSInspectionConfigurationResponseTypeDef",
     "DeleteTLSInspectionConfigurationResponseTypeDef",
     "UpdateTLSInspectionConfigurationResponseTypeDef",
     "FirewallStatusTypeDef",
+    "CustomActionOutputTypeDef",
     "CustomActionTypeDef",
+    "TLSInspectionConfigurationOutputTypeDef",
+    "StatelessRuleOutputTypeDef",
     "TLSInspectionConfigurationTypeDef",
     "StatelessRuleTypeDef",
     "CreateFirewallResponseTypeDef",
     "DeleteFirewallResponseTypeDef",
     "DescribeFirewallResponseTypeDef",
+    "FirewallPolicyOutputTypeDef",
     "FirewallPolicyTypeDef",
-    "CreateTLSInspectionConfigurationRequestRequestTypeDef",
     "DescribeTLSInspectionConfigurationResponseTypeDef",
+    "StatelessRulesAndCustomActionsOutputTypeDef",
+    "CreateTLSInspectionConfigurationRequestRequestTypeDef",
     "UpdateTLSInspectionConfigurationRequestRequestTypeDef",
     "StatelessRulesAndCustomActionsTypeDef",
-    "CreateFirewallPolicyRequestRequestTypeDef",
     "DescribeFirewallPolicyResponseTypeDef",
+    "CreateFirewallPolicyRequestRequestTypeDef",
     "UpdateFirewallPolicyRequestRequestTypeDef",
+    "RulesSourceOutputTypeDef",
     "RulesSourceTypeDef",
+    "RuleGroupOutputTypeDef",
     "RuleGroupTypeDef",
-    "CreateRuleGroupRequestRequestTypeDef",
     "DescribeRuleGroupResponseTypeDef",
+    "CreateRuleGroupRequestRequestTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
 )
 
+AddressOutputTypeDef = TypedDict(
+    "AddressOutputTypeDef",
+    {
+        "AddressDefinition": str,
+    },
+)
+
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressDefinition": str,
     },
 )
 
@@ -238,14 +284,35 @@
 )
 
 
 class SubnetMappingTypeDef(_RequiredSubnetMappingTypeDef, _OptionalSubnetMappingTypeDef):
     pass
 
 
+_RequiredSubnetMappingOutputTypeDef = TypedDict(
+    "_RequiredSubnetMappingOutputTypeDef",
+    {
+        "SubnetId": str,
+    },
+)
+_OptionalSubnetMappingOutputTypeDef = TypedDict(
+    "_OptionalSubnetMappingOutputTypeDef",
+    {
+        "IPAddressType": IPAddressTypeType,
+    },
+    total=False,
+)
+
+
+class SubnetMappingOutputTypeDef(
+    _RequiredSubnetMappingOutputTypeDef, _OptionalSubnetMappingOutputTypeDef
+):
+    pass
+
+
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "SubnetId": str,
         "EndpointId": str,
         "Status": AttachmentStatusType,
         "StatusMessage": str,
@@ -391,16 +458,16 @@
         "RuleGroupName": str,
         "RuleGroupArn": str,
         "Type": RuleGroupTypeType,
     },
     total=False,
 )
 
-StatefulRuleOptionsTypeDef = TypedDict(
-    "StatefulRuleOptionsTypeDef",
+StatefulRuleOptionsOutputTypeDef = TypedDict(
+    "StatefulRuleOptionsOutputTypeDef",
     {
         "RuleOrder": RuleOrderType,
     },
     total=False,
 )
 
 DescribeRuleGroupRequestRequestTypeDef = TypedDict(
@@ -418,14 +485,21 @@
     {
         "TLSInspectionConfigurationArn": str,
         "TLSInspectionConfigurationName": str,
     },
     total=False,
 )
 
+DimensionOutputTypeDef = TypedDict(
+    "DimensionOutputTypeDef",
+    {
+        "Value": str,
+    },
+)
+
 DimensionTypeDef = TypedDict(
     "DimensionTypeDef",
     {
         "Value": str,
     },
 )
 
@@ -449,14 +523,35 @@
 class DisassociateSubnetsRequestRequestTypeDef(
     _RequiredDisassociateSubnetsRequestRequestTypeDef,
     _OptionalDisassociateSubnetsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredEncryptionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEncryptionConfigurationOutputTypeDef",
+    {
+        "Type": EncryptionTypeType,
+    },
+)
+_OptionalEncryptionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEncryptionConfigurationOutputTypeDef",
+    {
+        "KeyId": str,
+    },
+    total=False,
+)
+
+
+class EncryptionConfigurationOutputTypeDef(
+    _RequiredEncryptionConfigurationOutputTypeDef, _OptionalEncryptionConfigurationOutputTypeDef
+):
+    pass
+
+
 FirewallMetadataTypeDef = TypedDict(
     "FirewallMetadataTypeDef",
     {
         "FirewallName": str,
         "FirewallArn": str,
     },
     total=False,
@@ -467,14 +562,39 @@
     {
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
+StatefulEngineOptionsOutputTypeDef = TypedDict(
+    "StatefulEngineOptionsOutputTypeDef",
+    {
+        "RuleOrder": RuleOrderType,
+        "StreamExceptionPolicy": StreamExceptionPolicyType,
+    },
+    total=False,
+)
+
+StatelessRuleGroupReferenceOutputTypeDef = TypedDict(
+    "StatelessRuleGroupReferenceOutputTypeDef",
+    {
+        "ResourceArn": str,
+        "Priority": int,
+    },
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 StatefulEngineOptionsTypeDef = TypedDict(
     "StatefulEngineOptionsTypeDef",
     {
         "RuleOrder": RuleOrderType,
         "StreamExceptionPolicy": StreamExceptionPolicyType,
     },
     total=False,
@@ -484,26 +604,53 @@
     "StatelessRuleGroupReferenceTypeDef",
     {
         "ResourceArn": str,
         "Priority": int,
     },
 )
 
+HeaderOutputTypeDef = TypedDict(
+    "HeaderOutputTypeDef",
+    {
+        "Protocol": StatefulRuleProtocolType,
+        "Source": str,
+        "SourcePort": str,
+        "Direction": StatefulRuleDirectionType,
+        "Destination": str,
+        "DestinationPort": str,
+    },
+)
+
 HeaderTypeDef = TypedDict(
     "HeaderTypeDef",
     {
         "Protocol": StatefulRuleProtocolType,
         "Source": str,
         "SourcePort": str,
         "Direction": StatefulRuleDirectionType,
         "Destination": str,
         "DestinationPort": str,
     },
 )
 
+IPSetOutputTypeDef = TypedDict(
+    "IPSetOutputTypeDef",
+    {
+        "Definition": List[str],
+    },
+)
+
+IPSetReferenceOutputTypeDef = TypedDict(
+    "IPSetReferenceOutputTypeDef",
+    {
+        "ReferenceArn": str,
+    },
+    total=False,
+)
+
 IPSetReferenceTypeDef = TypedDict(
     "IPSetReferenceTypeDef",
     {
         "ReferenceArn": str,
     },
     total=False,
 )
@@ -650,23 +797,61 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
+LogDestinationConfigOutputTypeDef = TypedDict(
+    "LogDestinationConfigOutputTypeDef",
+    {
+        "LogType": LogTypeType,
+        "LogDestinationType": LogDestinationTypeType,
+        "LogDestination": Dict[str, str],
+    },
+)
+
 LogDestinationConfigTypeDef = TypedDict(
     "LogDestinationConfigTypeDef",
     {
         "LogType": LogTypeType,
         "LogDestinationType": LogDestinationTypeType,
-        "LogDestination": Dict[str, str],
+        "LogDestination": Mapping[str, str],
+    },
+)
+
+PortRangeOutputTypeDef = TypedDict(
+    "PortRangeOutputTypeDef",
+    {
+        "FromPort": int,
+        "ToPort": int,
     },
 )
 
+_RequiredTCPFlagFieldOutputTypeDef = TypedDict(
+    "_RequiredTCPFlagFieldOutputTypeDef",
+    {
+        "Flags": List[TCPFlagType],
+    },
+)
+_OptionalTCPFlagFieldOutputTypeDef = TypedDict(
+    "_OptionalTCPFlagFieldOutputTypeDef",
+    {
+        "Masks": List[TCPFlagType],
+    },
+    total=False,
+)
+
+
+class TCPFlagFieldOutputTypeDef(
+    _RequiredTCPFlagFieldOutputTypeDef, _OptionalTCPFlagFieldOutputTypeDef
+):
+    pass
+
+
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
 )
@@ -705,14 +890,22 @@
     {
         "SyncStatus": PerObjectSyncStatusType,
         "UpdateToken": str,
     },
     total=False,
 )
 
+PortSetOutputTypeDef = TypedDict(
+    "PortSetOutputTypeDef",
+    {
+        "Definition": List[str],
+    },
+    total=False,
+)
+
 PortSetTypeDef = TypedDict(
     "PortSetTypeDef",
     {
         "Definition": Sequence[str],
     },
     total=False,
 )
@@ -732,14 +925,50 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+SourceMetadataOutputTypeDef = TypedDict(
+    "SourceMetadataOutputTypeDef",
+    {
+        "SourceArn": str,
+        "SourceUpdateToken": str,
+    },
+    total=False,
+)
+
+StatefulRuleOptionsTypeDef = TypedDict(
+    "StatefulRuleOptionsTypeDef",
+    {
+        "RuleOrder": RuleOrderType,
+    },
+    total=False,
+)
+
+_RequiredRuleOptionOutputTypeDef = TypedDict(
+    "_RequiredRuleOptionOutputTypeDef",
+    {
+        "Keyword": str,
+    },
+)
+_OptionalRuleOptionOutputTypeDef = TypedDict(
+    "_OptionalRuleOptionOutputTypeDef",
+    {
+        "Settings": List[str],
+    },
+    total=False,
+)
+
+
+class RuleOptionOutputTypeDef(_RequiredRuleOptionOutputTypeDef, _OptionalRuleOptionOutputTypeDef):
+    pass
+
+
 _RequiredRuleOptionTypeDef = TypedDict(
     "_RequiredRuleOptionTypeDef",
     {
         "Keyword": str,
     },
 )
 _OptionalRuleOptionTypeDef = TypedDict(
@@ -751,31 +980,56 @@
 )
 
 
 class RuleOptionTypeDef(_RequiredRuleOptionTypeDef, _OptionalRuleOptionTypeDef):
     pass
 
 
+RulesSourceListOutputTypeDef = TypedDict(
+    "RulesSourceListOutputTypeDef",
+    {
+        "Targets": List[str],
+        "TargetTypes": List[TargetTypeType],
+        "GeneratedRulesType": GeneratedRulesTypeType,
+    },
+)
+
 RulesSourceListTypeDef = TypedDict(
     "RulesSourceListTypeDef",
     {
         "Targets": Sequence[str],
         "TargetTypes": Sequence[TargetTypeType],
         "GeneratedRulesType": GeneratedRulesTypeType,
     },
 )
 
+ServerCertificateOutputTypeDef = TypedDict(
+    "ServerCertificateOutputTypeDef",
+    {
+        "ResourceArn": str,
+    },
+    total=False,
+)
+
 ServerCertificateTypeDef = TypedDict(
     "ServerCertificateTypeDef",
     {
         "ResourceArn": str,
     },
     total=False,
 )
 
+StatefulRuleGroupOverrideOutputTypeDef = TypedDict(
+    "StatefulRuleGroupOverrideOutputTypeDef",
+    {
+        "Action": Literal["DROP_TO_ALERT"],
+    },
+    total=False,
+)
+
 StatefulRuleGroupOverrideTypeDef = TypedDict(
     "StatefulRuleGroupOverrideTypeDef",
     {
         "Action": Literal["DROP_TO_ALERT"],
     },
     total=False,
 )
@@ -950,26 +1204,26 @@
 
 
 AssociateSubnetsResponseTypeDef = TypedDict(
     "AssociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
-        "SubnetMappings": List[SubnetMappingTypeDef],
+        "SubnetMappings": List[SubnetMappingOutputTypeDef],
         "UpdateToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateSubnetsResponseTypeDef = TypedDict(
     "DisassociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
-        "SubnetMappings": List[SubnetMappingTypeDef],
+        "SubnetMappings": List[SubnetMappingOutputTypeDef],
         "UpdateToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CIDRSummaryTypeDef = TypedDict(
     "CIDRSummaryTypeDef",
@@ -988,25 +1242,14 @@
         "FirewallArn": str,
         "FirewallName": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
-UpdateFirewallEncryptionConfigurationResponseTypeDef = TypedDict(
-    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "UpdateToken": str,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFirewallRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallRequestRequestTypeDef",
     {
         "FirewallName": str,
         "FirewallPolicyArn": str,
         "VpcId": str,
         "SubnetMappings": Sequence[SubnetMappingTypeDef],
@@ -1028,32 +1271,97 @@
 
 class CreateFirewallRequestRequestTypeDef(
     _RequiredCreateFirewallRequestRequestTypeDef, _OptionalCreateFirewallRequestRequestTypeDef
 ):
     pass
 
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+DescribeRuleGroupMetadataResponseTypeDef = TypedDict(
+    "DescribeRuleGroupMetadataResponseTypeDef",
+    {
+        "RuleGroupArn": str,
+        "RuleGroupName": str,
+        "Description": str,
+        "Type": RuleGroupTypeType,
+        "Capacity": int,
+        "StatefulRuleOptions": StatefulRuleOptionsOutputTypeDef,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PublishMetricActionOutputTypeDef = TypedDict(
+    "PublishMetricActionOutputTypeDef",
+    {
+        "Dimensions": List[DimensionOutputTypeDef],
+    },
+)
+
+PublishMetricActionTypeDef = TypedDict(
+    "PublishMetricActionTypeDef",
+    {
+        "Dimensions": Sequence[DimensionTypeDef],
+    },
+)
+
+UpdateFirewallEncryptionConfigurationResponseTypeDef = TypedDict(
+    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "UpdateToken": str,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListFirewallsResponseTypeDef = TypedDict(
+    "ListFirewallsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Firewalls": List[FirewallMetadataTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListFirewallPoliciesResponseTypeDef = TypedDict(
+    "ListFirewallPoliciesResponseTypeDef",
+    {
+        "NextToken": str,
+        "FirewallPolicies": List[FirewallPolicyMetadataTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFirewallPolicyResponseTypeDef = TypedDict(
     "_RequiredFirewallPolicyResponseTypeDef",
     {
         "FirewallPolicyName": str,
         "FirewallPolicyArn": str,
         "FirewallPolicyId": str,
     },
 )
 _OptionalFirewallPolicyResponseTypeDef = TypedDict(
     "_OptionalFirewallPolicyResponseTypeDef",
     {
         "Description": str,
         "FirewallPolicyStatus": ResourceStatusType,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ConsumedStatelessRuleCapacity": int,
         "ConsumedStatefulRuleCapacity": int,
         "NumberOfAssociations": int,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
 
 class FirewallPolicyResponseTypeDef(
@@ -1063,125 +1371,61 @@
 
 
 _RequiredFirewallTypeDef = TypedDict(
     "_RequiredFirewallTypeDef",
     {
         "FirewallPolicyArn": str,
         "VpcId": str,
-        "SubnetMappings": List[SubnetMappingTypeDef],
+        "SubnetMappings": List[SubnetMappingOutputTypeDef],
         "FirewallId": str,
     },
 )
 _OptionalFirewallTypeDef = TypedDict(
     "_OptionalFirewallTypeDef",
     {
         "FirewallName": str,
         "FirewallArn": str,
         "DeleteProtection": bool,
         "SubnetChangeProtection": bool,
         "FirewallPolicyChangeProtection": bool,
         "Description": str,
-        "Tags": List[TagTypeDef],
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 
 class FirewallTypeDef(_RequiredFirewallTypeDef, _OptionalFirewallTypeDef):
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "NextToken": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+PolicyVariablesOutputTypeDef = TypedDict(
+    "PolicyVariablesOutputTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-_RequiredRuleGroupResponseTypeDef = TypedDict(
-    "_RequiredRuleGroupResponseTypeDef",
-    {
-        "RuleGroupArn": str,
-        "RuleGroupName": str,
-        "RuleGroupId": str,
-    },
-)
-_OptionalRuleGroupResponseTypeDef = TypedDict(
-    "_OptionalRuleGroupResponseTypeDef",
-    {
-        "Description": str,
-        "Type": RuleGroupTypeType,
-        "Capacity": int,
-        "RuleGroupStatus": ResourceStatusType,
-        "Tags": List[TagTypeDef],
-        "ConsumedCapacity": int,
-        "NumberOfAssociations": int,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-        "SourceMetadata": SourceMetadataTypeDef,
-        "SnsTopic": str,
-        "LastModifiedTime": datetime,
+        "RuleVariables": Dict[str, IPSetOutputTypeDef],
     },
     total=False,
 )
 
-
-class RuleGroupResponseTypeDef(
-    _RequiredRuleGroupResponseTypeDef, _OptionalRuleGroupResponseTypeDef
-):
-    pass
-
-
-DescribeRuleGroupMetadataResponseTypeDef = TypedDict(
-    "DescribeRuleGroupMetadataResponseTypeDef",
+ReferenceSetsOutputTypeDef = TypedDict(
+    "ReferenceSetsOutputTypeDef",
     {
-        "RuleGroupArn": str,
-        "RuleGroupName": str,
-        "Description": str,
-        "Type": RuleGroupTypeType,
-        "Capacity": int,
-        "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PublishMetricActionTypeDef = TypedDict(
-    "PublishMetricActionTypeDef",
-    {
-        "Dimensions": Sequence[DimensionTypeDef],
-    },
-)
-
-ListFirewallsResponseTypeDef = TypedDict(
-    "ListFirewallsResponseTypeDef",
-    {
-        "NextToken": str,
-        "Firewalls": List[FirewallMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFirewallPoliciesResponseTypeDef = TypedDict(
-    "ListFirewallPoliciesResponseTypeDef",
-    {
-        "NextToken": str,
-        "FirewallPolicies": List[FirewallPolicyMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "IPSetReferences": Dict[str, IPSetReferenceOutputTypeDef],
     },
+    total=False,
 )
 
 ReferenceSetsTypeDef = TypedDict(
     "ReferenceSetsTypeDef",
     {
         "IPSetReferences": Mapping[str, IPSetReferenceTypeDef],
     },
@@ -1210,19 +1454,51 @@
     {
         "NextToken": str,
         "TLSInspectionConfigurations": List[TLSInspectionConfigurationMetadataTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LoggingConfigurationOutputTypeDef = TypedDict(
+    "LoggingConfigurationOutputTypeDef",
+    {
+        "LogDestinationConfigs": List[LogDestinationConfigOutputTypeDef],
+    },
+)
+
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
-        "LogDestinationConfigs": List[LogDestinationConfigTypeDef],
+        "LogDestinationConfigs": Sequence[LogDestinationConfigTypeDef],
+    },
+)
+
+ServerCertificateScopeOutputTypeDef = TypedDict(
+    "ServerCertificateScopeOutputTypeDef",
+    {
+        "Sources": List[AddressOutputTypeDef],
+        "Destinations": List[AddressOutputTypeDef],
+        "SourcePorts": List[PortRangeOutputTypeDef],
+        "DestinationPorts": List[PortRangeOutputTypeDef],
+        "Protocols": List[int],
+    },
+    total=False,
+)
+
+MatchAttributesOutputTypeDef = TypedDict(
+    "MatchAttributesOutputTypeDef",
+    {
+        "Sources": List[AddressOutputTypeDef],
+        "Destinations": List[AddressOutputTypeDef],
+        "SourcePorts": List[PortRangeOutputTypeDef],
+        "DestinationPorts": List[PortRangeOutputTypeDef],
+        "Protocols": List[int],
+        "TCPFlags": List[TCPFlagFieldOutputTypeDef],
     },
+    total=False,
 )
 
 ServerCertificateScopeTypeDef = TypedDict(
     "ServerCertificateScopeTypeDef",
     {
         "Sources": Sequence[AddressTypeDef],
         "Destinations": Sequence[AddressTypeDef],
@@ -1251,32 +1527,106 @@
     {
         "Attachment": AttachmentTypeDef,
         "Config": Dict[str, PerObjectStatusTypeDef],
     },
     total=False,
 )
 
+RuleVariablesOutputTypeDef = TypedDict(
+    "RuleVariablesOutputTypeDef",
+    {
+        "IPSets": Dict[str, IPSetOutputTypeDef],
+        "PortSets": Dict[str, PortSetOutputTypeDef],
+    },
+    total=False,
+)
+
 RuleVariablesTypeDef = TypedDict(
     "RuleVariablesTypeDef",
     {
         "IPSets": Mapping[str, IPSetTypeDef],
         "PortSets": Mapping[str, PortSetTypeDef],
     },
     total=False,
 )
 
+_RequiredRuleGroupResponseTypeDef = TypedDict(
+    "_RequiredRuleGroupResponseTypeDef",
+    {
+        "RuleGroupArn": str,
+        "RuleGroupName": str,
+        "RuleGroupId": str,
+    },
+)
+_OptionalRuleGroupResponseTypeDef = TypedDict(
+    "_OptionalRuleGroupResponseTypeDef",
+    {
+        "Description": str,
+        "Type": RuleGroupTypeType,
+        "Capacity": int,
+        "RuleGroupStatus": ResourceStatusType,
+        "Tags": List[TagOutputTypeDef],
+        "ConsumedCapacity": int,
+        "NumberOfAssociations": int,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "SourceMetadata": SourceMetadataOutputTypeDef,
+        "SnsTopic": str,
+        "LastModifiedTime": datetime,
+    },
+    total=False,
+)
+
+
+class RuleGroupResponseTypeDef(
+    _RequiredRuleGroupResponseTypeDef, _OptionalRuleGroupResponseTypeDef
+):
+    pass
+
+
+StatefulRuleOutputTypeDef = TypedDict(
+    "StatefulRuleOutputTypeDef",
+    {
+        "Action": StatefulActionType,
+        "Header": HeaderOutputTypeDef,
+        "RuleOptions": List[RuleOptionOutputTypeDef],
+    },
+)
+
 StatefulRuleTypeDef = TypedDict(
     "StatefulRuleTypeDef",
     {
         "Action": StatefulActionType,
         "Header": HeaderTypeDef,
         "RuleOptions": Sequence[RuleOptionTypeDef],
     },
 )
 
+_RequiredStatefulRuleGroupReferenceOutputTypeDef = TypedDict(
+    "_RequiredStatefulRuleGroupReferenceOutputTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalStatefulRuleGroupReferenceOutputTypeDef = TypedDict(
+    "_OptionalStatefulRuleGroupReferenceOutputTypeDef",
+    {
+        "Priority": int,
+        "Override": StatefulRuleGroupOverrideOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class StatefulRuleGroupReferenceOutputTypeDef(
+    _RequiredStatefulRuleGroupReferenceOutputTypeDef,
+    _OptionalStatefulRuleGroupReferenceOutputTypeDef,
+):
+    pass
+
+
 _RequiredStatefulRuleGroupReferenceTypeDef = TypedDict(
     "_RequiredStatefulRuleGroupReferenceTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalStatefulRuleGroupReferenceTypeDef = TypedDict(
@@ -1304,18 +1654,18 @@
     },
 )
 _OptionalTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "_OptionalTLSInspectionConfigurationResponseTypeDef",
     {
         "TLSInspectionConfigurationStatus": ResourceStatusType,
         "Description": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "LastModifiedTime": datetime,
         "NumberOfAssociations": int,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
         "Certificates": List[TlsCertificateDataTypeDef],
     },
     total=False,
 )
 
 
 class TLSInspectionConfigurationResponseTypeDef(
@@ -1329,14 +1679,30 @@
     "CapacityUsageSummaryTypeDef",
     {
         "CIDRs": CIDRSummaryTypeDef,
     },
     total=False,
 )
 
+ActionDefinitionOutputTypeDef = TypedDict(
+    "ActionDefinitionOutputTypeDef",
+    {
+        "PublishMetricAction": PublishMetricActionOutputTypeDef,
+    },
+    total=False,
+)
+
+ActionDefinitionTypeDef = TypedDict(
+    "ActionDefinitionTypeDef",
+    {
+        "PublishMetricAction": PublishMetricActionTypeDef,
+    },
+    total=False,
+)
+
 CreateFirewallPolicyResponseTypeDef = TypedDict(
     "CreateFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1355,74 +1721,57 @@
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateRuleGroupResponseTypeDef = TypedDict(
-    "CreateRuleGroupResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteRuleGroupResponseTypeDef = TypedDict(
-    "DeleteRuleGroupResponseTypeDef",
-    {
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
+DescribeLoggingConfigurationResponseTypeDef = TypedDict(
+    "DescribeLoggingConfigurationResponseTypeDef",
     {
-        "UpdateToken": str,
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "FirewallArn": str,
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ActionDefinitionTypeDef = TypedDict(
-    "ActionDefinitionTypeDef",
-    {
-        "PublishMetricAction": PublishMetricActionTypeDef,
-    },
-    total=False,
-)
-
-DescribeLoggingConfigurationResponseTypeDef = TypedDict(
-    "DescribeLoggingConfigurationResponseTypeDef",
+UpdateLoggingConfigurationResponseTypeDef = TypedDict(
+    "UpdateLoggingConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "FirewallName": str,
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
     total=False,
 )
 
-UpdateLoggingConfigurationResponseTypeDef = TypedDict(
-    "UpdateLoggingConfigurationResponseTypeDef",
+ServerCertificateConfigurationOutputTypeDef = TypedDict(
+    "ServerCertificateConfigurationOutputTypeDef",
     {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ServerCertificates": List[ServerCertificateOutputTypeDef],
+        "Scopes": List[ServerCertificateScopeOutputTypeDef],
+    },
+    total=False,
+)
+
+RuleDefinitionOutputTypeDef = TypedDict(
+    "RuleDefinitionOutputTypeDef",
+    {
+        "MatchAttributes": MatchAttributesOutputTypeDef,
+        "Actions": List[str],
     },
 )
 
 ServerCertificateConfigurationTypeDef = TypedDict(
     "ServerCertificateConfigurationTypeDef",
     {
         "ServerCertificates": Sequence[ServerCertificateTypeDef],
@@ -1435,14 +1784,40 @@
     "RuleDefinitionTypeDef",
     {
         "MatchAttributes": MatchAttributesTypeDef,
         "Actions": Sequence[str],
     },
 )
 
+CreateRuleGroupResponseTypeDef = TypedDict(
+    "CreateRuleGroupResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteRuleGroupResponseTypeDef = TypedDict(
+    "DeleteRuleGroupResponseTypeDef",
+    {
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "CreateTLSInspectionConfigurationResponseTypeDef",
     {
         "UpdateToken": str,
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1482,22 +1857,46 @@
 )
 
 
 class FirewallStatusTypeDef(_RequiredFirewallStatusTypeDef, _OptionalFirewallStatusTypeDef):
     pass
 
 
+CustomActionOutputTypeDef = TypedDict(
+    "CustomActionOutputTypeDef",
+    {
+        "ActionName": str,
+        "ActionDefinition": ActionDefinitionOutputTypeDef,
+    },
+)
+
 CustomActionTypeDef = TypedDict(
     "CustomActionTypeDef",
     {
         "ActionName": str,
         "ActionDefinition": ActionDefinitionTypeDef,
     },
 )
 
+TLSInspectionConfigurationOutputTypeDef = TypedDict(
+    "TLSInspectionConfigurationOutputTypeDef",
+    {
+        "ServerCertificateConfigurations": List[ServerCertificateConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
+StatelessRuleOutputTypeDef = TypedDict(
+    "StatelessRuleOutputTypeDef",
+    {
+        "RuleDefinition": RuleDefinitionOutputTypeDef,
+        "Priority": int,
+    },
+)
+
 TLSInspectionConfigurationTypeDef = TypedDict(
     "TLSInspectionConfigurationTypeDef",
     {
         "ServerCertificateConfigurations": Sequence[ServerCertificateConfigurationTypeDef],
     },
     total=False,
 )
@@ -1534,14 +1933,42 @@
         "UpdateToken": str,
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredFirewallPolicyOutputTypeDef = TypedDict(
+    "_RequiredFirewallPolicyOutputTypeDef",
+    {
+        "StatelessDefaultActions": List[str],
+        "StatelessFragmentDefaultActions": List[str],
+    },
+)
+_OptionalFirewallPolicyOutputTypeDef = TypedDict(
+    "_OptionalFirewallPolicyOutputTypeDef",
+    {
+        "StatelessRuleGroupReferences": List[StatelessRuleGroupReferenceOutputTypeDef],
+        "StatelessCustomActions": List[CustomActionOutputTypeDef],
+        "StatefulRuleGroupReferences": List[StatefulRuleGroupReferenceOutputTypeDef],
+        "StatefulDefaultActions": List[str],
+        "StatefulEngineOptions": StatefulEngineOptionsOutputTypeDef,
+        "TLSInspectionConfigurationArn": str,
+        "PolicyVariables": PolicyVariablesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class FirewallPolicyOutputTypeDef(
+    _RequiredFirewallPolicyOutputTypeDef, _OptionalFirewallPolicyOutputTypeDef
+):
+    pass
+
+
 _RequiredFirewallPolicyTypeDef = TypedDict(
     "_RequiredFirewallPolicyTypeDef",
     {
         "StatelessDefaultActions": Sequence[str],
         "StatelessFragmentDefaultActions": Sequence[str],
     },
 )
@@ -1560,14 +1987,46 @@
 )
 
 
 class FirewallPolicyTypeDef(_RequiredFirewallPolicyTypeDef, _OptionalFirewallPolicyTypeDef):
     pass
 
 
+DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "DescribeTLSInspectionConfigurationResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "TLSInspectionConfiguration": TLSInspectionConfigurationOutputTypeDef,
+        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
+    "_RequiredStatelessRulesAndCustomActionsOutputTypeDef",
+    {
+        "StatelessRules": List[StatelessRuleOutputTypeDef],
+    },
+)
+_OptionalStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
+    "_OptionalStatelessRulesAndCustomActionsOutputTypeDef",
+    {
+        "CustomActions": List[CustomActionOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class StatelessRulesAndCustomActionsOutputTypeDef(
+    _RequiredStatelessRulesAndCustomActionsOutputTypeDef,
+    _OptionalStatelessRulesAndCustomActionsOutputTypeDef,
+):
+    pass
+
+
 _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfigurationName": str,
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
     },
 )
@@ -1585,24 +2044,14 @@
 class CreateTLSInspectionConfigurationRequestRequestTypeDef(
     _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef,
     _OptionalCreateTLSInspectionConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
-    "DescribeTLSInspectionConfigurationResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
-        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
         "UpdateToken": str,
     },
 )
@@ -1642,14 +2091,24 @@
 
 class StatelessRulesAndCustomActionsTypeDef(
     _RequiredStatelessRulesAndCustomActionsTypeDef, _OptionalStatelessRulesAndCustomActionsTypeDef
 ):
     pass
 
 
+DescribeFirewallPolicyResponseTypeDef = TypedDict(
+    "DescribeFirewallPolicyResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
+        "FirewallPolicy": FirewallPolicyOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallPolicyRequestRequestTypeDef",
     {
         "FirewallPolicyName": str,
         "FirewallPolicy": FirewallPolicyTypeDef,
     },
 )
@@ -1668,24 +2127,14 @@
 class CreateFirewallPolicyRequestRequestTypeDef(
     _RequiredCreateFirewallPolicyRequestRequestTypeDef,
     _OptionalCreateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeFirewallPolicyResponseTypeDef = TypedDict(
-    "DescribeFirewallPolicyResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "FirewallPolicy": FirewallPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicy": FirewallPolicyTypeDef,
     },
 )
@@ -1705,25 +2154,57 @@
 class UpdateFirewallPolicyRequestRequestTypeDef(
     _RequiredUpdateFirewallPolicyRequestRequestTypeDef,
     _OptionalUpdateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
 
+RulesSourceOutputTypeDef = TypedDict(
+    "RulesSourceOutputTypeDef",
+    {
+        "RulesString": str,
+        "RulesSourceList": RulesSourceListOutputTypeDef,
+        "StatefulRules": List[StatefulRuleOutputTypeDef],
+        "StatelessRulesAndCustomActions": StatelessRulesAndCustomActionsOutputTypeDef,
+    },
+    total=False,
+)
+
 RulesSourceTypeDef = TypedDict(
     "RulesSourceTypeDef",
     {
         "RulesString": str,
         "RulesSourceList": RulesSourceListTypeDef,
         "StatefulRules": Sequence[StatefulRuleTypeDef],
         "StatelessRulesAndCustomActions": StatelessRulesAndCustomActionsTypeDef,
     },
     total=False,
 )
 
+_RequiredRuleGroupOutputTypeDef = TypedDict(
+    "_RequiredRuleGroupOutputTypeDef",
+    {
+        "RulesSource": RulesSourceOutputTypeDef,
+    },
+)
+_OptionalRuleGroupOutputTypeDef = TypedDict(
+    "_OptionalRuleGroupOutputTypeDef",
+    {
+        "RuleVariables": RuleVariablesOutputTypeDef,
+        "ReferenceSets": ReferenceSetsOutputTypeDef,
+        "StatefulRuleOptions": StatefulRuleOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class RuleGroupOutputTypeDef(_RequiredRuleGroupOutputTypeDef, _OptionalRuleGroupOutputTypeDef):
+    pass
+
+
 _RequiredRuleGroupTypeDef = TypedDict(
     "_RequiredRuleGroupTypeDef",
     {
         "RulesSource": RulesSourceTypeDef,
     },
 )
 _OptionalRuleGroupTypeDef = TypedDict(
@@ -1737,14 +2218,24 @@
 )
 
 
 class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
     pass
 
 
+DescribeRuleGroupResponseTypeDef = TypedDict(
+    "DescribeRuleGroupResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "RuleGroup": RuleGroupOutputTypeDef,
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupName": str,
         "Type": RuleGroupTypeType,
         "Capacity": int,
     },
@@ -1766,24 +2257,14 @@
 
 class CreateRuleGroupRequestRequestTypeDef(
     _RequiredCreateRuleGroupRequestRequestTypeDef, _OptionalCreateRuleGroupRequestRequestTypeDef
 ):
     pass
 
 
-DescribeRuleGroupResponseTypeDef = TypedDict(
-    "DescribeRuleGroupResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "RuleGroup": RuleGroupTypeDef,
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "UpdateToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall/type_defs.pyi` & `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for network-firewall service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_network_firewall.type_defs import AddressTypeDef
+    from mypy_boto3_network_firewall.type_defs import AddressOutputTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -44,18 +44,20 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AddressOutputTypeDef",
     "AddressTypeDef",
     "AssociateFirewallPolicyRequestRequestTypeDef",
     "AssociateFirewallPolicyResponseTypeDef",
     "SubnetMappingTypeDef",
+    "SubnetMappingOutputTypeDef",
     "AttachmentTypeDef",
     "IPSetMetadataTypeDef",
     "EncryptionConfigurationTypeDef",
     "TagTypeDef",
     "SourceMetadataTypeDef",
     "DeleteFirewallPolicyRequestRequestTypeDef",
     "DeleteFirewallRequestRequestTypeDef",
@@ -64,49 +66,67 @@
     "DeleteTLSInspectionConfigurationRequestRequestTypeDef",
     "DescribeFirewallPolicyRequestRequestTypeDef",
     "DescribeFirewallRequestRequestTypeDef",
     "DescribeLoggingConfigurationRequestRequestTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
     "DescribeResourcePolicyResponseTypeDef",
     "DescribeRuleGroupMetadataRequestRequestTypeDef",
-    "StatefulRuleOptionsTypeDef",
+    "StatefulRuleOptionsOutputTypeDef",
     "DescribeRuleGroupRequestRequestTypeDef",
     "DescribeTLSInspectionConfigurationRequestRequestTypeDef",
+    "DimensionOutputTypeDef",
     "DimensionTypeDef",
     "DisassociateSubnetsRequestRequestTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
     "FirewallMetadataTypeDef",
     "FirewallPolicyMetadataTypeDef",
+    "StatefulEngineOptionsOutputTypeDef",
+    "StatelessRuleGroupReferenceOutputTypeDef",
+    "TagOutputTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupReferenceTypeDef",
+    "HeaderOutputTypeDef",
     "HeaderTypeDef",
+    "IPSetOutputTypeDef",
+    "IPSetReferenceOutputTypeDef",
     "IPSetReferenceTypeDef",
     "IPSetTypeDef",
     "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
     "ListFirewallPoliciesRequestRequestTypeDef",
     "ListFirewallsRequestListFirewallsPaginateTypeDef",
     "ListFirewallsRequestRequestTypeDef",
     "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupMetadataTypeDef",
     "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
     "ListTLSInspectionConfigurationsRequestRequestTypeDef",
     "TLSInspectionConfigurationMetadataTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "LogDestinationConfigOutputTypeDef",
     "LogDestinationConfigTypeDef",
+    "PortRangeOutputTypeDef",
+    "TCPFlagFieldOutputTypeDef",
     "PortRangeTypeDef",
     "TCPFlagFieldTypeDef",
     "PaginatorConfigTypeDef",
     "PerObjectStatusTypeDef",
+    "PortSetOutputTypeDef",
     "PortSetTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "SourceMetadataOutputTypeDef",
+    "StatefulRuleOptionsTypeDef",
+    "RuleOptionOutputTypeDef",
     "RuleOptionTypeDef",
+    "RulesSourceListOutputTypeDef",
     "RulesSourceListTypeDef",
+    "ServerCertificateOutputTypeDef",
     "ServerCertificateTypeDef",
+    "StatefulRuleGroupOverrideOutputTypeDef",
     "StatefulRuleGroupOverrideTypeDef",
     "TlsCertificateDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallDeleteProtectionRequestRequestTypeDef",
     "UpdateFirewallDeleteProtectionResponseTypeDef",
     "UpdateFirewallDescriptionRequestRequestTypeDef",
     "UpdateFirewallDescriptionResponseTypeDef",
@@ -115,75 +135,101 @@
     "UpdateSubnetChangeProtectionRequestRequestTypeDef",
     "UpdateSubnetChangeProtectionResponseTypeDef",
     "AssociateSubnetsRequestRequestTypeDef",
     "AssociateSubnetsResponseTypeDef",
     "DisassociateSubnetsResponseTypeDef",
     "CIDRSummaryTypeDef",
     "UpdateFirewallEncryptionConfigurationRequestRequestTypeDef",
-    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
     "CreateFirewallRequestRequestTypeDef",
-    "FirewallPolicyResponseTypeDef",
-    "FirewallTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "RuleGroupResponseTypeDef",
     "DescribeRuleGroupMetadataResponseTypeDef",
+    "PublishMetricActionOutputTypeDef",
     "PublishMetricActionTypeDef",
+    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
     "ListFirewallsResponseTypeDef",
     "ListFirewallPoliciesResponseTypeDef",
+    "FirewallPolicyResponseTypeDef",
+    "FirewallTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PolicyVariablesOutputTypeDef",
+    "ReferenceSetsOutputTypeDef",
     "ReferenceSetsTypeDef",
     "PolicyVariablesTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "ListTLSInspectionConfigurationsResponseTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
+    "ServerCertificateScopeOutputTypeDef",
+    "MatchAttributesOutputTypeDef",
     "ServerCertificateScopeTypeDef",
     "MatchAttributesTypeDef",
     "SyncStateTypeDef",
+    "RuleVariablesOutputTypeDef",
     "RuleVariablesTypeDef",
+    "RuleGroupResponseTypeDef",
+    "StatefulRuleOutputTypeDef",
     "StatefulRuleTypeDef",
+    "StatefulRuleGroupReferenceOutputTypeDef",
     "StatefulRuleGroupReferenceTypeDef",
     "TLSInspectionConfigurationResponseTypeDef",
     "CapacityUsageSummaryTypeDef",
+    "ActionDefinitionOutputTypeDef",
+    "ActionDefinitionTypeDef",
     "CreateFirewallPolicyResponseTypeDef",
     "DeleteFirewallPolicyResponseTypeDef",
     "UpdateFirewallPolicyResponseTypeDef",
-    "CreateRuleGroupResponseTypeDef",
-    "DeleteRuleGroupResponseTypeDef",
-    "UpdateRuleGroupResponseTypeDef",
-    "ActionDefinitionTypeDef",
     "DescribeLoggingConfigurationResponseTypeDef",
-    "UpdateLoggingConfigurationRequestRequestTypeDef",
     "UpdateLoggingConfigurationResponseTypeDef",
+    "UpdateLoggingConfigurationRequestRequestTypeDef",
+    "ServerCertificateConfigurationOutputTypeDef",
+    "RuleDefinitionOutputTypeDef",
     "ServerCertificateConfigurationTypeDef",
     "RuleDefinitionTypeDef",
+    "CreateRuleGroupResponseTypeDef",
+    "DeleteRuleGroupResponseTypeDef",
+    "UpdateRuleGroupResponseTypeDef",
     "CreateTLSInspectionConfigurationResponseTypeDef",
     "DeleteTLSInspectionConfigurationResponseTypeDef",
     "UpdateTLSInspectionConfigurationResponseTypeDef",
     "FirewallStatusTypeDef",
+    "CustomActionOutputTypeDef",
     "CustomActionTypeDef",
+    "TLSInspectionConfigurationOutputTypeDef",
+    "StatelessRuleOutputTypeDef",
     "TLSInspectionConfigurationTypeDef",
     "StatelessRuleTypeDef",
     "CreateFirewallResponseTypeDef",
     "DeleteFirewallResponseTypeDef",
     "DescribeFirewallResponseTypeDef",
+    "FirewallPolicyOutputTypeDef",
     "FirewallPolicyTypeDef",
-    "CreateTLSInspectionConfigurationRequestRequestTypeDef",
     "DescribeTLSInspectionConfigurationResponseTypeDef",
+    "StatelessRulesAndCustomActionsOutputTypeDef",
+    "CreateTLSInspectionConfigurationRequestRequestTypeDef",
     "UpdateTLSInspectionConfigurationRequestRequestTypeDef",
     "StatelessRulesAndCustomActionsTypeDef",
-    "CreateFirewallPolicyRequestRequestTypeDef",
     "DescribeFirewallPolicyResponseTypeDef",
+    "CreateFirewallPolicyRequestRequestTypeDef",
     "UpdateFirewallPolicyRequestRequestTypeDef",
+    "RulesSourceOutputTypeDef",
     "RulesSourceTypeDef",
+    "RuleGroupOutputTypeDef",
     "RuleGroupTypeDef",
-    "CreateRuleGroupRequestRequestTypeDef",
     "DescribeRuleGroupResponseTypeDef",
+    "CreateRuleGroupRequestRequestTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
 )
 
+AddressOutputTypeDef = TypedDict(
+    "AddressOutputTypeDef",
+    {
+        "AddressDefinition": str,
+    },
+)
+
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressDefinition": str,
     },
 )
 
@@ -233,14 +279,33 @@
     },
     total=False,
 )
 
 class SubnetMappingTypeDef(_RequiredSubnetMappingTypeDef, _OptionalSubnetMappingTypeDef):
     pass
 
+_RequiredSubnetMappingOutputTypeDef = TypedDict(
+    "_RequiredSubnetMappingOutputTypeDef",
+    {
+        "SubnetId": str,
+    },
+)
+_OptionalSubnetMappingOutputTypeDef = TypedDict(
+    "_OptionalSubnetMappingOutputTypeDef",
+    {
+        "IPAddressType": IPAddressTypeType,
+    },
+    total=False,
+)
+
+class SubnetMappingOutputTypeDef(
+    _RequiredSubnetMappingOutputTypeDef, _OptionalSubnetMappingOutputTypeDef
+):
+    pass
+
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "SubnetId": str,
         "EndpointId": str,
         "Status": AttachmentStatusType,
         "StatusMessage": str,
@@ -384,16 +449,16 @@
         "RuleGroupName": str,
         "RuleGroupArn": str,
         "Type": RuleGroupTypeType,
     },
     total=False,
 )
 
-StatefulRuleOptionsTypeDef = TypedDict(
-    "StatefulRuleOptionsTypeDef",
+StatefulRuleOptionsOutputTypeDef = TypedDict(
+    "StatefulRuleOptionsOutputTypeDef",
     {
         "RuleOrder": RuleOrderType,
     },
     total=False,
 )
 
 DescribeRuleGroupRequestRequestTypeDef = TypedDict(
@@ -411,14 +476,21 @@
     {
         "TLSInspectionConfigurationArn": str,
         "TLSInspectionConfigurationName": str,
     },
     total=False,
 )
 
+DimensionOutputTypeDef = TypedDict(
+    "DimensionOutputTypeDef",
+    {
+        "Value": str,
+    },
+)
+
 DimensionTypeDef = TypedDict(
     "DimensionTypeDef",
     {
         "Value": str,
     },
 )
 
@@ -440,14 +512,33 @@
 
 class DisassociateSubnetsRequestRequestTypeDef(
     _RequiredDisassociateSubnetsRequestRequestTypeDef,
     _OptionalDisassociateSubnetsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredEncryptionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEncryptionConfigurationOutputTypeDef",
+    {
+        "Type": EncryptionTypeType,
+    },
+)
+_OptionalEncryptionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEncryptionConfigurationOutputTypeDef",
+    {
+        "KeyId": str,
+    },
+    total=False,
+)
+
+class EncryptionConfigurationOutputTypeDef(
+    _RequiredEncryptionConfigurationOutputTypeDef, _OptionalEncryptionConfigurationOutputTypeDef
+):
+    pass
+
 FirewallMetadataTypeDef = TypedDict(
     "FirewallMetadataTypeDef",
     {
         "FirewallName": str,
         "FirewallArn": str,
     },
     total=False,
@@ -458,14 +549,39 @@
     {
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
+StatefulEngineOptionsOutputTypeDef = TypedDict(
+    "StatefulEngineOptionsOutputTypeDef",
+    {
+        "RuleOrder": RuleOrderType,
+        "StreamExceptionPolicy": StreamExceptionPolicyType,
+    },
+    total=False,
+)
+
+StatelessRuleGroupReferenceOutputTypeDef = TypedDict(
+    "StatelessRuleGroupReferenceOutputTypeDef",
+    {
+        "ResourceArn": str,
+        "Priority": int,
+    },
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 StatefulEngineOptionsTypeDef = TypedDict(
     "StatefulEngineOptionsTypeDef",
     {
         "RuleOrder": RuleOrderType,
         "StreamExceptionPolicy": StreamExceptionPolicyType,
     },
     total=False,
@@ -475,26 +591,53 @@
     "StatelessRuleGroupReferenceTypeDef",
     {
         "ResourceArn": str,
         "Priority": int,
     },
 )
 
+HeaderOutputTypeDef = TypedDict(
+    "HeaderOutputTypeDef",
+    {
+        "Protocol": StatefulRuleProtocolType,
+        "Source": str,
+        "SourcePort": str,
+        "Direction": StatefulRuleDirectionType,
+        "Destination": str,
+        "DestinationPort": str,
+    },
+)
+
 HeaderTypeDef = TypedDict(
     "HeaderTypeDef",
     {
         "Protocol": StatefulRuleProtocolType,
         "Source": str,
         "SourcePort": str,
         "Direction": StatefulRuleDirectionType,
         "Destination": str,
         "DestinationPort": str,
     },
 )
 
+IPSetOutputTypeDef = TypedDict(
+    "IPSetOutputTypeDef",
+    {
+        "Definition": List[str],
+    },
+)
+
+IPSetReferenceOutputTypeDef = TypedDict(
+    "IPSetReferenceOutputTypeDef",
+    {
+        "ReferenceArn": str,
+    },
+    total=False,
+)
+
 IPSetReferenceTypeDef = TypedDict(
     "IPSetReferenceTypeDef",
     {
         "ReferenceArn": str,
     },
     total=False,
 )
@@ -637,22 +780,58 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+LogDestinationConfigOutputTypeDef = TypedDict(
+    "LogDestinationConfigOutputTypeDef",
+    {
+        "LogType": LogTypeType,
+        "LogDestinationType": LogDestinationTypeType,
+        "LogDestination": Dict[str, str],
+    },
+)
+
 LogDestinationConfigTypeDef = TypedDict(
     "LogDestinationConfigTypeDef",
     {
         "LogType": LogTypeType,
         "LogDestinationType": LogDestinationTypeType,
-        "LogDestination": Dict[str, str],
+        "LogDestination": Mapping[str, str],
+    },
+)
+
+PortRangeOutputTypeDef = TypedDict(
+    "PortRangeOutputTypeDef",
+    {
+        "FromPort": int,
+        "ToPort": int,
+    },
+)
+
+_RequiredTCPFlagFieldOutputTypeDef = TypedDict(
+    "_RequiredTCPFlagFieldOutputTypeDef",
+    {
+        "Flags": List[TCPFlagType],
     },
 )
+_OptionalTCPFlagFieldOutputTypeDef = TypedDict(
+    "_OptionalTCPFlagFieldOutputTypeDef",
+    {
+        "Masks": List[TCPFlagType],
+    },
+    total=False,
+)
+
+class TCPFlagFieldOutputTypeDef(
+    _RequiredTCPFlagFieldOutputTypeDef, _OptionalTCPFlagFieldOutputTypeDef
+):
+    pass
 
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
@@ -690,14 +869,22 @@
     {
         "SyncStatus": PerObjectSyncStatusType,
         "UpdateToken": str,
     },
     total=False,
 )
 
+PortSetOutputTypeDef = TypedDict(
+    "PortSetOutputTypeDef",
+    {
+        "Definition": List[str],
+    },
+    total=False,
+)
+
 PortSetTypeDef = TypedDict(
     "PortSetTypeDef",
     {
         "Definition": Sequence[str],
     },
     total=False,
 )
@@ -717,14 +904,48 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+SourceMetadataOutputTypeDef = TypedDict(
+    "SourceMetadataOutputTypeDef",
+    {
+        "SourceArn": str,
+        "SourceUpdateToken": str,
+    },
+    total=False,
+)
+
+StatefulRuleOptionsTypeDef = TypedDict(
+    "StatefulRuleOptionsTypeDef",
+    {
+        "RuleOrder": RuleOrderType,
+    },
+    total=False,
+)
+
+_RequiredRuleOptionOutputTypeDef = TypedDict(
+    "_RequiredRuleOptionOutputTypeDef",
+    {
+        "Keyword": str,
+    },
+)
+_OptionalRuleOptionOutputTypeDef = TypedDict(
+    "_OptionalRuleOptionOutputTypeDef",
+    {
+        "Settings": List[str],
+    },
+    total=False,
+)
+
+class RuleOptionOutputTypeDef(_RequiredRuleOptionOutputTypeDef, _OptionalRuleOptionOutputTypeDef):
+    pass
+
 _RequiredRuleOptionTypeDef = TypedDict(
     "_RequiredRuleOptionTypeDef",
     {
         "Keyword": str,
     },
 )
 _OptionalRuleOptionTypeDef = TypedDict(
@@ -734,31 +955,56 @@
     },
     total=False,
 )
 
 class RuleOptionTypeDef(_RequiredRuleOptionTypeDef, _OptionalRuleOptionTypeDef):
     pass
 
+RulesSourceListOutputTypeDef = TypedDict(
+    "RulesSourceListOutputTypeDef",
+    {
+        "Targets": List[str],
+        "TargetTypes": List[TargetTypeType],
+        "GeneratedRulesType": GeneratedRulesTypeType,
+    },
+)
+
 RulesSourceListTypeDef = TypedDict(
     "RulesSourceListTypeDef",
     {
         "Targets": Sequence[str],
         "TargetTypes": Sequence[TargetTypeType],
         "GeneratedRulesType": GeneratedRulesTypeType,
     },
 )
 
+ServerCertificateOutputTypeDef = TypedDict(
+    "ServerCertificateOutputTypeDef",
+    {
+        "ResourceArn": str,
+    },
+    total=False,
+)
+
 ServerCertificateTypeDef = TypedDict(
     "ServerCertificateTypeDef",
     {
         "ResourceArn": str,
     },
     total=False,
 )
 
+StatefulRuleGroupOverrideOutputTypeDef = TypedDict(
+    "StatefulRuleGroupOverrideOutputTypeDef",
+    {
+        "Action": Literal["DROP_TO_ALERT"],
+    },
+    total=False,
+)
+
 StatefulRuleGroupOverrideTypeDef = TypedDict(
     "StatefulRuleGroupOverrideTypeDef",
     {
         "Action": Literal["DROP_TO_ALERT"],
     },
     total=False,
 )
@@ -925,26 +1171,26 @@
     pass
 
 AssociateSubnetsResponseTypeDef = TypedDict(
     "AssociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
-        "SubnetMappings": List[SubnetMappingTypeDef],
+        "SubnetMappings": List[SubnetMappingOutputTypeDef],
         "UpdateToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateSubnetsResponseTypeDef = TypedDict(
     "DisassociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
-        "SubnetMappings": List[SubnetMappingTypeDef],
+        "SubnetMappings": List[SubnetMappingOutputTypeDef],
         "UpdateToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CIDRSummaryTypeDef = TypedDict(
     "CIDRSummaryTypeDef",
@@ -963,25 +1209,14 @@
         "FirewallArn": str,
         "FirewallName": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
-UpdateFirewallEncryptionConfigurationResponseTypeDef = TypedDict(
-    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "UpdateToken": str,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFirewallRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallRequestRequestTypeDef",
     {
         "FirewallName": str,
         "FirewallPolicyArn": str,
         "VpcId": str,
         "SubnetMappings": Sequence[SubnetMappingTypeDef],
@@ -1001,32 +1236,97 @@
 )
 
 class CreateFirewallRequestRequestTypeDef(
     _RequiredCreateFirewallRequestRequestTypeDef, _OptionalCreateFirewallRequestRequestTypeDef
 ):
     pass
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+DescribeRuleGroupMetadataResponseTypeDef = TypedDict(
+    "DescribeRuleGroupMetadataResponseTypeDef",
+    {
+        "RuleGroupArn": str,
+        "RuleGroupName": str,
+        "Description": str,
+        "Type": RuleGroupTypeType,
+        "Capacity": int,
+        "StatefulRuleOptions": StatefulRuleOptionsOutputTypeDef,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PublishMetricActionOutputTypeDef = TypedDict(
+    "PublishMetricActionOutputTypeDef",
+    {
+        "Dimensions": List[DimensionOutputTypeDef],
+    },
+)
+
+PublishMetricActionTypeDef = TypedDict(
+    "PublishMetricActionTypeDef",
+    {
+        "Dimensions": Sequence[DimensionTypeDef],
+    },
+)
+
+UpdateFirewallEncryptionConfigurationResponseTypeDef = TypedDict(
+    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "UpdateToken": str,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListFirewallsResponseTypeDef = TypedDict(
+    "ListFirewallsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Firewalls": List[FirewallMetadataTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListFirewallPoliciesResponseTypeDef = TypedDict(
+    "ListFirewallPoliciesResponseTypeDef",
+    {
+        "NextToken": str,
+        "FirewallPolicies": List[FirewallPolicyMetadataTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFirewallPolicyResponseTypeDef = TypedDict(
     "_RequiredFirewallPolicyResponseTypeDef",
     {
         "FirewallPolicyName": str,
         "FirewallPolicyArn": str,
         "FirewallPolicyId": str,
     },
 )
 _OptionalFirewallPolicyResponseTypeDef = TypedDict(
     "_OptionalFirewallPolicyResponseTypeDef",
     {
         "Description": str,
         "FirewallPolicyStatus": ResourceStatusType,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ConsumedStatelessRuleCapacity": int,
         "ConsumedStatefulRuleCapacity": int,
         "NumberOfAssociations": int,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
 class FirewallPolicyResponseTypeDef(
     _RequiredFirewallPolicyResponseTypeDef, _OptionalFirewallPolicyResponseTypeDef
@@ -1034,121 +1334,59 @@
     pass
 
 _RequiredFirewallTypeDef = TypedDict(
     "_RequiredFirewallTypeDef",
     {
         "FirewallPolicyArn": str,
         "VpcId": str,
-        "SubnetMappings": List[SubnetMappingTypeDef],
+        "SubnetMappings": List[SubnetMappingOutputTypeDef],
         "FirewallId": str,
     },
 )
 _OptionalFirewallTypeDef = TypedDict(
     "_OptionalFirewallTypeDef",
     {
         "FirewallName": str,
         "FirewallArn": str,
         "DeleteProtection": bool,
         "SubnetChangeProtection": bool,
         "FirewallPolicyChangeProtection": bool,
         "Description": str,
-        "Tags": List[TagTypeDef],
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 class FirewallTypeDef(_RequiredFirewallTypeDef, _OptionalFirewallTypeDef):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "NextToken": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+PolicyVariablesOutputTypeDef = TypedDict(
+    "PolicyVariablesOutputTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-_RequiredRuleGroupResponseTypeDef = TypedDict(
-    "_RequiredRuleGroupResponseTypeDef",
-    {
-        "RuleGroupArn": str,
-        "RuleGroupName": str,
-        "RuleGroupId": str,
-    },
-)
-_OptionalRuleGroupResponseTypeDef = TypedDict(
-    "_OptionalRuleGroupResponseTypeDef",
-    {
-        "Description": str,
-        "Type": RuleGroupTypeType,
-        "Capacity": int,
-        "RuleGroupStatus": ResourceStatusType,
-        "Tags": List[TagTypeDef],
-        "ConsumedCapacity": int,
-        "NumberOfAssociations": int,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-        "SourceMetadata": SourceMetadataTypeDef,
-        "SnsTopic": str,
-        "LastModifiedTime": datetime,
+        "RuleVariables": Dict[str, IPSetOutputTypeDef],
     },
     total=False,
 )
 
-class RuleGroupResponseTypeDef(
-    _RequiredRuleGroupResponseTypeDef, _OptionalRuleGroupResponseTypeDef
-):
-    pass
-
-DescribeRuleGroupMetadataResponseTypeDef = TypedDict(
-    "DescribeRuleGroupMetadataResponseTypeDef",
+ReferenceSetsOutputTypeDef = TypedDict(
+    "ReferenceSetsOutputTypeDef",
     {
-        "RuleGroupArn": str,
-        "RuleGroupName": str,
-        "Description": str,
-        "Type": RuleGroupTypeType,
-        "Capacity": int,
-        "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PublishMetricActionTypeDef = TypedDict(
-    "PublishMetricActionTypeDef",
-    {
-        "Dimensions": Sequence[DimensionTypeDef],
-    },
-)
-
-ListFirewallsResponseTypeDef = TypedDict(
-    "ListFirewallsResponseTypeDef",
-    {
-        "NextToken": str,
-        "Firewalls": List[FirewallMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFirewallPoliciesResponseTypeDef = TypedDict(
-    "ListFirewallPoliciesResponseTypeDef",
-    {
-        "NextToken": str,
-        "FirewallPolicies": List[FirewallPolicyMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "IPSetReferences": Dict[str, IPSetReferenceOutputTypeDef],
     },
+    total=False,
 )
 
 ReferenceSetsTypeDef = TypedDict(
     "ReferenceSetsTypeDef",
     {
         "IPSetReferences": Mapping[str, IPSetReferenceTypeDef],
     },
@@ -1177,21 +1415,53 @@
     {
         "NextToken": str,
         "TLSInspectionConfigurations": List[TLSInspectionConfigurationMetadataTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LoggingConfigurationOutputTypeDef = TypedDict(
+    "LoggingConfigurationOutputTypeDef",
+    {
+        "LogDestinationConfigs": List[LogDestinationConfigOutputTypeDef],
+    },
+)
+
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
-        "LogDestinationConfigs": List[LogDestinationConfigTypeDef],
+        "LogDestinationConfigs": Sequence[LogDestinationConfigTypeDef],
     },
 )
 
+ServerCertificateScopeOutputTypeDef = TypedDict(
+    "ServerCertificateScopeOutputTypeDef",
+    {
+        "Sources": List[AddressOutputTypeDef],
+        "Destinations": List[AddressOutputTypeDef],
+        "SourcePorts": List[PortRangeOutputTypeDef],
+        "DestinationPorts": List[PortRangeOutputTypeDef],
+        "Protocols": List[int],
+    },
+    total=False,
+)
+
+MatchAttributesOutputTypeDef = TypedDict(
+    "MatchAttributesOutputTypeDef",
+    {
+        "Sources": List[AddressOutputTypeDef],
+        "Destinations": List[AddressOutputTypeDef],
+        "SourcePorts": List[PortRangeOutputTypeDef],
+        "DestinationPorts": List[PortRangeOutputTypeDef],
+        "Protocols": List[int],
+        "TCPFlags": List[TCPFlagFieldOutputTypeDef],
+    },
+    total=False,
+)
+
 ServerCertificateScopeTypeDef = TypedDict(
     "ServerCertificateScopeTypeDef",
     {
         "Sources": Sequence[AddressTypeDef],
         "Destinations": Sequence[AddressTypeDef],
         "SourcePorts": Sequence[PortRangeTypeDef],
         "DestinationPorts": Sequence[PortRangeTypeDef],
@@ -1218,32 +1488,102 @@
     {
         "Attachment": AttachmentTypeDef,
         "Config": Dict[str, PerObjectStatusTypeDef],
     },
     total=False,
 )
 
+RuleVariablesOutputTypeDef = TypedDict(
+    "RuleVariablesOutputTypeDef",
+    {
+        "IPSets": Dict[str, IPSetOutputTypeDef],
+        "PortSets": Dict[str, PortSetOutputTypeDef],
+    },
+    total=False,
+)
+
 RuleVariablesTypeDef = TypedDict(
     "RuleVariablesTypeDef",
     {
         "IPSets": Mapping[str, IPSetTypeDef],
         "PortSets": Mapping[str, PortSetTypeDef],
     },
     total=False,
 )
 
+_RequiredRuleGroupResponseTypeDef = TypedDict(
+    "_RequiredRuleGroupResponseTypeDef",
+    {
+        "RuleGroupArn": str,
+        "RuleGroupName": str,
+        "RuleGroupId": str,
+    },
+)
+_OptionalRuleGroupResponseTypeDef = TypedDict(
+    "_OptionalRuleGroupResponseTypeDef",
+    {
+        "Description": str,
+        "Type": RuleGroupTypeType,
+        "Capacity": int,
+        "RuleGroupStatus": ResourceStatusType,
+        "Tags": List[TagOutputTypeDef],
+        "ConsumedCapacity": int,
+        "NumberOfAssociations": int,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "SourceMetadata": SourceMetadataOutputTypeDef,
+        "SnsTopic": str,
+        "LastModifiedTime": datetime,
+    },
+    total=False,
+)
+
+class RuleGroupResponseTypeDef(
+    _RequiredRuleGroupResponseTypeDef, _OptionalRuleGroupResponseTypeDef
+):
+    pass
+
+StatefulRuleOutputTypeDef = TypedDict(
+    "StatefulRuleOutputTypeDef",
+    {
+        "Action": StatefulActionType,
+        "Header": HeaderOutputTypeDef,
+        "RuleOptions": List[RuleOptionOutputTypeDef],
+    },
+)
+
 StatefulRuleTypeDef = TypedDict(
     "StatefulRuleTypeDef",
     {
         "Action": StatefulActionType,
         "Header": HeaderTypeDef,
         "RuleOptions": Sequence[RuleOptionTypeDef],
     },
 )
 
+_RequiredStatefulRuleGroupReferenceOutputTypeDef = TypedDict(
+    "_RequiredStatefulRuleGroupReferenceOutputTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalStatefulRuleGroupReferenceOutputTypeDef = TypedDict(
+    "_OptionalStatefulRuleGroupReferenceOutputTypeDef",
+    {
+        "Priority": int,
+        "Override": StatefulRuleGroupOverrideOutputTypeDef,
+    },
+    total=False,
+)
+
+class StatefulRuleGroupReferenceOutputTypeDef(
+    _RequiredStatefulRuleGroupReferenceOutputTypeDef,
+    _OptionalStatefulRuleGroupReferenceOutputTypeDef,
+):
+    pass
+
 _RequiredStatefulRuleGroupReferenceTypeDef = TypedDict(
     "_RequiredStatefulRuleGroupReferenceTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalStatefulRuleGroupReferenceTypeDef = TypedDict(
@@ -1269,18 +1609,18 @@
     },
 )
 _OptionalTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "_OptionalTLSInspectionConfigurationResponseTypeDef",
     {
         "TLSInspectionConfigurationStatus": ResourceStatusType,
         "Description": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "LastModifiedTime": datetime,
         "NumberOfAssociations": int,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
         "Certificates": List[TlsCertificateDataTypeDef],
     },
     total=False,
 )
 
 class TLSInspectionConfigurationResponseTypeDef(
     _RequiredTLSInspectionConfigurationResponseTypeDef,
@@ -1292,14 +1632,30 @@
     "CapacityUsageSummaryTypeDef",
     {
         "CIDRs": CIDRSummaryTypeDef,
     },
     total=False,
 )
 
+ActionDefinitionOutputTypeDef = TypedDict(
+    "ActionDefinitionOutputTypeDef",
+    {
+        "PublishMetricAction": PublishMetricActionOutputTypeDef,
+    },
+    total=False,
+)
+
+ActionDefinitionTypeDef = TypedDict(
+    "ActionDefinitionTypeDef",
+    {
+        "PublishMetricAction": PublishMetricActionTypeDef,
+    },
+    total=False,
+)
+
 CreateFirewallPolicyResponseTypeDef = TypedDict(
     "CreateFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1318,74 +1674,57 @@
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateRuleGroupResponseTypeDef = TypedDict(
-    "CreateRuleGroupResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteRuleGroupResponseTypeDef = TypedDict(
-    "DeleteRuleGroupResponseTypeDef",
-    {
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
+DescribeLoggingConfigurationResponseTypeDef = TypedDict(
+    "DescribeLoggingConfigurationResponseTypeDef",
     {
-        "UpdateToken": str,
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "FirewallArn": str,
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ActionDefinitionTypeDef = TypedDict(
-    "ActionDefinitionTypeDef",
-    {
-        "PublishMetricAction": PublishMetricActionTypeDef,
-    },
-    total=False,
-)
-
-DescribeLoggingConfigurationResponseTypeDef = TypedDict(
-    "DescribeLoggingConfigurationResponseTypeDef",
+UpdateLoggingConfigurationResponseTypeDef = TypedDict(
+    "UpdateLoggingConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "FirewallName": str,
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
     total=False,
 )
 
-UpdateLoggingConfigurationResponseTypeDef = TypedDict(
-    "UpdateLoggingConfigurationResponseTypeDef",
+ServerCertificateConfigurationOutputTypeDef = TypedDict(
+    "ServerCertificateConfigurationOutputTypeDef",
     {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ServerCertificates": List[ServerCertificateOutputTypeDef],
+        "Scopes": List[ServerCertificateScopeOutputTypeDef],
+    },
+    total=False,
+)
+
+RuleDefinitionOutputTypeDef = TypedDict(
+    "RuleDefinitionOutputTypeDef",
+    {
+        "MatchAttributes": MatchAttributesOutputTypeDef,
+        "Actions": List[str],
     },
 )
 
 ServerCertificateConfigurationTypeDef = TypedDict(
     "ServerCertificateConfigurationTypeDef",
     {
         "ServerCertificates": Sequence[ServerCertificateTypeDef],
@@ -1398,14 +1737,40 @@
     "RuleDefinitionTypeDef",
     {
         "MatchAttributes": MatchAttributesTypeDef,
         "Actions": Sequence[str],
     },
 )
 
+CreateRuleGroupResponseTypeDef = TypedDict(
+    "CreateRuleGroupResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteRuleGroupResponseTypeDef = TypedDict(
+    "DeleteRuleGroupResponseTypeDef",
+    {
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "CreateTLSInspectionConfigurationResponseTypeDef",
     {
         "UpdateToken": str,
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1443,22 +1808,46 @@
     },
     total=False,
 )
 
 class FirewallStatusTypeDef(_RequiredFirewallStatusTypeDef, _OptionalFirewallStatusTypeDef):
     pass
 
+CustomActionOutputTypeDef = TypedDict(
+    "CustomActionOutputTypeDef",
+    {
+        "ActionName": str,
+        "ActionDefinition": ActionDefinitionOutputTypeDef,
+    },
+)
+
 CustomActionTypeDef = TypedDict(
     "CustomActionTypeDef",
     {
         "ActionName": str,
         "ActionDefinition": ActionDefinitionTypeDef,
     },
 )
 
+TLSInspectionConfigurationOutputTypeDef = TypedDict(
+    "TLSInspectionConfigurationOutputTypeDef",
+    {
+        "ServerCertificateConfigurations": List[ServerCertificateConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
+StatelessRuleOutputTypeDef = TypedDict(
+    "StatelessRuleOutputTypeDef",
+    {
+        "RuleDefinition": RuleDefinitionOutputTypeDef,
+        "Priority": int,
+    },
+)
+
 TLSInspectionConfigurationTypeDef = TypedDict(
     "TLSInspectionConfigurationTypeDef",
     {
         "ServerCertificateConfigurations": Sequence[ServerCertificateConfigurationTypeDef],
     },
     total=False,
 )
@@ -1495,14 +1884,40 @@
         "UpdateToken": str,
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredFirewallPolicyOutputTypeDef = TypedDict(
+    "_RequiredFirewallPolicyOutputTypeDef",
+    {
+        "StatelessDefaultActions": List[str],
+        "StatelessFragmentDefaultActions": List[str],
+    },
+)
+_OptionalFirewallPolicyOutputTypeDef = TypedDict(
+    "_OptionalFirewallPolicyOutputTypeDef",
+    {
+        "StatelessRuleGroupReferences": List[StatelessRuleGroupReferenceOutputTypeDef],
+        "StatelessCustomActions": List[CustomActionOutputTypeDef],
+        "StatefulRuleGroupReferences": List[StatefulRuleGroupReferenceOutputTypeDef],
+        "StatefulDefaultActions": List[str],
+        "StatefulEngineOptions": StatefulEngineOptionsOutputTypeDef,
+        "TLSInspectionConfigurationArn": str,
+        "PolicyVariables": PolicyVariablesOutputTypeDef,
+    },
+    total=False,
+)
+
+class FirewallPolicyOutputTypeDef(
+    _RequiredFirewallPolicyOutputTypeDef, _OptionalFirewallPolicyOutputTypeDef
+):
+    pass
+
 _RequiredFirewallPolicyTypeDef = TypedDict(
     "_RequiredFirewallPolicyTypeDef",
     {
         "StatelessDefaultActions": Sequence[str],
         "StatelessFragmentDefaultActions": Sequence[str],
     },
 )
@@ -1519,14 +1934,44 @@
     },
     total=False,
 )
 
 class FirewallPolicyTypeDef(_RequiredFirewallPolicyTypeDef, _OptionalFirewallPolicyTypeDef):
     pass
 
+DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
+    "DescribeTLSInspectionConfigurationResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "TLSInspectionConfiguration": TLSInspectionConfigurationOutputTypeDef,
+        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
+    "_RequiredStatelessRulesAndCustomActionsOutputTypeDef",
+    {
+        "StatelessRules": List[StatelessRuleOutputTypeDef],
+    },
+)
+_OptionalStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
+    "_OptionalStatelessRulesAndCustomActionsOutputTypeDef",
+    {
+        "CustomActions": List[CustomActionOutputTypeDef],
+    },
+    total=False,
+)
+
+class StatelessRulesAndCustomActionsOutputTypeDef(
+    _RequiredStatelessRulesAndCustomActionsOutputTypeDef,
+    _OptionalStatelessRulesAndCustomActionsOutputTypeDef,
+):
+    pass
+
 _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfigurationName": str,
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
     },
 )
@@ -1542,24 +1987,14 @@
 
 class CreateTLSInspectionConfigurationRequestRequestTypeDef(
     _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef,
     _OptionalCreateTLSInspectionConfigurationRequestRequestTypeDef,
 ):
     pass
 
-DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
-    "DescribeTLSInspectionConfigurationResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
-        "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
         "UpdateToken": str,
     },
 )
@@ -1595,14 +2030,24 @@
 )
 
 class StatelessRulesAndCustomActionsTypeDef(
     _RequiredStatelessRulesAndCustomActionsTypeDef, _OptionalStatelessRulesAndCustomActionsTypeDef
 ):
     pass
 
+DescribeFirewallPolicyResponseTypeDef = TypedDict(
+    "DescribeFirewallPolicyResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
+        "FirewallPolicy": FirewallPolicyOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallPolicyRequestRequestTypeDef",
     {
         "FirewallPolicyName": str,
         "FirewallPolicy": FirewallPolicyTypeDef,
     },
 )
@@ -1619,24 +2064,14 @@
 
 class CreateFirewallPolicyRequestRequestTypeDef(
     _RequiredCreateFirewallPolicyRequestRequestTypeDef,
     _OptionalCreateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
-DescribeFirewallPolicyResponseTypeDef = TypedDict(
-    "DescribeFirewallPolicyResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "FirewallPolicy": FirewallPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicy": FirewallPolicyTypeDef,
     },
 )
@@ -1654,25 +2089,55 @@
 
 class UpdateFirewallPolicyRequestRequestTypeDef(
     _RequiredUpdateFirewallPolicyRequestRequestTypeDef,
     _OptionalUpdateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
+RulesSourceOutputTypeDef = TypedDict(
+    "RulesSourceOutputTypeDef",
+    {
+        "RulesString": str,
+        "RulesSourceList": RulesSourceListOutputTypeDef,
+        "StatefulRules": List[StatefulRuleOutputTypeDef],
+        "StatelessRulesAndCustomActions": StatelessRulesAndCustomActionsOutputTypeDef,
+    },
+    total=False,
+)
+
 RulesSourceTypeDef = TypedDict(
     "RulesSourceTypeDef",
     {
         "RulesString": str,
         "RulesSourceList": RulesSourceListTypeDef,
         "StatefulRules": Sequence[StatefulRuleTypeDef],
         "StatelessRulesAndCustomActions": StatelessRulesAndCustomActionsTypeDef,
     },
     total=False,
 )
 
+_RequiredRuleGroupOutputTypeDef = TypedDict(
+    "_RequiredRuleGroupOutputTypeDef",
+    {
+        "RulesSource": RulesSourceOutputTypeDef,
+    },
+)
+_OptionalRuleGroupOutputTypeDef = TypedDict(
+    "_OptionalRuleGroupOutputTypeDef",
+    {
+        "RuleVariables": RuleVariablesOutputTypeDef,
+        "ReferenceSets": ReferenceSetsOutputTypeDef,
+        "StatefulRuleOptions": StatefulRuleOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+class RuleGroupOutputTypeDef(_RequiredRuleGroupOutputTypeDef, _OptionalRuleGroupOutputTypeDef):
+    pass
+
 _RequiredRuleGroupTypeDef = TypedDict(
     "_RequiredRuleGroupTypeDef",
     {
         "RulesSource": RulesSourceTypeDef,
     },
 )
 _OptionalRuleGroupTypeDef = TypedDict(
@@ -1684,14 +2149,24 @@
     },
     total=False,
 )
 
 class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
     pass
 
+DescribeRuleGroupResponseTypeDef = TypedDict(
+    "DescribeRuleGroupResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "RuleGroup": RuleGroupOutputTypeDef,
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupName": str,
         "Type": RuleGroupTypeType,
         "Capacity": int,
     },
@@ -1711,24 +2186,14 @@
 )
 
 class CreateRuleGroupRequestRequestTypeDef(
     _RequiredCreateRuleGroupRequestRequestTypeDef, _OptionalCreateRuleGroupRequestRequestTypeDef
 ):
     pass
 
-DescribeRuleGroupResponseTypeDef = TypedDict(
-    "DescribeRuleGroupResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "RuleGroup": RuleGroupTypeDef,
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "UpdateToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall.egg-info/PKG-INFO` & `mypy-boto3-network-firewall-1.28.12/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-network-firewall
-Version: 1.28.0
-Summary: Type annotations for boto3.NetworkFirewall 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 network-firewall type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-network-firewall"></a>
 
 # mypy-boto3-network-firewall
 
 [![PyPI - mypy-boto3-network-firewall](https://img.shields.io/pypi/v/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-network-firewall?color=blue)](https://pypistats.org/packages/mypy-boto3-network-firewall)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-network-firewall)](https://pepy.tech/project/mypy-boto3-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NetworkFirewall 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[boto3.NetworkFirewall 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,18 +329,20 @@
 ### Typed dictionaries
 
 `mypy_boto3_network_firewall.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_network_firewall.type_defs import (
+    AddressOutputTypeDef,
     AddressTypeDef,
     AssociateFirewallPolicyRequestRequestTypeDef,
     AssociateFirewallPolicyResponseTypeDef,
     SubnetMappingTypeDef,
+    SubnetMappingOutputTypeDef,
     AttachmentTypeDef,
     IPSetMetadataTypeDef,
     EncryptionConfigurationTypeDef,
     TagTypeDef,
     SourceMetadataTypeDef,
     DeleteFirewallPolicyRequestRequestTypeDef,
     DeleteFirewallRequestRequestTypeDef,
@@ -381,49 +351,67 @@
     DeleteTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallRequestRequestTypeDef,
     DescribeLoggingConfigurationRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
     DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataRequestRequestTypeDef,
-    StatefulRuleOptionsTypeDef,
+    StatefulRuleOptionsOutputTypeDef,
     DescribeRuleGroupRequestRequestTypeDef,
     DescribeTLSInspectionConfigurationRequestRequestTypeDef,
+    DimensionOutputTypeDef,
     DimensionTypeDef,
     DisassociateSubnetsRequestRequestTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     FirewallMetadataTypeDef,
     FirewallPolicyMetadataTypeDef,
+    StatefulEngineOptionsOutputTypeDef,
+    StatelessRuleGroupReferenceOutputTypeDef,
+    TagOutputTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupReferenceTypeDef,
+    HeaderOutputTypeDef,
     HeaderTypeDef,
+    IPSetOutputTypeDef,
+    IPSetReferenceOutputTypeDef,
     IPSetReferenceTypeDef,
     IPSetTypeDef,
     ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
     ListFirewallPoliciesRequestRequestTypeDef,
     ListFirewallsRequestListFirewallsPaginateTypeDef,
     ListFirewallsRequestRequestTypeDef,
     ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupMetadataTypeDef,
     ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
     ListTLSInspectionConfigurationsRequestRequestTypeDef,
     TLSInspectionConfigurationMetadataTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    LogDestinationConfigOutputTypeDef,
     LogDestinationConfigTypeDef,
+    PortRangeOutputTypeDef,
+    TCPFlagFieldOutputTypeDef,
     PortRangeTypeDef,
     TCPFlagFieldTypeDef,
     PaginatorConfigTypeDef,
     PerObjectStatusTypeDef,
+    PortSetOutputTypeDef,
     PortSetTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    SourceMetadataOutputTypeDef,
+    StatefulRuleOptionsTypeDef,
+    RuleOptionOutputTypeDef,
     RuleOptionTypeDef,
+    RulesSourceListOutputTypeDef,
     RulesSourceListTypeDef,
+    ServerCertificateOutputTypeDef,
     ServerCertificateTypeDef,
+    StatefulRuleGroupOverrideOutputTypeDef,
     StatefulRuleGroupOverrideTypeDef,
     TlsCertificateDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallDeleteProtectionRequestRequestTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionRequestRequestTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
@@ -432,77 +420,96 @@
     UpdateSubnetChangeProtectionRequestRequestTypeDef,
     UpdateSubnetChangeProtectionResponseTypeDef,
     AssociateSubnetsRequestRequestTypeDef,
     AssociateSubnetsResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     CIDRSummaryTypeDef,
     UpdateFirewallEncryptionConfigurationRequestRequestTypeDef,
-    UpdateFirewallEncryptionConfigurationResponseTypeDef,
     CreateFirewallRequestRequestTypeDef,
-    FirewallPolicyResponseTypeDef,
-    FirewallTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    RuleGroupResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
+    PublishMetricActionOutputTypeDef,
     PublishMetricActionTypeDef,
+    UpdateFirewallEncryptionConfigurationResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListFirewallPoliciesResponseTypeDef,
+    FirewallPolicyResponseTypeDef,
+    FirewallTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PolicyVariablesOutputTypeDef,
+    ReferenceSetsOutputTypeDef,
     ReferenceSetsTypeDef,
     PolicyVariablesTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
+    ServerCertificateScopeOutputTypeDef,
+    MatchAttributesOutputTypeDef,
     ServerCertificateScopeTypeDef,
     MatchAttributesTypeDef,
     SyncStateTypeDef,
+    RuleVariablesOutputTypeDef,
     RuleVariablesTypeDef,
+    RuleGroupResponseTypeDef,
+    StatefulRuleOutputTypeDef,
     StatefulRuleTypeDef,
+    StatefulRuleGroupReferenceOutputTypeDef,
     StatefulRuleGroupReferenceTypeDef,
     TLSInspectionConfigurationResponseTypeDef,
     CapacityUsageSummaryTypeDef,
+    ActionDefinitionOutputTypeDef,
+    ActionDefinitionTypeDef,
     CreateFirewallPolicyResponseTypeDef,
     DeleteFirewallPolicyResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
-    CreateRuleGroupResponseTypeDef,
-    DeleteRuleGroupResponseTypeDef,
-    UpdateRuleGroupResponseTypeDef,
-    ActionDefinitionTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
-    UpdateLoggingConfigurationRequestRequestTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
+    UpdateLoggingConfigurationRequestRequestTypeDef,
+    ServerCertificateConfigurationOutputTypeDef,
+    RuleDefinitionOutputTypeDef,
     ServerCertificateConfigurationTypeDef,
     RuleDefinitionTypeDef,
+    CreateRuleGroupResponseTypeDef,
+    DeleteRuleGroupResponseTypeDef,
+    UpdateRuleGroupResponseTypeDef,
     CreateTLSInspectionConfigurationResponseTypeDef,
     DeleteTLSInspectionConfigurationResponseTypeDef,
     UpdateTLSInspectionConfigurationResponseTypeDef,
     FirewallStatusTypeDef,
+    CustomActionOutputTypeDef,
     CustomActionTypeDef,
+    TLSInspectionConfigurationOutputTypeDef,
+    StatelessRuleOutputTypeDef,
     TLSInspectionConfigurationTypeDef,
     StatelessRuleTypeDef,
     CreateFirewallResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DescribeFirewallResponseTypeDef,
+    FirewallPolicyOutputTypeDef,
     FirewallPolicyTypeDef,
-    CreateTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
+    StatelessRulesAndCustomActionsOutputTypeDef,
+    CreateTLSInspectionConfigurationRequestRequestTypeDef,
     UpdateTLSInspectionConfigurationRequestRequestTypeDef,
     StatelessRulesAndCustomActionsTypeDef,
-    CreateFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
+    CreateFirewallPolicyRequestRequestTypeDef,
     UpdateFirewallPolicyRequestRequestTypeDef,
+    RulesSourceOutputTypeDef,
     RulesSourceTypeDef,
+    RuleGroupOutputTypeDef,
     RuleGroupTypeDef,
-    CreateRuleGroupRequestRequestTypeDef,
     DescribeRuleGroupResponseTypeDef,
+    CreateRuleGroupRequestRequestTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_structure() -> AddressOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-network-firewall-1.28.0/mypy_boto3_network_firewall.egg-info/SOURCES.txt` & `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.0/setup.py` & `mypy-boto3-network-firewall-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-network-firewall",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_network_firewall"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.NetworkFirewall 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.NetworkFirewall 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

