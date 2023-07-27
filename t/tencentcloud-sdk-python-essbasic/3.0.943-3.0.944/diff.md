# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.943.tar", last modified: Wed Jul 26 00:37:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.944.tar", last modified: Thu Jul 27 02:15:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.943.tar` & `tencentcloud-sdk-python-essbasic-3.0.944.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    55045 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   387540 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54057 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-26 00:37:28.000000 tencentcloud-sdk-python-essbasic-3.0.943/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:37:29.000000 tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    55990 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   391825 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54057 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:15:44.000000 tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.943/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -500,14 +500,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def ChannelCreateWebThemeConfig(self, request):
+        """生成页面主题配置
+
+        :param request: Request instance for ChannelCreateWebThemeConfig.
+        :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateWebThemeConfigRequest`
+        :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateWebThemeConfigResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ChannelCreateWebThemeConfig", params, headers=headers)
+            response = json.loads(body)
+            model = models.ChannelCreateWebThemeConfigResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def ChannelDeleteRoleUsers(self, request):
         """通过此接口，删除员工绑定的角色，支持以电子签userId、客户系统userId两种方式调用。
 
         :param request: Request instance for ChannelDeleteRoleUsers.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelDeleteRoleUsersRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelDeleteRoleUsersResponse`
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20210526/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3273,14 +3273,101 @@
             for item in params.get("FailedCreateRoleData"):
                 obj = FailedCreateRoleData()
                 obj._deserialize(item)
                 self._FailedCreateRoleData.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class ChannelCreateWebThemeConfigRequest(AbstractModel):
+    """ChannelCreateWebThemeConfig请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
+        :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
+        :param _ThemeType: 主题类型<br/>EMBED_WEB_THEME：嵌入式主题
+<br/>目前只支持EMBED_WEB_THEME，web页面嵌入的主题风格配置
+        :type ThemeType: str
+        :param _WebThemeConfig: 主题配置
+        :type WebThemeConfig: :class:`tencentcloud.essbasic.v20210526.models.WebThemeConfig`
+        """
+        self._Agent = None
+        self._ThemeType = None
+        self._WebThemeConfig = None
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
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
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
+class ChannelCreateWebThemeConfigResponse(AbstractModel):
+    """ChannelCreateWebThemeConfig返回参数结构体
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
 class ChannelDeleteRoleUsersRequest(AbstractModel):
     """ChannelDeleteRoleUsers请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -12135,8 +12222,56 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class WebThemeConfig(AbstractModel):
+    """主题配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DisplaySignBrandLogo: 页面底部是否显示电子签logo
+<br/>true：允许在页面底部隐藏电子签logo 
+<br/>默认false，不允许允许在页面底部隐藏电子签logo
+        :type DisplaySignBrandLogo: bool
+        :param _WebEmbedThemeColor: 嵌入式主题颜色
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
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.944/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.943/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.944/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.943/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.944/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

