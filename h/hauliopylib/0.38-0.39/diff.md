# Comparing `tmp/hauliopylib-0.38.tar.gz` & `tmp/hauliopylib-0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hauliopylib-0.38.tar", last modified: Thu Jan  5 07:14:38 2023, max compression
+gzip compressed data, was "dist/hauliopylib-0.39.tar", last modified: Thu Jul 27 11:08:29 2023, max compression
```

## Comparing `hauliopylib-0.38.tar` & `hauliopylib-0.39.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-01-05 07:14:38.000000 hauliopylib-0.38/
--rw-r--r--   0 liming     (501) staff       (20)      487 2023-01-05 07:14:38.000000 hauliopylib-0.38/PKG-INFO
--rw-r--r--   0 liming     (501) staff       (20)      167 2020-07-08 14:24:54.000000 hauliopylib-0.38/README.md
-drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-01-05 07:14:38.000000 hauliopylib-0.38/hauliopylib/
--rw-r--r--   0 liming     (501) staff       (20)        0 2020-07-08 14:24:54.000000 hauliopylib-0.38/hauliopylib/__init__.py
-drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-01-05 07:14:38.000000 hauliopylib-0.38/hauliopylib/geo/
--rw-r--r--   0 liming     (501) staff       (20)     1285 2022-09-16 08:03:23.000000 hauliopylib-0.38/hauliopylib/geo/__init__.py
--rw-r--r--   0 liming     (501) staff       (20)    93213 2022-07-20 08:52:45.000000 hauliopylib-0.38/hauliopylib/geo/sg.py
--rw-r--r--   0 liming     (501) staff       (20)    42285 2022-11-15 02:42:31.000000 hauliopylib-0.38/hauliopylib/geo/th.py
--rw-r--r--   0 liming     (501) staff       (20)   118039 2023-01-05 07:14:17.000000 hauliopylib-0.38/hauliopylib/shared.py
--rw-r--r--   0 liming     (501) staff       (20)       21 2023-01-05 07:14:17.000000 hauliopylib-0.38/hauliopylib/version.py
-drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-01-05 07:14:38.000000 hauliopylib-0.38/hauliopylib.egg-info/
--rw-r--r--   0 liming     (501) staff       (20)      487 2023-01-05 07:14:37.000000 hauliopylib-0.38/hauliopylib.egg-info/PKG-INFO
--rw-r--r--   0 liming     (501) staff       (20)      299 2023-01-05 07:14:37.000000 hauliopylib-0.38/hauliopylib.egg-info/SOURCES.txt
--rw-r--r--   0 liming     (501) staff       (20)        1 2023-01-05 07:14:37.000000 hauliopylib-0.38/hauliopylib.egg-info/dependency_links.txt
--rw-r--r--   0 liming     (501) staff       (20)       12 2023-01-05 07:14:37.000000 hauliopylib-0.38/hauliopylib.egg-info/top_level.txt
--rw-r--r--   0 liming     (501) staff       (20)       38 2023-01-05 07:14:38.000000 hauliopylib-0.38/setup.cfg
--rw-r--r--   0 liming     (501) staff       (20)      855 2020-07-08 14:24:54.000000 hauliopylib-0.38/setup.py
+drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-07-27 11:08:29.000000 hauliopylib-0.39/
+-rw-r--r--   0 liming     (501) staff       (20)      487 2023-07-27 11:08:29.000000 hauliopylib-0.39/PKG-INFO
+-rw-r--r--   0 liming     (501) staff       (20)      167 2020-07-08 14:24:54.000000 hauliopylib-0.39/README.md
+drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-07-27 11:08:29.000000 hauliopylib-0.39/hauliopylib/
+-rw-r--r--   0 liming     (501) staff       (20)        0 2020-07-08 14:24:54.000000 hauliopylib-0.39/hauliopylib/__init__.py
+drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-07-27 11:08:29.000000 hauliopylib-0.39/hauliopylib/geo/
+-rw-r--r--   0 liming     (501) staff       (20)     1285 2022-09-16 08:03:23.000000 hauliopylib-0.39/hauliopylib/geo/__init__.py
+-rw-r--r--   0 liming     (501) staff       (20)    93219 2023-07-27 08:54:13.000000 hauliopylib-0.39/hauliopylib/geo/sg.py
+-rw-r--r--   0 liming     (501) staff       (20)    42285 2022-11-15 02:42:31.000000 hauliopylib-0.39/hauliopylib/geo/th.py
+-rw-r--r--   0 liming     (501) staff       (20)   118039 2023-01-05 07:14:17.000000 hauliopylib-0.39/hauliopylib/shared.py
+-rw-r--r--   0 liming     (501) staff       (20)       21 2023-07-27 11:06:44.000000 hauliopylib-0.39/hauliopylib/version.py
+drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-07-27 11:08:29.000000 hauliopylib-0.39/hauliopylib.egg-info/
+-rw-r--r--   0 liming     (501) staff       (20)      487 2023-07-27 11:08:29.000000 hauliopylib-0.39/hauliopylib.egg-info/PKG-INFO
+-rw-r--r--   0 liming     (501) staff       (20)      299 2023-07-27 11:08:29.000000 hauliopylib-0.39/hauliopylib.egg-info/SOURCES.txt
+-rw-r--r--   0 liming     (501) staff       (20)        1 2023-07-27 11:08:29.000000 hauliopylib-0.39/hauliopylib.egg-info/dependency_links.txt
+-rw-r--r--   0 liming     (501) staff       (20)       12 2023-07-27 11:08:29.000000 hauliopylib-0.39/hauliopylib.egg-info/top_level.txt
+-rw-r--r--   0 liming     (501) staff       (20)       38 2023-07-27 11:08:29.000000 hauliopylib-0.39/setup.cfg
+-rw-r--r--   0 liming     (501) staff       (20)      855 2020-07-08 14:24:54.000000 hauliopylib-0.39/setup.py
```

### Comparing `hauliopylib-0.38/hauliopylib/geo/__init__.py` & `hauliopylib-0.39/hauliopylib/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `hauliopylib-0.38/hauliopylib/geo/sg.py` & `hauliopylib-0.39/hauliopylib/geo/sg.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 LEVEL_SYNONYMS = "level|story|storey|floor|lv|basement"
 POSTAL_REGEX_CAPTURE = "(?i)" + ADDR_COMP_PRECEDING + "((?:Singapore|SG|S)?\s*[\(\-]?([0-9]{6})\)?)(?![0-9a-zA-Z\-/_])"
 BLOCK_PART_WSPACE_CAPTURE = "(?:BLOCK |BLK |BLOCK|BLK|[A-Z]{1,2})?\d+[A-Z]?(?:\s*[/\-]\s*(?:[A-Z]|\d+[A-Z]?)){0,2}(?:[\s,])"
 BLOCK_PART_DENSE_CAPTURE = "(?:BLOCK |BLK |BLOCK|BLK|[A-Z]{1,2})?(\d+[A-Z]?(?:[/\-](?:[A-Z]|\d+[A-Z]?)){0,2})(?:[\s,])"
 BLOCK_NUM_PART_DENSE_CAPTURE = "(?:BLOCK |BLK |BLOCK|BLK|[A-Z]{1,2})?(\d+(?:[/\-]\d+){0,2})(?:[\s,]?)"
 ROAD_NAME_PART = "(?:(?:lorong|lor)\s+\d{1,2}|[A-Z|']+(?:\s+[A-Z|']+)*)\s+"
 ROAD_SUFFIX_PART = "\s?(?:\d{1,3}|III|II|I)"
-BLOCK_STREET_REGEX1a = "(?i)" + ADDR_COMP_PRECEDING + "(?:" + BLOCK_PART_DENSE_CAPTURE + "|" + BLOCK_NUM_PART_DENSE_CAPTURE + ")[\s,]*(" + ROAD_NAME_PART + "(?:" + ROAD_SYNONYMS + ")(?:" + ROAD_SUFFIX_PART + ")?)(?:[\s\(\)\.,]|$)"
-BLOCK_STREET_REGEX1b = "(?i)" + ADDR_COMP_PRECEDING + "(" + ROAD_NAME_PART + "(?:" + ROAD_SYNONYMS + ")(?:" + ROAD_SUFFIX_PART + ")?)(?:[\s\(\)\.,]|$)"
-BLOCK_STREET_REGEX2a = "(?i)" + ADDR_COMP_PRECEDING + "(?:" + BLOCK_PART_DENSE_CAPTURE + "|" + BLOCK_NUM_PART_DENSE_CAPTURE + ")[\s,]*((?:" + ROAD_NAME_PART + ")?(?:jalan|jln|lorong|lor|mount|pulau)(?:\s+[A-Z]+)*(?:" + ROAD_SUFFIX_PART + ")?)(?:[\s\(\)\.,]|$)"
-BLOCK_STREET_REGEX2b = "(?i)" + ADDR_COMP_PRECEDING + "((?:" + ROAD_NAME_PART + ")?(?:jalan|jln|lorong|lor|mount|pulau)(?:\s+[A-Z]+)*(?:" + ROAD_SUFFIX_PART + ")?)(?:[\s\(\)\.,]|$)"
-BLOCK_STREET_REGEX3 = "(?i)" + ADDR_COMP_PRECEDING + "(?:" + BLOCK_PART_DENSE_CAPTURE + "|" + BLOCK_NUM_PART_DENSE_CAPTURE + ")?[\s,]*(" + EXACT_ROAD_NAMES + ")(?:[\s\(\)\.,]|$)"
-BLOCK_STREET_REGEX4 = "(?i)" + ADDR_COMP_PRECEDING + "(?:" + BLOCK_PART_DENSE_CAPTURE + "|" + BLOCK_NUM_PART_DENSE_CAPTURE + ")?[\s,]*(" + ROAD_NAME_PART + "(?:" + PARK_SYNONYMS + ")(?:" + ROAD_SUFFIX_PART + ")?)(?:[\s\(\)\.,]|$)"
+BLOCK_STREET_REGEX1a = "(?i)" + ADDR_COMP_PRECEDING + "(?:" + BLOCK_PART_DENSE_CAPTURE + "|" + BLOCK_NUM_PART_DENSE_CAPTURE + ")[\s,]*(" + ROAD_NAME_PART + "(?:" + ROAD_SYNONYMS + ")(?:" + ROAD_SUFFIX_PART + ")?)(?:[\s\(\)\.,#]|$)"
+BLOCK_STREET_REGEX1b = "(?i)" + ADDR_COMP_PRECEDING + "(" + ROAD_NAME_PART + "(?:" + ROAD_SYNONYMS + ")(?:" + ROAD_SUFFIX_PART + ")?)(?:[\s\(\)\.,#]|$)"
+BLOCK_STREET_REGEX2a = "(?i)" + ADDR_COMP_PRECEDING + "(?:" + BLOCK_PART_DENSE_CAPTURE + "|" + BLOCK_NUM_PART_DENSE_CAPTURE + ")[\s,]*((?:" + ROAD_NAME_PART + ")?(?:jalan|jln|lorong|lor|mount|pulau)(?:\s+[A-Z]+)*(?:" + ROAD_SUFFIX_PART + ")?)(?:[\s\(\)\.,#]|$)"
+BLOCK_STREET_REGEX2b = "(?i)" + ADDR_COMP_PRECEDING + "((?:" + ROAD_NAME_PART + ")?(?:jalan|jln|lorong|lor|mount|pulau)(?:\s+[A-Z]+)*(?:" + ROAD_SUFFIX_PART + ")?)(?:[\s\(\)\.,#]|$)"
+BLOCK_STREET_REGEX3 = "(?i)" + ADDR_COMP_PRECEDING + "(?:" + BLOCK_PART_DENSE_CAPTURE + "|" + BLOCK_NUM_PART_DENSE_CAPTURE + ")?[\s,]*(" + EXACT_ROAD_NAMES + ")(?:[\s\(\)\.,#]|$)"
+BLOCK_STREET_REGEX4 = "(?i)" + ADDR_COMP_PRECEDING + "(?:" + BLOCK_PART_DENSE_CAPTURE + "|" + BLOCK_NUM_PART_DENSE_CAPTURE + ")?[\s,]*(" + ROAD_NAME_PART + "(?:" + PARK_SYNONYMS + ")(?:" + ROAD_SUFFIX_PART + ")?)(?:[\s\(\)\.,#]|$)"
 CORE_UNIT_PART = "B?\d+[A-Z]?\d?(?:[\-/]B?\d*[A-Z]?\d?){0,9}"
 UNIT_PART_REGEX = "(?:unit\s|suite\s|#)" + CORE_UNIT_PART + "(?:\s?/\s?#" + CORE_UNIT_PART + "){0,5}"
 UNIT_BUILDING_REGEX = "(?i)" + ADDR_COMP_PRECEDING + "(" + UNIT_PART_REGEX + ")(?:([\s,].*)|$)"
 LEVEL_SUFFIX_PART = "\s+B?\d+[A-Za-z]?"
 LEVEL_BUILDING_REGEX = "(?i)" + ADDR_COMP_PRECEDING + "((?:\d+(?:st|nd|rd|th)\s+)?(?:" + LEVEL_SYNONYMS + ")(?:" + LEVEL_SUFFIX_PART + ")?)(?:([\s,].*)|$)"
 MAILBOX_BUILDING_REGEX = "(?i)" + ADDR_COMP_PRECEDING + "(?:mail\sbox|mailbox|box)\s+\d+(?:([\s,].+)|$)"
```

### Comparing `hauliopylib-0.38/hauliopylib/geo/th.py` & `hauliopylib-0.39/hauliopylib/geo/th.py`

 * *Files identical despite different names*

### Comparing `hauliopylib-0.38/hauliopylib/shared.py` & `hauliopylib-0.39/hauliopylib/shared.py`

 * *Files identical despite different names*

### Comparing `hauliopylib-0.38/setup.py` & `hauliopylib-0.39/setup.py`

 * *Files identical despite different names*

