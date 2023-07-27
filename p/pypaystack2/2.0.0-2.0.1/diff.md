# Comparing `tmp/pypaystack2-2.0.0.tar.gz` & `tmp/pypaystack2-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypaystack2-2.0.0.tar", max compression
+gzip compressed data, was "pypaystack2-2.0.1.tar", max compression
```

## Comparing `pypaystack2-2.0.0.tar` & `pypaystack2-2.0.1.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0     1079 2023-05-18 18:19:22.020864 pypaystack2-2.0.0/LICENSE
--rw-r--r--   0        0        0     1075 2023-05-18 18:19:22.020864 pypaystack2-2.0.0/README.md
--rw-r--r--   0        0        0     1770 2023-05-18 18:19:22.024197 pypaystack2-2.0.0/pypaystack2/__init__.py
--rw-r--r--   0        0        0      159 2023-05-18 18:19:22.024197 pypaystack2-2.0.0/pypaystack2/_metadata.py
--rw-r--r--   0        0        0     3930 2023-05-18 18:19:22.024197 pypaystack2-2.0.0/pypaystack2/api/__init__.py
--rw-r--r--   0        0        0     3924 2023-05-18 18:19:22.024197 pypaystack2-2.0.0/pypaystack2/api/apple_pay.py
--rw-r--r--   0        0        0    10735 2023-05-18 18:19:22.024197 pypaystack2-2.0.0/pypaystack2/api/bulk_charges.py
--rw-r--r--   0        0        0    12592 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/charge.py
--rw-r--r--   0        0        0    16779 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/customers.py
--rw-r--r--   0        0        0    21621 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/dedicated_accounts.py
--rw-r--r--   0        0        0    15954 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/disputes.py
--rw-r--r--   0        0        0     2387 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/integration.py
--rw-r--r--   0        0        0     7214 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/miscellaneous.py
--rw-r--r--   0        0        0    11648 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/payment_pages.py
--rw-r--r--   0        0        0    20737 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/payment_requests.py
--rw-r--r--   0        0        0    12243 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/plans.py
--rw-r--r--   0        0        0    10712 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/products.py
--rw-r--r--   0        0        0     7205 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/refunds.py
--rw-r--r--   0        0        0     6360 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/settlements.py
--rw-r--r--   0        0        0    12345 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/splits.py
--rw-r--r--   0        0        0    14547 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/subaccounts.py
--rw-r--r--   0        0        0    10647 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/subscriptions.py
--rw-r--r--   0        0        0    13088 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/terminals.py
--rw-r--r--   0        0        0    32495 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/transactions.py
--rw-r--r--   0        0        0    13598 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/transfer_recipients.py
--rw-r--r--   0        0        0     9574 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/transfers.py
--rw-r--r--   0        0        0     7014 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/transfers_control.py
--rw-r--r--   0        0        0     6234 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/verification.py
--rw-r--r--   0        0        0     5043 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/baseapi.py
--rw-r--r--   0        0        0      471 2023-05-18 18:19:22.030863 pypaystack2-2.0.0/pypaystack2/errors.py
--rw-r--r--   0        0        0     6660 2023-05-18 18:19:22.030863 pypaystack2-2.0.0/pypaystack2/paystack.py
--rw-r--r--   0        0        0    13981 2023-05-18 18:19:22.030863 pypaystack2-2.0.0/pypaystack2/utils.py
--rw-r--r--   0        0        0      845 2023-05-18 18:19:22.030863 pypaystack2-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1856 1970-01-01 00:00:00.000000 pypaystack2-2.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1079 2023-07-27 12:05:04.985192 pypaystack2-2.0.1/LICENSE
+-rwxr-xr-x   0        0        0     1075 2023-07-27 12:05:04.985192 pypaystack2-2.0.1/README.md
+-rwxr-xr-x   0        0        0     1770 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/__init__.py
+-rw-r--r--   0        0        0      159 2023-07-27 12:05:33.476159 pypaystack2-2.0.1/pypaystack2/_metadata.py
+-rwxr-xr-x   0        0        0     3930 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/__init__.py
+-rwxr-xr-x   0        0        0     3930 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/apple_pay.py
+-rwxr-xr-x   0        0        0    10735 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/bulk_charges.py
+-rwxr-xr-x   0        0        0    12645 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/charge.py
+-rwxr-xr-x   0        0        0    16806 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/customers.py
+-rwxr-xr-x   0        0        0    21621 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/dedicated_accounts.py
+-rwxr-xr-x   0        0        0    15957 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/disputes.py
+-rw-r--r--   0        0        0     2387 2023-07-27 11:47:10.314724 pypaystack2-2.0.1/pypaystack2/api/integration.py
+-rwxr-xr-x   0        0        0     7214 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/miscellaneous.py
+-rwxr-xr-x   0        0        0    11649 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/payment_pages.py
+-rw-r--r--   0        0        0    20737 2023-07-27 11:47:10.314724 pypaystack2-2.0.1/pypaystack2/api/payment_requests.py
+-rwxr-xr-x   0        0        0    12243 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/plans.py
+-rwxr-xr-x   0        0        0    10736 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/products.py
+-rwxr-xr-x   0        0        0     7205 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/refunds.py
+-rwxr-xr-x   0        0        0     6360 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/settlements.py
+-rwxr-xr-x   0        0        0    12361 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/splits.py
+-rwxr-xr-x   0        0        0    14547 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/subaccounts.py
+-rwxr-xr-x   0        0        0    10647 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/subscriptions.py
+-rw-r--r--   0        0        0    13089 2023-07-27 12:05:39.873045 pypaystack2-2.0.1/pypaystack2/api/terminals.py
+-rwxr-xr-x   0        0        0    32603 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/transactions.py
+-rwxr-xr-x   0        0        0    13614 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/transfer_recipients.py
+-rwxr-xr-x   0        0        0     9574 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/transfers.py
+-rwxr-xr-x   0        0        0     7013 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/transfers_control.py
+-rwxr-xr-x   0        0        0     6234 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/api/verification.py
+-rwxr-xr-x   0        0        0     5068 2023-07-27 12:05:04.998526 pypaystack2-2.0.1/pypaystack2/baseapi.py
+-rw-r--r--   0        0        0      377 2023-07-27 12:05:04.961858 pypaystack2-2.0.1/pypaystack2/exceptions.py
+-rw-r--r--   0        0        0     6660 2023-07-27 11:47:10.318058 pypaystack2-2.0.1/pypaystack2/paystack.py
+-rw-r--r--   0        0        0     1277 2023-07-27 12:05:04.961858 pypaystack2-2.0.1/pypaystack2/utils/__init__.py
+-rw-r--r--   0        0        0     4365 2023-07-27 12:05:04.961858 pypaystack2-2.0.1/pypaystack2/utils/enums.py
+-rw-r--r--   0        0        0     4139 2023-07-27 12:05:04.961858 pypaystack2-2.0.1/pypaystack2/utils/helpers.py
+-rw-r--r--   0        0        0     9250 2023-07-27 12:05:04.961858 pypaystack2-2.0.1/pypaystack2/utils/models.py
+-rwxr-xr-x   0        0        0      847 2023-07-27 12:05:05.001860 pypaystack2-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1856 1970-01-01 00:00:00.000000 pypaystack2-2.0.1/PKG-INFO
```

### Comparing `pypaystack2-2.0.0/LICENSE` & `pypaystack2-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/README.md` & `pypaystack2-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pypaystack2/__init__.py` & `pypaystack2-2.0.1/pypaystack2/__init__.py`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pypaystack2/api/__init__.py` & `pypaystack2-2.0.1/pypaystack2/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pypaystack2/api/apple_pay.py` & `pypaystack2-2.0.1/pypaystack2/api/apple_pay.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pypaystack2.baseapi import BaseAPI, BaseAsyncAPI
 from pypaystack2.utils import HTTPMethod, Response
 
 
 class ApplePay(BaseAPI):
     """Provides a wrapper for paystack Apple Pay API
 
-    The Apple Pay API allows you register your application's top-level domain or subdomain.
+    The Apple Pay API allows you to register your application's top-level domain or subdomain.
     [Visit paystack api doc](https://paystack.com/docs/api/apple-pay/)
     """
 
     def register_domain(self, domain_name: str) -> Response:
         """Register a top-level domain or subdomain for your Apple Pay integration.
 
         This method can only be called with one domain or subdomain at a time.
@@ -57,15 +57,15 @@
             "API calls does not allow HTTPMethod.DELETE have a body"
         )
 
 
 class AsyncApplePay(BaseAsyncAPI):
     """Provides a wrapper for paystack Apple Pay API
 
-    The Apple Pay API allows you register your application's top-level domain or subdomain.
+    The Apple Pay API allows you to register your application's top-level domain or subdomain.
     [Visit paystack api doc](https://paystack.com/docs/api/apple-pay/)
     """
 
     async def register_domain(self, domain_name: str) -> Response:
         """Register a top-level domain or subdomain for your Apple Pay integration.
 
         This method can only be called with one domain or subdomain at a time.
```

