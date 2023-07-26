# Comparing `tmp/hspylib-hqt-0.9.8.tar.gz` & `tmp/hspylib-hqt-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-hqt-0.9.8.tar", last modified: Wed Jul 26 22:06:37 2023, max compression
+gzip compressed data, was "hspylib-hqt-0.9.9.tar", last modified: Wed Jul 26 23:02:17 2023, max compression
```

## Comparing `hspylib-hqt-0.9.8.tar` & `hspylib-hqt-0.9.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 22:06:37.255998 hspylib-hqt-0.9.8/
--rw-r--r--   0 hjunior    (504) staff       (20)       21 2023-04-18 22:21:01.000000 hspylib-hqt-0.9.8/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)    12094 2023-07-26 22:06:37.254993 hspylib-hqt-0.9.8/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)    11082 2023-07-26 22:06:36.000000 hspylib-hqt-0.9.8/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 22:06:37.214029 hspylib-hqt-0.9.8/hqt/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-26 22:06:36.000000 hspylib-hqt-0.9.8/hqt/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      206 2023-07-26 22:06:36.000000 hspylib-hqt-0.9.8/hqt/__init__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 22:06:37.237168 hspylib-hqt-0.9.8/hqt/promotions/
--rw-r--r--   0 hjunior    (504) staff       (20)      302 2023-07-26 22:06:36.000000 hspylib-hqt-0.9.8/hqt/promotions/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      838 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.8/hqt/promotions/hcombobox.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7680 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.8/hqt/promotions/hconsole.py
--rw-r--r--   0 hjunior    (504) staff       (20)      667 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.8/hqt/promotions/hframe.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2570 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.8/hqt/promotions/hlabel.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6562 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.8/hqt/promotions/hlistwidget.py
--rw-r--r--   0 hjunior    (504) staff       (20)     4414 2023-07-26 18:11:27.000000 hspylib-hqt-0.9.8/hqt/promotions/hstacked_widget.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6227 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.8/hqt/promotions/htablemodel.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5448 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.8/hqt/promotions/htableview.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6283 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.8/hqt/promotions/htoolbox.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2592 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.8/hqt/qt_application.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3854 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.8/hqt/stream_capturer.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 22:06:37.244740 hspylib-hqt-0.9.8/hqt/views/
--rw-r--r--   0 hjunior    (504) staff       (20)      166 2023-07-26 22:06:36.000000 hspylib-hqt-0.9.8/hqt/views/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      862 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.8/hqt/views/main_view.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2313 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.8/hqt/views/qt_view.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 22:06:37.253408 hspylib-hqt-0.9.8/hspylib_hqt.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)    12094 2023-07-26 22:06:36.000000 hspylib-hqt-0.9.8/hspylib_hqt.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      626 2023-07-26 22:06:37.000000 hspylib-hqt-0.9.8/hspylib_hqt.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-26 22:06:36.000000 hspylib-hqt-0.9.8/hspylib_hqt.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       36 2023-07-26 22:06:36.000000 hspylib-hqt-0.9.8/hspylib_hqt.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        4 2023-07-26 22:06:36.000000 hspylib-hqt-0.9.8/hspylib_hqt.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-26 22:06:37.256157 hspylib-hqt-0.9.8/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     2071 2023-04-19 22:12:01.000000 hspylib-hqt-0.9.8/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 23:02:17.224942 hspylib-hqt-0.9.9/
+-rw-r--r--   0 hjunior    (504) staff       (20)       21 2023-04-18 22:21:01.000000 hspylib-hqt-0.9.9/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)    12094 2023-07-26 23:02:17.223667 hspylib-hqt-0.9.9/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)    11082 2023-07-26 23:02:08.000000 hspylib-hqt-0.9.9/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 23:02:17.163288 hspylib-hqt-0.9.9/hqt/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-26 23:02:08.000000 hspylib-hqt-0.9.9/hqt/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      206 2023-07-26 23:02:08.000000 hspylib-hqt-0.9.9/hqt/__init__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 23:02:17.201431 hspylib-hqt-0.9.9/hqt/promotions/
+-rw-r--r--   0 hjunior    (504) staff       (20)      302 2023-07-26 23:02:08.000000 hspylib-hqt-0.9.9/hqt/promotions/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      838 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.9/hqt/promotions/hcombobox.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7680 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.9/hqt/promotions/hconsole.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      667 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.9/hqt/promotions/hframe.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2570 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.9/hqt/promotions/hlabel.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6562 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.9/hqt/promotions/hlistwidget.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4414 2023-07-26 18:11:27.000000 hspylib-hqt-0.9.9/hqt/promotions/hstacked_widget.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6227 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.9/hqt/promotions/htablemodel.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     5448 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.9/hqt/promotions/htableview.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6283 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.9/hqt/promotions/htoolbox.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2592 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.9/hqt/qt_application.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3854 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.9/hqt/stream_capturer.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 23:02:17.211278 hspylib-hqt-0.9.9/hqt/views/
+-rw-r--r--   0 hjunior    (504) staff       (20)      166 2023-07-26 23:02:08.000000 hspylib-hqt-0.9.9/hqt/views/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      862 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.9/hqt/views/main_view.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2313 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.9/hqt/views/qt_view.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-26 23:02:17.221746 hspylib-hqt-0.9.9/hspylib_hqt.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)    12094 2023-07-26 23:02:17.000000 hspylib-hqt-0.9.9/hspylib_hqt.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      626 2023-07-26 23:02:17.000000 hspylib-hqt-0.9.9/hspylib_hqt.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-26 23:02:17.000000 hspylib-hqt-0.9.9/hspylib_hqt.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       36 2023-07-26 23:02:17.000000 hspylib-hqt-0.9.9/hspylib_hqt.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        9 2023-07-26 23:02:17.000000 hspylib-hqt-0.9.9/hspylib_hqt.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-26 23:02:17.225133 hspylib-hqt-0.9.9/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     2071 2023-04-19 22:12:01.000000 hspylib-hqt-0.9.9/setup.py
```

### Comparing `hspylib-hqt-0.9.8/PKG-INFO` & `hspylib-hqt-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-hqt
-Version: 0.9.8
+Version: 0.9.9
 Summary: HsPyLib - QT framework extensions
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-hqt/
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 
 # <img src="https://iili.io/HYBJFA7.png"  width="34" height="34"> HomeSetup Python Library - HsPyLib
 
 ## Your Python code is not JUST a script !!
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.8/gray)](docs/CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.9/gray)](docs/CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
 HsPyLib is a Python library that will elevate your experience to another level. It relies on well known principles as
 SOLID, DRY (Don't Repeat Yourself), KISS (Keep It Simple, Stupid) and YAGNI (You Ain’t Gonna Need It). It provides many
```

### Comparing `hspylib-hqt-0.9.8/README.md` & `hspylib-hqt-0.9.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # <img src="https://iili.io/HYBJFA7.png"  width="34" height="34"> HomeSetup Python Library - HsPyLib
 
 ## Your Python code is not JUST a script !!
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.8/gray)](docs/CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.9/gray)](docs/CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
 HsPyLib is a Python library that will elevate your experience to another level. It relies on well known principles as
 SOLID, DRY (Don't Repeat Yourself), KISS (Keep It Simple, Stupid) and YAGNI (You Ain’t Gonna Need It). It provides many
```

### Comparing `hspylib-hqt-0.9.8/hqt/promotions/hcombobox.py` & `hspylib-hqt-0.9.9/hqt/promotions/hcombobox.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.8/hqt/promotions/hconsole.py` & `hspylib-hqt-0.9.9/hqt/promotions/hconsole.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.8/hqt/promotions/hframe.py` & `hspylib-hqt-0.9.9/hqt/promotions/hframe.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.8/hqt/promotions/hlabel.py` & `hspylib-hqt-0.9.9/hqt/promotions/hlabel.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.8/hqt/promotions/hlistwidget.py` & `hspylib-hqt-0.9.9/hqt/promotions/hlistwidget.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.8/hqt/promotions/hstacked_widget.py` & `hspylib-hqt-0.9.9/hqt/promotions/hstacked_widget.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.8/hqt/promotions/htablemodel.py` & `hspylib-hqt-0.9.9/hqt/promotions/htablemodel.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.8/hqt/promotions/htableview.py` & `hspylib-hqt-0.9.9/hqt/promotions/htableview.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.8/hqt/promotions/htoolbox.py` & `hspylib-hqt-0.9.9/hqt/promotions/htoolbox.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.8/hqt/qt_application.py` & `hspylib-hqt-0.9.9/hqt/qt_application.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.8/hqt/stream_capturer.py` & `hspylib-hqt-0.9.9/hqt/stream_capturer.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.8/hqt/views/main_view.py` & `hspylib-hqt-0.9.9/hqt/views/main_view.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.8/hqt/views/qt_view.py` & `hspylib-hqt-0.9.9/hqt/views/qt_view.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.8/hspylib_hqt.egg-info/PKG-INFO` & `hspylib-hqt-0.9.9/hspylib_hqt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-hqt
-Version: 0.9.8
+Version: 0.9.9
 Summary: HsPyLib - QT framework extensions
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-hqt/
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 
 # <img src="https://iili.io/HYBJFA7.png"  width="34" height="34"> HomeSetup Python Library - HsPyLib
 
 ## Your Python code is not JUST a script !!
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.8/gray)](docs/CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.9/gray)](docs/CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
 HsPyLib is a Python library that will elevate your experience to another level. It relies on well known principles as
 SOLID, DRY (Don't Repeat Yourself), KISS (Keep It Simple, Stupid) and YAGNI (You Ain’t Gonna Need It). It provides many
```

### Comparing `hspylib-hqt-0.9.8/hspylib_hqt.egg-info/SOURCES.txt` & `hspylib-hqt-0.9.9/hspylib_hqt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.8/setup.py` & `hspylib-hqt-0.9.9/setup.py`

 * *Files identical despite different names*

