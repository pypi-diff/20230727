# Comparing `tmp/mypy-boto3-eks-1.28.0.tar.gz` & `tmp/mypy-boto3-eks-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-eks-1.28.0.tar", last modified: Thu Jul  6 20:59:30 2023, max compression
+gzip compressed data, was "mypy-boto3-eks-1.28.12.tar", last modified: Thu Jul 27 05:34:38 2023, max compression
```

## Comparing `mypy-boto3-eks-1.28.0.tar` & `mypy-boto3-eks-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:30.158292 mypy-boto3-eks-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:04.000000 mypy-boto3-eks-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-07-06 20:59:30.158292 mypy-boto3-eks-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-07-06 20:40:04.000000 mypy-boto3-eks-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:30.150292 mypy-boto3-eks-1.28.0/mypy_boto3_eks/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-06 20:40:04.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-06 20:40:04.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:40:04.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33061 2023-07-06 20:40:05.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33004 2023-07-06 20:40:05.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-07-06 20:40:05.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-07-06 20:40:05.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-07-06 20:40:05.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-06 20:40:05.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:04.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50680 2023-07-06 20:40:08.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50607 2023-07-06 20:40:08.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:04.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-06 20:40:05.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-06 20:40:05.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:30.158292 mypy-boto3-eks-1.28.0/mypy_boto3_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-07-06 20:59:29.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-06 20:59:29.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:29.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:29.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:29.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:29.000000 mypy-boto3-eks-1.28.0/mypy_boto3_eks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:30.158292 mypy-boto3-eks-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:40:04.000000 mypy-boto3-eks-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.088522 mypy-boto3-eks-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-07-27 05:34:38.088522 mypy-boto3-eks-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.084522 mypy-boto3-eks-1.28.12/mypy_boto3_eks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33061 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33004 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-07-27 05:21:40.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14286 2023-07-27 05:21:40.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53041 2023-07-27 05:21:41.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52968 2023-07-27 05:21:40.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-27 05:21:40.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-27 05:21:40.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.088522 mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-07-27 05:34:37.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 05:34:37.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:37.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:37.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:38.088522 mypy-boto3-eks-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/setup.py
```

### Comparing `mypy-boto3-eks-1.28.0/LICENSE` & `mypy-boto3-eks-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.0/PKG-INFO` & `mypy-boto3-eks-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-eks
-Version: 1.28.0
-Summary: Type annotations for boto3.EKS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.EKS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-eks"></a>
 
 # mypy-boto3-eks
 
 [![PyPI - mypy-boto3-eks](https://img.shields.io/pypi/v/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-eks?color=blue)](https://pypistats.org/packages/mypy-boto3-eks)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-eks)](https://pepy.tech/project/mypy-boto3-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EKS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[boto3.EKS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
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
 [mypy-boto3-eks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -449,19 +449,23 @@
     DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
     DescribeAddonVersionsRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
+    ProviderOutputTypeDef,
     ProviderTypeDef,
     ErrorDetailTypeDef,
+    FargateProfileSelectorOutputTypeDef,
+    IdentityProviderConfigOutputTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
+    LaunchTemplateSpecificationOutputTypeDef,
     ListAddonsRequestListAddonsPaginateTypeDef,
     ListAddonsRequestRequestTypeDef,
     ListAddonsResponseTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
     ListClustersResponseTypeDef,
     ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
@@ -473,15 +477,20 @@
     ListNodegroupsRequestRequestTypeDef,
     ListNodegroupsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUpdatesRequestListUpdatesPaginateTypeDef,
     ListUpdatesRequestRequestTypeDef,
     ListUpdatesResponseTypeDef,
+    LogSetupOutputTypeDef,
     LogSetupTypeDef,
+    NodegroupScalingConfigOutputTypeDef,
+    NodegroupUpdateConfigOutputTypeDef,
+    RemoteAccessConfigOutputTypeDef,
+    TaintOutputTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddonRequestRequestTypeDef,
     UpdateClusterVersionRequestRequestTypeDef,
     UpdateLabelsPayloadTypeDef,
@@ -491,42 +500,44 @@
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
     CreateFargateProfileRequestRequestTypeDef,
-    FargateProfileTypeDef,
     UpdateNodegroupVersionRequestRequestTypeDef,
     CreateNodegroupRequestRequestTypeDef,
     UpdateTaintsPayloadTypeDef,
     DescribeAddonRequestAddonActiveWaitTypeDef,
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
     DescribeNodegroupRequestNodegroupActiveWaitTypeDef,
     DescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
-    ListIdentityProviderConfigsResponseTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
+    FargateProfileTypeDef,
+    ListIdentityProviderConfigsResponseTypeDef,
     IdentityProviderConfigResponseTypeDef,
     IdentityTypeDef,
     NodegroupHealthTypeDef,
+    LoggingOutputTypeDef,
     LoggingTypeDef,
     UpdateTypeDef,
     AddonTypeDef,
     AddonInfoTypeDef,
+    UpdateNodegroupConfigRequestRequestTypeDef,
+    AssociateEncryptionConfigRequestRequestTypeDef,
     CreateFargateProfileResponseTypeDef,
     DeleteFargateProfileResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
-    UpdateNodegroupConfigRequestRequestTypeDef,
-    AssociateEncryptionConfigRequestRequestTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     NodegroupTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterConfigRequestRequestTypeDef,
     AssociateEncryptionConfigResponseTypeDef,
     AssociateIdentityProviderConfigResponseTypeDef,
```

### Comparing `mypy-boto3-eks-1.28.0/README.md` & `mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-eks
+Version: 1.28.12
+Summary: Type annotations for boto3.EKS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 eks type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-eks"></a>
 
 # mypy-boto3-eks
 
 [![PyPI - mypy-boto3-eks](https://img.shields.io/pypi/v/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-eks?color=blue)](https://pypistats.org/packages/mypy-boto3-eks)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-eks)](https://pepy.tech/project/mypy-boto3-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EKS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[boto3.EKS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
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
 [mypy-boto3-eks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -417,19 +449,23 @@
     DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
     DescribeAddonVersionsRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
+    ProviderOutputTypeDef,
     ProviderTypeDef,
     ErrorDetailTypeDef,
+    FargateProfileSelectorOutputTypeDef,
+    IdentityProviderConfigOutputTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
+    LaunchTemplateSpecificationOutputTypeDef,
     ListAddonsRequestListAddonsPaginateTypeDef,
     ListAddonsRequestRequestTypeDef,
     ListAddonsResponseTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
     ListClustersResponseTypeDef,
     ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
@@ -441,15 +477,20 @@
     ListNodegroupsRequestRequestTypeDef,
     ListNodegroupsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUpdatesRequestListUpdatesPaginateTypeDef,
     ListUpdatesRequestRequestTypeDef,
     ListUpdatesResponseTypeDef,
+    LogSetupOutputTypeDef,
     LogSetupTypeDef,
+    NodegroupScalingConfigOutputTypeDef,
+    NodegroupUpdateConfigOutputTypeDef,
+    RemoteAccessConfigOutputTypeDef,
+    TaintOutputTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddonRequestRequestTypeDef,
     UpdateClusterVersionRequestRequestTypeDef,
     UpdateLabelsPayloadTypeDef,
@@ -459,42 +500,44 @@
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
     CreateFargateProfileRequestRequestTypeDef,
-    FargateProfileTypeDef,
     UpdateNodegroupVersionRequestRequestTypeDef,
     CreateNodegroupRequestRequestTypeDef,
     UpdateTaintsPayloadTypeDef,
     DescribeAddonRequestAddonActiveWaitTypeDef,
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
     DescribeNodegroupRequestNodegroupActiveWaitTypeDef,
     DescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
-    ListIdentityProviderConfigsResponseTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
+    FargateProfileTypeDef,
+    ListIdentityProviderConfigsResponseTypeDef,
     IdentityProviderConfigResponseTypeDef,
     IdentityTypeDef,
     NodegroupHealthTypeDef,
+    LoggingOutputTypeDef,
     LoggingTypeDef,
     UpdateTypeDef,
     AddonTypeDef,
     AddonInfoTypeDef,
+    UpdateNodegroupConfigRequestRequestTypeDef,
+    AssociateEncryptionConfigRequestRequestTypeDef,
     CreateFargateProfileResponseTypeDef,
     DeleteFargateProfileResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
-    UpdateNodegroupConfigRequestRequestTypeDef,
-    AssociateEncryptionConfigRequestRequestTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     NodegroupTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterConfigRequestRequestTypeDef,
     AssociateEncryptionConfigResponseTypeDef,
     AssociateIdentityProviderConfigResponseTypeDef,
```

### Comparing `mypy-boto3-eks-1.28.0/mypy_boto3_eks/__init__.py` & `mypy-boto3-eks-1.28.12/mypy_boto3_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.0/mypy_boto3_eks/__init__.pyi` & `mypy-boto3-eks-1.28.12/mypy_boto3_eks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.0/mypy_boto3_eks/__main__.py` & `mypy-boto3-eks-1.28.12/mypy_boto3_eks/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EKS 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.EKS 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS\nOther"
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

### Comparing `mypy-boto3-eks-1.28.0/mypy_boto3_eks/client.py` & `mypy-boto3-eks-1.28.12/mypy_boto3_eks/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.0/mypy_boto3_eks/client.pyi` & `mypy-boto3-eks-1.28.12/mypy_boto3_eks/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.0/mypy_boto3_eks/literals.py` & `mypy-boto3-eks-1.28.12/mypy_boto3_eks/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,14 +328,15 @@
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
@@ -414,26 +415,28 @@
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

### Comparing `mypy-boto3-eks-1.28.0/mypy_boto3_eks/literals.pyi` & `mypy-boto3-eks-1.28.12/mypy_boto3_eks/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -326,14 +326,15 @@
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
@@ -412,26 +413,28 @@
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

### Comparing `mypy-boto3-eks-1.28.0/mypy_boto3_eks/paginator.py` & `mypy-boto3-eks-1.28.12/mypy_boto3_eks/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.0/mypy_boto3_eks/paginator.pyi` & `mypy-boto3-eks-1.28.12/mypy_boto3_eks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.0/mypy_boto3_eks/type_defs.py` & `mypy-boto3-eks-1.28.12/mypy_boto3_eks/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,19 +78,23 @@
     "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
     "DescribeAddonVersionsRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeFargateProfileRequestRequestTypeDef",
     "IdentityProviderConfigTypeDef",
     "DescribeNodegroupRequestRequestTypeDef",
     "DescribeUpdateRequestRequestTypeDef",
+    "ProviderOutputTypeDef",
     "ProviderTypeDef",
     "ErrorDetailTypeDef",
+    "FargateProfileSelectorOutputTypeDef",
+    "IdentityProviderConfigOutputTypeDef",
     "OidcIdentityProviderConfigTypeDef",
     "OIDCTypeDef",
     "IssueTypeDef",
+    "LaunchTemplateSpecificationOutputTypeDef",
     "ListAddonsRequestListAddonsPaginateTypeDef",
     "ListAddonsRequestRequestTypeDef",
     "ListAddonsResponseTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListClustersResponseTypeDef",
     "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
@@ -102,15 +106,20 @@
     "ListNodegroupsRequestRequestTypeDef",
     "ListNodegroupsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "ListUpdatesRequestRequestTypeDef",
     "ListUpdatesResponseTypeDef",
+    "LogSetupOutputTypeDef",
     "LogSetupTypeDef",
+    "NodegroupScalingConfigOutputTypeDef",
+    "NodegroupUpdateConfigOutputTypeDef",
+    "RemoteAccessConfigOutputTypeDef",
+    "TaintOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddonRequestRequestTypeDef",
     "UpdateClusterVersionRequestRequestTypeDef",
     "UpdateLabelsPayloadTypeDef",
@@ -120,42 +129,44 @@
     "AssociateIdentityProviderConfigRequestRequestTypeDef",
     "NodegroupResourcesTypeDef",
     "ClusterHealthTypeDef",
     "RegisterClusterRequestRequestTypeDef",
     "OutpostConfigRequestTypeDef",
     "OutpostConfigResponseTypeDef",
     "CreateFargateProfileRequestRequestTypeDef",
-    "FargateProfileTypeDef",
     "UpdateNodegroupVersionRequestRequestTypeDef",
     "CreateNodegroupRequestRequestTypeDef",
     "UpdateTaintsPayloadTypeDef",
     "DescribeAddonRequestAddonActiveWaitTypeDef",
     "DescribeAddonRequestAddonDeletedWaitTypeDef",
     "DescribeClusterRequestClusterActiveWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef",
     "DescribeNodegroupRequestNodegroupActiveWaitTypeDef",
     "DescribeNodegroupRequestNodegroupDeletedWaitTypeDef",
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     "DisassociateIdentityProviderConfigRequestRequestTypeDef",
-    "ListIdentityProviderConfigsResponseTypeDef",
+    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
+    "FargateProfileTypeDef",
+    "ListIdentityProviderConfigsResponseTypeDef",
     "IdentityProviderConfigResponseTypeDef",
     "IdentityTypeDef",
     "NodegroupHealthTypeDef",
+    "LoggingOutputTypeDef",
     "LoggingTypeDef",
     "UpdateTypeDef",
     "AddonTypeDef",
     "AddonInfoTypeDef",
+    "UpdateNodegroupConfigRequestRequestTypeDef",
+    "AssociateEncryptionConfigRequestRequestTypeDef",
     "CreateFargateProfileResponseTypeDef",
     "DeleteFargateProfileResponseTypeDef",
     "DescribeFargateProfileResponseTypeDef",
-    "UpdateNodegroupConfigRequestRequestTypeDef",
-    "AssociateEncryptionConfigRequestRequestTypeDef",
     "DescribeIdentityProviderConfigResponseTypeDef",
     "NodegroupTypeDef",
     "ClusterTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterConfigRequestRequestTypeDef",
     "AssociateEncryptionConfigResponseTypeDef",
     "AssociateIdentityProviderConfigResponseTypeDef",
@@ -592,14 +603,22 @@
 
 class DescribeUpdateRequestRequestTypeDef(
     _RequiredDescribeUpdateRequestRequestTypeDef, _OptionalDescribeUpdateRequestRequestTypeDef
 ):
     pass
 
 
+ProviderOutputTypeDef = TypedDict(
+    "ProviderOutputTypeDef",
+    {
+        "keyArn": str,
+    },
+    total=False,
+)
+
 ProviderTypeDef = TypedDict(
     "ProviderTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
@@ -610,14 +629,31 @@
         "errorCode": ErrorCodeType,
         "errorMessage": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
+FargateProfileSelectorOutputTypeDef = TypedDict(
+    "FargateProfileSelectorOutputTypeDef",
+    {
+        "namespace": str,
+        "labels": Dict[str, str],
+    },
+    total=False,
+)
+
+IdentityProviderConfigOutputTypeDef = TypedDict(
+    "IdentityProviderConfigOutputTypeDef",
+    {
+        "type": str,
+        "name": str,
+    },
+)
+
 OidcIdentityProviderConfigTypeDef = TypedDict(
     "OidcIdentityProviderConfigTypeDef",
     {
         "identityProviderConfigName": str,
         "identityProviderConfigArn": str,
         "clusterName": str,
         "issuerUrl": str,
@@ -647,14 +683,24 @@
         "code": NodegroupIssueCodeType,
         "message": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
+LaunchTemplateSpecificationOutputTypeDef = TypedDict(
+    "LaunchTemplateSpecificationOutputTypeDef",
+    {
+        "name": str,
+        "version": str,
+        "id": str,
+    },
+    total=False,
+)
+
 _RequiredListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
     "_RequiredListAddonsRequestListAddonsPaginateTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
@@ -952,23 +998,70 @@
     {
         "updateIds": List[str],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LogSetupOutputTypeDef = TypedDict(
+    "LogSetupOutputTypeDef",
+    {
+        "types": List[LogTypeType],
+        "enabled": bool,
+    },
+    total=False,
+)
+
 LogSetupTypeDef = TypedDict(
     "LogSetupTypeDef",
     {
         "types": Sequence[LogTypeType],
         "enabled": bool,
     },
     total=False,
 )
 
+NodegroupScalingConfigOutputTypeDef = TypedDict(
+    "NodegroupScalingConfigOutputTypeDef",
+    {
+        "minSize": int,
+        "maxSize": int,
+        "desiredSize": int,
+    },
+    total=False,
+)
+
+NodegroupUpdateConfigOutputTypeDef = TypedDict(
+    "NodegroupUpdateConfigOutputTypeDef",
+    {
+        "maxUnavailable": int,
+        "maxUnavailablePercentage": int,
+    },
+    total=False,
+)
+
+RemoteAccessConfigOutputTypeDef = TypedDict(
+    "RemoteAccessConfigOutputTypeDef",
+    {
+        "ec2SshKey": str,
+        "sourceSecurityGroups": List[str],
+    },
+    total=False,
+)
+
+TaintOutputTypeDef = TypedDict(
+    "TaintOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+        "effect": TaintEffectType,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1219,30 +1312,14 @@
 class CreateFargateProfileRequestRequestTypeDef(
     _RequiredCreateFargateProfileRequestRequestTypeDef,
     _OptionalCreateFargateProfileRequestRequestTypeDef,
 ):
     pass
 
 
-FargateProfileTypeDef = TypedDict(
-    "FargateProfileTypeDef",
-    {
-        "fargateProfileName": str,
-        "fargateProfileArn": str,
-        "clusterName": str,
-        "createdAt": datetime,
-        "podExecutionRoleArn": str,
-        "subnets": List[str],
-        "selectors": List[FargateProfileSelectorTypeDef],
-        "status": FargateProfileStatusType,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredUpdateNodegroupVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupVersionRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1521,32 +1598,57 @@
 class DisassociateIdentityProviderConfigRequestRequestTypeDef(
     _RequiredDisassociateIdentityProviderConfigRequestRequestTypeDef,
     _OptionalDisassociateIdentityProviderConfigRequestRequestTypeDef,
 ):
     pass
 
 
-ListIdentityProviderConfigsResponseTypeDef = TypedDict(
-    "ListIdentityProviderConfigsResponseTypeDef",
+EncryptionConfigOutputTypeDef = TypedDict(
+    "EncryptionConfigOutputTypeDef",
     {
-        "identityProviderConfigs": List[IdentityProviderConfigTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resources": List[str],
+        "provider": ProviderOutputTypeDef,
     },
+    total=False,
 )
 
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "resources": Sequence[str],
         "provider": ProviderTypeDef,
     },
     total=False,
 )
 
+FargateProfileTypeDef = TypedDict(
+    "FargateProfileTypeDef",
+    {
+        "fargateProfileName": str,
+        "fargateProfileArn": str,
+        "clusterName": str,
+        "createdAt": datetime,
+        "podExecutionRoleArn": str,
+        "subnets": List[str],
+        "selectors": List[FargateProfileSelectorOutputTypeDef],
+        "status": FargateProfileStatusType,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+ListIdentityProviderConfigsResponseTypeDef = TypedDict(
+    "ListIdentityProviderConfigsResponseTypeDef",
+    {
+        "identityProviderConfigs": List[IdentityProviderConfigOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 IdentityProviderConfigResponseTypeDef = TypedDict(
     "IdentityProviderConfigResponseTypeDef",
     {
         "oidc": OidcIdentityProviderConfigTypeDef,
     },
     total=False,
 )
@@ -1563,14 +1665,22 @@
     "NodegroupHealthTypeDef",
     {
         "issues": List[IssueTypeDef],
     },
     total=False,
 )
 
+LoggingOutputTypeDef = TypedDict(
+    "LoggingOutputTypeDef",
+    {
+        "clusterLogging": List[LogSetupOutputTypeDef],
+    },
+    total=False,
+)
+
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "clusterLogging": Sequence[LogSetupTypeDef],
     },
     total=False,
 )
@@ -1618,38 +1728,14 @@
         "publisher": str,
         "owner": str,
         "marketplaceInformation": MarketplaceInformationTypeDef,
     },
     total=False,
 )
 
-CreateFargateProfileResponseTypeDef = TypedDict(
-    "CreateFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteFargateProfileResponseTypeDef = TypedDict(
-    "DeleteFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeFargateProfileResponseTypeDef = TypedDict(
-    "DescribeFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateNodegroupConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1692,14 +1778,38 @@
 class AssociateEncryptionConfigRequestRequestTypeDef(
     _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
     _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
 
+CreateFargateProfileResponseTypeDef = TypedDict(
+    "CreateFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteFargateProfileResponseTypeDef = TypedDict(
+    "DeleteFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeFargateProfileResponseTypeDef = TypedDict(
+    "DescribeFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeIdentityProviderConfigResponseTypeDef = TypedDict(
     "DescribeIdentityProviderConfigResponseTypeDef",
     {
         "identityProviderConfig": IdentityProviderConfigResponseTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1712,27 +1822,27 @@
         "clusterName": str,
         "version": str,
         "releaseVersion": str,
         "createdAt": datetime,
         "modifiedAt": datetime,
         "status": NodegroupStatusType,
         "capacityType": CapacityTypesType,
-        "scalingConfig": NodegroupScalingConfigTypeDef,
+        "scalingConfig": NodegroupScalingConfigOutputTypeDef,
         "instanceTypes": List[str],
         "subnets": List[str],
-        "remoteAccess": RemoteAccessConfigTypeDef,
+        "remoteAccess": RemoteAccessConfigOutputTypeDef,
         "amiType": AMITypesType,
         "nodeRole": str,
         "labels": Dict[str, str],
-        "taints": List[TaintTypeDef],
+        "taints": List[TaintOutputTypeDef],
         "resources": NodegroupResourcesTypeDef,
         "diskSize": int,
         "health": NodegroupHealthTypeDef,
-        "updateConfig": NodegroupUpdateConfigTypeDef,
-        "launchTemplate": LaunchTemplateSpecificationTypeDef,
+        "updateConfig": NodegroupUpdateConfigOutputTypeDef,
+        "launchTemplate": LaunchTemplateSpecificationOutputTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
@@ -1741,22 +1851,22 @@
         "arn": str,
         "createdAt": datetime,
         "version": str,
         "endpoint": str,
         "roleArn": str,
         "resourcesVpcConfig": VpcConfigResponseTypeDef,
         "kubernetesNetworkConfig": KubernetesNetworkConfigResponseTypeDef,
-        "logging": LoggingTypeDef,
+        "logging": LoggingOutputTypeDef,
         "identity": IdentityTypeDef,
         "status": ClusterStatusType,
         "certificateAuthority": CertificateTypeDef,
         "clientRequestToken": str,
         "platformVersion": str,
         "tags": Dict[str, str],
-        "encryptionConfig": List[EncryptionConfigTypeDef],
+        "encryptionConfig": List[EncryptionConfigOutputTypeDef],
         "connectorConfig": ConnectorConfigResponseTypeDef,
         "id": str,
         "health": ClusterHealthTypeDef,
         "outpostConfig": OutpostConfigResponseTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-eks-1.28.0/mypy_boto3_eks/type_defs.pyi` & `mypy-boto3-eks-1.28.12/mypy_boto3_eks/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -77,19 +77,23 @@
     "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
     "DescribeAddonVersionsRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeFargateProfileRequestRequestTypeDef",
     "IdentityProviderConfigTypeDef",
     "DescribeNodegroupRequestRequestTypeDef",
     "DescribeUpdateRequestRequestTypeDef",
+    "ProviderOutputTypeDef",
     "ProviderTypeDef",
     "ErrorDetailTypeDef",
+    "FargateProfileSelectorOutputTypeDef",
+    "IdentityProviderConfigOutputTypeDef",
     "OidcIdentityProviderConfigTypeDef",
     "OIDCTypeDef",
     "IssueTypeDef",
+    "LaunchTemplateSpecificationOutputTypeDef",
     "ListAddonsRequestListAddonsPaginateTypeDef",
     "ListAddonsRequestRequestTypeDef",
     "ListAddonsResponseTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListClustersResponseTypeDef",
     "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
@@ -101,15 +105,20 @@
     "ListNodegroupsRequestRequestTypeDef",
     "ListNodegroupsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "ListUpdatesRequestRequestTypeDef",
     "ListUpdatesResponseTypeDef",
+    "LogSetupOutputTypeDef",
     "LogSetupTypeDef",
+    "NodegroupScalingConfigOutputTypeDef",
+    "NodegroupUpdateConfigOutputTypeDef",
+    "RemoteAccessConfigOutputTypeDef",
+    "TaintOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddonRequestRequestTypeDef",
     "UpdateClusterVersionRequestRequestTypeDef",
     "UpdateLabelsPayloadTypeDef",
@@ -119,42 +128,44 @@
     "AssociateIdentityProviderConfigRequestRequestTypeDef",
     "NodegroupResourcesTypeDef",
     "ClusterHealthTypeDef",
     "RegisterClusterRequestRequestTypeDef",
     "OutpostConfigRequestTypeDef",
     "OutpostConfigResponseTypeDef",
     "CreateFargateProfileRequestRequestTypeDef",
-    "FargateProfileTypeDef",
     "UpdateNodegroupVersionRequestRequestTypeDef",
     "CreateNodegroupRequestRequestTypeDef",
     "UpdateTaintsPayloadTypeDef",
     "DescribeAddonRequestAddonActiveWaitTypeDef",
     "DescribeAddonRequestAddonDeletedWaitTypeDef",
     "DescribeClusterRequestClusterActiveWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef",
     "DescribeNodegroupRequestNodegroupActiveWaitTypeDef",
     "DescribeNodegroupRequestNodegroupDeletedWaitTypeDef",
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     "DisassociateIdentityProviderConfigRequestRequestTypeDef",
-    "ListIdentityProviderConfigsResponseTypeDef",
+    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
+    "FargateProfileTypeDef",
+    "ListIdentityProviderConfigsResponseTypeDef",
     "IdentityProviderConfigResponseTypeDef",
     "IdentityTypeDef",
     "NodegroupHealthTypeDef",
+    "LoggingOutputTypeDef",
     "LoggingTypeDef",
     "UpdateTypeDef",
     "AddonTypeDef",
     "AddonInfoTypeDef",
+    "UpdateNodegroupConfigRequestRequestTypeDef",
+    "AssociateEncryptionConfigRequestRequestTypeDef",
     "CreateFargateProfileResponseTypeDef",
     "DeleteFargateProfileResponseTypeDef",
     "DescribeFargateProfileResponseTypeDef",
-    "UpdateNodegroupConfigRequestRequestTypeDef",
-    "AssociateEncryptionConfigRequestRequestTypeDef",
     "DescribeIdentityProviderConfigResponseTypeDef",
     "NodegroupTypeDef",
     "ClusterTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterConfigRequestRequestTypeDef",
     "AssociateEncryptionConfigResponseTypeDef",
     "AssociateIdentityProviderConfigResponseTypeDef",
@@ -583,14 +594,22 @@
 )
 
 class DescribeUpdateRequestRequestTypeDef(
     _RequiredDescribeUpdateRequestRequestTypeDef, _OptionalDescribeUpdateRequestRequestTypeDef
 ):
     pass
 
+ProviderOutputTypeDef = TypedDict(
+    "ProviderOutputTypeDef",
+    {
+        "keyArn": str,
+    },
+    total=False,
+)
+
 ProviderTypeDef = TypedDict(
     "ProviderTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
@@ -601,14 +620,31 @@
         "errorCode": ErrorCodeType,
         "errorMessage": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
+FargateProfileSelectorOutputTypeDef = TypedDict(
+    "FargateProfileSelectorOutputTypeDef",
+    {
+        "namespace": str,
+        "labels": Dict[str, str],
+    },
+    total=False,
+)
+
+IdentityProviderConfigOutputTypeDef = TypedDict(
+    "IdentityProviderConfigOutputTypeDef",
+    {
+        "type": str,
+        "name": str,
+    },
+)
+
 OidcIdentityProviderConfigTypeDef = TypedDict(
     "OidcIdentityProviderConfigTypeDef",
     {
         "identityProviderConfigName": str,
         "identityProviderConfigArn": str,
         "clusterName": str,
         "issuerUrl": str,
@@ -638,14 +674,24 @@
         "code": NodegroupIssueCodeType,
         "message": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
+LaunchTemplateSpecificationOutputTypeDef = TypedDict(
+    "LaunchTemplateSpecificationOutputTypeDef",
+    {
+        "name": str,
+        "version": str,
+        "id": str,
+    },
+    total=False,
+)
+
 _RequiredListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
     "_RequiredListAddonsRequestListAddonsPaginateTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
@@ -923,23 +969,70 @@
     {
         "updateIds": List[str],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LogSetupOutputTypeDef = TypedDict(
+    "LogSetupOutputTypeDef",
+    {
+        "types": List[LogTypeType],
+        "enabled": bool,
+    },
+    total=False,
+)
+
 LogSetupTypeDef = TypedDict(
     "LogSetupTypeDef",
     {
         "types": Sequence[LogTypeType],
         "enabled": bool,
     },
     total=False,
 )
 
+NodegroupScalingConfigOutputTypeDef = TypedDict(
+    "NodegroupScalingConfigOutputTypeDef",
+    {
+        "minSize": int,
+        "maxSize": int,
+        "desiredSize": int,
+    },
+    total=False,
+)
+
+NodegroupUpdateConfigOutputTypeDef = TypedDict(
+    "NodegroupUpdateConfigOutputTypeDef",
+    {
+        "maxUnavailable": int,
+        "maxUnavailablePercentage": int,
+    },
+    total=False,
+)
+
+RemoteAccessConfigOutputTypeDef = TypedDict(
+    "RemoteAccessConfigOutputTypeDef",
+    {
+        "ec2SshKey": str,
+        "sourceSecurityGroups": List[str],
+    },
+    total=False,
+)
+
+TaintOutputTypeDef = TypedDict(
+    "TaintOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+        "effect": TaintEffectType,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1176,30 +1269,14 @@
 
 class CreateFargateProfileRequestRequestTypeDef(
     _RequiredCreateFargateProfileRequestRequestTypeDef,
     _OptionalCreateFargateProfileRequestRequestTypeDef,
 ):
     pass
 
-FargateProfileTypeDef = TypedDict(
-    "FargateProfileTypeDef",
-    {
-        "fargateProfileName": str,
-        "fargateProfileArn": str,
-        "clusterName": str,
-        "createdAt": datetime,
-        "podExecutionRoleArn": str,
-        "subnets": List[str],
-        "selectors": List[FargateProfileSelectorTypeDef],
-        "status": FargateProfileStatusType,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredUpdateNodegroupVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupVersionRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1456,32 +1533,57 @@
 
 class DisassociateIdentityProviderConfigRequestRequestTypeDef(
     _RequiredDisassociateIdentityProviderConfigRequestRequestTypeDef,
     _OptionalDisassociateIdentityProviderConfigRequestRequestTypeDef,
 ):
     pass
 
-ListIdentityProviderConfigsResponseTypeDef = TypedDict(
-    "ListIdentityProviderConfigsResponseTypeDef",
+EncryptionConfigOutputTypeDef = TypedDict(
+    "EncryptionConfigOutputTypeDef",
     {
-        "identityProviderConfigs": List[IdentityProviderConfigTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resources": List[str],
+        "provider": ProviderOutputTypeDef,
     },
+    total=False,
 )
 
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "resources": Sequence[str],
         "provider": ProviderTypeDef,
     },
     total=False,
 )
 
+FargateProfileTypeDef = TypedDict(
+    "FargateProfileTypeDef",
+    {
+        "fargateProfileName": str,
+        "fargateProfileArn": str,
+        "clusterName": str,
+        "createdAt": datetime,
+        "podExecutionRoleArn": str,
+        "subnets": List[str],
+        "selectors": List[FargateProfileSelectorOutputTypeDef],
+        "status": FargateProfileStatusType,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+ListIdentityProviderConfigsResponseTypeDef = TypedDict(
+    "ListIdentityProviderConfigsResponseTypeDef",
+    {
+        "identityProviderConfigs": List[IdentityProviderConfigOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 IdentityProviderConfigResponseTypeDef = TypedDict(
     "IdentityProviderConfigResponseTypeDef",
     {
         "oidc": OidcIdentityProviderConfigTypeDef,
     },
     total=False,
 )
@@ -1498,14 +1600,22 @@
     "NodegroupHealthTypeDef",
     {
         "issues": List[IssueTypeDef],
     },
     total=False,
 )
 
+LoggingOutputTypeDef = TypedDict(
+    "LoggingOutputTypeDef",
+    {
+        "clusterLogging": List[LogSetupOutputTypeDef],
+    },
+    total=False,
+)
+
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "clusterLogging": Sequence[LogSetupTypeDef],
     },
     total=False,
 )
@@ -1553,38 +1663,14 @@
         "publisher": str,
         "owner": str,
         "marketplaceInformation": MarketplaceInformationTypeDef,
     },
     total=False,
 )
 
-CreateFargateProfileResponseTypeDef = TypedDict(
-    "CreateFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteFargateProfileResponseTypeDef = TypedDict(
-    "DeleteFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeFargateProfileResponseTypeDef = TypedDict(
-    "DescribeFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateNodegroupConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1623,14 +1709,38 @@
 
 class AssociateEncryptionConfigRequestRequestTypeDef(
     _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
     _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
+CreateFargateProfileResponseTypeDef = TypedDict(
+    "CreateFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteFargateProfileResponseTypeDef = TypedDict(
+    "DeleteFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeFargateProfileResponseTypeDef = TypedDict(
+    "DescribeFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeIdentityProviderConfigResponseTypeDef = TypedDict(
     "DescribeIdentityProviderConfigResponseTypeDef",
     {
         "identityProviderConfig": IdentityProviderConfigResponseTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1643,27 +1753,27 @@
         "clusterName": str,
         "version": str,
         "releaseVersion": str,
         "createdAt": datetime,
         "modifiedAt": datetime,
         "status": NodegroupStatusType,
         "capacityType": CapacityTypesType,
-        "scalingConfig": NodegroupScalingConfigTypeDef,
+        "scalingConfig": NodegroupScalingConfigOutputTypeDef,
         "instanceTypes": List[str],
         "subnets": List[str],
-        "remoteAccess": RemoteAccessConfigTypeDef,
+        "remoteAccess": RemoteAccessConfigOutputTypeDef,
         "amiType": AMITypesType,
         "nodeRole": str,
         "labels": Dict[str, str],
-        "taints": List[TaintTypeDef],
+        "taints": List[TaintOutputTypeDef],
         "resources": NodegroupResourcesTypeDef,
         "diskSize": int,
         "health": NodegroupHealthTypeDef,
-        "updateConfig": NodegroupUpdateConfigTypeDef,
-        "launchTemplate": LaunchTemplateSpecificationTypeDef,
+        "updateConfig": NodegroupUpdateConfigOutputTypeDef,
+        "launchTemplate": LaunchTemplateSpecificationOutputTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
@@ -1672,22 +1782,22 @@
         "arn": str,
         "createdAt": datetime,
         "version": str,
         "endpoint": str,
         "roleArn": str,
         "resourcesVpcConfig": VpcConfigResponseTypeDef,
         "kubernetesNetworkConfig": KubernetesNetworkConfigResponseTypeDef,
-        "logging": LoggingTypeDef,
+        "logging": LoggingOutputTypeDef,
         "identity": IdentityTypeDef,
         "status": ClusterStatusType,
         "certificateAuthority": CertificateTypeDef,
         "clientRequestToken": str,
         "platformVersion": str,
         "tags": Dict[str, str],
-        "encryptionConfig": List[EncryptionConfigTypeDef],
+        "encryptionConfig": List[EncryptionConfigOutputTypeDef],
         "connectorConfig": ConnectorConfigResponseTypeDef,
         "id": str,
         "health": ClusterHealthTypeDef,
         "outpostConfig": OutpostConfigResponseTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-eks-1.28.0/mypy_boto3_eks/waiter.py` & `mypy-boto3-eks-1.28.12/mypy_boto3_eks/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.0/mypy_boto3_eks/waiter.pyi` & `mypy-boto3-eks-1.28.12/mypy_boto3_eks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.0/mypy_boto3_eks.egg-info/PKG-INFO` & `mypy-boto3-eks-1.28.12/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-eks
-Version: 1.28.0
-Summary: Type annotations for boto3.EKS 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 eks type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-eks"></a>
 
 # mypy-boto3-eks
 
 [![PyPI - mypy-boto3-eks](https://img.shields.io/pypi/v/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-eks?color=blue)](https://pypistats.org/packages/mypy-boto3-eks)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-eks)](https://pepy.tech/project/mypy-boto3-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EKS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[boto3.EKS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
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
 [mypy-boto3-eks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -449,19 +417,23 @@
     DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
     DescribeAddonVersionsRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
+    ProviderOutputTypeDef,
     ProviderTypeDef,
     ErrorDetailTypeDef,
+    FargateProfileSelectorOutputTypeDef,
+    IdentityProviderConfigOutputTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
+    LaunchTemplateSpecificationOutputTypeDef,
     ListAddonsRequestListAddonsPaginateTypeDef,
     ListAddonsRequestRequestTypeDef,
     ListAddonsResponseTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
     ListClustersResponseTypeDef,
     ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
@@ -473,15 +445,20 @@
     ListNodegroupsRequestRequestTypeDef,
     ListNodegroupsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUpdatesRequestListUpdatesPaginateTypeDef,
     ListUpdatesRequestRequestTypeDef,
     ListUpdatesResponseTypeDef,
+    LogSetupOutputTypeDef,
     LogSetupTypeDef,
+    NodegroupScalingConfigOutputTypeDef,
+    NodegroupUpdateConfigOutputTypeDef,
+    RemoteAccessConfigOutputTypeDef,
+    TaintOutputTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddonRequestRequestTypeDef,
     UpdateClusterVersionRequestRequestTypeDef,
     UpdateLabelsPayloadTypeDef,
@@ -491,42 +468,44 @@
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
     CreateFargateProfileRequestRequestTypeDef,
-    FargateProfileTypeDef,
     UpdateNodegroupVersionRequestRequestTypeDef,
     CreateNodegroupRequestRequestTypeDef,
     UpdateTaintsPayloadTypeDef,
     DescribeAddonRequestAddonActiveWaitTypeDef,
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
     DescribeNodegroupRequestNodegroupActiveWaitTypeDef,
     DescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
-    ListIdentityProviderConfigsResponseTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
+    FargateProfileTypeDef,
+    ListIdentityProviderConfigsResponseTypeDef,
     IdentityProviderConfigResponseTypeDef,
     IdentityTypeDef,
     NodegroupHealthTypeDef,
+    LoggingOutputTypeDef,
     LoggingTypeDef,
     UpdateTypeDef,
     AddonTypeDef,
     AddonInfoTypeDef,
+    UpdateNodegroupConfigRequestRequestTypeDef,
+    AssociateEncryptionConfigRequestRequestTypeDef,
     CreateFargateProfileResponseTypeDef,
     DeleteFargateProfileResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
-    UpdateNodegroupConfigRequestRequestTypeDef,
-    AssociateEncryptionConfigRequestRequestTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     NodegroupTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterConfigRequestRequestTypeDef,
     AssociateEncryptionConfigResponseTypeDef,
     AssociateIdentityProviderConfigResponseTypeDef,
```

### Comparing `mypy-boto3-eks-1.28.0/mypy_boto3_eks.egg-info/SOURCES.txt` & `mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.0/setup.py` & `mypy-boto3-eks-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-eks",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_eks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EKS 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.EKS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

