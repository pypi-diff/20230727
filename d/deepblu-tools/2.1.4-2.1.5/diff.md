# Comparing `tmp/deepblu-tools-2.1.4.tar.gz` & `tmp/deepblu-tools-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepblu-tools-2.1.4.tar", last modified: Sat Jun 24 17:47:32 2023, max compression
+gzip compressed data, was "deepblu-tools-2.1.5.tar", last modified: Thu Jul 27 17:57:16 2023, max compression
```

## Comparing `deepblu-tools-2.1.4.tar` & `deepblu-tools-2.1.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-24 17:47:32.865215 deepblu-tools-2.1.4/
--rwxrwxr-x   0 sander    (1000) sander    (1000)       71 2022-08-07 18:17:34.000000 deepblu-tools-2.1.4/.gitignore
--rw-rw-r--   0 sander    (1000) sander    (1000)      972 2023-01-30 23:25:43.000000 deepblu-tools-2.1.4/.pre-commit-config.yaml
--rwxrwxr-x   0 sander    (1000) sander    (1000)    35147 2022-08-07 18:17:34.000000 deepblu-tools-2.1.4/LICENSE
--rw-rw-r--   0 sander    (1000) sander    (1000)     3820 2023-06-24 17:47:32.865215 deepblu-tools-2.1.4/PKG-INFO
--rwxrwxr-x   0 sander    (1000) sander    (1000)     3322 2023-01-31 10:18:03.000000 deepblu-tools-2.1.4/README.md
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-24 17:47:32.861215 deepblu-tools-2.1.4/done/
--rwxrwxr-x   0 sander    (1000) sander    (1000)      106 2023-01-30 23:26:08.000000 deepblu-tools-2.1.4/done/.htaccess
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-24 17:47:32.861215 deepblu-tools-2.1.4/extra/
--rwxrwxr-x   0 sander    (1000) sander    (1000)      878 2023-01-30 23:26:08.000000 deepblu-tools-2.1.4/extra/autofollow.js
--rwxrwxr-x   0 sander    (1000) sander    (1000)     3828 2023-01-30 23:30:15.000000 deepblu-tools-2.1.4/extra/autoliker.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      249 2023-01-30 22:00:46.000000 deepblu-tools-2.1.4/pyproject.toml
--rw-rw-r--   0 sander    (1000) sander    (1000)      424 2023-06-24 11:11:30.000000 deepblu-tools-2.1.4/requirements.txt
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-24 17:47:32.861215 deepblu-tools-2.1.4/schemas/
--rwxrwxr-x   0 sander    (1000) sander    (1000)    75745 2022-08-07 18:17:34.000000 deepblu-tools-2.1.4/schemas/uddf_3.2.2.xsd
--rw-rw-r--   0 sander    (1000) sander    (1000)     1002 2023-06-24 17:47:32.865215 deepblu-tools-2.1.4/setup.cfg
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-24 17:47:32.857215 deepblu-tools-2.1.4/src/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-24 17:47:32.861215 deepblu-tools-2.1.4/src/deepblu_tools/
--rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-08-07 18:17:34.000000 deepblu-tools-2.1.4/src/deepblu_tools/__init__.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-24 17:47:32.861215 deepblu-tools-2.1.4/src/deepblu_tools/bin/
--rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-08-07 18:17:34.000000 deepblu-tools-2.1.4/src/deepblu_tools/bin/__init__.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     3802 2023-01-30 23:30:25.000000 deepblu-tools-2.1.4/src/deepblu_tools/bin/cli.py
--rwxrwxr-x   0 sander    (1000) sander    (1000)     2847 2023-01-30 23:26:08.000000 deepblu-tools-2.1.4/src/deepblu_tools/deepblu_api.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-24 17:47:32.861215 deepblu-tools-2.1.4/src/deepblu_tools/models/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-24 17:47:32.865215 deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/
--rw-rw-r--   0 sander    (1000) sander    (1000)      393 2022-08-07 18:17:34.000000 deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/__init__.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      381 2022-09-17 19:35:57.000000 deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/buddy.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      296 2022-08-07 18:17:34.000000 deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/dive_base.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      842 2022-09-25 10:03:28.000000 deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/dive_gear.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     3539 2023-01-30 23:32:27.000000 deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/dive_log.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      561 2023-01-30 23:26:08.000000 deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/dive_profile.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      754 2023-01-30 23:26:09.000000 deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/dive_spot.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      873 2023-01-30 23:26:09.000000 deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/equipment.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      477 2022-08-07 18:17:34.000000 deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/gas_definition.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     4334 2023-01-30 23:31:59.000000 deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/log_book.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1113 2023-01-30 23:26:09.000000 deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/medium.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1487 2023-06-24 17:46:46.000000 deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/user.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1813 2023-01-30 23:31:52.000000 deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/way_point.py
--rw-rw-r--   0 sander    (1000) sander    (1000)   129159 2023-01-30 23:26:17.000000 deepblu-tools-2.1.4/src/deepblu_tools/models/uddf.py
--rwxrwxr-x   0 sander    (1000) sander    (1000)      628 2022-08-07 18:17:34.000000 deepblu-tools-2.1.4/src/deepblu_tools/utils.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-24 17:47:32.861215 deepblu-tools-2.1.4/src/deepblu_tools.egg-info/
--rw-rw-r--   0 sander    (1000) sander    (1000)     3820 2023-06-24 17:47:32.000000 deepblu-tools-2.1.4/src/deepblu_tools.egg-info/PKG-INFO
--rw-rw-r--   0 sander    (1000) sander    (1000)     1287 2023-06-24 17:47:32.000000 deepblu-tools-2.1.4/src/deepblu_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-24 17:47:32.000000 deepblu-tools-2.1.4/src/deepblu_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)       62 2023-06-24 17:47:32.000000 deepblu-tools-2.1.4/src/deepblu_tools.egg-info/entry_points.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2022-08-07 17:46:01.000000 deepblu-tools-2.1.4/src/deepblu_tools.egg-info/not-zip-safe
--rw-rw-r--   0 sander    (1000) sander    (1000)       76 2023-06-24 17:47:32.000000 deepblu-tools-2.1.4/src/deepblu_tools.egg-info/requires.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)       14 2023-06-24 17:47:32.000000 deepblu-tools-2.1.4/src/deepblu_tools.egg-info/top_level.txt
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-24 17:47:32.865215 deepblu-tools-2.1.4/web/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-24 17:47:32.865215 deepblu-tools-2.1.4/web/img/
--rwxrwxr-x   0 sander    (1000) sander    (1000)   159965 2022-08-07 18:17:34.000000 deepblu-tools-2.1.4/web/img/imported_into_subsurface.jpg
--rwxrwxr-x   0 sander    (1000) sander    (1000)     5383 2023-01-30 23:26:08.000000 deepblu-tools-2.1.4/web/index.php
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-07-27 17:57:16.602388 deepblu-tools-2.1.5/
+-rwxrwxr-x   0 sander    (1000) sander    (1000)       71 2022-08-07 18:17:34.000000 deepblu-tools-2.1.5/.gitignore
+-rw-rw-r--   0 sander    (1000) sander    (1000)      972 2023-01-30 23:25:43.000000 deepblu-tools-2.1.5/.pre-commit-config.yaml
+-rwxrwxr-x   0 sander    (1000) sander    (1000)    35147 2022-08-07 18:17:34.000000 deepblu-tools-2.1.5/LICENSE
+-rw-rw-r--   0 sander    (1000) sander    (1000)     3820 2023-07-27 17:57:16.602388 deepblu-tools-2.1.5/PKG-INFO
+-rwxrwxr-x   0 sander    (1000) sander    (1000)     3322 2023-01-31 10:18:03.000000 deepblu-tools-2.1.5/README.md
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-07-27 17:57:16.582388 deepblu-tools-2.1.5/done/
+-rwxrwxr-x   0 sander    (1000) sander    (1000)      106 2023-01-30 23:26:08.000000 deepblu-tools-2.1.5/done/.htaccess
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-07-27 17:57:16.586388 deepblu-tools-2.1.5/extra/
+-rwxrwxr-x   0 sander    (1000) sander    (1000)      878 2023-01-30 23:26:08.000000 deepblu-tools-2.1.5/extra/autofollow.js
+-rwxrwxr-x   0 sander    (1000) sander    (1000)     3828 2023-01-30 23:30:15.000000 deepblu-tools-2.1.5/extra/autoliker.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      249 2023-01-30 22:00:46.000000 deepblu-tools-2.1.5/pyproject.toml
+-rw-rw-r--   0 sander    (1000) sander    (1000)      425 2023-07-27 17:55:42.000000 deepblu-tools-2.1.5/requirements.txt
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-07-27 17:57:16.586388 deepblu-tools-2.1.5/schemas/
+-rwxrwxr-x   0 sander    (1000) sander    (1000)    75745 2022-08-07 18:17:34.000000 deepblu-tools-2.1.5/schemas/uddf_3.2.2.xsd
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1002 2023-07-27 17:57:16.602388 deepblu-tools-2.1.5/setup.cfg
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-07-27 17:57:16.582388 deepblu-tools-2.1.5/src/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-07-27 17:57:16.586388 deepblu-tools-2.1.5/src/deepblu_tools/
+-rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-08-07 18:17:34.000000 deepblu-tools-2.1.5/src/deepblu_tools/__init__.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-07-27 17:57:16.590388 deepblu-tools-2.1.5/src/deepblu_tools/bin/
+-rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-08-07 18:17:34.000000 deepblu-tools-2.1.5/src/deepblu_tools/bin/__init__.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     3802 2023-01-30 23:30:25.000000 deepblu-tools-2.1.5/src/deepblu_tools/bin/cli.py
+-rwxrwxr-x   0 sander    (1000) sander    (1000)     2847 2023-01-30 23:26:08.000000 deepblu-tools-2.1.5/src/deepblu_tools/deepblu_api.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-07-27 17:57:16.590388 deepblu-tools-2.1.5/src/deepblu_tools/models/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-07-27 17:57:16.598388 deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/
+-rw-rw-r--   0 sander    (1000) sander    (1000)      393 2022-08-07 18:17:34.000000 deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/__init__.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      381 2022-09-17 19:35:57.000000 deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/buddy.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      296 2022-08-07 18:17:34.000000 deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/dive_base.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      842 2022-09-25 10:03:28.000000 deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/dive_gear.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     3539 2023-01-30 23:32:27.000000 deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/dive_log.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      561 2023-01-30 23:26:08.000000 deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/dive_profile.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      754 2023-01-30 23:26:09.000000 deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/dive_spot.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      873 2023-01-30 23:26:09.000000 deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/equipment.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      477 2022-08-07 18:17:34.000000 deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/gas_definition.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4334 2023-01-30 23:31:59.000000 deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/log_book.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1113 2023-01-30 23:26:09.000000 deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/medium.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1487 2023-06-24 17:46:46.000000 deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/user.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1813 2023-01-30 23:31:52.000000 deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/way_point.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)   129159 2023-01-30 23:26:17.000000 deepblu-tools-2.1.5/src/deepblu_tools/models/uddf.py
+-rwxrwxr-x   0 sander    (1000) sander    (1000)      628 2022-08-07 18:17:34.000000 deepblu-tools-2.1.5/src/deepblu_tools/utils.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-07-27 17:57:16.590388 deepblu-tools-2.1.5/src/deepblu_tools.egg-info/
+-rw-rw-r--   0 sander    (1000) sander    (1000)     3820 2023-07-27 17:57:16.000000 deepblu-tools-2.1.5/src/deepblu_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1287 2023-07-27 17:57:16.000000 deepblu-tools-2.1.5/src/deepblu_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-07-27 17:57:16.000000 deepblu-tools-2.1.5/src/deepblu_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)       62 2023-07-27 17:57:16.000000 deepblu-tools-2.1.5/src/deepblu_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2022-08-07 17:46:01.000000 deepblu-tools-2.1.5/src/deepblu_tools.egg-info/not-zip-safe
+-rw-rw-r--   0 sander    (1000) sander    (1000)       76 2023-07-27 17:57:16.000000 deepblu-tools-2.1.5/src/deepblu_tools.egg-info/requires.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)       14 2023-07-27 17:57:16.000000 deepblu-tools-2.1.5/src/deepblu_tools.egg-info/top_level.txt
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-07-27 17:57:16.598388 deepblu-tools-2.1.5/web/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-07-27 17:57:16.598388 deepblu-tools-2.1.5/web/img/
+-rwxrwxr-x   0 sander    (1000) sander    (1000)   159965 2022-08-07 18:17:34.000000 deepblu-tools-2.1.5/web/img/imported_into_subsurface.jpg
+-rwxrwxr-x   0 sander    (1000) sander    (1000)     5383 2023-01-30 23:26:08.000000 deepblu-tools-2.1.5/web/index.php
```

### Comparing `deepblu-tools-2.1.4/.pre-commit-config.yaml` & `deepblu-tools-2.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/LICENSE` & `deepblu-tools-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/PKG-INFO` & `deepblu-tools-2.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepblu-tools
-Version: 2.1.4
+Version: 2.1.5
 Summary: Deepblu Tools
 Home-page: https://github.com/bluppfisk/deepblu-tools/
 Author: Sander Van de Moortel
 Author-email: sander.vandemoortel@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://github.com/bluppfisk/deepblu-tools/
 Platform: any
