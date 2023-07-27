# Comparing `tmp/alibabacloud_dm20151123-1.0.5.tar.gz` & `tmp/alibabacloud_dm20151123-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dm20151123-1.0.5.tar", last modified: Thu Sep 29 03:40:51 2022, max compression
+gzip compressed data, was "dist/alibabacloud_dm20151123-1.0.6.tar", last modified: Thu Jul 27 09:25:59 2023, max compression
```

## Comparing `alibabacloud_dm20151123-1.0.5.tar` & `alibabacloud_dm20151123-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 03:40:51.000000 alibabacloud_dm20151123-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      524 2022-09-29 03:40:50.000000 alibabacloud_dm20151123-1.0.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-09-29 03:40:50.000000 alibabacloud_dm20151123-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-09-29 03:40:50.000000 alibabacloud_dm20151123-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2322 2022-09-29 03:40:51.000000 alibabacloud_dm20151123-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1019 2022-09-29 03:40:50.000000 alibabacloud_dm20151123-1.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1104 2022-09-29 03:40:50.000000 alibabacloud_dm20151123-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 03:40:51.000000 alibabacloud_dm20151123-1.0.5/alibabacloud_dm20151123/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-29 03:40:50.000000 alibabacloud_dm20151123-1.0.5/alibabacloud_dm20151123/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140712 2022-09-29 03:40:50.000000 alibabacloud_dm20151123-1.0.5/alibabacloud_dm20151123/client.py
--rw-r--r--   0 root         (0) root         (0)   217650 2022-09-29 03:40:50.000000 alibabacloud_dm20151123-1.0.5/alibabacloud_dm20151123/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 03:40:51.000000 alibabacloud_dm20151123-1.0.5/alibabacloud_dm20151123.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2322 2022-09-29 03:40:50.000000 alibabacloud_dm20151123-1.0.5/alibabacloud_dm20151123.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2022-09-29 03:40:50.000000 alibabacloud_dm20151123-1.0.5/alibabacloud_dm20151123.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-29 03:40:50.000000 alibabacloud_dm20151123-1.0.5/alibabacloud_dm20151123.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-09-29 03:40:50.000000 alibabacloud_dm20151123-1.0.5/alibabacloud_dm20151123.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2022-09-29 03:40:50.000000 alibabacloud_dm20151123-1.0.5/alibabacloud_dm20151123.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-29 03:40:51.000000 alibabacloud_dm20151123-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2605 2022-09-29 03:40:50.000000 alibabacloud_dm20151123-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/alibabacloud_dm20151123/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/alibabacloud_dm20151123/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   144554 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/alibabacloud_dm20151123/client.py
+-rw-r--r--   0 root         (0) root         (0)   223721 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/alibabacloud_dm20151123/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/alibabacloud_dm20151123.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/alibabacloud_dm20151123.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/alibabacloud_dm20151123.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/alibabacloud_dm20151123.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/alibabacloud_dm20151123.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/alibabacloud_dm20151123.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-07-27 09:25:59.000000 alibabacloud_dm20151123-1.0.6/setup.py
```

### Comparing `alibabacloud_dm20151123-1.0.5/ChangeLog.md` & `alibabacloud_dm20151123-1.0.6/ChangeLog.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2022-09-29 Version: 1.0.5
+- Automatically generate sdk tasks.
+
 2022-08-02 Version: 1.0.4
 - The input parameter IpProtection of UpdateIpProtection API  is corrected to be required. 
 
 2022-05-20 Version: 1.0.3
 - Ip related APIs are changed to visiable and QPM is set as 60 .
 
 2022-04-21 Version: 1.0.2
```

### Comparing `alibabacloud_dm20151123-1.0.5/LICENSE` & `alibabacloud_dm20151123-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123-1.0.5/PKG-INFO` & `alibabacloud_dm20151123-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dm20151123
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud Dm (20151123) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dm20151123-1.0.5/README-CN.md` & `alibabacloud_dm20151123-1.0.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123-1.0.5/README.md` & `alibabacloud_dm20151123-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123-1.0.5/alibabacloud_dm20151123/client.py` & `alibabacloud_dm20151123-1.0.6/alibabacloud_dm20151123/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -909,14 +909,96 @@
     async def delete_domain_async(
         self,
         request: dm_20151123_models.DeleteDomainRequest,
     ) -> dm_20151123_models.DeleteDomainResponse:
         runtime = util_models.RuntimeOptions()
         return await self.delete_domain_with_options_async(request, runtime)
 
