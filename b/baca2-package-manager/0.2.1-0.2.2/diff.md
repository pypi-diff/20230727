# Comparing `tmp/baca2-package-manager-0.2.1.tar.gz` & `tmp/baca2-package-manager-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baca2-package-manager-0.2.1.tar", last modified: Thu Jul 27 14:00:35 2023, max compression
+gzip compressed data, was "baca2-package-manager-0.2.2.tar", last modified: Thu Jul 27 15:11:45 2023, max compression
```

## Comparing `baca2-package-manager-0.2.1.tar` & `baca2-package-manager-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 14:00:35.969170 baca2-package-manager-0.2.1/
--rw-rw-rw-   0        0        0    35823 2023-07-26 17:19:31.000000 baca2-package-manager-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      760 2023-07-27 14:00:35.969170 baca2-package-manager-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-07-26 18:31:13.000000 baca2-package-manager-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 14:00:35.945813 baca2-package-manager-0.2.1/baca2PackageManager/
--rw-rw-rw-   0        0        0      748 2023-07-26 18:26:18.000000 baca2-package-manager-0.2.1/baca2PackageManager/__init__.py
--rw-rw-rw-   0        0        0       83 2023-07-26 17:55:56.000000 baca2-package-manager-0.2.1/baca2PackageManager/consts.py
--rw-rw-rw-   0        0        0    24181 2023-07-27 13:53:59.000000 baca2-package-manager-0.2.1/baca2PackageManager/manager.py
--rw-rw-rw-   0        0        0      133 2023-07-26 17:58:18.000000 baca2-package-manager-0.2.1/baca2PackageManager/manager_exceptions.py
--rw-rw-rw-   0        0        0     5940 2023-07-26 18:08:03.000000 baca2-package-manager-0.2.1/baca2PackageManager/validators.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:00:35.965670 baca2-package-manager-0.2.1/baca2_package_manager.egg-info/
--rw-rw-rw-   0        0        0      760 2023-07-27 14:00:35.000000 baca2-package-manager-0.2.1/baca2_package_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-07-27 14:00:35.000000 baca2-package-manager-0.2.1/baca2_package_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 14:00:35.000000 baca2-package-manager-0.2.1/baca2_package_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 14:00:35.000000 baca2-package-manager-0.2.1/baca2_package_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-27 14:00:35.000000 baca2-package-manager-0.2.1/baca2_package_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 14:00:35.969170 baca2-package-manager-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      722 2023-07-27 13:59:24.000000 baca2-package-manager-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:00:35.967754 baca2-package-manager-0.2.1/tests/
--rw-rw-rw-   0        0        0    24517 2023-07-27 13:54:21.000000 baca2-package-manager-0.2.1/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:11:45.862127 baca2-package-manager-0.2.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-26 17:19:31.000000 baca2-package-manager-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      760 2023-07-27 15:11:45.862127 baca2-package-manager-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-07-26 18:31:13.000000 baca2-package-manager-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 15:11:45.797762 baca2-package-manager-0.2.2/baca2PackageManager/
+-rw-rw-rw-   0        0        0      748 2023-07-26 18:26:18.000000 baca2-package-manager-0.2.2/baca2PackageManager/__init__.py
+-rw-rw-rw-   0        0        0       83 2023-07-26 17:55:56.000000 baca2-package-manager-0.2.2/baca2PackageManager/consts.py
+-rw-rw-rw-   0        0        0    24899 2023-07-27 15:10:38.000000 baca2-package-manager-0.2.2/baca2PackageManager/manager.py
+-rw-rw-rw-   0        0        0      133 2023-07-26 17:58:18.000000 baca2-package-manager-0.2.2/baca2PackageManager/manager_exceptions.py
+-rw-rw-rw-   0        0        0     6069 2023-07-27 15:10:38.000000 baca2-package-manager-0.2.2/baca2PackageManager/validators.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:11:45.857770 baca2-package-manager-0.2.2/baca2_package_manager.egg-info/
+-rw-rw-rw-   0        0        0      760 2023-07-27 15:11:45.000000 baca2-package-manager-0.2.2/baca2_package_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-07-27 15:11:45.000000 baca2-package-manager-0.2.2/baca2_package_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 15:11:45.000000 baca2-package-manager-0.2.2/baca2_package_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 15:11:45.000000 baca2-package-manager-0.2.2/baca2_package_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-27 15:11:45.000000 baca2-package-manager-0.2.2/baca2_package_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 15:11:45.863133 baca2-package-manager-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-07-27 15:11:38.000000 baca2-package-manager-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:11:45.860286 baca2-package-manager-0.2.2/tests/
+-rw-rw-rw-   0        0        0    24517 2023-07-27 13:54:21.000000 baca2-package-manager-0.2.2/tests/tests.py
```

### Comparing `baca2-package-manager-0.2.1/LICENSE` & `baca2-package-manager-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.2.1/PKG-INFO` & `baca2-package-manager-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baca2-package-manager
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package manager for Baca2 project
 Home-page: https://github.com/BaCa2-project/BaCa2-package-manager
 Author: Baca2 Team
 Author-email: bartosz.deptula@student.uj.edu.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `baca2-package-manager-0.2.1/baca2PackageManager/__init__.py` & `baca2-package-manager-0.2.2/baca2PackageManager/__init__.py`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.2.1/baca2PackageManager/manager.py` & `baca2-package-manager-0.2.2/baca2PackageManager/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from os import remove, replace, walk, mkdir, rename, listdir
 from shutil import rmtree, copytree
 from yaml import safe_load, dump
 from re import match
 
 from .validators import isAny, isNone, isInt, isIntBetween, isFloat, isFloatBetween, isStr, is_, isIn, isShorter, \
