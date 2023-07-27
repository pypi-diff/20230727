# Comparing `tmp/tencentcloud-sdk-python-iottid-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-iottid-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iottid-3.0.943.tar", last modified: Wed Jul 26 00:39:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iottid-3.0.944.tar", last modified: Thu Jul 27 02:17:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iottid-3.0.943.tar` & `tencentcloud-sdk-python-iottid-3.0.944.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/tencentcloud/iottid/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/tencentcloud/iottid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/tencentcloud/iottid/v20190411/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/tencentcloud/iottid/v20190411/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9166 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/tencentcloud/iottid/v20190411/iottid_client.py
--rw-r--r--   0 root         (0) root         (0)     1707 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/tencentcloud/iottid/v20190411/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    23421 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/tencentcloud/iottid/v20190411/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/tencentcloud_sdk_python_iottid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/tencentcloud_sdk_python_iottid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/tencentcloud_sdk_python_iottid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/tencentcloud_sdk_python_iottid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/tencentcloud_sdk_python_iottid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-26 00:39:29.000000 tencentcloud-sdk-python-iottid-3.0.943/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/tencentcloud/iottid/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/tencentcloud/iottid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/tencentcloud/iottid/v20190411/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/tencentcloud/iottid/v20190411/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9166 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/tencentcloud/iottid/v20190411/iottid_client.py
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/tencentcloud/iottid/v20190411/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    23421 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/tencentcloud/iottid/v20190411/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/tencentcloud_sdk_python_iottid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/tencentcloud_sdk_python_iottid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/tencentcloud_sdk_python_iottid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/tencentcloud_sdk_python_iottid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/tencentcloud_sdk_python_iottid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-27 02:17:45.000000 tencentcloud-sdk-python-iottid-3.0.944/README.rst
```

### Comparing `tencentcloud-sdk-python-iottid-3.0.943/setup.py` & `tencentcloud-sdk-python-iottid-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iottid-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iottid-3.0.944/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iottid-3.0.943/tencentcloud/iottid/v20190411/iottid_client.py` & `tencentcloud-sdk-python-iottid-3.0.944/tencentcloud/iottid/v20190411/iottid_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iottid-3.0.943/tencentcloud/iottid/v20190411/errorcodes.py` & `tencentcloud-sdk-python-iottid-3.0.944/tencentcloud/iottid/v20190411/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iottid-3.0.943/tencentcloud/iottid/v20190411/models.py` & `tencentcloud-sdk-python-iottid-3.0.944/tencentcloud/iottid/v20190411/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iottid-3.0.943/tencentcloud_sdk_python_iottid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iottid-3.0.944/tencentcloud_sdk_python_iottid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iottid
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Iottid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iottid-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-iottid-3.0.944/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iottid
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Iottid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iottid-3.0.943/README.rst` & `tencentcloud-sdk-python-iottid-3.0.944/README.rst`

 * *Files identical despite different names*