```

### Comparing `deepblu-tools-2.1.4/README.md` & `deepblu-tools-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/extra/autofollow.js` & `deepblu-tools-2.1.5/extra/autofollow.js`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/extra/autoliker.py` & `deepblu-tools-2.1.5/extra/autoliker.py`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/schemas/uddf_3.2.2.xsd` & `deepblu-tools-2.1.5/schemas/uddf_3.2.2.xsd`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/setup.cfg` & `deepblu-tools-2.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/src/deepblu_tools/bin/cli.py` & `deepblu-tools-2.1.5/src/deepblu_tools/bin/cli.py`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/src/deepblu_tools/deepblu_api.py` & `deepblu-tools-2.1.5/src/deepblu_tools/deepblu_api.py`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/dive_gear.py` & `deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/dive_gear.py`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/dive_log.py` & `deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/dive_log.py`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/dive_profile.py` & `deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/dive_profile.py`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/dive_spot.py` & `deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/dive_spot.py`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/equipment.py` & `deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/equipment.py`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/log_book.py` & `deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/log_book.py`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/medium.py` & `deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/medium.py`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/user.py` & `deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/user.py`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/src/deepblu_tools/models/deepblu/way_point.py` & `deepblu-tools-2.1.5/src/deepblu_tools/models/deepblu/way_point.py`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/src/deepblu_tools/models/uddf.py` & `deepblu-tools-2.1.5/src/deepblu_tools/models/uddf.py`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/src/deepblu_tools/utils.py` & `deepblu-tools-2.1.5/src/deepblu_tools/utils.py`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/src/deepblu_tools.egg-info/PKG-INFO` & `deepblu-tools-2.1.5/src/deepblu_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepblu-tools
-Version: 2.1.4
+Version: 2.1.5
 Summary: Deepblu Tools
 Home-page: https://github.com/bluppfisk/deepblu-tools/
 Author: Sander Van de Moortel
 Author-email: sander.vandemoortel@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://github.com/bluppfisk/deepblu-tools/
 Platform: any
```

### Comparing `deepblu-tools-2.1.4/src/deepblu_tools.egg-info/SOURCES.txt` & `deepblu-tools-2.1.5/src/deepblu_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/web/img/imported_into_subsurface.jpg` & `deepblu-tools-2.1.5/web/img/imported_into_subsurface.jpg`

 * *Files identical despite different names*

### Comparing `deepblu-tools-2.1.4/web/index.php` & `deepblu-tools-2.1.5/web/index.php`

 * *Files identical despite different names*

