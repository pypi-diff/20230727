# Comparing `tmp/scratch-getdata-1.0.7.tar.gz` & `tmp/scratch-getdata-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratch-getdata-1.0.7.tar", last modified: Tue Jul 25 20:56:52 2023, max compression
+gzip compressed data, was "scratch-getdata-1.0.8.tar", last modified: Thu Jul 27 01:31:08 2023, max compression
```

## Comparing `scratch-getdata-1.0.7.tar` & `scratch-getdata-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-25 20:56:52.475944 scratch-getdata-1.0.7/
--rw-r--r--   0 runner    (1000) runner    (1000)     2987 2023-07-25 20:56:52.475944 scratch-getdata-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     2387 2023-07-25 19:32:03.000000 scratch-getdata-1.0.7/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      698 2023-07-25 20:56:17.000000 scratch-getdata-1.0.7/pyproject.toml
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-25 20:56:52.471944 scratch-getdata-1.0.7/scratch_getdata/
--rw-r--r--   0 runner    (1000) runner    (1000)      517 2023-07-25 19:32:23.000000 scratch-getdata-1.0.7/scratch_getdata/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4214 2023-07-25 19:30:04.000000 scratch-getdata-1.0.7/scratch_getdata/api_client.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-25 20:56:52.475944 scratch-getdata-1.0.7/scratch_getdata.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2987 2023-07-25 20:56:52.000000 scratch-getdata-1.0.7/scratch_getdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      285 2023-07-25 20:56:52.000000 scratch-getdata-1.0.7/scratch_getdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-25 20:56:52.000000 scratch-getdata-1.0.7/scratch_getdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-25 20:56:52.000000 scratch-getdata-1.0.7/scratch_getdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2023-07-25 20:56:52.000000 scratch-getdata-1.0.7/scratch_getdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-25 20:56:52.479945 scratch-getdata-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-28 02:32:47.000000 scratch-getdata-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-27 01:31:08.471429 scratch-getdata-1.0.8/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3123 2023-07-27 01:31:08.471429 scratch-getdata-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2523 2023-07-27 01:30:51.000000 scratch-getdata-1.0.8/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      698 2023-07-27 01:26:44.000000 scratch-getdata-1.0.8/pyproject.toml
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-27 01:31:08.467428 scratch-getdata-1.0.8/scratch_getdata/
+-rw-r--r--   0 runner    (1000) runner    (1000)      517 2023-07-25 19:32:23.000000 scratch-getdata-1.0.8/scratch_getdata/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5084 2023-07-27 01:26:21.000000 scratch-getdata-1.0.8/scratch_getdata/api_client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-27 01:31:08.471429 scratch-getdata-1.0.8/scratch_getdata.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3123 2023-07-27 01:31:08.000000 scratch-getdata-1.0.8/scratch_getdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      285 2023-07-27 01:31:08.000000 scratch-getdata-1.0.8/scratch_getdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-27 01:31:08.000000 scratch-getdata-1.0.8/scratch_getdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-27 01:31:08.000000 scratch-getdata-1.0.8/scratch_getdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2023-07-27 01:31:08.000000 scratch-getdata-1.0.8/scratch_getdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-27 01:31:08.471429 scratch-getdata-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-28 02:32:47.000000 scratch-getdata-1.0.8/setup.py
```

### Comparing `scratch-getdata-1.0.7/PKG-INFO` & `scratch-getdata-1.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratch-getdata
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Module to fetch scratch things from ScratchGetData
 Author: kokofixcomputers
 Author-email: kokofixcomputers <kokocanfixit@kokofixcomputers.serv00.net>
 Project-URL: Github, https://github.com/scratch-getdata/scratch-getdata-python
 Project-URL: Bug Tracker, https://github.com/scratch-getdata/scratch-getdata-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,14 +22,18 @@
 ------------
 The ScratchAPIClient class provides a convenient interface for accessing data from the Scratch API using the "https://scratch-get-data.kokoiscool.repl.co" base URL.
 Github: https://github.com/kokofixcomputers/Scratch-getdata
 
 Install: pip install scratch-getdata
 Import: from scratch_getdata import ScratchAPIClient
 
