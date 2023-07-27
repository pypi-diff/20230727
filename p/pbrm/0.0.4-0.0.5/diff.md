# Comparing `tmp/pbrm-0.0.4.tar.gz` & `tmp/pbrm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbrm-0.0.4.tar", last modified: Fri Mar 31 13:40:05 2023, max compression
+gzip compressed data, was "pbrm-0.0.5.tar", last modified: Thu Jul 27 06:23:47 2023, max compression
```

## Comparing `pbrm-0.0.4.tar` & `pbrm-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 13:40:05.299816 pbrm-0.0.4/
--rw-rw-rw-   0        0        0      253 2023-03-31 13:40:05.298469 pbrm-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-03-30 13:40:04.000000 pbrm-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-31 13:40:05.287099 pbrm-0.0.4/pbrm/
--rw-rw-rw-   0        0        0       22 2023-03-30 13:58:48.000000 pbrm-0.0.4/pbrm/__init__.py
--rw-rw-rw-   0        0        0      165 2023-03-30 13:06:26.000000 pbrm-0.0.4/pbrm/change_repository.py
--rw-rw-rw-   0        0        0     2906 2023-03-31 11:14:57.000000 pbrm-0.0.4/pbrm/command_process.py
--rw-rw-rw-   0        0        0     1567 2023-03-30 14:17:42.000000 pbrm-0.0.4/pbrm/config.py
--rw-rw-rw-   0        0        0      364 2023-03-30 14:07:02.000000 pbrm-0.0.4/pbrm/delete.py
--rw-rw-rw-   0        0        0      930 2023-03-30 12:40:35.000000 pbrm-0.0.4/pbrm/error.py
--rw-rw-rw-   0        0        0     1584 2023-03-31 13:32:04.000000 pbrm-0.0.4/pbrm/gif.py
--rw-rw-rw-   0        0        0     2197 2023-03-30 14:07:02.000000 pbrm-0.0.4/pbrm/main.py
--rw-rw-rw-   0        0        0     1072 2023-03-31 13:39:45.000000 pbrm-0.0.4/pbrm/pbrm_statistics.py
--rw-rw-rw-   0        0        0     3315 2023-03-31 10:55:19.000000 pbrm-0.0.4/pbrm/save_illust.py
-drwxrwxrwx   0        0        0        0 2023-03-31 13:40:05.297965 pbrm-0.0.4/pbrm/spider/
--rw-rw-rw-   0        0        0      213 2023-03-30 05:45:05.000000 pbrm-0.0.4/pbrm/spider/__init__.py
--rw-rw-rw-   0        0        0     1357 2023-03-30 14:19:07.000000 pbrm-0.0.4/pbrm/spider/cookie_verify.py
--rw-rw-rw-   0        0        0     1763 2023-03-30 14:31:52.000000 pbrm-0.0.4/pbrm/spider/get_bookmarks.py
--rw-rw-rw-   0        0        0     1922 2023-03-30 05:41:19.000000 pbrm-0.0.4/pbrm/spider/get_meta.py
--rw-rw-rw-   0        0        0     1099 2023-03-29 14:46:46.000000 pbrm-0.0.4/pbrm/spider/illust_download.py
--rw-rw-rw-   0        0        0     2954 2023-03-30 15:24:56.000000 pbrm-0.0.4/pbrm/update.py
--rw-rw-rw-   0        0        0      440 2023-03-30 05:25:55.000000 pbrm-0.0.4/pbrm/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-31 13:40:05.293343 pbrm-0.0.4/pbrm.egg-info/
--rw-rw-rw-   0        0        0      253 2023-03-31 13:40:05.000000 pbrm-0.0.4/pbrm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-03-31 13:40:05.000000 pbrm-0.0.4/pbrm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 13:40:05.000000 pbrm-0.0.4/pbrm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-03-31 13:40:05.000000 pbrm-0.0.4/pbrm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-03-31 13:40:05.000000 pbrm-0.0.4/pbrm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-31 13:40:05.000000 pbrm-0.0.4/pbrm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 13:40:05.300796 pbrm-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      496 2023-03-31 13:39:55.000000 pbrm-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:23:47.830129 pbrm-0.0.5/
+-rw-rw-rw-   0        0        0      269 2023-07-27 06:23:47.829145 pbrm-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1440 2023-07-27 06:13:33.000000 pbrm-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 06:23:47.811910 pbrm-0.0.5/pbrm/
+-rw-rw-rw-   0        0        0       22 2023-03-30 13:58:48.000000 pbrm-0.0.5/pbrm/__init__.py
+-rw-rw-rw-   0        0        0      165 2023-03-30 13:06:26.000000 pbrm-0.0.5/pbrm/change_repository.py
+-rw-rw-rw-   0        0        0     2906 2023-03-31 11:14:57.000000 pbrm-0.0.5/pbrm/command_process.py
+-rw-rw-rw-   0        0        0     1567 2023-03-30 14:17:42.000000 pbrm-0.0.5/pbrm/config.py
+-rw-rw-rw-   0        0        0      364 2023-03-30 14:07:02.000000 pbrm-0.0.5/pbrm/delete.py
+-rw-rw-rw-   0        0        0      930 2023-03-30 12:40:35.000000 pbrm-0.0.5/pbrm/error.py
+-rw-rw-rw-   0        0        0     1584 2023-03-31 13:32:04.000000 pbrm-0.0.5/pbrm/gif.py
+-rw-rw-rw-   0        0        0     2197 2023-03-30 14:07:02.000000 pbrm-0.0.5/pbrm/main.py
+-rw-rw-rw-   0        0        0     1556 2023-07-27 06:08:42.000000 pbrm-0.0.5/pbrm/pbrm_statistics.py
+-rw-rw-rw-   0        0        0     3315 2023-03-31 10:55:19.000000 pbrm-0.0.5/pbrm/save_illust.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:23:47.827129 pbrm-0.0.5/pbrm/spider/
+-rw-rw-rw-   0        0        0      213 2023-03-30 05:45:05.000000 pbrm-0.0.5/pbrm/spider/__init__.py
+-rw-rw-rw-   0        0        0     1357 2023-03-30 14:19:07.000000 pbrm-0.0.5/pbrm/spider/cookie_verify.py
+-rw-rw-rw-   0        0        0     1763 2023-03-30 14:31:52.000000 pbrm-0.0.5/pbrm/spider/get_bookmarks.py
+-rw-rw-rw-   0        0        0     1922 2023-03-30 05:41:19.000000 pbrm-0.0.5/pbrm/spider/get_meta.py
+-rw-rw-rw-   0        0        0     1099 2023-03-29 14:46:46.000000 pbrm-0.0.5/pbrm/spider/illust_download.py
+-rw-rw-rw-   0        0        0     3130 2023-07-27 06:04:22.000000 pbrm-0.0.5/pbrm/update.py
+-rw-rw-rw-   0        0        0      440 2023-03-30 05:25:55.000000 pbrm-0.0.5/pbrm/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:23:47.820188 pbrm-0.0.5/pbrm.egg-info/
+-rw-rw-rw-   0        0        0      269 2023-07-27 06:23:47.000000 pbrm-0.0.5/pbrm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-07-27 06:23:47.000000 pbrm-0.0.5/pbrm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 06:23:47.000000 pbrm-0.0.5/pbrm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-27 06:23:47.000000 pbrm-0.0.5/pbrm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-07-27 06:23:47.000000 pbrm-0.0.5/pbrm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-27 06:23:47.000000 pbrm-0.0.5/pbrm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 06:23:47.831127 pbrm-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      512 2023-07-27 06:20:18.000000 pbrm-0.0.5/setup.py
```

### Comparing `pbrm-0.0.4/pbrm/command_process.py` & `pbrm-0.0.5/pbrm/command_process.py`

 * *Files identical despite different names*

### Comparing `pbrm-0.0.4/pbrm/config.py` & `pbrm-0.0.5/pbrm/config.py`

 * *Files identical despite different names*

### Comparing `pbrm-0.0.4/pbrm/error.py` & `pbrm-0.0.5/pbrm/error.py`

 * *Files identical despite different names*

### Comparing `pbrm-0.0.4/pbrm/gif.py` & `pbrm-0.0.5/pbrm/gif.py`

 * *Files identical despite different names*

### Comparing `pbrm-0.0.4/pbrm/main.py` & `pbrm-0.0.5/pbrm/main.py`

 * *Files identical despite different names*

### Comparing `pbrm-0.0.4/pbrm/pbrm_statistics.py` & `pbrm-0.0.5/pbrm/pbrm_statistics.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,10 +23,22 @@
             with open(path + "/" + str(i["id"]) + "/meta.json", "r", encoding="utf-8") as f:
                 if json.loads(f.read())["userId"] != 0:
                     s.append(i["id"])
     return s
 
 
 def statistics_saved(path: str):
