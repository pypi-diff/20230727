# Comparing `tmp/tencentcloud-sdk-python-iotvideo-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-iotvideo-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotvideo-3.0.943.tar", last modified: Wed Jul 26 00:39:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotvideo-3.0.944.tar", last modified: Thu Jul 27 02:17:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotvideo-3.0.943.tar` & `tencentcloud-sdk-python-iotvideo-3.0.944.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89241 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)     2198 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   373888 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72567 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   303767 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64723 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)     3098 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   229605 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-26 00:39:33.000000 tencentcloud-sdk-python-iotvideo-3.0.943/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud_sdk_python_iotvideo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud_sdk_python_iotvideo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      861 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:39:34.000000 tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud_sdk_python_iotvideo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20211125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20211125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89241 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20211125/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20211125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   374676 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20211125/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20201215/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20201215/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72567 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20201215/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20201215/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   303767 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20201215/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20191126/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20191126/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64723 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20191126/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20191126/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   229605 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20191126/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud_sdk_python_iotvideo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud_sdk_python_iotvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      861 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:17:52.000000 tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud_sdk_python_iotvideo.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.943/setup.py` & `tencentcloud-sdk-python-iotvideo-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/iotvideo_client.py` & `tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20211125/iotvideo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/errorcodes.py` & `tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20211125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20211125/models.py` & `tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20211125/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -12128,19 +12128,27 @@
         :type Status: int
         :param _CSType: 云存类型，1为全时云存，2为事件云存
         :type CSType: int
         :param _CSShiftDuration: 云存回看时长
         :type CSShiftDuration: int
         :param _CSExpiredTime: 云存套餐过期时间
         :type CSExpiredTime: int
+        :param _CreatedAt: 云存套餐创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreatedAt: int
+        :param _UpdatedAt: 云存套餐更新时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpdatedAt: int
         """
         self._Status = None
         self._CSType = None
         self._CSShiftDuration = None
         self._CSExpiredTime = None
+        self._CreatedAt = None
+        self._UpdatedAt = None
 
     @property
     def Status(self):
         return self._Status
 
     @Status.setter
     def Status(self, Status):
@@ -12166,20 +12174,38 @@
     def CSExpiredTime(self):
         return self._CSExpiredTime
 
     @CSExpiredTime.setter
     def CSExpiredTime(self, CSExpiredTime):
         self._CSExpiredTime = CSExpiredTime
 
+    @property
+    def CreatedAt(self):
+        return self._CreatedAt
+
+    @CreatedAt.setter
+    def CreatedAt(self, CreatedAt):
+        self._CreatedAt = CreatedAt
+
+    @property
+    def UpdatedAt(self):
+        return self._UpdatedAt
+
+    @UpdatedAt.setter
+    def UpdatedAt(self, UpdatedAt):
+        self._UpdatedAt = UpdatedAt
+
 
     def _deserialize(self, params):
         self._Status = params.get("Status")
         self._CSType = params.get("CSType")
         self._CSShiftDuration = params.get("CSShiftDuration")
         self._CSExpiredTime = params.get("CSExpiredTime")
+        self._CreatedAt = params.get("CreatedAt")
+        self._UpdatedAt = params.get("UpdatedAt")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/iotvideo_client.py` & `tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20201215/iotvideo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/errorcodes.py` & `tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20201215/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20201215/models.py` & `tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20201215/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/iotvideo_client.py` & `tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20191126/iotvideo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/errorcodes.py` & `tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20191126/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/iotvideo/v20191126/models.py` & `tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/iotvideo/v20191126/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-iotvideo-3.0.944/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotvideo
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Iotvideo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.943/README.rst` & `tencentcloud-sdk-python-iotvideo-3.0.944/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.943/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotvideo-3.0.944/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotvideo
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Iotvideo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

