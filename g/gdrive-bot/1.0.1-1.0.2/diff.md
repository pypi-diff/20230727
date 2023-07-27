# Comparing `tmp/gdrive_bot-1.0.1-py3-none-any.whl.zip` & `tmp/gdrive_bot-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6214 bytes, number of entries: 10
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-27 10:13 g_bot/__init__.py
--rw-r--r--  2.0 unx     1925 b- defN 23-Jul-27 10:13 g_bot/cli.py
--rw-r--r--  2.0 unx       68 b- defN 23-Jul-27 10:13 g_bot/config.ini
--rw-r--r--  2.0 unx     6439 b- defN 23-Jul-27 10:13 g_bot/main.py
--rwxr-xr-x  2.0 unx     1064 b- defN 23-Jul-27 10:13 gdrive_bot-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1449 b- defN 23-Jul-27 10:13 gdrive_bot-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 10:13 gdrive_bot-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 23-Jul-27 10:13 gdrive_bot-1.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-27 10:13 gdrive_bot-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      780 b- defN 23-Jul-27 10:13 gdrive_bot-1.0.1.dist-info/RECORD
-10 files, 11886 bytes uncompressed, 4882 bytes compressed:  58.9%
+Zip file size: 6211 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-27 17:39 g_bot/__init__.py
+-rw-r--r--  2.0 unx     1920 b- defN 23-Jul-27 17:39 g_bot/cli.py
+-rw-r--r--  2.0 unx       68 b- defN 23-Jul-27 17:39 g_bot/config.ini
+-rw-r--r--  2.0 unx     6439 b- defN 23-Jul-27 17:39 g_bot/main.py
+-rwxr-xr-x  2.0 unx     1064 b- defN 23-Jul-27 17:39 gdrive_bot-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1449 b- defN 23-Jul-27 17:39 gdrive_bot-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 17:39 gdrive_bot-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 23-Jul-27 17:39 gdrive_bot-1.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-27 17:39 gdrive_bot-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      780 b- defN 23-Jul-27 17:39 gdrive_bot-1.0.2.dist-info/RECORD
+10 files, 11881 bytes uncompressed, 4879 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: g_bot/config.ini
 Comment: 
 
 Filename: g_bot/main.py
 Comment: 
 
-Filename: gdrive_bot-1.0.1.dist-info/LICENSE
+Filename: gdrive_bot-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: gdrive_bot-1.0.1.dist-info/METADATA
+Filename: gdrive_bot-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: gdrive_bot-1.0.1.dist-info/WHEEL
+Filename: gdrive_bot-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: gdrive_bot-1.0.1.dist-info/entry_points.txt
+Filename: gdrive_bot-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: gdrive_bot-1.0.1.dist-info/top_level.txt
+Filename: gdrive_bot-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: gdrive_bot-1.0.1.dist-info/RECORD
+Filename: gdrive_bot-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## g_bot/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.1"
+__version__ = "1.0.2"
```

## g_bot/cli.py

```diff
@@ -45,15 +45,15 @@
 		return setup()
 	elif args.command == "reset":
 		return reset()
 	elif args.command == "up":
 		file_name = os.path.basename(args.filename)
 		return upload_file(access_token, args.filename, file_name, folder_id)
 	elif args.command == "d":
-		file_name = os.path.basename(args.filename)
+		file_name = os.path.basename(args.url)
 		return download(args.url, access_token, folder_id)
 	elif args.version:
 		return print(__version__)
 	else:
 		parser.print_help()
 
 if __name__ == '__main__':
```

## Comparing `gdrive_bot-1.0.1.dist-info/LICENSE` & `gdrive_bot-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gdrive_bot-1.0.1.dist-info/METADATA` & `gdrive_bot-1.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdrive-bot
-Version: 1.0.1
+Version: 1.0.2
 Summary: upload files to gdrive with access token
 Home-page: https://github.com/jakbin/g-bot
 Author: Jak Bin
 Author-email: jakbin4747@gmail.com
 Project-URL: Bug Tracker, https://github.com/jakbin/g-bot/issues
 Keywords: gdrive,g-bot,gdrive-api,gdrive-api-bot,gdrive-file-upload,gdrive-upload
 Classifier: Programming Language :: Python :: 3.6
```

## Comparing `gdrive_bot-1.0.1.dist-info/RECORD` & `gdrive_bot-1.0.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-g_bot/__init__.py,sha256=d4QHYmS_30j0hPN8NmNPnQ_Z0TphDRbu4MtQj9cT9e8,22
-g_bot/cli.py,sha256=E1zRemXtxA7iSUp0VnA5ghYhW8GUvGRxZs8E3uKsixA,1925
+g_bot/__init__.py,sha256=Y3LSfRioSl2xch70pq_ULlvyECXyEtN3krVaWeGyaxk,22
+g_bot/cli.py,sha256=83pn-aweywyI1sZqUfULVMYG3VbEJzp1tuMC-Wpb44I,1920
 g_bot/config.ini,sha256=AE77TZygwBk73SK-f_XKKOMjJnmnJXna4xXkXEe0LbA,68
 g_bot/main.py,sha256=Q2QIxylDXH7RBFRkBmqm3i7qtiS4vrJr5zaKGFVohe0,6439
-gdrive_bot-1.0.1.dist-info/LICENSE,sha256=FZS6Irk3j4oEeg2gqkm72mWWiQf-NkKcqC_6dgE5JlI,1064
-gdrive_bot-1.0.1.dist-info/METADATA,sha256=mTYjDBMf31vxHfP4X0TCLHQQHA0qK4sC7P8hF_RnmKY,1449
-gdrive_bot-1.0.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-gdrive_bot-1.0.1.dist-info/entry_points.txt,sha256=HFOqmBxDrpETW8zsSNBsUYk_Z5Jl7VjlxH1So5HPl1c,41
-gdrive_bot-1.0.1.dist-info/top_level.txt,sha256=SL2B8nDFCT2jvwBhrE6AIE21v1NVC24gKkIejRcDfGo,6
-gdrive_bot-1.0.1.dist-info/RECORD,,
+gdrive_bot-1.0.2.dist-info/LICENSE,sha256=FZS6Irk3j4oEeg2gqkm72mWWiQf-NkKcqC_6dgE5JlI,1064
+gdrive_bot-1.0.2.dist-info/METADATA,sha256=Td4BQ-2U3AOdarRG3eBhVUiHCWv_R6kuxaJbzH2TCsM,1449
+gdrive_bot-1.0.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+gdrive_bot-1.0.2.dist-info/entry_points.txt,sha256=HFOqmBxDrpETW8zsSNBsUYk_Z5Jl7VjlxH1So5HPl1c,41
+gdrive_bot-1.0.2.dist-info/top_level.txt,sha256=SL2B8nDFCT2jvwBhrE6AIE21v1NVC24gKkIejRcDfGo,6
+gdrive_bot-1.0.2.dist-info/RECORD,,
```

