# Comparing `tmp/logPPP-1.1.0.tar.gz` & `tmp/logPPP-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logPPP-1.1.0.tar", last modified: Wed Jul 26 13:50:46 2023, max compression
+gzip compressed data, was "logPPP-1.1.1.tar", last modified: Thu Jul 27 03:52:02 2023, max compression
```

## Comparing `logPPP-1.1.0.tar` & `logPPP-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 13:50:46.532469 logPPP-1.1.0/
--rw-rw-rw-   0        0        0      126 2023-07-26 13:50:46.532469 logPPP-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      111 2023-07-26 10:16:17.000000 logPPP-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 13:50:46.516822 logPPP-1.1.0/logPPP.egg-info/
--rw-rw-rw-   0        0        0      126 2023-07-26 13:50:46.000000 logPPP-1.1.0/logPPP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-26 13:50:46.000000 logPPP-1.1.0/logPPP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 13:50:46.000000 logPPP-1.1.0/logPPP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 13:50:46.000000 logPPP-1.1.0/logPPP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 13:50:46.532469 logPPP-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      379 2023-07-26 10:16:17.000000 logPPP-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 13:50:46.516822 logPPP-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 13:50:46.516822 logPPP-1.1.0/src/logPPP/
--rw-rw-rw-   0        0        0      116 2023-07-26 10:16:17.000000 logPPP-1.1.0/src/logPPP/_ConsoleColors.py
--rw-rw-rw-   0        0        0     1687 2023-07-26 13:50:44.000000 logPPP-1.1.0/src/logPPP/__init__.py
--rw-rw-rw-   0        0        0      453 2023-07-26 10:16:17.000000 logPPP-1.1.0/src/logPPP/_util.py
--rw-rw-rw-   0        0        0      373 2023-07-26 10:16:17.000000 logPPP-1.1.0/src/logPPP/logPPPLevel.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:52:02.791176 logPPP-1.1.1/
+-rw-rw-rw-   0        0        0      126 2023-07-27 03:52:02.791176 logPPP-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-07-26 13:51:56.000000 logPPP-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 03:52:02.791176 logPPP-1.1.1/logPPP.egg-info/
+-rw-rw-rw-   0        0        0      126 2023-07-27 03:52:02.000000 logPPP-1.1.1/logPPP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-27 03:52:02.000000 logPPP-1.1.1/logPPP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 03:52:02.000000 logPPP-1.1.1/logPPP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 03:52:02.000000 logPPP-1.1.1/logPPP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 03:52:02.791176 logPPP-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      379 2023-07-26 10:16:17.000000 logPPP-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:52:02.791176 logPPP-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 03:52:02.791176 logPPP-1.1.1/src/logPPP/
+-rw-rw-rw-   0        0        0      116 2023-07-26 10:16:17.000000 logPPP-1.1.1/src/logPPP/_ConsoleColors.py
+-rw-rw-rw-   0        0        0     1914 2023-07-27 03:46:44.000000 logPPP-1.1.1/src/logPPP/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-07-26 10:16:17.000000 logPPP-1.1.1/src/logPPP/_util.py
+-rw-rw-rw-   0        0        0      373 2023-07-26 10:16:17.000000 logPPP-1.1.1/src/logPPP/logPPPLevel.py
```

### Comparing `logPPP-1.1.0/src/logPPP/__init__.py` & `logPPP-1.1.1/src/logPPP/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 import datetime
 
 from ._ConsoleColors import ConsoleColors
 from ._util import *
 from .logPPPLevel import logPPPLevel
 
 __all__ = ['__version__', 'IS_COLOR', 'LEVEL', 'logPPPLevel', 'info', 'warning', 'error', 'debug', 'critical']
-__version__ = '1.1.0'
+__version__ = '1.1.1'
 
 # 是否开启颜色
 IS_COLOR = True
 # 等级
 LEVEL = logPPPLevel.INFO
 
 
 # 日志输出
-def _base(args, sep=' ', end='\n', file=None, _level=logPPPLevel.INFO, color=ConsoleColors.RESET, is_color=True):
+def _base(*args, sep=' ', end='\n', file=None, _level=logPPPLevel.INFO, color=ConsoleColors.RESET, is_color=True):
+    args = sep.join(map(str, args))
     timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-    args = "{:<20} {:<8} {}  {}".format(timestamp, get_caller_file_basename_path(), _level['name'], args)
+    args = "{:<20} {:<8} {}  {}".format(timestamp, get_caller_file_basename_path(), _level.get('name'), args)
     if is_color is None and IS_COLOR or is_color is True:
         args = f"{color}{args}{ConsoleColors.RESET}"
     if _level['level'] >= LEVEL['level']:
         print(args, sep=sep, end=end, file=file)
 
 
 # info等级
-def info(args, sep=' ', end='\n', file=None, is_color=None):
-    _base(args, sep, end, file, logPPPLevel.INFO, ConsoleColors.RESET, is_color)
+def info(*args, sep=' ', end='\n', file=None, is_color=None):
+    _base(*args, sep=sep, end=end, file=file, _level=logPPPLevel.INFO, color=ConsoleColors.RESET, is_color=is_color)
 
 
 # warning等级
-def warning(args, sep=' ', end='\n', file=None, is_color=None):
-    _base(args, sep, end, file, logPPPLevel.WARNING, ConsoleColors.YELLOW, is_color)
+def warning(*args, sep=' ', end='\n', file=None, is_color=None):
+    _base(*args, sep=sep, end=end, file=file, _level=logPPPLevel.WARNING, color=ConsoleColors.YELLOW, is_color=is_color)
 
 
 # error等级
-def error(args, sep=' ', end='\n', file=None, is_color=None):
-    _base(args, sep, end, file, logPPPLevel.ERROR, ConsoleColors.RED, is_color)
+def error(*args, sep=' ', end='\n', file=None, is_color=None):
+    _base(*args, sep=sep, end=end, file=file, _level=logPPPLevel.ERROR, color=ConsoleColors.RED, is_color=is_color)
 
 
 # debug等级
-def debug(args, sep=' ', end='\n', file=None, is_color=None):
-    _base(args, sep, end, file, logPPPLevel.DEBUG, ConsoleColors.RED, is_color)
+def debug(*args, sep=' ', end='\n', file=None, is_color=None):
+    _base(*args, sep=sep, end=end, file=file, _level=logPPPLevel.DEBUG, color=ConsoleColors.RED, is_color=is_color)
 
 
 # critical等级
-def critical(args, sep=' ', end='\n', file=None, is_color=None):
-    _base(args, sep, end, file, logPPPLevel.CRITICAL, ConsoleColors.RED, is_color)
+def critical(*args, sep=' ', end='\n', file=None, is_color=None):
+    _base(*args, sep=sep, end=end, file=file, _level=logPPPLevel.CRITICAL, color=ConsoleColors.RED, is_color=is_color)
```

