# Comparing `tmp/aliyun-python-sdk-resourcemanager-1.2.5.tar.gz` & `tmp/aliyun-python-sdk-resourcemanager-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-resourcemanager-1.2.5.tar", last modified: Thu Jun  8 10:02:37 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-resourcemanager-1.2.6.tar", last modified: Thu Jul 27 03:06:57 2023, max compression
```

## Comparing `aliyun-python-sdk-resourcemanager-1.2.5.tar` & `aliyun-python-sdk-resourcemanager-1.2.6.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1597 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1597 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7198 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/
--rw-r--r--   0 root         (0) root         (0)     1540 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/AcceptHandshakeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/AttachControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2358 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/AttachPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2000 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/BindSecureMobilePhoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     1546 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelChangeAccountEmailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelCreateCloudAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelHandshakeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1548 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelPromoteResourceAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ChangeAccountEmailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CheckAccountDeleteRequest.py
--rw-r--r--   0 root         (0) root         (0)     2137 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateCloudAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2151 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1743 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateFolderRequest.py
--rw-r--r--   0 root         (0) root         (0)     1940 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreatePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1962 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreatePolicyVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2842 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateResourceAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1703 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2219 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1956 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateServiceLinkedRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeclineHandshakeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1785 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteFolderRequest.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeletePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeletePolicyVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1572 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1503 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteServiceLinkedRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1754 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeregisterDelegatedAdministratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1361 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DestroyResourceDirectoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DetachControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2358 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DetachPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DisableControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1351 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/EnableControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/EnableResourceDirectoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1556 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionCheckResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1546 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1717 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1377 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyEnablementStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1703 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetFolderRequest.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetHandshakeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetPayerForAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetPolicyVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetResourceDirectoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1765 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1561 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetServiceLinkedRoleDeletionStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1355 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/InitResourceDirectoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2320 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/InviteAccountToResourceDirectoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2740 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListAccountsForParentRequest.py
--rw-r--r--   0 root         (0) root         (0)     2304 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListAccountsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListAncestorsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListControlPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListControlPolicyAttachmentsForTargetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1921 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListDelegatedAdministratorsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListDelegatedServicesForAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2145 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListFoldersForParentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1755 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForResourceDirectoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2081 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2929 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListPolicyAttachmentsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListPolicyVersionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3345 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListResourceGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1884 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListRolesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2101 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTagKeysRequest.py
--rw-r--r--   0 root         (0) root         (0)     2573 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2284 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTagValuesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1940 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTargetAttachmentsForControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTrustedServiceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1765 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/MoveAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2278 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/MoveResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1703 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/PromoteResourceAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1750 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/RegisterDelegatedAdministratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/RemoveCloudAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1550 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ResendCreateCloudAccountEmailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1558 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ResendPromoteResourceAccountEmailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1544 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/RetryChangeAccountEmailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForBindSecureMobilePhoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     1608 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForEnableRDRequest.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SetDefaultPolicyVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SetMemberDeletionPermissionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2187 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2187 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateFolderRequest.py
--rw-r--r--   0 root         (0) root         (0)     1787 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2512 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      551 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyun_python_sdk_resourcemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyun_python_sdk_resourcemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7198 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyun_python_sdk_resourcemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyun_python_sdk_resourcemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyun_python_sdk_resourcemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyun_python_sdk_resourcemanager.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/AcceptHandshakeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/AttachControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/AttachPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/BindSecureMobilePhoneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CancelChangeAccountEmailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CancelCreateCloudAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CancelHandshakeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CancelPromoteResourceAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ChangeAccountEmailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CheckAccountDeleteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreateCloudAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreateControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreateFolderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreatePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreatePolicyVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreateResourceAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreateResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreateRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreateServiceLinkedRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeclineHandshakeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeleteAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeleteControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeleteFolderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeletePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeletePolicyVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeleteResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeleteRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeleteServiceLinkedRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeregisterDelegatedAdministratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1343 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DestroyResourceDirectoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DetachControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DetachPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DisableControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/EnableControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/EnableResourceDirectoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionCheckResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyEnablementStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetFolderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetHandshakeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetPayerForAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetPolicyVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetResourceDirectoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetServiceLinkedRoleDeletionStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1337 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/InitResourceDirectoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/InviteAccountToResourceDirectoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2722 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListAccountsForParentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListAccountsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListAncestorsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListControlPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListControlPolicyAttachmentsForTargetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListDelegatedAdministratorsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListDelegatedServicesForAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListFoldersForParentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForResourceDirectoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2063 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListPolicyAttachmentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListPolicyVersionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3327 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListResourceGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListRolesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListTagKeysRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2555 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListTagValuesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListTargetAttachmentsForControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListTrustedServiceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/MoveAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/MoveResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/PromoteResourceAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/RegisterDelegatedAdministratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/RemoveCloudAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ResendCreateCloudAccountEmailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ResendPromoteResourceAccountEmailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/RetryChangeAccountEmailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForBindSecureMobilePhoneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForEnableRDRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/SetDefaultPolicyVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/SetMemberDeletionPermissionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/UpdateAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/UpdateControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/UpdateFolderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/UpdateResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/UpdateRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2512 2023-07-27 03:06:57.000000 aliyun-python-sdk-resourcemanager-1.2.6/setup.py
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/LICENSE` & `aliyun-python-sdk-resourcemanager-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/PKG-INFO` & `aliyun-python-sdk-resourcemanager-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-resourcemanager
-Version: 1.2.5
+Version: 1.2.6
 Summary: The resourcemanager module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-resourcemanager
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/README.rst` & `aliyun-python-sdk-resourcemanager-1.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/PKG-INFO` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyun_python_sdk_resourcemanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-resourcemanager
-Version: 1.2.5
+Version: 1.2.6
 Summary: The resourcemanager module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-resourcemanager
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/SOURCES.txt` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyun_python_sdk_resourcemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/endpoint.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/AcceptHandshakeRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/AcceptHandshakeRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class AcceptHandshakeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'AcceptHandshake','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'AcceptHandshake')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/AttachControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/AttachControlPolicyRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class AttachControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'AttachControlPolicy','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'AttachControlPolicy')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/AttachPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/AttachPolicyRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class AttachPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'AttachPolicy','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'AttachPolicy')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/BindSecureMobilePhoneRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/BindSecureMobilePhoneRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class BindSecureMobilePhoneRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'BindSecureMobilePhone','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'BindSecureMobilePhone')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelChangeAccountEmailRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ChangeAccountEmailRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class CancelChangeAccountEmailRequest(RpcRequest):
+class ChangeAccountEmailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelChangeAccountEmail','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ChangeAccountEmail')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_AccountId(self): # String
 		return self.get_query_params().get('AccountId')
 
 	def set_AccountId(self, AccountId):  # String
 		self.add_query_param('AccountId', AccountId)
