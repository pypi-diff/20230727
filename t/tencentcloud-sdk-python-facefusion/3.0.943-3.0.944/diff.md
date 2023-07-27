# Comparing `tmp/tencentcloud-sdk-python-facefusion-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-facefusion-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-facefusion-3.0.943.tar", last modified: Wed Jul 26 00:37:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-facefusion-3.0.944.tar", last modified: Thu Jul 27 02:15:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-facefusion-3.0.943.tar` & `tencentcloud-sdk-python-facefusion-3.0.944.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud_sdk_python_facefusion.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud_sdk_python_facefusion.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      708 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud_sdk_python_facefusion.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20220927/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20220927/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3394 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20220927/facefusion_client.py
--rw-r--r--   0 root         (0) root         (0)     5459 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20220927/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    20924 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20220927/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20181201/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20181201/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5785 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20181201/facefusion_client.py
--rw-r--r--   0 root         (0) root         (0)     6738 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20181201/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    35069 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20181201/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-26 00:37:35.000000 tencentcloud-sdk-python-facefusion-3.0.943/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud_sdk_python_facefusion.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud_sdk_python_facefusion.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      708 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud_sdk_python_facefusion.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20220927/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20220927/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20220927/facefusion_client.py
+-rw-r--r--   0 root         (0) root         (0)     5459 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20220927/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    24611 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20220927/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20181201/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20181201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5785 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20181201/facefusion_client.py
+-rw-r--r--   0 root         (0) root         (0)     6738 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20181201/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    39231 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20181201/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-27 02:15:50.000000 tencentcloud-sdk-python-facefusion-3.0.944/README.rst
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.943/setup.py` & `tencentcloud-sdk-python-facefusion-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO` & `tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-facefusion
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Facefusion SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20220927/facefusion_client.py` & `tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20220927/facefusion_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20220927/errorcodes.py` & `tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20220927/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20220927/models.py` & `tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20220927/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -305,23 +305,26 @@
 0：不添加标识。
 其他数值：默认按1处理。
 建议您使用显著标识来提示结果图使用了人脸融合技术，是AI合成的图片。
         :type LogoAdd: int
         :param _LogoParam: 标识内容设置。
 默认在融合结果图右下角添加“本图片为AI合成图片”字样，您可根据自身需要替换为其他的Logo图片。
         :type LogoParam: :class:`tencentcloud.facefusion.v20220927.models.LogoParam`
+        :param _FuseParam: 融合参数。
+        :type FuseParam: :class:`tencentcloud.facefusion.v20220927.models.FuseParam`
         """
         self._ProjectId = None
         self._ModelId = None
         self._RspImgType = None
         self._MergeInfos = None
         self._FuseProfileDegree = None
         self._FuseFaceDegree = None
         self._LogoAdd = None
         self._LogoParam = None
+        self._FuseParam = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
@@ -379,14 +382,22 @@
     def LogoParam(self):
         return self._LogoParam
 
     @LogoParam.setter
     def LogoParam(self, LogoParam):
         self._LogoParam = LogoParam
 
+    @property
+    def FuseParam(self):
+        return self._FuseParam
+
+    @FuseParam.setter
+    def FuseParam(self, FuseParam):
+        self._FuseParam = FuseParam
+
 
     def _deserialize(self, params):
         self._ProjectId = params.get("ProjectId")
         self._ModelId = params.get("ModelId")
         self._RspImgType = params.get("RspImgType")
         if params.get("MergeInfos") is not None:
             self._MergeInfos = []
@@ -396,14 +407,17 @@
                 self._MergeInfos.append(obj)
         self._FuseProfileDegree = params.get("FuseProfileDegree")
         self._FuseFaceDegree = params.get("FuseFaceDegree")
         self._LogoAdd = params.get("LogoAdd")
         if params.get("LogoParam") is not None:
             self._LogoParam = LogoParam()
             self._LogoParam._deserialize(params.get("LogoParam"))
+        if params.get("FuseParam") is not None:
+            self._FuseParam = FuseParam()
+            self._FuseParam._deserialize(params.get("FuseParam"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -443,14 +457,87 @@
 
 
     def _deserialize(self, params):
         self._FusedImage = params.get("FusedImage")
         self._RequestId = params.get("RequestId")
 
 
+class FuseParam(AbstractModel):
+    """融合参数
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ImageCodecParam: 图片编码参数
+        :type ImageCodecParam: :class:`tencentcloud.facefusion.v20220927.models.ImageCodecParam`
+        """
+        self._ImageCodecParam = None
+
+    @property
+    def ImageCodecParam(self):
+        return self._ImageCodecParam
+
+    @ImageCodecParam.setter
+    def ImageCodecParam(self, ImageCodecParam):
+        self._ImageCodecParam = ImageCodecParam
+
+
+    def _deserialize(self, params):
+        if params.get("ImageCodecParam") is not None:
+            self._ImageCodecParam = ImageCodecParam()
+            self._ImageCodecParam._deserialize(params.get("ImageCodecParam"))
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
+class ImageCodecParam(AbstractModel):
+    """图片编码参数
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _MetaData: 元数据
+        :type MetaData: list of MetaData
+        """
+        self._MetaData = None
+
+    @property
+    def MetaData(self):
+        return self._MetaData
+
+    @MetaData.setter
+    def MetaData(self, MetaData):
+        self._MetaData = MetaData
+
+
+    def _deserialize(self, params):
+        if params.get("MetaData") is not None:
+            self._MetaData = []
+            for item in params.get("MetaData"):
+                obj = MetaData()
+                obj._deserialize(item)
+                self._MetaData.append(obj)
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
 class LogoParam(AbstractModel):
     """logo参数
 
     """
 
     def __init__(self):
         r"""