-    isDict, isPath, isSize, isList, memory_converting, valid_memory_size
+    isDict, isPath, isSize, isList, memory_converting, valid_memory_size, isBool
 from .consts import SUPPORTED_EXTENSIONS, BASE_DIR
 from .manager_exceptions import NoTestFound, NoSetFound, TestExistError
 
 __all__ = ['Package', 'TSet', 'TestF']
 
 def merge_settings(default: dict, to_add: dict) -> dict:
     """
@@ -143,49 +143,56 @@
     It's a class that represents a package.
     """
 
     #: Largest file acceptable to upload
     MAX_SUBMIT_MEMORY = '10G'
     #: Largest acceptable submit time
     MAX_SUBMIT_TIME = 600
+    MAX_CPUS = 16
     SETTINGS_VALIDATION = {
         'title': [[isStr]],
         'points': [[isInt], [isFloat]],
         'memory_limit': [[isSize, MAX_SUBMIT_MEMORY]],
         'time_limit': [[isIntBetween, 0, MAX_SUBMIT_TIME], [isFloatBetween, 0, MAX_SUBMIT_TIME]],
         'allowedExtensions': [[isIn, *SUPPORTED_EXTENSIONS], [isList, [isIn, *SUPPORTED_EXTENSIONS]]],
         'hinter': [[isNone], [isPath]],
         'checker': [[isNone], [isPath]],
-        'test_generator': [[isNone], [isPath]]
+        'test_generator': [[isNone], [isPath]],
+        'network': [[isNone], [isBool]],
+        'cpus': [[isNone], [isIntBetween, 1, MAX_CPUS]]
     }
     """
     Validation for ``Package`` settings.
     
     Available options are:
     
         * ``title``: package name
         * ``points``: maximum amount of points to earn
         * ``memory_limit``: is a memory limit
         * ``time_limit``: is a time limit
         * ``allowedExtensions``: extensions witch are accepted
         * ``hinter``: is a path or None value to actual hinter
         * ``checker``: is a path or None value to actual checker
         * ``test_generator``: is a path or None value to actual generator
+        * ``network``: is a bool value to allow network access
+        * ``cpus``: is a number of cpus to use
     """
 
     #: Default values for Package settings
     DEFAULT_SETTINGS = {
         'title': 'p',
         'points': 0,
         'memory_limit': '512M',
         'time_limit': 10,
         'allowedExtensions': 'cpp',
         'hinter': None,
         'checker': None,
-        'test_generator': None
+        'test_generator': None,
+        'network': False,
+        'cpus': 1
     }
 
     def __init__(self, path: Path, commit: str) -> None:
         """
         It takes a path to a folder, and then it creates a list of all the subfolders in that folder, and then it creates a
         TSet object for each of those subfolders
 
@@ -212,14 +219,30 @@
         """
         if not (self.commit_path / '.build').is_dir():
             mkdir(self.commit_path / '.build')
 
         if not (self.commit_path / '.build' / build_name).is_dir():
             mkdir(self.commit_path / '.build' / build_name)
 
+        return self.commit_path / '.build' / build_name
+
+    def check_build(self, build_name: str):
+        """
+        It checks if the build exists
+
+        :param build_name: The name of the build
+        :type build_name: str
+        """
+        build_dir = self.commit_path / '.build' / build_name
+
+        if not build_dir.is_dir():
+            return False
+
+        return any(list(walk(build_dir))[0][1:])
+
     def delete_build(self, build_name: str = None):
         """
         Deletes the build. If build_name is None, it deletes all builds.
 
         :param build_name: The name of the build, if None, it clears all builds
         :type build_name: str
         """
```

### Comparing `baca2-package-manager-0.2.1/baca2PackageManager/validators.py` & `baca2-package-manager-0.2.2/baca2PackageManager/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,23 @@
     check if val is in args
 
     :return: A boolean value.
     """
     return val in args
 
 
+def isBool(val):
+    """
+    check if val is bool
+
+    :return: A boolean value.
+    """
+    return type(val) == bool
+
+
 def isShorter(val, l: int):
     """
     check if val is string and has len < len(l)
 
     :return: A boolean value.
     """
     if isStr(val):
```

### Comparing `baca2-package-manager-0.2.1/baca2_package_manager.egg-info/PKG-INFO` & `baca2-package-manager-0.2.2/baca2_package_manager.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baca2-package-manager
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package manager for Baca2 project
 Home-page: https://github.com/BaCa2-project/BaCa2-package-manager
 Author: Baca2 Team
 Author-email: bartosz.deptula@student.uj.edu.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `baca2-package-manager-0.2.1/setup.py` & `baca2-package-manager-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='baca2-package-manager',
-    version='0.2.1',
+    version='0.2.2',
     author='Baca2 Team',
     author_email='bartosz.deptula@student.uj.edu.pl',
     description='A package manager for Baca2 project',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/BaCa2-project/BaCa2-package-manager',
     packages=setuptools.find_packages(),
```

### Comparing `baca2-package-manager-0.2.1/tests/tests.py` & `baca2-package-manager-0.2.2/tests/tests.py`

 * *Files identical despite different names*

