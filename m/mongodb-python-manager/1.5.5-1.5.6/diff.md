# Comparing `tmp/mongodb_python_manager-1.5.5.tar.gz` & `tmp/mongodb_python_manager-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_python_manager-1.5.5.tar", last modified: Mon Jul 10 09:35:40 2023, max compression
+gzip compressed data, was "mongodb_python_manager-1.5.6.tar", max compression
```

## Comparing `mongodb_python_manager-1.5.5.tar` & `mongodb_python_manager-1.5.6.tar`

### file list

```diff
@@ -1,45 +1,5 @@
-drwxr-xr-x   0 louisgiron   (501) staff       (20)        0 2023-07-10 09:35:40.412023 mongodb_python_manager-1.5.5/
-drwxr-xr-x   0 louisgiron   (501) staff       (20)        0 2023-07-10 09:35:40.375185 mongodb_python_manager-1.5.5/.eggs/
--rw-r--r--   0 louisgiron   (501) staff       (20)      211 2023-05-17 14:45:51.000000 mongodb_python_manager-1.5.5/.eggs/README.txt
--rw-r--r--   0 louisgiron   (501) staff       (20)       74 2023-06-23 08:29:39.000000 mongodb_python_manager-1.5.5/.gitignore
--rw-r--r--   0 louisgiron   (501) staff       (20)     1080 2023-05-09 13:15:51.000000 mongodb_python_manager-1.5.5/LICENSE
--rw-r--r--   0 louisgiron   (501) staff       (20)      403 2023-07-10 09:35:40.411256 mongodb_python_manager-1.5.5/PKG-INFO
--rw-r--r--   0 louisgiron   (501) staff       (20)     5051 2023-05-17 14:25:09.000000 mongodb_python_manager-1.5.5/README.md
-drwxr-xr-x   0 louisgiron   (501) staff       (20)        0 2023-07-10 09:35:40.375863 mongodb_python_manager-1.5.5/mongodb_python_manager/
--rw-r--r--   0 louisgiron   (501) staff       (20)     9790 2023-06-22 14:52:42.000000 mongodb_python_manager-1.5.5/mongodb_python_manager/__init__.py
-drwxr-xr-x   0 louisgiron   (501) staff       (20)        0 2023-07-10 09:35:40.388114 mongodb_python_manager-1.5.5/mongodb_python_manager/__pycache__/
--rw-r--r--   0 louisgiron   (501) staff       (20)     9318 2023-06-22 14:52:48.000000 mongodb_python_manager-1.5.5/mongodb_python_manager/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)     8547 2023-05-17 09:31:51.000000 mongodb_python_manager-1.5.5/mongodb_python_manager/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)     9280 2023-06-22 14:10:14.000000 mongodb_python_manager-1.5.5/mongodb_python_manager/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)     5802 2023-05-15 10:31:30.000000 mongodb_python_manager-1.5.5/mongodb_python_manager/__pycache__/mongodb_python_manager.cpython-310.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)    16818 2023-05-17 13:54:16.000000 mongodb_python_manager-1.5.5/mongodb_python_manager/__pycache__/test.cpython-310-pytest-7.3.1.pyc
-drwxr-xr-x   0 louisgiron   (501) staff       (20)        0 2023-07-10 09:35:40.379861 mongodb_python_manager-1.5.5/mongodb_python_manager.egg-info/
--rw-r--r--   0 louisgiron   (501) staff       (20)      403 2023-07-10 09:35:40.000000 mongodb_python_manager-1.5.5/mongodb_python_manager.egg-info/PKG-INFO
--rw-r--r--   0 louisgiron   (501) staff       (20)     1407 2023-07-10 09:35:40.000000 mongodb_python_manager-1.5.5/mongodb_python_manager.egg-info/SOURCES.txt
--rw-r--r--   0 louisgiron   (501) staff       (20)        1 2023-07-10 09:35:40.000000 mongodb_python_manager-1.5.5/mongodb_python_manager.egg-info/dependency_links.txt
--rw-r--r--   0 louisgiron   (501) staff       (20)       81 2023-07-10 09:35:40.000000 mongodb_python_manager-1.5.5/mongodb_python_manager.egg-info/requires.txt
--rw-r--r--   0 louisgiron   (501) staff       (20)       23 2023-07-10 09:35:40.000000 mongodb_python_manager-1.5.5/mongodb_python_manager.egg-info/top_level.txt
--rw-r--r--   0 louisgiron   (501) staff       (20)      894 2023-06-23 07:12:52.000000 mongodb_python_manager-1.5.5/package_installer.sh
--rw-r--r--   0 louisgiron   (501) staff       (20)      222 2023-05-15 10:10:39.000000 mongodb_python_manager-1.5.5/pyproject.toml
--rw-r--r--   0 louisgiron   (501) staff       (20)       34 2023-05-17 14:39:33.000000 mongodb_python_manager-1.5.5/pytest.ini
--rw-r--r--   0 louisgiron   (501) staff       (20)      180 2023-05-22 17:06:25.000000 mongodb_python_manager-1.5.5/requirements.txt
--rw-r--r--   0 louisgiron   (501) staff       (20)       14 2023-05-17 09:10:45.000000 mongodb_python_manager-1.5.5/runtime.txt
--rw-r--r--   0 louisgiron   (501) staff       (20)       38 2023-07-10 09:35:40.412201 mongodb_python_manager-1.5.5/setup.cfg
--rw-r--r--   0 louisgiron   (501) staff       (20)      860 2023-06-22 14:07:26.000000 mongodb_python_manager-1.5.5/setup.py
-drwxr-xr-x   0 louisgiron   (501) staff       (20)        0 2023-07-10 09:35:40.390778 mongodb_python_manager-1.5.5/tests/
--rw-r--r--   0 louisgiron   (501) staff       (20)        0 2023-05-17 14:40:08.000000 mongodb_python_manager-1.5.5/tests/__init__.py
-drwxr-xr-x   0 louisgiron   (501) staff       (20)        0 2023-07-10 09:35:40.409662 mongodb_python_manager-1.5.5/tests/__pycache__/
--rw-r--r--   0 louisgiron   (501) staff       (20)      234 2023-05-17 14:41:03.000000 mongodb_python_manager-1.5.5/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)      232 2023-05-31 09:42:13.000000 mongodb_python_manager-1.5.5/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)      232 2023-06-22 14:10:13.000000 mongodb_python_manager-1.5.5/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)    16823 2023-05-17 13:59:48.000000 mongodb_python_manager-1.5.5/tests/__pycache__/test.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)     7309 2023-05-17 14:39:40.000000 mongodb_python_manager-1.5.5/tests/__pycache__/test.cpython-310.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)    25727 2023-05-31 09:46:50.000000 mongodb_python_manager-1.5.5/tests/__pycache__/test_main.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)    25727 2023-06-22 14:18:06.000000 mongodb_python_manager-1.5.5/tests/__pycache__/test_main.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)     7314 2023-05-17 14:41:55.000000 mongodb_python_manager-1.5.5/tests/__pycache__/test_main.cpython-310.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)    27245 2023-06-22 14:06:55.000000 mongodb_python_manager-1.5.5/tests/__pycache__/test_main.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)    26077 2023-06-22 14:10:13.000000 mongodb_python_manager-1.5.5/tests/__pycache__/test_main.cpython-39-pytest-7.3.2.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)    18014 2023-05-17 14:41:04.000000 mongodb_python_manager-1.5.5/tests/__pycache__/test_main_module.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)    18008 2023-05-17 14:37:20.000000 mongodb_python_manager-1.5.5/tests/__pycache__/tests_main.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)     7315 2023-05-17 14:38:33.000000 mongodb_python_manager-1.5.5/tests/__pycache__/tests_main.cpython-310.pyc
--rw-r--r--   0 louisgiron   (501) staff       (20)    18028 2023-05-31 09:46:47.000000 mongodb_python_manager-1.5.5/tests/test_main.py
+-rw-r--r--   0        0        0     1080 2023-07-27 09:59:52.406521 mongodb_python_manager-1.5.6/LICENSE
+-rw-r--r--   0        0        0     5051 2023-07-27 09:59:52.406740 mongodb_python_manager-1.5.6/README.md
+-rw-r--r--   0        0        0     9790 2023-07-27 09:59:52.407019 mongodb_python_manager-1.5.6/mongodb_python_manager/__init__.py
+-rw-r--r--   0        0        0      779 2023-07-27 10:46:43.960446 mongodb_python_manager-1.5.6/pyproject.toml
+-rw-r--r--   0        0        0     6037 1970-01-01 00:00:00.000000 mongodb_python_manager-1.5.6/PKG-INFO
```

### Comparing `mongodb_python_manager-1.5.5/LICENSE` & `mongodb_python_manager-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodb_python_manager-1.5.5/README.md` & `mongodb_python_manager-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_python_manager-1.5.5/mongodb_python_manager/__init__.py` & `mongodb_python_manager-1.5.6/mongodb_python_manager/__init__.py`

 * *Files identical despite different names*

