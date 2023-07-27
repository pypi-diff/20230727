# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.943.tar", last modified: Wed Jul 26 00:37:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.944.tar", last modified: Thu Jul 27 02:15:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.943.tar` & `tencentcloud-sdk-python-ess-3.0.944.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    62244 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25058 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   438395 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-26 00:37:23.000000 tencentcloud-sdk-python-ess-3.0.943/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    65423 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25058 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   453453 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.943/setup.py` & `tencentcloud-sdk-python-ess-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.944/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def CreateEmbedWebUrl(self, request):
+        """本接口（CreateEmbedWebUrl）用于创建嵌入web的链接 本接口支持创建：创建印章，创建模板，修改模板，预览模板，预览合同流程的web链接 进入web连接后与当前控制台操作保持一致
+
+        :param request: Request instance for CreateEmbedWebUrl.
+        :type request: :class:`tencentcloud.ess.v20201111.models.CreateEmbedWebUrlRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.CreateEmbedWebUrlResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateEmbedWebUrl", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateEmbedWebUrlResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def CreateFlow(self, request):
         """通过模板创建签署流程<br/>
         适用场景：在标准制式的合同场景中，可通过提前预制好模板文件，每次调用模板文件的id，补充合同内容信息及签署信息生成电子合同。<br/>
         注：该接口是通过模板生成合同流程的前置接口，先创建一个不包含签署文件的流程。<br/>
         配合“创建电子文档”接口和“发起流程”接口使用。<br/>
 
         :param request: Request instance for CreateFlow.
