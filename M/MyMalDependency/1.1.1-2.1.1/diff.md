# Comparing `tmp/MyMalDependency-1.1.1.tar.gz` & `tmp/MyMalDependency-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MyMalDependency-1.1.1.tar", last modified: Thu Jul 27 02:53:48 2023, max compression
+gzip compressed data, was "dist\MyMalDependency-2.1.1.tar", last modified: Thu Jul 27 08:09:03 2023, max compression
```

## Comparing `MyMalDependency-1.1.1.tar` & `MyMalDependency-2.1.1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 02:53:48.000000 MyMalDependency-1.1.1/
-drwxrwxrwx   0        0        0        0 2023-07-27 02:53:48.000000 MyMalDependency-1.1.1/MyMalDependency.egg-info/
--rw-rw-rw-   0        0        0      208 2023-07-27 02:53:47.000000 MyMalDependency-1.1.1/MyMalDependency.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      164 2023-07-27 02:53:47.000000 MyMalDependency-1.1.1/MyMalDependency.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 02:53:47.000000 MyMalDependency-1.1.1/MyMalDependency.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 02:53:47.000000 MyMalDependency-1.1.1/MyMalDependency.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      208 2023-07-27 02:53:48.000000 MyMalDependency-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-27 02:53:48.000000 MyMalDependency-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      283 2023-07-27 02:53:42.000000 MyMalDependency-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:09:03.000000 MyMalDependency-2.1.1/
+drwxrwxrwx   0        0        0        0 2023-07-27 08:09:03.000000 MyMalDependency-2.1.1/MyMalDependency.egg-info/
+-rw-rw-rw-   0        0        0      208 2023-07-27 08:09:03.000000 MyMalDependency-2.1.1/MyMalDependency.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-07-27 08:09:03.000000 MyMalDependency-2.1.1/MyMalDependency.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 08:09:03.000000 MyMalDependency-2.1.1/MyMalDependency.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-27 08:09:03.000000 MyMalDependency-2.1.1/MyMalDependency.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 08:09:03.000000 MyMalDependency-2.1.1/MyMalDependency_package/
+-rw-rw-rw-   0        0        0      340 2023-07-27 02:50:48.000000 MyMalDependency-2.1.1/MyMalDependency_package/__init__.py
+-rw-rw-rw-   0        0        0      208 2023-07-27 08:09:03.000000 MyMalDependency-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-27 08:09:03.000000 MyMalDependency-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      328 2023-07-27 08:08:35.000000 MyMalDependency-2.1.1/setup.py
```

