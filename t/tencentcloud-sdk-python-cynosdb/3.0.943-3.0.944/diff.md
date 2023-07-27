# Comparing `tmp/tencentcloud-sdk-python-cynosdb-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-cynosdb-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.943.tar", last modified: Wed Jul 26 00:35:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.944.tar", last modified: Thu Jul 27 02:13:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cynosdb-3.0.943.tar` & `tencentcloud-sdk-python-cynosdb-3.0.944.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud/cynosdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)   119006 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud/cynosdb/v20190107/cynosdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11292 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   684756 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud_sdk_python_cynosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:35:25.000000 tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud/cynosdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)   119006 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11292 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   685467 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud_sdk_python_cynosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:13:32.000000 tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.943/setup.py` & `tencentcloud-sdk-python-cynosdb-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud/cynosdb/v20190107/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13780,24 +13780,30 @@
         :type Username: str
         :param _Host: 客户端host
         :type Host: str
         :param _Database: 数据库名
         :type Database: str
         :param _FileType: 文件类型，可选值：csv, original
         :type FileType: str
+        :param _OrderBy: 排序字段，可选值： QueryTime,LockTime,RowsExamined,RowsSent
+        :type OrderBy: str
+        :param _OrderByType: 排序类型，可选值：asc,desc
+        :type OrderByType: str
         """
         self._InstanceId = None
         self._StartTime = None
         self._EndTime = None
         self._Limit = None
         self._Offset = None
         self._Username = None
         self._Host = None
         self._Database = None
         self._FileType = None
+        self._OrderBy = None
+        self._OrderByType = None
 
     @property
     def InstanceId(self):
         return self._InstanceId
 
     @InstanceId.setter
     def InstanceId(self, InstanceId):
@@ -13863,25 +13869,43 @@
     def FileType(self):
         return self._FileType
 
     @FileType.setter
     def FileType(self, FileType):
         self._FileType = FileType
 
+    @property
+    def OrderBy(self):
+        return self._OrderBy
+
+    @OrderBy.setter
+    def OrderBy(self, OrderBy):
+        self._OrderBy = OrderBy
+
+    @property
+    def OrderByType(self):
+        return self._OrderByType
+
+    @OrderByType.setter
+    def OrderByType(self, OrderByType):
+        self._OrderByType = OrderByType
+
 
     def _deserialize(self, params):
         self._InstanceId = params.get("InstanceId")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
         self._Limit = params.get("Limit")
         self._Offset = params.get("Offset")
         self._Username = params.get("Username")
         self._Host = params.get("Host")
         self._Database = params.get("Database")
         self._FileType = params.get("FileType")
+        self._OrderBy = params.get("OrderBy")
+        self._OrderByType = params.get("OrderByType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.944/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.943/README.rst` & `tencentcloud-sdk-python-cynosdb-3.0.944/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.943/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.944/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

