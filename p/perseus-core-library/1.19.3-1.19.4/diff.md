# Comparing `tmp/perseus_core_library-1.19.3.tar.gz` & `tmp/perseus_core_library-1.19.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perseus_core_library-1.19.3.tar", max compression
+gzip compressed data, was "perseus_core_library-1.19.4.tar", max compression
```

## Comparing `perseus_core_library-1.19.3.tar` & `perseus_core_library-1.19.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     4626 2023-06-14 07:57:54.260063 perseus_core_library-1.19.3/CHANGELOG.md
--rw-r--r--   0        0        0     1089 2020-11-13 04:28:53.612751 perseus_core_library-1.19.3/LICENSE
--rwxr-xr-x   0        0        0      611 2023-03-31 11:33:19.503540 perseus_core_library-1.19.3/README.md
--rw-r--r--   0        0        0      991 2023-06-14 07:57:54.256205 perseus_core_library-1.19.3/pyproject.toml
--rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.806929 perseus_core_library-1.19.3/src/majormode/__init__.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.807149 perseus_core_library-1.19.3/src/majormode/perseus/__init__.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.807322 perseus_core_library-1.19.3/src/majormode/perseus/constant/__init__.py
--rw-r--r--   0        0        0     1304 2022-11-23 14:11:27.807886 perseus_core_library-1.19.3/src/majormode/perseus/constant/account.py
--rw-r--r--   0        0        0     2681 2022-11-23 14:11:27.808081 perseus_core_library-1.19.3/src/majormode/perseus/constant/application.py
--rw-r--r--   0        0        0     1451 2022-11-23 14:11:27.808916 perseus_core_library-1.19.3/src/majormode/perseus/constant/area.py
--rw-r--r--   0        0        0     1225 2022-11-23 14:11:27.809504 perseus_core_library-1.19.3/src/majormode/perseus/constant/contact.py
--rw-r--r--   0        0        0     1287 2022-11-23 14:11:27.809738 perseus_core_library-1.19.3/src/majormode/perseus/constant/date.py
--rw-r--r--   0        0        0     1967 2022-11-23 14:11:27.810232 perseus_core_library-1.19.3/src/majormode/perseus/constant/http.py
--rw-r--r--   0        0        0    67093 2022-11-23 14:11:27.811739 perseus_core_library-1.19.3/src/majormode/perseus/constant/locale.py
--rw-r--r--   0        0        0     1660 2022-11-28 07:57:27.015219 perseus_core_library-1.19.3/src/majormode/perseus/constant/logging.py
--rw-r--r--   0        0        0     1507 2022-11-23 14:11:27.812751 perseus_core_library-1.19.3/src/majormode/perseus/constant/notification.py
--rw-r--r--   0        0        0     1487 2022-11-23 14:11:27.812967 perseus_core_library-1.19.3/src/majormode/perseus/constant/obj.py
--rw-r--r--   0        0        0     2148 2022-11-23 14:11:27.813172 perseus_core_library-1.19.3/src/majormode/perseus/constant/phone.py
--rw-r--r--   0        0        0     1495 2022-11-23 14:11:27.813400 perseus_core_library-1.19.3/src/majormode/perseus/constant/privacy.py
--rw-r--r--   0        0        0     5637 2023-02-08 23:35:16.851783 perseus_core_library-1.19.3/src/majormode/perseus/constant/regex.py
--rw-r--r--   0        0        0     1216 2022-11-23 14:11:27.814168 perseus_core_library-1.19.3/src/majormode/perseus/constant/sort_order.py
--rw-r--r--   0        0        0     2418 2022-11-23 14:11:27.814721 perseus_core_library-1.19.3/src/majormode/perseus/constant/stage.py
--rw-r--r--   0        0        0     1232 2022-11-23 14:11:27.815078 perseus_core_library-1.19.3/src/majormode/perseus/constant/team.py
--rw-r--r--   0        0        0     1327 2022-11-23 14:11:27.815626 perseus_core_library-1.19.3/src/majormode/perseus/constant/url.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.816075 perseus_core_library-1.19.3/src/majormode/perseus/model/__init__.py
--rw-r--r--   0        0        0     2090 2023-02-08 23:34:13.342813 perseus_core_library-1.19.3/src/majormode/perseus/model/api_key.py
--rw-r--r--   0        0        0     3084 2023-02-08 23:34:13.317988 perseus_core_library-1.19.3/src/majormode/perseus/model/app.py
--rw-r--r--   0        0        0     2399 2023-02-08 23:34:13.342720 perseus_core_library-1.19.3/src/majormode/perseus/model/connection.py
--rw-r--r--   0        0        0    11488 2023-02-09 07:44:07.812315 perseus_core_library-1.19.3/src/majormode/perseus/model/contact.py
--rw-r--r--   0        0        0     5180 2023-02-08 23:35:01.771581 perseus_core_library-1.19.3/src/majormode/perseus/model/date.py
--rw-r--r--   0        0        0     8875 2022-11-23 14:11:27.818448 perseus_core_library-1.19.3/src/majormode/perseus/model/enum.py
--rwxr-xr-x   0        0        0    20872 2023-02-09 04:41:42.263143 perseus_core_library-1.19.3/src/majormode/perseus/model/geolocation.py
--rwxr-xr-x   0        0        0     2358 2023-02-08 23:34:41.390129 perseus_core_library-1.19.3/src/majormode/perseus/model/label.py
--rwxr-xr-x   0        0        0    14564 2023-02-08 23:35:01.747393 perseus_core_library-1.19.3/src/majormode/perseus/model/locale.py
--rwxr-xr-x   0        0        0    10597 2023-02-08 23:35:01.794562 perseus_core_library-1.19.3/src/majormode/perseus/model/obj.py
--rw-r--r--   0        0        0     2349 2023-02-08 14:09:26.884197 perseus_core_library-1.19.3/src/majormode/perseus/model/picture.py
--rw-r--r--   0        0        0     2704 2023-02-08 23:34:13.342895 perseus_core_library-1.19.3/src/majormode/perseus/model/smtp.py
--rwxr-xr-x   0        0        0     8584 2022-11-23 14:11:27.822916 perseus_core_library-1.19.3/src/majormode/perseus/model/version.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.823305 perseus_core_library-1.19.3/src/majormode/perseus/utils/__init__.py
--rw-r--r--   0        0        0    19613 2023-02-08 23:35:01.817196 perseus_core_library-1.19.3/src/majormode/perseus/utils/cast.py
--rw-r--r--   0        0        0     5740 2023-02-08 23:35:01.816672 perseus_core_library-1.19.3/src/majormode/perseus/utils/date_util.py
--rw-r--r--   0        0        0     2009 2023-02-08 23:35:01.816582 perseus_core_library-1.19.3/src/majormode/perseus/utils/egg_util.py
--rw-r--r--   0        0        0     9876 2022-11-23 14:11:27.828666 perseus_core_library-1.19.3/src/majormode/perseus/utils/file_util.py
--rw-r--r--   0        0        0    17555 2022-11-23 14:11:27.829089 perseus_core_library-1.19.3/src/majormode/perseus/utils/image_util.py
--rw-r--r--   0        0        0     6208 2023-02-08 23:35:01.816626 perseus_core_library-1.19.3/src/majormode/perseus/utils/key_util.py
--rw-r--r--   0        0        0     3538 2023-04-04 02:18:22.869306 perseus_core_library-1.19.3/src/majormode/perseus/utils/logging.py
--rwxr-xr-x   0        0        0     6226 2022-11-23 14:11:27.829728 perseus_core_library-1.19.3/src/majormode/perseus/utils/logrotate.py
--rw-r--r--   0        0        0     2232 2022-11-23 14:11:27.830576 perseus_core_library-1.19.3/src/majormode/perseus/utils/module_util.py
--rw-r--r--   0        0        0    40681 2023-02-08 23:35:01.817460 perseus_core_library-1.19.3/src/majormode/perseus/utils/photo_util.py
--rw-r--r--   0        0        0     2748 2022-11-23 14:11:27.832666 perseus_core_library-1.19.3/src/majormode/perseus/utils/setup_util.py
--rw-r--r--   0        0        0     2325 2023-02-08 23:35:01.817123 perseus_core_library-1.19.3/src/majormode/perseus/utils/socket_util.py
--rw-r--r--   0        0        0     2659 2023-02-08 23:35:01.816384 perseus_core_library-1.19.3/src/majormode/perseus/utils/stage.py
--rw-r--r--   0        0        0     6352 2023-06-14 07:56:40.282483 perseus_core_library-1.19.3/src/majormode/perseus/utils/string_util.py
--rw-r--r--   0        0        0     4384 2023-02-08 23:35:01.816604 perseus_core_library-1.19.3/src/majormode/perseus/utils/zip_util.py
--rw-r--r--   0        0        0     1671 1970-01-01 00:00:00.000000 perseus_core_library-1.19.3/setup.py
--rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 perseus_core_library-1.19.3/PKG-INFO
+-rw-r--r--   0        0        0     4728 2023-07-27 02:42:32.477916 perseus_core_library-1.19.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1089 2020-11-13 04:28:53.612751 perseus_core_library-1.19.4/LICENSE
+-rwxr-xr-x   0        0        0      611 2023-03-31 11:33:19.503540 perseus_core_library-1.19.4/README.md
+-rw-r--r--   0        0        0      991 2023-07-27 02:43:12.693686 perseus_core_library-1.19.4/pyproject.toml
+-rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.806929 perseus_core_library-1.19.4/src/majormode/__init__.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.807149 perseus_core_library-1.19.4/src/majormode/perseus/__init__.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.807322 perseus_core_library-1.19.4/src/majormode/perseus/constant/__init__.py
+-rw-r--r--   0        0        0     1304 2022-11-23 14:11:27.807886 perseus_core_library-1.19.4/src/majormode/perseus/constant/account.py
+-rw-r--r--   0        0        0     2681 2022-11-23 14:11:27.808081 perseus_core_library-1.19.4/src/majormode/perseus/constant/application.py
+-rw-r--r--   0        0        0     1451 2022-11-23 14:11:27.808916 perseus_core_library-1.19.4/src/majormode/perseus/constant/area.py
+-rw-r--r--   0        0        0     1225 2022-11-23 14:11:27.809504 perseus_core_library-1.19.4/src/majormode/perseus/constant/contact.py
+-rw-r--r--   0        0        0     1287 2022-11-23 14:11:27.809738 perseus_core_library-1.19.4/src/majormode/perseus/constant/date.py
+-rw-r--r--   0        0        0     1967 2022-11-23 14:11:27.810232 perseus_core_library-1.19.4/src/majormode/perseus/constant/http.py
+-rw-r--r--   0        0        0    67093 2022-11-23 14:11:27.811739 perseus_core_library-1.19.4/src/majormode/perseus/constant/locale.py
+-rw-r--r--   0        0        0     1660 2022-11-28 07:57:27.015219 perseus_core_library-1.19.4/src/majormode/perseus/constant/logging.py
+-rw-r--r--   0        0        0     1507 2022-11-23 14:11:27.812751 perseus_core_library-1.19.4/src/majormode/perseus/constant/notification.py
+-rw-r--r--   0        0        0     1487 2022-11-23 14:11:27.812967 perseus_core_library-1.19.4/src/majormode/perseus/constant/obj.py
+-rw-r--r--   0        0        0     2148 2022-11-23 14:11:27.813172 perseus_core_library-1.19.4/src/majormode/perseus/constant/phone.py
+-rw-r--r--   0        0        0     1495 2022-11-23 14:11:27.813400 perseus_core_library-1.19.4/src/majormode/perseus/constant/privacy.py
+-rw-r--r--   0        0        0     6418 2023-07-27 02:41:19.900237 perseus_core_library-1.19.4/src/majormode/perseus/constant/regex.py
+-rw-r--r--   0        0        0     1216 2022-11-23 14:11:27.814168 perseus_core_library-1.19.4/src/majormode/perseus/constant/sort_order.py
+-rw-r--r--   0        0        0     2418 2022-11-23 14:11:27.814721 perseus_core_library-1.19.4/src/majormode/perseus/constant/stage.py
+-rw-r--r--   0        0        0     1232 2022-11-23 14:11:27.815078 perseus_core_library-1.19.4/src/majormode/perseus/constant/team.py
+-rw-r--r--   0        0        0     1327 2022-11-23 14:11:27.815626 perseus_core_library-1.19.4/src/majormode/perseus/constant/url.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.816075 perseus_core_library-1.19.4/src/majormode/perseus/model/__init__.py
+-rw-r--r--   0        0        0     2090 2023-02-08 23:34:13.342813 perseus_core_library-1.19.4/src/majormode/perseus/model/api_key.py
+-rw-r--r--   0        0        0     3084 2023-02-08 23:34:13.317988 perseus_core_library-1.19.4/src/majormode/perseus/model/app.py
+-rw-r--r--   0        0        0     2399 2023-02-08 23:34:13.342720 perseus_core_library-1.19.4/src/majormode/perseus/model/connection.py
+-rw-r--r--   0        0        0    11488 2023-02-09 07:44:07.812315 perseus_core_library-1.19.4/src/majormode/perseus/model/contact.py
+-rw-r--r--   0        0        0     5180 2023-02-08 23:35:01.771581 perseus_core_library-1.19.4/src/majormode/perseus/model/date.py
+-rw-r--r--   0        0        0     8875 2022-11-23 14:11:27.818448 perseus_core_library-1.19.4/src/majormode/perseus/model/enum.py
+-rwxr-xr-x   0        0        0    20872 2023-02-09 04:41:42.263143 perseus_core_library-1.19.4/src/majormode/perseus/model/geolocation.py
+-rwxr-xr-x   0        0        0     2358 2023-02-08 23:34:41.390129 perseus_core_library-1.19.4/src/majormode/perseus/model/label.py
+-rwxr-xr-x   0        0        0    14564 2023-02-08 23:35:01.747393 perseus_core_library-1.19.4/src/majormode/perseus/model/locale.py
+-rwxr-xr-x   0        0        0    10597 2023-02-08 23:35:01.794562 perseus_core_library-1.19.4/src/majormode/perseus/model/obj.py
+-rw-r--r--   0        0        0     2349 2023-02-08 14:09:26.884197 perseus_core_library-1.19.4/src/majormode/perseus/model/picture.py
+-rw-r--r--   0        0        0     2704 2023-02-08 23:34:13.342895 perseus_core_library-1.19.4/src/majormode/perseus/model/smtp.py
+-rwxr-xr-x   0        0        0     8584 2022-11-23 14:11:27.822916 perseus_core_library-1.19.4/src/majormode/perseus/model/version.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 14:11:27.823305 perseus_core_library-1.19.4/src/majormode/perseus/utils/__init__.py
+-rw-r--r--   0        0        0    19613 2023-02-08 23:35:01.817196 perseus_core_library-1.19.4/src/majormode/perseus/utils/cast.py
+-rw-r--r--   0        0        0     5740 2023-02-08 23:35:01.816672 perseus_core_library-1.19.4/src/majormode/perseus/utils/date_util.py
+-rw-r--r--   0        0        0     2009 2023-02-08 23:35:01.816582 perseus_core_library-1.19.4/src/majormode/perseus/utils/egg_util.py
+-rw-r--r--   0        0        0     9876 2022-11-23 14:11:27.828666 perseus_core_library-1.19.4/src/majormode/perseus/utils/file_util.py
+-rw-r--r--   0        0        0    17555 2022-11-23 14:11:27.829089 perseus_core_library-1.19.4/src/majormode/perseus/utils/image_util.py
+-rw-r--r--   0        0        0     6208 2023-02-08 23:35:01.816626 perseus_core_library-1.19.4/src/majormode/perseus/utils/key_util.py
+-rw-r--r--   0        0        0     3538 2023-04-04 02:18:22.869306 perseus_core_library-1.19.4/src/majormode/perseus/utils/logging.py
+-rwxr-xr-x   0        0        0     6226 2022-11-23 14:11:27.829728 perseus_core_library-1.19.4/src/majormode/perseus/utils/logrotate.py
+-rw-r--r--   0        0        0     2232 2022-11-23 14:11:27.830576 perseus_core_library-1.19.4/src/majormode/perseus/utils/module_util.py
+-rw-r--r--   0        0        0    40681 2023-02-08 23:35:01.817460 perseus_core_library-1.19.4/src/majormode/perseus/utils/photo_util.py
+-rw-r--r--   0        0        0     2748 2022-11-23 14:11:27.832666 perseus_core_library-1.19.4/src/majormode/perseus/utils/setup_util.py
+-rw-r--r--   0        0        0     2325 2023-02-08 23:35:01.817123 perseus_core_library-1.19.4/src/majormode/perseus/utils/socket_util.py
+-rw-r--r--   0        0        0     2659 2023-02-08 23:35:01.816384 perseus_core_library-1.19.4/src/majormode/perseus/utils/stage.py
+-rw-r--r--   0        0        0     6352 2023-06-14 07:56:40.282483 perseus_core_library-1.19.4/src/majormode/perseus/utils/string_util.py
+-rw-r--r--   0        0        0     4384 2023-02-08 23:35:01.816604 perseus_core_library-1.19.4/src/majormode/perseus/utils/zip_util.py
+-rw-r--r--   0        0        0     1671 1970-01-01 00:00:00.000000 perseus_core_library-1.19.4/setup.py
+-rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 perseus_core_library-1.19.4/PKG-INFO
```

### Comparing `perseus_core_library-1.19.3/CHANGELOG.md` & `perseus_core_library-1.19.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,28 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [1.19.4] - 2023-07-27
+### Changed
+- Support E.123 notation for international telephone numbers
+
 ## [1.19.3] - 2023-06-14
