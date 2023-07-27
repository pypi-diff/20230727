# Comparing `tmp/tencentcloud-sdk-python-postgres-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-postgres-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.943.tar", last modified: Wed Jul 26 00:42:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.944.tar", last modified: Thu Jul 27 02:20:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-postgres-3.0.943.tar` & `tencentcloud-sdk-python-postgres-3.0.944.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/tencentcloud/postgres/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/tencentcloud/postgres/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/tencentcloud/postgres/v20170312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/tencentcloud/postgres/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20749 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/tencentcloud/postgres/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    86440 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/tencentcloud/postgres/v20170312/postgres_client.py
--rw-r--r--   0 root         (0) root         (0)   454366 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/tencentcloud/postgres/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/tencentcloud_sdk_python_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-26 00:42:15.000000 tencentcloud-sdk-python-postgres-3.0.943/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/tencentcloud/postgres/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/tencentcloud/postgres/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/tencentcloud/postgres/v20170312/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/tencentcloud/postgres/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20749 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/tencentcloud/postgres/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    86440 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/tencentcloud/postgres/v20170312/postgres_client.py
+-rw-r--r--   0 root         (0) root         (0)   455360 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/tencentcloud/postgres/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/tencentcloud_sdk_python_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-27 02:20:57.000000 tencentcloud-sdk-python-postgres-3.0.944/README.rst
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.943/setup.py` & `tencentcloud-sdk-python-postgres-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-postgres-3.0.944/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-postgres-3.0.943/tencentcloud/postgres/v20170312/errorcodes.py` & `tencentcloud-sdk-python-postgres-3.0.944/tencentcloud/postgres/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.943/tencentcloud/postgres/v20170312/postgres_client.py` & `tencentcloud-sdk-python-postgres-3.0.944/tencentcloud/postgres/v20170312/postgres_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.943/tencentcloud/postgres/v20170312/models.py` & `tencentcloud-sdk-python-postgres-3.0.944/tencentcloud/postgres/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2508,75 +2508,107 @@
 class CreateReadOnlyDBInstanceRequest(AbstractModel):
     """CreateReadOnlyDBInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _SpecCode: 售卖规格ID。该参数可以通过调用DescribeClasses的返回值中的SpecCode字段来获取。
+        :param _Zone: 实例所属主可用区， 如：ap-guangzhou-3；
+可用区信息可以通过调用 [DescribeZones](https://cloud.tencent.com/document/api/409/16769) 接口的返回值中的Zone字段来获取。
+        :type Zone: str
+        :param _MasterDBInstanceId: 只读实例的主实例ID。
+        :type MasterDBInstanceId: str
+        :param _SpecCode: 售卖规格码。该参数可以通过调用[DescribeClasses](https://cloud.tencent.com/document/api/409/89019)的返回值中的SpecCode字段来获取。
         :type SpecCode: str
         :param _Storage: 实例容量大小，单位：GB。
         :type Storage: int
-        :param _InstanceCount: 一次性购买的实例数量。取值1-100
+        :param _InstanceCount: 购买实例数量，取值范围：[1-10]。一次性购买支持最大数量10个，若超过该数量，可进行多次调用进行购买。
         :type InstanceCount: int
-        :param _Period: 购买时长，单位：月。目前只支持1,2,3,4,5,6,7,8,9,10,11,12,24,36这些值，按量计费模式下该参数传1。
+        :param _Period: 购买时长，单位：月。
+<li>预付费：支持1,2,3,4,5,6,7,8,9,10,11,12,24,36
+<li>后付费：只支持1
         :type Period: int
-        :param _MasterDBInstanceId: 只读实例的主实例ID
-        :type MasterDBInstanceId: str
-        :param _Zone: 可用区ID。该参数可以通过调用 DescribeZones 接口的返回值中的Zone字段来获取。
-        :type Zone: str
-        :param _ProjectId: 项目ID。
-        :type ProjectId: int
-        :param _DBVersion: 【废弃】不再需要指定，内核版本号与主实例保持一致
-        :type DBVersion: str
-        :param _InstanceChargeType: 实例计费类型。目前支持：PREPAID（预付费，即包年包月），POSTPAID_BY_HOUR（后付费，即按量计费）。默认值：PREPAID。如果主实例为后付费，只读实例必须也为后付费。
+        :param _VpcId: 私有网络ID，形如vpc-xxxxxxxx。有效的VpcId可通过登录控制台查询；也可以调用接口 [DescribeVpcEx](https://cloud.tencent.com/document/api/215/1372) ，从接口返回中的unVpcId字段获取。
+        :type VpcId: str
+        :param _SubnetId: 私有网络子网ID，形如subnet-xxxxxxxx。有效的私有网络子网ID可通过登录控制台查询；也可以调用接口 [DescribeSubnets ](https://cloud.tencent.com/document/api/215/15784)，从接口返回中的unSubnetId字段获取。
+        :type SubnetId: str
+        :param _InstanceChargeType: 实例计费类型，目前支持：
+<li>PREPAID：预付费，即包年包月。
+<li>POSTPAID_BY_HOUR：后付费，即按量计费。
+默认值：PREPAID。如果主实例为后付费，只读实例必须也为后付费。
         :type InstanceChargeType: str
-        :param _AutoVoucher: 是否自动使用代金券。1（是），0（否），默认不使用。
+        :param _AutoVoucher: 是否自动使用代金券：
+<li>0：否
+<li>1：是
+默认值：0
         :type AutoVoucher: int
         :param _VoucherIds: 代金券ID列表，目前仅支持指定一张代金券。
         :type VoucherIds: list of str
-        :param _AutoRenewFlag: 续费标记：0-正常续费（默认）；1-自动续费；
+        :param _AutoRenewFlag: 续费标记：
+<li>0：手动续费
+<li>1：自动续费
+默认值：0
         :type AutoRenewFlag: int
-        :param _VpcId: 私有网络ID。
-        :type VpcId: str
-        :param _SubnetId: 私有网络子网ID。
-        :type SubnetId: str
+        :param _ProjectId: 项目ID。
+        :type ProjectId: int
         :param _ActivityId: 优惠活动ID
         :type ActivityId: int
-        :param _Name: 实例名(后续支持)
-        :type Name: str
-        :param _NeedSupportIpv6: 是否需要支持Ipv6，1：是，0：否
-        :type NeedSupportIpv6: int
         :param _ReadOnlyGroupId: 只读组ID。
         :type ReadOnlyGroupId: str
-        :param _TagList: 实例需要绑定的Tag信息，默认为空（该类型为Tag数组类型）
+        :param _TagList: 实例需要绑定的Tag信息，默认为空；可以通过调用 [DescribeTags](https://cloud.tencent.com/document/api/651/35316) 返回值中的 Tags 字段来获取。
         :type TagList: :class:`tencentcloud.postgres.v20170312.models.Tag`
-        :param _SecurityGroupIds: 安全组id
+        :param _SecurityGroupIds: 实例所属安全组，该参数可以通过调用 [DescribeSecurityGroups](https://cloud.tencent.com/document/api/215/15808) 的返回值中的sgId字段来获取。若不指定该参数，则绑定默认安全组。
+
         :type SecurityGroupIds: list of str
+        :param _NeedSupportIpv6: 是否需要支持Ipv6：
+<li>0：否
+<li>1：是
+默认值：0
+        :type NeedSupportIpv6: int
+        :param _Name: 实例名(后续支持)
+        :type Name: str
+        :param _DBVersion: 【废弃】不再需要指定，内核版本号与主实例保持一致
+        :type DBVersion: str
         """
