# Comparing `tmp/python-aternos-3.0.3.tar.gz` & `tmp/python-aternos-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-aternos-3.0.3.tar", last modified: Tue Jul  4 10:57:30 2023, max compression
+gzip compressed data, was "python-aternos-3.0.4.tar", last modified: Thu Jul 27 06:59:45 2023, max compression
```

## Comparing `python-aternos-3.0.3.tar` & `python-aternos-3.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:57:30.170874 python-aternos-3.0.3/
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    11357 2022-02-15 14:48:20.000000 python-aternos-3.0.3/LICENSE
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      562 2022-08-23 06:43:33.000000 python-aternos-3.0.3/NOTICE
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7105 2023-07-04 10:57:30.170874 python-aternos-3.0.3/PKG-INFO
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5818 2023-07-04 10:56:37.000000 python-aternos-3.0.3/README.md
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      110 2022-07-01 10:05:05.000000 python-aternos-3.0.3/pyproject.toml
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:57:30.170874 python-aternos-3.0.3/python_aternos/
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      317 2023-05-29 07:28:42.000000 python-aternos-3.0.3/python_aternos/__init__.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6067 2023-05-29 05:43:14.000000 python-aternos-3.0.3/python_aternos/ataccount.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6926 2023-06-30 05:54:30.000000 python-aternos-3.0.3/python_aternos/atclient.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10133 2023-05-29 07:09:48.000000 python-aternos-3.0.3/python_aternos/atconf.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8889 2023-07-04 10:42:47.000000 python-aternos-3.0.3/python_aternos/atconnect.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2406 2022-10-31 13:26:01.000000 python-aternos-3.0.3/python_aternos/aterrors.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8655 2023-05-24 13:38:15.000000 python-aternos-3.0.3/python_aternos/atfile.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5259 2023-05-24 13:39:35.000000 python-aternos-3.0.3/python_aternos/atfm.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5888 2023-07-04 10:44:31.000000 python-aternos-3.0.3/python_aternos/atjsparse.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      579 2023-07-04 10:47:12.000000 python-aternos-3.0.3/python_aternos/atlog.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      344 2023-05-24 15:59:49.000000 python-aternos-3.0.3/python_aternos/atmd5.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     3329 2023-07-04 10:42:58.000000 python-aternos-3.0.3/python_aternos/atplayers.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10912 2023-05-29 08:06:02.000000 python-aternos-3.0.3/python_aternos/atserver.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     9974 2023-06-30 06:36:36.000000 python-aternos-3.0.3/python_aternos/atwss.py
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:57:30.170874 python-aternos-3.0.3/python_aternos.egg-info/
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7105 2023-07-04 10:57:30.000000 python-aternos-3.0.3/python_aternos.egg-info/PKG-INFO
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      692 2023-07-04 10:57:30.000000 python-aternos-3.0.3/python_aternos.egg-info/SOURCES.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)        1 2023-07-04 10:57:30.000000 python-aternos-3.0.3/python_aternos.egg-info/dependency_links.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      283 2023-07-04 10:57:30.000000 python-aternos-3.0.3/python_aternos.egg-info/requires.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)       15 2023-07-04 10:57:30.000000 python-aternos-3.0.3/python_aternos.egg-info/top_level.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      131 2023-07-04 10:57:30.170874 python-aternos-3.0.3/setup.cfg
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2139 2023-07-04 10:47:42.000000 python-aternos-3.0.3/setup.py
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:57:30.170874 python-aternos-3.0.3/tests/
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      923 2023-05-29 07:11:46.000000 python-aternos-3.0.3/tests/test_http.py
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1947 2022-12-25 13:47:12.000000 python-aternos-3.0.3/tests/test_js2py.py
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      741 2023-01-13 12:15:15.000000 python-aternos-3.0.3/tests/test_jsnode.py
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1191 2023-05-24 15:32:24.000000 python-aternos-3.0.3/tests/test_login.py
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-27 06:59:45.219407 python-aternos-3.0.4/
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    11357 2022-02-15 14:48:20.000000 python-aternos-3.0.4/LICENSE
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      562 2022-08-23 06:43:33.000000 python-aternos-3.0.4/NOTICE
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7105 2023-07-27 06:59:45.219407 python-aternos-3.0.4/PKG-INFO
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5818 2023-07-04 10:56:37.000000 python-aternos-3.0.4/README.md
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      110 2022-07-01 10:05:05.000000 python-aternos-3.0.4/pyproject.toml
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-27 06:59:45.219407 python-aternos-3.0.4/python_aternos/
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      317 2023-05-29 07:28:42.000000 python-aternos-3.0.4/python_aternos/__init__.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6067 2023-05-29 05:43:14.000000 python-aternos-3.0.4/python_aternos/ataccount.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6926 2023-06-30 05:54:30.000000 python-aternos-3.0.4/python_aternos/atclient.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10133 2023-05-29 07:09:48.000000 python-aternos-3.0.4/python_aternos/atconf.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8889 2023-07-04 10:42:47.000000 python-aternos-3.0.4/python_aternos/atconnect.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2406 2022-10-31 13:26:01.000000 python-aternos-3.0.4/python_aternos/aterrors.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8655 2023-05-24 13:38:15.000000 python-aternos-3.0.4/python_aternos/atfile.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5259 2023-05-24 13:39:35.000000 python-aternos-3.0.4/python_aternos/atfm.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6001 2023-07-27 06:54:09.000000 python-aternos-3.0.4/python_aternos/atjsparse.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      579 2023-07-04 10:47:12.000000 python-aternos-3.0.4/python_aternos/atlog.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      344 2023-05-24 15:59:49.000000 python-aternos-3.0.4/python_aternos/atmd5.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     3329 2023-07-04 10:42:58.000000 python-aternos-3.0.4/python_aternos/atplayers.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10912 2023-05-29 08:06:02.000000 python-aternos-3.0.4/python_aternos/atserver.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     9974 2023-06-30 06:36:36.000000 python-aternos-3.0.4/python_aternos/atwss.py
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-27 06:59:45.219407 python-aternos-3.0.4/python_aternos.egg-info/
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7105 2023-07-27 06:59:45.000000 python-aternos-3.0.4/python_aternos.egg-info/PKG-INFO
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      692 2023-07-27 06:59:45.000000 python-aternos-3.0.4/python_aternos.egg-info/SOURCES.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)        1 2023-07-27 06:59:45.000000 python-aternos-3.0.4/python_aternos.egg-info/dependency_links.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      283 2023-07-27 06:59:45.000000 python-aternos-3.0.4/python_aternos.egg-info/requires.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)       15 2023-07-27 06:59:45.000000 python-aternos-3.0.4/python_aternos.egg-info/top_level.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      131 2023-07-27 06:59:45.219407 python-aternos-3.0.4/setup.cfg
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2139 2023-07-27 06:59:30.000000 python-aternos-3.0.4/setup.py
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-27 06:59:45.219407 python-aternos-3.0.4/tests/
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      923 2023-05-29 07:11:46.000000 python-aternos-3.0.4/tests/test_http.py
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1947 2022-12-25 13:47:12.000000 python-aternos-3.0.4/tests/test_js2py.py
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      741 2023-01-13 12:15:15.000000 python-aternos-3.0.4/tests/test_jsnode.py
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1191 2023-05-24 15:32:24.000000 python-aternos-3.0.4/tests/test_login.py
```

### Comparing `python-aternos-3.0.3/LICENSE` & `python-aternos-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/NOTICE` & `python-aternos-3.0.4/NOTICE`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/PKG-INFO` & `python-aternos-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-aternos
-Version: 3.0.3
+Version: 3.0.4
 Summary: An unofficial Aternos API
 Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09)
 Author-email: aacd0709@mail.ru
 Project-URL: Documentation, https://python-aternos.codeberg.page
 Project-URL: GitHub, https://github.com/DarkCat09/python-aternos
 Project-URL: Bug Tracker, https://github.com/DarkCat09/python-aternos/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-aternos Version: 3.0.3 Summary: An
+Metadata-Version: 2.1 Name: python-aternos Version: 3.0.4 Summary: An
 unofficial Aternos API Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09) Author-email: aacd0709@mail.ru Project-
 URL: Documentation, https://python-aternos.codeberg.page Project-URL: GitHub,
 https://github.com/DarkCat09/python-aternos Project-URL: Bug Tracker, https://
 github.com/DarkCat09/python-aternos/issues Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `python-aternos-3.0.3/README.md` & `python-aternos-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/python_aternos/ataccount.py` & `python-aternos-3.0.4/python_aternos/ataccount.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/python_aternos/atclient.py` & `python-aternos-3.0.4/python_aternos/atclient.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/python_aternos/atconf.py` & `python-aternos-3.0.4/python_aternos/atconf.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/python_aternos/atconnect.py` & `python-aternos-3.0.4/python_aternos/atconnect.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/python_aternos/aterrors.py` & `python-aternos-3.0.4/python_aternos/aterrors.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/python_aternos/atfile.py` & `python-aternos-3.0.4/python_aternos/atfile.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/python_aternos/atfm.py` & `python-aternos-3.0.4/python_aternos/atfm.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/python_aternos/atjsparse.py` & `python-aternos-3.0.4/python_aternos/atjsparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,19 +135,22 @@
         super().__init__()
 
         ctx = js2py.EvalJs({'atob': atob})
         ctx.execute('''
         window.Map = function(_i){ };
         window.setTimeout = function(_f,_t){ };
         window.setInterval = function(_f,_t){ };
-        window.encodeURIComponent = function(_s){ };
+        window.encodeURIComponent = window.Map;
         window.document = { };
         document.doctype = { };
         document.currentScript = { };
-        document.getElementById = function(_s){ };
+        document.getElementById = window.Map;
+        document.prepend = window.Map;
+        document.append = window.Map;
+        document.appendChild = window.Map;
         ''')
 
         self.ctx = ctx
 
     def exec_js(self, func: str) -> None:
         self.ctx.execute(self.to_ecma5(func))
