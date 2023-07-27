# Comparing `tmp/Flask-Meter-1.0.2.tar.gz` & `tmp/Flask-Meter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Meter-1.0.2.tar", last modified: Thu Apr 20 16:37:49 2023, max compression
+gzip compressed data, was "dist/Flask-Meter-1.1.0.tar", last modified: Thu Jul 27 15:37:39 2023, max compression
```

## Comparing `Flask-Meter-1.0.2.tar` & `Flask-Meter-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.056286 Flask-Meter-1.0.2/
--rw-rw-r--   0 herman    (1000) herman    (1000)      156 2023-04-10 07:49:10.000000 Flask-Meter-1.0.2/AUTHORS.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     3267 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/CONTRIBUTING.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      489 2023-04-20 15:36:44.000000 Flask-Meter-1.0.2/HISTORY.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     1077 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/LICENSE
--rw-rw-r--   0 herman    (1000) herman    (1000)      264 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/MANIFEST.in
--rw-rw-r--   0 herman    (1000) herman    (1000)     3823 2023-04-20 16:37:49.056286 Flask-Meter-1.0.2/PKG-INFO
--rw-rw-r--   0 herman    (1000) herman    (1000)     2394 2023-04-20 07:43:19.000000 Flask-Meter-1.0.2/README.rst
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.048286 Flask-Meter-1.0.2/docs/
--rw-rw-r--   0 herman    (1000) herman    (1000)     6782 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/docs/Makefile
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.032286 Flask-Meter-1.0.2/docs/_build/
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.032286 Flask-Meter-1.0.2/docs/_build/html/
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.052286 Flask-Meter-1.0.2/docs/_build/html/_static/
--rw-rw-r--   0 herman    (1000) herman    (1000)      286 2023-04-10 12:45:48.000000 Flask-Meter-1.0.2/docs/_build/html/_static/file.png
--rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-04-10 12:45:48.000000 Flask-Meter-1.0.2/docs/_build/html/_static/minus.png
--rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-04-10 12:45:48.000000 Flask-Meter-1.0.2/docs/_build/html/_static/plus.png
--rw-rw-r--   0 herman    (1000) herman    (1000)       28 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/docs/authors.rst
--rwxrwxr-x   0 herman    (1000) herman    (1000)     8585 2023-04-10 13:26:44.000000 Flask-Meter-1.0.2/docs/conf.py
--rw-rw-r--   0 herman    (1000) herman    (1000)       33 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/docs/contributing.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      479 2023-04-20 15:37:13.000000 Flask-Meter-1.0.2/docs/flask_meter.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)       28 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/docs/history.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      298 2023-04-10 11:47:36.000000 Flask-Meter-1.0.2/docs/index.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     1147 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/docs/installation.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     6469 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/docs/make.bat
--rw-rw-r--   0 herman    (1000) herman    (1000)       70 2023-04-20 15:37:13.000000 Flask-Meter-1.0.2/docs/modules.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)       27 2023-04-10 06:09:30.000000 Flask-Meter-1.0.2/docs/readme.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      420 2023-04-10 11:51:37.000000 Flask-Meter-1.0.2/docs/usage.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     1724 2023-04-10 14:06:24.000000 Flask-Meter-1.0.2/pyproject.toml
--rw-rw-r--   0 herman    (1000) herman    (1000)       69 2023-04-20 16:37:49.060286 Flask-Meter-1.0.2/setup.cfg
--rw-rw-r--   0 herman    (1000) herman    (1000)       38 2023-04-10 08:04:42.000000 Flask-Meter-1.0.2/setup.py
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.036286 Flask-Meter-1.0.2/src/
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.056286 Flask-Meter-1.0.2/src/Flask_Meter.egg-info/
--rw-rw-r--   0 herman    (1000) herman    (1000)     3823 2023-04-20 16:37:48.000000 Flask-Meter-1.0.2/src/Flask_Meter.egg-info/PKG-INFO
--rw-rw-r--   0 herman    (1000) herman    (1000)      731 2023-04-20 16:37:49.000000 Flask-Meter-1.0.2/src/Flask_Meter.egg-info/SOURCES.txt
--rw-rw-r--   0 herman    (1000) herman    (1000)        1 2023-04-20 16:37:48.000000 Flask-Meter-1.0.2/src/Flask_Meter.egg-info/dependency_links.txt
--rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-04-20 16:37:48.000000 Flask-Meter-1.0.2/src/Flask_Meter.egg-info/requires.txt
--rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-04-20 16:37:48.000000 Flask-Meter-1.0.2/src/Flask_Meter.egg-info/top_level.txt
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.056286 Flask-Meter-1.0.2/src/flask_meter/
--rw-rw-r--   0 herman    (1000) herman    (1000)      109 2023-04-20 15:35:50.000000 Flask-Meter-1.0.2/src/flask_meter/__init__.py
--rw-rw-r--   0 herman    (1000) herman    (1000)     2227 2023-04-20 15:34:23.000000 Flask-Meter-1.0.2/src/flask_meter/flask_meter.py
--rw-rw-r--   0 herman    (1000) herman    (1000)     1179 2023-04-20 15:34:42.000000 Flask-Meter-1.0.2/src/flask_meter/git.py
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-20 16:37:49.056286 Flask-Meter-1.0.2/tests/
--rw-rw-r--   0 herman    (1000) herman    (1000)     2608 2023-04-20 15:34:23.000000 Flask-Meter-1.0.2/tests/test_flask_meter.py
--rw-rw-r--   0 herman    (1000) herman    (1000)      449 2023-04-20 15:34:05.000000 Flask-Meter-1.0.2/tests/test_git.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 15:37:39.870778 Flask-Meter-1.1.0/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      156 2023-07-26 22:55:52.000000 Flask-Meter-1.1.0/AUTHORS.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     3267 2018-04-17 03:06:44.000000 Flask-Meter-1.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      583 2023-07-27 15:35:04.000000 Flask-Meter-1.1.0/HISTORY.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1077 2018-04-17 03:06:44.000000 Flask-Meter-1.1.0/LICENSE
+-rw-rw-r--   0 herman    (1000) herman    (1000)      264 2018-04-17 03:06:44.000000 Flask-Meter-1.1.0/MANIFEST.in
+-rw-rw-r--   0 herman    (1000) herman    (1000)     4520 2023-07-27 15:37:39.870778 Flask-Meter-1.1.0/PKG-INFO
+-rw-rw-r--   0 herman    (1000) herman    (1000)     3091 2023-07-27 15:32:18.000000 Flask-Meter-1.1.0/README.rst
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 15:37:39.870778 Flask-Meter-1.1.0/docs/
+-rw-rw-r--   0 herman    (1000) herman    (1000)     6782 2018-04-17 03:06:44.000000 Flask-Meter-1.1.0/docs/Makefile
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 15:37:39.866778 Flask-Meter-1.1.0/docs/_build/
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 15:37:39.866778 Flask-Meter-1.1.0/docs/_build/html/
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 15:37:39.870778 Flask-Meter-1.1.0/docs/_build/html/_static/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      286 2023-02-19 21:41:17.000000 Flask-Meter-1.1.0/docs/_build/html/_static/file.png
+-rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-02-19 21:41:17.000000 Flask-Meter-1.1.0/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-02-19 21:41:17.000000 Flask-Meter-1.1.0/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 herman    (1000) herman    (1000)       28 2018-04-17 03:06:44.000000 Flask-Meter-1.1.0/docs/authors.rst
+-rwxrwxr-x   0 herman    (1000) herman    (1000)     8585 2023-07-26 22:55:52.000000 Flask-Meter-1.1.0/docs/conf.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)       33 2018-04-17 03:06:44.000000 Flask-Meter-1.1.0/docs/contributing.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      627 2023-07-27 15:34:02.000000 Flask-Meter-1.1.0/docs/flask_meter.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)       28 2018-04-17 03:06:44.000000 Flask-Meter-1.1.0/docs/history.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      298 2023-07-26 22:55:52.000000 Flask-Meter-1.1.0/docs/index.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1147 2018-04-17 03:06:44.000000 Flask-Meter-1.1.0/docs/installation.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     6469 2018-04-17 03:06:44.000000 Flask-Meter-1.1.0/docs/make.bat
+-rw-rw-r--   0 herman    (1000) herman    (1000)       70 2023-07-27 15:34:02.000000 Flask-Meter-1.1.0/docs/modules.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)       27 2018-04-17 03:06:44.000000 Flask-Meter-1.1.0/docs/readme.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      420 2023-07-26 22:55:52.000000 Flask-Meter-1.1.0/docs/usage.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1724 2023-07-26 22:55:52.000000 Flask-Meter-1.1.0/pyproject.toml
+-rw-rw-r--   0 herman    (1000) herman    (1000)       69 2023-07-27 15:37:39.874778 Flask-Meter-1.1.0/setup.cfg
+-rw-rw-r--   0 herman    (1000) herman    (1000)       38 2023-07-26 22:55:52.000000 Flask-Meter-1.1.0/setup.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 15:37:39.866778 Flask-Meter-1.1.0/src/
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 15:37:39.870778 Flask-Meter-1.1.0/src/Flask_Meter.egg-info/
+-rw-rw-r--   0 herman    (1000) herman    (1000)     4520 2023-07-27 15:37:39.000000 Flask-Meter-1.1.0/src/Flask_Meter.egg-info/PKG-INFO
+-rw-rw-r--   0 herman    (1000) herman    (1000)      788 2023-07-27 15:37:39.000000 Flask-Meter-1.1.0/src/Flask_Meter.egg-info/SOURCES.txt
+-rw-rw-r--   0 herman    (1000) herman    (1000)        1 2023-07-27 15:37:39.000000 Flask-Meter-1.1.0/src/Flask_Meter.egg-info/dependency_links.txt
+-rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-07-27 15:37:39.000000 Flask-Meter-1.1.0/src/Flask_Meter.egg-info/requires.txt
+-rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-07-27 15:37:39.000000 Flask-Meter-1.1.0/src/Flask_Meter.egg-info/top_level.txt
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 15:37:39.870778 Flask-Meter-1.1.0/src/flask_meter/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      109 2023-07-27 15:35:04.000000 Flask-Meter-1.1.0/src/flask_meter/__init__.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)     2504 2023-07-27 15:30:59.000000 Flask-Meter-1.1.0/src/flask_meter/flask_meter.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1179 2023-07-26 22:55:52.000000 Flask-Meter-1.1.0/src/flask_meter/git.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)      199 2023-07-27 15:30:59.000000 Flask-Meter-1.1.0/src/flask_meter/version.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 15:37:39.870778 Flask-Meter-1.1.0/tests/
+-rw-rw-r--   0 herman    (1000) herman    (1000)     2608 2023-07-26 22:55:52.000000 Flask-Meter-1.1.0/tests/test_flask_meter.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)      449 2023-07-26 22:55:52.000000 Flask-Meter-1.1.0/tests/test_git.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-07-27 15:37:39.870778 Flask-Meter-1.1.0/tests/version/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      377 2023-07-27 15:30:59.000000 Flask-Meter-1.1.0/tests/version/test_version.py
```

### Comparing `Flask-Meter-1.0.2/CONTRIBUTING.rst` & `Flask-Meter-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.2/LICENSE` & `Flask-Meter-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.2/PKG-INFO` & `Flask-Meter-1.1.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: Flask-Meter
-Version: 1.0.2
-Summary: Flask-Meter adds a healthcheck endpoint for Flask apps.
-Author-email: Herman Singh <kartstig@gmail.com>
-Maintainer-email: Herman Singh <kartstig@gmail.com>
-License: MIT License
-Project-URL: Donate, https://github.com/sponsors/Kartstig/dashboard
-Project-URL: Documentation, https://flask.palletsprojects.com/
-Project-URL: Source Code, https://github.com/Kartstig/flask-meter
-Project-URL: Issue Tracker, https://github.com/Kartstig/flask-meter/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 ===============================
 Flask-Meter
 ===============================
 
         Healthchecks for Flask_ Apps
 
 .. _Flask: https://github.com/pallets/flask/
