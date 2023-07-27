# Comparing `tmp/sci-oer-1.2.0.tar.gz` & `tmp/sci-oer-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sci-oer-1.2.0.tar", last modified: Sun Apr 30 14:18:40 2023, max compression
+gzip compressed data, was "sci-oer-1.3.0.tar", last modified: Thu Jul 27 16:28:57 2023, max compression
```

## Comparing `sci-oer-1.2.0.tar` & `sci-oer-1.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:18:40.671089 sci-oer-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-30 14:18:31.000000 sci-oer-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    23446 2023-04-30 14:18:31.000000 sci-oer-1.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-30 14:18:31.000000 sci-oer-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-30 14:18:31.000000 sci-oer-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-30 14:18:40.671089 sci-oer-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-04-30 14:18:31.000000 sci-oer-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-30 14:18:31.000000 sci-oer-1.2.0/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-30 14:18:31.000000 sci-oer-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-30 14:18:31.000000 sci-oer-1.2.0/pytype.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-30 14:18:31.000000 sci-oer-1.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:18:40.671089 sci-oer-1.2.0/sci_oer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-30 14:18:40.000000 sci-oer-1.2.0/sci_oer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-30 14:18:40.000000 sci-oer-1.2.0/sci_oer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 14:18:40.000000 sci-oer-1.2.0/sci_oer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-30 14:18:40.000000 sci-oer-1.2.0/sci_oer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-30 14:18:40.000000 sci-oer-1.2.0/sci_oer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-30 14:18:40.000000 sci-oer-1.2.0/sci_oer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:18:40.671089 sci-oer-1.2.0/scioer/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-30 14:18:31.000000 sci-oer-1.2.0/scioer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-30 14:18:40.000000 sci-oer-1.2.0/scioer/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-04-30 14:18:31.000000 sci-oer-1.2.0/scioer/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:18:40.671089 sci-oer-1.2.0/scioer/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:18:31.000000 sci-oer-1.2.0/scioer/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-30 14:18:31.000000 sci-oer-1.2.0/scioer/config/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-30 14:18:31.000000 sci-oer-1.2.0/scioer/config/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-04-30 14:18:31.000000 sci-oer-1.2.0/scioer/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 14:18:40.671089 sci-oer-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:18:40.671089 sci-oer-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-30 14:18:31.000000 sci-oer-1.2.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:28:57.660216 sci-oer-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-27 16:28:42.000000 sci-oer-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    25282 2023-07-27 16:28:42.000000 sci-oer-1.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-27 16:28:42.000000 sci-oer-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 16:28:42.000000 sci-oer-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-07-27 16:28:57.660216 sci-oer-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-07-27 16:28:42.000000 sci-oer-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-27 16:28:42.000000 sci-oer-1.3.0/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-27 16:28:42.000000 sci-oer-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-27 16:28:42.000000 sci-oer-1.3.0/pytype.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-27 16:28:42.000000 sci-oer-1.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:28:57.660216 sci-oer-1.3.0/sci_oer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-07-27 16:28:57.000000 sci-oer-1.3.0/sci_oer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 16:28:57.000000 sci-oer-1.3.0/sci_oer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:28:57.000000 sci-oer-1.3.0/sci_oer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-27 16:28:57.000000 sci-oer-1.3.0/sci_oer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-27 16:28:57.000000 sci-oer-1.3.0/sci_oer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 16:28:57.000000 sci-oer-1.3.0/sci_oer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:28:57.660216 sci-oer-1.3.0/scioer/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-27 16:28:42.000000 sci-oer-1.3.0/scioer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 16:28:57.000000 sci-oer-1.3.0/scioer/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-07-27 16:28:42.000000 sci-oer-1.3.0/scioer/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:28:57.660216 sci-oer-1.3.0/scioer/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:28:42.000000 sci-oer-1.3.0/scioer/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-27 16:28:42.000000 sci-oer-1.3.0/scioer/config/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-27 16:28:42.000000 sci-oer-1.3.0/scioer/config/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-27 16:28:42.000000 sci-oer-1.3.0/scioer/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 16:28:57.660216 sci-oer-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:28:57.660216 sci-oer-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-27 16:28:42.000000 sci-oer-1.3.0/tests/test_cli.py
```

### Comparing `sci-oer-1.2.0/CHANGELOG.md` & `sci-oer-1.3.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,26 @@
 # Changelog
 
