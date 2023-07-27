# Comparing `tmp/stigg_api_client_v2-0.508.0.tar.gz` & `tmp/stigg_api_client_v2-0.509.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.508.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.509.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.508.0.tar` & `stigg_api_client_v2-0.509.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1644 2023-07-27 06:55:16.615405 stigg_api_client_v2-0.508.0/README.md
--rw-r--r--   0        0        0      432 2023-07-27 06:55:59.919640 stigg_api_client_v2-0.508.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-27 06:55:16.615405 stigg_api_client_v2-0.508.0/stigg/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-27 06:55:16.615405 stigg_api_client_v2-0.508.0/stigg/client.py
--rw-r--r--   0        0        0    40986 2023-07-27 06:55:58.359635 stigg_api_client_v2-0.508.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0      460 2023-07-27 06:55:57.103630 stigg_api_client_v2-0.508.0/stigg/generated/archive_customer.py
--rw-r--r--   0        0        0     7303 2023-07-27 06:55:57.911633 stigg_api_client_v2-0.508.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    70891 2023-07-27 06:55:58.123634 stigg_api_client_v2-0.508.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-07-27 06:55:53.259616 stigg_api_client_v2-0.508.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-07-27 06:55:57.911633 stigg_api_client_v2-0.508.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-07-27 06:55:57.047630 stigg_api_client_v2-0.508.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-07-27 06:55:57.067630 stigg_api_client_v2-0.508.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    70464 2023-07-27 06:55:53.467617 stigg_api_client_v2-0.508.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-07-27 06:55:57.091630 stigg_api_client_v2-0.508.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    24198 2023-07-27 06:55:54.927622 stigg_api_client_v2-0.508.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-07-27 06:55:57.055630 stigg_api_client_v2-0.508.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-07-27 06:55:57.063630 stigg_api_client_v2-0.508.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-07-27 06:55:57.911633 stigg_api_client_v2-0.508.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    58974 2023-07-27 06:55:57.907633 stigg_api_client_v2-0.508.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-07-27 06:55:57.115630 stigg_api_client_v2-0.508.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-07-27 06:55:57.123630 stigg_api_client_v2-0.508.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-07-27 06:55:57.107630 stigg_api_client_v2-0.508.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-07-27 06:55:57.159630 stigg_api_client_v2-0.508.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-07-27 06:55:57.139630 stigg_api_client_v2-0.508.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-07-27 06:55:57.135630 stigg_api_client_v2-0.508.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-07-27 06:55:57.171630 stigg_api_client_v2-0.508.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-07-27 06:55:57.127630 stigg_api_client_v2-0.508.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-07-27 06:55:57.147630 stigg_api_client_v2-0.508.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-07-27 06:55:57.155630 stigg_api_client_v2-0.508.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-07-27 06:55:57.015630 stigg_api_client_v2-0.508.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-07-27 06:55:57.011630 stigg_api_client_v2-0.508.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-07-27 06:55:57.035630 stigg_api_client_v2-0.508.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   127090 2023-07-27 06:55:56.995630 stigg_api_client_v2-0.508.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-07-27 06:55:57.095630 stigg_api_client_v2-0.508.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-07-27 06:55:57.007630 stigg_api_client_v2-0.508.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-07-27 06:55:57.031630 stigg_api_client_v2-0.508.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-07-27 06:55:57.083630 stigg_api_client_v2-0.508.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-07-27 06:55:57.079630 stigg_api_client_v2-0.508.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-07-27 06:55:57.075630 stigg_api_client_v2-0.508.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-07-27 06:55:57.915633 stigg_api_client_v2-0.508.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-07-27 06:55:57.023630 stigg_api_client_v2-0.508.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-07-27 06:55:57.043630 stigg_api_client_v2-0.508.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-07-27 06:55:57.175630 stigg_api_client_v2-0.508.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.508.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-07-27 07:09:23.418953 stigg_api_client_v2-0.509.0/README.md
+-rw-r--r--   0        0        0      432 2023-07-27 07:10:09.840458 stigg_api_client_v2-0.509.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-27 07:09:23.422953 stigg_api_client_v2-0.509.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-27 07:09:23.422953 stigg_api_client_v2-0.509.0/stigg/client.py
+-rw-r--r--   0        0        0    40986 2023-07-27 07:10:08.112402 stigg_api_client_v2-0.509.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-27 07:10:06.612354 stigg_api_client_v2-0.509.0/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0     7303 2023-07-27 07:10:07.584385 stigg_api_client_v2-0.509.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    70891 2023-07-27 07:10:07.808393 stigg_api_client_v2-0.509.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-07-27 07:10:02.136212 stigg_api_client_v2-0.509.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-07-27 07:10:07.584385 stigg_api_client_v2-0.509.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-07-27 07:10:06.556352 stigg_api_client_v2-0.509.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-07-27 07:10:06.576353 stigg_api_client_v2-0.509.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    70464 2023-07-27 07:10:02.360219 stigg_api_client_v2-0.509.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-07-27 07:10:06.600354 stigg_api_client_v2-0.509.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24198 2023-07-27 07:10:04.056272 stigg_api_client_v2-0.509.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-07-27 07:10:06.564353 stigg_api_client_v2-0.509.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-07-27 07:10:06.568353 stigg_api_client_v2-0.509.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-07-27 07:10:07.584385 stigg_api_client_v2-0.509.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    58974 2023-07-27 07:10:07.572385 stigg_api_client_v2-0.509.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-07-27 07:10:06.624354 stigg_api_client_v2-0.509.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-07-27 07:10:06.632355 stigg_api_client_v2-0.509.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-07-27 07:10:06.620354 stigg_api_client_v2-0.509.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-07-27 07:10:06.672356 stigg_api_client_v2-0.509.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-07-27 07:10:06.648355 stigg_api_client_v2-0.509.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-07-27 07:10:06.644355 stigg_api_client_v2-0.509.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-07-27 07:10:06.684357 stigg_api_client_v2-0.509.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-07-27 07:10:06.640355 stigg_api_client_v2-0.509.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-07-27 07:10:06.656355 stigg_api_client_v2-0.509.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-07-27 07:10:06.668356 stigg_api_client_v2-0.509.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-07-27 07:10:06.524351 stigg_api_client_v2-0.509.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-07-27 07:10:06.516351 stigg_api_client_v2-0.509.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-07-27 07:10:06.544352 stigg_api_client_v2-0.509.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   127157 2023-07-27 07:10:06.500351 stigg_api_client_v2-0.509.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-07-27 07:10:06.604354 stigg_api_client_v2-0.509.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-07-27 07:10:06.512351 stigg_api_client_v2-0.509.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-07-27 07:10:06.540352 stigg_api_client_v2-0.509.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-07-27 07:10:06.592353 stigg_api_client_v2-0.509.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-07-27 07:10:06.588353 stigg_api_client_v2-0.509.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-07-27 07:10:06.584353 stigg_api_client_v2-0.509.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-07-27 07:10:07.588385 stigg_api_client_v2-0.509.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-07-27 07:10:06.528351 stigg_api_client_v2-0.509.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-07-27 07:10:06.548352 stigg_api_client_v2-0.509.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-07-27 07:10:06.688356 stigg_api_client_v2-0.509.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.509.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.508.0/README.md` & `stigg_api_client_v2-0.509.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.508.0/stigg/client.py` & `stigg_api_client_v2-0.509.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.509.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 
 from .archive_customer import ArchiveCustomer, ArchiveCustomerArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.509.0/stigg/generated/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/async_client.py` & `stigg_api_client_v2-0.509.0/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/base_client.py` & `stigg_api_client_v2-0.509.0/stigg/generated/base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.509.0/stigg/generated/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.509.0/stigg/generated/cancel_subscription.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/client.py` & `stigg_api_client_v2-0.509.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.509.0/stigg/generated/create_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.509.0/stigg/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerIsArchived = "CustomerIsArchived"
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.509.0/stigg/generated/estimate_subscription.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.509.0/stigg/generated/estimate_subscription_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.509.0/stigg/generated/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.509.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -125,25 +125,14 @@
     status: SyncStatus
 
 
 class CouponFragmentCustomers(BaseModel):
     id: str
 
 
