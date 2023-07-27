# Comparing `tmp/garth-0.2.5.tar.gz` & `tmp/garth-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.2.5.tar", last modified: Thu Jul 27 00:59:14 2023, max compression
+gzip compressed data, was "garth-0.2.6.tar", last modified: Thu Jul 27 06:56:09 2023, max compression
```

## Comparing `garth-0.2.5.tar` & `garth-0.2.6.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.2.5/LICENSE
--rw-r--r--   0        0        0     4529 2023-07-27 00:58:56.322378 garth-0.2.5/README.md
--rw-r--r--   0        0        0      390 2023-07-26 18:12:31.231211 garth-0.2.5/garth/__init__.py
--rw-r--r--   0        0        0      913 2023-07-23 13:39:36.444380 garth-0.2.5/garth/auth_token.py
--rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.2.5/garth/exc.py
--rw-r--r--   0        0        0     4852 2023-07-26 18:12:31.231364 garth-0.2.5/garth/http.py
--rw-r--r--   0        0        0       89 2023-07-26 13:24:49.158749 garth-0.2.5/garth/resources/__init__.py
--rw-r--r--   0        0        0     2719 2023-07-26 19:04:08.936987 garth-0.2.5/garth/resources/stress.py
--rw-r--r--   0        0        0     3552 2023-07-23 16:09:16.949253 garth-0.2.5/garth/sso.py
--rw-r--r--   0        0        0      573 2023-07-26 14:44:24.360714 garth-0.2.5/garth/utils.py
--rw-r--r--   0        0        0       22 2023-07-27 00:58:56.334579 garth-0.2.5/garth/version.py
--rw-r--r--   0        0        0      798 2023-07-27 00:59:14.459296 garth-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.2.5/tests/cassettes/test_client_get.yaml
--rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.2.5/tests/cassettes/test_client_post.yaml
--rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.2.5/tests/cassettes/test_client_request.yaml
--rw-r--r--   0        0        0     2331 2023-07-23 16:06:33.706591 garth-0.2.5/tests/cassettes/test_connectapi.yaml
--rw-r--r--   0        0        0     4564 2023-07-23 16:06:33.706751 garth-0.2.5/tests/cassettes/test_connectapi_refresh.yaml
--rw-r--r--   0        0        0     3231 2023-07-23 13:06:17.267462 garth-0.2.5/tests/cassettes/test_exchange.yaml
--rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.2.5/tests/cassettes/test_get_username.yaml
--rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.2.5/tests/cassettes/test_login_email_password_fail.yaml
--rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.2.5/tests/cassettes/test_login_success.yaml
--rw-r--r--   0        0        0     2270 2023-07-23 13:09:36.525519 garth-0.2.5/tests/cassettes/test_refresh.yaml
--rw-r--r--   0        0        0     2963 2023-07-23 13:36:21.976543 garth-0.2.5/tests/cassettes/test_refresh_expired.yaml
--rw-r--r--   0        0        0     2930 2023-07-26 18:12:31.231737 garth-0.2.5/tests/conftest.py
--rw-r--r--   0        0        0     6252 2023-07-26 13:24:49.161636 garth-0.2.5/tests/resources/cassettes/test_daily.yaml
--rw-r--r--   0        0        0    10389 2023-07-26 13:24:49.161944 garth-0.2.5/tests/resources/cassettes/test_daily_pagination.yaml
--rw-r--r--   0        0        0     4717 2023-07-26 13:24:49.162252 garth-0.2.5/tests/resources/cassettes/test_weekly.yaml
--rw-r--r--   0        0        0     7522 2023-07-26 13:24:49.162569 garth-0.2.5/tests/resources/cassettes/test_weekly_pagination.yaml
--rw-r--r--   0        0        0     1172 2023-07-26 13:24:49.162843 garth-0.2.5/tests/resources/test_stress.py
--rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.2.5/tests/test_auth_token.py
--rw-r--r--   0        0        0     4296 2023-07-26 18:12:31.231936 garth-0.2.5/tests/test_http.py
--rw-r--r--   0        0        0     2570 2023-07-23 13:18:13.595293 garth-0.2.5/tests/test_sso.py
--rw-r--r--   0        0        0      562 2023-07-26 14:44:24.930577 garth-0.2.5/tests/test_utils.py
--rw-r--r--   0        0        0     4792 1970-01-01 00:00:00.000000 garth-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.2.6/LICENSE
+-rw-r--r--   0        0        0     4529 2023-07-27 00:58:56.322378 garth-0.2.6/README.md
+-rw-r--r--   0        0        0      390 2023-07-27 01:55:22.122866 garth-0.2.6/garth/__init__.py
+-rw-r--r--   0        0        0      913 2023-07-23 13:39:36.444380 garth-0.2.6/garth/auth_token.py
+-rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.2.6/garth/exc.py
+-rw-r--r--   0        0        0     4852 2023-07-26 18:12:31.231364 garth-0.2.6/garth/http.py
+-rw-r--r--   0        0        0       89 2023-07-27 01:55:22.123534 garth-0.2.6/garth/resources/__init__.py
+-rw-r--r--   0        0        0      666 2023-07-27 06:53:34.111275 garth-0.2.6/garth/resources/stress.py
+-rw-r--r--   0        0        0     3552 2023-07-23 16:09:16.949253 garth-0.2.6/garth/sso.py
+-rw-r--r--   0        0        0     1617 2023-07-27 06:43:30.470402 garth-0.2.6/garth/stats.py
+-rw-r--r--   0        0        0      542 2023-07-27 06:15:45.456562 garth-0.2.6/garth/utils.py
+-rw-r--r--   0        0        0       22 2023-07-27 06:56:03.735171 garth-0.2.6/garth/version.py
+-rw-r--r--   0        0        0      798 2023-07-27 06:56:09.125954 garth-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.2.6/tests/cassettes/test_client_get.yaml
+-rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.2.6/tests/cassettes/test_client_post.yaml
+-rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.2.6/tests/cassettes/test_client_request.yaml
+-rw-r--r--   0        0        0     2331 2023-07-23 16:06:33.706591 garth-0.2.6/tests/cassettes/test_connectapi.yaml
+-rw-r--r--   0        0        0     4564 2023-07-23 16:06:33.706751 garth-0.2.6/tests/cassettes/test_connectapi_refresh.yaml
+-rw-r--r--   0        0        0     3231 2023-07-23 13:06:17.267462 garth-0.2.6/tests/cassettes/test_exchange.yaml
+-rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.2.6/tests/cassettes/test_get_username.yaml
+-rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.2.6/tests/cassettes/test_login_email_password_fail.yaml
+-rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.2.6/tests/cassettes/test_login_success.yaml
+-rw-r--r--   0        0        0     2270 2023-07-23 13:09:36.525519 garth-0.2.6/tests/cassettes/test_refresh.yaml
+-rw-r--r--   0        0        0     2963 2023-07-23 13:36:21.976543 garth-0.2.6/tests/cassettes/test_refresh_expired.yaml
+-rw-r--r--   0        0        0     2930 2023-07-26 18:12:31.231737 garth-0.2.6/tests/conftest.py
+-rw-r--r--   0        0        0     6252 2023-07-26 13:24:49.161636 garth-0.2.6/tests/resources/cassettes/test_daily.yaml
+-rw-r--r--   0        0        0    44427 2023-07-27 06:53:40.937606 garth-0.2.6/tests/resources/cassettes/test_daily_pagination.yaml
+-rw-r--r--   0        0        0     4717 2023-07-26 13:24:49.162252 garth-0.2.6/tests/resources/cassettes/test_weekly.yaml
+-rw-r--r--   0        0        0     7522 2023-07-26 13:24:49.162569 garth-0.2.6/tests/resources/cassettes/test_weekly_pagination.yaml
+-rw-r--r--   0        0        0     1176 2023-07-27 06:52:51.197184 garth-0.2.6/tests/resources/test_stress.py
+-rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.2.6/tests/test_auth_token.py
+-rw-r--r--   0        0        0     4296 2023-07-26 18:12:31.231936 garth-0.2.6/tests/test_http.py
+-rw-r--r--   0        0        0     2570 2023-07-23 13:18:13.595293 garth-0.2.6/tests/test_sso.py
+-rw-r--r--   0        0        0      531 2023-07-27 06:36:04.840395 garth-0.2.6/tests/test_utils.py
+-rw-r--r--   0        0        0     4792 1970-01-01 00:00:00.000000 garth-0.2.6/PKG-INFO
```

### Comparing `garth-0.2.5/LICENSE` & `garth-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/README.md` & `garth-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/garth/auth_token.py` & `garth-0.2.6/garth/auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/garth/http.py` & `garth-0.2.6/garth/http.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/garth/resources/stress.py` & `garth-0.2.6/garth/stats.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,54 @@
 from datetime import date, timedelta
 from typing import ClassVar
 
 from pydantic.dataclasses import dataclass
 
