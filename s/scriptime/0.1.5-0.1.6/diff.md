# Comparing `tmp/scriptime-0.1.5.tar.gz` & `tmp/scriptime-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptime-0.1.5.tar", last modified: Sun Jul  9 02:59:46 2023, max compression
+gzip compressed data, was "scriptime-0.1.6.tar", last modified: Thu Jul 27 19:23:01 2023, max compression
```

## Comparing `scriptime-0.1.5.tar` & `scriptime-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-09 02:59:46.252062 scriptime-0.1.5/
--rw-r--r--   0 jakestrasler   (501) staff       (20)     1087 2023-07-09 02:56:28.000000 scriptime-0.1.5/LICENSE
--rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 20:17:09.000000 scriptime-0.1.5/MANIFEST.in
--rw-r--r--   0 jakestrasler   (501) staff       (20)     5401 2023-07-09 02:59:46.251898 scriptime-0.1.5/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)     5091 2023-07-09 02:59:26.000000 scriptime-0.1.5/README.md
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-09 02:59:46.250315 scriptime-0.1.5/scriptime/
--rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-0.1.5/scriptime/__init__.py
--rw-r--r--   0 jakestrasler   (501) staff       (20)   701148 2023-07-05 22:10:39.000000 scriptime-0.1.5/scriptime/alert.wav
--rw-r--r--   0 jakestrasler   (501) staff       (20)     9874 2023-07-06 19:55:45.000000 scriptime-0.1.5/scriptime/main.py
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-09 02:59:46.251640 scriptime-0.1.5/scriptime.egg-info/
--rw-r--r--   0 jakestrasler   (501) staff       (20)     5401 2023-07-09 02:59:46.000000 scriptime-0.1.5/scriptime.egg-info/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)      262 2023-07-09 02:59:46.000000 scriptime-0.1.5/scriptime.egg-info/SOURCES.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-09 02:59:46.000000 scriptime-0.1.5/scriptime.egg-info/dependency_links.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       30 2023-07-09 02:59:46.000000 scriptime-0.1.5/scriptime.egg-info/requires.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-09 02:59:46.000000 scriptime-0.1.5/scriptime.egg-info/top_level.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-09 02:59:46.252110 scriptime-0.1.5/setup.cfg
--rw-r--r--   0 jakestrasler   (501) staff       (20)      694 2023-07-09 02:59:44.000000 scriptime-0.1.5/setup.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-27 19:23:01.201021 scriptime-0.1.6/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     1087 2023-07-09 02:56:28.000000 scriptime-0.1.6/LICENSE
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 20:17:09.000000 scriptime-0.1.6/MANIFEST.in
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     5401 2023-07-27 19:23:01.200884 scriptime-0.1.6/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     5091 2023-07-09 02:59:26.000000 scriptime-0.1.6/README.md
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-27 19:23:01.199858 scriptime-0.1.6/scriptime/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-0.1.6/scriptime/__init__.py
+-rw-r--r--   0 jakestrasler   (501) staff       (20)   701148 2023-07-05 22:10:39.000000 scriptime-0.1.6/scriptime/alert.wav
+-rw-r--r--   0 jakestrasler   (501) staff       (20)    10004 2023-07-27 19:21:26.000000 scriptime-0.1.6/scriptime/main.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-27 19:23:01.200652 scriptime-0.1.6/scriptime.egg-info/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     5401 2023-07-27 19:23:01.000000 scriptime-0.1.6/scriptime.egg-info/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      262 2023-07-27 19:23:01.000000 scriptime-0.1.6/scriptime.egg-info/SOURCES.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-27 19:23:01.000000 scriptime-0.1.6/scriptime.egg-info/dependency_links.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       30 2023-07-27 19:23:01.000000 scriptime-0.1.6/scriptime.egg-info/requires.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-27 19:23:01.000000 scriptime-0.1.6/scriptime.egg-info/top_level.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-27 19:23:01.201061 scriptime-0.1.6/setup.cfg
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      694 2023-07-27 19:22:59.000000 scriptime-0.1.6/setup.py
```

### Comparing `scriptime-0.1.5/LICENSE` & `scriptime-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scriptime-0.1.5/PKG-INFO` & `scriptime-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scriptime
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.
 Author: Jake Strasler
 Author-email: jstr36@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scriptime
```

### Comparing `scriptime-0.1.5/README.md` & `scriptime-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `scriptime-0.1.5/scriptime/alert.wav` & `scriptime-0.1.6/scriptime/alert.wav`

 * *Files identical despite different names*

### Comparing `scriptime-0.1.5/scriptime/main.py` & `scriptime-0.1.6/scriptime/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import json
 import os
 import platform
 import smtplib
 import sys
 import time
 from typing import Optional, Union
@@ -64,15 +65,17 @@
             - SMTP SSL server for sender email. If `method` is set to `"hardcode"`, then the sender email SMTP SSL server must be passed in as a string. Find your email server at: https://www.arclab.com/en/kb/email/list-of-smtp-and-pop3-servers-mailserver-list.html
         - `port`: int (optional)
             - SMTP SSL port for sender email. If `method` is set to `"hardcode"`, then the sender email SMTP SSL email port must be passed in as a string. Find your email port at: https://www.arclab.com/en/kb/email/list-of-smtp-and-pop3-servers-mailserver-list.html
         """
         current_time = time.localtime()
         formatted_time = time.strftime("%m-%d-%Y %H:%M:%S", current_time)
 
-        file_name = os.path.basename(__file__)
+        caller_frame = inspect.stack()[1]
+        caller_module = inspect.getmodule(caller_frame[0])
+        file_name = os.path.basename(caller_module.__file__)
 
         self.descriptor = f"[{formatted_time}] {file_name} Finished"
         self.sender_email = None
         self.sender_password = None
 
         if method == "json":
             # load passwords through json
```

### Comparing `scriptime-0.1.5/scriptime.egg-info/PKG-INFO` & `scriptime-0.1.6/scriptime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scriptime
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.
 Author: Jake Strasler
 Author-email: jstr36@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scriptime
```

### Comparing `scriptime-0.1.5/setup.py` & `scriptime-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="scriptime",
-    version="0.1.5",
+    version="0.1.6",
     author="Jake Strasler",
     author_email="jstr36@gmail.com",
     description="A Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["scriptime"],
     package_data={"scriptime": ["scriptime/alert.wav"]},
```

