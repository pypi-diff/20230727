# Comparing `tmp/tencentcloud-sdk-python-cfs-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-cfs-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.943.tar", last modified: Wed Jul 26 00:33:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.944.tar", last modified: Thu Jul 27 02:11:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfs-3.0.943.tar` & `tencentcloud-sdk-python-cfs-3.0.944.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/tencentcloud/cfs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/tencentcloud/cfs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/tencentcloud/cfs/v20190719/
--rw-r--r--   0 root         (0) root         (0)    40047 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/tencentcloud/cfs/v20190719/cfs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/tencentcloud/cfs/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15890 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/tencentcloud/cfs/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   194257 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/tencentcloud/cfs/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/tencentcloud_sdk_python_cfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-26 00:33:18.000000 tencentcloud-sdk-python-cfs-3.0.943/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/tencentcloud/cfs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/tencentcloud/cfs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/tencentcloud/cfs/v20190719/
+-rw-r--r--   0 root         (0) root         (0)    40047 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/tencentcloud/cfs/v20190719/cfs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/tencentcloud/cfs/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15890 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/tencentcloud/cfs/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   194815 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/tencentcloud/cfs/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/tencentcloud_sdk_python_cfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:11:28.000000 tencentcloud-sdk-python-cfs-3.0.944/README.rst
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.943/setup.py` & `tencentcloud-sdk-python-cfs-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfs-3.0.944/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfs-3.0.943/tencentcloud/cfs/v20190719/cfs_client.py` & `tencentcloud-sdk-python-cfs-3.0.944/tencentcloud/cfs/v20190719/cfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.943/tencentcloud/cfs/v20190719/errorcodes.py` & `tencentcloud-sdk-python-cfs-3.0.944/tencentcloud/cfs/v20190719/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.943/tencentcloud/cfs/v20190719/models.py` & `tencentcloud-sdk-python-cfs-3.0.944/tencentcloud/cfs/v20190719/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2763,18 +2763,24 @@
         r"""
         :param _FileSystemId: 文件系统 ID
         :type FileSystemId: str
         :param _VpcId: 私有网络（VPC） ID
         :type VpcId: str
         :param _SubnetId: 子网 ID
         :type SubnetId: str
+        :param _Offset: Offset 分页码
+        :type Offset: int
+        :param _Limit: Limit 页面大小
+        :type Limit: int
         """
         self._FileSystemId = None
         self._VpcId = None
         self._SubnetId = None
+        self._Offset = None
+        self._Limit = None
 
     @property
     def FileSystemId(self):
         return self._FileSystemId
 
     @FileSystemId.setter
     def FileSystemId(self, FileSystemId):
@@ -2792,19 +2798,37 @@
     def SubnetId(self):
         return self._SubnetId
 
     @SubnetId.setter
     def SubnetId(self, SubnetId):
         self._SubnetId = SubnetId
 
+    @property
+    def Offset(self):
+        return self._Offset
+
+    @Offset.setter
+    def Offset(self, Offset):
+        self._Offset = Offset
+
+    @property
+    def Limit(self):
+        return self._Limit
+
+    @Limit.setter
+    def Limit(self, Limit):
+        self._Limit = Limit
+
 
     def _deserialize(self, params):
         self._FileSystemId = params.get("FileSystemId")
         self._VpcId = params.get("VpcId")
         self._SubnetId = params.get("SubnetId")
+        self._Offset = params.get("Offset")
+        self._Limit = params.get("Limit")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.943/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.944/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.944/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.943/README.rst` & `tencentcloud-sdk-python-cfs-3.0.944/README.rst`

 * *Files identical despite different names*