+Api Key
+-
+You will need to signup at the api: https://scratch-get-data.kokoiscool.repl.co and get the api key first before using this.
+
 Usage
 -----
 1. Instantiating the ScratchAPIClient class:
 client = ScratchAPIClient()
 
 
 2. Retrieving the follower count of a user:
```

### Comparing `scratch-getdata-1.0.7/README.md` & `scratch-getdata-1.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 ------------
 The ScratchAPIClient class provides a convenient interface for accessing data from the Scratch API using the "https://scratch-get-data.kokoiscool.repl.co" base URL.
 Github: https://github.com/kokofixcomputers/Scratch-getdata
 
 Install: pip install scratch-getdata
 Import: from scratch_getdata import ScratchAPIClient
 
+Api Key
+-
+You will need to signup at the api: https://scratch-get-data.kokoiscool.repl.co and get the api key first before using this.
+
 Usage
 -----
 1. Instantiating the ScratchAPIClient class:
 client = ScratchAPIClient()
 
 
 2. Retrieving the follower count of a user:
```

### Comparing `scratch-getdata-1.0.7/pyproject.toml` & `scratch-getdata-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scratch-getdata"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="kokofixcomputers", email="kokocanfixit@kokofixcomputers.serv00.net" },
 ]
 dependencies = ['requests']
 description = "A Module to fetch scratch things from ScratchGetData"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `scratch-getdata-1.0.7/scratch_getdata/__init__.py` & `scratch-getdata-1.0.8/scratch_getdata/__init__.py`

 * *Files identical despite different names*

### Comparing `scratch-getdata-1.0.7/scratch_getdata/api_client.py` & `scratch-getdata-1.0.8/scratch_getdata/api_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,85 +3,130 @@
 class ScratchAPIClient:
     def __init__(self):
         print("It may take a while for ScratchForGetData to boot up like 3-10 seconds")
         self.base_url = "https://scratch-get-data.kokoiscool.repl.co"
 
     def get_follower_count(self, username, api_key):
         url = f"{self.base_url}/get/follower-count/{username}/"
-        response = requests.get(url, key=api_key)
+        params = {
+            "key": api_key
+        }
+        response = requests.get(url, params=params)
         return response.text.strip()  # Return the follower count as a string
 
     def is_scratcher(self, username, api_key):
         url = f"{self.base_url}/get/is_scratcher/{username}/"
-        response = requests.get(url, key=api_key)
+        params = {
+            "key": api_key
+        }
+        response = requests.get(url, params=params)
         return response.text.strip().lower() == "true"  # Return True or False based on the response
 
     def get_following_count(self, username, api_key):
         url = f"{self.base_url}/get/following-count/{username}/"
-        response = requests.get(url, key=api_key)
+        params = {
+            "key": api_key
+        }
+        response = requests.get(url, params=params)
         return response.text.strip()  # Return the following count as a string
 
     def get_wiwo(self, username, api_key):
         url = f"{self.base_url}/get/wiwo/{username}/"
-        response = requests.get(url, key=api_key)
+        params = {
+            "key": api_key
+        }
+        response = requests.get(url, params=params)
         return response.text.strip()  # Return the WiWo as a string
 
     def get_about_me(self, username, api_key):
         url = f"{self.base_url}/get/aboutme/{username}/"
-        response = requests.get(url, key=api_key)
+        params = {
+            "key": api_key
+        }
+        response = requests.get(url, params=params)
         return response.text.strip()  # Return the About Me text as a string
 
     def get_messages(self, username, api_key):
         url = f"{self.base_url}/get/messages/{username}/"
-        response = requests.get(url, key=api_key)
+        params = {
+            "key": api_key
+        }
+        response = requests.get(url, params=params)
         return response.text.strip()  # Return the Messages as a string
 
     def get_project_creator(self, project_id, api_key):
         url = f"{self.base_url}/get/project/creator/{project_id}/"