+	def get_Email(self): # String
+		return self.get_query_params().get('Email')
+
+	def set_Email(self, Email):  # String
+		self.add_query_param('Email', Email)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelCreateCloudAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CancelCreateCloudAccountRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CancelCreateCloudAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelCreateCloudAccount','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelCreateCloudAccount')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelHandshakeRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CancelHandshakeRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CancelHandshakeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelHandshake','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelHandshake')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelPromoteResourceAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ResendPromoteResourceAccountEmailRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class CancelPromoteResourceAccountRequest(RpcRequest):
+class ResendPromoteResourceAccountEmailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelPromoteResourceAccount','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ResendPromoteResourceAccountEmail')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ChangeAccountEmailRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetPayerForAccountRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,29 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class ChangeAccountEmailRequest(RpcRequest):
+class GetPayerForAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ChangeAccountEmail','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetPayerForAccount')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_AccountId(self): # String
 		return self.get_query_params().get('AccountId')
 
 	def set_AccountId(self, AccountId):  # String
 		self.add_query_param('AccountId', AccountId)
-	def get_Email(self): # String
-		return self.get_query_params().get('Email')
-
-	def set_Email(self, Email):  # String
-		self.add_query_param('Email', Email)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CheckAccountDeleteRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CheckAccountDeleteRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CheckAccountDeleteRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CheckAccountDelete','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CheckAccountDelete')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateCloudAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreateCloudAccountRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreateCloudAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateCloudAccount','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateCloudAccount')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreateControlPolicyRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreateControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateControlPolicy','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateControlPolicy')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateFolderRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreateFolderRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreateFolderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateFolder','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateFolder')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreatePolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreatePolicyRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreatePolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreatePolicy','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreatePolicy')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreatePolicyVersionRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreatePolicyVersionRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreatePolicyVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreatePolicyVersion','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreatePolicyVersion')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateResourceAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreateResourceAccountRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreateResourceAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateResourceAccount','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateResourceAccount')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateResourceGroupRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreateResourceGroupRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreateResourceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateResourceGroup','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateResourceGroup')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateRoleRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreateRoleRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreateRoleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateRole','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateRole')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateServiceLinkedRoleRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CreateServiceLinkedRoleRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreateServiceLinkedRoleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateServiceLinkedRole','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateServiceLinkedRole')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeclineHandshakeRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeclineHandshakeRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DeclineHandshakeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeclineHandshake','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeclineHandshake')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeleteAccountRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 import json
 
 class DeleteAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteAccount','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteAccount')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeleteControlPolicyRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DeleteControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteControlPolicy','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteControlPolicy')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteFolderRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetFolderRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class DeleteFolderRequest(RpcRequest):
