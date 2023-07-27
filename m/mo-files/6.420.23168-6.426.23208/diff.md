# Comparing `tmp/mo_files-6.420.23168-py2.py3-none-any.whl.zip` & `tmp/mo_files-6.426.23208-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 15850 bytes, number of entries: 8
+Zip file size: 15859 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat    18787 b- defN 23-May-30 12:09 mo_files/__init__.py
 -rw-rw-rw-  2.0 fat      197 b- defN 22-Dec-05 22:50 mo_files/mimetype.py
 -rw-rw-rw-  2.0 fat    11814 b- defN 23-Apr-30 18:14 mo_files/url.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-17 11:20 mo_files-6.420.23168.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1603 b- defN 23-Jun-17 11:20 mo_files-6.420.23168.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-17 11:20 mo_files-6.420.23168.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-17 11:20 mo_files-6.420.23168.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      649 b- defN 23-Jun-17 11:20 mo_files-6.420.23168.dist-info/RECORD
-8 files, 49894 bytes uncompressed, 14722 bytes compressed:  70.5%
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Jul-27 02:15 mo_files-6.426.23208.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1603 b- defN 23-Jul-27 02:15 mo_files-6.426.23208.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-27 02:15 mo_files-6.426.23208.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-27 02:15 mo_files-6.426.23208.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      649 b- defN 23-Jul-27 02:15 mo_files-6.426.23208.dist-info/RECORD
+8 files, 49894 bytes uncompressed, 14731 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: mo_files/mimetype.py
 Comment: 
 
 Filename: mo_files/url.py
 Comment: 
 
-Filename: mo_files-6.420.23168.dist-info/LICENSE
+Filename: mo_files-6.426.23208.dist-info/LICENSE
 Comment: 
 
-Filename: mo_files-6.420.23168.dist-info/METADATA
+Filename: mo_files-6.426.23208.dist-info/METADATA
 Comment: 
 
-Filename: mo_files-6.420.23168.dist-info/WHEEL
+Filename: mo_files-6.426.23208.dist-info/WHEEL
 Comment: 
 
-Filename: mo_files-6.420.23168.dist-info/top_level.txt
+Filename: mo_files-6.426.23208.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_files-6.420.23168.dist-info/RECORD
+Filename: mo_files-6.426.23208.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mo_files-6.420.23168.dist-info/LICENSE` & `mo_files-6.426.23208.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_files-6.420.23168.dist-info/METADATA` & `mo_files-6.426.23208.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-files
-Version: 6.420.23168
+Version: 6.426.23208
 Summary: More Files! Steamlined for UTF8 and JSON.
 Home-page: https://github.com/klahnakoski/mo-files
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
@@ -14,16 +14,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mo-dots (==9.417.23168)
 Requires-Dist: mo-future (==7.416.23168)
-Requires-Dist: mo-json (==6.420.23168)
-Requires-Dist: mo-logs (==8.417.23168)
+Requires-Dist: mo-json (==6.425.23207)
+Requires-Dist: mo-logs (==8.425.23207)
 Requires-Dist: mo-math (==7.417.23168)
 Provides-Extra: tests
 Requires-Dist: mo-testing ; extra == 'tests'
 
 # More Files!
 
 The `File` class makes the default assumption all files have cr-delimited unicode content that is UTF-8 encoded. This is great for JSON files. It also provides better operators over some common file manipulations.
```

