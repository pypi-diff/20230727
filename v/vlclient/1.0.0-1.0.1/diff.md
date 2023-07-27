# Comparing `tmp/vlclient-1.0.0.tar.gz` & `tmp/vlclient-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlclient-1.0.0.tar", max compression
+gzip compressed data, was "vlclient-1.0.1.tar", max compression
```

## Comparing `vlclient-1.0.0.tar` & `vlclient-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2023-07-27 08:18:59.154083 vlclient-1.0.0/LICENSE
--rw-r--r--   0        0        0      343 2023-07-27 07:50:58.156971 vlclient-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      963 2023-07-27 08:19:38.657082 vlclient-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-07-27 07:42:44.996970 vlclient-1.0.0/vlclient/__init__.py
--rw-r--r--   0        0        0     1739 2023-07-27 07:51:19.853971 vlclient-1.0.0/vlclient/auth.py
--rw-r--r--   0        0        0    41503 2023-07-27 08:00:41.160970 vlclient-1.0.0/vlclient/client.py
--rw-r--r--   0        0        0      688 2023-07-27 07:52:36.110971 vlclient-1.0.0/vlclient/exceptions.py
--rw-r--r--   0        0        0      550 2023-07-27 07:52:15.645972 vlclient-1.0.0/vlclient/resources.py
--rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 vlclient-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-27 08:18:59.154083 vlclient-1.0.1/LICENSE
+-rw-r--r--   0        0        0      343 2023-07-27 03:56:25.146937 vlclient-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      963 2023-07-27 08:19:38.657082 vlclient-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 07:42:44.996970 vlclient-1.0.1/vlclient/__init__.py
+-rw-r--r--   0        0        0     1739 2023-07-27 07:51:19.853971 vlclient-1.0.1/vlclient/auth.py
+-rw-r--r--   0        0        0    41513 2023-07-27 03:54:19.040924 vlclient-1.0.1/vlclient/client.py
+-rw-r--r--   0        0        0      688 2023-07-27 07:52:36.110971 vlclient-1.0.1/vlclient/exceptions.py
+-rw-r--r--   0        0        0      563 2023-07-27 03:47:59.534799 vlclient-1.0.1/vlclient/resources.py
+-rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 vlclient-1.0.1/PKG-INFO
```

### Comparing `vlclient-1.0.0/LICENSE` & `vlclient-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vlclient-1.0.0/README.md` & `vlclient-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vlclient-1.0.0/vlclient/auth.py` & `vlclient-1.0.1/vlclient/auth.py`

 * *Files identical despite different names*

### Comparing `vlclient-1.0.0/vlclient/client.py` & `vlclient-1.0.1/vlclient/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
         start_index: int = 0,
         end_index: int = 15,
         queue_id: t.Text = "null",
     ) -> dict:
         """
         MatchHistory_FetchMatchHistory
         Get recent matches for a player
-        There are 3 optional query parameters: start_index, end_index, and queue_id. queue can be one of null, competitive, custom, deathmatch, ggteam, newmap, onefa, snowball, spikerush, or unrated.
+        There are 3 optional query parameters: start_index, end_index, and queue_id. queue can be one of null, competitive, custom, deathmatch, ggteam, newmap, onefa, snowball, spikerush, hurm or unrated.
         """
         self.__check_queue_type(queue_id)
         puuid = self.__check_puuid(puuid)
         data = self.fetch(
             endpoint=f"/match-history/v1/history/{puuid}?startIndex={start_index}&endIndex={end_index}"
             + (f"&queue={queue_id}" if queue_id != "null" else ""),
             endpoint_type="pd",
@@ -289,15 +289,15 @@
         start_index: int = 0,
         end_index: int = 15,
         queue_id: t.Text = "competitive",
     ) -> dict:
         """
         MMR_FetchCompetitiveUpdates
         Get recent games and how they changed ranking
-        There are 3 optional query parameters: start_index, end_index, and queue_id. queue can be one of null, competitive, custom, deathmatch, ggteam, newmap, onefa, snowball, spikerush, or unrated.
+        There are 3 optional query parameters: start_index, end_index, and queue_id. queue can be one of null, competitive, custom, deathmatch, ggteam, newmap, onefa, snowball, spikerush, hurm or unrated.
         """
         self.__check_queue_type(queue_id)
         puuid = self.__check_puuid(puuid)
         data = self.fetch(
             endpoint=f"/mmr/v1/players/{puuid}/competitiveupdates?startIndex={start_index}&endIndex={end_index}"
             + (f"&queue={queue_id}" if queue_id != "" else ""),
             endpoint_type="pd",
```

### Comparing `vlclient-1.0.0/vlclient/exceptions.py` & `vlclient-1.0.1/vlclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `vlclient-1.0.0/vlclient/resources.py` & `vlclient-1.0.1/vlclient/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,10 @@
     "custom",
     "deathmatch",
     "ggteam",
     "snowball",
     "spikerush",
     "unrated",
     "onefa",
+    "hurm",
     "null",
 ]
```

### Comparing `vlclient-1.0.0/PKG-INFO` & `vlclient-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlclient
-Version: 1.0.0
+Version: 1.0.1
 Summary: Valorant Client API Wrapper
 Author: anntnzrb
 Author-email: anntnzrb@proton.me
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

