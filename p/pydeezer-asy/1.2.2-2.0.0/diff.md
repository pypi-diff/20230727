# Comparing `tmp/pydeezer_asy-1.2.2.tar.gz` & `tmp/pydeezer_asy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeezer_asy-1.2.2.tar", last modified: Thu Jul 20 19:35:58 2023, max compression
+gzip compressed data, was "pydeezer_asy-2.0.0.tar", last modified: Thu Jul 27 20:50:38 2023, max compression
```

## Comparing `pydeezer_asy-1.2.2.tar` & `pydeezer_asy-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 19:35:58.542185 pydeezer_asy-1.2.2/
--rw-rw-rw-   0        0        0     1662 2023-07-20 19:35:58.541195 pydeezer_asy-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1298 2023-07-12 12:53:05.000000 pydeezer_asy-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 19:35:58.464397 pydeezer_asy-1.2.2/deezer_asy/
--rw-rw-rw-   0        0        0    32057 2023-07-20 19:35:28.000000 pydeezer_asy-1.2.2/deezer_asy/DeezerAsy.py
--rw-rw-rw-   0        0        0      134 2023-07-07 16:55:48.000000 pydeezer_asy-1.2.2/deezer_asy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:35:58.486338 pydeezer_asy-1.2.2/deezer_asy/constants/
--rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/constants/__init__.py
--rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/constants/api_methods.py
--rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/constants/api_urls.py
--rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/constants/image_hosts.py
--rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/constants/networking_settings.py
--rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/constants/search_types.py
--rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/constants/track_formats.py
--rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.2/deezer_asy/exceptions.py
--rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-1.2.2/deezer_asy/util.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:35:58.539193 pydeezer_asy-1.2.2/pydeezer_asy.egg-info/
--rw-rw-rw-   0        0        0     1662 2023-07-20 19:35:58.000000 pydeezer_asy-1.2.2/pydeezer_asy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-07-20 19:35:58.000000 pydeezer_asy-1.2.2/pydeezer_asy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 19:35:58.000000 pydeezer_asy-1.2.2/pydeezer_asy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-20 19:35:58.000000 pydeezer_asy-1.2.2/pydeezer_asy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-20 19:35:58.000000 pydeezer_asy-1.2.2/pydeezer_asy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 19:35:58.543183 pydeezer_asy-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      749 2023-07-20 19:35:42.000000 pydeezer_asy-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:50:38.519834 pydeezer_asy-2.0.0/
+-rw-rw-rw-   0        0        0     1910 2023-07-27 20:50:38.516847 pydeezer_asy-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1546 2023-07-27 20:49:08.000000 pydeezer_asy-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 20:50:38.449600 pydeezer_asy-2.0.0/deezer_asy/
+-rw-rw-rw-   0        0        0    28680 2023-07-27 20:40:18.000000 pydeezer_asy-2.0.0/deezer_asy/DeezerAsy.py
+-rw-rw-rw-   0        0        0      136 2023-07-27 18:53:44.000000 pydeezer_asy-2.0.0/deezer_asy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:50:38.466551 pydeezer_asy-2.0.0/deezer_asy/constants/
+-rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/constants/__init__.py
+-rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/constants/api_methods.py
+-rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/constants/api_urls.py
+-rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/constants/image_hosts.py
+-rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/constants/networking_settings.py
+-rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/constants/search_types.py
+-rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/constants/track_formats.py
+-rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/exceptions.py
+-rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-2.0.0/deezer_asy/util.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:50:38.510860 pydeezer_asy-2.0.0/pydeezer_asy.egg-info/
+-rw-rw-rw-   0        0        0     1910 2023-07-27 20:50:38.000000 pydeezer_asy-2.0.0/pydeezer_asy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2023-07-27 20:50:38.000000 pydeezer_asy-2.0.0/pydeezer_asy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 20:50:38.000000 pydeezer_asy-2.0.0/pydeezer_asy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-27 20:50:38.000000 pydeezer_asy-2.0.0/pydeezer_asy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 20:50:38.000000 pydeezer_asy-2.0.0/pydeezer_asy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 20:50:38.519834 pydeezer_asy-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-07-27 20:50:26.000000 pydeezer_asy-2.0.0/setup.py
```

### Comparing `pydeezer_asy-1.2.2/PKG-INFO` & `pydeezer_asy-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: pydeezer_asy
-Version: 1.2.2
+Version: 2.0.0
 Summary: Asynchronous version of the `py-deezer` module
 Home-page: https://github.com/drhspfn/deezer-asy
 Author: drhspfn
 Author-email: drhspfn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # deezer-asy
 Asynchronous version of the [py-deezer](https://github.com/acgonzales/pydeezer) module
-
-
 At the moment, the functionality does not completely repeat the original library
 
-
-# Differences
+### Differences
 This version is asynchronous. Otherwise, it repeats the arguments of the original library.
 
-All that differs is initialization. You need to create a session that will get some information from your ARL, 
-`await deezer._generate_main_session()` is responsible for this. 
 
-It must be called when you start your application, in `on_startup` in your bot, or otherwise
+# Last update `2.0.0`
+    * Simplified module initialization
+    * Changed response type of `download_track` function: {'track': path, 'lyric': path or None}
+    
 
 
 # What works?
-* Getting information about albums, tracks (their tags).
+* Getting information about albums, playlists, artists, tracks (their tags).
 * Downloading tracks.
 
 
 # What needs to be done
 * Adding tags to .flac. `(So вЂ‹вЂ‹far, idling)`
 
 # Installation
@@ -39,23 +37,32 @@
 ```
 
 # Usage as a package
 
 ```python
 from deezer_asy import DeezerAsy
 import asyncio
+import logging
 
+logging.basicConfig(
+    level=logging.INFO,  
+    format="%(asctime)s [%(levelname)s] %(message)s",
+    datefmt="%Y-%m-%d %H:%M:%S"
+)
+logger = logging.getLogger("main_logger")
+loop = asyncio.get_event_loop()
 ARL = "edit this"
 
 async def main():
-    deezer = DeezerAsy(ARL)
+    # You can pass `loop` as an argument, or leave None
+    # If you want logging, pass the `logger` as an argument
+    deezer = DeezerAsy(ARL, loop=loop, logger=logger)
     await deezer._generate_main_session()
     track = await deezer.get_track(1421388612, True)
     data = await deezer.download_track(track['info'], './', with_lyrics=True, with_metadata=True)
     print(data)
 
 
 
 if __name__ == "__main__":
-    loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
 ```
```

### Comparing `pydeezer_asy-1.2.2/README.md` & `pydeezer_asy-2.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # deezer-asy
 Asynchronous version of the [py-deezer](https://github.com/acgonzales/pydeezer) module
-
-
 At the moment, the functionality does not completely repeat the original library
 
-
-# Differences
+### Differences
 This version is asynchronous. Otherwise, it repeats the arguments of the original library.
 
-All that differs is initialization. You need to create a session that will get some information from your ARL, 
-`await deezer._generate_main_session()` is responsible for this. 
 
-It must be called when you start your application, in `on_startup` in your bot, or otherwise
+# Last update `2.0.0`
+    * Simplified module initialization
+    * Changed response type of `download_track` function: {'track': path, 'lyric': path or None}
+    
 
 
 # What works?
-* Getting information about albums, tracks (their tags).
+* Getting information about albums, playlists, artists, tracks (their tags).
 * Downloading tracks.
 
 
 # What needs to be done
 * Adding tags to .flac. `(So ​​far, idling)`
 
 # Installation
@@ -28,23 +26,32 @@
 ```
 
 # Usage as a package
 
 ```python
 from deezer_asy import DeezerAsy
 import asyncio
+import logging
 
+logging.basicConfig(
+    level=logging.INFO,  
+    format="%(asctime)s [%(levelname)s] %(message)s",
+    datefmt="%Y-%m-%d %H:%M:%S"
+)
+logger = logging.getLogger("main_logger")
+loop = asyncio.get_event_loop()
 ARL = "edit this"
 
 async def main():
-    deezer = DeezerAsy(ARL)
+    # You can pass `loop` as an argument, or leave None
+    # If you want logging, pass the `logger` as an argument
+    deezer = DeezerAsy(ARL, loop=loop, logger=logger)
     await deezer._generate_main_session()
     track = await deezer.get_track(1421388612, True)
     data = await deezer.download_track(track['info'], './', with_lyrics=True, with_metadata=True)
     print(data)
 
 
 
 if __name__ == "__main__":
-    loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
 ```
```

### Comparing `pydeezer_asy-1.2.2/deezer_asy/DeezerAsy.py` & `pydeezer_asy-2.0.0/deezer_asy/DeezerAsy.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,145 +4,73 @@
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 import mutagen
 import aiofiles
 from mutagen.id3 import ID3, APIC
 from mutagen.easyid3 import EasyID3
 from os import path, remove
 import hashlib
-import httpx
-from  threading import Thread
+import httpx, json
 
 from .constants import *
 
 from .exceptions import LoginError
 from .exceptions import APIRequestError
 from .exceptions import DownloadLinkDecryptionError
 
 from . import util
 
+import logging
 
-class ResultThread(Thread):
-    def __init__(self, *args, **kwargs):
-        super(ResultThread, self).__init__(*args, **kwargs)
-        self._result = None
-
-    def run(self):
-        self._result = self._target(*self._args, **self._kwargs)
-
-    def result(self):
-        return self._result
 
 class DeezerAsy:
-    def __init__(self, arl) -> None:
-        """Instantiates a Deezer object
-
-        Keyword Arguments:
-            arl {str} -- Login using the given arl (default: {None})
-        """
-
+    def __init__(self, arl, loop=None, logger:logging.Logger=None) -> None:
+        self.logger = logger
         self.token = None
         self.arl = arl
+        self.loop = loop or asyncio.get_event_loop()
 
-        self._main_session = aiohttp.ClientSession(headers=networking_settings.HTTP_HEADERS)
-        self._main_session.cookie_jar.update_cookies({"arl": self.arl}, response_url=URL(api_urls.DEEZER_URL))
-
-
+        # if self.logger: self.logger.info('')
 
-    """
-        GENERAL
-    """
-    async def _generate_main_session(self):
-        await self.get_user_data()
-    def _sync_generate_main_session(self):
-        self.sync_get_user_data()
-    """
-        API
-    """
-    ####
-    def sync_get_user_data(self):
-        import requests
-        method = api_methods.GET_USER_DATA
 
-        l_session = requests.Session()
-        l_session.headers.update(networking_settings.HTTP_HEADERS)
+        if self.logger: self.logger.info('[INIT] Creating a Web Session')
+        self._main_session = aiohttp.ClientSession(headers=networking_settings.HTTP_HEADERS)
+        self._main_session.cookie_jar.update_cookies({"arl": self.arl}, response_url=URL(api_urls.DEEZER_URL))
 
+        if self.logger: self.logger.info('[INIT] Generation of auth data')
+        self.loop.run_until_complete(self.get_user_data())
         
-
-        token = "null"
-        if method != api_methods.GET_USER_DATA:
-            token = self.token
-
-        req = l_session.post(api_urls.API_URL,json={}, params={
-            "api_version": "1.0",
-            "api_token": token,
-            "input": "3",
-            "method": method
-        }, cookies={'arl': self.arl})
-        if req.status_code:
-            data = req.json()
-            data = data['results']
-            self.token = data["checkForm"]
-
-            if not data["USER"]["USER_ID"]:
-                raise LoginError("Arl is invalid.")
-
-            raw_user = data["USER"]
-
-            _arl = self.arl
-            self.cookies = l_session.cookies
-            
-            if raw_user["USER_PICTURE"]:
-                self.user = {
-                    "id": raw_user["USER_ID"],
-                    "name": raw_user["BLOG_NAME"],
-                    "arl": _arl,
-                    "image": "https://e-cdns-images.dzcdn.net/images/user/{0}/250x250-000000-80-0-0.jpg".format(raw_user["USER_PICTURE"])
-                }
+    
+    """
+    def generate_auth(self, save=False):
+        if save:
+            data = {
+                'token': self.token,
+                'cookies': self.cookies
+            }
+            with open('.auth_cache', "w") as file:
+                json.dump(data, file, indent=4)
+        else:
+            if path.exists('.auth_cache'):
+                with open('.auth_cache', "r") as file:
+                    data = json.load(file)
+                    self.token = data['token']
+                    self.cookies = data['cookies']
             else:
-                self.user = {
-                    "id": raw_user["USER_ID"],
-                    "name": raw_user["BLOG_NAME"],
-                    "arl": _arl,
-                    "image": "https://e-cdns-images.dzcdn.net/images/user/250x250-000000-80-0-0.jpg"
-                }
-    ####
-
-    async def get_user_data(self):
-        """Gets the data of the user, this will only work arl is the cookie. Make sure you have run login_via_arl() before using this.
-
-        Raises:
-            LoginError: Will raise if the arl given is not identified by Deezer
-        """
-
-        data = await self._api_call(api_methods.GET_USER_DATA)
-        data = data['results']
-        self.token = data["checkForm"]
-
-        if not data["USER"]["USER_ID"]:
-            raise LoginError("Arl is invalid.")
+                self.loop.run_until_complete(self.get_user_data())
+                self.generate_auth(True)
+    """
 
-        raw_user = data["USER"]
+    async def close_session(self):
+        if self.logger: self.logger.info('[CLOSING] Closing a local session')
+        if self._main_session:
+            await self._main_session.close()
 
-        _arl = await self.get_cookies()
-        self.cookies = _arl
-        
-        if raw_user["USER_PICTURE"]:
-            self.user = {
-                "id": raw_user["USER_ID"],
-                "name": raw_user["BLOG_NAME"],
-                "arl": _arl["arl"],
-                "image": "https://e-cdns-images.dzcdn.net/images/user/{0}/250x250-000000-80-0-0.jpg".format(raw_user["USER_PICTURE"])
-            }
-        else:
-            self.user = {
-                "id": raw_user["USER_ID"],
-                "name": raw_user["BLOG_NAME"],
-                "arl": _arl["arl"],
-                "image": "https://e-cdns-images.dzcdn.net/images/user/250x250-000000-80-0-0.jpg"
-            }
+    """
+        MAIN API
+    """
     async def get_cookies(self):
         """Get cookies in the domain of {api_urls.DEEZER_URL}
 
         Returns:
             dict -- Cookies
         """
 
@@ -152,110 +80,91 @@
             return g
         return None
     async def _api_call(self, method, params={}):
         token = "null"
         if method != api_methods.GET_USER_DATA:
             token = self.token
 
-        if self._main_session.closed:
-            async with httpx.AsyncClient(headers=networking_settings.HTTP_HEADERS, cookies=self.cookies) as session:
-                response = await session.post(api_urls.API_URL, json=params, params={
-                    "api_version": "1.0",
-                    "api_token": token,
-                    "input": "3",
-                    "method": method
-                })
-
-                data = response.json()
-        else:
-            async with self._main_session.post(api_urls.API_URL, json=params, params={
-                "api_version": "1.0",
-                "api_token": token,
-                "input": "3",
-                "method": method
-            }, cookies=await self.get_cookies()) as response:
-                data = await response.json()
-
 
+        async with self._main_session.post(api_urls.API_URL, json=params, params={
+            "api_version": "1.0",
+            "api_token": token,
+            "input": "3",
+            "method": method
+        }, cookies=await self.get_cookies()) as response:
+            data = await response.json()
+   
         if "error" in data and data["error"]:
             error_type = list(data["error"].keys())[0]
             error_message = data["error"][error_type]
+
             raise APIRequestError(
                 "{0} : {1}".format(error_type, error_message))
 
-
-        if self.token and not self._main_session.closed:
-            await self._main_session.close()
-
         return data
-    async def _legacy_api_call(self, method, params={}):
-        url = "{0}/{1}".format(api_urls.LEGACY_API_URL, method)
-        
-        async with httpx.AsyncClient(headers=networking_settings.HTTP_HEADERS, cookies=self.cookies) as session:
-            response = await session.get(url, params=params)
-            data = response.json()
-
-            if "error" in data and data["error"]:
-                error_type = list(data["error"].keys())[0]
-                error_message = data["error"][error_type]
-                raise APIRequestError(
-                    "{0} : {1}".format(error_type, error_message))
-
-            return data
     async def _legacy_search(self, method, query, limit=30, index=0):
         query = util.clean_query(query)
 
         data = await self._legacy_api_call(method, {
             "q": query,
             "limit": limit,
             "index": index
         })
 
         return data["data"]
-    async def get_track_valid_quality(self, track):
-        """Gets the valid download qualities of the given track
-
-        Arguments:
-            track {dict} -- Track dictionary, similar to the {info} value that is returned {using get_track()}
-
-        Returns:
-            list -- List of keys of the valid qualities from the {track_formats.TRACK_FORMAT_MAP}
-        """
-
-        track = track["DATA"] if "DATA" in track else track
+    async def _legacy_api_call(self, method, params={}):
+        url = "{0}/{1}".format(api_urls.LEGACY_API_URL, method)
+        async with self._main_session.get(url, cookies=self.cookies, params=params) as response:
+            data = await response.json()
+            
 
-        qualities = []
+            if "error" in data and data["error"]:
+                error_type = list(data["error"].keys())[0]
+                error_message = data["error"][error_type]
+                raise APIRequestError(
+                    "{0} : {1}".format(error_type, error_message))
 
-        # Fixes issue #4
-        for key in [track_formats.MP3_128, track_formats.MP3_320, track_formats.FLAC]:
-            download_url = await self.get_track_download_url(
-                track, quality=key, fallback=False)
+            return data
+    """
+        MAIN METHODS
+    """
+    async def get_user_data(self):
+        """Gets the data of the user, this will only work arl is the cookie. Make sure you have run login_via_arl() before using this.
 
+        Raises:
+            LoginError: Will raise if the arl given is not identified by Deezer
+        """
 
-            async with httpx.AsyncClient(headers=networking_settings.HTTP_HEADERS, cookies=self.cookies) as session:
-                res = await session.get(download_url)
+        data = await self._api_call(api_methods.GET_USER_DATA)
+        data = data['results']
+        self.token = data["checkForm"]
 
-                if res.status_code == 200 and int(res.headers["Content-length"]) > 0:
-                    qualities.append(key)
+        if not data["USER"]["USER_ID"]:
+            raise LoginError("Arl is invalid.")
 
-        return qualities
-    async def _select_valid_quality(self, track, quality):
-        valid_qualities = await self.get_track_valid_quality(track)
+        raw_user = data["USER"]
 
-        if not quality or not quality in valid_qualities:
-            default_size = int(track["FILESIZE"])
+        self.cookies = await self.get_cookies()
 
-            for key in track_formats.TRACK_FORMAT_MAP.keys():
-                if f"FILESIZE_{key}" in track and int(track[f"FILESIZE_{key}"]) == default_size:
-                    quality = track_formats.TRACK_FORMAT_MAP[key]
-                    break
+        if raw_user["USER_PICTURE"]:
+            self.user = {
+                "id": raw_user["USER_ID"],
+                "name": raw_user["BLOG_NAME"],
+                "arl": self.cookies["arl"],
+                "image": "https://e-cdns-images.dzcdn.net/images/user/{0}/250x250-000000-80-0-0.jpg".format(raw_user["USER_PICTURE"])
+            }
         else:
-            quality = track_formats.TRACK_FORMAT_MAP[quality]
+            self.user = {
+                "id": raw_user["USER_ID"],
+                "name": raw_user["BLOG_NAME"],
+                "arl": self.cookies["arl"],
+                "image": "https://e-cdns-images.dzcdn.net/images/user/250x250-000000-80-0-0.jpg"
+            }
+
 
-        return quality
     """
         ALBUM
     """
     async def get_album(self, album_id):
         """Gets the album data of the given {album_id}
 
         Arguments:
@@ -288,18 +197,17 @@
     async def _get_poster(self, poster_id, size=500, ext="jpg"):
         ext = ext.lower()
         if ext != "jpg" and ext != "png":
             raise ValueError("Image extension should only be jpg or png!")
 
         url = f'https://e-cdns-images.dzcdn.net/images/cover/{poster_id}/{size}x{size}.{ext}'
         
-        async with httpx.AsyncClient(headers=networking_settings.HTTP_HEADERS, cookies=self.cookies) as session:
-            response = await session.get(url)
-            if response.status_code == 200:
-                image_bytes = response.content
+        async with self._main_session.get(url,cookies=self.cookies) as response:
+            if response.status == 200:
+                image_bytes = await response.content.read()
                 
                 return {
                     "image": image_bytes,
                     "size": (size, size),
                     "ext": ext,
                     "mime_type": "image/jpeg" if ext == "jpg" else "image/png"
                 }
@@ -335,14 +243,68 @@
         Returns:
             list -- List of albums
         """
 
         return await self._legacy_search(api_methods.SEARCH_ALBUM, query, limit=limit, index=index)
 
     """
+        PLAYLIST
+    """
+    async def get_playlist(self, playlist_id):
+        """Gets the playlist data from the given playlist_id
+
+        Arguments:
+            playlist_id {str} -- Playlist Id
+
+        Returns:
+            dict -- Playlist data
+        """
+
+        data = await self._api_call(api_methods.PAGE_PLAYLIST, params={
+            "playlist_id": playlist_id,
+            "LANG": "en"
+        })
+
+        return data["results"]
+    async def get_playlist_tracks(self, playlist_id):
+        """Gets the tracks inside the playlist
+
+        Arguments:
+            playlist_id {str} -- Playlist Id
+
+        Returns:
+            list -- List of tracks
+        """
+
+        data = await self._api_call(api_methods.PLAYLIST_TRACKS, params={
+            "PLAYLIST_ID": playlist_id,
+            "NB": -1
+        })
+
+        for i, track in enumerate(data["results"]["data"]):
+            track["_POSITION"] = i + 1
+
+        return data["results"]["data"]
+    async def search_playlists(self, query, limit=30, index=0):
+        """Searches playlists on a given query
+
+        Arguments:
+            query {str} -- Query keyword
+
+        Keyword Arguments:
+            limit {int} -- Number of tracks (default: {30})
+            index {int} -- Offset (default: {0})
+
+        Returns:
+            list -- List of playlists
+        """
+
+        return await self._legacy_search(api_methods.SEARCH_PLAYLIST, query, limit=limit, index=index)
+
+    """
         ARTIST
     """
     async def get_artist(self, artist_id):
         """Gets the artist data from the given {artist_id}
 
         Arguments:
             artist_id {str} -- Artist Id
@@ -424,67 +386,14 @@
 
         Returns:
             list -- List of artists
         """
 
         return await self._legacy_search(api_methods.SEARCH_ARTIST, query, limit=limit, index=index)
 
-    """
-        PLAYLIST
-    """
-    async def get_playlist(self, playlist_id):
-        """Gets the playlist data from the given playlist_id
-
-        Arguments:
-            playlist_id {str} -- Playlist Id
-
-        Returns:
-            dict -- Playlist data
-        """
-
-        data = await self._api_call(api_methods.PAGE_PLAYLIST, params={
-            "playlist_id": playlist_id,
-            "LANG": "en"
-        })
-
-        return data["results"]
-    async def get_playlist_tracks(self, playlist_id):
-        """Gets the tracks inside the playlist
-
-        Arguments:
-            playlist_id {str} -- Playlist Id
-
-        Returns:
-            list -- List of tracks
-        """
-
-        data = await self._api_call(api_methods.PLAYLIST_TRACKS, params={
-            "PLAYLIST_ID": playlist_id,
-            "NB": -1
-        })
-
-        for i, track in enumerate(data["results"]["data"]):
-            track["_POSITION"] = i + 1
-
-        return data["results"]["data"]
-    async def search_playlists(self, query, limit=30, index=0):
-        """Searches playlists on a given query
-
-        Arguments:
-            query {str} -- Query keyword
-
-        Keyword Arguments:
-            limit {int} -- Number of tracks (default: {30})
-            index {int} -- Offset (default: {0})
-
-        Returns:
-            list -- List of playlists
-        """
-
-        return await self._legacy_search(api_methods.SEARCH_PLAYLIST, query, limit=limit, index=index)
 
     """
         TRACKS
     """
     async def search_tracks(self, query, limit=30, index=0):
         """Searches tracks on a given query
 
@@ -667,32 +576,29 @@
             cdn = track["MD5_ORIGIN"][0]
 
             return f'https://e-cdns-proxy-{cdn}.dzcdn.net/mobile/1/{step3}'
 
         url = decrypt_url(track_formats.TRACK_FORMAT_MAP[quality]["code"])
 
 
-        async with httpx.AsyncClient(headers=networking_settings.HTTP_HEADERS, cookies=self.cookies) as session:
-            response = await session.get(url)
-            if not fallback or (response.status_code == 200 and int(response.headers.get("Content-Length", 0)) > 0):
+        async with self._main_session.get(url, cookies=self.cookies) as response:
+            if not fallback or (response.status == 200 and int(response.headers.get("Content-Length", 0)) > 0):
                 return (url, quality)
             else:
                 if "fallback_qualities" in kwargs:
                     fallback_qualities = kwargs["fallback_qualities"]
                 else:
                     fallback_qualities = track_formats.FALLBACK_QUALITIES
 
                 for key in fallback_qualities:
                     url = decrypt_url(
                         track_formats.TRACK_FORMAT_MAP[key]["code"])
 
-                    async with httpx.AsyncClient(headers=networking_settings.HTTP_HEADERS, cookies=self.cookies) as session:
-                        response = await session.get(url)
-                    #async with self._main_session.get(url, cookies=self.get_cookies()) as response:
-                        if not fallback or (response.status_code == 200 and int(response.headers.get("Content-Length", 0)) > 0):
+                    async with self._main_session.get(url, cookies=self.cookies) as response:
+                        if not fallback or (response.status == 200 and int(response.headers.get("Content-Length", 0)) > 0):
                             return (url, key)  
     async def download_track(self, track, download_dir, quality=None, fallback=True, filename=None, renew=False,
             with_metadata=True, with_lyrics=True, tag_separator=", ", **kwargs):
         
         """Downloads the given track
 
         Arguments:
@@ -702,28 +608,33 @@
         Keyword Arguments:
             quality {str} -- Use values from {constants.track_formats}, will get the default quality if None or an invalid is given. (default: {None})
             filename {str} -- Filename with or without the extension (default: {None})
             renew {bool} -- Will renew the track object (default: {False})
             with_metadata {bool} -- If true, will write id3 tags into the file. (default: {True})
             with_lyrics {bool} -- If true, will find and save lyrics of the given track. (default: {True})
             tag_separator {str} -- Separator to separate multiple artists (default: {", "})
+        
+        Returns:
+            dict -- {'track': path_to_audio, 'lyric': path_to_lrc or None}
         """
 
         ###########################
         if with_lyrics:
             if "LYRICS" in track:
                 lyric_data = track["LYRICS"]
             else:
                 try:
                     if "DATA" in track:
-                        lyric_data = await self.get_track_lyrics(
-                            track["DATA"]["SNG_ID"])["info"]
+                        _lyric_data = await self.get_track_lyrics(
+                            track["DATA"]["SNG_ID"])
+                        lyric_data = _lyric_data["info"]
                     else:
-                        lyric_data = await self.get_track_lyrics(
-                            track["SNG_ID"])["info"]
+                        _lyric_data = await self.get_track_lyrics(
+                            track["SNG_ID"])
+                        lyric_data = _lyric_data["info"]
                 except APIRequestError:
                     with_lyrics = False
 
         track = track["DATA"] if "DATA" in track else track
         tags = await self.get_track_tags(track, separator=tag_separator, with_cover=False)
         url, quality_key = await self.get_track_download_url(
             track, quality, fallback=fallback, renew=renew, **kwargs)
@@ -740,57 +651,62 @@
 
         filename = util.clean_filename(filename)
         download_dir = path.normpath(download_dir)
         download_path = path.join(download_dir, filename)
         util.create_folders(download_dir)
         chunk_size = 2 * 1024
 
+
         async with httpx.AsyncClient(headers=networking_settings.HTTP_HEADERS, cookies=self.cookies) as client:
             res = await client.get(url, follow_redirects=True)
             data_iter = res.iter_bytes(chunk_size)
+        #async with self._main_session.get(url,cookies=self.cookies) as response:
+            #data_iter = response.content.iter_chunked(chunk_size)
             i = 0
             async with aiofiles.open(download_path, 'wb') as f:
                 f.seek(0)
             
                 for chunk in data_iter:
-                    if i % 3 > 0:
-                        await f.write(chunk)
-                    elif len(chunk) < chunk_size:
-                        await f.write(chunk)
-                        break
-                    else:
-                        cipher = Cipher(algorithms.Blowfish(blowfish_key),
-                                    modes.CBC(
-                                        bytes([i for i in range(8)])),
-                                    default_backend())
-
-                        decryptor = cipher.decryptor()
-                        dec_data = decryptor.update(
-                            chunk) + decryptor.finalize()
-
-                        await f.write(dec_data)
-
+                #async for chunk in data_iter:
+                    try:
+                        if i % 3 > 0:
+                            await f.write(chunk)
+                        elif len(chunk) < chunk_size:
+                            await f.write(chunk)
+                            break
+                        else:
+                            cipher = Cipher(algorithms.Blowfish(blowfish_key),
+                                        modes.CBC(
+                                            bytes([i for i in range(8)])),
+                                        default_backend())
+
+                            decryptor = cipher.decryptor()
+                            dec_data = decryptor.update(
+                                chunk) + decryptor.finalize()
+
+                            await f.write(dec_data)
+                    except:
+                        print(type(chunk))
                     i += 1
 
         if with_metadata:
             if ext.lower() == ".flac":
                 pass #self._write_flac_tags(download_path, track, tags=tags)
             else:
                 await self._write_mp3_tags(download_path, track, tags=tags)
         if with_lyrics:
             lyrics_path = path.join(download_dir, filename[:-len(ext)])
             lyric_check = await self.save_lyrics(lyric_data, lyrics_path)
             if not lyric_check[0]:
-                asyncio.get_event_loop().run_in_executor(None, remove, lyric_check[1])
-                return (download_path)
+                self.loop.run_in_executor(None, remove, lyric_check[1])
+                return {'track': download_path, 'lyruc': None}
 
-            return (download_path, lyric_check[1])
+            return {'track': download_path, 'lyruc': lyric_check[1]}
 
-        return (download_path)
-    
+        return {'track': download_path, 'lyruc': None}
     async def get_tracks(self, track_ids):
         """Gets the list of the tracks that corresponds with the given {track_ids}
 
         Arguments:
             track_ids {list} -- List of track id
 
         Returns:
@@ -856,33 +772,25 @@
             if not "LYRICS_SYNC_JSON" in lyric_data:
                 return (False, save_path)
 
             sync_data = lyric_data["LYRICS_SYNC_JSON"]
 
             for line in sync_data:
                 if str(line["line"]):
-                    f.write("{0}{1}".format(
+                    await f.write("{0}{1}".format(
                         line["lrc_timestamp"], line["line"]))
-                f.write("\n")
+                await f.write("\n")
 
         return (True, save_path)
     
     """
         TAG EDIT
 
         p.s: It might be blocking the thread, not sure
     """
-    async def __write_mp3_tags(self, path, track, tags=None):
-        loop = asyncio.new_event_loop()
-        asyncio.set_event_loop(loop)
-        _result = loop.run_until_complete(self._write_mp3_tags(path, track, tags))
-        result = await _result
-
-        return result
-    
     def __update_mp3(self, path, tags):
         audio = mutagen.File(path, easy=True)
         if audio is None:
             raise ValueError("Invalid file format")
 
         audio.delete()
         EasyID3.RegisterTextKey("label", "TPUB")
@@ -900,18 +808,16 @@
             cover_handle["APIC"] = APIC(
                 type=3,
                 mime=cover["mime_type"],
                 data=cover["image"]
             )
             cover_handle.save(path)
         audio.save()
-
     async def _write_mp3_tags(self, path, track, tags=None):
         track = track["DATA"] if "DATA" in track else track
 
         if not tags:
             tags = await self.get_track_tags(track)
 
-        _update_tags = ResultThread(target=self.__update_mp3, args=(path, tags,))
-        _update_tags.start()
-        _update_tags.join()
+        _ = await self.loop.run_in_executor(None, self.__update_mp3, path, tags)
+
         return True
```

### Comparing `pydeezer_asy-1.2.2/deezer_asy/constants/api_methods.py` & `pydeezer_asy-2.0.0/deezer_asy/constants/api_methods.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.2.2/deezer_asy/constants/track_formats.py` & `pydeezer_asy-2.0.0/deezer_asy/constants/track_formats.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.2.2/deezer_asy/util.py` & `pydeezer_asy-2.0.0/deezer_asy/util.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.2.2/pydeezer_asy.egg-info/PKG-INFO` & `pydeezer_asy-2.0.0/pydeezer_asy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: pydeezer-asy
-Version: 1.2.2
+Version: 2.0.0
 Summary: Asynchronous version of the `py-deezer` module
 Home-page: https://github.com/drhspfn/deezer-asy
 Author: drhspfn
 Author-email: drhspfn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # deezer-asy
 Asynchronous version of the [py-deezer](https://github.com/acgonzales/pydeezer) module
-
-
 At the moment, the functionality does not completely repeat the original library
 
-
-# Differences
+### Differences
 This version is asynchronous. Otherwise, it repeats the arguments of the original library.
 
-All that differs is initialization. You need to create a session that will get some information from your ARL, 
-`await deezer._generate_main_session()` is responsible for this. 
 
-It must be called when you start your application, in `on_startup` in your bot, or otherwise
+# Last update `2.0.0`
+    * Simplified module initialization
+    * Changed response type of `download_track` function: {'track': path, 'lyric': path or None}
+    
 
 
 # What works?
-* Getting information about albums, tracks (their tags).
+* Getting information about albums, playlists, artists, tracks (their tags).
 * Downloading tracks.
 
 
 # What needs to be done
 * Adding tags to .flac. `(So вЂ‹вЂ‹far, idling)`
 
 # Installation
@@ -39,23 +37,32 @@
 ```
 
 # Usage as a package
 
 ```python
 from deezer_asy import DeezerAsy
 import asyncio
+import logging
 
+logging.basicConfig(
+    level=logging.INFO,  
+    format="%(asctime)s [%(levelname)s] %(message)s",
+    datefmt="%Y-%m-%d %H:%M:%S"
+)
+logger = logging.getLogger("main_logger")
+loop = asyncio.get_event_loop()
 ARL = "edit this"
 
 async def main():
-    deezer = DeezerAsy(ARL)
+    # You can pass `loop` as an argument, or leave None
+    # If you want logging, pass the `logger` as an argument
+    deezer = DeezerAsy(ARL, loop=loop, logger=logger)
     await deezer._generate_main_session()
     track = await deezer.get_track(1421388612, True)
     data = await deezer.download_track(track['info'], './', with_lyrics=True, with_metadata=True)
     print(data)
 
 
 
 if __name__ == "__main__":
-    loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
 ```
```

### Comparing `pydeezer_asy-1.2.2/pydeezer_asy.egg-info/SOURCES.txt` & `pydeezer_asy-2.0.0/pydeezer_asy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.2.2/setup.py` & `pydeezer_asy-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='pydeezer_asy',
-    version='1.2.2',
+    version='2.0.0',
     description='Asynchronous version of the `py-deezer` module',
     author='drhspfn',
     author_email="drhspfn@gmail.com",
     packages=setuptools.find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/drhspfn/deezer-asy",
```

