# Comparing `tmp/tencentcloud-sdk-python-apigateway-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-apigateway-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.943.tar", last modified: Wed Jul 26 00:30:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.944.tar", last modified: Thu Jul 27 02:08:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-apigateway-3.0.943.tar` & `tencentcloud-sdk-python-apigateway-3.0.944.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud/apigateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud/apigateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud/apigateway/v20180808/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud/apigateway/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21433 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud/apigateway/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   648371 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud/apigateway/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)    96571 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud/apigateway/v20180808/apigateway_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud_sdk_python_apigateway.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-26 00:30:35.000000 tencentcloud-sdk-python-apigateway-3.0.943/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud/apigateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud/apigateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud/apigateway/v20180808/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud/apigateway/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21197 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud/apigateway/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   644386 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud/apigateway/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)    95541 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud/apigateway/v20180808/apigateway_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud_sdk_python_apigateway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-27 02:08:37.000000 tencentcloud-sdk-python-apigateway-3.0.944/README.rst
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.943/setup.py` & `tencentcloud-sdk-python-apigateway-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud/apigateway/v20180808/errorcodes.py` & `tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud/apigateway/v20180808/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,17 +112,14 @@
 
 # 事件总线绑定/解绑失败。
 FAILEDOPERATION_EBERROR = 'FailedOperation.EbError'
 
 # 域名格式错误。
 FAILEDOPERATION_FORMATERROR = 'FailedOperation.FormatError'
 
-# API文档生成失败。
-FAILEDOPERATION_GENERATEAPIDOCUMENTERROR = 'FailedOperation.GenerateApiDocumentError'
-
 # 获取角色失败，请确认完成API网关相关服务接口授权。
 FAILEDOPERATION_GETROLEERROR = 'FailedOperation.GetRoleError'
 
 # 实例不存在，或者无效状态。
 FAILEDOPERATION_INSTANCENOTEXIST = 'FailedOperation.InstanceNotExist'
 
 # Apis 自定义路径与默认路径冲突。
@@ -241,17 +238,14 @@
 
 # 服务当前环境状态，不支持此操作。
 INVALIDPARAMETERVALUE_INVALIDENVSTATUS = 'InvalidParameterValue.InvalidEnvStatus'
 
 # 参数取值错误。
 INVALIDPARAMETERVALUE_INVALIDFILTERNOTSUPPORTEDNAME = 'InvalidParameterValue.InvalidFilterNotSupportedName'
 
-# 参数GenLanguage取值错误。
-INVALIDPARAMETERVALUE_INVALIDGENLANGUAGE = 'InvalidParameterValue.InvalidGenLanguage'
-
 # 参数后端地址取值错误。
 INVALIDPARAMETERVALUE_INVALIDIPADDRESS = 'InvalidParameterValue.InvalidIPAddress'
 
 # 参数请求配额总数取值错误。
 INVALIDPARAMETERVALUE_INVALIDMAXREQUESTNUM = 'InvalidParameterValue.InvalidMaxRequestNum'
 
 # 方法错误。仅支持 ANY, BEGIN, GET, POST, DELETE, HEAD, PUT, OPTIONS, TRACE, PATCH，请修改后重新操作。
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud/apigateway/v20180808/models.py` & `tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud/apigateway/v20180808/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -12570,59 +12570,14 @@
 
 
     def _deserialize(self, params):
         self._Result = params.get("Result")
         self._RequestId = params.get("RequestId")
 
 
