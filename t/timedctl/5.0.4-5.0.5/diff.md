# Comparing `tmp/timedctl-5.0.4.tar.gz` & `tmp/timedctl-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timedctl-5.0.4.tar", max compression
+gzip compressed data, was "timedctl-5.0.5.tar", max compression
```

## Comparing `timedctl-5.0.4.tar` & `timedctl-5.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34454 2023-07-26 22:21:58.705275 timedctl-5.0.4/LICENSE
--rw-r--r--   0        0        0      774 2023-07-26 22:21:58.705275 timedctl-5.0.4/README.md
--rw-r--r--   0        0        0      849 2023-07-26 22:22:20.565919 timedctl-5.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 22:21:58.705275 timedctl-5.0.4/timedctl/__init__.py
--rw-r--r--   0        0        0     1831 2023-07-26 22:21:58.705275 timedctl-5.0.4/timedctl/helpers.py
--rwxr-xr-x   0        0        0    15810 2023-07-26 22:21:58.705275 timedctl-5.0.4/timedctl/timedctl.py
--rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 timedctl-5.0.4/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-27 17:46:25.159686 timedctl-5.0.5/LICENSE
+-rw-r--r--   0        0        0      774 2023-07-27 17:46:25.159686 timedctl-5.0.5/README.md
+-rw-r--r--   0        0        0      858 2023-07-27 17:46:59.416067 timedctl-5.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 17:46:25.159686 timedctl-5.0.5/timedctl/__init__.py
+-rw-r--r--   0        0        0     1831 2023-07-27 17:46:25.159686 timedctl-5.0.5/timedctl/helpers.py
+-rwxr-xr-x   0        0        0    17124 2023-07-27 17:46:25.159686 timedctl-5.0.5/timedctl/timedctl.py
+-rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 timedctl-5.0.5/PKG-INFO
```

### Comparing `timedctl-5.0.4/LICENSE` & `timedctl-5.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.4/README.md` & `timedctl-5.0.5/README.md`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.4/pyproject.toml` & `timedctl-5.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "timedctl"
-version = "5.0.4"
+version = "5.0.5"
 description = "CLI for timed"
 authors = ["Arthur Deierlein <arthur.deierlein@adfinis.com>", "Gian Klug <gian.klug@adfinis.com>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.3"
 pyfzf = "^0.3.1"
 rich = "^13.4.2"
 terminaltables = "^3.1.10"
-tomlkit = "^0.11.8"
+tomlkit = ">=0.11.8,<0.13.0"
 click-aliases = "^1.0.1"
 libtimed = "^0.4.4"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.2"
```

### Comparing `timedctl-5.0.4/timedctl/helpers.py` & `timedctl-5.0.5/timedctl/helpers.py`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.4/timedctl/timedctl.py` & `timedctl-5.0.5/timedctl/timedctl.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,16 +67,14 @@
     sso_realm = config.get("sso_realm")
     auth_path = "timedctl/auth"
     oidc_client = OIDCClient(client_id, sso_url, sso_realm, auth_path)
     token = oidc_client.authorize()
     return TimedAPIClient(token, url, api_namespace)
 
 
-
-
 def select_report(date):
     """FZF prompt to select a report."""
     reports = timed.reports.get(
         filters={"date": date}, include="task,task.project,task.project.customer"
     )
     report_view = []
     for report in reports:
@@ -465,38 +463,65 @@
         error_handler("ERR_NO_CURRENT_ACTIVITY")
 
 
 @activity.command(aliases=["gts", "ts"])
 def generate_timesheet():
     """Generate the timesheet of the current activities."""
     activities = timed.activities.get()
+    reports = timed.reports.get()
     if activities:
         for activity_obj in activities:
             attr = activity_obj["attributes"]
             if not attr["transferred"]:
                 # stop running activities
                 if not attr["to-time"]:
                     attr["to-time"] = datetime.datetime.now()
                 # calculate duration
                 duration = attr["to-time"] - attr["from-time"]
                 # get task
                 task = activity_obj["relationships"]["task"]["data"]["id"]
-                # create report
-                timed.reports.post(
-                    {
-                        "duration": duration,
-                        "comment": attr["comment"],
-                    },
-                    {"task": task},
-                )
+                # check if there is a report with the same comment that already exists
+                report = [
+                    x
+                    for x in reports
+                    if x["attributes"]["comment"] == attr["comment"]
+                    and x["relationships"]["task"]["data"]["id"] == task
+                ]
+                # if report has been found
+                if len(report) > 0:
+                    report = report[0]
+                    # deserialize the timedelta
+                    hours, minutes, seconds = report["attributes"]["duration"].split(
+                        ":"
+                    )
+                    old_duration = datetime.timedelta(
+                        hours=int(hours), minutes=int(minutes), seconds=int(seconds)
+                    )
+                    # calculate the new duration
+                    report["attributes"]["duration"] = old_duration + duration
+                    # update report
+                    timed.reports.patch(
+                        report["id"],
+                        report["attributes"],
+                        {"task": task},
+                    )
+                else:
+                    # create report
+                    r = timed.reports.post(
+                        {
+                            "duration": duration,
+                            "comment": attr["comment"],
+                        },
+                        {"task": task},
+                    )
+                    # append the report to the known reports
+                    reports.append(r.json()["data"])
                 # update activity to be transferred
                 attr["transferred"] = True
-                timed.activities.patch(
-                    activity_obj["id"], attr, {"task": task}
-                )
+                timed.activities.patch(activity_obj["id"], attr, {"task": task})
         msg("Timesheet generated successfully.")
     else:
         error_handler("ERR_NO_ACTIVITIES")
 
 
 if __name__ == "__main__":
     load_config()
```

### Comparing `timedctl-5.0.4/PKG-INFO` & `timedctl-5.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timedctl
-Version: 5.0.4
+Version: 5.0.5
 Summary: CLI for timed
 License: AGPL-3.0-only
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-aliases (>=1.0.1,<2.0.0)
 Requires-Dist: libtimed (>=0.4.4,<0.5.0)
 Requires-Dist: pyfzf (>=0.3.1,<0.4.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: terminaltables (>=3.1.10,<4.0.0)
-Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
+Requires-Dist: tomlkit (>=0.11.8,<0.13.0)
 Description-Content-Type: text/markdown
 
 # timedctl
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 
 
 Click TUI for [Timed](https://github.com/adfinis/timed-frontend) using [libtimed](https://github.com/adfinis/libtimed).
```

