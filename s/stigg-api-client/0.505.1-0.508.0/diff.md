# Comparing `tmp/stigg_api_client-0.505.1.tar.gz` & `tmp/stigg_api_client-0.508.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.505.1.tar", max compression
+gzip compressed data, was "stigg_api_client-0.508.0.tar", max compression
```

## Comparing `stigg_api_client-0.505.1.tar` & `stigg_api_client-0.508.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-07-25 16:15:50.595696 stigg_api_client-0.505.1/README.md
--rw-r--r--   0        0        0      460 2023-07-25 16:16:40.304018 stigg_api_client-0.505.1/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-25 16:15:50.595696 stigg_api_client-0.505.1/stigg/__init__.py
--rw-r--r--   0        0        0     1141 2023-07-25 16:15:50.595696 stigg_api_client-0.505.1/stigg/client.py
--rw-r--r--   0        0        0        0 2023-07-25 16:16:37.868003 stigg_api_client-0.505.1/stigg/generated/__init__.py
--rw-r--r--   0        0        0    49504 2023-07-25 16:16:38.388006 stigg_api_client-0.505.1/stigg/generated/operations.py
--rw-r--r--   0        0        0   465924 2023-07-25 16:16:38.176005 stigg_api_client-0.505.1/stigg/generated/schema.py
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 stigg_api_client-0.505.1/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-07-27 06:55:18.149724 stigg_api_client-0.508.0/README.md
+-rw-r--r--   0        0        0      460 2023-07-27 06:55:55.610226 stigg_api_client-0.508.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-27 06:55:18.149724 stigg_api_client-0.508.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1141 2023-07-27 06:55:18.149724 stigg_api_client-0.508.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-07-27 06:55:53.538200 stigg_api_client-0.508.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    51059 2023-07-27 06:55:54.010206 stigg_api_client-0.508.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   467048 2023-07-27 06:55:53.842204 stigg_api_client-0.508.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 stigg_api_client-0.508.0/PKG-INFO
```

### Comparing `stigg_api_client-0.505.1/README.md` & `stigg_api_client-0.508.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.505.1/stigg/client.py` & `stigg_api_client-0.508.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.505.1/stigg/generated/operations.py` & `stigg_api_client-0.508.0/stigg/generated/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,36 @@
     _frag_schedule_variables__as__BillingPeriodChangeVariables.billing_period()
     _frag_schedule_variables__as__UnitAmountChangeVariables = _frag_schedule_variables.__as__(_schema.UnitAmountChangeVariables)
     _frag_schedule_variables__as__UnitAmountChangeVariables.new_unit_amount()
     _frag_schedule_variables__as__UnitAmountChangeVariables.feature_id()
     return _frag
 
 
+def fragment_subscription_future_update_data():
+    _frag = sgqlc.operation.Fragment(_schema.SubscriptionFutureUpdate, 'SubscriptionFutureUpdateData')
+    _frag.subscription_schedule_type()
+    _frag.schedule_status()
+    _frag.scheduled_execution_time()
+    _frag_target_package = _frag.target_package()
+    _frag_target_package.id()
+    _frag_target_package.ref_id()
+    _frag_target_package.display_name()
+    _frag_schedule_variables = _frag.schedule_variables()
+    _frag_schedule_variables__as__DowngradeChangeVariables = _frag_schedule_variables.__as__(_schema.DowngradeChangeVariables)
+    _frag_schedule_variables__as__DowngradeChangeVariables.addon_ref_ids()
+    _frag_schedule_variables__as__DowngradeChangeVariables.billing_period()
+    _frag_schedule_variables__as__DowngradeChangeVariables.downgrade_plan_ref_id()
+    _frag_schedule_variables__as__BillingPeriodChangeVariables = _frag_schedule_variables.__as__(_schema.BillingPeriodChangeVariables)
+    _frag_schedule_variables__as__BillingPeriodChangeVariables.billing_period()
+    _frag_schedule_variables__as__UnitAmountChangeVariables = _frag_schedule_variables.__as__(_schema.UnitAmountChangeVariables)
+    _frag_schedule_variables__as__UnitAmountChangeVariables.new_unit_amount()
+    _frag_schedule_variables__as__UnitAmountChangeVariables.feature_id()
+    return _frag
+
+
 def fragment_subscription_fragment():
     _frag = sgqlc.operation.Fragment(_schema.CustomerSubscription, 'SubscriptionFragment')
     _frag.id()
     _frag.start_date()
     _frag.end_date()
     _frag.trial_end_date()
     _frag.cancellation_date()
@@ -227,14 +249,16 @@
     _frag_addons = _frag.addons()
     _frag_addons.id()
     _frag_addons.quantity()
     _frag_addons_addon = _frag_addons.addon()
     _frag_addons_addon.__fragment__(fragment_addon_fragment())
     _frag_scheduled_updates = _frag.scheduled_updates()
     _frag_scheduled_updates.__fragment__(fragment_subscription_scheduled_update_data())
+    _frag_future_updates = _frag.future_updates()
+    _frag_future_updates.__fragment__(fragment_subscription_future_update_data())
     return _frag
 
 
 def fragment_promotional_entitlement_fragment():
     _frag = sgqlc.operation.Fragment(_schema.PromotionalEntitlement, 'PromotionalEntitlementFragment')
     _frag.status()
     _frag.usage_limit()