@@ -551,14 +574,38 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def CreateOrganizationBatchSignUrl(self, request):
+        """通过此接口，创建企业批量签署链接，企业员工点击链接即可跳转控制台进行批量签署。
+        如果没有UserId，Name和Mobile必填，对应的员工必须在企业下已经实名，且该员工为批量签署合同中的签署方。
+
+        :param request: Request instance for CreateOrganizationBatchSignUrl.
+        :type request: :class:`tencentcloud.ess.v20201111.models.CreateOrganizationBatchSignUrlRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.CreateOrganizationBatchSignUrlResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateOrganizationBatchSignUrl", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateOrganizationBatchSignUrlResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def CreatePrepareFlow(self, request):
         """创建快速发起流程
         适用场景：用户通过API 合同文件及签署信息，并可通过我们返回的URL在页面完成签署控件等信息的编辑与确认，快速发起合同.
         注：该接口文件的resourceId 是通过上传文件之后获取的。
 
         :param request: Request instance for CreatePrepareFlow.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreatePrepareFlowRequest`
@@ -722,14 +769,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def CreateWebThemeConfig(self, request):
+        """用来创建页面主题配置
+
+        :param request: Request instance for CreateWebThemeConfig.
+        :type request: :class:`tencentcloud.ess.v20201111.models.CreateWebThemeConfigRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.CreateWebThemeConfigResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateWebThemeConfig", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateWebThemeConfigResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIntegrationDepartment(self, request):
         """通过此接口，删除企业的部门。
 
         :param request: Request instance for DeleteIntegrationDepartment.
         :type request: :class:`tencentcloud.ess.v20201111.models.DeleteIntegrationDepartmentRequest`
```

### Comparing `tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.943/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2251,14 +2251,145 @@
 
     def _deserialize(self, params):
         self._DocumentId = params.get("DocumentId")
         self._PreviewFileUrl = params.get("PreviewFileUrl")
         self._RequestId = params.get("RequestId")
 
 
+class CreateEmbedWebUrlRequest(AbstractModel):
+    """CreateEmbedWebUrl请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Operator: 操作者信息
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param _EmbedType: WEB嵌入资源类型。
+<br/>CREATE_SEAL: 创建印章
+<br/>PREVIEW_SEAL_LIST：预览印章列表
+<br/>PREVIEW_SEAL_DETAIL：预览印章详情
+<br/>EXTEND_SERVICE：拓展服务
+
+        :type EmbedType: str
+        :param _BusinessId: WEB嵌入的业务资源ID
+<br/>PREVIEW_SEAL_DETAIL，必填，取值为印章id
+        :type BusinessId: str
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
+        :param _Reviewer: 抄送方信息
+        :type Reviewer: :class:`tencentcloud.ess.v20201111.models.ReviewerInfo`
+        """
+        self._Operator = None
+        self._EmbedType = None
+        self._BusinessId = None
+        self._Agent = None
+        self._Reviewer = None
+
+    @property
+    def Operator(self):
+        return self._Operator
+
+    @Operator.setter
+    def Operator(self, Operator):
+        self._Operator = Operator
+
+    @property
+    def EmbedType(self):
+        return self._EmbedType
+
+    @EmbedType.setter
+    def EmbedType(self, EmbedType):
+        self._EmbedType = EmbedType
+
+    @property
+    def BusinessId(self):
+        return self._BusinessId
+
+    @BusinessId.setter
+    def BusinessId(self, BusinessId):
+        self._BusinessId = BusinessId
+
+    @property
+    def Agent(self):
+        return self._Agent
+
+    @Agent.setter
+    def Agent(self, Agent):
+        self._Agent = Agent
+
+    @property
+    def Reviewer(self):
+        return self._Reviewer
+
+    @Reviewer.setter
+    def Reviewer(self, Reviewer):
+        self._Reviewer = Reviewer
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self._Operator = UserInfo()
+            self._Operator._deserialize(params.get("Operator"))
+        self._EmbedType = params.get("EmbedType")
+        self._BusinessId = params.get("BusinessId")
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
+        if params.get("Reviewer") is not None:
+            self._Reviewer = ReviewerInfo()
+            self._Reviewer._deserialize(params.get("Reviewer"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateEmbedWebUrlResponse(AbstractModel):
+    """CreateEmbedWebUrl返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _WebUrl: 嵌入的web链接，有效期：5分钟
+EmbedType=PREVIEW_CC_FLOW，该url为h5链接
+        :type WebUrl: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._WebUrl = None
+        self._RequestId = None
+
+    @property
+    def WebUrl(self):
+        return self._WebUrl
+
+    @WebUrl.setter
+    def WebUrl(self, WebUrl):
+        self._WebUrl = WebUrl
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._WebUrl = params.get("WebUrl")
+        self._RequestId = params.get("RequestId")
+
+
 class CreateFlowApproversRequest(AbstractModel):
     """CreateFlowApprovers请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4413,14 +4544,160 @@
             self._QrCode._deserialize(params.get("QrCode"))
         if params.get("SignUrls") is not None:
             self._SignUrls = SignUrl()
             self._SignUrls._deserialize(params.get("SignUrls"))
         self._RequestId = params.get("RequestId")
 
 
+class CreateOrganizationBatchSignUrlRequest(AbstractModel):
+    """CreateOrganizationBatchSignUrl请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Operator: 调用方用户信息，UserId 必填，支持填入集团子公司经办人UserId。
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param _FlowIds: 指定需要进行批量签署的流程id，数量1-100，填写后用户将通过链接对这些合同进行批量签署。
+        :type FlowIds: list of str
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填。
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
+        :param _UserId: 员工的UserId，该UserId对应的员工必须已经加入企业并实名，Name和Mobile为空时该字段不能为空。（优先使用UserId对应的员工）
+        :type UserId: str
+        :param _Name: 员工姓名，该字段需要与Mobile组合使用，UserId为空时该字段不能为空。（UserId为空时，使用Name和Mbile对应的员工）
+        :type Name: str
+        :param _Mobile: 员工手机号码，该字段需要与Name组合使用，UserId为空时该字段不能为空。（UserId为空时，使用Name和Mbile对应的员工）
+        :type Mobile: str
+        """
+        self._Operator = None
+        self._FlowIds = None
+        self._Agent = None
+        self._UserId = None
+        self._Name = None
+        self._Mobile = None
+
+    @property
+    def Operator(self):
+        return self._Operator
+
+    @Operator.setter
+    def Operator(self, Operator):
+        self._Operator = Operator
+
+    @property
+    def FlowIds(self):
+        return self._FlowIds
+
+    @FlowIds.setter
+    def FlowIds(self, FlowIds):
+        self._FlowIds = FlowIds
+
+    @property
+    def Agent(self):
+        return self._Agent
+
+    @Agent.setter
+    def Agent(self, Agent):
+        self._Agent = Agent
+
+    @property
+    def UserId(self):
+        return self._UserId
+
+    @UserId.setter
+    def UserId(self, UserId):
+        self._UserId = UserId
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def Mobile(self):
+        return self._Mobile
+
+    @Mobile.setter
+    def Mobile(self, Mobile):
+        self._Mobile = Mobile
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self._Operator = UserInfo()
+            self._Operator._deserialize(params.get("Operator"))
+        self._FlowIds = params.get("FlowIds")
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
+        self._UserId = params.get("UserId")
+        self._Name = params.get("Name")
+        self._Mobile = params.get("Mobile")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateOrganizationBatchSignUrlResponse(AbstractModel):
+    """CreateOrganizationBatchSignUrl返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _SignUrl: 批量签署入口链接
+        :type SignUrl: str
+        :param _ExpiredTime: 链接过期时间戳
+        :type ExpiredTime: int
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._SignUrl = None
+        self._ExpiredTime = None
+        self._RequestId = None
+
+    @property
+    def SignUrl(self):
+        return self._SignUrl
+
+    @SignUrl.setter
+    def SignUrl(self, SignUrl):
+        self._SignUrl = SignUrl
+
+    @property
+    def ExpiredTime(self):
+        return self._ExpiredTime
+
+    @ExpiredTime.setter
+    def ExpiredTime(self, ExpiredTime):
+        self._ExpiredTime = ExpiredTime
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._SignUrl = params.get("SignUrl")
+        self._ExpiredTime = params.get("ExpiredTime")
+        self._RequestId = params.get("RequestId")
+
+
 class CreatePrepareFlowRequest(AbstractModel):
     """CreatePrepareFlow请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4437,23 +4714,26 @@
         :type Deadline: int
         :param _UserFlowTypeId: 用户自定义合同类型
         :type UserFlowTypeId: str
         :param _Approvers: 签署流程参与者信息，最大限制50方
         :type Approvers: list of FlowCreateApprover
         :param _IntelligentStatus: 打开智能添加填写区(默认开启，打开:"OPEN" 关闭："CLOSE")
         :type IntelligentStatus: str
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填	
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._ResourceId = None
         self._FlowName = None
         self._Unordered = None
         self._Deadline = None
         self._UserFlowTypeId = None
         self._Approvers = None
         self._IntelligentStatus = None
+        self._Agent = None
 
     @property
     def Operator(self):
         return self._Operator
 
     @Operator.setter
     def Operator(self, Operator):
@@ -4511,14 +4791,22 @@
     def IntelligentStatus(self):
         return self._IntelligentStatus
 
     @IntelligentStatus.setter
     def IntelligentStatus(self, IntelligentStatus):
         self._IntelligentStatus = IntelligentStatus
 
+    @property
+    def Agent(self):
+        return self._Agent
+
+    @Agent.setter
+    def Agent(self, Agent):
+        self._Agent = Agent
+
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
         self._ResourceId = params.get("ResourceId")
         self._FlowName = params.get("FlowName")
@@ -4528,14 +4816,17 @@
         if params.get("Approvers") is not None:
             self._Approvers = []
             for item in params.get("Approvers"):
                 obj = FlowCreateApprover()
                 obj._deserialize(item)
                 self._Approvers.append(obj)
         self._IntelligentStatus = params.get("IntelligentStatus")
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -5811,14 +6102,102 @@
         self._AppOriginalId = params.get("AppOriginalId")
         self._Path = params.get("Path")
         self._QrCode = params.get("QrCode")
         self._UrlType = params.get("UrlType")
         self._RequestId = params.get("RequestId")
 
 
+class CreateWebThemeConfigRequest(AbstractModel):
+    """CreateWebThemeConfig请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Operator: 操作人信息
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param _ThemeType: 主题类型
+<br/>EMBED_WEB_THEME：嵌入式主题
+<br/>目前只支持EMBED_WEB_THEME，web页面嵌入的主题风格配置
+        :type ThemeType: str
+        :param _WebThemeConfig: 主题配置
+        :type WebThemeConfig: :class:`tencentcloud.ess.v20201111.models.WebThemeConfig`
+        """
+        self._Operator = None
+        self._ThemeType = None
+        self._WebThemeConfig = None
+
+    @property
+    def Operator(self):
+        return self._Operator
+
+    @Operator.setter
+    def Operator(self, Operator):
+        self._Operator = Operator
+
+    @property
+    def ThemeType(self):
+        return self._ThemeType
+
+    @ThemeType.setter
+    def ThemeType(self, ThemeType):
+        self._ThemeType = ThemeType
+
+    @property
+    def WebThemeConfig(self):
+        return self._WebThemeConfig
+
+    @WebThemeConfig.setter
+    def WebThemeConfig(self, WebThemeConfig):
+        self._WebThemeConfig = WebThemeConfig
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self._Operator = UserInfo()
+            self._Operator._deserialize(params.get("Operator"))
+        self._ThemeType = params.get("ThemeType")
+        if params.get("WebThemeConfig") is not None:
+            self._WebThemeConfig = WebThemeConfig()
+            self._WebThemeConfig._deserialize(params.get("WebThemeConfig"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateWebThemeConfigResponse(AbstractModel):
+    """CreateWebThemeConfig返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._RequestId = params.get("RequestId")
+
+
 class DeleteIntegrationDepartmentRequest(AbstractModel):
     """DeleteIntegrationDepartment请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9784,14 +10163,18 @@
         :type Components: list of Component
         :param _ComponentLimitType: 签署方控件类型为 SIGN_SIGNATURE时，可以指定签署方签名方式
 	HANDWRITE – 手写签名
 	OCR_ESIGN -- AI智能识别手写签名
 	ESIGN -- 个人印章类型
 	SYSTEM_ESIGN -- 系统签名（该类型可以在用户签署时根据用户姓名一键生成一个签名来进行签署）
         :type ComponentLimitType: list of str
+        :param _ApproverVerifyTypes: 合同查看方式<br/>默认1 -实名查看 <br/>2-短信验证码查看(企业签署方暂不支持该方式)
+        :type ApproverVerifyTypes: list of int
+        :param _ApproverSignTypes: 合同签署方式(默认1,2) <br/>1-人脸认证 <br/>2-签署密码 <br/>3-运营商三要素
+        :type ApproverSignTypes: list of int non-negative
         """
         self._ApproverType = None
         self._OrganizationName = None
         self._ApproverName = None
         self._ApproverMobile = None
         self._ApproverIdCardType = None
         self._ApproverIdCardNumber = None
