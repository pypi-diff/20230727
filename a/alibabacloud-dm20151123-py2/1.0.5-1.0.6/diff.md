# Comparing `tmp/alibabacloud_dm20151123_py2-1.0.5.tar.gz` & `tmp/alibabacloud_dm20151123_py2-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dm20151123_py2-1.0.5.tar", last modified: Thu Sep 29 03:40:14 2022, max compression
+gzip compressed data, was "dist/alibabacloud_dm20151123_py2-1.0.6.tar", last modified: Thu Jul 27 09:25:27 2023, max compression
```

## Comparing `alibabacloud_dm20151123_py2-1.0.5.tar` & `alibabacloud_dm20151123_py2-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      475 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2466 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1030 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/alibabacloud_dm20151123/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/alibabacloud_dm20151123/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60168 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/alibabacloud_dm20151123/client.py
--rw-r--r--   0 root         (0) root         (0)   218922 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/alibabacloud_dm20151123/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/alibabacloud_dm20151123_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2466 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/alibabacloud_dm20151123_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/alibabacloud_dm20151123_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/alibabacloud_dm20151123_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/alibabacloud_dm20151123_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/alibabacloud_dm20151123_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2898 2022-09-29 03:40:14.000000 alibabacloud_dm20151123_py2-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:25:27.000000 alibabacloud_dm20151123_py2-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      538 2023-07-27 09:25:26.000000 alibabacloud_dm20151123_py2-1.0.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-27 09:25:26.000000 alibabacloud_dm20151123_py2-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-27 09:25:26.000000 alibabacloud_dm20151123_py2-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2466 2023-07-27 09:25:27.000000 alibabacloud_dm20151123_py2-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-07-27 09:25:26.000000 alibabacloud_dm20151123_py2-1.0.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-27 09:25:26.000000 alibabacloud_dm20151123_py2-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:25:27.000000 alibabacloud_dm20151123_py2-1.0.6/alibabacloud_dm20151123/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 09:25:26.000000 alibabacloud_dm20151123_py2-1.0.6/alibabacloud_dm20151123/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    61785 2023-07-27 09:25:26.000000 alibabacloud_dm20151123_py2-1.0.6/alibabacloud_dm20151123/client.py
+-rw-r--r--   0 root         (0) root         (0)   225039 2023-07-27 09:25:26.000000 alibabacloud_dm20151123_py2-1.0.6/alibabacloud_dm20151123/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:25:27.000000 alibabacloud_dm20151123_py2-1.0.6/alibabacloud_dm20151123_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2466 2023-07-27 09:25:27.000000 alibabacloud_dm20151123_py2-1.0.6/alibabacloud_dm20151123_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2023-07-27 09:25:27.000000 alibabacloud_dm20151123_py2-1.0.6/alibabacloud_dm20151123_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 09:25:27.000000 alibabacloud_dm20151123_py2-1.0.6/alibabacloud_dm20151123_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-27 09:25:27.000000 alibabacloud_dm20151123_py2-1.0.6/alibabacloud_dm20151123_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-27 09:25:27.000000 alibabacloud_dm20151123_py2-1.0.6/alibabacloud_dm20151123_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 09:25:27.000000 alibabacloud_dm20151123_py2-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-07-27 09:25:26.000000 alibabacloud_dm20151123_py2-1.0.6/setup.py
```

### Comparing `alibabacloud_dm20151123_py2-1.0.5/LICENSE` & `alibabacloud_dm20151123_py2-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123_py2-1.0.5/PKG-INFO` & `alibabacloud_dm20151123_py2-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dm20151123_py2
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud Dm (20151123) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dm20151123_py2-1.0.5/README-CN.md` & `alibabacloud_dm20151123_py2-1.0.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123_py2-1.0.5/README.md` & `alibabacloud_dm20151123_py2-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123_py2-1.0.5/alibabacloud_dm20151123/client.py` & `alibabacloud_dm20151123_py2-1.0.6/alibabacloud_dm20151123/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -392,14 +392,48 @@
             self.call_api(params, req, runtime)
         )
 
     def delete_domain(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_domain_with_options(request, runtime)
 
+    def delete_invalid_address_with_options(self, request, runtime):
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
+    def delete_invalid_address(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_invalid_address_with_options(request, runtime)
+
     def delete_ipfilter_by_edm_id_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.from_type):
             query['FromType'] = request.from_type
         if not UtilClient.is_unset(request.id):
             query['Id'] = request.id
@@ -839,16 +873,20 @@
         return self.modify_mail_address_with_options(request, runtime)
 
     def modify_pwby_domain_with_options(self, request, runtime):
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

### Comparing `alibabacloud_dm20151123_py2-1.0.5/alibabacloud_dm20151123/models.py` & `alibabacloud_dm20151123_py2-1.0.6/alibabacloud_dm20151123/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,14 +354,15 @@
             temp_model = BatchSendMailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CheckDomainRequest(TeaModel):
     def __init__(self, domain_id=None, owner_id=None, resource_owner_account=None, resource_owner_id=None):
+        # The ID of the domain name.
         self.domain_id = domain_id  # type: int
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
 
     def validate(self):
         pass
@@ -393,15 +394,23 @@
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
         return self
 
 
 class CheckDomainResponseBody(TeaModel):
     def __init__(self, domain_status=None, request_id=None):
+        # The status of the domain name. Indicates whether the domain name is verified and available.
+        # 
+        # *   0: indicates that the domain name is verified and available.
+        # *   1: indicates that the domain name fails to be verified and is unavailable.
+        # *   2: indicates that the domain name is available, but not filed or configured with a CNAME record.
+        # *   3: indicates that the domain name is available but not filed.
+        # *   4: indicates that the domain name is available but not configured with a CNAME record.
         self.domain_status = domain_status  # type: int
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CheckDomainResponseBody, self).to_map()
@@ -1124,14 +1133,116 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteInvalidAddressRequest(TeaModel):
+    def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, to_address=None):
+        self.owner_id = owner_id  # type: long
+        self.resource_owner_account = resource_owner_account  # type: str
+        self.resource_owner_id = resource_owner_id  # type: long
+        self.to_address = to_address  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteInvalidAddressRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteInvalidAddressResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteInvalidAddressResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeleteInvalidAddressResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeleteInvalidAddressResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, from_type=None, id=None, owner_id=None, resource_owner_account=None, resource_owner_id=None):
         self.from_type = from_type  # type: int
         self.id = id  # type: str
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
@@ -1336,14 +1447,15 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteReceiverRequest(TeaModel):
     def __init__(self, owner_id=None, receiver_id=None, resource_owner_account=None, resource_owner_id=None):
         self.owner_id = owner_id  # type: long
