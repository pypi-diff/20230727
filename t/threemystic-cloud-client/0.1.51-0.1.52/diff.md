# Comparing `tmp/threemystic_cloud_client-0.1.51.tar.gz` & `tmp/threemystic_cloud_client-0.1.52.tar.gz`

## Comparing `threemystic_cloud_client-0.1.51.tar` & `threemystic_cloud_client-0.1.52.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cli/actions/action_generate/__init__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cli/actions/action_test/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cli/actions/action_token/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
--rw-r--r--   0        0        0    35170 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12277 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
--rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/LICENSE
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/hatch.toml
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/pyproject.toml
--rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.51/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cli/actions/action_generate/__init__.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cli/actions/action_test/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cli/actions/action_token/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
+-rw-r--r--   0        0        0    35174 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12277 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
+-rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/LICENSE
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/hatch.toml
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/pyproject.toml
+-rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.52/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cli/actions/action_generate/__init__.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cli/actions/action_generate/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cli/actions/action_test/__init__.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cli/actions/action_test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cli/actions/action_token/__init__.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cli/actions/action_token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/base_class/base.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -741,16 +741,16 @@
         role = None,
         region = region
       )
       
     if resource_groups is None or (resource_groups is not None and len(resource_groups)<1):
       resource_groups = self.get_resource_groups(account=account, region= region,filters=filters_rg, rg_client= rg_client)
 
-    if resource_groups is None or (resource_groups is not None and len(resource_groups)<1):
-      return {}
+      if resource_groups is None or (resource_groups is not None and len(resource_groups)<1):
+        return {}
 
     resources = {} 
     boto_params = {}
     if len(filters_resource) > 0:
       boto_params["Filters"] = filters_resource
     
     boto_nextkey = "NextToken"
```

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.52/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/.gitignore` & `threemystic_cloud_client-0.1.52/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/LICENSE` & `threemystic_cloud_client-0.1.52/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/README.md` & `threemystic_cloud_client-0.1.52/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/hatch.toml` & `threemystic_cloud_client-0.1.52/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/pyproject.toml` & `threemystic_cloud_client-0.1.52/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.51/PKG-INFO` & `threemystic_cloud_client-0.1.52/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.51
+Version: 0.1.52
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

