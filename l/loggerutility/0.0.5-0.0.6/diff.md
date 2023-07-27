# Comparing `tmp/loggerutility-0.0.5-py3-none-any.whl.zip` & `tmp/loggerutility-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3046 bytes, number of entries: 6
--rw-r--r--  2.0 unx     1801 b- defN 22-Jun-28 11:34 loggerutility/__init__.py
--rw-r--r--  2.0 unx     1073 b- defN 22-Jun-28 11:35 loggerutility-0.0.5.dist-info/LICENCE.txt
--rw-r--r--  2.0 unx      557 b- defN 22-Jun-28 11:35 loggerutility-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jun-28 11:35 loggerutility-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 22-Jun-28 11:35 loggerutility-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      501 b- defN 22-Jun-28 11:35 loggerutility-0.0.5.dist-info/RECORD
-6 files, 4038 bytes uncompressed, 2132 bytes compressed:  47.2%
+Zip file size: 3133 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx     2041 b- defN 23-Jul-27 05:04 loggerutility/__init__.py
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-27 07:32 loggerutility-0.0.6.dist-info/LICENCE.txt
+-rw-rw-r--  2.0 unx      527 b- defN 23-Jul-27 07:32 loggerutility-0.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-27 07:32 loggerutility-0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Jul-27 07:32 loggerutility-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      501 b- defN 23-Jul-27 07:32 loggerutility-0.0.6.dist-info/RECORD
+6 files, 4248 bytes uncompressed, 2219 bytes compressed:  47.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: loggerutility/__init__.py
 Comment: 
 
-Filename: loggerutility-0.0.5.dist-info/LICENCE.txt
+Filename: loggerutility-0.0.6.dist-info/LICENCE.txt
 Comment: 
 
-Filename: loggerutility-0.0.5.dist-info/METADATA
+Filename: loggerutility-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: loggerutility-0.0.5.dist-info/WHEEL
+Filename: loggerutility-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: loggerutility-0.0.5.dist-info/top_level.txt
+Filename: loggerutility-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: loggerutility-0.0.5.dist-info/RECORD
+Filename: loggerutility-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## loggerutility/__init__.py

```diff
@@ -1,13 +1,14 @@
 # Added by Mahesh Saggam on [29-JUNE-21] To print console in a separate log file
 
 import logging
 from logging.handlers import RotatingFileHandler
 # from jproperties import Properties
 import os
+import traceback
 
 dir = 'log'
 
 if not os.path.exists(dir):
     os.makedirs(dir)
 
 for f in os.listdir(dir):
@@ -48,14 +49,20 @@
                     level=logging.DEBUG)
 logger = logging.getLogger(loggerName)
 logHandler = RotatingFileHandler(dir + '/' + filename, maxBytes=int(maxBytes), backupCount=int(backUpcount))
 logger.addHandler(logHandler)
 
 
 def log(msg, debugLevel):
+    stack = traceback.extract_stack()
+    filename, line, functionName, text = stack[-2]
+    index = filename.rfind('/')
+    filename = filename[index + 1:]
+    msg = '~' + filename + '~' + functionName + '~' + msg
+
     if debugLevel.strip() == '':
         debugLevel = 0
     else:
         debugLevel = int(debugLevel)
 
     # to print normal log use debugLvl 1
     if debugLevel == 0:
```

## Comparing `loggerutility-0.0.5.dist-info/LICENCE.txt` & `loggerutility-0.0.6.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `loggerutility-0.0.5.dist-info/METADATA` & `loggerutility-0.0.6.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: loggerutility
-Version: 0.0.5
+Version: 0.0.6
 Summary: Proteus Logger File
-Home-page: UNKNOWN
 Author: Proteus Technology PVT. LTD.
 Author-email: <apps@baseinformation.com>
-License: UNKNOWN
 Keywords: python,first package
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+License-File: LICENCE.txt
 
 Proteus Logger File
-
-
```