+        # The ID of the recipient list.
         self.receiver_id = receiver_id  # type: str
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
 
     def validate(self):
         pass
 
@@ -1374,14 +1486,15 @@
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
         return self
 
 
 class DeleteReceiverResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteReceiverResponseBody, self).to_map()
@@ -1548,14 +1661,15 @@
 
 
 class DeleteTagRequest(TeaModel):
     def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, tag_id=None):
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
+        # The ID of the tag.
         self.tag_id = tag_id  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteTagRequest, self).to_map()
@@ -1584,14 +1698,15 @@
         if m.get('TagId') is not None:
             self.tag_id = m.get('TagId')
         return self
 
 
 class DeleteTagResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteTagResponseBody, self).to_map()
@@ -1860,35 +1975,40 @@
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
         return self
 
 
 class DescDomainResponseBody(TeaModel):
     def __init__(self, cname_auth_status=None, cname_confirm_status=None, cname_record=None, create_time=None,
-                 default_domain=None, dns_mx=None, dns_spf=None, dns_txt=None, domain_id=None, domain_name=None, domain_status=None,
-                 domain_type=None, icp_status=None, mx_auth_status=None, mx_record=None, request_id=None, spf_auth_status=None,
-                 spf_record=None, tl_domain_name=None, tracef_record=None):
+                 default_domain=None, dkim_auth_status=None, dkim_public_key=None, dkim_rr=None, dns_mx=None, dns_spf=None,
+                 dns_txt=None, domain_id=None, domain_name=None, domain_status=None, domain_type=None, icp_status=None,
+                 mx_auth_status=None, mx_record=None, request_id=None, spf_auth_status=None, spf_record=None, spf_record_v2=None,
+                 tl_domain_name=None, tracef_record=None):
         self.cname_auth_status = cname_auth_status  # type: str
         self.cname_confirm_status = cname_confirm_status  # type: str
         self.cname_record = cname_record  # type: str
         self.create_time = create_time  # type: str
         self.default_domain = default_domain  # type: str