+    def delete_invalid_address_with_options(
+        self,
+        request: dm_20151123_models.DeleteInvalidAddressRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dm_20151123_models.DeleteInvalidAddressResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.to_address):
+            query['ToAddress'] = request.to_address
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteInvalidAddress',
+            version='2015-11-23',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dm_20151123_models.DeleteInvalidAddressResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_invalid_address_with_options_async(
+        self,
+        request: dm_20151123_models.DeleteInvalidAddressRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dm_20151123_models.DeleteInvalidAddressResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.to_address):
+            query['ToAddress'] = request.to_address
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteInvalidAddress',
+            version='2015-11-23',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dm_20151123_models.DeleteInvalidAddressResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_invalid_address(
+        self,
+        request: dm_20151123_models.DeleteInvalidAddressRequest,
+    ) -> dm_20151123_models.DeleteInvalidAddressResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_invalid_address_with_options(request, runtime)
+
+    async def delete_invalid_address_async(
+        self,
+        request: dm_20151123_models.DeleteInvalidAddressRequest,
+    ) -> dm_20151123_models.DeleteInvalidAddressResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_invalid_address_with_options_async(request, runtime)
+
     def delete_ipfilter_by_edm_id_with_options(
         self,
         request: dm_20151123_models.DeleteIpfilterByEdmIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DeleteIpfilterByEdmIdResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1970,16 +2052,20 @@
         request: dm_20151123_models.ModifyPWByDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.ModifyPWByDomainResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.password):
             query['Password'] = request.password
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyPWByDomain',
@@ -2002,16 +2088,20 @@
         request: dm_20151123_models.ModifyPWByDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.ModifyPWByDomainResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.password):
             query['Password'] = request.password
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyPWByDomain',
```

### Comparing `alibabacloud_dm20151123-1.0.5/alibabacloud_dm20151123/models.py` & `alibabacloud_dm20151123-1.0.6/alibabacloud_dm20151123/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,14 +410,15 @@
     def __init__(
         self,
         domain_id: int = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
+        # The ID of the domain name.
         self.domain_id = domain_id
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
@@ -453,15 +454,23 @@
 
 class CheckDomainResponseBody(TeaModel):
     def __init__(
         self,
         domain_status: int = None,
         request_id: str = None,
     ):
+        # The status of the domain name. Indicates whether the domain name is verified and available.
+        # 
+        # *   0: indicates that the domain name is verified and available.
+        # *   1: indicates that the domain name fails to be verified and is unavailable.
+        # *   2: indicates that the domain name is available, but not filed or configured with a CNAME record.
+        # *   3: indicates that the domain name is available but not filed.
+        # *   4: indicates that the domain name is available but not configured with a CNAME record.
         self.domain_status = domain_status
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1280,14 +1289,130 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteInvalidAddressRequest(TeaModel):
+    def __init__(
+        self,
+        owner_id: int = None,
+        resource_owner_account: str = None,
+        resource_owner_id: int = None,
+        to_address: str = None,
+    ):
+        self.owner_id = owner_id
+        self.resource_owner_account = resource_owner_account
+        self.resource_owner_id = resource_owner_id
+        self.to_address = to_address
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
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        if self.to_address is not None:
+            result['ToAddress'] = self.to_address
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        if m.get('ToAddress') is not None:
+            self.to_address = m.get('ToAddress')
+        return self
+
+
+class DeleteInvalidAddressResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteInvalidAddressResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteInvalidAddressResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteInvalidAddressResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteIpfilterByEdmIdRequest(TeaModel):
     def __init__(
         self,
         from_type: int = None,
         id: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
@@ -1527,14 +1652,15 @@
         self,
         owner_id: int = None,
         receiver_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         self.owner_id = owner_id
+        # The ID of the recipient list.
         self.receiver_id = receiver_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
@@ -1568,14 +1694,15 @@
 
 
 class DeleteReceiverResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1767,14 +1894,15 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         tag_id: int = None,
     ):
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
+        # The ID of the tag.
         self.tag_id = tag_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1806,14 +1934,15 @@
 
 
 class DeleteTagResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2125,48 +2254,56 @@
     def __init__(
         self,
         cname_auth_status: str = None,
         cname_confirm_status: str = None,
         cname_record: str = None,
         create_time: str = None,
         default_domain: str = None,
+        dkim_auth_status: str = None,
+        dkim_public_key: str = None,
+        dkim_rr: str = None,
         dns_mx: str = None,
         dns_spf: str = None,
         dns_txt: str = None,
         domain_id: str = None,
         domain_name: str = None,
         domain_status: str = None,
         domain_type: str = None,
         icp_status: str = None,
         mx_auth_status: str = None,
         mx_record: str = None,
         request_id: str = None,
         spf_auth_status: str = None,
         spf_record: str = None,
+        spf_record_v2: str = None,
         tl_domain_name: str = None,
         tracef_record: str = None,
     ):
         self.cname_auth_status = cname_auth_status
         self.cname_confirm_status = cname_confirm_status
         self.cname_record = cname_record
         self.create_time = create_time
         self.default_domain = default_domain
+        self.dkim_auth_status = dkim_auth_status
+        self.dkim_public_key = dkim_public_key
+        self.dkim_rr = dkim_rr
         self.dns_mx = dns_mx
         self.dns_spf = dns_spf
         self.dns_txt = dns_txt
         self.domain_id = domain_id
         self.domain_name = domain_name
         self.domain_status = domain_status
         self.domain_type = domain_type
         self.icp_status = icp_status
         self.mx_auth_status = mx_auth_status
         self.mx_record = mx_record
         self.request_id = request_id
         self.spf_auth_status = spf_auth_status
         self.spf_record = spf_record
+        self.spf_record_v2 = spf_record_v2
         self.tl_domain_name = tl_domain_name
         self.tracef_record = tracef_record
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2181,14 +2318,20 @@
             result['CnameConfirmStatus'] = self.cname_confirm_status
         if self.cname_record is not None:
             result['CnameRecord'] = self.cname_record
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
         if self.default_domain is not None:
             result['DefaultDomain'] = self.default_domain
+        if self.dkim_auth_status is not None:
+            result['DkimAuthStatus'] = self.dkim_auth_status
+        if self.dkim_public_key is not None:
+            result['DkimPublicKey'] = self.dkim_public_key
+        if self.dkim_rr is not None:
+            result['DkimRR'] = self.dkim_rr
         if self.dns_mx is not None:
             result['DnsMx'] = self.dns_mx
         if self.dns_spf is not None:
             result['DnsSpf'] = self.dns_spf
         if self.dns_txt is not None:
             result['DnsTxt'] = self.dns_txt
         if self.domain_id is not None:
@@ -2207,14 +2350,16 @@
             result['MxRecord'] = self.mx_record
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.spf_auth_status is not None:
             result['SpfAuthStatus'] = self.spf_auth_status
         if self.spf_record is not None:
             result['SpfRecord'] = self.spf_record
+        if self.spf_record_v2 is not None:
+            result['SpfRecordV2'] = self.spf_record_v2
         if self.tl_domain_name is not None:
             result['TlDomainName'] = self.tl_domain_name
         if self.tracef_record is not None:
             result['TracefRecord'] = self.tracef_record
         return result
 
     def from_map(self, m: dict = None):
@@ -2225,14 +2370,20 @@
             self.cname_confirm_status = m.get('CnameConfirmStatus')
         if m.get('CnameRecord') is not None:
             self.cname_record = m.get('CnameRecord')
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('DefaultDomain') is not None:
             self.default_domain = m.get('DefaultDomain')
+        if m.get('DkimAuthStatus') is not None:
+            self.dkim_auth_status = m.get('DkimAuthStatus')
+        if m.get('DkimPublicKey') is not None:
+            self.dkim_public_key = m.get('DkimPublicKey')
+        if m.get('DkimRR') is not None:
+            self.dkim_rr = m.get('DkimRR')
         if m.get('DnsMx') is not None:
             self.dns_mx = m.get('DnsMx')
         if m.get('DnsSpf') is not None:
             self.dns_spf = m.get('DnsSpf')
         if m.get('DnsTxt') is not None:
             self.dns_txt = m.get('DnsTxt')
         if m.get('DomainId') is not None:
@@ -2251,14 +2402,16 @@
             self.mx_record = m.get('MxRecord')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('SpfAuthStatus') is not None:
             self.spf_auth_status = m.get('SpfAuthStatus')
         if m.get('SpfRecord') is not None:
             self.spf_record = m.get('SpfRecord')
+        if m.get('SpfRecordV2') is not None:
+            self.spf_record_v2 = m.get('SpfRecordV2')
         if m.get('TlDomainName') is not None:
             self.tl_domain_name = m.get('TlDomainName')
         if m.get('TracefRecord') is not None:
             self.tracef_record = m.get('TracefRecord')
         return self
 
 
@@ -3396,44 +3549,56 @@
         return self
 
 
 class ModifyPWByDomainRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
+        owner_id: int = None,
         password: str = None,
-        resource_owner_id: str = None,
+        resource_owner_account: str = None,
+        resource_owner_id: int = None,
     ):
         self.domain_name = domain_name