+class GetFolderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteFolder','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetFolder')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeletePolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeletePolicyRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DeletePolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeletePolicy','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeletePolicy')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeletePolicyVersionRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/SetDefaultPolicyVersionRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class DeletePolicyVersionRequest(RpcRequest):
+class SetDefaultPolicyVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeletePolicyVersion','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SetDefaultPolicyVersion')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteResourceGroupRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeleteResourceGroupRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DeleteResourceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteResourceGroup','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteResourceGroup')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteRoleRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeleteRoleRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DeleteRoleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteRole','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteRole')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteServiceLinkedRoleRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeleteServiceLinkedRoleRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DeleteServiceLinkedRoleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteServiceLinkedRole','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteServiceLinkedRole')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeregisterDelegatedAdministratorRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeregisterDelegatedAdministratorRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DeregisterDelegatedAdministratorRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeregisterDelegatedAdministrator','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeregisterDelegatedAdministrator')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DestroyResourceDirectoryRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DestroyResourceDirectoryRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DestroyResourceDirectoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DestroyResourceDirectory','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DestroyResourceDirectory')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DetachControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DetachControlPolicyRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DetachControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DetachControlPolicy','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DetachControlPolicy')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DetachPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DetachPolicyRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DetachPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DetachPolicy','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DetachPolicy')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DisableControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DisableControlPolicyRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DisableControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DisableControlPolicy','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DisableControlPolicy')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/EnableControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/EnableControlPolicyRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class EnableControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'EnableControlPolicy','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'EnableControlPolicy')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/EnableResourceDirectoryRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/EnableResourceDirectoryRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class EnableResourceDirectoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'EnableResourceDirectory','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'EnableResourceDirectory')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionCheckResultRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionCheckResultRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetAccountDeletionCheckResultRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetAccountDeletionCheckResult','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetAccountDeletionCheckResult')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionStatusRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionStatusRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetAccountDeletionStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetAccountDeletionStatus','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetAccountDeletionStatus')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetAccountRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetAccount','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetAccount')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyEnablementStatusRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyEnablementStatusRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetControlPolicyEnablementStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetControlPolicyEnablementStatus','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetControlPolicyEnablementStatus')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetControlPolicy','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetControlPolicy')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetFolderRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeleteFolderRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class GetFolderRequest(RpcRequest):
+class DeleteFolderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetFolder','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteFolder')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetHandshakeRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetHandshakeRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetHandshakeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetHandshake','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetHandshake')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetPayerForAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/PromoteResourceAccountRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class GetPayerForAccountRequest(RpcRequest):
+class PromoteResourceAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetPayerForAccount','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'PromoteResourceAccount')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_AccountId(self): # String
 		return self.get_query_params().get('AccountId')
 
 	def set_AccountId(self, AccountId):  # String
 		self.add_query_param('AccountId', AccountId)