+        self.dkim_auth_status = dkim_auth_status  # type: str
+        self.dkim_public_key = dkim_public_key  # type: str
+        self.dkim_rr = dkim_rr  # type: str
         self.dns_mx = dns_mx  # type: str
         self.dns_spf = dns_spf  # type: str
         self.dns_txt = dns_txt  # type: str
         self.domain_id = domain_id  # type: str
         self.domain_name = domain_name  # type: str
         self.domain_status = domain_status  # type: str
         self.domain_type = domain_type  # type: str
         self.icp_status = icp_status  # type: str
         self.mx_auth_status = mx_auth_status  # type: str
         self.mx_record = mx_record  # type: str
         self.request_id = request_id  # type: str
         self.spf_auth_status = spf_auth_status  # type: str
         self.spf_record = spf_record  # type: str
+        self.spf_record_v2 = spf_record_v2  # type: str
         self.tl_domain_name = tl_domain_name  # type: str
         self.tracef_record = tracef_record  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1903,14 +2023,20 @@
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
@@ -1929,14 +2055,16 @@
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
 
     def from_map(self, m=None):
@@ -1947,14 +2075,20 @@
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
@@ -1973,14 +2107,16 @@
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
 
 
@@ -2980,42 +3116,53 @@
         if m.get('body') is not None:
             temp_model = ModifyMailAddressResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyPWByDomainRequest(TeaModel):
-    def __init__(self, domain_name=None, password=None, resource_owner_id=None):
+    def __init__(self, domain_name=None, owner_id=None, password=None, resource_owner_account=None,
+                 resource_owner_id=None):
         self.domain_name = domain_name  # type: str
+        self.owner_id = owner_id  # type: long
         self.password = password  # type: str
-        self.resource_owner_id = resource_owner_id  # type: str
+        self.resource_owner_account = resource_owner_account  # type: str
+        self.resource_owner_id = resource_owner_id  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyPWByDomainRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, code=None, message=None, request_id=None, success=None):
@@ -3097,15 +3244,17 @@
 
 class ModifyTagRequest(TeaModel):
     def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, tag_id=None,
                  tag_name=None):
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
+        # The ID of the tag.
         self.tag_id = tag_id  # type: int
+        # The name of the tag.
         self.tag_name = tag_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyTagRequest, self).to_map()
@@ -3138,14 +3287,15 @@
         if m.get('TagName') is not None:
             self.tag_name = m.get('TagName')
         return self
 
 
 class ModifyTagResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyTagResponseBody, self).to_map()
```

### Comparing `alibabacloud_dm20151123_py2-1.0.5/alibabacloud_dm20151123_py2.egg-info/PKG-INFO` & `alibabacloud_dm20151123_py2-1.0.6/alibabacloud_dm20151123_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dm20151123-py2
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud Dm (20151123) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dm20151123_py2-1.0.5/setup.py` & `alibabacloud_dm20151123_py2-1.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dm20151123_py2.
 
-Created on 29/09/2022
+Created on 27/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dm20151123"
 NAME = "alibabacloud_dm20151123_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dm (20151123) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.6, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.3, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

