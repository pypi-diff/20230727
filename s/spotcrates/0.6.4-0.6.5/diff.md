# Comparing `tmp/spotcrates-0.6.4.tar.gz` & `tmp/spotcrates-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotcrates-0.6.4.tar", max compression
+gzip compressed data, was "spotcrates-0.6.5.tar", max compression
```

## Comparing `spotcrates-0.6.4.tar` & `spotcrates-0.6.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-06-10 20:26:58.614364 spotcrates-0.6.4/LICENSE
--rw-r--r--   0        0        0    11842 2023-06-10 20:26:58.614364 spotcrates-0.6.4/README.md
--rw-r--r--   0        0        0      792 2023-06-11 03:41:03.306695 spotcrates-0.6.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-10 20:26:59.810367 spotcrates-0.6.4/spotcrates/__init__.py
--rw-r--r--   0        0        0    10264 2023-06-11 03:07:12.056616 spotcrates-0.6.4/spotcrates/cli.py
--rw-r--r--   0        0        0     2557 2023-06-10 23:12:51.552434 spotcrates-0.6.4/spotcrates/common.py
--rw-r--r--   0        0        0     9707 2023-06-10 23:13:05.032468 spotcrates-0.6.4/spotcrates/filters.py
--rw-r--r--   0        0        0    16425 2023-06-11 02:35:29.291569 spotcrates-0.6.4/spotcrates/playlists.py
--rw-r--r--   0        0        0      401 2023-06-10 20:26:59.810367 spotcrates-0.6.4/spotcrates/templates/auth_index.html
--rw-r--r--   0        0        0      173 2023-06-10 20:26:59.810367 spotcrates-0.6.4/spotcrates/templates/base.html
--rw-r--r--   0        0        0      150 2023-06-10 20:26:59.810367 spotcrates-0.6.4/spotcrates/templates/index.html
--rw-r--r--   0        0        0    12594 1970-01-01 00:00:00.000000 spotcrates-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-10 20:26:58.614364 spotcrates-0.6.5/LICENSE
+-rw-r--r--   0        0        0    11842 2023-06-10 20:26:58.614364 spotcrates-0.6.5/README.md
+-rw-r--r--   0        0        0      750 2023-07-27 00:36:19.272129 spotcrates-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-10 20:26:59.810367 spotcrates-0.6.5/spotcrates/__init__.py
+-rw-r--r--   0        0        0    10264 2023-06-11 03:07:12.056616 spotcrates-0.6.5/spotcrates/cli.py
+-rw-r--r--   0        0        0     2557 2023-07-23 16:11:26.985012 spotcrates-0.6.5/spotcrates/common.py
+-rw-r--r--   0        0        0     9707 2023-06-10 23:13:05.032468 spotcrates-0.6.5/spotcrates/filters.py
+-rw-r--r--   0        0        0    16553 2023-07-27 00:27:30.499578 spotcrates-0.6.5/spotcrates/playlists.py
+-rw-r--r--   0        0        0      401 2023-06-10 20:26:59.810367 spotcrates-0.6.5/spotcrates/templates/auth_index.html
+-rw-r--r--   0        0        0      173 2023-06-10 20:26:59.810367 spotcrates-0.6.5/spotcrates/templates/base.html
+-rw-r--r--   0        0        0      150 2023-06-10 20:26:59.810367 spotcrates-0.6.5/spotcrates/templates/index.html
+-rw-r--r--   0        0        0    12510 1970-01-01 00:00:00.000000 spotcrates-0.6.5/PKG-INFO
```

### Comparing `spotcrates-0.6.4/LICENSE` & `spotcrates-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spotcrates-0.6.4/README.md` & `spotcrates-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `spotcrates-0.6.4/pyproject.toml` & `spotcrates-0.6.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 [tool.poetry]
 name = "spotcrates"
-version = "0.6.4"
+version = "0.6.5"
 description = ""
 authors = ["Chris Mayes <cmayes@cmay.es>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 jinja2 = "^3.1.2"
 spotipy = "^2.22.1"
-flask-session = "^0.4.0"
 appdirs = "^1.4.4"
 pygtrie = "^2.5.0"
 types-appdirs = "^1.4.3.5"
 durations-nlp = "^1.0.1"
 tomli-w = "^1.0.0"
 tomli = "^2.0.1"
-redis = "^4.5.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 coverage = {extras = ["toml"], version = "^7.0.1"}
 flake8 = "^6.0.0"
 flake8-bugbear = "^22.12.6"
 mypy = "^0.991"
```

