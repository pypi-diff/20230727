# Comparing `tmp/CheeseLog-0.0.0.tar.gz` & `tmp/CheeseLog-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CheeseLog-0.0.0.tar", last modified: Wed Jul 26 15:31:20 2023, max compression
+gzip compressed data, was "CheeseLog-0.0.2.tar", last modified: Thu Jul 27 15:16:30 2023, max compression
```

## Comparing `CheeseLog-0.0.0.tar` & `CheeseLog-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-07-26 15:31:20.466305 CheeseLog-0.0.0/
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-07-26 15:31:20.465358 CheeseLog-0.0.0/CheeseLog/
--rw-r--r--   0 cheese     (501) staff       (20)     6175 2023-07-26 15:20:52.000000 CheeseLog-0.0.0/CheeseLog/__init__.py
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-07-26 15:31:20.465978 CheeseLog-0.0.0/CheeseLog.egg-info/
--rw-r--r--   0 cheese     (501) staff       (20)     3452 2023-07-26 15:31:20.000000 CheeseLog-0.0.0/CheeseLog.egg-info/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)      212 2023-07-26 15:31:20.000000 CheeseLog-0.0.0/CheeseLog.egg-info/SOURCES.txt
--rw-r--r--   0 cheese     (501) staff       (20)        1 2023-07-26 15:31:20.000000 CheeseLog-0.0.0/CheeseLog.egg-info/dependency_links.txt
--rw-r--r--   0 cheese     (501) staff       (20)       11 2023-07-26 15:31:20.000000 CheeseLog-0.0.0/CheeseLog.egg-info/requires.txt
--rw-r--r--   0 cheese     (501) staff       (20)       10 2023-07-26 15:31:20.000000 CheeseLog-0.0.0/CheeseLog.egg-info/top_level.txt
--rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 07:27:31.000000 CheeseLog-0.0.0/LICENSE
--rw-r--r--   0 cheese     (501) staff       (20)     3452 2023-07-26 15:31:20.466154 CheeseLog-0.0.0/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)     2947 2023-07-26 09:44:29.000000 CheeseLog-0.0.0/README.md
--rw-r--r--   0 cheese     (501) staff       (20)       38 2023-07-26 15:31:20.466371 CheeseLog-0.0.0/setup.cfg
--rw-r--r--   0 cheese     (501) staff       (20)      829 2023-07-26 15:31:05.000000 CheeseLog-0.0.0/setup.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-07-27 15:16:30.767676 CheeseLog-0.0.2/
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-07-27 15:16:30.766614 CheeseLog-0.0.2/CheeseLog/
+-rw-r--r--   0 cheese     (501) staff       (20)     6173 2023-07-27 15:06:08.000000 CheeseLog-0.0.2/CheeseLog/__init__.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-07-27 15:16:30.767347 CheeseLog-0.0.2/CheeseLog.egg-info/
+-rw-r--r--   0 cheese     (501) staff       (20)     3452 2023-07-27 15:16:30.000000 CheeseLog-0.0.2/CheeseLog.egg-info/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)      212 2023-07-27 15:16:30.000000 CheeseLog-0.0.2/CheeseLog.egg-info/SOURCES.txt
+-rw-r--r--   0 cheese     (501) staff       (20)        1 2023-07-27 15:16:30.000000 CheeseLog-0.0.2/CheeseLog.egg-info/dependency_links.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       11 2023-07-27 15:16:30.000000 CheeseLog-0.0.2/CheeseLog.egg-info/requires.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       10 2023-07-27 15:16:30.000000 CheeseLog-0.0.2/CheeseLog.egg-info/top_level.txt
+-rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 07:27:31.000000 CheeseLog-0.0.2/LICENSE
+-rw-r--r--   0 cheese     (501) staff       (20)     3452 2023-07-27 15:16:30.767550 CheeseLog-0.0.2/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)     2947 2023-07-26 09:44:29.000000 CheeseLog-0.0.2/README.md
+-rw-r--r--   0 cheese     (501) staff       (20)       38 2023-07-27 15:16:30.767753 CheeseLog-0.0.2/setup.cfg
+-rw-r--r--   0 cheese     (501) staff       (20)      829 2023-07-27 15:16:22.000000 CheeseLog-0.0.2/setup.py
```

### Comparing `CheeseLog-0.0.0/CheeseLog/__init__.py` & `CheeseLog-0.0.2/CheeseLog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.timerTemplate: Optional[str] = timerTemplate
 
 class Logger(threading.Thread):
     def __init__(self):
         self.filePath: Optional[str] = None
         self.messageTemplate: str = '(%level) %timer > %content'
         self.timerTemplate: str = '%Y-%m-%d %H:%M:%S.%f'
-        self.filter: NonNegativeInt | list[str] = []
+        self.filter: NonNegativeInt | set[str] = {}
         self.levels: dict[str, Level] = {
             'DEBUG': Level(10, '34', None, None),
             'INFO': Level(20, '32', None, None),
             'STARTING': Level(20, '32', None, None),
             'ENDING': Level(20, '34', None, None),
             'HTTP': Level(20, None, None, None),
             'WEBSOCKET': Level(20, None, None, None),
@@ -76,15 +76,15 @@
     '''
 
     ''' Validate '''
     if level not in logger.levels:
         raise KeyError('no level with this key')
 
     ''' Filter '''
-    if isinstance(logger.filter, list):
+    if isinstance(logger.filter, set):
         for _level in logger.filter:
             if level == _level:
                 return
     elif logger.levels[level].weight <= NonNegativeInt(logger.filter):
         return
 
     ''' Terminal '''
```

### Comparing `CheeseLog-0.0.0/CheeseLog.egg-info/PKG-INFO` & `CheeseLog-0.0.2/CheeseLog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheeseLog
-Version: 0.0.0
+Version: 0.0.2
 Summary: 日志系统。可在控制台输出一定格式的、可选颜色的内容，并支持写入指定的日志文件。
 Home-page: https://github.com/CheeseUnknown/CheeseLog
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: log
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CheeseLog-0.0.0/LICENSE` & `CheeseLog-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CheeseLog-0.0.0/PKG-INFO` & `CheeseLog-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheeseLog
-Version: 0.0.0
+Version: 0.0.2
 Summary: 日志系统。可在控制台输出一定格式的、可选颜色的内容，并支持写入指定的日志文件。
 Home-page: https://github.com/CheeseUnknown/CheeseLog
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: log
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CheeseLog-0.0.0/README.md` & `CheeseLog-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `CheeseLog-0.0.0/setup.py` & `CheeseLog-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('./README.md', 'r', encoding = 'utf-8') as f:
     longDescription = f.read()
 
 setuptools.setup(
     name = 'CheeseLog',
-    version = '0.0.0',
+    version = '0.0.2',
     author = 'Cheese Unknown',
     author_email = 'cheese@cheese.ren',
     description = '日志系统。可在控制台输出一定格式的、可选颜色的内容，并支持写入指定的日志文件。',
     long_description = longDescription,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/CheeseUnknown/CheeseLog',
     license = 'MIT',
```

