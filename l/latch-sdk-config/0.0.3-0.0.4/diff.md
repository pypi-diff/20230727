# Comparing `tmp/latch-sdk-config-0.0.3.tar.gz` & `tmp/latch-sdk-config-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch-sdk-config-0.0.3.tar", last modified: Thu Jul 27 21:40:37 2023, max compression
+gzip compressed data, was "latch-sdk-config-0.0.4.tar", last modified: Thu Jul 27 21:42:14 2023, max compression
```

## Comparing `latch-sdk-config-0.0.3.tar` & `latch-sdk-config-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 21:40:37.068170 latch-sdk-config-0.0.3/
--rw-r--r--   0 aidan      (501) staff       (20)     1065 2023-07-26 19:50:42.000000 latch-sdk-config-0.0.3/LICENSE
--rw-r--r--   0 aidan      (501) staff       (20)      448 2023-07-27 21:40:37.067904 latch-sdk-config-0.0.3/PKG-INFO
--rw-r--r--   0 aidan      (501) staff       (20)       18 2023-07-26 19:50:42.000000 latch-sdk-config-0.0.3/README.md
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 21:40:37.066412 latch-sdk-config-0.0.3/latch_sdk_config/
--rw-r--r--   0 aidan      (501) staff       (20)        0 2023-07-26 19:50:42.000000 latch-sdk-config-0.0.3/latch_sdk_config/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     3065 2023-07-27 21:40:09.000000 latch-sdk-config-0.0.3/latch_sdk_config/latch.py
--rw-r--r--   0 aidan      (501) staff       (20)     2877 2023-07-26 19:50:42.000000 latch-sdk-config-0.0.3/latch_sdk_config/user.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 21:40:37.067562 latch-sdk-config-0.0.3/latch_sdk_config.egg-info/
--rw-r--r--   0 aidan      (501) staff       (20)      448 2023-07-27 21:40:37.000000 latch-sdk-config-0.0.3/latch_sdk_config.egg-info/PKG-INFO
--rw-r--r--   0 aidan      (501) staff       (20)      266 2023-07-27 21:40:37.000000 latch-sdk-config-0.0.3/latch_sdk_config.egg-info/SOURCES.txt
--rw-r--r--   0 aidan      (501) staff       (20)        1 2023-07-27 21:40:37.000000 latch-sdk-config-0.0.3/latch_sdk_config.egg-info/dependency_links.txt
--rw-r--r--   0 aidan      (501) staff       (20)       17 2023-07-27 21:40:37.000000 latch-sdk-config-0.0.3/latch_sdk_config.egg-info/top_level.txt
--rw-r--r--   0 aidan      (501) staff       (20)       38 2023-07-27 21:40:37.068261 latch-sdk-config-0.0.3/setup.cfg
--rw-r--r--   0 aidan      (501) staff       (20)      511 2023-07-27 21:40:24.000000 latch-sdk-config-0.0.3/setup.py
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 21:42:14.507094 latch-sdk-config-0.0.4/
+-rw-r--r--   0 aidan      (501) staff       (20)     1065 2023-07-26 19:50:42.000000 latch-sdk-config-0.0.4/LICENSE
+-rw-r--r--   0 aidan      (501) staff       (20)      448 2023-07-27 21:42:14.506856 latch-sdk-config-0.0.4/PKG-INFO
+-rw-r--r--   0 aidan      (501) staff       (20)       18 2023-07-26 19:50:42.000000 latch-sdk-config-0.0.4/README.md
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 21:42:14.505494 latch-sdk-config-0.0.4/latch_sdk_config/
+-rw-r--r--   0 aidan      (501) staff       (20)        0 2023-07-26 19:50:42.000000 latch-sdk-config-0.0.4/latch_sdk_config/__init__.py
+-rw-r--r--   0 aidan      (501) staff       (20)     3034 2023-07-27 21:41:21.000000 latch-sdk-config-0.0.4/latch_sdk_config/latch.py
+-rw-r--r--   0 aidan      (501) staff       (20)     2877 2023-07-26 19:50:42.000000 latch-sdk-config-0.0.4/latch_sdk_config/user.py
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 21:42:14.506543 latch-sdk-config-0.0.4/latch_sdk_config.egg-info/
+-rw-r--r--   0 aidan      (501) staff       (20)      448 2023-07-27 21:42:14.000000 latch-sdk-config-0.0.4/latch_sdk_config.egg-info/PKG-INFO
+-rw-r--r--   0 aidan      (501) staff       (20)      266 2023-07-27 21:42:14.000000 latch-sdk-config-0.0.4/latch_sdk_config.egg-info/SOURCES.txt
+-rw-r--r--   0 aidan      (501) staff       (20)        1 2023-07-27 21:42:14.000000 latch-sdk-config-0.0.4/latch_sdk_config.egg-info/dependency_links.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       17 2023-07-27 21:42:14.000000 latch-sdk-config-0.0.4/latch_sdk_config.egg-info/top_level.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       38 2023-07-27 21:42:14.507165 latch-sdk-config-0.0.4/setup.cfg
+-rw-r--r--   0 aidan      (501) staff       (20)      511 2023-07-27 21:41:57.000000 latch-sdk-config-0.0.4/setup.py
```

### Comparing `latch-sdk-config-0.0.3/LICENSE` & `latch-sdk-config-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `latch-sdk-config-0.0.3/latch_sdk_config/latch.py` & `latch-sdk-config-0.0.4/latch_sdk_config/latch.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     execution: _ExecutionAPI
     user: _UserAPI
     centromere: _CentromereAPI
 
 
 @dataclass
 class _ConsoleRoutes:
-    developer: str = field(default_factory=lambda: urljoin(CONSOLE_URL, "/settings/developer"))
+    developer: str = urljoin(CONSOLE_URL, "/settings/developer")
 
 
 @dataclass(frozen=True)
 class _LatchConfig:
     api: _API
     console_routes: _ConsoleRoutes
     gql: str = f"{VACUOLE_URL}/graphql"
```

### Comparing `latch-sdk-config-0.0.3/latch_sdk_config/user.py` & `latch-sdk-config-0.0.4/latch_sdk_config/user.py`

 * *Files identical despite different names*

