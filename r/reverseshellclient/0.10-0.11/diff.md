# Comparing `tmp/reverseshellclient-0.10.tar.gz` & `tmp/reverseshellclient-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reverseshellclient-0.10.tar", last modified: Mon Jul 24 06:08:59 2023, max compression
+gzip compressed data, was "reverseshellclient-0.11.tar", last modified: Wed Jul 26 23:21:12 2023, max compression
```

## Comparing `reverseshellclient-0.10.tar` & `reverseshellclient-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 06:08:59.938480 reverseshellclient-0.10/
--rw-rw-rw-   0        0        0     1148 2023-07-24 06:08:55.000000 reverseshellclient-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      125 2023-07-24 06:08:54.000000 reverseshellclient-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     3663 2023-07-24 06:08:59.938480 reverseshellclient-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     2969 2023-07-24 06:03:47.000000 reverseshellclient-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 06:08:59.934576 reverseshellclient-0.10/reverseshellclient/
--rw-rw-rw-   0        0        0     2969 2023-07-24 06:03:47.000000 reverseshellclient-0.10/reverseshellclient/README.MD
--rw-rw-rw-   0        0        0     7226 2023-07-24 05:59:55.000000 reverseshellclient-0.10/reverseshellclient/__init__.py
--rw-rw-rw-   0        0        0        3 2023-07-24 06:08:59.000000 reverseshellclient-0.10/reverseshellclient/requirements.txt
--rw-rw-rw-   0        0        0       82 2023-07-24 06:08:59.000000 reverseshellclient-0.10/reverseshellclient/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-24 06:08:59.937504 reverseshellclient-0.10/reverseshellclient.egg-info/
--rw-rw-rw-   0        0        0     3663 2023-07-24 06:08:59.000000 reverseshellclient-0.10/reverseshellclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-07-24 06:08:59.000000 reverseshellclient-0.10/reverseshellclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 06:08:59.000000 reverseshellclient-0.10/reverseshellclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-24 06:08:59.000000 reverseshellclient-0.10/reverseshellclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-24 06:08:59.000000 reverseshellclient-0.10/reverseshellclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-24 06:08:59.939457 reverseshellclient-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1343 2023-07-24 06:08:59.000000 reverseshellclient-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:21:12.937385 reverseshellclient-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-07-26 23:21:05.000000 reverseshellclient-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      125 2023-07-26 23:21:03.000000 reverseshellclient-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     3663 2023-07-26 23:21:12.937385 reverseshellclient-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2969 2023-07-24 06:13:36.000000 reverseshellclient-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 23:21:12.933481 reverseshellclient-0.11/reverseshellclient/
+-rw-rw-rw-   0        0        0     2969 2023-07-24 06:13:36.000000 reverseshellclient-0.11/reverseshellclient/README.MD
+-rw-rw-rw-   0        0        0     7444 2023-07-26 21:42:11.000000 reverseshellclient-0.11/reverseshellclient/__init__.py
+-rw-rw-rw-   0        0        0        3 2023-07-26 23:21:12.000000 reverseshellclient-0.11/reverseshellclient/requirements.txt
+-rw-rw-rw-   0        0        0       82 2023-07-26 23:21:12.000000 reverseshellclient-0.11/reverseshellclient/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-26 23:21:12.937385 reverseshellclient-0.11/reverseshellclient.egg-info/
+-rw-rw-rw-   0        0        0     3663 2023-07-26 23:21:12.000000 reverseshellclient-0.11/reverseshellclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-07-26 23:21:12.000000 reverseshellclient-0.11/reverseshellclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 23:21:12.000000 reverseshellclient-0.11/reverseshellclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-26 23:21:12.000000 reverseshellclient-0.11/reverseshellclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-26 23:21:12.000000 reverseshellclient-0.11/reverseshellclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-26 23:21:12.939337 reverseshellclient-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1343 2023-07-26 23:21:12.000000 reverseshellclient-0.11/setup.py
```

### Comparing `reverseshellclient-0.10/LICENSE.rst` & `reverseshellclient-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `reverseshellclient-0.10/PKG-INFO` & `reverseshellclient-0.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reverseshellclient
-Version: 0.10
+Version: 0.11
 Summary: Reverse shell CLIENT for unbureaucratic server/client connections with file transfer / screenshots
 Home-page: https://github.com/hansalemaos/reverseshellclient
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: network,reverse,shell
 Classifier: Development Status :: 4 - Beta
```

### Comparing `reverseshellclient-0.10/README.md` & `reverseshellclient-0.11/README.md`

 * *Files identical despite different names*

### Comparing `reverseshellclient-0.10/reverseshellclient/README.MD` & `reverseshellclient-0.11/reverseshellclient/README.MD`

 * *Files identical despite different names*

### Comparing `reverseshellclient-0.10/reverseshellclient/__init__.py` & `reverseshellclient-0.11/reverseshellclient/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,16 +102,17 @@
                 path = path.decode("utf-8", "ignore")
                 print(
                     f"Received command: {putfilecommand.decode('utf-8', 'ignore')}{path}"
                 )
                 with open(path, mode="wb") as f:
                     f.write(filecontent)
                 abspath = os.path.normpath(os.path.join(os.getcwd(), path))
-                datatosend = encode_cmd(abspath, byte_len, command_start, command_end)
-                client_socket.send(datatosend)
+                allblocks = encode_cmd(abspath, byte_len, command_start, command_end)
+                for datatosend in [allblocks[i:i + byte_len] for i in range(0, len(allblocks), byte_len)]:
+                    client_socket.send(datatosend)
                 continue
             command = command.decode("utf-8")
             print(f"Received command: {command}")
             if command == command_screenshot:
                 with mss.mss() as sct:
                     img = sct.grab(sct.monitors[0])
                     datatosend = pickle.dumps(img)
@@ -131,16 +132,17 @@
                 p = subprocess.run(
                     command,
                     shell=True,
                     stderr=subprocess.PIPE,
                     stdout=subprocess.PIPE,
                 )
                 datatosend = before_stdout + p.stdout + before_stderr + p.stderr
-            datatosend = encode_cmd(datatosend, byte_len, command_start, command_end)
-            client_socket.send(datatosend)
+            allblocks = encode_cmd(datatosend, byte_len, command_start, command_end)
+            for datatosend in [allblocks[i:i + byte_len] for i in range(0, len(allblocks), byte_len)]:
+                client_socket.send(datatosend)
         except Exception as fe:
             datatosend = str(fe).encode("utf-8")
             datatosend = encode_cmd(datatosend, byte_len, command_start, command_end)
             client_socket.send(datatosend)
             continue
         except KeyboardInterrupt:
             client_socket.close()
```

### Comparing `reverseshellclient-0.10/reverseshellclient.egg-info/PKG-INFO` & `reverseshellclient-0.11/reverseshellclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reverseshellclient
-Version: 0.10
+Version: 0.11
 Summary: Reverse shell CLIENT for unbureaucratic server/client connections with file transfer / screenshots
 Home-page: https://github.com/hansalemaos/reverseshellclient
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: network,reverse,shell
 Classifier: Development Status :: 4 - Beta
```

### Comparing `reverseshellclient-0.10/setup.py` & `reverseshellclient-0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Reverse shell CLIENT for unbureaucratic server/client connections with file transfer / screenshots'''
 
 # Setting up
 setup(
     name="reverseshellclient",
     version=VERSION,
     license='MIT',
```

