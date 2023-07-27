# Comparing `tmp/pytbai-1.3.8.tar.gz` & `tmp/pytbai-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.3.8.tar", last modified: Wed Jul 26 15:25:11 2023, max compression
+gzip compressed data, was "pytbai-1.4.0.tar", last modified: Thu Jul 27 08:50:20 2023, max compression
```

## Comparing `pytbai-1.3.8.tar` & `pytbai-1.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.351533 pytbai-1.3.8/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2175 2023-07-26 15:25:08.000000 pytbai-1.3.8/CHANGELOG.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-26 15:25:08.000000 pytbai-1.3.8/CODE_OF_CONDUCT.md
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-26 15:25:08.000000 pytbai-1.3.8/LICENSE
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2023-07-26 15:25:08.000000 pytbai-1.3.8/MANIFEST.in
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-26 15:25:08.000000 pytbai-1.3.8/Makefile
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-26 15:25:11.351533 pytbai-1.3.8/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-26 15:25:08.000000 pytbai-1.3.8/README.md
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.335533 pytbai-1.3.8/pytbai/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    11073 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/core.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/definitions.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.339532 pytbai-1.3.8/pytbai/templates/
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.343532 pytbai-1.3.8/pytbai/templates/PDF/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/PDF/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/PDF/ticketbai.css
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/PDF/ticketbai.html
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.343532 pytbai-1.3.8/pytbai/templates/XML/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/XML/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/XML/tbai_structure.xml
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.343532 pytbai-1.3.8/pytbai/templates/XSD/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/XSD/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.347532 pytbai-1.3.8/pytbai/utils/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/utils/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/utils/crypto.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/utils/pdf.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4542 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/utils/xml.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.339532 pytbai-1.3.8/pytbai.egg-info/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-26 15:25:11.000000 pytbai-1.3.8/pytbai.egg-info/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      839 2023-07-26 15:25:11.000000 pytbai-1.3.8/pytbai.egg-info/SOURCES.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-26 15:25:11.000000 pytbai-1.3.8/pytbai.egg-info/dependency_links.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-26 15:25:11.000000 pytbai-1.3.8/pytbai.egg-info/top_level.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-26 15:25:08.000000 pytbai-1.3.8/requirements.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-26 15:25:11.351533 pytbai-1.3.8/setup.cfg
--rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1037 2023-07-26 15:25:08.000000 pytbai-1.3.8/setup.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.347532 pytbai-1.3.8/tests/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:08.000000 pytbai-1.3.8/tests/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.351533 pytbai-1.3.8/tests/certs/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-26 15:25:08.000000 pytbai-1.3.8/tests/certs/cert.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-26 15:25:08.000000 pytbai-1.3.8/tests/certs/cert_for_tests.p12
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-26 15:25:08.000000 pytbai-1.3.8/tests/certs/key.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-26 15:25:08.000000 pytbai-1.3.8/tests/context.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.351533 pytbai-1.3.8/tests/data/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3042 2023-07-26 15:25:08.000000 pytbai-1.3.8/tests/data/tbai_json.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-26 15:25:08.000000 pytbai-1.3.8/tests/test_basic.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.135464 pytbai-1.4.0/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2372 2023-07-27 08:50:18.000000 pytbai-1.4.0/CHANGELOG.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-27 08:50:18.000000 pytbai-1.4.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-27 08:50:18.000000 pytbai-1.4.0/LICENSE
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2023-07-27 08:50:18.000000 pytbai-1.4.0/MANIFEST.in
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-27 08:50:18.000000 pytbai-1.4.0/Makefile
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-27 08:50:20.135464 pytbai-1.4.0/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-27 08:50:18.000000 pytbai-1.4.0/README.md
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.131464 pytbai-1.4.0/pytbai/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    11073 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/core.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/definitions.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.131464 pytbai-1.4.0/pytbai/templates/
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.131464 pytbai-1.4.0/pytbai/templates/PDF/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/PDF/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/PDF/ticketbai.css
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/PDF/ticketbai.html
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.131464 pytbai-1.4.0/pytbai/templates/XML/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/XML/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/XML/tbai_structure.xml
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.131464 pytbai-1.4.0/pytbai/templates/XSD/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/XSD/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.131464 pytbai-1.4.0/pytbai/utils/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/utils/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/utils/crypto.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/utils/pdf.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     5065 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/utils/xml.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.131464 pytbai-1.4.0/pytbai.egg-info/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-27 08:50:20.000000 pytbai-1.4.0/pytbai.egg-info/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      839 2023-07-27 08:50:20.000000 pytbai-1.4.0/pytbai.egg-info/SOURCES.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-27 08:50:20.000000 pytbai-1.4.0/pytbai.egg-info/dependency_links.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-27 08:50:20.000000 pytbai-1.4.0/pytbai.egg-info/top_level.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-27 08:50:18.000000 pytbai-1.4.0/requirements.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-27 08:50:20.135464 pytbai-1.4.0/setup.cfg
+-rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1037 2023-07-27 08:50:18.000000 pytbai-1.4.0/setup.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.135464 pytbai-1.4.0/tests/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:18.000000 pytbai-1.4.0/tests/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.135464 pytbai-1.4.0/tests/certs/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-27 08:50:18.000000 pytbai-1.4.0/tests/certs/cert.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-27 08:50:18.000000 pytbai-1.4.0/tests/certs/cert_for_tests.p12
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-27 08:50:18.000000 pytbai-1.4.0/tests/certs/key.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-27 08:50:18.000000 pytbai-1.4.0/tests/context.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.135464 pytbai-1.4.0/tests/data/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3045 2023-07-27 08:50:18.000000 pytbai-1.4.0/tests/data/tbai_json.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-27 08:50:18.000000 pytbai-1.4.0/tests/test_basic.py
```

### Comparing `pytbai-1.3.8/CHANGELOG.txt` & `pytbai-1.4.0/CHANGELOG.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+1.4.0 (2023-07-27)
+------------------
+
+- fix test for DEV environment [Urtzi Odriozola <uodriozola@codesyntax.com>]
+
+- previous invoice fingerprint [Urtzi Odriozola <uodriozola@codesyntax.com>]
+
+
+
 1.3.8 (2023-07-26)
 ------------------
 
 - DEV url fixed [Urtzi Odriozola <uodriozola@codesyntax.com>]