@@ -617,14 +704,59 @@
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
+class MetaData(AbstractModel):
+    """MetaData数据结构，Key/Value格式
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _MetaKey: MetaData的Key
+        :type MetaKey: str
+        :param _MetaValue: MetaData的Value
+        :type MetaValue: str
+        """
+        self._MetaKey = None
+        self._MetaValue = None
+
+    @property
+    def MetaKey(self):
+        return self._MetaKey
+
+    @MetaKey.setter
+    def MetaKey(self, MetaKey):
+        self._MetaKey = MetaKey
+
+    @property
+    def MetaValue(self):
+        return self._MetaValue
+
+    @MetaValue.setter
+    def MetaValue(self, MetaValue):
+        self._MetaValue = MetaValue
+
+
+    def _deserialize(self, params):
+        self._MetaKey = params.get("MetaKey")
+        self._MetaValue = params.get("MetaValue")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class PublicMaterialInfos(AbstractModel):
     """素材信息
 
     """
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20181201/facefusion_client.py` & `tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20181201/facefusion_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20181201/errorcodes.py` & `tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20181201/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/facefusion/v20181201/models.py` & `tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/facefusion/v20181201/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -312,22 +312,25 @@
         :param _PornDetect: 历史遗留字段，无需填写。因为融合只需提取人脸特征，不需要鉴黄。
         :type PornDetect: int
         :param _CelebrityIdentify: 0表示不需要不适宜内容识别，1表示需要不适宜内容识别。默认值为0。
 请注意，不适宜内容识别服务开启后，您需要根据返回结果自行判断是否调整您的业务逻辑。例如提示您的用户图片非法，请更换图片。
         :type CelebrityIdentify: int
         :param _Url: 图片Url地址
         :type Url: str
+        :param _FuseParam: 融合参数
+        :type FuseParam: :class:`tencentcloud.facefusion.v20181201.models.FuseParam`
         """
         self._ProjectId = None
         self._ModelId = None
         self._RspImgType = None
         self._Image = None
         self._PornDetect = None
         self._CelebrityIdentify = None
         self._Url = None
+        self._FuseParam = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
@@ -377,23 +380,34 @@
     def Url(self):
         return self._Url
 
     @Url.setter
     def Url(self, Url):
         self._Url = Url
 
+    @property
+    def FuseParam(self):
+        return self._FuseParam
+
+    @FuseParam.setter
+    def FuseParam(self, FuseParam):
+        self._FuseParam = FuseParam
+
 
     def _deserialize(self, params):
         self._ProjectId = params.get("ProjectId")
         self._ModelId = params.get("ModelId")
         self._RspImgType = params.get("RspImgType")
         self._Image = params.get("Image")
         self._PornDetect = params.get("PornDetect")
         self._CelebrityIdentify = params.get("CelebrityIdentify")
         self._Url = params.get("Url")
+        if params.get("FuseParam") is not None:
+            self._FuseParam = FuseParam()
+            self._FuseParam._deserialize(params.get("FuseParam"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -612,22 +626,25 @@
         :type FuseProfileDegree: int
         :param _FuseFaceDegree: 五官融合比例，数值越高，融合后的五官越像素材人物。取值范围[0,100] 
 若此参数不填写，则使用人脸融合控制台中五官参数数值。（换脸版算法暂不支持此参数调整）
         :type FuseFaceDegree: int
         :param _CelebrityIdentify: 0表示不需要不适宜内容识别，1表示需要不适宜内容识别。默认值为0。
 请注意，不适宜内容识别服务开启后，您需要根据返回结果自行判断是否调整您的业务逻辑。例如提示您的用户图片非法，请更换图片。
         :type CelebrityIdentify: int
+        :param _FuseParam: 融合参数
+        :type FuseParam: :class:`tencentcloud.facefusion.v20181201.models.FuseParam`
         """
         self._ProjectId = None
         self._ModelId = None
         self._RspImgType = None
         self._MergeInfos = None
         self._FuseProfileDegree = None
         self._FuseFaceDegree = None
         self._CelebrityIdentify = None
