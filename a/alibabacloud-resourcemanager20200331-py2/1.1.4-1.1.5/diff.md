# Comparing `tmp/alibabacloud_resourcemanager20200331_py2-1.1.4.tar.gz` & `tmp/alibabacloud_resourcemanager20200331_py2-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcemanager20200331_py2-1.1.4.tar", last modified: Mon Jun  5 05:46:26 2023, max compression
+gzip compressed data, was "dist/alibabacloud_resourcemanager20200331_py2-1.1.5.tar", last modified: Thu Jul 27 03:04:05 2023, max compression
```

## Comparing `alibabacloud_resourcemanager20200331_py2-1.1.4.tar` & `alibabacloud_resourcemanager20200331_py2-1.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/
--rw-r--r--   0 root         (0) root         (0)      605 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2544 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1069 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1152 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/alibabacloud_resourcemanager20200331/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/alibabacloud_resourcemanager20200331/__init__.py
--rw-r--r--   0 root         (0) root         (0)   162875 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/alibabacloud_resourcemanager20200331/client.py
--rw-r--r--   0 root         (0) root         (0)   594770 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/alibabacloud_resourcemanager20200331/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/alibabacloud_resourcemanager20200331_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2544 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/alibabacloud_resourcemanager20200331_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      536 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/alibabacloud_resourcemanager20200331_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/alibabacloud_resourcemanager20200331_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/alibabacloud_resourcemanager20200331_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/alibabacloud_resourcemanager20200331_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2963 2023-06-05 05:46:26.000000 alibabacloud_resourcemanager20200331_py2-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/
+-rw-r--r--   0 root         (0) root         (0)      671 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/alibabacloud_resourcemanager20200331/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/alibabacloud_resourcemanager20200331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   162995 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/alibabacloud_resourcemanager20200331/client.py
+-rw-r--r--   0 root         (0) root         (0)   596410 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/alibabacloud_resourcemanager20200331/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/alibabacloud_resourcemanager20200331_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/alibabacloud_resourcemanager20200331_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      536 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/alibabacloud_resourcemanager20200331_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/alibabacloud_resourcemanager20200331_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/alibabacloud_resourcemanager20200331_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/alibabacloud_resourcemanager20200331_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-07-27 03:04:05.000000 alibabacloud_resourcemanager20200331_py2-1.1.5/setup.py
```

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.4/ChangeLog.md` & `alibabacloud_resourcemanager20200331_py2-1.1.5/ChangeLog.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-06-05 Version: 1.1.4
+- Modify endpoint for resourcemanager.
+
 2023-05-18 Version: 1.1.3
 - Supported more language for resourcemanager.
 
 2023-02-22 Version: 1.1.2
 - Supported more language for resourcemanager.
 
 2022-12-01 Version: 1.1.1
```

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.4/LICENSE` & `alibabacloud_resourcemanager20200331_py2-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.4/PKG-INFO` & `alibabacloud_resourcemanager20200331_py2-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_resourcemanager20200331_py2
-Version: 1.1.4
+Version: 1.1.5
 Summary: Alibaba Cloud ResourceManager (20200331) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.4/README-CN.md` & `alibabacloud_resourcemanager20200331_py2-1.1.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.4/README.md` & `alibabacloud_resourcemanager20200331_py2-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.4/alibabacloud_resourcemanager20200331/client.py` & `alibabacloud_resourcemanager20200331_py2-1.1.5/alibabacloud_resourcemanager20200331/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2810,14 +2810,16 @@
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

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.4/alibabacloud_resourcemanager20200331/models.py` & `alibabacloud_resourcemanager20200331_py2-1.1.5/alibabacloud_resourcemanager20200331/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -11421,17 +11421,46 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListResourceGroupsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListResourcesRequestResourceTypes(TeaModel):
+    def __init__(self, resource_type=None, service=None):
+        self.resource_type = resource_type  # type: str
+        self.service = service  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListResourcesRequestResourceTypes, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        if m.get('Service') is not None:
+            self.service = m.get('Service')
+        return self
+
+
 class ListResourcesRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None, region=None, resource_group_id=None, resource_id=None,
-                 resource_type=None, service=None):
+                 resource_type=None, resource_types=None, service=None):
         # The number of the page to return.
         # 
         # Pages start from page 1. Default value: 1.
         self.page_number = page_number  # type: int
         # The number of entries to return on each page.
         # 
         # Valid values: 1 to 100. Default value: 10.
@@ -11442,21 +11471,25 @@
         self.resource_group_id = resource_group_id  # type: str
         # The ID of the resource.
         self.resource_id = resource_id  # type: str
         # The resource type.
         # 
         # For more information about the supported resource types, see the **Resource type** column in [Alibaba Cloud services that support resource groups](~~94479~~).
         self.resource_type = resource_type  # type: str
+        self.resource_types = resource_types  # type: list[ListResourcesRequestResourceTypes]
         # The ID of the Alibaba Cloud service.
         # 
         # You can obtain the ID from the **Service code** column in [Alibaba Cloud services that support resource groups](~~94479~~).
         self.service = service  # type: str
 
     def validate(self):
-        pass
+        if self.resource_types:
+            for k in self.resource_types:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super(ListResourcesRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -11468,14 +11501,18 @@
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('PageNumber') is not None:
@@ -11486,14 +11523,19 @@
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
     def __init__(self, create_date=None, region_id=None, resource_group_id=None, resource_id=None,
@@ -14570,22 +14612,24 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class TagResourcesRequest(TeaModel):
     def __init__(self, resource_id=None, resource_type=None, tag=None):
+        # The ID of a resource group or member.
         self.resource_id = resource_id  # type: list[str]
         # The type of the objects to which you want to add tags. Valid values:
         # 
         # *   ResourceGroup : resource group. This is the default value.
         # *   Account: member.
         # 
         # >  This parameter is required if you add tags to members in a resource directory.
         self.resource_type = resource_type  # type: str
+        # The tags.
         self.tag = tag  # type: list[TagResourcesRequestTag]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
```

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.4/alibabacloud_resourcemanager20200331_py2.egg-info/PKG-INFO` & `alibabacloud_resourcemanager20200331_py2-1.1.5/alibabacloud_resourcemanager20200331_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-resourcemanager20200331-py2
-Version: 1.1.4
+Version: 1.1.5
 Summary: Alibaba Cloud ResourceManager (20200331) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.4/alibabacloud_resourcemanager20200331_py2.egg-info/SOURCES.txt` & `alibabacloud_resourcemanager20200331_py2-1.1.5/alibabacloud_resourcemanager20200331_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.4/setup.py` & `alibabacloud_resourcemanager20200331_py2-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcemanager20200331_py2.
 
-Created on 05/06/2023
+Created on 27/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcemanager20200331"
 NAME = "alibabacloud_resourcemanager20200331_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceManager (20200331) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

