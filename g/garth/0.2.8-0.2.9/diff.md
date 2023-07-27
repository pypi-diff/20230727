# Comparing `tmp/garth-0.2.8.tar.gz` & `tmp/garth-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.2.8.tar", last modified: Thu Jul 27 07:08:20 2023, max compression
+gzip compressed data, was "garth-0.2.9.tar", last modified: Thu Jul 27 13:32:20 2023, max compression
```

## Comparing `garth-0.2.8.tar` & `garth-0.2.9.tar`

### file list

```diff
@@ -1,36 +1,40 @@
--rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.2.8/LICENSE
--rw-r--r--   0        0        0     4529 2023-07-27 00:58:56.322378 garth-0.2.8/README.md
--rw-r--r--   0        0        0      390 2023-07-27 01:55:22.122866 garth-0.2.8/garth/__init__.py
--rw-r--r--   0        0        0      913 2023-07-23 13:39:36.444380 garth-0.2.8/garth/auth_token.py
--rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.2.8/garth/exc.py
--rw-r--r--   0        0        0     4852 2023-07-26 18:12:31.231364 garth-0.2.8/garth/http.py
--rw-r--r--   0        0        0        0 2023-07-27 07:00:55.127101 garth-0.2.8/garth/py.typed
--rw-r--r--   0        0        0       89 2023-07-27 01:55:22.123534 garth-0.2.8/garth/resources/__init__.py
--rw-r--r--   0        0        0      666 2023-07-27 06:53:34.111275 garth-0.2.8/garth/resources/stress.py
--rw-r--r--   0        0        0     3552 2023-07-23 16:09:16.949253 garth-0.2.8/garth/sso.py
--rw-r--r--   0        0        0     1617 2023-07-27 06:43:30.470402 garth-0.2.8/garth/stats.py
--rw-r--r--   0        0        0      542 2023-07-27 06:15:45.456562 garth-0.2.8/garth/utils.py
--rw-r--r--   0        0        0       22 2023-07-27 07:07:00.511661 garth-0.2.8/garth/version.py
--rw-r--r--   0        0        0     1069 2023-07-27 07:08:20.434488 garth-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.2.8/tests/cassettes/test_client_get.yaml
--rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.2.8/tests/cassettes/test_client_post.yaml
--rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.2.8/tests/cassettes/test_client_request.yaml
--rw-r--r--   0        0        0     2331 2023-07-23 16:06:33.706591 garth-0.2.8/tests/cassettes/test_connectapi.yaml
--rw-r--r--   0        0        0     4564 2023-07-23 16:06:33.706751 garth-0.2.8/tests/cassettes/test_connectapi_refresh.yaml
--rw-r--r--   0        0        0     3231 2023-07-23 13:06:17.267462 garth-0.2.8/tests/cassettes/test_exchange.yaml
--rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.2.8/tests/cassettes/test_get_username.yaml
--rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.2.8/tests/cassettes/test_login_email_password_fail.yaml
--rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.2.8/tests/cassettes/test_login_success.yaml
--rw-r--r--   0        0        0     2270 2023-07-23 13:09:36.525519 garth-0.2.8/tests/cassettes/test_refresh.yaml
--rw-r--r--   0        0        0     2963 2023-07-23 13:36:21.976543 garth-0.2.8/tests/cassettes/test_refresh_expired.yaml
--rw-r--r--   0        0        0     2930 2023-07-26 18:12:31.231737 garth-0.2.8/tests/conftest.py
--rw-r--r--   0        0        0     6252 2023-07-26 13:24:49.161636 garth-0.2.8/tests/resources/cassettes/test_daily.yaml
--rw-r--r--   0        0        0    44427 2023-07-27 06:53:40.937606 garth-0.2.8/tests/resources/cassettes/test_daily_pagination.yaml
--rw-r--r--   0        0        0     4717 2023-07-26 13:24:49.162252 garth-0.2.8/tests/resources/cassettes/test_weekly.yaml
--rw-r--r--   0        0        0     7522 2023-07-26 13:24:49.162569 garth-0.2.8/tests/resources/cassettes/test_weekly_pagination.yaml
--rw-r--r--   0        0        0     1176 2023-07-27 06:52:51.197184 garth-0.2.8/tests/resources/test_stress.py
--rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.2.8/tests/test_auth_token.py
--rw-r--r--   0        0        0     4296 2023-07-26 18:12:31.231936 garth-0.2.8/tests/test_http.py
--rw-r--r--   0        0        0     2570 2023-07-23 13:18:13.595293 garth-0.2.8/tests/test_sso.py
--rw-r--r--   0        0        0      531 2023-07-27 06:36:04.840395 garth-0.2.8/tests/test_utils.py
--rw-r--r--   0        0        0     4941 1970-01-01 00:00:00.000000 garth-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.2.9/LICENSE
+-rw-r--r--   0        0        0     4529 2023-07-27 00:58:56.322378 garth-0.2.9/README.md
+-rw-r--r--   0        0        0      420 2023-07-27 13:31:20.421115 garth-0.2.9/garth/__init__.py
+-rw-r--r--   0        0        0      913 2023-07-23 13:39:36.444380 garth-0.2.9/garth/auth_token.py
+-rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.2.9/garth/exc.py
+-rw-r--r--   0        0        0     4852 2023-07-26 18:12:31.231364 garth-0.2.9/garth/http.py
+-rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.2.9/garth/py.typed
+-rw-r--r--   0        0        0      133 2023-07-27 13:31:20.421414 garth-0.2.9/garth/resources/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-27 13:31:20.421527 garth-0.2.9/garth/resources/sleep.py
+-rw-r--r--   0        0        0      616 2023-07-27 13:31:20.421792 garth-0.2.9/garth/resources/stress.py
+-rw-r--r--   0        0        0     3552 2023-07-23 16:09:16.949253 garth-0.2.9/garth/sso.py
+-rw-r--r--   0        0        0     1610 2023-07-27 13:31:20.421985 garth-0.2.9/garth/stats.py
+-rw-r--r--   0        0        0      542 2023-07-27 06:15:45.456562 garth-0.2.9/garth/utils.py
+-rw-r--r--   0        0        0       22 2023-07-27 13:31:42.547838 garth-0.2.9/garth/version.py
+-rw-r--r--   0        0        0     1069 2023-07-27 13:32:20.431712 garth-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.2.9/tests/cassettes/test_client_get.yaml
+-rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.2.9/tests/cassettes/test_client_post.yaml
+-rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.2.9/tests/cassettes/test_client_request.yaml
+-rw-r--r--   0        0        0     2331 2023-07-23 16:06:33.706591 garth-0.2.9/tests/cassettes/test_connectapi.yaml
+-rw-r--r--   0        0        0     4564 2023-07-23 16:06:33.706751 garth-0.2.9/tests/cassettes/test_connectapi_refresh.yaml
+-rw-r--r--   0        0        0     3231 2023-07-23 13:06:17.267462 garth-0.2.9/tests/cassettes/test_exchange.yaml
+-rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.2.9/tests/cassettes/test_get_username.yaml
+-rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.2.9/tests/cassettes/test_login_email_password_fail.yaml
+-rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.2.9/tests/cassettes/test_login_success.yaml
+-rw-r--r--   0        0        0     2270 2023-07-23 13:09:36.525519 garth-0.2.9/tests/cassettes/test_refresh.yaml
+-rw-r--r--   0        0        0     2963 2023-07-23 13:36:21.976543 garth-0.2.9/tests/cassettes/test_refresh_expired.yaml
+-rw-r--r--   0        0        0     2930 2023-07-26 18:12:31.231737 garth-0.2.9/tests/conftest.py
+-rw-r--r--   0        0        0     3098 2023-07-27 13:31:20.422352 garth-0.2.9/tests/resources/cassettes/test_daily_sleep.yaml
+-rw-r--r--   0        0        0     6252 2023-07-27 13:31:20.422471 garth-0.2.9/tests/resources/cassettes/test_daily_stress.yaml
+-rw-r--r--   0        0        0    44427 2023-07-27 13:31:20.422659 garth-0.2.9/tests/resources/cassettes/test_daily_stress_pagination.yaml
+-rw-r--r--   0        0        0     4717 2023-07-27 13:31:20.422800 garth-0.2.9/tests/resources/cassettes/test_weekly_stress.yaml
+-rw-r--r--   0        0        0    16221 2023-07-27 13:31:20.422937 garth-0.2.9/tests/resources/cassettes/test_weekly_stress_beyond_data.yaml
+-rw-r--r--   0        0        0     7522 2023-07-27 13:31:20.423053 garth-0.2.9/tests/resources/cassettes/test_weekly_stress_pagination.yaml
+-rw-r--r--   0        0        0      358 2023-07-27 13:31:20.423425 garth-0.2.9/tests/resources/test_sleep.py
+-rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.2.9/tests/resources/test_stress.py
+-rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.2.9/tests/test_auth_token.py
+-rw-r--r--   0        0        0     4296 2023-07-26 18:12:31.231936 garth-0.2.9/tests/test_http.py
+-rw-r--r--   0        0        0     2570 2023-07-23 13:18:13.595293 garth-0.2.9/tests/test_sso.py
+-rw-r--r--   0        0        0      531 2023-07-27 13:16:10.645234 garth-0.2.9/tests/test_utils.py
+-rw-r--r--   0        0        0     4941 1970-01-01 00:00:00.000000 garth-0.2.9/PKG-INFO
```

### Comparing `garth-0.2.8/LICENSE` & `garth-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/README.md` & `garth-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/garth/auth_token.py` & `garth-0.2.9/garth/auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/garth/http.py` & `garth-0.2.9/garth/http.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/garth/resources/stress.py` & `garth-0.2.9/garth/resources/stress.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from datetime import date
 from typing import ClassVar
 
 from pydantic.dataclasses import dataclass
 
 from ..stats import Stats
 
 BASE_PATH = "/usersummary-service/stats/stress"