@@ -892,14 +916,15 @@
     price_fragment = fragment_price_fragment()
     product_fragment = fragment_product_fragment()
     promotional_entitlement_fragment = fragment_promotional_entitlement_fragment()
     reset_period_configuration_fragment = fragment_reset_period_configuration_fragment()
     slim_customer_fragment = fragment_slim_customer_fragment()
     slim_subscription_fragment = fragment_slim_subscription_fragment()
     subscription_fragment = fragment_subscription_fragment()
+    subscription_future_update_data = fragment_subscription_future_update_data()
     subscription_preview_fragment = fragment_subscription_preview_fragment()
     subscription_scheduled_update_data = fragment_subscription_scheduled_update_data()
     total_price_fragment = fragment_total_price_fragment()
     typography_configuration_fragment = fragment_typography_configuration_fragment()
     usage_history_fragment = fragment_usage_history_fragment()
     usage_updated_fragment = fragment_usage_updated_fragment()
```

### Comparing `stigg_api_client-0.505.1/stigg/generated/schema.py` & `stigg_api_client-0.508.0/stigg/generated/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -4076,15 +4076,15 @@
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
 
 
 class CustomerSubscription(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'addons', 'billing_id', 'billing_link_url', 'cancel_reason', 'cancellation_date', 'coupon', 'created_at', 'crm_id', 'crm_link_url', 'current_billing_period_end', 'customer', 'effective_end_date', 'end_date', 'environment', 'environment_id', 'experiment', 'experiment_info', 'id', 'is_custom_price_subscription', 'old_billing_id', 'outdated_price_packages', 'plan', 'prices', 'pricing_type', 'ref_id', 'resource', 'resource_id', 'scheduled_updates', 'start_date', 'status', 'subscription_entitlements', 'subscription_id', 'sync_states', 'total_price', 'trial_end_date', 'was_in_trial')
+    __field_names__ = ('additional_meta_data', 'addons', 'billing_id', 'billing_link_url', 'cancel_reason', 'cancellation_date', 'coupon', 'created_at', 'crm_id', 'crm_link_url', 'current_billing_period_end', 'customer', 'effective_end_date', 'end_date', 'environment', 'environment_id', 'experiment', 'experiment_info', 'future_updates', 'id', 'is_custom_price_subscription', 'old_billing_id', 'outdated_price_packages', 'plan', 'prices', 'pricing_type', 'ref_id', 'resource', 'resource_id', 'scheduled_updates', 'start_date', 'status', 'subscription_entitlements', 'subscription_id', 'sync_states', 'total_price', 'trial_end_date', 'was_in_trial')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddon')), graphql_name='addons', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(SubscriptionAddonFilter, graphql_name='filter', default={})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(SubscriptionAddonSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
 ))
     )
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
@@ -4099,14 +4099,15 @@
     customer = sgqlc.types.Field(sgqlc.types.non_null(Customer), graphql_name='customer')
     effective_end_date = sgqlc.types.Field(DateTime, graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field(DateTime, graphql_name='endDate')
     environment = sgqlc.types.Field(sgqlc.types.non_null('Environment'), graphql_name='environment')
     environment_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='environmentId')
     experiment = sgqlc.types.Field('Experiment', graphql_name='experiment')
     experiment_info = sgqlc.types.Field('experimentInfo', graphql_name='experimentInfo')
+    future_updates = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionFutureUpdate'))), graphql_name='futureUpdates')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     is_custom_price_subscription = sgqlc.types.Field(Boolean, graphql_name='isCustomPriceSubscription')
     old_billing_id = sgqlc.types.Field(String, graphql_name='oldBillingId')
     outdated_price_packages = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='outdatedPricePackages')
     plan = sgqlc.types.Field(sgqlc.types.non_null('Plan'), graphql_name='plan')
     prices = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionPrice')), graphql_name='prices', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(SubscriptionPriceFilter, graphql_name='filter', default={})),
@@ -6970,14 +6971,26 @@
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     id = sgqlc.types.Field(String, graphql_name='id')
     subscription_id = sgqlc.types.Field(String, graphql_name='subscriptionId')
     updated_at = sgqlc.types.Field(DateTime, graphql_name='updatedAt')
 
 
+class SubscriptionFutureUpdate(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('billing_id', 'created_at', 'schedule_status', 'schedule_variables', 'scheduled_execution_time', 'subscription_schedule_type', 'target_package')
+    billing_id = sgqlc.types.Field(String, graphql_name='billingId')
+    created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
+    schedule_status = sgqlc.types.Field(sgqlc.types.non_null(SubscriptionScheduleStatus), graphql_name='scheduleStatus')
+    schedule_variables = sgqlc.types.Field('ScheduleVariables', graphql_name='scheduleVariables')
+    scheduled_execution_time = sgqlc.types.Field(sgqlc.types.non_null(DateTime), graphql_name='scheduledExecutionTime')
+    subscription_schedule_type = sgqlc.types.Field(sgqlc.types.non_null(SubscriptionScheduleType), graphql_name='subscriptionScheduleType')
+    target_package = sgqlc.types.Field(PackageDTO, graphql_name='targetPackage')
+
+
 class SubscriptionMigrationTask(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('affected_customers_count', 'created_at', 'end_date', 'environment_id', 'id', 'initiated_package_id', 'packages', 'progress', 'start_date', 'status', 'task_type')
     affected_customers_count = sgqlc.types.Field(Int, graphql_name='affectedCustomersCount')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     end_date = sgqlc.types.Field(DateTime, graphql_name='endDate')
     environment_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='environmentId')
```

### Comparing `stigg_api_client-0.505.1/PKG-INFO` & `stigg_api_client-0.508.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.505.1
+Version: 0.508.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

