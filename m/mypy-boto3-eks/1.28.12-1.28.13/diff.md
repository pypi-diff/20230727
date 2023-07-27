# Comparing `tmp/mypy-boto3-eks-1.28.12.tar.gz` & `tmp/mypy-boto3-eks-1.28.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-eks-1.28.12.tar", last modified: Thu Jul 27 05:34:38 2023, max compression
+gzip compressed data, was "mypy-boto3-eks-1.28.13.tar", last modified: Thu Jul 27 19:34:20 2023, max compression
```

## Comparing `mypy-boto3-eks-1.28.12.tar` & `mypy-boto3-eks-1.28.13.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.088522 mypy-boto3-eks-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-07-27 05:34:38.088522 mypy-boto3-eks-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.084522 mypy-boto3-eks-1.28.12/mypy_boto3_eks/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33061 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33004 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-07-27 05:21:40.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14286 2023-07-27 05:21:40.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53041 2023-07-27 05:21:41.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    52968 2023-07-27 05:21:40.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-27 05:21:40.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-27 05:21:40.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.088522 mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-07-27 05:34:37.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 05:34:37.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:37.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:37.000000 mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:38.088522 mypy-boto3-eks-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:21:39.000000 mypy-boto3-eks-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:34:20.115558 mypy-boto3-eks-1.28.13/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 19:33:25.000000 mypy-boto3-eks-1.28.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-07-27 19:34:20.099558 mypy-boto3-eks-1.28.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-07-27 19:33:25.000000 mypy-boto3-eks-1.28.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:34:20.091558 mypy-boto3-eks-1.28.13/mypy_boto3_eks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-27 19:33:25.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-27 19:33:25.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 19:33:25.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33061 2023-07-27 19:33:26.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33004 2023-07-27 19:33:25.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-07-27 19:33:26.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-07-27 19:33:26.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-07-27 19:33:26.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-07-27 19:33:26.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:33:25.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52961 2023-07-27 19:33:28.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52888 2023-07-27 19:33:27.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 19:33:25.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-27 19:33:26.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-27 19:33:26.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:34:20.099558 mypy-boto3-eks-1.28.13/mypy_boto3_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-07-27 19:34:19.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 19:34:19.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:34:19.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:34:19.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 19:34:19.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 19:34:19.000000 mypy-boto3-eks-1.28.13/mypy_boto3_eks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 19:34:20.115558 mypy-boto3-eks-1.28.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 19:33:25.000000 mypy-boto3-eks-1.28.13/setup.py
```

### Comparing `mypy-boto3-eks-1.28.12/LICENSE` & `mypy-boto3-eks-1.28.13/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.12/PKG-INFO` & `mypy-boto3-eks-1.28.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-eks
-Version: 1.28.12
-Summary: Type annotations for boto3.EKS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.13
+Summary: Type annotations for boto3.EKS 1.28.13 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-eks)](https://pepy.tech/project/mypy-boto3-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EKS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[boto3.EKS 1.28.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -414,14 +414,15 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_eks.type_defs import (
     AddonIssueTypeDef,
     MarketplaceInformationTypeDef,
     CompatibilityTypeDef,
+    ResponseMetadataTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     AutoScalingGroupTypeDef,
     CertificateTypeDef,
     ClusterIssueTypeDef,
     ConnectorConfigResponseTypeDef,
     KubernetesNetworkConfigResponseTypeDef,
     VpcConfigResponseTypeDef,
@@ -439,18 +440,17 @@
     TaintTypeDef,
     DeleteAddonRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteFargateProfileRequestRequestTypeDef,
     DeleteNodegroupRequestRequestTypeDef,
     DeregisterClusterRequestRequestTypeDef,
     DescribeAddonConfigurationRequestRequestTypeDef,
-    DescribeAddonConfigurationResponseTypeDef,
     WaiterConfigTypeDef,
     DescribeAddonRequestRequestTypeDef,
-    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAddonVersionsRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
     ProviderOutputTypeDef,
@@ -458,49 +458,42 @@
     ErrorDetailTypeDef,
     FargateProfileSelectorOutputTypeDef,
     IdentityProviderConfigOutputTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
     LaunchTemplateSpecificationOutputTypeDef,
-    ListAddonsRequestListAddonsPaginateTypeDef,
     ListAddonsRequestRequestTypeDef,
-    ListAddonsResponseTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListClustersResponseTypeDef,
-    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
     ListFargateProfilesRequestRequestTypeDef,
-    ListFargateProfilesResponseTypeDef,
-    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
     ListIdentityProviderConfigsRequestRequestTypeDef,
-    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
     ListNodegroupsRequestRequestTypeDef,
-    ListNodegroupsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUpdatesRequestListUpdatesPaginateTypeDef,
     ListUpdatesRequestRequestTypeDef,
-    ListUpdatesResponseTypeDef,
     LogSetupOutputTypeDef,
     LogSetupTypeDef,
     NodegroupScalingConfigOutputTypeDef,
     NodegroupUpdateConfigOutputTypeDef,
     RemoteAccessConfigOutputTypeDef,
     TaintOutputTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddonRequestRequestTypeDef,
     UpdateClusterVersionRequestRequestTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateParamTypeDef,
     AddonHealthTypeDef,
     AddonVersionInfoTypeDef,
+    DescribeAddonConfigurationResponseTypeDef,
+    ListAddonsResponseTypeDef,
+    ListClustersResponseTypeDef,
+    ListFargateProfilesResponseTypeDef,
+    ListNodegroupsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUpdatesResponseTypeDef,
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
     CreateFargateProfileRequestRequestTypeDef,
@@ -511,14 +504,21 @@
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
     DescribeNodegroupRequestNodegroupActiveWaitTypeDef,
     DescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
+    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
+    ListAddonsRequestListAddonsPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
+    ListUpdatesRequestListUpdatesPaginateTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
     EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     FargateProfileTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     IdentityProviderConfigResponseTypeDef,
```

### Comparing `mypy-boto3-eks-1.28.12/README.md` & `mypy-boto3-eks-1.28.13/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-eks)](https://pepy.tech/project/mypy-boto3-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EKS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[boto3.EKS 1.28.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -382,14 +382,15 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_eks.type_defs import (
     AddonIssueTypeDef,
     MarketplaceInformationTypeDef,
     CompatibilityTypeDef,
+    ResponseMetadataTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     AutoScalingGroupTypeDef,
     CertificateTypeDef,
     ClusterIssueTypeDef,
     ConnectorConfigResponseTypeDef,
     KubernetesNetworkConfigResponseTypeDef,
     VpcConfigResponseTypeDef,
@@ -407,18 +408,17 @@
     TaintTypeDef,
     DeleteAddonRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteFargateProfileRequestRequestTypeDef,
     DeleteNodegroupRequestRequestTypeDef,
     DeregisterClusterRequestRequestTypeDef,
     DescribeAddonConfigurationRequestRequestTypeDef,
-    DescribeAddonConfigurationResponseTypeDef,
     WaiterConfigTypeDef,
     DescribeAddonRequestRequestTypeDef,
-    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAddonVersionsRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
     ProviderOutputTypeDef,
@@ -426,49 +426,42 @@
     ErrorDetailTypeDef,
     FargateProfileSelectorOutputTypeDef,
     IdentityProviderConfigOutputTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
     LaunchTemplateSpecificationOutputTypeDef,
-    ListAddonsRequestListAddonsPaginateTypeDef,
     ListAddonsRequestRequestTypeDef,
-    ListAddonsResponseTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListClustersResponseTypeDef,
-    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
     ListFargateProfilesRequestRequestTypeDef,
-    ListFargateProfilesResponseTypeDef,
-    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
     ListIdentityProviderConfigsRequestRequestTypeDef,
-    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
     ListNodegroupsRequestRequestTypeDef,
-    ListNodegroupsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUpdatesRequestListUpdatesPaginateTypeDef,
     ListUpdatesRequestRequestTypeDef,
-    ListUpdatesResponseTypeDef,
     LogSetupOutputTypeDef,
     LogSetupTypeDef,
     NodegroupScalingConfigOutputTypeDef,
     NodegroupUpdateConfigOutputTypeDef,
     RemoteAccessConfigOutputTypeDef,
     TaintOutputTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddonRequestRequestTypeDef,
     UpdateClusterVersionRequestRequestTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateParamTypeDef,
     AddonHealthTypeDef,
     AddonVersionInfoTypeDef,
+    DescribeAddonConfigurationResponseTypeDef,
+    ListAddonsResponseTypeDef,
+    ListClustersResponseTypeDef,
+    ListFargateProfilesResponseTypeDef,
+    ListNodegroupsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUpdatesResponseTypeDef,
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
     CreateFargateProfileRequestRequestTypeDef,
@@ -479,14 +472,21 @@
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
     DescribeNodegroupRequestNodegroupActiveWaitTypeDef,
     DescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
+    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
+    ListAddonsRequestListAddonsPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
+    ListUpdatesRequestListUpdatesPaginateTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
     EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     FargateProfileTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     IdentityProviderConfigResponseTypeDef,
```

### Comparing `mypy-boto3-eks-1.28.12/mypy_boto3_eks/__init__.py` & `mypy-boto3-eks-1.28.13/mypy_boto3_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.12/mypy_boto3_eks/__init__.pyi` & `mypy-boto3-eks-1.28.13/mypy_boto3_eks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.12/mypy_boto3_eks/__main__.py` & `mypy-boto3-eks-1.28.13/mypy_boto3_eks/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EKS 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        "Type annotations for boto3.EKS 1.28.13\nVersion:         1.28.13\nBuilder version:"
         " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.13")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-eks-1.28.12/mypy_boto3_eks/client.py` & `mypy-boto3-eks-1.28.13/mypy_boto3_eks/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.12/mypy_boto3_eks/client.pyi` & `mypy-boto3-eks-1.28.13/mypy_boto3_eks/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.12/mypy_boto3_eks/literals.py` & `mypy-boto3-eks-1.28.13/mypy_boto3_eks/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,32 +147,46 @@
 ListNodegroupsPaginatorName = Literal["list_nodegroups"]
 ListUpdatesPaginatorName = Literal["list_updates"]
 LogTypeType = Literal["api", "audit", "authenticator", "controllerManager", "scheduler"]
 NodegroupActiveWaiterName = Literal["nodegroup_active"]
 NodegroupDeletedWaiterName = Literal["nodegroup_deleted"]
 NodegroupIssueCodeType = Literal[
     "AccessDenied",
+    "AmiIdNotFound",
     "AsgInstanceLaunchFailures",
+    "AutoScalingGroupInstanceRefreshActive",
     "AutoScalingGroupInvalidConfiguration",
     "AutoScalingGroupNotFound",
+    "AutoScalingGroupOptInRequired",
+    "AutoScalingGroupRateLimitExceeded",
     "ClusterUnreachable",
+    "Ec2LaunchTemplateDeletionFailure",
+    "Ec2LaunchTemplateInvalidConfiguration",
+    "Ec2LaunchTemplateMaxLimitExceeded",
     "Ec2LaunchTemplateNotFound",
     "Ec2LaunchTemplateVersionMismatch",
     "Ec2SecurityGroupDeletionFailure",
     "Ec2SecurityGroupNotFound",
     "Ec2SubnetInvalidConfiguration",
+    "Ec2SubnetListTooLong",
     "Ec2SubnetMissingIpv6Assignment",
     "Ec2SubnetNotFound",
     "IamInstanceProfileNotFound",
     "IamLimitExceeded",
     "IamNodeRoleNotFound",
+    "IamThrottling",
     "InstanceLimitExceeded",
     "InsufficientFreeAddresses",
     "InternalFailure",
+    "LimitExceeded",
     "NodeCreationFailure",
+    "NodeTerminationFailure",
+    "PodEvictionFailure",
+    "SourceEc2LaunchTemplateNotFound",
+    "Unknown",
 ]
 NodegroupStatusType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATING", "DEGRADED", "DELETE_FAILED", "DELETING", "UPDATING"
 ]
 ResolveConflictsType = Literal["NONE", "OVERWRITE", "PRESERVE"]
 TaintEffectType = Literal["NO_EXECUTE", "NO_SCHEDULE", "PREFER_NO_SCHEDULE"]
 UpdateParamTypeType = Literal[
```

### Comparing `mypy-boto3-eks-1.28.12/mypy_boto3_eks/literals.pyi` & `mypy-boto3-eks-1.28.13/mypy_boto3_eks/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -145,32 +145,46 @@
 ListNodegroupsPaginatorName = Literal["list_nodegroups"]
 ListUpdatesPaginatorName = Literal["list_updates"]
 LogTypeType = Literal["api", "audit", "authenticator", "controllerManager", "scheduler"]
 NodegroupActiveWaiterName = Literal["nodegroup_active"]
 NodegroupDeletedWaiterName = Literal["nodegroup_deleted"]
 NodegroupIssueCodeType = Literal[
     "AccessDenied",
+    "AmiIdNotFound",
     "AsgInstanceLaunchFailures",
+    "AutoScalingGroupInstanceRefreshActive",
     "AutoScalingGroupInvalidConfiguration",
     "AutoScalingGroupNotFound",
+    "AutoScalingGroupOptInRequired",
+    "AutoScalingGroupRateLimitExceeded",
     "ClusterUnreachable",
+    "Ec2LaunchTemplateDeletionFailure",
+    "Ec2LaunchTemplateInvalidConfiguration",
+    "Ec2LaunchTemplateMaxLimitExceeded",
     "Ec2LaunchTemplateNotFound",
     "Ec2LaunchTemplateVersionMismatch",
     "Ec2SecurityGroupDeletionFailure",
     "Ec2SecurityGroupNotFound",
     "Ec2SubnetInvalidConfiguration",
+    "Ec2SubnetListTooLong",
     "Ec2SubnetMissingIpv6Assignment",
     "Ec2SubnetNotFound",
     "IamInstanceProfileNotFound",
     "IamLimitExceeded",
     "IamNodeRoleNotFound",
+    "IamThrottling",
     "InstanceLimitExceeded",
     "InsufficientFreeAddresses",
     "InternalFailure",
+    "LimitExceeded",
     "NodeCreationFailure",
+    "NodeTerminationFailure",
+    "PodEvictionFailure",
+    "SourceEc2LaunchTemplateNotFound",
+    "Unknown",
 ]
 NodegroupStatusType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATING", "DEGRADED", "DELETE_FAILED", "DELETING", "UPDATING"
 ]
 ResolveConflictsType = Literal["NONE", "OVERWRITE", "PRESERVE"]
 TaintEffectType = Literal["NO_EXECUTE", "NO_SCHEDULE", "PREFER_NO_SCHEDULE"]
 UpdateParamTypeType = Literal[
```

### Comparing `mypy-boto3-eks-1.28.12/mypy_boto3_eks/paginator.py` & `mypy-boto3-eks-1.28.13/mypy_boto3_eks/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,90 +77,90 @@
         self,
         *,
         kubernetesVersion: str = ...,
         addonName: str = ...,
         types: Sequence[str] = ...,
         publishers: Sequence[str] = ...,
         owners: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAddonVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.DescribeAddonVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#describeaddonversionspaginator)
         """
 
 
 class ListAddonsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAddons)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listaddonspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAddonsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAddons.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listaddonspaginator)
         """
 
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, include: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, include: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listclusterspaginator)
         """
 
 
 class ListFargateProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListFargateProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listfargateprofilespaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFargateProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListFargateProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listfargateprofilespaginator)
         """
 
 
 class ListIdentityProviderConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListIdentityProviderConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listidentityproviderconfigspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIdentityProviderConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListIdentityProviderConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listidentityproviderconfigspaginator)
         """
 
 
 class ListNodegroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListNodegroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listnodegroupspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNodegroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListNodegroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listnodegroupspaginator)
         """
 
 
