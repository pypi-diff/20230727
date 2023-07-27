# Comparing `tmp/pycasatunes-0.1.2.tar.gz` & `tmp/pycasatunes-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycasatunes-0.1.2.tar", max compression
+gzip compressed data, was "pycasatunes-0.1.3.tar", max compression
```

## Comparing `pycasatunes-0.1.2.tar` & `pycasatunes-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0      722 2021-08-06 22:14:59.626152 pycasatunes-0.1.2/README.md
--rw-r--r--   0        0        0     7827 2021-08-13 15:38:59.320592 pycasatunes-0.1.2/pycasatunes/__init__.py
--rw-r--r--   0        0        0     1678 2021-08-03 10:06:25.973800 pycasatunes-0.1.2/pycasatunes/client.py
--rw-r--r--   0        0        0       43 2021-07-31 11:01:51.627713 pycasatunes-0.1.2/pycasatunes/const.py
--rw-r--r--   0        0        0      106 2021-07-29 20:41:48.191503 pycasatunes-0.1.2/pycasatunes/exceptions.py
--rw-r--r--   0        0        0       25 2021-07-29 20:10:05.414889 pycasatunes-0.1.2/pycasatunes/objects/__init__.py
--rw-r--r--   0        0        0      462 2021-08-09 11:35:08.232599 pycasatunes-0.1.2/pycasatunes/objects/base.py
--rw-r--r--   0        0        0     3242 2021-08-11 07:31:17.138232 pycasatunes-0.1.2/pycasatunes/objects/media.py
--rw-r--r--   0        0        0     7608 2021-08-11 07:31:17.138232 pycasatunes-0.1.2/pycasatunes/objects/nowplaying.py
--rw-r--r--   0        0        0     1000 2021-08-03 18:36:09.216814 pycasatunes-0.1.2/pycasatunes/objects/source.py
--rw-r--r--   0        0        0     3530 2021-08-03 18:17:36.239979 pycasatunes-0.1.2/pycasatunes/objects/system.py
--rw-r--r--   0        0        0     4915 2021-08-11 07:31:17.138232 pycasatunes-0.1.2/pycasatunes/objects/zone.py
--rw-r--r--   0        0        0      735 2021-08-13 15:38:54.704622 pycasatunes-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1443 2021-08-13 15:41:53.779124 pycasatunes-0.1.2/setup.py
--rw-r--r--   0        0        0     1453 2021-08-13 15:41:53.779583 pycasatunes-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      722 2023-05-09 12:08:10.310945 pycasatunes-0.1.3/README.md
+-rw-r--r--   0        0        0     8123 2023-07-27 19:17:54.326603 pycasatunes-0.1.3/pycasatunes/__init__.py
+-rw-r--r--   0        0        0     1678 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/client.py
+-rw-r--r--   0        0        0       43 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/const.py
+-rw-r--r--   0        0        0      106 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/exceptions.py
+-rw-r--r--   0        0        0       25 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/objects/__init__.py
+-rw-r--r--   0        0        0      462 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/objects/base.py
+-rw-r--r--   0        0        0     3242 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/objects/media.py
+-rw-r--r--   0        0        0     7608 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/objects/nowplaying.py
+-rw-r--r--   0        0        0     1000 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/objects/source.py
+-rw-r--r--   0        0        0     3530 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/objects/system.py
+-rw-r--r--   0        0        0     4915 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/objects/zone.py
+-rw-r--r--   0        0        0      735 2023-07-27 19:19:11.106600 pycasatunes-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 pycasatunes-0.1.3/PKG-INFO
```

### Comparing `pycasatunes-0.1.2/README.md` & `pycasatunes-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pycasatunes-0.1.2/pycasatunes/__init__.py` & `pycasatunes-0.1.3/pycasatunes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,22 @@
         """Send player action and option."""
         response = await self._client.get(
             f"http://{self._host}:{API_PORT}/api/v1/zones/{zone_id}?SourceID={source}"
         )
         json = await response.json()
         self.logger.debug(json)
 
+    async def clear_playlist(self, source_id):
+        """Clear playlist on source."""
+        response = await self._client.get(
+            f"http://{self._host}:{API_PORT}/api/v1/sources/{source_id}/queue/delete"
+        )
+        json = await response.json()
+        self.logger.debug(json)
+
     async def player_action(self, zone_id, action, option=""):
         """Send player action and option."""
         response = await self._client.get(
             f"http://{self._host}:{API_PORT}/api/v1/zones/{zone_id}/player/{action}/{option}"
         )
         json = await response.json()
         self.logger.debug(json)
