# Comparing `tmp/steam-tools-ng-3.1.tar.gz` & `tmp/steam-tools-ng-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steam-tools-ng-3.1.tar", last modified: Fri Jul 21 18:46:33 2023, max compression
+gzip compressed data, was "steam-tools-ng-3.1.1.tar", last modified: Thu Jul 27 14:20:02 2023, max compression
```

## Comparing `steam-tools-ng-3.1.tar` & `steam-tools-ng-3.1.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.663149 steam-tools-ng-3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-21 18:46:33.663149 steam-tools-ng-3.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3438 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.655149 steam-tools-ng-3.1/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)    35901 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/i18n/fr.po
--rwxr-xr-x   0 runner    (1001) docker     (123)    45277 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/i18n/pt_BR.po
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 18:46:33.663149 steam-tools-ng-3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     6010 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.651148 steam-tools-ng-3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.655149 steam-tools-ng-3.1/src/steam_tools_ng/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.655149 steam-tools-ng-3.1/src/steam_tools_ng/console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/console/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/console/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/console/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/console/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.659149 steam-tools-ng-3.1/src/steam_tools_ng/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/cardfarming.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/confirmations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/coupons.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/fakerun.py
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/steamgifts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/steamguard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/steamtrades.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.659149 steam-tools-ng-3.1/src/steam_tools_ng/gtk/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/async_gtk.py
--rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/confirmation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/coupon.py
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    28209 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38713 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gtk/window.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.663149 steam-tools-ng-3.1/src/steam_tools_ng/icons/
--rw-r--r--   0 runner    (1001) docker     (123)   245142 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/icons/stng.ico
--rw-r--r--   0 runner    (1001) docker     (123)    97830 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/icons/stng.png
--rw-r--r--   0 runner    (1001) docker     (123)   231041 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_console.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31925 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_console.png
--rw-r--r--   0 runner    (1001) docker     (123)   229900 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_nc.ico
--rw-r--r--   0 runner    (1001) docker     (123)    66900 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_nc.png
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/logger_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/src/steam_tools_ng/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.655149 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-21 18:46:33.000000 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-21 18:46:33.000000 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:46:33.000000 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-21 18:46:33.000000 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:46:33.000000 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-21 18:46:33.000000 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 18:46:33.000000 steam-tools-ng-3.1/src/steam_tools_ng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/steam-tools-ng.desktop
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:33.663149 steam-tools-ng-3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 18:46:12.000000 steam-tools-ng-3.1/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:20:02.817341 steam-tools-ng-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-27 14:20:02.817341 steam-tools-ng-3.1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3334 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:20:02.809340 steam-tools-ng-3.1.1/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)    35901 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/i18n/fr.po
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47681 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/i18n/pt_BR.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:20:02.817341 steam-tools-ng-3.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6010 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:20:02.809340 steam-tools-ng-3.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:20:02.813341 steam-tools-ng-3.1.1/src/steam_tools_ng/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:20:02.813341 steam-tools-ng-3.1.1/src/steam_tools_ng/console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/console/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/console/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/console/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/console/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:20:02.813341 steam-tools-ng-3.1.1/src/steam_tools_ng/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/cardfarming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/confirmations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/coupons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/fakerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/steamgifts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/steamguard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/steamtrades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:20:02.817341 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15749 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/async_gtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/confirmation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28096 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38599 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:20:02.817341 steam-tools-ng-3.1.1/src/steam_tools_ng/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)   245142 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    97830 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng.png
+-rw-r--r--   0 runner    (1001) docker     (123)   231041 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_console.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    31925 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_console.png
+-rw-r--r--   0 runner    (1001) docker     (123)   229900 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_nc.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    66900 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_nc.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/logger_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/src/steam_tools_ng/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:20:02.813341 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-27 14:20:02.000000 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-27 14:20:02.000000 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:20:02.000000 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-27 14:20:02.000000 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:20:02.000000 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-27 14:20:02.000000 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 14:20:02.000000 steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/steam-tools-ng.desktop
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:20:02.817341 steam-tools-ng-3.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 14:19:47.000000 steam-tools-ng-3.1.1/tests/test_placeholder.py
```

### Comparing `steam-tools-ng-3.1/LICENSE` & `steam-tools-ng-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/PKG-INFO` & `steam-tools-ng-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steam-tools-ng
-Version: 3.1
+Version: 3.1.1
 Summary: Steam Tools NG
 Author: Lara Maia
 Author-email: dev@lara.monster
 License: GPLv3
 Project-URL: homepage, https://github.com/calendulish/steam-tools-ng
 Project-URL: repository, https://github.com
 Project-URL: changelog, https://github.com/calendulish/steam-tools-ng/releases
