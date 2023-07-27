# Comparing `tmp/alibabacloud_resourcemanager20200331-2.1.5.tar.gz` & `tmp/alibabacloud_resourcemanager20200331-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcemanager20200331-2.1.5.tar", last modified: Mon Jun  5 05:47:02 2023, max compression
+gzip compressed data, was "dist/alibabacloud_resourcemanager20200331-2.1.6.tar", last modified: Thu Jul 27 03:04:34 2023, max compression
```

## Comparing `alibabacloud_resourcemanager20200331-2.1.5.tar` & `alibabacloud_resourcemanager20200331-2.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:47:02.000000 alibabacloud_resourcemanager20200331-2.1.5/
--rw-r--r--   0 root         (0) root         (0)      961 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2400 2023-06-05 05:47:02.000000 alibabacloud_resourcemanager20200331-2.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1058 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1143 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:47:02.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331/__init__.py
--rw-r--r--   0 root         (0) root         (0)   387119 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331/client.py
--rw-r--r--   0 root         (0) root         (0)   589797 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:47:02.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2400 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      516 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-05 05:47:02.000000 alibabacloud_resourcemanager20200331-2.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2670 2023-06-05 05:47:01.000000 alibabacloud_resourcemanager20200331-2.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/alibabacloud_resourcemanager20200331/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/alibabacloud_resourcemanager20200331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   387359 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/alibabacloud_resourcemanager20200331/client.py
+-rw-r--r--   0 root         (0) root         (0)   591427 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/alibabacloud_resourcemanager20200331/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/alibabacloud_resourcemanager20200331.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/alibabacloud_resourcemanager20200331.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/alibabacloud_resourcemanager20200331.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/alibabacloud_resourcemanager20200331.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/alibabacloud_resourcemanager20200331.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/alibabacloud_resourcemanager20200331.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2671 2023-07-27 03:04:34.000000 alibabacloud_resourcemanager20200331-2.1.6/setup.py
```

### Comparing `alibabacloud_resourcemanager20200331-2.1.5/ChangeLog.md` & `alibabacloud_resourcemanager20200331-2.1.6/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-06-05 Version: 2.1.5
+- Modify endpoint for resourcemanager.
+
 2023-05-18 Version: 2.1.4
 - Supported more language for resourcemanager.
 
 2023-02-22 Version: 2.1.3
 - Supported more language for resourcemanager.
 
 2022-12-01 Version: 2.1.2
```

### Comparing `alibabacloud_resourcemanager20200331-2.1.5/LICENSE` & `alibabacloud_resourcemanager20200331-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331-2.1.5/PKG-INFO` & `alibabacloud_resourcemanager20200331-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_resourcemanager20200331
-Version: 2.1.5
+Version: 2.1.6
 Summary: Alibaba Cloud ResourceManager (20200331) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcemanager20200331-2.1.5/README-CN.md` & `alibabacloud_resourcemanager20200331-2.1.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331-2.1.5/README.md` & `alibabacloud_resourcemanager20200331-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331/client.py` & `alibabacloud_resourcemanager20200331-2.1.6/alibabacloud_resourcemanager20200331/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6042,14 +6042,16 @@
             query['Region'] = request.region
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.resource_types):
+            query['ResourceTypes'] = request.resource_types
         if not UtilClient.is_unset(request.service):
             query['Service'] = request.service
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListResources',
@@ -6090,14 +6092,16 @@
             query['Region'] = request.region
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.resource_types):
+            query['ResourceTypes'] = request.resource_types
         if not UtilClient.is_unset(request.service):
             query['Service'] = request.service
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListResources',
```

### Comparing `alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331/models.py` & `alibabacloud_resourcemanager20200331-2.1.6/alibabacloud_resourcemanager20200331/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -12783,23 +12783,57 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListResourceGroupsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListResourcesRequestResourceTypes(TeaModel):
+    def __init__(
+        self,
+        resource_type: str = None,
+        service: str = None,
+    ):
+        self.resource_type = resource_type
+        self.service = service
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        if self.service is not None:
+            result['Service'] = self.service
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        if m.get('Service') is not None:
+            self.service = m.get('Service')
+        return self
+
+
 class ListResourcesRequest(TeaModel):
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         region: str = None,
         resource_group_id: str = None,
         resource_id: str = None,
         resource_type: str = None,
+        resource_types: List[ListResourcesRequestResourceTypes] = None,
         service: str = None,
     ):
         # The number of the page to return.
         # 
         # Pages start from page 1. Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page.
@@ -12812,21 +12846,25 @@
         self.resource_group_id = resource_group_id
         # The ID of the resource.
         self.resource_id = resource_id
         # The resource type.
         # 
         # For more information about the supported resource types, see the **Resource type** column in [Alibaba Cloud services that support resource groups](~~94479~~).
         self.resource_type = resource_type
+        self.resource_types = resource_types
         # The ID of the Alibaba Cloud service.
         # 
         # You can obtain the ID from the **Service code** column in [Alibaba Cloud services that support resource groups](~~94479~~).
         self.service = service
 
     def validate(self):
-        pass
+        if self.resource_types:
+            for k in self.resource_types:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -12838,14 +12876,18 @@
             result['Region'] = self.region
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         if self.resource_id is not None:
             result['ResourceId'] = self.resource_id
         if self.resource_type is not None:
             result['ResourceType'] = self.resource_type
+        result['ResourceTypes'] = []
+        if self.resource_types is not None:
+            for k in self.resource_types:
+                result['ResourceTypes'].append(k.to_map() if k else None)
         if self.service is not None:
             result['Service'] = self.service
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('PageNumber') is not None:
@@ -12856,14 +12898,19 @@
             self.region = m.get('Region')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('ResourceId') is not None:
             self.resource_id = m.get('ResourceId')
         if m.get('ResourceType') is not None:
             self.resource_type = m.get('ResourceType')
+        self.resource_types = []
+        if m.get('ResourceTypes') is not None:
+            for k in m.get('ResourceTypes'):
+                temp_model = ListResourcesRequestResourceTypes()
+                self.resource_types.append(temp_model.from_map(k))
         if m.get('Service') is not None:
             self.service = m.get('Service')
         return self
 
 
 class ListResourcesResponseBodyResourcesResource(TeaModel):
     def __init__(
@@ -16316,22 +16363,24 @@
 class TagResourcesRequest(TeaModel):
     def __init__(
         self,
         resource_id: List[str] = None,
         resource_type: str = None,
         tag: List[TagResourcesRequestTag] = None,
     ):
+        # The ID of a resource group or member.
         self.resource_id = resource_id
         # The type of the objects to which you want to add tags. Valid values:
         # 
         # *   ResourceGroup : resource group. This is the default value.
         # *   Account: member.
         # 
         # >  This parameter is required if you add tags to members in a resource directory.
         self.resource_type = resource_type
+        # The tags.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
```

### Comparing `alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/PKG-INFO` & `alibabacloud_resourcemanager20200331-2.1.6/alibabacloud_resourcemanager20200331.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-resourcemanager20200331
-Version: 2.1.5
+Version: 2.1.6
 Summary: Alibaba Cloud ResourceManager (20200331) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcemanager20200331-2.1.5/alibabacloud_resourcemanager20200331.egg-info/SOURCES.txt` & `alibabacloud_resourcemanager20200331-2.1.6/alibabacloud_resourcemanager20200331.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331-2.1.5/setup.py` & `alibabacloud_resourcemanager20200331-2.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcemanager20200331.
 
-Created on 05/06/2023
+Created on 27/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcemanager20200331"
 NAME = "alibabacloud_resourcemanager20200331" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceManager (20200331) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