+        self.owner_id = owner_id
         self.password = password
+        self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.domain_name is not None:
             result['DomainName'] = self.domain_name
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
         if self.password is not None:
             result['Password'] = self.password
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
             result['ResourceOwnerId'] = self.resource_owner_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('DomainName') is not None:
             self.domain_name = m.get('DomainName')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
         if m.get('Password') is not None:
             self.password = m.get('Password')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
         return self
 
 
 class ModifyPWByDomainResponseBody(TeaModel):
     def __init__(
@@ -3532,15 +3697,17 @@
         resource_owner_id: int = None,
         tag_id: int = None,
         tag_name: str = None,
     ):
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
+        # The ID of the tag.
         self.tag_id = tag_id
+        # The name of the tag.
         self.tag_name = tag_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3576,14 +3743,15 @@
 
 
 class ModifyTagResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_dm20151123-1.0.5/alibabacloud_dm20151123.egg-info/PKG-INFO` & `alibabacloud_dm20151123-1.0.6/alibabacloud_dm20151123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dm20151123
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud Dm (20151123) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dm20151123-1.0.5/setup.py` & `alibabacloud_dm20151123-1.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dm20151123.
 
-Created on 29/09/2022
+Created on 27/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dm20151123"
 NAME = "alibabacloud_dm20151123" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dm (20151123) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

