# Comparing `tmp/Flask-Lib-0.2.0.tar.gz` & `tmp/Flask-Lib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Lib-0.2.0.tar", last modified: Thu Jul 27 14:13:16 2023, max compression
+gzip compressed data, was "Flask-Lib-0.2.1.tar", last modified: Thu Jul 27 15:26:49 2023, max compression
```

## Comparing `Flask-Lib-0.2.0.tar` & `Flask-Lib-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:16.766625 Flask-Lib-0.2.0/
--rw-rw-rw-   0        0        0     1529 2023-05-04 01:08:33.000000 Flask-Lib-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      701 2023-07-27 14:13:16.766625 Flask-Lib-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-05-09 00:54:20.000000 Flask-Lib-0.2.0/README.md
--rw-rw-rw-   0        0        0      801 2023-07-27 14:13:16.767622 Flask-Lib-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       36 2023-05-09 00:43:43.000000 Flask-Lib-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:16.742687 Flask-Lib-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:16.759643 Flask-Lib-0.2.0/src/Flask_Lib.egg-info/
--rw-rw-rw-   0        0        0      701 2023-07-27 14:13:16.000000 Flask-Lib-0.2.0/src/Flask_Lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-07-27 14:13:16.000000 Flask-Lib-0.2.0/src/Flask_Lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 14:13:16.000000 Flask-Lib-0.2.0/src/Flask_Lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      291 2023-07-27 14:13:16.000000 Flask-Lib-0.2.0/src/Flask_Lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-27 14:13:16.000000 Flask-Lib-0.2.0/src/Flask_Lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:16.764630 Flask-Lib-0.2.0/src/flasklib/
--rw-rw-rw-   0        0        0      218 2023-07-27 14:10:28.000000 Flask-Lib-0.2.0/src/flasklib/__init__.py
--rw-rw-rw-   0        0        0     2840 2023-05-04 22:19:44.000000 Flask-Lib-0.2.0/src/flasklib/dates.py
--rw-rw-rw-   0        0        0     1062 2023-05-04 22:19:44.000000 Flask-Lib-0.2.0/src/flasklib/errors.py
--rw-rw-rw-   0        0        0      836 2023-05-09 00:44:22.000000 Flask-Lib-0.2.0/src/flasklib/jinja.py
--rw-rw-rw-   0        0        0     1376 2023-05-04 01:27:16.000000 Flask-Lib-0.2.0/src/flasklib/json.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:16.765627 Flask-Lib-0.2.0/src/flasklib/mappers/
--rw-rw-rw-   0        0        0      129 2023-05-04 01:41:47.000000 Flask-Lib-0.2.0/src/flasklib/mappers/__init__.py
--rw-rw-rw-   0        0        0     1077 2023-07-27 14:06:42.000000 Flask-Lib-0.2.0/src/flasklib/mappers/mappers.py
--rw-rw-rw-   0        0        0     1937 2023-05-04 22:19:44.000000 Flask-Lib-0.2.0/src/flasklib/responses.py
--rw-rw-rw-   0        0        0      427 2023-05-04 22:19:44.000000 Flask-Lib-0.2.0/src/flasklib/startup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:26:49.615145 Flask-Lib-0.2.1/
+-rw-rw-rw-   0        0        0     1529 2023-05-04 01:08:33.000000 Flask-Lib-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      701 2023-07-27 15:26:49.616143 Flask-Lib-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-09 00:54:20.000000 Flask-Lib-0.2.1/README.md
+-rw-rw-rw-   0        0        0      801 2023-07-27 15:26:49.617140 Flask-Lib-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       36 2023-05-09 00:43:43.000000 Flask-Lib-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:26:49.595199 Flask-Lib-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 15:26:49.609161 Flask-Lib-0.2.1/src/Flask_Lib.egg-info/
+-rw-rw-rw-   0        0        0      701 2023-07-27 15:26:49.000000 Flask-Lib-0.2.1/src/Flask_Lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-07-27 15:26:49.000000 Flask-Lib-0.2.1/src/Flask_Lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 15:26:49.000000 Flask-Lib-0.2.1/src/Flask_Lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      291 2023-07-27 15:26:49.000000 Flask-Lib-0.2.1/src/Flask_Lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 15:26:49.000000 Flask-Lib-0.2.1/src/Flask_Lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 15:26:49.613151 Flask-Lib-0.2.1/src/flasklib/
+-rw-rw-rw-   0        0        0      218 2023-07-27 14:10:28.000000 Flask-Lib-0.2.1/src/flasklib/__init__.py
+-rw-rw-rw-   0        0        0     2840 2023-05-04 22:19:44.000000 Flask-Lib-0.2.1/src/flasklib/dates.py
+-rw-rw-rw-   0        0        0     1062 2023-05-04 22:19:44.000000 Flask-Lib-0.2.1/src/flasklib/errors.py
+-rw-rw-rw-   0        0        0      836 2023-05-09 00:44:22.000000 Flask-Lib-0.2.1/src/flasklib/jinja.py
+-rw-rw-rw-   0        0        0     1376 2023-05-04 01:27:16.000000 Flask-Lib-0.2.1/src/flasklib/json.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:26:49.615145 Flask-Lib-0.2.1/src/flasklib/mappers/
+-rw-rw-rw-   0        0        0      129 2023-05-04 01:41:47.000000 Flask-Lib-0.2.1/src/flasklib/mappers/__init__.py
+-rw-rw-rw-   0        0        0     1492 2023-07-27 15:25:17.000000 Flask-Lib-0.2.1/src/flasklib/mappers/mappers.py
+-rw-rw-rw-   0        0        0     1937 2023-05-04 22:19:44.000000 Flask-Lib-0.2.1/src/flasklib/responses.py
+-rw-rw-rw-   0        0        0      427 2023-05-04 22:19:44.000000 Flask-Lib-0.2.1/src/flasklib/startup.py
```

### Comparing `Flask-Lib-0.2.0/LICENSE` & `Flask-Lib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Lib-0.2.0/PKG-INFO` & `Flask-Lib-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: Flask-Lib
-Version: 0.2.0
+Version: 0.2.1
 Summary: Premade Flask tools to speed up development.
 Home-page: https://github.com/rrickgauer/Flask-Lib
 Author: Ryan Rickgauer
 Author-email: rrickgauer1@gmail.com
 License: UNKNOWN
 Description: # Flask-Lib
         Premade Flask tools to speed up development.
