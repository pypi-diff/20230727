# Comparing `tmp/garth-0.2.4.tar.gz` & `tmp/garth-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.2.4.tar", last modified: Wed Jul 26 14:57:14 2023, max compression
+gzip compressed data, was "garth-0.2.5.tar", last modified: Thu Jul 27 00:59:14 2023, max compression
```

## Comparing `garth-0.2.4.tar` & `garth-0.2.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.2.4/LICENSE
--rw-r--r--   0        0        0     4531 2023-07-26 13:24:49.157851 garth-0.2.4/README.md
--rw-r--r--   0        0        0      408 2023-07-26 13:24:49.158278 garth-0.2.4/garth/__init__.py
--rw-r--r--   0        0        0      913 2023-07-23 13:39:36.444380 garth-0.2.4/garth/auth_token.py
--rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.2.4/garth/exc.py
--rw-r--r--   0        0        0     4870 2023-07-23 16:06:33.692262 garth-0.2.4/garth/http.py
--rw-r--r--   0        0        0       89 2023-07-26 13:24:49.158749 garth-0.2.4/garth/resources/__init__.py
--rw-r--r--   0        0        0     2698 2023-07-26 14:56:27.975003 garth-0.2.4/garth/resources/stress.py
--rw-r--r--   0        0        0     3552 2023-07-23 16:09:16.949253 garth-0.2.4/garth/sso.py
--rw-r--r--   0        0        0      573 2023-07-26 14:44:24.360714 garth-0.2.4/garth/utils.py
--rw-r--r--   0        0        0       22 2023-07-26 14:57:08.603253 garth-0.2.4/garth/version.py
--rw-r--r--   0        0        0      854 2023-07-26 14:57:14.010285 garth-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.2.4/tests/cassettes/test_client_get.yaml
--rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.2.4/tests/cassettes/test_client_post.yaml
--rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.2.4/tests/cassettes/test_client_request.yaml
--rw-r--r--   0        0        0     2331 2023-07-23 16:06:33.706591 garth-0.2.4/tests/cassettes/test_connectapi.yaml
--rw-r--r--   0        0        0     4564 2023-07-23 16:06:33.706751 garth-0.2.4/tests/cassettes/test_connectapi_refresh.yaml
--rw-r--r--   0        0        0     3231 2023-07-23 13:06:17.267462 garth-0.2.4/tests/cassettes/test_exchange.yaml
--rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.2.4/tests/cassettes/test_get_username.yaml
--rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.2.4/tests/cassettes/test_login_email_password_fail.yaml
--rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.2.4/tests/cassettes/test_login_success.yaml
--rw-r--r--   0        0        0     2270 2023-07-23 13:09:36.525519 garth-0.2.4/tests/cassettes/test_refresh.yaml
--rw-r--r--   0        0        0     2963 2023-07-23 13:36:21.976543 garth-0.2.4/tests/cassettes/test_refresh_expired.yaml
--rw-r--r--   0        0        0     2940 2023-07-23 16:06:33.706957 garth-0.2.4/tests/conftest.py
--rw-r--r--   0        0        0     6252 2023-07-26 13:24:49.161636 garth-0.2.4/tests/resources/cassettes/test_daily.yaml
--rw-r--r--   0        0        0    10389 2023-07-26 13:24:49.161944 garth-0.2.4/tests/resources/cassettes/test_daily_pagination.yaml
--rw-r--r--   0        0        0     4717 2023-07-26 13:24:49.162252 garth-0.2.4/tests/resources/cassettes/test_weekly.yaml
--rw-r--r--   0        0        0     7522 2023-07-26 13:24:49.162569 garth-0.2.4/tests/resources/cassettes/test_weekly_pagination.yaml
--rw-r--r--   0        0        0     1172 2023-07-26 13:24:49.162843 garth-0.2.4/tests/resources/test_stress.py
--rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.2.4/tests/test_auth_token.py
--rw-r--r--   0        0        0     4314 2023-07-23 16:06:33.707155 garth-0.2.4/tests/test_http.py
--rw-r--r--   0        0        0     2570 2023-07-23 13:18:13.595293 garth-0.2.4/tests/test_sso.py
--rw-r--r--   0        0        0      562 2023-07-26 14:44:24.930577 garth-0.2.4/tests/test_utils.py
--rw-r--r--   0        0        0     4809 1970-01-01 00:00:00.000000 garth-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4529 2023-07-27 00:58:56.322378 garth-0.2.5/README.md
+-rw-r--r--   0        0        0      390 2023-07-26 18:12:31.231211 garth-0.2.5/garth/__init__.py
+-rw-r--r--   0        0        0      913 2023-07-23 13:39:36.444380 garth-0.2.5/garth/auth_token.py
+-rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.2.5/garth/exc.py
+-rw-r--r--   0        0        0     4852 2023-07-26 18:12:31.231364 garth-0.2.5/garth/http.py
+-rw-r--r--   0        0        0       89 2023-07-26 13:24:49.158749 garth-0.2.5/garth/resources/__init__.py
+-rw-r--r--   0        0        0     2719 2023-07-26 19:04:08.936987 garth-0.2.5/garth/resources/stress.py
+-rw-r--r--   0        0        0     3552 2023-07-23 16:09:16.949253 garth-0.2.5/garth/sso.py
+-rw-r--r--   0        0        0      573 2023-07-26 14:44:24.360714 garth-0.2.5/garth/utils.py
+-rw-r--r--   0        0        0       22 2023-07-27 00:58:56.334579 garth-0.2.5/garth/version.py
+-rw-r--r--   0        0        0      798 2023-07-27 00:59:14.459296 garth-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.2.5/tests/cassettes/test_client_get.yaml
+-rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.2.5/tests/cassettes/test_client_post.yaml
+-rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.2.5/tests/cassettes/test_client_request.yaml
+-rw-r--r--   0        0        0     2331 2023-07-23 16:06:33.706591 garth-0.2.5/tests/cassettes/test_connectapi.yaml
+-rw-r--r--   0        0        0     4564 2023-07-23 16:06:33.706751 garth-0.2.5/tests/cassettes/test_connectapi_refresh.yaml
+-rw-r--r--   0        0        0     3231 2023-07-23 13:06:17.267462 garth-0.2.5/tests/cassettes/test_exchange.yaml
+-rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.2.5/tests/cassettes/test_get_username.yaml
+-rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.2.5/tests/cassettes/test_login_email_password_fail.yaml
+-rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.2.5/tests/cassettes/test_login_success.yaml
+-rw-r--r--   0        0        0     2270 2023-07-23 13:09:36.525519 garth-0.2.5/tests/cassettes/test_refresh.yaml
+-rw-r--r--   0        0        0     2963 2023-07-23 13:36:21.976543 garth-0.2.5/tests/cassettes/test_refresh_expired.yaml
+-rw-r--r--   0        0        0     2930 2023-07-26 18:12:31.231737 garth-0.2.5/tests/conftest.py
+-rw-r--r--   0        0        0     6252 2023-07-26 13:24:49.161636 garth-0.2.5/tests/resources/cassettes/test_daily.yaml
+-rw-r--r--   0        0        0    10389 2023-07-26 13:24:49.161944 garth-0.2.5/tests/resources/cassettes/test_daily_pagination.yaml
+-rw-r--r--   0        0        0     4717 2023-07-26 13:24:49.162252 garth-0.2.5/tests/resources/cassettes/test_weekly.yaml
+-rw-r--r--   0        0        0     7522 2023-07-26 13:24:49.162569 garth-0.2.5/tests/resources/cassettes/test_weekly_pagination.yaml
+-rw-r--r--   0        0        0     1172 2023-07-26 13:24:49.162843 garth-0.2.5/tests/resources/test_stress.py
+-rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.2.5/tests/test_auth_token.py
+-rw-r--r--   0        0        0     4296 2023-07-26 18:12:31.231936 garth-0.2.5/tests/test_http.py
+-rw-r--r--   0        0        0     2570 2023-07-23 13:18:13.595293 garth-0.2.5/tests/test_sso.py
+-rw-r--r--   0        0        0      562 2023-07-26 14:44:24.930577 garth-0.2.5/tests/test_utils.py
+-rw-r--r--   0        0        0     4792 1970-01-01 00:00:00.000000 garth-0.2.5/PKG-INFO
```

### Comparing `garth-0.2.4/LICENSE` & `garth-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/README.md` & `garth-0.2.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ### Authentication
 
 The most important reasoning is to build a library with authentication that
 works on [Google Colab](https://colab.research.google.com/) and doesn't require
 tools like Cloudscraper. Garth, in comparison:
 
 1. Uses the same embedded SSO as the mobile app
-1. Only requires `requests` and `pydantic` as a dependencies
+1. Only requires `requests` and `pydantic` as dependencies
 1. Supports MFA
 1. Supports saving and resuming sessions to avoid the need to log in each time
 you run a script, which is particularly useful if you have MFA enabled
 1. Works on Google Colab
 
 ### Python 3.10+
```

### Comparing `garth-0.2.4/garth/auth_token.py` & `garth-0.2.5/garth/auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/garth/http.py` & `garth-0.2.5/garth/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,22 +129,22 @@
 
     def login(self, *args):
         self.auth_token = AuthToken.login(*args, client=self)
 
     def connectapi(self, path: str, **kwargs):
         return self.get("connect", path, api=True, **kwargs).json()
 
-    def save_session(self, dir_path: str):
+    def dump(self, dir_path: str):
         dir_path = os.path.expanduser(dir_path)
         with open(os.path.join(dir_path, "cookies.pickle"), "wb") as f:
             pickle.dump(self.sess.cookies, f)
         with open(os.path.join(dir_path, "auth_token.json"), "w") as f:
             json.dump(asdict(self.auth_token) if self.auth_token else {}, f)
 
-    def resume_session(self, dir_path: str):
+    def load(self, dir_path: str):
         dir_path = os.path.expanduser(dir_path)
         with open(os.path.join(dir_path, "cookies.pickle"), "rb") as f:
             cookies = pickle.load(f)
         with open(os.path.join(dir_path, "auth_token.json")) as f:
             auth_token = AuthToken(**json.load(f))
         self.configure(auth_token=auth_token, cookies=cookies)
```

### Comparing `garth-0.2.4/garth/resources/stress.py` & `garth-0.2.5/garth/resources/stress.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 BASE_PATH = "/usersummary-service/stats/stress"
 
 
 @dataclass(frozen=True)
 class DailyStress:
     calendar_date: date
     overall_stress_level: int
-    rest_stress_duration: int
-    low_stress_duration: int
-    medium_stress_duration: int
+    rest_stress_duration: int | None
+    low_stress_duration: int | None
+    medium_stress_duration: int | None
     high_stress_duration: int | None
 
     _path: ClassVar[str] = f"{BASE_PATH}/daily"
     _page_size: ClassVar[int] = 28
 
     @classmethod
     def get(
```

### Comparing `garth-0.2.4/garth/sso.py` & `garth-0.2.5/garth/sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/garth/utils.py` & `garth-0.2.5/garth/utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/cassettes/test_client_get.yaml` & `garth-0.2.5/tests/cassettes/test_client_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/cassettes/test_client_post.yaml` & `garth-0.2.5/tests/cassettes/test_client_post.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/cassettes/test_client_request.yaml` & `garth-0.2.5/tests/cassettes/test_client_request.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/cassettes/test_connectapi.yaml` & `garth-0.2.5/tests/cassettes/test_connectapi.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/cassettes/test_connectapi_refresh.yaml` & `garth-0.2.5/tests/cassettes/test_connectapi_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/cassettes/test_exchange.yaml` & `garth-0.2.5/tests/cassettes/test_exchange.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/cassettes/test_get_username.yaml` & `garth-0.2.5/tests/cassettes/test_get_username.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/cassettes/test_login_email_password_fail.yaml` & `garth-0.2.5/tests/cassettes/test_login_email_password_fail.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/cassettes/test_login_success.yaml` & `garth-0.2.5/tests/cassettes/test_login_success.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/cassettes/test_refresh.yaml` & `garth-0.2.5/tests/cassettes/test_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/cassettes/test_refresh_expired.yaml` & `garth-0.2.5/tests/cassettes/test_refresh_expired.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/conftest.py` & `garth-0.2.5/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     return token
 
 
 @pytest.fixture
 def authed_client(auth_token: AuthToken) -> Client:
     client = Client()
     try:
-        client.resume_session(os.environ["GARTH_SESSION"])
+        client.load(os.environ["GARTH_SESSION"])
     except KeyError:
         client.auth_token = auth_token
     return client
 
 
 def sanitize_cookie(cookie_value) -> str:
     return re.sub(r"=[^;]*", "=SANITIZED", cookie_value)
```

### Comparing `garth-0.2.4/tests/resources/cassettes/test_daily.yaml` & `garth-0.2.5/tests/resources/cassettes/test_daily.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/resources/cassettes/test_daily_pagination.yaml` & `garth-0.2.5/tests/resources/cassettes/test_daily_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/resources/cassettes/test_weekly.yaml` & `garth-0.2.5/tests/resources/cassettes/test_weekly.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/resources/cassettes/test_weekly_pagination.yaml` & `garth-0.2.5/tests/resources/cassettes/test_weekly_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/resources/test_stress.py` & `garth-0.2.5/tests/resources/test_stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/test_auth_token.py` & `garth-0.2.5/tests/test_auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/test_http.py` & `garth-0.2.5/tests/test_http.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,18 +105,18 @@
     assert not authed_client._username
     assert authed_client.username
     assert authed_client._username == authed_client.username
 
 
 def test_save_and_resume_session(authed_client: Client):
     with tempfile.TemporaryDirectory() as tempdir:
-        authed_client.save_session(tempdir)
+        authed_client.dump(tempdir)
 
         new_client = Client()
-        new_client.resume_session(tempdir)
+        new_client.load(tempdir)
 
         assert new_client.sess.cookies == authed_client.sess.cookies
         assert new_client.auth_token == authed_client.auth_token
 
 
 @pytest.mark.vcr
 def test_connectapi(authed_client: Client):
```

### Comparing `garth-0.2.4/tests/test_sso.py` & `garth-0.2.5/tests/test_sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/tests/test_utils.py` & `garth-0.2.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.4/PKG-INFO` & `garth-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: garth
-Version: 0.2.4
+Version: 0.2.5
 Summary: Garmin SSO auth + Connect client
 Author-Email: Matin Tamizi <mtamizi@duck.com>
 License: MIT
 Requires-Python: >=3.10
-Requires-Dist: requests>=2.27.0
-Requires-Dist: pydantic>=2.1.1
+Requires-Dist: requests
+Requires-Dist: pydantic
 Description-Content-Type: text/markdown
 
 # Garth
 
 [![CI](https://github.com/matin/garth/workflows/CI/badge.svg?event=push)](https://github.com/matin/garth/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
 [![codecov](https://codecov.io/gh/matin/garth/branch/main/graph/badge.svg?token=0EFFYJNFIL)](https://codecov.io/gh/matin/garth)
 
@@ -33,15 +33,15 @@
 ### Authentication
 
 The most important reasoning is to build a library with authentication that
 works on [Google Colab](https://colab.research.google.com/) and doesn't require
 tools like Cloudscraper. Garth, in comparison:
 
 1. Uses the same embedded SSO as the mobile app
-1. Only requires `requests` and `pydantic` as a dependencies
+1. Only requires `requests` and `pydantic` as dependencies
 1. Supports MFA
 1. Supports saving and resuming sessions to avoid the need to log in each time
 you run a script, which is particularly useful if you have MFA enabled
 1. Works on Google Colab
 
 ### Python 3.10+
```