-from .. import http
-from ..utils import camel_to_snake_dict, format_end_date
+from . import http
+from .utils import camel_to_snake_dict, format_end_date
 
 BASE_PATH = "/usersummary-service/stats/stress"
 
 
 @dataclass(frozen=True)
-class DailyStress:
+class Stats:
     calendar_date: date
-    overall_stress_level: int
-    rest_stress_duration: int | None
-    low_stress_duration: int | None
-    medium_stress_duration: int | None
-    high_stress_duration: int | None
 
-    _path: ClassVar[str] = f"{BASE_PATH}/daily"
-    _page_size: ClassVar[int] = 28
+    _path: ClassVar[str]
+    _page_size: ClassVar[int]
 
     @classmethod
-    def get(
+    def list(
         cls,
         end: date | str | None = None,
-        days: int = 1,
+        period: int = 1,
         *,
         client: http.Client | None = None,
-    ) -> list["DailyStress"]:
+    ) -> list["Stats"]:
         client = client or http.client
         end = format_end_date(end)
-        # paginate for more than 28 days
-        if days > cls._page_size:
-            page = cls.get(end, cls._page_size, client=client)
-            if page:
-                page = (
-                    cls.get(
-                        end - timedelta(days=cls._page_size),
-                        days - cls._page_size,
-                        client=client,
-                    )
-                    + page
-                )
-            return page
-        start = end - timedelta(days=days - 1)
-        path = f"{cls._path}/{start}/{end}"
-        daily_stress = client.connectapi(path)
-        daily_stress = [
-            camel_to_snake_dict(day | day.pop("values"))
-            for day in daily_stress
-        ]
-        return [cls(**day) for day in daily_stress]
-
-
-@dataclass(frozen=True)
-class WeeklyStress:
-    calendar_date: date
-    value: int
+        period_type = "days" if cls._path.endswith("daily") else "weeks"
 
