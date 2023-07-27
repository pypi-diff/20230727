# Comparing `tmp/cosmopawn-1.0.0.tar.gz` & `tmp/cosmopawn-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmopawn-1.0.0.tar", last modified: Thu Jul 27 03:51:33 2023, max compression
+gzip compressed data, was "cosmopawn-1.1.0.tar", last modified: Thu Jul 27 05:21:14 2023, max compression
```

## Comparing `cosmopawn-1.0.0.tar` & `cosmopawn-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 03:51:33.215652 cosmopawn-1.0.0/
--rw-rw-rw-   0        0        0     1064 2023-07-09 16:51:20.000000 cosmopawn-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1095 2023-07-27 03:51:33.214651 cosmopawn-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      570 2023-07-27 02:14:46.000000 cosmopawn-1.0.0/README.md
--rw-rw-rw-   0        0        0      570 2023-07-27 02:20:25.000000 cosmopawn-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 03:51:33.215652 cosmopawn-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-27 03:51:33.200078 cosmopawn-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 03:51:33.206630 cosmopawn-1.0.0/src/cosmopawn/
--rw-rw-rw-   0        0        0       32 2023-07-27 02:15:43.000000 cosmopawn-1.0.0/src/cosmopawn/__init__.py
--rw-rw-rw-   0        0        0     2051 2023-07-27 03:33:57.000000 cosmopawn-1.0.0/src/cosmopawn/cosmopawn.py
-drwxrwxrwx   0        0        0        0 2023-07-27 03:51:33.212652 cosmopawn-1.0.0/src/cosmopawn.egg-info/
--rw-rw-rw-   0        0        0     1095 2023-07-27 03:51:33.000000 cosmopawn-1.0.0/src/cosmopawn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-07-27 03:51:33.000000 cosmopawn-1.0.0/src/cosmopawn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 03:51:33.000000 cosmopawn-1.0.0/src/cosmopawn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-27 03:51:33.000000 cosmopawn-1.0.0/src/cosmopawn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 05:21:14.736060 cosmopawn-1.1.0/
+-rw-rw-rw-   0        0        0     1064 2023-07-09 16:51:20.000000 cosmopawn-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1152 2023-07-27 05:21:14.735055 cosmopawn-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      625 2023-07-27 05:19:50.000000 cosmopawn-1.1.0/README.md
+-rw-rw-rw-   0        0        0      570 2023-07-27 05:20:35.000000 cosmopawn-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 05:21:14.736060 cosmopawn-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 05:21:14.721508 cosmopawn-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 05:21:14.727527 cosmopawn-1.1.0/src/cosmopawn/
+-rw-rw-rw-   0        0        0       32 2023-07-27 02:15:43.000000 cosmopawn-1.1.0/src/cosmopawn/__init__.py
+-rw-rw-rw-   0        0        0     3315 2023-07-27 05:04:51.000000 cosmopawn-1.1.0/src/cosmopawn/cosmopawn.py
+drwxrwxrwx   0        0        0        0 2023-07-27 05:21:14.734033 cosmopawn-1.1.0/src/cosmopawn.egg-info/
+-rw-rw-rw-   0        0        0     1152 2023-07-27 05:21:14.000000 cosmopawn-1.1.0/src/cosmopawn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-07-27 05:21:14.000000 cosmopawn-1.1.0/src/cosmopawn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 05:21:14.000000 cosmopawn-1.1.0/src/cosmopawn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 05:21:14.000000 cosmopawn-1.1.0/src/cosmopawn.egg-info/top_level.txt
```

### Comparing `cosmopawn-1.0.0/LICENSE` & `cosmopawn-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmopawn-1.0.0/PKG-INFO` & `cosmopawn-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: cosmopawn
-Version: 1.0.0
+Version: 1.1.0
 Summary: An API wrapper for the CosmoPawn API in Python
 Author: pennacap
 Project-URL: Homepage, https://github.com/pennacap/cosmopawn-py
 Project-URL: Bug Tracker, https://github.com/pennacap/cosmopawn-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# CosmoPawn-Py : An API wrapper for [CosmoPawn](https://github.com/hczhu/CosmoPawn) in Python
+# CosmoPawn-Py : An API wrapper for [CosmoPawn](https://github.com/pennacap/cosmo-pawn) in Python
 ## Installation
 ```sh
 pip install cosmopawn
 # or
 pip3 install cosmopawn
+# or
+pip install git+https://github.com/pennacap/cosmopawn-py
 ```
 ## Usage
 ```py
 import cosmopawn
 wrapper = cosmopawn.CosmoPawn() # Or pass in an IP address / domain
-wrapper.download('dog', save_to='dog_pics', prefix='dog', no=10) # downloads 10 dog pictures, prefixing their file name with dog and saving it to dog_pics/
+wrapper.download('dog', prefix='dog_pics/dog', no=10) # downloads 10 dog pictures, prefixing their file name with dog and saving it to dog_pics/
 wrapper.upload(['file1.jpg', 'file2.png'], ['keyword1', 'keyword2']) # upload file1.jpg and file2.png with keywords keyword1 and keywords2
 ```
