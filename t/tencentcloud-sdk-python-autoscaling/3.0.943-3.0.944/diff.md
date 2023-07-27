# Comparing `tmp/tencentcloud-sdk-python-autoscaling-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-autoscaling-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.943.tar", last modified: Wed Jul 26 00:30:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.944.tar", last modified: Thu Jul 27 02:08:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-autoscaling-3.0.943.tar` & `tencentcloud-sdk-python-autoscaling-3.0.944.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud/autoscaling/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud/autoscaling/v20180419/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud/autoscaling/v20180419/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19989 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud/autoscaling/v20180419/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    60726 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud/autoscaling/v20180419/autoscaling_client.py
--rw-r--r--   0 root         (0) root         (0)   392015 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud/autoscaling/v20180419/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud/autoscaling/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud_sdk_python_autoscaling.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      525 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      761 2023-07-26 00:30:57.000000 tencentcloud-sdk-python-autoscaling-3.0.943/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud/autoscaling/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud/autoscaling/v20180419/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud/autoscaling/v20180419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19989 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud/autoscaling/v20180419/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    60726 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud/autoscaling/v20180419/autoscaling_client.py
+-rw-r--r--   0 root         (0) root         (0)   392015 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud/autoscaling/v20180419/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud/autoscaling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud_sdk_python_autoscaling.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      525 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-27 02:08:58.000000 tencentcloud-sdk-python-autoscaling-3.0.944/README.rst
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.943/setup.py` & `tencentcloud-sdk-python-autoscaling-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud/autoscaling/v20180419/errorcodes.py` & `tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud/autoscaling/v20180419/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud/autoscaling/v20180419/autoscaling_client.py` & `tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud/autoscaling/v20180419/autoscaling_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud/autoscaling/v20180419/models.py` & `tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud/autoscaling/v20180419/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.943/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.944/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.944/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.943/README.rst` & `tencentcloud-sdk-python-autoscaling-3.0.944/README.rst`

 * *Files identical despite different names*