@@ -9808,14 +10191,16 @@
         self._ApproverOption = None
         self._JumpUrl = None
         self._SignId = None
         self._ApproverNeedSignReview = None
         self._SignComponents = None
         self._Components = None
         self._ComponentLimitType = None
+        self._ApproverVerifyTypes = None
+        self._ApproverSignTypes = None
 
     @property
     def ApproverType(self):
         return self._ApproverType
 
     @ApproverType.setter
     def ApproverType(self, ApproverType):
@@ -9997,14 +10382,30 @@
     def ComponentLimitType(self):
         return self._ComponentLimitType
 
     @ComponentLimitType.setter
     def ComponentLimitType(self, ComponentLimitType):
         self._ComponentLimitType = ComponentLimitType
 
+    @property
+    def ApproverVerifyTypes(self):
+        return self._ApproverVerifyTypes
+
+    @ApproverVerifyTypes.setter
+    def ApproverVerifyTypes(self, ApproverVerifyTypes):
+        self._ApproverVerifyTypes = ApproverVerifyTypes
+
+    @property
+    def ApproverSignTypes(self):
+        return self._ApproverSignTypes
+
+    @ApproverSignTypes.setter
+    def ApproverSignTypes(self, ApproverSignTypes):
+        self._ApproverSignTypes = ApproverSignTypes
+
 
     def _deserialize(self, params):
         self._ApproverType = params.get("ApproverType")
         self._OrganizationName = params.get("OrganizationName")
         self._ApproverName = params.get("ApproverName")
         self._ApproverMobile = params.get("ApproverMobile")
         self._ApproverIdCardType = params.get("ApproverIdCardType")