### Comparing `pypaystack2-2.0.0/pypaystack2/api/bulk_charges.py` & `pypaystack2-2.0.1/pypaystack2/api/bulk_charges.py`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pypaystack2/api/charge.py` & `pypaystack2-2.0.1/pypaystack2/api/charge.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,15 @@
             pin: 4-digit PIN (send with a non-reusable authorization code)
             metadata: A dictionary of data.
             reference: Unique transaction reference. Only -, .\\`, = and alphanumeric characters allowed.
             ussd: USSD type to charge (don't send if charging an authorization code, bank or card)
             mobile_money: Mobile details (don't send if charging an authorization code, bank or card)
             device_id: This is the unique identifier of the device a user uses in making payment. Only -, .\\`,
                 = and alphanumeric characters allowed.
+            birthday: The birthdate of the customer.
 
         Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
         amount = validate_amount(amount)
         payload = {"email": email, "amount": amount}
```

### Comparing `pypaystack2-2.0.0/pypaystack2/api/customers.py` & `pypaystack2-2.0.1/pypaystack2/api/customers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
 from pypaystack2.baseapi import BaseAPI, BaseAsyncAPI
-from pypaystack2.errors import InvalidDataError
+from pypaystack2.exceptions import InvalidDataException
 from pypaystack2.utils import (
     add_to_payload,
     HTTPMethod,
     append_query_params,
     Identification,
     Country,
     RiskAction,
@@ -67,19 +67,19 @@
         end_date: Optional[str] = None,
         page: int = 1,
         pagination: int = 50,
     ) -> Response:
         """Fetches customers available on your integration.
 
         Args:
-            start_date: A timestamp from which to start listing customers e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-            end_date: A timestamp at which to stop listing customers e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            start_date: A timestamp from which to start listing customers e.g., 2016-09-24T00:00:05.000Z, 2016-09-21
+            end_date: A timestamp at which to stop listing customers e.g., 2016-09-24T00:00:05.000Z, 2016-09-21
             page: Specify exactly what page you want to retrieve. If not specified, we use a default value of 1.
             pagination: Specifies how many records you want to retrieve per page.
-                If not specified we use a default value of 50.
+                If not specified, we use a default value of 50.
 
         Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
         query_params = [
             ("page", page),
@@ -167,19 +167,19 @@
 
         Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
         if identification_type == Identification.BANK_ACCOUNT:
             if bank_code is None:
-                raise InvalidDataError(
+                raise InvalidDataException(
                     "`bank_code` is required if identification type is `Identification.BANK_ACCOUNT`"
                 )
             if account_number is None:
-                raise InvalidDataError(
+                raise InvalidDataException(
                     "`account_number` is required if identification type is `Identification.BANK_ACCOUNT`"
                 )
 
         url = self._parse_url(f"/customer/{email_or_code}/identification")
         payload = {
             "first_name": first_name,
             "last_name": last_name,
@@ -395,19 +395,19 @@
 
         Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
         if identification_type == Identification.BANK_ACCOUNT:
             if bank_code is None:
-                raise InvalidDataError(
+                raise InvalidDataException(
                     "`bank_code` is required if identification type is `Identification.BANK_ACCOUNT`"
                 )
             if account_number is None:
-                raise InvalidDataError(
+                raise InvalidDataException(
                     "`account_number` is required if identification type is `Identification.BANK_ACCOUNT`"
                 )
 
         url = self._parse_url(f"/customer/{email_or_code}/identification")
         payload = {
             "first_name": first_name,
             "last_name": last_name,
```

### Comparing `pypaystack2-2.0.0/pypaystack2/api/dedicated_accounts.py` & `pypaystack2-2.0.1/pypaystack2/api/dedicated_accounts.py`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pypaystack2/api/disputes.py` & `pypaystack2-2.0.1/pypaystack2/api/disputes.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Response,
 )
 
 
 class Dispute(BaseAPI):
     """Provides a wrapper for paystack Disputes API
 
