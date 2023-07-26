# Comparing `tmp/timedctl-5.0.3.tar.gz` & `tmp/timedctl-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timedctl-5.0.3.tar", max compression
+gzip compressed data, was "timedctl-5.0.4.tar", max compression
```

## Comparing `timedctl-5.0.3.tar` & `timedctl-5.0.4.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    34454 2023-07-25 08:57:31.776332 timedctl-5.0.3/LICENSE
--rw-r--r--   0        0        0      774 2023-07-25 08:57:31.776332 timedctl-5.0.3/README.md
--rw-r--r--   0        0        0      849 2023-07-25 08:57:52.532551 timedctl-5.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-25 08:57:31.780332 timedctl-5.0.3/timedctl/__init__.py
--rwxr-xr-x   0        0        0    17405 2023-07-25 08:57:31.780332 timedctl-5.0.3/timedctl/timedctl.py
--rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 timedctl-5.0.3/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-26 22:21:58.705275 timedctl-5.0.4/LICENSE
+-rw-r--r--   0        0        0      774 2023-07-26 22:21:58.705275 timedctl-5.0.4/README.md
+-rw-r--r--   0        0        0      849 2023-07-26 22:22:20.565919 timedctl-5.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 22:21:58.705275 timedctl-5.0.4/timedctl/__init__.py
+-rw-r--r--   0        0        0     1831 2023-07-26 22:21:58.705275 timedctl-5.0.4/timedctl/helpers.py
+-rwxr-xr-x   0        0        0    15810 2023-07-26 22:21:58.705275 timedctl-5.0.4/timedctl/timedctl.py
+-rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 timedctl-5.0.4/PKG-INFO
```

### Comparing `timedctl-5.0.3/LICENSE` & `timedctl-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.3/README.md` & `timedctl-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.3/pyproject.toml` & `timedctl-5.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "timedctl"
-version = "5.0.3"
+version = "5.0.4"
 description = "CLI for timed"
 authors = ["Arthur Deierlein <arthur.deierlein@adfinis.com>", "Gian Klug <gian.klug@adfinis.com>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.3"
 pyfzf = "^0.3.1"
 rich = "^13.4.2"
-libtimed = "^0.4.3"
 terminaltables = "^3.1.10"
 tomlkit = "^0.11.8"
 click-aliases = "^1.0.1"
+libtimed = "^0.4.4"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.2"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
```

### Comparing `timedctl-5.0.3/timedctl/timedctl.py` & `timedctl-5.0.4/timedctl/timedctl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 """CLI application for libtimed."""
 
 import datetime
 import os
 import re
-import sys
 
 import click
 import pyfzf
-import rich
 import terminaltables
 import tomllib
 from click_aliases import ClickAliasedGroup
 from libtimed import TimedAPIClient
 from libtimed.oidc import OIDCClient
 from tomlkit import dump
 
+from timedctl.helpers import msg, error_handler, fzf_wrapper, time_picker, time_sum
+
 
 def load_config():
     """Load the timedctl config."""
     cfg = {
         "username": "test",
         "timed_url": "https://timed.example.com",
         "sso_url": "https://sso.example.com",
@@ -67,71 +67,14 @@
     sso_realm = config.get("sso_realm")
     auth_path = "timedctl/auth"
     oidc_client = OIDCClient(client_id, sso_url, sso_realm, auth_path)
     token = oidc_client.authorize()
     return TimedAPIClient(token, url, api_namespace)
 
 
-def msg(message, nonl=False):
-    """Print a message in bold green."""
-    rich.print(f"[bold green]{message}[/bold green]", end="" if nonl else "\n")
-
-
-def error_handler(error):
-    """Handle errors."""
-    rich.print(f"[bold red]Error: {error}[/bold red]")
-    sys.exit(1)
-
-
-def fzf_wrapper(objects, title_key_array, prompt):
-    """Wrap pyfzf."""
-    # recursively resolve the title for each object
-    # . is separator for the keys.
-    titles = []
-    for obj in objects:
-        if isinstance(title_key_array[0], int):
-            title = obj[title_key_array[0]]
-        else:
-            title = obj
-            for key in title_key_array:
-                title = title[key]
-        titles.append(title)
-    # run the fzf prompt
-    result = [*pyfzf.FzfPrompt().prompt(titles, f"--prompt='{prompt}'"), None][0]
-    # turn the results back into objects
-    for obj in objects:
-        if isinstance(title_key_array[0], int):
-            title = obj[title_key_array[0]]
-        else:
-            title = obj
-            for key in title_key_array:
-                title = title[key]
-        if title == result:
-            return obj
-    error_handler("ERR_FZF_EXCEPTION")
-    return []
-
-
-def time_picker(default=None):
-    """Interactively pick a time using either arrow keys or typing."""
-    res = ""
-    while not re.match(r"^\d{1,2}:\d{2}:\d{2}$", res):
-        rich.print("[bold green]Duration[/bold green] (hh:mm:ss)", end="")
-        res = click.prompt("", default=default)
-    return res
-
-
-def time_sum(arr):
-    """Sum up an array of time strings."""
-    total = datetime.timedelta()
-    for line in arr[1:]:
-        val = line[-1]
-        total += val
-    # format as HH:MM:SS
-    return str(total)
 
 
 def select_report(date):
     """FZF prompt to select a report."""
     reports = timed.reports.get(
         filters={"date": date}, include="task,task.project,task.project.customer"
     )
@@ -524,30 +467,35 @@
 
 @activity.command(aliases=["gts", "ts"])
 def generate_timesheet():
     """Generate the timesheet of the current activities."""
     activities = timed.activities.get()
     if activities:
         for activity_obj in activities:
-            if not activity_obj["attributes"]["transferred"]:
-                if not activity_obj["attributes"]["to-time"]:
-                    activity_obj["attributes"]["to-time"] = datetime.datetime.now()
-                from_time = activity_obj["attributes"]["from-time"]
-                to_time = activity_obj["attributes"]["to-time"]
-                duration = to_time - from_time
+            attr = activity_obj["attributes"]
+            if not attr["transferred"]:
+                # stop running activities
+                if not attr["to-time"]:
+                    attr["to-time"] = datetime.datetime.now()
+                # calculate duration
+                duration = attr["to-time"] - attr["from-time"]
+                # get task
                 task = activity_obj["relationships"]["task"]["data"]["id"]
+                # create report
                 timed.reports.post(
                     {
                         "duration": duration,
-                        "comment": activity_obj["attributes"]["comment"],
+                        "comment": attr["comment"],
                     },
                     {"task": task},
                 )
+                # update activity to be transferred
+                attr["transferred"] = True
                 timed.activities.patch(
-                    activity_obj["id"], {"transferred": True}, {"task": task}
+                    activity_obj["id"], attr, {"task": task}
                 )
         msg("Timesheet generated successfully.")
     else:
         error_handler("ERR_NO_ACTIVITIES")
 
 
 if __name__ == "__main__":
```

### Comparing `timedctl-5.0.3/PKG-INFO` & `timedctl-5.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: timedctl
-Version: 5.0.3
+Version: 5.0.4
 Summary: CLI for timed
 License: AGPL-3.0-only
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-aliases (>=1.0.1,<2.0.0)
-Requires-Dist: libtimed (>=0.4.3,<0.5.0)
+Requires-Dist: libtimed (>=0.4.4,<0.5.0)
 Requires-Dist: pyfzf (>=0.3.1,<0.4.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: terminaltables (>=3.1.10,<4.0.0)
 Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
 Description-Content-Type: text/markdown
 
 # timedctl
```