@@ -172,13 +172,13 @@
 
     def paginate(
         self,
         *,
         name: str,
         nodegroupName: str = ...,
         addonName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListUpdates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listupdatespaginator)
         """
```

### Comparing `mypy-boto3-eks-1.28.12/mypy_boto3_eks/paginator.pyi` & `mypy-boto3-eks-1.28.13/mypy_boto3_eks/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -74,85 +74,85 @@
         self,
         *,
         kubernetesVersion: str = ...,
         addonName: str = ...,
         types: Sequence[str] = ...,
         publishers: Sequence[str] = ...,
         owners: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAddonVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.DescribeAddonVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#describeaddonversionspaginator)
         """
 
 class ListAddonsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAddons)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listaddonspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAddonsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAddons.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listaddonspaginator)
         """
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, include: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, include: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listclusterspaginator)
         """
 
 class ListFargateProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListFargateProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listfargateprofilespaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFargateProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListFargateProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listfargateprofilespaginator)
         """
 
 class ListIdentityProviderConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListIdentityProviderConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listidentityproviderconfigspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIdentityProviderConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListIdentityProviderConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listidentityproviderconfigspaginator)
         """
 
 class ListNodegroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListNodegroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listnodegroupspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNodegroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListNodegroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listnodegroupspaginator)
         """
 
 class ListUpdatesPaginator(Paginator):
@@ -163,13 +163,13 @@
 
     def paginate(
         self,
         *,
         name: str,
         nodegroupName: str = ...,
         addonName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListUpdates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/paginators/#listupdatespaginator)
         """
```

### Comparing `mypy-boto3-eks-1.28.12/mypy_boto3_eks/type_defs.py` & `mypy-boto3-eks-1.28.13/mypy_boto3_eks/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,19 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddonIssueTypeDef",
     "MarketplaceInformationTypeDef",
     "CompatibilityTypeDef",
+    "ResponseMetadataTypeDef",
     "OidcIdentityProviderConfigRequestTypeDef",
     "AutoScalingGroupTypeDef",
     "CertificateTypeDef",
     "ClusterIssueTypeDef",
     "ConnectorConfigResponseTypeDef",
     "KubernetesNetworkConfigResponseTypeDef",
     "VpcConfigResponseTypeDef",
@@ -68,18 +68,17 @@
     "TaintTypeDef",
     "DeleteAddonRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteFargateProfileRequestRequestTypeDef",
     "DeleteNodegroupRequestRequestTypeDef",
     "DeregisterClusterRequestRequestTypeDef",
     "DescribeAddonConfigurationRequestRequestTypeDef",
-    "DescribeAddonConfigurationResponseTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAddonRequestRequestTypeDef",
-    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAddonVersionsRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeFargateProfileRequestRequestTypeDef",
     "IdentityProviderConfigTypeDef",
     "DescribeNodegroupRequestRequestTypeDef",
     "DescribeUpdateRequestRequestTypeDef",
     "ProviderOutputTypeDef",