+        self._FuseParam = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
@@ -677,28 +694,39 @@
     def CelebrityIdentify(self):
         return self._CelebrityIdentify
 
     @CelebrityIdentify.setter
     def CelebrityIdentify(self, CelebrityIdentify):
         self._CelebrityIdentify = CelebrityIdentify
 
+    @property
+    def FuseParam(self):
+        return self._FuseParam
+
+    @FuseParam.setter
+    def FuseParam(self, FuseParam):
+        self._FuseParam = FuseParam
+
 
     def _deserialize(self, params):
         self._ProjectId = params.get("ProjectId")
         self._ModelId = params.get("ModelId")
         self._RspImgType = params.get("RspImgType")
         if params.get("MergeInfos") is not None:
             self._MergeInfos = []
             for item in params.get("MergeInfos"):
                 obj = MergeInfo()
                 obj._deserialize(item)
                 self._MergeInfos.append(obj)
         self._FuseProfileDegree = params.get("FuseProfileDegree")
         self._FuseFaceDegree = params.get("FuseFaceDegree")
         self._CelebrityIdentify = params.get("CelebrityIdentify")
+        if params.get("FuseParam") is not None:
+            self._FuseParam = FuseParam()
+            self._FuseParam._deserialize(params.get("FuseParam"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -929,14 +957,87 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class FuseParam(AbstractModel):
+    """融合参数
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ImageCodecParam: 图片编码参数
+        :type ImageCodecParam: :class:`tencentcloud.facefusion.v20181201.models.ImageCodecParam`
+        """
+        self._ImageCodecParam = None
+
+    @property
+    def ImageCodecParam(self):
+        return self._ImageCodecParam
+
+    @ImageCodecParam.setter
+    def ImageCodecParam(self, ImageCodecParam):
+        self._ImageCodecParam = ImageCodecParam
+
+
+    def _deserialize(self, params):
+        if params.get("ImageCodecParam") is not None:
+            self._ImageCodecParam = ImageCodecParam()
+            self._ImageCodecParam._deserialize(params.get("ImageCodecParam"))
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
+class ImageCodecParam(AbstractModel):
+    """图片编码参数
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _MetaData: 元数据
+        :type MetaData: list of MetaData
+        """
+        self._MetaData = None
+
+    @property
+    def MetaData(self):
+        return self._MetaData
+
+    @MetaData.setter
+    def MetaData(self, MetaData):
+        self._MetaData = MetaData
+
+
+    def _deserialize(self, params):
+        if params.get("MetaData") is not None:
+            self._MetaData = []
+            for item in params.get("MetaData"):
+                obj = MetaData()
+                obj._deserialize(item)
+                self._MetaData.append(obj)
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
 class MaterialFaceList(AbstractModel):
     """人脸信息
 
     """
 
     def __init__(self):
         r"""
@@ -1044,14 +1145,59 @@
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
+class MetaData(AbstractModel):
+    """MetaData数据结构，Key/Value格式
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _MetaKey: MetaData的Key
+        :type MetaKey: str
+        :param _MetaValue: MetaData的Value
+        :type MetaValue: str
+        """
+        self._MetaKey = None
+        self._MetaValue = None
+
+    @property
+    def MetaKey(self):
+        return self._MetaKey
+
+    @MetaKey.setter
+    def MetaKey(self, MetaKey):
+        self._MetaKey = MetaKey
+
+    @property
+    def MetaValue(self):
+        return self._MetaValue
+
+    @MetaValue.setter
+    def MetaValue(self, MetaValue):
+        self._MetaValue = MetaValue
+
+
+    def _deserialize(self, params):
+        self._MetaKey = params.get("MetaKey")
+        self._MetaValue = params.get("MetaValue")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class PublicMaterialInfos(AbstractModel):
     """素材信息
 
     """
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-facefusion-3.0.944/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-facefusion-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-facefusion-3.0.944/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-facefusion
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Facefusion SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.943/README.rst` & `tencentcloud-sdk-python-facefusion-3.0.944/README.rst`

 * *Files identical despite different names*

