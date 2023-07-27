# Comparing `tmp/pydeezer_asy-2.0.0.tar.gz` & `tmp/pydeezer_asy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeezer_asy-2.0.0.tar", last modified: Thu Jul 27 20:50:38 2023, max compression
+gzip compressed data, was "pydeezer_asy-2.1.0.tar", last modified: Thu Jul 27 21:28:20 2023, max compression
```

## Comparing `pydeezer_asy-2.0.0.tar` & `pydeezer_asy-2.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 20:50:38.519834 pydeezer_asy-2.0.0/
--rw-rw-rw-   0        0        0     1910 2023-07-27 20:50:38.516847 pydeezer_asy-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1546 2023-07-27 20:49:08.000000 pydeezer_asy-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 20:50:38.449600 pydeezer_asy-2.0.0/deezer_asy/
--rw-rw-rw-   0        0        0    28680 2023-07-27 20:40:18.000000 pydeezer_asy-2.0.0/deezer_asy/DeezerAsy.py
--rw-rw-rw-   0        0        0      136 2023-07-27 18:53:44.000000 pydeezer_asy-2.0.0/deezer_asy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 20:50:38.466551 pydeezer_asy-2.0.0/deezer_asy/constants/
--rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/constants/__init__.py
--rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/constants/api_methods.py
--rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/constants/api_urls.py
--rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/constants/image_hosts.py
--rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/constants/networking_settings.py
--rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/constants/search_types.py
--rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/constants/track_formats.py
--rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-2.0.0/deezer_asy/exceptions.py
--rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-2.0.0/deezer_asy/util.py
-drwxrwxrwx   0        0        0        0 2023-07-27 20:50:38.510860 pydeezer_asy-2.0.0/pydeezer_asy.egg-info/
--rw-rw-rw-   0        0        0     1910 2023-07-27 20:50:38.000000 pydeezer_asy-2.0.0/pydeezer_asy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-07-27 20:50:38.000000 pydeezer_asy-2.0.0/pydeezer_asy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 20:50:38.000000 pydeezer_asy-2.0.0/pydeezer_asy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-27 20:50:38.000000 pydeezer_asy-2.0.0/pydeezer_asy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-27 20:50:38.000000 pydeezer_asy-2.0.0/pydeezer_asy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 20:50:38.519834 pydeezer_asy-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      749 2023-07-27 20:50:26.000000 pydeezer_asy-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:28:20.736048 pydeezer_asy-2.1.0/
+-rw-rw-rw-   0        0        0     1910 2023-07-27 21:28:20.735050 pydeezer_asy-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1546 2023-07-27 20:49:08.000000 pydeezer_asy-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 21:28:20.553669 pydeezer_asy-2.1.0/deezer_asy/
+-rw-rw-rw-   0        0        0    28966 2023-07-27 21:28:13.000000 pydeezer_asy-2.1.0/deezer_asy/DeezerAsy.py
+-rw-rw-rw-   0        0        0      136 2023-07-27 18:53:44.000000 pydeezer_asy-2.1.0/deezer_asy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:28:20.581473 pydeezer_asy-2.1.0/deezer_asy/constants/
+-rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-2.1.0/deezer_asy/constants/__init__.py
+-rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-2.1.0/deezer_asy/constants/api_methods.py
+-rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-2.1.0/deezer_asy/constants/api_urls.py
+-rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-2.1.0/deezer_asy/constants/image_hosts.py
+-rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-2.1.0/deezer_asy/constants/networking_settings.py
+-rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-2.1.0/deezer_asy/constants/search_types.py
+-rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-2.1.0/deezer_asy/constants/track_formats.py
+-rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-2.1.0/deezer_asy/exceptions.py
+-rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-2.1.0/deezer_asy/util.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:28:20.731261 pydeezer_asy-2.1.0/pydeezer_asy.egg-info/
+-rw-rw-rw-   0        0        0     1910 2023-07-27 21:28:20.000000 pydeezer_asy-2.1.0/pydeezer_asy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2023-07-27 21:28:20.000000 pydeezer_asy-2.1.0/pydeezer_asy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 21:28:20.000000 pydeezer_asy-2.1.0/pydeezer_asy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-27 21:28:20.000000 pydeezer_asy-2.1.0/pydeezer_asy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 21:28:20.000000 pydeezer_asy-2.1.0/pydeezer_asy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 21:28:20.736048 pydeezer_asy-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-07-27 21:28:04.000000 pydeezer_asy-2.1.0/setup.py
```

### Comparing `pydeezer_asy-2.0.0/PKG-INFO` & `pydeezer_asy-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeezer_asy
-Version: 2.0.0
+Version: 2.1.0
 Summary: Asynchronous version of the `py-deezer` module
 Home-page: https://github.com/drhspfn/deezer-asy
 Author: drhspfn
 Author-email: drhspfn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pydeezer_asy-2.0.0/README.md` & `pydeezer_asy-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.0.0/deezer_asy/DeezerAsy.py` & `pydeezer_asy-2.1.0/deezer_asy/DeezerAsy.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,17 +171,19 @@
             album_id {str} -- Album Id
 
         Returns:
             dict -- Album data
         """
 
         data = await self._legacy_api_call("/album/{0}".format(album_id))
-
-        data["cover_id"] = str(data["cover_small"]).split(
-            "cover/")[1].split("/")[0]
+        if data["cover_small"]:
+            data["cover_id"] = str(data["cover_small"]).split(
+                "cover/")[1].split("/")[0]
+        else:
+            data["cover_id"] = -1
 
         return data
     async def get_album_poster(self, album, size=500, ext="jpg"):
         """Gets the album poster as a binary data
 
         Arguments:
             album {dict} -- Album data