@@ -18,12 +17,11 @@
 
     _path: ClassVar[str] = f"{BASE_PATH}/daily"
     _page_size: ClassVar[int] = 28
 
 
 @dataclass(frozen=True)
 class WeeklyStress(Stats):
-    calendar_date: date
     value: int
 
     _path: ClassVar[str] = f"{BASE_PATH}/weekly"
     _page_size: ClassVar[int] = 52
```

### Comparing `garth-0.2.8/garth/sso.py` & `garth-0.2.9/garth/sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/garth/stats.py` & `garth-0.2.9/garth/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         end: date | str | None = None,
         period: int = 1,
         *,
         client: http.Client | None = None,
     ) -> list["Stats"]:
         client = client or http.client
         end = format_end_date(end)
-        period_type = "days" if cls._path.endswith("daily") else "weeks"
+        period_type = "days" if "daily" in cls._path else "weeks"
 
         if period > cls._page_size:
             page = cls.list(end, cls._page_size, client=client)
             if not page:
                 return []
             page = (
                 cls.list(
```

### Comparing `garth-0.2.8/garth/utils.py` & `garth-0.2.9/garth/utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/pyproject.toml` & `garth-0.2.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
 ]
-version = "0.2.8"
+version = "0.2.9"
 
 [project.license]
 text = "MIT"
 
 [project.packages]
 include = [
     { from = ".", include = "garth" },
```

### Comparing `garth-0.2.8/tests/cassettes/test_client_get.yaml` & `garth-0.2.9/tests/cassettes/test_client_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/cassettes/test_client_post.yaml` & `garth-0.2.9/tests/cassettes/test_client_post.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/cassettes/test_client_request.yaml` & `garth-0.2.9/tests/cassettes/test_client_request.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/cassettes/test_connectapi.yaml` & `garth-0.2.9/tests/cassettes/test_connectapi.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/cassettes/test_connectapi_refresh.yaml` & `garth-0.2.9/tests/cassettes/test_connectapi_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/cassettes/test_exchange.yaml` & `garth-0.2.9/tests/cassettes/test_exchange.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/cassettes/test_get_username.yaml` & `garth-0.2.9/tests/cassettes/test_get_username.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/cassettes/test_login_email_password_fail.yaml` & `garth-0.2.9/tests/cassettes/test_login_email_password_fail.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/cassettes/test_login_success.yaml` & `garth-0.2.9/tests/cassettes/test_login_success.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/cassettes/test_refresh.yaml` & `garth-0.2.9/tests/cassettes/test_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/cassettes/test_refresh_expired.yaml` & `garth-0.2.9/tests/cassettes/test_refresh_expired.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/conftest.py` & `garth-0.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/resources/cassettes/test_daily.yaml` & `garth-0.2.9/tests/resources/cassettes/test_daily_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/resources/cassettes/test_daily_pagination.yaml` & `garth-0.2.9/tests/resources/cassettes/test_daily_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/resources/cassettes/test_weekly.yaml` & `garth-0.2.9/tests/resources/cassettes/test_weekly_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/resources/cassettes/test_weekly_pagination.yaml` & `garth-0.2.9/tests/resources/cassettes/test_weekly_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/resources/test_stress.py` & `garth-0.2.9/tests/resources/test_stress.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,39 +3,47 @@
 import pytest
 
 from garth import DailyStress, WeeklyStress
 from garth.http import Client
 
 
 @pytest.mark.vcr
-def test_daily(authed_client: Client):
+def test_daily_stress(authed_client: Client):
     end = date(2023, 7, 20)
     days = 20
     daily_stress = DailyStress.list(end, days, client=authed_client)
     assert daily_stress[-1].calendar_date == end
     assert len(daily_stress) == days
 
 
 @pytest.mark.vcr
-def test_daily_pagination(authed_client: Client):
+def test_daily_stress_pagination(authed_client: Client):
     end = date(2023, 7, 20)
     days = 60
     daily_stress = DailyStress.list(end, days, client=authed_client)
     assert len(daily_stress) == days
 
 
 @pytest.mark.vcr
-def test_weekly(authed_client: Client):
+def test_weekly_stress(authed_client: Client):
     end = date(2023, 7, 20)
     weeks = 52
     weekly_stress = WeeklyStress.list(end, weeks, client=authed_client)
     assert len(weekly_stress) == weeks
     assert weekly_stress[-1].calendar_date == end - timedelta(days=6)
 
 
 @pytest.mark.vcr
-def test_weekly_pagination(authed_client: Client):
+def test_weekly_stress_pagination(authed_client: Client):
     end = date(2023, 7, 20)
     weeks = 60
     weekly_stress = WeeklyStress.list(end, weeks, client=authed_client)
     assert len(weekly_stress) == weeks
     assert weekly_stress[-1].calendar_date == end - timedelta(days=6)
+
+
+@pytest.mark.vcr
+def test_weekly_stress_beyond_data(authed_client: Client):
+    end = date(2023, 7, 20)
+    weeks = 1000
+    weekly_stress = WeeklyStress.list(end, weeks, client=authed_client)
+    assert len(weekly_stress) < weeks
```

### Comparing `garth-0.2.8/tests/test_auth_token.py` & `garth-0.2.9/tests/test_auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/test_http.py` & `garth-0.2.9/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/test_sso.py` & `garth-0.2.9/tests/test_sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/tests/test_utils.py` & `garth-0.2.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.8/PKG-INFO` & `garth-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garth
-Version: 0.2.8
+Version: 0.2.9
 Summary: Garmin SSO auth + Connect client
 Author-Email: Matin Tamizi <mtamizi@duck.com>
 License: MIT
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

