# Comparing `tmp/peakventures-1.2.3.tar.gz` & `tmp/peakventures-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakventures-1.2.3.tar", max compression
+gzip compressed data, was "peakventures-1.2.4.tar", max compression
```

## Comparing `peakventures-1.2.3.tar` & `peakventures-1.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-05-26 05:31:43.775672 peakventures-1.2.3/peakventures/__init__.py
--rw-r--r--   0        0        0     1813 2023-07-12 17:49:47.662944 peakventures-1.2.3/peakventures/api.py
--rw-r--r--   0        0        0     4086 2023-07-26 19:37:35.703756 peakventures-1.2.3/peakventures/conversions.py
--rw-r--r--   0        0        0     1095 2023-07-26 09:29:28.910842 peakventures-1.2.3/peakventures/credentials.py
--rw-r--r--   0        0        0      830 2023-07-26 09:28:36.228718 peakventures-1.2.3/peakventures/storage.py
--rw-r--r--   0        0        0      351 2023-07-26 19:39:24.146134 peakventures-1.2.3/pyproject.toml
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 peakventures-1.2.3/setup.py
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 peakventures-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-26 05:31:43.775672 peakventures-1.2.4/peakventures/__init__.py
+-rw-r--r--   0        0        0     1813 2023-07-12 17:49:47.662944 peakventures-1.2.4/peakventures/api.py
+-rw-r--r--   0        0        0     4086 2023-07-27 14:34:46.765643 peakventures-1.2.4/peakventures/conversions.py
+-rw-r--r--   0        0        0     1095 2023-07-26 09:29:28.910842 peakventures-1.2.4/peakventures/credentials.py
+-rw-r--r--   0        0        0      830 2023-07-26 09:28:36.228718 peakventures-1.2.4/peakventures/storage.py
+-rw-r--r--   0        0        0      351 2023-07-27 14:34:54.871367 peakventures-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 peakventures-1.2.4/setup.py
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 peakventures-1.2.4/PKG-INFO
```

### Comparing `peakventures-1.2.3/peakventures/api.py` & `peakventures-1.2.4/peakventures/api.py`

 * *Files identical despite different names*

### Comparing `peakventures-1.2.3/peakventures/conversions.py` & `peakventures-1.2.4/peakventures/conversions.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,28 +73,28 @@
             buyside_network_account: str,
             partner_id: str,
             pixel_id: str,
             pixel_event: str,
             click_id: str,
             conversion_date: int,
             user_agent: str,
-            id_address: str,
+            ip_address: str,
             conversion_value: float) -> None:
         """
         Send conversion event.
 
         :param buyside_network: Buyside network name.
         :param buyside_network_account: Buyside network account name.
         :param partner_id: Partner id.
         :param pixel_id: Pixel id.
         :param pixel_event: Pixel event.
         :param click_id: Click id.
         :param conversion_date: Conversion date.
         :param user_agent: User agent.
-        :param id_address: IP address.
+        :param ip_address: IP address.
         :param conversion_value: Conversion value.
         """
 
         if not self.initialized:
             raise RuntimeError("ConversionsClient is not initialized, use `with` statement")
 
         self.connection.send(json.dumps({
@@ -102,15 +102,15 @@
             "BuysideNetworkAccount": buyside_network_account,
             "PartnerId": partner_id,
             "PixelId": pixel_id,
             "PixelEvent": pixel_event,
             "ClickId": click_id,
             "ConversionDate": conversion_date,
             "UserAgent": user_agent,
-            "IpAddress": id_address,
+            "IpAddress": ip_address,
             "ConversionValue": conversion_value,
         }))
 
         self.conversions_number += 1
 
     def __get_access_token(self: "ConversionsClient") -> str:
         """Get JWT token from client credentials."""
```

### Comparing `peakventures-1.2.3/peakventures/credentials.py` & `peakventures-1.2.4/peakventures/credentials.py`

 * *Files identical despite different names*

### Comparing `peakventures-1.2.3/peakventures/storage.py` & `peakventures-1.2.4/peakventures/storage.py`

 * *Files identical despite different names*

### Comparing `peakventures-1.2.3/setup.py` & `peakventures-1.2.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['boto3>=1.28.11,<2.0.0',
  'tenacity>=8.2.2,<9.0.0',
  'websockets>=11.0.3,<12.0.0']
 
 setup_kwargs = {
     'name': 'peakventures',
-    'version': '1.2.3',
+    'version': '1.2.4',
     'description': 'PeakVentures Python Utilities',
     'long_description': 'None',
     'author': 'Volodymyr Smirnov',
     'author_email': 'volodymyr@peakventures.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `peakventures-1.2.3/PKG-INFO` & `peakventures-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakventures
-Version: 1.2.3
+Version: 1.2.4
 Summary: PeakVentures Python Utilities
 Author: Volodymyr Smirnov
 Author-email: volodymyr@peakventures.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