-    illusts = [f for f in os.listdir(path) if os.path.isdir(os.path.join(path, f))]
+    all_illusts = [f for f in os.listdir(path) if os.path.isdir(os.path.join(path, f))]
+    illusts = []
+
+    for single_illusts in all_illusts:
+        with open(os.path.join(path, single_illusts + "/meta.json")) as f:
+            meta = json.loads(f.read())
+            if meta["userId"] == 0:
+                continue
+            elif len(os.listdir(path + "/" + single_illusts)) >= (meta["pageCount"] + 4 if meta["illustType"] == 2 else meta["pageCount"] + 2):
+                illusts.append(single_illusts)
+            else:
+                continue
+
     return illusts
```

### Comparing `pbrm-0.0.4/pbrm/save_illust.py` & `pbrm-0.0.5/pbrm/save_illust.py`

 * *Files identical despite different names*

### Comparing `pbrm-0.0.4/pbrm/spider/cookie_verify.py` & `pbrm-0.0.5/pbrm/spider/cookie_verify.py`

 * *Files identical despite different names*

### Comparing `pbrm-0.0.4/pbrm/spider/get_bookmarks.py` & `pbrm-0.0.5/pbrm/spider/get_bookmarks.py`

 * *Files identical despite different names*

### Comparing `pbrm-0.0.4/pbrm/spider/get_meta.py` & `pbrm-0.0.5/pbrm/spider/get_meta.py`

 * *Files identical despite different names*

### Comparing `pbrm-0.0.4/pbrm/spider/illust_download.py` & `pbrm-0.0.5/pbrm/spider/illust_download.py`

 * *Files identical despite different names*

### Comparing `pbrm-0.0.4/pbrm/update.py` & `pbrm-0.0.5/pbrm/update.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 from pbrm import spider
 from pbrm import save_illust
 from pbrm import utils
 import os
 from pbrm import delete
 
 
