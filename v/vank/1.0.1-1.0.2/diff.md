# Comparing `tmp/Vank-1.0.1.tar.gz` & `tmp/vank-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Vank-1.0.1.tar", last modified: Tue Mar 28 08:17:10 2023, max compression
+gzip compressed data, was "vank-1.0.2.tar", last modified: Thu Jul 27 09:02:14 2023, max compression
```

## Comparing `Vank-1.0.1.tar` & `vank-1.0.2.tar`

### file list

```diff
@@ -1,64 +1,62 @@
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-03-28 08:17:10.118207 Vank-1.0.1/
--rw-r--r--   0 vank       (501) staff       (20)     1066 2023-03-08 02:58:20.000000 Vank-1.0.1/LICENSE
--rw-r--r--   0 vank       (501) staff       (20)     1970 2023-03-28 08:17:10.117758 Vank-1.0.1/PKG-INFO
--rw-r--r--   0 vank       (501) staff       (20)      260 2023-03-08 02:58:20.000000 Vank-1.0.1/README.md
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-03-28 08:17:10.056075 Vank-1.0.1/Vank/
--rw-r--r--   0 vank       (501) staff       (20)        0 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)     1849 2023-03-11 08:07:38.000000 Vank-1.0.1/Vank/__main__.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-03-28 08:17:10.071579 Vank-1.0.1/Vank/cmds/
--rw-r--r--   0 vank       (501) staff       (20)     3208 2023-03-23 10:29:18.000000 Vank-1.0.1/Vank/cmds/init.py
--rw-r--r--   0 vank       (501) staff       (20)     1535 2023-03-10 17:43:19.000000 Vank-1.0.1/Vank/cmds/subapp.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-03-28 08:17:10.075172 Vank-1.0.1/Vank/core/
--rw-r--r--   0 vank       (501) staff       (20)       64 2023-03-08 03:18:25.000000 Vank-1.0.1/Vank/core/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)    11392 2023-03-28 08:04:44.000000 Vank-1.0.1/Vank/core/app.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-03-28 08:17:10.077604 Vank-1.0.1/Vank/core/config/
--rw-r--r--   0 vank       (501) staff       (20)     1171 2023-03-27 09:15:25.000000 Vank-1.0.1/Vank/core/config/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)     1266 2023-03-27 09:09:28.000000 Vank-1.0.1/Vank/core/config/base.py
--rw-r--r--   0 vank       (501) staff       (20)      863 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/core/exceptions.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-03-28 08:17:10.079403 Vank-1.0.1/Vank/core/handlers/
--rw-r--r--   0 vank       (501) staff       (20)       72 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/core/handlers/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)     1391 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/core/handlers/exception.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-03-28 08:17:10.083301 Vank-1.0.1/Vank/core/http/
--rw-r--r--   0 vank       (501) staff       (20)      114 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/core/http/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)     5863 2023-03-28 03:33:40.000000 Vank-1.0.1/Vank/core/http/request.py
--rw-r--r--   0 vank       (501) staff       (20)    10146 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/core/http/response.py
--rw-r--r--   0 vank       (501) staff       (20)     3794 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/core/http/status.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-03-28 08:17:10.090855 Vank-1.0.1/Vank/core/routing/
--rw-r--r--   0 vank       (501) staff       (20)        0 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/core/routing/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)     2540 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/core/routing/converters.py
--rw-r--r--   0 vank       (501) staff       (20)     7355 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/core/routing/route.py
--rw-r--r--   0 vank       (501) staff       (20)     3367 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/core/routing/router.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-03-28 08:17:10.093469 Vank-1.0.1/Vank/core/views/
--rw-r--r--   0 vank       (501) staff       (20)       87 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/core/views/__init__.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-03-28 08:17:10.096526 Vank-1.0.1/Vank/core/views/static/
--rw-r--r--   0 vank       (501) staff       (20)        0 2023-03-12 09:38:14.000000 Vank-1.0.1/Vank/core/views/static/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)     1372 2023-03-12 16:56:16.000000 Vank-1.0.1/Vank/core/views/static/control.py
--rw-r--r--   0 vank       (501) staff       (20)      279 2023-03-13 06:58:31.000000 Vank-1.0.1/Vank/core/views/static/views.py
--rw-r--r--   0 vank       (501) staff       (20)     3600 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/core/views/view.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-03-28 08:17:10.097446 Vank-1.0.1/Vank/log/
--rw-r--r--   0 vank       (501) staff       (20)        0 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/log/__init__.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-03-28 08:17:10.101794 Vank-1.0.1/Vank/middleware/
--rw-r--r--   0 vank       (501) staff       (20)       88 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/middleware/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)     1891 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/middleware/base.py
--rw-r--r--   0 vank       (501) staff       (20)     3601 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/middleware/cors.py
--rw-r--r--   0 vank       (501) staff       (20)     2789 2023-03-13 07:02:19.000000 Vank-1.0.1/Vank/middleware/session.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-03-28 08:17:10.116440 Vank-1.0.1/Vank/utils/
--rw-r--r--   0 vank       (501) staff       (20)      171 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/utils/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)     1004 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/utils/argument_inspect.py
--rw-r--r--   0 vank       (501) staff       (20)      707 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/utils/cmd.py
--rw-r--r--   0 vank       (501) staff       (20)     6249 2023-03-28 03:39:41.000000 Vank-1.0.1/Vank/utils/datastructures.py
--rw-r--r--   0 vank       (501) staff       (20)      414 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/utils/exception.py
--rw-r--r--   0 vank       (501) staff       (20)      563 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/utils/load_module.py
--rw-r--r--   0 vank       (501) staff       (20)     1064 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/utils/log.py
--rw-r--r--   0 vank       (501) staff       (20)     7025 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/utils/parsers.py
--rw-r--r--   0 vank       (501) staff       (20)     2809 2023-03-27 03:10:44.000000 Vank-1.0.1/Vank/utils/reloader.py
--rw-r--r--   0 vank       (501) staff       (20)      393 2023-03-08 02:58:20.000000 Vank-1.0.1/Vank/utils/response.py
--rw-r--r--   0 vank       (501) staff       (20)     1158 2023-03-27 03:38:46.000000 Vank-1.0.1/Vank/utils/signal.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-03-28 08:17:10.069675 Vank-1.0.1/Vank.egg-info/
--rw-r--r--   0 vank       (501) staff       (20)     1970 2023-03-28 08:17:10.000000 Vank-1.0.1/Vank.egg-info/PKG-INFO
--rw-r--r--   0 vank       (501) staff       (20)     1180 2023-03-28 08:17:10.000000 Vank-1.0.1/Vank.egg-info/SOURCES.txt
--rw-r--r--   0 vank       (501) staff       (20)        1 2023-03-28 08:17:10.000000 Vank-1.0.1/Vank.egg-info/dependency_links.txt
--rw-r--r--   0 vank       (501) staff       (20)       44 2023-03-28 08:17:10.000000 Vank-1.0.1/Vank.egg-info/requires.txt
--rw-r--r--   0 vank       (501) staff       (20)        5 2023-03-28 08:17:10.000000 Vank-1.0.1/Vank.egg-info/top_level.txt
--rw-r--r--   0 vank       (501) staff       (20)      650 2023-03-28 08:04:14.000000 Vank-1.0.1/pyproject.toml
--rw-r--r--   0 vank       (501) staff       (20)       38 2023-03-28 08:17:10.118356 Vank-1.0.1/setup.cfg
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.043025 vank-1.0.2/
+-rw-r--r--   0 vank       (501) staff       (20)     1066 2023-03-08 02:58:20.000000 vank-1.0.2/LICENSE
+-rw-r--r--   0 vank       (501) staff       (20)     2392 2023-07-27 09:02:14.042399 vank-1.0.2/PKG-INFO
+-rw-r--r--   0 vank       (501) staff       (20)      682 2023-07-19 09:53:59.000000 vank-1.0.2/README.md
+-rw-r--r--   0 vank       (501) staff       (20)      695 2023-07-19 09:53:59.000000 vank-1.0.2/pyproject.toml
+-rw-r--r--   0 vank       (501) staff       (20)       38 2023-07-27 09:02:14.043181 vank-1.0.2/setup.cfg
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.005644 vank-1.0.2/vank/
+-rw-r--r--   0 vank       (501) staff       (20)       64 2023-07-19 09:53:59.000000 vank-1.0.2/vank/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)     2069 2023-07-27 08:56:56.000000 vank-1.0.2/vank/__main__.py
+-rw-r--r--   0 vank       (501) staff       (20)       22 2023-07-19 09:53:59.000000 vank-1.0.2/vank/__version__.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.000704 vank-1.0.2/vank/applications/
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.012358 vank-1.0.2/vank/applications/static/
+-rw-r--r--   0 vank       (501) staff       (20)        0 2023-07-19 09:53:59.000000 vank-1.0.2/vank/applications/static/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)     1291 2023-07-21 09:45:07.000000 vank-1.0.2/vank/applications/static/control.py
+-rw-r--r--   0 vank       (501) staff       (20)      238 2023-07-21 11:24:01.000000 vank-1.0.2/vank/applications/static/urls.py
+-rw-r--r--   0 vank       (501) staff       (20)      382 2023-07-21 11:25:13.000000 vank-1.0.2/vank/applications/static/views.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.014099 vank-1.0.2/vank/cli/
+-rw-r--r--   0 vank       (501) staff       (20)     3518 2023-07-21 11:32:42.000000 vank-1.0.2/vank/cli/init.py
+-rw-r--r--   0 vank       (501) staff       (20)     1623 2023-07-24 03:20:51.000000 vank-1.0.2/vank/cli/subapp.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.019435 vank-1.0.2/vank/core/
+-rw-r--r--   0 vank       (501) staff       (20)      308 2023-07-19 09:53:59.000000 vank-1.0.2/vank/core/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)    13049 2023-07-24 09:57:03.000000 vank-1.0.2/vank/core/app.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.021094 vank-1.0.2/vank/core/config/
+-rw-r--r--   0 vank       (501) staff       (20)     1226 2023-07-21 10:21:42.000000 vank-1.0.2/vank/core/config/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)     2600 2023-07-25 02:41:46.000000 vank-1.0.2/vank/core/config/base.py
+-rw-r--r--   0 vank       (501) staff       (20)     5245 2023-07-21 10:37:28.000000 vank-1.0.2/vank/core/context.py
+-rw-r--r--   0 vank       (501) staff       (20)      875 2023-07-24 10:11:32.000000 vank-1.0.2/vank/core/exceptions.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.022557 vank-1.0.2/vank/core/handlers/
+-rw-r--r--   0 vank       (501) staff       (20)       72 2023-07-19 09:53:59.000000 vank-1.0.2/vank/core/handlers/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)     1275 2023-07-19 09:53:59.000000 vank-1.0.2/vank/core/handlers/exception.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.026009 vank-1.0.2/vank/core/http/
+-rw-r--r--   0 vank       (501) staff       (20)      127 2023-07-19 09:53:59.000000 vank-1.0.2/vank/core/http/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)     7076 2023-07-19 09:53:59.000000 vank-1.0.2/vank/core/http/request.py
+-rw-r--r--   0 vank       (501) staff       (20)    10398 2023-07-24 09:57:03.000000 vank-1.0.2/vank/core/http/response.py
+-rw-r--r--   0 vank       (501) staff       (20)     3792 2023-07-19 09:53:59.000000 vank-1.0.2/vank/core/http/status.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.029031 vank-1.0.2/vank/core/routing/
+-rw-r--r--   0 vank       (501) staff       (20)        0 2023-07-19 09:53:59.000000 vank-1.0.2/vank/core/routing/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)     2545 2023-07-24 03:20:51.000000 vank-1.0.2/vank/core/routing/converters.py
+-rw-r--r--   0 vank       (501) staff       (20)     6925 2023-07-21 10:21:42.000000 vank-1.0.2/vank/core/routing/route.py
+-rw-r--r--   0 vank       (501) staff       (20)     3316 2023-07-24 09:59:29.000000 vank-1.0.2/vank/core/routing/router.py
+-rw-r--r--   0 vank       (501) staff       (20)     1357 2023-07-21 10:57:22.000000 vank-1.0.2/vank/core/view.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.034292 vank-1.0.2/vank/middleware/
+-rw-r--r--   0 vank       (501) staff       (20)       88 2023-07-19 09:53:59.000000 vank-1.0.2/vank/middleware/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)     1621 2023-07-19 09:53:59.000000 vank-1.0.2/vank/middleware/base.py
+-rw-r--r--   0 vank       (501) staff       (20)     3640 2023-07-19 09:53:59.000000 vank-1.0.2/vank/middleware/cors.py
+-rw-r--r--   0 vank       (501) staff       (20)     2941 2023-07-19 09:53:59.000000 vank-1.0.2/vank/middleware/session.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.041444 vank-1.0.2/vank/utils/
+-rw-r--r--   0 vank       (501) staff       (20)      171 2023-07-19 09:53:59.000000 vank-1.0.2/vank/utils/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)      640 2023-07-21 10:37:28.000000 vank-1.0.2/vank/utils/cli.py
+-rw-r--r--   0 vank       (501) staff       (20)     6947 2023-07-21 10:37:28.000000 vank-1.0.2/vank/utils/datastructures.py
+-rw-r--r--   0 vank       (501) staff       (20)      996 2023-07-24 03:20:51.000000 vank-1.0.2/vank/utils/load_module.py
+-rw-r--r--   0 vank       (501) staff       (20)     1083 2023-07-19 09:53:59.000000 vank-1.0.2/vank/utils/log.py
+-rw-r--r--   0 vank       (501) staff       (20)     2439 2023-07-21 10:37:28.000000 vank-1.0.2/vank/utils/parsers.py
+-rw-r--r--   0 vank       (501) staff       (20)     2816 2023-07-21 11:02:28.000000 vank-1.0.2/vank/utils/reloader.py
+-rw-r--r--   0 vank       (501) staff       (20)     1113 2023-07-19 09:53:59.000000 vank-1.0.2/vank/utils/signal.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.009480 vank-1.0.2/vank.egg-info/
+-rw-r--r--   0 vank       (501) staff       (20)     2392 2023-07-27 09:02:13.000000 vank-1.0.2/vank.egg-info/PKG-INFO
+-rw-r--r--   0 vank       (501) staff       (20)     1156 2023-07-27 09:02:13.000000 vank-1.0.2/vank.egg-info/SOURCES.txt
+-rw-r--r--   0 vank       (501) staff       (20)        1 2023-07-27 09:02:13.000000 vank-1.0.2/vank.egg-info/dependency_links.txt
+-rw-r--r--   0 vank       (501) staff       (20)       51 2023-07-27 09:02:13.000000 vank-1.0.2/vank.egg-info/entry_points.txt
+-rw-r--r--   0 vank       (501) staff       (20)       20 2023-07-27 09:02:13.000000 vank-1.0.2/vank.egg-info/requires.txt
+-rw-r--r--   0 vank       (501) staff       (20)        5 2023-07-27 09:02:13.000000 vank-1.0.2/vank.egg-info/top_level.txt
```

### Comparing `Vank-1.0.1/LICENSE` & `vank-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Vank-1.0.1/PKG-INFO` & `vank-1.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Vank
-Version: 1.0.1
+Name: vank
+Version: 1.0.2
 Summary: A Python Web Framework
 Author-email: WanKe <852003793@qq.com>
 License: MIT License
         
         Copyright (c) 2022 852003793
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,26 +34,38 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vank
 
 一个基于Python的Web框架
 