### Comparing `spotcrates-0.6.4/spotcrates/cli.py` & `spotcrates-0.6.5/spotcrates/cli.py`

 * *Files identical despite different names*

### Comparing `spotcrates-0.6.4/spotcrates/common.py` & `spotcrates-0.6.5/spotcrates/common.py`

 * *Files identical despite different names*

### Comparing `spotcrates-0.6.4/spotcrates/filters.py` & `spotcrates-0.6.5/spotcrates/filters.py`

 * *Files identical despite different names*

### Comparing `spotcrates-0.6.4/spotcrates/playlists.py` & `spotcrates-0.6.5/spotcrates/playlists.py`

 * *Files 3% similar despite different names*

```diff
@@ -320,18 +320,16 @@
             f"Found a total of {len(target_playlist_ids)} newer than {oldest_timestamp}"
         )
         return target_playlist_ids
 
     def _get_playlist_track_ids(self, *args: str) -> Set[str]:
         track_ids: Set[str] = set([])
         for playlist_id in args:
-            # TODO: See about paring down to just the ID via "fields" param
-            playlist_items = get_all_items(
-                self.spotify, self.spotify.playlist_items(playlist_id)
-            )
+            playlist_items = self._filter_for_tracks(playlist_id)
+
             track_ids.update(
                 {playlist_item.get("track", {}).get("id") for playlist_item in playlist_items}
             )
 
         # Remove None in case any IDs failed to resolve
         with suppress(KeyError):
             # noinspection PyTypeChecker
@@ -358,21 +356,28 @@
             else:
                 self.logger.warning(f"No playlist found for name '{lower_name}'")
         return self._get_playlist_id_tracks(*playlist_ids)
 
     def _get_playlist_id_tracks(self, *playlist_ids: str) -> List[dict]:
         tracks = []
         for playlist_id in playlist_ids:
-            # TODO: See about paring down to just the ID via "fields" param
-            tracks.extend(
-                get_all_items(self.spotify, self.spotify.playlist_items(playlist_id))
-            )
+            filtered_tracks = self._filter_for_tracks(playlist_id)
+
+            tracks.extend(filtered_tracks)
 
         return tracks
 
+    def _filter_for_tracks(self, playlist_id):
+        all_tracks = get_all_items(self.spotify, self.spotify.playlist_items(playlist_id))
+        filtered_tracks = []
+        for cur_track in all_tracks:
+            if cur_track.get('track') and cur_track['track'].get('id'):
+                filtered_tracks.append(cur_track)
+        return filtered_tracks
+
     def _add_tracks_to_playlist(self, target_list:Dict[str, Any], add_tracks: List, replace_playlist=False):
         track_ids = {add_song["track"]["id"] for add_song in add_tracks}
 
         first_batch = True
         for id_batch in batched(track_ids, 100):
             if replace_playlist and first_batch:
                 self.spotify.playlist_replace_items(target_list["id"], id_batch)
```

### Comparing `spotcrates-0.6.4/PKG-INFO` & `spotcrates-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: spotcrates
-Version: 0.6.4
+Version: 0.6.5
 Summary: 
 Author: Chris Mayes
 Author-email: cmayes@cmay.es
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: durations-nlp (>=1.0.1,<2.0.0)
-Requires-Dist: flask-session (>=0.4.0,<0.5.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pygtrie (>=2.5.0,<3.0.0)
-Requires-Dist: redis (>=4.5.3,<5.0.0)
 Requires-Dist: spotipy (>=2.22.1,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
 Requires-Dist: types-appdirs (>=1.4.3.5,<2.0.0.0)
 Description-Content-Type: text/markdown
 
 # Spotcrates
```

