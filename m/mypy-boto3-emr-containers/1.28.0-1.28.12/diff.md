# Comparing `tmp/mypy-boto3-emr-containers-1.28.0.tar.gz` & `tmp/mypy-boto3-emr-containers-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-containers-1.28.0.tar", last modified: Thu Jul  6 20:59:33 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-containers-1.28.12.tar", last modified: Thu Jul 27 05:34:40 2023, max compression
```

## Comparing `mypy-boto3-emr-containers-1.28.0.tar` & `mypy-boto3-emr-containers-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.446299 mypy-boto3-emr-containers-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:39.000000 mypy-boto3-emr-containers-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-07-06 20:59:33.446299 mypy-boto3-emr-containers-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-07-06 20:40:39.000000 mypy-boto3-emr-containers-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.446299 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-06 20:40:39.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-06 20:40:39.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 20:40:39.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18379 2023-07-06 20:40:39.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-07-06 20:40:39.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-06 20:40:40.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-07-06 20:40:40.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-06 20:40:40.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-07-06 20:40:40.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:39.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25981 2023-07-06 20:40:41.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25950 2023-07-06 20:40:40.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:39.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.446299 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-07-06 20:59:33.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 20:59:33.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:33.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:33.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:33.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 20:59:33.000000 mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:33.446299 mypy-boto3-emr-containers-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-06 20:40:39.000000 mypy-boto3-emr-containers-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.156515 mypy-boto3-emr-containers-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-07-27 05:34:40.152515 mypy-boto3-emr-containers-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.148515 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18379 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    32747 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32706 2023-07-27 05:22:01.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.148515 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-07-27 05:34:39.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:34:40.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:39.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:39.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:39.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:39.000000 mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:40.156515 mypy-boto3-emr-containers-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 05:22:00.000000 mypy-boto3-emr-containers-1.28.12/setup.py
```

### Comparing `mypy-boto3-emr-containers-1.28.0/LICENSE` & `mypy-boto3-emr-containers-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.0/PKG-INFO` & `mypy-boto3-emr-containers-1.28.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-containers
-Version: 1.28.0
-Summary: Type annotations for boto3.EMRContainers 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.EMRContainers 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-emr-containers"></a>
 
 # mypy-boto3-emr-containers
 
 [![PyPI - mypy-boto3-emr-containers](https://img.shields.io/pypi/v/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-containers?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-containers)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-containers)](https://pepy.tech/project/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
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
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,17 +345,21 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_containers.type_defs import (
     CancelJobRunRequestRequestTypeDef,
     CancelJobRunResponseTypeDef,
     CertificateTypeDef,
+    CloudWatchMonitoringConfigurationOutputTypeDef,
     CloudWatchMonitoringConfigurationTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
+    EksInfoOutputTypeDef,
     EksInfoTypeDef,
+    ContainerLogRotationConfigurationOutputTypeDef,
     ContainerLogRotationConfigurationTypeDef,
     CreateJobTemplateResponseTypeDef,
     CreateManagedEndpointResponseTypeDef,
     CreateVirtualClusterResponseTypeDef,
     CredentialsTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeleteJobTemplateResponseTypeDef,
@@ -364,60 +368,75 @@
     DeleteVirtualClusterRequestRequestTypeDef,
     DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
     DescribeManagedEndpointRequestRequestTypeDef,
     DescribeVirtualClusterRequestRequestTypeDef,
     GetManagedEndpointSessionCredentialsRequestRequestTypeDef,
+    SparkSqlJobDriverOutputTypeDef,
+    SparkSubmitJobDriverOutputTypeDef,
     SparkSqlJobDriverTypeDef,
     SparkSubmitJobDriverTypeDef,
-    RetryPolicyConfigurationTypeDef,
+    RetryPolicyConfigurationOutputTypeDef,
     RetryPolicyExecutionTypeDef,
+    TemplateParameterConfigurationOutputTypeDef,
     TemplateParameterConfigurationTypeDef,
     ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
     ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     ListManagedEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
     ListVirtualClustersRequestRequestTypeDef,
+    S3MonitoringConfigurationOutputTypeDef,
     S3MonitoringConfigurationTypeDef,
     PaginatorConfigTypeDef,
+    ParametricCloudWatchMonitoringConfigurationOutputTypeDef,
     ParametricCloudWatchMonitoringConfigurationTypeDef,
+    ParametricS3MonitoringConfigurationOutputTypeDef,
     ParametricS3MonitoringConfigurationTypeDef,
     ResponseMetadataTypeDef,
+    RetryPolicyConfigurationTypeDef,
     StartJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ContainerInfoOutputTypeDef,
     ContainerInfoTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
+    JobDriverOutputTypeDef,
     JobDriverTypeDef,
+    MonitoringConfigurationOutputTypeDef,
     MonitoringConfigurationTypeDef,
+    ParametricMonitoringConfigurationOutputTypeDef,
     ParametricMonitoringConfigurationTypeDef,
+    ContainerProviderOutputTypeDef,
     ContainerProviderTypeDef,
+    ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
+    ParametricConfigurationOverridesOutputTypeDef,
     ParametricConfigurationOverridesTypeDef,
-    CreateVirtualClusterRequestRequestTypeDef,
     VirtualClusterTypeDef,
-    CreateManagedEndpointRequestRequestTypeDef,
+    CreateVirtualClusterRequestRequestTypeDef,
     EndpointTypeDef,
     JobRunTypeDef,
+    CreateManagedEndpointRequestRequestTypeDef,
     StartJobRunRequestRequestTypeDef,
+    JobTemplateDataOutputTypeDef,
     JobTemplateDataTypeDef,
     DescribeVirtualClusterResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     ListJobRunsResponseTypeDef,
-    CreateJobTemplateRequestRequestTypeDef,
     JobTemplateTypeDef,
+    CreateJobTemplateRequestRequestTypeDef,
     DescribeJobTemplateResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
 )
 
 
 def get_structure() -> CancelJobRunRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-emr-containers-1.28.0/README.md` & `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-emr-containers
+Version: 1.28.12
+Summary: Type annotations for boto3.EMRContainers 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 emr-containers type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-emr-containers"></a>
 
 # mypy-boto3-emr-containers
 
 [![PyPI - mypy-boto3-emr-containers](https://img.shields.io/pypi/v/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-containers?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-containers)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-containers)](https://pepy.tech/project/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
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
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,17 +345,21 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_containers.type_defs import (
     CancelJobRunRequestRequestTypeDef,
     CancelJobRunResponseTypeDef,
     CertificateTypeDef,
+    CloudWatchMonitoringConfigurationOutputTypeDef,
     CloudWatchMonitoringConfigurationTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
+    EksInfoOutputTypeDef,
     EksInfoTypeDef,
+    ContainerLogRotationConfigurationOutputTypeDef,
     ContainerLogRotationConfigurationTypeDef,
     CreateJobTemplateResponseTypeDef,
     CreateManagedEndpointResponseTypeDef,
     CreateVirtualClusterResponseTypeDef,
     CredentialsTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeleteJobTemplateResponseTypeDef,
@@ -332,60 +368,75 @@
     DeleteVirtualClusterRequestRequestTypeDef,
     DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
     DescribeManagedEndpointRequestRequestTypeDef,
     DescribeVirtualClusterRequestRequestTypeDef,
     GetManagedEndpointSessionCredentialsRequestRequestTypeDef,
+    SparkSqlJobDriverOutputTypeDef,
+    SparkSubmitJobDriverOutputTypeDef,
     SparkSqlJobDriverTypeDef,
     SparkSubmitJobDriverTypeDef,
-    RetryPolicyConfigurationTypeDef,
+    RetryPolicyConfigurationOutputTypeDef,
     RetryPolicyExecutionTypeDef,
+    TemplateParameterConfigurationOutputTypeDef,
     TemplateParameterConfigurationTypeDef,
     ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
     ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     ListManagedEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
     ListVirtualClustersRequestRequestTypeDef,
+    S3MonitoringConfigurationOutputTypeDef,
     S3MonitoringConfigurationTypeDef,
     PaginatorConfigTypeDef,
+    ParametricCloudWatchMonitoringConfigurationOutputTypeDef,
     ParametricCloudWatchMonitoringConfigurationTypeDef,
+    ParametricS3MonitoringConfigurationOutputTypeDef,
     ParametricS3MonitoringConfigurationTypeDef,
     ResponseMetadataTypeDef,
+    RetryPolicyConfigurationTypeDef,
     StartJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ContainerInfoOutputTypeDef,
     ContainerInfoTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
+    JobDriverOutputTypeDef,
     JobDriverTypeDef,
+    MonitoringConfigurationOutputTypeDef,
     MonitoringConfigurationTypeDef,
+    ParametricMonitoringConfigurationOutputTypeDef,
     ParametricMonitoringConfigurationTypeDef,
+    ContainerProviderOutputTypeDef,
     ContainerProviderTypeDef,
+    ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
+    ParametricConfigurationOverridesOutputTypeDef,
     ParametricConfigurationOverridesTypeDef,
-    CreateVirtualClusterRequestRequestTypeDef,
     VirtualClusterTypeDef,
-    CreateManagedEndpointRequestRequestTypeDef,
+    CreateVirtualClusterRequestRequestTypeDef,
     EndpointTypeDef,
     JobRunTypeDef,
+    CreateManagedEndpointRequestRequestTypeDef,
     StartJobRunRequestRequestTypeDef,
+    JobTemplateDataOutputTypeDef,
     JobTemplateDataTypeDef,
     DescribeVirtualClusterResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     ListJobRunsResponseTypeDef,
-    CreateJobTemplateRequestRequestTypeDef,
     JobTemplateTypeDef,
+    CreateJobTemplateRequestRequestTypeDef,
     DescribeJobTemplateResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
 )
 
 
 def get_structure() -> CancelJobRunRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/__init__.py` & `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/__init__.pyi` & `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/__main__.py` & `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRContainers 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.EMRContainers 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers\nOther"
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

### Comparing `mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/client.py` & `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/client.pyi` & `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/literals.py` & `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,15 @@
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
@@ -258,26 +259,28 @@
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

### Comparing `mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/literals.pyi` & `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,15 @@
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
@@ -256,26 +257,28 @@
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

### Comparing `mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/paginator.py` & `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/paginator.pyi` & `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/type_defs.py` & `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/type_defs.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -29,22 +29,25 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelJobRunRequestRequestTypeDef",
     "CancelJobRunResponseTypeDef",
     "CertificateTypeDef",
+    "CloudWatchMonitoringConfigurationOutputTypeDef",
     "CloudWatchMonitoringConfigurationTypeDef",
+    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
+    "EksInfoOutputTypeDef",
     "EksInfoTypeDef",
+    "ContainerLogRotationConfigurationOutputTypeDef",
     "ContainerLogRotationConfigurationTypeDef",
     "CreateJobTemplateResponseTypeDef",
     "CreateManagedEndpointResponseTypeDef",
     "CreateVirtualClusterResponseTypeDef",
     "CredentialsTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeleteJobTemplateResponseTypeDef",
@@ -53,60 +56,75 @@
     "DeleteVirtualClusterRequestRequestTypeDef",
     "DeleteVirtualClusterResponseTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
     "DescribeManagedEndpointRequestRequestTypeDef",
     "DescribeVirtualClusterRequestRequestTypeDef",
     "GetManagedEndpointSessionCredentialsRequestRequestTypeDef",
+    "SparkSqlJobDriverOutputTypeDef",
+    "SparkSubmitJobDriverOutputTypeDef",
     "SparkSqlJobDriverTypeDef",
     "SparkSubmitJobDriverTypeDef",
-    "RetryPolicyConfigurationTypeDef",
+    "RetryPolicyConfigurationOutputTypeDef",
     "RetryPolicyExecutionTypeDef",
+    "TemplateParameterConfigurationOutputTypeDef",
     "TemplateParameterConfigurationTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
     "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     "ListManagedEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     "ListVirtualClustersRequestRequestTypeDef",
+    "S3MonitoringConfigurationOutputTypeDef",
     "S3MonitoringConfigurationTypeDef",
     "PaginatorConfigTypeDef",
+    "ParametricCloudWatchMonitoringConfigurationOutputTypeDef",
     "ParametricCloudWatchMonitoringConfigurationTypeDef",
+    "ParametricS3MonitoringConfigurationOutputTypeDef",
     "ParametricS3MonitoringConfigurationTypeDef",
     "ResponseMetadataTypeDef",
+    "RetryPolicyConfigurationTypeDef",
     "StartJobRunResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "ContainerInfoOutputTypeDef",
     "ContainerInfoTypeDef",
     "GetManagedEndpointSessionCredentialsResponseTypeDef",
+    "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
+    "MonitoringConfigurationOutputTypeDef",
     "MonitoringConfigurationTypeDef",
+    "ParametricMonitoringConfigurationOutputTypeDef",
     "ParametricMonitoringConfigurationTypeDef",
+    "ContainerProviderOutputTypeDef",
     "ContainerProviderTypeDef",
+    "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
+    "ParametricConfigurationOverridesOutputTypeDef",
     "ParametricConfigurationOverridesTypeDef",
-    "CreateVirtualClusterRequestRequestTypeDef",
     "VirtualClusterTypeDef",
-    "CreateManagedEndpointRequestRequestTypeDef",
+    "CreateVirtualClusterRequestRequestTypeDef",
     "EndpointTypeDef",
     "JobRunTypeDef",
+    "CreateManagedEndpointRequestRequestTypeDef",
     "StartJobRunRequestRequestTypeDef",
+    "JobTemplateDataOutputTypeDef",
     "JobTemplateDataTypeDef",
     "DescribeVirtualClusterResponseTypeDef",
     "ListVirtualClustersResponseTypeDef",
     "DescribeManagedEndpointResponseTypeDef",
     "ListManagedEndpointsResponseTypeDef",
     "DescribeJobRunResponseTypeDef",
     "ListJobRunsResponseTypeDef",
-    "CreateJobTemplateRequestRequestTypeDef",
     "JobTemplateTypeDef",
+    "CreateJobTemplateRequestRequestTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
 )
 
 CancelJobRunRequestRequestTypeDef = TypedDict(
     "CancelJobRunRequestRequestTypeDef",
     {
@@ -129,35 +147,73 @@
     {
         "certificateArn": str,
         "certificateData": str,
     },
     total=False,
 )
 
+_RequiredCloudWatchMonitoringConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCloudWatchMonitoringConfigurationOutputTypeDef",
+    {
+        "logGroupName": str,
+    },
+)
+_OptionalCloudWatchMonitoringConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCloudWatchMonitoringConfigurationOutputTypeDef",
+    {
+        "logStreamNamePrefix": str,
+    },
+    total=False,
+)
+
+class CloudWatchMonitoringConfigurationOutputTypeDef(
+    _RequiredCloudWatchMonitoringConfigurationOutputTypeDef,
+    _OptionalCloudWatchMonitoringConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredCloudWatchMonitoringConfigurationTypeDef = TypedDict(
     "_RequiredCloudWatchMonitoringConfigurationTypeDef",
     {
         "logGroupName": str,
     },
 )
 _OptionalCloudWatchMonitoringConfigurationTypeDef = TypedDict(
     "_OptionalCloudWatchMonitoringConfigurationTypeDef",
     {
         "logStreamNamePrefix": str,
     },
     total=False,
 )
 
-
 class CloudWatchMonitoringConfigurationTypeDef(
     _RequiredCloudWatchMonitoringConfigurationTypeDef,
     _OptionalCloudWatchMonitoringConfigurationTypeDef,
 ):
     pass
 
+_RequiredConfigurationOutputTypeDef = TypedDict(
+    "_RequiredConfigurationOutputTypeDef",
+    {
+        "classification": str,
+    },
+)
+_OptionalConfigurationOutputTypeDef = TypedDict(
+    "_OptionalConfigurationOutputTypeDef",
+    {
+        "properties": Dict[str, str],
+        "configurations": List[Dict[str, Any]],
+    },
+    total=False,
+)
+
+class ConfigurationOutputTypeDef(
+    _RequiredConfigurationOutputTypeDef, _OptionalConfigurationOutputTypeDef
+):
+    pass
 
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
@@ -166,27 +222,41 @@
     {
         "properties": Mapping[str, str],
         "configurations": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
+EksInfoOutputTypeDef = TypedDict(
+    "EksInfoOutputTypeDef",
+    {
+        "namespace": str,
+    },
+    total=False,
+)
 
 EksInfoTypeDef = TypedDict(
     "EksInfoTypeDef",
     {
         "namespace": str,
     },
     total=False,
 )
 
+ContainerLogRotationConfigurationOutputTypeDef = TypedDict(
+    "ContainerLogRotationConfigurationOutputTypeDef",
+    {
+        "rotationSize": str,
+        "maxFilesToKeep": int,
+    },
+)
+
 ContainerLogRotationConfigurationTypeDef = TypedDict(
     "ContainerLogRotationConfigurationTypeDef",
     {
         "rotationSize": str,
         "maxFilesToKeep": int,
     },
 )
@@ -323,21 +393,48 @@
         "durationInSeconds": int,
         "logContext": str,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class GetManagedEndpointSessionCredentialsRequestRequestTypeDef(
     _RequiredGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
     _OptionalGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
 ):
     pass
 
+SparkSqlJobDriverOutputTypeDef = TypedDict(
+    "SparkSqlJobDriverOutputTypeDef",
+    {
+        "entryPoint": str,
+        "sparkSqlParameters": str,
+    },
+    total=False,
+)
+
+_RequiredSparkSubmitJobDriverOutputTypeDef = TypedDict(
+    "_RequiredSparkSubmitJobDriverOutputTypeDef",
+    {
+        "entryPoint": str,
+    },
+)
+_OptionalSparkSubmitJobDriverOutputTypeDef = TypedDict(
+    "_OptionalSparkSubmitJobDriverOutputTypeDef",
+    {
+        "entryPointArguments": List[str],
+        "sparkSubmitParameters": str,
+    },
+    total=False,
+)
+
+class SparkSubmitJobDriverOutputTypeDef(
+    _RequiredSparkSubmitJobDriverOutputTypeDef, _OptionalSparkSubmitJobDriverOutputTypeDef
+):
+    pass
 
 SparkSqlJobDriverTypeDef = TypedDict(
     "SparkSqlJobDriverTypeDef",
     {
         "entryPoint": str,
         "sparkSqlParameters": str,
     },
@@ -355,35 +452,42 @@
     {
         "entryPointArguments": Sequence[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
-
 class SparkSubmitJobDriverTypeDef(
     _RequiredSparkSubmitJobDriverTypeDef, _OptionalSparkSubmitJobDriverTypeDef
 ):
     pass
 
-
-RetryPolicyConfigurationTypeDef = TypedDict(
-    "RetryPolicyConfigurationTypeDef",
+RetryPolicyConfigurationOutputTypeDef = TypedDict(
+    "RetryPolicyConfigurationOutputTypeDef",
     {
         "maxAttempts": int,
     },
 )
 
 RetryPolicyExecutionTypeDef = TypedDict(
     "RetryPolicyExecutionTypeDef",
     {
         "currentAttemptCount": int,
     },
 )
 
+TemplateParameterConfigurationOutputTypeDef = TypedDict(
+    "TemplateParameterConfigurationOutputTypeDef",
+    {
+        "type": TemplateParameterDataTypeType,
+        "defaultValue": str,
+    },
+    total=False,
+)
+
 TemplateParameterConfigurationTypeDef = TypedDict(
     "TemplateParameterConfigurationTypeDef",
     {
         "type": TemplateParameterDataTypeType,
         "defaultValue": str,
     },
     total=False,
@@ -403,22 +507,20 @@
         "name": str,
         "states": Sequence[JobRunStateType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListJobRunsRequestListJobRunsPaginateTypeDef(
     _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
     _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -430,21 +532,19 @@
         "states": Sequence[JobRunStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
-
 ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     {
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -476,22 +576,20 @@
         "types": Sequence[str],
         "states": Sequence[EndpointStateType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
     _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListManagedEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListManagedEndpointsRequestRequestTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListManagedEndpointsRequestRequestTypeDef = TypedDict(
@@ -503,22 +601,20 @@
         "states": Sequence[EndpointStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListManagedEndpointsRequestRequestTypeDef(
     _RequiredListManagedEndpointsRequestRequestTypeDef,
     _OptionalListManagedEndpointsRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -553,14 +649,21 @@
         "states": Sequence[VirtualClusterStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+S3MonitoringConfigurationOutputTypeDef = TypedDict(
+    "S3MonitoringConfigurationOutputTypeDef",
+    {
+        "logUri": str,
+    },
+)
+
 S3MonitoringConfigurationTypeDef = TypedDict(
     "S3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
     },
 )
 
@@ -570,23 +673,40 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ParametricCloudWatchMonitoringConfigurationOutputTypeDef = TypedDict(
+    "ParametricCloudWatchMonitoringConfigurationOutputTypeDef",
+    {
+        "logGroupName": str,
+        "logStreamNamePrefix": str,
+    },
+    total=False,
+)
+
 ParametricCloudWatchMonitoringConfigurationTypeDef = TypedDict(
     "ParametricCloudWatchMonitoringConfigurationTypeDef",
     {
         "logGroupName": str,
         "logStreamNamePrefix": str,
     },
     total=False,
 )
 
+ParametricS3MonitoringConfigurationOutputTypeDef = TypedDict(
+    "ParametricS3MonitoringConfigurationOutputTypeDef",
+    {
+        "logUri": str,
+    },
+    total=False,
+)
+
 ParametricS3MonitoringConfigurationTypeDef = TypedDict(
     "ParametricS3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
     },
     total=False,
 )
@@ -598,14 +718,21 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+RetryPolicyConfigurationTypeDef = TypedDict(
+    "RetryPolicyConfigurationTypeDef",
+    {
+        "maxAttempts": int,
+    },
+)
+
 StartJobRunResponseTypeDef = TypedDict(
     "StartJobRunResponseTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "virtualClusterId": str,
@@ -625,14 +752,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+ContainerInfoOutputTypeDef = TypedDict(
+    "ContainerInfoOutputTypeDef",
+    {
+        "eksInfo": EksInfoOutputTypeDef,
+    },
+    total=False,
+)
+
 ContainerInfoTypeDef = TypedDict(
     "ContainerInfoTypeDef",
     {
         "eksInfo": EksInfoTypeDef,
     },
     total=False,
 )
@@ -643,44 +778,96 @@
         "id": str,
         "credentials": CredentialsTypeDef,
         "expiresAt": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+JobDriverOutputTypeDef = TypedDict(
+    "JobDriverOutputTypeDef",
+    {
+        "sparkSubmitJobDriver": SparkSubmitJobDriverOutputTypeDef,
+        "sparkSqlJobDriver": SparkSqlJobDriverOutputTypeDef,
+    },
+    total=False,
+)
+
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmitJobDriver": SparkSubmitJobDriverTypeDef,
         "sparkSqlJobDriver": SparkSqlJobDriverTypeDef,
     },
     total=False,
 )
 
+MonitoringConfigurationOutputTypeDef = TypedDict(
+    "MonitoringConfigurationOutputTypeDef",
+    {
+        "persistentAppUI": PersistentAppUIType,
+        "cloudWatchMonitoringConfiguration": CloudWatchMonitoringConfigurationOutputTypeDef,
+        "s3MonitoringConfiguration": S3MonitoringConfigurationOutputTypeDef,
+        "containerLogRotationConfiguration": ContainerLogRotationConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "persistentAppUI": PersistentAppUIType,
         "cloudWatchMonitoringConfiguration": CloudWatchMonitoringConfigurationTypeDef,
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "containerLogRotationConfiguration": ContainerLogRotationConfigurationTypeDef,
     },
     total=False,
 )
 
+ParametricMonitoringConfigurationOutputTypeDef = TypedDict(
+    "ParametricMonitoringConfigurationOutputTypeDef",
+    {
+        "persistentAppUI": str,
+        "cloudWatchMonitoringConfiguration": (
+            ParametricCloudWatchMonitoringConfigurationOutputTypeDef
+        ),
+        "s3MonitoringConfiguration": ParametricS3MonitoringConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ParametricMonitoringConfigurationTypeDef = TypedDict(
     "ParametricMonitoringConfigurationTypeDef",
     {
         "persistentAppUI": str,
         "cloudWatchMonitoringConfiguration": ParametricCloudWatchMonitoringConfigurationTypeDef,
         "s3MonitoringConfiguration": ParametricS3MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredContainerProviderOutputTypeDef = TypedDict(
+    "_RequiredContainerProviderOutputTypeDef",
+    {
+        "type": Literal["EKS"],
+        "id": str,
+    },
+)
+_OptionalContainerProviderOutputTypeDef = TypedDict(
+    "_OptionalContainerProviderOutputTypeDef",
+    {
+        "info": ContainerInfoOutputTypeDef,
+    },
+    total=False,
+)
+
+class ContainerProviderOutputTypeDef(
+    _RequiredContainerProviderOutputTypeDef, _OptionalContainerProviderOutputTypeDef
+):
+    pass
+
 _RequiredContainerProviderTypeDef = TypedDict(
     "_RequiredContainerProviderTypeDef",
     {
         "type": Literal["EKS"],
         "id": str,
     },
 )
@@ -688,120 +875,105 @@
     "_OptionalContainerProviderTypeDef",
     {
         "info": ContainerInfoTypeDef,
     },
     total=False,
 )
 
-
 class ContainerProviderTypeDef(
     _RequiredContainerProviderTypeDef, _OptionalContainerProviderTypeDef
 ):
     pass
 
+ConfigurationOverridesOutputTypeDef = TypedDict(
+    "ConfigurationOverridesOutputTypeDef",
+    {
+        "applicationConfiguration": List["ConfigurationOutputTypeDef"],
+        "monitoringConfiguration": MonitoringConfigurationOutputTypeDef,
+    },
+    total=False,
+)
 
 ConfigurationOverridesTypeDef = TypedDict(
     "ConfigurationOverridesTypeDef",
     {
         "applicationConfiguration": Sequence["ConfigurationTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
-ParametricConfigurationOverridesTypeDef = TypedDict(
-    "ParametricConfigurationOverridesTypeDef",
+ParametricConfigurationOverridesOutputTypeDef = TypedDict(
+    "ParametricConfigurationOverridesOutputTypeDef",
     {
-        "applicationConfiguration": Sequence["ConfigurationTypeDef"],
-        "monitoringConfiguration": ParametricMonitoringConfigurationTypeDef,
+        "applicationConfiguration": List["ConfigurationOutputTypeDef"],
+        "monitoringConfiguration": ParametricMonitoringConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateVirtualClusterRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVirtualClusterRequestRequestTypeDef",
-    {
-        "name": str,
-        "containerProvider": ContainerProviderTypeDef,
-        "clientToken": str,
-    },
-)
-_OptionalCreateVirtualClusterRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVirtualClusterRequestRequestTypeDef",
+ParametricConfigurationOverridesTypeDef = TypedDict(
+    "ParametricConfigurationOverridesTypeDef",
     {
-        "tags": Mapping[str, str],
+        "applicationConfiguration": Sequence["ConfigurationTypeDef"],
+        "monitoringConfiguration": ParametricMonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class CreateVirtualClusterRequestRequestTypeDef(
-    _RequiredCreateVirtualClusterRequestRequestTypeDef,
-    _OptionalCreateVirtualClusterRequestRequestTypeDef,
-):
-    pass
-
-
 VirtualClusterTypeDef = TypedDict(
     "VirtualClusterTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "state": VirtualClusterStateType,
-        "containerProvider": ContainerProviderTypeDef,
+        "containerProvider": ContainerProviderOutputTypeDef,
         "createdAt": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredCreateManagedEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateManagedEndpointRequestRequestTypeDef",
+_RequiredCreateVirtualClusterRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVirtualClusterRequestRequestTypeDef",
     {
         "name": str,
-        "virtualClusterId": str,
-        "type": str,
-        "releaseLabel": str,
-        "executionRoleArn": str,
+        "containerProvider": ContainerProviderTypeDef,
         "clientToken": str,
     },
 )
-_OptionalCreateManagedEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateManagedEndpointRequestRequestTypeDef",
+_OptionalCreateVirtualClusterRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVirtualClusterRequestRequestTypeDef",
     {
-        "certificateArn": str,
-        "configurationOverrides": ConfigurationOverridesTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
-class CreateManagedEndpointRequestRequestTypeDef(
-    _RequiredCreateManagedEndpointRequestRequestTypeDef,
-    _OptionalCreateManagedEndpointRequestRequestTypeDef,
+class CreateVirtualClusterRequestRequestTypeDef(
+    _RequiredCreateVirtualClusterRequestRequestTypeDef,
+    _OptionalCreateVirtualClusterRequestRequestTypeDef,
 ):
     pass
 
-
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "virtualClusterId": str,
         "type": str,
         "state": EndpointStateType,
         "releaseLabel": str,
         "executionRoleArn": str,
         "certificateArn": str,
         "certificateAuthority": CertificateTypeDef,
-        "configurationOverrides": ConfigurationOverridesTypeDef,
+        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
         "serverUrl": str,
         "createdAt": datetime,
         "securityGroup": str,
         "subnetIds": List[str],
         "stateDetails": str,
         "failureReason": FailureReasonType,
         "tags": Dict[str, str],
@@ -816,28 +988,55 @@
         "name": str,
         "virtualClusterId": str,
         "arn": str,
         "state": JobRunStateType,
         "clientToken": str,
         "executionRoleArn": str,
         "releaseLabel": str,
-        "configurationOverrides": ConfigurationOverridesTypeDef,
-        "jobDriver": JobDriverTypeDef,
+        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
+        "jobDriver": JobDriverOutputTypeDef,
         "createdAt": datetime,
         "createdBy": str,
         "finishedAt": datetime,
         "stateDetails": str,
         "failureReason": FailureReasonType,
         "tags": Dict[str, str],
-        "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
+        "retryPolicyConfiguration": RetryPolicyConfigurationOutputTypeDef,
         "retryPolicyExecution": RetryPolicyExecutionTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateManagedEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateManagedEndpointRequestRequestTypeDef",
+    {
+        "name": str,
+        "virtualClusterId": str,
+        "type": str,
+        "releaseLabel": str,
+        "executionRoleArn": str,
+        "clientToken": str,
+    },
+)
+_OptionalCreateManagedEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateManagedEndpointRequestRequestTypeDef",
+    {
+        "certificateArn": str,
+        "configurationOverrides": ConfigurationOverridesTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateManagedEndpointRequestRequestTypeDef(
+    _RequiredCreateManagedEndpointRequestRequestTypeDef,
+    _OptionalCreateManagedEndpointRequestRequestTypeDef,
+):
+    pass
+
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "virtualClusterId": str,
         "clientToken": str,
     },
 )
@@ -853,20 +1052,41 @@
         "jobTemplateId": str,
         "jobTemplateParameters": Mapping[str, str],
         "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
+_RequiredJobTemplateDataOutputTypeDef = TypedDict(
+    "_RequiredJobTemplateDataOutputTypeDef",
+    {
+        "executionRoleArn": str,
+        "releaseLabel": str,
+        "jobDriver": JobDriverOutputTypeDef,
+    },
+)
+_OptionalJobTemplateDataOutputTypeDef = TypedDict(
+    "_OptionalJobTemplateDataOutputTypeDef",
+    {
+        "configurationOverrides": ParametricConfigurationOverridesOutputTypeDef,
+        "parameterConfiguration": Dict[str, TemplateParameterConfigurationOutputTypeDef],
+        "jobTags": Dict[str, str],
+    },
+    total=False,
+)
+
+class JobTemplateDataOutputTypeDef(
+    _RequiredJobTemplateDataOutputTypeDef, _OptionalJobTemplateDataOutputTypeDef
+):
+    pass
 
 _RequiredJobTemplateDataTypeDef = TypedDict(
     "_RequiredJobTemplateDataTypeDef",
     {
         "executionRoleArn": str,
         "releaseLabel": str,
         "jobDriver": JobDriverTypeDef,
@@ -878,19 +1098,17 @@
         "configurationOverrides": ParametricConfigurationOverridesTypeDef,
         "parameterConfiguration": Mapping[str, TemplateParameterConfigurationTypeDef],
         "jobTags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class JobTemplateDataTypeDef(_RequiredJobTemplateDataTypeDef, _OptionalJobTemplateDataTypeDef):
     pass
 
-
 DescribeVirtualClusterResponseTypeDef = TypedDict(
     "DescribeVirtualClusterResponseTypeDef",
     {
         "virtualCluster": VirtualClusterTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -934,42 +1152,18 @@
     {
         "jobRuns": List[JobRunTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobTemplateRequestRequestTypeDef",
-    {
-        "name": str,
-        "clientToken": str,
-        "jobTemplateData": JobTemplateDataTypeDef,
-    },
-)
-_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobTemplateRequestRequestTypeDef",
-    {
-        "tags": Mapping[str, str],
-        "kmsKeyArn": str,
-    },
-    total=False,
-)
-
-
-class CreateJobTemplateRequestRequestTypeDef(
-    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredJobTemplateTypeDef = TypedDict(
     "_RequiredJobTemplateTypeDef",
     {
-        "jobTemplateData": JobTemplateDataTypeDef,
+        "jobTemplateData": JobTemplateDataOutputTypeDef,
     },
 )
 _OptionalJobTemplateTypeDef = TypedDict(
     "_OptionalJobTemplateTypeDef",
     {
         "name": str,
         "id": str,
@@ -979,18 +1173,38 @@
         "tags": Dict[str, str],
         "kmsKeyArn": str,
         "decryptionError": str,
     },
     total=False,
 )
 
-
 class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
     pass
 
+_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobTemplateRequestRequestTypeDef",
+    {
+        "name": str,
+        "clientToken": str,
+        "jobTemplateData": JobTemplateDataTypeDef,
+    },
+)
+_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobTemplateRequestRequestTypeDef",
+    {
+        "tags": Mapping[str, str],
+        "kmsKeyArn": str,
+    },
+    total=False,
+)
+
+class CreateJobTemplateRequestRequestTypeDef(
+    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
+):
+    pass
 
 DescribeJobTemplateResponseTypeDef = TypedDict(
     "DescribeJobTemplateResponseTypeDef",
     {
         "jobTemplate": JobTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers/type_defs.pyi` & `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers/type_defs.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,21 +29,26 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CancelJobRunRequestRequestTypeDef",
     "CancelJobRunResponseTypeDef",
     "CertificateTypeDef",
+    "CloudWatchMonitoringConfigurationOutputTypeDef",
     "CloudWatchMonitoringConfigurationTypeDef",
+    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
+    "EksInfoOutputTypeDef",
     "EksInfoTypeDef",
+    "ContainerLogRotationConfigurationOutputTypeDef",
     "ContainerLogRotationConfigurationTypeDef",
     "CreateJobTemplateResponseTypeDef",
     "CreateManagedEndpointResponseTypeDef",
     "CreateVirtualClusterResponseTypeDef",
     "CredentialsTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeleteJobTemplateResponseTypeDef",
@@ -52,60 +57,75 @@
     "DeleteVirtualClusterRequestRequestTypeDef",
     "DeleteVirtualClusterResponseTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
     "DescribeManagedEndpointRequestRequestTypeDef",
     "DescribeVirtualClusterRequestRequestTypeDef",
     "GetManagedEndpointSessionCredentialsRequestRequestTypeDef",
+    "SparkSqlJobDriverOutputTypeDef",
+    "SparkSubmitJobDriverOutputTypeDef",
     "SparkSqlJobDriverTypeDef",
     "SparkSubmitJobDriverTypeDef",
-    "RetryPolicyConfigurationTypeDef",
+    "RetryPolicyConfigurationOutputTypeDef",
     "RetryPolicyExecutionTypeDef",
+    "TemplateParameterConfigurationOutputTypeDef",
     "TemplateParameterConfigurationTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
     "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     "ListManagedEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     "ListVirtualClustersRequestRequestTypeDef",
+    "S3MonitoringConfigurationOutputTypeDef",
     "S3MonitoringConfigurationTypeDef",
     "PaginatorConfigTypeDef",
+    "ParametricCloudWatchMonitoringConfigurationOutputTypeDef",
     "ParametricCloudWatchMonitoringConfigurationTypeDef",
+    "ParametricS3MonitoringConfigurationOutputTypeDef",
     "ParametricS3MonitoringConfigurationTypeDef",
     "ResponseMetadataTypeDef",
+    "RetryPolicyConfigurationTypeDef",
     "StartJobRunResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "ContainerInfoOutputTypeDef",
     "ContainerInfoTypeDef",
     "GetManagedEndpointSessionCredentialsResponseTypeDef",
+    "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
+    "MonitoringConfigurationOutputTypeDef",
     "MonitoringConfigurationTypeDef",
+    "ParametricMonitoringConfigurationOutputTypeDef",
     "ParametricMonitoringConfigurationTypeDef",
+    "ContainerProviderOutputTypeDef",
     "ContainerProviderTypeDef",
+    "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
+    "ParametricConfigurationOverridesOutputTypeDef",
     "ParametricConfigurationOverridesTypeDef",
-    "CreateVirtualClusterRequestRequestTypeDef",
     "VirtualClusterTypeDef",
-    "CreateManagedEndpointRequestRequestTypeDef",
+    "CreateVirtualClusterRequestRequestTypeDef",
     "EndpointTypeDef",
     "JobRunTypeDef",
+    "CreateManagedEndpointRequestRequestTypeDef",
     "StartJobRunRequestRequestTypeDef",
+    "JobTemplateDataOutputTypeDef",
     "JobTemplateDataTypeDef",
     "DescribeVirtualClusterResponseTypeDef",
     "ListVirtualClustersResponseTypeDef",
     "DescribeManagedEndpointResponseTypeDef",
     "ListManagedEndpointsResponseTypeDef",
     "DescribeJobRunResponseTypeDef",
     "ListJobRunsResponseTypeDef",
-    "CreateJobTemplateRequestRequestTypeDef",
     "JobTemplateTypeDef",
+    "CreateJobTemplateRequestRequestTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
 )
 
 CancelJobRunRequestRequestTypeDef = TypedDict(
     "CancelJobRunRequestRequestTypeDef",
     {
@@ -128,34 +148,80 @@
     {
         "certificateArn": str,
         "certificateData": str,
     },
     total=False,
 )
 
+_RequiredCloudWatchMonitoringConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCloudWatchMonitoringConfigurationOutputTypeDef",
+    {
+        "logGroupName": str,
+    },
+)
+_OptionalCloudWatchMonitoringConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCloudWatchMonitoringConfigurationOutputTypeDef",
+    {
+        "logStreamNamePrefix": str,
+    },
+    total=False,
+)
+
+
+class CloudWatchMonitoringConfigurationOutputTypeDef(
+    _RequiredCloudWatchMonitoringConfigurationOutputTypeDef,
+    _OptionalCloudWatchMonitoringConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredCloudWatchMonitoringConfigurationTypeDef = TypedDict(
     "_RequiredCloudWatchMonitoringConfigurationTypeDef",
     {
         "logGroupName": str,
     },
 )
 _OptionalCloudWatchMonitoringConfigurationTypeDef = TypedDict(
     "_OptionalCloudWatchMonitoringConfigurationTypeDef",
     {
         "logStreamNamePrefix": str,
     },
     total=False,
 )
 
+
 class CloudWatchMonitoringConfigurationTypeDef(
     _RequiredCloudWatchMonitoringConfigurationTypeDef,
     _OptionalCloudWatchMonitoringConfigurationTypeDef,
 ):
     pass
 
+
+_RequiredConfigurationOutputTypeDef = TypedDict(
+    "_RequiredConfigurationOutputTypeDef",
+    {
+        "classification": str,
+    },
+)
+_OptionalConfigurationOutputTypeDef = TypedDict(
+    "_OptionalConfigurationOutputTypeDef",
+    {
+        "properties": Dict[str, str],
+        "configurations": List[Dict[str, Any]],
+    },
+    total=False,
+)
+
+
+class ConfigurationOutputTypeDef(
+    _RequiredConfigurationOutputTypeDef, _OptionalConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationTypeDef = TypedDict(
@@ -163,25 +229,43 @@
     {
         "properties": Mapping[str, str],
         "configurations": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
+
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
+
+EksInfoOutputTypeDef = TypedDict(
+    "EksInfoOutputTypeDef",
+    {
+        "namespace": str,
+    },
+    total=False,
+)
+
 EksInfoTypeDef = TypedDict(
     "EksInfoTypeDef",
     {
         "namespace": str,
     },
     total=False,
 )
 
+ContainerLogRotationConfigurationOutputTypeDef = TypedDict(
+    "ContainerLogRotationConfigurationOutputTypeDef",
+    {
+        "rotationSize": str,
+        "maxFilesToKeep": int,
+    },
+)
+
 ContainerLogRotationConfigurationTypeDef = TypedDict(
     "ContainerLogRotationConfigurationTypeDef",
     {
         "rotationSize": str,
         "maxFilesToKeep": int,
     },
 )
@@ -318,20 +402,53 @@
         "durationInSeconds": int,
         "logContext": str,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class GetManagedEndpointSessionCredentialsRequestRequestTypeDef(
     _RequiredGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
     _OptionalGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
 ):
     pass
 
+
+SparkSqlJobDriverOutputTypeDef = TypedDict(
+    "SparkSqlJobDriverOutputTypeDef",
+    {
+        "entryPoint": str,
+        "sparkSqlParameters": str,
+    },
+    total=False,
+)
+
+_RequiredSparkSubmitJobDriverOutputTypeDef = TypedDict(
+    "_RequiredSparkSubmitJobDriverOutputTypeDef",
+    {
+        "entryPoint": str,
+    },
+)
+_OptionalSparkSubmitJobDriverOutputTypeDef = TypedDict(
+    "_OptionalSparkSubmitJobDriverOutputTypeDef",
+    {
+        "entryPointArguments": List[str],
+        "sparkSubmitParameters": str,
+    },
+    total=False,
+)
+
+
+class SparkSubmitJobDriverOutputTypeDef(
+    _RequiredSparkSubmitJobDriverOutputTypeDef, _OptionalSparkSubmitJobDriverOutputTypeDef
+):
+    pass
+
+
 SparkSqlJobDriverTypeDef = TypedDict(
     "SparkSqlJobDriverTypeDef",
     {
         "entryPoint": str,
         "sparkSqlParameters": str,
     },
     total=False,
@@ -348,33 +465,44 @@
     {
         "entryPointArguments": Sequence[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
+
 class SparkSubmitJobDriverTypeDef(
     _RequiredSparkSubmitJobDriverTypeDef, _OptionalSparkSubmitJobDriverTypeDef
 ):
     pass
 
-RetryPolicyConfigurationTypeDef = TypedDict(
-    "RetryPolicyConfigurationTypeDef",
+
+RetryPolicyConfigurationOutputTypeDef = TypedDict(
+    "RetryPolicyConfigurationOutputTypeDef",
     {
         "maxAttempts": int,
     },
 )
 
 RetryPolicyExecutionTypeDef = TypedDict(
     "RetryPolicyExecutionTypeDef",
     {
         "currentAttemptCount": int,
     },
 )
 
+TemplateParameterConfigurationOutputTypeDef = TypedDict(
+    "TemplateParameterConfigurationOutputTypeDef",
+    {
+        "type": TemplateParameterDataTypeType,
+        "defaultValue": str,
+    },
+    total=False,
+)
+
 TemplateParameterConfigurationTypeDef = TypedDict(
     "TemplateParameterConfigurationTypeDef",
     {
         "type": TemplateParameterDataTypeType,
         "defaultValue": str,
     },
     total=False,
@@ -394,20 +522,22 @@
         "name": str,
         "states": Sequence[JobRunStateType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListJobRunsRequestListJobRunsPaginateTypeDef(
     _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
     _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -419,19 +549,21 @@
         "states": Sequence[JobRunStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
+
 ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     {
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -463,20 +595,22 @@
         "types": Sequence[str],
         "states": Sequence[EndpointStateType],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
     _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListManagedEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListManagedEndpointsRequestRequestTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListManagedEndpointsRequestRequestTypeDef = TypedDict(
@@ -488,20 +622,22 @@
         "states": Sequence[EndpointStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListManagedEndpointsRequestRequestTypeDef(
     _RequiredListManagedEndpointsRequestRequestTypeDef,
     _OptionalListManagedEndpointsRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -536,14 +672,21 @@
         "states": Sequence[VirtualClusterStateType],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+S3MonitoringConfigurationOutputTypeDef = TypedDict(
+    "S3MonitoringConfigurationOutputTypeDef",
+    {
+        "logUri": str,
+    },
+)
+
 S3MonitoringConfigurationTypeDef = TypedDict(
     "S3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
     },
 )
 
@@ -553,23 +696,40 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ParametricCloudWatchMonitoringConfigurationOutputTypeDef = TypedDict(
+    "ParametricCloudWatchMonitoringConfigurationOutputTypeDef",
+    {
+        "logGroupName": str,
+        "logStreamNamePrefix": str,
+    },
+    total=False,
+)
+
 ParametricCloudWatchMonitoringConfigurationTypeDef = TypedDict(
     "ParametricCloudWatchMonitoringConfigurationTypeDef",
     {
         "logGroupName": str,
         "logStreamNamePrefix": str,
     },
     total=False,
 )
 
+ParametricS3MonitoringConfigurationOutputTypeDef = TypedDict(
+    "ParametricS3MonitoringConfigurationOutputTypeDef",
+    {
+        "logUri": str,
+    },
+    total=False,
+)
+
 ParametricS3MonitoringConfigurationTypeDef = TypedDict(
     "ParametricS3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
     },
     total=False,
 )
@@ -581,14 +741,21 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+RetryPolicyConfigurationTypeDef = TypedDict(
+    "RetryPolicyConfigurationTypeDef",
+    {
+        "maxAttempts": int,
+    },
+)
+
 StartJobRunResponseTypeDef = TypedDict(
     "StartJobRunResponseTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "virtualClusterId": str,
@@ -608,14 +775,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+ContainerInfoOutputTypeDef = TypedDict(
+    "ContainerInfoOutputTypeDef",
+    {
+        "eksInfo": EksInfoOutputTypeDef,
+    },
+    total=False,
+)
+
 ContainerInfoTypeDef = TypedDict(
     "ContainerInfoTypeDef",
     {
         "eksInfo": EksInfoTypeDef,
     },
     total=False,
 )
@@ -626,44 +801,98 @@
         "id": str,
         "credentials": CredentialsTypeDef,
         "expiresAt": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+JobDriverOutputTypeDef = TypedDict(
+    "JobDriverOutputTypeDef",
+    {
+        "sparkSubmitJobDriver": SparkSubmitJobDriverOutputTypeDef,
+        "sparkSqlJobDriver": SparkSqlJobDriverOutputTypeDef,
+    },
+    total=False,
+)
+
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmitJobDriver": SparkSubmitJobDriverTypeDef,
         "sparkSqlJobDriver": SparkSqlJobDriverTypeDef,
     },
     total=False,
 )
 
+MonitoringConfigurationOutputTypeDef = TypedDict(
+    "MonitoringConfigurationOutputTypeDef",
+    {
+        "persistentAppUI": PersistentAppUIType,
+        "cloudWatchMonitoringConfiguration": CloudWatchMonitoringConfigurationOutputTypeDef,
+        "s3MonitoringConfiguration": S3MonitoringConfigurationOutputTypeDef,
+        "containerLogRotationConfiguration": ContainerLogRotationConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "persistentAppUI": PersistentAppUIType,
         "cloudWatchMonitoringConfiguration": CloudWatchMonitoringConfigurationTypeDef,
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "containerLogRotationConfiguration": ContainerLogRotationConfigurationTypeDef,
     },
     total=False,
 )
 
+ParametricMonitoringConfigurationOutputTypeDef = TypedDict(
+    "ParametricMonitoringConfigurationOutputTypeDef",
+    {
+        "persistentAppUI": str,
+        "cloudWatchMonitoringConfiguration": (
+            ParametricCloudWatchMonitoringConfigurationOutputTypeDef
+        ),
+        "s3MonitoringConfiguration": ParametricS3MonitoringConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ParametricMonitoringConfigurationTypeDef = TypedDict(
     "ParametricMonitoringConfigurationTypeDef",
     {
         "persistentAppUI": str,
         "cloudWatchMonitoringConfiguration": ParametricCloudWatchMonitoringConfigurationTypeDef,
         "s3MonitoringConfiguration": ParametricS3MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredContainerProviderOutputTypeDef = TypedDict(
+    "_RequiredContainerProviderOutputTypeDef",
+    {
+        "type": Literal["EKS"],
+        "id": str,
+    },
+)
+_OptionalContainerProviderOutputTypeDef = TypedDict(
+    "_OptionalContainerProviderOutputTypeDef",
+    {
+        "info": ContainerInfoOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ContainerProviderOutputTypeDef(
+    _RequiredContainerProviderOutputTypeDef, _OptionalContainerProviderOutputTypeDef
+):
+    pass
+
+
 _RequiredContainerProviderTypeDef = TypedDict(
     "_RequiredContainerProviderTypeDef",
     {
         "type": Literal["EKS"],
         "id": str,
     },
 )
@@ -671,114 +900,109 @@
     "_OptionalContainerProviderTypeDef",
     {
         "info": ContainerInfoTypeDef,
     },
     total=False,
 )
 
+
 class ContainerProviderTypeDef(
     _RequiredContainerProviderTypeDef, _OptionalContainerProviderTypeDef
 ):
     pass
 
-ConfigurationOverridesTypeDef = TypedDict(
-    "ConfigurationOverridesTypeDef",
+
+ConfigurationOverridesOutputTypeDef = TypedDict(
+    "ConfigurationOverridesOutputTypeDef",
     {
-        "applicationConfiguration": Sequence["ConfigurationTypeDef"],
-        "monitoringConfiguration": MonitoringConfigurationTypeDef,
+        "applicationConfiguration": List["ConfigurationOutputTypeDef"],
+        "monitoringConfiguration": MonitoringConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-ParametricConfigurationOverridesTypeDef = TypedDict(
-    "ParametricConfigurationOverridesTypeDef",
+ConfigurationOverridesTypeDef = TypedDict(
+    "ConfigurationOverridesTypeDef",
     {
         "applicationConfiguration": Sequence["ConfigurationTypeDef"],
-        "monitoringConfiguration": ParametricMonitoringConfigurationTypeDef,
+        "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateVirtualClusterRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVirtualClusterRequestRequestTypeDef",
+ParametricConfigurationOverridesOutputTypeDef = TypedDict(
+    "ParametricConfigurationOverridesOutputTypeDef",
     {
-        "name": str,
-        "containerProvider": ContainerProviderTypeDef,
-        "clientToken": str,
+        "applicationConfiguration": List["ConfigurationOutputTypeDef"],
+        "monitoringConfiguration": ParametricMonitoringConfigurationOutputTypeDef,
     },
+    total=False,
 )
-_OptionalCreateVirtualClusterRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVirtualClusterRequestRequestTypeDef",
+
+ParametricConfigurationOverridesTypeDef = TypedDict(
+    "ParametricConfigurationOverridesTypeDef",
     {
-        "tags": Mapping[str, str],
+        "applicationConfiguration": Sequence["ConfigurationTypeDef"],
+        "monitoringConfiguration": ParametricMonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
-class CreateVirtualClusterRequestRequestTypeDef(
-    _RequiredCreateVirtualClusterRequestRequestTypeDef,
-    _OptionalCreateVirtualClusterRequestRequestTypeDef,
-):
-    pass
-
 VirtualClusterTypeDef = TypedDict(
     "VirtualClusterTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "state": VirtualClusterStateType,
-        "containerProvider": ContainerProviderTypeDef,
+        "containerProvider": ContainerProviderOutputTypeDef,
         "createdAt": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredCreateManagedEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateManagedEndpointRequestRequestTypeDef",
+_RequiredCreateVirtualClusterRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVirtualClusterRequestRequestTypeDef",
     {
         "name": str,
-        "virtualClusterId": str,
-        "type": str,
-        "releaseLabel": str,
-        "executionRoleArn": str,
+        "containerProvider": ContainerProviderTypeDef,
         "clientToken": str,
     },
 )
-_OptionalCreateManagedEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateManagedEndpointRequestRequestTypeDef",
+_OptionalCreateVirtualClusterRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVirtualClusterRequestRequestTypeDef",
     {
-        "certificateArn": str,
-        "configurationOverrides": ConfigurationOverridesTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class CreateManagedEndpointRequestRequestTypeDef(
-    _RequiredCreateManagedEndpointRequestRequestTypeDef,
-    _OptionalCreateManagedEndpointRequestRequestTypeDef,
+
+class CreateVirtualClusterRequestRequestTypeDef(
+    _RequiredCreateVirtualClusterRequestRequestTypeDef,
+    _OptionalCreateVirtualClusterRequestRequestTypeDef,
 ):
     pass
 
+
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "virtualClusterId": str,
         "type": str,
         "state": EndpointStateType,
         "releaseLabel": str,
         "executionRoleArn": str,
         "certificateArn": str,
         "certificateAuthority": CertificateTypeDef,
-        "configurationOverrides": ConfigurationOverridesTypeDef,
+        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
         "serverUrl": str,
         "createdAt": datetime,
         "securityGroup": str,
         "subnetIds": List[str],
         "stateDetails": str,
         "failureReason": FailureReasonType,
         "tags": Dict[str, str],
@@ -793,28 +1017,57 @@
         "name": str,
         "virtualClusterId": str,
         "arn": str,
         "state": JobRunStateType,
         "clientToken": str,
         "executionRoleArn": str,
         "releaseLabel": str,
-        "configurationOverrides": ConfigurationOverridesTypeDef,
-        "jobDriver": JobDriverTypeDef,
+        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
+        "jobDriver": JobDriverOutputTypeDef,
         "createdAt": datetime,
         "createdBy": str,
         "finishedAt": datetime,
         "stateDetails": str,
         "failureReason": FailureReasonType,
         "tags": Dict[str, str],
-        "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
+        "retryPolicyConfiguration": RetryPolicyConfigurationOutputTypeDef,
         "retryPolicyExecution": RetryPolicyExecutionTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateManagedEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateManagedEndpointRequestRequestTypeDef",
+    {
+        "name": str,
+        "virtualClusterId": str,
+        "type": str,
+        "releaseLabel": str,
+        "executionRoleArn": str,
+        "clientToken": str,
+    },
+)
+_OptionalCreateManagedEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateManagedEndpointRequestRequestTypeDef",
+    {
+        "certificateArn": str,
+        "configurationOverrides": ConfigurationOverridesTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateManagedEndpointRequestRequestTypeDef(
+    _RequiredCreateManagedEndpointRequestRequestTypeDef,
+    _OptionalCreateManagedEndpointRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "virtualClusterId": str,
         "clientToken": str,
     },
 )
@@ -830,19 +1083,46 @@
         "jobTemplateId": str,
         "jobTemplateParameters": Mapping[str, str],
         "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredJobTemplateDataOutputTypeDef = TypedDict(
+    "_RequiredJobTemplateDataOutputTypeDef",
+    {
+        "executionRoleArn": str,
+        "releaseLabel": str,
+        "jobDriver": JobDriverOutputTypeDef,
+    },
+)
+_OptionalJobTemplateDataOutputTypeDef = TypedDict(
+    "_OptionalJobTemplateDataOutputTypeDef",
+    {
+        "configurationOverrides": ParametricConfigurationOverridesOutputTypeDef,
+        "parameterConfiguration": Dict[str, TemplateParameterConfigurationOutputTypeDef],
+        "jobTags": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class JobTemplateDataOutputTypeDef(
+    _RequiredJobTemplateDataOutputTypeDef, _OptionalJobTemplateDataOutputTypeDef
+):
+    pass
+
+
 _RequiredJobTemplateDataTypeDef = TypedDict(
     "_RequiredJobTemplateDataTypeDef",
     {
         "executionRoleArn": str,
         "releaseLabel": str,
         "jobDriver": JobDriverTypeDef,
     },
@@ -853,17 +1133,19 @@
         "configurationOverrides": ParametricConfigurationOverridesTypeDef,
         "parameterConfiguration": Mapping[str, TemplateParameterConfigurationTypeDef],
         "jobTags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class JobTemplateDataTypeDef(_RequiredJobTemplateDataTypeDef, _OptionalJobTemplateDataTypeDef):
     pass
 
+
 DescribeVirtualClusterResponseTypeDef = TypedDict(
     "DescribeVirtualClusterResponseTypeDef",
     {
         "virtualCluster": VirtualClusterTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -907,40 +1189,18 @@
     {
         "jobRuns": List[JobRunTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobTemplateRequestRequestTypeDef",
-    {
-        "name": str,
-        "clientToken": str,
-        "jobTemplateData": JobTemplateDataTypeDef,
-    },
-)
-_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobTemplateRequestRequestTypeDef",
-    {
-        "tags": Mapping[str, str],
-        "kmsKeyArn": str,
-    },
-    total=False,
-)
-
-class CreateJobTemplateRequestRequestTypeDef(
-    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
-):
-    pass
-
 _RequiredJobTemplateTypeDef = TypedDict(
     "_RequiredJobTemplateTypeDef",
     {
-        "jobTemplateData": JobTemplateDataTypeDef,
+        "jobTemplateData": JobTemplateDataOutputTypeDef,
     },
 )
 _OptionalJobTemplateTypeDef = TypedDict(
     "_OptionalJobTemplateTypeDef",
     {
         "name": str,
         "id": str,
@@ -950,17 +1210,43 @@
         "tags": Dict[str, str],
         "kmsKeyArn": str,
         "decryptionError": str,
     },
     total=False,
 )
 
+
 class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
     pass
 
+
+_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobTemplateRequestRequestTypeDef",
+    {
+        "name": str,
+        "clientToken": str,
+        "jobTemplateData": JobTemplateDataTypeDef,
+    },
+)
+_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobTemplateRequestRequestTypeDef",
+    {
+        "tags": Mapping[str, str],
+        "kmsKeyArn": str,
+    },
+    total=False,
+)
+
+
+class CreateJobTemplateRequestRequestTypeDef(
+    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
+):
+    pass
+
+
 DescribeJobTemplateResponseTypeDef = TypedDict(
     "DescribeJobTemplateResponseTypeDef",
     {
         "jobTemplate": JobTemplateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers.egg-info/PKG-INFO` & `mypy-boto3-emr-containers-1.28.12/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-emr-containers
-Version: 1.28.0
-Summary: Type annotations for boto3.EMRContainers 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 emr-containers type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-emr-containers"></a>
 
 # mypy-boto3-emr-containers
 
 [![PyPI - mypy-boto3-emr-containers](https://img.shields.io/pypi/v/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-containers?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-containers)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-containers)](https://pepy.tech/project/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
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
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,17 +313,21 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_containers.type_defs import (
     CancelJobRunRequestRequestTypeDef,
     CancelJobRunResponseTypeDef,
     CertificateTypeDef,
+    CloudWatchMonitoringConfigurationOutputTypeDef,
     CloudWatchMonitoringConfigurationTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
+    EksInfoOutputTypeDef,
     EksInfoTypeDef,
+    ContainerLogRotationConfigurationOutputTypeDef,
     ContainerLogRotationConfigurationTypeDef,
     CreateJobTemplateResponseTypeDef,
     CreateManagedEndpointResponseTypeDef,
     CreateVirtualClusterResponseTypeDef,
     CredentialsTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeleteJobTemplateResponseTypeDef,
@@ -364,60 +336,75 @@
     DeleteVirtualClusterRequestRequestTypeDef,
     DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
     DescribeManagedEndpointRequestRequestTypeDef,
     DescribeVirtualClusterRequestRequestTypeDef,
     GetManagedEndpointSessionCredentialsRequestRequestTypeDef,
+    SparkSqlJobDriverOutputTypeDef,
+    SparkSubmitJobDriverOutputTypeDef,
     SparkSqlJobDriverTypeDef,
     SparkSubmitJobDriverTypeDef,
-    RetryPolicyConfigurationTypeDef,
+    RetryPolicyConfigurationOutputTypeDef,
     RetryPolicyExecutionTypeDef,
+    TemplateParameterConfigurationOutputTypeDef,
     TemplateParameterConfigurationTypeDef,
     ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
     ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     ListManagedEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
     ListVirtualClustersRequestRequestTypeDef,
+    S3MonitoringConfigurationOutputTypeDef,
     S3MonitoringConfigurationTypeDef,
     PaginatorConfigTypeDef,
+    ParametricCloudWatchMonitoringConfigurationOutputTypeDef,
     ParametricCloudWatchMonitoringConfigurationTypeDef,
+    ParametricS3MonitoringConfigurationOutputTypeDef,
     ParametricS3MonitoringConfigurationTypeDef,
     ResponseMetadataTypeDef,
+    RetryPolicyConfigurationTypeDef,
     StartJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ContainerInfoOutputTypeDef,
     ContainerInfoTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
+    JobDriverOutputTypeDef,
     JobDriverTypeDef,
+    MonitoringConfigurationOutputTypeDef,
     MonitoringConfigurationTypeDef,
+    ParametricMonitoringConfigurationOutputTypeDef,
     ParametricMonitoringConfigurationTypeDef,
+    ContainerProviderOutputTypeDef,
     ContainerProviderTypeDef,
+    ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
+    ParametricConfigurationOverridesOutputTypeDef,
     ParametricConfigurationOverridesTypeDef,
-    CreateVirtualClusterRequestRequestTypeDef,
     VirtualClusterTypeDef,
-    CreateManagedEndpointRequestRequestTypeDef,
+    CreateVirtualClusterRequestRequestTypeDef,
     EndpointTypeDef,
     JobRunTypeDef,
+    CreateManagedEndpointRequestRequestTypeDef,
     StartJobRunRequestRequestTypeDef,
+    JobTemplateDataOutputTypeDef,
     JobTemplateDataTypeDef,
     DescribeVirtualClusterResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     ListJobRunsResponseTypeDef,
-    CreateJobTemplateRequestRequestTypeDef,
     JobTemplateTypeDef,
+    CreateJobTemplateRequestRequestTypeDef,
     DescribeJobTemplateResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
 )
 
 
 def get_structure() -> CancelJobRunRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-emr-containers-1.28.0/mypy_boto3_emr_containers.egg-info/SOURCES.txt` & `mypy-boto3-emr-containers-1.28.12/mypy_boto3_emr_containers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.0/setup.py` & `mypy-boto3-emr-containers-1.28.12/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr-containers",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_emr_containers"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMRContainers 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.EMRContainers 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

