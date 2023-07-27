# Comparing `tmp/masterpass-0.2.3.tar.gz` & `tmp/masterpass-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masterpass-0.2.3.tar", last modified: Thu Jul 27 01:25:16 2023, max compression
+gzip compressed data, was "masterpass-0.2.4.tar", last modified: Thu Jul 27 01:42:32 2023, max compression
```

## Comparing `masterpass-0.2.3.tar` & `masterpass-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-27 01:25:16.148211 masterpass-0.2.3/
--rw-r--r--   0 pedro      (503) staff       (20)     1076 2023-07-16 16:43:11.000000 masterpass-0.2.3/LICENSE
--rw-r--r--   0 pedro      (503) staff       (20)     3009 2023-07-27 01:25:16.148096 masterpass-0.2.3/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)     2369 2023-07-16 22:39:05.000000 masterpass-0.2.3/README.md
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-27 01:25:16.147238 masterpass-0.2.3/master/
--rw-r--r--   0 pedro      (503) staff       (20)       18 2023-07-27 01:24:42.000000 masterpass-0.2.3/master/__init__.py
--rwxr-xr-x   0 pedro      (503) staff       (20)     3737 2023-07-27 01:24:36.000000 masterpass-0.2.3/master/cli.py
--rw-r--r--   0 pedro      (503) staff       (20)      953 2023-07-16 16:09:16.000000 masterpass-0.2.3/master/logger.py
--rw-r--r--   0 pedro      (503) staff       (20)     2179 2023-07-16 16:09:38.000000 masterpass-0.2.3/master/master.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-27 01:25:16.147900 masterpass-0.2.3/masterpass.egg-info/
--rw-r--r--   0 pedro      (503) staff       (20)     3009 2023-07-27 01:25:16.000000 masterpass-0.2.3/masterpass.egg-info/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      266 2023-07-27 01:25:16.000000 masterpass-0.2.3/masterpass.egg-info/SOURCES.txt
--rw-r--r--   0 pedro      (503) staff       (20)        1 2023-07-27 01:25:16.000000 masterpass-0.2.3/masterpass.egg-info/dependency_links.txt
--rw-r--r--   0 pedro      (503) staff       (20)       43 2023-07-27 01:25:16.000000 masterpass-0.2.3/masterpass.egg-info/entry_points.txt
--rw-r--r--   0 pedro      (503) staff       (20)        7 2023-07-27 01:25:16.000000 masterpass-0.2.3/masterpass.egg-info/top_level.txt
--rw-r--r--   0 pedro      (503) staff       (20)       38 2023-07-27 01:25:16.148252 masterpass-0.2.3/setup.cfg
--rw-r--r--   0 pedro      (503) staff       (20)      946 2023-07-16 16:19:44.000000 masterpass-0.2.3/setup.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-27 01:42:32.229213 masterpass-0.2.4/
+-rw-r--r--   0 pedro      (503) staff       (20)     1076 2023-07-16 16:43:11.000000 masterpass-0.2.4/LICENSE
+-rw-r--r--   0 pedro      (503) staff       (20)     3009 2023-07-27 01:42:32.229096 masterpass-0.2.4/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)     2369 2023-07-16 22:39:05.000000 masterpass-0.2.4/README.md
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-27 01:42:32.228006 masterpass-0.2.4/master/
+-rw-r--r--   0 pedro      (503) staff       (20)       18 2023-07-27 01:42:22.000000 masterpass-0.2.4/master/__init__.py
+-rwxr-xr-x   0 pedro      (503) staff       (20)     3737 2023-07-27 01:24:36.000000 masterpass-0.2.4/master/cli.py
+-rw-r--r--   0 pedro      (503) staff       (20)      953 2023-07-16 16:09:16.000000 masterpass-0.2.4/master/logger.py
+-rw-r--r--   0 pedro      (503) staff       (20)     2181 2023-07-27 01:42:17.000000 masterpass-0.2.4/master/master.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-27 01:42:32.228883 masterpass-0.2.4/masterpass.egg-info/
+-rw-r--r--   0 pedro      (503) staff       (20)     3009 2023-07-27 01:42:32.000000 masterpass-0.2.4/masterpass.egg-info/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      266 2023-07-27 01:42:32.000000 masterpass-0.2.4/masterpass.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        1 2023-07-27 01:42:32.000000 masterpass-0.2.4/masterpass.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       43 2023-07-27 01:42:32.000000 masterpass-0.2.4/masterpass.egg-info/entry_points.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        7 2023-07-27 01:42:32.000000 masterpass-0.2.4/masterpass.egg-info/top_level.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       38 2023-07-27 01:42:32.229259 masterpass-0.2.4/setup.cfg
+-rw-r--r--   0 pedro      (503) staff       (20)      946 2023-07-16 16:19:44.000000 masterpass-0.2.4/setup.py
```

### Comparing `masterpass-0.2.3/LICENSE` & `masterpass-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `masterpass-0.2.3/PKG-INFO` & `masterpass-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterpass
-Version: 0.2.3
+Version: 0.2.4
 Summary: Deterministic password generator
 Home-page: https://github.com/jpedro/master
 Download-URL: https://github.com/jpedro/master/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
 Keywords: deterministic password generator
```

### Comparing `masterpass-0.2.3/README.md` & `masterpass-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `masterpass-0.2.3/master/cli.py` & `masterpass-0.2.4/master/cli.py`

 * *Files identical despite different names*

### Comparing `masterpass-0.2.3/master/logger.py` & `masterpass-0.2.4/master/logger.py`

 * *Files identical despite different names*

### Comparing `masterpass-0.2.3/master/master.py` & `masterpass-0.2.4/master/master.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def load(self) -> int:
         if not self.services is None:
             return len(self.services)
 
         self.services = set()
         if not os.path.isfile(self.path):
-            Logger.warn(f"File {self.path} doesn't exit.")
+            # Logger.warn(f"File {self.path} doesn't exit.")
             return 0
 
         with open(self.path, "r") as f:
             for line in f.readlines():
                 self.services.add(line.strip())
 
         Logger.debug(f"Loaded file {self.path}")
```

### Comparing `masterpass-0.2.3/masterpass.egg-info/PKG-INFO` & `masterpass-0.2.4/masterpass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterpass
-Version: 0.2.3
+Version: 0.2.4
 Summary: Deterministic password generator
 Home-page: https://github.com/jpedro/master
 Download-URL: https://github.com/jpedro/master/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
 Keywords: deterministic password generator
```

### Comparing `masterpass-0.2.3/setup.py` & `masterpass-0.2.4/setup.py`

 * *Files identical despite different names*