@@ -87,49 +86,42 @@
     "ErrorDetailTypeDef",
     "FargateProfileSelectorOutputTypeDef",
     "IdentityProviderConfigOutputTypeDef",
     "OidcIdentityProviderConfigTypeDef",
     "OIDCTypeDef",
     "IssueTypeDef",
     "LaunchTemplateSpecificationOutputTypeDef",
-    "ListAddonsRequestListAddonsPaginateTypeDef",
     "ListAddonsRequestRequestTypeDef",
-    "ListAddonsResponseTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
-    "ListClustersResponseTypeDef",
-    "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
     "ListFargateProfilesRequestRequestTypeDef",
-    "ListFargateProfilesResponseTypeDef",
-    "ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
     "ListIdentityProviderConfigsRequestRequestTypeDef",
-    "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
     "ListNodegroupsRequestRequestTypeDef",
-    "ListNodegroupsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "ListUpdatesRequestRequestTypeDef",
-    "ListUpdatesResponseTypeDef",
     "LogSetupOutputTypeDef",
     "LogSetupTypeDef",
     "NodegroupScalingConfigOutputTypeDef",
     "NodegroupUpdateConfigOutputTypeDef",
     "RemoteAccessConfigOutputTypeDef",
     "TaintOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddonRequestRequestTypeDef",
     "UpdateClusterVersionRequestRequestTypeDef",
     "UpdateLabelsPayloadTypeDef",
     "UpdateParamTypeDef",
     "AddonHealthTypeDef",
     "AddonVersionInfoTypeDef",
+    "DescribeAddonConfigurationResponseTypeDef",
+    "ListAddonsResponseTypeDef",
+    "ListClustersResponseTypeDef",
+    "ListFargateProfilesResponseTypeDef",
+    "ListNodegroupsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListUpdatesResponseTypeDef",
     "AssociateIdentityProviderConfigRequestRequestTypeDef",
     "NodegroupResourcesTypeDef",
     "ClusterHealthTypeDef",
     "RegisterClusterRequestRequestTypeDef",
     "OutpostConfigRequestTypeDef",
     "OutpostConfigResponseTypeDef",
     "CreateFargateProfileRequestRequestTypeDef",
@@ -140,14 +132,21 @@
     "DescribeAddonRequestAddonDeletedWaitTypeDef",
     "DescribeClusterRequestClusterActiveWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef",
     "DescribeNodegroupRequestNodegroupActiveWaitTypeDef",
     "DescribeNodegroupRequestNodegroupDeletedWaitTypeDef",
+    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+    "ListAddonsRequestListAddonsPaginateTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    "ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     "DisassociateIdentityProviderConfigRequestRequestTypeDef",
     "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
     "FargateProfileTypeDef",
     "ListIdentityProviderConfigsResponseTypeDef",
     "IdentityProviderConfigResponseTypeDef",
@@ -216,14 +215,25 @@
         "clusterVersion": str,
         "platformVersions": List[str],
         "defaultVersion": bool,
     },
     total=False,
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
 _RequiredOidcIdentityProviderConfigRequestTypeDef = TypedDict(
     "_RequiredOidcIdentityProviderConfigRequestTypeDef",
     {
         "identityProviderConfigName": str,
         "issuerUrl": str,
         "clientId": str,
     },
@@ -236,22 +246,20 @@
         "groupsClaim": str,
         "groupsPrefix": str,
         "requiredClaims": Mapping[str, str],
     },
     total=False,
 )
 
-
 class OidcIdentityProviderConfigRequestTypeDef(
     _RequiredOidcIdentityProviderConfigRequestTypeDef,
     _OptionalOidcIdentityProviderConfigRequestTypeDef,
 ):
     pass
 
-
 AutoScalingGroupTypeDef = TypedDict(
     "AutoScalingGroupTypeDef",
     {
         "name": str,
     },
     total=False,
 )
@@ -350,21 +358,19 @@
         "clientRequestToken": str,
         "tags": Mapping[str, str],
         "configurationValues": str,
     },
     total=False,
 )
 
-
 class CreateAddonRequestRequestTypeDef(
     _RequiredCreateAddonRequestRequestTypeDef, _OptionalCreateAddonRequestRequestTypeDef
 ):
     pass
 
-
 KubernetesNetworkConfigRequestTypeDef = TypedDict(
     "KubernetesNetworkConfigRequestTypeDef",
     {
         "serviceIpv4Cidr": str,
         "ipFamily": IpFamilyType,
     },
     total=False,
@@ -450,21 +456,19 @@
     "_OptionalDeleteAddonRequestRequestTypeDef",
     {
         "preserve": bool,
     },
     total=False,
 )
 
-
 class DeleteAddonRequestRequestTypeDef(
     _RequiredDeleteAddonRequestRequestTypeDef, _OptionalDeleteAddonRequestRequestTypeDef
 ):
     pass
 
-
 DeleteClusterRequestRequestTypeDef = TypedDict(
     "DeleteClusterRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -495,24 +499,14 @@
     "DescribeAddonConfigurationRequestRequestTypeDef",
     {
         "addonName": str,
         "addonVersion": str,
     },
 )
 
