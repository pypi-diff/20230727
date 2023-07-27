# Comparing `tmp/alibabacloud_xrengine20230313-1.0.1.tar.gz` & `tmp/alibabacloud_xrengine20230313-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_xrengine20230313-1.0.1.tar", last modified: Tue Jul 18 07:01:06 2023, max compression
+gzip compressed data, was "dist/alibabacloud_xrengine20230313-1.0.2.tar", last modified: Thu Jul 27 08:06:14 2023, max compression
```

## Comparing `alibabacloud_xrengine20230313-1.0.1.tar` & `alibabacloud_xrengine20230313-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51357 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313/client.py
--rw-r--r--   0 root         (0) root         (0)   170675 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 08:06:14.000000 alibabacloud_xrengine20230313-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-27 08:06:14.000000 alibabacloud_xrengine20230313-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 08:06:14.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62573 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313/client.py
+-rw-r--r--   0 root         (0) root         (0)   216135 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 08:06:14.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 08:06:14.000000 alibabacloud_xrengine20230313-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-07-27 08:06:13.000000 alibabacloud_xrengine20230313-1.0.2/setup.py
```

### Comparing `alibabacloud_xrengine20230313-1.0.1/LICENSE` & `alibabacloud_xrengine20230313-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-1.0.1/PKG-INFO` & `alibabacloud_xrengine20230313-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_xrengine20230313
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud xrEngine (20230313) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_xrengine20230313-1.0.1/README-CN.md` & `alibabacloud_xrengine20230313-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-1.0.1/README.md` & `alibabacloud_xrengine20230313-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313/client.py` & `alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -95,14 +95,84 @@
     ) -> str:
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
+    def auth_user_with_options(
+        self,
+        request: xr_engine_20230313_models.AuthUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.AuthUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.jwt_token):
+            query['JwtToken'] = request.jwt_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='AuthUser',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.AuthUserResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def auth_user_with_options_async(
+        self,
+        request: xr_engine_20230313_models.AuthUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.AuthUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.jwt_token):
+            query['JwtToken'] = request.jwt_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='AuthUser',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.AuthUserResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def auth_user(
+        self,
+        request: xr_engine_20230313_models.AuthUserRequest,
+    ) -> xr_engine_20230313_models.AuthUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.auth_user_with_options(request, runtime)
+
+    async def auth_user_async(
+        self,
+        request: xr_engine_20230313_models.AuthUserRequest,
+    ) -> xr_engine_20230313_models.AuthUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.auth_user_with_options_async(request, runtime)
+
     def get_map_data_with_options(
         self,
         request: xr_engine_20230313_models.GetMapDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.GetMapDataResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -481,21 +551,105 @@
     async def locate_async(
         self,
         request: xr_engine_20230313_models.LocateRequest,
     ) -> xr_engine_20230313_models.LocateResponse:
         runtime = util_models.RuntimeOptions()
         return await self.locate_with_options_async(request, runtime)
 
+    def login_model_scope_with_options(
+        self,
+        request: xr_engine_20230313_models.LoginModelScopeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.LoginModelScopeResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.emp_id):
+            body['EmpId'] = request.emp_id
+        if not UtilClient.is_unset(request.emp_name):
+            body['EmpName'] = request.emp_name
+        if not UtilClient.is_unset(request.token):
+            body['Token'] = request.token
+        if not UtilClient.is_unset(request.type):
+            body['Type'] = request.type
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='LoginModelScope',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.LoginModelScopeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def login_model_scope_with_options_async(
+        self,
+        request: xr_engine_20230313_models.LoginModelScopeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.LoginModelScopeResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.emp_id):
+            body['EmpId'] = request.emp_id
+        if not UtilClient.is_unset(request.emp_name):
+            body['EmpName'] = request.emp_name
+        if not UtilClient.is_unset(request.token):
+            body['Token'] = request.token
+        if not UtilClient.is_unset(request.type):
+            body['Type'] = request.type
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='LoginModelScope',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.LoginModelScopeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def login_model_scope(
+        self,
+        request: xr_engine_20230313_models.LoginModelScopeRequest,
+    ) -> xr_engine_20230313_models.LoginModelScopeResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.login_model_scope_with_options(request, runtime)
+
+    async def login_model_scope_async(
+        self,
+        request: xr_engine_20230313_models.LoginModelScopeRequest,
+    ) -> xr_engine_20230313_models.LoginModelScopeResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.login_model_scope_with_options_async(request, runtime)
+
     def pop_batch_query_object_project_status_with_options(
         self,
         request: xr_engine_20230313_models.PopBatchQueryObjectProjectStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.PopBatchQueryObjectProjectStatusResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.jwt_token):
+            body['JwtToken'] = request.jwt_token
         if not UtilClient.is_unset(request.project_ids):
             body['ProjectIds'] = request.project_ids
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PopBatchQueryObjectProjectStatus',
@@ -516,14 +670,16 @@
     async def pop_batch_query_object_project_status_with_options_async(
         self,
         request: xr_engine_20230313_models.PopBatchQueryObjectProjectStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.PopBatchQueryObjectProjectStatusResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.jwt_token):
+            body['JwtToken'] = request.jwt_token
         if not UtilClient.is_unset(request.project_ids):
             body['ProjectIds'] = request.project_ids
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PopBatchQueryObjectProjectStatus',
@@ -630,16 +786,20 @@
         request: xr_engine_20230313_models.PopBuildObjectProjectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.PopBuildObjectProjectResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.project_id):
             query['ProjectId'] = request.project_id
+        body = {}
+        if not UtilClient.is_unset(request.jwt_token):
+            body['JwtToken'] = request.jwt_token
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PopBuildObjectProject',
             version='2023-03-13',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -658,16 +818,20 @@
         request: xr_engine_20230313_models.PopBuildObjectProjectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.PopBuildObjectProjectResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.project_id):
             query['ProjectId'] = request.project_id
+        body = {}
+        if not UtilClient.is_unset(request.jwt_token):
+            body['JwtToken'] = request.jwt_token
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PopBuildObjectProject',
             version='2023-03-13',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -780,20 +944,26 @@
     ) -> xr_engine_20230313_models.PopCreateObjectProjectResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.auto_build):
             body['AutoBuild'] = request.auto_build
         if not UtilClient.is_unset(request.biz_usage):
             body['BizUsage'] = request.biz_usage
+        if not UtilClient.is_unset(request.custom_source):
+            body['CustomSource'] = request.custom_source
         if not UtilClient.is_unset(request.dependencies):
             body['Dependencies'] = request.dependencies
         if not UtilClient.is_unset(request.intro):
             body['Intro'] = request.intro
+        if not UtilClient.is_unset(request.jwt_token):
+            body['JwtToken'] = request.jwt_token
         if not UtilClient.is_unset(request.mode):
             body['Mode'] = request.mode
