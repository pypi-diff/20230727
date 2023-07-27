# Comparing `tmp/slack-react-0.3.1.tar.gz` & `tmp/slack-react-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-react-0.3.1.tar", last modified: Thu Jul 27 07:45:48 2023, max compression
+gzip compressed data, was "slack-react-0.3.2.tar", last modified: Thu Jul 27 07:47:01 2023, max compression
```

## Comparing `slack-react-0.3.1.tar` & `slack-react-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:45:48.196898 slack-react-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:45:48.196898 slack-react-0.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-27 07:45:36.000000 slack-react-0.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:45:48.196898 slack-react-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-27 07:45:36.000000 slack-react-0.3.1/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-27 07:45:36.000000 slack-react-0.3.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-27 07:45:36.000000 slack-react-0.3.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 07:45:36.000000 slack-react-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-27 07:45:36.000000 slack-react-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-07-27 07:45:48.196898 slack-react-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-27 07:45:36.000000 slack-react-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-27 07:45:36.000000 slack-react-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 07:45:48.196898 slack-react-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:45:48.196898 slack-react-0.3.1/slack_react.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-07-27 07:45:48.000000 slack-react-0.3.1/slack_react.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-27 07:45:48.000000 slack-react-0.3.1/slack_react.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 07:45:48.000000 slack-react-0.3.1/slack_react.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 07:45:48.000000 slack-react-0.3.1/slack_react.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 07:45:48.000000 slack-react-0.3.1/slack_react.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 07:45:48.000000 slack-react-0.3.1/slack_react.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    11178 2023-07-27 07:45:36.000000 slack-react-0.3.1/slack_react.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:47:01.395688 slack-react-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:47:01.391687 slack-react-0.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-27 07:46:51.000000 slack-react-0.3.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:47:01.391687 slack-react-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-27 07:46:51.000000 slack-react-0.3.2/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-27 07:46:51.000000 slack-react-0.3.2/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-27 07:46:51.000000 slack-react-0.3.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 07:46:51.000000 slack-react-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-27 07:46:51.000000 slack-react-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-07-27 07:47:01.395688 slack-react-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-27 07:46:51.000000 slack-react-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-27 07:46:51.000000 slack-react-0.3.2/init.ipy
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-27 07:46:51.000000 slack-react-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 07:47:01.395688 slack-react-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:47:01.395688 slack-react-0.3.2/slack_react.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-07-27 07:47:01.000000 slack-react-0.3.2/slack_react.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-27 07:47:01.000000 slack-react-0.3.2/slack_react.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 07:47:01.000000 slack-react-0.3.2/slack_react.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 07:47:01.000000 slack-react-0.3.2/slack_react.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 07:47:01.000000 slack-react-0.3.2/slack_react.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 07:47:01.000000 slack-react-0.3.2/slack_react.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11102 2023-07-27 07:46:51.000000 slack-react-0.3.2/slack_react.py
```

### Comparing `slack-react-0.3.1/.github/workflows/pypi.yaml` & `slack-react-0.3.2/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `slack-react-0.3.1/.github/workflows/release.yaml` & `slack-react-0.3.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `slack-react-0.3.1/LICENSE` & `slack-react-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-react-0.3.1/PKG-INFO` & `slack-react-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-react
-Version: 0.3.1
+Version: 0.3.2
 Summary: Add reactions that spell out messages to Slack messages
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `slack-react-0.3.1/README.md` & `slack-react-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `slack-react-0.3.1/pyproject.toml` & `slack-react-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,14 @@
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "appdirs",
   "rich",
   "slack_sdk"
 ]
-version = "0.3.1"
+version = "0.3.2"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 slack-react = "slack_react:main"
```

### Comparing `slack-react-0.3.1/slack_react.egg-info/PKG-INFO` & `slack-react-0.3.2/slack_react.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-react
-Version: 0.3.1
+Version: 0.3.2
 Summary: Add reactions that spell out messages to Slack messages
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `slack-react-0.3.1/slack_react.py` & `slack-react-0.3.2/slack_react.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import re
 import shutil
 import sys
 from typing import Dict, List
 
 import slack_sdk
 from appdirs import user_cache_dir
-from rich import print
 from rich.logging import RichHandler
 
 APP_NAME = "slack-react"
 LOGGER = logging.getLogger(__name__)
 
 # mapping of alphabets to their corresponding emoji names
 EMOJI_MAPPING = {
@@ -265,15 +264,14 @@
 
 def get_channel_id(client, channel_name):
     # the channels are in the 'channels' field of the response
     channels = smart_cache(client)
 
     # iterate over the channels to find the one with the given name
     for channel in channels:
-        # print(channel["name"])
         if channel["name"] == channel_name:
             return channel["id"]
 
 
 def find_matching_message(client, channel_id, regex):
     # get the history of the channel
     response = client.conversations_history(channel=channel_id)
@@ -336,23 +334,23 @@
 
     # create a client instance
     client = slack_sdk.WebClient(token=args.token)
 
     channel_id = get_channel_id(client, args.channel)
 
     if not channel_id:
-        print(f"Channel '{args.channel}' not found", file=sys.stderr)
+        LOGGER.error(f"Channel '{args.channel}' not found")
         return 1
 
     response = client.conversations_history(channel=channel_id)
 
     if args.message:
         message = find_matching_message(client, channel_id, args.message)
         if not message:
-            print("Message not found", file=sys.stderr)
+            LOGGER.error("Message not found")
             return 1
         ts = message["ts"]
     else:
         # Default to last message
         ts = response.get("messages", [{"ts": None}])[0]["ts"]
 
     if not ts:
```

