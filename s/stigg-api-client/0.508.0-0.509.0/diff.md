# Comparing `tmp/stigg_api_client-0.508.0.tar.gz` & `tmp/stigg_api_client-0.509.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.508.0.tar", max compression
+gzip compressed data, was "stigg_api_client-0.509.0.tar", max compression
```

## Comparing `stigg_api_client-0.508.0.tar` & `stigg_api_client-0.509.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-07-27 06:55:18.149724 stigg_api_client-0.508.0/README.md
--rw-r--r--   0        0        0      460 2023-07-27 06:55:55.610226 stigg_api_client-0.508.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-27 06:55:18.149724 stigg_api_client-0.508.0/stigg/__init__.py
--rw-r--r--   0        0        0     1141 2023-07-27 06:55:18.149724 stigg_api_client-0.508.0/stigg/client.py
--rw-r--r--   0        0        0        0 2023-07-27 06:55:53.538200 stigg_api_client-0.508.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0    51059 2023-07-27 06:55:54.010206 stigg_api_client-0.508.0/stigg/generated/operations.py
--rw-r--r--   0        0        0   467048 2023-07-27 06:55:53.842204 stigg_api_client-0.508.0/stigg/generated/schema.py
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 stigg_api_client-0.508.0/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-07-27 07:09:22.270223 stigg_api_client-0.509.0/README.md
+-rw-r--r--   0        0        0      460 2023-07-27 07:09:55.634335 stigg_api_client-0.509.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-27 07:09:22.270223 stigg_api_client-0.509.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1141 2023-07-27 07:09:22.270223 stigg_api_client-0.509.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-07-27 07:09:53.722333 stigg_api_client-0.509.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    51059 2023-07-27 07:09:54.142334 stigg_api_client-0.509.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   467141 2023-07-27 07:09:53.986334 stigg_api_client-0.509.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 stigg_api_client-0.509.0/PKG-INFO
```

### Comparing `stigg_api_client-0.508.0/README.md` & `stigg_api_client-0.509.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.508.0/stigg/client.py` & `stigg_api_client-0.509.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.508.0/stigg/generated/operations.py` & `stigg_api_client-0.509.0/stigg/generated/operations.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.508.0/stigg/generated/schema.py` & `stigg_api_client-0.509.0/stigg/generated/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -2697,15 +2697,16 @@
     direction = sgqlc.types.Field(sgqlc.types.non_null(SortDirection), graphql_name='direction')
     field = sgqlc.types.Field(sgqlc.types.non_null(SubscriptionAddonSortFields), graphql_name='field')
     nulls = sgqlc.types.Field(SortNulls, graphql_name='nulls')
 
 
 class SubscriptionBillingInfo(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('tax_rate_ids',)
+    __field_names__ = ('tax_percentage', 'tax_rate_ids')
+    tax_percentage = sgqlc.types.Field(Float, graphql_name='taxPercentage')
     tax_rate_ids = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='taxRateIds')
 
 
 class SubscriptionCancelReasonFilterComparison(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('eq', 'gt', 'gte', 'i_like', 'in_', 'is_', 'is_not', 'like', 'lt', 'lte', 'neq', 'not_ilike', 'not_in', 'not_like')
     eq = sgqlc.types.Field(SubscriptionCancelReason, graphql_name='eq')
```

### Comparing `stigg_api_client-0.508.0/PKG-INFO` & `stigg_api_client-0.509.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.508.0
+Version: 0.509.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