```

### Comparing `Flask-Lib-0.2.0/setup.cfg` & `Flask-Lib-0.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2046 6c61 736b 2d4c 6962 0d0a 7665   = Flask-Lib..ve
-00000020: 7273 696f 6e20 3d20 302e 322e 300d 0a64  rsion = 0.2.0..d
+00000020: 7273 696f 6e20 3d20 302e 322e 310d 0a64  rsion = 0.2.1..d
 00000030: 6573 6372 6970 7469 6f6e 203d 2050 7265  escription = Pre
 00000040: 6d61 6465 2046 6c61 736b 2074 6f6f 6c73  made Flask tools
 00000050: 2074 6f20 7370 6565 6420 7570 2064 6576   to speed up dev
 00000060: 656c 6f70 6d65 6e74 2e0d 0a61 7574 686f  elopment...autho
 00000070: 7220 3d20 5279 616e 2052 6963 6b67 6175  r = Ryan Rickgau
 00000080: 6572 0d0a 6175 7468 6f72 5f65 6d61 696c  er..author_email
 00000090: 203d 2072 7269 636b 6761 7565 7231 4067   = rrickgauer1@g
```

### Comparing `Flask-Lib-0.2.0/src/Flask_Lib.egg-info/PKG-INFO` & `Flask-Lib-0.2.1/src/Flask_Lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: Flask-Lib
-Version: 0.2.0
+Version: 0.2.1
 Summary: Premade Flask tools to speed up development.
 Home-page: https://github.com/rrickgauer/Flask-Lib
 Author: Ryan Rickgauer
 Author-email: rrickgauer1@gmail.com
 License: UNKNOWN
 Description: # Flask-Lib
         Premade Flask tools to speed up development.
```

### Comparing `Flask-Lib-0.2.0/src/flasklib/dates.py` & `Flask-Lib-0.2.1/src/flasklib/dates.py`

 * *Files identical despite different names*

### Comparing `Flask-Lib-0.2.0/src/flasklib/errors.py` & `Flask-Lib-0.2.1/src/flasklib/errors.py`

 * *Files identical despite different names*

### Comparing `Flask-Lib-0.2.0/src/flasklib/jinja.py` & `Flask-Lib-0.2.1/src/flasklib/jinja.py`

 * *Files identical despite different names*

### Comparing `Flask-Lib-0.2.0/src/flasklib/json.py` & `Flask-Lib-0.2.1/src/flasklib/json.py`

 * *Files identical despite different names*

### Comparing `Flask-Lib-0.2.0/src/flasklib/mappers/mappers.py` & `Flask-Lib-0.2.1/src/flasklib/mappers/mappers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 from __future__ import annotations
 import datetime
 import uuid
 from dacite.core import from_dict
 import dacite
 from typing import TypeVar, Type, Dict, List
+import enum
 
 
+def _try_map_date_str(day_str: str):
+    """Try mapping a date string value"""
+    
+    try:
+        return datetime.date.fromisoformat(day_str)
+    except:
+        return datetime.datetime.fromisoformat(day_str).date()
+
 T = TypeVar("T")
 
 MAPPER_CONFIG = dacite.Config(
     cast = [
         uuid.UUID, 
+        enum.Enum
     ],
 
     type_hooks = {
         datetime.datetime: datetime.datetime.fromisoformat,
-        datetime.date: datetime.date.fromisoformat,
+        datetime.date: _try_map_date_str,
         datetime.time: datetime.time.fromisoformat,
     },
 )
 
 
+
 def map_dicts(data: List[Dict], class_type: Type[T]) -> List[T]:
     """Map the dictionaries to the specified type."""
     return [map_dict(d, class_type) for d in data]
 
 
 def map_dict(data: Dict, class_type: Type[T]) -> T:
     """Map the given dictionary to the specified type"""
@@ -37,8 +48,15 @@
     @classmethod
     def from_dicts(cls, data: List[Dict]):
         return map_dicts(data, cls)
 
     @classmethod
     def from_dict(cls, data: Dict):
         return map_dict(data, cls)
-    
+    
+
+def get_mapper_config() -> dacite.Config:
+    return MAPPER_CONFIG
+
+def set_mapper_config(newconfig: dacite.Config):
+    global MAPPER_CONFIG
+    MAPPER_CONFIG = newconfig
```

### Comparing `Flask-Lib-0.2.0/src/flasklib/responses.py` & `Flask-Lib-0.2.1/src/flasklib/responses.py`

 * *Files identical despite different names*