+        if not UtilClient.is_unset(request.recommend_status):
+            body['RecommendStatus'] = request.recommend_status
         if not UtilClient.is_unset(request.title):
             body['Title'] = request.title
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PopCreateObjectProject',
@@ -818,20 +988,26 @@
     ) -> xr_engine_20230313_models.PopCreateObjectProjectResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.auto_build):
             body['AutoBuild'] = request.auto_build
         if not UtilClient.is_unset(request.biz_usage):
             body['BizUsage'] = request.biz_usage
+        if not UtilClient.is_unset(request.custom_source):
+            body['CustomSource'] = request.custom_source
         if not UtilClient.is_unset(request.dependencies):
             body['Dependencies'] = request.dependencies
         if not UtilClient.is_unset(request.intro):
             body['Intro'] = request.intro
+        if not UtilClient.is_unset(request.jwt_token):
+            body['JwtToken'] = request.jwt_token
         if not UtilClient.is_unset(request.mode):
             body['Mode'] = request.mode
+        if not UtilClient.is_unset(request.recommend_status):
+            body['RecommendStatus'] = request.recommend_status
         if not UtilClient.is_unset(request.title):
             body['Title'] = request.title
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PopCreateObjectProject',
@@ -1027,23 +1203,107 @@
     async def pop_list_feature_to_avatar_project_async(
         self,
         request: xr_engine_20230313_models.PopListFeatureToAvatarProjectRequest,
     ) -> xr_engine_20230313_models.PopListFeatureToAvatarProjectResponse:
         runtime = util_models.RuntimeOptions()
         return await self.pop_list_feature_to_avatar_project_with_options_async(request, runtime)
 
+    def pop_list_object_case_with_options(
+        self,
+        request: xr_engine_20230313_models.PopListObjectCaseRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopListObjectCaseResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.current):
+            body['Current'] = request.current
+        if not UtilClient.is_unset(request.jwt_token):
+            body['JwtToken'] = request.jwt_token
+        if not UtilClient.is_unset(request.size):
+            body['Size'] = request.size
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PopListObjectCase',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopListObjectCaseResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def pop_list_object_case_with_options_async(
+        self,
+        request: xr_engine_20230313_models.PopListObjectCaseRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopListObjectCaseResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.current):
+            body['Current'] = request.current
+        if not UtilClient.is_unset(request.jwt_token):
+            body['JwtToken'] = request.jwt_token
+        if not UtilClient.is_unset(request.size):
+            body['Size'] = request.size
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PopListObjectCase',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopListObjectCaseResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def pop_list_object_case(
+        self,
+        request: xr_engine_20230313_models.PopListObjectCaseRequest,
+    ) -> xr_engine_20230313_models.PopListObjectCaseResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.pop_list_object_case_with_options(request, runtime)
+
+    async def pop_list_object_case_async(
+        self,
+        request: xr_engine_20230313_models.PopListObjectCaseRequest,
+    ) -> xr_engine_20230313_models.PopListObjectCaseResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.pop_list_object_case_with_options_async(request, runtime)
+
     def pop_list_object_project_with_options(
         self,
         request: xr_engine_20230313_models.PopListObjectProjectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.PopListObjectProjectResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.audit_status):
+            body['AuditStatus'] = request.audit_status
         if not UtilClient.is_unset(request.current):
             body['Current'] = request.current
+        if not UtilClient.is_unset(request.custom_source):
+            body['CustomSource'] = request.custom_source
+        if not UtilClient.is_unset(request.jwt_token):
+            body['JwtToken'] = request.jwt_token
         if not UtilClient.is_unset(request.size):
             body['Size'] = request.size
         if not UtilClient.is_unset(request.sort_field):
             body['SortField'] = request.sort_field
         if not UtilClient.is_unset(request.status):
             body['Status'] = request.status
         if not UtilClient.is_unset(request.title):
@@ -1072,16 +1332,22 @@
     async def pop_list_object_project_with_options_async(
         self,
         request: xr_engine_20230313_models.PopListObjectProjectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.PopListObjectProjectResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.audit_status):
+            body['AuditStatus'] = request.audit_status
         if not UtilClient.is_unset(request.current):
             body['Current'] = request.current
+        if not UtilClient.is_unset(request.custom_source):
+            body['CustomSource'] = request.custom_source
+        if not UtilClient.is_unset(request.jwt_token):
+            body['JwtToken'] = request.jwt_token
         if not UtilClient.is_unset(request.size):
             body['Size'] = request.size
         if not UtilClient.is_unset(request.sort_field):
             body['SortField'] = request.sort_field
         if not UtilClient.is_unset(request.status):
             body['Status'] = request.status
         if not UtilClient.is_unset(request.title):
@@ -1126,16 +1392,20 @@
         request: xr_engine_20230313_models.PopObjectProjectDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.PopObjectProjectDetailResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.project_id):
             query['ProjectId'] = request.project_id
+        body = {}
+        if not UtilClient.is_unset(request.jwt_token):
+            body['JwtToken'] = request.jwt_token
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PopObjectProjectDetail',
             version='2023-03-13',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -1154,16 +1424,20 @@
         request: xr_engine_20230313_models.PopObjectProjectDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.PopObjectProjectDetailResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.project_id):
             query['ProjectId'] = request.project_id
+        body = {}
+        if not UtilClient.is_unset(request.jwt_token):
+            body['JwtToken'] = request.jwt_token
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PopObjectProjectDetail',
             version='2023-03-13',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -1198,16 +1472,20 @@
     ) -> xr_engine_20230313_models.PopVideoSaveSourceResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.project_id):
             query['ProjectId'] = request.project_id
         if not UtilClient.is_unset(request.source_type):
             query['SourceType'] = request.source_type
+        body = {}
+        if not UtilClient.is_unset(request.jwt_token):
+            body['JwtToken'] = request.jwt_token
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PopVideoSaveSource',
             version='2023-03-13',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -1228,16 +1506,20 @@
     ) -> xr_engine_20230313_models.PopVideoSaveSourceResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.project_id):
             query['ProjectId'] = request.project_id
         if not UtilClient.is_unset(request.source_type):
             query['SourceType'] = request.source_type
+        body = {}
+        if not UtilClient.is_unset(request.jwt_token):
+            body['JwtToken'] = request.jwt_token
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PopVideoSaveSource',
             version='2023-03-13',
             protocol='HTTPS',
             pathname='/',
             method='POST',
