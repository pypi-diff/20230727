# Comparing `tmp/dohome_api-0.2.6.tar.gz` & `tmp/dohome_api-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dohome_api-0.2.6.tar", last modified: Sat Feb 11 09:43:11 2023, max compression
+gzip compressed data, was "dohome_api-0.2.7.tar", last modified: Thu Jul 27 21:47:04 2023, max compression
```

## Comparing `dohome_api-0.2.6.tar` & `dohome_api-0.2.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-02-11 09:43:11.749061 dohome_api-0.2.6/
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1072 2023-02-11 09:02:15.000000 dohome_api-0.2.6/LICENSE
--rw-r--r--   0 mishamyrt   (501) staff       (20)      870 2023-02-11 09:43:11.748806 dohome_api-0.2.6/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)      519 2023-02-11 09:02:15.000000 dohome_api-0.2.6/README.md
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-02-11 09:43:11.742580 dohome_api-0.2.6/dohome_api/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      221 2023-02-11 09:31:28.000000 dohome_api-0.2.6/dohome_api/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      722 2023-02-11 09:02:15.000000 dohome_api-0.2.6/dohome_api/commands.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-02-11 09:43:11.744048 dohome_api-0.2.6/dohome_api/gateway/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      106 2023-02-11 09:29:34.000000 dohome_api-0.2.6/dohome_api/gateway/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      130 2023-02-11 09:23:55.000000 dohome_api-0.2.6/dohome_api/gateway/constants.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      134 2023-02-11 09:28:31.000000 dohome_api-0.2.6/dohome_api/gateway/exceptions.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1805 2023-02-11 09:28:56.000000 dohome_api-0.2.6/dohome_api/gateway/gateway.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      561 2023-02-11 09:20:17.000000 dohome_api-0.2.6/dohome_api/gateway/utils.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-02-11 09:43:11.746314 dohome_api-0.2.6/dohome_api/light/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      175 2023-02-11 09:09:28.000000 dohome_api-0.2.6/dohome_api/light/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      269 2023-02-11 09:02:15.000000 dohome_api-0.2.6/dohome_api/light/brightness.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1020 2023-02-11 09:08:15.000000 dohome_api-0.2.6/dohome_api/light/broadcast.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      246 2023-02-11 09:06:56.000000 dohome_api-0.2.6/dohome_api/light/exceptions.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     4178 2023-02-11 09:10:41.000000 dohome_api-0.2.6/dohome_api/light/light.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      426 2023-02-11 09:02:15.000000 dohome_api-0.2.6/dohome_api/light/request.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      693 2023-02-11 09:02:15.000000 dohome_api-0.2.6/dohome_api/light/temperature.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      579 2023-02-11 09:02:15.000000 dohome_api-0.2.6/dohome_api/light/uint8.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-02-11 09:43:11.747490 dohome_api-0.2.6/dohome_api/transport/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      163 2023-02-11 09:02:15.000000 dohome_api-0.2.6/dohome_api/transport/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1626 2023-02-11 09:02:15.000000 dohome_api-0.2.6/dohome_api/transport/broadcast.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      168 2023-02-11 09:02:15.000000 dohome_api-0.2.6/dohome_api/transport/constants.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1080 2023-02-11 09:02:15.000000 dohome_api-0.2.6/dohome_api/transport/direct.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      333 2023-02-11 09:02:15.000000 dohome_api-0.2.6/dohome_api/transport/interface.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      852 2023-02-11 09:02:15.000000 dohome_api-0.2.6/dohome_api/transport/util.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-02-11 09:43:11.748302 dohome_api-0.2.6/dohome_api.egg-info/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      870 2023-02-11 09:43:11.000000 dohome_api-0.2.6/dohome_api.egg-info/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)      884 2023-02-11 09:43:11.000000 dohome_api-0.2.6/dohome_api.egg-info/SOURCES.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2023-02-11 09:43:11.000000 dohome_api-0.2.6/dohome_api.egg-info/dependency_links.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)       33 2023-02-11 09:43:11.000000 dohome_api-0.2.6/dohome_api.egg-info/requires.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)       11 2023-02-11 09:43:11.000000 dohome_api-0.2.6/dohome_api.egg-info/top_level.txt
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-02-11 09:43:11.748453 dohome_api-0.2.6/scripts/
--rwxr-xr-x   0 mishamyrt   (501) staff       (20)     2129 2023-02-11 09:18:35.000000 dohome_api-0.2.6/scripts/dohome_rgb
--rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2023-02-11 09:43:11.749127 dohome_api-0.2.6/setup.cfg
--rw-r--r--   0 mishamyrt   (501) staff       (20)      935 2023-02-11 09:31:48.000000 dohome_api-0.2.6/setup.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-27 21:47:04.459046 dohome_api-0.2.7/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1072 2023-02-11 09:02:15.000000 dohome_api-0.2.7/LICENSE
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      870 2023-07-27 21:47:04.458816 dohome_api-0.2.7/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      519 2023-02-11 09:02:15.000000 dohome_api-0.2.7/README.md
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-27 21:47:04.453905 dohome_api-0.2.7/dohome_api/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      221 2023-02-11 09:31:28.000000 dohome_api-0.2.7/dohome_api/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      722 2023-02-11 09:02:15.000000 dohome_api-0.2.7/dohome_api/commands.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-27 21:47:04.454942 dohome_api-0.2.7/dohome_api/gateway/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      106 2023-02-11 09:29:34.000000 dohome_api-0.2.7/dohome_api/gateway/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      130 2023-02-11 09:23:55.000000 dohome_api-0.2.7/dohome_api/gateway/constants.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      134 2023-02-11 09:28:31.000000 dohome_api-0.2.7/dohome_api/gateway/exceptions.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1805 2023-02-11 09:28:56.000000 dohome_api-0.2.7/dohome_api/gateway/gateway.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      561 2023-02-11 09:20:17.000000 dohome_api-0.2.7/dohome_api/gateway/utils.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-27 21:47:04.456410 dohome_api-0.2.7/dohome_api/light/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      175 2023-02-11 09:09:28.000000 dohome_api-0.2.7/dohome_api/light/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      269 2023-02-11 09:02:15.000000 dohome_api-0.2.7/dohome_api/light/brightness.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1132 2023-07-27 21:46:01.000000 dohome_api-0.2.7/dohome_api/light/broadcast.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      246 2023-02-11 09:06:56.000000 dohome_api-0.2.7/dohome_api/light/exceptions.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     4178 2023-02-11 09:10:41.000000 dohome_api-0.2.7/dohome_api/light/light.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      426 2023-02-11 09:02:15.000000 dohome_api-0.2.7/dohome_api/light/request.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      693 2023-02-11 09:02:15.000000 dohome_api-0.2.7/dohome_api/light/temperature.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      579 2023-02-11 09:02:15.000000 dohome_api-0.2.7/dohome_api/light/uint8.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-27 21:47:04.457647 dohome_api-0.2.7/dohome_api/transport/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      163 2023-02-11 09:02:15.000000 dohome_api-0.2.7/dohome_api/transport/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1626 2023-02-11 09:02:15.000000 dohome_api-0.2.7/dohome_api/transport/broadcast.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      168 2023-02-11 09:02:15.000000 dohome_api-0.2.7/dohome_api/transport/constants.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1080 2023-02-11 09:02:15.000000 dohome_api-0.2.7/dohome_api/transport/direct.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      333 2023-02-11 09:02:15.000000 dohome_api-0.2.7/dohome_api/transport/interface.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      852 2023-02-11 09:02:15.000000 dohome_api-0.2.7/dohome_api/transport/util.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-27 21:47:04.458477 dohome_api-0.2.7/dohome_api.egg-info/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      870 2023-07-27 21:47:04.000000 dohome_api-0.2.7/dohome_api.egg-info/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      884 2023-07-27 21:47:04.000000 dohome_api-0.2.7/dohome_api.egg-info/SOURCES.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2023-07-27 21:47:04.000000 dohome_api-0.2.7/dohome_api.egg-info/dependency_links.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       33 2023-07-27 21:47:04.000000 dohome_api-0.2.7/dohome_api.egg-info/requires.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       11 2023-07-27 21:47:04.000000 dohome_api-0.2.7/dohome_api.egg-info/top_level.txt
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-27 21:47:04.458619 dohome_api-0.2.7/scripts/
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)     2129 2023-02-11 09:18:35.000000 dohome_api-0.2.7/scripts/dohome_rgb
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2023-07-27 21:47:04.459098 dohome_api-0.2.7/setup.cfg
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      935 2023-02-11 09:31:48.000000 dohome_api-0.2.7/setup.py
```

### Comparing `dohome_api-0.2.6/LICENSE` & `dohome_api-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.6/PKG-INFO` & `dohome_api-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dohome_api
-Version: 0.2.6
+Version: 0.2.7
 Summary: Library for controlling smart bulbs that are controlled by the DoIT protocol
 Author: Mikhael Khrustik
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dohome_api-0.2.6/README.md` & `dohome_api-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.6/dohome_api/commands.py` & `dohome_api-0.2.7/dohome_api/commands.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.6/dohome_api/gateway/gateway.py` & `dohome_api-0.2.7/dohome_api/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.6/dohome_api/gateway/utils.py` & `dohome_api-0.2.7/dohome_api/gateway/utils.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.6/dohome_api/light/broadcast.py` & `dohome_api-0.2.7/dohome_api/light/broadcast.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,18 +11,20 @@
     _timeout: float
 
     def __init__(self, sids: List[str], transport: DoHomeBroadcastTransport, timeout = 1.0):
         super().__init__(sids, transport)
         self._sids = sids
         self._timeout = timeout
 