```

### Comparing `cosmopawn-1.0.0/pyproject.toml` & `cosmopawn-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cosmopawn"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="pennacap" },
 ]
 description = "An API wrapper for the CosmoPawn API in Python"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `cosmopawn-1.0.0/src/cosmopawn/cosmopawn.py` & `cosmopawn-1.1.0/src/cosmopawn/cosmopawn.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import hashlib
 import typing
 import requests
 import os
 
+
 class CosmoPawn:
     """The main API wrapper class"""
+
     def __init__(self, domain: str = 'http://143.198.148.104/'):
         self.domain: str = domain
 
     def upload(self, images: typing.Union[str, bytes, list[typing.Union[str, bytes]]], keywords: list[str]):
         """Upload images to CosmoPawn
 
         Args:
@@ -25,29 +28,52 @@
                 with open(i, 'rb') as f:
                     req = requests.post(
                         self.domain+'/upload', data=f.read(), headers={'Keywords': ','.join(keywords)})
                     if not req.ok:
                         raise Exception(
                             'Error uploading image "'+i+'": '+req.text)
             else:
-                req = requests.post(self.domain+'/upload', data=i, headers={'Keywords': ','.join(keywords)})
+                req = requests.post(
+                    self.domain+'/upload', data=i, headers={'Keywords': ','.join(keywords)})
                 if not req.ok:
                     raise Exception('Error uploading image: '+req.text)
 
-    def download(self, keyword: str, prefix: str = '', save_to: str = '.', no: int = -1):
-        os.makedirs(save_to, exist_ok=True)
+    def download(self, keyword: str, prefix: str = './', no: int = -1, verify: bool = True, skip_errors : bool = False):
+        """Download images from CosmoPawn
+
+        Args:
+            keyword (str): The keyword to use
+            prefix (str, optional): The prefix to append to the image (either a directory, a filename prefix or both). Defaults to './'.
+            no (int, optional): The number of images to fetch. Defaults to -1.
+            verify (bool, optional): Sets whether the image's SHA256 hash is checked. Defaults to True.
+            skip_errors (bool, optional): _description_. Sets whether to continue if an image fails to download. Defaults to False.
+        """
+        os.makedirs(os.path.dirname(prefix), exist_ok=True)
         req = requests.get(self.domain+'/'+keyword)
         if not req.ok:
             raise Exception(
                 F'Error {req.status_code} fetching keyword "{keyword}"')
         images = req.json()
-        count = 0
+        imgs_found = []
         for i in images:
-            if no != -1 and count == no:
+            if no != -1 and len(imgs_found) == no:
                 return
             req = requests.get(self.domain+'/images/'+i)
             if not req.ok:
-                continue
-            with open(save_to+'/'+prefix+i, 'wb') as f:
+                if skip_errors:
+                    continue
+                else:
+                    raise Exception(f'Error fetching image "{i}"')
+            with open(prefix+i, 'wb') as f:
                 f.write(req.content)
-            count += 1
-    
+            imgs_found += [i]
+        if verify:
+            hashes = requests.get(self.domain+'/keywords/'+keyword+'.sha256')
+            if not hashes.ok:
+                raise Exception('Error fetching SHA256 hashes for keyword "'+keyword+'"')
+            hashes = hashes.json()
+            for x in imgs_found:
+                with open(prefix+x, 'rb') as f:
+                    if hashlib.sha256(f.read()).hexdigest() != hashes[x]:
+                        raise Exception(f'Hash failed for {x}')
+        
+
```

### Comparing `cosmopawn-1.0.0/src/cosmopawn.egg-info/PKG-INFO` & `cosmopawn-1.1.0/src/cosmopawn.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: cosmopawn
-Version: 1.0.0
+Version: 1.1.0
 Summary: An API wrapper for the CosmoPawn API in Python
 Author: pennacap
 Project-URL: Homepage, https://github.com/pennacap/cosmopawn-py
 Project-URL: Bug Tracker, https://github.com/pennacap/cosmopawn-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# CosmoPawn-Py : An API wrapper for [CosmoPawn](https://github.com/hczhu/CosmoPawn) in Python
+# CosmoPawn-Py : An API wrapper for [CosmoPawn](https://github.com/pennacap/cosmo-pawn) in Python
 ## Installation
 ```sh
 pip install cosmopawn
 # or
 pip3 install cosmopawn
+# or
+pip install git+https://github.com/pennacap/cosmopawn-py
 ```
 ## Usage
 ```py
 import cosmopawn
 wrapper = cosmopawn.CosmoPawn() # Or pass in an IP address / domain
-wrapper.download('dog', save_to='dog_pics', prefix='dog', no=10) # downloads 10 dog pictures, prefixing their file name with dog and saving it to dog_pics/
+wrapper.download('dog', prefix='dog_pics/dog', no=10) # downloads 10 dog pictures, prefixing their file name with dog and saving it to dog_pics/
 wrapper.upload(['file1.jpg', 'file2.png'], ['keyword1', 'keyword2']) # upload file1.jpg and file2.png with keywords keyword1 and keywords2
 ```
```