-class DocumentSDK(AbstractModel):
-    """api文档下载
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _DocumentURL: 生成的 document 会存放到 COS 中，此出参返回产生文件的下载链接。
-        :type DocumentURL: str
-        :param _SdkURL: 生成的 SDK 会存放到 COS 中，此出参返回产生 SDK 文件的下载链接。
-        :type SdkURL: str
-        """
-        self._DocumentURL = None
-        self._SdkURL = None
-
-    @property
-    def DocumentURL(self):
-        return self._DocumentURL
-
-    @DocumentURL.setter
-    def DocumentURL(self, DocumentURL):
-        self._DocumentURL = DocumentURL
-
-    @property
-    def SdkURL(self):
-        return self._SdkURL
-
-    @SdkURL.setter
-    def SdkURL(self, SdkURL):
-        self._SdkURL = SdkURL
-
-
-    def _deserialize(self, params):
-        self._DocumentURL = params.get("DocumentURL")
-        self._SdkURL = params.get("SdkURL")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class DomainSetList(AbstractModel):
     """服务自定义域名列表
 
     """
 
     def __init__(self):
         r"""
@@ -13101,110 +13056,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class GenerateApiDocumentRequest(AbstractModel):
-    """GenerateApiDocument请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ServiceId: 待创建文档的服务唯一 ID。
-        :type ServiceId: str
-        :param _GenEnvironment: 待创建 SDK 的服务所在环境。
-        :type GenEnvironment: str
-        :param _GenLanguage: 待创建 SDK 的语言。当前只支持 Python 和 JavaScript。
-        :type GenLanguage: str
-        """
-        self._ServiceId = None
-        self._GenEnvironment = None
-        self._GenLanguage = None
-
-    @property
-    def ServiceId(self):
-        return self._ServiceId
-
-    @ServiceId.setter
-    def ServiceId(self, ServiceId):
-        self._ServiceId = ServiceId
-
-    @property
-    def GenEnvironment(self):
-        return self._GenEnvironment
-
-    @GenEnvironment.setter
-    def GenEnvironment(self, GenEnvironment):
-        self._GenEnvironment = GenEnvironment
-
-    @property
-    def GenLanguage(self):
-        return self._GenLanguage
-
-    @GenLanguage.setter
-    def GenLanguage(self, GenLanguage):
-        self._GenLanguage = GenLanguage
-
-
-    def _deserialize(self, params):
-        self._ServiceId = params.get("ServiceId")
-        self._GenEnvironment = params.get("GenEnvironment")
-        self._GenLanguage = params.get("GenLanguage")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class GenerateApiDocumentResponse(AbstractModel):
-    """GenerateApiDocument返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Result: api文档&sdk链接。
-        :type Result: :class:`tencentcloud.apigateway.v20180808.models.DocumentSDK`
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._Result = None
-        self._RequestId = None
-
-    @property
-    def Result(self):
-        return self._Result
-
-    @Result.setter
-    def Result(self, Result):
-        self._Result = Result
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("Result") is not None:
-            self._Result = DocumentSDK()
-            self._Result._deserialize(params.get("Result"))
-        self._RequestId = params.get("RequestId")
-
-
 class HealthCheckConf(AbstractModel):
     """健康检查配置，包括TsfHealthCheckConf和TargetServicesHealthCheckConf
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud/apigateway/v20180808/apigateway_client.py` & `tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud/apigateway/v20180808/apigateway_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1674,39 +1674,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def GenerateApiDocument(self, request):
-        """接口已废弃
-
-        本接口（GenerateApiDocument）用于自动生成 API 文档和 SDK，一个服务的一个环境生成一份文档和 SDK。
-
-        :param request: Request instance for GenerateApiDocument.
-        :type request: :class:`tencentcloud.apigateway.v20180808.models.GenerateApiDocumentRequest`
-        :rtype: :class:`tencentcloud.apigateway.v20180808.models.GenerateApiDocumentResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("GenerateApiDocument", params, headers=headers)
-            response = json.loads(body)
-            model = models.GenerateApiDocumentResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
     def ImportOpenApi(self, request):
         """本接口（ImportOpenApi）用于将OpenAPI规范定义的API导入到API网关。
 
         :param request: Request instance for ImportOpenApi.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.ImportOpenApiRequest`
         :rtype: :class:`tencentcloud.apigateway.v20180808.models.ImportOpenApiResponse`
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.943'
+__version__ = '3.0.944'
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.944/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.943/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.944/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.943/README.rst` & `tencentcloud-sdk-python-apigateway-3.0.944/README.rst`

 * *Files identical despite different names*