@@ -101,17 +69,32 @@
 * Documentation: https://flask-meter.readthedocs.io.
 
 
 Features
 --------
 
 * Current Git Commit
+* Current Version
 * Accepts custom functions
 
 
+Configuration
+-------------
+
++---------------------+------------------------------+------+---------+
+| Config Key          | Description                  | Type | Default |
++=====================+==============================+======+=========+
+| FLASK_METER_ENABLE  | Enable/Disable Flask-Meter   | bool | True    |
++---------------------+------------------------------+------+---------+
+| FLASK_METER_GIT     | Enable/Disable Git Stats     | bool | True    |
++---------------------+------------------------------+------+---------+
+| FLASK_METER_VERSION | Enable/Disable Version Stats | bool | True    |
++---------------------+------------------------------+------+---------+
+
+
 Sponsorship
 -----------
 
 Put your logo here! `Become a sponsor`_ and support this project!
 
 .. _Become a sponsor: https://github.com/sponsors/Kartstig
```

### Comparing `Flask-Meter-1.0.2/docs/Makefile` & `Flask-Meter-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.2/docs/conf.py` & `Flask-Meter-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.2/docs/installation.rst` & `Flask-Meter-1.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.2/docs/make.bat` & `Flask-Meter-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.2/pyproject.toml` & `Flask-Meter-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.2/src/Flask_Meter.egg-info/SOURCES.txt` & `Flask-Meter-1.1.0/src/Flask_Meter.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -26,9 +26,11 @@
 src/Flask_Meter.egg-info/SOURCES.txt
 src/Flask_Meter.egg-info/dependency_links.txt
 src/Flask_Meter.egg-info/requires.txt
 src/Flask_Meter.egg-info/top_level.txt
 src/flask_meter/__init__.py
 src/flask_meter/flask_meter.py
 src/flask_meter/git.py
