# Comparing `tmp/kingunit-0.0.5.tar.gz` & `tmp/kingunit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit/dist/.tmp-j_3w1qs1/kingunit-0.0.5.tar", last modified: Thu Jul 27 06:32:11 2023, max compression
+gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit/dist/.tmp-oauey5l1/kingunit-0.0.6.tar", last modified: Thu Jul 27 06:36:18 2023, max compression
```

## Comparing `kingunit-0.0.5.tar` & `kingunit-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:32:11.453187 kingunit-0.0.5/
--rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-27 06:32:11.452977 kingunit-0.0.5/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      557 2023-07-21 01:16:19.000000 kingunit-0.0.5/README.md
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:32:11.449633 kingunit-0.0.5/kingunit/
--rw-r--r--   0 jiayu      (501) staff       (20)       45 2023-07-21 00:51:02.000000 kingunit-0.0.5/kingunit/__init__.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:32:11.451229 kingunit-0.0.5/kingunit/cmd/
--rw-r--r--   0 jiayu      (501) staff       (20)       18 2023-07-19 01:25:45.000000 kingunit-0.0.5/kingunit/cmd/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)     1417 2023-07-21 00:48:38.000000 kingunit-0.0.5/kingunit/cmd/cmd.py
--rw-r--r--   0 jiayu      (501) staff       (20)      107 2023-07-21 00:49:06.000000 kingunit-0.0.5/kingunit/cmd/main.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:32:11.451834 kingunit-0.0.5/kingunit/config/
--rw-r--r--   0 jiayu      (501) staff       (20)       24 2023-07-19 07:26:28.000000 kingunit-0.0.5/kingunit/config/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)      330 2023-07-21 00:48:38.000000 kingunit-0.0.5/kingunit/config/loader.py
--rw-r--r--   0 jiayu      (501) staff       (20)     4367 2023-07-27 06:18:46.000000 kingunit-0.0.5/kingunit/generator.py
--rw-r--r--   0 jiayu      (501) staff       (20)      699 2023-07-21 01:17:04.000000 kingunit-0.0.5/kingunit/init.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:32:11.452719 kingunit-0.0.5/kingunit/utils/
--rw-r--r--   0 jiayu      (501) staff       (20)       66 2023-07-27 06:19:49.000000 kingunit-0.0.5/kingunit/utils/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)      181 2023-07-18 05:54:49.000000 kingunit-0.0.5/kingunit/utils/loader.py
--rw-r--r--   0 jiayu      (501) staff       (20)     2447 2023-07-21 00:48:38.000000 kingunit-0.0.5/kingunit/utils/mail.py
--rw-r--r--   0 jiayu      (501) staff       (20)      171 2023-07-27 06:19:42.000000 kingunit-0.0.5/kingunit/utils/validator.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:32:11.450548 kingunit-0.0.5/kingunit.egg-info/
--rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-27 06:32:11.000000 kingunit-0.0.5/kingunit.egg-info/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      466 2023-07-27 06:32:11.000000 kingunit-0.0.5/kingunit.egg-info/SOURCES.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-27 06:32:11.000000 kingunit-0.0.5/kingunit.egg-info/dependency_links.txt
--rw-r--r--   0 jiayu      (501) staff       (20)       57 2023-07-27 06:32:11.000000 kingunit-0.0.5/kingunit.egg-info/requires.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-27 06:32:11.000000 kingunit-0.0.5/kingunit.egg-info/top_level.txt
--rw-r--r--   0 jiayu      (501) staff       (20)      493 2023-07-27 06:30:49.000000 kingunit-0.0.5/pyproject.toml
--rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-27 06:32:11.453257 kingunit-0.0.5/setup.cfg
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:36:18.762961 kingunit-0.0.6/
+-rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-27 06:36:18.762735 kingunit-0.0.6/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      557 2023-07-21 01:16:19.000000 kingunit-0.0.6/README.md
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:36:18.759255 kingunit-0.0.6/kingunit/
+-rw-r--r--   0 jiayu      (501) staff       (20)       46 2023-07-27 06:35:32.000000 kingunit-0.0.6/kingunit/__init__.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:36:18.761118 kingunit-0.0.6/kingunit/cmd/
+-rw-r--r--   0 jiayu      (501) staff       (20)       19 2023-07-27 06:35:22.000000 kingunit-0.0.6/kingunit/cmd/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     1417 2023-07-21 00:48:38.000000 kingunit-0.0.6/kingunit/cmd/cmd.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      107 2023-07-21 00:49:06.000000 kingunit-0.0.6/kingunit/cmd/main.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:36:18.761607 kingunit-0.0.6/kingunit/config/
+-rw-r--r--   0 jiayu      (501) staff       (20)       24 2023-07-19 07:26:28.000000 kingunit-0.0.6/kingunit/config/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      330 2023-07-21 00:48:38.000000 kingunit-0.0.6/kingunit/config/loader.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     4367 2023-07-27 06:18:46.000000 kingunit-0.0.6/kingunit/generator.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      699 2023-07-21 01:17:04.000000 kingunit-0.0.6/kingunit/init.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:36:18.762383 kingunit-0.0.6/kingunit/utils/
+-rw-r--r--   0 jiayu      (501) staff       (20)       66 2023-07-27 06:19:49.000000 kingunit-0.0.6/kingunit/utils/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      181 2023-07-18 05:54:49.000000 kingunit-0.0.6/kingunit/utils/loader.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     2447 2023-07-21 00:48:38.000000 kingunit-0.0.6/kingunit/utils/mail.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      171 2023-07-27 06:19:42.000000 kingunit-0.0.6/kingunit/utils/validator.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:36:18.760362 kingunit-0.0.6/kingunit.egg-info/
+-rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-27 06:36:18.000000 kingunit-0.0.6/kingunit.egg-info/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      466 2023-07-27 06:36:18.000000 kingunit-0.0.6/kingunit.egg-info/SOURCES.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-27 06:36:18.000000 kingunit-0.0.6/kingunit.egg-info/dependency_links.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)       57 2023-07-27 06:36:18.000000 kingunit-0.0.6/kingunit.egg-info/requires.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-27 06:36:18.000000 kingunit-0.0.6/kingunit.egg-info/top_level.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)      493 2023-07-27 06:36:13.000000 kingunit-0.0.6/pyproject.toml
+-rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-27 06:36:18.763026 kingunit-0.0.6/setup.cfg
```

### Comparing `kingunit-0.0.5/PKG-INFO` & `kingunit-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit
-Version: 0.0.5
+Version: 0.0.6
 Summary: KingUnit
 Author-email: 东南dnf <zjy2414@outlook.com>
 Project-URL: Home, https://github.com/zjy2414
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # KingUnit
```

### Comparing `kingunit-0.0.5/README.md` & `kingunit-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.5/kingunit/cmd/cmd.py` & `kingunit-0.0.6/kingunit/cmd/cmd.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.5/kingunit/generator.py` & `kingunit-0.0.6/kingunit/generator.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.5/kingunit/init.py` & `kingunit-0.0.6/kingunit/init.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.5/kingunit/utils/mail.py` & `kingunit-0.0.6/kingunit/utils/mail.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.5/kingunit.egg-info/PKG-INFO` & `kingunit-0.0.6/kingunit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit
-Version: 0.0.5
+Version: 0.0.6
 Summary: KingUnit
 Author-email: 东南dnf <zjy2414@outlook.com>
 Project-URL: Home, https://github.com/zjy2414
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # KingUnit
```