-def work_exists(pid: str, path: str, unavailable: bool):
+def work_exists(pid: str, path: str, unavailable: bool, is_gif: bool, num: int):
     if os.path.exists(path + "/" + pid) and os.path.isdir(path + "/" + pid):
-        if len(os.listdir(path + "/" + pid)) > (1 if unavailable else 2):
+        # 判断是否保存完全(防止因网络原因导致的下载中断)
+        if len(os.listdir(path + "/" + pid)) >= (1 if unavailable else (num + 4 if is_gif else num + 2)):
             return True
         else:
             return False
 
     return False
 
 
@@ -61,12 +62,12 @@
     if auto_remove:
         illusts = [f for f in os.listdir(path) if os.path.isdir(os.path.join(path, f))]
         for i in illusts:
             if i not in all_illust:
                 delete.delete(os.path.join(path, i))
 
     with open(os.path.join(path, "log.json"), "w", encoding="utf-8") as f:
-        f.write(json.dumps(log))
+        f.write(json.dumps(log, ensure_ascii=False))
 
     with open(os.path.join(path, "bookmarks.json"), "w", encoding="utf-8") as f:
-        f.write(json.dumps(bookmarks))
+        f.write(json.dumps(bookmarks, ensure_ascii=False))
```

### Comparing `pbrm-0.0.4/pbrm.egg-info/SOURCES.txt` & `pbrm-0.0.5/pbrm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

