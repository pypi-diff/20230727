# Comparing `tmp/micrologai-1.3.2.tar.gz` & `tmp/micrologai-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micrologai-1.3.2.tar", last modified: Wed Jul 26 09:45:55 2023, max compression
+gzip compressed data, was "micrologai-1.3.3.tar", last modified: Thu Jul 27 20:14:28 2023, max compression
```

## Comparing `micrologai-1.3.2.tar` & `micrologai-1.3.3.tar`

### file list

```diff
@@ -1,117 +1,116 @@
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:55.364992 micrologai-1.3.2/
--rw-r--r--   0 laffra     (501) staff       (20)    30607 2023-07-05 22:06:54.000000 micrologai-1.3.2/LICENSE
--rw-r--r--   0 laffra     (501) staff       (20)      213 2023-07-19 13:43:23.000000 micrologai-1.3.2/MANIFEST.in
--rw-r--r--   0 laffra     (501) staff       (20)    45847 2023-07-26 09:45:55.367812 micrologai-1.3.2/PKG-INFO
--rw-r--r--   0 laffra     (501) staff       (20)    10207 2023-07-26 08:16:40.000000 micrologai-1.3.2/README.md
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:54.723538 micrologai-1.3.2/dashboard/
--rw-r--r--   0 laffra     (501) staff       (20)       75 2023-07-19 12:55:56.000000 micrologai-1.3.2/dashboard/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)    11820 2023-07-26 08:52:27.000000 micrologai-1.3.2/dashboard/canvas.py
--rw-r--r--   0 laffra     (501) staff       (20)      864 2023-07-25 13:00:57.000000 micrologai-1.3.2/dashboard/colors.py
--rw-r--r--   0 laffra     (501) staff       (20)      699 2023-07-19 12:55:56.000000 micrologai-1.3.2/dashboard/config.py
--rw-r--r--   0 laffra     (501) staff       (20)     8238 2023-07-19 15:09:18.000000 micrologai-1.3.2/dashboard/design.py
--rw-r--r--   0 laffra     (501) staff       (20)     1854 2023-07-19 12:55:56.000000 micrologai-1.3.2/dashboard/dialog.py
--rw-r--r--   0 laffra     (501) staff       (20)    26036 2023-07-25 12:33:02.000000 micrologai-1.3.2/dashboard/index.html
--rw-r--r--   0 laffra     (501) staff       (20)    12685 2023-07-26 09:27:45.000000 micrologai-1.3.2/dashboard/main.py
--rw-r--r--   0 laffra     (501) staff       (20)     1800 2023-07-19 12:55:56.000000 micrologai-1.3.2/dashboard/markdown.py
--rw-r--r--   0 laffra     (501) staff       (20)     1799 2023-07-25 13:09:32.000000 micrologai-1.3.2/dashboard/profiler.py
--rw-r--r--   0 laffra     (501) staff       (20)     2209 2023-07-19 12:55:56.000000 micrologai-1.3.2/dashboard/tips.py
--rw-r--r--   0 laffra     (501) staff       (20)     4245 2023-07-19 12:55:56.000000 micrologai-1.3.2/dashboard/treeview.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:54.753858 micrologai-1.3.2/dashboard/views/
--rw-r--r--   0 laffra     (501) staff       (20)     2165 2023-07-26 09:43:49.000000 micrologai-1.3.2/dashboard/views/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)    15240 2023-07-26 09:28:44.000000 micrologai-1.3.2/dashboard/views/call.py
--rw-r--r--   0 laffra     (501) staff       (20)     4826 2023-07-26 09:30:34.000000 micrologai-1.3.2/dashboard/views/marker.py
--rw-r--r--   0 laffra     (501) staff       (20)     4441 2023-07-26 09:31:18.000000 micrologai-1.3.2/dashboard/views/status.py
--rw-r--r--   0 laffra     (501) staff       (20)     2152 2023-07-19 12:55:56.000000 micrologai-1.3.2/dashboard/views/timeline.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:54.849261 micrologai-1.3.2/examples/
--rw-r--r--   0 laffra     (501) staff       (20)     1758 2023-06-08 14:12:55.000000 micrologai-1.3.2/examples/binaryTrees.py
--rw-r--r--   0 laffra     (501) staff       (20)    24814 2023-04-22 19:02:44.000000 micrologai-1.3.2/examples/books.json
--rw-r--r--   0 laffra     (501) staff       (20)     2213 2023-07-08 19:41:25.000000 micrologai-1.3.2/examples/bookstore.py
--rw-r--r--   0 laffra     (501) staff       (20)      998 2023-07-24 09:17:39.000000 micrologai-1.3.2/examples/dataframes.py
--rw-r--r--   0 laffra     (501) staff       (20)     1417 2023-07-24 08:53:57.000000 micrologai-1.3.2/examples/example.py
--rw-r--r--   0 laffra     (501) staff       (20)     1021 2023-07-12 07:42:28.000000 micrologai-1.3.2/examples/files.py
--rw-r--r--   0 laffra     (501) staff       (20)    13859 2023-07-25 12:36:42.000000 micrologai-1.3.2/examples/go.py
--rw-r--r--   0 laffra     (501) staff       (20)     1857 2023-06-15 09:37:09.000000 micrologai-1.3.2/examples/helloworld.py
--rw-r--r--   0 laffra     (501) staff       (20)     1127 2023-07-08 12:02:09.000000 micrologai-1.3.2/examples/memory.py
--rw-r--r--   0 laffra     (501) staff       (20)     1178 2023-07-24 10:45:34.000000 micrologai-1.3.2/examples/modules.py
--rwxr-xr-x   0 laffra     (501) staff       (20)      410 2023-07-24 11:06:15.000000 micrologai-1.3.2/examples/runall.sh
--rw-r--r--   0 laffra     (501) staff       (20)      913 2023-07-24 13:11:27.000000 micrologai-1.3.2/examples/startstop.py
--rw-r--r--   0 laffra     (501) staff       (20)      631 2023-06-08 16:27:45.000000 micrologai-1.3.2/examples/threads.py
--rw-r--r--   0 laffra     (501) staff       (20)    93813 2023-07-24 11:09:29.000000 micrologai-1.3.2/examples/treemap.ipynb
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:54.916238 micrologai-1.3.2/microlog/
--rw-r--r--   0 laffra     (501) staff       (20)      302 2023-07-26 09:45:34.000000 micrologai-1.3.2/microlog/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)     2798 2023-07-24 11:03:18.000000 micrologai-1.3.2/microlog/api.py
--rw-r--r--   0 laffra     (501) staff       (20)      769 2023-07-24 11:11:41.000000 micrologai-1.3.2/microlog/config.py
--rw-r--r--   0 laffra     (501) staff       (20)     3431 2023-07-19 12:56:01.000000 micrologai-1.3.2/microlog/explain.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:55.087185 micrologai-1.3.2/microlog/images/
--rw-r--r--   0 laffra     (501) staff       (20)   292932 2023-07-12 16:09:27.000000 micrologai-1.3.2/microlog/images/anomaly.png
--rw-rw-r--   0 laffra     (501) staff       (20)     7246 2023-04-21 09:21:45.000000 micrologai-1.3.2/microlog/images/apple-touch-icon.png
--rw-r--r--   0 laffra     (501) staff       (20)    91386 2023-07-12 16:45:27.000000 micrologai-1.3.2/microlog/images/chatgpt.png
--rw-r--r--   0 laffra     (501) staff       (20)   218816 2023-07-12 16:24:41.000000 micrologai-1.3.2/microlog/images/design-go.png
--rw-r--r--   0 laffra     (501) staff       (20)   222723 2023-04-10 13:38:11.000000 micrologai-1.3.2/microlog/images/dialog.png
--rw-r--r--   0 laffra     (501) staff       (20)   227072 2023-04-10 13:38:11.000000 micrologai-1.3.2/microlog/images/error-log.png
--rw-rw-r--   0 laffra     (501) staff       (20)      423 2023-04-21 09:21:34.000000 micrologai-1.3.2/microlog/images/favicon-16x16.png
--rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-21 09:21:34.000000 micrologai-1.3.2/microlog/images/favicon-32x32.png
--rw-r--r--   0 laffra     (501) staff       (20)   160359 2023-07-12 16:32:21.000000 micrologai-1.3.2/microlog/images/fd-leak.png
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:55.252718 micrologai-1.3.2/microlog/images/icons/
--rw-r--r--   0 laffra     (501) staff       (20)    14969 2023-04-25 09:23:09.000000 micrologai-1.3.2/microlog/images/icons/asyncio.png
--rw-r--r--   0 laffra     (501) staff       (20)    31709 2023-04-25 10:02:27.000000 micrologai-1.3.2/microlog/images/icons/dataclasses.png
--rw-r--r--   0 laffra     (501) staff       (20)    23729 2023-04-27 10:35:43.000000 micrologai-1.3.2/microlog/images/icons/email.png
--rw-r--r--   0 laffra     (501) staff       (20)   204541 2023-04-27 10:32:24.000000 micrologai-1.3.2/microlog/images/icons/google.png
--rw-r--r--   0 laffra     (501) staff       (20)     1533 2023-04-25 10:35:56.000000 micrologai-1.3.2/microlog/images/icons/guppy.png
--rw-r--r--   0 laffra     (501) staff       (20)   129197 2023-04-25 10:51:41.000000 micrologai-1.3.2/microlog/images/icons/http.png
--rw-r--r--   0 laffra     (501) staff       (20)    37752 2023-04-24 18:36:39.000000 micrologai-1.3.2/microlog/images/icons/jupyter.png
--rw-r--r--   0 laffra     (501) staff       (20)   198202 2023-04-24 18:31:13.000000 micrologai-1.3.2/microlog/images/icons/matplotlib.png
--rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-24 18:23:52.000000 micrologai-1.3.2/microlog/images/icons/microlog.png
--rw-r--r--   0 laffra     (501) staff       (20)    17540 2023-04-24 18:44:11.000000 micrologai-1.3.2/microlog/images/icons/networkx.png
--rw-r--r--   0 laffra     (501) staff       (20)    29693 2023-04-24 18:19:33.000000 micrologai-1.3.2/microlog/images/icons/numpy.png
--rw-r--r--   0 laffra     (501) staff       (20)     4625 2023-04-24 18:22:51.000000 micrologai-1.3.2/microlog/images/icons/pandas.png
--rw-r--r--   0 laffra     (501) staff       (20)     1532 2023-04-25 09:29:26.000000 micrologai-1.3.2/microlog/images/icons/pyparsing.png
--rw-r--r--   0 laffra     (501) staff       (20)     7209 2023-04-25 09:59:48.000000 micrologai-1.3.2/microlog/images/icons/pytest.png
--rw-r--r--   0 laffra     (501) staff       (20)    24301 2023-04-24 18:42:54.000000 micrologai-1.3.2/microlog/images/icons/python.png
--rw-r--r--   0 laffra     (501) staff       (20)    26832 2023-04-25 10:30:25.000000 micrologai-1.3.2/microlog/images/icons/re.png
--rw-r--r--   0 laffra     (501) staff       (20)     4223 2023-04-25 09:54:17.000000 micrologai-1.3.2/microlog/images/icons/squarify.png
--rw-r--r--   0 laffra     (501) staff       (20)    23401 2023-04-25 10:49:22.000000 micrologai-1.3.2/microlog/images/icons/ssl.png
--rw-r--r--   0 laffra     (501) staff       (20)    73176 2023-04-24 18:34:02.000000 micrologai-1.3.2/microlog/images/icons/tornado.png
--rw-r--r--   0 laffra     (501) staff       (20)      694 2023-04-25 10:42:25.000000 micrologai-1.3.2/microlog/images/icons/urllib.png
--rw-r--r--   0 laffra     (501) staff       (20)    63526 2023-04-27 10:38:44.000000 micrologai-1.3.2/microlog/images/icons/wsgi.png
--rw-r--r--   0 laffra     (501) staff       (20)     9088 2023-04-25 09:25:52.000000 micrologai-1.3.2/microlog/images/icons/zmq.png
--rw-r--r--   0 laffra     (501) staff       (20)   158577 2023-07-12 16:28:13.000000 micrologai-1.3.2/microlog/images/log.png
--rw-r--r--   0 laffra     (501) staff       (20)    39070 2023-07-08 10:22:16.000000 micrologai-1.3.2/microlog/images/logo-bing.png
--rw-r--r--   0 laffra     (501) staff       (20)     9392 2023-07-08 10:09:42.000000 micrologai-1.3.2/microlog/images/logo-brave.png
--rw-r--r--   0 laffra     (501) staff       (20)    39117 2023-07-08 10:21:00.000000 micrologai-1.3.2/microlog/images/logo-duckduckgo.png
--rw-r--r--   0 laffra     (501) staff       (20)    55096 2023-07-08 10:06:59.000000 micrologai-1.3.2/microlog/images/logo-google.png
--rw-r--r--   0 laffra     (501) staff       (20)    11762 2023-07-08 10:24:53.000000 micrologai-1.3.2/microlog/images/logo-hackernews.png
--rw-r--r--   0 laffra     (501) staff       (20)    10721 2023-07-08 10:22:58.000000 micrologai-1.3.2/microlog/images/logo-sourcegraph.png
--rw-r--r--   0 laffra     (501) staff       (20)    20187 2023-07-08 10:25:37.000000 micrologai-1.3.2/microlog/images/logo-stackoverflow.png
--rw-r--r--   0 laffra     (501) staff       (20)    95279 2023-07-08 10:25:22.000000 micrologai-1.3.2/microlog/images/logo-twitter.png
--rw-r--r--   0 laffra     (501) staff       (20)   241629 2023-04-11 09:10:24.000000 micrologai-1.3.2/microlog/images/markdown.png
--rw-r--r--   0 laffra     (501) staff       (20)   171389 2023-07-12 16:38:49.000000 micrologai-1.3.2/microlog/images/memory-leak.png
--rw-r--r--   0 laffra     (501) staff       (20)   184418 2023-07-12 10:42:50.000000 micrologai-1.3.2/microlog/images/overview.png
--rw-r--r--   0 laffra     (501) staff       (20)      262 2023-05-03 09:04:18.000000 micrologai-1.3.2/microlog/images/spinner.png
--rw-r--r--   0 laffra     (501) staff       (20)    68422 2023-04-10 13:38:11.000000 micrologai-1.3.2/microlog/images/status.png
--rw-r--r--   0 laffra     (501) staff       (20)   122085 2023-07-12 16:48:20.000000 micrologai-1.3.2/microlog/images/tips.png
--rw-r--r--   0 laffra     (501) staff       (20)   187519 2023-07-12 10:57:11.000000 micrologai-1.3.2/microlog/images/zoomedin.png
--rw-r--r--   0 laffra     (501) staff       (20)     4873 2023-07-24 11:05:10.000000 micrologai-1.3.2/microlog/log.py
--rw-r--r--   0 laffra     (501) staff       (20)     9743 2023-07-24 10:08:40.000000 micrologai-1.3.2/microlog/models.py
--rw-r--r--   0 laffra     (501) staff       (20)     6238 2023-07-24 12:56:21.000000 micrologai-1.3.2/microlog/server.py
--rw-r--r--   0 laffra     (501) staff       (20)      538 2023-07-19 13:49:13.000000 micrologai-1.3.2/microlog/sitecustomize.py
--rw-r--r--   0 laffra     (501) staff       (20)    17190 2023-07-24 10:07:20.000000 micrologai-1.3.2/microlog/tracer.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:55.297272 micrologai-1.3.2/micrologai.egg-info/
--rw-r--r--   0 laffra     (501) staff       (20)    45847 2023-07-26 09:45:54.000000 micrologai-1.3.2/micrologai.egg-info/PKG-INFO
--rw-r--r--   0 laffra     (501) staff       (20)     2789 2023-07-26 09:45:54.000000 micrologai-1.3.2/micrologai.egg-info/SOURCES.txt
--rw-r--r--   0 laffra     (501) staff       (20)        1 2023-07-26 09:45:54.000000 micrologai-1.3.2/micrologai.egg-info/dependency_links.txt
--rw-r--r--   0 laffra     (501) staff       (20)       48 2023-07-26 09:45:54.000000 micrologai-1.3.2/micrologai.egg-info/entry_points.txt
--rw-r--r--   0 laffra     (501) staff       (20)       41 2023-07-26 09:45:54.000000 micrologai-1.3.2/micrologai.egg-info/requires.txt
--rw-r--r--   0 laffra     (501) staff       (20)       19 2023-07-26 09:45:54.000000 micrologai-1.3.2/micrologai.egg-info/top_level.txt
--rw-r--r--   0 laffra     (501) staff       (20)      893 2023-07-26 09:45:34.000000 micrologai-1.3.2/pyproject.toml
--rw-r--r--   0 laffra     (501) staff       (20)       79 2023-07-26 09:45:55.375461 micrologai-1.3.2/setup.cfg
--rw-r--r--   0 laffra     (501) staff       (20)     1560 2023-07-26 09:45:34.000000 micrologai-1.3.2/setup.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:55.362493 micrologai-1.3.2/tests/
--rw-r--r--   0 laffra     (501) staff       (20)     1970 2023-07-03 09:26:47.000000 micrologai-1.3.2/tests/test_call_view.py
--rw-r--r--   0 laffra     (501) staff       (20)     1326 2023-06-25 13:55:44.000000 micrologai-1.3.2/tests/test_canvas.py
--rw-r--r--   0 laffra     (501) staff       (20)      318 2023-06-21 13:19:34.000000 micrologai-1.3.2/tests/test_log.py
--rw-r--r--   0 laffra     (501) staff       (20)     1755 2023-07-26 09:43:39.000000 micrologai-1.3.2/tests/test_marker_view.py
--rw-r--r--   0 laffra     (501) staff       (20)      920 2023-06-21 12:59:07.000000 micrologai-1.3.2/tests/test_print.py
--rw-r--r--   0 laffra     (501) staff       (20)      727 2023-07-02 20:31:07.000000 micrologai-1.3.2/tests/test_status.py
--rw-r--r--   0 laffra     (501) staff       (20)     2071 2023-07-02 20:45:33.000000 micrologai-1.3.2/tests/test_status_view.py
--rw-r--r--   0 laffra     (501) staff       (20)     3265 2023-07-02 20:24:48.000000 micrologai-1.3.2/tests/test_tracer.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.968997 micrologai-1.3.3/
+-rw-r--r--   0 laffra     (501) staff       (20)    30607 2023-07-05 22:06:54.000000 micrologai-1.3.3/LICENSE
+-rw-r--r--   0 laffra     (501) staff       (20)      213 2023-07-19 13:43:23.000000 micrologai-1.3.3/MANIFEST.in
+-rw-r--r--   0 laffra     (501) staff       (20)    46678 2023-07-27 20:14:28.971424 micrologai-1.3.3/PKG-INFO
+-rw-r--r--   0 laffra     (501) staff       (20)    11038 2023-07-26 18:33:07.000000 micrologai-1.3.3/README.md
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.384308 micrologai-1.3.3/dashboard/
+-rw-r--r--   0 laffra     (501) staff       (20)       75 2023-07-19 12:55:56.000000 micrologai-1.3.3/dashboard/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)    12401 2023-07-27 20:00:40.000000 micrologai-1.3.3/dashboard/canvas.py
+-rw-r--r--   0 laffra     (501) staff       (20)      864 2023-07-25 13:00:57.000000 micrologai-1.3.3/dashboard/colors.py
+-rw-r--r--   0 laffra     (501) staff       (20)      699 2023-07-19 12:55:56.000000 micrologai-1.3.3/dashboard/config.py
+-rw-r--r--   0 laffra     (501) staff       (20)     8571 2023-07-27 07:37:34.000000 micrologai-1.3.3/dashboard/design.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1854 2023-07-19 12:55:56.000000 micrologai-1.3.3/dashboard/dialog.py
+-rw-r--r--   0 laffra     (501) staff       (20)    13720 2023-07-27 19:59:14.000000 micrologai-1.3.3/dashboard/main.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1800 2023-07-19 12:55:56.000000 micrologai-1.3.3/dashboard/markdown.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1799 2023-07-25 13:09:32.000000 micrologai-1.3.3/dashboard/profiler.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2218 2023-07-27 07:38:32.000000 micrologai-1.3.3/dashboard/tips.py
+-rw-r--r--   0 laffra     (501) staff       (20)     4245 2023-07-19 12:55:56.000000 micrologai-1.3.3/dashboard/treeview.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.411112 micrologai-1.3.3/dashboard/views/
+-rw-r--r--   0 laffra     (501) staff       (20)     2165 2023-07-26 09:43:49.000000 micrologai-1.3.3/dashboard/views/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)    15841 2023-07-27 19:32:02.000000 micrologai-1.3.3/dashboard/views/call.py
+-rw-r--r--   0 laffra     (501) staff       (20)     5010 2023-07-27 20:05:28.000000 micrologai-1.3.3/dashboard/views/marker.py
+-rw-r--r--   0 laffra     (501) staff       (20)     4416 2023-07-26 13:59:52.000000 micrologai-1.3.3/dashboard/views/status.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2152 2023-07-19 12:55:56.000000 micrologai-1.3.3/dashboard/views/timeline.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.501963 micrologai-1.3.3/examples/
+-rw-r--r--   0 laffra     (501) staff       (20)     1758 2023-06-08 14:12:55.000000 micrologai-1.3.3/examples/binaryTrees.py
+-rw-r--r--   0 laffra     (501) staff       (20)    24814 2023-04-22 19:02:44.000000 micrologai-1.3.3/examples/books.json
+-rw-r--r--   0 laffra     (501) staff       (20)     2213 2023-07-08 19:41:25.000000 micrologai-1.3.3/examples/bookstore.py
+-rw-r--r--   0 laffra     (501) staff       (20)      998 2023-07-24 09:17:39.000000 micrologai-1.3.3/examples/dataframes.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1417 2023-07-24 08:53:57.000000 micrologai-1.3.3/examples/example.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1021 2023-07-12 07:42:28.000000 micrologai-1.3.3/examples/files.py
+-rw-r--r--   0 laffra     (501) staff       (20)    13859 2023-07-25 12:36:42.000000 micrologai-1.3.3/examples/go.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1857 2023-06-15 09:37:09.000000 micrologai-1.3.3/examples/helloworld.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1127 2023-07-08 12:02:09.000000 micrologai-1.3.3/examples/memory.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1178 2023-07-24 10:45:34.000000 micrologai-1.3.3/examples/modules.py
+-rwxr-xr-x   0 laffra     (501) staff       (20)      410 2023-07-24 11:06:15.000000 micrologai-1.3.3/examples/runall.sh
+-rw-r--r--   0 laffra     (501) staff       (20)      913 2023-07-24 13:11:27.000000 micrologai-1.3.3/examples/startstop.py
+-rw-r--r--   0 laffra     (501) staff       (20)      631 2023-06-08 16:27:45.000000 micrologai-1.3.3/examples/threads.py
+-rw-r--r--   0 laffra     (501) staff       (20)    93813 2023-07-24 11:09:29.000000 micrologai-1.3.3/examples/treemap.ipynb
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.557129 micrologai-1.3.3/microlog/
+-rw-r--r--   0 laffra     (501) staff       (20)      302 2023-07-27 20:13:48.000000 micrologai-1.3.3/microlog/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2798 2023-07-24 11:03:18.000000 micrologai-1.3.3/microlog/api.py
+-rw-r--r--   0 laffra     (501) staff       (20)      769 2023-07-24 11:11:41.000000 micrologai-1.3.3/microlog/config.py
+-rw-r--r--   0 laffra     (501) staff       (20)     3431 2023-07-19 12:56:01.000000 micrologai-1.3.3/microlog/explain.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.738247 micrologai-1.3.3/microlog/images/
+-rw-r--r--   0 laffra     (501) staff       (20)   292932 2023-07-12 16:09:27.000000 micrologai-1.3.3/microlog/images/anomaly.png
+-rw-rw-r--   0 laffra     (501) staff       (20)     7246 2023-04-21 09:21:45.000000 micrologai-1.3.3/microlog/images/apple-touch-icon.png
+-rw-r--r--   0 laffra     (501) staff       (20)    91386 2023-07-12 16:45:27.000000 micrologai-1.3.3/microlog/images/chatgpt.png
+-rw-r--r--   0 laffra     (501) staff       (20)   218816 2023-07-12 16:24:41.000000 micrologai-1.3.3/microlog/images/design-go.png
+-rw-r--r--   0 laffra     (501) staff       (20)   222723 2023-04-10 13:38:11.000000 micrologai-1.3.3/microlog/images/dialog.png
+-rw-r--r--   0 laffra     (501) staff       (20)   227072 2023-04-10 13:38:11.000000 micrologai-1.3.3/microlog/images/error-log.png
+-rw-rw-r--   0 laffra     (501) staff       (20)      423 2023-04-21 09:21:34.000000 micrologai-1.3.3/microlog/images/favicon-16x16.png
+-rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-21 09:21:34.000000 micrologai-1.3.3/microlog/images/favicon-32x32.png
+-rw-r--r--   0 laffra     (501) staff       (20)   160359 2023-07-12 16:32:21.000000 micrologai-1.3.3/microlog/images/fd-leak.png
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.875154 micrologai-1.3.3/microlog/images/icons/
+-rw-r--r--   0 laffra     (501) staff       (20)    14969 2023-04-25 09:23:09.000000 micrologai-1.3.3/microlog/images/icons/asyncio.png
+-rw-r--r--   0 laffra     (501) staff       (20)    31709 2023-04-25 10:02:27.000000 micrologai-1.3.3/microlog/images/icons/dataclasses.png
+-rw-r--r--   0 laffra     (501) staff       (20)    23729 2023-04-27 10:35:43.000000 micrologai-1.3.3/microlog/images/icons/email.png
+-rw-r--r--   0 laffra     (501) staff       (20)   204541 2023-04-27 10:32:24.000000 micrologai-1.3.3/microlog/images/icons/google.png
+-rw-r--r--   0 laffra     (501) staff       (20)     1533 2023-04-25 10:35:56.000000 micrologai-1.3.3/microlog/images/icons/guppy.png
+-rw-r--r--   0 laffra     (501) staff       (20)   129197 2023-04-25 10:51:41.000000 micrologai-1.3.3/microlog/images/icons/http.png
+-rw-r--r--   0 laffra     (501) staff       (20)    37752 2023-04-24 18:36:39.000000 micrologai-1.3.3/microlog/images/icons/jupyter.png
+-rw-r--r--   0 laffra     (501) staff       (20)   198202 2023-04-24 18:31:13.000000 micrologai-1.3.3/microlog/images/icons/matplotlib.png
+-rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-24 18:23:52.000000 micrologai-1.3.3/microlog/images/icons/microlog.png
+-rw-r--r--   0 laffra     (501) staff       (20)    17540 2023-04-24 18:44:11.000000 micrologai-1.3.3/microlog/images/icons/networkx.png
+-rw-r--r--   0 laffra     (501) staff       (20)    29693 2023-04-24 18:19:33.000000 micrologai-1.3.3/microlog/images/icons/numpy.png
+-rw-r--r--   0 laffra     (501) staff       (20)     4625 2023-04-24 18:22:51.000000 micrologai-1.3.3/microlog/images/icons/pandas.png
+-rw-r--r--   0 laffra     (501) staff       (20)     1532 2023-04-25 09:29:26.000000 micrologai-1.3.3/microlog/images/icons/pyparsing.png
+-rw-r--r--   0 laffra     (501) staff       (20)     7209 2023-04-25 09:59:48.000000 micrologai-1.3.3/microlog/images/icons/pytest.png
+-rw-r--r--   0 laffra     (501) staff       (20)    24301 2023-04-24 18:42:54.000000 micrologai-1.3.3/microlog/images/icons/python.png
+-rw-r--r--   0 laffra     (501) staff       (20)    26832 2023-04-25 10:30:25.000000 micrologai-1.3.3/microlog/images/icons/re.png
+-rw-r--r--   0 laffra     (501) staff       (20)     4223 2023-04-25 09:54:17.000000 micrologai-1.3.3/microlog/images/icons/squarify.png
+-rw-r--r--   0 laffra     (501) staff       (20)    23401 2023-04-25 10:49:22.000000 micrologai-1.3.3/microlog/images/icons/ssl.png
+-rw-r--r--   0 laffra     (501) staff       (20)    73176 2023-04-24 18:34:02.000000 micrologai-1.3.3/microlog/images/icons/tornado.png
+-rw-r--r--   0 laffra     (501) staff       (20)      694 2023-04-25 10:42:25.000000 micrologai-1.3.3/microlog/images/icons/urllib.png
+-rw-r--r--   0 laffra     (501) staff       (20)    63526 2023-04-27 10:38:44.000000 micrologai-1.3.3/microlog/images/icons/wsgi.png
+-rw-r--r--   0 laffra     (501) staff       (20)     9088 2023-04-25 09:25:52.000000 micrologai-1.3.3/microlog/images/icons/zmq.png
+-rw-r--r--   0 laffra     (501) staff       (20)   158577 2023-07-12 16:28:13.000000 micrologai-1.3.3/microlog/images/log.png
+-rw-r--r--   0 laffra     (501) staff       (20)    39070 2023-07-08 10:22:16.000000 micrologai-1.3.3/microlog/images/logo-bing.png
+-rw-r--r--   0 laffra     (501) staff       (20)     9392 2023-07-08 10:09:42.000000 micrologai-1.3.3/microlog/images/logo-brave.png
+-rw-r--r--   0 laffra     (501) staff       (20)    39117 2023-07-08 10:21:00.000000 micrologai-1.3.3/microlog/images/logo-duckduckgo.png
+-rw-r--r--   0 laffra     (501) staff       (20)    55096 2023-07-08 10:06:59.000000 micrologai-1.3.3/microlog/images/logo-google.png
+-rw-r--r--   0 laffra     (501) staff       (20)    11762 2023-07-08 10:24:53.000000 micrologai-1.3.3/microlog/images/logo-hackernews.png
+-rw-r--r--   0 laffra     (501) staff       (20)    10721 2023-07-08 10:22:58.000000 micrologai-1.3.3/microlog/images/logo-sourcegraph.png
+-rw-r--r--   0 laffra     (501) staff       (20)    20187 2023-07-08 10:25:37.000000 micrologai-1.3.3/microlog/images/logo-stackoverflow.png
+-rw-r--r--   0 laffra     (501) staff       (20)    95279 2023-07-08 10:25:22.000000 micrologai-1.3.3/microlog/images/logo-twitter.png
+-rw-r--r--   0 laffra     (501) staff       (20)   241629 2023-04-11 09:10:24.000000 micrologai-1.3.3/microlog/images/markdown.png
+-rw-r--r--   0 laffra     (501) staff       (20)   171389 2023-07-12 16:38:49.000000 micrologai-1.3.3/microlog/images/memory-leak.png
+-rw-r--r--   0 laffra     (501) staff       (20)   184418 2023-07-12 10:42:50.000000 micrologai-1.3.3/microlog/images/overview.png
+-rw-r--r--   0 laffra     (501) staff       (20)      262 2023-05-03 09:04:18.000000 micrologai-1.3.3/microlog/images/spinner.png
+-rw-r--r--   0 laffra     (501) staff       (20)    68422 2023-04-10 13:38:11.000000 micrologai-1.3.3/microlog/images/status.png
+-rw-r--r--   0 laffra     (501) staff       (20)   122085 2023-07-12 16:48:20.000000 micrologai-1.3.3/microlog/images/tips.png
+-rw-r--r--   0 laffra     (501) staff       (20)   187519 2023-07-12 10:57:11.000000 micrologai-1.3.3/microlog/images/zoomedin.png
+-rw-r--r--   0 laffra     (501) staff       (20)     4844 2023-07-26 12:10:57.000000 micrologai-1.3.3/microlog/log.py
+-rw-r--r--   0 laffra     (501) staff       (20)     9743 2023-07-24 10:08:40.000000 micrologai-1.3.3/microlog/models.py
+-rw-r--r--   0 laffra     (501) staff       (20)     6102 2023-07-27 20:12:14.000000 micrologai-1.3.3/microlog/server.py
+-rw-r--r--   0 laffra     (501) staff       (20)      538 2023-07-19 13:49:13.000000 micrologai-1.3.3/microlog/sitecustomize.py
+-rw-r--r--   0 laffra     (501) staff       (20)    17190 2023-07-24 10:07:20.000000 micrologai-1.3.3/microlog/tracer.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.915794 micrologai-1.3.3/micrologai.egg-info/
+-rw-r--r--   0 laffra     (501) staff       (20)    46678 2023-07-27 20:14:28.000000 micrologai-1.3.3/micrologai.egg-info/PKG-INFO
+-rw-r--r--   0 laffra     (501) staff       (20)     2768 2023-07-27 20:14:28.000000 micrologai-1.3.3/micrologai.egg-info/SOURCES.txt
+-rw-r--r--   0 laffra     (501) staff       (20)        1 2023-07-27 20:14:28.000000 micrologai-1.3.3/micrologai.egg-info/dependency_links.txt
+-rw-r--r--   0 laffra     (501) staff       (20)       48 2023-07-27 20:14:28.000000 micrologai-1.3.3/micrologai.egg-info/entry_points.txt
+-rw-r--r--   0 laffra     (501) staff       (20)       41 2023-07-27 20:14:28.000000 micrologai-1.3.3/micrologai.egg-info/requires.txt
+-rw-r--r--   0 laffra     (501) staff       (20)       19 2023-07-27 20:14:28.000000 micrologai-1.3.3/micrologai.egg-info/top_level.txt
+-rw-r--r--   0 laffra     (501) staff       (20)      893 2023-07-27 20:13:48.000000 micrologai-1.3.3/pyproject.toml
+-rw-r--r--   0 laffra     (501) staff       (20)       79 2023-07-27 20:14:28.981920 micrologai-1.3.3/setup.cfg
+-rw-r--r--   0 laffra     (501) staff       (20)     1560 2023-07-27 20:13:48.000000 micrologai-1.3.3/setup.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.966525 micrologai-1.3.3/tests/
+-rw-r--r--   0 laffra     (501) staff       (20)     1970 2023-07-03 09:26:47.000000 micrologai-1.3.3/tests/test_call_view.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1326 2023-06-25 13:55:44.000000 micrologai-1.3.3/tests/test_canvas.py
+-rw-r--r--   0 laffra     (501) staff       (20)      318 2023-06-21 13:19:34.000000 micrologai-1.3.3/tests/test_log.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1755 2023-07-26 09:43:39.000000 micrologai-1.3.3/tests/test_marker_view.py
+-rw-r--r--   0 laffra     (501) staff       (20)      920 2023-06-21 12:59:07.000000 micrologai-1.3.3/tests/test_print.py
+-rw-r--r--   0 laffra     (501) staff       (20)      727 2023-07-02 20:31:07.000000 micrologai-1.3.3/tests/test_status.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2071 2023-07-02 20:45:33.000000 micrologai-1.3.3/tests/test_status_view.py
+-rw-r--r--   0 laffra     (501) staff       (20)     3265 2023-07-02 20:24:48.000000 micrologai-1.3.3/tests/test_tracer.py
```

### Comparing `micrologai-1.3.2/LICENSE` & `micrologai-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/PKG-INFO` & `micrologai-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrologai
-Version: 1.3.2
+Version: 1.3.3
 Summary: A continuous profiler and logger for Python written entirely in Python
 Home-page: https://www.chrislaffra.org/
 Author: Chris Laffra
 Author-email: Chris Laffra <chris@chrislaffra.com>
 License:                      Server Side Public License
                              VERSION 1, OCTOBER 16, 2018
         
