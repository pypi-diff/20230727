# Comparing `tmp/rospy_yaml_include-0.0.1.tar.gz` & `tmp/rospy_yaml_include-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rospy_yaml_include-0.0.1.tar", last modified: Wed Jul 26 18:41:25 2023, max compression
+gzip compressed data, was "rospy_yaml_include-0.0.2.tar", last modified: Thu Jul 27 16:02:19 2023, max compression
```

## Comparing `rospy_yaml_include-0.0.1.tar` & `rospy_yaml_include-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-26 18:41:25.900408 rospy_yaml_include-0.0.1/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1598 2023-07-26 18:41:25.900408 rospy_yaml_include-0.0.1/PKG-INFO
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1383 2023-07-25 22:16:24.000000 rospy_yaml_include-0.0.1/README.md
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-26 18:41:25.900408 rospy_yaml_include-0.0.1/rospy_yaml_include/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)        0 2023-07-25 22:00:38.000000 rospy_yaml_include-0.0.1/rospy_yaml_include/__init__.py
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     2067 2023-07-26 15:58:47.000000 rospy_yaml_include-0.0.1/rospy_yaml_include/yaml_include.py
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-26 18:41:25.900408 rospy_yaml_include-0.0.1/rospy_yaml_include.egg-info/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1598 2023-07-26 18:41:25.000000 rospy_yaml_include-0.0.1/rospy_yaml_include.egg-info/PKG-INFO
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      307 2023-07-26 18:41:25.000000 rospy_yaml_include-0.0.1/rospy_yaml_include.egg-info/SOURCES.txt
--rw-rw-r--   0 brennan   (1000) brennan   (1000)        1 2023-07-26 18:41:25.000000 rospy_yaml_include-0.0.1/rospy_yaml_include.egg-info/dependency_links.txt
--rw-rw-r--   0 brennan   (1000) brennan   (1000)       19 2023-07-26 18:41:25.000000 rospy_yaml_include-0.0.1/rospy_yaml_include.egg-info/top_level.txt
--rw-rw-r--   0 brennan   (1000) brennan   (1000)       38 2023-07-26 18:41:25.900408 rospy_yaml_include-0.0.1/setup.cfg
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      477 2023-07-26 15:34:53.000000 rospy_yaml_include-0.0.1/setup.py
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-26 18:41:25.900408 rospy_yaml_include-0.0.1/tests/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1297 2023-07-26 15:55:07.000000 rospy_yaml_include-0.0.1/tests/test_path_include.py
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1398 2023-07-25 22:00:38.000000 rospy_yaml_include-0.0.1/tests/test_rospy_include.py
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-27 16:02:19.317545 rospy_yaml_include-0.0.2/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     1598 2023-07-27 16:02:19.317545 rospy_yaml_include-0.0.2/PKG-INFO
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     1383 2023-07-25 22:16:24.000000 rospy_yaml_include-0.0.2/README.md
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-27 16:02:19.317545 rospy_yaml_include-0.0.2/rospy_yaml_include/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)        0 2023-07-25 22:00:38.000000 rospy_yaml_include-0.0.2/rospy_yaml_include/__init__.py
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     3189 2023-07-26 22:21:08.000000 rospy_yaml_include-0.0.2/rospy_yaml_include/yaml_include.py
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-27 16:02:19.317545 rospy_yaml_include-0.0.2/rospy_yaml_include.egg-info/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     1598 2023-07-27 16:02:19.000000 rospy_yaml_include-0.0.2/rospy_yaml_include.egg-info/PKG-INFO
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)      338 2023-07-27 16:02:19.000000 rospy_yaml_include-0.0.2/rospy_yaml_include.egg-info/SOURCES.txt
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)        1 2023-07-27 16:02:19.000000 rospy_yaml_include-0.0.2/rospy_yaml_include.egg-info/dependency_links.txt
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)       19 2023-07-27 16:02:19.000000 rospy_yaml_include-0.0.2/rospy_yaml_include.egg-info/top_level.txt
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)       38 2023-07-27 16:02:19.317545 rospy_yaml_include-0.0.2/setup.cfg
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)      477 2023-07-26 22:22:18.000000 rospy_yaml_include-0.0.2/setup.py
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-27 16:02:19.317545 rospy_yaml_include-0.0.2/tests/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     1297 2023-07-26 15:55:07.000000 rospy_yaml_include-0.0.2/tests/test_path_include.py
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     1327 2023-07-26 22:21:52.000000 rospy_yaml_include-0.0.2/tests/test_relative_include.py
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     1398 2023-07-25 22:00:38.000000 rospy_yaml_include-0.0.2/tests/test_rospy_include.py
```

### Comparing `rospy_yaml_include-0.0.1/PKG-INFO` & `rospy_yaml_include-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rospy_yaml_include
-Version: 0.0.1
+Version: 0.0.2
 Summary: rospy_yaml_include
-Home-page: https://git.whoi.edu/acomms/rospy_yaml_config/
+Home-page: https://git.whoi.edu/acomms/rospy_yaml_include
 Author: WHOI Acomms Group
 Description-Content-Type: text/markdown
 
 # rospy_yaml_include
 
 ## Introduction
```

### Comparing `rospy_yaml_include-0.0.1/README.md` & `rospy_yaml_include-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rospy_yaml_include-0.0.1/rospy_yaml_include.egg-info/PKG-INFO` & `rospy_yaml_include-0.0.2/rospy_yaml_include.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rospy-yaml-include
-Version: 0.0.1
+Version: 0.0.2
 Summary: rospy_yaml_include
-Home-page: https://git.whoi.edu/acomms/rospy_yaml_config/
+Home-page: https://git.whoi.edu/acomms/rospy_yaml_include
 Author: WHOI Acomms Group
 Description-Content-Type: text/markdown
 
 # rospy_yaml_include
 
 ## Introduction
```

### Comparing `rospy_yaml_include-0.0.1/tests/test_path_include.py` & `rospy_yaml_include-0.0.2/tests/test_path_include.py`

 * *Files identical despite different names*

### Comparing `rospy_yaml_include-0.0.1/tests/test_rospy_include.py` & `rospy_yaml_include-0.0.2/tests/test_rospy_include.py`

 * *Files identical despite different names*