+        self._Zone = None
+        self._MasterDBInstanceId = None
         self._SpecCode = None
         self._Storage = None
         self._InstanceCount = None
         self._Period = None
-        self._MasterDBInstanceId = None
-        self._Zone = None
-        self._ProjectId = None
-        self._DBVersion = None
+        self._VpcId = None
+        self._SubnetId = None
         self._InstanceChargeType = None
         self._AutoVoucher = None
         self._VoucherIds = None
         self._AutoRenewFlag = None
-        self._VpcId = None
-        self._SubnetId = None
+        self._ProjectId = None
         self._ActivityId = None
-        self._Name = None
-        self._NeedSupportIpv6 = None
         self._ReadOnlyGroupId = None
         self._TagList = None
         self._SecurityGroupIds = None
+        self._NeedSupportIpv6 = None
+        self._Name = None
+        self._DBVersion = None
+
+    @property
+    def Zone(self):
+        return self._Zone
+
+    @Zone.setter
+    def Zone(self, Zone):
+        self._Zone = Zone
+
+    @property
+    def MasterDBInstanceId(self):
+        return self._MasterDBInstanceId
+
+    @MasterDBInstanceId.setter
+    def MasterDBInstanceId(self, MasterDBInstanceId):
+        self._MasterDBInstanceId = MasterDBInstanceId
 
     @property
     def SpecCode(self):
         return self._SpecCode
 
     @SpecCode.setter
     def SpecCode(self, SpecCode):
@@ -2603,44 +2635,28 @@
         return self._Period
 
     @Period.setter
     def Period(self, Period):
         self._Period = Period
 
     @property
-    def MasterDBInstanceId(self):
-        return self._MasterDBInstanceId
-
-    @MasterDBInstanceId.setter
-    def MasterDBInstanceId(self, MasterDBInstanceId):
-        self._MasterDBInstanceId = MasterDBInstanceId
-
-    @property
-    def Zone(self):
-        return self._Zone
-
-    @Zone.setter
-    def Zone(self, Zone):
-        self._Zone = Zone
-
-    @property
-    def ProjectId(self):
-        return self._ProjectId
+    def VpcId(self):
+        return self._VpcId
 
