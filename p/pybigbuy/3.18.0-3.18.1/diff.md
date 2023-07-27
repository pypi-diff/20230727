# Comparing `tmp/pybigbuy-3.18.0.tar.gz` & `tmp/pybigbuy-3.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybigbuy-3.18.0.tar", max compression
+gzip compressed data, was "pybigbuy-3.18.1.tar", max compression
```

## Comparing `pybigbuy-3.18.0.tar` & `pybigbuy-3.18.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/LICENSE
--rw-r--r--   0        0        0      456 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/README.md
--rw-r--r--   0        0        0      649 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/bigbuy/__init__.py
--rw-r--r--   0        0        0    24609 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/bigbuy/api.py
--rw-r--r--   0        0        0    12700 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/bigbuy/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/bigbuy/py.typed
--rw-r--r--   0        0        0     1403 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/bigbuy/rate_limit.py
--rw-r--r--   0        0        0      952 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/pyproject.toml
--rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 pybigbuy-3.18.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-27 15:29:23.227348 pybigbuy-3.18.1/LICENSE
+-rw-r--r--   0        0        0      456 2023-07-27 15:29:23.227348 pybigbuy-3.18.1/README.md
+-rw-r--r--   0        0        0      665 2023-07-27 15:29:23.227348 pybigbuy-3.18.1/bigbuy/__init__.py
+-rw-r--r--   0        0        0    24800 2023-07-27 15:29:23.227348 pybigbuy-3.18.1/bigbuy/api.py
+-rw-r--r--   0        0        0    12786 2023-07-27 15:29:23.227348 pybigbuy-3.18.1/bigbuy/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-27 15:29:23.227348 pybigbuy-3.18.1/bigbuy/py.typed
+-rw-r--r--   0        0        0     1403 2023-07-27 15:29:23.227348 pybigbuy-3.18.1/bigbuy/rate_limit.py
+-rw-r--r--   0        0        0      952 2023-07-27 15:29:23.227348 pybigbuy-3.18.1/pyproject.toml
+-rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 pybigbuy-3.18.1/PKG-INFO
```

### Comparing `pybigbuy-3.18.0/LICENSE` & `pybigbuy-3.18.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybigbuy-3.18.0/bigbuy/__init__.py` & `pybigbuy-3.18.1/bigbuy/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Bigbuy
 -------
 
 Bigbuy is a library for Python that wraps the BigBuy API.
 """
 
 __author__ = 'Bixoto <info@bixoto.com>'
-__version__ = '3.18.0'
+__version__ = '3.18.1'
 
 from .api import BigBuy
 from .exceptions import (
     BBError, BBResponseError, BBPackError, BBExportError, BBProductError, BBStockError,
     BBNoCarrierError, BBBankWireTooLowError, BBMoneyBoxTooLowError, BBTemporaryOrderError, BBOrderAlreadyExistsError,
     BBOrderTooLowError, BBIncorrectRefError, BBInvalidPaymentError, BBZipcodeFormatError, BBProductNotFoundError,
-    BBServerError, BBRateLimitError, BBValidationError, BBWarehouseSplitError, BBShippingError,
+    BBServerError, BBRateLimitError, BBValidationError, BBWarehouseSplitError, BBShippingError, BBTimeoutError,
 )
 from .rate_limit import RateLimit
```

### Comparing `pybigbuy-3.18.0/bigbuy/api.py` & `pybigbuy-3.18.1/bigbuy/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,14 +440,18 @@
         """
         return self.get_json_api(f'order/reference/{reference}', **params)
 
     def get_order_by_id(self, order_id: Id, **params):
         """Get order information."""
         return self.get_json_api(f'order/{order_id}', **params)
 
