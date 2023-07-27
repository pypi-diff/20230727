# Comparing `tmp/awsx-0.4.tar.gz` & `tmp/awsx-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsx-0.4.tar", last modified: Tue Jul  4 13:45:17 2023, max compression
+gzip compressed data, was "awsx-0.5.tar", last modified: Thu Jul 27 00:24:50 2023, max compression
```

## Comparing `awsx-0.4.tar` & `awsx-0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mini       (501) staff       (20)        0 2023-07-04 13:45:17.521254 awsx-0.4/
--rw-r--r--   0 mini       (501) staff       (20)       46 2023-07-04 13:45:17.521148 awsx-0.4/PKG-INFO
-drwxr-xr-x   0 mini       (501) staff       (20)        0 2023-07-04 13:45:17.521025 awsx-0.4/awsx.egg-info/
--rw-r--r--   0 mini       (501) staff       (20)       46 2023-07-04 13:45:17.000000 awsx-0.4/awsx.egg-info/PKG-INFO
--rw-r--r--   0 mini       (501) staff       (20)      186 2023-07-04 13:45:17.000000 awsx-0.4/awsx.egg-info/SOURCES.txt
--rw-r--r--   0 mini       (501) staff       (20)        1 2023-07-04 13:45:17.000000 awsx-0.4/awsx.egg-info/dependency_links.txt
--rw-r--r--   0 mini       (501) staff       (20)       41 2023-07-04 13:45:17.000000 awsx-0.4/awsx.egg-info/entry_points.txt
--rw-r--r--   0 mini       (501) staff       (20)       12 2023-07-04 13:45:17.000000 awsx-0.4/awsx.egg-info/requires.txt
--rw-r--r--   0 mini       (501) staff       (20)        5 2023-07-04 13:45:17.000000 awsx-0.4/awsx.egg-info/top_level.txt
--rw-r--r--   0 mini       (501) staff       (20)      890 2023-07-04 13:44:27.000000 awsx-0.4/main.py
--rw-r--r--   0 mini       (501) staff       (20)       38 2023-07-04 13:45:17.521282 awsx-0.4/setup.cfg
--rw-r--r--   0 mini       (501) staff       (20)      247 2023-07-04 13:45:16.000000 awsx-0.4/setup.py
+drwxr-xr-x   0 mini       (501) staff       (20)        0 2023-07-27 00:24:50.160822 awsx-0.5/
+-rw-r--r--   0 mini       (501) staff       (20)       46 2023-07-27 00:24:50.160704 awsx-0.5/PKG-INFO
+drwxr-xr-x   0 mini       (501) staff       (20)        0 2023-07-27 00:24:50.160563 awsx-0.5/awsx.egg-info/
+-rw-r--r--   0 mini       (501) staff       (20)       46 2023-07-27 00:24:50.000000 awsx-0.5/awsx.egg-info/PKG-INFO
+-rw-r--r--   0 mini       (501) staff       (20)      186 2023-07-27 00:24:50.000000 awsx-0.5/awsx.egg-info/SOURCES.txt
+-rw-r--r--   0 mini       (501) staff       (20)        1 2023-07-27 00:24:50.000000 awsx-0.5/awsx.egg-info/dependency_links.txt
+-rw-r--r--   0 mini       (501) staff       (20)       41 2023-07-27 00:24:50.000000 awsx-0.5/awsx.egg-info/entry_points.txt
+-rw-r--r--   0 mini       (501) staff       (20)       12 2023-07-27 00:24:50.000000 awsx-0.5/awsx.egg-info/requires.txt
+-rw-r--r--   0 mini       (501) staff       (20)        5 2023-07-27 00:24:50.000000 awsx-0.5/awsx.egg-info/top_level.txt
+-rw-r--r--   0 mini       (501) staff       (20)      803 2023-07-27 00:23:43.000000 awsx-0.5/main.py
+-rw-r--r--   0 mini       (501) staff       (20)       38 2023-07-27 00:24:50.160855 awsx-0.5/setup.cfg
+-rw-r--r--   0 mini       (501) staff       (20)      247 2023-07-27 00:23:43.000000 awsx-0.5/setup.py
```

### Comparing `awsx-0.4/main.py` & `awsx-0.5/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,20 +18,19 @@
     # print("ARN: ", response['Arn'])
 
 
 @click.command()
 def role_token():
     session = boto3.Session()
     credentials = session.get_credentials()
-    current_credentials = credentials.get_frozen_credentials()
 
     credential = {
-        'access_key': current_credentials.access_key,
-        'secret_key': current_credentials.secret_key,
-        'token': current_credentials.token
+        'access_key': credentials.access_key,
+        'secret_key': credentials.secret_key,
+        'token': credentials.token
     }
 
     print(identity_arn())
     print(credential)
 
 
 if __name__ == "__main__":
```

