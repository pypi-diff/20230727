# Comparing `tmp/youtube-transcriber1-1.0.0.tar.gz` & `tmp/youtube-transcriber1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube-transcriber1-1.0.0.tar", last modified: Thu Jul 27 04:27:47 2023, max compression
+gzip compressed data, was "youtube-transcriber1-1.1.0.tar", last modified: Thu Jul 27 19:08:37 2023, max compression
```

## Comparing `youtube-transcriber1-1.0.0.tar` & `youtube-transcriber1-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 akram      (501) staff       (20)        0 2023-07-27 04:27:47.299451 youtube-transcriber1-1.0.0/
--rw-r--r--   0 akram      (501) staff       (20)       64 2023-07-27 04:27:47.298093 youtube-transcriber1-1.0.0/PKG-INFO
--rw-r--r--   0 akram      (501) staff       (20)       38 2023-07-27 04:27:47.299867 youtube-transcriber1-1.0.0/setup.cfg
--rw-r--r--   0 akram      (501) staff       (20)      347 2023-07-27 04:24:44.000000 youtube-transcriber1-1.0.0/setup.py
-drwxr-xr-x   0 akram      (501) staff       (20)        0 2023-07-27 04:27:47.289823 youtube-transcriber1-1.0.0/youtube_transcriber/
--rw-r--r--   0 akram      (501) staff       (20)        0 2023-07-27 02:43:20.000000 youtube-transcriber1-1.0.0/youtube_transcriber/__init__.py
-drwxr-xr-x   0 akram      (501) staff       (20)        0 2023-07-27 04:27:47.290972 youtube-transcriber1-1.0.0/youtube_transcriber/gui/
--rw-r--r--   0 akram      (501) staff       (20)        0 2023-07-27 02:43:07.000000 youtube-transcriber1-1.0.0/youtube_transcriber/gui/__init__.py
--rw-r--r--   0 akram      (501) staff       (20)     2265 2023-07-27 02:54:43.000000 youtube-transcriber1-1.0.0/youtube_transcriber/gui/transcriber.py
--rw-r--r--   0 akram      (501) staff       (20)      217 2023-07-27 02:46:14.000000 youtube-transcriber1-1.0.0/youtube_transcriber/main.py
--rw-r--r--   0 akram      (501) staff       (20)      327 2023-07-27 04:26:34.000000 youtube-transcriber1-1.0.0/youtube_transcriber/setup.py
-drwxr-xr-x   0 akram      (501) staff       (20)        0 2023-07-27 04:27:47.296544 youtube-transcriber1-1.0.0/youtube_transcriber1.egg-info/
--rw-r--r--   0 akram      (501) staff       (20)       64 2023-07-27 04:27:47.000000 youtube-transcriber1-1.0.0/youtube_transcriber1.egg-info/PKG-INFO
--rw-r--r--   0 akram      (501) staff       (20)      438 2023-07-27 04:27:47.000000 youtube-transcriber1-1.0.0/youtube_transcriber1.egg-info/SOURCES.txt
--rw-r--r--   0 akram      (501) staff       (20)        1 2023-07-27 04:27:47.000000 youtube-transcriber1-1.0.0/youtube_transcriber1.egg-info/dependency_links.txt
--rw-r--r--   0 akram      (501) staff       (20)       70 2023-07-27 04:27:47.000000 youtube-transcriber1-1.0.0/youtube_transcriber1.egg-info/entry_points.txt
--rw-r--r--   0 akram      (501) staff       (20)       15 2023-07-27 04:27:47.000000 youtube-transcriber1-1.0.0/youtube_transcriber1.egg-info/requires.txt
--rw-r--r--   0 akram      (501) staff       (20)       20 2023-07-27 04:27:47.000000 youtube-transcriber1-1.0.0/youtube_transcriber1.egg-info/top_level.txt
+drwxr-xr-x   0 akram      (501) staff       (20)        0 2023-07-27 19:08:37.950135 youtube-transcriber1-1.1.0/
+-rw-r--r--   0 akram      (501) staff       (20)       64 2023-07-27 19:08:37.949241 youtube-transcriber1-1.1.0/PKG-INFO
+-rw-r--r--   0 akram      (501) staff       (20)       38 2023-07-27 19:08:37.950359 youtube-transcriber1-1.1.0/setup.cfg
+-rw-r--r--   0 akram      (501) staff       (20)      347 2023-07-27 19:08:01.000000 youtube-transcriber1-1.1.0/setup.py
+drwxr-xr-x   0 akram      (501) staff       (20)        0 2023-07-27 19:08:37.940811 youtube-transcriber1-1.1.0/youtube_transcriber/
+-rw-r--r--   0 akram      (501) staff       (20)        0 2023-07-27 02:43:20.000000 youtube-transcriber1-1.1.0/youtube_transcriber/__init__.py
+drwxr-xr-x   0 akram      (501) staff       (20)        0 2023-07-27 19:08:37.942615 youtube-transcriber1-1.1.0/youtube_transcriber/gui/
+-rw-r--r--   0 akram      (501) staff       (20)        0 2023-07-27 02:43:07.000000 youtube-transcriber1-1.1.0/youtube_transcriber/gui/__init__.py
+-rw-r--r--   0 akram      (501) staff       (20)     3081 2023-07-27 19:05:07.000000 youtube-transcriber1-1.1.0/youtube_transcriber/gui/transcriber.py
+-rw-r--r--   0 akram      (501) staff       (20)      217 2023-07-27 02:46:14.000000 youtube-transcriber1-1.1.0/youtube_transcriber/main.py
+-rw-r--r--   0 akram      (501) staff       (20)      327 2023-07-27 04:26:34.000000 youtube-transcriber1-1.1.0/youtube_transcriber/setup.py
+drwxr-xr-x   0 akram      (501) staff       (20)        0 2023-07-27 19:08:37.947572 youtube-transcriber1-1.1.0/youtube_transcriber1.egg-info/
+-rw-r--r--   0 akram      (501) staff       (20)       64 2023-07-27 19:08:37.000000 youtube-transcriber1-1.1.0/youtube_transcriber1.egg-info/PKG-INFO
+-rw-r--r--   0 akram      (501) staff       (20)      438 2023-07-27 19:08:37.000000 youtube-transcriber1-1.1.0/youtube_transcriber1.egg-info/SOURCES.txt
+-rw-r--r--   0 akram      (501) staff       (20)        1 2023-07-27 19:08:37.000000 youtube-transcriber1-1.1.0/youtube_transcriber1.egg-info/dependency_links.txt
+-rw-r--r--   0 akram      (501) staff       (20)       70 2023-07-27 19:08:37.000000 youtube-transcriber1-1.1.0/youtube_transcriber1.egg-info/entry_points.txt
+-rw-r--r--   0 akram      (501) staff       (20)       15 2023-07-27 19:08:37.000000 youtube-transcriber1-1.1.0/youtube_transcriber1.egg-info/requires.txt
+-rw-r--r--   0 akram      (501) staff       (20)       20 2023-07-27 19:08:37.000000 youtube-transcriber1-1.1.0/youtube_transcriber1.egg-info/top_level.txt
```

