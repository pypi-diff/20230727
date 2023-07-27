# Comparing `tmp/omniunibot-0.0.6.tar.gz` & `tmp/omniunibot-0.0.7.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniunibot-0.0.6.tar", last modified: Mon May 29 12:13:32 2023, max compression
+gzip compressed data, was "omniunibot-0.0.7.post1.tar", last modified: Thu Jul 27 04:22:23 2023, max compression
```

## Comparing `omniunibot-0.0.6.tar` & `omniunibot-0.0.7.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:13:32.832872 omniunibot-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-29 12:13:15.000000 omniunibot-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-29 12:13:32.832872 omniunibot-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-05-29 12:13:15.000000 omniunibot-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:13:32.832872 omniunibot-0.0.6/omniunibot/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/server.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:13:32.832872 omniunibot-0.0.6/omniunibot/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/wrapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/wrapper/dingtalk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/wrapper/feishu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/wrapper/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/wrapper/wecom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:13:32.832872 omniunibot-0.0.6/omniunibot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-29 12:13:32.000000 omniunibot-0.0.6/omniunibot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-29 12:13:32.000000 omniunibot-0.0.6/omniunibot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 12:13:32.000000 omniunibot-0.0.6/omniunibot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 12:13:32.000000 omniunibot-0.0.6/omniunibot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-29 12:13:32.000000 omniunibot-0.0.6/omniunibot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 12:13:32.000000 omniunibot-0.0.6/omniunibot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 12:13:32.832872 omniunibot-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-29 12:13:15.000000 omniunibot-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 04:22:23.285489 omniunibot-0.0.7.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-27 04:22:14.000000 omniunibot-0.0.7.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-27 04:22:23.285489 omniunibot-0.0.7.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-27 04:22:14.000000 omniunibot-0.0.7.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 04:22:23.285489 omniunibot-0.0.7.post1/omniunibot/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-27 04:22:14.000000 omniunibot-0.0.7.post1/omniunibot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-27 04:22:14.000000 omniunibot-0.0.7.post1/omniunibot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 04:22:14.000000 omniunibot-0.0.7.post1/omniunibot/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-27 04:22:14.000000 omniunibot-0.0.7.post1/omniunibot/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-07-27 04:22:14.000000 omniunibot-0.0.7.post1/omniunibot/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 04:22:14.000000 omniunibot-0.0.7.post1/omniunibot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 04:22:23.285489 omniunibot-0.0.7.post1/omniunibot/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 04:22:14.000000 omniunibot-0.0.7.post1/omniunibot/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-27 04:22:14.000000 omniunibot-0.0.7.post1/omniunibot/wrapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-27 04:22:14.000000 omniunibot-0.0.7.post1/omniunibot/wrapper/dingtalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-27 04:22:14.000000 omniunibot-0.0.7.post1/omniunibot/wrapper/feishu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-27 04:22:14.000000 omniunibot-0.0.7.post1/omniunibot/wrapper/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-27 04:22:14.000000 omniunibot-0.0.7.post1/omniunibot/wrapper/wecom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 04:22:23.285489 omniunibot-0.0.7.post1/omniunibot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-27 04:22:23.000000 omniunibot-0.0.7.post1/omniunibot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-27 04:22:23.000000 omniunibot-0.0.7.post1/omniunibot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 04:22:23.000000 omniunibot-0.0.7.post1/omniunibot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 04:22:23.000000 omniunibot-0.0.7.post1/omniunibot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-27 04:22:23.000000 omniunibot-0.0.7.post1/omniunibot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 04:22:23.000000 omniunibot-0.0.7.post1/omniunibot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 04:22:23.285489 omniunibot-0.0.7.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-27 04:22:14.000000 omniunibot-0.0.7.post1/setup.py
```

### Comparing `omniunibot-0.0.6/LICENSE` & `omniunibot-0.0.7.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.6/PKG-INFO` & `omniunibot-0.0.7.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniunibot
-Version: 0.0.6
+Version: 0.0.7.post1
 Summary: A universal multiplatform message bot
 Home-page: https://github.com/yttty/omniunibot
 Author: yttty
 Author-email: yttty@noreply.com
 License: MIT
 Keywords: bots
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `omniunibot-0.0.6/README.md` & `omniunibot-0.0.7.post1/README.md`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.6/omniunibot/__main__.py` & `omniunibot-0.0.7.post1/omniunibot/__main__.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.6/omniunibot/client.py` & `omniunibot-0.0.7.post1/omniunibot/client.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.6/omniunibot/server.py` & `omniunibot-0.0.7.post1/omniunibot/server.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.6/omniunibot/wrapper/base.py` & `omniunibot-0.0.7.post1/omniunibot/wrapper/base.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.6/omniunibot/wrapper/dingtalk.py` & `omniunibot-0.0.7.post1/omniunibot/wrapper/dingtalk.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.6/omniunibot/wrapper/feishu.py` & `omniunibot-0.0.7.post1/omniunibot/wrapper/feishu.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.6/omniunibot/wrapper/slack.py` & `omniunibot-0.0.7.post1/omniunibot/wrapper/slack.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.6/omniunibot/wrapper/wecom.py` & `omniunibot-0.0.7.post1/omniunibot/wrapper/wecom.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.6/omniunibot.egg-info/PKG-INFO` & `omniunibot-0.0.7.post1/omniunibot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniunibot
-Version: 0.0.6
+Version: 0.0.7.post1
 Summary: A universal multiplatform message bot
 Home-page: https://github.com/yttty/omniunibot
 Author: yttty
 Author-email: yttty@noreply.com
 License: MIT
 Keywords: bots
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `omniunibot-0.0.6/omniunibot.egg-info/SOURCES.txt` & `omniunibot-0.0.7.post1/omniunibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.6/setup.py` & `omniunibot-0.0.7.post1/setup.py`

 * *Files identical despite different names*