+## [v1.3.0](https://github.com/sci-oer/student-cli/releases/v1.3.0) (2023-07-27)
+
+[Full Changelog](https://github.com/sci-oer/student-cli/compare/v1.2.0...v1.3.0)
+
+**Merged pull requests:**
+
+- chore\(deps\): update dependency pyyaml to v6.0.1 [\#160](https://github.com/sci-oer/student-cli/pull/160) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency click to v8.1.6 [\#159](https://github.com/sci-oer/student-cli/pull/159) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency pyparsing to v3.1.0 [\#158](https://github.com/sci-oer/student-cli/pull/158) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency pytest to v7.4.0 [\#157](https://github.com/sci-oer/student-cli/pull/157) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency rich to v13.4.2 [\#156](https://github.com/sci-oer/student-cli/pull/156) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency typing\_extensions to v4.7.1 [\#155](https://github.com/sci-oer/student-cli/pull/155) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency setuptools to v67.8.0 [\#154](https://github.com/sci-oer/student-cli/pull/154) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency docker to v6.1.3 [\#151](https://github.com/sci-oer/student-cli/pull/151) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update pypa/gh-action-pypi-publish action to v1.8.8 [\#150](https://github.com/sci-oer/student-cli/pull/150) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency typer to v0.9.0 [\#149](https://github.com/sci-oer/student-cli/pull/149) ([renovate[bot]](https://github.com/apps/renovate))
+
 ## [v1.2.0](https://github.com/sci-oer/student-cli/releases/v1.2.0) (2023-04-30)
 
 [Full Changelog](https://github.com/sci-oer/student-cli/compare/v1.1.0...v1.2.0)
 
 **Implemented enhancements:**
 
 - feat: add readline so prompts can be edited [\#148](https://github.com/sci-oer/student-cli/pull/148) ([MarshallAsch](https://github.com/MarshallAsch))
```

### Comparing `sci-oer-1.2.0/LICENSE` & `sci-oer-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sci-oer-1.2.0/PKG-INFO` & `sci-oer-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sci-oer
-Version: 1.2.0
+Version: 1.3.0
 Summary: A cli application to help launch the sci-oer course container
 Author-email: Marshall Asch <masch@uoguelph.ca>
 Project-URL: Documentation, https://github.com/sci-oer/student-cli/blob/main/README.md
 Project-URL: Source, https://github.com/sci-oer/student-cli
 Project-URL: Bug Tracker, https://github.com/sci-oer/student-cli/issues
 Project-URL: Funding, https://github.com/sci-oer/student-cli/blob/main/.github/FUNDING.md
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sci-oer-1.2.0/README.md` & `sci-oer-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sci-oer-1.2.0/pyproject.toml` & `sci-oer-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sci-oer-1.2.0/pytype.cfg` & `sci-oer-1.3.0/pytype.cfg`

 * *Files identical despite different names*

### Comparing `sci-oer-1.2.0/sci_oer.egg-info/PKG-INFO` & `sci-oer-1.3.0/sci_oer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sci-oer
-Version: 1.2.0
+Version: 1.3.0
 Summary: A cli application to help launch the sci-oer course container
 Author-email: Marshall Asch <masch@uoguelph.ca>
 Project-URL: Documentation, https://github.com/sci-oer/student-cli/blob/main/README.md
 Project-URL: Source, https://github.com/sci-oer/student-cli
 Project-URL: Bug Tracker, https://github.com/sci-oer/student-cli/issues
 Project-URL: Funding, https://github.com/sci-oer/student-cli/blob/main/.github/FUNDING.md
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sci-oer-1.2.0/scioer/cli.py` & `sci-oer-1.3.0/scioer/cli.py`

 * *Files identical despite different names*

### Comparing `sci-oer-1.2.0/scioer/config/load.py` & `sci-oer-1.3.0/scioer/config/load.py`

 * *Files identical despite different names*

### Comparing `sci-oer-1.2.0/scioer/config/parse.py` & `sci-oer-1.3.0/scioer/config/parse.py`

 * *Files identical despite different names*

### Comparing `sci-oer-1.2.0/scioer/docker.py` & `sci-oer-1.3.0/scioer/docker.py`

 * *Files identical despite different names*

