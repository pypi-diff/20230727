# Comparing `tmp/pytbai-1.4.0.tar.gz` & `tmp/pytbai-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.4.0.tar", last modified: Thu Jul 27 08:50:20 2023, max compression
+gzip compressed data, was "pytbai-1.4.1.tar", last modified: Thu Jul 27 09:17:02 2023, max compression
```

## Comparing `pytbai-1.4.0.tar` & `pytbai-1.4.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.135464 pytbai-1.4.0/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2372 2023-07-27 08:50:18.000000 pytbai-1.4.0/CHANGELOG.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-27 08:50:18.000000 pytbai-1.4.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-27 08:50:18.000000 pytbai-1.4.0/LICENSE
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2023-07-27 08:50:18.000000 pytbai-1.4.0/MANIFEST.in
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-27 08:50:18.000000 pytbai-1.4.0/Makefile
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-27 08:50:20.135464 pytbai-1.4.0/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-27 08:50:18.000000 pytbai-1.4.0/README.md
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.131464 pytbai-1.4.0/pytbai/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    11073 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/core.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/definitions.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.131464 pytbai-1.4.0/pytbai/templates/
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.131464 pytbai-1.4.0/pytbai/templates/PDF/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/PDF/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/PDF/ticketbai.css
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/PDF/ticketbai.html
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.131464 pytbai-1.4.0/pytbai/templates/XML/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/XML/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/XML/tbai_structure.xml
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.131464 pytbai-1.4.0/pytbai/templates/XSD/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/XSD/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/templates/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.131464 pytbai-1.4.0/pytbai/utils/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/utils/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/utils/crypto.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/utils/pdf.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     5065 2023-07-27 08:50:18.000000 pytbai-1.4.0/pytbai/utils/xml.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.131464 pytbai-1.4.0/pytbai.egg-info/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-27 08:50:20.000000 pytbai-1.4.0/pytbai.egg-info/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      839 2023-07-27 08:50:20.000000 pytbai-1.4.0/pytbai.egg-info/SOURCES.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-27 08:50:20.000000 pytbai-1.4.0/pytbai.egg-info/dependency_links.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-27 08:50:20.000000 pytbai-1.4.0/pytbai.egg-info/top_level.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-27 08:50:18.000000 pytbai-1.4.0/requirements.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-27 08:50:20.135464 pytbai-1.4.0/setup.cfg
--rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1037 2023-07-27 08:50:18.000000 pytbai-1.4.0/setup.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.135464 pytbai-1.4.0/tests/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:18.000000 pytbai-1.4.0/tests/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.135464 pytbai-1.4.0/tests/certs/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-27 08:50:18.000000 pytbai-1.4.0/tests/certs/cert.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-27 08:50:18.000000 pytbai-1.4.0/tests/certs/cert_for_tests.p12
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-27 08:50:18.000000 pytbai-1.4.0/tests/certs/key.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-27 08:50:18.000000 pytbai-1.4.0/tests/context.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 08:50:20.135464 pytbai-1.4.0/tests/data/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3045 2023-07-27 08:50:18.000000 pytbai-1.4.0/tests/data/tbai_json.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-27 08:50:18.000000 pytbai-1.4.0/tests/test_basic.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:02.096448 pytbai-1.4.1/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2476 2023-07-27 09:17:00.000000 pytbai-1.4.1/CHANGELOG.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-27 09:17:00.000000 pytbai-1.4.1/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-27 09:17:00.000000 pytbai-1.4.1/LICENSE
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2023-07-27 09:17:00.000000 pytbai-1.4.1/MANIFEST.in
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-27 09:17:00.000000 pytbai-1.4.1/Makefile
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-27 09:17:02.096448 pytbai-1.4.1/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-27 09:17:00.000000 pytbai-1.4.1/README.md
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:02.096448 pytbai-1.4.1/pytbai/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    11073 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/core.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/definitions.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:02.096448 pytbai-1.4.1/pytbai/templates/
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:02.096448 pytbai-1.4.1/pytbai/templates/PDF/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/templates/PDF/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/templates/PDF/ticketbai.css
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/templates/PDF/ticketbai.html
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:02.096448 pytbai-1.4.1/pytbai/templates/XML/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/templates/XML/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/templates/XML/tbai_structure.xml
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:02.096448 pytbai-1.4.1/pytbai/templates/XSD/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/templates/XSD/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/templates/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:02.096448 pytbai-1.4.1/pytbai/utils/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/utils/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/utils/crypto.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/utils/pdf.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     5086 2023-07-27 09:17:00.000000 pytbai-1.4.1/pytbai/utils/xml.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:02.096448 pytbai-1.4.1/pytbai.egg-info/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-27 09:17:02.000000 pytbai-1.4.1/pytbai.egg-info/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      839 2023-07-27 09:17:02.000000 pytbai-1.4.1/pytbai.egg-info/SOURCES.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-27 09:17:02.000000 pytbai-1.4.1/pytbai.egg-info/dependency_links.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-27 09:17:02.000000 pytbai-1.4.1/pytbai.egg-info/top_level.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-27 09:17:00.000000 pytbai-1.4.1/requirements.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-27 09:17:02.096448 pytbai-1.4.1/setup.cfg
+-rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1037 2023-07-27 09:17:00.000000 pytbai-1.4.1/setup.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:02.096448 pytbai-1.4.1/tests/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:00.000000 pytbai-1.4.1/tests/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:02.096448 pytbai-1.4.1/tests/certs/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-27 09:17:00.000000 pytbai-1.4.1/tests/certs/cert.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-27 09:17:00.000000 pytbai-1.4.1/tests/certs/cert_for_tests.p12
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-27 09:17:00.000000 pytbai-1.4.1/tests/certs/key.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-27 09:17:00.000000 pytbai-1.4.1/tests/context.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:17:02.096448 pytbai-1.4.1/tests/data/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3045 2023-07-27 09:17:00.000000 pytbai-1.4.1/tests/data/tbai_json.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-27 09:17:00.000000 pytbai-1.4.1/tests/test_basic.py
```

### Comparing `pytbai-1.4.0/CHANGELOG.txt` & `pytbai-1.4.1/CHANGELOG.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+1.4.1 (2023-07-27)
+------------------
+
+- xml structure [Urtzi Odriozola <uodriozola@codesyntax.com>]
+
+
+
 1.4.0 (2023-07-27)
 ------------------
 
 - fix test for DEV environment [Urtzi Odriozola <uodriozola@codesyntax.com>]
 
 - previous invoice fingerprint [Urtzi Odriozola <uodriozola@codesyntax.com>]