@@ -191,19 +193,23 @@
             ext {str} -- Extension of the image, can be ('.jpg' or '.png') (default: {"jpg"})
 
         Returns:
             bytes -- Binary data of the image
         """
         return await self._get_poster(album["cover_id"], size=size, ext=ext)
     async def _get_poster(self, poster_id, size=500, ext="jpg"):
+         
+        
         ext = ext.lower()
         if ext != "jpg" and ext != "png":
             raise ValueError("Image extension should only be jpg or png!")
-
-        url = f'https://e-cdns-images.dzcdn.net/images/cover/{poster_id}/{size}x{size}.{ext}'
+        if poster_id == -1:
+            url = "https://static.vecteezy.com/system/resources/thumbnails/022/059/000/small/no-image-available-icon-vector.jpg"
+        else:
+            url = f'https://e-cdns-images.dzcdn.net/images/cover/{poster_id}/{size}x{size}.{ext}'
         
         async with self._main_session.get(url,cookies=self.cookies) as response:
             if response.status == 200:
                 image_bytes = await response.content.read()
                 
                 return {
                     "image": image_bytes,
```

### Comparing `pydeezer_asy-2.0.0/deezer_asy/constants/api_methods.py` & `pydeezer_asy-2.1.0/deezer_asy/constants/api_methods.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.0.0/deezer_asy/constants/track_formats.py` & `pydeezer_asy-2.1.0/deezer_asy/constants/track_formats.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.0.0/deezer_asy/util.py` & `pydeezer_asy-2.1.0/deezer_asy/util.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.0.0/pydeezer_asy.egg-info/PKG-INFO` & `pydeezer_asy-2.1.0/pydeezer_asy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeezer-asy
-Version: 2.0.0
+Version: 2.1.0
 Summary: Asynchronous version of the `py-deezer` module
 Home-page: https://github.com/drhspfn/deezer-asy
 Author: drhspfn
 Author-email: drhspfn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pydeezer_asy-2.0.0/pydeezer_asy.egg-info/SOURCES.txt` & `pydeezer_asy-2.1.0/pydeezer_asy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.0.0/setup.py` & `pydeezer_asy-2.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='pydeezer_asy',
-    version='2.0.0',
+    version='2.1.0',
     description='Asynchronous version of the `py-deezer` module',
     author='drhspfn',
     author_email="drhspfn@gmail.com",
     packages=setuptools.find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/drhspfn/deezer-asy",
```