-    async def _send_request(self, request: str):
+    async def _send_request(self, request: str, attempts=5):
         response_data = await self._transport.send_request(
             request, self._timeout, len(self._sids)
         )
         responses = list(map(parse_response, response_data))
         if len(responses) < len(self._sids):
+            if attempts > 0:
+                return await self._send_request(request, attempts - 1)
             raise NotEnoughException
         for response in responses:
             if response["res"] != 0:
                 raise BadCommandException
         return responses[0]
```

### Comparing `dohome_api-0.2.6/dohome_api/light/light.py` & `dohome_api-0.2.7/dohome_api/light/light.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.6/dohome_api/light/temperature.py` & `dohome_api-0.2.7/dohome_api/light/temperature.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.6/dohome_api/light/uint8.py` & `dohome_api-0.2.7/dohome_api/light/uint8.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.6/dohome_api/transport/broadcast.py` & `dohome_api-0.2.7/dohome_api/transport/broadcast.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.6/dohome_api/transport/direct.py` & `dohome_api-0.2.7/dohome_api/transport/direct.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.6/dohome_api/transport/util.py` & `dohome_api-0.2.7/dohome_api/transport/util.py`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.6/dohome_api.egg-info/PKG-INFO` & `dohome_api-0.2.7/dohome_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dohome-api
-Version: 0.2.6
+Version: 0.2.7
 Summary: Library for controlling smart bulbs that are controlled by the DoIT protocol
 Author: Mikhael Khrustik
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dohome_api-0.2.6/dohome_api.egg-info/SOURCES.txt` & `dohome_api-0.2.7/dohome_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.6/scripts/dohome_rgb` & `dohome_api-0.2.7/scripts/dohome_rgb`

 * *Files identical despite different names*

### Comparing `dohome_api-0.2.6/setup.py` & `dohome_api-0.2.7/setup.py`

 * *Files identical despite different names*

