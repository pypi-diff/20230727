# Comparing `tmp/reverseshellserver-0.10.tar.gz` & `tmp/reverseshellserver-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reverseshellserver-0.10.tar", last modified: Mon Jul 24 06:07:47 2023, max compression
+gzip compressed data, was "reverseshellserver-0.11.tar", last modified: Wed Jul 26 23:18:52 2023, max compression
```

## Comparing `reverseshellserver-0.10.tar` & `reverseshellserver-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 06:07:47.586408 reverseshellserver-0.10/
--rw-rw-rw-   0        0        0     1148 2023-07-24 06:07:32.000000 reverseshellserver-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      125 2023-07-24 06:07:28.000000 reverseshellserver-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     2824 2023-07-24 06:07:47.586408 reverseshellserver-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     2130 2023-07-24 05:56:20.000000 reverseshellserver-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 06:07:47.581560 reverseshellserver-0.10/reverseshellserver/
--rw-rw-rw-   0        0        0     2130 2023-07-24 05:56:20.000000 reverseshellserver-0.10/reverseshellserver/README.MD
--rw-rw-rw-   0        0        0    13230 2023-07-24 05:57:08.000000 reverseshellserver-0.10/reverseshellserver/__init__.py
--rw-rw-rw-   0        0        0       75 2023-07-24 06:07:46.000000 reverseshellserver-0.10/reverseshellserver/requirements.txt
--rw-rw-rw-   0        0        0   176029 2023-07-24 06:07:46.000000 reverseshellserver-0.10/reverseshellserver/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-24 06:07:47.585435 reverseshellserver-0.10/reverseshellserver.egg-info/
--rw-rw-rw-   0        0        0     2824 2023-07-24 06:07:47.000000 reverseshellserver-0.10/reverseshellserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-07-24 06:07:47.000000 reverseshellserver-0.10/reverseshellserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 06:07:47.000000 reverseshellserver-0.10/reverseshellserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-07-24 06:07:47.000000 reverseshellserver-0.10/reverseshellserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-24 06:07:47.000000 reverseshellserver-0.10/reverseshellserver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-24 06:07:47.587383 reverseshellserver-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1507 2023-07-24 06:07:46.000000 reverseshellserver-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:18:52.576121 reverseshellserver-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-07-26 23:18:43.000000 reverseshellserver-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      125 2023-07-26 23:18:40.000000 reverseshellserver-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     2824 2023-07-26 23:18:52.577097 reverseshellserver-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2130 2023-07-24 06:13:36.000000 reverseshellserver-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 23:18:52.571240 reverseshellserver-0.11/reverseshellserver/
+-rw-rw-rw-   0        0        0     2130 2023-07-24 06:13:36.000000 reverseshellserver-0.11/reverseshellserver/README.MD
+-rw-rw-rw-   0        0        0    13337 2023-07-26 21:44:30.000000 reverseshellserver-0.11/reverseshellserver/__init__.py
+-rw-rw-rw-   0        0        0       75 2023-07-26 23:18:51.000000 reverseshellserver-0.11/reverseshellserver/requirements.txt
+-rw-rw-rw-   0        0        0   176029 2023-07-26 23:18:51.000000 reverseshellserver-0.11/reverseshellserver/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-26 23:18:52.576121 reverseshellserver-0.11/reverseshellserver.egg-info/
+-rw-rw-rw-   0        0        0     2824 2023-07-26 23:18:52.000000 reverseshellserver-0.11/reverseshellserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-07-26 23:18:52.000000 reverseshellserver-0.11/reverseshellserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 23:18:52.000000 reverseshellserver-0.11/reverseshellserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-26 23:18:52.000000 reverseshellserver-0.11/reverseshellserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-26 23:18:52.000000 reverseshellserver-0.11/reverseshellserver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-26 23:18:52.579050 reverseshellserver-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1507 2023-07-26 23:18:51.000000 reverseshellserver-0.11/setup.py
```

### Comparing `reverseshellserver-0.10/LICENSE.rst` & `reverseshellserver-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `reverseshellserver-0.10/PKG-INFO` & `reverseshellserver-0.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reverseshellserver
-Version: 0.10
+Version: 0.11
 Summary: Reverse shell SERVER for unbureaucratic server/client connections with file transfer / screenshots
 Home-page: https://github.com/hansalemaos/reverseshellserver
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: network,reverse,shell
 Classifier: Development Status :: 4 - Beta
```

### Comparing `reverseshellserver-0.10/README.md` & `reverseshellserver-0.11/README.md`

 * *Files identical despite different names*

### Comparing `reverseshellserver-0.10/reverseshellserver/README.MD` & `reverseshellserver-0.11/reverseshellserver/README.MD`

 * *Files identical despite different names*

### Comparing `reverseshellserver-0.10/reverseshellserver/__init__.py` & `reverseshellserver-0.11/reverseshellserver/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,16 @@
             cmd_encoded = cmd.encode("utf-8")
         cmd_encoded = encode_cmd(
             cmd_encoded=cmd_encoded,
             byte_len=byte_len,
             command_start=command_start,
             command_end=command_end,
         )
-        client_socket.send(cmd_encoded)
+        for datatosend in [cmd_encoded[i:i + byte_len] for i in range(0, len(cmd_encoded), byte_len)]:
+            client_socket.send(datatosend)
         response_from_client = b""
         while command_end not in response_from_client:
             response_from_client += client_socket.recv(byte_len)
         response_from_client = response_from_client.split(command_start, maxsplit=1)[
             1
         ].split(command_end, maxsplit=1)[0]
         if cmd == command_screenshot:
```

### Comparing `reverseshellserver-0.10/reverseshellserver/thirdparty.json` & `reverseshellserver-0.11/reverseshellserver/thirdparty.json`

 * *Files identical despite different names*

### Comparing `reverseshellserver-0.10/reverseshellserver.egg-info/PKG-INFO` & `reverseshellserver-0.11/reverseshellserver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reverseshellserver
-Version: 0.10
+Version: 0.11
 Summary: Reverse shell SERVER for unbureaucratic server/client connections with file transfer / screenshots
 Home-page: https://github.com/hansalemaos/reverseshellserver
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: network,reverse,shell
 Classifier: Development Status :: 4 - Beta
```

### Comparing `reverseshellserver-0.10/setup.py` & `reverseshellserver-0.11/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Reverse shell SERVER for unbureaucratic server/client connections with file transfer / screenshots'''
 
 # Setting up
 setup(
     name="reverseshellserver",
     version=VERSION,
     license='MIT',
```

