# Comparing `tmp/odin_sdk_python-0.0.3.tar.gz` & `tmp/odin_sdk_python-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odin_sdk_python-0.0.3.tar", max compression
+gzip compressed data, was "odin_sdk_python-0.0.4.tar", max compression
```

## Comparing `odin_sdk_python-0.0.3.tar` & `odin_sdk_python-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1349 2023-07-26 15:41:42.692116 odin_sdk_python-0.0.3/README.md
--rw-r--r--   0        0        0     1102 2023-07-26 15:41:42.692507 odin_sdk_python-0.0.3/odin/__init__.py
--rw-r--r--   0        0        0     4046 2023-07-26 15:41:42.692726 odin_sdk_python-0.0.3/odin/example.py
--rw-r--r--   0        0        0      483 2023-07-26 15:41:42.693153 odin_sdk_python-0.0.3/odin/exceptions.py
--rw-r--r--   0        0        0      932 2023-07-26 15:41:42.693496 odin_sdk_python-0.0.3/odin/models/__init__.py
--rw-r--r--   0        0        0     2823 2023-07-26 15:41:42.693754 odin_sdk_python-0.0.3/odin/models/certificate_search_response_model.py
--rw-r--r--   0        0        0      434 2023-07-26 15:41:42.694008 odin_sdk_python-0.0.3/odin/models/get_certificate_count.py
--rw-r--r--   0        0        0     7214 2023-07-26 15:41:42.694304 odin_sdk_python-0.0.3/odin/models/get_certificate_hash_details.py
--rw-r--r--   0        0        0      960 2023-07-26 15:41:42.694466 odin_sdk_python-0.0.3/odin/models/get_certificates_summary.py
--rw-r--r--   0        0        0      429 2023-07-26 15:41:42.694636 odin_sdk_python-0.0.3/odin/models/get_host_count.py
--rw-r--r--   0        0        0     1166 2023-07-26 15:41:42.694819 odin_sdk_python-0.0.3/odin/models/get_hosts_cve_details.py
--rw-r--r--   0        0        0     6979 2023-07-26 15:41:42.695054 odin_sdk_python-0.0.3/odin/models/get_hosts_ip_details_response.py
--rw-r--r--   0        0        0      941 2023-07-26 15:41:42.695234 odin_sdk_python-0.0.3/odin/models/get_hosts_summary_response.py
--rw-r--r--   0        0        0     7628 2023-07-26 15:41:42.695421 odin_sdk_python-0.0.3/odin/models/search_hosts_response_model.py
--rw-r--r--   0        0        0     6375 2023-07-26 15:41:42.695618 odin_sdk_python-0.0.3/odin/odin_client.py
--rw-r--r--   0        0        0      453 2023-07-26 15:42:06.310705 odin_sdk_python-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 odin_sdk_python-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1349 2023-07-26 15:41:42.692116 odin_sdk_python-0.0.4/README.md
+-rw-r--r--   0        0        0     1102 2023-07-26 15:41:42.692507 odin_sdk_python-0.0.4/odin/__init__.py
+-rw-r--r--   0        0        0     4046 2023-07-26 15:41:42.692726 odin_sdk_python-0.0.4/odin/example.py
+-rw-r--r--   0        0        0      483 2023-07-26 15:41:42.693153 odin_sdk_python-0.0.4/odin/exceptions.py
+-rw-r--r--   0        0        0      932 2023-07-26 15:41:42.693496 odin_sdk_python-0.0.4/odin/models/__init__.py
+-rw-r--r--   0        0        0     2823 2023-07-26 15:41:42.693754 odin_sdk_python-0.0.4/odin/models/certificate_search_response_model.py
+-rw-r--r--   0        0        0      434 2023-07-26 15:41:42.694008 odin_sdk_python-0.0.4/odin/models/get_certificate_count.py
+-rw-r--r--   0        0        0     7214 2023-07-26 15:41:42.694304 odin_sdk_python-0.0.4/odin/models/get_certificate_hash_details.py
+-rw-r--r--   0        0        0      960 2023-07-26 15:41:42.694466 odin_sdk_python-0.0.4/odin/models/get_certificates_summary.py
+-rw-r--r--   0        0        0      429 2023-07-26 15:41:42.694636 odin_sdk_python-0.0.4/odin/models/get_host_count.py
+-rw-r--r--   0        0        0     1166 2023-07-26 15:41:42.694819 odin_sdk_python-0.0.4/odin/models/get_hosts_cve_details.py
+-rw-r--r--   0        0        0     7022 2023-07-27 05:09:19.179558 odin_sdk_python-0.0.4/odin/models/get_hosts_ip_details_response.py
+-rw-r--r--   0        0        0      941 2023-07-26 15:41:42.695234 odin_sdk_python-0.0.4/odin/models/get_hosts_summary_response.py
+-rw-r--r--   0        0        0     7628 2023-07-26 15:41:42.695421 odin_sdk_python-0.0.4/odin/models/search_hosts_response_model.py
+-rw-r--r--   0        0        0     6375 2023-07-26 15:41:42.695618 odin_sdk_python-0.0.4/odin/odin_client.py
+-rw-r--r--   0        0        0      453 2023-07-27 05:10:15.399279 odin_sdk_python-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 odin_sdk_python-0.0.4/PKG-INFO
```

### Comparing `odin_sdk_python-0.0.3/README.md` & `odin_sdk_python-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.3/odin/__init__.py` & `odin_sdk_python-0.0.4/odin/__init__.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.3/odin/example.py` & `odin_sdk_python-0.0.4/odin/example.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.3/odin/models/__init__.py` & `odin_sdk_python-0.0.4/odin/models/__init__.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.3/odin/models/certificate_search_response_model.py` & `odin_sdk_python-0.0.4/odin/models/certificate_search_response_model.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.3/odin/models/get_certificate_hash_details.py` & `odin_sdk_python-0.0.4/odin/models/get_certificate_hash_details.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.3/odin/models/get_certificates_summary.py` & `odin_sdk_python-0.0.4/odin/models/get_certificates_summary.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.3/odin/models/get_hosts_cve_details.py` & `odin_sdk_python-0.0.4/odin/models/get_hosts_cve_details.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.3/odin/models/get_hosts_ip_details_response.py` & `odin_sdk_python-0.0.4/odin/models/get_hosts_ip_details_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 class GetHostsIpDetailsResponse:
     def __init__(self, data):
         self.success = None
         self.data = Data()
 
+        self.message = data.get('message')
         self.success = data.get('success')
         self.data.populate_from_data(data.get('data', {}))
 
 
 class Data:
     def __init__(self):
         self.asn = ASN()
```

### Comparing `odin_sdk_python-0.0.3/odin/models/get_hosts_summary_response.py` & `odin_sdk_python-0.0.4/odin/models/get_hosts_summary_response.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.3/odin/models/search_hosts_response_model.py` & `odin_sdk_python-0.0.4/odin/models/search_hosts_response_model.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.3/odin/odin_client.py` & `odin_sdk_python-0.0.4/odin/odin_client.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.3/PKG-INFO` & `odin_sdk_python-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odin-sdk-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: Allows to interact easily with the Odin API and access various cybersecurity services, certificate information, and more.
 Author: Anukul Kumar
 Author-email: anukul.kumar@cyble.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