@@ -605,47 +605,52 @@
 git3 clone https://github.com/micrologai/microlog
 cd micrologai/microlog
 python3 setup.py install
 ```
 
 # How to use microlog.ai
 
-If you used the setup command shown above, _Microlog_ is enabled for all Python processes running on that Python VM. 
-
+If you used the setup command shown above, _Microlog_ is enabled as a continuous profiler for all Python processes running on that Python VM. 
 To use microlog manually, use:
 ```python
 import microlog
 
 with microlog.enabled():
     # run any Python code
 ```
 
+The part of _Microlog_ that records the execution can be found in [microlog/tracer.py](microlog/tracer.py#L89). It starts a new thread and samples the other threads at regular intervals, see [sample](microlog/tracer.py#L240). The tracer also sets up wrappers for logging and print statements. The logs are compressed and saved when _Microlog_ is stopped, by [microlog/log.py](microlog/log.py#L94).
+
 To give you an idea of the features of _Microlog_, you could run all the examples. This does assume you set up microlog globally. In that case, run:
 
 ```console
 sh examples/runall.sh
 ```
 
 This runs for a minute and eventually produces 13 logs. You will see lines appear looking like this:
 
 ```console
 📈 Microlog ··· 26.3s ··· 4.6KB ··· examples-memory ··· http://127.0.0.1:4000/log/examples-memory/2023_07_12_10_24_53 🚀
 ```
 
 This shows how long the app ran, the size of the (compressed) log, its name, and a URL to view the result.
-The report URL is rendered by the _Microlog_ server implemented in `microlog/server.py`.  If it is not yet running,
+The report URL is rendered by the _Microlog_ server implemented in [microlog/server.py](microlog/server.py).  If it is not yet running,
 you can start it as follows:
 
 ```console
 python3 microlog/server.py
 ```
 
 # The Microlog.ai UI 
 
-To describe the UI features of _Microlog_, we will look at the output of the `examples\memory.py` example:
+A live demo of the _Microlog_ UI can be found at [micrologai.github.io/microlog](https://micrologai.github.io/microlog/). The UI is
+written almost entirely in Python, see [dashboard](dashboard). The _Microlog_ UI runs in the browser using PyScript. 
+
+To describe the UI features of _Microlog_, we will look at the output of the [examples\memory.py](examples\memory.py) example (the live preview is at
+[GitHub Pages](https://micrologai.github.io/microlog/#examples-memory/2023_07_26_14_11_38/)):
 
 ![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/overview.png)
 
 The main elements of the UI are:
 
  - `Log list`, at the left, showing currently available logs on the local machine.
  - `Timeline`, the starting point for analysis of your application:
```