```

### Comparing `pycasatunes-0.1.2/pycasatunes/client.py` & `pycasatunes-0.1.3/pycasatunes/client.py`

 * *Files identical despite different names*

### Comparing `pycasatunes-0.1.2/pycasatunes/objects/media.py` & `pycasatunes-0.1.3/pycasatunes/objects/media.py`

 * *Files identical despite different names*

### Comparing `pycasatunes-0.1.2/pycasatunes/objects/nowplaying.py` & `pycasatunes-0.1.3/pycasatunes/objects/nowplaying.py`

 * *Files identical despite different names*

### Comparing `pycasatunes-0.1.2/pycasatunes/objects/source.py` & `pycasatunes-0.1.3/pycasatunes/objects/source.py`

 * *Files identical despite different names*

### Comparing `pycasatunes-0.1.2/pycasatunes/objects/system.py` & `pycasatunes-0.1.3/pycasatunes/objects/system.py`

 * *Files identical despite different names*

### Comparing `pycasatunes-0.1.2/pycasatunes/objects/zone.py` & `pycasatunes-0.1.3/pycasatunes/objects/zone.py`

 * *Files identical despite different names*

### Comparing `pycasatunes-0.1.2/pyproject.toml` & `pycasatunes-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycasatunes"
-version = "0.1.2"
+version = "0.1.3"
 description = "Asynchronous python client for CasaTunes."
 authors = ["Jon Kristian Nilsen <hello@jonkristian.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jonkristian/pycasatunes"
 repository = "https://github.com/jonkristian/pycasatunes"
 documentation = "https://github.com/jonkristian/pycasatunes"
```

### Comparing `pycasatunes-0.1.2/PKG-INFO` & `pycasatunes-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: pycasatunes
-Version: 0.1.2
+Version: 0.1.3
 Summary: Asynchronous python client for CasaTunes.
 Home-page: https://github.com/jonkristian/pycasatunes
 License: MIT
 Keywords: casatunes,multiroom,api,async,client
 Author: Jon Kristian Nilsen
 Author-email: hello@jonkristian.no
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
 Project-URL: Documentation, https://github.com/jonkristian/pycasatunes
 Project-URL: Repository, https://github.com/jonkristian/pycasatunes
 Description-Content-Type: text/markdown
 
 # PyCasaTunes
```

#### html2text {}

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 2.1 Name: pycasatunes Version: 0.1.2 Summary: Asynchronous
+Metadata-Version: 2.1 Name: pycasatunes Version: 0.1.3 Summary: Asynchronous
 python client for CasaTunes. Home-page: https://github.com/jonkristian/
 pycasatunes License: MIT Keywords: casatunes,multiroom,api,async,client Author:
 Jon Kristian Nilsen Author-email: hello@jonkristian.no Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-Dist: aiohttp
-(>=3.7.4,<4.0.0) Project-URL: Documentation, https://github.com/jonkristian/
-pycasatunes Project-URL: Repository, https://github.com/jonkristian/pycasatunes
-Description-Content-Type: text/markdown # PyCasaTunes Asynchronous python
-client for CasaTunes. This package allows you to interact with CasaTunes API to
-control your home audio. ## Installation ```bash pip install pycasatunes ``` ##
-Attributions - [@timmo001](https://github.com/timmo001) for source of
-inspiration with his [aiolyric package](https://github.com/timmo001/aiolyric).
-- [@ludeeus](https://github.com/ludeeus) for his generator class. # â­ï¸ this
-repository if you found it useful â¤ï¸ [Buy_Me_A_Coffee]
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Dist: aiohttp (>=3.7.4,<4.0.0) Project-URL:
+Documentation, https://github.com/jonkristian/pycasatunes Project-URL:
+Repository, https://github.com/jonkristian/pycasatunes Description-Content-
+Type: text/markdown # PyCasaTunes Asynchronous python client for CasaTunes.
+This package allows you to interact with CasaTunes API to control your home
+audio. ## Installation ```bash pip install pycasatunes ``` ## Attributions -
+[@timmo001](https://github.com/timmo001) for source of inspiration with his
+[aiolyric package](https://github.com/timmo001/aiolyric). - [@ludeeus](https://
+github.com/ludeeus) for his generator class. # â­ï¸ this repository if you
+found it useful â¤ï¸ [Buy_Me_A_Coffee]
```