+src/flask_meter/version.py
 tests/test_flask_meter.py
-tests/test_git.py
+tests/test_git.py
+tests/version/test_version.py
```

### Comparing `Flask-Meter-1.0.2/src/flask_meter/flask_meter.py` & `Flask-Meter-1.1.0/src/flask_meter/flask_meter.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal  # Python 3.7 support
 
 from .git import git_stats, GitReturn
+from .version import read_version_file
 
 logger = logging.getLogger(__name__)
 
 
 FuncList = List[Callable]
 
 ResponseJson = Dict[
@@ -35,14 +36,17 @@
         self.app = app
         self.app.config["FLASK_METER_ENABLE"] = self.app.config.get(
             "FLASK_METER_ENABLE", True
         )
         self.app.config["FLASK_METER_GIT"] = self.app.config.get(
             "FLASK_METER_GIT", True
         )
+        self.app.config["FLASK_METER_VERSION"] = self.app.config.get(
+            "FLASK_METER_VERSION", True
+        )
         self.start_time = datetime.now()
 
         def _health() -> flask.Response:
             data: ResponseJson = {
                 "uptime": str(datetime.now() - self.start_time),
                 "app": self.app.name,
             }
@@ -62,11 +66,14 @@
                 data.update(results)
 
             data["status"] = "OK" if all(raw_results) else "DOWN"
 
             if self.app.config["FLASK_METER_GIT"]:
                 data.update({"git": git_stats()})
 
+            if self.app.config["FLASK_METER_VERSION"]:
+                data.update({"version": read_version_file()})
+
             return flask.jsonify(data)
 
         if self.app.config["FLASK_METER_ENABLE"]:
             self.app.add_url_rule("/_health", "_health", _health)
```

### Comparing `Flask-Meter-1.0.2/src/flask_meter/git.py` & `Flask-Meter-1.1.0/src/flask_meter/git.py`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.2/tests/test_flask_meter.py` & `Flask-Meter-1.1.0/tests/test_flask_meter.py`

 * *Files identical despite different names*