### Comparing `micrologai-1.3.2/README.md` & `micrologai-1.3.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,47 +32,52 @@
 git3 clone https://github.com/micrologai/microlog
 cd micrologai/microlog
 python3 setup.py install
 ```
 
 # How to use microlog.ai
 
-If you used the setup command shown above, _Microlog_ is enabled for all Python processes running on that Python VM. 
-
+If you used the setup command shown above, _Microlog_ is enabled as a continuous profiler for all Python processes running on that Python VM. 
 To use microlog manually, use:
 ```python
 import microlog
 
 with microlog.enabled():
     # run any Python code
 ```
 
+The part of _Microlog_ that records the execution can be found in [microlog/tracer.py](microlog/tracer.py#L89). It starts a new thread and samples the other threads at regular intervals, see [sample](microlog/tracer.py#L240). The tracer also sets up wrappers for logging and print statements. The logs are compressed and saved when _Microlog_ is stopped, by [microlog/log.py](microlog/log.py#L94).
+
 To give you an idea of the features of _Microlog_, you could run all the examples. This does assume you set up microlog globally. In that case, run:
 
 ```console
 sh examples/runall.sh
 ```
 
 This runs for a minute and eventually produces 13 logs. You will see lines appear looking like this:
 
 ```console
 📈 Microlog ··· 26.3s ··· 4.6KB ··· examples-memory ··· http://127.0.0.1:4000/log/examples-memory/2023_07_12_10_24_53 🚀
 ```
 
 This shows how long the app ran, the size of the (compressed) log, its name, and a URL to view the result.
-The report URL is rendered by the _Microlog_ server implemented in `microlog/server.py`.  If it is not yet running,
+The report URL is rendered by the _Microlog_ server implemented in [microlog/server.py](microlog/server.py).  If it is not yet running,
 you can start it as follows:
 
 ```console
 python3 microlog/server.py
 ```
 
 # The Microlog.ai UI 
 
-To describe the UI features of _Microlog_, we will look at the output of the `examples\memory.py` example:
+A live demo of the _Microlog_ UI can be found at [micrologai.github.io/microlog](https://micrologai.github.io/microlog/). The UI is
+written almost entirely in Python, see [dashboard](dashboard). The _Microlog_ UI runs in the browser using PyScript. 
+
+To describe the UI features of _Microlog_, we will look at the output of the [examples\memory.py](examples\memory.py) example (the live preview is at
+[GitHub Pages](https://micrologai.github.io/microlog/#examples-memory/2023_07_26_14_11_38/)):
 
 ![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/overview.png)
 
 The main elements of the UI are:
 
  - `Log list`, at the left, showing currently available logs on the local machine.
  - `Timeline`, the starting point for analysis of your application:
```

