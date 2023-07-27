# Comparing `tmp/tencentcloud-sdk-python-lcic-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-lcic-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.943.tar", last modified: Wed Jul 26 00:40:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.944.tar", last modified: Thu Jul 27 02:18:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lcic-3.0.943.tar` & `tencentcloud-sdk-python-lcic-3.0.944.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/tencentcloud/lcic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48865 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/tencentcloud/lcic/v20220817/lcic_client.py
--rw-r--r--   0 root         (0) root         (0)     4414 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   233364 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/tencentcloud/lcic/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/tencentcloud_sdk_python_lcic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-26 00:40:03.000000 tencentcloud-sdk-python-lcic-3.0.943/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:18:27.000000 tencentcloud-sdk-python-lcic-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-27 02:18:26.000000 tencentcloud-sdk-python-lcic-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:18:27.000000 tencentcloud-sdk-python-lcic-3.0.944/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:18:26.000000 tencentcloud-sdk-python-lcic-3.0.944/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:18:27.000000 tencentcloud-sdk-python-lcic-3.0.944/tencentcloud/lcic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:18:27.000000 tencentcloud-sdk-python-lcic-3.0.944/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:18:26.000000 tencentcloud-sdk-python-lcic-3.0.944/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48865 2023-07-27 02:18:26.000000 tencentcloud-sdk-python-lcic-3.0.944/tencentcloud/lcic/v20220817/lcic_client.py
+-rw-r--r--   0 root         (0) root         (0)     4414 2023-07-27 02:18:26.000000 tencentcloud-sdk-python-lcic-3.0.944/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   233364 2023-07-27 02:18:26.000000 tencentcloud-sdk-python-lcic-3.0.944/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:18:26.000000 tencentcloud-sdk-python-lcic-3.0.944/tencentcloud/lcic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:18:27.000000 tencentcloud-sdk-python-lcic-3.0.944/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:18:27.000000 tencentcloud-sdk-python-lcic-3.0.944/tencentcloud_sdk_python_lcic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:18:27.000000 tencentcloud-sdk-python-lcic-3.0.944/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-27 02:18:27.000000 tencentcloud-sdk-python-lcic-3.0.944/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-27 02:18:27.000000 tencentcloud-sdk-python-lcic-3.0.944/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:18:27.000000 tencentcloud-sdk-python-lcic-3.0.944/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-27 02:18:27.000000 tencentcloud-sdk-python-lcic-3.0.944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-27 02:18:26.000000 tencentcloud-sdk-python-lcic-3.0.944/README.rst
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.943/setup.py` & `tencentcloud-sdk-python-lcic-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lcic-3.0.944/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lcic-3.0.943/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-lcic-3.0.944/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.943/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-lcic-3.0.944/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.943/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-lcic-3.0.944/tencentcloud/lcic/v20220817/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5158,16 +5158,16 @@
 
     def __init__(self):
         r"""
         :param _Timestamp: 事件发生的秒级unix时间戳。
         :type Timestamp: int
         :param _EventType: 事件类型,有以下值:
 RoomStart:房间开始 RoomEnd:房间结束 MemberJoin:成员加入 MemberQuit:成员退出 RecordFinish:录制结束
-Camera0n: 摄像头打开
-Camera0ff: 摄像头关闭
+CameraOn: 摄像头打开
+CameraOff: 摄像头关闭
 MicOn: 麦克风打开
 MicOff: 麦克风关闭
 ScreenOn: 屏幕共享打开
 ScreenOff: 屏幕共享关闭
 VisibleOn: 页面可见
 VisibleOff: 页面不可见
         :type EventType: str
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.943/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.944/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.944/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.943/README.rst` & `tencentcloud-sdk-python-lcic-3.0.944/README.rst`

 * *Files identical despite different names*