@@ -26,18 +26,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [STNG] Steam Tools NG (formerly Steam Tools)
 ========================================
 [![STNG](https://lara.monster/archive/stng_last.png)](https://github.com/calendulish/steam-tools-ng)  
   
-[![transifex](https://img.shields.io/badge/transifex-contribute%20now-blue.svg?style=flat)](https://www.transifex.com/shypixie/steam-tools-ng)
+[![transifex](https://img.shields.io/badge/transifex-contribute%20now-blue.svg?style=flat)](https://www.transifex.com/calendulish/steam-tools-ng)
 [![windows build status](https://badges.lara.monster/calendulish/.github/steam-tools-ng-windows-build)](https://github.com/calendulish/steam-tools-ng/actions/workflows/build.yml)
 [![linux build status](https://badges.lara.monster/calendulish/.github/steam-tools-ng-linux-build)](https://github.com/calendulish/steam-tools-ng/actions/workflows/build.yml)
-[![Quality](https://api.codiga.io/project/33951/score/svg)](https://app.codiga.io/project/33951/dashboard)
 [![GitHub license](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](https://www.gnu.org/licenses/gpl-3.0.html)
 [![GitHub release](https://img.shields.io/github/release/calendulish/steam-tools-ng.svg?style=flat)](https://github.com/calendulish/steam-tools-ng/releases)
 
 Some useful tools to use with steam client or compatible programs and websites.
 
 You can run the follow modules from steam-tools:
```

### Comparing `steam-tools-ng-3.1/README.md` & `steam-tools-ng-3.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [STNG] Steam Tools NG (formerly Steam Tools)
 ========================================
 [![STNG](https://lara.monster/archive/stng_last.png)](https://github.com/calendulish/steam-tools-ng)  
   
-[![transifex](https://img.shields.io/badge/transifex-contribute%20now-blue.svg?style=flat)](https://www.transifex.com/shypixie/steam-tools-ng)
+[![transifex](https://img.shields.io/badge/transifex-contribute%20now-blue.svg?style=flat)](https://www.transifex.com/calendulish/steam-tools-ng)
 [![windows build status](https://badges.lara.monster/calendulish/.github/steam-tools-ng-windows-build)](https://github.com/calendulish/steam-tools-ng/actions/workflows/build.yml)
 [![linux build status](https://badges.lara.monster/calendulish/.github/steam-tools-ng-linux-build)](https://github.com/calendulish/steam-tools-ng/actions/workflows/build.yml)
-[![Quality](https://api.codiga.io/project/33951/score/svg)](https://app.codiga.io/project/33951/dashboard)
 [![GitHub license](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](https://www.gnu.org/licenses/gpl-3.0.html)
 [![GitHub release](https://img.shields.io/github/release/calendulish/steam-tools-ng.svg?style=flat)](https://github.com/calendulish/steam-tools-ng/releases)
 
 Some useful tools to use with steam client or compatible programs and websites.
 
 You can run the follow modules from steam-tools:
```

### Comparing `steam-tools-ng-3.1/i18n/fr.po` & `steam-tools-ng-3.1.1/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/i18n/pt_BR.po` & `steam-tools-ng-3.1.1/i18n/pt_BR.po`

 * *Files 8% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 # Lara Maia <dev@lara.monster>, 2023
 #
 
 msgid ""
 msgstr ""
 "Project-Id-Version: steam-tools-ng\n"
 "Report-Msgid-Bugs-To: dev@lara.monster\n"
-"POT-Creation-Date: 2023-04-03 05:17-0300\n"
+"POT-Creation-Date: 2023-07-27 10:21-0300\n"
 "PO-Revision-Date: 2018-04-15 21:27+0000\n"
 "Last-Translator: Lara Maia <dev@lara.monster>, 2023\n"
 "Language-Team: Portuguese (Brazil) (https://app.transifex.com/calendulish/teams/85593/pt_BR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pt_BR\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
-#: src/steam_tools_ng/cli.py:108 src/steam_tools_ng/cli.py:113
-#: src/steam_tools_ng/gui.py:116 src/steam_tools_ng/gui.py:121
+#: src/steam_tools_ng/cli.py:136 src/steam_tools_ng/cli.py:141
+#: src/steam_tools_ng/gui.py:135 src/steam_tools_ng/gui.py:140
 msgid "Done!"
 msgstr "Feito!"
 
 #: src/steam_tools_ng/config.py:60
 msgid "Light"
 msgstr "Claro"
 
@@ -123,30 +123,42 @@
 msgstr "Nível (0-100)"
 
 #: src/steam_tools_ng/config.py:96
 msgid "Level (100-0)"
 msgstr "Nível (100-0)"
 
 #: src/steam_tools_ng/config.py:100
-msgid "Run all and restart"
-msgstr "Executar todos e reiniciar"
+msgid ""
+"Run all and restart\n"
+"Run all strategies and restart"
+msgstr ""
+"Rodar todas e reiniciar\n"
+"Rodar todas as estratégias e reiniciar"
 
 #: src/steam_tools_ng/config.py:101
-msgid "Stop after reach minimum points and wait"
-msgstr "Parar após alcançar os pontos mínimos e esperar"
+msgid ""
+"Stop and wait\n"
+"after minimum points"
+msgstr ""
+"Parar e aguardar\n"
+"depois dos pontos mínimos"
 
 #: src/steam_tools_ng/config.py:102
-msgid "Stop after reach minimum points and restart"
-msgstr "Parar após alcançar os pontos mínimos e reiniciar"
+msgid ""
+"Stop and restart\n"
+"after minimum points"
+msgstr ""
+"Parar e reiniciar\n"
+"após os pontos mínimos"
 
 #: src/steam_tools_ng/config.py:106
 msgid "Free Coupons"
 msgstr "Cupons Grátis"
 
-#: src/steam_tools_ng/config.py:107 src/steam_tools_ng/gtk/window.py:139
+#: src/steam_tools_ng/config.py:107 src/steam_tools_ng/gtk/window.py:151
 msgid "Confirmations"
 msgstr "Confirmações"
 
 #: src/steam_tools_ng/config.py:108
 msgid "Steam Trades"
 msgstr "Steam Trades"
 
@@ -178,129 +190,132 @@
 msgid "75% OFF"
 msgstr "75% de Desconto"
 
 #: src/steam_tools_ng/config.py:119
 msgid "90% OFF"
 msgstr "90% de Desconto"
 
-#: src/steam_tools_ng/config.py:238
+#: src/steam_tools_ng/config.py:237
 msgid "Unsupported language requested. Fallbacking to English."
 msgstr "Idioma não suportado requisitado. Usando Inglês."
 
-#: src/steam_tools_ng/config.py:242
+#: src/steam_tools_ng/config.py:241
 msgid ""
 "Please, fix your config file. Available values for {}:\n"
 "{}"
 msgstr ""
 "Por favor, conserte seu arquivo de configuração. Valores disponíveis para {}:\n"
 "{}"
 
-#: src/steam_tools_ng/config.py:264
+#: src/steam_tools_ng/config.py:263
 msgid "Incorrect log directory. Fallbacking to default."
 msgstr "Diretório de log incorreto. Usando o valor padrão."
 
-#: src/steam_tools_ng/config.py:310
+#: src/steam_tools_ng/config.py:309
 msgid "Unable to open steam-tools-ng.log"
 msgstr "Não foi possível abrir steam-tools-ng.log"
 
-#: src/steam_tools_ng/config.py:331
+#: src/steam_tools_ng/config.py:330
 msgid "Saving {}:{} on config file"
 msgstr "Salvando {}:{} no arquivo de configuração"
 
-#: src/steam_tools_ng/config.py:337
+#: src/steam_tools_ng/config.py:336
 msgid "Not saving {}:{} because values are already updated"
 msgstr "Não salvando {}:{} porque os valores já estão atualizados"
 
-#: src/steam_tools_ng/console/authenticator.py:59
-#: src/steam_tools_ng/console/cli.py:107
-#: src/steam_tools_ng/gtk/application.py:73
-#: src/steam_tools_ng/gtk/authenticator.py:95
-#: src/steam_tools_ng/gtk/window.py:651
+#: src/steam_tools_ng/console/authenticator.py:58
+#: src/steam_tools_ng/console/cli.py:108
+#: src/steam_tools_ng/gtk/application.py:69
+#: src/steam_tools_ng/gtk/authenticator.py:85
 msgid "SteamId is invalid"
 msgstr "SteamId é inválido"
 
-#: src/steam_tools_ng/console/authenticator.py:64
-#: src/steam_tools_ng/console/login.py:85
-#: src/steam_tools_ng/gtk/authenticator.py:110
-#: src/steam_tools_ng/gtk/login.py:199
+#: src/steam_tools_ng/console/authenticator.py:63
+#: src/steam_tools_ng/console/authenticator.py:138
+#: src/steam_tools_ng/console/login.py:73
+#: src/steam_tools_ng/gtk/authenticator.py:102
+#: src/steam_tools_ng/gtk/authenticator.py:212
+#: src/steam_tools_ng/gtk/login.py:171
 msgid "Retrieving user data"
 msgstr "Recuperando dados do usuário"
 
-#: src/steam_tools_ng/console/authenticator.py:68
+#: src/steam_tools_ng/console/authenticator.py:67
+#: src/steam_tools_ng/console/authenticator.py:142
 msgid ""
 "Some login data is missing. If the problem persists, run:\n"
 "{} --reset"
 msgstr ""
 "Alguns dados de login estão faltando. Se o problema persistir, execute:\n"
 "{} --reset"
 
-#: src/steam_tools_ng/console/authenticator.py:82
-#: src/steam_tools_ng/console/authenticator.py:118
-#: src/steam_tools_ng/console/cli.py:145
-#: src/steam_tools_ng/console/login.py:182
+#: src/steam_tools_ng/console/authenticator.py:79
+#: src/steam_tools_ng/console/authenticator.py:114
+#: src/steam_tools_ng/console/authenticator.py:160
+#: src/steam_tools_ng/console/cli.py:139
+#: src/steam_tools_ng/console/login.py:154
+#: src/steam_tools_ng/core/cardfarming.py:61
 #: src/steam_tools_ng/core/cardfarming.py:119
-#: src/steam_tools_ng/core/cardfarming.py:171
-#: src/steam_tools_ng/core/cardfarming.py:206
-#: src/steam_tools_ng/core/confirmations.py:60
-#: src/steam_tools_ng/core/coupons.py:83
-#: src/steam_tools_ng/core/coupons.py:132
+#: src/steam_tools_ng/core/cardfarming.py:161
+#: src/steam_tools_ng/core/confirmations.py:67
+#: src/steam_tools_ng/core/coupons.py:89
+#: src/steam_tools_ng/core/coupons.py:148
 #: src/steam_tools_ng/core/fakerun.py:62
 #: src/steam_tools_ng/core/fakerun.py:112
-#: src/steam_tools_ng/core/steamgifts.py:45
-#: src/steam_tools_ng/core/steamgifts.py:71
-#: src/steam_tools_ng/core/steamgifts.py:120
-#: src/steam_tools_ng/core/steamgifts.py:173
-#: src/steam_tools_ng/core/steamtrades.py:54
-#: src/steam_tools_ng/core/steamtrades.py:91
-#: src/steam_tools_ng/core/steamtrades.py:110
-#: src/steam_tools_ng/gtk/application.py:151
-#: src/steam_tools_ng/gtk/authenticator.py:127
-#: src/steam_tools_ng/gtk/authenticator.py:169
-#: src/steam_tools_ng/gtk/login.py:303
+#: src/steam_tools_ng/core/steamgifts.py:44
+#: src/steam_tools_ng/core/steamgifts.py:70
+#: src/steam_tools_ng/core/steamgifts.py:119
+#: src/steam_tools_ng/core/steamgifts.py:172
+#: src/steam_tools_ng/core/steamtrades.py:53
+#: src/steam_tools_ng/core/steamtrades.py:90
+#: src/steam_tools_ng/core/steamtrades.py:109
+#: src/steam_tools_ng/gtk/application.py:140
+#: src/steam_tools_ng/gtk/authenticator.py:118
+#: src/steam_tools_ng/gtk/authenticator.py:166
+#: src/steam_tools_ng/gtk/authenticator.py:245
 msgid "Check your connection. (server down?)"
 msgstr "Verifique sua conexão. (server caiu?)"
 
-#: src/steam_tools_ng/console/authenticator.py:86
-#: src/steam_tools_ng/gtk/authenticator.py:130
+#: src/steam_tools_ng/console/authenticator.py:83
+#: src/steam_tools_ng/gtk/authenticator.py:121
 msgid ""
 "There's already an authenticator active for that account.\n"
 "Remove your current steam authenticator and try again."
 msgstr ""
 "Já existe um autenticador ativo para essa conta.\n"
 "Remova o seu autenticador steam atual e tente novamente."
 
-#: src/steam_tools_ng/console/authenticator.py:92
-#: src/steam_tools_ng/gtk/authenticator.py:135
+#: src/steam_tools_ng/console/authenticator.py:89
+#: src/steam_tools_ng/gtk/authenticator.py:126
 msgid ""
 "You must have a phone registered on your steam account to proceed.\n"
 "Go to your Steam Account Settings, add a Phone Number, and try again."
 msgstr ""
 "Você precisa ter um telefone registrado em sua conta steam para continuar.\n"
 "Vá para as Configurações da sua Conta Steam, adicione um Número de Telefone, e tente novamente."
 
-#: src/steam_tools_ng/console/authenticator.py:100
+#: src/steam_tools_ng/console/authenticator.py:97
 msgid "Enter the code received by SMS"
 msgstr "Insira o código recebido por SMS"
 
-#: src/steam_tools_ng/console/authenticator.py:104
-#: src/steam_tools_ng/gtk/authenticator.py:154
+#: src/steam_tools_ng/console/authenticator.py:101
+#: src/steam_tools_ng/gtk/authenticator.py:149
 msgid "Adding authenticator"
 msgstr "Adicionando autenticador"
 
-#: src/steam_tools_ng/console/authenticator.py:115
+#: src/steam_tools_ng/console/authenticator.py:111
 msgid "Invalid SMS Code. Please, check the code and try again."
 msgstr "Código SMS inválido. Por favor, verifique o código e tente novamente."
 
-#: src/steam_tools_ng/console/authenticator.py:124
-#: src/steam_tools_ng/gtk/authenticator.py:180
+#: src/steam_tools_ng/console/authenticator.py:120
+#: src/steam_tools_ng/gtk/authenticator.py:179
 msgid "Saving new secrets"
 msgstr "Salvando novos segredos"
 
-#: src/steam_tools_ng/console/authenticator.py:131
-#: src/steam_tools_ng/gtk/authenticator.py:187
+#: src/steam_tools_ng/console/authenticator.py:127
+#: src/steam_tools_ng/gtk/authenticator.py:186
 msgid ""
 "RECOVERY CODE\n"
 "\n"
 "You will need this code to recovery your Steam Account\n"
 "if you lose access to STNG Authenticator. So, writedown this recovery code.\n"
 "\n"
 "YOU WILL NOT ABLE TO VIEW IT AGAIN!\n"
@@ -308,128 +323,167 @@
 "CÓDIGO DE RECUPERAÇÃO\n"
 "\n"
 "Você vai precisar deste código para recuperar sua Conta do Steam\n"
 "caso você perca acesso ao Autenticador do STNG. Então, escreva e guarde esse código de recuperação\n"
 "\n"
 "VOCÊ NÃO CONSEGUIRÁ VER ISSO NOVAMENTE!\n"
 
-#: src/steam_tools_ng/console/cli.py:60
+#: src/steam_tools_ng/console/authenticator.py:148
+msgid "Enter the revocation code"
+msgstr "Insira o código de revogação"
+
+#: src/steam_tools_ng/console/authenticator.py:151
+msgid "Removing authenticator"
+msgstr "Removendo o autenticador"
+
+#: src/steam_tools_ng/console/authenticator.py:163
+#: src/steam_tools_ng/gtk/authenticator.py:257
+msgid "Too many attempts, try again later."
+msgstr "Muitas tentativas, tente novamente mais tarde."
+
+#: src/steam_tools_ng/console/authenticator.py:167
+#: src/steam_tools_ng/gtk/authenticator.py:263
+msgid "Authenticator has been removed."
+msgstr "O autenticador foi removido."
+
+#: src/steam_tools_ng/console/authenticator.py:169
+#: src/steam_tools_ng/gtk/authenticator.py:265
+msgid "Unable to remove the authenticator."
+msgstr "Não foi possível remover o autenticador."
+
+#: src/steam_tools_ng/console/cli.py:63
 msgid ""
 "{} module has been disabled because you have a stlib built without "
 "SteamWorks support. To enable it again, reinstall stlib with SteamWorks "
 "support"
 msgstr ""
 "O módulo {} foi desabilitado porque você tem uma stlib construída sem "
 "suporte a SteamWorks. Para habilitar ele novamente, reinstale a stlib com "
 "support a SteamWorks"
 
-#: src/steam_tools_ng/console/cli.py:69
+#: src/steam_tools_ng/console/cli.py:72
 #, python-brace-format
 msgid ""
 "{0} module has been disabled because you don't have {0} plugin installed. To"
 " enable it again, install the {0} plugin."
 msgstr ""
 "O módulo {0} foi desabilitado porque você não tem o plugin {0} instalado. "
 "Para habilitar ele novamente, instale o plugin {0}."
 
 #: src/steam_tools_ng/console/cli.py:128
-#: src/steam_tools_ng/gtk/application.py:133
+#: src/steam_tools_ng/gtk/application.py:126
 msgid "Logging on Steam. Please wait!"
 msgstr "Logando no Steam. Por favor aguarde!"
 
-#: src/steam_tools_ng/console/cli.py:140
+#: src/steam_tools_ng/console/cli.py:143
+#: src/steam_tools_ng/gtk/application.py:145
+msgid "Waiting 10 seconds to try again"
+msgstr "Aguardando 10 segundos para tentar novamente"
+
+#: src/steam_tools_ng/console/cli.py:147
 msgid "Steam login Successful"
 msgstr "Login no Steam efetuado com sucesso"
 
-#: src/steam_tools_ng/console/cli.py:153
-#: src/steam_tools_ng/gtk/application.py:161
+#: src/steam_tools_ng/console/cli.py:154
+#: src/steam_tools_ng/gtk/application.py:158
 #, python-format
 msgid "SteamAPI key found: %s"
 msgstr "Chave da SteamAPI encontrada:%s"
 
-#: src/steam_tools_ng/console/cli.py:158
-#: src/steam_tools_ng/gtk/application.py:166
+#: src/steam_tools_ng/console/cli.py:159
+#: src/steam_tools_ng/gtk/application.py:163
 msgid "Updating your SteamAPI dev key"
 msgstr "Atualizando sua dev key da SteamAPI"
 
-#: src/steam_tools_ng/console/cli.py:165
-#: src/steam_tools_ng/gtk/application.py:174
+#: src/steam_tools_ng/console/cli.py:166
+#: src/steam_tools_ng/gtk/application.py:171
 msgid "Something wrong with your SteamAPI dev key"
 msgstr "Alguma coisa errado com a sua dev key da SteamAPI"
 
-#: src/steam_tools_ng/console/cli.py:174
+#: src/steam_tools_ng/console/cli.py:168
+#: src/steam_tools_ng/gtk/application.py:173
+msgid "Limited account! Using dummy API key"
+msgstr "Conta limitada! Usando chave API da Alice"
+
+#: src/steam_tools_ng/console/cli.py:178
 #, python-format
 msgid "Initializing module %s"
 msgstr "Inicializando módulo %s"
 
-#: src/steam_tools_ng/console/cli.py:177
-#: src/steam_tools_ng/gtk/application.py:211
+#: src/steam_tools_ng/console/cli.py:181
+#: src/steam_tools_ng/gtk/application.py:215
 #, python-format
 msgid "Adding a new callback for %s"
 msgstr "Adicionando um novo callback para %s"
 
-#: src/steam_tools_ng/console/login.py:61 src/steam_tools_ng/gtk/login.py:147
+#: src/steam_tools_ng/console/login.py:56 src/steam_tools_ng/gtk/login.py:120
 msgid "Password decode failed. Trying RAW."
 msgstr "Decodificação da senha falhou. Tentando RAW."
 
-#: src/steam_tools_ng/console/login.py:93
+#: src/steam_tools_ng/console/login.py:81
 msgid "Please, write your username"
 msgstr "Por favor, escreva seu nome de usuário"
 
-#: src/steam_tools_ng/console/login.py:98
+#: src/steam_tools_ng/console/login.py:86
 msgid "Please, write your password (IT'S HIDDEN, and will be encrypted)"
 msgstr ""
 "Por favor, escreva sua senha (ELA ESTÁ ESCONDIDA, and vai ser encryptada)"
 
-#: src/steam_tools_ng/console/login.py:118 src/steam_tools_ng/gtk/login.py:221
+#: src/steam_tools_ng/console/login.py:95 src/steam_tools_ng/gtk/login.py:183
 msgid ""
 "No shared secret found. Trying to log-in without two-factor authentication."
 msgstr ""
 "Nenhum segredo partilhado encontrado. Tentando logar sem autenticação de "
 "dois fatores."
 
-#: src/steam_tools_ng/console/login.py:124 src/steam_tools_ng/gtk/login.py:227
+#: src/steam_tools_ng/console/login.py:97 src/steam_tools_ng/gtk/login.py:186
 msgid "Logging in"
 msgstr "Logando"
 
-#: src/steam_tools_ng/console/login.py:131
+#: src/steam_tools_ng/console/login.py:109
 msgid "Write code received by email"
 msgstr "Digite o código recebido por email"
 
-#: src/steam_tools_ng/console/login.py:138 src/steam_tools_ng/gtk/login.py:246
+#: src/steam_tools_ng/console/login.py:115
 msgid "Retrying login in 10 seconds"
 msgstr "Tentando novamente em 10 segundos"
 
-#: src/steam_tools_ng/console/login.py:143
-#: src/steam_tools_ng/console/login.py:173 src/steam_tools_ng/gtk/login.py:251
-#: src/steam_tools_ng/gtk/login.py:298
+#: src/steam_tools_ng/console/login.py:120
+#: src/steam_tools_ng/console/login.py:142 src/steam_tools_ng/gtk/login.py:215
+#: src/steam_tools_ng/gtk/login.py:269
 msgid "shared secret is invalid!"
 msgstr "segredo partilhado é inválido!"
 
-#: src/steam_tools_ng/console/login.py:146
+#: src/steam_tools_ng/console/login.py:123
 msgid "Write Steam Code"
 msgstr "Escreva o Código Steam"
 
-#: src/steam_tools_ng/console/login.py:152 src/steam_tools_ng/gtk/login.py:263
+#: src/steam_tools_ng/console/login.py:128 src/steam_tools_ng/gtk/login.py:228
 msgid ""
 "Your network is blocked!\n"
 "It'll take some time until unblocked. Please, try again later\n"
 msgstr ""
 "Sua rede está bloqueada!\n"
 "Vai levar algum tempo até que seja desbloqueada. Por favor, tente novamente mais tarde\n"
 
-#: src/steam_tools_ng/console/login.py:159
+#: src/steam_tools_ng/console/login.py:133
 msgid "Steam server is requesting a captcha code."
 msgstr "O servidor Steam está requisitando um código de captcha."
 
-#: src/steam_tools_ng/console/login.py:166
-msgid "Open {} in an image view and write captcha code that it shows"
+#: src/steam_tools_ng/console/login.py:138
+msgid "Write Captcha Code"
+msgstr "Escreva o código captcha"
+
+#: src/steam_tools_ng/console/login.py:149
+msgid ""
+"If your previous authenticator has been removed,\n"
+"open your config file and remove the old secrets."
 msgstr ""
-"Abra {} em um visualizador de imagem e digite o código de captcha que ela "
-"mostrar"
+"Se o autenticador anterior foi removido,\n"
+"abra o arquivo de configuração e remova os segredos antigos."
 
 #: src/steam_tools_ng/console/utils.py:39
 msgid "[Y/n]"
 msgstr "[S/n]"
 
 #: src/steam_tools_ng/console/utils.py:41
 msgid "[y/N]"
@@ -453,174 +507,175 @@
 msgid "n"
 msgstr "n"
 
 #: src/steam_tools_ng/console/utils.py:78
 msgid "Please, try again."
 msgstr "Por favor, tente novamente."
 
-#: src/steam_tools_ng/console/utils.py:140 src/steam_tools_ng/gtk/utils.py:701
+#: src/steam_tools_ng/console/utils.py:136 src/steam_tools_ng/gtk/utils.py:820
 #, python-format
 msgid "%s has been stopped due user request"
 msgstr "%s parou por requisição do usuário"
 
+#: src/steam_tools_ng/core/cardfarming.py:61
+#: src/steam_tools_ng/core/cardfarming.py:79
 #: src/steam_tools_ng/core/cardfarming.py:119
-#: src/steam_tools_ng/core/cardfarming.py:137
-#: src/steam_tools_ng/core/cardfarming.py:171
-#: src/steam_tools_ng/core/cardfarming.py:174
-#: src/steam_tools_ng/core/cardfarming.py:206
-#: src/steam_tools_ng/core/cardfarming.py:214
-#: src/steam_tools_ng/core/confirmations.py:36
-#: src/steam_tools_ng/core/confirmations.py:54
-#: src/steam_tools_ng/core/confirmations.py:56
-#: src/steam_tools_ng/core/confirmations.py:60
-#: src/steam_tools_ng/core/coupons.py:43 src/steam_tools_ng/core/coupons.py:51
-#: src/steam_tools_ng/core/coupons.py:76 src/steam_tools_ng/core/coupons.py:83
-#: src/steam_tools_ng/core/coupons.py:133
-#: src/steam_tools_ng/core/coupons.py:141
-#: src/steam_tools_ng/core/coupons.py:163
-#: src/steam_tools_ng/core/steamgifts.py:45
-#: src/steam_tools_ng/core/steamgifts.py:60
+#: src/steam_tools_ng/core/cardfarming.py:122
+#: src/steam_tools_ng/core/cardfarming.py:161
+#: src/steam_tools_ng/core/cardfarming.py:169
+#: src/steam_tools_ng/core/confirmations.py:43
+#: src/steam_tools_ng/core/confirmations.py:61
+#: src/steam_tools_ng/core/confirmations.py:63
+#: src/steam_tools_ng/core/confirmations.py:67
+#: src/steam_tools_ng/core/coupons.py:49 src/steam_tools_ng/core/coupons.py:57
+#: src/steam_tools_ng/core/coupons.py:82 src/steam_tools_ng/core/coupons.py:89
+#: src/steam_tools_ng/core/coupons.py:149
+#: src/steam_tools_ng/core/coupons.py:157
+#: src/steam_tools_ng/core/coupons.py:179
+#: src/steam_tools_ng/core/steamgifts.py:44
+#: src/steam_tools_ng/core/steamgifts.py:59
 #: src/steam_tools_ng/core/steamguard.py:76
 #: src/steam_tools_ng/core/steamguard.py:79
-#: src/steam_tools_ng/core/steamtrades.py:45
-#: src/steam_tools_ng/core/steamtrades.py:69
-#: src/steam_tools_ng/core/steamtrades.py:136
+#: src/steam_tools_ng/core/steamtrades.py:44
+#: src/steam_tools_ng/core/steamtrades.py:68
+#: src/steam_tools_ng/core/steamtrades.py:135
 msgid "Waiting Changes"
 msgstr "Aguardando Mudanças"
 
-#: src/steam_tools_ng/core/cardfarming.py:134
+#: src/steam_tools_ng/core/cardfarming.py:76
 msgid "Invalid game id {}. Ignoring."
 msgstr "Id do jogo inválido {}. Ignorando."
 
-#: src/steam_tools_ng/core/cardfarming.py:137
+#: src/steam_tools_ng/core/cardfarming.py:79
 #: src/steam_tools_ng/core/fakerun.py:40
 #: src/steam_tools_ng/core/fakerun.py:142
 msgid "Steam Client is not running."
 msgstr "O Cliente Steam não está em execução"
 
-#: src/steam_tools_ng/core/cardfarming.py:147
+#: src/steam_tools_ng/core/cardfarming.py:89
 #: src/steam_tools_ng/core/fakerun.py:135
 msgid "Running {}"
 msgstr "Rodando {}"
 
-#: src/steam_tools_ng/core/cardfarming.py:160
+#: src/steam_tools_ng/core/cardfarming.py:108
 msgid "Updating {} drops"
 msgstr "Atualizando {} drops"
 
-#: src/steam_tools_ng/core/cardfarming.py:161
+#: src/steam_tools_ng/core/cardfarming.py:109
 msgid "Game paused"
 msgstr "Jogo pausado"
 
-#: src/steam_tools_ng/core/cardfarming.py:174
+#: src/steam_tools_ng/core/cardfarming.py:122
 msgid "Steam Server is busy"
 msgstr "O Servidor do Steam está ocupado"
 
-#: src/steam_tools_ng/core/cardfarming.py:186
+#: src/steam_tools_ng/core/cardfarming.py:134
 msgid "{} ({})"
 msgstr "{} ({})"
 
-#: src/steam_tools_ng/core/cardfarming.py:186
+#: src/steam_tools_ng/core/cardfarming.py:134
 msgid "Done"
 msgstr "Feito"
 
-#: src/steam_tools_ng/core/cardfarming.py:214
+#: src/steam_tools_ng/core/cardfarming.py:169
 msgid "No more cards to drop."
 msgstr "Sem mais cartas para dropar."
 
-#: src/steam_tools_ng/core/cardfarming.py:230
+#: src/steam_tools_ng/core/cardfarming.py:185
 #: src/steam_tools_ng/core/fakerun.py:124
 msgid "Loading {}"
 msgstr "Carregando {}"
 
-#: src/steam_tools_ng/core/cardfarming.py:234
+#: src/steam_tools_ng/core/cardfarming.py:189
 msgid "Skipping {}"
 msgstr "Pulando {}"
 
-#: src/steam_tools_ng/core/cardfarming.py:300
+#: src/steam_tools_ng/core/cardfarming.py:256
 msgid " +{} other"
 msgstr "+{} outro"
 
-#: src/steam_tools_ng/core/cardfarming.py:302
+#: src/steam_tools_ng/core/cardfarming.py:258
 msgid " +{} others"
 msgstr "+{} outros"
 
-#: src/steam_tools_ng/core/cardfarming.py:307
+#: src/steam_tools_ng/core/cardfarming.py:263
 msgid "{} from {} remaining ({} cards)"
 msgstr "{} de {} restante ({} cartas)"
 
-#: src/steam_tools_ng/core/confirmations.py:36
+#: src/steam_tools_ng/core/confirmations.py:43
 msgid "The current identity secret is invalid."
 msgstr "O segredo de identidade atual é inválido."
 
-#: src/steam_tools_ng/core/confirmations.py:46
+#: src/steam_tools_ng/core/confirmations.py:53
 msgid "Unable to find deviceid. Generating from identity."
 msgstr ""
 "Não foi possível encontrar o id de dispositivo. Gerando a partir da "
 "identidade."
 
-#: src/steam_tools_ng/core/confirmations.py:54
+#: src/steam_tools_ng/core/confirmations.py:61
 msgid "Error when fetch confirmations"
 msgstr "Erro ao coletar confirmações"
 
-#: src/steam_tools_ng/core/confirmations.py:56
+#: src/steam_tools_ng/core/confirmations.py:63
 msgid "Steam is not running"
 msgstr "O Steam não está rodando"
 
-#: src/steam_tools_ng/core/confirmations.py:58
-#: src/steam_tools_ng/gtk/login.py:200 src/steam_tools_ng/gtk/window.py:662
+#: src/steam_tools_ng/core/confirmations.py:65
+#: src/steam_tools_ng/gtk/login.py:172 src/steam_tools_ng/gtk/window.py:654
 msgid "Not logged in"
 msgstr "Não está logado"
 
-#: src/steam_tools_ng/core/coupons.py:43
+#: src/steam_tools_ng/core/coupons.py:49
 msgid "No botID found"
 msgstr "BotID não encontrado"
 
-#: src/steam_tools_ng/core/coupons.py:51
+#: src/steam_tools_ng/core/coupons.py:57
 msgid "Invalid config. Each bot must have id and token."
 msgstr "Configuração inválida. Cada bot precisa ter um id e um token"
 
-#: src/steam_tools_ng/core/coupons.py:58
+#: src/steam_tools_ng/core/coupons.py:64
 msgid "Failed when trying to get owned games"
 msgstr "Falhou ao tentar recuperar os jogos de propriedade"
 
-#: src/steam_tools_ng/core/coupons.py:69
+#: src/steam_tools_ng/core/coupons.py:75
 msgid "The botid {} is invalid"
 msgstr "O botid {} é inválido"
 
-#: src/steam_tools_ng/core/coupons.py:76
+#: src/steam_tools_ng/core/coupons.py:82
 msgid "Error when fetch inventory"
 msgstr "Erro ao buscar no inventário"
 
-#: src/steam_tools_ng/core/coupons.py:91
+#: src/steam_tools_ng/core/coupons.py:97
 msgid "The botid {} has no coupons available"
 msgstr "O botid {} não tem cupons disponíveis"
 
-#: src/steam_tools_ng/core/coupons.py:91
+#: src/steam_tools_ng/core/coupons.py:97
 msgid "Skipping"
 msgstr "Ignorando"
 
-#: src/steam_tools_ng/core/coupons.py:109
+#: src/steam_tools_ng/core/coupons.py:116
 msgid "Stopping fetching coupons (requested by user)"
 msgstr "Parando de buscar cupons (requisitado pelo usuário)"
 
-#: src/steam_tools_ng/core/coupons.py:114
+#: src/steam_tools_ng/core/coupons.py:126
+#: src/steam_tools_ng/core/coupons.py:130
 #, python-format
 msgid "Ignoring coupon %s due blacklist"
 msgstr "Ignorando cupom %s devido a lista negra"
 
-#: src/steam_tools_ng/core/coupons.py:120
+#: src/steam_tools_ng/core/coupons.py:136
 #, python-format
 msgid "Ignoring coupon %s due low discount value"
 msgstr "Ignorando cupom %s devido ao valor baixo de desconto"
 
-#: src/steam_tools_ng/core/coupons.py:141
+#: src/steam_tools_ng/core/coupons.py:157
 msgid "Failed to get package details"
 msgstr "Falha ao recuperar detalhes do pacote"
 
-#: src/steam_tools_ng/core/coupons.py:163
+#: src/steam_tools_ng/core/coupons.py:179
 msgid "Api rate limit reached. Waiting."
 msgstr "Chegou ao limite de chamadas à api. Aguardando."
 
 #: src/steam_tools_ng/core/fakerun.py:31
 msgid "Mixing ingredients"
 msgstr "Misturando ingredientes"
 
@@ -654,91 +709,91 @@
 
 #: src/steam_tools_ng/core/fakerun.py:134
 msgid "Running for {} minutes."
 msgstr "Rodando por {} minutos."
 
 #: src/steam_tools_ng/core/steamgifts.py:34
 #: src/steam_tools_ng/core/steamtrades.py:33
-#: src/steam_tools_ng/gtk/application.py:207
+#: src/steam_tools_ng/gtk/application.py:211
 msgid "Loading"
 msgstr "Carregando"
 
-#: src/steam_tools_ng/core/steamgifts.py:40
+#: src/steam_tools_ng/core/steamgifts.py:37
 msgid "Unable to find Steamgifts plugin."
 msgstr "Não foi possível encontrar o plugin Steamgifts."
 
-#: src/steam_tools_ng/core/steamgifts.py:49
-#: src/steam_tools_ng/core/steamtrades.py:58
+#: src/steam_tools_ng/core/steamgifts.py:48
+#: src/steam_tools_ng/core/steamtrades.py:57
 msgid "Unable to login. Trying again in 15 seconds"
 msgstr "Não foi possível logar. Tentando novamente em 15 segundos"
 
-#: src/steam_tools_ng/core/steamgifts.py:53
-#: src/steam_tools_ng/core/steamtrades.py:62
+#: src/steam_tools_ng/core/steamgifts.py:52
+#: src/steam_tools_ng/core/steamtrades.py:61
 msgid "User is suspended."
 msgstr "Usuário está suspenso."
 
-#: src/steam_tools_ng/core/steamgifts.py:60
+#: src/steam_tools_ng/core/steamgifts.py:59
 msgid "Your profile must be public to use steamgifts."
 msgstr "Seu perfil precisa ser público para usar o steamgifts."
 
-#: src/steam_tools_ng/core/steamgifts.py:64
-#: src/steam_tools_ng/core/steamtrades.py:77
+#: src/steam_tools_ng/core/steamgifts.py:63
+#: src/steam_tools_ng/core/steamtrades.py:76
 msgid "User is not logged in. Trying again in 30 seconds"
 msgstr "Usuário não está logado. Tentando novamente em 30 segundos"
 
-#: src/steam_tools_ng/core/steamgifts.py:75
+#: src/steam_tools_ng/core/steamgifts.py:74
 msgid "Unable to configure steamgifts."
 msgstr "Não foi possível configurar o steamgifts"
 
-#: src/steam_tools_ng/core/steamgifts.py:90
+#: src/steam_tools_ng/core/steamgifts.py:89
 msgid "Strategy {} is disabled. Skipping."
 msgstr "Estratégia {} está desabilitada. Ignorando."
 
-#: src/steam_tools_ng/core/steamgifts.py:137
+#: src/steam_tools_ng/core/steamgifts.py:136
 msgid "No giveaways to join for strategy {}. Skipping."
 msgstr "Nenhum giveaway para entrar para a estratégia {}. Ignorando."
 
-#: src/steam_tools_ng/core/steamgifts.py:150
+#: src/steam_tools_ng/core/steamgifts.py:149
 msgid "Minimum points reached."
 msgstr "Pontos mínimos alcançado."
 
-#: src/steam_tools_ng/core/steamgifts.py:169
+#: src/steam_tools_ng/core/steamgifts.py:168
 msgid "Unable to join {}."
 msgstr "Não foi possível entrar em {}."
 
-#: src/steam_tools_ng/core/steamgifts.py:178
+#: src/steam_tools_ng/core/steamgifts.py:177
 msgid "No giveaways available to join."
 msgstr "Nenhum giveaway disponível para entrar."
 
-#: src/steam_tools_ng/core/steamgifts.py:182
+#: src/steam_tools_ng/core/steamgifts.py:181
 msgid "Giveaway is already ended."
 msgstr "O giveaway já acabou."
 
-#: src/steam_tools_ng/core/steamgifts.py:186
-#: src/steam_tools_ng/core/steamtrades.py:126
+#: src/steam_tools_ng/core/steamgifts.py:185
+#: src/steam_tools_ng/core/steamtrades.py:125
 msgid "Login is lost. Trying to relogin."
 msgstr "O Login foi perdido. Tentando relogar."
 
-#: src/steam_tools_ng/core/steamgifts.py:191
+#: src/steam_tools_ng/core/steamgifts.py:190
 msgid "User don't have required level to join."
 msgstr "Usuário não tem o level necessário para entrar."
 
-#: src/steam_tools_ng/core/steamgifts.py:195
+#: src/steam_tools_ng/core/steamgifts.py:194
 msgid "User don't have required points to join."
 msgstr "Usuário não tem os pontos necessários para entrar"
 
-#: src/steam_tools_ng/core/steamgifts.py:212
+#: src/steam_tools_ng/core/steamgifts.py:211
 msgid "Waiting before next strategy"
 msgstr "Aguardando antes da próxima estratégia"
 
-#: src/steam_tools_ng/core/steamgifts.py:218
+#: src/steam_tools_ng/core/steamgifts.py:217
 msgid "Restarting due to mode selection"
 msgstr "Reiniciando devido ao modo selecionado"
 
-#: src/steam_tools_ng/core/steamgifts.py:226
+#: src/steam_tools_ng/core/steamgifts.py:225
 msgid "Waiting for next cycle"
 msgstr "Aguardando o próximo ciclo"
 
 #: src/steam_tools_ng/core/steamguard.py:55
 msgid "Steam is not running."
 msgstr "O Steam não está em execução"
 
@@ -774,237 +829,256 @@
 msgid "Running"
 msgstr "Rodando"
 
 #: src/steam_tools_ng/core/steamguard.py:89
 msgid "New code in {} seconds"
 msgstr "Novo código em {} segundos"
 
-#: src/steam_tools_ng/core/steamtrades.py:39
+#: src/steam_tools_ng/core/steamtrades.py:36
 msgid "Unable to find Steamtrades plugin"
 msgstr "Não foi possível encontrar o plugin do Steamtrades"
 
-#: src/steam_tools_ng/core/steamtrades.py:45
+#: src/steam_tools_ng/core/steamtrades.py:44
 msgid "No trade ID found"
 msgstr "Nenhum ID de trade encontrado"
 
-#: src/steam_tools_ng/core/steamtrades.py:69
+#: src/steam_tools_ng/core/steamtrades.py:68
 msgid "Your profile must be public to use steamtrades."
 msgstr "Seu perfil precisa ser público para usar o steamtrades."
 
-#: src/steam_tools_ng/core/steamtrades.py:73
+#: src/steam_tools_ng/core/steamtrades.py:72
 msgid "You must be level 1 or greater to use steamtrades."
 msgstr "Você precisa ser level 1 ou maior para usar o steamtrades."
 
-#: src/steam_tools_ng/core/steamtrades.py:87
+#: src/steam_tools_ng/core/steamtrades.py:86
 msgid "Unable to find trade id"
 msgstr "Não foi possível encontrar o id de troca"
 
-#: src/steam_tools_ng/core/steamtrades.py:103
+#: src/steam_tools_ng/core/steamtrades.py:102
 msgid "Bumped!"
 msgstr "Bumped!"
 
-#: src/steam_tools_ng/core/steamtrades.py:106
+#: src/steam_tools_ng/core/steamtrades.py:105
 msgid "Unable to bump"
 msgstr "Não foi possível levantar"
 
-#: src/steam_tools_ng/core/steamtrades.py:115
+#: src/steam_tools_ng/core/steamtrades.py:114
 msgid "No trades available to bump"
 msgstr "Nenhum trade disponível para entrar."
 
-#: src/steam_tools_ng/core/steamtrades.py:122
+#: src/steam_tools_ng/core/steamtrades.py:121
 msgid "Trade {}({}) is closed"
 msgstr "Trade {}({}) está fechado"
 
-#: src/steam_tools_ng/gtk/about.py:46
+#: src/steam_tools_ng/gtk/about.py:47
 msgid "Git Repository"
 msgstr "Repositório Git"
 
-#: src/steam_tools_ng/gtk/about.py:49
+#: src/steam_tools_ng/gtk/about.py:50
 msgid "Made with Love <3"
 msgstr "Feito com amor <3"
 
-#: src/steam_tools_ng/gtk/application.py:134
+#: src/steam_tools_ng/gtk/application.py:127
 msgid "Logging on Steam"
 msgstr "Logando no Steam"
 
-#: src/steam_tools_ng/gtk/application.py:188
+#: src/steam_tools_ng/gtk/application.py:194
 #, python-format
 msgid "%s is requesting a reinitialization."
 msgstr "%s está requisitando uma reinicialização."
 
-#: src/steam_tools_ng/gtk/application.py:193
+#: src/steam_tools_ng/gtk/application.py:199
 #, python-format
 msgid "%s is enabled but not initialized. Initializing now."
 msgstr "%s está habilitado mas não inicializado. Inicializando agora."
 
-#: src/steam_tools_ng/gtk/application.py:218
+#: src/steam_tools_ng/gtk/application.py:222
 #, python-format
 msgid "%s is disabled but not cancelled. Cancelling now."
 msgstr "%s está desabilitado mas não cancelado. Cancelando agora."
 
-#: src/steam_tools_ng/gtk/application.py:225
-#: src/steam_tools_ng/gtk/utils.py:203 src/steam_tools_ng/gtk/window.py:715
+#: src/steam_tools_ng/gtk/application.py:229
+#: src/steam_tools_ng/gtk/utils.py:255 src/steam_tools_ng/gtk/window.py:724
 msgid "Disabled"
 msgstr "Desabilitado"
 
-#: src/steam_tools_ng/gtk/application.py:279
+#: src/steam_tools_ng/gtk/application.py:282
 msgid ""
 "Skipping confirmations update because data doesn't seem to have changed"
 msgstr ""
 "Ignorando atualização das confirmações porque os dados não parecem ter "
 "mudado"
 
-#: src/steam_tools_ng/gtk/authenticator.py:43
-msgid "Add Authenticator"
-msgstr "Adicionar Autenticador"
+#: src/steam_tools_ng/gtk/application.py:305
+#: src/steam_tools_ng/gtk/application.py:307
+#: src/steam_tools_ng/gtk/utils.py:758
+msgid "Nothing"
+msgstr "Nada"
 
-#: src/steam_tools_ng/gtk/authenticator.py:49
-msgid "New Authenticator"
-msgstr "Novo autenticador"
+#: src/steam_tools_ng/gtk/authenticator.py:39
+msgid "Manage Steam Authenticator"
+msgstr "Gerenciar Autenticador Steam"
 
-#: src/steam_tools_ng/gtk/authenticator.py:69
+#: src/steam_tools_ng/gtk/authenticator.py:51
 msgid "SMS Code:"
 msgstr "Código SMS:"
 
-#: src/steam_tools_ng/gtk/authenticator.py:117
+#: src/steam_tools_ng/gtk/authenticator.py:56
+msgid "Revocation Code:"
+msgstr "Código de Revogação:"
+
+#: src/steam_tools_ng/gtk/authenticator.py:108
+#: src/steam_tools_ng/gtk/authenticator.py:218
 msgid ""
 "Some login data is missing. If the problem persists, go to:\n"
 "Settings -> Login -> Advanced -> and click on RESET Everything."
 msgstr ""
 "Algum dado de login está faltando. Se o problema persistir, vá para:\n"
 "Configurações -> Login -> Avançado -> e clique em RESETAR Tudo."
 
-#: src/steam_tools_ng/gtk/authenticator.py:145
+#: src/steam_tools_ng/gtk/authenticator.py:136
 msgid ""
 "Enter bellow the code received by SMS\n"
 "and click on 'Add Authenticator' button"
 msgstr ""
 "Insira abaixo o código recebido por SMS\n"
 "e clique no botão 'Adicionar Autenticador'"
 
-#: src/steam_tools_ng/gtk/authenticator.py:164
+#: src/steam_tools_ng/gtk/authenticator.py:143
+#: src/steam_tools_ng/gtk/authenticator.py:207
+msgid "Add Authenticator"
+msgstr "Adicionar Autenticador"
+
+#: src/steam_tools_ng/gtk/authenticator.py:159
 msgid ""
 "Invalid SMS Code. Please,\n"
 "check the code and try again."
 msgstr ""
 "Código SMS inválido. Por favor,\n"
 "verifique o código e tente novamente."
 
-#: src/steam_tools_ng/gtk/confirmation.py:49
+#: src/steam_tools_ng/gtk/authenticator.py:225
+msgid ""
+"Enter bellow the revocation code and click on 'Remove Authenticator' button"
+msgstr ""
+"Insira abaixo o código de revogação e clique no botão 'Remover autenticador'"
+
+#: src/steam_tools_ng/gtk/authenticator.py:232
+#: src/steam_tools_ng/gtk/authenticator.py:252
+msgid "Remove Authenticator"
+msgstr "Remover Autenticador"
+
+#: src/steam_tools_ng/gtk/confirmation.py:48
 msgid "accept"
 msgstr "aceitar"
 
-#: src/steam_tools_ng/gtk/confirmation.py:51
+#: src/steam_tools_ng/gtk/confirmation.py:48
 msgid "cancel"
 msgstr "cancelar"
 
-#: src/steam_tools_ng/gtk/confirmation.py:61
+#: src/steam_tools_ng/gtk/confirmation.py:51
 msgid "Finalize Confirmation"
 msgstr "Finalizar Confirmação"
 
-#: src/steam_tools_ng/gtk/confirmation.py:79
-#: src/steam_tools_ng/gtk/coupon.py:72
+#: src/steam_tools_ng/gtk/confirmation.py:61
+#: src/steam_tools_ng/gtk/coupon.py:52
 msgid "Continue"
 msgstr "Continuar"
 
-#: src/steam_tools_ng/gtk/confirmation.py:84
-#: src/steam_tools_ng/gtk/coupon.py:76 src/steam_tools_ng/gtk/window.py:173
+#: src/steam_tools_ng/gtk/confirmation.py:66
+#: src/steam_tools_ng/gtk/coupon.py:56 src/steam_tools_ng/gtk/window.py:177
 msgid "Cancel"
 msgstr "Cancelar"
 
-#: src/steam_tools_ng/gtk/confirmation.py:89
-#: src/steam_tools_ng/gtk/coupon.py:89
-msgid "You must select something"
-msgstr "Você precisa selecionar alguma coisa"
-
-#: src/steam_tools_ng/gtk/confirmation.py:95
+#: src/steam_tools_ng/gtk/confirmation.py:72
 msgid ""
 "Do you really want to {} ALL confirmations?\n"
 "It can't be undone!"
 msgstr ""
 "Você realmente quer {} TODAS as confirmações?\n"
 "Isso não pode ser desfeito!"
 
-#: src/steam_tools_ng/gtk/confirmation.py:108
-msgid "You are trading the following items with {}:"
-msgstr "Você está trocando os seguintes items com {}:"
-
-#: src/steam_tools_ng/gtk/confirmation.py:113
+#: src/steam_tools_ng/gtk/confirmation.py:76
 msgid ""
-"Do you really want to {} that?\n"
+"{}\n"
+"Do you want to {} the offer?\n"
 "It can't be undone!"
 msgstr ""
-"Você realmente deseja {} este?\n"
+"{}\n"
+"Você quer {} a oferta?\n"
 "Isso não pode ser desfeito!"
 
-#: src/steam_tools_ng/gtk/confirmation.py:118
-msgid "You will give"
-msgstr "Você irá oferecer"
+#: src/steam_tools_ng/gtk/confirmation.py:83
+#: src/steam_tools_ng/gtk/coupon.py:82
+msgid "You must select something"
+msgstr "Você precisa selecionar alguma coisa"
 
 #: src/steam_tools_ng/gtk/confirmation.py:125
-msgid "You will receive"
-msgstr "Você irá receber"
-
-#: src/steam_tools_ng/gtk/confirmation.py:174
-msgid "Steam Server is slow. Please, try again."
-msgstr "O Servidor Steam está lento. Por favor, tente novamente."
+msgid ""
+"Unable to complete this confirmation. The reason is one of the following:\n"
+"\n"
+"1. The confirmation you choose already gone. Try another one.\n"
+"2. You wrote a wrong token in config. Update you config.\n"
+"3. The Steam server is slow. Wait a minute and try again.\n"
+"\n"
+"If you keep seeing this error, please update the confirmation list."
+msgstr ""
+"Não foi possível completar essa confirmação. A razão é uma dessas:\n"
+"\n"
+"1. A confirmação que você escolheu já se foi. Tente outra.\n"
+"2. Você escreveu um token errado na configuração. Atualize sua configuração.\n"
+"3. O servidor do Steam está lento. Aguarde 1 minuto e tente novamente.\n"
+"\n"
+"Se você continuar vendo esse erro, por favor atualize a lista de confirmações."
 
-#: src/steam_tools_ng/gtk/confirmation.py:190
+#: src/steam_tools_ng/gtk/confirmation.py:146
 msgid "Your steam is invalid. (are you logged in?)"
 msgstr "Seu steam é inválido. (você está logado?)"
 
-#: src/steam_tools_ng/gtk/confirmation.py:194
+#: src/steam_tools_ng/gtk/confirmation.py:150
 msgid "Waiting Steam Server (OP: {})"
 msgstr "Aguardando o Servidor do Steam (OP: {})"
 
-#: src/steam_tools_ng/gtk/confirmation.py:212
-#: src/steam_tools_ng/gtk/coupon.py:163
-#, python-format
-msgid "Unable to remove tree path %s (already removed?). Ignoring."
-msgstr ""
-"Não foi possível remover o caminho de árvore %s (já foi removido?). "
-"Ignorando."
-
-#: src/steam_tools_ng/gtk/confirmation.py:220
+#: src/steam_tools_ng/gtk/confirmation.py:179
 msgid "Waiting Steam Server response"
 msgstr "Aguardando resposta do Servidor Steam"
 
-#: src/steam_tools_ng/gtk/confirmation.py:239
-msgid "Updating tree"
-msgstr "Atualizando árvore"
-
-#: src/steam_tools_ng/gtk/coupon.py:54
+#: src/steam_tools_ng/gtk/coupon.py:64
 msgid "Get Coupon"
 msgstr "Obter Cupom"
 
-#: src/steam_tools_ng/gtk/coupon.py:82
+#: src/steam_tools_ng/gtk/coupon.py:68
 msgid "You must wait {} seconds to get another coupon"
 msgstr "Você precisa aguardar {} segundos antes de obter outro cupom"
 
-#: src/steam_tools_ng/gtk/coupon.py:96
-msgid ""
-"You are about to giveaway all coupons in your inventory\n"
-"The items will be automatically accepted and transfered in 1 minute"
-msgstr ""
-"Você está prestes a doar todos os cupons do seu inventário\n"
-"Os itens serão automaticamente aceitos e transferidos em 1 minuto"
-
-#: src/steam_tools_ng/gtk/coupon.py:105
+#: src/steam_tools_ng/gtk/coupon.py:77
 msgid ""
 "You are about to request {}\n"
 "The item will be automatically added at your inventory in 1 minute"
 msgstr ""
 "Você está prestes a requisitar {}\n"
 "O item será automaticamente adicionado ao seu inventário em 1 minuto"
 
-#: src/steam_tools_ng/gtk/coupon.py:133
+#: src/steam_tools_ng/gtk/coupon.py:87
+msgid "Send Coupon"
+msgstr "Enviar Cupom"
+
+#: src/steam_tools_ng/gtk/coupon.py:91
+msgid ""
+"You are about to giveaway all coupons in your inventory\n"
+"The items will be automatically accepted and transferred in 1 minute"
+msgstr ""
+"Você está prestes a doar todos os cupons do seu inventário\n"
+"Os itens serão automaticamente aceitos e transferidos em 1 minuto"
+
+#: src/steam_tools_ng/gtk/coupon.py:119
 msgid "Inventory is empty."
 msgstr "O inventário está vazio."
 
-#: src/steam_tools_ng/gtk/coupon.py:145
+#: src/steam_tools_ng/gtk/coupon.py:131
 msgid ""
 "Unable to complete this trade. The reason is one of the following:\n"
 "\n"
 "1. The item you choose already gone. Try another one.\n"
 "2. You wrote a wrong token in config. Update you config.\n"
 "3. The Steam server is slow. Wait a minute and try again.\n"
 "\n"
@@ -1014,263 +1088,248 @@
 "\n"
 "1. O item que você escolheu já acabou. Tente outro.\n"
 "2. Você escreveu um token errado na configuração. Atualize sua configuração.\n"
 "3. O servidor do Steam está lento. Aguarde 1 minuto e tente novamente.\n"
 "\n"
 "Se você continuar vendo esse erro, por favor atualize sua lista de cupons."
 
-#: src/steam_tools_ng/gtk/coupon.py:169
+#: src/steam_tools_ng/gtk/coupon.py:149
 msgid "Waiting Steam Server"
 msgstr "Aguardando o Servidor do Steam"
 
-#: src/steam_tools_ng/gtk/coupon.py:179
+#: src/steam_tools_ng/gtk/coupon.py:159
 msgid "Your steamid is invalid. (are you logged in?)"
 msgstr "Seu steamid é inválido. (você está logado?)"
 
-#: src/steam_tools_ng/gtk/coupon.py:207
+#: src/steam_tools_ng/gtk/coupon.py:183
 msgid "botid to donation is invalid. Check your config."
 msgstr "botid de doação é inválido. Verifique sua configuração."
 
-#: src/steam_tools_ng/gtk/coupon.py:219
+#: src/steam_tools_ng/gtk/coupon.py:195
 msgid "You will need to manually confirm the trade offer. Check your email."
 msgstr "Você vai precisar confirmar a troca manualmente. Verifique seu email."
 
-#: src/steam_tools_ng/gtk/coupon.py:230
+#: src/steam_tools_ng/gtk/coupon.py:206
 msgid ""
 "Mobile confirmation is needed but the confirmation module isn't enabled.\n"
 "You will need to manually confirm the trade offer."
 msgstr ""
 "Uma confirmação de celular é necessária mas o módulo de confirmações não está habilitado.\n"
 "Você vai precisar confirmar manualmente a oferta de troca."
 
-#: src/steam_tools_ng/gtk/coupon.py:255
+#: src/steam_tools_ng/gtk/coupon.py:229
 msgid "Waiting trade confirmation"
 msgstr "Aguardando a confirmação da troca"
 
-#: src/steam_tools_ng/gtk/login.py:50
+#: src/steam_tools_ng/gtk/login.py:48
 msgid "Log-in"
 msgstr "Logar"
 
-#: src/steam_tools_ng/gtk/login.py:56
+#: src/steam_tools_ng/gtk/login.py:51
 msgid "Login"
 msgstr "Login"
 
-#: src/steam_tools_ng/gtk/login.py:76 src/steam_tools_ng/gtk/window.py:292
+#: src/steam_tools_ng/gtk/login.py:59 src/steam_tools_ng/gtk/window.py:295
 msgid "Username:"
 msgstr "Nome de usuário:"
 
-#: src/steam_tools_ng/gtk/login.py:78
+#: src/steam_tools_ng/gtk/login.py:61
 msgid "Password:"
 msgstr "Senha:"
 
-#: src/steam_tools_ng/gtk/login.py:82
-msgid "Steam Code:"
-msgstr "Código Steam:"
-
-#: src/steam_tools_ng/gtk/login.py:83
-msgid "Mail Code:"
-msgstr "Código do Email:"
-
-#: src/steam_tools_ng/gtk/login.py:86
+#: src/steam_tools_ng/gtk/login.py:65
 msgid "Code:"
 msgstr "Código:"
 
-#: src/steam_tools_ng/gtk/login.py:89
-msgid "Captcha Text:"
-msgstr "Texto captcha:"
-
-#: src/steam_tools_ng/gtk/login.py:92
+#: src/steam_tools_ng/gtk/login.py:69
 msgid "Save Password:"
 msgstr "Salvar Senha:"
 
-#: src/steam_tools_ng/gtk/login.py:97
+#: src/steam_tools_ng/gtk/login.py:76
 msgid "Advanced Login"
 msgstr "Login Avançado"
 
-#: src/steam_tools_ng/gtk/login.py:107 src/steam_tools_ng/gtk/window.py:282
+#: src/steam_tools_ng/gtk/login.py:88 src/steam_tools_ng/gtk/window.py:285
 msgid "Identity Secret:"
 msgstr "Segredo de Identidade:"
 
-#: src/steam_tools_ng/gtk/login.py:114 src/steam_tools_ng/gtk/window.py:273
+#: src/steam_tools_ng/gtk/login.py:95 src/steam_tools_ng/gtk/window.py:276
 msgid "Shared Secret:"
 msgstr "Segredo Partilhado:"
 
-#: src/steam_tools_ng/gtk/login.py:179
+#: src/steam_tools_ng/gtk/login.py:144
 msgid "Login cancelled! Modules will not work correctly!"
 msgstr "Login cancelado! Os módulos não funcionarão corretamente!"
 
-#: src/steam_tools_ng/gtk/login.py:194
+#: src/steam_tools_ng/gtk/login.py:163
 msgid "Username or Password is blank!"
 msgstr "Nome de usuário ou Senha está vazio!"
 
-#: src/steam_tools_ng/gtk/login.py:239
+#: src/steam_tools_ng/gtk/login.py:200
 msgid ""
 "Write code received by email\n"
 "and click on 'Log-in' button"
 msgstr ""
 "Escreva o código recebido por email\n"
 "e click no botão 'Logar'"
 
-#: src/steam_tools_ng/gtk/login.py:257
+#: src/steam_tools_ng/gtk/login.py:209
+msgid "Retrying login in {} seconds"
+msgstr "Tentando entrar novamente em {} segundos"
+
+#: src/steam_tools_ng/gtk/login.py:221
 msgid "Write Steam Code bellow and click on 'Log-in'"
 msgstr "Escreva o Código Steam abaixo e clique em 'Logar'"
 
-#: src/steam_tools_ng/gtk/login.py:272
+#: src/steam_tools_ng/gtk/login.py:238
 msgid ""
 "Write captcha code as shown bellow\n"
 "and click on 'Log-in' button"
 msgstr ""
 "Escreva o código captcha como mostrado abaixo\n"
 "e clique no botão 'Logar'"
 
-#: src/steam_tools_ng/gtk/settings.py:43 src/steam_tools_ng/gtk/window.py:66
-#: src/steam_tools_ng/gtk/window.py:192 src/steam_tools_ng/gtk/window.py:313
-#: src/steam_tools_ng/gtk/window.py:373 src/steam_tools_ng/gtk/window.py:491
-#: src/steam_tools_ng/gtk/window.py:597
+#: src/steam_tools_ng/gtk/login.py:260
+msgid ""
+"\n"
+"\n"
+"If your previous authenticator has been removed,\n"
+"open advanced login bellow and remove the old secrets."
+msgstr ""
+"\n"
+"\n"
+"Se o autenticador anterior foi removido,\n"
+"abra o login avançado abaixo e remova os segredos antigos."
+
+#: src/steam_tools_ng/gtk/login.py:275
+msgid ""
+"Check your connection. (server down? blocked?)\n"
+"Waiting {}"
+msgstr ""
+"Verifique sua conexão. (server caiu? bloqueado?)\n"
+"Aguardando {}"
+
+#: src/steam_tools_ng/gtk/settings.py:40 src/steam_tools_ng/gtk/window.py:66
+#: src/steam_tools_ng/gtk/window.py:196 src/steam_tools_ng/gtk/window.py:316
+#: src/steam_tools_ng/gtk/window.py:372 src/steam_tools_ng/gtk/window.py:487
+#: src/steam_tools_ng/gtk/window.py:596
 msgid "Settings"
 msgstr "Configurações"
 
-#: src/steam_tools_ng/gtk/settings.py:66
+#: src/steam_tools_ng/gtk/settings.py:51
 msgid "General"
 msgstr "Geral"
 
-#: src/steam_tools_ng/gtk/settings.py:69
+#: src/steam_tools_ng/gtk/settings.py:54
 msgid "Config File Directory"
 msgstr "Diretório do Arquivo de Configuração"
 
-#: src/steam_tools_ng/gtk/settings.py:75
+#: src/steam_tools_ng/gtk/settings.py:60
 msgid "Config / Log file Directory"
 msgstr "Diretório do arquivo de Configuração / Log"
 
-#: src/steam_tools_ng/gtk/settings.py:79
+#: src/steam_tools_ng/gtk/settings.py:64
 msgid "Log File Directory"
 msgstr "Diretório do Arquivo de Log"
 
-#: src/steam_tools_ng/gtk/settings.py:87
+#: src/steam_tools_ng/gtk/settings.py:72
 msgid "Theme:"
 msgstr "Tema:"
 
-#: src/steam_tools_ng/gtk/settings.py:96
+#: src/steam_tools_ng/gtk/settings.py:81
+#: src/steam_tools_ng/gtk/settings.py:150
 msgid "Language"
 msgstr "Idioma"
 
-#: src/steam_tools_ng/gtk/settings.py:102
+#: src/steam_tools_ng/gtk/settings.py:87
 msgid "Show close button:"
 msgstr "Mostrar botão fechar:"
 
-#: src/steam_tools_ng/gtk/settings.py:111
+#: src/steam_tools_ng/gtk/settings.py:96
 msgid "Logger"
 msgstr "Logger"
 
-#: src/steam_tools_ng/gtk/settings.py:115
+#: src/steam_tools_ng/gtk/settings.py:100
 msgid "Level:"
 msgstr "Nível:"
 
-#: src/steam_tools_ng/gtk/settings.py:123
+#: src/steam_tools_ng/gtk/settings.py:108
 msgid "Console level:"
 msgstr "Nível do console:"
 
-#: src/steam_tools_ng/gtk/settings.py:132
+#: src/steam_tools_ng/gtk/settings.py:117
 msgid "Log color:"
 msgstr "Cor do log:"
 
-#: src/steam_tools_ng/gtk/utils.py:186 src/steam_tools_ng/gtk/utils.py:234
+#: src/steam_tools_ng/gtk/settings.py:153
+msgid "You must restart the STNG to apply the new language"
+msgstr "Você precisa reiniciar o STNG para aplicar o novo idioma"
+
+#: src/steam_tools_ng/gtk/utils.py:238 src/steam_tools_ng/gtk/utils.py:334
 msgid "Waiting another process"
 msgstr "Aguardando outro processo"
 
-#: src/steam_tools_ng/gtk/utils.py:290
+#: src/steam_tools_ng/gtk/utils.py:398
 msgid "Waiting"
 msgstr "Aguardando"
 
-#: src/steam_tools_ng/gtk/utils.py:341
+#: src/steam_tools_ng/gtk/utils.py:449
 msgid "Loading..."
 msgstr "Carregando..."
 
-#: src/steam_tools_ng/gtk/utils.py:378
+#: src/steam_tools_ng/gtk/utils.py:483
 msgid "Text Copied to Clipboard"
 msgstr "Texto copiado para a Área de Transferência"
 
-#: src/steam_tools_ng/gtk/utils.py:546
+#: src/steam_tools_ng/gtk/utils.py:616
 msgid ""
 "Please, fix your config file. Accepted values for {} are:\n"
 "{}"
 msgstr ""
 "Por favor, corrija seu arquivo de configuração. Valores aceitos para {} são:\n"
 "{}"
 
-#: src/steam_tools_ng/gtk/utils.py:611
-msgid "Ignoring value from {} on column {} item {} because value is empty"
-msgstr "Ignorando valor de {} na coluna {} item {} porque o valor está vazio"
-
-#: src/steam_tools_ng/gtk/utils.py:624
-msgid "Nothing"
-msgstr "Nada"
-
-#: src/steam_tools_ng/gtk/utils.py:628
+#: src/steam_tools_ng/gtk/utils.py:762
 msgid "Various"
 msgstr "Vários"
 
-#: src/steam_tools_ng/gtk/utils.py:668
-msgid "Fatal Error"
-msgstr "Erro Fatal"
-
-#: src/steam_tools_ng/gtk/utils.py:689
+#: src/steam_tools_ng/gtk/utils.py:794
 msgid "Ok"
 msgstr "Ok"
 
 #: src/steam_tools_ng/gtk/window.py:67
 msgid "About"
 msgstr "Sobre"
 
 #: src/steam_tools_ng/gtk/window.py:68
 msgid "Exit"
 msgstr "Sair"
 
-#: src/steam_tools_ng/gtk/window.py:118
+#: src/steam_tools_ng/gtk/window.py:97
+msgid "Limited Account! Some modules will not work!"
+msgstr "Conta Limitada! Alguns módulos não irão funcionar!"
+
+#: src/steam_tools_ng/gtk/window.py:130
 msgid "Coupons"
 msgstr "Cupons"
 
-#: src/steam_tools_ng/gtk/window.py:142
-msgid "confid"
-msgstr "confid"
-
-#: src/steam_tools_ng/gtk/window.py:142
-msgid "creatorid"
-msgstr "creatorid"
-
-#: src/steam_tools_ng/gtk/window.py:142
-msgid "key"
-msgstr "chave"
-
-#: src/steam_tools_ng/gtk/window.py:142
-msgid "give"
-msgstr "oferecendo"
-
-#: src/steam_tools_ng/gtk/window.py:142
-msgid "to"
-msgstr "para"
-
-#: src/steam_tools_ng/gtk/window.py:142
-msgid "receive"
-msgstr "recebendo"
-
-#: src/steam_tools_ng/gtk/window.py:166
+#: src/steam_tools_ng/gtk/window.py:170
 msgid "Accept"
 msgstr "Aceitar"
 
-#: src/steam_tools_ng/gtk/window.py:180
+#: src/steam_tools_ng/gtk/window.py:184
 msgid "Accept All"
 msgstr "Aceitar Tudo"
 
-#: src/steam_tools_ng/gtk/window.py:187
+#: src/steam_tools_ng/gtk/window.py:191
 msgid "Cancel All"
 msgstr "Cancelar Tudo"
 
-#: src/steam_tools_ng/gtk/window.py:195 src/steam_tools_ng/gtk/window.py:315
-#: src/steam_tools_ng/gtk/window.py:375 src/steam_tools_ng/gtk/window.py:493
+#: src/steam_tools_ng/gtk/window.py:199 src/steam_tools_ng/gtk/window.py:318
+#: src/steam_tools_ng/gtk/window.py:374 src/steam_tools_ng/gtk/window.py:489
 msgid "Enable:"
 msgstr "Habilitar:"
 
 #: src/steam_tools_ng/gtk/window.py:209
 msgid ""
 "steamguard module has been disabled because you have\n"
 "logged in but no shared secret is found. To enable it again,\n"
@@ -1278,247 +1337,243 @@
 "or use STNG as your Steam Authenticator\n"
 msgstr ""
 "o módulo steamguard foi desabilitado porque você logou mas\n"
 "nenhum segredo partilhado foi encontrado. Para habilitar isso novamente,\n"
 "vá para Avançado e adicione um segredo partilhado válido\n"
 "ou use o STNG como seu Steam Authenticator\n"
 
-#: src/steam_tools_ng/gtk/window.py:219
+#: src/steam_tools_ng/gtk/window.py:220
 msgid "Enable Confirmations:"
 msgstr "Habilitar Confirmações:"
 
-#: src/steam_tools_ng/gtk/window.py:235
+#: src/steam_tools_ng/gtk/window.py:231
 msgid ""
 "confirmations module has been disabled because you have\n"
 "logged in but no identity secret is found. To enable it again,\n"
 "go to login -> advanced and add a valid identity secret\n"
 "or use STNG as your Steam Authenticator\n"
 msgstr ""
 "o módulo confirmações foi desabilitado por que você logou\n"
 "mas nenhum segredo partilhado foi encontrado. Para habilitar\n"
 "isso novamente, vá para login -> avançado e adicione um segredo\n"
 "partilhado válido ou use o STNG como seu Autenticador Steam\n"
 
-#: src/steam_tools_ng/gtk/window.py:246
+#: src/steam_tools_ng/gtk/window.py:243
 msgid "Login with another account"
 msgstr "Logar com outra conta"
 
-#: src/steam_tools_ng/gtk/window.py:252
-msgid "Use STNG as your Steam Authenticator"
-msgstr "Usar o STNG como seu Autenticador Steam"
+#: src/steam_tools_ng/gtk/window.py:249
+msgid "Add STNG as your Steam Authenticator"
+msgstr "Adicionar STNG como seu Autenticador Steam"
+
+#: src/steam_tools_ng/gtk/window.py:255
+msgid "Remove STNG Authenticator from your Steam Account"
+msgstr "Remover o Autenticador STNG da sua Conta Steam"
 
-#: src/steam_tools_ng/gtk/window.py:258
+#: src/steam_tools_ng/gtk/window.py:261
 msgid "Remove Saved Password"
 msgstr "Remover Senha Salva"
 
-#: src/steam_tools_ng/gtk/window.py:264
+#: src/steam_tools_ng/gtk/window.py:267
 msgid "Advanced"
 msgstr "Avançado"
 
-#: src/steam_tools_ng/gtk/window.py:268
+#: src/steam_tools_ng/gtk/window.py:271
 msgid ""
 "Warning: Don't mess up these settings unless you know what you are doing!"
 msgstr ""
 "Aviso: Não mexa nessas configurações a não ser que você saiba o que está "
 "fazendo!"
 
-#: src/steam_tools_ng/gtk/window.py:276
-msgid "Token:"
-msgstr "Token:"
-
 #: src/steam_tools_ng/gtk/window.py:279
-msgid "Token Secure:"
-msgstr "Token Seguro:"
+msgid "Access Token:"
+msgstr "Token de Acesso:"
+
+#: src/steam_tools_ng/gtk/window.py:282
+msgid "Refresh Token:"
+msgstr "Token de Atualização:"
 
-#: src/steam_tools_ng/gtk/window.py:285
+#: src/steam_tools_ng/gtk/window.py:288
 msgid "Device ID:"
 msgstr "ID de Dispositivo:"
 
-#: src/steam_tools_ng/gtk/window.py:288
+#: src/steam_tools_ng/gtk/window.py:291
 msgid "Steam ID:"
 msgstr "ID do Steam:"
 
-#: src/steam_tools_ng/gtk/window.py:296
+#: src/steam_tools_ng/gtk/window.py:299
 msgid "Reset Everything (USE WITH CAUTION!!!)"
 msgstr "Resetar Tudo (USE COM CUIDADO!!!)"
 
-#: src/steam_tools_ng/gtk/window.py:319
+#: src/steam_tools_ng/gtk/window.py:321
 msgid "Mandatory waiting:"
 msgstr "Espera obrigatória:"
 
-#: src/steam_tools_ng/gtk/window.py:324
+#: src/steam_tools_ng/gtk/window.py:326
 msgid "Wait while running:"
 msgstr "Espera enquanto roda:"
 
-#: src/steam_tools_ng/gtk/window.py:330
+#: src/steam_tools_ng/gtk/window.py:332
 msgid "Wait for drops:"
 msgstr "Espera pelos drops:"
 
-#: src/steam_tools_ng/gtk/window.py:333
+#: src/steam_tools_ng/gtk/window.py:335
 msgid "Max concurrency:"
 msgstr "Simultaneidade Máxima:"
 
-#: src/steam_tools_ng/gtk/window.py:336
+#: src/steam_tools_ng/gtk/window.py:338
 msgid "Invisible:"
 msgstr "Invisível:"
 
-#: src/steam_tools_ng/gtk/window.py:340
+#: src/steam_tools_ng/gtk/window.py:341
 msgid "Reverse Sorting:"
 msgstr "Organizar Inversamente:"
 
 #: src/steam_tools_ng/gtk/window.py:352
 msgid ""
 "cardfarming module has been disabled because you have\n"
 "a stlib built without SteamWorks support. To enable it again,\n"
 "reinstall stlib with SteamWorks support\n"
 msgstr ""
 "o módulo de fazenda de cartas foi desabilitado porque você tem\n"
 "um stlib construído sem suporte a SteamWorks. Para habilitar novamente,\n"
 "reinstale a stlib com suporte a SteamWorks.\n"
 
-#: src/steam_tools_ng/gtk/window.py:380
+#: src/steam_tools_ng/gtk/window.py:378
 msgid "Developer Giveaways"
 msgstr "Giveaways de Desenvolvedor"
 
-#: src/steam_tools_ng/gtk/window.py:388
+#: src/steam_tools_ng/gtk/window.py:385
 msgid "Mode:"
 msgstr "Modo:"
 
-#: src/steam_tools_ng/gtk/window.py:396
+#: src/steam_tools_ng/gtk/window.py:393
 msgid "Wait after each strategy:"
 msgstr "Espera após cada estratégia:"
 
-#: src/steam_tools_ng/gtk/window.py:403
+#: src/steam_tools_ng/gtk/window.py:400
 msgid "Wait after full cycle:"
 msgstr "Espera após ciclo completo:"
 
-#: src/steam_tools_ng/gtk/window.py:409
+#: src/steam_tools_ng/gtk/window.py:406
 msgid "Minimum points:"
 msgstr "Pontos mínimos:"
 
-#: src/steam_tools_ng/gtk/window.py:414 src/steam_tools_ng/gtk/window.py:417
+#: src/steam_tools_ng/gtk/window.py:411 src/steam_tools_ng/gtk/window.py:414
 msgid "Strategy {}"
 msgstr "Estratégia {}"
 
-#: src/steam_tools_ng/gtk/window.py:425
+#: src/steam_tools_ng/gtk/window.py:421
 msgid "Minimum"
 msgstr "Mínimo"
 
-#: src/steam_tools_ng/gtk/window.py:429
+#: src/steam_tools_ng/gtk/window.py:425
 msgid "Maximum"
 msgstr "Máximo"
 
-#: src/steam_tools_ng/gtk/window.py:445
+#: src/steam_tools_ng/gtk/window.py:441
 msgid "Restrict Type:"
 msgstr "Restringir Tipo:"
 
-#: src/steam_tools_ng/gtk/window.py:454
+#: src/steam_tools_ng/gtk/window.py:450
 msgid "Sort Type:"
 msgstr "Tipo de Ordenação:"
 
-#: src/steam_tools_ng/gtk/window.py:471
+#: src/steam_tools_ng/gtk/window.py:467
 msgid ""
 "steamgifts module has been disabled because you don't\n"
 "have steamgifts plugin installed. To enable it again,\n"
 "install the steamgifts plugin.\n"
 msgstr ""
 "o módulo steamgifts foi desabilitado porque você não\n"
 "tem o plugin steamgifts instalado. Para habilitar ele novamente,\n"
 "instale o plugin steamgifts.\n"
 
-#: src/steam_tools_ng/gtk/window.py:499
+#: src/steam_tools_ng/gtk/window.py:494
 msgid "Trade IDs:"
 msgstr "IDs dos Trades:"
 
-#: src/steam_tools_ng/gtk/window.py:503
+#: src/steam_tools_ng/gtk/window.py:498
 msgid "Wait for Bump:"
 msgstr "Espera para Bump:"
 
-#: src/steam_tools_ng/gtk/window.py:514
+#: src/steam_tools_ng/gtk/window.py:509
 msgid ""
 "steamtrades module has been disabled because you don't\n"
 "have steamtrades plugin installed. To enable it again,\n"
 "install the steamtrades plugin.\n"
 msgstr ""
 "o módulo steamtrades foi desabilitado porque você não\n"
 "tem o plugin steamtrades instalado. Para habilitar ele novamente,\n"
 "instale o plugin steamtrades.\n"
 
-#: src/steam_tools_ng/gtk/window.py:524
+#: src/steam_tools_ng/gtk/window.py:519
 msgid ""
 "Warning: It's a heavy uncached operation. Fetch only once a day or you will "
 "be blocked."
 msgstr ""
 "Aviso: Isso é uma operação pesada não cacheada. Busque somente uma vez ao "
 "dia ou você será bloqueado."
 
-#: src/steam_tools_ng/gtk/window.py:542
+#: src/steam_tools_ng/gtk/window.py:537
 msgid "Coupon List"
 msgstr "Lista de Cupons"
 
-#: src/steam_tools_ng/gtk/window.py:545
-msgid "price"
-msgstr "preço"
-
-#: src/steam_tools_ng/gtk/window.py:545
-msgid "name"
-msgstr "nome"
-
-#: src/steam_tools_ng/gtk/window.py:569
+#: src/steam_tools_ng/gtk/window.py:568
 msgid "Fetch"
 msgstr "Buscar"
 
-#: src/steam_tools_ng/gtk/window.py:578
+#: src/steam_tools_ng/gtk/window.py:577
 msgid "Stop fetching"
 msgstr "Parar de buscar"
 
-#: src/steam_tools_ng/gtk/window.py:585
+#: src/steam_tools_ng/gtk/window.py:584
 msgid "Get selected"
 msgstr "Obter o selecionado"
 
-#: src/steam_tools_ng/gtk/window.py:592
+#: src/steam_tools_ng/gtk/window.py:591
 msgid "Send"
 msgstr "Enviar"
 
-#: src/steam_tools_ng/gtk/window.py:599
+#: src/steam_tools_ng/gtk/window.py:598
 msgid "BotIDs:"
 msgstr "BotIDs:"
 
-#: src/steam_tools_ng/gtk/window.py:603
+#: src/steam_tools_ng/gtk/window.py:602
 msgid "Tokens:"
 msgstr "Tokens:"
 
-#: src/steam_tools_ng/gtk/window.py:607
+#: src/steam_tools_ng/gtk/window.py:606
 msgid "BotID To Donate:"
 msgstr "BotID para Doação:"
 
-#: src/steam_tools_ng/gtk/window.py:610
+#: src/steam_tools_ng/gtk/window.py:609
 msgid "Token To Donate:"
 msgstr "Token para Doação:"
 
-#: src/steam_tools_ng/gtk/window.py:613
+#: src/steam_tools_ng/gtk/window.py:612
 msgid "Blacklist:"
 msgstr "Lista Negra:"
 
-#: src/steam_tools_ng/gtk/window.py:618
+#: src/steam_tools_ng/gtk/window.py:617
 msgid "Minimum Discount:"
 msgstr "Desconto mínimo:"
 
-#: src/steam_tools_ng/gtk/window.py:673
+#: src/steam_tools_ng/gtk/window.py:665
 msgid "You are logged in as:\n"
 msgstr "Você está logado como:\n"
 
-#: src/steam_tools_ng/gtk/window.py:874
+#: src/steam_tools_ng/gtk/window.py:871
 msgid "Reseting... Please wait!"
 msgstr "Resetando... Por favor aguarde!"
 
-#: src/steam_tools_ng/gtk/window.py:899
-msgid "Removing saved password..."
-msgstr "Removendo senha salva..."
-
-#: src/steam_tools_ng/gtk/window.py:911
+#: src/steam_tools_ng/gtk/window.py:886 src/steam_tools_ng/gtk/window.py:905
 msgid ""
 "Successful!\n"
 "Exiting..."
 msgstr ""
 "Sucesso!\n"
 "Saindo..."
+
+#: src/steam_tools_ng/gtk/window.py:893
+msgid "Removing saved password..."
+msgstr "Removendo senha salva..."
```

### Comparing `steam-tools-ng-3.1/pyproject.toml` & `steam-tools-ng-3.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "certifi", "cx_Freeze; sys_platform == 'win32'"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "steam-tools-ng"
-version = "3.1"
+version = "3.1.1"
 description = "Steam Tools NG"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "GPLv3"}
 keywords = ["steam", "valve"]
 authors = [{email = "dev@lara.monster"}, {name = "Lara Maia"}]
 classifiers = [
```

### Comparing `steam-tools-ng-3.1/setup.py` & `steam-tools-ng-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/__init__.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/__init__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/__main__.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/__main__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/cli.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/cli.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/config.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,17 +93,17 @@
     ('points+', _("Points (0-50)")),
     ('points-', _("Points (50-0)")),
     ('level+', _("Level (0-100)")),
     ('level-', _("Level (100-0)")),
 ])
 
 steamgifts_modes = OrderedDict([
-    ('run_all_and_restart', _('Run all and restart')),
-    ('stop_after_minimum_and_wait', _('Stop after reach minimum points and wait')),
-    ('stop_after_minimum_and_restart', _('Stop after reach minimum points and restart')),
+    ('run_all_and_restart', _('Run all and restart\nRun all strategies and restart')),
+    ('stop_after_minimum_and_wait', _('Stop and wait\nafter minimum points')),
+    ('stop_after_minimum_and_restart', _('Stop and restart\nafter minimum points')),
 ])
 
 plugins = OrderedDict([
     ("coupons", _("Free Coupons")),
     ("confirmations", _("Confirmations")),
     ("steamtrades", _("Steam Trades")),
     ("steamgifts", _("Steam Gifts")),
```

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/console/authenticator.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/console/authenticator.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/console/cli.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/console/cli.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/console/login.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/console/login.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/console/utils.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/console/utils.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/core/__init__.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/core/__init__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/core/cardfarming.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/core/cardfarming.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/core/confirmations.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/core/confirmations.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/core/coupons.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/core/coupons.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/core/fakerun.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/core/fakerun.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/core/steamgifts.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/core/steamgifts.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/core/steamguard.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/core/steamguard.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/core/steamtrades.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/core/steamtrades.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/core/utils.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/core/utils.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/gtk/__init__.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/__init__.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/gtk/about.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/about.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/gtk/application.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,17 @@
             while self.main_window.get_realized():
                 if login_window.has_user_data:
                     break
 
                 await asyncio.sleep(1)
 
     async def async_activate(self) -> None:
+        # TODO: Wait for window manager catch the main window position and size
+        await asyncio.sleep(3)
+
         assert isinstance(self.main_window, window.Main)
         login_session = await login.Login.new_session(0, api_url=self.api_url)
 
         self.main_window.statusbar.set_warning("steamguard", _("Logging on Steam. Please wait!"))
         log.info(_("Logging on Steam"))
         try_count = 3
```

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/gtk/async_gtk.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/async_gtk.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/gtk/authenticator.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/authenticator.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/gtk/confirmation.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/confirmation.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/gtk/coupon.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/coupon.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/gtk/login.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/login.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/gtk/settings.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,22 +54,28 @@
         config_button.set_label(_("Config File Directory"))
         config_button.set_name("config_button")
         config_button.set_hexpand(True)
         config_button.connect("clicked", self.on_config_button_clicked)
 
         if config.parser.get("logger", "log_directory") == str(config.config_file_directory):
             config_button.set_label(_("Config / Log file Directory"))
-            general_section.grid.attach(config_button, 0, 1, 2, 1)
+            general_section.attach(config_button, 0, 1, 2, 1)
         else:
+            buttons_grid = Gtk.Grid()
+            buttons_grid.set_column_homogeneous(10)
+            buttons_grid.set_column_spacing(10)
+
             log_button = Gtk.Button()
             log_button.set_label(_("Log File Directory"))
             log_button.set_name("log_button")
             log_button.connect("clicked", self.on_log_button_clicked)
-            general_section.grid.attach(config_button, 0, 1, 1, 1)
-            general_section.grid.attach(log_button, 1, 1, 1, 1)
+
+            buttons_grid.attach(config_button, 0, 1, 1, 1)
+            buttons_grid.attach(log_button, 1, 1, 1, 1)
+            general_section.attach(buttons_grid, 0, 1, 2, 1)
 
         theme = general_section.new_item(
             "theme",
             _("Theme:"),
             Gtk.DropDown,
             0, 3,
             items=config.gtk_themes,
```

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/gtk/utils.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -558,120 +558,130 @@
         self._display.set_markup(markup(self._default_display_text, font_size='large', font_weight='bold'))
 
     def unset_level(self) -> None:
         self._level_bar.set_value(0)
         self._level_bar.set_max_value(0)
 
 
-class Section(Gtk.Grid):
-    items = []
-
-    def __init__(self, name: str) -> None:
+class _SectionItem(Gtk.Grid):
+    def __init__(self,
+                 section: 'Section',
+                 name: str,
+                 label: Optional[str],
+                 widget: Type[Gtk.Widget],
+                 items: Optional[OrderedDict[str, str]] = None,
+                 ) -> None:
         super().__init__()
-        # for backward compatibility
-        self.grid = self
+        self.set_column_homogeneous(True)
 
+        self.section = section
+        self.items = items
         self.set_name(name)
-        self.set_row_spacing(10)
-        self.set_column_spacing(10)
-        self.set_margin_top(10)
-        self.set_margin_bottom(10)
-        self.set_margin_start(10)
-        self.set_margin_end(10)
 
-    # noinspection PyProtectedMember
-    @staticmethod
-    def __get_section_name(item: 'Item') -> str:
-        assert isinstance(item._section_name, str)
-        return item._section_name
-
-    @staticmethod
-    def __set_visible(item: 'Item', state: bool) -> None:
-        item.label.set_visible(state)
-        super(item.__class__, item).set_visible(state)
-
-    @staticmethod
-    def __update_values(item: 'Item', items: Optional[OrderedDict[str, str]] = None) -> None:
-        if isinstance(item, Gtk.DropDown):
-            assert isinstance(items, OrderedDict), "DropDown needs items mapping"
-            value = config.parser.get(item.get_section_name(), item.get_name())
+        self.widget = widget()
+        self.widget.set_hexpand(True)
+
+        if isinstance(self.widget, Gtk.Switch):
+            self.widget.set_halign(Gtk.Align.END)
+
+        if label:
+            self.label = Gtk.Label()
+            self.label.set_name(name)
+            self.label.set_text(label)
+            self.label.set_halign(Gtk.Align.START)
+
+            self.attach(self.label, 0, 0, 1, 1)
+            self.attach_next_to(self.widget, self.label, Gtk.PositionType.RIGHT, 1, 1)
+        else:
+            self.attach(self.widget, 0, 0, 1, 1)
+
+        if items:
             string_list = Gtk.StringList()
 
             for option_label in items.values():
                 string_list.append(_(option_label))
 
-            item.set_model(string_list)
+            self.widget.set_model(string_list)
 
-            try:
-                current_option = list(items).index(value)
-            except ValueError:
-                import sys
-
-                error_message = _("Please, fix your config file. Accepted values for {} are:\n{}").format(
-                    item.get_name(),
-                    ', '.join(items.keys()),
-                )
-                log.exception(error_message)
-                traceback_info = sys.exc_info()[2]
-                fatal_error_dialog(ValueError(error_message), traceback.extract_tb(traceback_info))
-                # unset active item
-                current_option = -1
-
-            item.set_selected(current_option)
-
-        if isinstance(item, (Gtk.CheckButton, Gtk.Switch)):
-            value = config.parser.getboolean(item.get_section_name(), item.get_name())
-            item.set_active(value)
-
-        if isinstance(item, Gtk.Entry):
-            if value := config.parser.get(item.get_section_name(), item.get_name()):
-                item.set_text(value)
+    def __getattr__(self, item: str) -> Any:
+        return getattr(self.widget, item)
 
-    def new_item(
-            self,
-            name: str,
-            label: Optional[str],
-            widget: Type[Gtk.Widget],
-            *grid_position: int,
-            items: Optional[OrderedDict[str, str]] = None,
-    ) -> Gtk.Widget:
-        bases = (widget,)
+    def __update_dropdown(self) -> None:
+        value = config.parser.get(self.section.get_name(), self.get_name())
 
-        body = {
-            'label': None,
-            '_section_name': None,
-            '__init__': lambda item_: super(item_.__class__, item_).__init__(),
-            'get_section_name': self.__get_section_name,
-            'set_visible': self.__set_visible,
-            'update_values': lambda item_: self.__update_values(item_, items)
-        }
+        try:
+            current_option = list(self.items).index(value)
+        except ValueError:
+            import sys
 
-        if label:
-            body['label'] = Gtk.Label()
+            error_message = _("Please, fix your config file. Accepted values for {} are:\n{}").format(
+                self.name,
+                ', '.join(self.items.keys()),
+            )
+            log.exception(error_message)
+            traceback_info = sys.exc_info()[2]
+            fatal_error_dialog(ValueError(error_message), traceback.extract_tb(traceback_info))
+            # unset active item
+            current_option = -1
 
-        section = self.get_name()
-        value: Union[str, bool, int]
+        self.widget.set_selected(current_option)
 
-        item = type('Item', bases, body)()
-        assert isinstance(item, Gtk.Widget)
+    def __update_switch(self) -> None:
+        value = config.parser.getboolean(self.section.get_name(), self.get_name())
 
-        item.set_hexpand(True)
-        item.set_name(name)
-        item._section_name = section
+        self.widget.set_active(value)
 
-        if item.label:
-            item.label.set_name(name)
-            item.label.set_text(label)
-            item.label.set_halign(Gtk.Align.START)
+    def __update_entry(self) -> None:
+        value = config.parser.get(self.section.get_name(), self.get_name())
+
+        self.widget.get_buffer().set_text(value, -1)
+
+    def update_values(self) -> None:
+        if config.config_file.is_file():
+            config.parser.read(config.config_file)
+        else:
+            log.debug("Config file not read")
 
-            self.grid.attach(item.label, *grid_position, 1, 1)
-            self.grid.attach_next_to(item, item.label, Gtk.PositionType.RIGHT, 1, 1)
+        if isinstance(self.widget, Gtk.DropDown):
+            self.__update_dropdown()
+        elif isinstance(self.widget, Gtk.Switch):
+            self.__update_switch()
         else:
-            self.grid.attach(item, *grid_position, 1, 1)
+            self.__update_entry()
 
+    def set_visible(self, state: bool) -> None:
+        self.label.set_visible(state)
+        super(self.__class__, self).set_visible(state)
+
+    def connect(self, name: str, callback: Callable[..., Any], *args, **kwargs) -> None:
+        self.widget.connect(name, lambda widget, *data: callback(self, *data, *args, **kwargs))
+
+
+class Section(Gtk.Grid):
+    def __init__(self, name: str) -> None:
+        super().__init__()
+        self.items = []
+
+        self.set_name(name)
+        self.set_row_spacing(10)
+        self.set_margin_top(10)
+        self.set_margin_bottom(10)
+        self.set_margin_start(10)
+        self.set_margin_end(10)
+
+    def new_item(
+            self,
+            name: str,
+            label: Optional[str],
+            widget: Type[Gtk.Widget],
+            *grid_position: int,
+            items: Optional[OrderedDict[str, str]] = None,
+    ) -> Gtk.Widget:
+        item = _SectionItem(self, name, label, widget, items=items)
+        self.attach(item, *grid_position, 1, 1)
         self.items.append(item)
 
         if not name.startswith('_'):
             item.update_values()
 
         return item
 
@@ -815,41 +825,28 @@
     if exception and not isinstance(exception, asyncio.CancelledError):
         stack = task.get_stack()
         application = Gtk.Application.get_default()
 
         fatal_error_dialog(exception, stack, application.get_active_window())
 
 
-def on_setting_state_set(switch: Gtk.Switch, state: bool) -> None:
-    section = switch.get_section_name()
-    option = switch.get_name()
+def on_setting_state_set(item: _SectionItem, state: bool) -> None:
+    config.new(item.section.get_name(), item.get_name(), state)
 
-    config.new(section, option, state)
 
+def on_setting_changed(item: _SectionItem) -> None:
+    current_value = item.get_text()
+    config.new(item.section.get_name(), item.get_name(), current_value)
 
-def on_setting_changed(entry: Gtk.Entry) -> None:
-    current_value = entry.get_text()
-    section = entry.get_section_name()
-    option = entry.get_name()
 
-    config.new(section, option, current_value)
-
-
-def on_digit_only_setting_changed(entry: Gtk.Entry) -> None:
-    current_value = entry.get_text()
-    section = entry.get_section_name()
-    option = entry.get_name()
+def on_digit_only_setting_changed(item: _SectionItem) -> None:
+    current_value = item.get_text()
 
     if current_value.isdigit():
-        config.new(section, option, int(current_value))
+        config.new(item.section.get_name(), item.get_name(), int(current_value))
     else:
-        entry.handler_block_by_func(on_digit_only_setting_changed)
-        entry.set_text(remove_letters(current_value))
-        entry.handler_unblock_by_func(on_digit_only_setting_changed)
-
+        item.get_buffer().set_text(remove_letters(current_value), -1)
 
-def on_dropdown_setting_changed(dropdown: 'Item', _spec: Any, items: OrderedDict[str, str]) -> None:
-    current_value = list(items)[dropdown.get_selected()]
-    section = dropdown.get_section_name()
-    option = dropdown.get_name()
 
-    config.new(section, option, current_value)
+def on_dropdown_setting_changed(item: _SectionItem, _spec: Any, items: OrderedDict[str, str]) -> None:
+    current_value = list(items)[item.get_selected()]
+    config.new(item.section.get_name(), item.get_name(), current_value)
```

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/gtk/window.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/gtk/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,45 +131,41 @@
 
         # grid managed by plugin switch
         self.steamguard_status = utils.Status(4)
         self.cardfarming_status = utils.Status(6)
         self.steamgifts_status = utils.Status(5)
         self.steamtrades_status = utils.Status(5)
 
-        steamguard_section.grid.attach(self.steamguard_status, 0, 0, 2, 1)
+        steamguard_section.attach(self.steamguard_status, 0, 0, 2, 1)
 
         steamguard_stack = Gtk.Stack()
         steamguard_stack.set_vexpand(True)
-        steamguard_section.grid.attach(steamguard_stack, 1, 1, 1, 1)
+        steamguard_section.attach(steamguard_stack, 1, 1, 1, 1)
 
         steamguard_sidebar = Gtk.StackSidebar()
         steamguard_sidebar.set_stack(steamguard_stack)
         steamguard_sidebar.set_size_request(150, -1)
-        steamguard_section.grid.attach(steamguard_sidebar, 0, 1, 1, 1)
+        steamguard_section.attach(steamguard_sidebar, 0, 1, 1, 1)
 
         self.confirmations_grid = Gtk.Grid()
         self.confirmations_grid.set_row_spacing(10)
         steamguard_stack.add_titled(self.confirmations_grid, "confirmations", _("Confirmations"))
 
         confirmation_tree_headers = 'id', 'creatorid', 'nonce', '_give', '_to', '_receive', 'summary',
         self.confirmations_tree = utils.SimpleTextTree(*confirmation_tree_headers)
         self.confirmations_grid.attach(self.confirmations_tree, 0, 0, 4, 1)
 
         for index, column in enumerate(self.confirmations_tree.view.get_columns()):
-            column.set_resizable(True)
+            if index != 0:
+                column.set_resizable(True)
+                column.set_expand(True)
 
             if index in (1, 2, 3, 7):
                 column.set_visible(False)
 
-            if index in (4, 6):
-                column.set_fixed_width(190)
-
-            if index == 5:
-                column.set_fixed_width(100)
-
         self.confirmations_tree.model.connect("selection-changed", self.on_tree_selection_changed)
 
         accept_button = Gtk.Button()
         accept_button.set_margin_start(3)
         accept_button.set_margin_end(3)
         accept_button.set_label(_('Accept'))
         accept_button.connect('clicked', self.on_validate_confirmations, "allow")
@@ -194,20 +190,19 @@
         cancel_all_button.set_margin_end(3)
         cancel_all_button.set_label(_('Cancel All'))
         cancel_all_button.connect('clicked', self.on_validate_confirmations, "cancel", True)
         self.confirmations_grid.attach(cancel_all_button, 3, 1, 1, 1)
 
         steamguard_settings = utils.Section("steamguard")
         steamguard_settings.stackup_section(_("Settings"), steamguard_stack)
-        steamguard_settings.grid.set_halign(Gtk.Align.CENTER)
+        steamguard_settings.set_halign(Gtk.Align.CENTER)
 
         self.steamguard_enable = steamguard_settings.new_item("enable", _("Enable:"), Gtk.Switch, 0, 0)
-        self.steamguard_enable.set_margin_top(40)
+        self.steamguard_enable.widget.set_margin_top(40)
         self.steamguard_enable.label.set_margin_top(40)
-        self.steamguard_enable.set_halign(Gtk.Align.END)
         self.steamguard_enable.connect("state-set", utils.on_setting_state_set)
 
         self.steamguard_disabled = Gtk.Label()
         self.steamguard_disabled.set_justify(Gtk.Justification.CENTER)
         self.steamguard_disabled.set_halign(Gtk.Align.CENTER)
 
         _message = _(
@@ -215,23 +210,21 @@
             "logged in but no shared secret is found. To enable it again,\n"
             "go to Advanced and add a valid shared secret\n"
             "or use STNG as your Steam Authenticator\n"
         )
 
         self.steamguard_disabled.set_markup(utils.markup(_message, color="hotpink", background="black"))
         self.steamguard_disabled.set_visible(False)
-        steamguard_section.grid.attach(self.steamguard_disabled, 0, 0, 2, 1)
+        steamguard_section.attach(self.steamguard_disabled, 0, 0, 2, 1)
 
         self.confirmations_enable = steamguard_settings.new_item(
             "enable_confirmations", _("Enable Confirmations:"),
             Gtk.Switch,
             0, 1,
         )
-
-        self.confirmations_enable.set_halign(Gtk.Align.END)
         self.confirmations_enable.connect("state-set", utils.on_setting_state_set)
 
         self.confirmations_disabled = Gtk.Label()
         self.confirmations_disabled.set_justify(Gtk.Justification.CENTER)
         self.confirmations_disabled.set_halign(Gtk.Align.CENTER)
 
         _message = _(
@@ -246,43 +239,43 @@
         self.confirmations_grid.attach(self.confirmations_disabled, 0, 0, 4, 1)
 
         login_button = Gtk.Button()
         login_button.set_margin_top(40)
         login_button.set_label(_("Login with another account"))
         login_button.set_name("login_button")
         login_button.connect('clicked', self.on_login_button_clicked)
-        steamguard_settings.grid.attach(login_button, 0, 2, 2, 1)
+        steamguard_settings.attach(login_button, 0, 2, 2, 1)
 
         new_authenticator_button = Gtk.Button()
         new_authenticator_button.set_label(_("Add STNG as your Steam Authenticator"))
         new_authenticator_button.set_name("new_authenticator_button")
         new_authenticator_button.connect("clicked", self.on_new_authenticator_clicked)
-        steamguard_settings.grid.attach(new_authenticator_button, 0, 3, 2, 1)
+        steamguard_settings.attach(new_authenticator_button, 0, 3, 2, 1)
 
         remove_authenticator_button = Gtk.Button()
         remove_authenticator_button.set_label(_("Remove STNG Authenticator from your Steam Account"))
         remove_authenticator_button.set_name("remove_authenticator_button")
         remove_authenticator_button.connect("clicked", self.on_remove_authenticator_clicked)
-        steamguard_settings.grid.attach(remove_authenticator_button, 0, 4, 2, 1)
+        steamguard_settings.attach(remove_authenticator_button, 0, 4, 2, 1)
 
         reset_password_button = Gtk.Button()
         reset_password_button.set_label(_("Remove Saved Password"))
         reset_password_button.set_name("reset_password_button")
         reset_password_button.connect("clicked", self.on_reset_password_clicked)
-        steamguard_settings.grid.attach(reset_password_button, 0, 5, 2, 1)
+        steamguard_settings.attach(reset_password_button, 0, 5, 2, 1)
 
         steamguard_advanced = utils.Section("login")
         steamguard_advanced.stackup_section(_("Advanced"), steamguard_stack, scroll=True)
 
         warning_label = Gtk.Label()
         warning_label.set_markup(utils.markup(
             _("Warning: Don't mess up these settings unless you know what you are doing!"),
             color='darkred' if self.theme == 'light' else 'red',
         ))
-        steamguard_advanced.grid.attach(warning_label, 0, 0, 2, 1)
+        steamguard_advanced.attach(warning_label, 0, 0, 2, 1)
 
         shared_secret = steamguard_advanced.new_item('shared_secret', _("Shared Secret:"), Gtk.Entry, 0, 1)
         shared_secret.connect('changed', utils.on_setting_changed)
 
         access_token_item = steamguard_advanced.new_item("access_token", _("Access Token:"), Gtk.Entry, 0, 2)
         access_token_item.connect("changed", utils.on_setting_changed)
 
@@ -302,32 +295,31 @@
         account_name = steamguard_advanced.new_item('account_name', _("Username:"), Gtk.Entry, 0, 7)
         account_name.connect('changed', utils.on_setting_changed)
 
         reset_button = Gtk.Button()
         reset_button.set_label(_("Reset Everything (USE WITH CAUTION!!!)"))
         reset_button.set_name("reset_button")
         reset_button.connect("clicked", self.on_reset_clicked)
-        steamguard_advanced.grid.attach(reset_button, 0, 8, 2, 1)
+        steamguard_advanced.attach(reset_button, 0, 8, 2, 1)
 
-        cardfarming_section.grid.attach(self.cardfarming_status, 0, 0, 2, 1)
+        cardfarming_section.attach(self.cardfarming_status, 0, 0, 2, 1)
 
         cardfarming_stack = Gtk.Stack()
         cardfarming_stack.set_vexpand(True)
-        cardfarming_section.grid.attach(cardfarming_stack, 1, 1, 1, 1)
+        cardfarming_section.attach(cardfarming_stack, 1, 1, 1, 1)
 
         cardfarming_sidebar = Gtk.StackSidebar()
         cardfarming_sidebar.set_stack(cardfarming_stack)
         cardfarming_sidebar.set_size_request(150, -1)
-        cardfarming_section.grid.attach(cardfarming_sidebar, 0, 1, 1, 1)
+        cardfarming_section.attach(cardfarming_sidebar, 0, 1, 1, 1)
 
         cardfarming_settings = utils.Section("cardfarming")
         cardfarming_settings.stackup_section(_("Settings"), cardfarming_stack, scroll=True)
 
         cardfarming_enable = cardfarming_settings.new_item("enable", _("Enable:"), Gtk.Switch, 0, 1)
-        cardfarming_enable.set_halign(Gtk.Align.END)
         cardfarming_enable.connect("state-set", utils.on_setting_state_set)
 
         mandatory_waiting = cardfarming_settings.new_item("mandatory_waiting", _("Mandatory waiting:"), Gtk.Entry, 0, 2)
         mandatory_waiting.connect("changed", utils.on_digit_only_setting_changed)
 
         wait_while_running = cardfarming_settings.new_item(
             "wait_while_running",
@@ -340,19 +332,17 @@
         wait_for_drops = cardfarming_settings.new_item("wait_for_drops", _("Wait for drops:"), Gtk.Entry, 0, 4)
         wait_for_drops.connect("changed", utils.on_digit_only_setting_changed)
 
         max_concurrency = cardfarming_settings.new_item("max_concurrency", _("Max concurrency:"), Gtk.Entry, 0, 5)
         max_concurrency.connect("changed", utils.on_digit_only_setting_changed)
 
         cardfarming_invisible = cardfarming_settings.new_item("invisible", _("Invisible:"), Gtk.Switch, 0, 6)
-        cardfarming_invisible.set_halign(Gtk.Align.END)
         cardfarming_invisible.connect("state-set", utils.on_setting_state_set)
 
         reverse_sorting = cardfarming_settings.new_item("reverse_sorting", _("Reverse Sorting:"), Gtk.Switch, 0, 7)
-        reverse_sorting.set_halign(Gtk.Align.END)
         reverse_sorting.connect("state-set", utils.on_setting_state_set)
 
         if not stlib.steamworks_available:
             cardfarming_settings.set_sensitive(False)
             cardfarming_enable.set_active(False)
             _cardfarming_disabled = Gtk.Label()
             _cardfarming_disabled.set_justify(Gtk.Justification.CENTER)
@@ -363,38 +353,36 @@
                 "a stlib built without SteamWorks support. To enable it again,\n"
                 "reinstall stlib with SteamWorks support\n"
             )
 
             _cardfarming_disabled.set_markup(utils.markup(_message, color="hotpink", background="black"))
             cardfarming_section.attach(_cardfarming_disabled, 0, 0, 2, 1)
 
-        steamgifts_section.grid.attach(self.steamgifts_status, 0, 0, 2, 1)
+        steamgifts_section.attach(self.steamgifts_status, 0, 0, 2, 1)
 
         steamgifts_stack = Gtk.Stack()
         steamgifts_stack.set_vexpand(True)
-        steamgifts_section.grid.attach(steamgifts_stack, 1, 1, 1, 1)
+        steamgifts_section.attach(steamgifts_stack, 1, 1, 1, 1)
 
         steamgifts_sidebar = Gtk.StackSidebar()
         steamgifts_sidebar.set_stack(steamgifts_stack)
         steamgifts_sidebar.set_size_request(150, -1)
-        steamgifts_section.grid.attach(steamgifts_sidebar, 0, 1, 1, 1)
+        steamgifts_section.attach(steamgifts_sidebar, 0, 1, 1, 1)
 
         steamgifts_settings = utils.Section("steamgifts")
         steamgifts_settings.stackup_section(_("Settings"), steamgifts_stack)
 
         steamgifts_enable = steamgifts_settings.new_item("enable", _("Enable:"), Gtk.Switch, 0, 0)
-        steamgifts_enable.set_halign(Gtk.Align.END)
         steamgifts_enable.connect('state-set', utils.on_setting_state_set)
 
         developer_giveaways = steamgifts_settings.new_item(
             "developer_giveaways", _("Developer Giveaways"),
             Gtk.Switch,
             0, 1,
         )
-        developer_giveaways.set_halign(Gtk.Align.END)
         developer_giveaways.connect("state-set", utils.on_setting_state_set)
 
         steamgifts_mode = steamgifts_settings.new_item(
             "mode", _("Mode:"),
             Gtk.DropDown,
             0, 2,
             items=config.steamgifts_modes,
@@ -420,32 +408,31 @@
 
         for index in range(1, 6):
             strategy_section = utils.Section(f"steamgifts_strategy{index}")
             strategy_section.stackup_section(_("Strategy {}").format(index), steamgifts_stack, scroll=True)
 
             label = Gtk.Label()
             label.set_text(_("Strategy {}").format(index))
-            strategy_section.grid.attach(label, 0, 0, 1, 1)
+            strategy_section.attach(label, 0, 0, 1, 1)
 
             enable = strategy_section.new_item("enable", None, Gtk.Switch, 2, 0)
-            enable.set_halign(Gtk.Align.END)
             enable.connect("state-set", utils.on_setting_state_set)
 
             minimum_label = Gtk.Label()
             minimum_label.set_text(_("Minimum"))
-            strategy_section.grid.attach(minimum_label, 1, 1, 1, 1)
+            strategy_section.attach(minimum_label, 1, 1, 1, 1)
 
             maximum_label = Gtk.Label()
             maximum_label.set_text(_("Maximum"))
-            strategy_section.grid.attach(maximum_label, 2, 1, 1, 1)
+            strategy_section.attach(maximum_label, 2, 1, 1, 1)
 
             for tree_level, item in enumerate(["points", "level", "copies", "metascore", "entries"]):
                 label = Gtk.Label()
                 label.set_text(_(item))
-                strategy_section.grid.attach(label, 0, tree_level + 2, 1, 1)
+                strategy_section.attach(label, 0, tree_level + 2, 1, 1)
 
                 minimum = strategy_section.new_item(f"minimum_{item}", None, Gtk.Entry, 1, tree_level + 2)
                 minimum.connect("changed", utils.on_digit_only_setting_changed)
 
                 maximum = strategy_section.new_item(f"maximum_{item}", None, Gtk.Entry, 2, tree_level + 2)
                 maximum.connect("changed", utils.on_digit_only_setting_changed)
 
@@ -479,34 +466,33 @@
             _message = _(
                 "steamgifts module has been disabled because you don't\n"
                 "have steamgifts plugin installed. To enable it again,\n"
                 "install the steamgifts plugin.\n"
             )
 
             _steamgifts_disabled.set_markup(utils.markup(_message, color="hotpink", background="black"))
-            steamgifts_section.grid.attach(_steamgifts_disabled, 0, 0, 2, 2)
+            steamgifts_section.attach(_steamgifts_disabled, 0, 0, 2, 2)
 
-        steamtrades_section.grid.attach(self.steamtrades_status, 0, 0, 2, 1)
+        steamtrades_section.attach(self.steamtrades_status, 0, 0, 2, 1)
 
         steamtrades_stack = Gtk.Stack()
         steamtrades_stack.set_vexpand(True)
-        steamtrades_section.grid.attach(steamtrades_stack, 1, 1, 1, 1)
+        steamtrades_section.attach(steamtrades_stack, 1, 1, 1, 1)
 
         steamtrades_sidebar = Gtk.StackSidebar()
         steamtrades_sidebar.set_stack(steamtrades_stack)
         steamtrades_sidebar.set_size_request(150, -1)
-        steamtrades_section.grid.attach(steamtrades_sidebar, 0, 1, 1, 1)
+        steamtrades_section.attach(steamtrades_sidebar, 0, 1, 1, 1)
 
         steamtrades_settings = utils.Section("steamtrades")
         steamtrades_settings.stackup_section(_("Settings"), steamtrades_stack)
 
         steamtrades_enable = steamtrades_settings.new_item("enable", _("Enable:"), Gtk.Switch, 0, 1)
         steamtrades_enable.label.set_margin_top(40)
-        steamtrades_enable.set_margin_top(40)
-        steamtrades_enable.set_halign(Gtk.Align.END)
+        steamtrades_enable.widget.set_margin_top(40)
         steamtrades_enable.connect("state-set", utils.on_setting_state_set)
 
         trade_ids = steamtrades_settings.new_item("trade_ids", _("Trade IDs:"), Gtk.Entry, 0, 2)
         trade_ids.set_placeholder_text('12345, asdfg, ...')
         trade_ids.connect("changed", utils.on_setting_changed)
 
         wait_for_bump = steamtrades_settings.new_item("wait_for_bump", _("Wait for Bump:"), Gtk.Entry, 0, 3)
@@ -522,33 +508,33 @@
             _message = _(
                 "steamtrades module has been disabled because you don't\n"
                 "have steamtrades plugin installed. To enable it again,\n"
                 "install the steamtrades plugin.\n"
             )
 
             _steamtrades_disabled.set_markup(utils.markup(_message, color="hotpink", background="black"))
-            steamtrades_settings.grid.attach(_steamtrades_disabled, 0, 1, 2, 2)
+            steamtrades_settings.attach(_steamtrades_disabled, 0, 1, 2, 2)
 
         self.coupon_warning = Gtk.Label()
         self.coupon_warning.set_markup(utils.markup(
             _("Warning: It's a heavy uncached operation. Fetch only once a day or you will be blocked."),
             color='darkred' if self.theme == 'light' else 'red',
         ))
         self.coupon_warning.set_margin_top(37)
         self.coupon_warning.set_margin_bottom(37)
-        coupons_section.grid.attach(self.coupon_warning, 0, 0, 2, 1)
+        coupons_section.attach(self.coupon_warning, 0, 0, 2, 1)
 
         coupons_stack = Gtk.Stack()
         coupons_stack.set_vexpand(True)
-        coupons_section.grid.attach(coupons_stack, 1, 1, 1, 1)
+        coupons_section.attach(coupons_stack, 1, 1, 1, 1)
 
         coupons_sidebar = Gtk.StackSidebar()
         coupons_sidebar.set_stack(coupons_stack)
         coupons_sidebar.set_size_request(150, -1)
-        coupons_section.grid.attach(coupons_sidebar, 0, 1, 1, 1)
+        coupons_section.attach(coupons_sidebar, 0, 1, 1, 1)
 
         self.coupons_grid = Gtk.Grid()
         self.coupons_grid.set_row_spacing(10)
         coupons_stack.add_titled(self.coupons_grid, "coupons_list", _("Coupon List"))
 
         coupons_tree_headers = '_price', '_name', 'link', 'botid', 'token', 'assetid'
         self.coupons_tree = utils.SimpleTextTree(*coupons_tree_headers)
@@ -559,25 +545,21 @@
         price_column = self.coupons_tree.view.get_columns()[1]
         price_column.set_sorter(price_sorter)
 
         self.coupons_tree.view.sort_by_column(price_column, Gtk.SortType.ASCENDING)
         self.coupons_grid.attach(self.coupons_tree, 0, 0, 4, 2)
 
         for index, column in enumerate(self.coupons_tree.view.get_columns()):
-            column.set_resizable(True)
+            if column != 0:
+                column.set_resizable(True)
+                column.set_expand(True)
 
             if index in (0, 3, 4, 5, 6):
                 column.set_visible(False)
 
-            if index == 1:
-                column.set_fixed_width(80)
-
-            if index == 2:
-                column.set_fixed_width(400)
-
         self.coupons_tree.view.connect("activate", self.on_coupon_double_clicked)
         self.coupons_tree.model.connect("selection-changed", self.on_tree_selection_changed)
 
         self.coupon_progress = Gtk.LevelBar()
         self.coupons_grid.attach(self.coupon_progress, 0, 3, 4, 1)
 
         fetch_coupons_button = Gtk.Button()
@@ -781,23 +763,36 @@
     @staticmethod
     def on_tree_selection_changed(view: Gtk.SingleSelection, position, item_count: int) -> None:
         item = view.get_selected_item()
         if parent := item.get_parent():
             view.set_selected(parent.get_position())
 
     @staticmethod
-    def on_stack_child_changed(stack: Gtk.Stack, *args) -> None:
-        section = stack.get_visible_child()
+    def on_stack_child_changed(tabs: Gtk.Stack, *args) -> None:
+        main_section = tabs.get_visible_child()
+
+        if not (config_stack := main_section.get_child_at(1, 1)):
+            log.debug("Not reading config values cause GUI didn't finish loading")
+            return
+
+        for config_section in config_stack.observe_children():
+            if isinstance(config_section, Gtk.ScrolledWindow):
+                # ScrolledWindow > ViewPort > Section
+                config_section = config_section.get_child().get_child()
 
-        for item in section.items:
-            if item.get_name().startswith('_'):
+            if not isinstance(config_section, utils.Section):
+                log.debug(f"Not reading config for {config_section} cause there's no config section")
                 continue
 
-            log.debug(f'Reading {section.get_name()}:{item.get_name()} from config file')
-            item.update_values()
+            for item in config_section.items:
+                if item.get_name().startswith('_'):
+                    continue
+
+                log.debug(f'Reading {item.section.get_name()}:{item.get_name()} from config file')
+                item.update_values()
 
     @staticmethod
     def coupon_sorting(item1: utils.SimpleTextTreeItem, item2: utils.SimpleTextTreeItem, *data: Any) -> Any:
         if float(item1.price) < float(item2.price):
             return -1
 
         return 0 if item1.price == item2.price else 1
```

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/gui.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/gui.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/i18n.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/i18n.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/icons/stng.ico` & `steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng.ico`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/icons/stng.png` & `steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng.png`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_console.ico` & `steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_console.ico`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_console.png` & `steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_console.png`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_nc.ico` & `steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_nc.ico`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/icons/stng_nc.png` & `steam-tools-ng-3.1.1/src/steam_tools_ng/icons/stng_nc.png`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng/logger_handlers.py` & `steam-tools-ng-3.1.1/src/steam_tools_ng/logger_handlers.py`

 * *Files identical despite different names*

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng.egg-info/PKG-INFO` & `steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steam-tools-ng
-Version: 3.1
+Version: 3.1.1
 Summary: Steam Tools NG
 Author: Lara Maia
 Author-email: dev@lara.monster
 License: GPLv3
 Project-URL: homepage, https://github.com/calendulish/steam-tools-ng
 Project-URL: repository, https://github.com
 Project-URL: changelog, https://github.com/calendulish/steam-tools-ng/releases
@@ -26,18 +26,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [STNG] Steam Tools NG (formerly Steam Tools)
 ========================================
 [![STNG](https://lara.monster/archive/stng_last.png)](https://github.com/calendulish/steam-tools-ng)  
   
-[![transifex](https://img.shields.io/badge/transifex-contribute%20now-blue.svg?style=flat)](https://www.transifex.com/shypixie/steam-tools-ng)
+[![transifex](https://img.shields.io/badge/transifex-contribute%20now-blue.svg?style=flat)](https://www.transifex.com/calendulish/steam-tools-ng)
 [![windows build status](https://badges.lara.monster/calendulish/.github/steam-tools-ng-windows-build)](https://github.com/calendulish/steam-tools-ng/actions/workflows/build.yml)
 [![linux build status](https://badges.lara.monster/calendulish/.github/steam-tools-ng-linux-build)](https://github.com/calendulish/steam-tools-ng/actions/workflows/build.yml)
-[![Quality](https://api.codiga.io/project/33951/score/svg)](https://app.codiga.io/project/33951/dashboard)
 [![GitHub license](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](https://www.gnu.org/licenses/gpl-3.0.html)
 [![GitHub release](https://img.shields.io/github/release/calendulish/steam-tools-ng.svg?style=flat)](https://github.com/calendulish/steam-tools-ng/releases)
 
 Some useful tools to use with steam client or compatible programs and websites.
 
 You can run the follow modules from steam-tools:
```

### Comparing `steam-tools-ng-3.1/src/steam_tools_ng.egg-info/SOURCES.txt` & `steam-tools-ng-3.1.1/src/steam_tools_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

