# Comparing `tmp/mypy-boto3-elb-1.28.0.tar.gz` & `tmp/mypy-boto3-elb-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elb-1.28.0.tar", last modified: Thu Jul  6 20:59:33 2023, max compression
+gzip compressed data, was "mypy-boto3-elb-1.28.12.tar", last modified: Thu Jul 27 05:34:39 2023, max compression
```

## Comparing `mypy-boto3-elb-1.28.0.tar` & `mypy-boto3-elb-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.070298 mypy-boto3-elb-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:26.000000 mypy-boto3-elb-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-07-06 20:59:33.070298 mypy-boto3-elb-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15511 2023-07-06 20:40:26.000000 mypy-boto3-elb-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.054298 mypy-boto3-elb-1.28.0/mypy_boto3_elb/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-06 20:40:27.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-06 20:40:27.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-06 20:40:27.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24944 2023-07-06 20:40:27.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24903 2023-07-06 20:40:27.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-07-06 20:40:27.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-06 20:40:27.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-06 20:40:27.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-06 20:40:27.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:27.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24593 2023-07-06 20:40:28.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24570 2023-07-06 20:40:27.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:26.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-06 20:40:27.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-06 20:40:27.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.070298 mypy-boto3-elb-1.28.0/mypy_boto3_elb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-07-06 20:59:32.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-06 20:59:32.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:32.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:32.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:32.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:32.000000 mypy-boto3-elb-1.28.0/mypy_boto3_elb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:33.070298 mypy-boto3-elb-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:40:26.000000 mypy-boto3-elb-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.908516 mypy-boto3-elb-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-07-27 05:34:39.904516 mypy-boto3-elb-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.904516 mypy-boto3-elb-1.28.12/mypy_boto3_elb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24944 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24903 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27896 2023-07-27 05:21:53.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27865 2023-07-27 05:21:53.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:39.904516 mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-07-27 05:34:39.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 05:34:39.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:39.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:39.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:39.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:39.000000 mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:39.908516 mypy-boto3-elb-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-27 05:21:52.000000 mypy-boto3-elb-1.28.12/setup.py
```

### Comparing `mypy-boto3-elb-1.28.0/LICENSE` & `mypy-boto3-elb-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.0/PKG-INFO` & `mypy-boto3-elb-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elb
-Version: 1.28.0
-Summary: Type annotations for boto3.ElasticLoadBalancing 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ElasticLoadBalancing 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-elb"></a>
 
 # mypy-boto3-elb
 
 [![PyPI - mypy-boto3-elb](https://img.shields.io/pypi/v/mypy-boto3-elb.svg?color=blue)](https://pypi.org/project/mypy-boto3-elb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elb.svg?color=blue)](https://pypi.org/project/mypy-boto3-elb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elb?color=blue)](https://pypistats.org/packages/mypy-boto3-elb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elb)](https://pepy.tech/project/mypy-boto3-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancing 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
+[boto3.ElasticLoadBalancing 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
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
 [mypy-boto3-elb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,98 +357,108 @@
 ### Typed dictionaries
 
 `mypy_boto3_elb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elb.type_defs import (
+    AccessLogOutputTypeDef,
     AccessLogTypeDef,
     AddAvailabilityZonesInputRequestTypeDef,
     AddAvailabilityZonesOutputTypeDef,
     TagTypeDef,
+    AdditionalAttributeOutputTypeDef,
     AdditionalAttributeTypeDef,
     AppCookieStickinessPolicyTypeDef,
     ApplySecurityGroupsToLoadBalancerInputRequestTypeDef,
     ApplySecurityGroupsToLoadBalancerOutputTypeDef,
     AttachLoadBalancerToSubnetsInputRequestTypeDef,
     AttachLoadBalancerToSubnetsOutputTypeDef,
     BackendServerDescriptionTypeDef,
     HealthCheckTypeDef,
+    HealthCheckOutputTypeDef,
+    ConnectionDrainingOutputTypeDef,
     ConnectionDrainingTypeDef,
+    ConnectionSettingsOutputTypeDef,
     ConnectionSettingsTypeDef,
     ListenerTypeDef,
     CreateAccessPointOutputTypeDef,
     CreateAppCookieStickinessPolicyInputRequestTypeDef,
     CreateLBCookieStickinessPolicyInputRequestTypeDef,
     PolicyAttributeTypeDef,
+    CrossZoneLoadBalancingOutputTypeDef,
     CrossZoneLoadBalancingTypeDef,
     DeleteAccessPointInputRequestTypeDef,
     DeleteLoadBalancerListenerInputRequestTypeDef,
     DeleteLoadBalancerPolicyInputRequestTypeDef,
     InstanceTypeDef,
+    InstanceOutputTypeDef,
     DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
     DescribeAccessPointsInputRequestTypeDef,
     DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
     WaiterConfigTypeDef,
     InstanceStateTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     DescribeLoadBalancerPoliciesInputRequestTypeDef,
     DescribeLoadBalancerPolicyTypesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DetachLoadBalancerFromSubnetsInputRequestTypeDef,
     DetachLoadBalancerFromSubnetsOutputTypeDef,
     LBCookieStickinessPolicyTypeDef,
+    ListenerOutputTypeDef,
     SourceSecurityGroupTypeDef,
     PaginatorConfigTypeDef,
     PolicyAttributeDescriptionTypeDef,
     PolicyAttributeTypeDescriptionTypeDef,
     RemoveAvailabilityZonesInputRequestTypeDef,
     RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
     ResponseMetadataTypeDef,
     SetLoadBalancerListenerSSLCertificateInputRequestTypeDef,
     SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef,
     SetLoadBalancerPoliciesOfListenerInputRequestTypeDef,
+    TagOutputTypeDef,
     AddTagsInputRequestTypeDef,
-    TagDescriptionTypeDef,
     ConfigureHealthCheckInputRequestTypeDef,
     ConfigureHealthCheckOutputTypeDef,
     CreateAccessPointInputRequestTypeDef,
     CreateLoadBalancerListenerInputRequestTypeDef,
-    ListenerDescriptionTypeDef,
     CreateLoadBalancerPolicyInputRequestTypeDef,
+    LoadBalancerAttributesOutputTypeDef,
     LoadBalancerAttributesTypeDef,
     DeregisterEndPointsInputRequestTypeDef,
-    DeregisterEndPointsOutputTypeDef,
     DescribeEndPointStateInputRequestTypeDef,
     RegisterEndPointsInputRequestTypeDef,
+    DeregisterEndPointsOutputTypeDef,
     RegisterEndPointsOutputTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     DescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     DescribeEndPointStateOutputTypeDef,
     PoliciesTypeDef,
+    ListenerDescriptionTypeDef,
     PolicyDescriptionTypeDef,
     PolicyTypeDescriptionTypeDef,
     RemoveTagsInputRequestTypeDef,
-    DescribeTagsOutputTypeDef,
+    TagDescriptionTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
-    ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
+    ModifyLoadBalancerAttributesInputRequestTypeDef,
     LoadBalancerDescriptionTypeDef,
     DescribeLoadBalancerPoliciesOutputTypeDef,
     DescribeLoadBalancerPolicyTypesOutputTypeDef,
+    DescribeTagsOutputTypeDef,
     DescribeAccessPointsOutputTypeDef,
 )
 
 
-def get_structure() -> AccessLogTypeDef:
+def get_structure() -> AccessLogOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elb-1.28.0/README.md` & `mypy-boto3-elb-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-elb"></a>
 
 # mypy-boto3-elb
 
 [![PyPI - mypy-boto3-elb](https://img.shields.io/pypi/v/mypy-boto3-elb.svg?color=blue)](https://pypi.org/project/mypy-boto3-elb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elb.svg?color=blue)](https://pypi.org/project/mypy-boto3-elb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elb?color=blue)](https://pypistats.org/packages/mypy-boto3-elb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elb)](https://pepy.tech/project/mypy-boto3-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancing 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
+[boto3.ElasticLoadBalancing 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
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
 [mypy-boto3-elb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,98 +325,108 @@
 ### Typed dictionaries
 
 `mypy_boto3_elb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elb.type_defs import (
+    AccessLogOutputTypeDef,
     AccessLogTypeDef,
     AddAvailabilityZonesInputRequestTypeDef,
     AddAvailabilityZonesOutputTypeDef,
     TagTypeDef,
+    AdditionalAttributeOutputTypeDef,
     AdditionalAttributeTypeDef,
     AppCookieStickinessPolicyTypeDef,
     ApplySecurityGroupsToLoadBalancerInputRequestTypeDef,
     ApplySecurityGroupsToLoadBalancerOutputTypeDef,
     AttachLoadBalancerToSubnetsInputRequestTypeDef,
     AttachLoadBalancerToSubnetsOutputTypeDef,
     BackendServerDescriptionTypeDef,
     HealthCheckTypeDef,
+    HealthCheckOutputTypeDef,
+    ConnectionDrainingOutputTypeDef,
     ConnectionDrainingTypeDef,
+    ConnectionSettingsOutputTypeDef,
     ConnectionSettingsTypeDef,
     ListenerTypeDef,
     CreateAccessPointOutputTypeDef,
     CreateAppCookieStickinessPolicyInputRequestTypeDef,
     CreateLBCookieStickinessPolicyInputRequestTypeDef,
     PolicyAttributeTypeDef,
+    CrossZoneLoadBalancingOutputTypeDef,
     CrossZoneLoadBalancingTypeDef,
     DeleteAccessPointInputRequestTypeDef,
     DeleteLoadBalancerListenerInputRequestTypeDef,
     DeleteLoadBalancerPolicyInputRequestTypeDef,
     InstanceTypeDef,
+    InstanceOutputTypeDef,
     DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
     DescribeAccessPointsInputRequestTypeDef,
     DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
     WaiterConfigTypeDef,
     InstanceStateTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     DescribeLoadBalancerPoliciesInputRequestTypeDef,
     DescribeLoadBalancerPolicyTypesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DetachLoadBalancerFromSubnetsInputRequestTypeDef,
     DetachLoadBalancerFromSubnetsOutputTypeDef,
     LBCookieStickinessPolicyTypeDef,
+    ListenerOutputTypeDef,
     SourceSecurityGroupTypeDef,
     PaginatorConfigTypeDef,
     PolicyAttributeDescriptionTypeDef,
     PolicyAttributeTypeDescriptionTypeDef,
     RemoveAvailabilityZonesInputRequestTypeDef,
     RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
     ResponseMetadataTypeDef,
     SetLoadBalancerListenerSSLCertificateInputRequestTypeDef,
     SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef,
     SetLoadBalancerPoliciesOfListenerInputRequestTypeDef,
+    TagOutputTypeDef,
     AddTagsInputRequestTypeDef,
-    TagDescriptionTypeDef,
     ConfigureHealthCheckInputRequestTypeDef,
     ConfigureHealthCheckOutputTypeDef,
     CreateAccessPointInputRequestTypeDef,
     CreateLoadBalancerListenerInputRequestTypeDef,
-    ListenerDescriptionTypeDef,
     CreateLoadBalancerPolicyInputRequestTypeDef,
+    LoadBalancerAttributesOutputTypeDef,
     LoadBalancerAttributesTypeDef,
     DeregisterEndPointsInputRequestTypeDef,
-    DeregisterEndPointsOutputTypeDef,
     DescribeEndPointStateInputRequestTypeDef,
     RegisterEndPointsInputRequestTypeDef,
+    DeregisterEndPointsOutputTypeDef,
     RegisterEndPointsOutputTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     DescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     DescribeEndPointStateOutputTypeDef,
     PoliciesTypeDef,
+    ListenerDescriptionTypeDef,
     PolicyDescriptionTypeDef,
     PolicyTypeDescriptionTypeDef,
     RemoveTagsInputRequestTypeDef,
-    DescribeTagsOutputTypeDef,
+    TagDescriptionTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
-    ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
+    ModifyLoadBalancerAttributesInputRequestTypeDef,
     LoadBalancerDescriptionTypeDef,
     DescribeLoadBalancerPoliciesOutputTypeDef,
     DescribeLoadBalancerPolicyTypesOutputTypeDef,
+    DescribeTagsOutputTypeDef,
     DescribeAccessPointsOutputTypeDef,
 )
 
 
-def get_structure() -> AccessLogTypeDef:
+def get_structure() -> AccessLogOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elb-1.28.0/mypy_boto3_elb/__init__.py` & `mypy-boto3-elb-1.28.12/mypy_boto3_elb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.0/mypy_boto3_elb/__init__.pyi` & `mypy-boto3-elb-1.28.12/mypy_boto3_elb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.0/mypy_boto3_elb/__main__.py` & `mypy-boto3-elb-1.28.12/mypy_boto3_elb/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticLoadBalancing 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ElasticLoadBalancing 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing\nOther"
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

### Comparing `mypy-boto3-elb-1.28.0/mypy_boto3_elb/client.py` & `mypy-boto3-elb-1.28.12/mypy_boto3_elb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.0/mypy_boto3_elb/client.pyi` & `mypy-boto3-elb-1.28.12/mypy_boto3_elb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.0/mypy_boto3_elb/literals.py` & `mypy-boto3-elb-1.28.12/mypy_boto3_elb/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,15 @@
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
@@ -241,26 +242,28 @@
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

### Comparing `mypy-boto3-elb-1.28.0/mypy_boto3_elb/literals.pyi` & `mypy-boto3-elb-1.28.12/mypy_boto3_elb/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,15 @@
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
@@ -239,26 +240,28 @@
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

### Comparing `mypy-boto3-elb-1.28.0/mypy_boto3_elb/paginator.py` & `mypy-boto3-elb-1.28.12/mypy_boto3_elb/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.0/mypy_boto3_elb/paginator.pyi` & `mypy-boto3-elb-1.28.12/mypy_boto3_elb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.0/mypy_boto3_elb/type_defs.py` & `mypy-boto3-elb-1.28.12/mypy_boto3_elb/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,112 +2,143 @@
 Type annotations for elb service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_elb.type_defs import AccessLogTypeDef
+    from mypy_boto3_elb.type_defs import AccessLogOutputTypeDef
 
-    data: AccessLogTypeDef = {...}
+    data: AccessLogOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AccessLogOutputTypeDef",
     "AccessLogTypeDef",
     "AddAvailabilityZonesInputRequestTypeDef",
     "AddAvailabilityZonesOutputTypeDef",
     "TagTypeDef",
+    "AdditionalAttributeOutputTypeDef",
     "AdditionalAttributeTypeDef",
     "AppCookieStickinessPolicyTypeDef",
     "ApplySecurityGroupsToLoadBalancerInputRequestTypeDef",
     "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
     "AttachLoadBalancerToSubnetsInputRequestTypeDef",
     "AttachLoadBalancerToSubnetsOutputTypeDef",
     "BackendServerDescriptionTypeDef",
     "HealthCheckTypeDef",
+    "HealthCheckOutputTypeDef",
+    "ConnectionDrainingOutputTypeDef",
     "ConnectionDrainingTypeDef",
+    "ConnectionSettingsOutputTypeDef",
     "ConnectionSettingsTypeDef",
     "ListenerTypeDef",
     "CreateAccessPointOutputTypeDef",
     "CreateAppCookieStickinessPolicyInputRequestTypeDef",
     "CreateLBCookieStickinessPolicyInputRequestTypeDef",
     "PolicyAttributeTypeDef",
+    "CrossZoneLoadBalancingOutputTypeDef",
     "CrossZoneLoadBalancingTypeDef",
     "DeleteAccessPointInputRequestTypeDef",
     "DeleteLoadBalancerListenerInputRequestTypeDef",
     "DeleteLoadBalancerPolicyInputRequestTypeDef",
     "InstanceTypeDef",
+    "InstanceOutputTypeDef",
     "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
     "DescribeAccessPointsInputRequestTypeDef",
     "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
     "WaiterConfigTypeDef",
     "InstanceStateTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     "DescribeLoadBalancerPoliciesInputRequestTypeDef",
     "DescribeLoadBalancerPolicyTypesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DetachLoadBalancerFromSubnetsInputRequestTypeDef",
     "DetachLoadBalancerFromSubnetsOutputTypeDef",
     "LBCookieStickinessPolicyTypeDef",
+    "ListenerOutputTypeDef",
     "SourceSecurityGroupTypeDef",
     "PaginatorConfigTypeDef",
     "PolicyAttributeDescriptionTypeDef",
     "PolicyAttributeTypeDescriptionTypeDef",
     "RemoveAvailabilityZonesInputRequestTypeDef",
     "RemoveAvailabilityZonesOutputTypeDef",
     "TagKeyOnlyTypeDef",
     "ResponseMetadataTypeDef",
     "SetLoadBalancerListenerSSLCertificateInputRequestTypeDef",
     "SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef",
     "SetLoadBalancerPoliciesOfListenerInputRequestTypeDef",
+    "TagOutputTypeDef",
     "AddTagsInputRequestTypeDef",
-    "TagDescriptionTypeDef",
     "ConfigureHealthCheckInputRequestTypeDef",
     "ConfigureHealthCheckOutputTypeDef",
     "CreateAccessPointInputRequestTypeDef",
     "CreateLoadBalancerListenerInputRequestTypeDef",
-    "ListenerDescriptionTypeDef",
     "CreateLoadBalancerPolicyInputRequestTypeDef",
+    "LoadBalancerAttributesOutputTypeDef",
     "LoadBalancerAttributesTypeDef",
     "DeregisterEndPointsInputRequestTypeDef",
-    "DeregisterEndPointsOutputTypeDef",
     "DescribeEndPointStateInputRequestTypeDef",
     "RegisterEndPointsInputRequestTypeDef",
+    "DeregisterEndPointsOutputTypeDef",
     "RegisterEndPointsOutputTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef",
     "DescribeEndPointStateInputInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateOutputTypeDef",
     "PoliciesTypeDef",
+    "ListenerDescriptionTypeDef",
     "PolicyDescriptionTypeDef",
     "PolicyTypeDescriptionTypeDef",
     "RemoveTagsInputRequestTypeDef",
-    "DescribeTagsOutputTypeDef",
+    "TagDescriptionTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "ModifyLoadBalancerAttributesOutputTypeDef",
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "LoadBalancerDescriptionTypeDef",
     "DescribeLoadBalancerPoliciesOutputTypeDef",
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
+    "DescribeTagsOutputTypeDef",
     "DescribeAccessPointsOutputTypeDef",
 )
 
+_RequiredAccessLogOutputTypeDef = TypedDict(
+    "_RequiredAccessLogOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalAccessLogOutputTypeDef = TypedDict(
+    "_OptionalAccessLogOutputTypeDef",
+    {
+        "S3BucketName": str,
+        "EmitInterval": int,
+        "S3BucketPrefix": str,
+    },
+    total=False,
+)
+
+
+class AccessLogOutputTypeDef(_RequiredAccessLogOutputTypeDef, _OptionalAccessLogOutputTypeDef):
+    pass
+
+
 _RequiredAccessLogTypeDef = TypedDict(
     "_RequiredAccessLogTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalAccessLogTypeDef = TypedDict(
@@ -156,14 +187,23 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
+AdditionalAttributeOutputTypeDef = TypedDict(
+    "AdditionalAttributeOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 AdditionalAttributeTypeDef = TypedDict(
     "AdditionalAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -226,14 +266,46 @@
         "Interval": int,
         "Timeout": int,
         "UnhealthyThreshold": int,
         "HealthyThreshold": int,
     },
 )
 
+HealthCheckOutputTypeDef = TypedDict(
+    "HealthCheckOutputTypeDef",
+    {
+        "Target": str,
+        "Interval": int,
+        "Timeout": int,
+        "UnhealthyThreshold": int,
+        "HealthyThreshold": int,
+    },
+)
+
+_RequiredConnectionDrainingOutputTypeDef = TypedDict(
+    "_RequiredConnectionDrainingOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalConnectionDrainingOutputTypeDef = TypedDict(
+    "_OptionalConnectionDrainingOutputTypeDef",
+    {
+        "Timeout": int,
+    },
+    total=False,
+)
+
+
+class ConnectionDrainingOutputTypeDef(
+    _RequiredConnectionDrainingOutputTypeDef, _OptionalConnectionDrainingOutputTypeDef
+):
+    pass
+
+
 _RequiredConnectionDrainingTypeDef = TypedDict(
     "_RequiredConnectionDrainingTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalConnectionDrainingTypeDef = TypedDict(
@@ -247,14 +319,21 @@
 
 class ConnectionDrainingTypeDef(
     _RequiredConnectionDrainingTypeDef, _OptionalConnectionDrainingTypeDef
 ):
     pass
 
 
+ConnectionSettingsOutputTypeDef = TypedDict(
+    "ConnectionSettingsOutputTypeDef",
+    {
+        "IdleTimeout": int,
+    },
+)
+
 ConnectionSettingsTypeDef = TypedDict(
     "ConnectionSettingsTypeDef",
     {
         "IdleTimeout": int,
     },
 )
 
@@ -325,14 +404,21 @@
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
     total=False,
 )
 
+CrossZoneLoadBalancingOutputTypeDef = TypedDict(
+    "CrossZoneLoadBalancingOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+
 CrossZoneLoadBalancingTypeDef = TypedDict(
     "CrossZoneLoadBalancingTypeDef",
     {
         "Enabled": bool,
     },
 )
 
@@ -363,14 +449,22 @@
     "InstanceTypeDef",
     {
         "InstanceId": str,
     },
     total=False,
 )
 
+InstanceOutputTypeDef = TypedDict(
+    "InstanceOutputTypeDef",
+    {
+        "InstanceId": str,
+    },
+    total=False,
+)
+
 DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
     "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -484,14 +578,36 @@
     {
         "PolicyName": str,
         "CookieExpirationPeriod": int,
     },
     total=False,
 )
 
+_RequiredListenerOutputTypeDef = TypedDict(
+    "_RequiredListenerOutputTypeDef",
+    {
+        "Protocol": str,
+        "LoadBalancerPort": int,
+        "InstancePort": int,
+    },
+)
+_OptionalListenerOutputTypeDef = TypedDict(
+    "_OptionalListenerOutputTypeDef",
+    {
+        "InstanceProtocol": str,
+        "SSLCertificateId": str,
+    },
+    total=False,
+)
+
+
+class ListenerOutputTypeDef(_RequiredListenerOutputTypeDef, _OptionalListenerOutputTypeDef):
+    pass
+
+
 SourceSecurityGroupTypeDef = TypedDict(
     "SourceSecurityGroupTypeDef",
     {
         "OwnerAlias": str,
         "GroupName": str,
     },
     total=False,
@@ -586,43 +702,53 @@
     {
         "LoadBalancerName": str,
         "LoadBalancerPort": int,
         "PolicyNames": Sequence[str],
     },
 )
 
-AddTagsInputRequestTypeDef = TypedDict(
-    "AddTagsInputRequestTypeDef",
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
     {
-        "LoadBalancerNames": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
+        "Key": str,
     },
 )
-
-TagDescriptionTypeDef = TypedDict(
-    "TagDescriptionTypeDef",
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
     {
-        "LoadBalancerName": str,
-        "Tags": List[TagTypeDef],
+        "Value": str,
     },
     total=False,
 )
 
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
+
+AddTagsInputRequestTypeDef = TypedDict(
+    "AddTagsInputRequestTypeDef",
+    {
+        "LoadBalancerNames": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 ConfigureHealthCheckInputRequestTypeDef = TypedDict(
     "ConfigureHealthCheckInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "HealthCheck": HealthCheckTypeDef,
     },
 )
 
 ConfigureHealthCheckOutputTypeDef = TypedDict(
     "ConfigureHealthCheckOutputTypeDef",
     {
-        "HealthCheck": HealthCheckTypeDef,
+        "HealthCheck": HealthCheckOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAccessPointInputRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPointInputRequestTypeDef",
     {
@@ -653,23 +779,14 @@
     "CreateLoadBalancerListenerInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Listeners": Sequence[ListenerTypeDef],
     },
 )
 
-ListenerDescriptionTypeDef = TypedDict(
-    "ListenerDescriptionTypeDef",
-    {
-        "Listener": ListenerTypeDef,
-        "PolicyNames": List[str],
-    },
-    total=False,
-)
-
 _RequiredCreateLoadBalancerPolicyInputRequestTypeDef = TypedDict(
     "_RequiredCreateLoadBalancerPolicyInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "PolicyName": str,
         "PolicyTypeName": str,
     },
@@ -686,42 +803,46 @@
 class CreateLoadBalancerPolicyInputRequestTypeDef(
     _RequiredCreateLoadBalancerPolicyInputRequestTypeDef,
     _OptionalCreateLoadBalancerPolicyInputRequestTypeDef,
 ):
     pass
 
 
+LoadBalancerAttributesOutputTypeDef = TypedDict(
+    "LoadBalancerAttributesOutputTypeDef",
+    {
+        "CrossZoneLoadBalancing": CrossZoneLoadBalancingOutputTypeDef,
+        "AccessLog": AccessLogOutputTypeDef,
+        "ConnectionDraining": ConnectionDrainingOutputTypeDef,
+        "ConnectionSettings": ConnectionSettingsOutputTypeDef,
+        "AdditionalAttributes": List[AdditionalAttributeOutputTypeDef],
+    },
+    total=False,
+)
+
 LoadBalancerAttributesTypeDef = TypedDict(
     "LoadBalancerAttributesTypeDef",
     {
         "CrossZoneLoadBalancing": CrossZoneLoadBalancingTypeDef,
         "AccessLog": AccessLogTypeDef,
         "ConnectionDraining": ConnectionDrainingTypeDef,
         "ConnectionSettings": ConnectionSettingsTypeDef,
-        "AdditionalAttributes": List[AdditionalAttributeTypeDef],
+        "AdditionalAttributes": Sequence[AdditionalAttributeTypeDef],
     },
     total=False,
 )
 
 DeregisterEndPointsInputRequestTypeDef = TypedDict(
     "DeregisterEndPointsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Instances": Sequence[InstanceTypeDef],
     },
 )
 
-DeregisterEndPointsOutputTypeDef = TypedDict(
-    "DeregisterEndPointsOutputTypeDef",
-    {
-        "Instances": List[InstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeEndPointStateInputRequestTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputRequestTypeDef",
     {
         "LoadBalancerName": str,
     },
 )
 _OptionalDescribeEndPointStateInputRequestTypeDef = TypedDict(
@@ -744,18 +865,26 @@
     "RegisterEndPointsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Instances": Sequence[InstanceTypeDef],
     },
 )
 
+DeregisterEndPointsOutputTypeDef = TypedDict(
+    "DeregisterEndPointsOutputTypeDef",
+    {
+        "Instances": List[InstanceOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterEndPointsOutputTypeDef = TypedDict(
     "RegisterEndPointsOutputTypeDef",
     {
-        "Instances": List[InstanceTypeDef],
+        "Instances": List[InstanceOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccountLimitsOutputTypeDef = TypedDict(
     "DescribeAccountLimitsOutputTypeDef",
     {
@@ -848,14 +977,23 @@
         "AppCookieStickinessPolicies": List[AppCookieStickinessPolicyTypeDef],
         "LBCookieStickinessPolicies": List[LBCookieStickinessPolicyTypeDef],
         "OtherPolicies": List[str],
     },
     total=False,
 )
 
+ListenerDescriptionTypeDef = TypedDict(
+    "ListenerDescriptionTypeDef",
+    {
+        "Listener": ListenerOutputTypeDef,
+        "PolicyNames": List[str],
+    },
+    total=False,
+)
+
 PolicyDescriptionTypeDef = TypedDict(
     "PolicyDescriptionTypeDef",
     {
         "PolicyName": str,
         "PolicyTypeName": str,
         "PolicyAttributeDescriptions": List[PolicyAttributeDescriptionTypeDef],
     },
@@ -876,44 +1014,45 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Tags": Sequence[TagKeyOnlyTypeDef],
     },
 )
 
-DescribeTagsOutputTypeDef = TypedDict(
-    "DescribeTagsOutputTypeDef",
+TagDescriptionTypeDef = TypedDict(
+    "TagDescriptionTypeDef",
     {
-        "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoadBalancerName": str,
+        "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
-        "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
+        "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
+ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesOutputTypeDef",
     {
         "LoadBalancerName": str,
-        "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
+        "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesOutputTypeDef",
+ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoadBalancerDescriptionTypeDef = TypedDict(
     "LoadBalancerDescriptionTypeDef",
     {
         "LoadBalancerName": str,
@@ -922,16 +1061,16 @@
         "CanonicalHostedZoneNameID": str,
         "ListenerDescriptions": List[ListenerDescriptionTypeDef],
         "Policies": PoliciesTypeDef,
         "BackendServerDescriptions": List[BackendServerDescriptionTypeDef],
         "AvailabilityZones": List[str],
         "Subnets": List[str],
         "VPCId": str,
-        "Instances": List[InstanceTypeDef],
-        "HealthCheck": HealthCheckTypeDef,
+        "Instances": List[InstanceOutputTypeDef],
+        "HealthCheck": HealthCheckOutputTypeDef,
         "SourceSecurityGroup": SourceSecurityGroupTypeDef,
         "SecurityGroups": List[str],
         "CreatedTime": datetime,
         "Scheme": str,
     },
     total=False,
 )
@@ -948,14 +1087,22 @@
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
     {
         "PolicyTypeDescriptions": List[PolicyTypeDescriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DescribeTagsOutputTypeDef = TypedDict(
+    "DescribeTagsOutputTypeDef",
+    {
+        "TagDescriptions": List[TagDescriptionTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeAccessPointsOutputTypeDef = TypedDict(
     "DescribeAccessPointsOutputTypeDef",
     {
         "LoadBalancerDescriptions": List[LoadBalancerDescriptionTypeDef],
         "NextMarker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-elb-1.28.0/mypy_boto3_elb/type_defs.pyi` & `mypy-boto3-elb-1.28.12/mypy_boto3_elb/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -2,111 +2,140 @@
 Type annotations for elb service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_elb.type_defs import AccessLogTypeDef
+    from mypy_boto3_elb.type_defs import AccessLogOutputTypeDef
 
-    data: AccessLogTypeDef = {...}
+    data: AccessLogOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AccessLogOutputTypeDef",
     "AccessLogTypeDef",
     "AddAvailabilityZonesInputRequestTypeDef",
     "AddAvailabilityZonesOutputTypeDef",
     "TagTypeDef",
+    "AdditionalAttributeOutputTypeDef",
     "AdditionalAttributeTypeDef",
     "AppCookieStickinessPolicyTypeDef",
     "ApplySecurityGroupsToLoadBalancerInputRequestTypeDef",
     "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
     "AttachLoadBalancerToSubnetsInputRequestTypeDef",
     "AttachLoadBalancerToSubnetsOutputTypeDef",
     "BackendServerDescriptionTypeDef",
     "HealthCheckTypeDef",
+    "HealthCheckOutputTypeDef",
+    "ConnectionDrainingOutputTypeDef",
     "ConnectionDrainingTypeDef",
+    "ConnectionSettingsOutputTypeDef",
     "ConnectionSettingsTypeDef",
     "ListenerTypeDef",
     "CreateAccessPointOutputTypeDef",
     "CreateAppCookieStickinessPolicyInputRequestTypeDef",
     "CreateLBCookieStickinessPolicyInputRequestTypeDef",
     "PolicyAttributeTypeDef",
+    "CrossZoneLoadBalancingOutputTypeDef",
     "CrossZoneLoadBalancingTypeDef",
     "DeleteAccessPointInputRequestTypeDef",
     "DeleteLoadBalancerListenerInputRequestTypeDef",
     "DeleteLoadBalancerPolicyInputRequestTypeDef",
     "InstanceTypeDef",
+    "InstanceOutputTypeDef",
     "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
     "DescribeAccessPointsInputRequestTypeDef",
     "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
     "WaiterConfigTypeDef",
     "InstanceStateTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     "DescribeLoadBalancerPoliciesInputRequestTypeDef",
     "DescribeLoadBalancerPolicyTypesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DetachLoadBalancerFromSubnetsInputRequestTypeDef",
     "DetachLoadBalancerFromSubnetsOutputTypeDef",
     "LBCookieStickinessPolicyTypeDef",
+    "ListenerOutputTypeDef",
     "SourceSecurityGroupTypeDef",
     "PaginatorConfigTypeDef",
     "PolicyAttributeDescriptionTypeDef",
     "PolicyAttributeTypeDescriptionTypeDef",
     "RemoveAvailabilityZonesInputRequestTypeDef",
     "RemoveAvailabilityZonesOutputTypeDef",
     "TagKeyOnlyTypeDef",
     "ResponseMetadataTypeDef",
     "SetLoadBalancerListenerSSLCertificateInputRequestTypeDef",
     "SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef",
     "SetLoadBalancerPoliciesOfListenerInputRequestTypeDef",
+    "TagOutputTypeDef",
     "AddTagsInputRequestTypeDef",
-    "TagDescriptionTypeDef",
     "ConfigureHealthCheckInputRequestTypeDef",
     "ConfigureHealthCheckOutputTypeDef",
     "CreateAccessPointInputRequestTypeDef",
     "CreateLoadBalancerListenerInputRequestTypeDef",
-    "ListenerDescriptionTypeDef",
     "CreateLoadBalancerPolicyInputRequestTypeDef",
+    "LoadBalancerAttributesOutputTypeDef",
     "LoadBalancerAttributesTypeDef",
     "DeregisterEndPointsInputRequestTypeDef",
-    "DeregisterEndPointsOutputTypeDef",
     "DescribeEndPointStateInputRequestTypeDef",
     "RegisterEndPointsInputRequestTypeDef",
+    "DeregisterEndPointsOutputTypeDef",
     "RegisterEndPointsOutputTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef",
     "DescribeEndPointStateInputInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateOutputTypeDef",
     "PoliciesTypeDef",
+    "ListenerDescriptionTypeDef",
     "PolicyDescriptionTypeDef",
     "PolicyTypeDescriptionTypeDef",
     "RemoveTagsInputRequestTypeDef",
-    "DescribeTagsOutputTypeDef",
+    "TagDescriptionTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "ModifyLoadBalancerAttributesOutputTypeDef",
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "LoadBalancerDescriptionTypeDef",
     "DescribeLoadBalancerPoliciesOutputTypeDef",
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
+    "DescribeTagsOutputTypeDef",
     "DescribeAccessPointsOutputTypeDef",
 )
 
+_RequiredAccessLogOutputTypeDef = TypedDict(
+    "_RequiredAccessLogOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalAccessLogOutputTypeDef = TypedDict(
+    "_OptionalAccessLogOutputTypeDef",
+    {
+        "S3BucketName": str,
+        "EmitInterval": int,
+        "S3BucketPrefix": str,
+    },
+    total=False,
+)
+
+class AccessLogOutputTypeDef(_RequiredAccessLogOutputTypeDef, _OptionalAccessLogOutputTypeDef):
+    pass
+
 _RequiredAccessLogTypeDef = TypedDict(
     "_RequiredAccessLogTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalAccessLogTypeDef = TypedDict(
@@ -151,14 +180,23 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+AdditionalAttributeOutputTypeDef = TypedDict(
+    "AdditionalAttributeOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 AdditionalAttributeTypeDef = TypedDict(
     "AdditionalAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -221,14 +259,44 @@
         "Interval": int,
         "Timeout": int,
         "UnhealthyThreshold": int,
         "HealthyThreshold": int,
     },
 )
 
+HealthCheckOutputTypeDef = TypedDict(
+    "HealthCheckOutputTypeDef",
+    {
+        "Target": str,
+        "Interval": int,
+        "Timeout": int,
+        "UnhealthyThreshold": int,
+        "HealthyThreshold": int,
+    },
+)
+
+_RequiredConnectionDrainingOutputTypeDef = TypedDict(
+    "_RequiredConnectionDrainingOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalConnectionDrainingOutputTypeDef = TypedDict(
+    "_OptionalConnectionDrainingOutputTypeDef",
+    {
+        "Timeout": int,
+    },
+    total=False,
+)
+
+class ConnectionDrainingOutputTypeDef(
+    _RequiredConnectionDrainingOutputTypeDef, _OptionalConnectionDrainingOutputTypeDef
+):
+    pass
+
 _RequiredConnectionDrainingTypeDef = TypedDict(
     "_RequiredConnectionDrainingTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalConnectionDrainingTypeDef = TypedDict(
@@ -240,14 +308,21 @@
 )
 
 class ConnectionDrainingTypeDef(
     _RequiredConnectionDrainingTypeDef, _OptionalConnectionDrainingTypeDef
 ):
     pass
 
+ConnectionSettingsOutputTypeDef = TypedDict(
+    "ConnectionSettingsOutputTypeDef",
+    {
+        "IdleTimeout": int,
+    },
+)
+
 ConnectionSettingsTypeDef = TypedDict(
     "ConnectionSettingsTypeDef",
     {
         "IdleTimeout": int,
     },
 )
 
@@ -314,14 +389,21 @@
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
     total=False,
 )
 
+CrossZoneLoadBalancingOutputTypeDef = TypedDict(
+    "CrossZoneLoadBalancingOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+
 CrossZoneLoadBalancingTypeDef = TypedDict(
     "CrossZoneLoadBalancingTypeDef",
     {
         "Enabled": bool,
     },
 )
 
@@ -352,14 +434,22 @@
     "InstanceTypeDef",
     {
         "InstanceId": str,
     },
     total=False,
 )
 
+InstanceOutputTypeDef = TypedDict(
+    "InstanceOutputTypeDef",
+    {
+        "InstanceId": str,
+    },
+    total=False,
+)
+
 DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
     "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -473,14 +563,34 @@
     {
         "PolicyName": str,
         "CookieExpirationPeriod": int,
     },
     total=False,
 )
 
+_RequiredListenerOutputTypeDef = TypedDict(
+    "_RequiredListenerOutputTypeDef",
+    {
+        "Protocol": str,
+        "LoadBalancerPort": int,
+        "InstancePort": int,
+    },
+)
+_OptionalListenerOutputTypeDef = TypedDict(
+    "_OptionalListenerOutputTypeDef",
+    {
+        "InstanceProtocol": str,
+        "SSLCertificateId": str,
+    },
+    total=False,
+)
+
+class ListenerOutputTypeDef(_RequiredListenerOutputTypeDef, _OptionalListenerOutputTypeDef):
+    pass
+
 SourceSecurityGroupTypeDef = TypedDict(
     "SourceSecurityGroupTypeDef",
     {
         "OwnerAlias": str,
         "GroupName": str,
     },
     total=False,
@@ -575,43 +685,51 @@
     {
         "LoadBalancerName": str,
         "LoadBalancerPort": int,
         "PolicyNames": Sequence[str],
     },
 )
 
-AddTagsInputRequestTypeDef = TypedDict(
-    "AddTagsInputRequestTypeDef",
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
     {
-        "LoadBalancerNames": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
+        "Key": str,
     },
 )
-
-TagDescriptionTypeDef = TypedDict(
-    "TagDescriptionTypeDef",
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
     {
-        "LoadBalancerName": str,
-        "Tags": List[TagTypeDef],
+        "Value": str,
     },
     total=False,
 )
 
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
+AddTagsInputRequestTypeDef = TypedDict(
+    "AddTagsInputRequestTypeDef",
+    {
+        "LoadBalancerNames": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 ConfigureHealthCheckInputRequestTypeDef = TypedDict(
     "ConfigureHealthCheckInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "HealthCheck": HealthCheckTypeDef,
     },
 )
 
 ConfigureHealthCheckOutputTypeDef = TypedDict(
     "ConfigureHealthCheckOutputTypeDef",
     {
-        "HealthCheck": HealthCheckTypeDef,
+        "HealthCheck": HealthCheckOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAccessPointInputRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPointInputRequestTypeDef",
     {
@@ -640,23 +758,14 @@
     "CreateLoadBalancerListenerInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Listeners": Sequence[ListenerTypeDef],
     },
 )
 
-ListenerDescriptionTypeDef = TypedDict(
-    "ListenerDescriptionTypeDef",
-    {
-        "Listener": ListenerTypeDef,
-        "PolicyNames": List[str],
-    },
-    total=False,
-)
-
 _RequiredCreateLoadBalancerPolicyInputRequestTypeDef = TypedDict(
     "_RequiredCreateLoadBalancerPolicyInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "PolicyName": str,
         "PolicyTypeName": str,
     },
@@ -671,42 +780,46 @@
 
 class CreateLoadBalancerPolicyInputRequestTypeDef(
     _RequiredCreateLoadBalancerPolicyInputRequestTypeDef,
     _OptionalCreateLoadBalancerPolicyInputRequestTypeDef,
 ):
     pass
 
+LoadBalancerAttributesOutputTypeDef = TypedDict(
+    "LoadBalancerAttributesOutputTypeDef",
+    {
+        "CrossZoneLoadBalancing": CrossZoneLoadBalancingOutputTypeDef,
+        "AccessLog": AccessLogOutputTypeDef,
+        "ConnectionDraining": ConnectionDrainingOutputTypeDef,
+        "ConnectionSettings": ConnectionSettingsOutputTypeDef,
+        "AdditionalAttributes": List[AdditionalAttributeOutputTypeDef],
+    },
+    total=False,
+)
+
 LoadBalancerAttributesTypeDef = TypedDict(
     "LoadBalancerAttributesTypeDef",
     {
         "CrossZoneLoadBalancing": CrossZoneLoadBalancingTypeDef,
         "AccessLog": AccessLogTypeDef,
         "ConnectionDraining": ConnectionDrainingTypeDef,
         "ConnectionSettings": ConnectionSettingsTypeDef,
-        "AdditionalAttributes": List[AdditionalAttributeTypeDef],
+        "AdditionalAttributes": Sequence[AdditionalAttributeTypeDef],
     },
     total=False,
 )
 
 DeregisterEndPointsInputRequestTypeDef = TypedDict(
     "DeregisterEndPointsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Instances": Sequence[InstanceTypeDef],
     },
 )
 
-DeregisterEndPointsOutputTypeDef = TypedDict(
-    "DeregisterEndPointsOutputTypeDef",
-    {
-        "Instances": List[InstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeEndPointStateInputRequestTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputRequestTypeDef",
     {
         "LoadBalancerName": str,
     },
 )
 _OptionalDescribeEndPointStateInputRequestTypeDef = TypedDict(
@@ -727,18 +840,26 @@
     "RegisterEndPointsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Instances": Sequence[InstanceTypeDef],
     },
 )
 
+DeregisterEndPointsOutputTypeDef = TypedDict(
+    "DeregisterEndPointsOutputTypeDef",
+    {
+        "Instances": List[InstanceOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterEndPointsOutputTypeDef = TypedDict(
     "RegisterEndPointsOutputTypeDef",
     {
-        "Instances": List[InstanceTypeDef],
+        "Instances": List[InstanceOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccountLimitsOutputTypeDef = TypedDict(
     "DescribeAccountLimitsOutputTypeDef",
     {
@@ -825,14 +946,23 @@
         "AppCookieStickinessPolicies": List[AppCookieStickinessPolicyTypeDef],
         "LBCookieStickinessPolicies": List[LBCookieStickinessPolicyTypeDef],
         "OtherPolicies": List[str],
     },
     total=False,
 )
 
+ListenerDescriptionTypeDef = TypedDict(
+    "ListenerDescriptionTypeDef",
+    {
+        "Listener": ListenerOutputTypeDef,
+        "PolicyNames": List[str],
+    },
+    total=False,
+)
+
 PolicyDescriptionTypeDef = TypedDict(
     "PolicyDescriptionTypeDef",
     {
         "PolicyName": str,
         "PolicyTypeName": str,
         "PolicyAttributeDescriptions": List[PolicyAttributeDescriptionTypeDef],
     },
@@ -853,44 +983,45 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Tags": Sequence[TagKeyOnlyTypeDef],
     },
 )
 
-DescribeTagsOutputTypeDef = TypedDict(
-    "DescribeTagsOutputTypeDef",
+TagDescriptionTypeDef = TypedDict(
+    "TagDescriptionTypeDef",
     {
-        "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoadBalancerName": str,
+        "Tags": List[TagOutputTypeDef],
     },
+    total=False,
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
-        "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
+        "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
+ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesOutputTypeDef",
     {
         "LoadBalancerName": str,
-        "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
+        "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesOutputTypeDef",
+ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoadBalancerDescriptionTypeDef = TypedDict(
     "LoadBalancerDescriptionTypeDef",
     {
         "LoadBalancerName": str,
@@ -899,16 +1030,16 @@
         "CanonicalHostedZoneNameID": str,
         "ListenerDescriptions": List[ListenerDescriptionTypeDef],
         "Policies": PoliciesTypeDef,
         "BackendServerDescriptions": List[BackendServerDescriptionTypeDef],
         "AvailabilityZones": List[str],
         "Subnets": List[str],
         "VPCId": str,
-        "Instances": List[InstanceTypeDef],
-        "HealthCheck": HealthCheckTypeDef,
+        "Instances": List[InstanceOutputTypeDef],
+        "HealthCheck": HealthCheckOutputTypeDef,
         "SourceSecurityGroup": SourceSecurityGroupTypeDef,
         "SecurityGroups": List[str],
         "CreatedTime": datetime,
         "Scheme": str,
     },
     total=False,
 )
@@ -925,14 +1056,22 @@
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
     {
         "PolicyTypeDescriptions": List[PolicyTypeDescriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DescribeTagsOutputTypeDef = TypedDict(
+    "DescribeTagsOutputTypeDef",
+    {
+        "TagDescriptions": List[TagDescriptionTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeAccessPointsOutputTypeDef = TypedDict(
     "DescribeAccessPointsOutputTypeDef",
     {
         "LoadBalancerDescriptions": List[LoadBalancerDescriptionTypeDef],
         "NextMarker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-elb-1.28.0/mypy_boto3_elb/waiter.py` & `mypy-boto3-elb-1.28.12/mypy_boto3_elb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.0/mypy_boto3_elb/waiter.pyi` & `mypy-boto3-elb-1.28.12/mypy_boto3_elb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.0/mypy_boto3_elb.egg-info/PKG-INFO` & `mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elb
-Version: 1.28.0
-Summary: Type annotations for boto3.ElasticLoadBalancing 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ElasticLoadBalancing 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-elb"></a>
 
 # mypy-boto3-elb
 
 [![PyPI - mypy-boto3-elb](https://img.shields.io/pypi/v/mypy-boto3-elb.svg?color=blue)](https://pypi.org/project/mypy-boto3-elb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elb.svg?color=blue)](https://pypi.org/project/mypy-boto3-elb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elb?color=blue)](https://pypistats.org/packages/mypy-boto3-elb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elb)](https://pepy.tech/project/mypy-boto3-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancing 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
+[boto3.ElasticLoadBalancing 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
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
 [mypy-boto3-elb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,98 +357,108 @@
 ### Typed dictionaries
 
 `mypy_boto3_elb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elb.type_defs import (
+    AccessLogOutputTypeDef,
     AccessLogTypeDef,
     AddAvailabilityZonesInputRequestTypeDef,
     AddAvailabilityZonesOutputTypeDef,
     TagTypeDef,
+    AdditionalAttributeOutputTypeDef,
     AdditionalAttributeTypeDef,
     AppCookieStickinessPolicyTypeDef,
     ApplySecurityGroupsToLoadBalancerInputRequestTypeDef,
     ApplySecurityGroupsToLoadBalancerOutputTypeDef,
     AttachLoadBalancerToSubnetsInputRequestTypeDef,
     AttachLoadBalancerToSubnetsOutputTypeDef,
     BackendServerDescriptionTypeDef,
     HealthCheckTypeDef,
+    HealthCheckOutputTypeDef,
+    ConnectionDrainingOutputTypeDef,
     ConnectionDrainingTypeDef,
+    ConnectionSettingsOutputTypeDef,
     ConnectionSettingsTypeDef,
     ListenerTypeDef,
     CreateAccessPointOutputTypeDef,
     CreateAppCookieStickinessPolicyInputRequestTypeDef,
     CreateLBCookieStickinessPolicyInputRequestTypeDef,
     PolicyAttributeTypeDef,
+    CrossZoneLoadBalancingOutputTypeDef,
     CrossZoneLoadBalancingTypeDef,
     DeleteAccessPointInputRequestTypeDef,
     DeleteLoadBalancerListenerInputRequestTypeDef,
     DeleteLoadBalancerPolicyInputRequestTypeDef,
     InstanceTypeDef,
+    InstanceOutputTypeDef,
     DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
     DescribeAccessPointsInputRequestTypeDef,
     DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
     WaiterConfigTypeDef,
     InstanceStateTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     DescribeLoadBalancerPoliciesInputRequestTypeDef,
     DescribeLoadBalancerPolicyTypesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DetachLoadBalancerFromSubnetsInputRequestTypeDef,
     DetachLoadBalancerFromSubnetsOutputTypeDef,
     LBCookieStickinessPolicyTypeDef,
+    ListenerOutputTypeDef,
     SourceSecurityGroupTypeDef,
     PaginatorConfigTypeDef,
     PolicyAttributeDescriptionTypeDef,
     PolicyAttributeTypeDescriptionTypeDef,
     RemoveAvailabilityZonesInputRequestTypeDef,
     RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
     ResponseMetadataTypeDef,
     SetLoadBalancerListenerSSLCertificateInputRequestTypeDef,
     SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef,
     SetLoadBalancerPoliciesOfListenerInputRequestTypeDef,
+    TagOutputTypeDef,
     AddTagsInputRequestTypeDef,
-    TagDescriptionTypeDef,
     ConfigureHealthCheckInputRequestTypeDef,
     ConfigureHealthCheckOutputTypeDef,
     CreateAccessPointInputRequestTypeDef,
     CreateLoadBalancerListenerInputRequestTypeDef,
-    ListenerDescriptionTypeDef,
     CreateLoadBalancerPolicyInputRequestTypeDef,
+    LoadBalancerAttributesOutputTypeDef,
     LoadBalancerAttributesTypeDef,
     DeregisterEndPointsInputRequestTypeDef,
-    DeregisterEndPointsOutputTypeDef,
     DescribeEndPointStateInputRequestTypeDef,
     RegisterEndPointsInputRequestTypeDef,
+    DeregisterEndPointsOutputTypeDef,
     RegisterEndPointsOutputTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     DescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     DescribeEndPointStateOutputTypeDef,
     PoliciesTypeDef,
+    ListenerDescriptionTypeDef,
     PolicyDescriptionTypeDef,
     PolicyTypeDescriptionTypeDef,
     RemoveTagsInputRequestTypeDef,
-    DescribeTagsOutputTypeDef,
+    TagDescriptionTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
-    ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
+    ModifyLoadBalancerAttributesInputRequestTypeDef,
     LoadBalancerDescriptionTypeDef,
     DescribeLoadBalancerPoliciesOutputTypeDef,
     DescribeLoadBalancerPolicyTypesOutputTypeDef,
+    DescribeTagsOutputTypeDef,
     DescribeAccessPointsOutputTypeDef,
 )
 
 
-def get_structure() -> AccessLogTypeDef:
+def get_structure() -> AccessLogOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elb-1.28.0/mypy_boto3_elb.egg-info/SOURCES.txt` & `mypy-boto3-elb-1.28.12/mypy_boto3_elb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.28.0/setup.py` & `mypy-boto3-elb-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elb",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_elb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticLoadBalancing 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ElasticLoadBalancing 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

