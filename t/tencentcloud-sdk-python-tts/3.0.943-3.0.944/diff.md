# Comparing `tmp/tencentcloud-sdk-python-tts-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-tts-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.943.tar", last modified: Wed Jul 26 00:47:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.944.tar", last modified: Thu Jul 27 02:27:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tts-3.0.943.tar` & `tencentcloud-sdk-python-tts-3.0.944.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:47:50.000000 tencentcloud-sdk-python-tts-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-26 00:47:48.000000 tencentcloud-sdk-python-tts-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:47:50.000000 tencentcloud-sdk-python-tts-3.0.943/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:47:50.000000 tencentcloud-sdk-python-tts-3.0.943/tencentcloud/tts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:47:48.000000 tencentcloud-sdk-python-tts-3.0.943/tencentcloud/tts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:47:50.000000 tencentcloud-sdk-python-tts-3.0.943/tencentcloud/tts/v20190823/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:47:48.000000 tencentcloud-sdk-python-tts-3.0.943/tencentcloud/tts/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5572 2023-07-26 00:47:48.000000 tencentcloud-sdk-python-tts-3.0.943/tencentcloud/tts/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    23658 2023-07-26 00:47:48.000000 tencentcloud-sdk-python-tts-3.0.943/tencentcloud/tts/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)     5922 2023-07-26 00:47:48.000000 tencentcloud-sdk-python-tts-3.0.943/tencentcloud/tts/v20190823/tts_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:47:48.000000 tencentcloud-sdk-python-tts-3.0.943/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:47:50.000000 tencentcloud-sdk-python-tts-3.0.943/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:47:50.000000 tencentcloud-sdk-python-tts-3.0.943/tencentcloud_sdk_python_tts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:47:50.000000 tencentcloud-sdk-python-tts-3.0.943/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-26 00:47:50.000000 tencentcloud-sdk-python-tts-3.0.943/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:47:50.000000 tencentcloud-sdk-python-tts-3.0.943/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:47:50.000000 tencentcloud-sdk-python-tts-3.0.943/tencentcloud_sdk_python_tts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:47:50.000000 tencentcloud-sdk-python-tts-3.0.943/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-26 00:47:48.000000 tencentcloud-sdk-python-tts-3.0.943/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    23692 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/models.py
+-rw-r--r--   0 root         (0) root         (0)     5922 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/tts_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud_sdk_python_tts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud_sdk_python_tts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/README.rst
```

### Comparing `tencentcloud-sdk-python-tts-3.0.943/setup.py` & `tencentcloud-sdk-python-tts-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.943/tencentcloud/tts/v20190823/errorcodes.py` & `tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.943/tencentcloud/tts/v20190823/models.py` & `tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         :type Volume: float
         :param _Speed: 语速，范围：[-2，2]，分别对应不同语速：<li>-2代表0.6倍</li><li>-1代表0.8倍</li><li>0代表1.0倍（默认）</li><li>1代表1.2倍</li><li>2代表1.5倍</li>如果需要更细化的语速，可以保留小数点后 2 位，例如0.5 1.1 1.8等。<br>参数值与实际语速转换，可参考[代码示例](https://sdk-1300466766.cos.ap-shanghai.myqcloud.com/sample/speed_sample.tar.gz)
         :type Speed: float
         :param _ProjectId: 项目id，用户自定义，默认为0。
         :type ProjectId: int
         :param _VoiceType: 音色 ID，包括标准音色与精品音色，精品音色拟真度更高，价格不同于标准音色，请参见[购买指南](https://cloud.tencent.com/document/product/1073/34112)。完整的音色 ID 列表请参见[音色列表](https://cloud.tencent.com/document/product/1073/92668)。
         :type VoiceType: int
-        :param _PrimaryLanguage: 主语言类型：<li>1-中文（默认）</li><li>2-英文</li>
+        :param _PrimaryLanguage: 主语言类型：<li>1-中文（默认）</li><li>2-英文</li><li>3-日文</li>
         :type PrimaryLanguage: int
         :param _SampleRate: 音频采样率：<li>16000：16k（默认）</li><li>8000：8k</li>
         :type SampleRate: int
         :param _Codec: 返回音频格式，可取值：mp3（默认），wav，pcm
         :type Codec: str
         :param _CallbackUrl: 回调 URL，用户自行搭建的用于接收识别结果的服务URL。如果用户使用轮询方式获取识别结果，则无需提交该参数。[回调说明](https://cloud.tencent.com/document/product/1073/55746)
         :type CallbackUrl: str
@@ -508,15 +508,15 @@
         :type Speed: float
         :param _ProjectId: 项目id，用户自定义，默认为0。
         :type ProjectId: int
         :param _ModelType: 模型类型，1-默认模型。
         :type ModelType: int
         :param _VoiceType: 音色 ID，包括标准音色与精品音色，精品音色拟真度更高，价格不同于标准音色，请参见[购买指南](https://cloud.tencent.com/document/product/1073/34112)。完整的音色 ID 列表请参见[音色列表](https://cloud.tencent.com/document/product/1073/92668)。
         :type VoiceType: int
-        :param _PrimaryLanguage: 主语言类型：<li>1-中文（默认）</li><li>2-英文</li>
+        :param _PrimaryLanguage: 主语言类型：<li>1-中文（默认）</li><li>2-英文</li><li>3-日文</li>
         :type PrimaryLanguage: int
         :param _SampleRate: 音频采样率：
 <li>24000：24k（部分音色支持，请参见[音色列表](https://cloud.tencent.com/document/product/1073/92668)）</li>
 <li>16000：16k（默认）</li>
 <li>8000：8k</li>
         :type SampleRate: int
         :param _Codec: 返回音频格式，可取值：wav（默认），mp3，pcm
```

### Comparing `tencentcloud-sdk-python-tts-3.0.943/tencentcloud/tts/v20190823/tts_client.py` & `tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/tts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tts-3.0.944/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tts-3.0.943/tencentcloud_sdk_python_tts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.944/tencentcloud_sdk_python_tts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.944/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.943/README.rst` & `tencentcloud-sdk-python-tts-3.0.944/README.rst`

 * *Files identical despite different names*