-## Fixed
+### Fixed
 - Fix the function `string_to_keywords` to filter keywords that are not composed of the minimal required number of characters
 
 ## [1.19.2] - 2023-04-04
-## Added
+### Added
 - Add the functions `set_up_logger` and `get_console_handler` in the new module `majormode.perseus.utils.logging`
 
 ## [1.19.0] - 2023-02-08
-## Added
+### Added
 - Move the class `ISO8601DateTime` to the new module `majormode.perseus.model.date`
 - Add the class `Picture` in the new module `majormode.perseus.model.picture`
 
 ## [1.18.24] - 2022-11-28
 ### Added
 - Add the method `cast_string_to_logging_level`
```

### Comparing `perseus_core_library-1.19.3/LICENSE` & `perseus_core_library-1.19.4/LICENSE`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/README.md` & `perseus_core_library-1.19.4/README.md`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/pyproject.toml` & `perseus_core_library-1.19.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 keywords = ["core", "library", "perseus"]
 license = "SEE LICENSE IN <LICENSE.md>"
 name = "perseus-core-library"
 packages = [{ include = "majormode", from = "src" }]
 readme = "README.md"
 repository = "https://github.com/majormode/perseus-core-python-library"
-version = "1.19.3"
+version = "1.19.4"
 
 [tool.poetry.dependencies]
 exifread = "^3.0.0"
 jsonpickle = "^3.0.1"
 pillow = "^9.5.0"
 python = "^3.9"
 python-dateutil = "^2.8.2"