```

### Comparing `pytbai-1.4.0/LICENSE` & `pytbai-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.0/PKG-INFO` & `pytbai-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.4.0
+Version: 1.4.1
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.4.0/README.md` & `pytbai-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.0/pytbai/core.py` & `pytbai-1.4.1/pytbai/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,16 +314,23 @@
         )
         return invoice
 
     def sign_and_send(self, invoice, p12_path, password, pre_invoice=None):
         xml = build_xml(self, invoice, pre_invoice)
         key, cert = get_keycert_from_p12(p12_path, password.encode("utf-8"))
         signed_xml = sign_xml(xml, key, cert)
+        result_json = {
+            "TBAI_ID": None,
+            "CSV": None,
+            "SignedXML": None,
+            "ResponseXML": None,
+        }
+
         if not validate_xml(signed_xml):
-            return (None, None)
+            return result_json
 
         key_file = tempfile.NamedTemporaryFile()
         key_file.write(key)
         key_file.flush()
         cert_file = tempfile.NamedTemporaryFile()
         cert_file.write(cert)
         cert_file.flush()
@@ -337,20 +344,14 @@
             data=etree.tostring(signed_xml),
             cert=(cert_file.name, key_file.name),
         )
 
         key_file.close()
         cert_file.close()
 
-        result_json = {
-            "TBAI_ID": None,
-            "CSV": None,
-            "SignedXML": None,
-            "ResponseXML": None,
-        }
         if response.ok:
             response_xml = etree.fromstring(response.content)
             state = response_xml.find(".//Estado").text
             if state == "01":
                 logger.error("XML not accepted")
                 result_json["ResponseXML"] = response.content
                 return result_json
```

### Comparing `pytbai-1.4.0/pytbai/definitions.py` & `pytbai-1.4.1/pytbai/definitions.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.0/pytbai/templates/PDF/ticketbai.html` & `pytbai-1.4.1/pytbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.0/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.4.1/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.0/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.4.1/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.0/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.4.1/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.0/pytbai/utils/pdf.py` & `pytbai-1.4.1/pytbai/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.0/pytbai/utils/xml.py` & `pytbai-1.4.1/pytbai/utils/xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,16 @@
             vat_rate = ET.SubElement(rate_detail, "TipoImpositivo")
             vat_rate.text = str(float(rate[0]))
             vat_fee = ET.SubElement(rate_detail, "CuotaImpuesto")
             vat_fee.text = str(rate[1]["fee"])
 
     if pre_invoice:
         fp_root = root.find(".//HuellaTBAI")
-        p_inv = ET.SubElement(fp_root, "EncadenamientoFacturaAnterior")
+        p_inv = ET.Element("EncadenamientoFacturaAnterior")
+        fp_root.insert(0, p_inv)
         serial_code = ET.SubElement(p_inv, "SerieFacturaAnterior")
         serial_code.text = pre_invoice["serial_code"]
         num = ET.SubElement(p_inv, "NumFacturaAnterior")
         num.text = pre_invoice["num"]
         signature_value = ET.SubElement(
             p_inv, "SignatureValueFirmaFacturaAnterior"
         )
```

### Comparing `pytbai-1.4.0/pytbai.egg-info/PKG-INFO` & `pytbai-1.4.1/pytbai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.4.0
+Version: 1.4.1
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.4.0/pytbai.egg-info/SOURCES.txt` & `pytbai-1.4.1/pytbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.0/setup.py` & `pytbai-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.4.0",
+    version="1.4.1",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
```

### Comparing `pytbai-1.4.0/tests/certs/cert.pem` & `pytbai-1.4.1/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.0/tests/certs/cert_for_tests.p12` & `pytbai-1.4.1/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.0/tests/certs/key.pem` & `pytbai-1.4.1/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.0/tests/data/tbai_json.py` & `pytbai-1.4.1/tests/data/tbai_json.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.0/tests/test_basic.py` & `pytbai-1.4.1/tests/test_basic.py`

 * *Files identical despite different names*