-    _path: ClassVar[str] = f"{BASE_PATH}/weekly"
-    _page_size: ClassVar[int] = 52
-
-    @classmethod
-    def get(
-        cls,
-        end: date | str | None = None,
-        weeks: int = 1,
-        *,
-        client: http.Client | None = None,
-    ) -> list["WeeklyStress"]:
-        client = client or http.client
-        end = format_end_date(end)
-        # paginate for more than 52 weeks
-        if weeks > cls._page_size:
-            page = cls.get(end, cls._page_size, client=client)
-            if page:
-                page = (
-                    cls.get(
-                        end - timedelta(weeks=cls._page_size),
-                        weeks - cls._page_size,
-                        client=client,
-                    )
-                    + page
+        if period > cls._page_size:
+            page = cls.list(end, cls._page_size, client=client)
+            if not page:
+                return []
+            page = (
+                cls.list(
+                    end - timedelta(**{period_type: cls._page_size}),
+                    period - cls._page_size,
+                    client=client,
                 )
+                + page
+            )
             return page
-        path = f"{cls._path}/{end}/{weeks}"
-        weekly_stress = client.connectapi(path)
-        weekly_stress = [camel_to_snake_dict(week) for week in weekly_stress]
-        return [cls(**week) for week in weekly_stress]
+
+        if period_type == "weeks":
+            path = f"{cls._path}/{end}/{period}"
+        else:
+            start = end - timedelta(**{period_type: period - 1})
+            path = f"{cls._path}/{start}/{end}"
+        page_dirs = client.connectapi(path)
+        if page_dirs and "values" in page_dirs[0]:
+            page_dirs = [stat | stat.pop("values") for stat in page_dirs]
+        page_dirs = [camel_to_snake_dict(stat) for stat in page_dirs]
+        return [cls(**stat) for stat in page_dirs]
```

### Comparing `garth-0.2.5/garth/sso.py` & `garth-0.2.6/garth/sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/garth/utils.py` & `garth-0.2.6/garth/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from datetime import date, timedelta
+from datetime import date
 
 CAMEL_TO_SNAKE = re.compile(r"((?<=[a-z0-9])[A-Z]|(?!^)[A-Z](?=[a-z]))")
 
 
 def camel_to_snake(camel_str: str) -> str:
     snake_str = CAMEL_TO_SNAKE.sub(r"_\1", camel_str)
     return snake_str.lower()
@@ -11,11 +11,11 @@
 
 def camel_to_snake_dict(camel_dict: dict) -> dict:
     return {camel_to_snake(k): v for k, v in camel_dict.items()}
 
 
 def format_end_date(end: date | str | None) -> date:
     if end is None:
-        end = date.today() - timedelta(days=1)
+        end = date.today()
     elif isinstance(end, str):
         end = date.fromisoformat(end)
     return end
```

### Comparing `garth-0.2.5/pyproject.toml` & `garth-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 dependencies = [
     "requests",
     "pydantic",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
-version = "0.2.5"
+version = "0.2.6"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `garth-0.2.5/tests/cassettes/test_client_get.yaml` & `garth-0.2.6/tests/cassettes/test_client_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/cassettes/test_client_post.yaml` & `garth-0.2.6/tests/cassettes/test_client_post.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/cassettes/test_client_request.yaml` & `garth-0.2.6/tests/cassettes/test_client_request.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/cassettes/test_connectapi.yaml` & `garth-0.2.6/tests/cassettes/test_connectapi.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/cassettes/test_connectapi_refresh.yaml` & `garth-0.2.6/tests/cassettes/test_connectapi_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/cassettes/test_exchange.yaml` & `garth-0.2.6/tests/cassettes/test_exchange.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/cassettes/test_get_username.yaml` & `garth-0.2.6/tests/cassettes/test_get_username.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/cassettes/test_login_email_password_fail.yaml` & `garth-0.2.6/tests/cassettes/test_login_email_password_fail.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/cassettes/test_login_success.yaml` & `garth-0.2.6/tests/cassettes/test_login_success.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/cassettes/test_refresh.yaml` & `garth-0.2.6/tests/cassettes/test_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/cassettes/test_refresh_expired.yaml` & `garth-0.2.6/tests/cassettes/test_refresh_expired.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/conftest.py` & `garth-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/resources/cassettes/test_daily.yaml` & `garth-0.2.6/tests/resources/cassettes/test_daily.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/resources/cassettes/test_weekly.yaml` & `garth-0.2.6/tests/resources/cassettes/test_weekly.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/resources/cassettes/test_weekly_pagination.yaml` & `garth-0.2.6/tests/resources/cassettes/test_weekly_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/resources/test_stress.py` & `garth-0.2.6/tests/resources/test_stress.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 from garth.http import Client
 
 
 @pytest.mark.vcr
 def test_daily(authed_client: Client):
     end = date(2023, 7, 20)
     days = 20
-    daily_stress = DailyStress.get(end, days, client=authed_client)
+    daily_stress = DailyStress.list(end, days, client=authed_client)
     assert daily_stress[-1].calendar_date == end
     assert len(daily_stress) == days
 
 
 @pytest.mark.vcr
 def test_daily_pagination(authed_client: Client):
     end = date(2023, 7, 20)
-    days = 30
-    daily_stress = DailyStress.get(end, days, client=authed_client)
+    days = 60
+    daily_stress = DailyStress.list(end, days, client=authed_client)
     assert len(daily_stress) == days
 
 
 @pytest.mark.vcr
 def test_weekly(authed_client: Client):
     end = date(2023, 7, 20)
     weeks = 52
-    weekly_stress = WeeklyStress.get(end, weeks, client=authed_client)
+    weekly_stress = WeeklyStress.list(end, weeks, client=authed_client)
     assert len(weekly_stress) == weeks
     assert weekly_stress[-1].calendar_date == end - timedelta(days=6)
 
 
 @pytest.mark.vcr
 def test_weekly_pagination(authed_client: Client):
     end = date(2023, 7, 20)
     weeks = 60
-    weekly_stress = WeeklyStress.get(end, weeks, client=authed_client)
+    weekly_stress = WeeklyStress.list(end, weeks, client=authed_client)
     assert len(weekly_stress) == weeks
     assert weekly_stress[-1].calendar_date == end - timedelta(days=6)
```

### Comparing `garth-0.2.5/tests/test_auth_token.py` & `garth-0.2.6/tests/test_auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/test_http.py` & `garth-0.2.6/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/test_sso.py` & `garth-0.2.6/tests/test_sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.5/tests/test_utils.py` & `garth-0.2.6/tests/test_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import date, timedelta
+from datetime import date
 
 from garth.utils import camel_to_snake, camel_to_snake_dict, format_end_date
 
 
 def test_camel_to_snake():
     assert camel_to_snake("hiThereHuman") == "hi_there_human"
 
@@ -11,9 +11,9 @@
     assert camel_to_snake_dict({"hiThereHuman": "hi"}) == {
         "hi_there_human": "hi"
     }
 
 
 def test_format_end_date():
     assert format_end_date("2021-01-01") == date(2021, 1, 1)
-    assert format_end_date(None) == date.today() - timedelta(days=1)
+    assert format_end_date(None) == date.today()
     assert format_end_date(date(2021, 1, 1)) == date(2021, 1, 1)
```

### Comparing `garth-0.2.5/PKG-INFO` & `garth-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garth
-Version: 0.2.5
+Version: 0.2.6
 Summary: Garmin SSO auth + Connect client
 Author-Email: Matin Tamizi <mtamizi@duck.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: requests
 Requires-Dist: pydantic
 Description-Content-Type: text/markdown
```