```

### Comparing `perseus_core_library-1.19.3/src/majormode/__init__.py` & `perseus_core_library-1.19.4/src/majormode/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/__init__.py` & `perseus_core_library-1.19.4/src/majormode/perseus/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/__init__.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/account.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/account.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/application.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/application.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/area.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/area.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/contact.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/contact.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/date.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/date.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/http.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/http.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/locale.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/locale.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/logging.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/logging.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/notification.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/notification.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/obj.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/obj.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/phone.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/phone.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/privacy.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/privacy.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/regex.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/regex.py`

 * *Files 11% similar despite different names*

```diff
@@ -74,20 +74,41 @@
 # Contact Mapping).  EPP-style phone numbers use the format
 # `+CCC.NNNNNNNNNNxEEEE`, where `C` is the 1–3 digit country code,
 # `N` is up to 14 digits, and `E` is the (optional) extension.  The
 # leading plus sign and the dot following the country code are required.
 # The literal "x" character is required only if an extension is provided.
 #
 # References :
-# - E.164 numbering plan; https://www.itu.int/rec/T-REC-E.164-201011-I/en>
-# - Extensible Provisioning Protocol (EPP) Contact Mapping);
+#
+# - E.164 Numbering plan; https://www.itu.int/rec/T-REC-E.164-201011-I/en,
+#   https://en.wikipedia.org/wiki/E.164
+#
+# - E.123 Notation for national and international telephone numbers,
+#   e-mail addresses and web addresses;
+#   https://en.wikipedia.org/wiki/E.123
+#
+#   For digit grouping, E.123 specifically recommends that:
+#
+#   - Only spaces be used to visually separate groups of numbers "unless
+#     an agreed upon explicit symbol (e.g. hyphen) is necessary for
+#     procedural purposes" in national notation;
+#   - Only spaces should be used to visually separate groups of numbers
+#     in international notation;
+#   - Spaces should separate country code, area code and local number.
+#
+# - Extensible Provisioning Protocol (EPP) Contact Mapping)
 #   https://tools.ietf.org/html/rfc5733#section-2.5
 #