```

### Comparing `alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313/models.py` & `alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,180 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import List, Dict, Any
+from typing import Dict, List, Any
+
+
+class AuthUserRequest(TeaModel):
+    def __init__(
+        self,
+        jwt_token: str = None,
+    ):
+        self.jwt_token = jwt_token
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
+        if self.jwt_token is not None:
+            result['JwtToken'] = self.jwt_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('JwtToken') is not None:
+            self.jwt_token = m.get('JwtToken')
+        return self
+
+
+class AuthUserResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        jwt_token: str = None,
+        type: str = None,
+    ):
+        self.jwt_token = jwt_token
+        self.type = type
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
+        if self.jwt_token is not None:
+            result['JwtToken'] = self.jwt_token
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('JwtToken') is not None:
+            self.jwt_token = m.get('JwtToken')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class AuthUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: AuthUserResponseBodyData = None,
+        error_name: str = None,
+        http_code: int = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.error_name = error_name
+        self.http_code = http_code
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.error_name is not None:
+            result['ErrorName'] = self.error_name
+        if self.http_code is not None:
+            result['HttpCode'] = self.http_code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = AuthUserResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('ErrorName') is not None:
+            self.error_name = m.get('ErrorName')
+        if m.get('HttpCode') is not None:
+            self.http_code = m.get('HttpCode')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class AuthUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AuthUserResponseBody = None,
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
+            temp_model = AuthUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
 
 
 class GetMapDataRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         jwt_token: str = None,
@@ -843,36 +1012,235 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = LocateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class LoginModelScopeRequest(TeaModel):
+    def __init__(
+        self,
+        emp_id: str = None,
+        emp_name: str = None,
+        token: str = None,
+        type: str = None,
+    ):
+        self.emp_id = emp_id
+        self.emp_name = emp_name
+        self.token = token
+        self.type = type
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
+        if self.emp_id is not None:
+            result['EmpId'] = self.emp_id
+        if self.emp_name is not None:
+            result['EmpName'] = self.emp_name
+        if self.token is not None:
+            result['Token'] = self.token
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EmpId') is not None:
+            self.emp_id = m.get('EmpId')
+        if m.get('EmpName') is not None:
+            self.emp_name = m.get('EmpName')
+        if m.get('Token') is not None:
+            self.token = m.get('Token')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class LoginModelScopeResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        jwt_token: str = None,
+        nickname: str = None,
+        uid: str = None,
+    ):
+        self.jwt_token = jwt_token
+        self.nickname = nickname
+        self.uid = uid
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
+        if self.jwt_token is not None:
+            result['JwtToken'] = self.jwt_token
+        if self.nickname is not None:
+            result['Nickname'] = self.nickname
+        if self.uid is not None:
+            result['Uid'] = self.uid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('JwtToken') is not None:
+            self.jwt_token = m.get('JwtToken')
+        if m.get('Nickname') is not None:
+            self.nickname = m.get('Nickname')
+        if m.get('Uid') is not None:
+            self.uid = m.get('Uid')
+        return self
+
+
+class LoginModelScopeResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: LoginModelScopeResponseBodyData = None,
+        error_name: str = None,
+        http_code: int = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.error_name = error_name
+        self.http_code = http_code
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.error_name is not None:
+            result['ErrorName'] = self.error_name
+        if self.http_code is not None:
+            result['HttpCode'] = self.http_code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = LoginModelScopeResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('ErrorName') is not None:
+            self.error_name = m.get('ErrorName')
+        if m.get('HttpCode') is not None:
+            self.http_code = m.get('HttpCode')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class LoginModelScopeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: LoginModelScopeResponseBody = None,
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
+            temp_model = LoginModelScopeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class PopBatchQueryObjectProjectStatusRequest(TeaModel):
     def __init__(
         self,
+        jwt_token: str = None,
         project_ids: str = None,
     ):
+        self.jwt_token = jwt_token
         self.project_ids = project_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.jwt_token is not None:
+            result['JwtToken'] = self.jwt_token
         if self.project_ids is not None:
             result['ProjectIds'] = self.project_ids
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('JwtToken') is not None:
+            self.jwt_token = m.get('JwtToken')
         if m.get('ProjectIds') is not None:
             self.project_ids = m.get('ProjectIds')
         return self
 
 
 class PopBatchQueryObjectProjectStatusResponseBodyData(TeaModel):
     def __init__(
@@ -1143,33 +1511,39 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PopBuildObjectProjectRequest(TeaModel):
     def __init__(
         self,
+        jwt_token: str = None,
         project_id: str = None,
     ):
+        self.jwt_token = jwt_token
         self.project_id = project_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.jwt_token is not None:
+            result['JwtToken'] = self.jwt_token
         if self.project_id is not None:
             result['ProjectId'] = self.project_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('JwtToken') is not None:
+            self.jwt_token = m.get('JwtToken')
         if m.get('ProjectId') is not None:
             self.project_id = m.get('ProjectId')
         return self
 
 
 class PopBuildObjectProjectResponseBody(TeaModel):
     def __init__(
@@ -1776,24 +2150,30 @@
 
 
 class PopCreateObjectProjectRequest(TeaModel):
     def __init__(
         self,
         auto_build: bool = None,
         biz_usage: str = None,
+        custom_source: str = None,
         dependencies: str = None,
         intro: str = None,
+        jwt_token: str = None,
         mode: str = None,
+        recommend_status: str = None,
         title: str = None,
     ):
         self.auto_build = auto_build
         self.biz_usage = biz_usage
+        self.custom_source = custom_source
         self.dependencies = dependencies
         self.intro = intro
+        self.jwt_token = jwt_token
         self.mode = mode
+        self.recommend_status = recommend_status
         self.title = title
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1801,36 +2181,48 @@
             return _map
 
         result = dict()
         if self.auto_build is not None:
             result['AutoBuild'] = self.auto_build
         if self.biz_usage is not None:
             result['BizUsage'] = self.biz_usage
+        if self.custom_source is not None:
+            result['CustomSource'] = self.custom_source
         if self.dependencies is not None:
             result['Dependencies'] = self.dependencies
         if self.intro is not None:
             result['Intro'] = self.intro
+        if self.jwt_token is not None:
+            result['JwtToken'] = self.jwt_token
         if self.mode is not None:
             result['Mode'] = self.mode
+        if self.recommend_status is not None:
+            result['RecommendStatus'] = self.recommend_status
         if self.title is not None:
             result['Title'] = self.title
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AutoBuild') is not None:
             self.auto_build = m.get('AutoBuild')
         if m.get('BizUsage') is not None:
             self.biz_usage = m.get('BizUsage')
+        if m.get('CustomSource') is not None:
+            self.custom_source = m.get('CustomSource')
         if m.get('Dependencies') is not None:
             self.dependencies = m.get('Dependencies')
         if m.get('Intro') is not None:
             self.intro = m.get('Intro')
+        if m.get('JwtToken') is not None:
+            self.jwt_token = m.get('JwtToken')
         if m.get('Mode') is not None:
             self.mode = m.get('Mode')
+        if m.get('RecommendStatus') is not None:
+            self.recommend_status = m.get('RecommendStatus')
         if m.get('Title') is not None:
             self.title = m.get('Title')
         return self
 
 
 class PopCreateObjectProjectResponseBodyDataBuildDetail(TeaModel):
     def __init__(
@@ -2250,44 +2642,105 @@
         if m.get('Type') is not None:
             self.type = m.get('Type')
         if m.get('Url') is not None:
             self.url = m.get('Url')
         return self
 
 
+class PopCreateObjectProjectResponseBodyDataSourceToken(TeaModel):
+    def __init__(
+        self,
+        access_key_id: str = None,
+        access_key_secret: str = None,
+        dir: str = None,
+        expiration: str = None,
+        host: str = None,
+        security_token: str = None,
+    ):
+        self.access_key_id = access_key_id
+        self.access_key_secret = access_key_secret
+        self.dir = dir
+        self.expiration = expiration
+        self.host = host
+        self.security_token = security_token
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
+        if self.access_key_id is not None:
+            result['AccessKeyId'] = self.access_key_id
+        if self.access_key_secret is not None:
+            result['AccessKeySecret'] = self.access_key_secret
+        if self.dir is not None:
+            result['Dir'] = self.dir
+        if self.expiration is not None:
+            result['Expiration'] = self.expiration
+        if self.host is not None:
+            result['Host'] = self.host
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessKeyId') is not None:
+            self.access_key_id = m.get('AccessKeyId')
+        if m.get('AccessKeySecret') is not None:
+            self.access_key_secret = m.get('AccessKeySecret')
+        if m.get('Dir') is not None:
+            self.dir = m.get('Dir')
+        if m.get('Expiration') is not None:
+            self.expiration = m.get('Expiration')
+        if m.get('Host') is not None:
+            self.host = m.get('Host')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
 class PopCreateObjectProjectResponseBodyDataSource(TeaModel):
     def __init__(
         self,
         clothes: List[PopCreateObjectProjectResponseBodyDataSourceClothes] = None,
         create_time: str = None,
         deleted: bool = None,
         modified_time: str = None,
         oss_key: str = None,
         policy: PopCreateObjectProjectResponseBodyDataSourcePolicy = None,
         source_files: List[PopCreateObjectProjectResponseBodyDataSourceSourceFiles] = None,
+        token: PopCreateObjectProjectResponseBodyDataSourceToken = None,
     ):
         self.clothes = clothes
         self.create_time = create_time
         self.deleted = deleted
         self.modified_time = modified_time
         self.oss_key = oss_key
         self.policy = policy
         self.source_files = source_files
+        self.token = token
 
     def validate(self):
         if self.clothes:
             for k in self.clothes:
                 if k:
                     k.validate()
         if self.policy:
             self.policy.validate()
         if self.source_files:
             for k in self.source_files:
                 if k:
                     k.validate()
+        if self.token:
+            self.token.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -2305,14 +2758,16 @@
             result['OssKey'] = self.oss_key
         if self.policy is not None:
             result['Policy'] = self.policy.to_map()
         result['SourceFiles'] = []
         if self.source_files is not None:
             for k in self.source_files:
                 result['SourceFiles'].append(k.to_map() if k else None)
+        if self.token is not None:
+            result['Token'] = self.token.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         self.clothes = []
         if m.get('Clothes') is not None:
             for k in m.get('Clothes'):
@@ -2330,51 +2785,60 @@
             temp_model = PopCreateObjectProjectResponseBodyDataSourcePolicy()
             self.policy = temp_model.from_map(m['Policy'])
         self.source_files = []
         if m.get('SourceFiles') is not None:
             for k in m.get('SourceFiles'):
                 temp_model = PopCreateObjectProjectResponseBodyDataSourceSourceFiles()
                 self.source_files.append(temp_model.from_map(k))
+        if m.get('Token') is not None:
+            temp_model = PopCreateObjectProjectResponseBodyDataSourceToken()
+            self.token = temp_model.from_map(m['Token'])
         return self
 
 
 class PopCreateObjectProjectResponseBodyData(TeaModel):
     def __init__(
         self,
+        audit_status: str = None,
         auto_build: bool = None,
         biz_usage: str = None,
         build_detail: PopCreateObjectProjectResponseBodyDataBuildDetail = None,
         check_status: str = None,
         create_mode: str = None,
         create_time: str = None,
+        custom_source: str = None,
         dataset: PopCreateObjectProjectResponseBodyDataDataset = None,
         deleted: bool = None,
         dependencies: str = None,
         ext: str = None,
         id: str = None,
         intro: str = None,
         modified_time: str = None,
+        recommend_status: str = None,
         source: PopCreateObjectProjectResponseBodyDataSource = None,
         status: str = None,
         title: str = None,
         type: str = None,
     ):
+        self.audit_status = audit_status
         self.auto_build = auto_build
         self.biz_usage = biz_usage
         self.build_detail = build_detail
         self.check_status = check_status
         self.create_mode = create_mode
         self.create_time = create_time
+        self.custom_source = custom_source
         self.dataset = dataset
         self.deleted = deleted
         self.dependencies = dependencies
         self.ext = ext
         self.id = id
         self.intro = intro
         self.modified_time = modified_time
+        self.recommend_status = recommend_status
         self.source = source
         self.status = status
         self.title = title
         self.type = type
 
     def validate(self):
         if self.build_detail:
@@ -2386,65 +2850,75 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.audit_status is not None:
+            result['AuditStatus'] = self.audit_status
         if self.auto_build is not None:
             result['AutoBuild'] = self.auto_build
         if self.biz_usage is not None:
             result['BizUsage'] = self.biz_usage
         if self.build_detail is not None:
             result['BuildDetail'] = self.build_detail.to_map()
         if self.check_status is not None:
             result['CheckStatus'] = self.check_status
         if self.create_mode is not None:
             result['CreateMode'] = self.create_mode
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
+        if self.custom_source is not None:
+            result['CustomSource'] = self.custom_source
         if self.dataset is not None:
             result['Dataset'] = self.dataset.to_map()
         if self.deleted is not None:
             result['Deleted'] = self.deleted
         if self.dependencies is not None:
             result['Dependencies'] = self.dependencies
         if self.ext is not None:
             result['Ext'] = self.ext
         if self.id is not None:
             result['Id'] = self.id
         if self.intro is not None:
             result['Intro'] = self.intro
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
+        if self.recommend_status is not None:
+            result['RecommendStatus'] = self.recommend_status
         if self.source is not None:
             result['Source'] = self.source.to_map()
         if self.status is not None:
             result['Status'] = self.status
         if self.title is not None:
             result['Title'] = self.title
         if self.type is not None:
             result['Type'] = self.type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AuditStatus') is not None:
+            self.audit_status = m.get('AuditStatus')
         if m.get('AutoBuild') is not None:
             self.auto_build = m.get('AutoBuild')
         if m.get('BizUsage') is not None:
             self.biz_usage = m.get('BizUsage')
         if m.get('BuildDetail') is not None:
             temp_model = PopCreateObjectProjectResponseBodyDataBuildDetail()
             self.build_detail = temp_model.from_map(m['BuildDetail'])
         if m.get('CheckStatus') is not None:
             self.check_status = m.get('CheckStatus')
         if m.get('CreateMode') is not None:
             self.create_mode = m.get('CreateMode')
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
+        if m.get('CustomSource') is not None:
+            self.custom_source = m.get('CustomSource')
         if m.get('Dataset') is not None:
             temp_model = PopCreateObjectProjectResponseBodyDataDataset()
             self.dataset = temp_model.from_map(m['Dataset'])
         if m.get('Deleted') is not None:
             self.deleted = m.get('Deleted')
         if m.get('Dependencies') is not None:
             self.dependencies = m.get('Dependencies')
@@ -2452,14 +2926,16 @@
             self.ext = m.get('Ext')
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('Intro') is not None:
             self.intro = m.get('Intro')
         if m.get('ModifiedTime') is not None:
             self.modified_time = m.get('ModifiedTime')
+        if m.get('RecommendStatus') is not None:
+            self.recommend_status = m.get('RecommendStatus')
         if m.get('Source') is not None:
             temp_model = PopCreateObjectProjectResponseBodyDataSource()
             self.source = temp_model.from_map(m['Source'])
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('Title') is not None:
             self.title = m.get('Title')
@@ -3377,25 +3853,857 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PopListFeatureToAvatarProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class PopListObjectCaseRequest(TeaModel):
+    def __init__(
+        self,
+        current: int = None,
+        jwt_token: str = None,
+        size: int = None,
+    ):
+        self.current = current
+        self.jwt_token = jwt_token
+        self.size = size
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
+        if self.current is not None:
+            result['Current'] = self.current
+        if self.jwt_token is not None:
+            result['JwtToken'] = self.jwt_token
+        if self.size is not None:
+            result['Size'] = self.size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Current') is not None:
+            self.current = m.get('Current')
+        if m.get('JwtToken') is not None:
+            self.jwt_token = m.get('JwtToken')
+        if m.get('Size') is not None:
+            self.size = m.get('Size')
+        return self
+
+
+class PopListObjectCaseResponseBodyDataBuildDetail(TeaModel):
+    def __init__(
+        self,
+        completed_time: str = None,
+        create_time: str = None,
+        deleted: bool = None,
+        error_message: str = None,
+        estimated_duration: int = None,
+        modified_time: str = None,
+        running_time: str = None,
+        submit_time: str = None,
+    ):
+        self.completed_time = completed_time
+        self.create_time = create_time
+        self.deleted = deleted
+        self.error_message = error_message
+        self.estimated_duration = estimated_duration
+        self.modified_time = modified_time
+        self.running_time = running_time
+        self.submit_time = submit_time
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
+        if self.completed_time is not None:
+            result['CompletedTime'] = self.completed_time
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.deleted is not None:
+            result['Deleted'] = self.deleted
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.estimated_duration is not None:
+            result['EstimatedDuration'] = self.estimated_duration
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.running_time is not None:
+            result['RunningTime'] = self.running_time
+        if self.submit_time is not None:
+            result['SubmitTime'] = self.submit_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CompletedTime') is not None:
+            self.completed_time = m.get('CompletedTime')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Deleted') is not None:
+            self.deleted = m.get('Deleted')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('EstimatedDuration') is not None:
+            self.estimated_duration = m.get('EstimatedDuration')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('RunningTime') is not None:
+            self.running_time = m.get('RunningTime')
+        if m.get('SubmitTime') is not None:
+            self.submit_time = m.get('SubmitTime')
+        return self
+
+
+class PopListObjectCaseResponseBodyDataDatasetPolicy(TeaModel):
+    def __init__(
+        self,
+        access_id: str = None,
+        dir: str = None,
+        expire: str = None,
+        host: str = None,
+        policy: str = None,
+        signature: str = None,
+    ):
+        self.access_id = access_id
+        self.dir = dir
+        self.expire = expire
+        self.host = host
+        self.policy = policy
+        self.signature = signature
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
+        if self.access_id is not None:
+            result['AccessId'] = self.access_id
+        if self.dir is not None:
+            result['Dir'] = self.dir
+        if self.expire is not None:
+            result['Expire'] = self.expire
+        if self.host is not None:
+            result['Host'] = self.host
+        if self.policy is not None:
+            result['Policy'] = self.policy
+        if self.signature is not None:
+            result['Signature'] = self.signature
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessId') is not None:
+            self.access_id = m.get('AccessId')
+        if m.get('Dir') is not None:
+            self.dir = m.get('Dir')
+        if m.get('Expire') is not None:
+            self.expire = m.get('Expire')
+        if m.get('Host') is not None:
+            self.host = m.get('Host')
+        if m.get('Policy') is not None:
+            self.policy = m.get('Policy')
+        if m.get('Signature') is not None:
+            self.signature = m.get('Signature')
+        return self
+
+
+class PopListObjectCaseResponseBodyDataDataset(TeaModel):
+    def __init__(
+        self,
+        build_result_url: Dict[str, Any] = None,
+        cover_url: str = None,
+        create_time: str = None,
+        deleted: bool = None,
+        error_message: str = None,
+        glb_model_url: str = None,
+        model_url: str = None,
+        modified_time: str = None,
+        origin_result_url: str = None,
+        oss_key: str = None,
+        policy: PopListObjectCaseResponseBodyDataDatasetPolicy = None,
+        pose_url: str = None,
+        preview_url: str = None,
+    ):
+        self.build_result_url = build_result_url
+        self.cover_url = cover_url
+        self.create_time = create_time
+        self.deleted = deleted
+        self.error_message = error_message
+        self.glb_model_url = glb_model_url
+        self.model_url = model_url
+        self.modified_time = modified_time
+        self.origin_result_url = origin_result_url
+        self.oss_key = oss_key
+        self.policy = policy
+        self.pose_url = pose_url
+        self.preview_url = preview_url
+
+    def validate(self):
+        if self.policy:
+            self.policy.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.build_result_url is not None:
+            result['BuildResultUrl'] = self.build_result_url
+        if self.cover_url is not None:
+            result['CoverUrl'] = self.cover_url
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.deleted is not None:
+            result['Deleted'] = self.deleted
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.glb_model_url is not None:
+            result['GlbModelUrl'] = self.glb_model_url
+        if self.model_url is not None:
+            result['ModelUrl'] = self.model_url
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.origin_result_url is not None:
+            result['OriginResultUrl'] = self.origin_result_url
+        if self.oss_key is not None:
+            result['OssKey'] = self.oss_key
+        if self.policy is not None:
+            result['Policy'] = self.policy.to_map()
+        if self.pose_url is not None:
+            result['PoseUrl'] = self.pose_url
+        if self.preview_url is not None:
+            result['PreviewUrl'] = self.preview_url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BuildResultUrl') is not None:
+            self.build_result_url = m.get('BuildResultUrl')
+        if m.get('CoverUrl') is not None:
+            self.cover_url = m.get('CoverUrl')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Deleted') is not None:
+            self.deleted = m.get('Deleted')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('GlbModelUrl') is not None:
+            self.glb_model_url = m.get('GlbModelUrl')
+        if m.get('ModelUrl') is not None:
+            self.model_url = m.get('ModelUrl')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('OriginResultUrl') is not None:
+            self.origin_result_url = m.get('OriginResultUrl')
+        if m.get('OssKey') is not None:
+            self.oss_key = m.get('OssKey')
+        if m.get('Policy') is not None:
+            temp_model = PopListObjectCaseResponseBodyDataDatasetPolicy()
+            self.policy = temp_model.from_map(m['Policy'])
+        if m.get('PoseUrl') is not None:
+            self.pose_url = m.get('PoseUrl')
+        if m.get('PreviewUrl') is not None:
+            self.preview_url = m.get('PreviewUrl')
+        return self
+
+
+class PopListObjectCaseResponseBodyDataSourceClothes(TeaModel):
+    def __init__(
+        self,
+        cover_url: str = None,
+        create_time: str = None,
+        deleted: bool = None,
+        modified_time: str = None,
+        name: str = None,
+        oss_key: str = None,
+        type: str = None,
+    ):
+        self.cover_url = cover_url
+        self.create_time = create_time
+        self.deleted = deleted
+        self.modified_time = modified_time
+        self.name = name
+        self.oss_key = oss_key
+        self.type = type
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
+        if self.cover_url is not None:
+            result['CoverUrl'] = self.cover_url
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.deleted is not None:
+            result['Deleted'] = self.deleted
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.oss_key is not None:
+            result['OssKey'] = self.oss_key
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CoverUrl') is not None:
+            self.cover_url = m.get('CoverUrl')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Deleted') is not None:
+            self.deleted = m.get('Deleted')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('OssKey') is not None:
+            self.oss_key = m.get('OssKey')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class PopListObjectCaseResponseBodyDataSourcePolicy(TeaModel):
+    def __init__(
+        self,
+        access_id: str = None,
+        dir: str = None,
+        expire: str = None,
+        host: str = None,
+        policy: str = None,
+        signature: str = None,
+    ):
+        self.access_id = access_id
+        self.dir = dir
+        self.expire = expire
+        self.host = host
+        self.policy = policy
+        self.signature = signature
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
+        if self.access_id is not None:
+            result['AccessId'] = self.access_id
+        if self.dir is not None:
+            result['Dir'] = self.dir
+        if self.expire is not None:
+            result['Expire'] = self.expire
+        if self.host is not None:
+            result['Host'] = self.host
+        if self.policy is not None:
+            result['Policy'] = self.policy
+        if self.signature is not None:
+            result['Signature'] = self.signature
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessId') is not None:
+            self.access_id = m.get('AccessId')
+        if m.get('Dir') is not None:
+            self.dir = m.get('Dir')
+        if m.get('Expire') is not None:
+            self.expire = m.get('Expire')
+        if m.get('Host') is not None:
+            self.host = m.get('Host')
+        if m.get('Policy') is not None:
+            self.policy = m.get('Policy')
+        if m.get('Signature') is not None:
+            self.signature = m.get('Signature')
+        return self
+
+
+class PopListObjectCaseResponseBodyDataSourceSourceFiles(TeaModel):
+    def __init__(
+        self,
+        cover_url: str = None,
+        create_time: str = None,
+        deleted: bool = None,
+        file_name: str = None,
+        filesize: int = None,
+        modified_time: str = None,
+        oss_key: str = None,
+        type: str = None,
+        url: str = None,
+    ):
+        self.cover_url = cover_url
+        self.create_time = create_time
+        self.deleted = deleted
+        self.file_name = file_name
+        self.filesize = filesize
+        self.modified_time = modified_time
+        self.oss_key = oss_key
+        self.type = type
+        self.url = url
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
+        if self.cover_url is not None:
+            result['CoverUrl'] = self.cover_url
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.deleted is not None:
+            result['Deleted'] = self.deleted
+        if self.file_name is not None:
+            result['FileName'] = self.file_name
+        if self.filesize is not None:
+            result['Filesize'] = self.filesize
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.oss_key is not None:
+            result['OssKey'] = self.oss_key
+        if self.type is not None:
+            result['Type'] = self.type
+        if self.url is not None:
+            result['Url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CoverUrl') is not None:
+            self.cover_url = m.get('CoverUrl')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Deleted') is not None:
+            self.deleted = m.get('Deleted')
+        if m.get('FileName') is not None:
+            self.file_name = m.get('FileName')
+        if m.get('Filesize') is not None:
+            self.filesize = m.get('Filesize')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('OssKey') is not None:
+            self.oss_key = m.get('OssKey')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        return self
+
+
+class PopListObjectCaseResponseBodyDataSource(TeaModel):
+    def __init__(
+        self,
+        clothes: List[PopListObjectCaseResponseBodyDataSourceClothes] = None,
+        create_time: str = None,
+        deleted: bool = None,
+        modified_time: str = None,
+        oss_key: str = None,
+        policy: PopListObjectCaseResponseBodyDataSourcePolicy = None,
+        source_files: List[PopListObjectCaseResponseBodyDataSourceSourceFiles] = None,
+    ):
+        self.clothes = clothes
+        self.create_time = create_time
+        self.deleted = deleted
+        self.modified_time = modified_time
+        self.oss_key = oss_key
+        self.policy = policy
+        self.source_files = source_files
+
+    def validate(self):
+        if self.clothes:
+            for k in self.clothes:
+                if k:
+                    k.validate()
+        if self.policy:
+            self.policy.validate()
+        if self.source_files:
+            for k in self.source_files:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Clothes'] = []
+        if self.clothes is not None:
+            for k in self.clothes:
+                result['Clothes'].append(k.to_map() if k else None)
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.deleted is not None:
+            result['Deleted'] = self.deleted
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.oss_key is not None:
+            result['OssKey'] = self.oss_key
+        if self.policy is not None:
+            result['Policy'] = self.policy.to_map()
+        result['SourceFiles'] = []
+        if self.source_files is not None:
+            for k in self.source_files:
+                result['SourceFiles'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.clothes = []
+        if m.get('Clothes') is not None:
+            for k in m.get('Clothes'):
+                temp_model = PopListObjectCaseResponseBodyDataSourceClothes()
+                self.clothes.append(temp_model.from_map(k))
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Deleted') is not None:
+            self.deleted = m.get('Deleted')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('OssKey') is not None:
+            self.oss_key = m.get('OssKey')
+        if m.get('Policy') is not None:
+            temp_model = PopListObjectCaseResponseBodyDataSourcePolicy()
+            self.policy = temp_model.from_map(m['Policy'])
+        self.source_files = []
+        if m.get('SourceFiles') is not None:
+            for k in m.get('SourceFiles'):
+                temp_model = PopListObjectCaseResponseBodyDataSourceSourceFiles()
+                self.source_files.append(temp_model.from_map(k))
+        return self
+
+
+class PopListObjectCaseResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        audit_status: str = None,
+        auto_build: bool = None,
+        biz_usage: str = None,
+        build_detail: PopListObjectCaseResponseBodyDataBuildDetail = None,
+        check_status: str = None,
+        create_mode: str = None,
+        create_time: str = None,
+        custom_source: str = None,
+        dataset: PopListObjectCaseResponseBodyDataDataset = None,
+        deleted: bool = None,
+        dependencies: str = None,
+        ext: str = None,
+        id: str = None,
+        intro: str = None,
+        modified_time: str = None,
+        source: PopListObjectCaseResponseBodyDataSource = None,
+        status: str = None,
+        title: str = None,
+        type: str = None,
+    ):
+        self.audit_status = audit_status
+        self.auto_build = auto_build
+        self.biz_usage = biz_usage
+        self.build_detail = build_detail
+        self.check_status = check_status
+        self.create_mode = create_mode
+        self.create_time = create_time
+        self.custom_source = custom_source
+        self.dataset = dataset
+        self.deleted = deleted
+        self.dependencies = dependencies
+        self.ext = ext
+        self.id = id
+        self.intro = intro
+        self.modified_time = modified_time
+        self.source = source
+        self.status = status
+        self.title = title
+        self.type = type
+
+    def validate(self):
+        if self.build_detail:
+            self.build_detail.validate()
+        if self.dataset:
+            self.dataset.validate()
+        if self.source:
+            self.source.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.audit_status is not None:
+            result['AuditStatus'] = self.audit_status
+        if self.auto_build is not None:
+            result['AutoBuild'] = self.auto_build
+        if self.biz_usage is not None:
+            result['BizUsage'] = self.biz_usage
+        if self.build_detail is not None:
+            result['BuildDetail'] = self.build_detail.to_map()
+        if self.check_status is not None:
+            result['CheckStatus'] = self.check_status
+        if self.create_mode is not None:
+            result['CreateMode'] = self.create_mode
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.custom_source is not None:
+            result['CustomSource'] = self.custom_source
+        if self.dataset is not None:
+            result['Dataset'] = self.dataset.to_map()
+        if self.deleted is not None:
+            result['Deleted'] = self.deleted
+        if self.dependencies is not None:
+            result['Dependencies'] = self.dependencies
+        if self.ext is not None:
+            result['Ext'] = self.ext
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.intro is not None:
+            result['Intro'] = self.intro
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.source is not None:
+            result['Source'] = self.source.to_map()
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.title is not None:
+            result['Title'] = self.title
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AuditStatus') is not None:
+            self.audit_status = m.get('AuditStatus')
+        if m.get('AutoBuild') is not None:
+            self.auto_build = m.get('AutoBuild')
+        if m.get('BizUsage') is not None:
+            self.biz_usage = m.get('BizUsage')
+        if m.get('BuildDetail') is not None:
+            temp_model = PopListObjectCaseResponseBodyDataBuildDetail()
+            self.build_detail = temp_model.from_map(m['BuildDetail'])
+        if m.get('CheckStatus') is not None:
+            self.check_status = m.get('CheckStatus')
+        if m.get('CreateMode') is not None:
+            self.create_mode = m.get('CreateMode')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('CustomSource') is not None:
+            self.custom_source = m.get('CustomSource')
+        if m.get('Dataset') is not None:
+            temp_model = PopListObjectCaseResponseBodyDataDataset()
+            self.dataset = temp_model.from_map(m['Dataset'])
+        if m.get('Deleted') is not None:
+            self.deleted = m.get('Deleted')
+        if m.get('Dependencies') is not None:
+            self.dependencies = m.get('Dependencies')
+        if m.get('Ext') is not None:
+            self.ext = m.get('Ext')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Intro') is not None:
+            self.intro = m.get('Intro')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('Source') is not None:
+            temp_model = PopListObjectCaseResponseBodyDataSource()
+            self.source = temp_model.from_map(m['Source'])
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('Title') is not None:
+            self.title = m.get('Title')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class PopListObjectCaseResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        current: int = None,
+        data: List[PopListObjectCaseResponseBodyData] = None,
+        error_name: str = None,
+        http_code: int = None,
+        message: str = None,
+        pages: int = None,
+        request_id: str = None,
+        size: int = None,
+        success: bool = None,
+        total: int = None,
+    ):
+        self.code = code
+        self.current = current
+        self.data = data
+        self.error_name = error_name
+        self.http_code = http_code
+        self.message = message
+        self.pages = pages
+        self.request_id = request_id
+        self.size = size
+        self.success = success
+        self.total = total
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.current is not None:
+            result['Current'] = self.current
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.error_name is not None:
+            result['ErrorName'] = self.error_name
+        if self.http_code is not None:
+            result['HttpCode'] = self.http_code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.pages is not None:
+            result['Pages'] = self.pages
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.size is not None:
+            result['Size'] = self.size
+        if self.success is not None:
+            result['Success'] = self.success
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Current') is not None:
+            self.current = m.get('Current')
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = PopListObjectCaseResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('ErrorName') is not None:
+            self.error_name = m.get('ErrorName')
+        if m.get('HttpCode') is not None:
+            self.http_code = m.get('HttpCode')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('Pages') is not None:
+            self.pages = m.get('Pages')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Size') is not None:
+            self.size = m.get('Size')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class PopListObjectCaseResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: PopListObjectCaseResponseBody = None,
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
+            temp_model = PopListObjectCaseResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class PopListObjectProjectRequest(TeaModel):
     def __init__(
         self,
+        audit_status: str = None,
         current: int = None,
+        custom_source: str = None,
+        jwt_token: str = None,
         size: int = None,
         sort_field: str = None,
         status: str = None,
         title: str = None,
         with_source: bool = None,
     ):
+        self.audit_status = audit_status
         self.current = current
+        self.custom_source = custom_source
+        self.jwt_token = jwt_token
         self.size = size
         self.sort_field = sort_field
         self.status = status
         self.title = title
         self.with_source = with_source
 
     def validate(self):
@@ -3403,32 +4711,44 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.audit_status is not None:
+            result['AuditStatus'] = self.audit_status
         if self.current is not None:
             result['Current'] = self.current
+        if self.custom_source is not None:
+            result['CustomSource'] = self.custom_source
+        if self.jwt_token is not None:
+            result['JwtToken'] = self.jwt_token
         if self.size is not None:
             result['Size'] = self.size
         if self.sort_field is not None:
             result['SortField'] = self.sort_field
         if self.status is not None:
             result['Status'] = self.status
         if self.title is not None:
             result['Title'] = self.title
         if self.with_source is not None:
             result['WithSource'] = self.with_source
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AuditStatus') is not None:
+            self.audit_status = m.get('AuditStatus')
         if m.get('Current') is not None:
             self.current = m.get('Current')
+        if m.get('CustomSource') is not None:
+            self.custom_source = m.get('CustomSource')
+        if m.get('JwtToken') is not None:
+            self.jwt_token = m.get('JwtToken')
         if m.get('Size') is not None:
             self.size = m.get('Size')
         if m.get('SortField') is not None:
             self.sort_field = m.get('SortField')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('Title') is not None:
@@ -3942,38 +5262,42 @@
                 self.source_files.append(temp_model.from_map(k))
         return self
 
 
 class PopListObjectProjectResponseBodyData(TeaModel):
     def __init__(
         self,
+        audit_status: str = None,
         auto_build: bool = None,
         biz_usage: str = None,
         build_detail: PopListObjectProjectResponseBodyDataBuildDetail = None,
         check_status: str = None,
         create_mode: str = None,
         create_time: str = None,
+        custom_source: str = None,
         dataset: PopListObjectProjectResponseBodyDataDataset = None,
         deleted: bool = None,
         dependencies: str = None,
         ext: str = None,
         id: str = None,
         intro: str = None,
         modified_time: str = None,
         source: PopListObjectProjectResponseBodyDataSource = None,
         status: str = None,
         title: str = None,
         type: str = None,
     ):
+        self.audit_status = audit_status
         self.auto_build = auto_build
         self.biz_usage = biz_usage
         self.build_detail = build_detail
         self.check_status = check_status
         self.create_mode = create_mode
         self.create_time = create_time
+        self.custom_source = custom_source
         self.dataset = dataset
         self.deleted = deleted
         self.dependencies = dependencies
         self.ext = ext
         self.id = id
         self.intro = intro
         self.modified_time = modified_time
@@ -3992,26 +5316,30 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.audit_status is not None:
+            result['AuditStatus'] = self.audit_status
         if self.auto_build is not None:
             result['AutoBuild'] = self.auto_build
         if self.biz_usage is not None:
             result['BizUsage'] = self.biz_usage
         if self.build_detail is not None:
             result['BuildDetail'] = self.build_detail.to_map()
         if self.check_status is not None:
             result['CheckStatus'] = self.check_status
         if self.create_mode is not None:
             result['CreateMode'] = self.create_mode
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
+        if self.custom_source is not None:
+            result['CustomSource'] = self.custom_source
         if self.dataset is not None:
             result['Dataset'] = self.dataset.to_map()
         if self.deleted is not None:
             result['Deleted'] = self.deleted
         if self.dependencies is not None:
             result['Dependencies'] = self.dependencies
         if self.ext is not None:
@@ -4030,27 +5358,31 @@
             result['Title'] = self.title
         if self.type is not None:
             result['Type'] = self.type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AuditStatus') is not None:
+            self.audit_status = m.get('AuditStatus')
         if m.get('AutoBuild') is not None:
             self.auto_build = m.get('AutoBuild')
         if m.get('BizUsage') is not None:
             self.biz_usage = m.get('BizUsage')
         if m.get('BuildDetail') is not None:
             temp_model = PopListObjectProjectResponseBodyDataBuildDetail()
             self.build_detail = temp_model.from_map(m['BuildDetail'])
         if m.get('CheckStatus') is not None:
             self.check_status = m.get('CheckStatus')
         if m.get('CreateMode') is not None:
             self.create_mode = m.get('CreateMode')
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
+        if m.get('CustomSource') is not None:
+            self.custom_source = m.get('CustomSource')
         if m.get('Dataset') is not None:
             temp_model = PopListObjectProjectResponseBodyDataDataset()
             self.dataset = temp_model.from_map(m['Dataset'])
         if m.get('Deleted') is not None:
             self.deleted = m.get('Deleted')
         if m.get('Dependencies') is not None:
             self.dependencies = m.get('Dependencies')
@@ -4212,33 +5544,39 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PopObjectProjectDetailRequest(TeaModel):
     def __init__(
         self,
+        jwt_token: str = None,
         project_id: str = None,
     ):
+        self.jwt_token = jwt_token
         self.project_id = project_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.jwt_token is not None:
+            result['JwtToken'] = self.jwt_token
         if self.project_id is not None:
             result['ProjectId'] = self.project_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('JwtToken') is not None:
+            self.jwt_token = m.get('JwtToken')
         if m.get('ProjectId') is not None:
             self.project_id = m.get('ProjectId')
         return self
 
 
 class PopObjectProjectDetailResponseBodyDataBuildDetail(TeaModel):
     def __init__(
@@ -4984,37 +6322,43 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PopVideoSaveSourceRequest(TeaModel):
     def __init__(
         self,
+        jwt_token: str = None,
         project_id: str = None,
         source_type: str = None,
     ):
+        self.jwt_token = jwt_token
         self.project_id = project_id
         self.source_type = source_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.jwt_token is not None:
+            result['JwtToken'] = self.jwt_token
         if self.project_id is not None:
             result['ProjectId'] = self.project_id
         if self.source_type is not None:
             result['SourceType'] = self.source_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('JwtToken') is not None:
+            self.jwt_token = m.get('JwtToken')
         if m.get('ProjectId') is not None:
             self.project_id = m.get('ProjectId')
         if m.get('SourceType') is not None:
             self.source_type = m.get('SourceType')
         return self
```

### Comparing `alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313.egg-info/PKG-INFO` & `alibabacloud_xrengine20230313-1.0.2/alibabacloud_xrengine20230313.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-xrengine20230313
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud xrEngine (20230313) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_xrengine20230313-1.0.1/setup.py` & `alibabacloud_xrengine20230313-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_xrengine20230313.
 
-Created on 18/07/2023
+Created on 27/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_xrengine20230313"
 NAME = "alibabacloud_xrengine20230313" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud xrEngine (20230313) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.10, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