### Comparing `micrologai-1.3.2/dashboard/canvas.py` & `micrologai-1.3.3/dashboard/canvas.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,31 +10,34 @@
 
 import dashboard.profiler as profiler
 from dashboard import config
 
 jquery = js.jQuery
 
 class Canvas():
-    def __init__(self, elementId, redrawCallback, dragCallback=None, zoomCallback=None, minOffsetX=0, minOffsetY=0, fixedX=False, fixedY=False, fixedScaleX=False, fixedScaleY=False) -> None:
+    def __init__(self, elementId, redrawCallback, dragCallback=None, zoomCallback=None, clickCallback=None, minOffsetX=0, minOffsetY=0, fixedX=False, fixedY=False, fixedScaleX=False, fixedScaleY=False) -> None:
         self.scaleX = config.CANVAS_INITIAL_SCALE
         self.scaleY = config.CANVAS_INITIAL_SCALE
         self.offsetX = config.CANVAS_INITIAL_OFFSET_X
         self.offsetY = config.CANVAS_INITIAL_OFFSET_Y
         self.redrawCallback = redrawCallback
         self.dragCallback = dragCallback
         self.zoomCallback = zoomCallback
+        self.clickCallback = clickCallback
         self.elementId = elementId
         self.minOffsetX = minOffsetX
         self.minOffsetY = minOffsetY
         self.canvas = jquery(elementId)
         self._width = float(self.canvas.attr("width") or js.jQuery("body").width())
         self._height = float(self.canvas.attr("height") or js.jQuery("body").height())
         self.context = self.canvas[0].getContext("2d")
         self.dragX = 0
         self.dragY = 0
