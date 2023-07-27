# Comparing `tmp/DeepLScrapper-1.0.0.tar.gz` & `tmp/DeepLScrapper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepLScrapper-1.0.0.tar", last modified: Thu Jul 27 18:29:35 2023, max compression
+gzip compressed data, was "DeepLScrapper-1.0.1.tar", last modified: Thu Jul 27 18:52:33 2023, max compression
```

## Comparing `DeepLScrapper-1.0.0.tar` & `DeepLScrapper-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 ochotzas   (501) staff       (20)        0 2023-07-27 18:29:35.600221 DeepLScrapper-1.0.0/
-drwxr-xr-x   0 ochotzas   (501) staff       (20)        0 2023-07-27 18:29:35.599884 DeepLScrapper-1.0.0/DeepLScrapper.egg-info/
--rw-r--r--   0 ochotzas   (501) staff       (20)      149 2023-07-27 18:29:35.000000 DeepLScrapper-1.0.0/DeepLScrapper.egg-info/PKG-INFO
--rw-r--r--   0 ochotzas   (501) staff       (20)      192 2023-07-27 18:29:35.000000 DeepLScrapper-1.0.0/DeepLScrapper.egg-info/SOURCES.txt
--rw-r--r--   0 ochotzas   (501) staff       (20)        1 2023-07-27 18:29:35.000000 DeepLScrapper-1.0.0/DeepLScrapper.egg-info/dependency_links.txt
--rw-r--r--   0 ochotzas   (501) staff       (20)       39 2023-07-27 18:29:35.000000 DeepLScrapper-1.0.0/DeepLScrapper.egg-info/requires.txt
--rw-r--r--   0 ochotzas   (501) staff       (20)        1 2023-07-27 18:29:35.000000 DeepLScrapper-1.0.0/DeepLScrapper.egg-info/top_level.txt
--rw-r--r--   0 ochotzas   (501) staff       (20)      149 2023-07-27 18:29:35.600102 DeepLScrapper-1.0.0/PKG-INFO
--rw-r--r--   0 ochotzas   (501) staff       (20)       38 2023-07-27 18:29:35.600282 DeepLScrapper-1.0.0/setup.cfg
--rw-r--r--   0 ochotzas   (501) staff       (20)      341 2023-07-27 18:09:31.000000 DeepLScrapper-1.0.0/setup.py
+drwxr-xr-x   0 ochotzas   (501) staff       (20)        0 2023-07-27 18:52:33.050027 DeepLScrapper-1.0.1/
+drwxr-xr-x   0 ochotzas   (501) staff       (20)        0 2023-07-27 18:52:33.049608 DeepLScrapper-1.0.1/DeepLScrapper.egg-info/
+-rw-r--r--   0 ochotzas   (501) staff       (20)      149 2023-07-27 18:52:33.000000 DeepLScrapper-1.0.1/DeepLScrapper.egg-info/PKG-INFO
+-rw-r--r--   0 ochotzas   (501) staff       (20)      202 2023-07-27 18:52:33.000000 DeepLScrapper-1.0.1/DeepLScrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 ochotzas   (501) staff       (20)        1 2023-07-27 18:52:33.000000 DeepLScrapper-1.0.1/DeepLScrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 ochotzas   (501) staff       (20)       39 2023-07-27 18:52:33.000000 DeepLScrapper-1.0.1/DeepLScrapper.egg-info/requires.txt
+-rw-r--r--   0 ochotzas   (501) staff       (20)        1 2023-07-27 18:52:33.000000 DeepLScrapper-1.0.1/DeepLScrapper.egg-info/top_level.txt
+-rw-r--r--   0 ochotzas   (501) staff       (20)      149 2023-07-27 18:52:33.049822 DeepLScrapper-1.0.1/PKG-INFO
+-rw-r--r--   0 ochotzas   (501) staff       (20)     4706 2023-07-27 18:50:30.000000 DeepLScrapper-1.0.1/README.md
+-rw-r--r--   0 ochotzas   (501) staff       (20)       38 2023-07-27 18:52:33.050083 DeepLScrapper-1.0.1/setup.cfg
+-rw-r--r--   0 ochotzas   (501) staff       (20)      341 2023-07-27 18:51:16.000000 DeepLScrapper-1.0.1/setup.py
```

