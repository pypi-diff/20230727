# Comparing `tmp/pyjanitor-0.8.0.tar.gz` & `tmp/pyjanitor-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyjanitor-0.8.0.tar", last modified: Sat Nov 10 19:04:46 2018, max compression
+gzip compressed data, was "dist/pyjanitor-0.9.0.tar", last modified: Wed Nov 21 17:31:04 2018, max compression
```

## Comparing `pyjanitor-0.8.0.tar` & `pyjanitor-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2018-11-10 19:04:46.000000 pyjanitor-0.8.0/
--rw-r--r--   0 ericmjl    (501) staff       (20)      295 2018-11-10 19:04:46.000000 pyjanitor-0.8.0/PKG-INFO
--rw-r--r--   0 ericmjl    (501) staff       (20)     1064 2018-10-25 12:58:18.000000 pyjanitor-0.8.0/LICENSE
--rw-r--r--   0 ericmjl    (501) staff       (20)      158 2018-10-25 12:58:18.000000 pyjanitor-0.8.0/requirements.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)     3709 2018-10-25 12:58:18.000000 pyjanitor-0.8.0/CONTRIBUTING.rst
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2018-11-10 19:04:46.000000 pyjanitor-0.8.0/pyjanitor.egg-info/
--rw-r--r--   0 ericmjl    (501) staff       (20)      295 2018-11-10 19:04:46.000000 pyjanitor-0.8.0/pyjanitor.egg-info/PKG-INFO
--rw-r--r--   0 ericmjl    (501) staff       (20)      308 2018-11-10 19:04:46.000000 pyjanitor-0.8.0/pyjanitor.egg-info/SOURCES.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)      158 2018-11-10 19:04:46.000000 pyjanitor-0.8.0/pyjanitor.egg-info/requires.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)        8 2018-11-10 19:04:46.000000 pyjanitor-0.8.0/pyjanitor.egg-info/top_level.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)        1 2018-11-10 19:04:46.000000 pyjanitor-0.8.0/pyjanitor.egg-info/dependency_links.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)      129 2018-10-25 12:58:18.000000 pyjanitor-0.8.0/MANIFEST.in
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2018-11-10 19:04:46.000000 pyjanitor-0.8.0/janitor/
--rw-r--r--   0 ericmjl    (501) staff       (20)    29937 2018-11-10 19:03:52.000000 pyjanitor-0.8.0/janitor/functions.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      201 2018-11-10 19:04:31.000000 pyjanitor-0.8.0/janitor/__init__.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       40 2018-10-25 12:58:18.000000 pyjanitor-0.8.0/janitor/errors.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      412 2018-11-10 19:04:31.000000 pyjanitor-0.8.0/setup.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      480 2018-11-04 15:00:49.000000 pyjanitor-0.8.0/AUTHORS.rst
--rw-r--r--   0 ericmjl    (501) staff       (20)       38 2018-11-10 19:04:46.000000 pyjanitor-0.8.0/setup.cfg
--rw-r--r--   0 ericmjl    (501) staff       (20)     6314 2018-11-04 15:00:49.000000 pyjanitor-0.8.0/README.rst
+drwx------   0 maer3    (1506609526) maer3    (1506609526)        0 2018-11-21 17:31:04.000000 pyjanitor-0.9.0/
+drwx------   0 maer3    (1506609526) maer3    (1506609526)        0 2018-11-21 17:31:04.000000 pyjanitor-0.9.0/janitor/
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)       40 2018-09-13 17:38:26.000000 pyjanitor-0.9.0/janitor/errors.py
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)      201 2018-11-21 17:29:20.000000 pyjanitor-0.9.0/janitor/__init__.py
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)    43740 2018-11-21 16:22:24.000000 pyjanitor-0.9.0/janitor/functions.py
+drwx------   0 maer3    (1506609526) maer3    (1506609526)        0 2018-11-21 17:31:04.000000 pyjanitor-0.9.0/pyjanitor.egg-info/
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)      308 2018-11-21 17:31:04.000000 pyjanitor-0.9.0/pyjanitor.egg-info/SOURCES.txt
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)        8 2018-11-21 17:31:04.000000 pyjanitor-0.9.0/pyjanitor.egg-info/top_level.txt
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)        1 2018-11-21 17:31:04.000000 pyjanitor-0.9.0/pyjanitor.egg-info/dependency_links.txt
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)      261 2018-11-21 17:31:04.000000 pyjanitor-0.9.0/pyjanitor.egg-info/PKG-INFO
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)      158 2018-11-21 17:31:04.000000 pyjanitor-0.9.0/pyjanitor.egg-info/requires.txt
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)     6314 2018-11-21 16:22:24.000000 pyjanitor-0.9.0/README.rst
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)     1064 2018-09-13 17:38:26.000000 pyjanitor-0.9.0/LICENSE
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)      480 2018-11-21 16:22:24.000000 pyjanitor-0.9.0/AUTHORS.rst
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)      158 2018-09-13 17:38:26.000000 pyjanitor-0.9.0/requirements.txt
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)      129 2018-09-13 17:38:26.000000 pyjanitor-0.9.0/MANIFEST.in
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)       38 2018-11-21 17:31:04.000000 pyjanitor-0.9.0/setup.cfg
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)      261 2018-11-21 17:31:04.000000 pyjanitor-0.9.0/PKG-INFO
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)      412 2018-11-21 17:29:20.000000 pyjanitor-0.9.0/setup.py
+-rw-------   0 maer3    (1506609526) maer3    (1506609526)     3709 2018-09-13 17:38:26.000000 pyjanitor-0.9.0/CONTRIBUTING.rst
```

### Comparing `pyjanitor-0.8.0/LICENSE` & `pyjanitor-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjanitor-0.8.0/CONTRIBUTING.rst` & `pyjanitor-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyjanitor-0.8.0/README.rst` & `pyjanitor-0.9.0/README.rst`

 * *Files identical despite different names*