+        self.dragging = False
+        self.mouseDown = False
         self.maxX = 0
         self.fixedX = fixedX
         self.fixedY = fixedY
         self.fixedScaleX = fixedScaleX
         self.fixedScaleY = fixedScaleY
         self.setupEventHandlers()
 
@@ -46,52 +49,66 @@
             .on("mouseup", pyodide.ffi.create_proxy(lambda event: self.mouseup(event))) \
             .on("mousewheel", pyodide.ffi.create_proxy(lambda event: self.mousewheel(event)))
 
     def mousedown(self, event):
         from dashboard.dialog import dialog
         self.dragX = event.originalEvent.pageX
         self.dragY = event.originalEvent.pageY
+        self.hideHighlights()
+        self.mouseDown = True
+        self.dragging = False
 
     def isDragging(self):
-        return self.dragX != 0
+        return self.dragging
 
     def mousemove(self, event):
-        if self.isDragging():
+        if self.mouseDown:
+            self.dragging = True
             dx = 0 if self.fixedX else event.originalEvent.pageX - self.dragX
             dy = 0 if self.fixedY else event.originalEvent.pageY - self.dragY
             if self.offsetX + dx > self.width() * 0.9:
                 dx = 0
             self.dragX = event.originalEvent.pageX
             self.dragY = event.originalEvent.pageY
             if dx < -3 or dx > 3 or dy:
                 self.drag(dx, dy, event)
             event.preventDefault()
     
     def drag(self, dx, dy, event=None):
         if not self.fixedX:
             self.offsetX = self.offsetX + dx
         if not self.fixedY:
-            self.offsetY = min(21, self.offsetY + dy)
+            self.offsetY = min(0, self.offsetY + dy)
         if event and self.dragCallback:
             self.dragCallback(dx, dy)
             self.redraw()
 
     def mouseleave(self, event):
         self.dragX = 0
         self.dragY = 0
+        self.dragging = False
+        self.mouseDown = False
 
     def mouseup(self, event):
-        self.dragX = 0
-        self.dragY = 0
-        if self.offsetY > 0:
-            self.offsetY = 0
-            self.redraw()
+        if self.isDragging():
+            self.dragX = 0
+            self.dragY = 0
+        else:
+            if self.offsetY > 0:
+                self.offsetY = 0
+            self.clickCallback(event.originalEvent.offsetX, event.originalEvent.offsetY)
+        self.dragging = False
+        self.mouseDown = False
+
+    def hideHighlights(self):
+        js.jQuery(".highlight").css("left", 10000)
 
     def mousewheel(self, event):
         event.preventDefault()
+        self.hideHighlights()
         x = event.originalEvent.offsetX
         y = event.originalEvent.offsetY
         self.zoom(x, y, 2 if event.originalEvent.wheelDelta > 0 else 0.5, event)
 
     def on(self, event, callback):
         self.canvas.on(event, pyodide.ffi.create_proxy(lambda event: callback(event)))
         return self
@@ -124,22 +141,23 @@
             self.canvas.attr("width", width)
         else:
             return self._width
 
     def height(self, height=0):
         return self.canvas.attr("height", height) if height else float(self.canvas.attr("height") or 0)
 
-    @profiler.profile("Canvas.toScreenX")
     def toScreenX(self, x):
         return x * self.scaleX + self.offsetX
 
+    def toScreenY(self, y):
+        return y * self.scaleY + self.offsetY
+
     def fromScreenX(self, x):
         return x - self.offsetX / self.scaleX
 
-    @profiler.profile("Canvas.toScreenDimension")
     def toScreenDimension(self, w):
         return w * self.scaleX
 
     def fromScreenDimension(self, w):
         return w / self.scaleX
 
     def setStrokeStyle(self, color):
```

### Comparing `micrologai-1.3.2/dashboard/colors.py` & `micrologai-1.3.3/dashboard/colors.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/dashboard/config.py` & `micrologai-1.3.3/dashboard/config.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/dashboard/design.py` & `micrologai-1.3.3/dashboard/design.py`

 * *Files 26% similar despite different names*

```diff
@@ -190,45 +190,45 @@
             return images[node.name]
         topName = node.name.split(".")[0]
         if topName in images:
             return images[topName]
 
 
 images = {
-    "runpy": "/images/icons/python.png",
-    "matplotlib": "/images/icons/matplotlib.png",
-    "matplotlib_inline": "/images/icons/matplotlib.png",
-    "squarify": "/images/icons/squarify.png",
-    "pandas": "/images/icons/pandas.png",
-    "numpy": "/images/icons/numpy.png",
-    "asyncio": "/images/icons/asyncio.png",
-    "pyparsing": "/images/icons/pyparsing.png",
-    "ssl": "/images/icons/ssl.png",
-    "http": "/images/icons/http.png",
-    "httplib2": "/images/icons/http.png",
-    "urllib3": "/images/icons/http.png",
-    "socket": "/images/icons/http.png",
-    "pluggy": "/images/icons/pluggy.webp",
-    "pytest": "/images/icons/pytest.png",
-    "testing_tools": "/images/icons/pytest.png",
-    "_pytest": "/images/icons/pytest.png",
-    "networkx": "/images/icons/networkx.png",
-    "re": "/images/icons/re.png",
-    "sre_compile": "/images/icons/re.png",
-    "sre_parse": "/images/icons/re.png",
-    "dataclasses": "/images/icons/dataclasses.png",
-    "tornado": "/images/icons/tornado.png",
-    "urllib": "/images/icons/urllib.png",
-    "guppy": "/images/icons/guppy.png",
-    "zmq": "/images/icons/zmq.png",
-    "email": "/images/icons/email.png",
-    "google_auth_oauthlib": "/images/icons/google.png",
-    "google_auth_httplib2": "/images/icons/google.png",
-    "googleapiclient": "/images/icons/google.png",
-    "google": "/images/icons/google.png",
-    "wsgiref": "/images/icons/wsgi.png",
-    "IPython": "/images/icons/jupyter.png",
-    "jupyter_client": "/images/icons/jupyter.png",
-    "ipykernel": "/images/icons/jupyter.png",
-    "Jupyter": "/images/icons/jupyter.png",
-    "microlog": "/images/icons/microlog.png",
+    "runpy": "/microlog/images/icons/python.png",
+    "matplotlib": "/microlog/images/icons/matplotlib.png",
+    "matplotlib_inline": "/microlog/images/icons/matplotlib.png",
+    "squarify": "/microlog/images/icons/squarify.png",
+    "pandas": "/microlog/images/icons/pandas.png",
+    "numpy": "/microlog/images/icons/numpy.png",
+    "asyncio": "/microlog/images/icons/asyncio.png",
+    "pyparsing": "/microlog/images/icons/pyparsing.png",
+    "ssl": "/microlog/images/icons/ssl.png",
+    "http": "/microlog/images/icons/http.png",
+    "httplib2": "/microlog/images/icons/http.png",
+    "urllib3": "/microlog/images/icons/http.png",
+    "socket": "/microlog/images/icons/http.png",
+    "pluggy": "/microlog/images/icons/pluggy.webp",
+    "pytest": "/microlog/images/icons/pytest.png",
+    "testing_tools": "/microlog/images/icons/pytest.png",
+    "_pytest": "/microlog/images/icons/pytest.png",
+    "networkx": "/microlog/images/icons/networkx.png",
+    "re": "/microlog/images/icons/re.png",
+    "sre_compile": "/microlog/images/icons/re.png",
+    "sre_parse": "/microlog/images/icons/re.png",
+    "dataclasses": "/microlog/images/icons/dataclasses.png",
+    "tornado": "/microlog/images/icons/tornado.png",
+    "urllib": "/microlog/images/icons/urllib.png",
+    "guppy": "/microlog/images/icons/guppy.png",
+    "zmq": "/microlog/images/icons/zmq.png",
+    "email": "/microlog/images/icons/email.png",
+    "google_auth_oauthlib": "/microlog/images/icons/google.png",
+    "google_auth_httplib2": "/microlog/images/icons/google.png",
+    "googleapiclient": "/microlog/images/icons/google.png",
+    "google": "/microlog/images/icons/google.png",
+    "wsgiref": "/microlog/images/icons/wsgi.png",
+    "IPython": "/microlog/images/icons/jupyter.png",
+    "jupyter_client": "/microlog/images/icons/jupyter.png",
+    "ipykernel": "/microlog/images/icons/jupyter.png",
+    "Jupyter": "/microlog/images/icons/jupyter.png",
+    "microlog": "/microlog/images/icons/microlog.png",
 }
```

### Comparing `micrologai-1.3.2/dashboard/dialog.py` & `micrologai-1.3.3/dashboard/dialog.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/dashboard/main.py` & `micrologai-1.3.3/dashboard/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,51 +40,59 @@
         self.currentTab = "Timeline"
         self.hover = None
         self.calls = []
         self.statuses = []
         self.markers = []
         self.design = Design([])
         self.tips = Tips([])
-        self.flameCanvas = self.createCanvas(self.flameElementId, self.clickFlame, self.dragFlame, self.zoomFlame, self.flameMousemove, fixedScaleY=True)
-        self.timelineCanvas = self.createCanvas(self.timelineElementId, self.clickTimeline, self.dragTimeline, self.zoomTimeline, self.timelineMousemove, fixedY=True, fixedScaleY=True)
+        self.flameCanvas = self.createCanvas(self.flameElementId, self.drawFlame, self.clickFlame, self.dragFlame, self.zoomFlame, self.flameMousemove, fixedScaleY=True)
+        self.timelineCanvas = self.createCanvas(self.timelineElementId, self.drawTimeline, self.clickTimeline, self.dragTimeline, self.zoomTimeline, self.timelineMousemove, fixedY=True, fixedScaleY=True)
         js.jQuery(".tabs").on("tabsactivate", pyodide.ffi.create_proxy(lambda event, ui: self.activateTab(event, ui)))
+        js.jQuery("#filter").val(getFilterFromUrl())
 
     def dragFlame(self, dx, dy):
         self.timelineCanvas.drag(dx, dy)
         CallView.positionThreads(self.flameCanvas)
+        self.drawTimeline()
 
     def zoomFlame(self, x, y, scale):
         self.timelineCanvas.zoom(x, y, scale)
+        self.drawTimeline()
 
     def dragTimeline(self, dx, dy):
         self.flameCanvas.drag(dx, dy)
+        self.drawFlame()
 
     def zoomTimeline(self, x, y, scale):
         self.flameCanvas.zoom(x, y, scale)
+        self.drawFlame()
 
     def resize(self, width, height):
         timelineHeight = config.TIMELINE_OFFSET_Y + config.TIMELINE_HEIGHT 
         self.timelineCanvas.width(width)
         self.timelineCanvas.height(timelineHeight)
         self.flameCanvas.width(width)
         self.flameCanvas.height(height - timelineHeight)
         self.redraw()
 