-# @depracated: REGEX_PATTERN_PHONE_NUMBER = r'(([+][(]?[0-9]{1,3}[)]?)|([(]?[0-9]{4}[)]?))\s*[)]?[-\s\.]?[(]?[0-9]{1,3}[)]?([-\s\.]?[0-9]{3})([-\s\.]?[0-9]{3,4})'
-REGEX_PATTERN_PHONE_NUMBER = r'^\+[0-9]{1,3}\.[0-9]{4,14}(?:x.+)?$'
+#
+# @patch: [2023-06-27] We made the dot (following the country code)
+#   optional to support E.123 Notation for international telephone
+#   numbers.
+#
+# @deprecated: REGEX_PATTERN_PHONE_NUMBER = r'(([+][(]?[0-9]{1,3}[)]?)|([(]?[0-9]{4}[)]?))\s*[)]?[-\s\.]?[(]?[0-9]{1,3}[)]?([-\s\.]?[0-9]{3})([-\s\.]?[0-9]{3,4})'
+REGEX_PATTERN_PHONE_NUMBER = r'^\+[0-9]{1,3}\.{0,1}[0-9]{4,14}(?:x.+)?$'
 
 # Pattern of a regular expression to match a username:
 #
 # 1. MUST only contain lowercase/uppercase letters, digits, underscores,
 #    and periods
 #
 # 2. MUST start with a lowercase/uppercase letter