-### QuickStart
+### 特性
+
+- 高度个性化: 你可以构建许多自定义的组件添加到配置当中、在恰当的时机使用他们。例如自定义路由转换器、错误处理器等。
+- 低学习成本: 这是一个非常简单的框架，你可以在仅仅几个小时内学习完并熟练使用它。
+- 完备的文档: 具有非常详细的文档供开发者们学习，并且了解框架是如何运行的。
+
+***
+
+### 快速开始
+
 - 安装Vank
+
 ```shell
-pip install Vank
+pip install vank
 ```
+
 - 初始化项目
 
 ```shell
-python -m Vank init -n mysite
+python -m vank init -n mysite
 ```
+
 - 运行项目
+
 ```shell
 cd mysite
 python main.py
 ```
 
- 
 ***
 [技术文档](http://docs.bestvank.cn/)
```

### Comparing `Vank-1.0.1/Vank/__main__.py` & `vank-1.0.2/vank/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,70 @@
 # @FileName: __main__.py
 # @Date    : 2023/1/24-21:27
-# @Author  : Vank
-# @Project : Vank
+# @Author  : vank
+# @Project : vank
 import sys
 import pkgutil
 from pathlib import Path
 from difflib import get_close_matches
-from Vank.utils.cmd import BaseCommand
-from Vank.utils.load_module import import_from_str
+from vank.utils.cli import BaseCommand
+from vank.utils.load_module import import_from_str
 
 
 class MainCommand(BaseCommand):
-    epilog = '可以通过 python -m Vank <命令> -h 查看用法'
+    epilog = 'You can view usage through python -m vank <command> -h'
 
     def run(self, argv):
         c = argv[1] if len(argv) > 1 else 'help'
 
         if c in ['help', '-h', '-help']:
             self.print_help()
             sys.exit()
         self.dispatch(c, argv)
 
     def dispatch(self, c, argv):
         commands = self.find_commands()
         try:
             command_class = commands[c]
         except KeyError:
-            self.stderr.write(f'未知命令:{c}\n')
+            self.stderr.write(f'Unknown command:{c}\n')
             close_matches = get_close_matches(c, commands)
             if close_matches:
-                self.stderr.write(f'与{c}相似的命令有:\n- ')
+                self.stderr.write(f'I guess what you are thinking is:\n- ')
                 self.stderr.write("\n- ".join(close_matches))
         else:
-            import_from_str(command_class)().run(argv)
+            command_class().run(argv)
 
     def find_commands(self):
         cmds = {}
-        builtin_cmds_path = Path(__file__).parent.joinpath('cmds').as_posix()
+        builtin_cmds_path = Path(__file__).parent.joinpath('cli').as_posix()
         for module_finder, name, is_package in pkgutil.iter_modules([builtin_cmds_path]):
             if is_package:
                 continue
             cmds.update(
-                {name: f'Vank.cmds.{name}.Command'}
+                {name: import_from_str(f'vank.cli.{name}:Command')}
             )
 
         return cmds
 
     def print_help(self):
-        self.stdout.write('当前可用的命令有:\n- ')
+        self.stdout.write('The currently available commands are:\n- ')
         self.stdout.write(
             '\n- '.join(
                 [
                     f'{name.ljust(25, " ")}{cls.description or "---"}'
                     for name, cls in self.find_commands().items()
                 ]
             ))
-        self.stdout.write(f'\n\n{self.epilog}')
+        self.stdout.write(f'\n\n{self.epilog}\n')
 
 
-MainCommand().run(sys.argv)
+def entry_point():
+    """
+    此函数主要作用是为了在分发包时的console_scripts提供入口点
+    """
+    main = MainCommand()
+    sys.exit(main.run(sys.argv))
+
+
+if __name__ == '__main__':
+    entry_point()
```

### Comparing `Vank-1.0.1/Vank/cmds/init.py` & `vank-1.0.2/vank/cli/init.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 # @FileName: init.py
 # @Date    : 2023/1/27-1:28
-# @Author  : Vank
-# @Project : Vank
-import hashlib
+# @Author  : vank
+# @Project : vank
 import sys
-import os.path
 import time
-
-from Vank.utils.cmd import BaseCommand
+import hashlib
+import os.path
+from vank.utils.cli import BaseCommand
 
 settings_template = """
 from pathlib import Path
 
 PROJECT_BASE_DIR = Path(__file__).parent
 # 密钥
 SECRET_KEY = '%(secret)s'
 
+# 子应用
+SUB_APPLICATIONS = [
+    'vank.applications.static.urls:sub',
+]
+
 # 含参数路由转换器
 ROUTE_CONVERTERS = {
-    'int': 'Vank.core.routing.converters.IntConverter',
-    'float': 'Vank.core.routing.converters.FloatConverter',
-    'email': 'Vank.core.routing.converters.EmailConverter',
-    'uuid': 'Vank.core.routing.converters.UUIDConverter',
-    'path': 'Vank.core.routing.converters.PathConverter',
+    'int': 'vank.core.routing.converters:IntConverter',
+    'float': 'vank.core.routing.converters:FloatConverter',
+    'email': 'vank.core.routing.converters:EmailConverter',
+    'uuid': 'vank.core.routing.converters:UUIDConverter',
+    'path': 'vank.core.routing.converters:PathConverter',
+    'str': 'vank.core.routing.converters:StrConverter',
 }
 
 # 中间件
 MIDDLEWARES = [
-    'Vank.middleware.session.SessionMiddleware'
+    'vank.middleware.session:SessionMiddleware'
 ]
 
 # 错误处理器
-ERROR_HANDLER = 'Vank.core.handlers.exception.default_handler'
+ERROR_HANDLER = 'vank.core.handlers.exception:default_handler'
+
+# 处理静态文件(生产环境请设置为False)
+USE_STATIC = True
 
 # 静态文件URL
-STATIC_URL = '/static/'
+STATIC_URL = '/static'
 
 # 静态文件存放路径
 STATIC_PATH = PROJECT_BASE_DIR / 'statics'
 
+# 静态文件路由端点
+STATIC_ENDPOINT = 'static'
+
 # 热重载
 AUTO_RELOAD = True
 
 # 热重载检测间隔
 AUTO_RELOAD_INTERVAL = 1
 
 # 主机地址
@@ -71,15 +82,15 @@
 
 # lax strict none
 SESSION_COOKIE_SAME_SITE = 'lax'
 
 # SECURE
 SESSION_COOKIE_SECURE = False
 
-#域
+# 域
 SESSION_COOKIE_DOMAIN = None
 
 # 跨域允许的header
 CORS_ALLOWED_HEADERS = ["*"]
 
 # 跨域允许的method
 CORS_ALLOWED_METHODS = ["*"]
@@ -91,56 +102,55 @@
 WITH_CREDENTIALS = True
 
 # max-age
 CORS_MAX_AGE = 500
 
 """
 main_template = """
-from Vank.core.app import Application
-from Vank.core.http.response import Response
+from vank.core import Application, request, response
 
 app = Application()
 
 
 @app.new_route('/')
-def say_hi(request, *args, **kwargs):
-    return Response('Hi!')
+def say_hi(*args, **kwargs):
+    return response.ResponsePlain(f'Hi,your request path is {request.path}')
 
 
 if __name__ == '__main__':
     app.start()
 
 """
 
 init_templates = {
     'settings.py': settings_template,
     'main.py': main_template,
 }
 
 
 class Command(BaseCommand):
-    description = '通过init命令初始化项目'
+    description = 'Initialize the project through this command'
 
     def run(self, argv):
         options, args = self.parser.parse_known_args(argv[2:])
         project_name = options.name
         if project_name:
             project_dir = os.path.join(os.getcwd(), project_name)
             if os.path.exists(project_dir):
-                self.stderr.write(f'文件夹`{project_name}`已经存在、无法创建\n')
+                self.stderr.write(f'The folder "{project_name}" already exists and cannot be created\n')
                 sys.exit()
         else:
             project_dir = os.getcwd()
         os.makedirs(project_dir, exist_ok=True)
         variables = dict(
             secret=hashlib.sha256(str(time.time_ns()).encode()).hexdigest()
         )
         for file_name, template in init_templates.items():
             with open(os.path.join(project_dir, file_name), 'w', encoding='utf-8') as f:
-                f.write(template % variables)
+                f.write(template.lstrip() % variables)
 
     def init_arguments(self):
         self.parser.add_argument(
             '-n',
             '--name',
-            help='在新的目录下初始化项目'
+            help='Initialize the project in a new directory'
         )
```

### Comparing `Vank-1.0.1/Vank/cmds/subapp.py` & `vank-1.0.2/vank/cli/subapp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 # @FileName: subapp.py
 # @Date    : 2023/1/27-1:29
-# @Author  : Vank
-# @Project : Vank
+# @Author  : vank
+# @Project : vank
 import os
 import sys
 
-from Vank.utils.cmd import BaseCommand
+from vank.utils.cli import BaseCommand
 
 control_template = """"""
 views_template = """
-from Vank.core.app import SubApplication
+from vank.core import SubApplication, request, response
 
-{name}_sub = SubApplication('{name}')
+api_sub = SubApplication('api')
 
-# 在此编码
+# 在此编写你的视图
 
 """
 init_template = """"""
 subapp_files = {
     'control.py': control_template,
     'views.py': views_template,
     '__init__.py': init_template
 }
 
 
 class Command(BaseCommand):
-    description = '你可以通过此命令创建一个子应用'
+    description = 'You can create a sub application through this command'
 
     def run(self, argv):
         options, args = self.parser.parse_known_args(argv[2:])
         name = options.name
         dir_ = options.directory
         if not dir_:
             sub_app_dir = os.path.join(os.getcwd(), name)
         else:
             sub_app_dir = os.path.join(dir_, name)
         try:
             os.makedirs(sub_app_dir)
         except FileExistsError:
-            self.stderr.write(f'"{name}"子应用已存在,无法创建')
+            self.stderr.write(f'The "{name}" sub application already exists and cannot be created')
             sys.exit()
         for file_name, template in subapp_files.items():
             with open(os.path.join(sub_app_dir, file_name), 'w', encoding='utf-8') as f:
                 f.write(template.lstrip().format(name=name))
 
     def init_arguments(self):
         self.parser.add_argument(
             '-n',
             '--name',
-            help='子应用的名称',
+            help='Name of sub application',
             required=True
         )
         self.parser.add_argument(
             '-d',
             '--directory',
-            help='指定子应用所在的目录'
+            help='Specify the directory where the sub application is located'
         )
```

### Comparing `Vank-1.0.1/Vank/core/app.py` & `vank-1.0.2/vank/core/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,103 +1,107 @@
+import atexit
 import inspect
 import logging
-from typing import List, Optional, Union
-from Vank.core.config import conf
-from Vank.core.views.view import View
-from Vank.core.views.static.views import StaticView
-from Vank.utils import import_from_str
-from Vank.utils.log import setup_config as setup_log_config
-from Vank.core.routing.route import Route
-from Vank.core.routing.router import Router
-from Vank.core.exceptions import NonResponseException
-from Vank.core.handlers.exception import conv_exc_to_response
-from Vank.core.http import (request as req, response as rep)
-from Vank.utils.reloader import run_in_reloader
-from Vank.utils.signal import on_start_up, on_request_start, on_request_end
+import typing as t
+from vank.core.view import View
+from vank.core.config import conf
+from vank.utils import import_from_str
+from vank.__version__ import __version__
+from vank.core.routing.route import Route
+from vank.core.http.request import Request
+from vank.core.routing.router import Router
+from wsgiref.simple_server import make_server
+from vank.utils.reloader import run_in_reloader
+from vank.middleware.base import BaseMiddleware
+from vank.core.http.response import BaseResponse
+from vank.core.context import request, application
+from vank.core.exceptions import NoResponseException
+from vank.utils.log import setup_config as setup_log_config
+from vank.core.handlers.exception import conv_exc_to_response
+from vank.utils.signal import on_request_start, on_request_end, on_stop_down
 
-__version__ = '1.0.1'
 logger = logging.getLogger('console')
 
 
 class Base:
     def __init__(self):
         # 实例化路由映射表
         self.router = Router()
 
-    def __set_route(self, route_path, view_func, methods, **kwargs):
+    def _set_route(self, route_path, view_func, methods, **kwargs):
         """
         添加路由
         """
-        assert route_path.startswith('/'), f'{view_func} 视图的路由"{route_path}"应该以/开头'
+        assert route_path.startswith('/'), f'The route "{route_path}" of the {view_func!r} view should start with "/"'
         # 获取endpoint
-        endpoint = kwargs.pop('endpoint', None) or view_func.__name__
-        # 判断本实例是否为子应用,那么就应该加上子应用名字
-        if isinstance(self, SubApplication):
-            endpoint = f'{self.name}.{endpoint}'
+        endpoint = kwargs.pop('endpoint', None)
+        if not isinstance(endpoint, str) or not endpoint:
+            raise ValueError(f'Please provide an endpoint for %s' % view_func)
         # 实例化一个路由
         route = Route(route_path, methods, endpoint, **kwargs)
         # 添加到路由映射表中
         self.router.add_route(route_path, route, view_func)
 
-    def adapt_view_func(self, func_or_class, methods):
+    def adapt_view_func(self, func_or_class: t.Union[t.Callable, View], methods):
         # 利用inspect 检查是否为类或者函数
-        if inspect.isclass(func_or_class) and issubclass(func_or_class, View):
+        if inspect.isclass(func_or_class) and issubclass(func_or_class, View):  # noqa
             # 当视图为 View 视图的子类时 methods 应该为None
             if methods is not None:
-                raise ValueError(f'使用类视图 {func_or_class} 不应传入methods 参数')
+                raise ValueError(f'The methods parameter should not be passed in when using class view {func_or_class}')
             view = func_or_class()
             methods_list = view.get_view_methods
         elif inspect.isfunction(func_or_class):
             view = func_or_class
             methods_list = methods
         else:
-            raise ValueError(f'视图应该为一个函数或View的子类 而不是{func_or_class}')
+            raise ValueError(
+                f'View-function should be a function or subclass of "View" instead of {type(func_or_class).__name__}')
 
         return view, methods_list
 
-    def new_route(self, route_path: str, methods=None, **kwargs):
-        def decorator(func_or_class):
+    def new_route(self, route_path: str, methods: t.Optional[t.Sequence] = None, **kwargs):
+        def decorator(func_or_class: t.Union[t.Callable, View]):
             view, methods_list = self.adapt_view_func(func_or_class, methods)
             # 调用set_route方法
-            self.__set_route(route_path, view, methods_list, **kwargs)
+            self._set_route(route_path, view, methods_list, **kwargs)
             return func_or_class
 
         return decorator
 
-    def get(self, route_path, **kwargs):
+    def get(self, route_path: str, **kwargs):
         """
         注册视图允许的请求方法仅为get的快捷方式
         """
         return self.new_route(route_path, ['GET'], **kwargs)
 
-    def post(self, route_path, **kwargs):
+    def post(self, route_path: str, **kwargs):
         """
         注册视图允许的请求方法仅为post的快捷方式
         """
         return self.new_route(route_path, ['POST'], **kwargs)
 
-    def put(self, route_path, **kwargs):
+    def put(self, route_path: str, **kwargs):
         """
         注册视图允许的请求方法仅为put的快捷方式
         """
         return self.new_route(route_path, ['PUT'], **kwargs)
 
-    def patch(self, route_path, **kwargs):
+    def patch(self, route_path: str, **kwargs):
         """
         注册视图允许的请求方法仅为patch的快捷方式
         """
         return self.new_route(route_path, ['PATCH'], **kwargs)
 
-    def delete(self, route_path, **kwargs):
+    def delete(self, route_path: str, **kwargs):
         """
         注册视图允许的请求方法仅为delete的快捷方式
         """
         return self.new_route(route_path, ['DELETE'], **kwargs)
 
-    def add_route(self, route_path: str, func_or_class, methods=None, **kwargs):
+    def add_route(self, route_path: str, func_or_class: t.Union[t.Callable, View], methods=None, **kwargs):
         self.new_route(route_path, methods, **kwargs)(func_or_class)
         return self
 
 
 class Application(Base):
     def __init__(self):
         super(Application, self).__init__()
@@ -110,173 +114,196 @@
         # 子应用列表
         self.sub_applications = {}
         self._setup()
 
     def _setup(self):
         # 配置logging
         setup_log_config(conf.LOGGING)
-        self.new_route(conf.STATIC_URL + '<path:fp>', endpoint='statics')(StaticView)
+        for sub_application in conf.SUB_APPLICATIONS:
+            self.include(sub_application)
         # 初始化中间件
-        self.initial_middleware_stack()
+        self.initialize_middleware_stack()
+        # 将on_stop_down信号的emit方法注册到atexit中
+        atexit.register(on_stop_down.emit, sender=self)
 
-    def initial_middleware_stack(self):
+    def initialize_middleware_stack(self):
         """
         初始化中间件 接收到的请求将会传入self.middlewares进行处理
         当配置文件中没有中间件时 self.middlewares 为 conv_exc_to_response
         :return:
         """
         # 将实例方法 get_response 包裹在全局异常处理转换器中
         get_response_func = conv_exc_to_response(self.__get_response, self.error_handler)
 
         for m_str in reversed(conf.MIDDLEWARES):
             # 导入中间件类
             middleware_class = import_from_str(m_str)
+            if not issubclass(middleware_class, BaseMiddleware):
+                raise ValueError(f'"%s" Should be a subclass of "BaseMiddleware" instead of %s' % (
+                    m_str,
+                    type(middleware_class).__name__
+                ))
             # 实例化中间件 将handler传入其中
             middleware_instance = middleware_class(get_response_func)
-
-            if not middleware_instance:
-                raise RuntimeError(f'初始化中间件错误,{middleware_instance} 中间件不应该为空')
-
             # 如果该中间件有handle_view方法 那么就添加到__handle_view_middlewares中
             if hasattr(middleware_instance, 'handle_view'):
                 self.__handle_view_middlewares.insert(0, middleware_instance.handle_view)
             # 将中间件包裹在全局异常处理转换器中
             get_response_func = conv_exc_to_response(middleware_instance, self.error_handler)
-
-        # 形成一个中间件栈
         self.entry_func = get_response_func
 
-    def __get_response(self, request, *args, **kwargs):
+    def __get_response(self, *args, **kwargs):
         """
         获取response  如果任意一个中间件定义了 handle_view方法  该方法会调用调用handle_view
         如果 所有的handle_view返回值都是None 那么 请求会进入 对应的视图函数
 
         当 视图函数返回一个非 BaseResponse 或 BaseResponse子类实例时
         raise NonResponseException
 
         :param request:
         :return:
         """
         response = None
-        # 获取到对应的处理试图和该试图所需的参数
-        view_func, view_kwargs = self.__dispatch_route(request)
+        # 获取到对应的处理视图和该视图所需的参数
+        view_func, view_kwargs = self.__dispatch_route()
         view_kwargs.update(kwargs)
         handle_view_middlewares = self.__handle_view_middlewares.copy()
         # 执行handle_view
         for view_handler in handle_view_middlewares:
-            response = view_handler(request, view_func, **view_kwargs)
+            response = view_handler(view_func, **view_kwargs)
             if response:
                 break
 
         # 如果handle_view 没有返回response 那么就交给视图函数处理
         if not response:
-            response = view_func(request, **view_kwargs)
+            response = view_func(**view_kwargs)
         # 当视图返回的不是BaseResponse 或 BaseResponse子类的实例 raise NonResponseException
-        if not isinstance(response, rep.BaseResponse):
-            raise NonResponseException("服务未返回响应")
+        if not isinstance(response, BaseResponse):
+            raise NoResponseException(f'The view "%s" did not return a response' % view_func)
 
         return response
 
     def start(self):
         """
         开启服务
         :return: None
         """
-        assert self.router.endpoint_func_dic, '未能找到至少一个以上的视图处理请求'
-        # 开启服务信号
-        on_start_up.emit(self)
         # 判断是否使用热重载
         if conf.AUTO_RELOAD:
             run_in_reloader(
                 self._inner_run,
                 conf.AUTO_RELOAD_INTERVAL,
             )
         else:
             self._inner_run()
 
     def _inner_run(self):
-        from wsgiref.simple_server import make_server
         logger.warning(
-            f"你的服务运行于:http://{conf.DEFAULT_HOST}:{conf.DEFAULT_PORT}/\n"
-            f"- 请勿用于生产环境\n"
-            f"- 版本号:{__version__}\n"
+            f"Your service is running on:http://{conf.DEFAULT_HOST}:{conf.DEFAULT_PORT}/\n"
+            f"- Do not use in production environment\n"
+            f"- Version number:{__version__}\n"
         )
         httpd = make_server(conf.DEFAULT_HOST, conf.DEFAULT_PORT, self)
         httpd.serve_forever()
 
-    def include(self, sub: Union[str, "SubApplication"]):
+    def include(self, sub: t.Union[str, "SubApplication"]):
         """
         将子应用挂载到Application中,类似Flask的register_blueprint
         """
         if isinstance(sub, str):
             sub = import_from_str(sub)
         if not isinstance(sub, SubApplication):
-            raise TypeError(f"参数 sub类型不应该为{type(sub)}")
+            raise TypeError(f'The type of parameter "sub" should be "SubApplication" instead of {type(sub)}')
         if sub.name in self.sub_applications.keys():
-            raise ValueError(f'挂载子应用失败 {sub}:不能出现重复的子应用名称 <{sub.name}>')
+            raise ValueError(f'Failed to include "%s": Cannot have duplicate sub application names "%s"' % (
+                sub,
+                sub.name
+            ))
 
         self.router.include_router(sub.router)  # 将子应用的路由包含到主路由中
         sub.root = self  # 对子应用进行绑定
         self.sub_applications[sub.name] = sub
 
-    def __dispatch_route(self, request):
+    def __dispatch_route(self):
         """
         根据请求信息找到处理该url的视图函数
-        :param request:封装的request请求实例 详情请看Vank/core/http/request
         :return:一个视图函数
         """
-        view_function, view_kwargs = self.router.match(request)
+        view_function, view_kwargs = self.router.match()
         return view_function, view_kwargs
 
-    def _finish_response(self, response, start_response) -> List[bytes]:
+    def _finish_response(self, response: BaseResponse, start_response: callable) -> t.Iterable[bytes]:
         """
         处理response 调用start_response设置响应状态码和响应头
-        并返回一个二进制可迭代对象
         :param response: 封装的response 详情请看Vank/core/http/response
         :param start_response: WSGI规范的start_response
-        :return: list[bytes] 返回的body数据
+        :return: Iterable[bytes] 返回的body数据
         """
-        start_response(response.status, list(response.headers.items()))
+        # 默认的output的header参数是”Set-Cookie:“
+        # 我们只需要后面的值而不需要”Set-Cookie:“
+        # 所以应该将header行参设置为空
+        headers = response.headers.items()
+        # 设置cookie
+        headers.extend([("Set-Cookie", cookie.output(header="")) for cookie in response.cookies.values()])
+        start_response(response.status, headers)
         return response
 
-    def __call__(self, environ, start_response) -> List[bytes]:
+    def __call__(self, environ: dict, start_response: callable) -> t.Iterable[bytes]:
         """
         被WSGI Server调用
         :param environ:环境变量以及请求参数等
         :param start_response:WSGI规范的一个function 我们需要给他设置响应码以及响应头等信息
         :return:作为响应数据
         """
-        request = req.Request(environ)
+        app_token = application._wrapped.set(self)  # noqa
+        request_token = request._wrapped.set(Request(environ))  # noqa
         # 请求开始信号
-        on_request_start.emit(self, request=request)
-        response = self.entry_func(request)
+        on_request_start.emit(self)
+        response = self.entry_func()
         # 请求结束信号
-        on_request_end.emit(self, request=request, response=response)
+        on_request_end.emit(self, response=response)
         # 关闭request的资源
         request.close()
-
+        request._wrapped.reset(request_token)  # noqa
+        application._wrapped.reset(app_token)  # noqa
         return self._finish_response(response, start_response)
 
-    def url_for(self, endpoint, **kwargs):
-        return self.router.url_for(endpoint, **kwargs)
+    def url_reflect(self, endpoint: str, **kwargs):
+        return self.router.url_reflect(endpoint, **kwargs)
+
+    def _set_route(self, route_path, view_func, methods, **kwargs):
+        endpoint = kwargs.pop("endpoint", None)
+        if endpoint is None:
+            endpoint = view_func.__name__
+        kwargs["endpoint"] = endpoint
+        return super()._set_route(route_path, view_func, methods, **kwargs)
 
 
 class SubApplication(Base):
-    def __init__(self, name, prefix: Optional[str] = None):
+    def __init__(self, name: str, prefix: t.Optional[str] = None):
         super(SubApplication, self).__init__()
         self.name = name
         self.prefix = prefix
         if self.prefix:
-            assert not self.prefix.endswith('/'), "url前缀不应以 '/'结尾"
-            assert self.prefix.startswith('/'), "url前缀应以 '/'开头"
-        self.root: "Application" = None
+            assert not self.prefix.endswith('/'), 'The Route prefix should not end with "/"'
+            assert self.prefix.startswith('/'), 'The Route prefix should start with "/"'
+        self.root: t.Optional[Application] = None
+
+    def _set_route(self, route_path: str, view_func: t.Callable, methods: t.Sequence, **kwargs):
+        endpoint = kwargs.pop("endpoint", None)
+        if endpoint is None:
+            endpoint = f"{self.name}.{view_func.__name__}"
+        kwargs["endpoint"] = endpoint
+        return super()._set_route(route_path, view_func, methods, **kwargs)
 
-    def new_route(self, route_path: str, methods=None, **kwargs):
+    def new_route(self, route_path: str, methods: t.Optional[t.Sequence] = None, **kwargs):
         if self.prefix:
-            assert route_path.startswith("/"), f'子应用{self.name}视图的路由"{route_path}"应该以/开头'
+            assert route_path.startswith("/"), f'The route "{route_path}" of the sub application "{self.name}"' \
+                                               f' should start with "/"'
             route_path = self.prefix + route_path
         return super(SubApplication, self).new_route(route_path, methods, **kwargs)
 
-    def url_for(self, endpoint, **kwargs):
+    def url_reflect(self, endpoint: str, **kwargs):
         if not isinstance(self.root, Application):
-            raise TypeError(f'url_for失败,root的类型应为{type(Application).__name__} 你忘记挂载了吗?')
-        return self.root.url_for(endpoint, **kwargs)
+            raise TypeError(f'The type of root should be {type(Application).__name__}.'
+                            f' Did you forget to be included to Application?')
+        return self.root.url_reflect(endpoint, **kwargs)
```

### Comparing `Vank-1.0.1/Vank/core/config/__init__.py` & `vank-1.0.2/vank/core/config/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from importlib import import_module
-from Vank.utils.signal import configs_check
-from Vank.core.config import base
+from vank.utils.signal import configs_check
+from vank.core.config import base
 
 for item in dir(base):
     if not item.startswith('check_'):
         continue
     f = getattr(base, item)
     if not callable(f):
         continue
@@ -15,17 +15,17 @@
 class Settings(base.BaseSettings):
     def __init__(self):
         module = os.environ.get('PROJECT_SETTING', None)
         try:
             self.module = import_module(module)
         except:
             raise ModuleNotFoundError(
-                f"\n运行失败,未能找到配置模块的路径环境变量(PROJECT_SETTING)\n"
-                f"当前配置路径:PROJECT_SETTING='{module}'\n"
-                f"请像下面这样添加配置模块的路径:\n"
+                f"\nFailed, unable to find path environment variable for configuration module (PROJECT SETTING)\n"
+                f"Current configuration module path:PROJECT_SETTING='{module!r}'\n"
+                f"Please add the correct path for the configuration module as follows:\n"
                 f"import os\n"
                 f"os.environ['PROJECT_SETTING']='your setting module path'"
             )
         for setting_name in dir(self.module):
             if not setting_name.isupper():
                 continue
             setattr(self, setting_name, getattr(self.module, setting_name))
```

### Comparing `Vank-1.0.1/Vank/core/exceptions.py` & `vank-1.0.2/vank/core/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # @filename: exceptions.py
 # @Time:    2022/7/26-1:40
-# @Author:  Vank
-from Vank.core.http import status
+# @Author:  vank
 
-
-class UrlForNotFound(Exception):
+class ReflectNotFound(Exception):
     def __init__(self, endpoint, **arguments):
-        super(UrlForNotFound, self).__init__(f'url_for未找到对应的路径 <{endpoint}><==>{"".join(arguments.keys())}')
+        super(ReflectNotFound, self).__init__(f'URL reflect did not find the corresponding path'
+                                              f' <{endpoint}><==>{"".join(arguments.keys())}')
 
 
 class NotFoundException(Exception):
     """资源未找到错误"""
 
 
 class MethodNotAllowedException(Exception):
-    def __init__(self, msg, allow, *args, **kwargs):
+    def __init__(self, msg, allow, *args):
         self.allow = allow
-        super(MethodNotAllowedException, self).__init__(msg, *args, **kwargs)
+        super(MethodNotAllowedException, self).__init__(msg, *args)
 
     """请求方法不允许错误"""
 
 
 class PermissionDeniedException(Exception):
     """权限错误"""
 
 
-class NonResponseException(Exception):
+class NoResponseException(Exception):
     """视图未返回Response"""
 
 
 class NoneViewMethodException(Exception):
     """类视图未定义至少一个类方法"""
```

### Comparing `Vank-1.0.1/Vank/core/handlers/exception.py` & `vank-1.0.2/vank/core/handlers/exception.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,40 @@
-from Vank.core.http import HTTP_Status
-from Vank.core.http import response
-from Vank.core.exceptions import *
-from Vank.utils.exception import get_exception_reason
+from vank.core.http import response
+from vank.core.exceptions import *
 from logging import getLogger
 
-logger = getLogger()
+logger = getLogger('server')
 
 
 def conv_exc_to_response(get_response_func, error_handler):
     """
     全局的捕获异常,将异常转换为对应的response
     :param get_response_func: 获取reponse的函数 当存在中间件时 该参数为上一个中间件 不存在时 为 APP实例下的__get_response方法
     :param error_handler: 处理错误的处理器
     :return:
     """
 
-    def inner(request, *args, **kwargs):
+    def inner(*args, **kwargs):
         try:
-            return get_response_func(request, *args, **kwargs)
+            return get_response_func(*args, **kwargs)
         except Exception as e:
-            return error_handler(request, e)
+            return error_handler(e)
 
     return inner
 
 
-def default_handler(request, exc):
+def default_handler(exc):
     """
     错误处理器 根据对应的错误返回对应的Response 如果未找到对应错误 默认返回 Response 500
-    :param request: request对象
     :param exc: Exception对象
     :return: Response
     """
-    logger.error("", exc_info=exc)
     if isinstance(exc, NotFoundException):
-        return response.Response404()
-
-    if isinstance(exc, MethodNotAllowedException):
-        return response.Response405(exc.allow)
-
-    if isinstance(exc, PermissionDeniedException):
-        return response.Response403()
-
-    return response.Response500()
+        resp = response.Response404()
+    elif isinstance(exc, MethodNotAllowedException):
+        resp = response.Response405(exc.allow)
+    elif isinstance(exc, PermissionDeniedException):
+        resp = response.Response403()
+    else:
+        resp = response.Response500()
+    logger.error("Error - ", exc_info=exc)
+    return resp
```

### Comparing `Vank-1.0.1/Vank/core/http/response.py` & `vank-1.0.2/vank/core/http/response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import os
 import re
 import json
+import typing as t
 from urllib.parse import quote
 from mimetypes import guess_type
+from vank.core.config import conf
 from email.utils import formatdate
 from http.cookies import SimpleCookie
-from typing import Union, Optional, Any
-from Vank.core.config import conf
-from Vank.core.http import http_status_dict
-from Vank.utils.datastructures import Headers
+from vank.core.http import http_status_dict
+from vank.utils.datastructures import Headers
 
 
 class BaseResponse:
     default_status = 200
     media_type = 'text/plain'
 
     def __init__(self,
-                 content: Optional[Union[bytes, str]] = b"",
-                 status: Optional[int] = None,
-                 headers=None,
-                 *args,
-                 **kwargs):
+                 content: t.Optional[t.Union[bytes, str]] = b"",
+                 status: t.Optional[int] = None,
+                 headers: t.Optional[t.Union[dict, Headers]] = None,
+                 media_type: str = None,
+                 ):
         # 判断status是否传入  如果没有传入那么就设置未默认的status
         self._status = status or self.default_status
         self._charset = None
         self._content = content or b""
         self._body = None
         self._raw_headers = headers
         self._headers = None
         self._cookies = None
