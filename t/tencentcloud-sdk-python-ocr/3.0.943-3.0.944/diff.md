# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.943.tar", last modified: Wed Jul 26 00:41:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.944.tar", last modified: Thu Jul 27 02:20:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.943.tar` & `tencentcloud-sdk-python-ocr-3.0.944.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5894 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   115946 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)   820213 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-26 00:41:51.000000 tencentcloud-sdk-python-ocr-3.0.943/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   115943 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)   821044 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/README.rst
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.943/setup.py` & `tencentcloud-sdk-python-ocr-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2212,15 +2212,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VatInvoiceOCR(self, request):
-        """本接口支持增值税专用发票、增值税普通发票、增值税电子专票、增值税电子普票、电子发票（普通发票）、电子发票（增值税专用发票）德全字段的内容检测和识别，包括发票代码、发票号码、打印发票代码、打印发票号码、开票日期、合计金额、校验码、税率、合计税额、价税合计、购买方识别号、复核、销售方识别号、开票人、密码区1、密码区2、密码区3、密码区4、发票名称、购买方名称、销售方名称、服务名称、备注、规格型号、数量、单价、金额、税额、收款人等字段，点击[立即试用](https://cloud.tencent.com/product/ocr)。
+        """本接口支持增值税专用发票、增值税普通发票、增值税电子专票、增值税电子普票、电子发票（普通发票）、电子发票（增值税专用发票）全字段的内容检测和识别，包括发票代码、发票号码、打印发票代码、打印发票号码、开票日期、合计金额、校验码、税率、合计税额、价税合计、购买方识别号、复核、销售方识别号、开票人、密码区1、密码区2、密码区3、密码区4、发票名称、购买方名称、销售方名称、服务名称、备注、规格型号、数量、单价、金额、税额、收款人等字段，点击[立即试用](https://cloud.tencent.com/product/ocr)。
 
         默认接口请求频率限制：10次/秒。
 
         :param request: Request instance for VatInvoiceOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.VatInvoiceOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.VatInvoiceOCRResponse`
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.943/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6252,19 +6252,22 @@
 ReflectWarn，是否开启反光检测
 
 SDK 设置方式参考：
 Config = Json.stringify({"CropIdCard":true,"CropPortrait":true})
 API 3.0 Explorer 设置方式参考：
 Config = {"CropIdCard":true,"CropPortrait":true}
         :type Config: str
+        :param _EnableRecognitionRectify: 默认值为true，打开识别结果纠正开关。开关开启后，身份证号、出生日期、性别，三个字段会进行矫正补齐，统一结果输出；若关闭此开关，以上三个字段不会进行矫正补齐，保持原始识别结果输出，若原图出现篡改情况，这三个字段的识别结果可能会不统一。
+        :type EnableRecognitionRectify: bool
         """
         self._ImageBase64 = None
         self._ImageUrl = None
         self._CardSide = None
         self._Config = None
+        self._EnableRecognitionRectify = None
 
     @property
     def ImageBase64(self):
         return self._ImageBase64
 
     @ImageBase64.setter
     def ImageBase64(self, ImageBase64):
@@ -6290,20 +6293,29 @@
     def Config(self):
         return self._Config
 
     @Config.setter
     def Config(self, Config):
         self._Config = Config
 
+    @property
+    def EnableRecognitionRectify(self):
+        return self._EnableRecognitionRectify
+
+    @EnableRecognitionRectify.setter
+    def EnableRecognitionRectify(self, EnableRecognitionRectify):
+        self._EnableRecognitionRectify = EnableRecognitionRectify
+
 
     def _deserialize(self, params):
         self._ImageBase64 = params.get("ImageBase64")
         self._ImageUrl = params.get("ImageUrl")
         self._CardSide = params.get("CardSide")
         self._Config = params.get("Config")
+        self._EnableRecognitionRectify = params.get("EnableRecognitionRectify")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.943/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.944/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.944/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.943/README.rst` & `tencentcloud-sdk-python-ocr-3.0.944/README.rst`

 * *Files identical despite different names*