```

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/sort_order.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/sort_order.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/stage.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/stage.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/team.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/team.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/constant/url.py` & `perseus_core_library-1.19.4/src/majormode/perseus/constant/url.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/model/__init__.py` & `perseus_core_library-1.19.4/src/majormode/perseus/model/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/model/api_key.py` & `perseus_core_library-1.19.4/src/majormode/perseus/model/api_key.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/model/app.py` & `perseus_core_library-1.19.4/src/majormode/perseus/model/app.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/model/connection.py` & `perseus_core_library-1.19.4/src/majormode/perseus/model/connection.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/model/contact.py` & `perseus_core_library-1.19.4/src/majormode/perseus/model/contact.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/model/date.py` & `perseus_core_library-1.19.4/src/majormode/perseus/model/date.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/model/enum.py` & `perseus_core_library-1.19.4/src/majormode/perseus/model/enum.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/model/geolocation.py` & `perseus_core_library-1.19.4/src/majormode/perseus/model/geolocation.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/model/label.py` & `perseus_core_library-1.19.4/src/majormode/perseus/model/label.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/model/locale.py` & `perseus_core_library-1.19.4/src/majormode/perseus/model/locale.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/model/obj.py` & `perseus_core_library-1.19.4/src/majormode/perseus/model/obj.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/model/picture.py` & `perseus_core_library-1.19.4/src/majormode/perseus/model/picture.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/model/smtp.py` & `perseus_core_library-1.19.4/src/majormode/perseus/model/smtp.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/model/version.py` & `perseus_core_library-1.19.4/src/majormode/perseus/model/version.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/__init__.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/cast.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/cast.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/date_util.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/date_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/egg_util.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/egg_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/file_util.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/image_util.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/image_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/key_util.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/key_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/logging.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/logging.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/logrotate.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/logrotate.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/module_util.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/module_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/photo_util.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/photo_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/setup_util.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/setup_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/socket_util.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/socket_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/stage.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/stage.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/string_util.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/string_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/src/majormode/perseus/utils/zip_util.py` & `perseus_core_library-1.19.4/src/majormode/perseus/utils/zip_util.py`

 * *Files identical despite different names*