+	def get_Email(self): # String
+		return self.get_query_params().get('Email')
+
+	def set_Email(self, Email):  # String
+		self.add_query_param('Email', Email)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetPolicyRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetPolicy','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetPolicy')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetPolicyVersionRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListPolicyVersionsRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,34 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class GetPolicyVersionRequest(RpcRequest):
+class ListPolicyVersionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetPolicyVersion','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListPolicyVersions')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_PolicyType(self): # String
 		return self.get_query_params().get('PolicyType')
 
 	def set_PolicyType(self, PolicyType):  # String
 		self.add_query_param('PolicyType', PolicyType)
-	def get_VersionId(self): # String
-		return self.get_query_params().get('VersionId')
-
-	def set_VersionId(self, VersionId):  # String
-		self.add_query_param('VersionId', VersionId)
 	def get_PolicyName(self): # String
 		return self.get_query_params().get('PolicyName')
 
 	def set_PolicyName(self, PolicyName):  # String
 		self.add_query_param('PolicyName', PolicyName)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetResourceDirectoryRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetResourceDirectoryRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetResourceDirectoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetResourceDirectory','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetResourceDirectory')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetResourceGroupRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetResourceGroupRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetResourceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetResourceGroup','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetResourceGroup')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetRoleRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListControlPolicyAttachmentsForTargetRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class GetRoleRequest(RpcRequest):
+class ListControlPolicyAttachmentsForTargetRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetRole','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListControlPolicyAttachmentsForTarget')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_RoleName(self): # String
-		return self.get_query_params().get('RoleName')
+	def get_TargetId(self): # String
+		return self.get_query_params().get('TargetId')
 
-	def set_RoleName(self, RoleName):  # String
-		self.add_query_param('RoleName', RoleName)
+	def set_TargetId(self, TargetId):  # String
+		self.add_query_param('TargetId', TargetId)
 	def get_Language(self): # String
 		return self.get_query_params().get('Language')
 
 	def set_Language(self, Language):  # String
 		self.add_query_param('Language', Language)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetServiceLinkedRoleDeletionStatusRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetServiceLinkedRoleDeletionStatusRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetServiceLinkedRoleDeletionStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetServiceLinkedRoleDeletionStatus','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetServiceLinkedRoleDeletionStatus')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/InitResourceDirectoryRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/InitResourceDirectoryRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class InitResourceDirectoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'InitResourceDirectory','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'InitResourceDirectory')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/InviteAccountToResourceDirectoryRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/InviteAccountToResourceDirectoryRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class InviteAccountToResourceDirectoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'InviteAccountToResourceDirectory','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'InviteAccountToResourceDirectory')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListAccountsForParentRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListAccountsForParentRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListAccountsForParentRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListAccountsForParent','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListAccountsForParent')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListAccountsRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListAccountsRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListAccountsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListAccounts','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListAccounts')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListAncestorsRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListAncestorsRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListAncestorsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListAncestors','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListAncestors')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListControlPoliciesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListPoliciesRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class ListControlPoliciesRequest(RpcRequest):
+class ListPoliciesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListControlPolicies','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListPolicies')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListControlPolicyAttachmentsForTargetRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetRoleRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class ListControlPolicyAttachmentsForTargetRequest(RpcRequest):
+class GetRoleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListControlPolicyAttachmentsForTarget','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetRole')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_TargetId(self): # String
-		return self.get_query_params().get('TargetId')
+	def get_RoleName(self): # String
+		return self.get_query_params().get('RoleName')
 
-	def set_TargetId(self, TargetId):  # String
-		self.add_query_param('TargetId', TargetId)
+	def set_RoleName(self, RoleName):  # String
+		self.add_query_param('RoleName', RoleName)
 	def get_Language(self): # String
 		return self.get_query_params().get('Language')
 
 	def set_Language(self, Language):  # String
 		self.add_query_param('Language', Language)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListDelegatedAdministratorsRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListDelegatedAdministratorsRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListDelegatedAdministratorsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListDelegatedAdministrators','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListDelegatedAdministrators')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListDelegatedServicesForAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/RemoveCloudAccountRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class ListDelegatedServicesForAccountRequest(RpcRequest):
