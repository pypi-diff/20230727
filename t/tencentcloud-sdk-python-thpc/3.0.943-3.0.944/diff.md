# Comparing `tmp/tencentcloud-sdk-python-thpc-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-thpc-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-thpc-3.0.943.tar", last modified: Wed Jul 26 00:45:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-thpc-3.0.944.tar", last modified: Thu Jul 27 02:25:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-thpc-3.0.943.tar` & `tencentcloud-sdk-python-thpc-3.0.944.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20230321/
--rw-r--r--   0 root         (0) root         (0)    17767 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20230321/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20230321/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4389 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20230321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   157753 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20230321/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20211109/
--rw-r--r--   0 root         (0) root         (0)     4628 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20211109/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20211109/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2035 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20211109/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    63030 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20211109/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20220401/
--rw-r--r--   0 root         (0) root         (0)    16797 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20220401/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20220401/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4733 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20220401/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   142732 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20220401/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud_sdk_python_thpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud_sdk_python_thpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      781 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:45:59.000000 tencentcloud-sdk-python-thpc-3.0.943/tencentcloud_sdk_python_thpc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-27 02:25:07.000000 tencentcloud-sdk-python-thpc-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20230321/
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20230321/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20230321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4389 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20230321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   157753 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20230321/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20211109/
+-rw-r--r--   0 root         (0) root         (0)     4628 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20211109/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20211109/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20211109/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    63030 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20211109/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20220401/
+-rw-r--r--   0 root         (0) root         (0)    16797 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20220401/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20220401/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4733 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20220401/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   142732 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20220401/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-27 02:25:07.000000 tencentcloud-sdk-python-thpc-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud_sdk_python_thpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud_sdk_python_thpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      781 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:25:08.000000 tencentcloud-sdk-python-thpc-3.0.944/tencentcloud_sdk_python_thpc.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.943/setup.py` & `tencentcloud-sdk-python-thpc-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20230321/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20230321/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20230321/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20230321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20230321/models.py` & `tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20230321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20211109/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20211109/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20211109/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20211109/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20211109/models.py` & `tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20211109/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20220401/thpc_client.py` & `tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20220401/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20220401/errorcodes.py` & `tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20220401/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.943/tencentcloud/thpc/v20220401/models.py` & `tencentcloud-sdk-python-thpc-3.0.944/tencentcloud/thpc/v20220401/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-thpc-3.0.944/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-thpc
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Thpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-thpc-3.0.943/README.rst` & `tencentcloud-sdk-python-thpc-3.0.944/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.943/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-thpc-3.0.944/tencentcloud_sdk_python_thpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-thpc-3.0.943/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-thpc-3.0.944/tencentcloud_sdk_python_thpc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-thpc
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Thpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

