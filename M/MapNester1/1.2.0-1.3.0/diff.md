# Comparing `tmp/MapNester1-1.2.0.tar.gz` & `tmp/MapNester1-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MapNester1-1.2.0.tar", last modified: Thu Jul 27 13:26:49 2023, max compression
+gzip compressed data, was "MapNester1-1.3.0.tar", last modified: Thu Jul 27 13:55:19 2023, max compression
```

## Comparing `MapNester1-1.2.0.tar` & `MapNester1-1.3.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 13:26:49.117576 MapNester1-1.2.0/
--rw-rw-rw-   0        0        0      238 2023-07-27 13:26:49.117576 MapNester1-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-07-27 13:25:35.487289 MapNester1-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 13:55:19.800538 MapNester1-1.3.0/
+-rw-rw-rw-   0        0        0      238 2023-07-27 13:55:19.801539 MapNester1-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-07-27 13:50:25.217050 MapNester1-1.3.0/setup.py
```