-    The Disputes API allows you manage transaction disputes on your integration.
+    The Disputes API allows you to manage transaction disputes on your integration.
     https://paystack.com/docs/api/#dispute
     """
 
     def get_disputes(
         self,
         start_date: str,
         end_date: str,
```

### Comparing `pypaystack2-2.0.0/pypaystack2/api/integration.py` & `pypaystack2-2.0.1/pypaystack2/api/integration.py`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pypaystack2/api/miscellaneous.py` & `pypaystack2-2.0.1/pypaystack2/api/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pypaystack2/api/payment_pages.py` & `pypaystack2-2.0.1/pypaystack2/api/payment_pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Optional
 
-
 from pypaystack2.baseapi import BaseAPI, BaseAsyncAPI
 from pypaystack2.utils import add_to_payload, append_query_params, HTTPMethod, Response
 
 
 class PaymentPage(BaseAPI):
     """Provides a wrapper for paystack Payment Pages API
 
@@ -63,17 +62,17 @@
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
     ) -> Response:
         """Fetch payment pages available on your integration.
 
         Args:
             page: Specifies exactly what page you want to retrieve.
-                If not specified we use a default value of 1.
+                If not specified, we use a default value of 1.
             pagination: Specifies how many records you want to retrieve per page.
-                If not specified we use a default value of 50.
+                If not specified, we use a default value of 50.
             start_date: A timestamp from which to start listing page e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
             end_date: A timestamp at which to stop listing page e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
 
         Returns:
             A named tuple containing the response gotten from paystack's server.
         """
