# Comparing `tmp/garth-0.2.7.tar.gz` & `tmp/garth-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.2.7.tar", last modified: Thu Jul 27 07:03:35 2023, max compression
+gzip compressed data, was "garth-0.2.8.tar", last modified: Thu Jul 27 07:08:20 2023, max compression
```

## Comparing `garth-0.2.7.tar` & `garth-0.2.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.2.7/LICENSE
--rw-r--r--   0        0        0     4529 2023-07-27 00:58:56.322378 garth-0.2.7/README.md
--rw-r--r--   0        0        0      390 2023-07-27 01:55:22.122866 garth-0.2.7/garth/__init__.py
--rw-r--r--   0        0        0      913 2023-07-23 13:39:36.444380 garth-0.2.7/garth/auth_token.py
--rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.2.7/garth/exc.py
--rw-r--r--   0        0        0     4852 2023-07-26 18:12:31.231364 garth-0.2.7/garth/http.py
--rw-r--r--   0        0        0        0 2023-07-27 07:00:55.127101 garth-0.2.7/garth/py.typed
--rw-r--r--   0        0        0       89 2023-07-27 01:55:22.123534 garth-0.2.7/garth/resources/__init__.py
--rw-r--r--   0        0        0      666 2023-07-27 06:53:34.111275 garth-0.2.7/garth/resources/stress.py
--rw-r--r--   0        0        0     3552 2023-07-23 16:09:16.949253 garth-0.2.7/garth/sso.py
--rw-r--r--   0        0        0     1617 2023-07-27 06:43:30.470402 garth-0.2.7/garth/stats.py
--rw-r--r--   0        0        0      542 2023-07-27 06:15:45.456562 garth-0.2.7/garth/utils.py
--rw-r--r--   0        0        0       22 2023-07-27 07:03:21.130352 garth-0.2.7/garth/version.py
--rw-r--r--   0        0        0      917 2023-07-27 07:03:35.429026 garth-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.2.7/tests/cassettes/test_client_get.yaml
--rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.2.7/tests/cassettes/test_client_post.yaml
--rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.2.7/tests/cassettes/test_client_request.yaml
--rw-r--r--   0        0        0     2331 2023-07-23 16:06:33.706591 garth-0.2.7/tests/cassettes/test_connectapi.yaml
--rw-r--r--   0        0        0     4564 2023-07-23 16:06:33.706751 garth-0.2.7/tests/cassettes/test_connectapi_refresh.yaml
--rw-r--r--   0        0        0     3231 2023-07-23 13:06:17.267462 garth-0.2.7/tests/cassettes/test_exchange.yaml
--rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.2.7/tests/cassettes/test_get_username.yaml
--rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.2.7/tests/cassettes/test_login_email_password_fail.yaml
--rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.2.7/tests/cassettes/test_login_success.yaml
--rw-r--r--   0        0        0     2270 2023-07-23 13:09:36.525519 garth-0.2.7/tests/cassettes/test_refresh.yaml
--rw-r--r--   0        0        0     2963 2023-07-23 13:36:21.976543 garth-0.2.7/tests/cassettes/test_refresh_expired.yaml
--rw-r--r--   0        0        0     2930 2023-07-26 18:12:31.231737 garth-0.2.7/tests/conftest.py
--rw-r--r--   0        0        0     6252 2023-07-26 13:24:49.161636 garth-0.2.7/tests/resources/cassettes/test_daily.yaml
--rw-r--r--   0        0        0    44427 2023-07-27 06:53:40.937606 garth-0.2.7/tests/resources/cassettes/test_daily_pagination.yaml
--rw-r--r--   0        0        0     4717 2023-07-26 13:24:49.162252 garth-0.2.7/tests/resources/cassettes/test_weekly.yaml
--rw-r--r--   0        0        0     7522 2023-07-26 13:24:49.162569 garth-0.2.7/tests/resources/cassettes/test_weekly_pagination.yaml
--rw-r--r--   0        0        0     1176 2023-07-27 06:52:51.197184 garth-0.2.7/tests/resources/test_stress.py
--rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.2.7/tests/test_auth_token.py
--rw-r--r--   0        0        0     4296 2023-07-26 18:12:31.231936 garth-0.2.7/tests/test_http.py
--rw-r--r--   0        0        0     2570 2023-07-23 13:18:13.595293 garth-0.2.7/tests/test_sso.py
--rw-r--r--   0        0        0      531 2023-07-27 06:36:04.840395 garth-0.2.7/tests/test_utils.py
--rw-r--r--   0        0        0     4792 1970-01-01 00:00:00.000000 garth-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.2.8/LICENSE
+-rw-r--r--   0        0        0     4529 2023-07-27 00:58:56.322378 garth-0.2.8/README.md
+-rw-r--r--   0        0        0      390 2023-07-27 01:55:22.122866 garth-0.2.8/garth/__init__.py
+-rw-r--r--   0        0        0      913 2023-07-23 13:39:36.444380 garth-0.2.8/garth/auth_token.py
+-rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.2.8/garth/exc.py
+-rw-r--r--   0        0        0     4852 2023-07-26 18:12:31.231364 garth-0.2.8/garth/http.py
+-rw-r--r--   0        0        0        0 2023-07-27 07:00:55.127101 garth-0.2.8/garth/py.typed
+-rw-r--r--   0        0        0       89 2023-07-27 01:55:22.123534 garth-0.2.8/garth/resources/__init__.py
+-rw-r--r--   0        0        0      666 2023-07-27 06:53:34.111275 garth-0.2.8/garth/resources/stress.py
+-rw-r--r--   0        0        0     3552 2023-07-23 16:09:16.949253 garth-0.2.8/garth/sso.py
+-rw-r--r--   0        0        0     1617 2023-07-27 06:43:30.470402 garth-0.2.8/garth/stats.py
+-rw-r--r--   0        0        0      542 2023-07-27 06:15:45.456562 garth-0.2.8/garth/utils.py
+-rw-r--r--   0        0        0       22 2023-07-27 07:07:00.511661 garth-0.2.8/garth/version.py
+-rw-r--r--   0        0        0     1069 2023-07-27 07:08:20.434488 garth-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.2.8/tests/cassettes/test_client_get.yaml
+-rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.2.8/tests/cassettes/test_client_post.yaml
+-rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.2.8/tests/cassettes/test_client_request.yaml
+-rw-r--r--   0        0        0     2331 2023-07-23 16:06:33.706591 garth-0.2.8/tests/cassettes/test_connectapi.yaml
+-rw-r--r--   0        0        0     4564 2023-07-23 16:06:33.706751 garth-0.2.8/tests/cassettes/test_connectapi_refresh.yaml
+-rw-r--r--   0        0        0     3231 2023-07-23 13:06:17.267462 garth-0.2.8/tests/cassettes/test_exchange.yaml
+-rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.2.8/tests/cassettes/test_get_username.yaml
+-rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.2.8/tests/cassettes/test_login_email_password_fail.yaml
+-rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.2.8/tests/cassettes/test_login_success.yaml
+-rw-r--r--   0        0        0     2270 2023-07-23 13:09:36.525519 garth-0.2.8/tests/cassettes/test_refresh.yaml
+-rw-r--r--   0        0        0     2963 2023-07-23 13:36:21.976543 garth-0.2.8/tests/cassettes/test_refresh_expired.yaml
+-rw-r--r--   0        0        0     2930 2023-07-26 18:12:31.231737 garth-0.2.8/tests/conftest.py
+-rw-r--r--   0        0        0     6252 2023-07-26 13:24:49.161636 garth-0.2.8/tests/resources/cassettes/test_daily.yaml
+-rw-r--r--   0        0        0    44427 2023-07-27 06:53:40.937606 garth-0.2.8/tests/resources/cassettes/test_daily_pagination.yaml
+-rw-r--r--   0        0        0     4717 2023-07-26 13:24:49.162252 garth-0.2.8/tests/resources/cassettes/test_weekly.yaml
+-rw-r--r--   0        0        0     7522 2023-07-26 13:24:49.162569 garth-0.2.8/tests/resources/cassettes/test_weekly_pagination.yaml
+-rw-r--r--   0        0        0     1176 2023-07-27 06:52:51.197184 garth-0.2.8/tests/resources/test_stress.py
+-rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.2.8/tests/test_auth_token.py
+-rw-r--r--   0        0        0     4296 2023-07-26 18:12:31.231936 garth-0.2.8/tests/test_http.py
+-rw-r--r--   0        0        0     2570 2023-07-23 13:18:13.595293 garth-0.2.8/tests/test_sso.py
+-rw-r--r--   0        0        0      531 2023-07-27 06:36:04.840395 garth-0.2.8/tests/test_utils.py
+-rw-r--r--   0        0        0     4941 1970-01-01 00:00:00.000000 garth-0.2.8/PKG-INFO
```

### Comparing `garth-0.2.7/LICENSE` & `garth-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/README.md` & `garth-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/garth/auth_token.py` & `garth-0.2.8/garth/auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/garth/http.py` & `garth-0.2.8/garth/http.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/garth/resources/stress.py` & `garth-0.2.8/garth/resources/stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/garth/sso.py` & `garth-0.2.8/garth/sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/garth/stats.py` & `garth-0.2.8/garth/stats.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/garth/utils.py` & `garth-0.2.8/garth/utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/pyproject.toml` & `garth-0.2.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 ]
 dependencies = [
     "requests",
     "pydantic",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
-version = "0.2.7"
+classifiers = [
+    "Operating System :: MacOS :: MacOS X",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: POSIX :: Linux",
+]
+version = "0.2.8"
 
 [project.license]
 text = "MIT"
 
 [project.packages]
 include = [
     { from = ".", include = "garth" },
```

### Comparing `garth-0.2.7/tests/cassettes/test_client_get.yaml` & `garth-0.2.8/tests/cassettes/test_client_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/cassettes/test_client_post.yaml` & `garth-0.2.8/tests/cassettes/test_client_post.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/cassettes/test_client_request.yaml` & `garth-0.2.8/tests/cassettes/test_client_request.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/cassettes/test_connectapi.yaml` & `garth-0.2.8/tests/cassettes/test_connectapi.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/cassettes/test_connectapi_refresh.yaml` & `garth-0.2.8/tests/cassettes/test_connectapi_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/cassettes/test_exchange.yaml` & `garth-0.2.8/tests/cassettes/test_exchange.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/cassettes/test_get_username.yaml` & `garth-0.2.8/tests/cassettes/test_get_username.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/cassettes/test_login_email_password_fail.yaml` & `garth-0.2.8/tests/cassettes/test_login_email_password_fail.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/cassettes/test_login_success.yaml` & `garth-0.2.8/tests/cassettes/test_login_success.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/cassettes/test_refresh.yaml` & `garth-0.2.8/tests/cassettes/test_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/cassettes/test_refresh_expired.yaml` & `garth-0.2.8/tests/cassettes/test_refresh_expired.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/conftest.py` & `garth-0.2.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/resources/cassettes/test_daily.yaml` & `garth-0.2.8/tests/resources/cassettes/test_daily.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/resources/cassettes/test_daily_pagination.yaml` & `garth-0.2.8/tests/resources/cassettes/test_daily_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/resources/cassettes/test_weekly.yaml` & `garth-0.2.8/tests/resources/cassettes/test_weekly.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/resources/cassettes/test_weekly_pagination.yaml` & `garth-0.2.8/tests/resources/cassettes/test_weekly_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/resources/test_stress.py` & `garth-0.2.8/tests/resources/test_stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/test_auth_token.py` & `garth-0.2.8/tests/test_auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/test_http.py` & `garth-0.2.8/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/test_sso.py` & `garth-0.2.8/tests/test_sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/tests/test_utils.py` & `garth-0.2.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.7/PKG-INFO` & `garth-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: garth
-Version: 0.2.7
+Version: 0.2.8
 Summary: Garmin SSO auth + Connect client
 Author-Email: Matin Tamizi <mtamizi@duck.com>
 License: MIT
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Requires-Dist: requests
 Requires-Dist: pydantic
 Description-Content-Type: text/markdown
 
 # Garth
```