```

### Comparing `pytbai-1.3.8/LICENSE` & `pytbai-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.8/PKG-INFO` & `pytbai-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.3.8
+Version: 1.4.0
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.3.8/README.md` & `pytbai-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.8/pytbai/core.py` & `pytbai-1.4.0/pytbai/core.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.8/pytbai/definitions.py` & `pytbai-1.4.0/pytbai/definitions.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.8/pytbai/templates/PDF/ticketbai.html` & `pytbai-1.4.0/pytbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.8/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.4.0/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.8/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.4.0/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.8/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.4.0/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.8/pytbai/utils/pdf.py` & `pytbai-1.4.0/pytbai/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.8/pytbai/utils/xml.py` & `pytbai-1.4.0/pytbai/utils/xml.py`

 * *Files 12% similar despite different names*

```diff
@@ -82,14 +82,26 @@
             vat_base = ET.SubElement(rate_detail, "BaseImponible")
             vat_base.text = str(rate[1]["base"])
             vat_rate = ET.SubElement(rate_detail, "TipoImpositivo")
             vat_rate.text = str(float(rate[0]))
             vat_fee = ET.SubElement(rate_detail, "CuotaImpuesto")
             vat_fee.text = str(rate[1]["fee"])
 
+    if pre_invoice:
+        fp_root = root.find(".//HuellaTBAI")
+        p_inv = ET.SubElement(fp_root, "EncadenamientoFacturaAnterior")
+        serial_code = ET.SubElement(p_inv, "SerieFacturaAnterior")
+        serial_code.text = pre_invoice["serial_code"]
+        num = ET.SubElement(p_inv, "NumFacturaAnterior")
+        num.text = pre_invoice["num"]
+        signature_value = ET.SubElement(
+            p_inv, "SignatureValueFirmaFacturaAnterior"
+        )
+        signature_value.text = pre_invoice["signature_value"]
+
     return root
 
 
 def validate_xml(xml):
     path = os.path.dirname(pytbai.__file__)
     xsd_file = os.path.join(path, "templates/XSD/ticketBaiV1-2-1.xsd")
     with open(xsd_file, "r") as file:
```

### Comparing `pytbai-1.3.8/pytbai.egg-info/PKG-INFO` & `pytbai-1.4.0/pytbai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.3.8
+Version: 1.4.0
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.3.8/pytbai.egg-info/SOURCES.txt` & `pytbai-1.4.0/pytbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.8/setup.py` & `pytbai-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.3.8",
+    version="1.4.0",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
```

### Comparing `pytbai-1.3.8/tests/certs/cert.pem` & `pytbai-1.4.0/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.8/tests/certs/cert_for_tests.p12` & `pytbai-1.4.0/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.8/tests/certs/key.pem` & `pytbai-1.4.0/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.8/tests/data/tbai_json.py` & `pytbai-1.4.0/tests/data/tbai_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 TBAI_JSON = {
     "version": "1.2",
     "env": "DEV",
     "subject": {
         "entity_id": "99999974E",
         "name": "REPRESENTANTESPJ FICTICIO",
         "authority_api": "https://tbai-z.prep.gipuzkoa.eus/sarrerak/alta",
-        "qr_api": "https://tbai.prep.gipuzkoa.eus/qr",
+        "qr_api": "https://tbai.prep.gipuzkoa.eus/qr/",
         "multi_recipient": "N",
         "external_invoice": "N",
     },
     "software": {
         "license": "TBAIGIPRE00000000501",
         "dev_entity": "P2000000F",
         "soft_name": "FAKTURABAI",
@@ -20,15 +20,15 @@
 TBAI_INVOICE_JSON = {
     "version": "1.2",
     "env": "DEV",
     "subject": {
         "entity_id": "99999974E",
         "name": "REPRESENTANTESPJ FICTICIO",
         "authority_api": "https://tbai-z.prep.gipuzkoa.eus/sarrerak/alta",
-        "qr_api": "https://tbai.prep.gipuzkoa.eus/qr",
+        "qr_api": "https://tbai.prep.gipuzkoa.eus/qr/",
         "multi_recipient": "N",
         "external_invoice": "N",
     },
     "invoice": {
         "serial_code": "TB-2021-S",
         "num": 1,
         "description": "Primera factura",
@@ -52,15 +52,15 @@
 TBAI_INVOICE_LINES_JSON = {
     "version": "1.2",
     "env": "DEV",
     "subject": {
         "entity_id": "99999974E",
         "name": "REPRESENTANTESPJ FICTICIO",
         "authority_api": "https://tbai-z.prep.gipuzkoa.eus/sarrerak/alta",
-        "qr_api": "https://tbai.prep.gipuzkoa.eus/qr",
+        "qr_api": "https://tbai.prep.gipuzkoa.eus/qr/",
         "multi_recipient": "N",
         "external_invoice": "N",
     },
     "invoice": {
         "serial_code": "TB-2021-S",
         "num": 1,
         "description": "Primera factura",
```

### Comparing `pytbai-1.3.8/tests/test_basic.py` & `pytbai-1.4.0/tests/test_basic.py`

 * *Files identical despite different names*

