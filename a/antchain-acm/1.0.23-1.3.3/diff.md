# Comparing `tmp/antchain_acm-1.0.23.tar.gz` & `tmp/antchain_acm-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_acm-1.0.23.tar", last modified: Fri Jun 17 09:01:26 2022, max compression
+gzip compressed data, was "dist/antchain_acm-1.3.3.tar", last modified: Thu Jul 27 02:06:38 2023, max compression
```

## Comparing `antchain_acm-1.0.23.tar` & `antchain_acm-1.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-17 09:01:26.000000 antchain_acm-1.0.23/
--rw-r--r--   0 root         (0) root         (0)      600 2022-06-17 09:01:25.000000 antchain_acm-1.0.23/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-06-17 09:01:25.000000 antchain_acm-1.0.23/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2171 2022-06-17 09:01:26.000000 antchain_acm-1.0.23/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      812 2022-06-17 09:01:25.000000 antchain_acm-1.0.23/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      998 2022-06-17 09:01:25.000000 antchain_acm-1.0.23/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-17 09:01:26.000000 antchain_acm-1.0.23/antchain_acm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2171 2022-06-17 09:01:25.000000 antchain_acm-1.0.23/antchain_acm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2022-06-17 09:01:25.000000 antchain_acm-1.0.23/antchain_acm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-17 09:01:25.000000 antchain_acm-1.0.23/antchain_acm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-06-17 09:01:25.000000 antchain_acm-1.0.23/antchain_acm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-06-17 09:01:25.000000 antchain_acm-1.0.23/antchain_acm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-17 09:01:26.000000 antchain_acm-1.0.23/antchain_sdk_acm/
--rw-r--r--   0 root         (0) root         (0)       22 2022-06-17 09:01:25.000000 antchain_acm-1.0.23/antchain_sdk_acm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73050 2022-06-17 09:01:25.000000 antchain_acm-1.0.23/antchain_sdk_acm/client.py
--rw-r--r--   0 root         (0) root         (0)   138427 2022-06-17 09:01:25.000000 antchain_acm-1.0.23/antchain_sdk_acm/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2022-06-17 09:01:26.000000 antchain_acm-1.0.23/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2022-06-17 09:01:25.000000 antchain_acm-1.0.23/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:06:38.000000 antchain_acm-1.3.3/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-27 02:06:37.000000 antchain_acm-1.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-27 02:06:37.000000 antchain_acm-1.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-07-27 02:06:38.000000 antchain_acm-1.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-07-27 02:06:37.000000 antchain_acm-1.3.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2023-07-27 02:06:37.000000 antchain_acm-1.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:06:38.000000 antchain_acm-1.3.3/antchain_acm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-07-27 02:06:38.000000 antchain_acm-1.3.3/antchain_acm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2023-07-27 02:06:38.000000 antchain_acm-1.3.3/antchain_acm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:06:38.000000 antchain_acm-1.3.3/antchain_acm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-27 02:06:38.000000 antchain_acm-1.3.3/antchain_acm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-27 02:06:38.000000 antchain_acm-1.3.3/antchain_acm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:06:38.000000 antchain_acm-1.3.3/antchain_sdk_acm/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 02:06:37.000000 antchain_acm-1.3.3/antchain_sdk_acm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89046 2023-07-27 02:06:37.000000 antchain_acm-1.3.3/antchain_sdk_acm/client.py
+-rw-r--r--   0 root         (0) root         (0)   164317 2023-07-27 02:06:37.000000 antchain_acm-1.3.3/antchain_sdk_acm/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 02:06:38.000000 antchain_acm-1.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-07-27 02:06:37.000000 antchain_acm-1.3.3/setup.py
```

### Comparing `antchain_acm-1.0.23/LICENSE` & `antchain_acm-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_acm-1.0.23/PKG-INFO` & `antchain_acm-1.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_acm
-Version: 1.0.23
+Version: 1.3.3
 Summary: Ant Chain Acm SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain_sdk_acm
-        pip install antchain_sdk_acm
+        # Install the antchain-acm
+        pip install antchain-acm
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_acm-1.0.23/README-CN.md` & `antchain_acm-1.3.3/README-CN.md`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## 安装
 
 - **使用 pip 安装(推荐)**
 
 如未安装 `pip`, 请先至pip官网 [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") 安装pip .
 
 ```bash
-# 安装 antchain_sdk_acm
-pip install antchain_sdk_acm
+# 安装 antchain-acm
+pip install antchain-acm
 ```
 
 ## 问题
 
 [提交 Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new)，不符合指南的问题可能会立即关闭。
 
 ## 使用说明
```