+        self.media_type = media_type or self.media_type
 
     @property
     def body(self):
         if getattr(self, '_body') is None:
             if isinstance(self._content, bytes):
                 self._body = self._content
             else:
@@ -48,20 +49,20 @@
                 self._headers = self._raw_headers
             else:
                 self._headers = Headers(self._raw_headers)
             # 设置Content-Type
             if 'Content-Type' not in self._headers:
                 content_type = self.media_type
                 if content_type.startswith('text/') and 'charset' not in content_type:
-                    content_type += f'; charset={self.charset}'
-                self._headers.setdefault('Content-Type', content_type)
+                    content_type = f'{content_type}; charset={self.charset}'
+                self._headers.add('Content-Type', content_type)
             # 设置content-length
             if 'Content-Length' not in self._headers:
                 if self.body and self._status >= 200 and self._status not in (204, 304):
-                    self._headers.setdefault('Content-Type', str(len(self.body)))
+                    self._headers.setdefault('Content-Length', str(len(self.body)))
         return self._headers
 
     @property
     def charset(self):
         if getattr(self, '_charset') is None:
             pattern = re.compile(r';\s*charset=(?P<charset>[^\s;]+)', re.I)
             res = pattern.search(self.headers.get('Content-Type', ''))
@@ -76,22 +77,22 @@
         return f"{self._status} {http_status_dict.get(self._status, 'Unknow Status Code')}"
 
     def __iter__(self):
         yield from [self.body]
 
     def add_cookie(self,
                    key: str,
-                   value: str = "",
-                   max_age=None,
-                   expires=None,
-                   path: str = "/",
-                   domain=None,
-                   secure=False,
-                   httponly=False,
-                   same_site=None
+                   value: t.Optional[str] = "",
+                   max_age: t.Optional[t.Union[int, str]] = None,
+                   expires: t.Optional[t.Union[int, str]] = None,
+                   path: t.Optional[str] = "/",
+                   domain: t.Optional[str] = None,
+                   secure: t.Optional[bool] = False,
+                   httponly: t.Optional[bool] = False,
+                   same_site: t.Optional[str] = None
                    ):
         # 当max_age 和expires同时提供时 绝大多数浏览器除了IE会将expires忽略
         # 换而言之就是expires会失效
         self.cookies[key] = value
         cookie = self.cookies[key]
         if max_age:
             cookie['max-age'] = max_age