```

### Comparing `pypaystack2-2.0.0/pypaystack2/api/payment_requests.py` & `pypaystack2-2.0.1/pypaystack2/api/payment_requests.py`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pypaystack2/api/plans.py` & `pypaystack2-2.0.1/pypaystack2/api/plans.py`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pypaystack2/api/products.py` & `pypaystack2-2.0.1/pypaystack2/api/products.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
 from pypaystack2.baseapi import BaseAPI, BaseAsyncAPI
-from pypaystack2.errors import InvalidDataError
+from pypaystack2.exceptions import InvalidDataException
 from pypaystack2.utils import (
     Currency,
     add_to_payload,
     append_query_params,
     HTTPMethod,
     Response,
 )
@@ -43,15 +43,15 @@
             A named tuple containing the response gotten from paystack's server.
 
         Raises:
             InvalidDataError: When unlimited is set to True and quantity has a value.
         """
 
         if unlimited is True and quantity is not None:
-            raise InvalidDataError(
+            raise InvalidDataException(
                 "You can't have unlimited set to True and have a quantity value."
             )
 
         url = self._parse_url("/product")
 
         payload = {
             "name": name,
@@ -136,15 +136,15 @@
             A named tuple containing the response gotten from paystack's server.
 
         Raises:
             InvalidDataError: When unlimited is set to True and quantity has a value.
         """
 
         if unlimited is True and quantity is not None:
-            raise InvalidDataError(
+            raise InvalidDataException(
                 "You can't have unlimited set to True and quantity have a value."
             )
         url = self._parse_url(f"/product/{id}")
         payload = {
             "name": name,
             "description": description,
             "price": price,
@@ -190,15 +190,15 @@
             A named tuple containing the response gotten from paystack's server.
 
         Raises:
             InvalidDataError: When unlimited is set to True and quantity has a value.
         """
 
         if unlimited is True and quantity is not None:
-            raise InvalidDataError(
+            raise InvalidDataException(
                 "You can't have unlimited set to True and have a quantity value."
             )
 
         url = self._parse_url("/product")
 
         payload = {
             "name": name,
@@ -283,15 +283,15 @@
             A named tuple containing the response gotten from paystack's server.
 
         Raises:
             InvalidDataError: When unlimited is set to True and quantity has a value.
         """
 
         if unlimited is True and quantity is not None:
-            raise InvalidDataError(
+            raise InvalidDataException(
                 "You can't have unlimited set to True and quantity have a value."
             )
         url = self._parse_url(f"/product/{id}")
         payload = {
             "name": name,
             "description": description,
             "price": price,
```

### Comparing `pypaystack2-2.0.0/pypaystack2/api/refunds.py` & `pypaystack2-2.0.1/pypaystack2/api/refunds.py`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pypaystack2/api/settlements.py` & `pypaystack2-2.0.1/pypaystack2/api/settlements.py`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pypaystack2/api/splits.py` & `pypaystack2-2.0.1/pypaystack2/api/splits.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
 from pypaystack2.baseapi import BaseAPI, BaseAsyncAPI
-from pypaystack2.errors import InvalidDataError
+from pypaystack2.exceptions import InvalidDataException
 from pypaystack2.utils import (
     Bearer,
     Currency,
     Split,
     add_to_payload,
     append_query_params,
     validate_amount,
@@ -131,15 +131,15 @@
 
         Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
         if bearer_subaccount:
             if bearer_type != Bearer.SUB_ACCOUNT:
-                raise InvalidDataError(
+                raise InvalidDataException(
                     "`bearer_subaccount` can only have a value if `bearer_type` is `Bearer.SUBACCOUNT`"
                 )
 
         payload = {
             "name": name,
             "active": active,
         }
@@ -302,15 +302,15 @@
 
         Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
         if bearer_subaccount:
             if bearer_type != Bearer.SUB_ACCOUNT:
-                raise InvalidDataError(
+                raise InvalidDataException(
                     "`bearer_subaccount` can only have a value if `bearer_type` is `Bearer.SUBACCOUNT`"
                 )
 
         payload = {
             "name": name,
             "active": active,
         }
```

### Comparing `pypaystack2-2.0.0/pypaystack2/api/subaccounts.py` & `pypaystack2-2.0.1/pypaystack2/api/subaccounts.py`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pypaystack2/api/subscriptions.py` & `pypaystack2-2.0.1/pypaystack2/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pypaystack2/api/terminals.py` & `pypaystack2-2.0.1/pypaystack2/api/terminals.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from typing import Optional
 
 from pypaystack2.baseapi import BaseAPI, BaseAsyncAPI
-from pypaystack2.errors import InvalidDataError
+from pypaystack2.exceptions import InvalidDataException
 from pypaystack2.utils import (
     TerminalEvent,
     TerminalEventAction,
     append_query_params,
     HTTPMethod,
     Response,
 )
 
 
 class Terminal(BaseAPI):
     """Provides a wrapper for paystack Terminal API
 
-    The Terminal API allows you to create and manage recurring
-    payment on your integration.
-    https://paystack.com/docs/api/#terminal
+    The Terminal API allows you to build delightful in-person payment experiences.
+    https://paystack.com/docs/api/terminal/
     """
 
     def send_event(
         self,
         terminal_id: str,
         type: TerminalEvent,
         action: TerminalEventAction,
@@ -50,15 +49,15 @@
             },
             TerminalEvent.INVOICE: {
                 TerminalEventAction.PROCESS,
                 TerminalEventAction.VIEW,
             },
         }
         if action not in supported_actions_mapping[type]:
-            raise InvalidDataError(
+            raise InvalidDataException(
                 f"Terminal Event: {type} does not support Terminal Event Action: {action}"
             )
 
         url = self._parse_url(f"/terminal/{terminal_id}/event")
 
         payload = {
             "type": type,
@@ -126,15 +125,15 @@
 
         Returns:
             A named tuple containing the response gotten from paystack's server.
         """
         url = self._parse_url(f"/terminal/{terminal_id}/")
         return self._handle_request(HTTPMethod.GET, url)
 
-    def updated_terminal(self, terminal_id: str, name: str, address: str) -> Response:
+    def update_terminal(self, terminal_id: str, name: str, address: str) -> Response:
         """Update the details of a Terminal
 
         Args:
             terminal_id: The ID of the Terminal you want to update
             name: Name of the terminal
             address: The address of the Terminal
 
@@ -219,15 +218,15 @@
             },
             TerminalEvent.INVOICE: {
                 TerminalEventAction.PROCESS,
                 TerminalEventAction.VIEW,
             },
         }
         if action not in supported_actions_mapping[type]:
-            raise InvalidDataError(
+            raise InvalidDataException(
                 f"Terminal Event: {type} does not support Terminal Event Action: {action}"
             )
 
         url = self._parse_url(f"/terminal/{terminal_id}/event")
 
         payload = {
             "type": type,
@@ -295,15 +294,15 @@
 
         Returns:
             A named tuple containing the response gotten from paystack's server.
         """
         url = self._parse_url(f"/terminal/{terminal_id}/")
         return await self._handle_request(HTTPMethod.GET, url)
 
-    async def updated_terminal(
+    async def update_terminal(
         self, terminal_id: str, name: str, address: str
     ) -> Response:
         """Update the details of a Terminal
 
         Args:
             terminal_id: The ID of the Terminal you want to update
             name: Name of the terminal
```

### Comparing `pypaystack2-2.0.0/pypaystack2/api/transactions.py` & `pypaystack2-2.0.1/pypaystack2/api/transactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
 from pypaystack2.baseapi import BaseAPI, BaseAsyncAPI
-from pypaystack2.errors import InvalidDataError
+from pypaystack2.exceptions import InvalidDataException
 from pypaystack2.utils import (
     Bearer,
     Channel,
     Currency,
     TransactionStatus,
     add_to_payload,
     append_query_params,
@@ -66,15 +66,17 @@
 
         Raises:
             InvalidDataError: When email is not provided.
         """
         amount = validate_amount(amount)
 
         if not email:
-            raise InvalidDataError("Customer's Email is required for initialization")
+            raise InvalidDataException(
+                "Customer's Email is required for initialization"
+            )
 
         url = self._parse_url("/transaction/initialize")
         payload = {
             "email": email,
             "amount": amount,
         }
 
@@ -212,18 +214,18 @@
         Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
         amount = validate_amount(amount)
 
         if not email:
-            raise InvalidDataError("Customer's Email is required to charge")
+            raise InvalidDataException("Customer's Email is required to charge")
 
         if not auth_code:
-            raise InvalidDataError("Customer's Auth code is required to charge")
+            raise InvalidDataException("Customer's Auth code is required to charge")
 
         url = self._parse_url("/transaction/charge_authorization")
         payload = {
             "authorization_code": auth_code,
             "email": email,
             "amount": amount,
         }
@@ -370,18 +372,18 @@
             InvalidDataError: When Customer's email is not provided. When Customer's auth code is not provided.
         """
         amount = validate_amount(amount)
         if at_least:
             at_least = validate_amount(at_least)
 
         if not email:
-            raise InvalidDataError("Customer's Email is required to charge")
+            raise InvalidDataException("Customer's Email is required to charge")
 
         if not auth_code:
-            raise InvalidDataError("Customer's Auth code is required to charge")
+            raise InvalidDataException("Customer's Auth code is required to charge")
 
         url = self._parse_url("/transaction/partial_debit")
         payload = {
             "authorization_code": auth_code,
             "currency": currency,
             "amount": amount,
             "email": email,
@@ -443,15 +445,17 @@
 
         Raises:
             InvalidDataError: When email is not provided.
         """
         amount = validate_amount(amount)
 
         if not email:
-            raise InvalidDataError("Customer's Email is required for initialization")
+            raise InvalidDataException(
+                "Customer's Email is required for initialization"
+            )
 
         url = self._parse_url("/transaction/initialize")
         payload = {
             "email": email,
             "amount": amount,
         }
 
@@ -589,18 +593,18 @@
         Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
         amount = validate_amount(amount)
 
         if not email:
-            raise InvalidDataError("Customer's Email is required to charge")
+            raise InvalidDataException("Customer's Email is required to charge")
 
         if not auth_code:
-            raise InvalidDataError("Customer's Auth code is required to charge")
+            raise InvalidDataException("Customer's Auth code is required to charge")
 
         url = self._parse_url("/transaction/charge_authorization")
         payload = {
             "authorization_code": auth_code,
             "email": email,
             "amount": amount,
         }
@@ -747,18 +751,18 @@
             InvalidDataError: When Customer's email is not provided. When Customer's auth code is not provided.
         """
         amount = validate_amount(amount)
         if at_least:
             at_least = validate_amount(at_least)
 
         if not email:
-            raise InvalidDataError("Customer's Email is required to charge")
+            raise InvalidDataException("Customer's Email is required to charge")
 
         if not auth_code:
-            raise InvalidDataError("Customer's Auth code is required to charge")
+            raise InvalidDataException("Customer's Auth code is required to charge")
 
         url = self._parse_url("/transaction/partial_debit")
         payload = {
             "authorization_code": auth_code,
             "currency": currency,
             "amount": amount,
             "email": email,
```

### Comparing `pypaystack2-2.0.0/pypaystack2/api/transfer_recipients.py` & `pypaystack2-2.0.1/pypaystack2/api/transfer_recipients.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
 from pypaystack2.baseapi import BaseAPI, BaseAsyncAPI
-from pypaystack2.errors import InvalidDataError
+from pypaystack2.exceptions import InvalidDataException
 from pypaystack2.utils import (
     Currency,
     RecipientType,
     add_to_payload,
     append_query_params,
     HTTPMethod,
     Response,
@@ -54,15 +54,15 @@
         Returns:
             A named tuple containing the response gotten from paystack's server.
         """
         # FIXME: type is a keyword arg, might replace
         # if it raises issues.
         if type == RecipientType.NUBAN or type == RecipientType.BASA:
             if bank_code is None:
-                raise InvalidDataError(
+                raise InvalidDataException(
                     "`bank_code` is required if type is `TRType.NUBAN` or `TRType.BASA`"
                 )
 
         url = self._parse_url("/transferrecipient")
 
         payload = {
             "type": type,
@@ -230,15 +230,15 @@
         Returns:
             A named tuple containing the response gotten from paystack's server.
         """
         # FIXME: type is a keyword arg, might replace
         # if it raises issues.
         if type == RecipientType.NUBAN or type == RecipientType.BASA:
             if bank_code is None:
-                raise InvalidDataError(
+                raise InvalidDataException(
                     "`bank_code` is required if type is `TRType.NUBAN` or `TRType.BASA`"
                 )
 
         url = self._parse_url("/transferrecipient")
 
         payload = {
             "type": type,
```

### Comparing `pypaystack2-2.0.0/pypaystack2/api/transfers.py` & `pypaystack2-2.0.1/pypaystack2/api/transfers.py`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pypaystack2/api/transfers_control.py` & `pypaystack2-2.0.1/pypaystack2/api/transfers_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pypaystack2.baseapi import BaseAPI, BaseAsyncAPI
 from pypaystack2.utils import Reason, HTTPMethod, Response
 
 
 class TransferControl(BaseAPI):
     """Provides a wrapper for paystack Transfers Control API
 
-    The Transfers Control API allows you to manage settings of your transfers.
+    The Transfer Control API allows you to manage settings of your transfers.
     https://paystack.com/docs/api/#transfer-control
     """
 
     def check_balance(self) -> Response:
         """Fetch the available balance on your integration
 
         Returns:
```

### Comparing `pypaystack2-2.0.0/pypaystack2/api/verification.py` & `pypaystack2-2.0.1/pypaystack2/api/verification.py`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pypaystack2/baseapi.py` & `pypaystack2-2.0.1/pypaystack2/baseapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 from abc import ABC, abstractmethod
 from typing import Union, Optional
 
 import httpx
 from httpx import codes
+
 from pypaystack2._metadata import __version__
-from pypaystack2.errors import InvalidMethodError, MissingAuthKeyError
+from pypaystack2.exceptions import InvalidMethodException, MissingAuthKeyException
 from pypaystack2.utils import HTTPMethod, Response
 
 
 class AbstractAPI(ABC):
     _CONTENT_TYPE = "application/json"
     _BASE_URL = "https://api.paystack.co"
 
@@ -24,15 +25,15 @@
         if auth_key:
             self._PAYSTACK_AUTHORIZATION_KEY = auth_key
         else:
             self._PAYSTACK_AUTHORIZATION_KEY = os.getenv(
                 "PAYSTACK_AUTHORIZATION_KEY", None
             )
         if not self._PAYSTACK_AUTHORIZATION_KEY:
-            raise MissingAuthKeyError(
+            raise MissingAuthKeyException(
                 "Missing Authorization key argument or env variable"
             )
 
     def _parse_url(self, endpoint_path: str) -> str:
         return f"{self._BASE_URL}{endpoint_path}"
 
     @property
@@ -109,15 +110,15 @@
         http_method = http_methods_map.get(method)
 
         http_method_kwargs = self._parse_http_method_kwargs(
             url=url, method=method, data=data
         )
 
         if not http_method:
-            raise InvalidMethodError(
+            raise InvalidMethodException(
                 "HTTP Request method not recognised or implemented"
             )
 
         response = http_method(**http_method_kwargs)
         if codes.is_success(response.status_code):
             return self._parse_response(response)
         else:
@@ -137,15 +138,15 @@
         """
         async with httpx.AsyncClient() as client:
             http_method = getattr(client, method.value.lower(), None)
             http_method_kwargs = self._parse_http_method_kwargs(
                 url=url, method=method, data=data
             )
             if not http_method:
-                raise InvalidMethodError(
+                raise InvalidMethodException(
                     "HTTP Request method not recognised or implemented"
                 )
             response = await http_method(**http_method_kwargs)
 
         if codes.is_success(response.status_code):
             return self._parse_response(response)
         else:
```

### Comparing `pypaystack2-2.0.0/pypaystack2/paystack.py` & `pypaystack2-2.0.1/pypaystack2/paystack.py`

 * *Files identical despite different names*

### Comparing `pypaystack2-2.0.0/pyproject.toml` & `pypaystack2-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypaystack2"
-version = "2.0.0"
+version = "2.0.1"
 description = "A developer-friendly API wrapper."
 authors = ["Gbenga Adeyi <adeyigbenga005@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "pypaystack2" }]
 keywords = ["paystack-python", "pypaystack", "paystack", "paystackapi"]
 license = "MIT"
 classifiers = [
@@ -18,15 +18,15 @@
 httpx = "^0.24.0"
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^0.21.0"
 mkdocs = "^1.4.2"
 mkdocs-material = "^8.5.11"
 typer = "^0.7.0"
-mkdocstrings = {extras = ["python"], version = "^0.21.2"}
+mkdocstrings = { extras = ["python"], version = "^0.21.2" }
 pytest = "^7.2.0"
 black = "^22.12.0"
 tomli = "^2.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pypaystack2-2.0.0/PKG-INFO` & `pypaystack2-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypaystack2
-Version: 2.0.0
+Version: 2.0.1
 Summary: A developer-friendly API wrapper.
 License: MIT
 Keywords: paystack-python,pypaystack,paystack,paystackapi
 Author: Gbenga Adeyi
 Author-email: adeyigbenga005@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