### Comparing `perseus_core_library-1.19.3/setup.py` & `perseus_core_library-1.19.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'python-dateutil>=2.8.2,<3.0.0',
  'pytz>=2023.3,<2024.0',
  'six>=1.16.0,<2.0.0',
  'unidecode>=1.3.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'perseus-core-library',
-    'version': '1.19.3',
+    'version': '1.19.4',
     'description': 'Perseus Core Python library',
     'long_description': '# Perseus: Core Python Library\n\nPerseus Core Python Library is a repository of reusable Python components to be shared with Python projects integrating Perseus RESTful API server framework.\n\nThese components have minimal dependencies on other libraries, so that they can be deployed easily.  In addition, these components will keep their interfaces as stable as possible, so that other Python projects can integrate these components without having to worry about changes in the future.\n\n\nTo install the Perseus Core Python Library, enter the follow command line:\n\n```bash\n$ pip install perseus-core-library\n```\n',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel.caune@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/majormode/perseus-core-python-library',
```

### Comparing `perseus_core_library-1.19.3/PKG-INFO` & `perseus_core_library-1.19.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perseus-core-library
-Version: 1.19.3
+Version: 1.19.4
 Summary: Perseus Core Python library
 Home-page: https://github.com/majormode/perseus-core-python-library
 License: SEE LICENSE IN <LICENSE.md>
 Keywords: core,library,perseus
 Author: Daniel CAUNE
 Author-email: daniel.caune@gmail.com
 Requires-Python: >=3.9,<4.0
```

