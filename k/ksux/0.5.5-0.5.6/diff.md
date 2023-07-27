# Comparing `tmp/ksux-0.5.5.tar.gz` & `tmp/ksux-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ksux-0.5.5.tar", last modified: Thu Jul 27 12:45:58 2023, max compression
+gzip compressed data, was "ksux-0.5.6.tar", last modified: Thu Jul 27 13:31:59 2023, max compression
```

## Comparing `ksux-0.5.5.tar` & `ksux-0.5.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:58.040868 ksux-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-27 12:45:46.000000 ksux-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 12:45:46.000000 ksux-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-27 12:45:58.040868 ksux-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-27 12:45:46.000000 ksux-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-27 12:45:51.000000 ksux-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:45:58.040868 ksux-0.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:58.036868 ksux-0.5.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:46.000000 ksux-0.5.5/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:58.036868 ksux-0.5.5/src/ksux/
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-27 12:45:51.000000 ksux-0.5.5/src/ksux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:58.036868 ksux-0.5.5/src/ksux/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/src/create_manifests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/src/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/src/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/src/save_manifests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/src/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:58.036868 ksux-0.5.5/src/ksux/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/tests/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/tests/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/tests/test_read_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:58.036868 ksux-0.5.5/src/ksux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-27 12:45:58.000000 ksux-0.5.5/src/ksux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-27 12:45:58.000000 ksux-0.5.5/src/ksux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:45:58.000000 ksux-0.5.5/src/ksux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 12:45:58.000000 ksux-0.5.5/src/ksux.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-27 12:45:58.000000 ksux-0.5.5/src/ksux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 12:45:58.000000 ksux-0.5.5/src/ksux.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:59.182695 ksux-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-27 13:31:45.000000 ksux-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 13:31:45.000000 ksux-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-27 13:31:59.182695 ksux-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-27 13:31:45.000000 ksux-0.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-27 13:31:52.000000 ksux-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:31:59.182695 ksux-0.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:59.178695 ksux-0.5.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:45.000000 ksux-0.5.6/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:59.182695 ksux-0.5.6/src/ksux/
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-27 13:31:52.000000 ksux-0.5.6/src/ksux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 13:31:45.000000 ksux-0.5.6/src/ksux/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:59.182695 ksux-0.5.6/src/ksux/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-27 13:31:45.000000 ksux-0.5.6/src/ksux/src/create_manifests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-27 13:31:45.000000 ksux-0.5.6/src/ksux/src/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-27 13:31:45.000000 ksux-0.5.6/src/ksux/src/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-27 13:31:45.000000 ksux-0.5.6/src/ksux/src/save_manifests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-27 13:31:45.000000 ksux-0.5.6/src/ksux/src/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:59.182695 ksux-0.5.6/src/ksux/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:45.000000 ksux-0.5.6/src/ksux/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-27 13:31:45.000000 ksux-0.5.6/src/ksux/tests/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-27 13:31:45.000000 ksux-0.5.6/src/ksux/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-27 13:31:45.000000 ksux-0.5.6/src/ksux/tests/test_read_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:59.182695 ksux-0.5.6/src/ksux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-27 13:31:59.000000 ksux-0.5.6/src/ksux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-27 13:31:59.000000 ksux-0.5.6/src/ksux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:31:59.000000 ksux-0.5.6/src/ksux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 13:31:59.000000 ksux-0.5.6/src/ksux.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-27 13:31:59.000000 ksux-0.5.6/src/ksux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 13:31:59.000000 ksux-0.5.6/src/ksux.egg-info/top_level.txt
```

### Comparing `ksux-0.5.5/LICENSE` & `ksux-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ksux-0.5.5/PKG-INFO` & `ksux-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksux
-Version: 0.5.5
+Version: 0.5.6
 Summary: Easy customization of kubernetes manifests
 Author: Tomas Sladecek
 License: MIT License
         
         Copyright (c) 2022 Tomáš Sládeček
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ksux Version: 0.5.5 Summary: Easy customization of
+Metadata-Version: 2.1 Name: ksux Version: 0.5.6 Summary: Easy customization of
 kubernetes manifests Author: Tomas Sladecek License: MIT License Copyright (c)
 2022 TomÃ¡Å¡ SlÃ¡deÄek Permission is hereby granted, free of charge, to any
 person obtaining a copy of this software and associated documentation files
 (the "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
```

### Comparing `ksux-0.5.5/README.md` & `ksux-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `ksux-0.5.5/pyproject.toml` & `ksux-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ksux"
-version = "0.5.5"
+version = "0.5.6"
 authors = [
     { name = "Tomas Sladecek" }
 ]
 description = "Easy customization of kubernetes manifests"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `ksux-0.5.5/src/ksux/__init__.py` & `ksux-0.5.6/src/ksux/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     parser.add_argument('--dry-run', help='Print manifests to stdout', action="store_true")
     parser.add_argument('-q', '--quiet', help='Do not print debug, info and warning messages', action='store_true')
     parser.add_argument('--version', help='Package version', action="store_true")
 
     args = parser.parse_args()
 
     if args.version:
-        print('0.5.5')
+        print('0.5.6')
         exit(0)
 
     if args.quiet:
         logging.root.setLevel(logging.ERROR)
     else:
         logging.root.setLevel(logging.INFO)
```

### Comparing `ksux-0.5.5/src/ksux/src/create_manifests.py` & `ksux-0.5.6/src/ksux/src/create_manifests.py`

 * *Files identical despite different names*

### Comparing `ksux-0.5.5/src/ksux/src/patch.py` & `ksux-0.5.6/src/ksux/src/patch.py`

 * *Files identical despite different names*

### Comparing `ksux-0.5.5/src/ksux/src/read_file.py` & `ksux-0.5.6/src/ksux/src/read_file.py`

 * *Files identical despite different names*

### Comparing `ksux-0.5.5/src/ksux/src/save_manifests.py` & `ksux-0.5.6/src/ksux/src/save_manifests.py`

 * *Files identical despite different names*

### Comparing `ksux-0.5.5/src/ksux/src/schemas.py` & `ksux-0.5.6/src/ksux/src/schemas.py`

 * *Files identical despite different names*

### Comparing `ksux-0.5.5/src/ksux/tests/test_patch.py` & `ksux-0.5.6/src/ksux/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `ksux-0.5.5/src/ksux/tests/test_read_file.py` & `ksux-0.5.6/src/ksux/tests/test_read_file.py`

 * *Files identical despite different names*

### Comparing `ksux-0.5.5/src/ksux.egg-info/PKG-INFO` & `ksux-0.5.6/src/ksux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksux
-Version: 0.5.5
+Version: 0.5.6
 Summary: Easy customization of kubernetes manifests
 Author: Tomas Sladecek
 License: MIT License
         
         Copyright (c) 2022 Tomáš Sládeček
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ksux Version: 0.5.5 Summary: Easy customization of
+Metadata-Version: 2.1 Name: ksux Version: 0.5.6 Summary: Easy customization of
 kubernetes manifests Author: Tomas Sladecek License: MIT License Copyright (c)
 2022 TomÃ¡Å¡ SlÃ¡deÄek Permission is hereby granted, free of charge, to any
 person obtaining a copy of this software and associated documentation files
 (the "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
```

### Comparing `ksux-0.5.5/src/ksux.egg-info/SOURCES.txt` & `ksux-0.5.6/src/ksux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