@@ -102,28 +103,25 @@
         if domain:
             cookie['domain'] = domain
         if secure:
             cookie['secure'] = True
         if httponly:
             cookie['httponly'] = True
         if same_site:
-            assert same_site in ["lax", "none", "strict"], 'same_site的值必须为 "lax", "none", "strict"'
+            assert same_site in ["lax", "none", "strict"], \
+                'The value of same_site must be one of "lax", "none", or "strict"'
             cookie['samesite'] = same_site
-        # 默认的output的header参数是”Set-Cookie:“
-        # 我们只需要后面的值而不需要”Set-Cookie:“
-        # 所以应该将header设置为空
-        self.headers.add('Set-Cookie', cookie.output(header=""))
 
     def delete_cookie(self,
                       key: str,
-                      path: str = "/",
-                      domain=None,
-                      secure: bool = False,
-                      httponly: bool = False,
-                      same_site=None):
+                      path: t.Optional[str] = "/",
+                      domain: t.Optional[str] = None,
+                      secure: t.Optional[bool] = False,
+                      httponly: t.Optional[bool] = False,
+                      same_site: t.Optional[str] = None):
         self.add_cookie(
             key,
             max_age=0,
             expires="Thu, 01 Jan 1970 00:00:00 GMT",  # 设置此值可以将cookie删除
             path=path,
             domain=domain,
             secure=secure,
@@ -134,30 +132,30 @@
     @property
     def cookies(self):
         if getattr(self, '_cookies') is None:
             self._cookies = SimpleCookie()
         return self._cookies
 
 
-class Response(BaseResponse):
+class ResponsePlain(BaseResponse):
     def __init__(self,
-                 content: Optional[Union[bytes, str]] = b"",
+                 content: t.Optional[t.Union[bytes, str]] = b"",
                  status=200,
                  headers=None,
                  *args,
                  **kwargs):
         """
         普通响应
         :param data:响应数据
         :param status:状态码
         :param headers:响应头
         :param args:
         :param kwargs:
         """
-        super(Response, self).__init__(content, status, headers=headers, *args, **kwargs)
+        super(ResponsePlain, self).__init__(content, status, headers=headers, *args, **kwargs)
 
 
 class Response404(BaseResponse):
     """
     资源未找到 404
     """
     default_status = 404
@@ -218,28 +216,28 @@
     """
     将文件根据chunk_size以块的方式读入到内存当中,
     """
     chunk_size = 2048
     media_type = 'application/octet-stream'
 
     def __init__(self, filepath: str, filename=None, as_attachment=True, media_type=None, *args, **kwargs):
-        assert not kwargs.get('content', None), 'ResponseFile不应该有content'
+        assert not kwargs.get('content', None), 'This response should not have the "content" parameter'
         self.as_attachment = as_attachment
         self.filepath = os.path.abspath(filepath)
         self.filename = filename
         self.user_media_type = media_type
         super(ResponseFile, self).__init__(*args, **kwargs)
         self.update_headers()
 
     def update_headers(self):
         # 判断文件是否存在 如果不存在那么raise FileNotFoundError
         if not os.path.exists(self.filepath):
-            raise FileNotFoundError(f'{self.filepath}文件不存在')
+            raise FileNotFoundError(f'"{self.filepath}"File does not exist')
         if not os.path.isfile(self.filepath):
-            raise TypeError(f'{self.filepath}不是文件')
+            raise TypeError(f'"{self.filepath}"This is not a file')
         # 获取文件的统计信息
         stat = os.stat(self.filepath)
         # 根据统计信息的st_size 可以获取到文件的长度
         content_length = stat.st_size
         # 获取最后修改时间
         last_modified = formatdate(stat.st_mtime, usegmt=True)
         if self.filename:
@@ -286,16 +284,20 @@
 
         self.headers.update('Location', quote(url, safe="/#%[]=:;$&()+,!?*@'~"))
 
 
 class ResponseJson(BaseResponse):
     media_type = f'application/json'
 
-    def __init__(self, content: Any, *args, **kwargs):
+    def __init__(self, content: t.Any, *args, **kwargs):
         content = json.dumps(
             content,
             allow_nan=False,
             indent=None,
             separators=(",", ":"),  # 获得最紧凑的json
         )
 
         super(ResponseJson, self).__init__(content, *args, **kwargs)
+
+
+class ResponseHtml(BaseResponse):
+    media_type = "text/html"
```

### Comparing `Vank-1.0.1/Vank/core/http/status.py` & `vank-1.0.2/vank/core/http/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import IntEnum
 
 
-class HTTP_Status(IntEnum):
+class HttpStatus(IntEnum):
     HTTP_100_CONTINUE = 100, 'Continue'
     HTTP_101_SWITCHING_PROTOCOLS = 101, 'Switching Protocols'
     HTTP_102_PROCESSING = 102, 'Processing'
     HTTP_103_EARLY_HINTS = 103, 'Early Hints'
 
     # success
     HTTP_200_OK = 200, 'OK'
@@ -80,8 +80,8 @@
     def __new__(cls, code, phrase):
         obj = int.__new__(cls, code)
         obj._value_ = code
         obj.phrase = phrase
         return obj
 
 
-http_status_dict = {item: item.phrase for item in HTTP_Status.__members__.values()}
+http_status_dict = {item: item.phrase for item in HttpStatus.__members__.values()}
```

### Comparing `Vank-1.0.1/Vank/core/routing/converters.py` & `vank-1.0.2/vank/core/routing/converters.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class BasicConverter(metaclass=ABCMeta):
     regex = None
     name = ""
 
     def __init__(self):
-        assert self.name, "必须为子类转换器配置名字 -->name"
+        assert self.name, "You must configure a name for the route converter"
 
     @abstractmethod
     def convert_to_python(self, value):
         """
         将 value 转换为python Object 此方法应由子类完成
         :param value: 需要被转换为Python Object的值
         :return:
```

### Comparing `Vank-1.0.1/Vank/core/routing/route.py` & `vank-1.0.2/vank/core/routing/route.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,134 +1,116 @@
 # @filename: route.py
 # @Time:    2022/7/26-0:33
-# @Author:  Vank
+# @Author:  vank
 import re
+import inspect
 from urllib.parse import quote
-from Vank.core.config import conf
-from importlib import import_module
-from Vank.core import exceptions
+from functools import lru_cache
+from vank.core import exceptions
+from vank.core.config import conf
+from vank.utils.load_module import import_from_str
+
+# 构建路由正则
+build_route_regex_pattern = re.compile(
+    "(?P<static_route>[^{]*){(?P<variable>[a-zA-Z_][a-zA-Z0-9_]*):(?P<converter>[a-zA-Z_][a-zA-Z0-9_]*)}"
+)
+
+
+def parse_route_rule(rule):
+    start = 0
+    end = len(rule)
+    while start < end:
+        # 通过语法正则匹配出动态路由
+        res = build_route_regex_pattern.search(rule, start)
+        # 如果没有匹配出结果、说明剩余的字符串是静态的
+        if not res:
+            break
+        result_dict = res.groupdict()
+        static_route = result_dict.get("static_route")
+        variable = result_dict.get("variable")
+        converter = result_dict.get("converter")
+        if result_dict.get("static_route"):
+            yield None, static_route
+        yield converter, variable
+        start = res.end()
+    # 拼接剩余静态路由
+    if start < end:
+        legacy_route = rule[start:]
+        if '{' in legacy_route or '}' in legacy_route:
+            raise SyntaxError('Incorrect routing syntax.Should not appear single "{" or "}"')
+        yield None, legacy_route
+
+
+@lru_cache(maxsize=None)
+def get_converters():
+    """
+    获取路由转换器
+    """
+    convert_dict = dict()
+    for converter_name, convert_module_path in conf.ROUTE_CONVERTERS.items():
+        if converter_name in convert_dict.keys():
+            raise ValueError(f'The converter name "{converter_name}" cannot be duplicate')
+        converter_class = import_from_str(convert_module_path)
+        convert_dict[converter_name] = converter_class()
+    return convert_dict
 
 
 class BaseRoute:
     def __init__(self, route_path: str, methods: list, endpoint: str, *args, **kwargs):
-        self.route_pattern = None
-        self.route_path = route_path
-        self.methods = self.__parse_methods(methods)
-        self.endpoint = endpoint
+        self.route_pattern = None  # 解析后的路由规则
+        self.route_path = route_path  # 用户定义的路由规则
+        self.methods = self.__parse_methods(methods)  # 路由的method
+        self.endpoint = endpoint  # 端点
         self.regex_list = []
-        # 源自于werkzug.routing
-        self.rule_regex_pattern = re.compile(r"""
-            (?P<static_route>[^<]*)                           # 静态的路由 比如/123/<int:id> 那么 /123/就为静态路由
-            <
-            (?:
-                (?P<converter_name>[a-zA-Z_][a-zA-Z0-9_]*)   # 转换器名字
-                (?:\((?P<conv_args>.*?)\))?                  # 转换器参数
-                \:                                      # 分隔符 :
-            )?
-            (?P<variable>[a-zA-Z_][a-zA-Z0-9_]*)        # 变量名字
-            >
-            """, re.VERBOSE)
         # 转换器类型
-        self.converters = self.__load_converters()
+        self.converters = get_converters()
         # 参数所对应的转换器
         self.argument_converters = {}
         # 构建正则
-        self.build_rule_regex()
-
-    def __load_converters(self):
-        """
-        从setting加载转换器
-        """
-        convters_tmp = {}
-        for converter_name, converter_path in conf.ROUTE_CONVERTERS.items():
-            module, cls_name = converter_path.rsplit('.', maxsplit=1)
-            if converter_name in convters_tmp.keys():
-                raise ValueError(f'转换器名字不能重复:{converter_name},请修改')
-            convters_tmp[converter_name] = getattr(import_module(module), cls_name)()
-
-        return convters_tmp
+        self.setup()
 
     def __parse_methods(self, methods: list):
         if not methods:
             return ["GET", "POST", "PUT", "PATCH", "DELETE", "HEAD", "OPTIONS", "TRACE"]
         methods_upper = [method.upper() for method in methods]
         if not set(methods_upper) < {"GET", "POST", "PUT", "PATCH", "DELETE", "HEAD", "OPTIONS", "TRACE"}:
-            raise ValueError(f'{self.endpoint}定义路由请求方法时出错,存在非HTTP请求方法')
+            raise ValueError(f'"{self.endpoint}"Binding failed, there are non HTTP request methods present')
         return methods_upper
 
     def __get_converter_list(self):
         """
         获取所有转换器的列表
         """
         return self.converters.keys()
 
-    def __parse_rule(self, path):
-        """
-        解析路由规则,通过regex将路由规则中的静态规则和变量规则提取出来
-        :return:
-        """
-
-        if not path:
-            yield None, None, None
-            return
-
-        variable_names = set()
-        position = 0
-        end = len(path)
-        count = 0
-        while position < end:
-            res = self.rule_regex_pattern.match(path, position)
-            if not res:
-                break
-            data_dic = res.groupdict()
-            static_route = data_dic['static_route']
-            if static_route:
-                yield None, None, static_route
-            variable_name = data_dic['variable']
-            converter = data_dic['converter_name']
-            conv_args = data_dic['conv_args']
-            if not converter and variable_name:
-                raise SyntaxError(f'endpoint:[{self.endpoint}]的路由参数有误:{variable_name}必须指定类型'
-                                  f' <{"/".join(self.__get_converter_list())}:variable_name>')
-
-            if variable_name in variable_names:
-                raise LookupError(f'路由:{path}变量名:{variable_name}只能使用一次')
-            variable_names.add(variable_name)
-            yield converter, conv_args or None, variable_name
-            position = res.end()
-        if position < end:
-            other = path[position:]
-            if ">" in other or "<" in other:
-                raise SyntaxError(f"{self.endpoint}存在错误的路由:{path} 不应存在:{other}")
-            yield None, None, other
-
-    def build_rule_regex(self):
+    def setup(self):
         """
         创建一条属于这条路由的正则
         :return:
         """
-        for converter_name, conv_args, virable_name in self.__parse_rule(self.route_path):
-            if not converter_name:
-                if virable_name:
-                    self.regex_list.append(virable_name)
+        for converter_name, static_or_variable in parse_route_rule(self.route_path):
+            # 没有路由转换器,但是static_or_variable不为空、则可以判定static_or_variable为静态的路由
+            if not converter_name and static_or_variable:
+                # 需要将静态路径escape防止出现安全问题
+                # 例如 '/foo.bar' 如果直接append那么如果访问/fooobar也是能够访问到此条路由，这是不合法的
+                self.regex_list.append(re.escape(static_or_variable))
                 continue
-            converter = self.converters.get(converter_name)
-            if not converter:
-                raise LookupError(
-                    f'{self.endpoint}的变量类型[{converter_name}]无法解析,'
-                    f'目前支持的类型为{"/".join(self.__get_converter_list())}')
+            # ===处理动态路由===
+            if static_or_variable in self.argument_converters.keys():
+                raise SyntaxError('Duplicate keyword parameters cannot appear in route path')
+            converter = self.converters.get(converter_name, None)
+            if converter is None:
+                raise SyntaxError(f'{converter_name} Converter does not exist.')
             # 将变量名对应的转换器添加到字典中,在路由过来的时候以便转换为相应的类型
-            self.argument_converters.update({virable_name: converter})
-            self.regex_list.append(f"(?P<{virable_name}>{converter.regex})")
-
+            self.argument_converters.update({static_or_variable: converter})
+            self.regex_list.append(f"(?P<{static_or_variable}>{converter.regex})")
+        # 开始拼接解析后的路由规则
         regex = f"^{''.join(self.regex_list)}$"
 
         self.route_pattern = re.compile(regex)
-        # print(self.route_pattern)
-        # print(self.endpoint)
 
     def convert_arguments(self, **arguments):
         """
         将变量转换为对应的类型
         例如:将整数字符串转换为int类型
         """
         for arg_name, arg_value in arguments.items():
@@ -140,39 +122,45 @@
 class Route(BaseRoute):
     def __init__(self, route_path, methods, endpoint, *args, **kwargs):
         super(Route, self).__init__(route_path, methods, endpoint, *args, **kwargs)
 
     def check_method(self, request_method):
         return request_method.upper() in self.methods
 
-    def url_for(self, endpoint: str, **arguments):
-        # 根据endpoint名字反向转换为url 如果有其他关键字参数那么会将它们转换为查询参数
-        if not endpoint == self.endpoint or not set(arguments.keys()).issuperset(set(self.argument_converters.keys())):
-            raise exceptions.UrlForNotFound(endpoint, **arguments)
-        route_path = self.route_path
-        # 将参数转换为url
-        # /<int:hello> ==>url_for(xxx,hello=1)==>/1
-        for key, converter in self.argument_converters.keys():
-            value = converter.convert_to_url(arguments.pop(key))
-            route_path = route_path.replace(f'<{converter.name}:{key}>', value)
-        # 处理剩余的关键字参数
+    def url_reflect(self, endpoint: str, **arguments):
+        """
+        根据endpoint查找对应的url
+        """
+        # 根据endpoint反向构建url、并且传入的arguments必须为该路由所需的可变路由参数的超集
+        if not endpoint == self.endpoint or not set(arguments.keys()).issuperset(self.argument_converters.keys()):
+            raise exceptions.ReflectNotFound(endpoint, **arguments)
+        url = self.route_path
+        # 将传入的arguments替换为url、甚于的参数作为查询参数
+        for variable_name, converter in self.argument_converters.items():
+            value = converter.convert_to_url(arguments.pop(variable_name))
+            raw_rule = '{%(variable_name)s:%(converter_name)s}' % dict(
+                variable_name=variable_name,
+                converter_name=converter.name
+            )
+            url = url.replace(raw_rule, value)
         query_args = "&".join([f"{key}={value}" for key, value in arguments.items()])
-        # 如果有查询参数那么进行拼接
         if query_args:
-            route_path = route_path + f"?{query_args}"
+            url = url + f"?{query_args}"
         # 为了解决URL规范问题需要对route_path进行quote
         # safe参数指的是不对safe的值进行转换
-        return quote(route_path, safe="/#%[]=:;$&()+,!?*@'~")
+        return quote(url, safe="/#%[]=:;$&()+,!?*@'~")
 
     def __str__(self):
-        return '<{cls_name}>:{regex} <==> {endpoint}'.format(
+        return '<{cls_name}>:"{route_path}" <==> "{endpoint}"'.format(
+            route_path=self.route_path,
             cls_name=self.__class__.__name__,
             regex=self.route_pattern,
             endpoint=self.endpoint
         )
 
     def __repr__(self):
-        return '<{cls_name}>:{regex} <==> {endpoint}'.format(
+        return '<{cls_name}>:"{route_path}" <==> "{endpoint}"'.format(
+            route_path=self.route_path,
             cls_name=self.__class__.__name__,
             regex=self.route_pattern,
             endpoint=self.endpoint
         )
```

### Comparing `Vank-1.0.1/Vank/core/routing/router.py` & `vank-1.0.2/vank/core/routing/router.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,54 @@
-from Vank.core import exceptions
-from Vank.core.routing.route import Route
+from vank.core import exceptions
+from vank.core.context import request
+from vank.core.routing.route import Route
 
 
 class Router:
     def __init__(self):
         self._routes = []
         self.route_path_set = set()
         # endpoint -->view_func 映射
         self.endpoint_func_dic = {}
 
     def add_route(self, route_path: str, route: "Route", view_func):
         """
         添加路由到路由列表中 同时校验是否有相同路由
         """
         if route_path in self.route_path_set:
-            raise LookupError(f'不能同时存在相同路由:[{route_path}]')
-
+            raise ValueError('"%s" This route is already in the router.' % route_path)
+        # 不能存在多个相同的endpoint
+        if route.endpoint in self.endpoint_func_dic:
+            raise ValueError('"%s" This endpoint is already in the router.' % route.endpoint)
         self.route_path_set.add(route_path)
         self._routes.append(route)
-        # 判断是否有相同的endpoint且该endpoint应该指向同一视图函数 否则报错
-        endpoint = route.endpoint
-        exist_func = self.endpoint_func_dic.get(endpoint, None)
-        if exist_func and view_func is not exist_func:
-            raise ValueError(f'一个endpoint不应指向多个视图:[{endpoint}]')
-        self.endpoint_func_dic[endpoint] = view_func
+        self.endpoint_func_dic[route.endpoint] = view_func
 
-    def match(self, request):
+    def match(self):
         """
         需要检查请求方法,需要
-        :param request:
         :return:
         """
 
         for route in self._routes:
             # 遍历路由列表并匹配
             res = route.route_pattern.match(request.path)
             if not res:
                 continue
             # 判断请求方法是否允许
             if not route.check_method(request.method):
-                raise exceptions.MethodNotAllowedException(f'{request.method.upper()}方法不被允许', allow=route.methods)
+                raise exceptions.MethodNotAllowedException(f'"{request.method.upper()}" Method is not allowed',
+                                                           allow=route.methods)
             # 获取endpoint和类型转换后的参数
             endpoint, arguments = route.endpoint, route.convert_arguments(**res.groupdict())
             view_function = self.endpoint_func_dic.get(endpoint)
             return view_function, arguments
 
         # 如果路由规则都没有找到那么就报404错误
-        raise exceptions.NotFoundException(f'资源 {request.path} 未找到')
+        raise exceptions.NotFoundException(f'Resource {request.path} not found')
 
     @property
     def routes(self):
         for route in self._routes:
             yield route
 
     def include_router(self, router: "Router"):
@@ -62,21 +60,21 @@
             # 获取路由未构建时的路径
             route_path = route.route_path
             # 获取视图函数
             view_func = router.endpoint_func_dic.get(route.endpoint)
             # 添加到主路由中
             self.add_route(route_path, route, view_func)
 
-    def url_for(self, endpoint: str, **arguments):
+    def url_reflect(self, endpoint: str, **arguments):
         for route in self.routes:
             try:
-                return route.url_for(endpoint, **arguments)
-            except exceptions.UrlForNotFound:
+                return route.url_reflect(endpoint, **arguments)
+            except exceptions.ReflectNotFound:
                 pass
-        raise exceptions.UrlForNotFound(endpoint, **arguments)
+        raise exceptions.ReflectNotFound(endpoint, **arguments)
 
     def __str__(self):
         return '\n'.join(
             '{route} <==> {view_func}'
             .format(route=route, view_func=self.endpoint_func_dic.get(route.endpoint))
             for route in self.routes
         )
```

### Comparing `Vank-1.0.1/Vank/core/views/static/control.py` & `vank-1.0.2/vank/applications/static/control.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 from pathlib import Path
-from Vank.core.config import conf
-from Vank.core.http.response import ResponseFile, Response
-from Vank.core.http.request import Request
-from Vank.core.exceptions import NotFoundException
+from vank.core.config import conf
 from email.utils import parsedate_to_datetime
+from vank.core.exceptions import NotFoundException
+from vank.core.http.response import ResponseFile, ResponsePlain
 
 
-def _get_file_modified(gmt_date: str, file_mtime) -> bool:
+def _is_file_modified(gmt_date: str, file_mtime) -> bool:
     """
     判断http header的modify时间和当前文件的modify时间是否相等
     """
     try:
         gmt_timestamp = parsedate_to_datetime(gmt_date).timestamp()
     except:
         return True
     else:
         return int(gmt_timestamp) == int(file_mtime)
 
 
-def get_file(request: "Request", fp):
+def get_file(if_modify_since: str, fp: str):
     full_path = Path(conf.STATIC_PATH).joinpath(fp)
     # 判断文件是否存在
     if not full_path.exists():
-        raise NotFoundException(f'{full_path}资源不存在')
+        raise NotFoundException(f'"{full_path}"Resource does not exist')
     # 判断是否为文件夹
     if full_path.is_dir():
-        raise NotFoundException('不允许索引目录')
+        raise NotFoundException('Index directory not allowed')
     # 获取modify时间,如果没有修改那么不返回文件
     # https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Headers/If-Modified-Since
-    if_modify_since = request.headers.get('IF_MODIFIED_SINCE', None)
     if if_modify_since:
         last_modify_time = full_path.stat().st_mtime
-        if _get_file_modified(if_modify_since, last_modify_time):
-            return Response(status=304)
+        if _is_file_modified(if_modify_since, last_modify_time):
+            return ResponsePlain(status=304)
     return ResponseFile(filepath=full_path.as_posix())
```

### Comparing `Vank-1.0.1/Vank/middleware/base.py` & `vank-1.0.2/vank/middleware/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,33 @@
-# @FileName: base.py
-# @Date    : 2022/9/7-1:17
-# @Author  : Vank
-# @Project : Vank
-
-
 class BaseMiddleware:
     """
     中间件基类
     实例方法:
-        def handle_request(self, request):
+        def handle_request(self):
             在接收到请求时 调用此方法
-            :param request: BasicRequest
             :return: 返回None 继续执行下一个中间件  返回Response 则直接返回到客户端
 
             ...
 
             return None
 
-        def handle_view(self, request, view_func, **view_kwargs):
+        def handle_view(self, view_func, **view_kwargs):
 
             在进入视图之前调用此方法
-            :param request: BasicRequest
             :param view_func: 对应的视图函数
             :param view_kwargs: 对应的视图函数所需可变参数
             :return: 返回None 继续执行下一个中间件  返回Response 则直接返回到客户端
 
             ...
 
             return None
 
-        def handle_response(self, request, response):
+        def handle_response(self, response):
 
             在视图函数处理该请求之后调用此方法
-            :param request: BasicRequest
             :param response: BasicResponse
             :return: 此方法应当始终返回 response
 
             ...
 
             return response
     """
@@ -45,21 +36,21 @@
         """
 
         :param get_response_callable: 为一个可调用对象 用于获取响应
         """
 
         self.get_response_callable = get_response_callable
 
-    def __call__(self, request, *args, **kwargs):
+    def __call__(self, *args, **kwargs):
         response = None
         # 处理请求
         if hasattr(self, 'handle_request'):
-            response = self.handle_request(request)
+            response = self.handle_request()
         # 交给对应的函数处理
         if not response:
-            response = self.get_response_callable(request, *args, **kwargs)
+            response = self.get_response_callable(*args, **kwargs)
 
         # 处理response
         if hasattr(self, 'handle_response'):
-            response = self.handle_response(request, response)
+            response = self.handle_response(response)
 
         return response
```

### Comparing `Vank-1.0.1/Vank/middleware/cors.py` & `vank-1.0.2/vank/middleware/cors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from Vank.core.config import conf
-from Vank.core.http.response import Response, Response400
-from Vank.middleware.base import BaseMiddleware
+from vank.core.config import conf
+from vank.core.context import request
+from vank.middleware.base import BaseMiddleware
+from vank.core.http.response import ResponsePlain, Response400
 
 
 class CorsMiddleware(BaseMiddleware):
     """解决跨域问题的中间件"""
     max_age: int = conf.CORS_MAX_AGE
     with_credentials: bool = conf.WITH_CREDENTIALS
     allowed_origins: list[str] = conf.CORS_ALLOWED_ORIGINS or ['*']
@@ -33,15 +34,15 @@
         # ========allowed headers========
         if self.with_credentials:
             response_headers['Access-Control-Allow-Credentials'] = 'true'
         # max-age
         response_headers['Access-Control-Max-Age'] = str(self.max_age)
         self.response_headers = response_headers
 
-    def handle_request(self, request):  # noqa
+    def handle_request(self):  # noqa
         # 判断请求方法是否为OPTIONS
         # 并且带有ACCESS_CONTROL_REQUEST_METHOD(接下来真正的请求会使用到哪个HTTP方法)
         # 以及ORIGIN在HTTP头部
         # 否则不处理此次请求
         if (
                 not request.method == 'OPTIONS'
                 and 'ACCESS_CONTROL_REQUEST_METHOD' not in request.headers
@@ -75,8 +76,8 @@
                 failed_flag = True
                 break
             else:
                 # 如果都符合,那么应该返回
                 response_headers['Access-Control-Allow-Headers'] = headers
         if failed_flag:
             return Response400('', headers=response_headers)
-        return Response('OK', headers=response_headers)
+        return ResponsePlain('OK', headers=response_headers)
```

### Comparing `Vank-1.0.1/Vank/middleware/session.py` & `vank-1.0.2/vank/middleware/session.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# Created by Vank
-# DateTime: 2022/12/23-16:50
-# Encoding: UTF-8
-import base64
 import json
-
+import base64
+from http.cookies import Morsel
+from vank.core.config import conf
+from vank.core.context import request
+from vank.utils.datastructures import Session
+from vank.middleware.base import BaseMiddleware
 from itsdangerous import TimestampSigner, BadSignature
 
-from Vank.middleware.base import BaseMiddleware
-from Vank.core.config import conf
-from Vank.utils.datastructures import Session
-
 
 class SessionMiddleware(BaseMiddleware):
     def __init__(self, get_response_callable):
         super(SessionMiddleware, self).__init__(get_response_callable)
         self.signer = TimestampSigner(conf.SECRET_KEY)
 
-    def handle_request(self, request, *args, **kwargs):
+    def handle_request(self, *args, **kwargs):
         # 获取cookie
-        signed_session_value = request.cookies.get(conf.SESSION_COOKIE_NAME, "").encode('utf-8')
+        signed_session_value = request.cookies.get(conf.SESSION_COOKIE_NAME, "")
+        if isinstance(signed_session_value, Morsel):
+            signed_session_value = signed_session_value.value
+        signed_session_value = signed_session_value.encode('utf-8')
         # 使用signer进行unsign得到base64编码(base64编码可以提高传输可靠性) 然后将base64编码进行解码得到json序列
         # 再将序列转为python object
         try:
             value = self.signer.unsign(signed_session_value, max_age=conf.SESSION_COOKIE_MAX_AGE)
             session = Session(json.loads(base64.b64decode(value)))
         except BadSignature as e:
             # 如果unsign失败 那么实例化一个空的Session
             session = Session()
         setattr(request, 'session', session)
         return None
 
-    def handle_response(self, request, response):
+    def handle_response(self, response):
         session: Session = getattr(request, 'session')
         # 判断此次请求是否有session
         # 如果有session且当前session内容为空
         # 那么将其删除
         if request.cookies.get(conf.SESSION_COOKIE_NAME, None) and not session:
             response.delete_cookie(
                 conf.SESSION_COOKIE_NAME,
```

### Comparing `Vank-1.0.1/Vank/utils/datastructures.py` & `vank-1.0.2/vank/utils/datastructures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import copy
 import tempfile
+import typing as t
 
 
 class SpooledUploadFile:
     """
     利用内置库tempfile的SpooledTemporaryFile;当文件超过特定大小时，将其写到磁盘
     """
 
@@ -30,76 +32,96 @@
     def __str__(self):
         return f'<{self.__class__.__name__}>:{self.filename}'
 
     def __repr__(self):
         return f'<{self.__class__.__name__}>:{self.filename}'
 
 
-class ReadOnlyMultiDict:
-    """只读多值字典"""
+class MultiValueDict(dict):
 
-    def __init__(self, *args, ):
-        if args:
-            self._list = [(k, v) for k, v in args[0]]
-            self._dict = dict(self._list)
-        else:
-            self._list = []
-            self._dict = {}
-
-    def get(self, key, default=None):
-        return self._dict.get(key, default)
-
-    def get_list(self, key, default=None):
-        temp = []
-        for k, v in self._list:
-            if k == key:
-                temp.append(v)
-        return temp or default
+    def get(self, key, default: t.Optional = None):
+        val = super().get(key)
+        return val[-1] if val else default
 
     def keys(self):
-        return self._dict.keys()
+        yield from self
+
+    def items(self):
+        for key in self:
+            yield key, self[key]
 
     def values(self):
-        return self._dict.values()
+        for key in self:
+            yield self[key]
 
-    def items(self):
-        return self._dict.items()
+    def get_all(self, key, default: t.Optional[t.Any] = None, t_class: t.Optional[t.Type] = list):
+        try:
+            val = super().__getitem__(key)
+        except KeyError:
+            val = default
+        else:
+            val = t_class(val)
 
-    def __getitem__(self, item):
-        return self._dict[item]
+        return val
 
-    def __contains__(self, item):
-        return item in self.keys()
+    def copy(self):
+        return copy.copy(self)
 
-    def __str__(self):
-        return f"<{self.__class__.__name__}>:({self.items()})"
+    def setlist(self, key, value: t.List):
+        """
+        设置一个list，这将覆盖原有的key对应的值
+        @param key:
+        @param value:
+        @return:
+        """
+        super().__setitem__(key, value)
+
+    def append_value(self, key, value, error=True):
+        try:
+            val = self[key]
+        except KeyError:
+            if error:
+                raise
+            super().__setitem__(key, [value])
+        else:
+            val.append(value)
 
-    def __repr__(self):
-        return f"<{self.__class__.__name__}>:({self.items()})"
+    def __setitem__(self, key, value):
+        super().__setitem__(key, [value])
+
+    def __getitem__(self, item):
+        val = super().__getitem__(item)
+        try:
+            return val[-1]
+        except IndexError:
+            return val
 
+    def __copy__(self):
+        return self.__class__((k, self.get_all(k)[:]) for k in self)
 
-class Form(ReadOnlyMultiDict):
+
+class Form(MultiValueDict):
     """
     form表单
     """
 
     def close(self):
         [item.close() for item in self.values() if isinstance(item, SpooledUploadFile)]
 
 
-class QueryString(ReadOnlyMultiDict):
+class QueryString(MultiValueDict):
     """查询参数"""
     pass
 
 
 class Headers:
     def __init__(self, raw_headers=None):
         self._list = []
         if raw_headers:
-            self._list = [(key.encode('latin-1'), value.encode('latin-1')) for key, value in raw_headers.items()]
+            self._list = [(key.encode('latin-1'), value.encode('latin-1')) for key, value in raw_headers]
 
     def __iter__(self):
         return iter(self._list)
 
     def __getitem__(self, item: str):
         res = [value.decode('latin-1') for key, value in self._list if key.decode('latin-1').lower() == item.lower()]
         if res:
@@ -142,31 +164,37 @@
             if item[0].decode('latin-1').lower() == key.lower():
                 self._list.pop(idx)
 
     def __contains__(self, key):
         res = [item_key for item_key, value in self.items() if item_key.lower() == key.lower()]
         return any(res)
 
+    def __str__(self):
+        return f'<{self.__class__.__name__}>:{self.items()}'
+
+    def __repr__(self):
+        return f'<{self.__class__.__name__}>:{self.items()}'
+
 
 class Session:
     def __init__(self, session=None):
         self._session = session or {}
         self._is_changed = False  # session是否修改的标志 SessionMiddleware的handle_response会用到
 
     def __getitem__(self, key):
         if key in self._session.keys():
             return self._session[key]
-        raise KeyError(f'session key {key}不存在')
+        raise KeyError(f'Session key "{key}" does not exist')
 
     def __delitem__(self, key):
         if key in self.keys():
             del self._session[key]
             self._is_changed = True
         else:
-            raise KeyError(f'无法删除 session key {key}不存在')
+            raise KeyError(f'Unable to delete session key."{key}" does not exist')
 
     def __setitem__(self, key, value):
         self._session[key] = value
         self._is_changed = True
 
     def __bool__(self):
         return bool(self._session)
```

### Comparing `Vank-1.0.1/Vank/utils/log.py` & `vank-1.0.2/vank/utils/log.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Created by Vank
+# Created by vank
 # DateTime: 2022/10/28-17:33
 # Encoding: UTF-8
 import logging.config
 
 DEFAULT = {
     "version": 1,
     "disable_existing_loggers": False,
@@ -35,12 +35,12 @@
         },
     },
 }
 
 
 def setup_config(user_log):
     """
-    :param user_log: settings中的LOGGING
+    :param user_log: log配置
     """
     logging.config.dictConfig(DEFAULT)
-    if user_log:
+    if isinstance(user_log, dict) and user_log:
         logging.config.dictConfig(user_log)
```

### Comparing `Vank-1.0.1/Vank/utils/reloader.py` & `vank-1.0.2/vank/utils/reloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Created by Vank
+# Created by vank
 # DateTime: 2022/12/7-10:44
 # Encoding: UTF-8
 import sys
 import time
 import os.path
 import threading
 import typing as t
@@ -28,26 +28,26 @@
             current_modify_time = os.stat(name).st_mtime
             previous_modify_time = self.modify_times.get(name, None)
             if not previous_modify_time:
                 self.modify_times[name] = current_modify_time
                 continue
 
             if current_modify_time > previous_modify_time:
-                logger.warning(f'检测到文件{name}已经改变 重启!')
+                logger.warning(f'File {name} has changed!')
                 self.trigger_reload()
 
     def trigger_reload(self):
         sys.exit(3)
 
     def restart_with_reloader(self):
         """
         通过subprocess重启服务
         """
         while 1:
-            logger.warning('服务发生变化、重启'.center(20, '='))
+            logger.warning('The service has changed and is currently restarting'.center(20, '='))
             # 获取启动参数
             args = self._get_args_for_reloading()
             # 创建新的环境变量
             environment = {**os.environ.copy(), 'autoreload': '1'}
             # 启动新的子进程服务、在重载的服务未退出时会阻塞
             exit_code = subprocess.call(args, env=environment)
             # 判断exit_code是否为3，否则结束当前服务
```

### Comparing `Vank-1.0.1/Vank/utils/signal.py` & `vank-1.0.2/vank/utils/signal.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import typing as t
 from threading import Lock
-from functools import wraps
 
 
 class Signal:
     """
     信号是一种设计模式,解决了一对多的hard-code问题
     """
 
     def __init__(self):
         self.lock = Lock()
         self._binds: t.Dict[int, t.Callable] = {}
 
-    def bind(self, listener: t.Callable, identify: int = None, *array, **kwargs):
+    def bind(self, listener: t.Callable, identify: int = None):
         """
         绑定
         """
 
         with self.lock:
             if identify is None:
                 identify = id(listener)
@@ -37,10 +36,10 @@
             return [
                 (identify, listener, listener(signal=self, sender=sender, *args, **kwargs))
                 for identify, listener in self._binds.items()
             ]
 
 
 configs_check = Signal()
-on_start_up = Signal()
+on_stop_down = Signal()
 on_request_start = Signal()
 on_request_end = Signal()
```

### Comparing `Vank-1.0.1/Vank.egg-info/PKG-INFO` & `vank-1.0.2/vank.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Vank
-Version: 1.0.1
+Name: vank
+Version: 1.0.2
 Summary: A Python Web Framework
 Author-email: WanKe <852003793@qq.com>
 License: MIT License
         
         Copyright (c) 2022 852003793
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,26 +34,38 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vank
 
 一个基于Python的Web框架
 
-### QuickStart
+### 特性
+
+- 高度个性化: 你可以构建许多自定义的组件添加到配置当中、在恰当的时机使用他们。例如自定义路由转换器、错误处理器等。
+- 低学习成本: 这是一个非常简单的框架，你可以在仅仅几个小时内学习完并熟练使用它。
+- 完备的文档: 具有非常详细的文档供开发者们学习，并且了解框架是如何运行的。
+
+***
+
+### 快速开始
+
 - 安装Vank
+
 ```shell
-pip install Vank
+pip install vank
 ```
+
 - 初始化项目
 
 ```shell
-python -m Vank init -n mysite
+python -m vank init -n mysite
 ```
+
 - 运行项目
+
 ```shell
 cd mysite
 python main.py
 ```
 
- 
 ***
 [技术文档](http://docs.bestvank.cn/)
```

