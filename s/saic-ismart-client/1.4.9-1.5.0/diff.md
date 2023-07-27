# Comparing `tmp/saic_ismart_client-1.4.9.tar.gz` & `tmp/saic_ismart_client-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client-1.4.9.tar", last modified: Sun Jul 23 18:08:36 2023, max compression
+gzip compressed data, was "saic_ismart_client-1.5.0.tar", last modified: Thu Jul 27 13:59:51 2023, max compression
```

## Comparing `saic_ismart_client-1.4.9.tar` & `saic_ismart_client-1.5.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:36.562830 saic_ismart_client-1.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-23 18:08:36.562830 saic_ismart_client-1.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 18:08:36.562830 saic_ismart_client-1.4.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:36.550830 saic_ismart_client-1.4.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:36.554830 saic_ismart_client-1.4.9/src/saic_ismart_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:36.550830 saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:36.558830 saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:36.558830 saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:36.558830 saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24328 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/common_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/message_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:36.558830 saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v1_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v1_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:36.558830 saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v2_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v2_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v2_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:36.562830 saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v3_0/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v3_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23497 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v3_0/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    43908 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/src/saic_ismart_client/saic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:36.554830 saic_ismart_client-1.4.9/src/saic_ismart_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-23 18:08:36.000000 saic_ismart_client-1.4.9/src/saic_ismart_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-23 18:08:36.000000 saic_ismart_client-1.4.9/src/saic_ismart_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 18:08:36.000000 saic_ismart_client-1.4.9/src/saic_ismart_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-23 18:08:36.000000 saic_ismart_client-1.4.9/src/saic_ismart_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-23 18:08:36.000000 saic_ismart_client-1.4.9/src/saic_ismart_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:08:36.562830 saic_ismart_client-1.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/tests/test_Message_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/tests/test_Message_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/tests/test_Message_v3_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/tests/test_abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-23 18:08:22.000000 saic_ismart_client-1.4.9/tests/test_saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.516771 saic_ismart_client-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.516771 saic_ismart_client-1.5.0/src/saic_ismart_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.516771 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25362 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/common_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/message_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v1_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v1_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v2_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v2_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v2_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v3_0/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v3_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23497 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v3_0/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44103 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-27 13:59:51.000000 saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-27 13:59:51.000000 saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:59:51.000000 saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-27 13:59:51.000000 saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 13:59:51.000000 saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/tests/test_Message_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/tests/test_Message_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/tests/test_Message_v3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/tests/test_abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/tests/test_saic_api.py
```

### Comparing `saic_ismart_client-1.4.9/LICENSE` & `saic_ismart_client-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/PKG-INFO` & `saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: saic_ismart_client
-Version: 1.4.9
+Name: saic-ismart-client
+Version: 1.5.0
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.4.9/README.md` & `saic_ismart_client-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/pyproject.toml` & `saic_ismart_client-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client"
-version = "1.4.9"
+version = "1.5.0"
 authors = [
     { name = "Thomas Salm", email="saic-python-client@devtom.de"},
 ]
 dependencies = [
     "asn1tools >= 0.166.0",
     "requests >= 2.31.0",
     "urllib3 >= 2.0.3",
```

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1` & `saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1` & `saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1` & `saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1` & `saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/abrp_api.py` & `saic_ismart_client-1.5.0/src/saic_ismart_client/abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/common_model.py` & `saic_ismart_client-1.5.0/src/saic_ismart_client/common_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,50 @@
 
 class ScheduledChargingMode(Enum):
     DISABLED = 2
     UNTIL_CONFIGURED_SOC = 3
     UNTIL_CONFIGURED_TIME = 1
 
 
+class ChargeCurrentLimitCode(Enum):
+    C_IGNORE = 0
+    C_6A = 1
+    C_8A = 2
+    C_16A = 3
+    C_MAX = 4
+
+    @staticmethod
+    def to_code(limit: str):
+        match limit.upper():
+            case "6A":
+                return ChargeCurrentLimitCode.C_6A
+            case "8A":
+                return ChargeCurrentLimitCode.C_8A
+            case "16A":
+                return ChargeCurrentLimitCode.C_16A
+            case "MAX":
+                return ChargeCurrentLimitCode.C_MAX
+            case _:
+                raise ValueError(f'Unknown charge current limit: {limit}')
+
+    def get_limit(self) -> str:
+        match self:
+            case ChargeCurrentLimitCode.C_6A:
+                return "6A"
+            case ChargeCurrentLimitCode.C_8A:
+                return "8A"
+            case ChargeCurrentLimitCode.C_16A:
+                return "16A"
+            case ChargeCurrentLimitCode.C_MAX:
+                return "Max"
+            case _:
+                raise ValueError(f'Unknown charge current limit code: {self}')
+
+
+
 class TargetBatteryCode(Enum):
     P_40 = 1
     P_50 = 2
     P_60 = 3
     P_70 = 4
     P_80 = 5
     P_90 = 6
```

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/message_decoder.py` & `saic_ismart_client-1.5.0/src/saic_ismart_client/message_decoder.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v1_1/Message.py` & `saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v1_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v1_1/data_model.py` & `saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v1_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v2_1/Message.py` & `saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v2_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v2_1/data_model.py` & `saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v2_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v3_0/Message.py` & `saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v3_0/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/ota_v3_0/data_model.py` & `saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v3_0/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client/saic_api.py` & `saic_ismart_client-1.5.0/src/saic_ismart_client/saic_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 import urllib.parse
 from typing import cast
 
 import requests as requests
 
 from saic_ismart_client.common_model import AbstractMessage, AbstractMessageBody, Header, MessageBodyV2, MessageV2, \
-    ScheduledChargingMode, TargetBatteryCode
+    ScheduledChargingMode, TargetBatteryCode, ChargeCurrentLimitCode
 from saic_ismart_client.ota_v1_1.Message import MessageCoderV11
 from saic_ismart_client.ota_v1_1.data_model import AbortSendMessageReq, AlarmSwitch, AlarmSwitchReq, Message, \
     MessageBodyV11, MessageListReq, MessageListResp, MessageV11, MpAlarmSettingType, MpUserLoggingInReq, \
     MpUserLoggingInRsp, StartEndNumber, Timestamp, VinInfo
 from saic_ismart_client.ota_v2_1.Message import MessageCoderV21
 from saic_ismart_client.ota_v2_1.data_model import OtaRvcReq, OtaRvcStatus25857, OtaRvmVehicleStatusReq, \
     OtaRvmVehicleStatusResp25857, RvcReqParam
@@ -635,18 +635,24 @@
 
     def start_charging(self, vin_info: VinInfo, event_id: str = None) -> MessageV30:
         return self.control_charging(False, vin_info, event_id)
 
     def start_charging_with_retry(self, vin_info: VinInfo) -> MessageV30:
         return self.handle_retry(self.start_charging, vin_info)
 
-    def set_target_battery_soc(self, target_soc: TargetBatteryCode, vin_info: VinInfo, event_id: str = None):
+    def set_target_battery_soc(
+            self,
+            target_soc: TargetBatteryCode,
+            vin_info: VinInfo,
+            charge_current_limit: ChargeCurrentLimitCode = ChargeCurrentLimitCode.C_IGNORE,
+            event_id: str = None
+    ):
         chrg_setng_req = OtaChrgSetngReq()
         chrg_setng_req.onBdChrgTrgtSOCReq = target_soc.value
-        chrg_setng_req.altngChrgCrntReq = 4
+        chrg_setng_req.altngChrgCrntReq = charge_current_limit.value
         chrg_setng_req.tboxV2XSpSOCReq = 0
         chrg_setng_req_msg = MessageV30(MessageBodyV30(), chrg_setng_req)
         application_id = '516'
         application_data_protocol_version = 768
         self.message_V3_0_coder.initialize_message(self.uid, self.get_token(), vin_info.vin, application_id,
                                                    application_data_protocol_version, 3, chrg_setng_req_msg)
         if event_id is not None:
```

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client.egg-info/PKG-INFO` & `saic_ismart_client-1.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: saic-ismart-client
-Version: 1.4.9
+Name: saic_ismart_client
+Version: 1.5.0
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.4.9/src/saic_ismart_client.egg-info/SOURCES.txt` & `saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/tests/test_Message_v1_1.py` & `saic_ismart_client-1.5.0/tests/test_Message_v1_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/tests/test_Message_v2_1.py` & `saic_ismart_client-1.5.0/tests/test_Message_v2_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/tests/test_Message_v3_0.py` & `saic_ismart_client-1.5.0/tests/test_Message_v3_0.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/tests/test_abrp_api.py` & `saic_ismart_client-1.5.0/tests/test_abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.9/tests/test_saic_api.py` & `saic_ismart_client-1.5.0/tests/test_saic_api.py`

 * *Files identical despite different names*