@@ -10036,14 +10437,16 @@
         if params.get("Components") is not None:
             self._Components = []
             for item in params.get("Components"):
                 obj = Component()
                 obj._deserialize(item)
                 self._Components.append(obj)
         self._ComponentLimitType = params.get("ComponentLimitType")
+        self._ApproverVerifyTypes = params.get("ApproverVerifyTypes")
+        self._ApproverSignTypes = params.get("ApproverSignTypes")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -12480,14 +12883,59 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ReviewerInfo(AbstractModel):
+    """关注方信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Name: 姓名
+        :type Name: str
+        :param _Mobile: 手机号
+        :type Mobile: str
+        """
+        self._Name = None
+        self._Mobile = None
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def Mobile(self):
+        return self._Mobile
+
+    @Mobile.setter
+    def Mobile(self, Mobile):
+        self._Mobile = Mobile
+
+
+    def _deserialize(self, params):
+        self._Name = params.get("Name")
+        self._Mobile = params.get("Mobile")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class SealInfo(AbstractModel):
     """模板结构体中的印章信息
 
     """
 
 
 class SignQrCode(AbstractModel):
@@ -14226,8 +14674,57 @@
         if params.get("PdfVerifyResults") is not None:
             self._PdfVerifyResults = []
             for item in params.get("PdfVerifyResults"):
                 obj = PdfVerifyResult()
                 obj._deserialize(item)
                 self._PdfVerifyResults.append(obj)
         self._VerifySerialNo = params.get("VerifySerialNo")
