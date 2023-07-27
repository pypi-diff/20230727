# Comparing `tmp/mypy-boto3-appstream-1.28.0.tar.gz` & `tmp/mypy-boto3-appstream-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appstream-1.28.0.tar", last modified: Thu Jul  6 20:58:58 2023, max compression
+gzip compressed data, was "mypy-boto3-appstream-1.28.12.tar", last modified: Thu Jul 27 05:34:18 2023, max compression
```

## Comparing `mypy-boto3-appstream-1.28.0.tar` & `mypy-boto3-appstream-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.814221 mypy-boto3-appstream-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:33:36.000000 mypy-boto3-appstream-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-07-06 20:58:58.802221 mypy-boto3-appstream-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21934 2023-07-06 20:33:36.000000 mypy-boto3-appstream-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.790221 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-06 20:33:36.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-06 20:33:36.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:33:36.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57916 2023-07-06 20:33:37.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57822 2023-07-06 20:33:37.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-07-06 20:33:39.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-07-06 20:33:37.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-07-06 20:33:37.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-07-06 20:33:37.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:33:36.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69713 2023-07-06 20:33:40.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69616 2023-07-06 20:33:39.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:33:36.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-06 20:33:37.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-06 20:33:37.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.802221 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-07-06 20:58:58.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-06 20:58:58.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:58.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 20:58:58.000000 mypy-boto3-appstream-1.28.0/mypy_boto3_appstream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:58.814221 mypy-boto3-appstream-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:33:36.000000 mypy-boto3-appstream-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.620576 mypy-boto3-appstream-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23892 2023-07-27 05:34:18.620576 mypy-boto3-appstream-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22397 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.616577 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57916 2023-07-27 05:17:35.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57822 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-07-27 05:17:35.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-27 05:17:35.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-07-27 05:17:35.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-07-27 05:17:35.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    74161 2023-07-27 05:17:37.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74054 2023-07-27 05:17:36.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-27 05:17:35.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-27 05:17:35.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.620576 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23892 2023-07-27 05:34:18.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-27 05:34:18.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:18.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:18.000000 mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:18.620576 mypy-boto3-appstream-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:17:34.000000 mypy-boto3-appstream-1.28.12/setup.py
```

### Comparing `mypy-boto3-appstream-1.28.0/LICENSE` & `mypy-boto3-appstream-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.0/PKG-INFO` & `mypy-boto3-appstream-1.28.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appstream
-Version: 1.28.0
-Summary: Type annotations for boto3.AppStream 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AppStream 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-appstream"></a>
 
 # mypy-boto3-appstream
 
 [![PyPI - mypy-boto3-appstream](https://img.shields.io/pypi/v/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appstream?color=blue)](https://pypistats.org/packages/mypy-boto3-appstream)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appstream)](https://pepy.tech/project/mypy-boto3-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppStream 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[boto3.AppStream 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
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
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -415,36 +415,40 @@
 ### Typed dictionaries
 
 `mypy_boto3_appstream.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appstream.type_defs import (
+    AccessEndpointOutputTypeDef,
     AccessEndpointTypeDef,
     AppBlockBuilderAppBlockAssociationTypeDef,
     AppBlockBuilderStateChangeReasonTypeDef,
     ResourceErrorTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigOutputTypeDef,
     ErrorDetailsTypeDef,
-    S3LocationTypeDef,
+    S3LocationOutputTypeDef,
     ApplicationFleetAssociationTypeDef,
     ApplicationSettingsResponseTypeDef,
     ApplicationSettingsTypeDef,
     AssociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     AssociateApplicationFleetRequestRequestTypeDef,
     AssociateApplicationToEntitlementRequestRequestTypeDef,
     AssociateFleetRequestRequestTypeDef,
     UserStackAssociationTypeDef,
+    CertificateBasedAuthPropertiesOutputTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityStatusTypeDef,
     ComputeCapacityTypeDef,
     CopyImageRequestRequestTypeDef,
     CopyImageResponseTypeDef,
+    VpcConfigTypeDef,
     CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
     CreateAppBlockBuilderStreamingURLResultTypeDef,
+    S3LocationTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
     CreateImageBuilderStreamingURLResultTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
@@ -484,28 +488,33 @@
     DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeSessionsRequestRequestTypeDef,
     DescribeStacksRequestDescribeStacksPaginateTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeUsageReportSubscriptionsRequestRequestTypeDef,
     DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
     DescribeUserStackAssociationsRequestRequestTypeDef,
+    UserStackAssociationOutputTypeDef,
     DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UserTypeDef,
+    ServiceAccountCredentialsOutputTypeDef,
     DisableUserRequestRequestTypeDef,
     DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     DisassociateApplicationFleetRequestRequestTypeDef,
     DisassociateApplicationFromEntitlementRequestRequestTypeDef,
     DisassociateFleetRequestRequestTypeDef,
+    DomainJoinInfoOutputTypeDef,
     EnableUserRequestRequestTypeDef,
     EntitledApplicationTypeDef,
+    EntitlementAttributeOutputTypeDef,
     ExpireSessionRequestRequestTypeDef,
     FleetErrorTypeDef,
     ImageBuilderStateChangeReasonTypeDef,
     NetworkAccessConfigurationTypeDef,
+    ImagePermissionsOutputTypeDef,
     ImagePermissionsTypeDef,
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
     ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
     ListAssociatedFleetsResultTypeDef,
     ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
@@ -513,52 +522,56 @@
     ListAssociatedStacksResultTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     StackErrorTypeDef,
+    StorageConnectorOutputTypeDef,
+    StreamingExperienceSettingsOutputTypeDef,
+    UserSettingOutputTypeDef,
     StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
     StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AssociateAppBlockBuilderAppBlockResultTypeDef,
     DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
     AppBlockBuilderTypeDef,
-    CreateAppBlockBuilderRequestRequestTypeDef,
-    UpdateAppBlockBuilderRequestRequestTypeDef,
     ApplicationTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    ScriptDetailsTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
+    ScriptDetailsOutputTypeDef,
     AssociateApplicationFleetResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
     BatchAssociateUserStackRequestRequestTypeDef,
     BatchDisassociateUserStackRequestRequestTypeDef,
-    DescribeUserStackAssociationsResultTypeDef,
-    UserStackAssociationErrorTypeDef,
+    CreateAppBlockBuilderRequestRequestTypeDef,
+    UpdateAppBlockBuilderRequestRequestTypeDef,
+    CreateApplicationRequestRequestTypeDef,
+    ScriptDetailsTypeDef,
+    UpdateApplicationRequestRequestTypeDef,
     CreateDirectoryConfigRequestRequestTypeDef,
-    DirectoryConfigTypeDef,
     UpdateDirectoryConfigRequestRequestTypeDef,
     CreateEntitlementRequestRequestTypeDef,
-    EntitlementTypeDef,
     UpdateEntitlementRequestRequestTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateImageBuilderRequestRequestTypeDef,
     UpdateFleetRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     UpdateStackRequestRequestTypeDef,
     DescribeFleetsRequestFleetStartedWaitTypeDef,
     DescribeFleetsRequestFleetStoppedWaitTypeDef,
+    DescribeUserStackAssociationsResultTypeDef,
+    UserStackAssociationErrorTypeDef,
     DescribeUsersResultTypeDef,
+    DirectoryConfigTypeDef,
     ListEntitledApplicationsResultTypeDef,
+    EntitlementTypeDef,
     FleetTypeDef,
     ImageBuilderTypeDef,
     SessionTypeDef,
     SharedImagePermissionsTypeDef,
     UpdateImagePermissionsRequestRequestTypeDef,
     UsageReportSubscriptionTypeDef,
     StackTypeDef,
@@ -599,15 +612,15 @@
     DeleteImageResultTypeDef,
     DescribeImagesResultTypeDef,
     CreateAppBlockResultTypeDef,
     DescribeAppBlocksResultTypeDef,
 )
 
 
-def get_structure() -> AccessEndpointTypeDef:
+def get_structure() -> AccessEndpointOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appstream-1.28.0/README.md` & `mypy-boto3-appstream-1.28.12/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-appstream"></a>
 
 # mypy-boto3-appstream
 
 [![PyPI - mypy-boto3-appstream](https://img.shields.io/pypi/v/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appstream?color=blue)](https://pypistats.org/packages/mypy-boto3-appstream)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appstream)](https://pepy.tech/project/mypy-boto3-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppStream 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[boto3.AppStream 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
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
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -383,36 +383,40 @@
 ### Typed dictionaries
 
 `mypy_boto3_appstream.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appstream.type_defs import (
+    AccessEndpointOutputTypeDef,
     AccessEndpointTypeDef,
     AppBlockBuilderAppBlockAssociationTypeDef,
     AppBlockBuilderStateChangeReasonTypeDef,
     ResourceErrorTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigOutputTypeDef,
     ErrorDetailsTypeDef,
-    S3LocationTypeDef,
+    S3LocationOutputTypeDef,
     ApplicationFleetAssociationTypeDef,
     ApplicationSettingsResponseTypeDef,
     ApplicationSettingsTypeDef,
     AssociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     AssociateApplicationFleetRequestRequestTypeDef,
     AssociateApplicationToEntitlementRequestRequestTypeDef,
     AssociateFleetRequestRequestTypeDef,
     UserStackAssociationTypeDef,
+    CertificateBasedAuthPropertiesOutputTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityStatusTypeDef,
     ComputeCapacityTypeDef,
     CopyImageRequestRequestTypeDef,
     CopyImageResponseTypeDef,
+    VpcConfigTypeDef,
     CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
     CreateAppBlockBuilderStreamingURLResultTypeDef,
+    S3LocationTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
     CreateImageBuilderStreamingURLResultTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
@@ -452,28 +456,33 @@
     DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeSessionsRequestRequestTypeDef,
     DescribeStacksRequestDescribeStacksPaginateTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeUsageReportSubscriptionsRequestRequestTypeDef,
     DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
     DescribeUserStackAssociationsRequestRequestTypeDef,
+    UserStackAssociationOutputTypeDef,
     DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UserTypeDef,
+    ServiceAccountCredentialsOutputTypeDef,
     DisableUserRequestRequestTypeDef,
     DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     DisassociateApplicationFleetRequestRequestTypeDef,
     DisassociateApplicationFromEntitlementRequestRequestTypeDef,
     DisassociateFleetRequestRequestTypeDef,
+    DomainJoinInfoOutputTypeDef,
     EnableUserRequestRequestTypeDef,
     EntitledApplicationTypeDef,
+    EntitlementAttributeOutputTypeDef,
     ExpireSessionRequestRequestTypeDef,
     FleetErrorTypeDef,
     ImageBuilderStateChangeReasonTypeDef,
     NetworkAccessConfigurationTypeDef,
+    ImagePermissionsOutputTypeDef,
     ImagePermissionsTypeDef,
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
     ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
     ListAssociatedFleetsResultTypeDef,
     ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
@@ -481,52 +490,56 @@
     ListAssociatedStacksResultTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     StackErrorTypeDef,
+    StorageConnectorOutputTypeDef,
+    StreamingExperienceSettingsOutputTypeDef,
+    UserSettingOutputTypeDef,
     StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
     StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AssociateAppBlockBuilderAppBlockResultTypeDef,
     DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
     AppBlockBuilderTypeDef,
-    CreateAppBlockBuilderRequestRequestTypeDef,
-    UpdateAppBlockBuilderRequestRequestTypeDef,
     ApplicationTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    ScriptDetailsTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
+    ScriptDetailsOutputTypeDef,
     AssociateApplicationFleetResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
     BatchAssociateUserStackRequestRequestTypeDef,
     BatchDisassociateUserStackRequestRequestTypeDef,
-    DescribeUserStackAssociationsResultTypeDef,
-    UserStackAssociationErrorTypeDef,
+    CreateAppBlockBuilderRequestRequestTypeDef,
+    UpdateAppBlockBuilderRequestRequestTypeDef,
+    CreateApplicationRequestRequestTypeDef,
+    ScriptDetailsTypeDef,
+    UpdateApplicationRequestRequestTypeDef,
     CreateDirectoryConfigRequestRequestTypeDef,
-    DirectoryConfigTypeDef,
     UpdateDirectoryConfigRequestRequestTypeDef,
     CreateEntitlementRequestRequestTypeDef,
-    EntitlementTypeDef,
     UpdateEntitlementRequestRequestTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateImageBuilderRequestRequestTypeDef,
     UpdateFleetRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     UpdateStackRequestRequestTypeDef,
     DescribeFleetsRequestFleetStartedWaitTypeDef,
     DescribeFleetsRequestFleetStoppedWaitTypeDef,
+    DescribeUserStackAssociationsResultTypeDef,
+    UserStackAssociationErrorTypeDef,
     DescribeUsersResultTypeDef,
+    DirectoryConfigTypeDef,
     ListEntitledApplicationsResultTypeDef,
+    EntitlementTypeDef,
     FleetTypeDef,
     ImageBuilderTypeDef,
     SessionTypeDef,
     SharedImagePermissionsTypeDef,
     UpdateImagePermissionsRequestRequestTypeDef,
     UsageReportSubscriptionTypeDef,
     StackTypeDef,
@@ -567,15 +580,15 @@
     DeleteImageResultTypeDef,
     DescribeImagesResultTypeDef,
     CreateAppBlockResultTypeDef,
     DescribeAppBlocksResultTypeDef,
 )
 
 
-def get_structure() -> AccessEndpointTypeDef:
+def get_structure() -> AccessEndpointOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/__init__.py` & `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/__init__.pyi` & `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/__main__.py` & `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppStream 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.AppStream 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream\nOther"
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

### Comparing `mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/client.py` & `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/client.pyi` & `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/literals.py` & `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,14 +320,15 @@
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
@@ -406,26 +407,28 @@
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

### Comparing `mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/literals.pyi` & `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -318,14 +318,15 @@
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
@@ -404,26 +405,28 @@
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

### Comparing `mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/paginator.py` & `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/paginator.pyi` & `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/type_defs.py` & `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for appstream service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_appstream.type_defs import AccessEndpointTypeDef
+    from mypy_boto3_appstream.type_defs import AccessEndpointOutputTypeDef
 
-    data: AccessEndpointTypeDef = {...}
+    data: AccessEndpointOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -55,36 +55,40 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AccessEndpointOutputTypeDef",
     "AccessEndpointTypeDef",
     "AppBlockBuilderAppBlockAssociationTypeDef",
     "AppBlockBuilderStateChangeReasonTypeDef",
     "ResourceErrorTypeDef",
-    "VpcConfigTypeDef",
+    "VpcConfigOutputTypeDef",
     "ErrorDetailsTypeDef",
-    "S3LocationTypeDef",
+    "S3LocationOutputTypeDef",
     "ApplicationFleetAssociationTypeDef",
     "ApplicationSettingsResponseTypeDef",
     "ApplicationSettingsTypeDef",
     "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "AssociateApplicationFleetRequestRequestTypeDef",
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     "AssociateFleetRequestRequestTypeDef",
     "UserStackAssociationTypeDef",
+    "CertificateBasedAuthPropertiesOutputTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
     "ComputeCapacityStatusTypeDef",
     "ComputeCapacityTypeDef",
     "CopyImageRequestRequestTypeDef",
     "CopyImageResponseTypeDef",
+    "VpcConfigTypeDef",
     "CreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
     "CreateAppBlockBuilderStreamingURLResultTypeDef",
+    "S3LocationTypeDef",
     "ServiceAccountCredentialsTypeDef",
     "EntitlementAttributeTypeDef",
     "DomainJoinInfoTypeDef",
     "CreateImageBuilderStreamingURLRequestRequestTypeDef",
     "CreateImageBuilderStreamingURLResultTypeDef",
     "StorageConnectorTypeDef",
     "StreamingExperienceSettingsTypeDef",
@@ -124,28 +128,33 @@
     "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     "DescribeSessionsRequestRequestTypeDef",
     "DescribeStacksRequestDescribeStacksPaginateTypeDef",
     "DescribeStacksRequestRequestTypeDef",
     "DescribeUsageReportSubscriptionsRequestRequestTypeDef",
     "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
     "DescribeUserStackAssociationsRequestRequestTypeDef",
+    "UserStackAssociationOutputTypeDef",
     "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
     "UserTypeDef",
+    "ServiceAccountCredentialsOutputTypeDef",
     "DisableUserRequestRequestTypeDef",
     "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "DisassociateApplicationFleetRequestRequestTypeDef",
     "DisassociateApplicationFromEntitlementRequestRequestTypeDef",
     "DisassociateFleetRequestRequestTypeDef",
+    "DomainJoinInfoOutputTypeDef",
     "EnableUserRequestRequestTypeDef",
     "EntitledApplicationTypeDef",
+    "EntitlementAttributeOutputTypeDef",
     "ExpireSessionRequestRequestTypeDef",
     "FleetErrorTypeDef",
     "ImageBuilderStateChangeReasonTypeDef",
     "NetworkAccessConfigurationTypeDef",
+    "ImagePermissionsOutputTypeDef",
     "ImagePermissionsTypeDef",
     "ImageStateChangeReasonTypeDef",
     "LastReportGenerationExecutionErrorTypeDef",
     "ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
     "ListAssociatedFleetsRequestRequestTypeDef",
     "ListAssociatedFleetsResultTypeDef",
     "ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
@@ -153,52 +162,56 @@
     "ListAssociatedStacksResultTypeDef",
     "ListEntitledApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "StackErrorTypeDef",
+    "StorageConnectorOutputTypeDef",
+    "StreamingExperienceSettingsOutputTypeDef",
+    "UserSettingOutputTypeDef",
     "StartAppBlockBuilderRequestRequestTypeDef",
     "StartFleetRequestRequestTypeDef",
     "StartImageBuilderRequestRequestTypeDef",
     "StopAppBlockBuilderRequestRequestTypeDef",
     "StopFleetRequestRequestTypeDef",
     "StopImageBuilderRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AssociateAppBlockBuilderAppBlockResultTypeDef",
     "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
     "AppBlockBuilderTypeDef",
-    "CreateAppBlockBuilderRequestRequestTypeDef",
-    "UpdateAppBlockBuilderRequestRequestTypeDef",
     "ApplicationTypeDef",
-    "CreateApplicationRequestRequestTypeDef",
-    "ScriptDetailsTypeDef",
-    "UpdateApplicationRequestRequestTypeDef",
+    "ScriptDetailsOutputTypeDef",
     "AssociateApplicationFleetResultTypeDef",
     "DescribeApplicationFleetAssociationsResultTypeDef",
     "BatchAssociateUserStackRequestRequestTypeDef",
     "BatchDisassociateUserStackRequestRequestTypeDef",
-    "DescribeUserStackAssociationsResultTypeDef",
-    "UserStackAssociationErrorTypeDef",
+    "CreateAppBlockBuilderRequestRequestTypeDef",
+    "UpdateAppBlockBuilderRequestRequestTypeDef",
+    "CreateApplicationRequestRequestTypeDef",
+    "ScriptDetailsTypeDef",
+    "UpdateApplicationRequestRequestTypeDef",
     "CreateDirectoryConfigRequestRequestTypeDef",
-    "DirectoryConfigTypeDef",
     "UpdateDirectoryConfigRequestRequestTypeDef",
     "CreateEntitlementRequestRequestTypeDef",
-    "EntitlementTypeDef",
     "UpdateEntitlementRequestRequestTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateImageBuilderRequestRequestTypeDef",
     "UpdateFleetRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "UpdateStackRequestRequestTypeDef",
     "DescribeFleetsRequestFleetStartedWaitTypeDef",
     "DescribeFleetsRequestFleetStoppedWaitTypeDef",
+    "DescribeUserStackAssociationsResultTypeDef",
+    "UserStackAssociationErrorTypeDef",
     "DescribeUsersResultTypeDef",
+    "DirectoryConfigTypeDef",
     "ListEntitledApplicationsResultTypeDef",
+    "EntitlementTypeDef",
     "FleetTypeDef",
     "ImageBuilderTypeDef",
     "SessionTypeDef",
     "SharedImagePermissionsTypeDef",
     "UpdateImagePermissionsRequestRequestTypeDef",
     "UsageReportSubscriptionTypeDef",
     "StackTypeDef",
@@ -238,14 +251,35 @@
     "CreateUpdatedImageResultTypeDef",
     "DeleteImageResultTypeDef",
     "DescribeImagesResultTypeDef",
     "CreateAppBlockResultTypeDef",
     "DescribeAppBlocksResultTypeDef",
 )
 
+_RequiredAccessEndpointOutputTypeDef = TypedDict(
+    "_RequiredAccessEndpointOutputTypeDef",
+    {
+        "EndpointType": Literal["STREAMING"],
+    },
+)
+_OptionalAccessEndpointOutputTypeDef = TypedDict(
+    "_OptionalAccessEndpointOutputTypeDef",
+    {
+        "VpceId": str,
+    },
+    total=False,
+)
+
+
+class AccessEndpointOutputTypeDef(
+    _RequiredAccessEndpointOutputTypeDef, _OptionalAccessEndpointOutputTypeDef
+):
+    pass
+
+
 _RequiredAccessEndpointTypeDef = TypedDict(
     "_RequiredAccessEndpointTypeDef",
     {
         "EndpointType": Literal["STREAMING"],
     },
 )
 _OptionalAccessEndpointTypeDef = TypedDict(
@@ -284,48 +318,48 @@
         "ErrorCode": FleetErrorCodeType,
         "ErrorMessage": str,
         "ErrorTimestamp": datetime,
     },
     total=False,
 )
 
