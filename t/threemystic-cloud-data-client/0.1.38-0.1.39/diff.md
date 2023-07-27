# Comparing `tmp/threemystic_cloud_data_client-0.1.38.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.39.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.38.tar` & `threemystic_cloud_data_client-0.1.39.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py
--rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
--rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
--rw-r--r--   0        0        0    10075 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    13572 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/hatch.toml
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/pyproject.toml
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.38/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py
+-rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
+-rw-r--r--   0        0        0    11187 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py
+-rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    13572 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/hatch.toml
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/pyproject.toml
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.39/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     }
   ]
     
   
   async def __redshift(self, client, *args, **kwargs):
 
     return self.get_cloud_client().general_boto_call_array(
-      boto_call=lambda item: client.list_hosted_zones(**item),
+      boto_call=lambda item: client.describe_clusters(**item),
       boto_params={},
       boto_nextkey = "Marker",
       boto_key="Clusters"
     )
     
   
   async def _process_account_data_region(self, account, region, resource_groups, loop, *args, **kwargs):
```

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,18 @@
       data_action="dns",
       logger_name= "cloud_data_client_aws_client_action_dns",
       *args, **kwargs)
     
     
     self.data_id_name = "Id"
     
-    self.arn_lambda = (lambda item: item["extra_id"])
+    self.arn_lambda = (lambda item: self.get_cloud_client().get_resource_general_arn(
+      resource_type= "route53",
+      resource_type_sub= "hostedzone", **item # {region, account_id, resource_id}
+    ))
     
     self.auto_region_resourcebytype= ["Amazon MemoryDB"]
     self.resource_group_filter = [
     {
       'Name': 'resource-type',
       'Values': [
         'AWS::Route53::HostedZone',
```

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,17 +6,20 @@
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="memorydb",
       logger_name= "cloud_data_client_aws_client_action_memorydb",
       *args, **kwargs)
     
     
-    self.data_id_name = "ARN"
+    self.data_id_name = "Name"
     
-    self.arn_lambda = (lambda item: item["extra_id"])
+    self.arn_lambda = (lambda item: self.get_cloud_client().get_resource_general_arn(
+      resource_type= "memorydb",
+      resource_type_sub= "cluster", **item # {region, account_id, resource_id}
+    ))
     
     self.auto_region_resourcebytype= ["Amazon MemoryDB"]
     self.resource_group_filter = [
     {
       'Name': 'resource-type',
       'Values': [
         'AWS::MemoryDB::Cluster',
```

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
       data_action="vmss",
       logger_name= "cloud_data_client_aws_client_action_vmss",
       *args, **kwargs)
     
     
     self.data_id_name = "AutoScalingGroupARN"
     
-    self.arn_lambda = (lambda item: item["extra_id"])
+    self.arn_lambda = (lambda item: item[self.data_id_name])
     
     self.auto_region_resourcebytype= ["Amazon Elastic Compute Cloud - Compute"]
     self.resource_group_filter = [
     {
       'Name': 'resource-type',
       'Values': [
         'AWS::EC2::Instance',
```

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
       )
       return {}
   
   async def __process_get_resources_public_record_sets(self, client, account, dns, *args, **kwargs):    
     try:      
       return [ record_set for record_set in self.get_cloud_client().sdk_request(
           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
-          lambda_sdk_command=lambda: client.record_sets.list_all_by_dns_zone(resource_group_name= self.get_cloud_client().get_resource_group_from_resource(resource= dns), private_zone_name= dns.name)
+          lambda_sdk_command=lambda: client.record_sets.list_all_by_dns_zone(resource_group_name= self.get_cloud_client().get_resource_group_from_resource(resource= dns), zone_name= dns.name)
         )
       ]
            
     except Exception as err:
       self.get_common().get_logger().exception(
         msg= f"__process_get_resources_public_record_sets: {err}",
         extra={
```

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/base_class/base.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py` & `threemystic_cloud_data_client-0.1.39/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/.gitignore` & `threemystic_cloud_data_client-0.1.39/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/LICENSE` & `threemystic_cloud_data_client-0.1.39/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/README.md` & `threemystic_cloud_data_client-0.1.39/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/hatch.toml` & `threemystic_cloud_data_client-0.1.39/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/pyproject.toml` & `threemystic_cloud_data_client-0.1.39/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.38/PKG-INFO` & `threemystic_cloud_data_client-0.1.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.38
+Version: 0.1.39
 Summary: A tool for collecting data from various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_data_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_data_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