```

### Comparing `python-aternos-3.0.3/python_aternos/atlog.py` & `python-aternos-3.0.4/python_aternos/atlog.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/python_aternos/atplayers.py` & `python-aternos-3.0.4/python_aternos/atplayers.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/python_aternos/atserver.py` & `python-aternos-3.0.4/python_aternos/atserver.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/python_aternos/atwss.py` & `python-aternos-3.0.4/python_aternos/atwss.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/python_aternos.egg-info/PKG-INFO` & `python-aternos-3.0.4/python_aternos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-aternos
-Version: 3.0.3
+Version: 3.0.4
 Summary: An unofficial Aternos API
 Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09)
 Author-email: aacd0709@mail.ru
 Project-URL: Documentation, https://python-aternos.codeberg.page
 Project-URL: GitHub, https://github.com/DarkCat09/python-aternos
 Project-URL: Bug Tracker, https://github.com/DarkCat09/python-aternos/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-aternos Version: 3.0.3 Summary: An
+Metadata-Version: 2.1 Name: python-aternos Version: 3.0.4 Summary: An
 unofficial Aternos API Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09) Author-email: aacd0709@mail.ru Project-
 URL: Documentation, https://python-aternos.codeberg.page Project-URL: GitHub,
 https://github.com/DarkCat09/python-aternos Project-URL: Bug Tracker, https://
 github.com/DarkCat09/python-aternos/issues Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `python-aternos-3.0.3/python_aternos.egg-info/SOURCES.txt` & `python-aternos-3.0.4/python_aternos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/setup.py` & `python-aternos-3.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'rt') as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name='python-aternos',
-    version='3.0.3',
+    version='3.0.4',
     author='Chechkenev Andrey (@DarkCat09)',
     author_email='aacd0709@mail.ru',
     description='An unofficial Aternos API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/DarkCat09/python-aternos',
     project_urls={
```

### Comparing `python-aternos-3.0.3/tests/test_http.py` & `python-aternos-3.0.4/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/tests/test_js2py.py` & `python-aternos-3.0.4/tests/test_js2py.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/tests/test_jsnode.py` & `python-aternos-3.0.4/tests/test_jsnode.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.3/tests/test_login.py` & `python-aternos-3.0.4/tests/test_login.py`

 * *Files identical despite different names*