-        self._RequestId = params.get("RequestId")
+        self._RequestId = params.get("RequestId")
+
+
+class WebThemeConfig(AbstractModel):
+    """页面主题配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DisplaySignBrandLogo: 是否页面底部显示电子签logo
+<br/>true：允许在页面底部隐藏电子签logo
+<br/>false：不允许允许在页面底部隐藏电子签logo
+<br/>默认false，不隐藏logo
+        :type DisplaySignBrandLogo: bool
+        :param _WebEmbedThemeColor: 主题颜色
+<br/>支持十六进制颜色值以及RGB格式颜色值，例如：#D54941，rgb(213, 73, 65)
+        :type WebEmbedThemeColor: str
+        """
+        self._DisplaySignBrandLogo = None
+        self._WebEmbedThemeColor = None
+
+    @property
+    def DisplaySignBrandLogo(self):
+        return self._DisplaySignBrandLogo
+
+    @DisplaySignBrandLogo.setter
+    def DisplaySignBrandLogo(self, DisplaySignBrandLogo):
+        self._DisplaySignBrandLogo = DisplaySignBrandLogo
+
+    @property
+    def WebEmbedThemeColor(self):
+        return self._WebEmbedThemeColor
+
+    @WebEmbedThemeColor.setter
+    def WebEmbedThemeColor(self, WebEmbedThemeColor):
+        self._WebEmbedThemeColor = WebEmbedThemeColor
+
+
+    def _deserialize(self, params):
+        self._DisplaySignBrandLogo = params.get("DisplaySignBrandLogo")
+        self._WebEmbedThemeColor = params.get("WebEmbedThemeColor")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+
```

### Comparing `tencentcloud-sdk-python-ess-3.0.943/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.944/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.944/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.943/README.rst` & `tencentcloud-sdk-python-ess-3.0.944/README.rst`

 * *Files identical despite different names*

