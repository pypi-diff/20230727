# Comparing `tmp/raycut-0.0.1.tar.gz` & `tmp/raycut-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raycut-0.0.1.tar", last modified: Thu Jul 27 19:43:12 2023, max compression
+gzip compressed data, was "raycut-0.0.2.tar", last modified: Thu Jul 27 19:50:54 2023, max compression
```

## Comparing `raycut-0.0.1.tar` & `raycut-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-27 19:43:12.458817 raycut-0.0.1/
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      533 2023-07-27 19:43:12.458817 raycut-0.0.1/PKG-INFO
-drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-27 19:43:12.458817 raycut-0.0.1/raycut/
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)     2791 2023-07-27 19:36:44.000000 raycut-0.0.1/raycut/__init__.py
-drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-27 19:43:12.458817 raycut-0.0.1/raycut.egg-info/
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      533 2023-07-27 19:43:12.000000 raycut-0.0.1/raycut.egg-info/PKG-INFO
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      176 2023-07-27 19:43:12.000000 raycut-0.0.1/raycut.egg-info/SOURCES.txt
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)        1 2023-07-27 19:43:12.000000 raycut-0.0.1/raycut.egg-info/dependency_links.txt
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)       10 2023-07-27 19:43:12.000000 raycut-0.0.1/raycut.egg-info/requires.txt
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)        7 2023-07-27 19:43:12.000000 raycut-0.0.1/raycut.egg-info/top_level.txt
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)       38 2023-07-27 19:43:12.458817 raycut-0.0.1/setup.cfg
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      689 2023-07-27 19:43:01.000000 raycut-0.0.1/setup.py
+drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-27 19:50:54.854313 raycut-0.0.2/
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      533 2023-07-27 19:50:54.854313 raycut-0.0.2/PKG-INFO
+drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-27 19:50:54.854313 raycut-0.0.2/raycut/
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)     2847 2023-07-27 19:49:44.000000 raycut-0.0.2/raycut/__init__.py
+drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-27 19:50:54.854313 raycut-0.0.2/raycut.egg-info/
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      533 2023-07-27 19:50:54.000000 raycut-0.0.2/raycut.egg-info/PKG-INFO
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      176 2023-07-27 19:50:54.000000 raycut-0.0.2/raycut.egg-info/SOURCES.txt
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)        1 2023-07-27 19:50:54.000000 raycut-0.0.2/raycut.egg-info/dependency_links.txt
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)       10 2023-07-27 19:50:54.000000 raycut-0.0.2/raycut.egg-info/requires.txt
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)        7 2023-07-27 19:50:54.000000 raycut-0.0.2/raycut.egg-info/top_level.txt
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)       38 2023-07-27 19:50:54.854313 raycut-0.0.2/setup.cfg
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      689 2023-07-27 19:49:27.000000 raycut-0.0.2/setup.py
```

### Comparing `raycut-0.0.1/PKG-INFO` & `raycut-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raycut
-Version: 0.0.1
+Version: 0.0.2
 Summary: A convenience library for Ray that allows you to run a function on a remote
 Home-page: http://github.com/d33tah/raycut
 Author: Jacek "d33tah" Wielemborek
 Author-email: d33tah@gmail.com
 License: WTFPL
 
 A convenience library for Ray that allows you to run a function on a remote
```

### Comparing `raycut-0.0.1/raycut/__init__.py` & `raycut-0.0.2/raycut/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,18 @@
     - ray start --address=$RAY_HEAD_IP:6379 --object-manager-port=8076
 '''
 
 def init(aws_access_key_id, aws_secret_access_key):
     subprocess.check_call('mkdir -p ~/.aws && pip install boto3 ray && apt update && apt install rsync -y', shell=True)
 
     p = pathlib.Path('~/.aws/').expanduser()
-    (p / 'credentials').rename( p / f'credentials_backup_{time.time()}')
+    try:
+        (p / 'credentials').rename( p / f'credentials_backup_{time.time()}')
+    except FileNotFoundError:
+        pass
     with open(p / 'credentials', 'w') as f:
         f.write(f'''
         # added by raycut
         [default]
         aws_access_key_id = {aws_access_key_id}
         aws_secret_access_key = {aws_secret_access_key}
         ''')
```

### Comparing `raycut-0.0.1/raycut.egg-info/PKG-INFO` & `raycut-0.0.2/raycut.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raycut
-Version: 0.0.1
+Version: 0.0.2
 Summary: A convenience library for Ray that allows you to run a function on a remote
 Home-page: http://github.com/d33tah/raycut
 Author: Jacek "d33tah" Wielemborek
 Author-email: d33tah@gmail.com
 License: WTFPL
 
 A convenience library for Ray that allows you to run a function on a remote
```

### Comparing `raycut-0.0.1/setup.py` & `raycut-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 a remote instance with a single function call.
 '''
 
 from setuptools import setup
 
 setup(
     name='raycut',
-    version='0.0.1',
+    version='0.0.2',
     description=__doc__,
     long_description=long_description,
     url='http://github.com/d33tah/raycut',
     author='Jacek "d33tah" Wielemborek',
     author_email='d33tah@gmail.com',
     license='WTFPL',
     packages=['raycut'],
```

