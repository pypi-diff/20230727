# Comparing `tmp/btl-0.9.2-py3-none-any.whl.zip` & `tmp/btl-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 264170 bytes, number of entries: 71
+Zip file size: 264176 bytes, number of entries: 71
 -rw-rw-r--  2.0 unx      100 b- defN 23-Jul-17 13:42 btl/__init__.py
 -rw-rw-r--  2.0 unx     8397 b- defN 23-Jul-27 15:21 btl/cli.py
 -rw-rw-r--  2.0 unx      144 b- defN 23-Jul-22 16:37 btl/const.py
 -rw-rw-r--  2.0 unx     4443 b- defN 23-Jul-23 12:54 btl/db.py
 -rw-rw-r--  2.0 unx     8161 b- defN 23-Jul-25 19:12 btl/fcutil.py
 -rw-rw-r--  2.0 unx     2591 b- defN 23-Jul-23 17:15 btl/library.py
 -rw-rw-r--  2.0 unx     1009 b- defN 23-Jul-25 22:22 btl/params.py
@@ -60,14 +60,14 @@
 -rw-rw-r--  2.0 unx     2090 b- defN 23-Jul-22 20:22 btl/ui/shapeselector.ui
 -rw-rw-r--  2.0 unx      926 b- defN 23-Jul-22 14:37 btl/ui/shapewidget.py
 -rw-rw-r--  2.0 unx     3311 b- defN 23-Jul-23 11:19 btl/ui/tablecell.py
 -rw-rw-r--  2.0 unx     2259 b- defN 23-Jul-25 22:42 btl/ui/tooleditor.py
 -rw-rw-r--  2.0 unx     4553 b- defN 23-Jul-25 22:10 btl/ui/tooleditor.ui
 -rw-rw-r--  2.0 unx     6412 b- defN 23-Jul-25 22:41 btl/ui/toolproperties.py
 -rw-rw-r--  2.0 unx      897 b- defN 23-Jul-22 15:04 btl/ui/util.py
--rw-rw-r--  2.0 unx     1023 b- defN 23-Jul-27 15:24 btl-0.9.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4835 b- defN 23-Jul-27 15:24 btl-0.9.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-27 15:24 btl-0.9.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 23-Jul-27 15:24 btl-0.9.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        4 b- defN 23-Jul-27 15:24 btl-0.9.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5867 b- defN 23-Jul-27 15:24 btl-0.9.2.dist-info/RECORD
-71 files, 715804 bytes uncompressed, 255036 bytes compressed:  64.4%
+-rw-rw-r--  2.0 unx     1023 b- defN 23-Jul-27 15:28 btl-0.9.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4835 b- defN 23-Jul-27 15:28 btl-0.9.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-27 15:28 btl-0.9.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       56 b- defN 23-Jul-27 15:28 btl-0.9.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        4 b- defN 23-Jul-27 15:28 btl-0.9.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5867 b- defN 23-Jul-27 15:28 btl-0.9.3.dist-info/RECORD
+71 files, 715812 bytes uncompressed, 255042 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -189,26 +189,26 @@
 
 Filename: btl/ui/toolproperties.py
 Comment: 
 
 Filename: btl/ui/util.py
 Comment: 
 
-Filename: btl-0.9.2.dist-info/LICENSE
+Filename: btl-0.9.3.dist-info/LICENSE
 Comment: 
 
-Filename: btl-0.9.2.dist-info/METADATA
+Filename: btl-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: btl-0.9.2.dist-info/WHEEL
+Filename: btl-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: btl-0.9.2.dist-info/entry_points.txt
+Filename: btl-0.9.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: btl-0.9.2.dist-info/top_level.txt
+Filename: btl-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: btl-0.9.2.dist-info/RECORD
+Filename: btl-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `btl-0.9.2.dist-info/LICENSE` & `btl-0.9.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `btl-0.9.2.dist-info/METADATA` & `btl-0.9.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btl
-Version: 0.9.2
+Version: 0.9.3
 Summary: A FreeCAD addon and a CLI tool to manage tool libraries
 Author-email: Samuel <knipknap@gmail.com>
 Project-URL: Homepage, https://github.com/knipknap/better-tool-library
 Project-URL: Bug Tracker, https://github.com/knipknap/better-tool-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `btl-0.9.2.dist-info/RECORD` & `btl-0.9.3.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -59,13 +59,13 @@
 btl/ui/shapeselector.ui,sha256=X2fpYceTQVUpxS-pMSBsWwl9VqkeUdWtHQre-YLsKJY,2090
 btl/ui/shapewidget.py,sha256=_5Fcl0UzKNanrvkjLSYIwVoxkJIzwMm4N5GT1JYShlA,926
 btl/ui/tablecell.py,sha256=fMd_hzOgEWsu5oyk5VSNGB8wyuA_rNUBdksYgxQR28A,3311
 btl/ui/tooleditor.py,sha256=A-oRi-Bul6ME9Zh9KwNkdDP73Pt7K1S18GCVQM1K9YU,2259
 btl/ui/tooleditor.ui,sha256=JQewVoEwb_Cl-5FljuTP1gWssRBjHFisQn9SGWuwmBo,4553
 btl/ui/toolproperties.py,sha256=TaXmT9L12N18uLZXttgCqxjP7ugOHqKQCmJ7NxsETfE,6412
 btl/ui/util.py,sha256=DZbp95leRgq2uqyxTtnUY6K5NsFLXK8nHkcEJhD7v6s,897
-btl-0.9.2.dist-info/LICENSE,sha256=-cTHe6o4KABO5UuKTy2y6I7USmI3pJOWW_VR-sD8ti0,1023
-btl-0.9.2.dist-info/METADATA,sha256=sErt2DrU3GzuSdEzDxvc0UEWuld3HtRgyhDNXhzISgo,4835
-btl-0.9.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-btl-0.9.2.dist-info/entry_points.txt,sha256=tQ0tCWonotZ_v25QGH7onkUnniMxBwMPhCmtSWG3ENQ,48
-btl-0.9.2.dist-info/top_level.txt,sha256=ag8f5JjCBHkwl5n2_yIRBcsSCa0qLVqjd2w_lnvRM8E,4
-btl-0.9.2.dist-info/RECORD,,
+btl-0.9.3.dist-info/LICENSE,sha256=-cTHe6o4KABO5UuKTy2y6I7USmI3pJOWW_VR-sD8ti0,1023
+btl-0.9.3.dist-info/METADATA,sha256=5kXkqkEnKWVI1uqwYZe8xPObJDCUx_QhvswNDoxpxEI,4835
+btl-0.9.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+btl-0.9.3.dist-info/entry_points.txt,sha256=M7a2KDVjWO35s7PtD6lLjfpZrjnSDBT8THOhFCX4w6U,56
+btl-0.9.3.dist-info/top_level.txt,sha256=ag8f5JjCBHkwl5n2_yIRBcsSCa0qLVqjd2w_lnvRM8E,4
+btl-0.9.3.dist-info/RECORD,,
```