-    def createCanvas(self, elementId, click, drag, zoom, mousemove, fixedY=False, fixedScaleY=False):
-        return (canvas.Canvas(elementId, self.redraw, drag, zoom, minOffsetX=48, minOffsetY=0, fixedY=fixedY, fixedScaleY=fixedScaleY)
-            .on("mousemove", mousemove)
-            .on("click", click))
+    def createCanvas(self, elementId, redraw, click, drag, zoom, mousemove, fixedY=False, fixedScaleY=False):
+        return (canvas.Canvas(elementId, redraw, drag, zoom, click, minOffsetX=48, minOffsetY=0, fixedY=fixedY, fixedScaleY=fixedScaleY)
+            .on("mousemove", mousemove))
 
     def activateTab(self, event, ui):
         self.currentTab = ui.newTab.text()
         self.redraw()
 
     def reset(self):
         self.timelineCanvas.reset()
         self.flameCanvas.reset()
+        self.hover = None
+        CallView.reset()
+        StatusView.reset()
+        MarkerView.reset()
 
     @profiler.profile("Flamegraph.convertLog")
     def convertLog(self, log):
         self.calls = [ CallView(self.flameCanvas, model) for model in log.log.calls ]
         self.statuses = [ StatusView(self.timelineCanvas, model) for model in log.log.statuses ]
         self.markers = [ MarkerView(self.timelineCanvas, model) for model in log.log.markers ]
 
@@ -109,18 +117,17 @@
         self.hover = None
         js.jQuery(self.flameElementId).empty()
         js.jQuery(self.timelineElementId).empty()
    
     @profiler.report("Redrawing the whole UI.")
     def redraw(self, event=None):
         if self.currentTab == "Timeline":
-            self.draw()
-            debug("Draw", profiler.getTime("Flamegraph.draw"))
+            self.drawTimeline()
+            self.drawFlame()
         elif self.currentTab == "Design":
-            js.jQuery("#debug").html("")
             self.design = Design(self.calls)
             self.design.draw()
         elif self.currentTab == "Explanation":
             explain(getLogFromUrl())
         elif self.currentTab == "Tips":
             self.tips = Tips(self.calls)
         if event:
@@ -142,142 +149,180 @@
             <tr>
                 <td class="log-when">At&nbsp;{when:.2f}s</td>
                 <td class="log-stack">{fixNewline(stack)}</td>
                 <td class="log-message">{entry}</td>
             </tr>
         """
 
-    @profiler.profile("Flamegraph.draw")
-    def draw(self):
-        self.flameCanvas.clear("#DDD")
-        self.timelineCanvas.clear("#DDD")
+    def loading(self, name):
+        self.clear()
+        self.timelineCanvas.text(-20, 20, f"Loading {name}...", color="#BBB", font="16px Arial")
+
+    def clear(self, canvas=None):
+        if canvas:
+            canvas.clear("#222")
+        else:
+            self.flameCanvas.clear("#222")
+            self.timelineCanvas.clear("#222")
+        dialog.hide()
+        js.jQuery(".highlight").css("left", 10000)
+
+    @profiler.report("Flamegraph.drawTimeline")
+    def drawTimeline(self, event=None):
+        self.clear(self.timelineCanvas)
+        js.jQuery("#hairline").css("display", "none")
         self.hover = None
+        self.drawStatuses()
+        self.drawMarkers()
+        self.timeline.draw(self.timelineCanvas)
+
+    @profiler.profile("Flamegraph.drawStatuses")
+    def drawStatuses(self):
         canvasScaleX = self.flameCanvas.scaleX
         canvasOffsetX = self.flameCanvas.offsetX
         canvasWidth = self.flameCanvas.width()
         StatusView.drawAll(self.timelineCanvas, [
             view for view in self.sampleStatuses()
             if not view.offscreen(canvasScaleX, canvasOffsetX, canvasWidth)
         ])
-        self.timeline.draw(self.timelineCanvas)
-        CallView.drawAll(self.flameCanvas, [
-            view for view in self.calls
+
+    @profiler.profile("Flamegraph.drawMarkers")
+    def drawMarkers(self):
+        canvasScaleX = self.flameCanvas.scaleX
+        canvasOffsetX = self.flameCanvas.offsetX
+        canvasWidth = self.flameCanvas.width()
+        MarkerView.drawAll(self.timelineCanvas, [
+            view for view in self.markers
             if not view.offscreen(canvasScaleX, canvasOffsetX, canvasWidth)
         ])
-        MarkerView.drawAll(self.timelineCanvas, [
-            view for view in self.markers 
+        
+    @profiler.report("Flamegraph.drawFlame")
+    def drawFlame(self, event=None):
+        self.clear(self.flameCanvas)
+        js.jQuery("#hairline").css("display", "none")
+        canvasScaleX = self.flameCanvas.scaleX
+        canvasOffsetX = self.flameCanvas.offsetX
+        canvasWidth = self.flameCanvas.width()
+        CallView.drawAll(self.flameCanvas, [
+            view for view in self.calls
             if not view.offscreen(canvasScaleX, canvasOffsetX, canvasWidth)
         ])
         
     def sampleStatuses(self):
         if not self.statuses: 
             return []
         statuses = [ self.statuses[0] ]
         sample = int(max(1, 1 / self.flameCanvas.scaleX / 4))
         for n in range(len(self.statuses)):
             if n % sample == 0:
                 statuses.append(self.statuses[n])
         statuses.append(self.statuses[-1])
         return statuses
 
-
     def flameMousemove(self, event):
         self.mousemoveCanvas(self.flameCanvas, self.calls, event)
 
     def timelineMousemove(self, event):
         self.mousemoveCanvas(self.timelineCanvas, self.statuses, event)
         self.mousemoveCanvas(self.timelineCanvas, self.markers, event)
     
     def mousemoveCanvas(self, canvas, views, event):
         if canvas.isDragging() or not hasattr(event.originalEvent, "offsetX"):
             return
         x, y, _, _ = canvas.absolute(event.originalEvent.offsetX, event.originalEvent.offsetY)
-        w = canvas.width()
+        canvasScaleX = self.flameCanvas.scaleX
+        canvasOffsetX = self.flameCanvas.offsetX
+        canvasWidth = self.flameCanvas.width()
         for view in views:
-            if not view.offscreen(w) and view.inside(x, y):
+            if not view.offscreen(canvasScaleX, canvasOffsetX, canvasWidth) and view.inside(x, y):
                 if not self.hover is view:
                     if self.hover:
                         self.hover.mouseleave(x, y)
                     view.mouseenter(x, y)
                     self.hover = view
                 view.mousemove(x, y)
 
-    def clickFlame(self, event):
-        self.clickCanvas(self.flameCanvas, self.calls, event)
+    def clickFlame(self, x, y):
+        self.clickCanvas(self.flameCanvas, self.calls, x, y)
 
-    def clickTimeline(self, event):
-        self.clickCanvas(self.timelineCanvas, self.markers, event)
+    def clickTimeline(self, x, y):
+        self.clickCanvas(self.timelineCanvas, self.markers, x, y)
 
-    def clickCanvas(self, canvas, views, event):
-        if canvas.isDragging() or not hasattr(event.originalEvent, "offsetX"):
-            return
-        x, y, _, _ = canvas.absolute(event.originalEvent.offsetX, event.originalEvent.offsetY)
+    def clickCanvas(self, canvas, views, x, y):
+        x, y, _, _ = canvas.absolute(x, y)
         for view in views:
             if view.inside(x, y):
+                print("click", x, y, view)
                 view.click(x, y)
                 return True
         dialog.hide()
 
 
 def setUrl(log=None):
     if not "Electron" in js.navigator.userAgent:
-        server = js.location.hostname
-        port = js.location.port
         filter = js.jQuery(".filter").val()
         if log:
-            url = f"http://{server}:{port}/log/{log}?filter={filter}"
-        else:
-            url = f"http://{server}:{port}/?filter={filter}"
-        js.history.pushState(js.object(), "", url)
+            url = f"#{log}/{filter}"
+            js.history.pushState(js.object(), "", url)
 
 
 def showLog(log):
-    dialog.hide()
-    CallView.reset()
-    StatusView.reset()
-    MarkerView.reset()
+    flamegraph.clear()
     flamegraph.reset()
     loadLog(log)
     setUrl(log)
     js.jQuery("#explanation").text("")
     js.jQuery("#tabs-log").find("table").empty()
 
 
 def loadLog(name):
-    url = f"http://127.0.0.1:4000/zip/{name}"
+    flamegraph.loading(name)
+    url = f"zip/{name}"
     js.jQuery.get(url, pyodide.ffi.create_proxy(lambda data, status, xhr: showFlamegraph(data)))
 
 
 def explain(name):
     if not js.jQuery("#explanation").text():
-        js.jQuery("#explanation").text("Asking OpenAI to explain this program...")
-        url = f"http://127.0.0.1:4000/explain/{name}"
+        message = "Asking OpenAI to explain this program..."
+        if js.document.location.host == 'micrologai.github.io':
+            "This feature is not enabled on Github Pages."
+        js.jQuery("#explanation").text(message)
+        url = f"explain/{name}"
         js.jQuery.get(url, pyodide.ffi.create_proxy(lambda data, status, xhr: js.jQuery("#explanation").html(markdown.toHTML(data))))
 
 
 @profiler.profile("Logs.show")
 def showAllLogs():
     dialog.hide()
     filter = js.jQuery(".filter").val()
-    url = f"http://127.0.0.1:4000/logs?filter={filter}"
+    url = f"logs?filter={filter}"
     js.jQuery.get(url, pyodide.ffi.create_proxy(lambda data, status, xhr: renderLogs(data.strip().split("\n"))))
     js.jQuery(".logs") \
         .empty() \
-        .append(js.jQuery("<img>").addClass("loading").attr("src", "/images/spinner.gif"))
+        .append(js.jQuery("<img>").addClass("loading").attr("src", "/microlog/images/spinner.gif"))
 
 
 def deleteLog(name, doneHandler):
-    url = f"http://127.0.0.1:4000/delete/{name}"
+    url = f"delete/{name}"
     js.jQuery.get(url, pyodide.ffi.create_proxy(lambda data, status, xhr: doneHandler()))
 
 
 def getLogFromUrl():
-    path = js.document.location.pathname
-    if path.startswith("/log/"):
-        return path[len("/log/"):]
+    hash = js.document.location.hash
+    if hash:
+        app, name, _ = hash[1:].split("/")
+        return f"{app}/{name}"
+    return ""
+
+def getFilterFromUrl():
+    hash = js.document.location.hash
+    if hash:
+        _, _, filter = hash[1:].split("/")
+        return filter
+    return ""
 
 
 def renderLogs(logList: List[str]):
     from collections import defaultdict
     if not any(logList):
         js.jQuery(".logs").empty().append(js.jQuery("<span>").css("color", "pink").text("No matching logs found")),
         return
@@ -299,29 +344,18 @@
 
 
 flamegraph = Flamegraph("#flameCanvas", "#timelineCanvas")
 
 
 def showFlamegraph(data):
     log.log.load(data)
-    js.jQuery("#debug").html("")
     flamegraph.load(log)
     flamegraph.redraw()
 
 
-def debug(label: str, value=None) -> None:
-    if value == None:
-        message = label
-    else:
-        val = f"{value:.3f}" if isinstance(value, float) else value
-        message = f"{label}: {val}<br>"
-    js.jQuery("#debug").html(message + js.jQuery("#debug").html())
-    js.console.log(message)
-    
-
 def refreshLogs(event=None):
     js.setTimeout(pyodide.ffi.create_proxy(lambda: showAllLogs()), 1)
 
 
 def setupLogHandlers():
     js.jQuery(".refresh").click(pyodide.ffi.create_proxy(refreshLogs))
     js.jQuery(".filter").keyup(pyodide.ffi.create_proxy(refreshLogs))
@@ -345,12 +379,11 @@
     js.jQuery(".logs").css("height", height - filterHeight)
     js.jQuery(".tree").css("height", height - filterHeight - padding)
 
 def main():
     setupLogHandlers()
     showAllLogs()
     loadLog(getLogFromUrl())
-    debug("Logs", profiler.getTime("Logs.show"))
     js.jQuery(js.window).on("resize", pyodide.ffi.create_proxy(resize))
     resize()
 
 main()
```

### Comparing `micrologai-1.3.2/dashboard/markdown.py` & `micrologai-1.3.3/dashboard/markdown.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/dashboard/profiler.py` & `micrologai-1.3.3/dashboard/profiler.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/dashboard/tips.py` & `micrologai-1.3.3/dashboard/tips.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         prompt = " AND ".join(random.choice(PROMPTS).split(" "))
         js.jQuery("#tips").empty() \
             .append(js.jQuery("<div>").html(f"""
                 {usage}
                 To improve best practices or performance of your code, consider these resources:
             """)) \
             .append(*[
-                self.createButton(provider, f"/images/logo-{provider.lower()}.png", f"{url}Python AND {' AND '.join(list(self.modules)[:2])} AND {prompt}")
+                self.createButton(provider, f"/microlog/images/logo-{provider.lower()}.png", f"{url}Python AND {' AND '.join(list(self.modules)[:2])} AND {prompt}")
                 for provider, url in SEARCH_URLS.items()
             ])
     
     def createButton(self, provider, logo, url):
         return (js.jQuery("<button>")
             .addClass("tips-button")
             .append(
```

### Comparing `micrologai-1.3.2/dashboard/treeview.py` & `micrologai-1.3.3/dashboard/treeview.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/dashboard/views/__init__.py` & `micrologai-1.3.3/dashboard/views/__init__.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/dashboard/views/call.py` & `micrologai-1.3.3/dashboard/views/call.py`

 * *Files 6% similar despite different names*

```diff
@@ -146,15 +146,16 @@
             self.canvas.line(self.x, self.y, self.x + self.w, self.y, 1, "#DDD")
             self.canvas.line(self.x, self.y, self.x, self.y + self.h, 1, "#AAA")
         if w > self.minWidth:
             dx = self.canvas.fromScreenDimension(4)
             self.canvas.text(self.x + dx, self.y + 2, self.getLabel(), color, self.w - 2 * dx)
 
     def click(self, x, y):
-        self.showPopup(x, y)
+        if not self.canvas.isDragging():
+            self.showPopup(x, y)
 
     def showPopup(self, x, y):
         if self.canvas.isDragging():
             return
         if dialog.showing and CallView.selected is self:
             dialog.hide()
             return
@@ -185,21 +186,27 @@
 
     def highlightCall(self, link):
         CallView.selected = CallView.instances[int(link.attr("index"))]
         self.canvas.redraw()
 
     def mouseenter(self, x, y):
         View.mouseenter(self, x, y)
+        left = self.canvas.toScreenX(self.x)
+        top = self.canvas.toScreenY(self.y) + config.FLAME_OFFSET_Y + config.TIMELINE_HEIGHT + 4
+        w = self.canvas.toScreenDimension(self.w)
+        h = config.LINE_HEIGHT
         if self.threadId in self.showThreads and self.canvas.toScreenDimension(self.w) > self.minWidth:
-            self.canvas.rect(self.x, self.y, self.w, self.h, 2, "red")
+            js.jQuery(".call-highlight").appendTo(self.canvas.canvas.parent())
+            js.jQuery("#call-highlight-top").css("left", left).css("top", top).css("width", w).css("height", 0)
+            js.jQuery("#call-highlight-bottom").css("left", left).css("top", top + h).css("width", w).css("height", 0)
+            js.jQuery("#call-highlight-left").css("left", left).css("top", top).css("width", 0).css("height", h)
+            js.jQuery("#call-highlight-right").css("left", left + w).css("top", top).css("width", 0).css("height", h)
 
     def mouseleave(self, x, y):
         View.mouseleave(self, x, y)
-        if self.threadId in self.showThreads and self.canvas.toScreenDimension(self.w) > self.minWidth:
-            self.canvas.redraw()
         
     def getCpu(self):
         stats = [
             view
             for view in status.StatusView.instances
             if view.when >= self.when and view.when <= self.when + self.duration
         ]
```

### Comparing `micrologai-1.3.2/dashboard/views/marker.py` & `micrologai-1.3.3/dashboard/views/marker.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,19 +83,22 @@
 
     def mouseenter(self, x, y):
         View.mouseenter(self, x, y)
         self.select()
     
     def select(self):
         self.draw()
-        self.canvas.rect(self.x, self.y, self.w, self.h, color="white")
+        (js.jQuery("#marker-highlight")
+            .css("left", self.canvas.toScreenX(self.x))
+            .css("top", self.canvas.toScreenY(self.y) + 42)
+            .click(pyodide.ffi.create_proxy(lambda event: self.click(0, 0)))
+            .appendTo(self.canvas.canvas.parent()))
 
     def mouseleave(self, x, y):
         View.mouseleave(self, x, y)
-        self.canvas.redraw()
 
     def formatStack(self, full=True):
         def shortFile(filename):
             parts = filename.split("/")
             if parts[-1] == "__init__.py":
                 parts.pop()
             return parts[-1]
```

### Comparing `micrologai-1.3.2/dashboard/views/status.py` & `micrologai-1.3.3/dashboard/views/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     def reset(cls):
         StatusView.instances.clear()
         js.jQuery("#summary").css("display", "none")
 
     def inside(self, x, y):
         if not self.previous:
             return False
-        return not self.offscreen() and x >= self.previous.x and x < self.x and y >= self.y and y < self.y + self.h
+        return x >= self.previous.x and x < self.x and y >= self.y and y < self.y + self.h
 
     @classmethod
     @profiler.profile("StatusView.drawAll")
     def drawAll(cls, canvas: canvas.Canvas, views):
         if views:
             canvas.clear("#222")
             cls.drawCpu(canvas, views)
```

### Comparing `micrologai-1.3.2/dashboard/views/timeline.py` & `micrologai-1.3.3/dashboard/views/timeline.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/examples/binaryTrees.py` & `micrologai-1.3.3/examples/binaryTrees.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/examples/books.json` & `micrologai-1.3.3/examples/books.json`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/examples/bookstore.py` & `micrologai-1.3.3/examples/bookstore.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/examples/dataframes.py` & `micrologai-1.3.3/examples/dataframes.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/examples/example.py` & `micrologai-1.3.3/examples/example.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/examples/files.py` & `micrologai-1.3.3/examples/files.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/examples/go.py` & `micrologai-1.3.3/examples/go.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/examples/helloworld.py` & `micrologai-1.3.3/examples/helloworld.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/examples/memory.py` & `micrologai-1.3.3/examples/memory.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/examples/modules.py` & `micrologai-1.3.3/examples/modules.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/examples/startstop.py` & `micrologai-1.3.3/examples/startstop.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/examples/threads.py` & `micrologai-1.3.3/examples/threads.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/examples/treemap.ipynb` & `micrologai-1.3.3/examples/treemap.ipynb`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/api.py` & `micrologai-1.3.3/microlog/api.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/config.py` & `micrologai-1.3.3/microlog/config.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/explain.py` & `micrologai-1.3.3/microlog/explain.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/anomaly.png` & `micrologai-1.3.3/microlog/images/anomaly.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/apple-touch-icon.png` & `micrologai-1.3.3/microlog/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/chatgpt.png` & `micrologai-1.3.3/microlog/images/chatgpt.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/design-go.png` & `micrologai-1.3.3/microlog/images/design-go.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/dialog.png` & `micrologai-1.3.3/microlog/images/dialog.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/error-log.png` & `micrologai-1.3.3/microlog/images/error-log.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/favicon-32x32.png` & `micrologai-1.3.3/microlog/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/fd-leak.png` & `micrologai-1.3.3/microlog/images/fd-leak.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/asyncio.png` & `micrologai-1.3.3/microlog/images/icons/asyncio.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/dataclasses.png` & `micrologai-1.3.3/microlog/images/icons/dataclasses.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/email.png` & `micrologai-1.3.3/microlog/images/icons/email.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/google.png` & `micrologai-1.3.3/microlog/images/icons/google.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/guppy.png` & `micrologai-1.3.3/microlog/images/icons/guppy.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/http.png` & `micrologai-1.3.3/microlog/images/icons/http.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/jupyter.png` & `micrologai-1.3.3/microlog/images/icons/jupyter.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/matplotlib.png` & `micrologai-1.3.3/microlog/images/icons/matplotlib.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/microlog.png` & `micrologai-1.3.3/microlog/images/icons/microlog.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/networkx.png` & `micrologai-1.3.3/microlog/images/icons/networkx.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/numpy.png` & `micrologai-1.3.3/microlog/images/icons/numpy.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/pandas.png` & `micrologai-1.3.3/microlog/images/icons/pandas.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/pyparsing.png` & `micrologai-1.3.3/microlog/images/icons/pyparsing.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/pytest.png` & `micrologai-1.3.3/microlog/images/icons/pytest.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/python.png` & `micrologai-1.3.3/microlog/images/icons/python.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/re.png` & `micrologai-1.3.3/microlog/images/icons/re.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/squarify.png` & `micrologai-1.3.3/microlog/images/icons/squarify.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/ssl.png` & `micrologai-1.3.3/microlog/images/icons/ssl.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/tornado.png` & `micrologai-1.3.3/microlog/images/icons/tornado.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/urllib.png` & `micrologai-1.3.3/microlog/images/icons/urllib.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/wsgi.png` & `micrologai-1.3.3/microlog/images/icons/wsgi.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/icons/zmq.png` & `micrologai-1.3.3/microlog/images/icons/zmq.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/log.png` & `micrologai-1.3.3/microlog/images/log.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/logo-bing.png` & `micrologai-1.3.3/microlog/images/logo-bing.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/logo-brave.png` & `micrologai-1.3.3/microlog/images/logo-brave.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/logo-duckduckgo.png` & `micrologai-1.3.3/microlog/images/logo-duckduckgo.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/logo-google.png` & `micrologai-1.3.3/microlog/images/logo-google.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/logo-hackernews.png` & `micrologai-1.3.3/microlog/images/logo-hackernews.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/logo-sourcegraph.png` & `micrologai-1.3.3/microlog/images/logo-sourcegraph.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/logo-stackoverflow.png` & `micrologai-1.3.3/microlog/images/logo-stackoverflow.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/logo-twitter.png` & `micrologai-1.3.3/microlog/images/logo-twitter.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/markdown.png` & `micrologai-1.3.3/microlog/images/markdown.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/memory-leak.png` & `micrologai-1.3.3/microlog/images/memory-leak.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/overview.png` & `micrologai-1.3.3/microlog/images/overview.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/status.png` & `micrologai-1.3.3/microlog/images/status.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/tips.png` & `micrologai-1.3.3/microlog/images/tips.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/images/zoomedin.png` & `micrologai-1.3.3/microlog/images/zoomedin.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/log.py` & `micrologai-1.3.3/microlog/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #
 # Microlog. Copyright (c) 2023 laffra, dcharbon. All rights reserved.
 #
 
 from collections import defaultdict
 import datetime
 import os
-import re
 import sys
 import time
 import bz2
-import traceback;
 
 from microlog import config
 from microlog.models import Call
 from microlog.models import CallSite
 from microlog.models import Stack
 from microlog.models import Status
 from microlog.models import toGB
 from microlog.models import Marker
 
 verbose = True
-debug = False
+debug = True
 
 class Log():
     def __init__(self):
         self.start()
 
     def start(self):
         self.running = True
```

### Comparing `micrologai-1.3.2/microlog/models.py` & `micrologai-1.3.3/microlog/models.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/server.py` & `micrologai-1.3.3/microlog/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,61 +33,61 @@
     logger.info(s)
 
 
 class LogServer(BaseHTTPRequestHandler):
     def do_GET(self):
         debug(f"GET {self.path}")
         try:
-            if self.path.startswith("/logs?"):
+            if "/logs?" in self.path:
                 import urllib
                 query = urllib.parse.urlparse(self.path).query
                 query_components = dict(qc.split("=") for qc in query.split("&"))
                 filter = query_components["filter"]
                 logs = []
                 for root, dirs, files in os.walk(paths.logs_path, topdown=False):
                     for name in sorted([file for file in files if file.endswith(".zip")]):
                         application = root.split("/")[-1]
                         if name.endswith(".zip") and filter in root:
                             logs.append(f"{application}/{name[:-4]}\n")
                 return self.sendData("text/html", bytes("\n".join(logs), encoding="utf-8"))
 
-            if self.path.startswith("/zip/"):
-                name = f"{self.path[5:]}.log.zip".replace("%20", " ")
+            if "/zip/" in self.path:
+                name = f"{self.path[self.path.index('/zip/') + 5:]}.log.zip".replace("%20", " ")
                 return self.sendData("application/microlog", self.readLog(name))
 
             if self.path.startswith("/delete/"):
                 name = f"{self.path[8:]}.log.zip".replace("%20", " ")
-                if name.startswith("logs/"):
-                    name = name[5:]
                 path = os.path.join(paths.logs_path, name)
                 os.remove(path)
                 return self.sendData("text/html", bytes("OK", encoding="utf-8"))
 
-            if self.path.startswith("/explain/"):
+            if "/explain/" in self.path:
                 import explain
-                name = f"{self.path[9:]}.log.zip".replace("%20", " ")
+                name = f"{self.path[self.path.index('/explain/') + 9:]}.log.zip".replace("%20", " ")
                 log = self.readLog(name)
                 debug(f"Explain {name}")
                 debug(f"Log is {len(log)} bytes")
                 explanation = explain.explainLog(name.split("/")[0], log.decode("utf-8"))
                 print(explanation)
                 return self.sendData("text/html", bytes(explanation, encoding="utf-8"))
 
             if self.path in ["/stop"]:
                 return 
 
-            if self.path.startswith("/images/"):
-                with open(f"microlog/{self.path[1:]}", "rb") as fd:
+            if self.path.startswith("/microlog/images/"):
+                with open(self.path[1:], "rb") as fd:
                     return self.sendData("image/png", fd.read())
 
-            if self.path in ["", "/"] or self.path.startswith("/?filter=") or self.path.startswith("/log/") and not self.path.endswith(".py"):
-                with open('dashboard/index.html') as fd:
+            if self.path in ["", "/"]:
+                with open('index.html') as fd:
                     return self.sendData("text/html", bytes(f"{fd.read()}", encoding="utf-8"))
 
-            name = "/".join(self.path.split("/")[4:]) if self.path.startswith("/log/") else self.path[1:]
+            name = self.path[1:]
+            if not os.path.exists(name) and name.startswith("microlog/"):
+                name = name[9:]
             with open(name) as fd:
                 return self.sendData("text/html", bytes(f"{fd.read()}", encoding="utf-8"))
         except Exception as e:
             logging.error(e)
             import traceback
             traceback.print_exc()
             return str(e)
```

### Comparing `micrologai-1.3.2/microlog/sitecustomize.py` & `micrologai-1.3.3/microlog/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/microlog/tracer.py` & `micrologai-1.3.3/microlog/tracer.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/micrologai.egg-info/PKG-INFO` & `micrologai-1.3.3/micrologai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrologai
-Version: 1.3.2
+Version: 1.3.3
 Summary: A continuous profiler and logger for Python written entirely in Python
 Home-page: https://www.chrislaffra.org/
 Author: Chris Laffra
 Author-email: Chris Laffra <chris@chrislaffra.com>
 License:                      Server Side Public License
                              VERSION 1, OCTOBER 16, 2018
         
@@ -605,47 +605,52 @@
 git3 clone https://github.com/micrologai/microlog
 cd micrologai/microlog
 python3 setup.py install
 ```
 
 # How to use microlog.ai
 
-If you used the setup command shown above, _Microlog_ is enabled for all Python processes running on that Python VM. 
-
+If you used the setup command shown above, _Microlog_ is enabled as a continuous profiler for all Python processes running on that Python VM. 
 To use microlog manually, use:
 ```python
 import microlog
 
 with microlog.enabled():
     # run any Python code
 ```
 
+The part of _Microlog_ that records the execution can be found in [microlog/tracer.py](microlog/tracer.py#L89). It starts a new thread and samples the other threads at regular intervals, see [sample](microlog/tracer.py#L240). The tracer also sets up wrappers for logging and print statements. The logs are compressed and saved when _Microlog_ is stopped, by [microlog/log.py](microlog/log.py#L94).
+
 To give you an idea of the features of _Microlog_, you could run all the examples. This does assume you set up microlog globally. In that case, run:
 
 ```console
 sh examples/runall.sh
 ```
 
 This runs for a minute and eventually produces 13 logs. You will see lines appear looking like this:
 
 ```console
 📈 Microlog ··· 26.3s ··· 4.6KB ··· examples-memory ··· http://127.0.0.1:4000/log/examples-memory/2023_07_12_10_24_53 🚀
 ```
 
 This shows how long the app ran, the size of the (compressed) log, its name, and a URL to view the result.
-The report URL is rendered by the _Microlog_ server implemented in `microlog/server.py`.  If it is not yet running,
+The report URL is rendered by the _Microlog_ server implemented in [microlog/server.py](microlog/server.py).  If it is not yet running,
 you can start it as follows:
 
 ```console
 python3 microlog/server.py
 ```
 
 # The Microlog.ai UI 
 
-To describe the UI features of _Microlog_, we will look at the output of the `examples\memory.py` example:
+A live demo of the _Microlog_ UI can be found at [micrologai.github.io/microlog](https://micrologai.github.io/microlog/). The UI is
+written almost entirely in Python, see [dashboard](dashboard). The _Microlog_ UI runs in the browser using PyScript. 
+
+To describe the UI features of _Microlog_, we will look at the output of the [examples\memory.py](examples\memory.py) example (the live preview is at
+[GitHub Pages](https://micrologai.github.io/microlog/#examples-memory/2023_07_26_14_11_38/)):
 
 ![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/overview.png)
 
 The main elements of the UI are:
 
  - `Log list`, at the left, showing currently available logs on the local machine.
  - `Timeline`, the starting point for analysis of your application:
```

### Comparing `micrologai-1.3.2/micrologai.egg-info/SOURCES.txt` & `micrologai-1.3.3/micrologai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 setup.py
 dashboard/__init__.py
 dashboard/canvas.py
 dashboard/colors.py
 dashboard/config.py
 dashboard/design.py
 dashboard/dialog.py
-dashboard/index.html
 dashboard/main.py
 dashboard/markdown.py
 dashboard/profiler.py
 dashboard/tips.py
 dashboard/treeview.py
 dashboard/views/__init__.py
 dashboard/views/call.py
```

### Comparing `micrologai-1.3.2/pyproject.toml` & `micrologai-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "micrologai"
-version = "1.3.2"
+version = "1.3.3"
 description = "A continuous profiler and logger for Python written entirely in Python"
 readme = "README.md"
 authors = [{ name = "Chris Laffra", email = "chris@chrislaffra.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `micrologai-1.3.2/setup.py` & `micrologai-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='Microlog',
     description='A continuous profiler and logger for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version="1.3.2",
+    version="1.3.3",
     author='Chris Laffra',
     author_email='laffra@gmail.com',
     url='https://www.chrislaffra.org/',
     packages=setuptools.find_packages(include=[
         'microlog',
         'dashboard',
     ]),
```

### Comparing `micrologai-1.3.2/tests/test_call_view.py` & `micrologai-1.3.3/tests/test_call_view.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/tests/test_canvas.py` & `micrologai-1.3.3/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/tests/test_marker_view.py` & `micrologai-1.3.3/tests/test_marker_view.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/tests/test_print.py` & `micrologai-1.3.3/tests/test_print.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/tests/test_status.py` & `micrologai-1.3.3/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/tests/test_status_view.py` & `micrologai-1.3.3/tests/test_status_view.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.2/tests/test_tracer.py` & `micrologai-1.3.3/tests/test_tracer.py`

 * *Files identical despite different names*