+class RemoveCloudAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListDelegatedServicesForAccount','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'RemoveCloudAccount')
+		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListFoldersForParentRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListFoldersForParentRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListFoldersForParentRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListFoldersForParent','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListFoldersForParent')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForAccountRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListHandshakesForAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListHandshakesForAccount','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListHandshakesForAccount')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForResourceDirectoryRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForResourceDirectoryRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListHandshakesForResourceDirectoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListHandshakesForResourceDirectory','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListHandshakesForResourceDirectory')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListPoliciesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListControlPoliciesRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class ListPoliciesRequest(RpcRequest):
+class ListControlPoliciesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListPolicies','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListControlPolicies')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListPolicyAttachmentsRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListPolicyAttachmentsRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListPolicyAttachmentsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListPolicyAttachments','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListPolicyAttachments')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListPolicyVersionsRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/GetPolicyVersionRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,29 +16,34 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class ListPolicyVersionsRequest(RpcRequest):
+class GetPolicyVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListPolicyVersions','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetPolicyVersion')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_PolicyType(self): # String
 		return self.get_query_params().get('PolicyType')
 
 	def set_PolicyType(self, PolicyType):  # String
 		self.add_query_param('PolicyType', PolicyType)
+	def get_VersionId(self): # String
+		return self.get_query_params().get('VersionId')
+
+	def set_VersionId(self, VersionId):  # String
+		self.add_query_param('VersionId', VersionId)
 	def get_PolicyName(self): # String
 		return self.get_query_params().get('PolicyName')
 
 	def set_PolicyName(self, PolicyName):  # String
 		self.add_query_param('PolicyName', PolicyName)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListResourceGroupsRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListResourceGroupsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListResourceGroupsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListResourceGroups','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListResourceGroups')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListResourcesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListResourcesRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListResources','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListResources')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
@@ -48,14 +48,23 @@
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_query_param('PageSize', PageSize)
 	def get_ResourceId(self): # String
 		return self.get_query_params().get('ResourceId')
 
 	def set_ResourceId(self, ResourceId):  # String
 		self.add_query_param('ResourceId', ResourceId)
+	def get_ResourceTypes(self): # Array
+		return self.get_query_params().get('ResourceTypes')
+
+	def set_ResourceTypes(self, ResourceTypes):  # Array
+		for index1, value1 in enumerate(ResourceTypes):
+			if value1.get('Service') is not None:
+				self.add_query_param('ResourceTypes.' + str(index1 + 1) + '.Service', value1.get('Service'))
+			if value1.get('ResourceType') is not None:
+				self.add_query_param('ResourceTypes.' + str(index1 + 1) + '.ResourceType', value1.get('ResourceType'))
 	def get_ResourceType(self): # String
 		return self.get_query_params().get('ResourceType')
 
 	def set_ResourceType(self, ResourceType):  # String
 		self.add_query_param('ResourceType', ResourceType)
 	def get_Service(self): # String
 		return self.get_query_params().get('Service')
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListRolesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListRolesRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListRolesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListRoles','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListRoles')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTagKeysRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListTagKeysRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListTagKeysRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTagKeys','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTagKeys')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTagResourcesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListTagResourcesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListTagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTagResources','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTagResources')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTagValuesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListTagValuesRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListTagValuesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTagValues','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTagValues')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTargetAttachmentsForControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListTargetAttachmentsForControlPolicyRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListTargetAttachmentsForControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTargetAttachmentsForControlPolicy','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTargetAttachmentsForControlPolicy')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTrustedServiceStatusRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListTrustedServiceStatusRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListTrustedServiceStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTrustedServiceStatus','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTrustedServiceStatus')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/MoveAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/MoveAccountRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class MoveAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'MoveAccount','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'MoveAccount')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/MoveResourcesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/MoveResourcesRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class MoveResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'MoveResources','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'MoveResources')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/PromoteResourceAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/RetryChangeAccountEmailRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,29 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class PromoteResourceAccountRequest(RpcRequest):
+class RetryChangeAccountEmailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'PromoteResourceAccount','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'RetryChangeAccountEmail')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_AccountId(self): # String
 		return self.get_query_params().get('AccountId')
 
 	def set_AccountId(self, AccountId):  # String
 		self.add_query_param('AccountId', AccountId)