-        response = requests.get(url, key=api_key)
+        params = {
+            "key": api_key
+        }
+        response = requests.get(url, params=params)
         return response.text.strip()  # Return the project creator username as a string
 
     def get_project_name(self, project_id, api_key):
         url = f"{self.base_url}/get/project/name/{project_id}/"
-        response = requests.get(url, key=api_key)
+        params = {
+            "key": api_key
+        }
+        response = requests.get(url, params=params)
         return response.text.strip()  # Return the project name as a string
 
     def get_project_description(self, project_id, api_key):
         url = f"{self.base_url}/get/project/notes_and_credits/{project_id}/"
-        response = requests.get(url, key=api_key)
+        params = {
+            "key": api_key
+        }
+        response = requests.get(url, params=params)
         return response.text.strip()  # Return the project description as a string
 
     def get_project_instructions(self, project_id, api_key):
         url = f"{self.base_url}/get/project/instructions/{project_id}/"
-        response = requests.get(url, key=api_key)
+        params = {
+            "key": api_key
+        }
+        response = requests.get(url, params=params)
         return response.text.strip()  # Return the project instructions as a string
 
     def get_project_blocks(self, project_id, api_key):
         url = f"{self.base_url}/get/project/blocks/{project_id}/"
-        response = requests.get(url, key=api_key)
+        params = {
+            "key": api_key
+        }
+        response = requests.get(url, params=params)
         return response.text.strip()  # Return the project blocks as a string
 
     def get_forum_title(self, post_id, api_key):
         url = f"{self.base_url}/get/forum/title/{post_id}/"
-        response = requests.get(url, key=api_key)
+        params = {
+            "key": api_key
+        }
+        response = requests.get(url, params=params)
         return response.text.strip()  # Return the forum post title as a string
 
     def get_forum_category(self, post_id, api_key):
         url = f"{self.base_url}/get/forum/category/{post_id}/"
-        response = requests.get(url, key=api_key)
+        params = {
+            "key": api_key
+        }
+        response = requests.get(url, params=params)
         return response.text.strip()  # Return the forum post category as a string
 
     def get_scratch_user_country(self, username, api_key):
         url = f"{self.base_url}/get/user/country/{username}/"
-        response = requests.get(url, key=api_key)
+        params = {
+            "key": api_key
+        }
+        response = requests.get(url, params=params)
         return response.text.strip()  # Return the Scratch user's country as a string
 
     def get_studio_title(self, studio_id, api_key):
         url = f"{self.base_url}/get/studio/title/{studio_id}/"
-        response = requests.get(url, key=api_key)
+        params = {
+            "key": api_key
+        }
+        response = requests.get(url, params=params)
         return response.text.strip()  # Return the Scratch studio title as string
 
 class TestConnection:
 
   def test():
     base_url = "https://scratch-get-data.kokoiscool.repl.co"
```

### Comparing `scratch-getdata-1.0.7/scratch_getdata.egg-info/PKG-INFO` & `scratch-getdata-1.0.8/scratch_getdata.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratch-getdata
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Module to fetch scratch things from ScratchGetData
 Author: kokofixcomputers
 Author-email: kokofixcomputers <kokocanfixit@kokofixcomputers.serv00.net>
 Project-URL: Github, https://github.com/scratch-getdata/scratch-getdata-python
 Project-URL: Bug Tracker, https://github.com/scratch-getdata/scratch-getdata-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,14 +22,18 @@
 ------------
 The ScratchAPIClient class provides a convenient interface for accessing data from the Scratch API using the "https://scratch-get-data.kokoiscool.repl.co" base URL.
 Github: https://github.com/kokofixcomputers/Scratch-getdata
 
 Install: pip install scratch-getdata
 Import: from scratch_getdata import ScratchAPIClient
 
+Api Key
+-
+You will need to signup at the api: https://scratch-get-data.kokoiscool.repl.co and get the api key first before using this.
+
 Usage
 -----
 1. Instantiating the ScratchAPIClient class:
 client = ScratchAPIClient()
 
 
 2. Retrieving the follower count of a user:
```

