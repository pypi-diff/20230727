# Comparing `tmp/s1290080_learn-1.0.0.tar.gz` & `tmp/s1290080_learn-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s1290080_learn-1.0.0.tar", last modified: Thu Jul 27 10:37:28 2023, max compression
+gzip compressed data, was "s1290080_learn-1.0.1.tar", last modified: Thu Jul 27 11:05:07 2023, max compression
```

## Comparing `s1290080_learn-1.0.0.tar` & `s1290080_learn-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 10:37:28.603214 s1290080_learn-1.0.0/
--rw-rw-rw-   0        0        0     1087 2023-07-27 10:28:27.000000 s1290080_learn-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0       88 2023-07-27 10:37:28.602259 s1290080_learn-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 10:37:28.578994 s1290080_learn-1.0.0/s1290080_learn/
--rw-rw-rw-   0        0        0        0 2023-07-27 10:10:11.000000 s1290080_learn-1.0.0/s1290080_learn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:37:28.596104 s1290080_learn-1.0.0/s1290080_learn/statistics/
--rw-rw-rw-   0        0        0        0 2023-07-27 10:10:11.000000 s1290080_learn-1.0.0/s1290080_learn/statistics/__init__.py
--rw-rw-rw-   0        0        0      678 2023-07-27 10:10:15.000000 s1290080_learn-1.0.0/s1290080_learn/statistics/frequenciesOfItems.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:37:28.599213 s1290080_learn-1.0.0/s1290080_learn/visualization/
--rw-rw-rw-   0        0        0        0 2023-07-27 10:10:11.000000 s1290080_learn-1.0.0/s1290080_learn/visualization/__init__.py
--rw-rw-rw-   0        0        0      945 2023-07-27 10:13:12.000000 s1290080_learn-1.0.0/s1290080_learn/visualization/heatMapItemsFrequencies.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:37:28.590723 s1290080_learn-1.0.0/s1290080_learn.egg-info/
--rw-rw-rw-   0        0        0       88 2023-07-27 10:37:28.000000 s1290080_learn-1.0.0/s1290080_learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-07-27 10:37:28.000000 s1290080_learn-1.0.0/s1290080_learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 10:37:28.000000 s1290080_learn-1.0.0/s1290080_learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-27 10:37:28.000000 s1290080_learn-1.0.0/s1290080_learn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-27 10:37:28.000000 s1290080_learn-1.0.0/s1290080_learn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 10:37:28.603214 s1290080_learn-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      160 2023-07-27 10:28:27.000000 s1290080_learn-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:05:07.578410 s1290080_learn-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2023-07-27 10:28:27.000000 s1290080_learn-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      112 2023-07-27 11:05:07.577409 s1290080_learn-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 11:05:07.548268 s1290080_learn-1.0.1/s1290080_learn/
+-rw-rw-rw-   0        0        0        0 2023-07-27 10:10:11.000000 s1290080_learn-1.0.1/s1290080_learn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:05:07.564531 s1290080_learn-1.0.1/s1290080_learn/statistics/
+-rw-rw-rw-   0        0        0        0 2023-07-27 10:10:11.000000 s1290080_learn-1.0.1/s1290080_learn/statistics/__init__.py
+-rw-rw-rw-   0        0        0      678 2023-07-27 10:10:15.000000 s1290080_learn-1.0.1/s1290080_learn/statistics/frequenciesOfItems.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:05:07.574892 s1290080_learn-1.0.1/s1290080_learn/visualization/
+-rw-rw-rw-   0        0        0        0 2023-07-27 10:10:11.000000 s1290080_learn-1.0.1/s1290080_learn/visualization/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-07-27 10:13:12.000000 s1290080_learn-1.0.1/s1290080_learn/visualization/heatMapItemsFrequencies.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:05:07.559530 s1290080_learn-1.0.1/s1290080_learn.egg-info/
+-rw-rw-rw-   0        0        0      112 2023-07-27 11:05:07.000000 s1290080_learn-1.0.1/s1290080_learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-07-27 11:05:07.000000 s1290080_learn-1.0.1/s1290080_learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:05:07.000000 s1290080_learn-1.0.1/s1290080_learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-27 11:05:07.000000 s1290080_learn-1.0.1/s1290080_learn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-27 11:05:07.000000 s1290080_learn-1.0.1/s1290080_learn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:05:07.579408 s1290080_learn-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      186 2023-07-27 11:04:16.000000 s1290080_learn-1.0.1/setup.py
```

### Comparing `s1290080_learn-1.0.0/LICENSE.txt` & `s1290080_learn-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `s1290080_learn-1.0.0/s1290080_learn/statistics/frequenciesOfItems.py` & `s1290080_learn-1.0.1/s1290080_learn/statistics/frequenciesOfItems.py`

 * *Files identical despite different names*

### Comparing `s1290080_learn-1.0.0/s1290080_learn/visualization/heatMapItemsFrequencies.py` & `s1290080_learn-1.0.1/s1290080_learn/visualization/heatMapItemsFrequencies.py`

 * *Files identical despite different names*