-DescribeAddonConfigurationResponseTypeDef = TypedDict(
-    "DescribeAddonConfigurationResponseTypeDef",
-    {
-        "addonName": str,
-        "addonVersion": str,
-        "configurationSchema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -522,23 +516,20 @@
     "DescribeAddonRequestRequestTypeDef",
     {
         "clusterName": str,
         "addonName": str,
     },
 )
 
-DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef = TypedDict(
-    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "kubernetesVersion": str,
-        "addonName": str,
-        "types": Sequence[str],
-        "publishers": Sequence[str],
-        "owners": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeAddonVersionsRequestRequestTypeDef = TypedDict(
     "DescribeAddonVersionsRequestRequestTypeDef",
     {
@@ -596,21 +587,19 @@
     {
         "nodegroupName": str,
         "addonName": str,
     },
     total=False,
 )
 
-
 class DescribeUpdateRequestRequestTypeDef(
     _RequiredDescribeUpdateRequestRequestTypeDef, _OptionalDescribeUpdateRequestRequestTypeDef
 ):
     pass
 
-
 ProviderOutputTypeDef = TypedDict(
     "ProviderOutputTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
@@ -693,36 +682,14 @@
         "name": str,
         "version": str,
         "id": str,
     },
     total=False,
 )
 
-_RequiredListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
-    "_RequiredListAddonsRequestListAddonsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
-    "_OptionalListAddonsRequestListAddonsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAddonsRequestListAddonsPaginateTypeDef(
-    _RequiredListAddonsRequestListAddonsPaginateTypeDef,
-    _OptionalListAddonsRequestListAddonsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAddonsRequestRequestTypeDef = TypedDict(
     "_RequiredListAddonsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListAddonsRequestRequestTypeDef = TypedDict(
@@ -730,80 +697,29 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListAddonsRequestRequestTypeDef(
     _RequiredListAddonsRequestRequestTypeDef, _OptionalListAddonsRequestRequestTypeDef
 ):
     pass
 
-
-ListAddonsResponseTypeDef = TypedDict(
-    "ListAddonsResponseTypeDef",
-    {
-        "addons": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "include": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "include": Sequence[str],
     },
     total=False,
 )
 
-ListClustersResponseTypeDef = TypedDict(
-    "ListClustersResponseTypeDef",
-    {
-        "clusters": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
-    "_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
-    "_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFargateProfilesRequestListFargateProfilesPaginateTypeDef(
-    _RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
-    _OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFargateProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListFargateProfilesRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListFargateProfilesRequestRequestTypeDef = TypedDict(
@@ -811,53 +727,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListFargateProfilesRequestRequestTypeDef(
     _RequiredListFargateProfilesRequestRequestTypeDef,
     _OptionalListFargateProfilesRequestRequestTypeDef,
 ):
     pass
 
-
-ListFargateProfilesResponseTypeDef = TypedDict(
-    "ListFargateProfilesResponseTypeDef",
-    {
-        "fargateProfileNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef(
-    _RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
-    _OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListIdentityProviderConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListIdentityProviderConfigsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListIdentityProviderConfigsRequestRequestTypeDef = TypedDict(
@@ -865,44 +748,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListIdentityProviderConfigsRequestRequestTypeDef(
     _RequiredListIdentityProviderConfigsRequestRequestTypeDef,
     _OptionalListIdentityProviderConfigsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
-    "_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
-    "_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListNodegroupsRequestListNodegroupsPaginateTypeDef(
-    _RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef,
-    _OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListNodegroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListNodegroupsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListNodegroupsRequestRequestTypeDef = TypedDict(
@@ -910,69 +769,26 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListNodegroupsRequestRequestTypeDef(
     _RequiredListNodegroupsRequestRequestTypeDef, _OptionalListNodegroupsRequestRequestTypeDef
 ):
     pass
 
-
-ListNodegroupsResponseTypeDef = TypedDict(
-    "ListNodegroupsResponseTypeDef",
-    {
-        "nodegroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
-    "_RequiredListUpdatesRequestListUpdatesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
-    "_OptionalListUpdatesRequestListUpdatesPaginateTypeDef",
-    {
-        "nodegroupName": str,
-        "addonName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUpdatesRequestListUpdatesPaginateTypeDef(
-    _RequiredListUpdatesRequestListUpdatesPaginateTypeDef,
-    _OptionalListUpdatesRequestListUpdatesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUpdatesRequestRequestTypeDef = TypedDict(
     "_RequiredListUpdatesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListUpdatesRequestRequestTypeDef = TypedDict(
@@ -982,30 +798,19 @@
         "addonName": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListUpdatesRequestRequestTypeDef(
     _RequiredListUpdatesRequestRequestTypeDef, _OptionalListUpdatesRequestRequestTypeDef
 ):
     pass
 
-
-ListUpdatesResponseTypeDef = TypedDict(
-    "ListUpdatesResponseTypeDef",
-    {
-        "updateIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LogSetupOutputTypeDef = TypedDict(
     "LogSetupOutputTypeDef",
     {
         "types": List[LogTypeType],
         "enabled": bool,
     },
     total=False,
@@ -1054,35 +859,14 @@
         "key": str,
         "value": str,
         "effect": TaintEffectType,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1110,21 +894,19 @@
         "resolveConflicts": ResolveConflictsType,
         "clientRequestToken": str,
         "configurationValues": str,
     },
     total=False,
 )
 
-
 class UpdateAddonRequestRequestTypeDef(
     _RequiredUpdateAddonRequestRequestTypeDef, _OptionalUpdateAddonRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateClusterVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterVersionRequestRequestTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
@@ -1132,22 +914,20 @@
     "_OptionalUpdateClusterVersionRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
-
 class UpdateClusterVersionRequestRequestTypeDef(
     _RequiredUpdateClusterVersionRequestRequestTypeDef,
     _OptionalUpdateClusterVersionRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateLabelsPayloadTypeDef = TypedDict(
     "UpdateLabelsPayloadTypeDef",
     {
         "addOrUpdateLabels": Mapping[str, str],
         "removeLabels": Sequence[str],
     },
     total=False,
@@ -1177,14 +957,77 @@
         "architecture": List[str],
         "compatibilities": List[CompatibilityTypeDef],
         "requiresConfiguration": bool,
     },
     total=False,
 )
 
+DescribeAddonConfigurationResponseTypeDef = TypedDict(
+    "DescribeAddonConfigurationResponseTypeDef",
+    {
+        "addonName": str,
+        "addonVersion": str,
+        "configurationSchema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAddonsResponseTypeDef = TypedDict(
+    "ListAddonsResponseTypeDef",
+    {
+        "addons": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListClustersResponseTypeDef = TypedDict(
+    "ListClustersResponseTypeDef",
+    {
+        "clusters": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFargateProfilesResponseTypeDef = TypedDict(
+    "ListFargateProfilesResponseTypeDef",
+    {
+        "fargateProfileNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListNodegroupsResponseTypeDef = TypedDict(
+    "ListNodegroupsResponseTypeDef",
+    {
+        "nodegroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListUpdatesResponseTypeDef = TypedDict(
+    "ListUpdatesResponseTypeDef",
+    {
+        "updateIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredAssociateIdentityProviderConfigRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateIdentityProviderConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "oidc": OidcIdentityProviderConfigRequestTypeDef,
     },
 )
@@ -1193,22 +1036,20 @@
     {
         "tags": Mapping[str, str],
         "clientRequestToken": str,
     },
     total=False,
 )
 
-
 class AssociateIdentityProviderConfigRequestRequestTypeDef(
     _RequiredAssociateIdentityProviderConfigRequestRequestTypeDef,
     _OptionalAssociateIdentityProviderConfigRequestRequestTypeDef,
 ):
     pass
 
-
 NodegroupResourcesTypeDef = TypedDict(
     "NodegroupResourcesTypeDef",
     {
         "autoScalingGroups": List[AutoScalingGroupTypeDef],
         "remoteAccessSecurityGroup": str,
     },
     total=False,
@@ -1234,21 +1075,19 @@
     {
         "clientRequestToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class RegisterClusterRequestRequestTypeDef(
     _RequiredRegisterClusterRequestRequestTypeDef, _OptionalRegisterClusterRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredOutpostConfigRequestTypeDef = TypedDict(
     "_RequiredOutpostConfigRequestTypeDef",
     {
         "outpostArns": Sequence[str],
         "controlPlaneInstanceType": str,
     },
 )
@@ -1256,21 +1095,19 @@
     "_OptionalOutpostConfigRequestTypeDef",
     {
         "controlPlanePlacement": ControlPlanePlacementRequestTypeDef,
     },
     total=False,
 )
 
-
 class OutpostConfigRequestTypeDef(
     _RequiredOutpostConfigRequestTypeDef, _OptionalOutpostConfigRequestTypeDef
 ):
     pass
 
-
 _RequiredOutpostConfigResponseTypeDef = TypedDict(
     "_RequiredOutpostConfigResponseTypeDef",
     {
         "outpostArns": List[str],
         "controlPlaneInstanceType": str,
     },
 )
@@ -1278,21 +1115,19 @@
     "_OptionalOutpostConfigResponseTypeDef",
     {
         "controlPlanePlacement": ControlPlanePlacementResponseTypeDef,
     },
     total=False,
 )
 
-
 class OutpostConfigResponseTypeDef(
     _RequiredOutpostConfigResponseTypeDef, _OptionalOutpostConfigResponseTypeDef
 ):
     pass
 
-
 _RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFargateProfileRequestRequestTypeDef",
     {
         "fargateProfileName": str,
         "clusterName": str,
         "podExecutionRoleArn": str,
     },
@@ -1304,22 +1139,20 @@
         "selectors": Sequence[FargateProfileSelectorTypeDef],
         "clientRequestToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateFargateProfileRequestRequestTypeDef(
     _RequiredCreateFargateProfileRequestRequestTypeDef,
     _OptionalCreateFargateProfileRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateNodegroupVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupVersionRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1331,22 +1164,20 @@
         "launchTemplate": LaunchTemplateSpecificationTypeDef,
         "force": bool,
         "clientRequestToken": str,
     },
     total=False,
 )
 
-
 class UpdateNodegroupVersionRequestRequestTypeDef(
     _RequiredUpdateNodegroupVersionRequestRequestTypeDef,
     _OptionalUpdateNodegroupVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateNodegroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNodegroupRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
         "subnets": Sequence[str],
         "nodeRole": str,
@@ -1369,21 +1200,19 @@
         "capacityType": CapacityTypesType,
         "version": str,
         "releaseVersion": str,
     },
     total=False,
 )
 
-
 class CreateNodegroupRequestRequestTypeDef(
     _RequiredCreateNodegroupRequestRequestTypeDef, _OptionalCreateNodegroupRequestRequestTypeDef
 ):
     pass
 
-
 UpdateTaintsPayloadTypeDef = TypedDict(
     "UpdateTaintsPayloadTypeDef",
     {
         "addOrUpdateTaints": Sequence[TaintTypeDef],
         "removeTaints": Sequence[TaintTypeDef],
     },
     total=False,
@@ -1400,22 +1229,20 @@
     "_OptionalDescribeAddonRequestAddonActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAddonRequestAddonActiveWaitTypeDef(
     _RequiredDescribeAddonRequestAddonActiveWaitTypeDef,
     _OptionalDescribeAddonRequestAddonActiveWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAddonRequestAddonDeletedWaitTypeDef = TypedDict(
     "_RequiredDescribeAddonRequestAddonDeletedWaitTypeDef",
     {
         "clusterName": str,
         "addonName": str,
     },
 )
@@ -1423,66 +1250,60 @@
     "_OptionalDescribeAddonRequestAddonDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAddonRequestAddonDeletedWaitTypeDef(
     _RequiredDescribeAddonRequestAddonDeletedWaitTypeDef,
     _OptionalDescribeAddonRequestAddonDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeClusterRequestClusterActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeClusterRequestClusterActiveWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalDescribeClusterRequestClusterActiveWaitTypeDef = TypedDict(
     "_OptionalDescribeClusterRequestClusterActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeClusterRequestClusterActiveWaitTypeDef(
     _RequiredDescribeClusterRequestClusterActiveWaitTypeDef,
     _OptionalDescribeClusterRequestClusterActiveWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeClusterRequestClusterDeletedWaitTypeDef = TypedDict(
     "_RequiredDescribeClusterRequestClusterDeletedWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalDescribeClusterRequestClusterDeletedWaitTypeDef = TypedDict(
     "_OptionalDescribeClusterRequestClusterDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeClusterRequestClusterDeletedWaitTypeDef(
     _RequiredDescribeClusterRequestClusterDeletedWaitTypeDef,
     _OptionalDescribeClusterRequestClusterDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeFargateProfileRequestFargateProfileActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeFargateProfileRequestFargateProfileActiveWaitTypeDef",
     {
         "clusterName": str,
         "fargateProfileName": str,
     },
 )
@@ -1490,22 +1311,20 @@
     "_OptionalDescribeFargateProfileRequestFargateProfileActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef(
     _RequiredDescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
     _OptionalDescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef = TypedDict(
     "_RequiredDescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef",
     {
         "clusterName": str,
         "fargateProfileName": str,
     },
 )
@@ -1513,22 +1332,20 @@
     "_OptionalDescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef(
     _RequiredDescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
     _OptionalDescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeNodegroupRequestNodegroupActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeNodegroupRequestNodegroupActiveWaitTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1536,22 +1353,20 @@
     "_OptionalDescribeNodegroupRequestNodegroupActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeNodegroupRequestNodegroupActiveWaitTypeDef(
     _RequiredDescribeNodegroupRequestNodegroupActiveWaitTypeDef,
     _OptionalDescribeNodegroupRequestNodegroupActiveWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeNodegroupRequestNodegroupDeletedWaitTypeDef = TypedDict(
     "_RequiredDescribeNodegroupRequestNodegroupDeletedWaitTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1559,21 +1374,143 @@
     "_OptionalDescribeNodegroupRequestNodegroupDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeNodegroupRequestNodegroupDeletedWaitTypeDef(
     _RequiredDescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
     _OptionalDescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
 ):
     pass
 
+DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef = TypedDict(
+    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+    {
+        "kubernetesVersion": str,
+        "addonName": str,
+        "types": Sequence[str],
+        "publishers": Sequence[str],
+        "owners": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
+    "_RequiredListAddonsRequestListAddonsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
+    "_OptionalListAddonsRequestListAddonsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAddonsRequestListAddonsPaginateTypeDef(
+    _RequiredListAddonsRequestListAddonsPaginateTypeDef,
+    _OptionalListAddonsRequestListAddonsPaginateTypeDef,
+):
+    pass
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "include": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
+    "_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
+    "_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFargateProfilesRequestListFargateProfilesPaginateTypeDef(
+    _RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+    _OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+):
+    pass
+
+_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef(
+    _RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+    _OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+):
+    pass
+
+_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
+    "_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
+    "_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListNodegroupsRequestListNodegroupsPaginateTypeDef(
+    _RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef,
+    _OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
+    "_RequiredListUpdatesRequestListUpdatesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
+    "_OptionalListUpdatesRequestListUpdatesPaginateTypeDef",
+    {
+        "nodegroupName": str,
+        "addonName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUpdatesRequestListUpdatesPaginateTypeDef(
+    _RequiredListUpdatesRequestListUpdatesPaginateTypeDef,
+    _OptionalListUpdatesRequestListUpdatesPaginateTypeDef,
+):
+    pass
 
 DescribeIdentityProviderConfigRequestRequestTypeDef = TypedDict(
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "identityProviderConfig": IdentityProviderConfigTypeDef,
     },
@@ -1590,22 +1527,20 @@
     "_OptionalDisassociateIdentityProviderConfigRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
-
 class DisassociateIdentityProviderConfigRequestRequestTypeDef(
     _RequiredDisassociateIdentityProviderConfigRequestRequestTypeDef,
     _OptionalDisassociateIdentityProviderConfigRequestRequestTypeDef,
 ):
     pass
 
-
 EncryptionConfigOutputTypeDef = TypedDict(
     "EncryptionConfigOutputTypeDef",
     {
         "resources": List[str],
         "provider": ProviderOutputTypeDef,
     },
     total=False,
@@ -1637,15 +1572,15 @@
 )
 
 ListIdentityProviderConfigsResponseTypeDef = TypedDict(
     "ListIdentityProviderConfigsResponseTypeDef",
     {
         "identityProviderConfigs": List[IdentityProviderConfigOutputTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IdentityProviderConfigResponseTypeDef = TypedDict(
     "IdentityProviderConfigResponseTypeDef",
     {
         "oidc": OidcIdentityProviderConfigTypeDef,
@@ -1747,22 +1682,20 @@
         "scalingConfig": NodegroupScalingConfigTypeDef,
         "updateConfig": NodegroupUpdateConfigTypeDef,
         "clientRequestToken": str,
     },
     total=False,
 )
 
-
 class UpdateNodegroupConfigRequestRequestTypeDef(
     _RequiredUpdateNodegroupConfigRequestRequestTypeDef,
     _OptionalUpdateNodegroupConfigRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "encryptionConfig": Sequence[EncryptionConfigTypeDef],
     },
 )
@@ -1770,51 +1703,49 @@
     "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
-
 class AssociateEncryptionConfigRequestRequestTypeDef(
     _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
     _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
-
 CreateFargateProfileResponseTypeDef = TypedDict(
     "CreateFargateProfileResponseTypeDef",
     {
         "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFargateProfileResponseTypeDef = TypedDict(
     "DeleteFargateProfileResponseTypeDef",
     {
         "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFargateProfileResponseTypeDef = TypedDict(
     "DescribeFargateProfileResponseTypeDef",
     {
         "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIdentityProviderConfigResponseTypeDef = TypedDict(
     "DescribeIdentityProviderConfigResponseTypeDef",
     {
         "identityProviderConfig": IdentityProviderConfigResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NodegroupTypeDef = TypedDict(
     "NodegroupTypeDef",
     {
         "nodegroupName": str,
@@ -1889,21 +1820,19 @@
         "tags": Mapping[str, str],
         "encryptionConfig": Sequence[EncryptionConfigTypeDef],
         "outpostConfig": OutpostConfigRequestTypeDef,
     },
     total=False,
 )
 
-
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateClusterConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterConfigRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateClusterConfigRequestRequestTypeDef = TypedDict(
@@ -1912,184 +1841,182 @@
         "resourcesVpcConfig": VpcConfigRequestTypeDef,
         "logging": LoggingTypeDef,
         "clientRequestToken": str,
     },
     total=False,
 )
 
-
 class UpdateClusterConfigRequestRequestTypeDef(
     _RequiredUpdateClusterConfigRequestRequestTypeDef,
     _OptionalUpdateClusterConfigRequestRequestTypeDef,
 ):
     pass
 
-
 AssociateEncryptionConfigResponseTypeDef = TypedDict(
     "AssociateEncryptionConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateIdentityProviderConfigResponseTypeDef = TypedDict(
     "AssociateIdentityProviderConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUpdateResponseTypeDef = TypedDict(
     "DescribeUpdateResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateIdentityProviderConfigResponseTypeDef = TypedDict(
     "DisassociateIdentityProviderConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAddonResponseTypeDef = TypedDict(
     "UpdateAddonResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterConfigResponseTypeDef = TypedDict(
     "UpdateClusterConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterVersionResponseTypeDef = TypedDict(
     "UpdateClusterVersionResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNodegroupConfigResponseTypeDef = TypedDict(
     "UpdateNodegroupConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNodegroupVersionResponseTypeDef = TypedDict(
     "UpdateNodegroupVersionResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAddonResponseTypeDef = TypedDict(
     "CreateAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAddonResponseTypeDef = TypedDict(
     "DeleteAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAddonResponseTypeDef = TypedDict(
     "DescribeAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAddonVersionsResponseTypeDef = TypedDict(
     "DescribeAddonVersionsResponseTypeDef",
     {
         "addons": List[AddonInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateNodegroupResponseTypeDef = TypedDict(
     "CreateNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteNodegroupResponseTypeDef = TypedDict(
     "DeleteNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNodegroupResponseTypeDef = TypedDict(
     "DescribeNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeregisterClusterResponseTypeDef = TypedDict(
     "DeregisterClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterClusterResponseTypeDef = TypedDict(
     "RegisterClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-eks-1.28.12/mypy_boto3_eks/type_defs.pyi` & `mypy-boto3-eks-1.28.13/mypy_boto3_eks/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,18 +38,20 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AddonIssueTypeDef",
     "MarketplaceInformationTypeDef",
     "CompatibilityTypeDef",
+    "ResponseMetadataTypeDef",
     "OidcIdentityProviderConfigRequestTypeDef",
     "AutoScalingGroupTypeDef",
     "CertificateTypeDef",
     "ClusterIssueTypeDef",
     "ConnectorConfigResponseTypeDef",
     "KubernetesNetworkConfigResponseTypeDef",
     "VpcConfigResponseTypeDef",
@@ -67,18 +69,17 @@
     "TaintTypeDef",
     "DeleteAddonRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteFargateProfileRequestRequestTypeDef",
     "DeleteNodegroupRequestRequestTypeDef",
     "DeregisterClusterRequestRequestTypeDef",
     "DescribeAddonConfigurationRequestRequestTypeDef",
-    "DescribeAddonConfigurationResponseTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAddonRequestRequestTypeDef",
-    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAddonVersionsRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeFargateProfileRequestRequestTypeDef",
     "IdentityProviderConfigTypeDef",
     "DescribeNodegroupRequestRequestTypeDef",
     "DescribeUpdateRequestRequestTypeDef",
     "ProviderOutputTypeDef",
@@ -86,49 +87,42 @@
     "ErrorDetailTypeDef",
     "FargateProfileSelectorOutputTypeDef",
     "IdentityProviderConfigOutputTypeDef",
     "OidcIdentityProviderConfigTypeDef",
     "OIDCTypeDef",
     "IssueTypeDef",
     "LaunchTemplateSpecificationOutputTypeDef",
-    "ListAddonsRequestListAddonsPaginateTypeDef",
     "ListAddonsRequestRequestTypeDef",
-    "ListAddonsResponseTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
-    "ListClustersResponseTypeDef",
-    "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
     "ListFargateProfilesRequestRequestTypeDef",
-    "ListFargateProfilesResponseTypeDef",
-    "ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
     "ListIdentityProviderConfigsRequestRequestTypeDef",
-    "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
     "ListNodegroupsRequestRequestTypeDef",
-    "ListNodegroupsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "ListUpdatesRequestRequestTypeDef",
-    "ListUpdatesResponseTypeDef",
     "LogSetupOutputTypeDef",
     "LogSetupTypeDef",
     "NodegroupScalingConfigOutputTypeDef",
     "NodegroupUpdateConfigOutputTypeDef",
     "RemoteAccessConfigOutputTypeDef",
     "TaintOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddonRequestRequestTypeDef",
     "UpdateClusterVersionRequestRequestTypeDef",
     "UpdateLabelsPayloadTypeDef",
     "UpdateParamTypeDef",
     "AddonHealthTypeDef",
     "AddonVersionInfoTypeDef",
+    "DescribeAddonConfigurationResponseTypeDef",
+    "ListAddonsResponseTypeDef",
+    "ListClustersResponseTypeDef",
+    "ListFargateProfilesResponseTypeDef",
+    "ListNodegroupsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListUpdatesResponseTypeDef",
     "AssociateIdentityProviderConfigRequestRequestTypeDef",
     "NodegroupResourcesTypeDef",
     "ClusterHealthTypeDef",
     "RegisterClusterRequestRequestTypeDef",
     "OutpostConfigRequestTypeDef",
     "OutpostConfigResponseTypeDef",
     "CreateFargateProfileRequestRequestTypeDef",
@@ -139,14 +133,21 @@
     "DescribeAddonRequestAddonDeletedWaitTypeDef",
     "DescribeClusterRequestClusterActiveWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef",
     "DescribeNodegroupRequestNodegroupActiveWaitTypeDef",
     "DescribeNodegroupRequestNodegroupDeletedWaitTypeDef",
+    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+    "ListAddonsRequestListAddonsPaginateTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    "ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     "DisassociateIdentityProviderConfigRequestRequestTypeDef",
     "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
     "FargateProfileTypeDef",
     "ListIdentityProviderConfigsResponseTypeDef",
     "IdentityProviderConfigResponseTypeDef",
@@ -215,14 +216,25 @@
         "clusterVersion": str,
         "platformVersions": List[str],
         "defaultVersion": bool,
     },
     total=False,
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
 _RequiredOidcIdentityProviderConfigRequestTypeDef = TypedDict(
     "_RequiredOidcIdentityProviderConfigRequestTypeDef",
     {
         "identityProviderConfigName": str,
         "issuerUrl": str,
         "clientId": str,
     },
@@ -235,20 +247,22 @@
         "groupsClaim": str,
         "groupsPrefix": str,
         "requiredClaims": Mapping[str, str],
     },
     total=False,
 )
 
+
 class OidcIdentityProviderConfigRequestTypeDef(
     _RequiredOidcIdentityProviderConfigRequestTypeDef,
     _OptionalOidcIdentityProviderConfigRequestTypeDef,
 ):
     pass
 
+
 AutoScalingGroupTypeDef = TypedDict(
     "AutoScalingGroupTypeDef",
     {
         "name": str,
     },
     total=False,
 )
@@ -347,19 +361,21 @@
         "clientRequestToken": str,
         "tags": Mapping[str, str],
         "configurationValues": str,
     },
     total=False,
 )
 
+
 class CreateAddonRequestRequestTypeDef(
     _RequiredCreateAddonRequestRequestTypeDef, _OptionalCreateAddonRequestRequestTypeDef
 ):
     pass
 
+
 KubernetesNetworkConfigRequestTypeDef = TypedDict(
     "KubernetesNetworkConfigRequestTypeDef",
     {
         "serviceIpv4Cidr": str,
         "ipFamily": IpFamilyType,
     },
     total=False,
@@ -445,19 +461,21 @@
     "_OptionalDeleteAddonRequestRequestTypeDef",
     {
         "preserve": bool,
     },
     total=False,
 )
 
+
 class DeleteAddonRequestRequestTypeDef(
     _RequiredDeleteAddonRequestRequestTypeDef, _OptionalDeleteAddonRequestRequestTypeDef
 ):
     pass
 
+
 DeleteClusterRequestRequestTypeDef = TypedDict(
     "DeleteClusterRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -488,24 +506,14 @@
     "DescribeAddonConfigurationRequestRequestTypeDef",
     {
         "addonName": str,
         "addonVersion": str,
     },
 )
 
-DescribeAddonConfigurationResponseTypeDef = TypedDict(
-    "DescribeAddonConfigurationResponseTypeDef",
-    {
-        "addonName": str,
-        "addonVersion": str,
-        "configurationSchema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -515,23 +523,20 @@
     "DescribeAddonRequestRequestTypeDef",
     {
         "clusterName": str,
         "addonName": str,
     },
 )
 
-DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef = TypedDict(
-    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "kubernetesVersion": str,
-        "addonName": str,
-        "types": Sequence[str],
-        "publishers": Sequence[str],
-        "owners": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeAddonVersionsRequestRequestTypeDef = TypedDict(
     "DescribeAddonVersionsRequestRequestTypeDef",
     {
@@ -589,19 +594,21 @@
     {
         "nodegroupName": str,
         "addonName": str,
     },
     total=False,
 )
 
+
 class DescribeUpdateRequestRequestTypeDef(
     _RequiredDescribeUpdateRequestRequestTypeDef, _OptionalDescribeUpdateRequestRequestTypeDef
 ):
     pass
 
+
 ProviderOutputTypeDef = TypedDict(
     "ProviderOutputTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
@@ -684,34 +691,14 @@
         "name": str,
         "version": str,
         "id": str,
     },
     total=False,
 )
 
-_RequiredListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
-    "_RequiredListAddonsRequestListAddonsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
-    "_OptionalListAddonsRequestListAddonsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAddonsRequestListAddonsPaginateTypeDef(
-    _RequiredListAddonsRequestListAddonsPaginateTypeDef,
-    _OptionalListAddonsRequestListAddonsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAddonsRequestRequestTypeDef = TypedDict(
     "_RequiredListAddonsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListAddonsRequestRequestTypeDef = TypedDict(
@@ -719,76 +706,31 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListAddonsRequestRequestTypeDef(
     _RequiredListAddonsRequestRequestTypeDef, _OptionalListAddonsRequestRequestTypeDef
 ):
     pass
 
-ListAddonsResponseTypeDef = TypedDict(
-    "ListAddonsResponseTypeDef",
-    {
-        "addons": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "include": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "include": Sequence[str],
     },
     total=False,
 )
 
-ListClustersResponseTypeDef = TypedDict(
-    "ListClustersResponseTypeDef",
-    {
-        "clusters": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
-    "_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
-    "_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFargateProfilesRequestListFargateProfilesPaginateTypeDef(
-    _RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
-    _OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
-):
-    pass
-
 _RequiredListFargateProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListFargateProfilesRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListFargateProfilesRequestRequestTypeDef = TypedDict(
@@ -796,48 +738,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListFargateProfilesRequestRequestTypeDef(
     _RequiredListFargateProfilesRequestRequestTypeDef,
     _OptionalListFargateProfilesRequestRequestTypeDef,
 ):
     pass
 
-ListFargateProfilesResponseTypeDef = TypedDict(
-    "ListFargateProfilesResponseTypeDef",
-    {
-        "fargateProfileNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef(
-    _RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
-    _OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
-):
-    pass
 
 _RequiredListIdentityProviderConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListIdentityProviderConfigsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
@@ -846,39 +761,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListIdentityProviderConfigsRequestRequestTypeDef(
     _RequiredListIdentityProviderConfigsRequestRequestTypeDef,
     _OptionalListIdentityProviderConfigsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
-    "_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
-    "_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListNodegroupsRequestListNodegroupsPaginateTypeDef(
-    _RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef,
-    _OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef,
-):
-    pass
 
 _RequiredListNodegroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListNodegroupsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
@@ -887,65 +784,28 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListNodegroupsRequestRequestTypeDef(
     _RequiredListNodegroupsRequestRequestTypeDef, _OptionalListNodegroupsRequestRequestTypeDef
 ):
     pass
 
-ListNodegroupsResponseTypeDef = TypedDict(
-    "ListNodegroupsResponseTypeDef",
-    {
-        "nodegroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
-    "_RequiredListUpdatesRequestListUpdatesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
-    "_OptionalListUpdatesRequestListUpdatesPaginateTypeDef",
-    {
-        "nodegroupName": str,
-        "addonName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUpdatesRequestListUpdatesPaginateTypeDef(
-    _RequiredListUpdatesRequestListUpdatesPaginateTypeDef,
-    _OptionalListUpdatesRequestListUpdatesPaginateTypeDef,
-):
-    pass
-
 _RequiredListUpdatesRequestRequestTypeDef = TypedDict(
     "_RequiredListUpdatesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListUpdatesRequestRequestTypeDef = TypedDict(
@@ -955,27 +815,20 @@
         "addonName": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListUpdatesRequestRequestTypeDef(
     _RequiredListUpdatesRequestRequestTypeDef, _OptionalListUpdatesRequestRequestTypeDef
 ):
     pass
 
-ListUpdatesResponseTypeDef = TypedDict(
-    "ListUpdatesResponseTypeDef",
-    {
-        "updateIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 LogSetupOutputTypeDef = TypedDict(
     "LogSetupOutputTypeDef",
     {
         "types": List[LogTypeType],
         "enabled": bool,
     },
@@ -1025,35 +878,14 @@
         "key": str,
         "value": str,
         "effect": TaintEffectType,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1081,19 +913,21 @@
         "resolveConflicts": ResolveConflictsType,
         "clientRequestToken": str,
         "configurationValues": str,
     },
     total=False,
 )
 
+
 class UpdateAddonRequestRequestTypeDef(
     _RequiredUpdateAddonRequestRequestTypeDef, _OptionalUpdateAddonRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateClusterVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterVersionRequestRequestTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
@@ -1101,20 +935,22 @@
     "_OptionalUpdateClusterVersionRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
+
 class UpdateClusterVersionRequestRequestTypeDef(
     _RequiredUpdateClusterVersionRequestRequestTypeDef,
     _OptionalUpdateClusterVersionRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateLabelsPayloadTypeDef = TypedDict(
     "UpdateLabelsPayloadTypeDef",
     {
         "addOrUpdateLabels": Mapping[str, str],
         "removeLabels": Sequence[str],
     },
     total=False,
@@ -1144,14 +980,77 @@
         "architecture": List[str],
         "compatibilities": List[CompatibilityTypeDef],
         "requiresConfiguration": bool,
     },
     total=False,
 )
 
+DescribeAddonConfigurationResponseTypeDef = TypedDict(
+    "DescribeAddonConfigurationResponseTypeDef",
+    {
+        "addonName": str,
+        "addonVersion": str,
+        "configurationSchema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAddonsResponseTypeDef = TypedDict(
+    "ListAddonsResponseTypeDef",
+    {
+        "addons": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListClustersResponseTypeDef = TypedDict(
+    "ListClustersResponseTypeDef",
+    {
+        "clusters": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFargateProfilesResponseTypeDef = TypedDict(
+    "ListFargateProfilesResponseTypeDef",
+    {
+        "fargateProfileNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListNodegroupsResponseTypeDef = TypedDict(
+    "ListNodegroupsResponseTypeDef",
+    {
+        "nodegroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListUpdatesResponseTypeDef = TypedDict(
+    "ListUpdatesResponseTypeDef",
+    {
+        "updateIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredAssociateIdentityProviderConfigRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateIdentityProviderConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "oidc": OidcIdentityProviderConfigRequestTypeDef,
     },
 )
@@ -1160,20 +1059,22 @@
     {
         "tags": Mapping[str, str],
         "clientRequestToken": str,
     },
     total=False,
 )
 
+
 class AssociateIdentityProviderConfigRequestRequestTypeDef(
     _RequiredAssociateIdentityProviderConfigRequestRequestTypeDef,
     _OptionalAssociateIdentityProviderConfigRequestRequestTypeDef,
 ):
     pass
 
+
 NodegroupResourcesTypeDef = TypedDict(
     "NodegroupResourcesTypeDef",
     {
         "autoScalingGroups": List[AutoScalingGroupTypeDef],
         "remoteAccessSecurityGroup": str,
     },
     total=False,
@@ -1199,19 +1100,21 @@
     {
         "clientRequestToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class RegisterClusterRequestRequestTypeDef(
     _RequiredRegisterClusterRequestRequestTypeDef, _OptionalRegisterClusterRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredOutpostConfigRequestTypeDef = TypedDict(
     "_RequiredOutpostConfigRequestTypeDef",
     {
         "outpostArns": Sequence[str],
         "controlPlaneInstanceType": str,
     },
 )
@@ -1219,19 +1122,21 @@
     "_OptionalOutpostConfigRequestTypeDef",
     {
         "controlPlanePlacement": ControlPlanePlacementRequestTypeDef,
     },
     total=False,
 )
 
+
 class OutpostConfigRequestTypeDef(
     _RequiredOutpostConfigRequestTypeDef, _OptionalOutpostConfigRequestTypeDef
 ):
     pass
 
+
 _RequiredOutpostConfigResponseTypeDef = TypedDict(
     "_RequiredOutpostConfigResponseTypeDef",
     {
         "outpostArns": List[str],
         "controlPlaneInstanceType": str,
     },
 )
@@ -1239,19 +1144,21 @@
     "_OptionalOutpostConfigResponseTypeDef",
     {
         "controlPlanePlacement": ControlPlanePlacementResponseTypeDef,
     },
     total=False,
 )
 
+
 class OutpostConfigResponseTypeDef(
     _RequiredOutpostConfigResponseTypeDef, _OptionalOutpostConfigResponseTypeDef
 ):
     pass
 
+
 _RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFargateProfileRequestRequestTypeDef",
     {
         "fargateProfileName": str,
         "clusterName": str,
         "podExecutionRoleArn": str,
     },
@@ -1263,20 +1170,22 @@
         "selectors": Sequence[FargateProfileSelectorTypeDef],
         "clientRequestToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateFargateProfileRequestRequestTypeDef(
     _RequiredCreateFargateProfileRequestRequestTypeDef,
     _OptionalCreateFargateProfileRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateNodegroupVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupVersionRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1288,20 +1197,22 @@
         "launchTemplate": LaunchTemplateSpecificationTypeDef,
         "force": bool,
         "clientRequestToken": str,
     },
     total=False,
 )
 
+
 class UpdateNodegroupVersionRequestRequestTypeDef(
     _RequiredUpdateNodegroupVersionRequestRequestTypeDef,
     _OptionalUpdateNodegroupVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateNodegroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNodegroupRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
         "subnets": Sequence[str],
         "nodeRole": str,
@@ -1324,19 +1235,21 @@
         "capacityType": CapacityTypesType,
         "version": str,
         "releaseVersion": str,
     },
     total=False,
 )
 
+
 class CreateNodegroupRequestRequestTypeDef(
     _RequiredCreateNodegroupRequestRequestTypeDef, _OptionalCreateNodegroupRequestRequestTypeDef
 ):
     pass
 
+
 UpdateTaintsPayloadTypeDef = TypedDict(
     "UpdateTaintsPayloadTypeDef",
     {
         "addOrUpdateTaints": Sequence[TaintTypeDef],
         "removeTaints": Sequence[TaintTypeDef],
     },
     total=False,
@@ -1353,20 +1266,22 @@
     "_OptionalDescribeAddonRequestAddonActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAddonRequestAddonActiveWaitTypeDef(
     _RequiredDescribeAddonRequestAddonActiveWaitTypeDef,
     _OptionalDescribeAddonRequestAddonActiveWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAddonRequestAddonDeletedWaitTypeDef = TypedDict(
     "_RequiredDescribeAddonRequestAddonDeletedWaitTypeDef",
     {
         "clusterName": str,
         "addonName": str,
     },
 )
@@ -1374,60 +1289,66 @@
     "_OptionalDescribeAddonRequestAddonDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAddonRequestAddonDeletedWaitTypeDef(
     _RequiredDescribeAddonRequestAddonDeletedWaitTypeDef,
     _OptionalDescribeAddonRequestAddonDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeClusterRequestClusterActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeClusterRequestClusterActiveWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalDescribeClusterRequestClusterActiveWaitTypeDef = TypedDict(
     "_OptionalDescribeClusterRequestClusterActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeClusterRequestClusterActiveWaitTypeDef(
     _RequiredDescribeClusterRequestClusterActiveWaitTypeDef,
     _OptionalDescribeClusterRequestClusterActiveWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeClusterRequestClusterDeletedWaitTypeDef = TypedDict(
     "_RequiredDescribeClusterRequestClusterDeletedWaitTypeDef",
     {
         "name": str,
     },
 )
 _OptionalDescribeClusterRequestClusterDeletedWaitTypeDef = TypedDict(
     "_OptionalDescribeClusterRequestClusterDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeClusterRequestClusterDeletedWaitTypeDef(
     _RequiredDescribeClusterRequestClusterDeletedWaitTypeDef,
     _OptionalDescribeClusterRequestClusterDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeFargateProfileRequestFargateProfileActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeFargateProfileRequestFargateProfileActiveWaitTypeDef",
     {
         "clusterName": str,
         "fargateProfileName": str,
     },
 )
@@ -1435,20 +1356,22 @@
     "_OptionalDescribeFargateProfileRequestFargateProfileActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef(
     _RequiredDescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
     _OptionalDescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef = TypedDict(
     "_RequiredDescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef",
     {
         "clusterName": str,
         "fargateProfileName": str,
     },
 )
@@ -1456,20 +1379,22 @@
     "_OptionalDescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef(
     _RequiredDescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
     _OptionalDescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeNodegroupRequestNodegroupActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeNodegroupRequestNodegroupActiveWaitTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1477,20 +1402,22 @@
     "_OptionalDescribeNodegroupRequestNodegroupActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeNodegroupRequestNodegroupActiveWaitTypeDef(
     _RequiredDescribeNodegroupRequestNodegroupActiveWaitTypeDef,
     _OptionalDescribeNodegroupRequestNodegroupActiveWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeNodegroupRequestNodegroupDeletedWaitTypeDef = TypedDict(
     "_RequiredDescribeNodegroupRequestNodegroupDeletedWaitTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1498,20 +1425,156 @@
     "_OptionalDescribeNodegroupRequestNodegroupDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeNodegroupRequestNodegroupDeletedWaitTypeDef(
     _RequiredDescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
     _OptionalDescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
 ):
     pass
 
+
+DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef = TypedDict(
+    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+    {
+        "kubernetesVersion": str,
+        "addonName": str,
+        "types": Sequence[str],
+        "publishers": Sequence[str],
+        "owners": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
+    "_RequiredListAddonsRequestListAddonsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
+    "_OptionalListAddonsRequestListAddonsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAddonsRequestListAddonsPaginateTypeDef(
+    _RequiredListAddonsRequestListAddonsPaginateTypeDef,
+    _OptionalListAddonsRequestListAddonsPaginateTypeDef,
+):
+    pass
+
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "include": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
+    "_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
+    "_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFargateProfilesRequestListFargateProfilesPaginateTypeDef(
+    _RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+    _OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef(
+    _RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+    _OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
+    "_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
+    "_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListNodegroupsRequestListNodegroupsPaginateTypeDef(
+    _RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef,
+    _OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
+    "_RequiredListUpdatesRequestListUpdatesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
+    "_OptionalListUpdatesRequestListUpdatesPaginateTypeDef",
+    {
+        "nodegroupName": str,
+        "addonName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUpdatesRequestListUpdatesPaginateTypeDef(
+    _RequiredListUpdatesRequestListUpdatesPaginateTypeDef,
+    _OptionalListUpdatesRequestListUpdatesPaginateTypeDef,
+):
+    pass
+
+
 DescribeIdentityProviderConfigRequestRequestTypeDef = TypedDict(
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "identityProviderConfig": IdentityProviderConfigTypeDef,
     },
 )
@@ -1527,20 +1590,22 @@
     "_OptionalDisassociateIdentityProviderConfigRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
+
 class DisassociateIdentityProviderConfigRequestRequestTypeDef(
     _RequiredDisassociateIdentityProviderConfigRequestRequestTypeDef,
     _OptionalDisassociateIdentityProviderConfigRequestRequestTypeDef,
 ):
     pass
 
+
 EncryptionConfigOutputTypeDef = TypedDict(
     "EncryptionConfigOutputTypeDef",
     {
         "resources": List[str],
         "provider": ProviderOutputTypeDef,
     },
     total=False,
@@ -1572,15 +1637,15 @@
 )
 
 ListIdentityProviderConfigsResponseTypeDef = TypedDict(
     "ListIdentityProviderConfigsResponseTypeDef",
     {
         "identityProviderConfigs": List[IdentityProviderConfigOutputTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IdentityProviderConfigResponseTypeDef = TypedDict(
     "IdentityProviderConfigResponseTypeDef",
     {
         "oidc": OidcIdentityProviderConfigTypeDef,
@@ -1682,20 +1747,22 @@
         "scalingConfig": NodegroupScalingConfigTypeDef,
         "updateConfig": NodegroupUpdateConfigTypeDef,
         "clientRequestToken": str,
     },
     total=False,
 )
 
+
 class UpdateNodegroupConfigRequestRequestTypeDef(
     _RequiredUpdateNodegroupConfigRequestRequestTypeDef,
     _OptionalUpdateNodegroupConfigRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "encryptionConfig": Sequence[EncryptionConfigTypeDef],
     },
 )
@@ -1703,49 +1770,51 @@
     "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
+
 class AssociateEncryptionConfigRequestRequestTypeDef(
     _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
     _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
+
 CreateFargateProfileResponseTypeDef = TypedDict(
     "CreateFargateProfileResponseTypeDef",
     {
         "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFargateProfileResponseTypeDef = TypedDict(
     "DeleteFargateProfileResponseTypeDef",
     {
         "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFargateProfileResponseTypeDef = TypedDict(
     "DescribeFargateProfileResponseTypeDef",
     {
         "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIdentityProviderConfigResponseTypeDef = TypedDict(
     "DescribeIdentityProviderConfigResponseTypeDef",
     {
         "identityProviderConfig": IdentityProviderConfigResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NodegroupTypeDef = TypedDict(
     "NodegroupTypeDef",
     {
         "nodegroupName": str,
@@ -1820,19 +1889,21 @@
         "tags": Mapping[str, str],
         "encryptionConfig": Sequence[EncryptionConfigTypeDef],
         "outpostConfig": OutpostConfigRequestTypeDef,
     },
     total=False,
 )
 
+
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateClusterConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterConfigRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateClusterConfigRequestRequestTypeDef = TypedDict(
@@ -1841,182 +1912,184 @@
         "resourcesVpcConfig": VpcConfigRequestTypeDef,
         "logging": LoggingTypeDef,
         "clientRequestToken": str,
     },
     total=False,
 )
 
+
 class UpdateClusterConfigRequestRequestTypeDef(
     _RequiredUpdateClusterConfigRequestRequestTypeDef,
     _OptionalUpdateClusterConfigRequestRequestTypeDef,
 ):
     pass
 
+
 AssociateEncryptionConfigResponseTypeDef = TypedDict(
     "AssociateEncryptionConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateIdentityProviderConfigResponseTypeDef = TypedDict(
     "AssociateIdentityProviderConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUpdateResponseTypeDef = TypedDict(
     "DescribeUpdateResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateIdentityProviderConfigResponseTypeDef = TypedDict(
     "DisassociateIdentityProviderConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAddonResponseTypeDef = TypedDict(
     "UpdateAddonResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterConfigResponseTypeDef = TypedDict(
     "UpdateClusterConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterVersionResponseTypeDef = TypedDict(
     "UpdateClusterVersionResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNodegroupConfigResponseTypeDef = TypedDict(
     "UpdateNodegroupConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNodegroupVersionResponseTypeDef = TypedDict(
     "UpdateNodegroupVersionResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAddonResponseTypeDef = TypedDict(
     "CreateAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAddonResponseTypeDef = TypedDict(
     "DeleteAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAddonResponseTypeDef = TypedDict(
     "DescribeAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAddonVersionsResponseTypeDef = TypedDict(
     "DescribeAddonVersionsResponseTypeDef",
     {
         "addons": List[AddonInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateNodegroupResponseTypeDef = TypedDict(
     "CreateNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteNodegroupResponseTypeDef = TypedDict(
     "DeleteNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNodegroupResponseTypeDef = TypedDict(
     "DescribeNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeregisterClusterResponseTypeDef = TypedDict(
     "DeregisterClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterClusterResponseTypeDef = TypedDict(
     "RegisterClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-eks-1.28.12/mypy_boto3_eks/waiter.py` & `mypy-boto3-eks-1.28.13/mypy_boto3_eks/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.12/mypy_boto3_eks/waiter.pyi` & `mypy-boto3-eks-1.28.13/mypy_boto3_eks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/PKG-INFO` & `mypy-boto3-eks-1.28.13/mypy_boto3_eks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-eks
-Version: 1.28.12
-Summary: Type annotations for boto3.EKS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.13
+Summary: Type annotations for boto3.EKS 1.28.13 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-eks.svg?color=blue)](https://pypi.org/project/mypy-boto3-eks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_eks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-eks)](https://pepy.tech/project/mypy-boto3-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EKS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[boto3.EKS 1.28.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -414,14 +414,15 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_eks.type_defs import (
     AddonIssueTypeDef,
     MarketplaceInformationTypeDef,
     CompatibilityTypeDef,
+    ResponseMetadataTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     AutoScalingGroupTypeDef,
     CertificateTypeDef,
     ClusterIssueTypeDef,
     ConnectorConfigResponseTypeDef,
     KubernetesNetworkConfigResponseTypeDef,
     VpcConfigResponseTypeDef,
@@ -439,18 +440,17 @@
     TaintTypeDef,
     DeleteAddonRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteFargateProfileRequestRequestTypeDef,
     DeleteNodegroupRequestRequestTypeDef,
     DeregisterClusterRequestRequestTypeDef,
     DescribeAddonConfigurationRequestRequestTypeDef,
-    DescribeAddonConfigurationResponseTypeDef,
     WaiterConfigTypeDef,
     DescribeAddonRequestRequestTypeDef,
-    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAddonVersionsRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
     ProviderOutputTypeDef,
@@ -458,49 +458,42 @@
     ErrorDetailTypeDef,
     FargateProfileSelectorOutputTypeDef,
     IdentityProviderConfigOutputTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
     LaunchTemplateSpecificationOutputTypeDef,
-    ListAddonsRequestListAddonsPaginateTypeDef,
     ListAddonsRequestRequestTypeDef,
-    ListAddonsResponseTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListClustersResponseTypeDef,
-    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
     ListFargateProfilesRequestRequestTypeDef,
-    ListFargateProfilesResponseTypeDef,
-    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
     ListIdentityProviderConfigsRequestRequestTypeDef,
-    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
     ListNodegroupsRequestRequestTypeDef,
-    ListNodegroupsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUpdatesRequestListUpdatesPaginateTypeDef,
     ListUpdatesRequestRequestTypeDef,
-    ListUpdatesResponseTypeDef,
     LogSetupOutputTypeDef,
     LogSetupTypeDef,
     NodegroupScalingConfigOutputTypeDef,
     NodegroupUpdateConfigOutputTypeDef,
     RemoteAccessConfigOutputTypeDef,
     TaintOutputTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddonRequestRequestTypeDef,
     UpdateClusterVersionRequestRequestTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateParamTypeDef,
     AddonHealthTypeDef,
     AddonVersionInfoTypeDef,
+    DescribeAddonConfigurationResponseTypeDef,
+    ListAddonsResponseTypeDef,
+    ListClustersResponseTypeDef,
+    ListFargateProfilesResponseTypeDef,
+    ListNodegroupsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUpdatesResponseTypeDef,
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
     CreateFargateProfileRequestRequestTypeDef,
@@ -511,14 +504,21 @@
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
     DescribeNodegroupRequestNodegroupActiveWaitTypeDef,
     DescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
+    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
+    ListAddonsRequestListAddonsPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
+    ListUpdatesRequestListUpdatesPaginateTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
     EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     FargateProfileTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     IdentityProviderConfigResponseTypeDef,
```

### Comparing `mypy-boto3-eks-1.28.12/mypy_boto3_eks.egg-info/SOURCES.txt` & `mypy-boto3-eks-1.28.13/mypy_boto3_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-eks-1.28.12/setup.py` & `mypy-boto3-eks-1.28.13/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-eks",
-    version="1.28.12",
+    version="1.28.13",
     packages=["mypy_boto3_eks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EKS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.EKS 1.28.13 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

