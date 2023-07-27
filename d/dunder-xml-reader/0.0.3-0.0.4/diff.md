# Comparing `tmp/dunder_xml_reader-0.0.3.tar.gz` & `tmp/dunder_xml_reader-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dunder_xml_reader-0.0.3.tar", last modified: Mon Apr 17 20:17:15 2023, max compression
+gzip compressed data, was "dunder_xml_reader-0.0.4.tar", last modified: Thu Jul 27 03:03:04 2023, max compression
```

## Comparing `dunder_xml_reader-0.0.3.tar` & `dunder_xml_reader-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:17:15.146545 dunder_xml_reader-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    52875 2023-04-17 20:17:15.146545 dunder_xml_reader-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:17:15.142545 dunder_xml_reader-0.0.3/dunder_xml_reader/
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/dunder_xml_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/dunder_xml_reader/safe_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/dunder_xml_reader/xml_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/dunder_xml_reader/xml_node_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:17:15.142545 dunder_xml_reader-0.0.3/dunder_xml_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    52875 2023-04-17 20:17:15.000000 dunder_xml_reader-0.0.3/dunder_xml_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-17 20:17:15.000000 dunder_xml_reader-0.0.3/dunder_xml_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:17:15.000000 dunder_xml_reader-0.0.3/dunder_xml_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 20:17:15.000000 dunder_xml_reader-0.0.3/dunder_xml_reader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-17 20:17:15.146545 dunder_xml_reader-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:17:15.142545 dunder_xml_reader-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/test/test_safe_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/test/test_xml_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-17 20:16:49.000000 dunder_xml_reader-0.0.3/test/test_xml_node_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:03:04.128629 dunder_xml_reader-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    52880 2023-07-27 03:03:04.128629 dunder_xml_reader-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:03:04.128629 dunder_xml_reader-0.0.4/dunder_xml_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/dunder_xml_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/dunder_xml_reader/safe_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/dunder_xml_reader/xml_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/dunder_xml_reader/xml_node_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:03:04.128629 dunder_xml_reader-0.0.4/dunder_xml_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    52880 2023-07-27 03:03:04.000000 dunder_xml_reader-0.0.4/dunder_xml_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-27 03:03:04.000000 dunder_xml_reader-0.0.4/dunder_xml_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:03:04.000000 dunder_xml_reader-0.0.4/dunder_xml_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 03:03:04.000000 dunder_xml_reader-0.0.4/dunder_xml_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-27 03:03:04.132629 dunder_xml_reader-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:03:04.128629 dunder_xml_reader-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/test/test_safe_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/test/test_xml_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/test/test_xml_node_list.py
```

### Comparing `dunder_xml_reader-0.0.3/LICENSE` & `dunder_xml_reader-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dunder_xml_reader-0.0.3/PKG-INFO` & `dunder_xml_reader-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dunder_xml_reader
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pythonic XML parsing/reading
 Author-email: Steve Brettschneider <steve@bluehousefamily.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -987,15 +987,15 @@
 If your object-graph is wrapped in a SafeReference instance, it will check at each level
 for the requested attribute to be there or missing.  If it's there, it will return the
 requested attribute.  However, if it's not there, it will return a default-value.  Here's
 an example:
 
     >>> cxml = parse_cxml(raw_xml_text_thats_missing_a_BillTo_element)
     >>> safe_cxml = safe_reference(cxml, 'n/a')
-    >>> x = cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    >>> x = safe_cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
     >>> print(x)
     n/a
     >>>
 
 This result of `n/a` will be the result no matter what item is missing (`Request`, `OrderRequest`,
 `OrderRequestHeader`, `BillTo`, etc.) along the way.  If any of the objects in that long
 dereferencing are missing, the default will be returned.  However, if nothing is missing, the
```

### Comparing `dunder_xml_reader-0.0.3/README.md` & `dunder_xml_reader-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
 If your object-graph is wrapped in a SafeReference instance, it will check at each level
 for the requested attribute to be there or missing.  If it's there, it will return the
 requested attribute.  However, if it's not there, it will return a default-value.  Here's
 an example:
 
     >>> cxml = parse_cxml(raw_xml_text_thats_missing_a_BillTo_element)
     >>> safe_cxml = safe_reference(cxml, 'n/a')
-    >>> x = cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    >>> x = safe_cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
     >>> print(x)
     n/a
     >>>
 
 This result of `n/a` will be the result no matter what item is missing (`Request`, `OrderRequest`,
 `OrderRequestHeader`, `BillTo`, etc.) along the way.  If any of the objects in that long
 dereferencing are missing, the default will be returned.  However, if nothing is missing, the
