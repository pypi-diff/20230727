# Comparing `tmp/tencentcloud-sdk-python-asr-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-asr-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.943.tar", last modified: Wed Jul 26 00:30:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.944.tar", last modified: Thu Jul 27 02:08:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asr-3.0.943.tar` & `tencentcloud-sdk-python-asr-3.0.944.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud_sdk_python_asr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud_sdk_python_asr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29417 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)     7480 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   112062 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-26 00:30:47.000000 tencentcloud-sdk-python-asr-3.0.943/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/tencentcloud_sdk_python_asr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/tencentcloud_sdk_python_asr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/tencentcloud/asr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29417 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/tencentcloud/asr/v20190614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   112062 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/tencentcloud/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:08:48.000000 tencentcloud-sdk-python-asr-3.0.944/README.rst
```

### Comparing `tencentcloud-sdk-python-asr-3.0.943/setup.py` & `tencentcloud-sdk-python-asr-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.943/tencentcloud_sdk_python_asr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.944/tencentcloud_sdk_python_asr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-asr-3.0.944/tencentcloud/asr/v20190614/asr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-asr-3.0.944/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.943/tencentcloud/asr/v20190614/models.py` & `tencentcloud-sdk-python-asr-3.0.944/tencentcloud/asr/v20190614/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asr-3.0.944/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-asr-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.944/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.943/README.rst` & `tencentcloud-sdk-python-asr-3.0.944/README.rst`

 * *Files identical despite different names*