### Comparing `antchain_acm-1.0.23/README.md` & `antchain_acm-1.3.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## Installation
 
 - **Install with pip**
 
 Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
 
 ```bash
-# Install the antchain_sdk_acm
-pip install antchain_sdk_acm
+# Install the antchain-acm
+pip install antchain-acm
 ```
 
 ## Issues
 
 [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
 
 ## Usage
```

### Comparing `antchain_acm-1.0.23/antchain_acm.egg-info/PKG-INFO` & `antchain_acm-1.3.3/antchain_acm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-acm
-Version: 1.0.23
+Version: 1.3.3
 Summary: Ant Chain Acm SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain_sdk_acm
-        pip install antchain_sdk_acm
+        # Install the antchain-acm
+        pip install antchain-acm
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_acm-1.0.23/antchain_sdk_acm/client.py` & `antchain_acm-1.3.3/antchain_sdk_acm/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -131,15 +131,17 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.23'
+                    'sdk_version': '1.3.3',
+                    '_prod_code': 'acm',
+                    '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -196,15 +198,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -233,15 +235,17 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.23'
+                    'sdk_version': '1.3.3',
+                    '_prod_code': 'acm',
+                    '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -302,30 +306,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetCustomerResponse:
         """
         Description: 查询企业详情
         Summary: 获取企业
         """
         UtilClient.validate_model(request)
-        return acm_models.GetCustomerResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetCustomerResponse(),
             self.do_request('1.0', 'antcloud.acm.customer.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_customer_ex_async(
         self,
         request: acm_models.GetCustomerRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetCustomerResponse:
         """
         Description: 查询企业详情
         Summary: 获取企业
         """
         UtilClient.validate_model(request)
-        return acm_models.GetCustomerResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetCustomerResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.customer.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def get_operator(
         self,
         request: acm_models.GetOperatorRequest,
     ) -> acm_models.GetOperatorResponse:
@@ -356,30 +362,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetOperatorResponse:
         """
         Description: 查询一个操作员的详情
         Summary: 获取操作员
         """
         UtilClient.validate_model(request)
-        return acm_models.GetOperatorResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetOperatorResponse(),
             self.do_request('1.0', 'antcloud.acm.operator.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_operator_ex_async(
         self,
         request: acm_models.GetOperatorRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetOperatorResponse:
         """
         Description: 查询一个操作员的详情
         Summary: 获取操作员
         """
         UtilClient.validate_model(request)
-        return acm_models.GetOperatorResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetOperatorResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.operator.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_operator(
         self,
         request: acm_models.QueryOperatorRequest,
     ) -> acm_models.QueryOperatorResponse:
@@ -410,30 +418,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.QueryOperatorResponse:
         """
         Description: 查询操作员列表
         Summary: 查询操作员
         """
         UtilClient.validate_model(request)
-        return acm_models.QueryOperatorResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.QueryOperatorResponse(),
             self.do_request('1.0', 'antcloud.acm.operator.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_operator_ex_async(
         self,
         request: acm_models.QueryOperatorRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.QueryOperatorResponse:
         """
         Description: 查询操作员列表
         Summary: 查询操作员
         """
         UtilClient.validate_model(request)
-        return acm_models.QueryOperatorResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.QueryOperatorResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.operator.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def search_operator(
         self,
         request: acm_models.SearchOperatorRequest,
     ) -> acm_models.SearchOperatorResponse:
@@ -464,30 +474,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.SearchOperatorResponse:
         """
         Description: 搜索操作员
         Summary: 搜索操作员
         """
         UtilClient.validate_model(request)
-        return acm_models.SearchOperatorResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.SearchOperatorResponse(),
             self.do_request('1.0', 'antcloud.acm.operator.search', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def search_operator_ex_async(
         self,
         request: acm_models.SearchOperatorRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.SearchOperatorResponse:
         """
         Description: 搜索操作员
         Summary: 搜索操作员
         """
         UtilClient.validate_model(request)
-        return acm_models.SearchOperatorResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.SearchOperatorResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.operator.search', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def create_operator(
         self,
         request: acm_models.CreateOperatorRequest,
     ) -> acm_models.CreateOperatorResponse:
@@ -518,30 +530,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.CreateOperatorResponse:
         """
         Description: 创建操作员
         Summary: 创建操作员
         """
         UtilClient.validate_model(request)
-        return acm_models.CreateOperatorResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.CreateOperatorResponse(),
             self.do_request('1.0', 'antcloud.acm.operator.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def create_operator_ex_async(
         self,
         request: acm_models.CreateOperatorRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.CreateOperatorResponse:
         """
         Description: 创建操作员
         Summary: 创建操作员
         """
         UtilClient.validate_model(request)
-        return acm_models.CreateOperatorResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.CreateOperatorResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.operator.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def update_operator(
         self,
         request: acm_models.UpdateOperatorRequest,
     ) -> acm_models.UpdateOperatorResponse:
@@ -572,30 +586,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.UpdateOperatorResponse:
         """
         Description: 更新操作员
         Summary: 更新操作员
         """
         UtilClient.validate_model(request)
-        return acm_models.UpdateOperatorResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.UpdateOperatorResponse(),
             self.do_request('1.0', 'antcloud.acm.operator.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def update_operator_ex_async(
         self,
         request: acm_models.UpdateOperatorRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.UpdateOperatorResponse:
         """
         Description: 更新操作员
         Summary: 更新操作员
         """
         UtilClient.validate_model(request)
-        return acm_models.UpdateOperatorResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.UpdateOperatorResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.operator.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def delete_operator(
         self,
         request: acm_models.DeleteOperatorRequest,
     ) -> acm_models.DeleteOperatorResponse:
@@ -626,30 +642,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.DeleteOperatorResponse:
         """
         Description: 删除操作员
         Summary: 删除操作员
         """
         UtilClient.validate_model(request)
-        return acm_models.DeleteOperatorResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.DeleteOperatorResponse(),
             self.do_request('1.0', 'antcloud.acm.operator.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def delete_operator_ex_async(
         self,
         request: acm_models.DeleteOperatorRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.DeleteOperatorResponse:
         """
         Description: 删除操作员
         Summary: 删除操作员
         """
         UtilClient.validate_model(request)
-        return acm_models.DeleteOperatorResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.DeleteOperatorResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.operator.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def add_tenant_member(
         self,
         request: acm_models.AddTenantMemberRequest,
     ) -> acm_models.AddTenantMemberResponse:
@@ -680,30 +698,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.AddTenantMemberResponse:
         """
         Description: 添加租户成员
         Summary: 添加租户成员
         """
         UtilClient.validate_model(request)
-        return acm_models.AddTenantMemberResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.AddTenantMemberResponse(),
             self.do_request('1.0', 'antcloud.acm.tenant.member.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def add_tenant_member_ex_async(
         self,
         request: acm_models.AddTenantMemberRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.AddTenantMemberResponse:
         """
         Description: 添加租户成员
         Summary: 添加租户成员
         """
         UtilClient.validate_model(request)
-        return acm_models.AddTenantMemberResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.AddTenantMemberResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.tenant.member.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def create_tenant(
         self,
         request: acm_models.CreateTenantRequest,
     ) -> acm_models.CreateTenantResponse:
@@ -734,30 +754,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.CreateTenantResponse:
         """
         Description: 初始化租户
         Summary: 初始化租户
         """
         UtilClient.validate_model(request)
-        return acm_models.CreateTenantResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.CreateTenantResponse(),
             self.do_request('1.0', 'antcloud.acm.tenant.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def create_tenant_ex_async(
         self,
         request: acm_models.CreateTenantRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.CreateTenantResponse:
         """
         Description: 初始化租户
         Summary: 初始化租户
         """
         UtilClient.validate_model(request)
-        return acm_models.CreateTenantResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.CreateTenantResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.tenant.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def get_tenant(
         self,
         request: acm_models.GetTenantRequest,
     ) -> acm_models.GetTenantResponse:
@@ -788,30 +810,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetTenantResponse:
         """
         Description: 查询租户详情
         Summary: 获取用户信息
         """
         UtilClient.validate_model(request)
-        return acm_models.GetTenantResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetTenantResponse(),
             self.do_request('1.0', 'antcloud.acm.tenant.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_tenant_ex_async(
         self,
         request: acm_models.GetTenantRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetTenantResponse:
         """
         Description: 查询租户详情
         Summary: 获取用户信息
         """
         UtilClient.validate_model(request)
-        return acm_models.GetTenantResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetTenantResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.tenant.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_tenant(
         self,
         request: acm_models.QueryTenantRequest,
     ) -> acm_models.QueryTenantResponse:
@@ -842,30 +866,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.QueryTenantResponse:
         """
         Description: 查询租户列表
         Summary: 查询租户列表
         """
         UtilClient.validate_model(request)
-        return acm_models.QueryTenantResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.QueryTenantResponse(),
             self.do_request('1.0', 'antcloud.acm.tenant.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_tenant_ex_async(
         self,
         request: acm_models.QueryTenantRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.QueryTenantResponse:
         """
         Description: 查询租户列表
         Summary: 查询租户列表
         """
         UtilClient.validate_model(request)
-        return acm_models.QueryTenantResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.QueryTenantResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.tenant.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def get_antpassport_tenant(
         self,
         request: acm_models.GetAntpassportTenantRequest,
     ) -> acm_models.GetAntpassportTenantResponse:
@@ -896,87 +922,35 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetAntpassportTenantResponse:
         """
         Description: 根据蚂蚁通行证uid查询租户id
         Summary: 查询租户ID
         """
         UtilClient.validate_model(request)
-        return acm_models.GetAntpassportTenantResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetAntpassportTenantResponse(),
             self.do_request('1.0', 'antcloud.acm.antpassport.tenant.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_antpassport_tenant_ex_async(
         self,
         request: acm_models.GetAntpassportTenantRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetAntpassportTenantResponse:
         """
         Description: 根据蚂蚁通行证uid查询租户id
         Summary: 查询租户ID
         """
         UtilClient.validate_model(request)
-        return acm_models.GetAntpassportTenantResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetAntpassportTenantResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.antpassport.tenant.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def list_accesskey(
-        self,
-        request: acm_models.ListAccesskeyRequest,
-    ) -> acm_models.ListAccesskeyResponse:
-        """
-        Description: 获取用户AccessKey信息
-        Summary: 获取用户AccessKey信息
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.list_accesskey_ex(request, headers, runtime)
-
-    async def list_accesskey_async(
-        self,
-        request: acm_models.ListAccesskeyRequest,
-    ) -> acm_models.ListAccesskeyResponse:
-        """
-        Description: 获取用户AccessKey信息
-        Summary: 获取用户AccessKey信息
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.list_accesskey_ex_async(request, headers, runtime)
-
-    def list_accesskey_ex(
-        self,
-        request: acm_models.ListAccesskeyRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> acm_models.ListAccesskeyResponse:
-        """
-        Description: 获取用户AccessKey信息
-        Summary: 获取用户AccessKey信息
-        """
-        UtilClient.validate_model(request)
-        return acm_models.ListAccesskeyResponse().from_map(
-            self.do_request('1.0', 'antcloud.acm.accesskey.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def list_accesskey_ex_async(
-        self,
-        request: acm_models.ListAccesskeyRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> acm_models.ListAccesskeyResponse:
-        """
-        Description: 获取用户AccessKey信息
-        Summary: 获取用户AccessKey信息
-        """
-        UtilClient.validate_model(request)
-        return acm_models.ListAccesskeyResponse().from_map(
-            await self.do_request_async('1.0', 'antcloud.acm.accesskey.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
     def get_currentid(
         self,
         request: acm_models.GetCurrentidRequest,
     ) -> acm_models.GetCurrentidResponse:
         """
         Description: 获取调用接口所使用AccessKey对应的身份实体信息
         Summary: 获取调用接口所使用AccessKey对应的身份实体信息
@@ -1004,87 +978,35 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetCurrentidResponse:
         """
         Description: 获取调用接口所使用AccessKey对应的身份实体信息
         Summary: 获取调用接口所使用AccessKey对应的身份实体信息
         """
         UtilClient.validate_model(request)
-        return acm_models.GetCurrentidResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetCurrentidResponse(),
             self.do_request('1.0', 'antcloud.acm.currentid.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_currentid_ex_async(
         self,
         request: acm_models.GetCurrentidRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetCurrentidResponse:
         """
         Description: 获取调用接口所使用AccessKey对应的身份实体信息
         Summary: 获取调用接口所使用AccessKey对应的身份实体信息
         """
         UtilClient.validate_model(request)
-        return acm_models.GetCurrentidResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetCurrentidResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.currentid.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def get_accessor(
-        self,
-        request: acm_models.GetAccessorRequest,
-    ) -> acm_models.GetAccessorResponse:
-        """
-        Description: 获取用户Accessor信息
-        Summary: 获取用户Accessor信息
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.get_accessor_ex(request, headers, runtime)
-
-    async def get_accessor_async(
-        self,
-        request: acm_models.GetAccessorRequest,
-    ) -> acm_models.GetAccessorResponse:
-        """
-        Description: 获取用户Accessor信息
-        Summary: 获取用户Accessor信息
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.get_accessor_ex_async(request, headers, runtime)
-
-    def get_accessor_ex(
-        self,
-        request: acm_models.GetAccessorRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> acm_models.GetAccessorResponse:
-        """
-        Description: 获取用户Accessor信息
-        Summary: 获取用户Accessor信息
-        """
-        UtilClient.validate_model(request)
-        return acm_models.GetAccessorResponse().from_map(
-            self.do_request('1.0', 'antcloud.acm.accessor.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def get_accessor_ex_async(
-        self,
-        request: acm_models.GetAccessorRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> acm_models.GetAccessorResponse:
-        """
-        Description: 获取用户Accessor信息
-        Summary: 获取用户Accessor信息
-        """
-        UtilClient.validate_model(request)
-        return acm_models.GetAccessorResponse().from_map(
-            await self.do_request_async('1.0', 'antcloud.acm.accessor.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
     def get_tenant_dingtoken(
         self,
         request: acm_models.GetTenantDingtokenRequest,
     ) -> acm_models.GetTenantDingtokenResponse:
         """
         Description: 获取租户对应的钉钉授权token信息，内部接口
         Summary: 获取租户的钉钉授权
@@ -1112,30 +1034,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetTenantDingtokenResponse:
         """
         Description: 获取租户对应的钉钉授权token信息，内部接口
         Summary: 获取租户的钉钉授权
         """
         UtilClient.validate_model(request)
-        return acm_models.GetTenantDingtokenResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetTenantDingtokenResponse(),
             self.do_request('1.0', 'antcloud.acm.tenant.dingtoken.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_tenant_dingtoken_ex_async(
         self,
         request: acm_models.GetTenantDingtokenRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetTenantDingtokenResponse:
         """
         Description: 获取租户对应的钉钉授权token信息，内部接口
         Summary: 获取租户的钉钉授权
         """
         UtilClient.validate_model(request)
-        return acm_models.GetTenantDingtokenResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetTenantDingtokenResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.tenant.dingtoken.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_admin(
         self,
         request: acm_models.QueryAdminRequest,
     ) -> acm_models.QueryAdminResponse:
@@ -1166,30 +1090,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.QueryAdminResponse:
         """
         Description: 分页查询管理员，内部接口
         Summary: 分页查询管理员
         """
         UtilClient.validate_model(request)
-        return acm_models.QueryAdminResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.QueryAdminResponse(),
             self.do_request('1.0', 'antcloud.acm.admin.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_admin_ex_async(
         self,
         request: acm_models.QueryAdminRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.QueryAdminResponse:
         """
         Description: 分页查询管理员，内部接口
         Summary: 分页查询管理员
         """
         UtilClient.validate_model(request)
-        return acm_models.QueryAdminResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.QueryAdminResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.admin.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def get_tenant_iaasaccount(
         self,
         request: acm_models.GetTenantIaasaccountRequest,
     ) -> acm_models.GetTenantIaasaccountResponse:
@@ -1220,30 +1146,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetTenantIaasaccountResponse:
         """
         Description: 获取租户的IaaS账号
         Summary: 获取租户的IaaS账号
         """
         UtilClient.validate_model(request)
-        return acm_models.GetTenantIaasaccountResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetTenantIaasaccountResponse(),
             self.do_request('1.0', 'antcloud.acm.tenant.iaasaccount.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_tenant_iaasaccount_ex_async(
         self,
         request: acm_models.GetTenantIaasaccountRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetTenantIaasaccountResponse:
         """
         Description: 获取租户的IaaS账号
         Summary: 获取租户的IaaS账号
         """
         UtilClient.validate_model(request)
-        return acm_models.GetTenantIaasaccountResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetTenantIaasaccountResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.tenant.iaasaccount.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def list_customer(
         self,
         request: acm_models.ListCustomerRequest,
     ) -> acm_models.ListCustomerResponse:
@@ -1274,30 +1202,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.ListCustomerResponse:
         """
         Description: 查询企业列表(内部接口,私有云开放)
         Summary: 查询企业列表
         """
         UtilClient.validate_model(request)
-        return acm_models.ListCustomerResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.ListCustomerResponse(),
             self.do_request('1.0', 'antcloud.acm.customer.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def list_customer_ex_async(
         self,
         request: acm_models.ListCustomerRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.ListCustomerResponse:
         """
         Description: 查询企业列表(内部接口,私有云开放)
         Summary: 查询企业列表
         """
         UtilClient.validate_model(request)
-        return acm_models.ListCustomerResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.ListCustomerResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.customer.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def check_alipay_tenant(
         self,
         request: acm_models.CheckAlipayTenantRequest,
     ) -> acm_models.CheckAlipayTenantResponse:
@@ -1328,30 +1258,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.CheckAlipayTenantResponse:
         """
         Description: 支付宝账号证书信息校验及校验、入驻、打标
         Summary: 支付宝账号证书信息校验、入驻、打标
         """
         UtilClient.validate_model(request)
-        return acm_models.CheckAlipayTenantResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.CheckAlipayTenantResponse(),
             self.do_request('1.0', 'antcloud.acm.alipay.tenant.check', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def check_alipay_tenant_ex_async(
         self,
         request: acm_models.CheckAlipayTenantRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.CheckAlipayTenantResponse:
         """
         Description: 支付宝账号证书信息校验及校验、入驻、打标
         Summary: 支付宝账号证书信息校验、入驻、打标
         """
         UtilClient.validate_model(request)
-        return acm_models.CheckAlipayTenantResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.CheckAlipayTenantResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.alipay.tenant.check', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_tenant_status(
         self,
         request: acm_models.QueryTenantStatusRequest,
     ) -> acm_models.QueryTenantStatusResponse:
@@ -1382,30 +1314,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.QueryTenantStatusResponse:
         """
         Description: 租户入住状态查询
         Summary: 租户入住状态查询
         """
         UtilClient.validate_model(request)
-        return acm_models.QueryTenantStatusResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.QueryTenantStatusResponse(),
             self.do_request('1.0', 'antcloud.acm.tenant.status.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_tenant_status_ex_async(
         self,
         request: acm_models.QueryTenantStatusRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.QueryTenantStatusResponse:
         """
         Description: 租户入住状态查询
         Summary: 租户入住状态查询
         """
         UtilClient.validate_model(request)
-        return acm_models.QueryTenantStatusResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.QueryTenantStatusResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.tenant.status.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def create_antchain_tenant(
         self,
         request: acm_models.CreateAntchainTenantRequest,
     ) -> acm_models.CreateAntchainTenantResponse:
@@ -1436,30 +1370,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.CreateAntchainTenantResponse:
         """
         Description: 账号创建
         Summary: 账号创建
         """
         UtilClient.validate_model(request)
-        return acm_models.CreateAntchainTenantResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.CreateAntchainTenantResponse(),
             self.do_request('1.0', 'antcloud.acm.antchain.tenant.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def create_antchain_tenant_ex_async(
         self,
         request: acm_models.CreateAntchainTenantRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.CreateAntchainTenantResponse:
         """
         Description: 账号创建
         Summary: 账号创建
         """
         UtilClient.validate_model(request)
-        return acm_models.CreateAntchainTenantResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.CreateAntchainTenantResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.antchain.tenant.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def update_customer_identity(
         self,
         request: acm_models.UpdateCustomerIdentityRequest,
     ) -> acm_models.UpdateCustomerIdentityResponse:
@@ -1490,138 +1426,88 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.UpdateCustomerIdentityResponse:
         """
         Description: 客户认证信息更新
         Summary: 客户认证信息更新
         """
         UtilClient.validate_model(request)
-        return acm_models.UpdateCustomerIdentityResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.UpdateCustomerIdentityResponse(),
             self.do_request('1.0', 'antcloud.acm.customer.identity.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def update_customer_identity_ex_async(
         self,
         request: acm_models.UpdateCustomerIdentityRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.UpdateCustomerIdentityResponse:
         """
         Description: 客户认证信息更新
         Summary: 客户认证信息更新
         """
         UtilClient.validate_model(request)
-        return acm_models.UpdateCustomerIdentityResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.UpdateCustomerIdentityResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.customer.identity.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def check_login_id(
-        self,
-        request: acm_models.CheckLoginIdRequest,
-    ) -> acm_models.CheckLoginIdResponse:
-        """
-        Description: 校验邮箱是否可以创建账号
-        Summary: 校验邮箱是否可以创建账号
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.check_login_id_ex(request, headers, runtime)
-
-    async def check_login_id_async(
-        self,
-        request: acm_models.CheckLoginIdRequest,
-    ) -> acm_models.CheckLoginIdResponse:
-        """
-        Description: 校验邮箱是否可以创建账号
-        Summary: 校验邮箱是否可以创建账号
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.check_login_id_ex_async(request, headers, runtime)
-
-    def check_login_id_ex(
-        self,
-        request: acm_models.CheckLoginIdRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> acm_models.CheckLoginIdResponse:
-        """
-        Description: 校验邮箱是否可以创建账号
-        Summary: 校验邮箱是否可以创建账号
-        """
-        UtilClient.validate_model(request)
-        return acm_models.CheckLoginIdResponse().from_map(
-            self.do_request('1.0', 'antcloud.acm.login.id.check', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def check_login_id_ex_async(
-        self,
-        request: acm_models.CheckLoginIdRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> acm_models.CheckLoginIdResponse:
-        """
-        Description: 校验邮箱是否可以创建账号
-        Summary: 校验邮箱是否可以创建账号
-        """
-        UtilClient.validate_model(request)
-        return acm_models.CheckLoginIdResponse().from_map(
-            await self.do_request_async('1.0', 'antcloud.acm.login.id.check', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
     def get_master_tenant(
         self,
         request: acm_models.GetMasterTenantRequest,
     ) -> acm_models.GetMasterTenantResponse:
         """
-        Description: 使用租户ID查询租户信息
-        Summary: 使用租户ID查询租户信息
+        Description: 使用用户ID或用户CODE查询用户信息
+        Summary: 使用用户ID或用户CODE查询用户信息
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_master_tenant_ex(request, headers, runtime)
 
     async def get_master_tenant_async(
         self,
         request: acm_models.GetMasterTenantRequest,
     ) -> acm_models.GetMasterTenantResponse:
         """
-        Description: 使用租户ID查询租户信息
-        Summary: 使用租户ID查询租户信息
+        Description: 使用用户ID或用户CODE查询用户信息
+        Summary: 使用用户ID或用户CODE查询用户信息
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_master_tenant_ex_async(request, headers, runtime)
 
     def get_master_tenant_ex(
         self,
         request: acm_models.GetMasterTenantRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetMasterTenantResponse:
         """
-        Description: 使用租户ID查询租户信息
-        Summary: 使用租户ID查询租户信息
+        Description: 使用用户ID或用户CODE查询用户信息
+        Summary: 使用用户ID或用户CODE查询用户信息
         """
         UtilClient.validate_model(request)
-        return acm_models.GetMasterTenantResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetMasterTenantResponse(),
             self.do_request('1.0', 'antcloud.acm.master.tenant.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_master_tenant_ex_async(
         self,
         request: acm_models.GetMasterTenantRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.GetMasterTenantResponse:
         """
-        Description: 使用租户ID查询租户信息
-        Summary: 使用租户ID查询租户信息
+        Description: 使用用户ID或用户CODE查询用户信息
+        Summary: 使用用户ID或用户CODE查询用户信息
         """
         UtilClient.validate_model(request)
-        return acm_models.GetMasterTenantResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.GetMasterTenantResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.master.tenant.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def check_loginname(
         self,
         request: acm_models.CheckLoginnameRequest,
     ) -> acm_models.CheckLoginnameResponse:
@@ -1652,30 +1538,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.CheckLoginnameResponse:
         """
         Description: 检查邮箱是否可以用来注册
         Summary: 检查邮箱是否可以用来注册
         """
         UtilClient.validate_model(request)
-        return acm_models.CheckLoginnameResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.CheckLoginnameResponse(),
             self.do_request('1.0', 'antcloud.acm.loginname.check', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def check_loginname_ex_async(
         self,
         request: acm_models.CheckLoginnameRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.CheckLoginnameResponse:
         """
         Description: 检查邮箱是否可以用来注册
         Summary: 检查邮箱是否可以用来注册
         """
         UtilClient.validate_model(request)
-        return acm_models.CheckLoginnameResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.CheckLoginnameResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.loginname.check', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_tenant_tag(
         self,
         request: acm_models.QueryTenantTagRequest,
     ) -> acm_models.QueryTenantTagResponse:
@@ -1706,30 +1594,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.QueryTenantTagResponse:
         """
         Description: 查询租户的标签
         Summary: 查询租户的标签列表
         """
         UtilClient.validate_model(request)
-        return acm_models.QueryTenantTagResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.QueryTenantTagResponse(),
             self.do_request('1.0', 'antcloud.acm.tenant.tag.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_tenant_tag_ex_async(
         self,
         request: acm_models.QueryTenantTagRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.QueryTenantTagResponse:
         """
         Description: 查询租户的标签
         Summary: 查询租户的标签列表
         """
         UtilClient.validate_model(request)
-        return acm_models.QueryTenantTagResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.QueryTenantTagResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.tenant.tag.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def add_tenant_businesstag(
         self,
         request: acm_models.AddTenantBusinesstagRequest,
     ) -> acm_models.AddTenantBusinesstagResponse:
@@ -1760,30 +1650,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.AddTenantBusinesstagResponse:
         """
         Description: 租户增加业务标签
         Summary: 租户增加业务标签
         """
         UtilClient.validate_model(request)
-        return acm_models.AddTenantBusinesstagResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.AddTenantBusinesstagResponse(),
             self.do_request('1.0', 'antcloud.acm.tenant.businesstag.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def add_tenant_businesstag_ex_async(
         self,
         request: acm_models.AddTenantBusinesstagRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.AddTenantBusinesstagResponse:
         """
         Description: 租户增加业务标签
         Summary: 租户增加业务标签
         """
         UtilClient.validate_model(request)
-        return acm_models.AddTenantBusinesstagResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.AddTenantBusinesstagResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.tenant.businesstag.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def remove_tenant_businesstag(
         self,
         request: acm_models.RemoveTenantBusinesstagRequest,
     ) -> acm_models.RemoveTenantBusinesstagResponse:
@@ -1814,30 +1706,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.RemoveTenantBusinesstagResponse:
         """
         Description: 删除业务标签
         Summary: 删除业务标签
         """
         UtilClient.validate_model(request)
-        return acm_models.RemoveTenantBusinesstagResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.RemoveTenantBusinesstagResponse(),
             self.do_request('1.0', 'antcloud.acm.tenant.businesstag.remove', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def remove_tenant_businesstag_ex_async(
         self,
         request: acm_models.RemoveTenantBusinesstagRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.RemoveTenantBusinesstagResponse:
         """
         Description: 删除业务标签
         Summary: 删除业务标签
         """
         UtilClient.validate_model(request)
-        return acm_models.RemoveTenantBusinesstagResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.RemoveTenantBusinesstagResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.tenant.businesstag.remove', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def send_operator_activeemail(
         self,
         request: acm_models.SendOperatorActiveemailRequest,
     ) -> acm_models.SendOperatorActiveemailResponse:
@@ -1868,25 +1762,531 @@
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.SendOperatorActiveemailResponse:
         """
         Description: 用户发送操作员的激活邮件
         Summary: 操作员发送激活邮件
         """
         UtilClient.validate_model(request)
-        return acm_models.SendOperatorActiveemailResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.SendOperatorActiveemailResponse(),
             self.do_request('1.0', 'antcloud.acm.operator.activeemail.send', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def send_operator_activeemail_ex_async(
         self,
         request: acm_models.SendOperatorActiveemailRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> acm_models.SendOperatorActiveemailResponse:
         """
         Description: 用户发送操作员的激活邮件
         Summary: 操作员发送激活邮件
         """
         UtilClient.validate_model(request)
-        return acm_models.SendOperatorActiveemailResponse().from_map(
+        return TeaCore.from_map(
+            acm_models.SendOperatorActiveemailResponse(),
             await self.do_request_async('1.0', 'antcloud.acm.operator.activeemail.send', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def sync_tenant_info(
+        self,
+        request: acm_models.SyncTenantInfoRequest,
+    ) -> acm_models.SyncTenantInfoResponse:
+        """
+        Description: 账号信息同步
+        Summary: 账号信息同步
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.sync_tenant_info_ex(request, headers, runtime)
+
+    async def sync_tenant_info_async(
+        self,
+        request: acm_models.SyncTenantInfoRequest,
+    ) -> acm_models.SyncTenantInfoResponse:
+        """
+        Description: 账号信息同步
+        Summary: 账号信息同步
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.sync_tenant_info_ex_async(request, headers, runtime)
+
+    def sync_tenant_info_ex(
+        self,
+        request: acm_models.SyncTenantInfoRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.SyncTenantInfoResponse:
+        """
+        Description: 账号信息同步
+        Summary: 账号信息同步
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.SyncTenantInfoResponse(),
+            self.do_request('1.0', 'antcloud.acm.tenant.info.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def sync_tenant_info_ex_async(
+        self,
+        request: acm_models.SyncTenantInfoRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.SyncTenantInfoResponse:
+        """
+        Description: 账号信息同步
+        Summary: 账号信息同步
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.SyncTenantInfoResponse(),
+            await self.do_request_async('1.0', 'antcloud.acm.tenant.info.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_oauth_serviceaccount(
+        self,
+        request: acm_models.CreateOauthServiceaccountRequest,
+    ) -> acm_models.CreateOauthServiceaccountResponse:
+        """
+        Description: 三方授权创建服务账号
+        Summary: 三方授权创建服务账号
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_oauth_serviceaccount_ex(request, headers, runtime)
+
+    async def create_oauth_serviceaccount_async(
+        self,
+        request: acm_models.CreateOauthServiceaccountRequest,
+    ) -> acm_models.CreateOauthServiceaccountResponse:
+        """
+        Description: 三方授权创建服务账号
+        Summary: 三方授权创建服务账号
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_oauth_serviceaccount_ex_async(request, headers, runtime)
+
+    def create_oauth_serviceaccount_ex(
+        self,
+        request: acm_models.CreateOauthServiceaccountRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.CreateOauthServiceaccountResponse:
+        """
+        Description: 三方授权创建服务账号
+        Summary: 三方授权创建服务账号
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.CreateOauthServiceaccountResponse(),
+            self.do_request('1.0', 'antcloud.acm.oauth.serviceaccount.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_oauth_serviceaccount_ex_async(
+        self,
+        request: acm_models.CreateOauthServiceaccountRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.CreateOauthServiceaccountResponse:
+        """
+        Description: 三方授权创建服务账号
+        Summary: 三方授权创建服务账号
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.CreateOauthServiceaccountResponse(),
+            await self.do_request_async('1.0', 'antcloud.acm.oauth.serviceaccount.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_oauth_serviceaccount(
+        self,
+        request: acm_models.GetOauthServiceaccountRequest,
+    ) -> acm_models.GetOauthServiceaccountResponse:
+        """
+        Description: 三方授权获取服务账号信息
+        Summary: 三方授权获取服务账号信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_oauth_serviceaccount_ex(request, headers, runtime)
+
+    async def get_oauth_serviceaccount_async(
+        self,
+        request: acm_models.GetOauthServiceaccountRequest,
+    ) -> acm_models.GetOauthServiceaccountResponse:
+        """
+        Description: 三方授权获取服务账号信息
+        Summary: 三方授权获取服务账号信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_oauth_serviceaccount_ex_async(request, headers, runtime)
+
+    def get_oauth_serviceaccount_ex(
+        self,
+        request: acm_models.GetOauthServiceaccountRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.GetOauthServiceaccountResponse:
+        """
+        Description: 三方授权获取服务账号信息
+        Summary: 三方授权获取服务账号信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.GetOauthServiceaccountResponse(),
+            self.do_request('1.0', 'antcloud.acm.oauth.serviceaccount.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_oauth_serviceaccount_ex_async(
+        self,
+        request: acm_models.GetOauthServiceaccountRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.GetOauthServiceaccountResponse:
+        """
+        Description: 三方授权获取服务账号信息
+        Summary: 三方授权获取服务账号信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.GetOauthServiceaccountResponse(),
+            await self.do_request_async('1.0', 'antcloud.acm.oauth.serviceaccount.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def enable_oauth_mobilelogin(
+        self,
+        request: acm_models.EnableOauthMobileloginRequest,
+    ) -> acm_models.EnableOauthMobileloginResponse:
+        """
+        Description: 三方授权开通手机号登陆
+        Summary: 三方授权开通手机号登陆
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.enable_oauth_mobilelogin_ex(request, headers, runtime)
+
+    async def enable_oauth_mobilelogin_async(
+        self,
+        request: acm_models.EnableOauthMobileloginRequest,
+    ) -> acm_models.EnableOauthMobileloginResponse:
+        """
+        Description: 三方授权开通手机号登陆
+        Summary: 三方授权开通手机号登陆
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.enable_oauth_mobilelogin_ex_async(request, headers, runtime)
+
+    def enable_oauth_mobilelogin_ex(
+        self,
+        request: acm_models.EnableOauthMobileloginRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.EnableOauthMobileloginResponse:
+        """
+        Description: 三方授权开通手机号登陆
+        Summary: 三方授权开通手机号登陆
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.EnableOauthMobileloginResponse(),
+            self.do_request('1.0', 'antcloud.acm.oauth.mobilelogin.enable', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def enable_oauth_mobilelogin_ex_async(
+        self,
+        request: acm_models.EnableOauthMobileloginRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.EnableOauthMobileloginResponse:
+        """
+        Description: 三方授权开通手机号登陆
+        Summary: 三方授权开通手机号登陆
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.EnableOauthMobileloginResponse(),
+            await self.do_request_async('1.0', 'antcloud.acm.oauth.mobilelogin.enable', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def disable_oauth_mobilelogin(
+        self,
+        request: acm_models.DisableOauthMobileloginRequest,
+    ) -> acm_models.DisableOauthMobileloginResponse:
+        """
+        Description: 三方授权关闭手机号登陆
+        Summary: 三方授权关闭手机号登陆
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.disable_oauth_mobilelogin_ex(request, headers, runtime)
+
+    async def disable_oauth_mobilelogin_async(
+        self,
+        request: acm_models.DisableOauthMobileloginRequest,
+    ) -> acm_models.DisableOauthMobileloginResponse:
+        """
+        Description: 三方授权关闭手机号登陆
+        Summary: 三方授权关闭手机号登陆
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.disable_oauth_mobilelogin_ex_async(request, headers, runtime)
+
+    def disable_oauth_mobilelogin_ex(
+        self,
+        request: acm_models.DisableOauthMobileloginRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.DisableOauthMobileloginResponse:
+        """
+        Description: 三方授权关闭手机号登陆
+        Summary: 三方授权关闭手机号登陆
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.DisableOauthMobileloginResponse(),
+            self.do_request('1.0', 'antcloud.acm.oauth.mobilelogin.disable', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def disable_oauth_mobilelogin_ex_async(
+        self,
+        request: acm_models.DisableOauthMobileloginRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.DisableOauthMobileloginResponse:
+        """
+        Description: 三方授权关闭手机号登陆
+        Summary: 三方授权关闭手机号登陆
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.DisableOauthMobileloginResponse(),
+            await self.do_request_async('1.0', 'antcloud.acm.oauth.mobilelogin.disable', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_serviceaccount_oneparty(
+        self,
+        request: acm_models.CreateServiceaccountOnepartyRequest,
+    ) -> acm_models.CreateServiceaccountOnepartyResponse:
+        """
+        Description: 提供给一方化平台代客创建服务账号（ak sk）
+        Summary: 一方化会员服务账号创建
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_serviceaccount_oneparty_ex(request, headers, runtime)
+
+    async def create_serviceaccount_oneparty_async(
+        self,
+        request: acm_models.CreateServiceaccountOnepartyRequest,
+    ) -> acm_models.CreateServiceaccountOnepartyResponse:
+        """
+        Description: 提供给一方化平台代客创建服务账号（ak sk）
+        Summary: 一方化会员服务账号创建
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_serviceaccount_oneparty_ex_async(request, headers, runtime)
+
+    def create_serviceaccount_oneparty_ex(
+        self,
+        request: acm_models.CreateServiceaccountOnepartyRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.CreateServiceaccountOnepartyResponse:
+        """
+        Description: 提供给一方化平台代客创建服务账号（ak sk）
+        Summary: 一方化会员服务账号创建
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.CreateServiceaccountOnepartyResponse(),
+            self.do_request('1.0', 'antcloud.acm.serviceaccount.oneparty.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_serviceaccount_oneparty_ex_async(
+        self,
+        request: acm_models.CreateServiceaccountOnepartyRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.CreateServiceaccountOnepartyResponse:
+        """
+        Description: 提供给一方化平台代客创建服务账号（ak sk）
+        Summary: 一方化会员服务账号创建
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.CreateServiceaccountOnepartyResponse(),
+            await self.do_request_async('1.0', 'antcloud.acm.serviceaccount.oneparty.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_serviceaccount_oneparty(
+        self,
+        request: acm_models.GetServiceaccountOnepartyRequest,
+    ) -> acm_models.GetServiceaccountOnepartyResponse:
+        """
+        Description: 一方化会员服务账号查询（ak sk）
+        Summary: 一方化会员服务账号查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_serviceaccount_oneparty_ex(request, headers, runtime)
+
+    async def get_serviceaccount_oneparty_async(
+        self,
+        request: acm_models.GetServiceaccountOnepartyRequest,
+    ) -> acm_models.GetServiceaccountOnepartyResponse:
+        """
+        Description: 一方化会员服务账号查询（ak sk）
+        Summary: 一方化会员服务账号查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_serviceaccount_oneparty_ex_async(request, headers, runtime)
+
+    def get_serviceaccount_oneparty_ex(
+        self,
+        request: acm_models.GetServiceaccountOnepartyRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.GetServiceaccountOnepartyResponse:
+        """
+        Description: 一方化会员服务账号查询（ak sk）
+        Summary: 一方化会员服务账号查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.GetServiceaccountOnepartyResponse(),
+            self.do_request('1.0', 'antcloud.acm.serviceaccount.oneparty.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_serviceaccount_oneparty_ex_async(
+        self,
+        request: acm_models.GetServiceaccountOnepartyRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.GetServiceaccountOnepartyResponse:
+        """
+        Description: 一方化会员服务账号查询（ak sk）
+        Summary: 一方化会员服务账号查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.GetServiceaccountOnepartyResponse(),
+            await self.do_request_async('1.0', 'antcloud.acm.serviceaccount.oneparty.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def apply_trustlogin_token(
+        self,
+        request: acm_models.ApplyTrustloginTokenRequest,
+    ) -> acm_models.ApplyTrustloginTokenResponse:
+        """
+        Description: token用于三方会员免密登录，与数科官网token不通用
+        Summary: 三方会员免密登录token申请
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.apply_trustlogin_token_ex(request, headers, runtime)
+
+    async def apply_trustlogin_token_async(
+        self,
+        request: acm_models.ApplyTrustloginTokenRequest,
+    ) -> acm_models.ApplyTrustloginTokenResponse:
+        """
+        Description: token用于三方会员免密登录，与数科官网token不通用
+        Summary: 三方会员免密登录token申请
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.apply_trustlogin_token_ex_async(request, headers, runtime)
+
+    def apply_trustlogin_token_ex(
+        self,
+        request: acm_models.ApplyTrustloginTokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.ApplyTrustloginTokenResponse:
+        """
+        Description: token用于三方会员免密登录，与数科官网token不通用
+        Summary: 三方会员免密登录token申请
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.ApplyTrustloginTokenResponse(),
+            self.do_request('1.0', 'antcloud.acm.trustlogin.token.apply', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def apply_trustlogin_token_ex_async(
+        self,
+        request: acm_models.ApplyTrustloginTokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.ApplyTrustloginTokenResponse:
+        """
+        Description: token用于三方会员免密登录，与数科官网token不通用
+        Summary: 三方会员免密登录token申请
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.ApplyTrustloginTokenResponse(),
+            await self.do_request_async('1.0', 'antcloud.acm.trustlogin.token.apply', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def verify_trustlogin_token(
+        self,
+        request: acm_models.VerifyTrustloginTokenRequest,
+    ) -> acm_models.VerifyTrustloginTokenResponse:
+        """
+        Description: 三方会员免密登录token校验，与数科官网token不通用
+        Summary: 三方会员免密登录token校验
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.verify_trustlogin_token_ex(request, headers, runtime)
+
+    async def verify_trustlogin_token_async(
+        self,
+        request: acm_models.VerifyTrustloginTokenRequest,
+    ) -> acm_models.VerifyTrustloginTokenResponse:
+        """
+        Description: 三方会员免密登录token校验，与数科官网token不通用
+        Summary: 三方会员免密登录token校验
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.verify_trustlogin_token_ex_async(request, headers, runtime)
+
+    def verify_trustlogin_token_ex(
+        self,
+        request: acm_models.VerifyTrustloginTokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.VerifyTrustloginTokenResponse:
+        """
+        Description: 三方会员免密登录token校验，与数科官网token不通用
+        Summary: 三方会员免密登录token校验
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.VerifyTrustloginTokenResponse(),
+            self.do_request('1.0', 'antcloud.acm.trustlogin.token.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def verify_trustlogin_token_ex_async(
+        self,
+        request: acm_models.VerifyTrustloginTokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> acm_models.VerifyTrustloginTokenResponse:
+        """
+        Description: 三方会员免密登录token校验，与数科官网token不通用
+        Summary: 三方会员免密登录token校验
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            acm_models.VerifyTrustloginTokenResponse(),
+            await self.do_request_async('1.0', 'antcloud.acm.trustlogin.token.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_acm-1.0.23/antchain_sdk_acm/models.py` & `antchain_acm-1.3.3/antchain_sdk_acm/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,14 +66,18 @@
         # 每个目标主机的最大连接数（分主机域名的长链接最大总数
         self.max_requests_per_host = max_requests_per_host
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.access_key_id is not None:
             result['accessKeyId'] = self.access_key_id
         if self.access_key_secret is not None:
             result['accessKeySecret'] = self.access_key_secret
         if self.security_token is not None:
             result['securityToken'] = self.security_token
@@ -173,14 +177,18 @@
         # Accessor类型(RAM/ACCOUNT)
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.access_key is not None:
             result['access_key'] = self.access_key
         if self.access_secret is not None:
             result['access_secret'] = self.access_secret
         if self.account is not None:
             result['account'] = self.account
@@ -221,14 +229,18 @@
         self.tag_value = tag_value
 
     def validate(self):
         self.validate_required(self.tag_type, 'tag_type')
         self.validate_required(self.tag_value, 'tag_value')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.tag_type is not None:
             result['tag_type'] = self.tag_type
         if self.tag_value is not None:
             result['tag_value'] = self.tag_value
         return result
 
@@ -261,14 +273,18 @@
         # AccessKey最近一次修改时间，ISO8601格式
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.create_time is not None:
             result['create_time'] = self.create_time
         if self.id is not None:
             result['id'] = self.id
         if self.secret is not None:
             result['secret'] = self.secret
@@ -310,14 +326,18 @@
         # 企业最近一次修改时间，ISO8601格式
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.create_time is not None:
             result['create_time'] = self.create_time
         if self.id is not None:
             result['id'] = self.id
         if self.name is not None:
             result['name'] = self.name
@@ -373,14 +393,18 @@
         # 租户最近一次修改时间，ISO8601格式
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.ant_account is not None:
             result['ant_account'] = self.ant_account
         if self.ant_uid is not None:
             result['ant_uid'] = self.ant_uid
         if self.business_owner_id is not None:
             result['business_owner_id'] = self.business_owner_id
@@ -472,14 +496,18 @@
         # 操作员最近一次修改时间，ISO8601格式
         self.update_time = update_time
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.create_time is not None:
             result['create_time'] = self.create_time
         if self.customer is not None:
             result['customer'] = self.customer
         if self.email is not None:
             result['email'] = self.email
@@ -551,14 +579,18 @@
         # 企业ID
         self.customer = customer
 
     def validate(self):
         self.validate_required(self.customer, 'customer')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.customer is not None:
             result['customer'] = self.customer
         return result
 
@@ -598,14 +630,18 @@
         self.update_time = update_time
 
     def validate(self):
         self.validate_required(self.id, 'id')
         self.validate_required(self.name, 'name')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -652,14 +688,18 @@
         # 金融云操作员id
         self.operator_id = operator_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.login_name is not None:
             result['login_name'] = self.login_name
         if self.operator_id is not None:
             result['operator_id'] = self.operator_id
@@ -747,14 +787,18 @@
         self.validate_required(self.login_name, 'login_name')
         self.validate_required(self.mobile, 'mobile')
         self.validate_required(self.nickname, 'nickname')
         self.validate_required(self.real_name, 'real_name')
         self.validate_required(self.status, 'status')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -861,14 +905,18 @@
         # 部门唯一码
         self.department_code = department_code
 
     def validate(self):
         self.validate_required(self.customer, 'customer')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.customer is not None:
             result['customer'] = self.customer
         if self.page_num is not None:
             result['page_num'] = self.page_num
@@ -934,14 +982,18 @@
                 if k:
                     k.validate()
         self.validate_required(self.page_num, 'page_num')
         self.validate_required(self.page_size, 'page_size')
         self.validate_required(self.total_count, 'total_count')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1008,14 +1060,18 @@
         # 租户唯一标识
         self.tenant = tenant
 
     def validate(self):
         self.validate_required(self.customer, 'customer')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.customer is not None:
             result['customer'] = self.customer
         if self.login_name is not None:
             result['login_name'] = self.login_name
@@ -1085,14 +1141,18 @@
                 if k:
                     k.validate()
         self.validate_required(self.page_num, 'page_num')
         self.validate_required(self.page_size, 'page_size')
         self.validate_required(self.total_count, 'total_count')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1175,14 +1235,18 @@
         self.reset_password_when_first_login = reset_password_when_first_login
 
     def validate(self):
         self.validate_required(self.login_name, 'login_name')
         self.validate_required(self.real_name, 'real_name')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.customer is not None:
             result['customer'] = self.customer
         if self.external_id is not None:
             result['external_id'] = self.external_id
@@ -1256,14 +1320,18 @@
         # 操作员唯一ID
         self.operator_id = operator_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1307,14 +1375,18 @@
         # 操作员真实姓名
         self.real_name = real_name
 
     def validate(self):
         self.validate_required(self.operator_id, 'operator_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.email is not None:
             result['email'] = self.email
         if self.mobile is not None:
             result['mobile'] = self.mobile
@@ -1398,14 +1470,18 @@
         self.validate_required(self.mobile, 'mobile')
         self.validate_required(self.nickname, 'nickname')
         self.validate_required(self.real_name, 'real_name')
         self.validate_required(self.status, 'status')
         self.validate_required(self.tenants, 'tenants')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1477,14 +1553,18 @@
         # 操作员唯一id
         self.operator_id = operator_id
 
     def validate(self):
         self.validate_required(self.operator_id, 'operator_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.operator_id is not None:
             result['operator_id'] = self.operator_id
         return result
 
@@ -1511,14 +1591,18 @@
         # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1550,14 +1634,18 @@
         self.tenant = tenant
 
     def validate(self):
         self.validate_required(self.operator_id, 'operator_id')
         self.validate_required(self.tenant, 'tenant')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.operator_id is not None:
             result['operator_id'] = self.operator_id
         if self.tenant is not None:
             result['tenant'] = self.tenant
@@ -1588,14 +1676,18 @@
         # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1635,14 +1727,18 @@
         # 描述信息
         self.description = description
 
     def validate(self):
         self.validate_required(self.ant_uid, 'ant_uid')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.ant_uid is not None:
             result['ant_uid'] = self.ant_uid
         if self.business_owner_id is not None:
             result['business_owner_id'] = self.business_owner_id
@@ -1688,14 +1784,18 @@
         # 租户唯一标识
         self.tenant = tenant
 
     def validate(self):
         self.validate_required(self.tenant, 'tenant')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1727,14 +1827,18 @@
         # 租户唯一标识
         self.tenant = tenant
 
     def validate(self):
         self.validate_required(self.tenant, 'tenant')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.tenant is not None:
             result['tenant'] = self.tenant
         return result
 
@@ -1792,14 +1896,18 @@
         self.update_time = update_time
 
     def validate(self):
         self.validate_required(self.ant_account, 'ant_account')
         self.validate_required(self.business_owner_id, 'business_owner_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1873,14 +1981,18 @@
         # 分页大小，默认值为10
         self.page_size = page_size
 
     def validate(self):
         self.validate_required(self.customer, 'customer')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.customer is not None:
             result['customer'] = self.customer
         if self.page_num is not None:
             result['page_num'] = self.page_num
@@ -1934,14 +2046,18 @@
         if self.tenants:
             for k in self.tenants:
                 if k:
                     k.validate()
         self.validate_required(self.total_count, 'total_count')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1990,14 +2106,18 @@
         # 蚂蚁通行证uid
         self.ant_uid = ant_uid
 
     def validate(self):
         self.validate_required(self.ant_uid, 'ant_uid')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.ant_uid is not None:
             result['ant_uid'] = self.ant_uid
         return result
 
@@ -2026,14 +2146,18 @@
         self.result_msg = result_msg
         self.tenant = tenant
 
     def validate(self):
         self.validate_required(self.tenant, 'tenant')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2050,111 +2174,30 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('tenant') is not None:
             self.tenant = m.get('tenant')
         return self
 
 
-class ListAccesskeyRequest(TeaModel):
-    def __init__(
-        self,
-        auth_token: str = None,
-        user_id: str = None,
-    ):
-        # OAuth模式下的授权token
-        self.auth_token = auth_token
-        # 操作员或服务账号唯一ID
-        self.user_id = user_id
-
-    def validate(self):
-        self.validate_required(self.user_id, 'user_id')
-
-    def to_map(self):
-        result = dict()
-        if self.auth_token is not None:
-            result['auth_token'] = self.auth_token
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('auth_token') is not None:
-            self.auth_token = m.get('auth_token')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        return self
-
-
-class ListAccesskeyResponse(TeaModel):
-    def __init__(
-        self,
-        req_msg_id: str = None,
-        result_code: str = None,
-        result_msg: str = None,
-        access_keys: List[AccessKey] = None,
-    ):
-        # 请求唯一ID，用于链路跟踪和问题排查
-        self.req_msg_id = req_msg_id
-        # 结果码，一般OK表示调用成功
-        self.result_code = result_code
-        # 异常信息的文本描述
-        self.result_msg = result_msg
-        # AccessKey列表
-        self.access_keys = access_keys
-
-    def validate(self):
-        self.validate_required(self.access_keys, 'access_keys')
-        if self.access_keys:
-            for k in self.access_keys:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        result = dict()
-        if self.req_msg_id is not None:
-            result['req_msg_id'] = self.req_msg_id
-        if self.result_code is not None:
-            result['result_code'] = self.result_code
-        if self.result_msg is not None:
-            result['result_msg'] = self.result_msg
-        result['access_keys'] = []
-        if self.access_keys is not None:
-            for k in self.access_keys:
-                result['access_keys'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('req_msg_id') is not None:
-            self.req_msg_id = m.get('req_msg_id')
-        if m.get('result_code') is not None:
-            self.result_code = m.get('result_code')
-        if m.get('result_msg') is not None:
-            self.result_msg = m.get('result_msg')
-        self.access_keys = []
-        if m.get('access_keys') is not None:
-            for k in m.get('access_keys'):
-                temp_model = AccessKey()
-                self.access_keys.append(temp_model.from_map(k))
-        return self
-
-
 class GetCurrentidRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
@@ -2196,14 +2239,18 @@
         self.validate_required(self.create_time, 'create_time')
         self.validate_required(self.customer, 'customer')
         self.validate_required(self.id, 'id')
         self.validate_required(self.type, 'type')
         self.validate_required(self.update_time, 'update_time')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2236,153 +2283,14 @@
         if m.get('type') is not None:
             self.type = m.get('type')
         if m.get('update_time') is not None:
             self.update_time = m.get('update_time')
         return self
 
 
-class GetAccessorRequest(TeaModel):
-    def __init__(
-        self,
-        auth_token: str = None,
-        access_key_id: str = None,
-        tenant: str = None,
-        user_id: str = None,
-    ):
-        # OAuth模式下的授权token
-        self.auth_token = auth_token
-        # Accessor关联的accessKey
-        self.access_key_id = access_key_id
-        # 租户唯一标识
-        self.tenant = tenant
-        # 操作员或服务账号唯一ID
-        self.user_id = user_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        result = dict()
-        if self.auth_token is not None:
-            result['auth_token'] = self.auth_token
-        if self.access_key_id is not None:
-            result['access_key_id'] = self.access_key_id
-        if self.tenant is not None:
-            result['tenant'] = self.tenant
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('auth_token') is not None:
-            self.auth_token = m.get('auth_token')
-        if m.get('access_key_id') is not None:
-            self.access_key_id = m.get('access_key_id')
-        if m.get('tenant') is not None:
-            self.tenant = m.get('tenant')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        return self
-
-
-class GetAccessorResponse(TeaModel):
-    def __init__(
-        self,
-        req_msg_id: str = None,
-        result_code: str = None,
-        result_msg: str = None,
-        access_key: str = None,
-        access_secret: str = None,
-        account: str = None,
-        create_time: str = None,
-        id: str = None,
-        tenant: str = None,
-        type: str = None,
-        user_id: str = None,
-    ):
-        # 请求唯一ID，用于链路跟踪和问题排查
-        self.req_msg_id = req_msg_id
-        # 结果码，一般OK表示调用成功
-        self.result_code = result_code
-        # 异常信息的文本描述
-        self.result_msg = result_msg
-        # Accessor关联的AccessKey
-        self.access_key = access_key
-        # Accessor关联的AccessKey的密钥，加密传输，网关返回后，使用调用方的AccessSecret进行解密
-        self.access_secret = access_secret
-        # AccessKey的密钥，加密传输，网关返回后，使用调用方的AccessSecret进行解密
-        self.account = account
-        # AccessKey创建时间，ISO8601格式
-        self.create_time = create_time
-        # Accessor唯一标识
-        self.id = id
-        # 关联的租户
-        self.tenant = tenant
-        # Accessor类型(RAM/ACCOUNT)
-        self.type = type
-        # 关联的用户ID
-        self.user_id = user_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        result = dict()
-        if self.req_msg_id is not None:
-            result['req_msg_id'] = self.req_msg_id
-        if self.result_code is not None:
-            result['result_code'] = self.result_code
-        if self.result_msg is not None:
-            result['result_msg'] = self.result_msg
-        if self.access_key is not None:
-            result['access_key'] = self.access_key
-        if self.access_secret is not None:
-            result['access_secret'] = self.access_secret
-        if self.account is not None:
-            result['account'] = self.account
-        if self.create_time is not None:
-            result['create_time'] = self.create_time
-        if self.id is not None:
-            result['id'] = self.id
-        if self.tenant is not None:
-            result['tenant'] = self.tenant
-        if self.type is not None:
-            result['type'] = self.type
-        if self.user_id is not None:
-            result['userId'] = self.user_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('req_msg_id') is not None:
-            self.req_msg_id = m.get('req_msg_id')
-        if m.get('result_code') is not None:
-            self.result_code = m.get('result_code')
-        if m.get('result_msg') is not None:
-            self.result_msg = m.get('result_msg')
-        if m.get('access_key') is not None:
-            self.access_key = m.get('access_key')
-        if m.get('access_secret') is not None:
-            self.access_secret = m.get('access_secret')
-        if m.get('account') is not None:
-            self.account = m.get('account')
-        if m.get('create_time') is not None:
-            self.create_time = m.get('create_time')
-        if m.get('id') is not None:
-            self.id = m.get('id')
-        if m.get('tenant') is not None:
-            self.tenant = m.get('tenant')
-        if m.get('type') is not None:
-            self.type = m.get('type')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
-        return self
-
-
 class GetTenantDingtokenRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product: str = None,
         tenant: str = None,
     ):
@@ -2394,14 +2302,18 @@
         self.tenant = tenant
 
     def validate(self):
         self.validate_required(self.product, 'product')
         self.validate_required(self.tenant, 'tenant')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product is not None:
             result['product'] = self.product
         if self.tenant is not None:
             result['tenant'] = self.tenant
@@ -2453,14 +2365,18 @@
     def validate(self):
         self.validate_required(self.access_token, 'access_token')
         self.validate_required(self.agent_id, 'agent_id')
         self.validate_required(self.corp_id, 'corp_id')
         self.validate_required(self.js_ticket, 'js_ticket')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2512,14 +2428,18 @@
         # 租户唯一标识
         self.tenant = tenant
 
     def validate(self):
         self.validate_required(self.tenant, 'tenant')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.tenant is not None:
             result['tenant'] = self.tenant
         return result
 
@@ -2553,14 +2473,18 @@
         self.validate_required(self.operators, 'operators')
         if self.operators:
             for k in self.operators:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2600,14 +2524,18 @@
         # 一方化调用参数，阿里云服务名
         self.source_id = source_id
 
     def validate(self):
         self.validate_required(self.tenant, 'tenant')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.tenant is not None:
             result['tenant'] = self.tenant
         if self.source_id is not None:
             result['source_id'] = self.source_id
@@ -2659,14 +2587,18 @@
         # 是否是sts模式
         self.sts_mode = sts_mode
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2719,14 +2651,18 @@
         # OAuth模式下的授权token
         self.auth_token = auth_token
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
@@ -2756,14 +2692,18 @@
         self.validate_required(self.customers, 'customers')
         if self.customers:
             for k in self.customers:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2817,14 +2757,18 @@
 
     def validate(self):
         self.validate_required(self.channel_code, 'channel_code')
         self.validate_required(self.scene_code, 'scene_code')
         self.validate_required(self.tenant_id, 'tenant_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.cert_no is not None:
             result['cert_no'] = self.cert_no
         if self.channel_code is not None:
             result['channel_code'] = self.channel_code
@@ -2874,14 +2818,18 @@
         # 智科租户id(支付宝会员id)
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2921,14 +2869,18 @@
 
     def validate(self):
         self.validate_required(self.channel_code, 'channel_code')
         self.validate_required(self.scene_code, 'scene_code')
         self.validate_required(self.tenant_id, 'tenant_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.channel_code is not None:
             result['channel_code'] = self.channel_code
         if self.scene_code is not None:
             result['scene_code'] = self.scene_code
@@ -2969,14 +2921,18 @@
         # 智科租户id（支付宝会员id）
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3056,14 +3012,18 @@
     def validate(self):
         self.validate_required(self.name, 'name')
         self.validate_required(self.user_type, 'user_type')
         self.validate_required(self.bussiness_code, 'bussiness_code')
         self.validate_required(self.is_alipay_tenant, 'is_alipay_tenant')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.name is not None:
             result['name'] = self.name
         if self.user_type is not None:
             result['user_type'] = self.user_type
@@ -3148,14 +3108,18 @@
         # 客户id
         self.customer_id = customer_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3221,14 +3185,18 @@
     def validate(self):
         self.validate_required(self.name, 'name')
         self.validate_required(self.cert_no, 'cert_no')
         self.validate_required(self.cert_type, 'cert_type')
         self.validate_required(self.business_code, 'business_code')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.customer_id is not None:
             result['customer_id'] = self.customer_id
         if self.name is not None:
             result['name'] = self.name
@@ -3294,14 +3262,18 @@
         # 返回客户id
         self.customer_id = customer_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3318,97 +3290,14 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('customer_id') is not None:
             self.customer_id = m.get('customer_id')
         return self
 
 
-class CheckLoginIdRequest(TeaModel):
-    def __init__(
-        self,
-        auth_token: str = None,
-        login_name: str = None,
-    ):
-        # OAuth模式下的授权token
-        self.auth_token = auth_token
-        # 登录id
-        self.login_name = login_name
-
-    def validate(self):
-        self.validate_required(self.login_name, 'login_name')
-
-    def to_map(self):
-        result = dict()
-        if self.auth_token is not None:
-            result['auth_token'] = self.auth_token
-        if self.login_name is not None:
-            result['login_name'] = self.login_name
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('auth_token') is not None:
-            self.auth_token = m.get('auth_token')
-        if m.get('login_name') is not None:
-            self.login_name = m.get('login_name')
-        return self
-
-
-class CheckLoginIdResponse(TeaModel):
-    def __init__(
-        self,
-        req_msg_id: str = None,
-        result_code: str = None,
-        result_msg: str = None,
-        exist: bool = None,
-        tenant_id: str = None,
-    ):
-        # 请求唯一ID，用于链路跟踪和问题排查
-        self.req_msg_id = req_msg_id
-        # 结果码，一般OK表示调用成功
-        self.result_code = result_code
-        # 异常信息的文本描述
-        self.result_msg = result_msg
-        # 是否存在
-        self.exist = exist
-        # 所属的租户id
-        self.tenant_id = tenant_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        result = dict()
-        if self.req_msg_id is not None:
-            result['req_msg_id'] = self.req_msg_id
-        if self.result_code is not None:
-            result['result_code'] = self.result_code
-        if self.result_msg is not None:
-            result['result_msg'] = self.result_msg
-        if self.exist is not None:
-            result['exist'] = self.exist
-        if self.tenant_id is not None:
-            result['tenant_id'] = self.tenant_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('req_msg_id') is not None:
-            self.req_msg_id = m.get('req_msg_id')
-        if m.get('result_code') is not None:
-            self.result_code = m.get('result_code')
-        if m.get('result_msg') is not None:
-            self.result_msg = m.get('result_msg')
-        if m.get('exist') is not None:
-            self.exist = m.get('exist')
-        if m.get('tenant_id') is not None:
-            self.tenant_id = m.get('tenant_id')
-        return self
-
-
 class GetMasterTenantRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         tenant_id: str = None,
         name: str = None,
     ):
@@ -3419,14 +3308,18 @@
         # 用户CODE
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
         if self.name is not None:
             result['name'] = self.name
@@ -3496,14 +3389,18 @@
         # 企业姓名
         self.firm_name = firm_name
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3583,14 +3480,18 @@
         # 邮箱名称
         self.login_name = login_name
 
     def validate(self):
         self.validate_required(self.login_name, 'login_name')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.login_name is not None:
             result['login_name'] = self.login_name
         return result
 
@@ -3623,14 +3524,18 @@
         # 所属租户ID
         self.tenant_id = tenant_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3666,14 +3571,18 @@
         # 租户id
         self.tenant_id = tenant_id
 
     def validate(self):
         self.validate_required(self.tenant_id, 'tenant_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
         return result
 
@@ -3706,14 +3615,18 @@
     def validate(self):
         if self.tags:
             for k in self.tags:
                 if k:
                     k.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3758,14 +3671,18 @@
 
     def validate(self):
         self.validate_required(self.tenant_id, 'tenant_id')
         self.validate_required(self.business_code, 'business_code')
         self.validate_required(self.auth_code, 'auth_code')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
         if self.business_code is not None:
             result['business_code'] = self.business_code
@@ -3800,14 +3717,18 @@
         # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3843,14 +3764,18 @@
 
     def validate(self):
         self.validate_required(self.tenant_id, 'tenant_id')
         self.validate_required(self.business_code, 'business_code')
         self.validate_required(self.auth_code, 'auth_code')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
         if self.business_code is not None:
             result['business_code'] = self.business_code
@@ -3885,14 +3810,18 @@
         # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3920,14 +3849,18 @@
         # 操作员ID
         self.operator_id = operator_id
 
     def validate(self):
         self.validate_required(self.operator_id, 'operator_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.operator_id is not None:
             result['operator_id'] = self.operator_id
         return result
 
@@ -3954,27 +3887,990 @@
         # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class SyncTenantInfoRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        tenant_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 账号ID
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        return self
+
+
+class SyncTenantInfoResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class CreateOauthServiceaccountRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        access_token: str = None,
+        description: str = None,
+        alias: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 三方授权凭证
+        self.access_token = access_token
+        # 服务账号描述
+        self.description = description
+        # 服务账号别名
+        self.alias = alias
+
+    def validate(self):
+        self.validate_required(self.access_token, 'access_token')
+        self.validate_required(self.description, 'description')
+        self.validate_required(self.alias, 'alias')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.access_token is not None:
+            result['access_token'] = self.access_token
+        if self.description is not None:
+            result['description'] = self.description
+        if self.alias is not None:
+            result['alias'] = self.alias
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('access_token') is not None:
+            self.access_token = m.get('access_token')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('alias') is not None:
+            self.alias = m.get('alias')
+        return self
+
+
+class CreateOauthServiceaccountResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        id: str = None,
+        description: str = None,
+        alias: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 服务账号ID
+        self.id = id
+        # 服务账号描述
+        self.description = description
+        # 服务账号别名
+        self.alias = alias
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
+        if self.id is not None:
+            result['id'] = self.id
+        if self.description is not None:
+            result['description'] = self.description
+        if self.alias is not None:
+            result['alias'] = self.alias
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('alias') is not None:
+            self.alias = m.get('alias')
+        return self
+
+
+class GetOauthServiceaccountRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        access_token: str = None,
+        service_account_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 三方授权凭证
+        self.access_token = access_token
+        # 服务账号ID
+        self.service_account_id = service_account_id
+
+    def validate(self):
+        self.validate_required(self.access_token, 'access_token')
+        self.validate_required(self.service_account_id, 'service_account_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.access_token is not None:
+            result['access_token'] = self.access_token
+        if self.service_account_id is not None:
+            result['service_account_id'] = self.service_account_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('access_token') is not None:
+            self.access_token = m.get('access_token')
+        if m.get('service_account_id') is not None:
+            self.service_account_id = m.get('service_account_id')
+        return self
+
+
+class GetOauthServiceaccountResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        access_key: str = None,
+        access_secret: str = None,
+        alias: str = None,
+        description: str = None,
+        id: str = None,
+        name: str = None,
+        tenant_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 服务账号AK
+        self.access_key = access_key
+        # 服务账号SK
+        self.access_secret = access_secret
+        # 服务账号别名
+        self.alias = alias
+        # 服务账号描述
+        self.description = description
+        # 服务账号ID
+        self.id = id
+        # 服务名称
+        self.name = name
+        # 服务账号归属的账号ID
+        self.tenant_id = tenant_id
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.access_key is not None:
+            result['access_key'] = self.access_key
+        if self.access_secret is not None:
+            result['access_secret'] = self.access_secret
+        if self.alias is not None:
+            result['alias'] = self.alias
+        if self.description is not None:
+            result['description'] = self.description
+        if self.id is not None:
+            result['id'] = self.id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('access_key') is not None:
+            self.access_key = m.get('access_key')
+        if m.get('access_secret') is not None:
+            self.access_secret = m.get('access_secret')
+        if m.get('alias') is not None:
+            self.alias = m.get('alias')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        return self
+
+
+class EnableOauthMobileloginRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        access_token: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 三方授权凭证
+        self.access_token = access_token
+
+    def validate(self):
+        self.validate_required(self.access_token, 'access_token')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.access_token is not None:
+            result['access_token'] = self.access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('access_token') is not None:
+            self.access_token = m.get('access_token')
+        return self
+
+
+class EnableOauthMobileloginResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class DisableOauthMobileloginRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        access_token: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 三方授权凭证
+        self.access_token = access_token
+
+    def validate(self):
+        self.validate_required(self.access_token, 'access_token')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.access_token is not None:
+            result['access_token'] = self.access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('access_token') is not None:
+            self.access_token = m.get('access_token')
+        return self
+
+
+class DisableOauthMobileloginResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class CreateServiceaccountOnepartyRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        tenant_id: str = None,
+        source_system: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 租户ID
+        self.tenant_id = tenant_id
+        # 系统来源
+        self.source_system = source_system
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.source_system, 'source_system')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.source_system is not None:
+            result['source_system'] = self.source_system
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('source_system') is not None:
+            self.source_system = m.get('source_system')
+        return self
+
+
+class CreateServiceaccountOnepartyResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        access_key: str = None,
+        access_secret: str = None,
+        user_id: str = None,
+        user_type: str = None,
+        status: str = None,
+        tenant_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # accessKey
+        self.access_key = access_key
+        # accessSecret
+        self.access_secret = access_secret
+        # 用户ID
+        self.user_id = user_id
+        # 用户类型
+        self.user_type = user_type
+        # ak状态
+        self.status = status
+        # 租户ID
+        self.tenant_id = tenant_id
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.access_key is not None:
+            result['access_key'] = self.access_key
+        if self.access_secret is not None:
+            result['access_secret'] = self.access_secret
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.user_type is not None:
+            result['user_type'] = self.user_type
+        if self.status is not None:
+            result['status'] = self.status
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('access_key') is not None:
+            self.access_key = m.get('access_key')
+        if m.get('access_secret') is not None:
+            self.access_secret = m.get('access_secret')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('user_type') is not None:
+            self.user_type = m.get('user_type')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        return self
+
+
+class GetServiceaccountOnepartyRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        tenant_id: str = None,
+        source_system: str = None,
+        iam_access_key: str = None,
+        user_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 租户ID
+        self.tenant_id = tenant_id
+        # 系统来源
+        self.source_system = source_system
+        # accessKey
+        self.iam_access_key = iam_access_key
+        # 用户id（服务账号）。和iam_access_key参数二选一
+        self.user_id = user_id
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.source_system, 'source_system')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.source_system is not None:
+            result['source_system'] = self.source_system
+        if self.iam_access_key is not None:
+            result['iam_access_key'] = self.iam_access_key
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('source_system') is not None:
+            self.source_system = m.get('source_system')
+        if m.get('iam_access_key') is not None:
+            self.iam_access_key = m.get('iam_access_key')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        return self
+
+
+class GetServiceaccountOnepartyResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        tenant_id: str = None,
+        user_id: str = None,
+        user_type: str = None,
+        access_key: str = None,
+        access_secret: str = None,
+        status: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 租户ID
+        self.tenant_id = tenant_id
+        # 用户ID
+        self.user_id = user_id
+        # 用户类型
+        self.user_type = user_type
+        # accessKey
+        self.access_key = access_key
+        # accessSecret
+        self.access_secret = access_secret
+        # status
+        self.status = status
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.user_type is not None:
+            result['user_type'] = self.user_type
+        if self.access_key is not None:
+            result['access_key'] = self.access_key
+        if self.access_secret is not None:
+            result['access_secret'] = self.access_secret
+        if self.status is not None:
+            result['status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('user_type') is not None:
+            self.user_type = m.get('user_type')
+        if m.get('access_key') is not None:
+            self.access_key = m.get('access_key')
+        if m.get('access_secret') is not None:
+            self.access_secret = m.get('access_secret')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        return self
+
+
+class ApplyTrustloginTokenRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        user_id: str = None,
+        source_system: str = None,
+        login_name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 用户ID
+        # 
+        self.user_id = user_id
+        # 系统来源
+        self.source_system = source_system
+        # 登录账号
+        # 
+        self.login_name = login_name
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.source_system, 'source_system')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.source_system is not None:
+            result['source_system'] = self.source_system
+        if self.login_name is not None:
+            result['login_name'] = self.login_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('source_system') is not None:
+            self.source_system = m.get('source_system')
+        if m.get('login_name') is not None:
+            self.login_name = m.get('login_name')
+        return self
+
+
+class ApplyTrustloginTokenResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        user_id: str = None,
+        access_token: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 用户ID
+        # 
+        self.user_id = user_id
+        # 用于登录的token
+        # 
+        self.access_token = access_token
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.access_token is not None:
+            result['access_token'] = self.access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('access_token') is not None:
+            self.access_token = m.get('access_token')
+        return self
+
+
+class VerifyTrustloginTokenRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        source_system: str = None,
+        access_token: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        # 系统来源
+        # 
+        self.source_system = source_system
+        # 申请免密登录时获取的token
+        # 
+        self.access_token = access_token
+
+    def validate(self):
+        self.validate_required(self.source_system, 'source_system')
+        self.validate_required(self.access_token, 'access_token')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.source_system is not None:
+            result['source_system'] = self.source_system
+        if self.access_token is not None:
+            result['access_token'] = self.access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('source_system') is not None:
+            self.source_system = m.get('source_system')
+        if m.get('access_token') is not None:
+            self.access_token = m.get('access_token')
+        return self
+
+
+class VerifyTrustloginTokenResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        user_id: str = None,
+        result: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 用户ID
+        # 
+        self.user_id = user_id
+        # 验证结果，VALID有效，INVALID无效
+        self.result = result
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('result') is not None:
+            self.result = m.get('result')
         return self
```

### Comparing `antchain_acm-1.0.23/setup.py` & `antchain_acm-1.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_acm.
 
-Created on 17/06/2022
+Created on 27/07/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_acm"
 NAME = "antchain_acm" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Acm SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