```

### Comparing `dunder_xml_reader-0.0.3/dunder_xml_reader/__init__.py` & `dunder_xml_reader-0.0.4/dunder_xml_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `dunder_xml_reader-0.0.3/dunder_xml_reader/safe_reference.py` & `dunder_xml_reader-0.0.4/dunder_xml_reader/safe_reference.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,29 @@
         try:
             return SafeReference(getattr(self.object, item), self.default)
         except:
             if self.object is not self.default:
                 print(f"SafeReference: Dereference fault: {self.object.__class__.__name__}.{item}", file=sys.stderr)
             return SafeReference(self.default, self.default)
 
+    class Iterator:
+        def __init__(self, obj):
+            self.obj = obj
+            self.max_index = len(obj)
+            self.current_index = 0
+
+        def __next__(self):
+            if self.current_index < self.max_index:
+                self.current_index += 1
+                return self.obj[self.current_index-1]
+            raise StopIteration
+
+    def __iter__(self):
+        return SafeReference.Iterator(self)
+
     def __getitem__(self, item):
         try:
             return SafeReference(self.object.__getitem__(item), self.default)
         except:
             return SafeReference(self.default, self.default)
 
     def __len__(self):
```

### Comparing `dunder_xml_reader-0.0.3/dunder_xml_reader/xml_node.py` & `dunder_xml_reader-0.0.4/dunder_xml_reader/xml_node.py`

 * *Files identical despite different names*

### Comparing `dunder_xml_reader-0.0.3/dunder_xml_reader/xml_node_list.py` & `dunder_xml_reader-0.0.4/dunder_xml_reader/xml_node_list.py`

 * *Files identical despite different names*

### Comparing `dunder_xml_reader-0.0.3/dunder_xml_reader.egg-info/PKG-INFO` & `dunder_xml_reader-0.0.4/dunder_xml_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dunder-xml-reader
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pythonic XML parsing/reading
 Author-email: Steve Brettschneider <steve@bluehousefamily.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -987,15 +987,15 @@
 If your object-graph is wrapped in a SafeReference instance, it will check at each level
 for the requested attribute to be there or missing.  If it's there, it will return the
 requested attribute.  However, if it's not there, it will return a default-value.  Here's
 an example:
 
     >>> cxml = parse_cxml(raw_xml_text_thats_missing_a_BillTo_element)
     >>> safe_cxml = safe_reference(cxml, 'n/a')
-    >>> x = cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    >>> x = safe_cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
     >>> print(x)
     n/a
     >>>
 
 This result of `n/a` will be the result no matter what item is missing (`Request`, `OrderRequest`,
 `OrderRequestHeader`, `BillTo`, etc.) along the way.  If any of the objects in that long
 dereferencing are missing, the default will be returned.  However, if nothing is missing, the
```

### Comparing `dunder_xml_reader-0.0.3/pyproject.toml` & `dunder_xml_reader-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dunder_xml_reader"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Steve Brettschneider", email="steve@bluehousefamily.com" },
 ]
 description = "Pythonic XML parsing/reading"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dunder_xml_reader-0.0.3/test/test_safe_reference.py` & `dunder_xml_reader-0.0.4/test/test_safe_reference.py`

 * *Files 8% similar despite different names*

```diff
@@ -122,8 +122,23 @@
 
 def test_passes_bool_dereference_unsuccessfully_gracefully(sut, mocker):
     # When
     mocker.patch('sys.stderr')
     result = bool(sut.Footer.From.Credential[0].Identity.text())
 
     # Then
-    assert result # Still is True because the default evaluates to True.
+    assert result  # Still is True because the default evaluates to True.
+
+
+def test_iterating_and_indexing_as_array(sut):
+    # Given
+    result = []
+
+    # When
+    for item in sut.Header.To.Credential:
+        result.append(item.identity.text())
+
+    # Then
+    assert result == ['bigadmin@marketplace.org', 'admin@acme.com']
+    assert sut.Header.To.Credential[2] == "isnt-there"  # Doesn't exist in the XML
+
+
```

### Comparing `dunder_xml_reader-0.0.3/test/test_xml_node.py` & `dunder_xml_reader-0.0.4/test/test_xml_node.py`

 * *Files identical despite different names*

### Comparing `dunder_xml_reader-0.0.3/test/test_xml_node_list.py` & `dunder_xml_reader-0.0.4/test/test_xml_node_list.py`

 * *Files identical despite different names*