-class SlimCustomerFragment(BaseModel):
-    id: str
-    name: Optional[str]
-    email: Optional[str]
-    created_at: Optional[Any] = Field(alias="createdAt")
-    updated_at: Any = Field(alias="updatedAt")
-    ref_id: str = Field(alias="refId")
-    billing_id: Optional[str] = Field(alias="billingId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class PromotionalEntitlementFragment(BaseModel):
     status: PromotionalEntitlementStatus
     usage_limit: Optional[float] = Field(alias="usageLimit")
     feature_id: str = Field(alias="featureId")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -158,14 +147,25 @@
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     ref_id: str = Field(alias="refId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
 
 
+class SlimCustomerFragment(BaseModel):
+    id: str
+    name: Optional[str]
+    email: Optional[str]
+    created_at: Optional[Any] = Field(alias="createdAt")
+    updated_at: Any = Field(alias="updatedAt")
+    ref_id: str = Field(alias="refId")
+    billing_id: Optional[str] = Field(alias="billingId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class CustomerFragment(SlimCustomerFragment):
     has_payment_method: bool = Field(alias="hasPaymentMethod")
     has_active_subscription: bool = Field(alias="hasActiveSubscription")
     default_payment_expiration_month: Optional[int] = Field(
         alias="defaultPaymentExpirationMonth"
     )
     default_payment_expiration_year: Optional[int] = Field(
@@ -329,41 +329,19 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
-class CustomerPortalPromotionalEntitlement(BaseModel):
-    display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
-
-
-class CustomerPortalSubscriptionPriceFragment(BaseModel):
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    billing_model: Optional[BillingModel] = Field(alias="billingModel")
-    price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
-    feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
-
-
-class CustomerPortalSubscriptionPriceFragmentPrice(BaseModel):
-    amount: float
-    currency: Currency
-
-
-class CustomerPortalSubscriptionPriceFragmentFeature(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
     display_name: str = Field(alias="displayName")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    quantity: int
 
 
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
@@ -410,19 +388,32 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
+class CustomerPortalSubscriptionPriceFragment(BaseModel):
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    billing_model: Optional[BillingModel] = Field(alias="billingModel")
+    price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
+    feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
+
+
+class CustomerPortalSubscriptionPriceFragmentPrice(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class CustomerPortalSubscriptionPriceFragmentFeature(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
-    quantity: int
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
 
 
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing_type: PricingType = Field(alias="pricingType")
     prices: List["CustomerPortalSubscriptionFragmentPrices"]
@@ -502,14 +493,23 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
+class CustomerPortalPromotionalEntitlement(BaseModel):
+    display_name: str = Field(alias="displayName")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
+
+
 class CustomerResourceFragment(BaseModel):
     resource_id: str = Field(alias="resourceId")
 
 
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
@@ -548,61 +548,14 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
-class SubscriptionFutureUpdateData(BaseModel):
-    subscription_schedule_type: SubscriptionScheduleType = Field(
-        alias="subscriptionScheduleType"
-    )
-    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
-    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
-    target_package: Optional["SubscriptionFutureUpdateDataTargetPackage"] = Field(
-        alias="targetPackage"
-    )
-    schedule_variables: Optional[
-        Annotated[
-            Union[
-                "SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables",
-                "SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables",
-                "SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables",
-            ],
-            Field(discriminator="typename__"),
-        ]
-    ] = Field(alias="scheduleVariables")
-
-
-class SubscriptionFutureUpdateDataTargetPackage(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-
-
-class SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables(
-    BaseModel
-):
-    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-
-
-class SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables(BaseModel):
-    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
-    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
-
-
-class SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables(BaseModel):
-    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
-    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
-    feature_id: Optional[str] = Field(alias="featureId")
-
-
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -734,14 +687,61 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
+class SubscriptionFutureUpdateData(BaseModel):
+    subscription_schedule_type: SubscriptionScheduleType = Field(
+        alias="subscriptionScheduleType"
+    )
+    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
+    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
+    target_package: Optional["SubscriptionFutureUpdateDataTargetPackage"] = Field(
+        alias="targetPackage"
+    )
+    schedule_variables: Optional[
+        Annotated[
+            Union[
+                "SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables",
+            ],
+            Field(discriminator="typename__"),
+        ]
+    ] = Field(alias="scheduleVariables")
+
+
+class SubscriptionFutureUpdateDataTargetPackage(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+
+
+class SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+    BaseModel
+):
+    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+
+
+class SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables(BaseModel):
+    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
+    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
+
+
+class SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables(BaseModel):
+    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
+    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
+    feature_id: Optional[str] = Field(alias="featureId")
+
+
 class SubscriptionFragment(BaseModel):
     id: str
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
     trial_end_date: Optional[Any] = Field(alias="trialEndDate")
     cancellation_date: Optional[Any] = Field(alias="cancellationDate")
     effective_end_date: Optional[Any] = Field(alias="effectiveEndDate")
@@ -1407,17 +1407,17 @@
 PriceFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
-SlimCustomerFragment.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
 PromotionalEntitlementFragmentFeature.update_forward_refs()
+SlimCustomerFragment.update_forward_refs()
 CustomerFragment.update_forward_refs()
 CustomerFragmentTrialedPlans.update_forward_refs()
 CustomerFragmentExperimentInfo.update_forward_refs()
 CustomerFragmentCoupon.update_forward_refs()
 CustomerFragmentEligibleForTrial.update_forward_refs()
 CustomerFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalBillingInformation.update_forward_refs()
@@ -1431,49 +1431,44 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
-CustomerPortalSubscriptionPriceFragment.update_forward_refs()
-CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
-CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
+CustomerPortalSubscriptionPriceFragment.update_forward_refs()
+CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
+CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPrices.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerResourceFragment.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
-SubscriptionFutureUpdateData.update_forward_refs()
-SubscriptionFutureUpdateDataTargetPackage.update_forward_refs()
-SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
-SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
-SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
 ProductFragmentProductSettingsDowngradePlan.update_forward_refs()
 PlanFragment.update_forward_refs()
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
@@ -1485,14 +1480,19 @@
 TotalPriceFragmentSubTotal.update_forward_refs()
 TotalPriceFragmentTotal.update_forward_refs()
 SubscriptionScheduledUpdateData.update_forward_refs()
 SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
+SubscriptionFutureUpdateData.update_forward_refs()
+SubscriptionFutureUpdateDataTargetPackage.update_forward_refs()
+SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
 SubscriptionFragmentExperimentInfo.update_forward_refs()
 SubscriptionFragmentPrices.update_forward_refs()
 SubscriptionFragmentPricesPrice.update_forward_refs()
 SubscriptionFragmentTotalPrice.update_forward_refs()
 SubscriptionFragmentPlan.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.509.0/stigg/generated/get_active_subscriptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.509.0/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.509.0/stigg/generated/get_customer_by_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.509.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.509.0/stigg/generated/get_mock_paywall.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.509.0/stigg/generated/get_products.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.509.0/stigg/generated/get_sdk_configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.509.0/stigg/generated/input_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -2134,14 +2134,15 @@
 class SubscriptionAddonSort(BaseModel):
     direction: SortDirection
     field: SubscriptionAddonSortFields
     nulls: Optional[SortNulls]
 
 
 class SubscriptionBillingInfo(BaseModel):
+    tax_percentage: Optional[float] = Field(alias="taxPercentage")
     tax_rate_ids: Optional[List[str]] = Field(alias="taxRateIds")
 
 
 class SubscriptionCancelReasonFilterComparison(BaseModel):
     eq: Optional[SubscriptionCancelReason]
     gt: Optional[SubscriptionCancelReason]
     gte: Optional[SubscriptionCancelReason]
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.509.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.509.0/stigg/generated/provision_customer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.509.0/stigg/generated/provision_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.509.0/stigg/generated/report_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.508.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.509.0/stigg/generated/update_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-27 06:55
+# Generated by ariadne-codegen on 2023-07-27 07:10
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.508.0/PKG-INFO` & `stigg_api_client_v2-0.509.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.508.0
+Version: 0.509.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

