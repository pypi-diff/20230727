# Comparing `tmp/recognite-0.1.0rc1.tar.gz` & `tmp/recognite-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recognite-0.1.0rc1.tar", last modified: Wed Jul 26 12:29:48 2023, max compression
+gzip compressed data, was "recognite-0.1.0rc2.tar", last modified: Thu Jul 27 13:05:10 2023, max compression
```

## Comparing `recognite-0.1.0rc1.tar` & `recognite-0.1.0rc2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:48.709915 recognite-0.1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-26 12:29:36.000000 recognite-0.1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-26 12:29:48.709915 recognite-0.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-26 12:29:36.000000 recognite-0.1.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:48.709915 recognite-0.1.0rc1/recognite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-26 12:29:48.000000 recognite-0.1.0rc1/recognite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-26 12:29:48.000000 recognite-0.1.0rc1/recognite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:29:48.000000 recognite-0.1.0rc1/recognite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:29:48.000000 recognite-0.1.0rc1/recognite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 12:29:48.000000 recognite-0.1.0rc1/recognite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:29:48.000000 recognite-0.1.0rc1/recognite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:29:48.709915 recognite-0.1.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-26 12:29:36.000000 recognite-0.1.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:10.853813 recognite-0.1.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-27 13:04:58.000000 recognite-0.1.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-27 13:05:10.853813 recognite-0.1.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-07-27 13:04:58.000000 recognite-0.1.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:05:10.853813 recognite-0.1.0rc2/recognite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-27 13:05:10.000000 recognite-0.1.0rc2/recognite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-27 13:05:10.000000 recognite-0.1.0rc2/recognite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:05:10.000000 recognite-0.1.0rc2/recognite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:05:10.000000 recognite-0.1.0rc2/recognite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-27 13:05:10.000000 recognite-0.1.0rc2/recognite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:05:10.000000 recognite-0.1.0rc2/recognite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:05:10.853813 recognite-0.1.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-27 13:04:58.000000 recognite-0.1.0rc2/setup.py
```

### Comparing `recognite-0.1.0rc1/LICENSE` & `recognite-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `recognite-0.1.0rc1/setup.py` & `recognite-0.1.0rc2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,17 +31,18 @@
         'Programming Language :: Python :: 3.8',
     ],
     description="Recognite is a library to kickstart your next PyTorch-based "
     "recognition project.",
     install_requires=requirements,
     license="MIT license",
     long_description=readme,
+    long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='recognite',
     name='recognite',
     packages=find_packages(include=['recognite', 'recognite.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/florisdf/recognite',
-    version='0.1.0-rc1',
+    version='0.1.0-rc2',
     zip_safe=False,
 )
```