+    def get_order_delivery_notes(self, order_id: Id, **params):
+        """Get delivery notes for an order."""
+        return self.get_json_api(f'order/delivery-notes/{order_id}', **params)
+
     def upload_order_invoice(self, order_id: Id, file_b64_content: str, mime_type: str, concept: str, amount: float,
                              **params):
         """
         Upload a base64-encoded invoice to an order in PENDING INVOICE status.
         """
         invoice_payload = {
             "id_order": str(order_id),
```

### Comparing `pybigbuy-3.18.0/bigbuy/exceptions.py` & `pybigbuy-3.18.1/bigbuy/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,18 @@
     pass
 
 
 class BBServerError(BBResponseError):
     pass
 
 
+class BBTimeoutError(BBServerError, TimeoutError):
+    pass
+
+
 class BBValidationError(BBResponseError):
     def __init__(self, error_fields, response: Response, **kwargs):
         text = "Validation failed: %s" % str(error_fields)
         super().__init__(text, response, **kwargs)
         self.error_fields = error_fields
 
 
@@ -277,42 +281,43 @@
         return
 
     is_5xx = response.status_code // 100 == 5
 
     if content is None:
         if text == "You exceeded the rate limit":
             error_class: Type[BBResponseError] = BBRateLimitError
-        elif is_5xx or \
-                text.startswith("<html><body><h1>504 Gateway Time-out</h1>") or \
-                "Internal Server Error" in text or \
-                text == "Bad Gateway":
+        elif "<h1>504 Gateway Time-out</h1>" in text:
+            error_class = BBTimeoutError
+        elif is_5xx or text == "Bad Gateway" or "Internal Server Error" in text:
             error_class = BBServerError
         else:
             error_class = BBResponseError
 
         # Trim what we can.
         if text.startswith("<html>") or text.startswith("<!DOCTYPE html>"):
-            if m := re.match(r".+<body>(.+)</body>\s*</html>\s*", text, re.DOTALL):
+            if m := re.match(r".+<body>(.+)</body>", text, re.DOTALL):
                 text = m.group(1).strip()
 
-                # Trim "<h1>504 Gateway Time-out</h1>"
-                if m := re.match(r"<h1>5\d\d .+?</h1>(.+)$", text, re.DOTALL):
-                    text = m.group(1).strip()
-
                 # <div class="container">
                 #    <h1>Oops! An Error Occurred</h1>
                 #    <h2>The server returned a "500 Internal Server Error".</h2>
                 #    <p>
                 #        Something is broken. Please let us know what you were doing when this error occurred.
                 #        We will fix it as soon as possible. Sorry for any inconvenience caused.
                 #    </p>
                 # </div>
-                if m := re.match(r'<div class="container">\s*<h1>Oops! An Error Occurred</h1>\s*'
-                                 r'<h2>The server returned a "500 Internal Server Error".</h2>\s*'
-                                 r'<p>(.+)</p>\s*</div>$', text, re.DOTALL):
+                if m := re.match(r'<div class="container">(.+)</div>', text, re.DOTALL):
+                    text = m.group(1).strip()
+
+                text = text.replace("<h1>Oops! An Error Occurred</h1>", "").strip()
+
+                if m := re.match(r'<h2>The server returned a "500 Internal Server Error".</h2>\s*'
+                                 r'<p>(.+)</p>$', text, re.DOTALL):
+                    text = m.group(1).strip()
+                elif m := re.match(r'<h1>5.. .*?</h1>\s*(.+)', text, re.DOTALL):
                     text = m.group(1).strip()
 
         raise error_class(text, response)
 
     content = cast(dict, response.json())
 
     bb_code = "unknown"
```

### Comparing `pybigbuy-3.18.0/bigbuy/rate_limit.py` & `pybigbuy-3.18.1/bigbuy/rate_limit.py`

 * *Files identical despite different names*

### Comparing `pybigbuy-3.18.0/pyproject.toml` & `pybigbuy-3.18.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybigbuy"
-version = "3.18.0"
+version = "3.18.1"
 description = "BigBuy API client in Python"
 authors = ["Bixoto <info@bixoto.com>"]
 license = "MIT"
 include = ["bigbuy/py.typed"]
 readme = "README.md"
 # https://github.com/python-poetry/poetry/issues/705#issuecomment-444742697
 packages = [
```

### Comparing `pybigbuy-3.18.0/PKG-INFO` & `pybigbuy-3.18.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybigbuy
-Version: 3.18.0
+Version: 3.18.1
 Summary: BigBuy API client in Python
 License: MIT
 Author: Bixoto
 Author-email: info@bixoto.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