-	def get_Email(self): # String
-		return self.get_query_params().get('Email')
-
-	def set_Email(self, Email):  # String
-		self.add_query_param('Email', Email)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/RegisterDelegatedAdministratorRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/RegisterDelegatedAdministratorRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class RegisterDelegatedAdministratorRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'RegisterDelegatedAdministrator','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'RegisterDelegatedAdministrator')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/RemoveCloudAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ResendCreateCloudAccountEmailRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class RemoveCloudAccountRequest(RpcRequest):
+class ResendCreateCloudAccountEmailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'RemoveCloudAccount','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ResendCreateCloudAccountEmail')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_AccountId(self): # String
-		return self.get_query_params().get('AccountId')
+	def get_RecordId(self): # String
+		return self.get_query_params().get('RecordId')
 
-	def set_AccountId(self, AccountId):  # String
-		self.add_query_param('AccountId', AccountId)
+	def set_RecordId(self, RecordId):  # String
+		self.add_query_param('RecordId', RecordId)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ResendCreateCloudAccountEmailRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/ListDelegatedServicesForAccountRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,24 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class ResendCreateCloudAccountEmailRequest(RpcRequest):
+class ListDelegatedServicesForAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ResendCreateCloudAccountEmail','resourcemanager')
-		self.set_protocol_type('https')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListDelegatedServicesForAccount')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_RecordId(self): # String
-		return self.get_query_params().get('RecordId')
+	def get_AccountId(self): # String
+		return self.get_query_params().get('AccountId')
 
-	def set_RecordId(self, RecordId):  # String
-		self.add_query_param('RecordId', RecordId)
+	def set_AccountId(self, AccountId):  # String
+		self.add_query_param('AccountId', AccountId)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ResendPromoteResourceAccountEmailRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CancelPromoteResourceAccountRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class ResendPromoteResourceAccountEmailRequest(RpcRequest):
+class CancelPromoteResourceAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ResendPromoteResourceAccountEmail','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelPromoteResourceAccount')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/RetryChangeAccountEmailRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/CancelChangeAccountEmailRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class RetryChangeAccountEmailRequest(RpcRequest):
+class CancelChangeAccountEmailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'RetryChangeAccountEmail','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelChangeAccountEmail')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForBindSecureMobilePhoneRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForBindSecureMobilePhoneRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class SendVerificationCodeForBindSecureMobilePhoneRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SendVerificationCodeForBindSecureMobilePhone','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SendVerificationCodeForBindSecureMobilePhone')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForEnableRDRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForEnableRDRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class SendVerificationCodeForEnableRDRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SendVerificationCodeForEnableRD','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SendVerificationCodeForEnableRD')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SetDefaultPolicyVersionRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/DeletePolicyVersionRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class SetDefaultPolicyVersionRequest(RpcRequest):
+class DeletePolicyVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SetDefaultPolicyVersion','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeletePolicyVersion')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SetMemberDeletionPermissionRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/SetMemberDeletionPermissionRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class SetMemberDeletionPermissionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SetMemberDeletionPermission','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SetMemberDeletionPermission')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/TagResourcesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/TagResourcesRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class TagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'TagResources','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'TagResources')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UntagResourcesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/UntagResourcesRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class UntagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UntagResources','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UntagResources')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/UpdateAccountRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class UpdateAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateAccount','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateAccount')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/UpdateControlPolicyRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class UpdateControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateControlPolicy','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateControlPolicy')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateFolderRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/UpdateFolderRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class UpdateFolderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateFolder','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateFolder')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateResourceGroupRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/UpdateResourceGroupRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class UpdateResourceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateResourceGroup','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateResourceGroup')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateRoleRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.6/aliyunsdkresourcemanager/request/v20200331/UpdateRoleRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class UpdateRoleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateRole','resourcemanager')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateRole')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.5/setup.py` & `aliyun-python-sdk-resourcemanager-1.2.6/setup.py`

 * *Files identical despite different names*