-VpcConfigTypeDef = TypedDict(
-    "VpcConfigTypeDef",
+VpcConfigOutputTypeDef = TypedDict(
+    "VpcConfigOutputTypeDef",
     {
-        "SubnetIds": Sequence[str],
-        "SecurityGroupIds": Sequence[str],
+        "SubnetIds": List[str],
+        "SecurityGroupIds": List[str],
     },
     total=False,
 )
 
 ErrorDetailsTypeDef = TypedDict(
     "ErrorDetailsTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-_RequiredS3LocationTypeDef = TypedDict(
-    "_RequiredS3LocationTypeDef",
+_RequiredS3LocationOutputTypeDef = TypedDict(
+    "_RequiredS3LocationOutputTypeDef",
     {
         "S3Bucket": str,
     },
 )
-_OptionalS3LocationTypeDef = TypedDict(
-    "_OptionalS3LocationTypeDef",
+_OptionalS3LocationOutputTypeDef = TypedDict(
+    "_OptionalS3LocationOutputTypeDef",
     {
         "S3Key": str,
     },
     total=False,
 )
 
 
-class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
+class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
     pass
 
 
 ApplicationFleetAssociationTypeDef = TypedDict(
     "ApplicationFleetAssociationTypeDef",
     {
         "FleetName": str,
@@ -416,14 +450,23 @@
 
 class UserStackAssociationTypeDef(
     _RequiredUserStackAssociationTypeDef, _OptionalUserStackAssociationTypeDef
 ):
     pass
 
 
+CertificateBasedAuthPropertiesOutputTypeDef = TypedDict(
+    "CertificateBasedAuthPropertiesOutputTypeDef",
+    {
+        "Status": CertificateBasedAuthStatusType,
+        "CertificateAuthorityArn": str,
+    },
+    total=False,
+)
+
 CertificateBasedAuthPropertiesTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesTypeDef",
     {
         "Status": CertificateBasedAuthStatusType,
         "CertificateAuthorityArn": str,
     },
     total=False,
@@ -486,14 +529,23 @@
     "CopyImageResponseTypeDef",
     {
         "DestinationImageName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
+    {
+        "SubnetIds": Sequence[str],
+        "SecurityGroupIds": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
     {
         "AppBlockBuilderName": str,
     },
 )
 _OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
@@ -517,14 +569,33 @@
     {
         "StreamingURL": str,
         "Expires": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredS3LocationTypeDef = TypedDict(
+    "_RequiredS3LocationTypeDef",
+    {
+        "S3Bucket": str,
+    },
+)
+_OptionalS3LocationTypeDef = TypedDict(
+    "_OptionalS3LocationTypeDef",
+    {
+        "S3Key": str,
+    },
+    total=False,
+)
+
+
+class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
+    pass
+
+
 ServiceAccountCredentialsTypeDef = TypedDict(
     "ServiceAccountCredentialsTypeDef",
     {
         "AccountName": str,
         "AccountPassword": str,
     },
 )
@@ -1071,14 +1142,37 @@
         "AuthenticationType": AuthenticationTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredUserStackAssociationOutputTypeDef = TypedDict(
+    "_RequiredUserStackAssociationOutputTypeDef",
+    {
+        "StackName": str,
+        "UserName": str,
+        "AuthenticationType": AuthenticationTypeType,
+    },
+)
+_OptionalUserStackAssociationOutputTypeDef = TypedDict(
+    "_OptionalUserStackAssociationOutputTypeDef",
+    {
+        "SendEmailNotification": bool,
+    },
+    total=False,
+)
+
+
+class UserStackAssociationOutputTypeDef(
+    _RequiredUserStackAssociationOutputTypeDef, _OptionalUserStackAssociationOutputTypeDef
+):
+    pass
+
+
 _RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
     "_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef",
     {
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 _OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
@@ -1140,14 +1234,22 @@
 )
 
 
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
 
+ServiceAccountCredentialsOutputTypeDef = TypedDict(
+    "ServiceAccountCredentialsOutputTypeDef",
+    {
+        "AccountName": str,
+        "AccountPassword": str,
+    },
+)
+
 DisableUserRequestRequestTypeDef = TypedDict(
     "DisableUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
@@ -1181,14 +1283,23 @@
     "DisassociateFleetRequestRequestTypeDef",
     {
         "FleetName": str,
         "StackName": str,
     },
 )
 
+DomainJoinInfoOutputTypeDef = TypedDict(
+    "DomainJoinInfoOutputTypeDef",
+    {
+        "DirectoryName": str,
+        "OrganizationalUnitDistinguishedName": str,
+    },
+    total=False,
+)
+
 EnableUserRequestRequestTypeDef = TypedDict(
     "EnableUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
@@ -1196,14 +1307,22 @@
 EntitledApplicationTypeDef = TypedDict(
     "EntitledApplicationTypeDef",
     {
         "ApplicationIdentifier": str,
     },
 )
 
+EntitlementAttributeOutputTypeDef = TypedDict(
+    "EntitlementAttributeOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
 ExpireSessionRequestRequestTypeDef = TypedDict(
     "ExpireSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
@@ -1230,14 +1349,23 @@
     {
         "EniPrivateIpAddress": str,
         "EniId": str,
     },
     total=False,
 )
 
+ImagePermissionsOutputTypeDef = TypedDict(
+    "ImagePermissionsOutputTypeDef",
+    {
+        "allowFleet": bool,
+        "allowImageBuilder": bool,
+    },
+    total=False,
+)
+
 ImagePermissionsTypeDef = TypedDict(
     "ImagePermissionsTypeDef",
     {
         "allowFleet": bool,
         "allowImageBuilder": bool,
     },
     total=False,
@@ -1432,14 +1560,52 @@
     {
         "ErrorCode": StackErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+_RequiredStorageConnectorOutputTypeDef = TypedDict(
+    "_RequiredStorageConnectorOutputTypeDef",
+    {
+        "ConnectorType": StorageConnectorTypeType,
+    },
+)
+_OptionalStorageConnectorOutputTypeDef = TypedDict(
+    "_OptionalStorageConnectorOutputTypeDef",
+    {
+        "ResourceIdentifier": str,
+        "Domains": List[str],
+    },
+    total=False,
+)
+
+
+class StorageConnectorOutputTypeDef(
+    _RequiredStorageConnectorOutputTypeDef, _OptionalStorageConnectorOutputTypeDef
+):
+    pass
+
+
+StreamingExperienceSettingsOutputTypeDef = TypedDict(
+    "StreamingExperienceSettingsOutputTypeDef",
+    {
+        "PreferredProtocol": PreferredProtocolType,
+    },
+    total=False,
+)
+
+UserSettingOutputTypeDef = TypedDict(
+    "UserSettingOutputTypeDef",
+    {
+        "Action": ActionType,
+        "Permission": PermissionType,
+    },
+)
+
 StartAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "StartAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1528,38 +1694,114 @@
 _RequiredAppBlockBuilderTypeDef = TypedDict(
     "_RequiredAppBlockBuilderTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Platform": Literal["WINDOWS_SERVER_2019"],
         "InstanceType": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "State": AppBlockBuilderStateType,
     },
 )
 _OptionalAppBlockBuilderTypeDef = TypedDict(
     "_OptionalAppBlockBuilderTypeDef",
     {
         "DisplayName": str,
         "Description": str,
         "EnableDefaultInternetAccess": bool,
         "IamRoleArn": str,
         "CreatedTime": datetime,
         "AppBlockBuilderErrors": List[ResourceErrorTypeDef],
         "StateChangeReason": AppBlockBuilderStateChangeReasonTypeDef,
-        "AccessEndpoints": List[AccessEndpointTypeDef],
+        "AccessEndpoints": List[AccessEndpointOutputTypeDef],
     },
     total=False,
 )
 
 
 class AppBlockBuilderTypeDef(_RequiredAppBlockBuilderTypeDef, _OptionalAppBlockBuilderTypeDef):
     pass
 
 
+ApplicationTypeDef = TypedDict(
+    "ApplicationTypeDef",
+    {
+        "Name": str,
+        "DisplayName": str,
+        "IconURL": str,
+        "LaunchPath": str,
+        "LaunchParameters": str,
+        "Enabled": bool,
+        "Metadata": Dict[str, str],
+        "WorkingDirectory": str,
+        "Description": str,
+        "Arn": str,
+        "AppBlockArn": str,
+        "IconS3Location": S3LocationOutputTypeDef,
+        "Platforms": List[PlatformTypeType],
+        "InstanceFamilies": List[str],
+        "CreatedTime": datetime,
+    },
+    total=False,
+)
+
+_RequiredScriptDetailsOutputTypeDef = TypedDict(
+    "_RequiredScriptDetailsOutputTypeDef",
+    {
+        "ScriptS3Location": S3LocationOutputTypeDef,
+        "ExecutablePath": str,
+        "TimeoutInSeconds": int,
+    },
+)
+_OptionalScriptDetailsOutputTypeDef = TypedDict(
+    "_OptionalScriptDetailsOutputTypeDef",
+    {
+        "ExecutableParameters": str,
+    },
+    total=False,
+)
+
+
+class ScriptDetailsOutputTypeDef(
+    _RequiredScriptDetailsOutputTypeDef, _OptionalScriptDetailsOutputTypeDef
+):
+    pass
+
+
+AssociateApplicationFleetResultTypeDef = TypedDict(
+    "AssociateApplicationFleetResultTypeDef",
+    {
+        "ApplicationFleetAssociation": ApplicationFleetAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeApplicationFleetAssociationsResultTypeDef = TypedDict(
+    "DescribeApplicationFleetAssociationsResultTypeDef",
+    {
+        "ApplicationFleetAssociations": List[ApplicationFleetAssociationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchAssociateUserStackRequestRequestTypeDef = TypedDict(
+    "BatchAssociateUserStackRequestRequestTypeDef",
+    {
+        "UserStackAssociations": Sequence[UserStackAssociationTypeDef],
+    },
+)
+
+BatchDisassociateUserStackRequestRequestTypeDef = TypedDict(
+    "BatchDisassociateUserStackRequestRequestTypeDef",
+    {
+        "UserStackAssociations": Sequence[UserStackAssociationTypeDef],
+    },
+)
+
 _RequiredCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
         "Platform": Literal["WINDOWS_SERVER_2019"],
         "InstanceType": str,
         "VpcConfig": VpcConfigTypeDef,
@@ -1612,36 +1854,14 @@
 class UpdateAppBlockBuilderRequestRequestTypeDef(
     _RequiredUpdateAppBlockBuilderRequestRequestTypeDef,
     _OptionalUpdateAppBlockBuilderRequestRequestTypeDef,
 ):
     pass
 
 
-ApplicationTypeDef = TypedDict(
-    "ApplicationTypeDef",
-    {
-        "Name": str,
-        "DisplayName": str,
-        "IconURL": str,
-        "LaunchPath": str,
-        "LaunchParameters": str,
-        "Enabled": bool,
-        "Metadata": Dict[str, str],
-        "WorkingDirectory": str,
-        "Description": str,
-        "Arn": str,
-        "AppBlockArn": str,
-        "IconS3Location": S3LocationTypeDef,
-        "Platforms": List[PlatformTypeType],
-        "InstanceFamilies": List[str],
-        "CreatedTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "Name": str,
         "IconS3Location": S3LocationTypeDef,
         "LaunchPath": str,
         "Platforms": Sequence[PlatformTypeType],
@@ -1713,64 +1933,14 @@
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
 
-AssociateApplicationFleetResultTypeDef = TypedDict(
-    "AssociateApplicationFleetResultTypeDef",
-    {
-        "ApplicationFleetAssociation": ApplicationFleetAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeApplicationFleetAssociationsResultTypeDef = TypedDict(
-    "DescribeApplicationFleetAssociationsResultTypeDef",
-    {
-        "ApplicationFleetAssociations": List[ApplicationFleetAssociationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchAssociateUserStackRequestRequestTypeDef = TypedDict(
-    "BatchAssociateUserStackRequestRequestTypeDef",
-    {
-        "UserStackAssociations": Sequence[UserStackAssociationTypeDef],
-    },
-)
-
-BatchDisassociateUserStackRequestRequestTypeDef = TypedDict(
-    "BatchDisassociateUserStackRequestRequestTypeDef",
-    {
-        "UserStackAssociations": Sequence[UserStackAssociationTypeDef],
-    },
-)
-
-DescribeUserStackAssociationsResultTypeDef = TypedDict(
-    "DescribeUserStackAssociationsResultTypeDef",
-    {
-        "UserStackAssociations": List[UserStackAssociationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UserStackAssociationErrorTypeDef = TypedDict(
-    "UserStackAssociationErrorTypeDef",
-    {
-        "UserStackAssociation": UserStackAssociationTypeDef,
-        "ErrorCode": UserStackAssociationErrorCodeType,
-        "ErrorMessage": str,
-    },
-    total=False,
-)
-
 _RequiredCreateDirectoryConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDirectoryConfigRequestRequestTypeDef",
     {
         "DirectoryName": str,
         "OrganizationalUnitDistinguishedNames": Sequence[str],
     },
 )
@@ -1787,36 +1957,14 @@
 class CreateDirectoryConfigRequestRequestTypeDef(
     _RequiredCreateDirectoryConfigRequestRequestTypeDef,
     _OptionalCreateDirectoryConfigRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDirectoryConfigTypeDef = TypedDict(
-    "_RequiredDirectoryConfigTypeDef",
-    {
-        "DirectoryName": str,
-    },
-)
-_OptionalDirectoryConfigTypeDef = TypedDict(
-    "_OptionalDirectoryConfigTypeDef",
-    {
-        "OrganizationalUnitDistinguishedNames": List[str],
-        "ServiceAccountCredentials": ServiceAccountCredentialsTypeDef,
-        "CreatedTime": datetime,
-        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
-    },
-    total=False,
-)
-
-
-class DirectoryConfigTypeDef(_RequiredDirectoryConfigTypeDef, _OptionalDirectoryConfigTypeDef):
-    pass
-
-
 _RequiredUpdateDirectoryConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDirectoryConfigRequestRequestTypeDef",
     {
         "DirectoryName": str,
     },
 )
 _OptionalUpdateDirectoryConfigRequestRequestTypeDef = TypedDict(
@@ -1857,38 +2005,14 @@
 
 class CreateEntitlementRequestRequestTypeDef(
     _RequiredCreateEntitlementRequestRequestTypeDef, _OptionalCreateEntitlementRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredEntitlementTypeDef = TypedDict(
-    "_RequiredEntitlementTypeDef",
-    {
-        "Name": str,
-        "StackName": str,
-        "AppVisibility": AppVisibilityType,
-        "Attributes": List[EntitlementAttributeTypeDef],
-    },
-)
-_OptionalEntitlementTypeDef = TypedDict(
-    "_OptionalEntitlementTypeDef",
-    {
-        "Description": str,
-        "CreatedTime": datetime,
-        "LastModifiedTime": datetime,
-    },
-    total=False,
-)
-
-
-class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
-    pass
-
-
 _RequiredUpdateEntitlementRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEntitlementRequestRequestTypeDef",
     {
         "Name": str,
         "StackName": str,
     },
 )
@@ -2089,32 +2213,97 @@
         "Names": Sequence[str],
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+DescribeUserStackAssociationsResultTypeDef = TypedDict(
+    "DescribeUserStackAssociationsResultTypeDef",
+    {
+        "UserStackAssociations": List[UserStackAssociationOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UserStackAssociationErrorTypeDef = TypedDict(
+    "UserStackAssociationErrorTypeDef",
+    {
+        "UserStackAssociation": UserStackAssociationOutputTypeDef,
+        "ErrorCode": UserStackAssociationErrorCodeType,
+        "ErrorMessage": str,
+    },
+    total=False,
+)
+
 DescribeUsersResultTypeDef = TypedDict(
     "DescribeUsersResultTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDirectoryConfigTypeDef = TypedDict(
+    "_RequiredDirectoryConfigTypeDef",
+    {
+        "DirectoryName": str,
+    },
+)
+_OptionalDirectoryConfigTypeDef = TypedDict(
+    "_OptionalDirectoryConfigTypeDef",
+    {
+        "OrganizationalUnitDistinguishedNames": List[str],
+        "ServiceAccountCredentials": ServiceAccountCredentialsOutputTypeDef,
+        "CreatedTime": datetime,
+        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class DirectoryConfigTypeDef(_RequiredDirectoryConfigTypeDef, _OptionalDirectoryConfigTypeDef):
+    pass
+
+
 ListEntitledApplicationsResultTypeDef = TypedDict(
     "ListEntitledApplicationsResultTypeDef",
     {
         "EntitledApplications": List[EntitledApplicationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredEntitlementTypeDef = TypedDict(
+    "_RequiredEntitlementTypeDef",
+    {
+        "Name": str,
+        "StackName": str,
+        "AppVisibility": AppVisibilityType,
+        "Attributes": List[EntitlementAttributeOutputTypeDef],
+    },
+)
+_OptionalEntitlementTypeDef = TypedDict(
+    "_OptionalEntitlementTypeDef",
+    {
+        "Description": str,
+        "CreatedTime": datetime,
+        "LastModifiedTime": datetime,
+    },
+    total=False,
+)
+
+
+class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
+    pass
+
+
 _RequiredFleetTypeDef = TypedDict(
     "_RequiredFleetTypeDef",
     {
         "Arn": str,
         "Name": str,
         "InstanceType": str,
         "ComputeCapacityStatus": ComputeCapacityStatusTypeDef,
@@ -2127,26 +2316,26 @@
         "DisplayName": str,
         "Description": str,
         "ImageName": str,
         "ImageArn": str,
         "FleetType": FleetTypeType,
         "MaxUserDurationInSeconds": int,
         "DisconnectTimeoutInSeconds": int,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "CreatedTime": datetime,
         "FleetErrors": List[FleetErrorTypeDef],
         "EnableDefaultInternetAccess": bool,
-        "DomainJoinInfo": DomainJoinInfoTypeDef,
+        "DomainJoinInfo": DomainJoinInfoOutputTypeDef,
         "IdleDisconnectTimeoutInSeconds": int,
         "IamRoleArn": str,
         "StreamView": StreamViewType,
         "Platform": PlatformTypeType,
         "MaxConcurrentSessions": int,
         "UsbDeviceFilterStrings": List[str],
-        "SessionScriptS3Location": S3LocationTypeDef,
+        "SessionScriptS3Location": S3LocationOutputTypeDef,
     },
     total=False,
 )
 
 
 class FleetTypeDef(_RequiredFleetTypeDef, _OptionalFleetTypeDef):
     pass
@@ -2161,27 +2350,27 @@
 _OptionalImageBuilderTypeDef = TypedDict(
     "_OptionalImageBuilderTypeDef",
     {
         "Arn": str,
         "ImageArn": str,
         "Description": str,
         "DisplayName": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "InstanceType": str,
         "Platform": PlatformTypeType,
         "IamRoleArn": str,
         "State": ImageBuilderStateType,
         "StateChangeReason": ImageBuilderStateChangeReasonTypeDef,
         "CreatedTime": datetime,
         "EnableDefaultInternetAccess": bool,
-        "DomainJoinInfo": DomainJoinInfoTypeDef,
+        "DomainJoinInfo": DomainJoinInfoOutputTypeDef,
         "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
         "ImageBuilderErrors": List[ResourceErrorTypeDef],
         "AppstreamAgentVersion": str,
-        "AccessEndpoints": List[AccessEndpointTypeDef],
+        "AccessEndpoints": List[AccessEndpointOutputTypeDef],
     },
     total=False,
 )
 
 
 class ImageBuilderTypeDef(_RequiredImageBuilderTypeDef, _OptionalImageBuilderTypeDef):
     pass
@@ -2214,15 +2403,15 @@
     pass
 
 
 SharedImagePermissionsTypeDef = TypedDict(
     "SharedImagePermissionsTypeDef",
     {
         "sharedAccountId": str,
-        "imagePermissions": ImagePermissionsTypeDef,
+        "imagePermissions": ImagePermissionsOutputTypeDef,
     },
 )
 
 UpdateImagePermissionsRequestRequestTypeDef = TypedDict(
     "UpdateImagePermissionsRequestRequestTypeDef",
     {
         "Name": str,
@@ -2251,23 +2440,23 @@
 _OptionalStackTypeDef = TypedDict(
     "_OptionalStackTypeDef",
     {
         "Arn": str,
         "Description": str,
         "DisplayName": str,
         "CreatedTime": datetime,
-        "StorageConnectors": List[StorageConnectorTypeDef],
+        "StorageConnectors": List[StorageConnectorOutputTypeDef],
         "RedirectURL": str,
         "FeedbackURL": str,
         "StackErrors": List[StackErrorTypeDef],
-        "UserSettings": List[UserSettingTypeDef],
+        "UserSettings": List[UserSettingOutputTypeDef],
         "ApplicationSettings": ApplicationSettingsResponseTypeDef,
-        "AccessEndpoints": List[AccessEndpointTypeDef],
+        "AccessEndpoints": List[AccessEndpointOutputTypeDef],
         "EmbedHostDomains": List[str],
-        "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
+        "StreamingExperienceSettings": StreamingExperienceSettingsOutputTypeDef,
     },
     total=False,
 )
 
 
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
@@ -2350,15 +2539,15 @@
         "Platform": PlatformTypeType,
         "Description": str,
         "StateChangeReason": ImageStateChangeReasonTypeDef,
         "Applications": List[ApplicationTypeDef],
         "CreatedTime": datetime,
         "PublicBaseImageReleasedDate": datetime,
         "AppstreamAgentVersion": str,
-        "ImagePermissions": ImagePermissionsTypeDef,
+        "ImagePermissions": ImagePermissionsOutputTypeDef,
         "ImageErrors": List[ResourceErrorTypeDef],
     },
     total=False,
 )
 
 
 class ImageTypeDef(_RequiredImageTypeDef, _OptionalImageTypeDef):
@@ -2381,18 +2570,18 @@
     },
 )
 _OptionalAppBlockTypeDef = TypedDict(
     "_OptionalAppBlockTypeDef",
     {
         "Description": str,
         "DisplayName": str,
-        "SourceS3Location": S3LocationTypeDef,
-        "SetupScriptDetails": ScriptDetailsTypeDef,
+        "SourceS3Location": S3LocationOutputTypeDef,
+        "SetupScriptDetails": ScriptDetailsOutputTypeDef,
         "CreatedTime": datetime,
-        "PostSetupScriptDetails": ScriptDetailsTypeDef,
+        "PostSetupScriptDetails": ScriptDetailsOutputTypeDef,
         "PackagingType": PackagingTypeType,
         "State": AppBlockStateType,
         "AppBlockErrors": List[ErrorDetailsTypeDef],
     },
     total=False,
 )
```

### Comparing `mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/type_defs.pyi` & `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for appstream service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_appstream.type_defs import AccessEndpointTypeDef
+    from mypy_boto3_appstream.type_defs import AccessEndpointOutputTypeDef
 
-    data: AccessEndpointTypeDef = {...}
+    data: AccessEndpointOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -54,36 +54,40 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AccessEndpointOutputTypeDef",
     "AccessEndpointTypeDef",
     "AppBlockBuilderAppBlockAssociationTypeDef",
     "AppBlockBuilderStateChangeReasonTypeDef",
     "ResourceErrorTypeDef",
-    "VpcConfigTypeDef",
+    "VpcConfigOutputTypeDef",
     "ErrorDetailsTypeDef",
-    "S3LocationTypeDef",
+    "S3LocationOutputTypeDef",
     "ApplicationFleetAssociationTypeDef",
     "ApplicationSettingsResponseTypeDef",
     "ApplicationSettingsTypeDef",
     "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "AssociateApplicationFleetRequestRequestTypeDef",
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     "AssociateFleetRequestRequestTypeDef",
     "UserStackAssociationTypeDef",
+    "CertificateBasedAuthPropertiesOutputTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
     "ComputeCapacityStatusTypeDef",
     "ComputeCapacityTypeDef",
     "CopyImageRequestRequestTypeDef",
     "CopyImageResponseTypeDef",
+    "VpcConfigTypeDef",
     "CreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
     "CreateAppBlockBuilderStreamingURLResultTypeDef",
+    "S3LocationTypeDef",
     "ServiceAccountCredentialsTypeDef",
     "EntitlementAttributeTypeDef",
     "DomainJoinInfoTypeDef",
     "CreateImageBuilderStreamingURLRequestRequestTypeDef",
     "CreateImageBuilderStreamingURLResultTypeDef",
     "StorageConnectorTypeDef",
     "StreamingExperienceSettingsTypeDef",
@@ -123,28 +127,33 @@
     "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     "DescribeSessionsRequestRequestTypeDef",
     "DescribeStacksRequestDescribeStacksPaginateTypeDef",
     "DescribeStacksRequestRequestTypeDef",
     "DescribeUsageReportSubscriptionsRequestRequestTypeDef",
     "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
     "DescribeUserStackAssociationsRequestRequestTypeDef",
+    "UserStackAssociationOutputTypeDef",
     "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
     "UserTypeDef",
+    "ServiceAccountCredentialsOutputTypeDef",
     "DisableUserRequestRequestTypeDef",
     "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "DisassociateApplicationFleetRequestRequestTypeDef",
     "DisassociateApplicationFromEntitlementRequestRequestTypeDef",
     "DisassociateFleetRequestRequestTypeDef",
+    "DomainJoinInfoOutputTypeDef",
     "EnableUserRequestRequestTypeDef",
     "EntitledApplicationTypeDef",
+    "EntitlementAttributeOutputTypeDef",
     "ExpireSessionRequestRequestTypeDef",
     "FleetErrorTypeDef",
     "ImageBuilderStateChangeReasonTypeDef",
     "NetworkAccessConfigurationTypeDef",
+    "ImagePermissionsOutputTypeDef",
     "ImagePermissionsTypeDef",
     "ImageStateChangeReasonTypeDef",
     "LastReportGenerationExecutionErrorTypeDef",
     "ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
     "ListAssociatedFleetsRequestRequestTypeDef",
     "ListAssociatedFleetsResultTypeDef",
     "ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
@@ -152,52 +161,56 @@
     "ListAssociatedStacksResultTypeDef",
     "ListEntitledApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "StackErrorTypeDef",
+    "StorageConnectorOutputTypeDef",
+    "StreamingExperienceSettingsOutputTypeDef",
+    "UserSettingOutputTypeDef",
     "StartAppBlockBuilderRequestRequestTypeDef",
     "StartFleetRequestRequestTypeDef",
     "StartImageBuilderRequestRequestTypeDef",
     "StopAppBlockBuilderRequestRequestTypeDef",
     "StopFleetRequestRequestTypeDef",
     "StopImageBuilderRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AssociateAppBlockBuilderAppBlockResultTypeDef",
     "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
     "AppBlockBuilderTypeDef",
-    "CreateAppBlockBuilderRequestRequestTypeDef",
-    "UpdateAppBlockBuilderRequestRequestTypeDef",
     "ApplicationTypeDef",
-    "CreateApplicationRequestRequestTypeDef",
-    "ScriptDetailsTypeDef",
-    "UpdateApplicationRequestRequestTypeDef",
+    "ScriptDetailsOutputTypeDef",
     "AssociateApplicationFleetResultTypeDef",
     "DescribeApplicationFleetAssociationsResultTypeDef",
     "BatchAssociateUserStackRequestRequestTypeDef",
     "BatchDisassociateUserStackRequestRequestTypeDef",
-    "DescribeUserStackAssociationsResultTypeDef",
-    "UserStackAssociationErrorTypeDef",
+    "CreateAppBlockBuilderRequestRequestTypeDef",
+    "UpdateAppBlockBuilderRequestRequestTypeDef",
+    "CreateApplicationRequestRequestTypeDef",
+    "ScriptDetailsTypeDef",
+    "UpdateApplicationRequestRequestTypeDef",
     "CreateDirectoryConfigRequestRequestTypeDef",
-    "DirectoryConfigTypeDef",
     "UpdateDirectoryConfigRequestRequestTypeDef",
     "CreateEntitlementRequestRequestTypeDef",
-    "EntitlementTypeDef",
     "UpdateEntitlementRequestRequestTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateImageBuilderRequestRequestTypeDef",
     "UpdateFleetRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "UpdateStackRequestRequestTypeDef",
     "DescribeFleetsRequestFleetStartedWaitTypeDef",
     "DescribeFleetsRequestFleetStoppedWaitTypeDef",
+    "DescribeUserStackAssociationsResultTypeDef",
+    "UserStackAssociationErrorTypeDef",
     "DescribeUsersResultTypeDef",
+    "DirectoryConfigTypeDef",
     "ListEntitledApplicationsResultTypeDef",
+    "EntitlementTypeDef",
     "FleetTypeDef",
     "ImageBuilderTypeDef",
     "SessionTypeDef",
     "SharedImagePermissionsTypeDef",
     "UpdateImagePermissionsRequestRequestTypeDef",
     "UsageReportSubscriptionTypeDef",
     "StackTypeDef",
@@ -237,14 +250,33 @@
     "CreateUpdatedImageResultTypeDef",
     "DeleteImageResultTypeDef",
     "DescribeImagesResultTypeDef",
     "CreateAppBlockResultTypeDef",
     "DescribeAppBlocksResultTypeDef",
 )
 
+_RequiredAccessEndpointOutputTypeDef = TypedDict(
+    "_RequiredAccessEndpointOutputTypeDef",
+    {
+        "EndpointType": Literal["STREAMING"],
+    },
+)
+_OptionalAccessEndpointOutputTypeDef = TypedDict(
+    "_OptionalAccessEndpointOutputTypeDef",
+    {
+        "VpceId": str,
+    },
+    total=False,
+)
+
+class AccessEndpointOutputTypeDef(
+    _RequiredAccessEndpointOutputTypeDef, _OptionalAccessEndpointOutputTypeDef
+):
+    pass
+
 _RequiredAccessEndpointTypeDef = TypedDict(
     "_RequiredAccessEndpointTypeDef",
     {
         "EndpointType": Literal["STREAMING"],
     },
 )
 _OptionalAccessEndpointTypeDef = TypedDict(
@@ -281,47 +313,47 @@
         "ErrorCode": FleetErrorCodeType,
         "ErrorMessage": str,
         "ErrorTimestamp": datetime,
     },
     total=False,
 )
 
-VpcConfigTypeDef = TypedDict(
-    "VpcConfigTypeDef",
+VpcConfigOutputTypeDef = TypedDict(
+    "VpcConfigOutputTypeDef",
     {
-        "SubnetIds": Sequence[str],
-        "SecurityGroupIds": Sequence[str],
+        "SubnetIds": List[str],
+        "SecurityGroupIds": List[str],
     },
     total=False,
 )
 
 ErrorDetailsTypeDef = TypedDict(
     "ErrorDetailsTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-_RequiredS3LocationTypeDef = TypedDict(
-    "_RequiredS3LocationTypeDef",
+_RequiredS3LocationOutputTypeDef = TypedDict(
+    "_RequiredS3LocationOutputTypeDef",
     {
         "S3Bucket": str,
     },
 )
-_OptionalS3LocationTypeDef = TypedDict(
-    "_OptionalS3LocationTypeDef",
+_OptionalS3LocationOutputTypeDef = TypedDict(
+    "_OptionalS3LocationOutputTypeDef",
     {
         "S3Key": str,
     },
     total=False,
 )
 
-class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
+class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
     pass
 
 ApplicationFleetAssociationTypeDef = TypedDict(
     "ApplicationFleetAssociationTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
@@ -407,14 +439,23 @@
 )
 
 class UserStackAssociationTypeDef(
     _RequiredUserStackAssociationTypeDef, _OptionalUserStackAssociationTypeDef
 ):
     pass
 
+CertificateBasedAuthPropertiesOutputTypeDef = TypedDict(
+    "CertificateBasedAuthPropertiesOutputTypeDef",
+    {
+        "Status": CertificateBasedAuthStatusType,
+        "CertificateAuthorityArn": str,
+    },
+    total=False,
+)
+
 CertificateBasedAuthPropertiesTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesTypeDef",
     {
         "Status": CertificateBasedAuthStatusType,
         "CertificateAuthorityArn": str,
     },
     total=False,
@@ -473,14 +514,23 @@
     "CopyImageResponseTypeDef",
     {
         "DestinationImageName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
+    {
+        "SubnetIds": Sequence[str],
+        "SecurityGroupIds": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
     {
         "AppBlockBuilderName": str,
     },
 )
 _OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
@@ -502,14 +552,31 @@
     {
         "StreamingURL": str,
         "Expires": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredS3LocationTypeDef = TypedDict(
+    "_RequiredS3LocationTypeDef",
+    {
+        "S3Bucket": str,
+    },
+)
+_OptionalS3LocationTypeDef = TypedDict(
+    "_OptionalS3LocationTypeDef",
+    {
+        "S3Key": str,
+    },
+    total=False,
+)
+
+class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
+    pass
+
 ServiceAccountCredentialsTypeDef = TypedDict(
     "ServiceAccountCredentialsTypeDef",
     {
         "AccountName": str,
         "AccountPassword": str,
     },
 )
@@ -1038,14 +1105,35 @@
         "AuthenticationType": AuthenticationTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredUserStackAssociationOutputTypeDef = TypedDict(
+    "_RequiredUserStackAssociationOutputTypeDef",
+    {
+        "StackName": str,
+        "UserName": str,
+        "AuthenticationType": AuthenticationTypeType,
+    },
+)
+_OptionalUserStackAssociationOutputTypeDef = TypedDict(
+    "_OptionalUserStackAssociationOutputTypeDef",
+    {
+        "SendEmailNotification": bool,
+    },
+    total=False,
+)
+
+class UserStackAssociationOutputTypeDef(
+    _RequiredUserStackAssociationOutputTypeDef, _OptionalUserStackAssociationOutputTypeDef
+):
+    pass
+
 _RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
     "_RequiredDescribeUsersRequestDescribeUsersPaginateTypeDef",
     {
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 _OptionalDescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
@@ -1101,14 +1189,22 @@
     },
     total=False,
 )
 
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
+ServiceAccountCredentialsOutputTypeDef = TypedDict(
+    "ServiceAccountCredentialsOutputTypeDef",
+    {
+        "AccountName": str,
+        "AccountPassword": str,
+    },
+)
+
 DisableUserRequestRequestTypeDef = TypedDict(
     "DisableUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
@@ -1142,14 +1238,23 @@
     "DisassociateFleetRequestRequestTypeDef",
     {
         "FleetName": str,
         "StackName": str,
     },
 )
 
+DomainJoinInfoOutputTypeDef = TypedDict(
+    "DomainJoinInfoOutputTypeDef",
+    {
+        "DirectoryName": str,
+        "OrganizationalUnitDistinguishedName": str,
+    },
+    total=False,
+)
+
 EnableUserRequestRequestTypeDef = TypedDict(
     "EnableUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
@@ -1157,14 +1262,22 @@
 EntitledApplicationTypeDef = TypedDict(
     "EntitledApplicationTypeDef",
     {
         "ApplicationIdentifier": str,
     },
 )
 
+EntitlementAttributeOutputTypeDef = TypedDict(
+    "EntitlementAttributeOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
 ExpireSessionRequestRequestTypeDef = TypedDict(
     "ExpireSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
@@ -1191,14 +1304,23 @@
     {
         "EniPrivateIpAddress": str,
         "EniId": str,
     },
     total=False,
 )
 
+ImagePermissionsOutputTypeDef = TypedDict(
+    "ImagePermissionsOutputTypeDef",
+    {
+        "allowFleet": bool,
+        "allowImageBuilder": bool,
+    },
+    total=False,
+)
+
 ImagePermissionsTypeDef = TypedDict(
     "ImagePermissionsTypeDef",
     {
         "allowFleet": bool,
         "allowImageBuilder": bool,
     },
     total=False,
@@ -1383,14 +1505,50 @@
     {
         "ErrorCode": StackErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+_RequiredStorageConnectorOutputTypeDef = TypedDict(
+    "_RequiredStorageConnectorOutputTypeDef",
+    {
+        "ConnectorType": StorageConnectorTypeType,
+    },
+)
+_OptionalStorageConnectorOutputTypeDef = TypedDict(
+    "_OptionalStorageConnectorOutputTypeDef",
+    {
+        "ResourceIdentifier": str,
+        "Domains": List[str],
+    },
+    total=False,
+)
+
+class StorageConnectorOutputTypeDef(
+    _RequiredStorageConnectorOutputTypeDef, _OptionalStorageConnectorOutputTypeDef
+):
+    pass
+
+StreamingExperienceSettingsOutputTypeDef = TypedDict(
+    "StreamingExperienceSettingsOutputTypeDef",
+    {
+        "PreferredProtocol": PreferredProtocolType,
+    },
+    total=False,
+)
+
+UserSettingOutputTypeDef = TypedDict(
+    "UserSettingOutputTypeDef",
+    {
+        "Action": ActionType,
+        "Permission": PermissionType,
+    },
+)
+
 StartAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "StartAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1477,36 +1635,110 @@
 _RequiredAppBlockBuilderTypeDef = TypedDict(
     "_RequiredAppBlockBuilderTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Platform": Literal["WINDOWS_SERVER_2019"],
         "InstanceType": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "State": AppBlockBuilderStateType,
     },
 )
 _OptionalAppBlockBuilderTypeDef = TypedDict(
     "_OptionalAppBlockBuilderTypeDef",
     {
         "DisplayName": str,
         "Description": str,
         "EnableDefaultInternetAccess": bool,
         "IamRoleArn": str,
         "CreatedTime": datetime,
         "AppBlockBuilderErrors": List[ResourceErrorTypeDef],
         "StateChangeReason": AppBlockBuilderStateChangeReasonTypeDef,
-        "AccessEndpoints": List[AccessEndpointTypeDef],
+        "AccessEndpoints": List[AccessEndpointOutputTypeDef],
     },
     total=False,
 )
 
 class AppBlockBuilderTypeDef(_RequiredAppBlockBuilderTypeDef, _OptionalAppBlockBuilderTypeDef):
     pass
 
+ApplicationTypeDef = TypedDict(
+    "ApplicationTypeDef",
+    {
+        "Name": str,
+        "DisplayName": str,
+        "IconURL": str,
+        "LaunchPath": str,
+        "LaunchParameters": str,
+        "Enabled": bool,
+        "Metadata": Dict[str, str],
+        "WorkingDirectory": str,
+        "Description": str,
+        "Arn": str,
+        "AppBlockArn": str,
+        "IconS3Location": S3LocationOutputTypeDef,
+        "Platforms": List[PlatformTypeType],
+        "InstanceFamilies": List[str],
+        "CreatedTime": datetime,
+    },
+    total=False,
+)
+
+_RequiredScriptDetailsOutputTypeDef = TypedDict(
+    "_RequiredScriptDetailsOutputTypeDef",
+    {
+        "ScriptS3Location": S3LocationOutputTypeDef,
+        "ExecutablePath": str,
+        "TimeoutInSeconds": int,
+    },
+)
+_OptionalScriptDetailsOutputTypeDef = TypedDict(
+    "_OptionalScriptDetailsOutputTypeDef",
+    {
+        "ExecutableParameters": str,
+    },
+    total=False,
+)
+
+class ScriptDetailsOutputTypeDef(
+    _RequiredScriptDetailsOutputTypeDef, _OptionalScriptDetailsOutputTypeDef
+):
+    pass
+
+AssociateApplicationFleetResultTypeDef = TypedDict(
+    "AssociateApplicationFleetResultTypeDef",
+    {
+        "ApplicationFleetAssociation": ApplicationFleetAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeApplicationFleetAssociationsResultTypeDef = TypedDict(
+    "DescribeApplicationFleetAssociationsResultTypeDef",
+    {
+        "ApplicationFleetAssociations": List[ApplicationFleetAssociationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchAssociateUserStackRequestRequestTypeDef = TypedDict(
+    "BatchAssociateUserStackRequestRequestTypeDef",
+    {
+        "UserStackAssociations": Sequence[UserStackAssociationTypeDef],
+    },
+)
+
+BatchDisassociateUserStackRequestRequestTypeDef = TypedDict(
+    "BatchDisassociateUserStackRequestRequestTypeDef",
+    {
+        "UserStackAssociations": Sequence[UserStackAssociationTypeDef],
+    },
+)
+
 _RequiredCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
         "Platform": Literal["WINDOWS_SERVER_2019"],
         "InstanceType": str,
         "VpcConfig": VpcConfigTypeDef,
@@ -1555,36 +1787,14 @@
 
 class UpdateAppBlockBuilderRequestRequestTypeDef(
     _RequiredUpdateAppBlockBuilderRequestRequestTypeDef,
     _OptionalUpdateAppBlockBuilderRequestRequestTypeDef,
 ):
     pass
 
-ApplicationTypeDef = TypedDict(
-    "ApplicationTypeDef",
-    {
-        "Name": str,
-        "DisplayName": str,
-        "IconURL": str,
-        "LaunchPath": str,
-        "LaunchParameters": str,
-        "Enabled": bool,
-        "Metadata": Dict[str, str],
-        "WorkingDirectory": str,
-        "Description": str,
-        "Arn": str,
-        "AppBlockArn": str,
-        "IconS3Location": S3LocationTypeDef,
-        "Platforms": List[PlatformTypeType],
-        "InstanceFamilies": List[str],
-        "CreatedTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "Name": str,
         "IconS3Location": S3LocationTypeDef,
         "LaunchPath": str,
         "Platforms": Sequence[PlatformTypeType],
@@ -1650,64 +1860,14 @@
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-AssociateApplicationFleetResultTypeDef = TypedDict(
-    "AssociateApplicationFleetResultTypeDef",
-    {
-        "ApplicationFleetAssociation": ApplicationFleetAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeApplicationFleetAssociationsResultTypeDef = TypedDict(
-    "DescribeApplicationFleetAssociationsResultTypeDef",
-    {
-        "ApplicationFleetAssociations": List[ApplicationFleetAssociationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchAssociateUserStackRequestRequestTypeDef = TypedDict(
-    "BatchAssociateUserStackRequestRequestTypeDef",
-    {
-        "UserStackAssociations": Sequence[UserStackAssociationTypeDef],
-    },
-)
-
-BatchDisassociateUserStackRequestRequestTypeDef = TypedDict(
-    "BatchDisassociateUserStackRequestRequestTypeDef",
-    {
-        "UserStackAssociations": Sequence[UserStackAssociationTypeDef],
-    },
-)
-
-DescribeUserStackAssociationsResultTypeDef = TypedDict(
-    "DescribeUserStackAssociationsResultTypeDef",
-    {
-        "UserStackAssociations": List[UserStackAssociationTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UserStackAssociationErrorTypeDef = TypedDict(
-    "UserStackAssociationErrorTypeDef",
-    {
-        "UserStackAssociation": UserStackAssociationTypeDef,
-        "ErrorCode": UserStackAssociationErrorCodeType,
-        "ErrorMessage": str,
-    },
-    total=False,
-)
-
 _RequiredCreateDirectoryConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDirectoryConfigRequestRequestTypeDef",
     {
         "DirectoryName": str,
         "OrganizationalUnitDistinguishedNames": Sequence[str],
     },
 )
@@ -1722,34 +1882,14 @@
 
 class CreateDirectoryConfigRequestRequestTypeDef(
     _RequiredCreateDirectoryConfigRequestRequestTypeDef,
     _OptionalCreateDirectoryConfigRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDirectoryConfigTypeDef = TypedDict(
-    "_RequiredDirectoryConfigTypeDef",
-    {
-        "DirectoryName": str,
-    },
-)
-_OptionalDirectoryConfigTypeDef = TypedDict(
-    "_OptionalDirectoryConfigTypeDef",
-    {
-        "OrganizationalUnitDistinguishedNames": List[str],
-        "ServiceAccountCredentials": ServiceAccountCredentialsTypeDef,
-        "CreatedTime": datetime,
-        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
-    },
-    total=False,
-)
-
-class DirectoryConfigTypeDef(_RequiredDirectoryConfigTypeDef, _OptionalDirectoryConfigTypeDef):
-    pass
-
 _RequiredUpdateDirectoryConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDirectoryConfigRequestRequestTypeDef",
     {
         "DirectoryName": str,
     },
 )
 _OptionalUpdateDirectoryConfigRequestRequestTypeDef = TypedDict(
@@ -1786,36 +1926,14 @@
 )
 
 class CreateEntitlementRequestRequestTypeDef(
     _RequiredCreateEntitlementRequestRequestTypeDef, _OptionalCreateEntitlementRequestRequestTypeDef
 ):
     pass
 
-_RequiredEntitlementTypeDef = TypedDict(
-    "_RequiredEntitlementTypeDef",
-    {
-        "Name": str,
-        "StackName": str,
-        "AppVisibility": AppVisibilityType,
-        "Attributes": List[EntitlementAttributeTypeDef],
-    },
-)
-_OptionalEntitlementTypeDef = TypedDict(
-    "_OptionalEntitlementTypeDef",
-    {
-        "Description": str,
-        "CreatedTime": datetime,
-        "LastModifiedTime": datetime,
-    },
-    total=False,
-)
-
-class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
-    pass
-
 _RequiredUpdateEntitlementRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEntitlementRequestRequestTypeDef",
     {
         "Name": str,
         "StackName": str,
     },
 )
@@ -2006,32 +2124,93 @@
         "Names": Sequence[str],
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+DescribeUserStackAssociationsResultTypeDef = TypedDict(
+    "DescribeUserStackAssociationsResultTypeDef",
+    {
+        "UserStackAssociations": List[UserStackAssociationOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UserStackAssociationErrorTypeDef = TypedDict(
+    "UserStackAssociationErrorTypeDef",
+    {
+        "UserStackAssociation": UserStackAssociationOutputTypeDef,
+        "ErrorCode": UserStackAssociationErrorCodeType,
+        "ErrorMessage": str,
+    },
+    total=False,
+)
+
 DescribeUsersResultTypeDef = TypedDict(
     "DescribeUsersResultTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDirectoryConfigTypeDef = TypedDict(
+    "_RequiredDirectoryConfigTypeDef",
+    {
+        "DirectoryName": str,
+    },
+)
+_OptionalDirectoryConfigTypeDef = TypedDict(
+    "_OptionalDirectoryConfigTypeDef",
+    {
+        "OrganizationalUnitDistinguishedNames": List[str],
+        "ServiceAccountCredentials": ServiceAccountCredentialsOutputTypeDef,
+        "CreatedTime": datetime,
+        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
+class DirectoryConfigTypeDef(_RequiredDirectoryConfigTypeDef, _OptionalDirectoryConfigTypeDef):
+    pass
+
 ListEntitledApplicationsResultTypeDef = TypedDict(
     "ListEntitledApplicationsResultTypeDef",
     {
         "EntitledApplications": List[EntitledApplicationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredEntitlementTypeDef = TypedDict(
+    "_RequiredEntitlementTypeDef",
+    {
+        "Name": str,
+        "StackName": str,
+        "AppVisibility": AppVisibilityType,
+        "Attributes": List[EntitlementAttributeOutputTypeDef],
+    },
+)
+_OptionalEntitlementTypeDef = TypedDict(
+    "_OptionalEntitlementTypeDef",
+    {
+        "Description": str,
+        "CreatedTime": datetime,
+        "LastModifiedTime": datetime,
+    },
+    total=False,
+)
+
+class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
+    pass
+
 _RequiredFleetTypeDef = TypedDict(
     "_RequiredFleetTypeDef",
     {
         "Arn": str,
         "Name": str,
         "InstanceType": str,
         "ComputeCapacityStatus": ComputeCapacityStatusTypeDef,
@@ -2044,26 +2223,26 @@
         "DisplayName": str,
         "Description": str,
         "ImageName": str,
         "ImageArn": str,
         "FleetType": FleetTypeType,
         "MaxUserDurationInSeconds": int,
         "DisconnectTimeoutInSeconds": int,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "CreatedTime": datetime,
         "FleetErrors": List[FleetErrorTypeDef],
         "EnableDefaultInternetAccess": bool,
-        "DomainJoinInfo": DomainJoinInfoTypeDef,
+        "DomainJoinInfo": DomainJoinInfoOutputTypeDef,
         "IdleDisconnectTimeoutInSeconds": int,
         "IamRoleArn": str,
         "StreamView": StreamViewType,
         "Platform": PlatformTypeType,
         "MaxConcurrentSessions": int,
         "UsbDeviceFilterStrings": List[str],
-        "SessionScriptS3Location": S3LocationTypeDef,
+        "SessionScriptS3Location": S3LocationOutputTypeDef,
     },
     total=False,
 )
 
 class FleetTypeDef(_RequiredFleetTypeDef, _OptionalFleetTypeDef):
     pass
 
@@ -2076,27 +2255,27 @@
 _OptionalImageBuilderTypeDef = TypedDict(
     "_OptionalImageBuilderTypeDef",
     {
         "Arn": str,
         "ImageArn": str,
         "Description": str,
         "DisplayName": str,
-        "VpcConfig": VpcConfigTypeDef,
+        "VpcConfig": VpcConfigOutputTypeDef,
         "InstanceType": str,
         "Platform": PlatformTypeType,
         "IamRoleArn": str,
         "State": ImageBuilderStateType,
         "StateChangeReason": ImageBuilderStateChangeReasonTypeDef,
         "CreatedTime": datetime,
         "EnableDefaultInternetAccess": bool,
-        "DomainJoinInfo": DomainJoinInfoTypeDef,
+        "DomainJoinInfo": DomainJoinInfoOutputTypeDef,
         "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
         "ImageBuilderErrors": List[ResourceErrorTypeDef],
         "AppstreamAgentVersion": str,
-        "AccessEndpoints": List[AccessEndpointTypeDef],
+        "AccessEndpoints": List[AccessEndpointOutputTypeDef],
     },
     total=False,
 )
 
 class ImageBuilderTypeDef(_RequiredImageBuilderTypeDef, _OptionalImageBuilderTypeDef):
     pass
 
@@ -2125,15 +2304,15 @@
 class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
     pass
 
 SharedImagePermissionsTypeDef = TypedDict(
     "SharedImagePermissionsTypeDef",
     {
         "sharedAccountId": str,
-        "imagePermissions": ImagePermissionsTypeDef,
+        "imagePermissions": ImagePermissionsOutputTypeDef,
     },
 )
 
 UpdateImagePermissionsRequestRequestTypeDef = TypedDict(
     "UpdateImagePermissionsRequestRequestTypeDef",
     {
         "Name": str,
@@ -2162,23 +2341,23 @@
 _OptionalStackTypeDef = TypedDict(
     "_OptionalStackTypeDef",
     {
         "Arn": str,
         "Description": str,
         "DisplayName": str,
         "CreatedTime": datetime,
-        "StorageConnectors": List[StorageConnectorTypeDef],
+        "StorageConnectors": List[StorageConnectorOutputTypeDef],
         "RedirectURL": str,
         "FeedbackURL": str,
         "StackErrors": List[StackErrorTypeDef],
-        "UserSettings": List[UserSettingTypeDef],
+        "UserSettings": List[UserSettingOutputTypeDef],
         "ApplicationSettings": ApplicationSettingsResponseTypeDef,
-        "AccessEndpoints": List[AccessEndpointTypeDef],
+        "AccessEndpoints": List[AccessEndpointOutputTypeDef],
         "EmbedHostDomains": List[str],
-        "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
+        "StreamingExperienceSettings": StreamingExperienceSettingsOutputTypeDef,
     },
     total=False,
 )
 
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
 
@@ -2259,15 +2438,15 @@
         "Platform": PlatformTypeType,
         "Description": str,
         "StateChangeReason": ImageStateChangeReasonTypeDef,
         "Applications": List[ApplicationTypeDef],
         "CreatedTime": datetime,
         "PublicBaseImageReleasedDate": datetime,
         "AppstreamAgentVersion": str,
-        "ImagePermissions": ImagePermissionsTypeDef,
+        "ImagePermissions": ImagePermissionsOutputTypeDef,
         "ImageErrors": List[ResourceErrorTypeDef],
     },
     total=False,
 )
 
 class ImageTypeDef(_RequiredImageTypeDef, _OptionalImageTypeDef):
     pass
@@ -2288,18 +2467,18 @@
     },
 )
 _OptionalAppBlockTypeDef = TypedDict(
     "_OptionalAppBlockTypeDef",
     {
         "Description": str,
         "DisplayName": str,
-        "SourceS3Location": S3LocationTypeDef,
-        "SetupScriptDetails": ScriptDetailsTypeDef,
+        "SourceS3Location": S3LocationOutputTypeDef,
+        "SetupScriptDetails": ScriptDetailsOutputTypeDef,
         "CreatedTime": datetime,
-        "PostSetupScriptDetails": ScriptDetailsTypeDef,
+        "PostSetupScriptDetails": ScriptDetailsOutputTypeDef,
         "PackagingType": PackagingTypeType,
         "State": AppBlockStateType,
         "AppBlockErrors": List[ErrorDetailsTypeDef],
     },
     total=False,
 )
```

### Comparing `mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/waiter.py` & `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.0/mypy_boto3_appstream/waiter.pyi` & `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.0/mypy_boto3_appstream.egg-info/PKG-INFO` & `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appstream
-Version: 1.28.0
-Summary: Type annotations for boto3.AppStream 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AppStream 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-appstream"></a>
 
 # mypy-boto3-appstream
 
 [![PyPI - mypy-boto3-appstream](https://img.shields.io/pypi/v/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appstream?color=blue)](https://pypistats.org/packages/mypy-boto3-appstream)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appstream)](https://pepy.tech/project/mypy-boto3-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppStream 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[boto3.AppStream 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
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
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -415,36 +415,40 @@
 ### Typed dictionaries
 
 `mypy_boto3_appstream.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appstream.type_defs import (
+    AccessEndpointOutputTypeDef,
     AccessEndpointTypeDef,
     AppBlockBuilderAppBlockAssociationTypeDef,
     AppBlockBuilderStateChangeReasonTypeDef,
     ResourceErrorTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigOutputTypeDef,
     ErrorDetailsTypeDef,
-    S3LocationTypeDef,
+    S3LocationOutputTypeDef,
     ApplicationFleetAssociationTypeDef,
     ApplicationSettingsResponseTypeDef,
     ApplicationSettingsTypeDef,
     AssociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     AssociateApplicationFleetRequestRequestTypeDef,
     AssociateApplicationToEntitlementRequestRequestTypeDef,
     AssociateFleetRequestRequestTypeDef,
     UserStackAssociationTypeDef,
+    CertificateBasedAuthPropertiesOutputTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityStatusTypeDef,
     ComputeCapacityTypeDef,
     CopyImageRequestRequestTypeDef,
     CopyImageResponseTypeDef,
+    VpcConfigTypeDef,
     CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
     CreateAppBlockBuilderStreamingURLResultTypeDef,
+    S3LocationTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
     CreateImageBuilderStreamingURLResultTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
@@ -484,28 +488,33 @@
     DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeSessionsRequestRequestTypeDef,
     DescribeStacksRequestDescribeStacksPaginateTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeUsageReportSubscriptionsRequestRequestTypeDef,
     DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
     DescribeUserStackAssociationsRequestRequestTypeDef,
+    UserStackAssociationOutputTypeDef,
     DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UserTypeDef,
+    ServiceAccountCredentialsOutputTypeDef,
     DisableUserRequestRequestTypeDef,
     DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef,
     DisassociateApplicationFleetRequestRequestTypeDef,
     DisassociateApplicationFromEntitlementRequestRequestTypeDef,
     DisassociateFleetRequestRequestTypeDef,
+    DomainJoinInfoOutputTypeDef,
     EnableUserRequestRequestTypeDef,
     EntitledApplicationTypeDef,
+    EntitlementAttributeOutputTypeDef,
     ExpireSessionRequestRequestTypeDef,
     FleetErrorTypeDef,
     ImageBuilderStateChangeReasonTypeDef,
     NetworkAccessConfigurationTypeDef,
+    ImagePermissionsOutputTypeDef,
     ImagePermissionsTypeDef,
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
     ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
     ListAssociatedFleetsResultTypeDef,
     ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef,
@@ -513,52 +522,56 @@
     ListAssociatedStacksResultTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     StackErrorTypeDef,
+    StorageConnectorOutputTypeDef,
+    StreamingExperienceSettingsOutputTypeDef,
+    UserSettingOutputTypeDef,
     StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
     StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AssociateAppBlockBuilderAppBlockResultTypeDef,
     DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
     AppBlockBuilderTypeDef,
-    CreateAppBlockBuilderRequestRequestTypeDef,
-    UpdateAppBlockBuilderRequestRequestTypeDef,
     ApplicationTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    ScriptDetailsTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
+    ScriptDetailsOutputTypeDef,
     AssociateApplicationFleetResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
     BatchAssociateUserStackRequestRequestTypeDef,
     BatchDisassociateUserStackRequestRequestTypeDef,
-    DescribeUserStackAssociationsResultTypeDef,
-    UserStackAssociationErrorTypeDef,
+    CreateAppBlockBuilderRequestRequestTypeDef,
+    UpdateAppBlockBuilderRequestRequestTypeDef,
+    CreateApplicationRequestRequestTypeDef,
+    ScriptDetailsTypeDef,
+    UpdateApplicationRequestRequestTypeDef,
     CreateDirectoryConfigRequestRequestTypeDef,
-    DirectoryConfigTypeDef,
     UpdateDirectoryConfigRequestRequestTypeDef,
     CreateEntitlementRequestRequestTypeDef,
-    EntitlementTypeDef,
     UpdateEntitlementRequestRequestTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateImageBuilderRequestRequestTypeDef,
     UpdateFleetRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     UpdateStackRequestRequestTypeDef,
     DescribeFleetsRequestFleetStartedWaitTypeDef,
     DescribeFleetsRequestFleetStoppedWaitTypeDef,
+    DescribeUserStackAssociationsResultTypeDef,
+    UserStackAssociationErrorTypeDef,
     DescribeUsersResultTypeDef,
+    DirectoryConfigTypeDef,
     ListEntitledApplicationsResultTypeDef,
+    EntitlementTypeDef,
     FleetTypeDef,
     ImageBuilderTypeDef,
     SessionTypeDef,
     SharedImagePermissionsTypeDef,
     UpdateImagePermissionsRequestRequestTypeDef,
     UsageReportSubscriptionTypeDef,
     StackTypeDef,
@@ -599,15 +612,15 @@
     DeleteImageResultTypeDef,
     DescribeImagesResultTypeDef,
     CreateAppBlockResultTypeDef,
     DescribeAppBlocksResultTypeDef,
 )
 
 
-def get_structure() -> AccessEndpointTypeDef:
+def get_structure() -> AccessEndpointOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appstream-1.28.0/mypy_boto3_appstream.egg-info/SOURCES.txt` & `mypy-boto3-appstream-1.28.12/mypy_boto3_appstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.0/setup.py` & `mypy-boto3-appstream-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appstream",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_appstream"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppStream 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.AppStream 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

