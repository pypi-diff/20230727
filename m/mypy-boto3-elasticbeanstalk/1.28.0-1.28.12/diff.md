# Comparing `tmp/mypy-boto3-elasticbeanstalk-1.28.0.tar.gz` & `tmp/mypy-boto3-elasticbeanstalk-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elasticbeanstalk-1.28.0.tar", last modified: Thu Jul  6 20:59:31 2023, max compression
+gzip compressed data, was "mypy-boto3-elasticbeanstalk-1.28.12.tar", last modified: Thu Jul 27 05:34:38 2023, max compression
```

## Comparing `mypy-boto3-elasticbeanstalk-1.28.0.tar` & `mypy-boto3-elasticbeanstalk-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:31.406294 mypy-boto3-elasticbeanstalk-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:17.000000 mypy-boto3-elasticbeanstalk-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21444 2023-07-06 20:59:31.406294 mypy-boto3-elasticbeanstalk-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19923 2023-07-06 20:40:17.000000 mypy-boto3-elasticbeanstalk-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:31.382294 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-06 20:40:17.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-06 20:40:17.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-06 20:40:17.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42742 2023-07-06 20:40:19.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42680 2023-07-06 20:40:18.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-07-06 20:40:20.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11773 2023-07-06 20:40:20.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-06 20:40:19.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-07-06 20:40:19.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:17.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    52858 2023-07-06 20:40:21.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    52819 2023-07-06 20:40:21.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:17.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-07-06 20:40:20.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-06 20:40:19.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:31.406294 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21444 2023-07-06 20:59:31.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-06 20:59:31.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:31.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:31.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:31.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 20:59:31.000000 mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:31.406294 mypy-boto3-elasticbeanstalk-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-06 20:40:17.000000 mypy-boto3-elasticbeanstalk-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.732520 mypy-boto3-elasticbeanstalk-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21767 2023-07-27 05:34:38.732520 mypy-boto3-elasticbeanstalk-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20244 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.732520 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42742 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42680 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55546 2023-07-27 05:21:49.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55503 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-27 05:21:48.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.732520 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21767 2023-07-27 05:34:38.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-27 05:34:38.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:38.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:38.000000 mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:38.732520 mypy-boto3-elasticbeanstalk-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:21:47.000000 mypy-boto3-elasticbeanstalk-1.28.12/setup.py
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/LICENSE` & `mypy-boto3-elasticbeanstalk-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/PKG-INFO` & `mypy-boto3-elasticbeanstalk-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticbeanstalk
-Version: 1.28.0
-Summary: Type annotations for boto3.ElasticBeanstalk 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ElasticBeanstalk 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-elasticbeanstalk"></a>
 
 # mypy-boto3-elasticbeanstalk
 
 [![PyPI - mypy-boto3-elasticbeanstalk](https://img.shields.io/pypi/v/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elasticbeanstalk?color=blue)](https://pypistats.org/packages/mypy-boto3-elasticbeanstalk)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticbeanstalk)](https://pepy.tech/project/mypy-boto3-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticBeanstalk 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[boto3.ElasticBeanstalk 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [mypy-boto3-elasticbeanstalk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -397,32 +397,37 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticbeanstalk.type_defs import (
     AbortEnvironmentUpdateMessageRequestTypeDef,
     LatencyTypeDef,
     StatusCodesTypeDef,
-    S3LocationTypeDef,
-    SourceBuildInformationTypeDef,
+    S3LocationOutputTypeDef,
+    SourceBuildInformationOutputTypeDef,
+    MaxAgeRuleOutputTypeDef,
+    MaxCountRuleOutputTypeDef,
     MaxAgeRuleTypeDef,
     MaxCountRuleTypeDef,
     ApplyEnvironmentManagedActionRequestRequestTypeDef,
     ApplyEnvironmentManagedActionResultTypeDef,
     AssociateEnvironmentOperationsRoleMessageRequestTypeDef,
     AutoScalingGroupTypeDef,
     BuildConfigurationTypeDef,
     BuilderTypeDef,
     CPUUtilizationTypeDef,
     CheckDNSAvailabilityMessageRequestTypeDef,
     CheckDNSAvailabilityResultMessageTypeDef,
     ComposeEnvironmentsMessageRequestTypeDef,
     OptionRestrictionRegexTypeDef,
+    ConfigurationOptionSettingOutputTypeDef,
     ConfigurationOptionSettingTypeDef,
     ValidationMessageTypeDef,
     TagTypeDef,
+    S3LocationTypeDef,
+    SourceBuildInformationTypeDef,
     SourceConfigurationTypeDef,
     EnvironmentTierTypeDef,
     OptionSpecificationTypeDef,
     PlatformSummaryTypeDef,
     CreateStorageLocationResultMessageTypeDef,
     CustomAmiTypeDef,
     DeleteApplicationMessageRequestTypeDef,
@@ -449,14 +454,15 @@
     DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeInstancesHealthRequestRequestTypeDef,
     DescribePlatformVersionRequestRequestTypeDef,
     DisassociateEnvironmentOperationsRoleMessageRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EnvironmentLinkTypeDef,
+    EnvironmentTierOutputTypeDef,
     EnvironmentInfoDescriptionTypeDef,
     InstanceTypeDef,
     LaunchConfigurationTypeDef,
     LaunchTemplateTypeDef,
     LoadBalancerTypeDef,
     QueueTypeDef,
     TriggerTypeDef,
@@ -469,34 +475,35 @@
     ListenerTypeDef,
     PaginatorConfigTypeDef,
     PlatformFrameworkTypeDef,
     PlatformProgrammingLanguageTypeDef,
     RebuildEnvironmentMessageRequestTypeDef,
     RequestEnvironmentInfoMessageRequestTypeDef,
     ResourceQuotaTypeDef,
+    TagOutputTypeDef,
     ResponseMetadataTypeDef,
     RestartAppServerMessageRequestTypeDef,
     RetrieveEnvironmentInfoMessageRequestTypeDef,
     SwapEnvironmentCNAMEsMessageRequestTypeDef,
     TerminateEnvironmentMessageRequestTypeDef,
     UpdateApplicationMessageRequestTypeDef,
     UpdateApplicationVersionMessageRequestTypeDef,
     ApplicationMetricsTypeDef,
     ApplicationVersionDescriptionTypeDef,
+    ApplicationVersionLifecycleConfigOutputTypeDef,
     ApplicationVersionLifecycleConfigTypeDef,
     SystemStatusTypeDef,
     ConfigurationOptionDescriptionTypeDef,
     ConfigurationSettingsDescriptionResponseMetadataTypeDef,
     ConfigurationSettingsDescriptionTypeDef,
     ValidateConfigurationSettingsMessageRequestTypeDef,
     ConfigurationSettingsValidationMessagesTypeDef,
-    CreateApplicationVersionMessageRequestTypeDef,
-    CreatePlatformVersionRequestRequestTypeDef,
-    ResourceTagsDescriptionMessageTypeDef,
     UpdateTagsForResourceMessageRequestTypeDef,
+    CreatePlatformVersionRequestRequestTypeDef,
+    CreateApplicationVersionMessageRequestTypeDef,
     CreateConfigurationTemplateMessageRequestTypeDef,
     CreateEnvironmentMessageRequestTypeDef,
     DescribeConfigurationOptionsMessageRequestTypeDef,
     UpdateConfigurationTemplateMessageRequestTypeDef,
     UpdateEnvironmentMessageRequestTypeDef,
     CreatePlatformVersionResultTypeDef,
     DeletePlatformVersionResultTypeDef,
@@ -513,17 +520,19 @@
     ListPlatformBranchesRequestRequestTypeDef,
     ListPlatformBranchesResultTypeDef,
     ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef,
     ListPlatformVersionsRequestRequestTypeDef,
     LoadBalancerDescriptionTypeDef,
     PlatformDescriptionTypeDef,
     ResourceQuotasTypeDef,
+    ResourceTagsDescriptionMessageTypeDef,
     DescribeEnvironmentHealthResultTypeDef,
     ApplicationVersionDescriptionMessageTypeDef,
     ApplicationVersionDescriptionsMessageTypeDef,
+    ApplicationResourceLifecycleConfigOutputTypeDef,
     ApplicationResourceLifecycleConfigTypeDef,
     SingleInstanceHealthTypeDef,
     ConfigurationOptionsDescriptionTypeDef,
     ConfigurationSettingsDescriptionsTypeDef,
     EnvironmentResourceDescriptionsMessageTypeDef,
     EnvironmentResourcesDescriptionTypeDef,
     DescribePlatformVersionResultTypeDef,
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/README.md` & `mypy-boto3-elasticbeanstalk-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-elasticbeanstalk"></a>
 
 # mypy-boto3-elasticbeanstalk
 
 [![PyPI - mypy-boto3-elasticbeanstalk](https://img.shields.io/pypi/v/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elasticbeanstalk?color=blue)](https://pypistats.org/packages/mypy-boto3-elasticbeanstalk)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticbeanstalk)](https://pepy.tech/project/mypy-boto3-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticBeanstalk 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[boto3.ElasticBeanstalk 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [mypy-boto3-elasticbeanstalk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,32 +365,37 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticbeanstalk.type_defs import (
     AbortEnvironmentUpdateMessageRequestTypeDef,
     LatencyTypeDef,
     StatusCodesTypeDef,
-    S3LocationTypeDef,
-    SourceBuildInformationTypeDef,
+    S3LocationOutputTypeDef,
+    SourceBuildInformationOutputTypeDef,
+    MaxAgeRuleOutputTypeDef,
+    MaxCountRuleOutputTypeDef,
     MaxAgeRuleTypeDef,
     MaxCountRuleTypeDef,
     ApplyEnvironmentManagedActionRequestRequestTypeDef,
     ApplyEnvironmentManagedActionResultTypeDef,
     AssociateEnvironmentOperationsRoleMessageRequestTypeDef,
     AutoScalingGroupTypeDef,
     BuildConfigurationTypeDef,
     BuilderTypeDef,
     CPUUtilizationTypeDef,
     CheckDNSAvailabilityMessageRequestTypeDef,
     CheckDNSAvailabilityResultMessageTypeDef,
     ComposeEnvironmentsMessageRequestTypeDef,
     OptionRestrictionRegexTypeDef,
+    ConfigurationOptionSettingOutputTypeDef,
     ConfigurationOptionSettingTypeDef,
     ValidationMessageTypeDef,
     TagTypeDef,
+    S3LocationTypeDef,
+    SourceBuildInformationTypeDef,
     SourceConfigurationTypeDef,
     EnvironmentTierTypeDef,
     OptionSpecificationTypeDef,
     PlatformSummaryTypeDef,
     CreateStorageLocationResultMessageTypeDef,
     CustomAmiTypeDef,
     DeleteApplicationMessageRequestTypeDef,
@@ -417,14 +422,15 @@
     DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeInstancesHealthRequestRequestTypeDef,
     DescribePlatformVersionRequestRequestTypeDef,
     DisassociateEnvironmentOperationsRoleMessageRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EnvironmentLinkTypeDef,
+    EnvironmentTierOutputTypeDef,
     EnvironmentInfoDescriptionTypeDef,
     InstanceTypeDef,
     LaunchConfigurationTypeDef,
     LaunchTemplateTypeDef,
     LoadBalancerTypeDef,
     QueueTypeDef,
     TriggerTypeDef,
@@ -437,34 +443,35 @@
     ListenerTypeDef,
     PaginatorConfigTypeDef,
     PlatformFrameworkTypeDef,
     PlatformProgrammingLanguageTypeDef,
     RebuildEnvironmentMessageRequestTypeDef,
     RequestEnvironmentInfoMessageRequestTypeDef,
     ResourceQuotaTypeDef,
+    TagOutputTypeDef,
     ResponseMetadataTypeDef,
     RestartAppServerMessageRequestTypeDef,
     RetrieveEnvironmentInfoMessageRequestTypeDef,
     SwapEnvironmentCNAMEsMessageRequestTypeDef,
     TerminateEnvironmentMessageRequestTypeDef,
     UpdateApplicationMessageRequestTypeDef,
     UpdateApplicationVersionMessageRequestTypeDef,
     ApplicationMetricsTypeDef,
     ApplicationVersionDescriptionTypeDef,
+    ApplicationVersionLifecycleConfigOutputTypeDef,
     ApplicationVersionLifecycleConfigTypeDef,
     SystemStatusTypeDef,
     ConfigurationOptionDescriptionTypeDef,
     ConfigurationSettingsDescriptionResponseMetadataTypeDef,
     ConfigurationSettingsDescriptionTypeDef,
     ValidateConfigurationSettingsMessageRequestTypeDef,
     ConfigurationSettingsValidationMessagesTypeDef,
-    CreateApplicationVersionMessageRequestTypeDef,
-    CreatePlatformVersionRequestRequestTypeDef,
-    ResourceTagsDescriptionMessageTypeDef,
     UpdateTagsForResourceMessageRequestTypeDef,
+    CreatePlatformVersionRequestRequestTypeDef,
+    CreateApplicationVersionMessageRequestTypeDef,
     CreateConfigurationTemplateMessageRequestTypeDef,
     CreateEnvironmentMessageRequestTypeDef,
     DescribeConfigurationOptionsMessageRequestTypeDef,
     UpdateConfigurationTemplateMessageRequestTypeDef,
     UpdateEnvironmentMessageRequestTypeDef,
     CreatePlatformVersionResultTypeDef,
     DeletePlatformVersionResultTypeDef,
@@ -481,17 +488,19 @@
     ListPlatformBranchesRequestRequestTypeDef,
     ListPlatformBranchesResultTypeDef,
     ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef,
     ListPlatformVersionsRequestRequestTypeDef,
     LoadBalancerDescriptionTypeDef,
     PlatformDescriptionTypeDef,
     ResourceQuotasTypeDef,
+    ResourceTagsDescriptionMessageTypeDef,
     DescribeEnvironmentHealthResultTypeDef,
     ApplicationVersionDescriptionMessageTypeDef,
     ApplicationVersionDescriptionsMessageTypeDef,
+    ApplicationResourceLifecycleConfigOutputTypeDef,
     ApplicationResourceLifecycleConfigTypeDef,
     SingleInstanceHealthTypeDef,
     ConfigurationOptionsDescriptionTypeDef,
     ConfigurationSettingsDescriptionsTypeDef,
     EnvironmentResourceDescriptionsMessageTypeDef,
     EnvironmentResourcesDescriptionTypeDef,
     DescribePlatformVersionResultTypeDef,
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/__init__.py` & `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/__init__.pyi` & `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/__main__.py` & `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticBeanstalk 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ElasticBeanstalk 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk\nOther"
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

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/client.py` & `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/client.pyi` & `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/literals.py` & `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,14 +243,15 @@
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
@@ -329,26 +330,28 @@
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

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/literals.pyi` & `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,15 @@
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
@@ -327,26 +328,28 @@
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

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/paginator.py` & `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/paginator.pyi` & `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/type_defs.py` & `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,32 +43,37 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AbortEnvironmentUpdateMessageRequestTypeDef",
     "LatencyTypeDef",
     "StatusCodesTypeDef",
-    "S3LocationTypeDef",
-    "SourceBuildInformationTypeDef",
+    "S3LocationOutputTypeDef",
+    "SourceBuildInformationOutputTypeDef",
+    "MaxAgeRuleOutputTypeDef",
+    "MaxCountRuleOutputTypeDef",
     "MaxAgeRuleTypeDef",
     "MaxCountRuleTypeDef",
     "ApplyEnvironmentManagedActionRequestRequestTypeDef",
     "ApplyEnvironmentManagedActionResultTypeDef",
     "AssociateEnvironmentOperationsRoleMessageRequestTypeDef",
     "AutoScalingGroupTypeDef",
     "BuildConfigurationTypeDef",
     "BuilderTypeDef",
     "CPUUtilizationTypeDef",
     "CheckDNSAvailabilityMessageRequestTypeDef",
     "CheckDNSAvailabilityResultMessageTypeDef",
     "ComposeEnvironmentsMessageRequestTypeDef",
     "OptionRestrictionRegexTypeDef",
+    "ConfigurationOptionSettingOutputTypeDef",
     "ConfigurationOptionSettingTypeDef",
     "ValidationMessageTypeDef",
     "TagTypeDef",
+    "S3LocationTypeDef",
+    "SourceBuildInformationTypeDef",
     "SourceConfigurationTypeDef",
     "EnvironmentTierTypeDef",
     "OptionSpecificationTypeDef",
     "PlatformSummaryTypeDef",
     "CreateStorageLocationResultMessageTypeDef",
     "CustomAmiTypeDef",
     "DeleteApplicationMessageRequestTypeDef",
@@ -95,14 +100,15 @@
     "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
     "DescribeInstancesHealthRequestRequestTypeDef",
     "DescribePlatformVersionRequestRequestTypeDef",
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnvironmentLinkTypeDef",
+    "EnvironmentTierOutputTypeDef",
     "EnvironmentInfoDescriptionTypeDef",
     "InstanceTypeDef",
     "LaunchConfigurationTypeDef",
     "LaunchTemplateTypeDef",
     "LoadBalancerTypeDef",
     "QueueTypeDef",
     "TriggerTypeDef",
@@ -115,34 +121,35 @@
     "ListenerTypeDef",
     "PaginatorConfigTypeDef",
     "PlatformFrameworkTypeDef",
     "PlatformProgrammingLanguageTypeDef",
     "RebuildEnvironmentMessageRequestTypeDef",
     "RequestEnvironmentInfoMessageRequestTypeDef",
     "ResourceQuotaTypeDef",
+    "TagOutputTypeDef",
     "ResponseMetadataTypeDef",
     "RestartAppServerMessageRequestTypeDef",
     "RetrieveEnvironmentInfoMessageRequestTypeDef",
     "SwapEnvironmentCNAMEsMessageRequestTypeDef",
     "TerminateEnvironmentMessageRequestTypeDef",
     "UpdateApplicationMessageRequestTypeDef",
     "UpdateApplicationVersionMessageRequestTypeDef",
     "ApplicationMetricsTypeDef",
     "ApplicationVersionDescriptionTypeDef",
+    "ApplicationVersionLifecycleConfigOutputTypeDef",
     "ApplicationVersionLifecycleConfigTypeDef",
     "SystemStatusTypeDef",
     "ConfigurationOptionDescriptionTypeDef",
     "ConfigurationSettingsDescriptionResponseMetadataTypeDef",
     "ConfigurationSettingsDescriptionTypeDef",
     "ValidateConfigurationSettingsMessageRequestTypeDef",
     "ConfigurationSettingsValidationMessagesTypeDef",
-    "CreateApplicationVersionMessageRequestTypeDef",
-    "CreatePlatformVersionRequestRequestTypeDef",
-    "ResourceTagsDescriptionMessageTypeDef",
     "UpdateTagsForResourceMessageRequestTypeDef",
+    "CreatePlatformVersionRequestRequestTypeDef",
+    "CreateApplicationVersionMessageRequestTypeDef",
     "CreateConfigurationTemplateMessageRequestTypeDef",
     "CreateEnvironmentMessageRequestTypeDef",
     "DescribeConfigurationOptionsMessageRequestTypeDef",
     "UpdateConfigurationTemplateMessageRequestTypeDef",
     "UpdateEnvironmentMessageRequestTypeDef",
     "CreatePlatformVersionResultTypeDef",
     "DeletePlatformVersionResultTypeDef",
@@ -159,17 +166,19 @@
     "ListPlatformBranchesRequestRequestTypeDef",
     "ListPlatformBranchesResultTypeDef",
     "ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef",
     "ListPlatformVersionsRequestRequestTypeDef",
     "LoadBalancerDescriptionTypeDef",
     "PlatformDescriptionTypeDef",
     "ResourceQuotasTypeDef",
+    "ResourceTagsDescriptionMessageTypeDef",
     "DescribeEnvironmentHealthResultTypeDef",
     "ApplicationVersionDescriptionMessageTypeDef",
     "ApplicationVersionDescriptionsMessageTypeDef",
+    "ApplicationResourceLifecycleConfigOutputTypeDef",
     "ApplicationResourceLifecycleConfigTypeDef",
     "SingleInstanceHealthTypeDef",
     "ConfigurationOptionsDescriptionTypeDef",
     "ConfigurationSettingsDescriptionsTypeDef",
     "EnvironmentResourceDescriptionsMessageTypeDef",
     "EnvironmentResourcesDescriptionTypeDef",
     "DescribePlatformVersionResultTypeDef",
@@ -217,32 +226,74 @@
         "Status3xx": int,
         "Status4xx": int,
         "Status5xx": int,
     },
     total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
+S3LocationOutputTypeDef = TypedDict(
+    "S3LocationOutputTypeDef",
     {
         "S3Bucket": str,
         "S3Key": str,
     },
     total=False,
 )
 
-SourceBuildInformationTypeDef = TypedDict(
-    "SourceBuildInformationTypeDef",
+SourceBuildInformationOutputTypeDef = TypedDict(
+    "SourceBuildInformationOutputTypeDef",
     {
         "SourceType": SourceTypeType,
         "SourceRepository": SourceRepositoryType,
         "SourceLocation": str,
     },
 )
 
+_RequiredMaxAgeRuleOutputTypeDef = TypedDict(
+    "_RequiredMaxAgeRuleOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalMaxAgeRuleOutputTypeDef = TypedDict(
+    "_OptionalMaxAgeRuleOutputTypeDef",
+    {
+        "MaxAgeInDays": int,
+        "DeleteSourceFromS3": bool,
+    },
+    total=False,
+)
+
+
+class MaxAgeRuleOutputTypeDef(_RequiredMaxAgeRuleOutputTypeDef, _OptionalMaxAgeRuleOutputTypeDef):
+    pass
+
+
+_RequiredMaxCountRuleOutputTypeDef = TypedDict(
+    "_RequiredMaxCountRuleOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalMaxCountRuleOutputTypeDef = TypedDict(
+    "_OptionalMaxCountRuleOutputTypeDef",
+    {
+        "MaxCount": int,
+        "DeleteSourceFromS3": bool,
+    },
+    total=False,
+)
+
+
+class MaxCountRuleOutputTypeDef(
+    _RequiredMaxCountRuleOutputTypeDef, _OptionalMaxCountRuleOutputTypeDef
+):
+    pass
+
+
 _RequiredMaxAgeRuleTypeDef = TypedDict(
     "_RequiredMaxAgeRuleTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalMaxAgeRuleTypeDef = TypedDict(
@@ -407,14 +458,25 @@
     {
         "Pattern": str,
         "Label": str,
     },
     total=False,
 )
 
+ConfigurationOptionSettingOutputTypeDef = TypedDict(
+    "ConfigurationOptionSettingOutputTypeDef",
+    {
+        "ResourceName": str,
+        "Namespace": str,
+        "OptionName": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 ConfigurationOptionSettingTypeDef = TypedDict(
     "ConfigurationOptionSettingTypeDef",
     {
         "ResourceName": str,
         "Namespace": str,
         "OptionName": str,
         "Value": str,
@@ -438,14 +500,32 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
+    {
+        "S3Bucket": str,
+        "S3Key": str,
+    },
+    total=False,
+)
+
+SourceBuildInformationTypeDef = TypedDict(
+    "SourceBuildInformationTypeDef",
+    {
+        "SourceType": SourceTypeType,
+        "SourceRepository": SourceRepositoryType,
+        "SourceLocation": str,
+    },
+)
+
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "ApplicationName": str,
         "TemplateName": str,
     },
     total=False,
@@ -843,14 +923,24 @@
     {
         "LinkName": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
+EnvironmentTierOutputTypeDef = TypedDict(
+    "EnvironmentTierOutputTypeDef",
+    {
+        "Name": str,
+        "Type": str,
+        "Version": str,
+    },
+    total=False,
+)
+
 EnvironmentInfoDescriptionTypeDef = TypedDict(
     "EnvironmentInfoDescriptionTypeDef",
     {
         "InfoType": EnvironmentInfoTypeType,
         "Ec2InstanceId": str,
         "SampleTimestamp": datetime,
         "Message": str,
@@ -1044,14 +1134,23 @@
     "ResourceQuotaTypeDef",
     {
         "Maximum": int,
     },
     total=False,
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
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -1171,24 +1270,33 @@
 ApplicationVersionDescriptionTypeDef = TypedDict(
     "ApplicationVersionDescriptionTypeDef",
     {
         "ApplicationVersionArn": str,
         "ApplicationName": str,
         "Description": str,
         "VersionLabel": str,
-        "SourceBuildInformation": SourceBuildInformationTypeDef,
+        "SourceBuildInformation": SourceBuildInformationOutputTypeDef,
         "BuildArn": str,
-        "SourceBundle": S3LocationTypeDef,
+        "SourceBundle": S3LocationOutputTypeDef,
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Status": ApplicationVersionStatusType,
     },
     total=False,
 )
 
+ApplicationVersionLifecycleConfigOutputTypeDef = TypedDict(
+    "ApplicationVersionLifecycleConfigOutputTypeDef",
+    {
+        "MaxCountRule": MaxCountRuleOutputTypeDef,
+        "MaxAgeRule": MaxAgeRuleOutputTypeDef,
+    },
+    total=False,
+)
+
 ApplicationVersionLifecycleConfigTypeDef = TypedDict(
     "ApplicationVersionLifecycleConfigTypeDef",
     {
         "MaxCountRule": MaxCountRuleTypeDef,
         "MaxAgeRule": MaxAgeRuleTypeDef,
     },
     total=False,
@@ -1229,15 +1337,15 @@
         "ApplicationName": str,
         "TemplateName": str,
         "Description": str,
         "EnvironmentName": str,
         "DeploymentStatus": ConfigurationDeploymentStatusType,
         "DateCreated": datetime,
         "DateUpdated": datetime,
-        "OptionSettings": List[ConfigurationOptionSettingTypeDef],
+        "OptionSettings": List[ConfigurationOptionSettingOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigurationSettingsDescriptionTypeDef = TypedDict(
     "ConfigurationSettingsDescriptionTypeDef",
     {
@@ -1246,15 +1354,15 @@
         "ApplicationName": str,
         "TemplateName": str,
         "Description": str,
         "EnvironmentName": str,
         "DeploymentStatus": ConfigurationDeploymentStatusType,
         "DateCreated": datetime,
         "DateUpdated": datetime,
-        "OptionSettings": List[ConfigurationOptionSettingTypeDef],
+        "OptionSettings": List[ConfigurationOptionSettingOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredValidateConfigurationSettingsMessageRequestTypeDef = TypedDict(
     "_RequiredValidateConfigurationSettingsMessageRequestTypeDef",
     {
@@ -1283,39 +1391,33 @@
     "ConfigurationSettingsValidationMessagesTypeDef",
     {
         "Messages": List[ValidationMessageTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateApplicationVersionMessageRequestTypeDef = TypedDict(
-    "_RequiredCreateApplicationVersionMessageRequestTypeDef",
+_RequiredUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_RequiredUpdateTagsForResourceMessageRequestTypeDef",
     {
-        "ApplicationName": str,
-        "VersionLabel": str,
+        "ResourceArn": str,
     },
 )
-_OptionalCreateApplicationVersionMessageRequestTypeDef = TypedDict(
-    "_OptionalCreateApplicationVersionMessageRequestTypeDef",
+_OptionalUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_OptionalUpdateTagsForResourceMessageRequestTypeDef",
     {
-        "Description": str,
-        "SourceBuildInformation": SourceBuildInformationTypeDef,
-        "SourceBundle": S3LocationTypeDef,
-        "BuildConfiguration": BuildConfigurationTypeDef,
-        "AutoCreateApplication": bool,
-        "Process": bool,
-        "Tags": Sequence[TagTypeDef],
+        "TagsToAdd": Sequence[TagTypeDef],
+        "TagsToRemove": Sequence[str],
     },
     total=False,
 )
 
 
-class CreateApplicationVersionMessageRequestTypeDef(
-    _RequiredCreateApplicationVersionMessageRequestTypeDef,
-    _OptionalCreateApplicationVersionMessageRequestTypeDef,
+class UpdateTagsForResourceMessageRequestTypeDef(
+    _RequiredUpdateTagsForResourceMessageRequestTypeDef,
+    _OptionalUpdateTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
 
 _RequiredCreatePlatformVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePlatformVersionRequestRequestTypeDef",
     {
@@ -1338,42 +1440,39 @@
 class CreatePlatformVersionRequestRequestTypeDef(
     _RequiredCreatePlatformVersionRequestRequestTypeDef,
     _OptionalCreatePlatformVersionRequestRequestTypeDef,
 ):
     pass
 
 
-ResourceTagsDescriptionMessageTypeDef = TypedDict(
-    "ResourceTagsDescriptionMessageTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourceTags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
-    "_RequiredUpdateTagsForResourceMessageRequestTypeDef",
+_RequiredCreateApplicationVersionMessageRequestTypeDef = TypedDict(
+    "_RequiredCreateApplicationVersionMessageRequestTypeDef",
     {
-        "ResourceArn": str,
+        "ApplicationName": str,
+        "VersionLabel": str,
     },
 )
-_OptionalUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
-    "_OptionalUpdateTagsForResourceMessageRequestTypeDef",
+_OptionalCreateApplicationVersionMessageRequestTypeDef = TypedDict(
+    "_OptionalCreateApplicationVersionMessageRequestTypeDef",
     {
-        "TagsToAdd": Sequence[TagTypeDef],
-        "TagsToRemove": Sequence[str],
+        "Description": str,
+        "SourceBuildInformation": SourceBuildInformationTypeDef,
+        "SourceBundle": S3LocationTypeDef,
+        "BuildConfiguration": BuildConfigurationTypeDef,
+        "AutoCreateApplication": bool,
+        "Process": bool,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class UpdateTagsForResourceMessageRequestTypeDef(
-    _RequiredUpdateTagsForResourceMessageRequestTypeDef,
-    _OptionalUpdateTagsForResourceMessageRequestTypeDef,
+class CreateApplicationVersionMessageRequestTypeDef(
+    _RequiredCreateApplicationVersionMessageRequestTypeDef,
+    _OptionalCreateApplicationVersionMessageRequestTypeDef,
 ):
     pass
 
 
 _RequiredCreateConfigurationTemplateMessageRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationTemplateMessageRequestTypeDef",
     {
@@ -1709,14 +1808,23 @@
         "EnvironmentQuota": ResourceQuotaTypeDef,
         "ConfigurationTemplateQuota": ResourceQuotaTypeDef,
         "CustomPlatformQuota": ResourceQuotaTypeDef,
     },
     total=False,
 )
 
+ResourceTagsDescriptionMessageTypeDef = TypedDict(
+    "ResourceTagsDescriptionMessageTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourceTags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeEnvironmentHealthResultTypeDef = TypedDict(
     "DescribeEnvironmentHealthResultTypeDef",
     {
         "EnvironmentName": str,
         "HealthStatus": str,
         "Status": EnvironmentHealthType,
         "Color": str,
@@ -1741,14 +1849,23 @@
     {
         "ApplicationVersions": List[ApplicationVersionDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ApplicationResourceLifecycleConfigOutputTypeDef = TypedDict(
+    "ApplicationResourceLifecycleConfigOutputTypeDef",
+    {
+        "ServiceRole": str,
+        "VersionLifecycleConfig": ApplicationVersionLifecycleConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 ApplicationResourceLifecycleConfigTypeDef = TypedDict(
     "ApplicationResourceLifecycleConfigTypeDef",
     {
         "ServiceRole": str,
         "VersionLifecycleConfig": ApplicationVersionLifecycleConfigTypeDef,
     },
     total=False,
@@ -1827,24 +1944,24 @@
         "ApplicationArn": str,
         "ApplicationName": str,
         "Description": str,
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Versions": List[str],
         "ConfigurationTemplates": List[str],
-        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
+        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigOutputTypeDef,
     },
     total=False,
 )
 
 ApplicationResourceLifecycleDescriptionMessageTypeDef = TypedDict(
     "ApplicationResourceLifecycleDescriptionMessageTypeDef",
     {
         "ApplicationName": str,
-        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
+        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateApplicationMessageRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationMessageRequestTypeDef",
     {
@@ -1902,15 +2019,15 @@
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Status": EnvironmentStatusType,
         "AbortableOperationInProgress": bool,
         "Health": EnvironmentHealthType,
         "HealthStatus": EnvironmentHealthStatusType,
         "Resources": EnvironmentResourcesDescriptionTypeDef,
-        "Tier": EnvironmentTierTypeDef,
+        "Tier": EnvironmentTierOutputTypeDef,
         "EnvironmentLinks": List[EnvironmentLinkTypeDef],
         "EnvironmentArn": str,
         "OperationsRole": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1930,15 +2047,15 @@
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Status": EnvironmentStatusType,
         "AbortableOperationInProgress": bool,
         "Health": EnvironmentHealthType,
         "HealthStatus": EnvironmentHealthStatusType,
         "Resources": EnvironmentResourcesDescriptionTypeDef,
-        "Tier": EnvironmentTierTypeDef,
+        "Tier": EnvironmentTierOutputTypeDef,
         "EnvironmentLinks": List[EnvironmentLinkTypeDef],
         "EnvironmentArn": str,
         "OperationsRole": str,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/type_defs.pyi` & `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,32 +42,37 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AbortEnvironmentUpdateMessageRequestTypeDef",
     "LatencyTypeDef",
     "StatusCodesTypeDef",
-    "S3LocationTypeDef",
-    "SourceBuildInformationTypeDef",
+    "S3LocationOutputTypeDef",
+    "SourceBuildInformationOutputTypeDef",
+    "MaxAgeRuleOutputTypeDef",
+    "MaxCountRuleOutputTypeDef",
     "MaxAgeRuleTypeDef",
     "MaxCountRuleTypeDef",
     "ApplyEnvironmentManagedActionRequestRequestTypeDef",
     "ApplyEnvironmentManagedActionResultTypeDef",
     "AssociateEnvironmentOperationsRoleMessageRequestTypeDef",
     "AutoScalingGroupTypeDef",
     "BuildConfigurationTypeDef",
     "BuilderTypeDef",
     "CPUUtilizationTypeDef",
     "CheckDNSAvailabilityMessageRequestTypeDef",
     "CheckDNSAvailabilityResultMessageTypeDef",
     "ComposeEnvironmentsMessageRequestTypeDef",
     "OptionRestrictionRegexTypeDef",
+    "ConfigurationOptionSettingOutputTypeDef",
     "ConfigurationOptionSettingTypeDef",
     "ValidationMessageTypeDef",
     "TagTypeDef",
+    "S3LocationTypeDef",
+    "SourceBuildInformationTypeDef",
     "SourceConfigurationTypeDef",
     "EnvironmentTierTypeDef",
     "OptionSpecificationTypeDef",
     "PlatformSummaryTypeDef",
     "CreateStorageLocationResultMessageTypeDef",
     "CustomAmiTypeDef",
     "DeleteApplicationMessageRequestTypeDef",
@@ -94,14 +99,15 @@
     "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
     "DescribeInstancesHealthRequestRequestTypeDef",
     "DescribePlatformVersionRequestRequestTypeDef",
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnvironmentLinkTypeDef",
+    "EnvironmentTierOutputTypeDef",
     "EnvironmentInfoDescriptionTypeDef",
     "InstanceTypeDef",
     "LaunchConfigurationTypeDef",
     "LaunchTemplateTypeDef",
     "LoadBalancerTypeDef",
     "QueueTypeDef",
     "TriggerTypeDef",
@@ -114,34 +120,35 @@
     "ListenerTypeDef",
     "PaginatorConfigTypeDef",
     "PlatformFrameworkTypeDef",
     "PlatformProgrammingLanguageTypeDef",
     "RebuildEnvironmentMessageRequestTypeDef",
     "RequestEnvironmentInfoMessageRequestTypeDef",
     "ResourceQuotaTypeDef",
+    "TagOutputTypeDef",
     "ResponseMetadataTypeDef",
     "RestartAppServerMessageRequestTypeDef",
     "RetrieveEnvironmentInfoMessageRequestTypeDef",
     "SwapEnvironmentCNAMEsMessageRequestTypeDef",
     "TerminateEnvironmentMessageRequestTypeDef",
     "UpdateApplicationMessageRequestTypeDef",
     "UpdateApplicationVersionMessageRequestTypeDef",
     "ApplicationMetricsTypeDef",
     "ApplicationVersionDescriptionTypeDef",
+    "ApplicationVersionLifecycleConfigOutputTypeDef",
     "ApplicationVersionLifecycleConfigTypeDef",
     "SystemStatusTypeDef",
     "ConfigurationOptionDescriptionTypeDef",
     "ConfigurationSettingsDescriptionResponseMetadataTypeDef",
     "ConfigurationSettingsDescriptionTypeDef",
     "ValidateConfigurationSettingsMessageRequestTypeDef",
     "ConfigurationSettingsValidationMessagesTypeDef",
-    "CreateApplicationVersionMessageRequestTypeDef",
-    "CreatePlatformVersionRequestRequestTypeDef",
-    "ResourceTagsDescriptionMessageTypeDef",
     "UpdateTagsForResourceMessageRequestTypeDef",
+    "CreatePlatformVersionRequestRequestTypeDef",
+    "CreateApplicationVersionMessageRequestTypeDef",
     "CreateConfigurationTemplateMessageRequestTypeDef",
     "CreateEnvironmentMessageRequestTypeDef",
     "DescribeConfigurationOptionsMessageRequestTypeDef",
     "UpdateConfigurationTemplateMessageRequestTypeDef",
     "UpdateEnvironmentMessageRequestTypeDef",
     "CreatePlatformVersionResultTypeDef",
     "DeletePlatformVersionResultTypeDef",
@@ -158,17 +165,19 @@
     "ListPlatformBranchesRequestRequestTypeDef",
     "ListPlatformBranchesResultTypeDef",
     "ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef",
     "ListPlatformVersionsRequestRequestTypeDef",
     "LoadBalancerDescriptionTypeDef",
     "PlatformDescriptionTypeDef",
     "ResourceQuotasTypeDef",
+    "ResourceTagsDescriptionMessageTypeDef",
     "DescribeEnvironmentHealthResultTypeDef",
     "ApplicationVersionDescriptionMessageTypeDef",
     "ApplicationVersionDescriptionsMessageTypeDef",
+    "ApplicationResourceLifecycleConfigOutputTypeDef",
     "ApplicationResourceLifecycleConfigTypeDef",
     "SingleInstanceHealthTypeDef",
     "ConfigurationOptionsDescriptionTypeDef",
     "ConfigurationSettingsDescriptionsTypeDef",
     "EnvironmentResourceDescriptionsMessageTypeDef",
     "EnvironmentResourcesDescriptionTypeDef",
     "DescribePlatformVersionResultTypeDef",
@@ -216,32 +225,70 @@
         "Status3xx": int,
         "Status4xx": int,
         "Status5xx": int,
     },
     total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
+S3LocationOutputTypeDef = TypedDict(
+    "S3LocationOutputTypeDef",
     {
         "S3Bucket": str,
         "S3Key": str,
     },
     total=False,
 )
 
-SourceBuildInformationTypeDef = TypedDict(
-    "SourceBuildInformationTypeDef",
+SourceBuildInformationOutputTypeDef = TypedDict(
+    "SourceBuildInformationOutputTypeDef",
     {
         "SourceType": SourceTypeType,
         "SourceRepository": SourceRepositoryType,
         "SourceLocation": str,
     },
 )
 
+_RequiredMaxAgeRuleOutputTypeDef = TypedDict(
+    "_RequiredMaxAgeRuleOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalMaxAgeRuleOutputTypeDef = TypedDict(
+    "_OptionalMaxAgeRuleOutputTypeDef",
+    {
+        "MaxAgeInDays": int,
+        "DeleteSourceFromS3": bool,
+    },
+    total=False,
+)
+
+class MaxAgeRuleOutputTypeDef(_RequiredMaxAgeRuleOutputTypeDef, _OptionalMaxAgeRuleOutputTypeDef):
+    pass
+
+_RequiredMaxCountRuleOutputTypeDef = TypedDict(
+    "_RequiredMaxCountRuleOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalMaxCountRuleOutputTypeDef = TypedDict(
+    "_OptionalMaxCountRuleOutputTypeDef",
+    {
+        "MaxCount": int,
+        "DeleteSourceFromS3": bool,
+    },
+    total=False,
+)
+
+class MaxCountRuleOutputTypeDef(
+    _RequiredMaxCountRuleOutputTypeDef, _OptionalMaxCountRuleOutputTypeDef
+):
+    pass
+
 _RequiredMaxAgeRuleTypeDef = TypedDict(
     "_RequiredMaxAgeRuleTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalMaxAgeRuleTypeDef = TypedDict(
@@ -398,14 +445,25 @@
     {
         "Pattern": str,
         "Label": str,
     },
     total=False,
 )
 
+ConfigurationOptionSettingOutputTypeDef = TypedDict(
+    "ConfigurationOptionSettingOutputTypeDef",
+    {
+        "ResourceName": str,
+        "Namespace": str,
+        "OptionName": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 ConfigurationOptionSettingTypeDef = TypedDict(
     "ConfigurationOptionSettingTypeDef",
     {
         "ResourceName": str,
         "Namespace": str,
         "OptionName": str,
         "Value": str,
@@ -429,14 +487,32 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
+    {
+        "S3Bucket": str,
+        "S3Key": str,
+    },
+    total=False,
+)
+
+SourceBuildInformationTypeDef = TypedDict(
+    "SourceBuildInformationTypeDef",
+    {
+        "SourceType": SourceTypeType,
+        "SourceRepository": SourceRepositoryType,
+        "SourceLocation": str,
+    },
+)
+
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "ApplicationName": str,
         "TemplateName": str,
     },
     total=False,
@@ -828,14 +904,24 @@
     {
         "LinkName": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
+EnvironmentTierOutputTypeDef = TypedDict(
+    "EnvironmentTierOutputTypeDef",
+    {
+        "Name": str,
+        "Type": str,
+        "Version": str,
+    },
+    total=False,
+)
+
 EnvironmentInfoDescriptionTypeDef = TypedDict(
     "EnvironmentInfoDescriptionTypeDef",
     {
         "InfoType": EnvironmentInfoTypeType,
         "Ec2InstanceId": str,
         "SampleTimestamp": datetime,
         "Message": str,
@@ -1027,14 +1113,23 @@
     "ResourceQuotaTypeDef",
     {
         "Maximum": int,
     },
     total=False,
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
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -1148,24 +1243,33 @@
 ApplicationVersionDescriptionTypeDef = TypedDict(
     "ApplicationVersionDescriptionTypeDef",
     {
         "ApplicationVersionArn": str,
         "ApplicationName": str,
         "Description": str,
         "VersionLabel": str,
-        "SourceBuildInformation": SourceBuildInformationTypeDef,
+        "SourceBuildInformation": SourceBuildInformationOutputTypeDef,
         "BuildArn": str,
-        "SourceBundle": S3LocationTypeDef,
+        "SourceBundle": S3LocationOutputTypeDef,
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Status": ApplicationVersionStatusType,
     },
     total=False,
 )
 
+ApplicationVersionLifecycleConfigOutputTypeDef = TypedDict(
+    "ApplicationVersionLifecycleConfigOutputTypeDef",
+    {
+        "MaxCountRule": MaxCountRuleOutputTypeDef,
+        "MaxAgeRule": MaxAgeRuleOutputTypeDef,
+    },
+    total=False,
+)
+
 ApplicationVersionLifecycleConfigTypeDef = TypedDict(
     "ApplicationVersionLifecycleConfigTypeDef",
     {
         "MaxCountRule": MaxCountRuleTypeDef,
         "MaxAgeRule": MaxAgeRuleTypeDef,
     },
     total=False,
@@ -1206,15 +1310,15 @@
         "ApplicationName": str,
         "TemplateName": str,
         "Description": str,
         "EnvironmentName": str,
         "DeploymentStatus": ConfigurationDeploymentStatusType,
         "DateCreated": datetime,
         "DateUpdated": datetime,
-        "OptionSettings": List[ConfigurationOptionSettingTypeDef],
+        "OptionSettings": List[ConfigurationOptionSettingOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigurationSettingsDescriptionTypeDef = TypedDict(
     "ConfigurationSettingsDescriptionTypeDef",
     {
@@ -1223,15 +1327,15 @@
         "ApplicationName": str,
         "TemplateName": str,
         "Description": str,
         "EnvironmentName": str,
         "DeploymentStatus": ConfigurationDeploymentStatusType,
         "DateCreated": datetime,
         "DateUpdated": datetime,
-        "OptionSettings": List[ConfigurationOptionSettingTypeDef],
+        "OptionSettings": List[ConfigurationOptionSettingOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredValidateConfigurationSettingsMessageRequestTypeDef = TypedDict(
     "_RequiredValidateConfigurationSettingsMessageRequestTypeDef",
     {
@@ -1258,38 +1362,32 @@
     "ConfigurationSettingsValidationMessagesTypeDef",
     {
         "Messages": List[ValidationMessageTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateApplicationVersionMessageRequestTypeDef = TypedDict(
-    "_RequiredCreateApplicationVersionMessageRequestTypeDef",
+_RequiredUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_RequiredUpdateTagsForResourceMessageRequestTypeDef",
     {
-        "ApplicationName": str,
-        "VersionLabel": str,
+        "ResourceArn": str,
     },
 )
-_OptionalCreateApplicationVersionMessageRequestTypeDef = TypedDict(
-    "_OptionalCreateApplicationVersionMessageRequestTypeDef",
+_OptionalUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_OptionalUpdateTagsForResourceMessageRequestTypeDef",
     {
-        "Description": str,
-        "SourceBuildInformation": SourceBuildInformationTypeDef,
-        "SourceBundle": S3LocationTypeDef,
-        "BuildConfiguration": BuildConfigurationTypeDef,
-        "AutoCreateApplication": bool,
-        "Process": bool,
-        "Tags": Sequence[TagTypeDef],
+        "TagsToAdd": Sequence[TagTypeDef],
+        "TagsToRemove": Sequence[str],
     },
     total=False,
 )
 
-class CreateApplicationVersionMessageRequestTypeDef(
-    _RequiredCreateApplicationVersionMessageRequestTypeDef,
-    _OptionalCreateApplicationVersionMessageRequestTypeDef,
+class UpdateTagsForResourceMessageRequestTypeDef(
+    _RequiredUpdateTagsForResourceMessageRequestTypeDef,
+    _OptionalUpdateTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
 _RequiredCreatePlatformVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePlatformVersionRequestRequestTypeDef",
     {
         "PlatformName": str,
@@ -1309,41 +1407,38 @@
 
 class CreatePlatformVersionRequestRequestTypeDef(
     _RequiredCreatePlatformVersionRequestRequestTypeDef,
     _OptionalCreatePlatformVersionRequestRequestTypeDef,
 ):
     pass
 
-ResourceTagsDescriptionMessageTypeDef = TypedDict(
-    "ResourceTagsDescriptionMessageTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourceTags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
-    "_RequiredUpdateTagsForResourceMessageRequestTypeDef",
+_RequiredCreateApplicationVersionMessageRequestTypeDef = TypedDict(
+    "_RequiredCreateApplicationVersionMessageRequestTypeDef",
     {
-        "ResourceArn": str,
+        "ApplicationName": str,
+        "VersionLabel": str,
     },
 )
-_OptionalUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
-    "_OptionalUpdateTagsForResourceMessageRequestTypeDef",
+_OptionalCreateApplicationVersionMessageRequestTypeDef = TypedDict(
+    "_OptionalCreateApplicationVersionMessageRequestTypeDef",
     {
-        "TagsToAdd": Sequence[TagTypeDef],
-        "TagsToRemove": Sequence[str],
+        "Description": str,
+        "SourceBuildInformation": SourceBuildInformationTypeDef,
+        "SourceBundle": S3LocationTypeDef,
+        "BuildConfiguration": BuildConfigurationTypeDef,
+        "AutoCreateApplication": bool,
+        "Process": bool,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class UpdateTagsForResourceMessageRequestTypeDef(
-    _RequiredUpdateTagsForResourceMessageRequestTypeDef,
-    _OptionalUpdateTagsForResourceMessageRequestTypeDef,
+class CreateApplicationVersionMessageRequestTypeDef(
+    _RequiredCreateApplicationVersionMessageRequestTypeDef,
+    _OptionalCreateApplicationVersionMessageRequestTypeDef,
 ):
     pass
 
 _RequiredCreateConfigurationTemplateMessageRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationTemplateMessageRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1672,14 +1767,23 @@
         "EnvironmentQuota": ResourceQuotaTypeDef,
         "ConfigurationTemplateQuota": ResourceQuotaTypeDef,
         "CustomPlatformQuota": ResourceQuotaTypeDef,
     },
     total=False,
 )
 
+ResourceTagsDescriptionMessageTypeDef = TypedDict(
+    "ResourceTagsDescriptionMessageTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourceTags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeEnvironmentHealthResultTypeDef = TypedDict(
     "DescribeEnvironmentHealthResultTypeDef",
     {
         "EnvironmentName": str,
         "HealthStatus": str,
         "Status": EnvironmentHealthType,
         "Color": str,
@@ -1704,14 +1808,23 @@
     {
         "ApplicationVersions": List[ApplicationVersionDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ApplicationResourceLifecycleConfigOutputTypeDef = TypedDict(
+    "ApplicationResourceLifecycleConfigOutputTypeDef",
+    {
+        "ServiceRole": str,
+        "VersionLifecycleConfig": ApplicationVersionLifecycleConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 ApplicationResourceLifecycleConfigTypeDef = TypedDict(
     "ApplicationResourceLifecycleConfigTypeDef",
     {
         "ServiceRole": str,
         "VersionLifecycleConfig": ApplicationVersionLifecycleConfigTypeDef,
     },
     total=False,
@@ -1790,24 +1903,24 @@
         "ApplicationArn": str,
         "ApplicationName": str,
         "Description": str,
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Versions": List[str],
         "ConfigurationTemplates": List[str],
-        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
+        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigOutputTypeDef,
     },
     total=False,
 )
 
 ApplicationResourceLifecycleDescriptionMessageTypeDef = TypedDict(
     "ApplicationResourceLifecycleDescriptionMessageTypeDef",
     {
         "ApplicationName": str,
-        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
+        "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateApplicationMessageRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationMessageRequestTypeDef",
     {
@@ -1863,15 +1976,15 @@
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Status": EnvironmentStatusType,
         "AbortableOperationInProgress": bool,
         "Health": EnvironmentHealthType,
         "HealthStatus": EnvironmentHealthStatusType,
         "Resources": EnvironmentResourcesDescriptionTypeDef,
-        "Tier": EnvironmentTierTypeDef,
+        "Tier": EnvironmentTierOutputTypeDef,
         "EnvironmentLinks": List[EnvironmentLinkTypeDef],
         "EnvironmentArn": str,
         "OperationsRole": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1891,15 +2004,15 @@
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "Status": EnvironmentStatusType,
         "AbortableOperationInProgress": bool,
         "Health": EnvironmentHealthType,
         "HealthStatus": EnvironmentHealthStatusType,
         "Resources": EnvironmentResourcesDescriptionTypeDef,
-        "Tier": EnvironmentTierTypeDef,
+        "Tier": EnvironmentTierOutputTypeDef,
         "EnvironmentLinks": List[EnvironmentLinkTypeDef],
         "EnvironmentArn": str,
         "OperationsRole": str,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/waiter.py` & `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk/waiter.pyi` & `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO` & `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticbeanstalk
-Version: 1.28.0
-Summary: Type annotations for boto3.ElasticBeanstalk 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ElasticBeanstalk 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-elasticbeanstalk"></a>
 
 # mypy-boto3-elasticbeanstalk
 
 [![PyPI - mypy-boto3-elasticbeanstalk](https://img.shields.io/pypi/v/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elasticbeanstalk?color=blue)](https://pypistats.org/packages/mypy-boto3-elasticbeanstalk)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticbeanstalk)](https://pepy.tech/project/mypy-boto3-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticBeanstalk 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[boto3.ElasticBeanstalk 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [mypy-boto3-elasticbeanstalk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -397,32 +397,37 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticbeanstalk.type_defs import (
     AbortEnvironmentUpdateMessageRequestTypeDef,
     LatencyTypeDef,
     StatusCodesTypeDef,
-    S3LocationTypeDef,
-    SourceBuildInformationTypeDef,
+    S3LocationOutputTypeDef,
+    SourceBuildInformationOutputTypeDef,
+    MaxAgeRuleOutputTypeDef,
+    MaxCountRuleOutputTypeDef,
     MaxAgeRuleTypeDef,
     MaxCountRuleTypeDef,
     ApplyEnvironmentManagedActionRequestRequestTypeDef,
     ApplyEnvironmentManagedActionResultTypeDef,
     AssociateEnvironmentOperationsRoleMessageRequestTypeDef,
     AutoScalingGroupTypeDef,
     BuildConfigurationTypeDef,
     BuilderTypeDef,
     CPUUtilizationTypeDef,
     CheckDNSAvailabilityMessageRequestTypeDef,
     CheckDNSAvailabilityResultMessageTypeDef,
     ComposeEnvironmentsMessageRequestTypeDef,
     OptionRestrictionRegexTypeDef,
+    ConfigurationOptionSettingOutputTypeDef,
     ConfigurationOptionSettingTypeDef,
     ValidationMessageTypeDef,
     TagTypeDef,
+    S3LocationTypeDef,
+    SourceBuildInformationTypeDef,
     SourceConfigurationTypeDef,
     EnvironmentTierTypeDef,
     OptionSpecificationTypeDef,
     PlatformSummaryTypeDef,
     CreateStorageLocationResultMessageTypeDef,
     CustomAmiTypeDef,
     DeleteApplicationMessageRequestTypeDef,
@@ -449,14 +454,15 @@
     DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeInstancesHealthRequestRequestTypeDef,
     DescribePlatformVersionRequestRequestTypeDef,
     DisassociateEnvironmentOperationsRoleMessageRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EnvironmentLinkTypeDef,
+    EnvironmentTierOutputTypeDef,
     EnvironmentInfoDescriptionTypeDef,
     InstanceTypeDef,
     LaunchConfigurationTypeDef,
     LaunchTemplateTypeDef,
     LoadBalancerTypeDef,
     QueueTypeDef,
     TriggerTypeDef,
@@ -469,34 +475,35 @@
     ListenerTypeDef,
     PaginatorConfigTypeDef,
     PlatformFrameworkTypeDef,
     PlatformProgrammingLanguageTypeDef,
     RebuildEnvironmentMessageRequestTypeDef,
     RequestEnvironmentInfoMessageRequestTypeDef,
     ResourceQuotaTypeDef,
+    TagOutputTypeDef,
     ResponseMetadataTypeDef,
     RestartAppServerMessageRequestTypeDef,
     RetrieveEnvironmentInfoMessageRequestTypeDef,
     SwapEnvironmentCNAMEsMessageRequestTypeDef,
     TerminateEnvironmentMessageRequestTypeDef,
     UpdateApplicationMessageRequestTypeDef,
     UpdateApplicationVersionMessageRequestTypeDef,
     ApplicationMetricsTypeDef,
     ApplicationVersionDescriptionTypeDef,
+    ApplicationVersionLifecycleConfigOutputTypeDef,
     ApplicationVersionLifecycleConfigTypeDef,
     SystemStatusTypeDef,
     ConfigurationOptionDescriptionTypeDef,
     ConfigurationSettingsDescriptionResponseMetadataTypeDef,
     ConfigurationSettingsDescriptionTypeDef,
     ValidateConfigurationSettingsMessageRequestTypeDef,
     ConfigurationSettingsValidationMessagesTypeDef,
-    CreateApplicationVersionMessageRequestTypeDef,
-    CreatePlatformVersionRequestRequestTypeDef,
-    ResourceTagsDescriptionMessageTypeDef,
     UpdateTagsForResourceMessageRequestTypeDef,
+    CreatePlatformVersionRequestRequestTypeDef,
+    CreateApplicationVersionMessageRequestTypeDef,
     CreateConfigurationTemplateMessageRequestTypeDef,
     CreateEnvironmentMessageRequestTypeDef,
     DescribeConfigurationOptionsMessageRequestTypeDef,
     UpdateConfigurationTemplateMessageRequestTypeDef,
     UpdateEnvironmentMessageRequestTypeDef,
     CreatePlatformVersionResultTypeDef,
     DeletePlatformVersionResultTypeDef,
@@ -513,17 +520,19 @@
     ListPlatformBranchesRequestRequestTypeDef,
     ListPlatformBranchesResultTypeDef,
     ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef,
     ListPlatformVersionsRequestRequestTypeDef,
     LoadBalancerDescriptionTypeDef,
     PlatformDescriptionTypeDef,
     ResourceQuotasTypeDef,
+    ResourceTagsDescriptionMessageTypeDef,
     DescribeEnvironmentHealthResultTypeDef,
     ApplicationVersionDescriptionMessageTypeDef,
     ApplicationVersionDescriptionsMessageTypeDef,
+    ApplicationResourceLifecycleConfigOutputTypeDef,
     ApplicationResourceLifecycleConfigTypeDef,
     SingleInstanceHealthTypeDef,
     ConfigurationOptionsDescriptionTypeDef,
     ConfigurationSettingsDescriptionsTypeDef,
     EnvironmentResourceDescriptionsMessageTypeDef,
     EnvironmentResourcesDescriptionTypeDef,
     DescribePlatformVersionResultTypeDef,
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt` & `mypy-boto3-elasticbeanstalk-1.28.12/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.0/setup.py` & `mypy-boto3-elasticbeanstalk-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elasticbeanstalk",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_elasticbeanstalk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticBeanstalk 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ElasticBeanstalk 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