-    @ProjectId.setter
-    def ProjectId(self, ProjectId):
-        self._ProjectId = ProjectId
+    @VpcId.setter
+    def VpcId(self, VpcId):
+        self._VpcId = VpcId
 
     @property
-    def DBVersion(self):
-        return self._DBVersion
+    def SubnetId(self):
+        return self._SubnetId
 
-    @DBVersion.setter
-    def DBVersion(self, DBVersion):
-        self._DBVersion = DBVersion
+    @SubnetId.setter
+    def SubnetId(self, SubnetId):
+        self._SubnetId = SubnetId
 
     @property
     def InstanceChargeType(self):
         return self._InstanceChargeType
 
     @InstanceChargeType.setter
     def InstanceChargeType(self, InstanceChargeType):
@@ -2667,54 +2683,30 @@
         return self._AutoRenewFlag
 
     @AutoRenewFlag.setter
     def AutoRenewFlag(self, AutoRenewFlag):
         self._AutoRenewFlag = AutoRenewFlag
 
     @property
-    def VpcId(self):
-        return self._VpcId
-
-    @VpcId.setter
-    def VpcId(self, VpcId):
-        self._VpcId = VpcId
-
-    @property
-    def SubnetId(self):
-        return self._SubnetId
+    def ProjectId(self):
+        return self._ProjectId
 
-    @SubnetId.setter
-    def SubnetId(self, SubnetId):
-        self._SubnetId = SubnetId
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
 
     @property
     def ActivityId(self):
         return self._ActivityId
 
     @ActivityId.setter
     def ActivityId(self, ActivityId):
         self._ActivityId = ActivityId
 
     @property
-    def Name(self):
-        return self._Name
-
-    @Name.setter
-    def Name(self, Name):
-        self._Name = Name
-
-    @property
-    def NeedSupportIpv6(self):
-        return self._NeedSupportIpv6
-
-    @NeedSupportIpv6.setter
-    def NeedSupportIpv6(self, NeedSupportIpv6):
-        self._NeedSupportIpv6 = NeedSupportIpv6
-
-    @property
     def ReadOnlyGroupId(self):
         return self._ReadOnlyGroupId
 
     @ReadOnlyGroupId.setter
     def ReadOnlyGroupId(self, ReadOnlyGroupId):
         self._ReadOnlyGroupId = ReadOnlyGroupId
 
@@ -2730,38 +2722,62 @@
     def SecurityGroupIds(self):
         return self._SecurityGroupIds
 
     @SecurityGroupIds.setter
     def SecurityGroupIds(self, SecurityGroupIds):
         self._SecurityGroupIds = SecurityGroupIds
 
+    @property
+    def NeedSupportIpv6(self):
+        return self._NeedSupportIpv6
+
+    @NeedSupportIpv6.setter
+    def NeedSupportIpv6(self, NeedSupportIpv6):
+        self._NeedSupportIpv6 = NeedSupportIpv6
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def DBVersion(self):
+        return self._DBVersion
+
+    @DBVersion.setter
+    def DBVersion(self, DBVersion):
+        self._DBVersion = DBVersion
+
 
     def _deserialize(self, params):
+        self._Zone = params.get("Zone")
+        self._MasterDBInstanceId = params.get("MasterDBInstanceId")
         self._SpecCode = params.get("SpecCode")
         self._Storage = params.get("Storage")
         self._InstanceCount = params.get("InstanceCount")
         self._Period = params.get("Period")
-        self._MasterDBInstanceId = params.get("MasterDBInstanceId")
-        self._Zone = params.get("Zone")
-        self._ProjectId = params.get("ProjectId")
-        self._DBVersion = params.get("DBVersion")
+        self._VpcId = params.get("VpcId")
+        self._SubnetId = params.get("SubnetId")
         self._InstanceChargeType = params.get("InstanceChargeType")
         self._AutoVoucher = params.get("AutoVoucher")
         self._VoucherIds = params.get("VoucherIds")
         self._AutoRenewFlag = params.get("AutoRenewFlag")
-        self._VpcId = params.get("VpcId")
-        self._SubnetId = params.get("SubnetId")
+        self._ProjectId = params.get("ProjectId")
         self._ActivityId = params.get("ActivityId")
-        self._Name = params.get("Name")
-        self._NeedSupportIpv6 = params.get("NeedSupportIpv6")
         self._ReadOnlyGroupId = params.get("ReadOnlyGroupId")
         if params.get("TagList") is not None:
             self._TagList = Tag()
             self._TagList._deserialize(params.get("TagList"))
         self._SecurityGroupIds = params.get("SecurityGroupIds")
+        self._NeedSupportIpv6 = params.get("NeedSupportIpv6")
+        self._Name = params.get("Name")
+        self._DBVersion = params.get("DBVersion")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.943/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.944/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.944/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.943/README.rst` & `tencentcloud-sdk-python-postgres-3.0.944/README.rst`

 * *Files identical despite different names*

