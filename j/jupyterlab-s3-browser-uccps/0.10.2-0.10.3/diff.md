# Comparing `tmp/jupyterlab_s3_browser_uccps-0.10.2.tar.gz` & `tmp/jupyterlab_s3_browser_uccps-0.10.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jupyterlab_s3_browser_uccps-0.10.2.tar", last modified: Thu Jul 27 05:47:02 2023, max compression
+gzip compressed data, was "dist/jupyterlab_s3_browser_uccps-0.10.3.tar", last modified: Thu Jul 27 06:23:29 2023, max compression
```

## Comparing `jupyterlab_s3_browser_uccps-0.10.2.tar` & `jupyterlab_s3_browser_uccps-0.10.3.tar`

### file list

```diff
@@ -1,63 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyter-config/
--rwxr-xr-x   0 root         (0) root         (0)       96 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyter-config/jupyterlab_s3_browser.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/labextension/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/labextension/static/
--rw-r--r--   0 root         (0) root         (0)     6842 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/labextension/static/268.f31edca7f28c6bfffe28.js
--rw-r--r--   0 root         (0) root         (0)    10952 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/labextension/static/534.9645931ef1a95d5a9df1.js
--rw-r--r--   0 root         (0) root         (0)     1499 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/labextension/static/742.e2d83637b4dbb625a240.js
--rw-r--r--   0 root         (0) root         (0)     7245 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/labextension/static/remoteEntry.aa6024c5ea40b82c48e7.js
--rw-r--r--   0 root         (0) root         (0)      164 2023-07-27 05:47:01.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/labextension/static/style.js
--rwxr-xr-x   0 root         (0) root         (0)     3753 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/labextension/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 05:34:11.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-07-27 05:34:11.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/tests/test_auth.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-07-27 05:34:11.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/tests/test_get_s3.py
--rwxr-xr-x   0 root         (0) root         (0)     2026 2023-07-27 05:38:35.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      523 2023-07-27 05:34:11.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/_version.py
--rw-r--r--   0 root         (0) root         (0)    12123 2023-07-27 05:40:25.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/labextension/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/labextension/static/
--rw-r--r--   0 root         (0) root         (0)     6842 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/labextension/static/268.f31edca7f28c6bfffe28.js
--rw-r--r--   0 root         (0) root         (0)    10952 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/labextension/static/534.9645931ef1a95d5a9df1.js
--rw-r--r--   0 root         (0) root         (0)     1499 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/labextension/static/742.e2d83637b4dbb625a240.js
--rw-r--r--   0 root         (0) root         (0)     7245 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/labextension/static/remoteEntry.aa6024c5ea40b82c48e7.js
--rw-r--r--   0 root         (0) root         (0)      164 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/labextension/static/style.js
--rwxr-xr-x   0 root         (0) root         (0)     3753 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/labextension/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/tests/test_auth.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/tests/test_get_s3.py
--rwxr-xr-x   0 root         (0) root         (0)     2026 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/__init__.py
--rw-r--r--   0 root         (0) root         (0)      523 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/_version.py
--rw-r--r--   0 root         (0) root         (0)    12083 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps.egg-info/
--rw-r--r--   0 root         (0) root         (0)      736 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1882 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 04:48:27.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      121 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/src/
--rwxr-xr-x   0 root         (0) root         (0)     5344 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.2/src/browser.ts
--rwxr-xr-x   0 root         (0) root         (0)    12368 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.2/src/contents.ts
--rwxr-xr-x   0 root         (0) root         (0)     1767 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.2/src/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/style/
--rw-r--r--   0 root         (0) root         (0)     2146 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.2/style/base.css
--rw-r--r--   0 root         (0) root         (0)     2456 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.2/style/bucket-dark.svg
--rw-r--r--   0 root         (0) root         (0)     2401 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.2/style/bucket-light.svg
--rwxr-xr-x   0 root         (0) root         (0)       25 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.2/style/index.css
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.2/style/index.js
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.2/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)      457 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.2/MANIFEST.in
--rwxr-xr-x   0 root         (0) root         (0)     1976 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.2/README.md
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.2/install.json
--rwxr-xr-x   0 root         (0) root         (0)     3611 2023-07-27 04:44:02.000000 jupyterlab_s3_browser_uccps-0.10.2/package.json
--rw-r--r--   0 root         (0) root         (0)      145 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.2/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)     2681 2023-07-27 05:46:48.000000 jupyterlab_s3_browser_uccps-0.10.2/setup.py
--rwxr-xr-x   0 root         (0) root         (0)      556 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.2/tsconfig.json
--rw-r--r--   0 root         (0) root         (0)   226989 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.2/yarn.lock
--rw-r--r--   0 root         (0) root         (0)      736 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 05:47:02.000000 jupyterlab_s3_browser_uccps-0.10.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyter-config/
+-rwxr-xr-x   0 root         (0) root         (0)       96 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyter-config/jupyterlab_s3_browser.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/
+-rw-r--r--   0 root         (0) root         (0)     6842 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/268.f31edca7f28c6bfffe28.js
+-rw-r--r--   0 root         (0) root         (0)    10952 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/534.9645931ef1a95d5a9df1.js
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/742.e2d83637b4dbb625a240.js
+-rw-r--r--   0 root         (0) root         (0)     7245 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/remoteEntry.aa6024c5ea40b82c48e7.js
+-rw-r--r--   0 root         (0) root         (0)      164 2023-07-27 06:23:28.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/style.js
+-rwxr-xr-x   0 root         (0) root         (0)     3753 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 05:34:11.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-27 05:34:11.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/tests/test_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-07-27 05:34:11.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/tests/test_get_s3.py
+-rwxr-xr-x   0 root         (0) root         (0)     2026 2023-07-27 05:38:35.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      523 2023-07-27 05:34:11.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/_version.py
+-rw-r--r--   0 root         (0) root         (0)    12122 2023-07-27 06:22:45.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/labextension/
+-rwxr-xr-x   0 root         (0) root         (0)     3753 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/labextension/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/tests/test_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/tests/test_get_s3.py
+-rwxr-xr-x   0 root         (0) root         (0)     2026 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      523 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/_version.py
+-rw-r--r--   0 root         (0) root         (0)    12082 2023-07-27 06:22:55.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      736 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 04:48:27.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/src/
+-rwxr-xr-x   0 root         (0) root         (0)     5344 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/src/browser.ts
+-rwxr-xr-x   0 root         (0) root         (0)    12368 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/src/contents.ts
+-rwxr-xr-x   0 root         (0) root         (0)     1767 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/src/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/style/
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/style/base.css
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.3/style/bucket-dark.svg
+-rw-r--r--   0 root         (0) root         (0)     2401 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.3/style/bucket-light.svg
+-rwxr-xr-x   0 root         (0) root         (0)       25 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/style/index.css
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/style/index.js
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.3/LICENSE
+-rwxr-xr-x   0 root         (0) root         (0)      457 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.3/MANIFEST.in
+-rwxr-xr-x   0 root         (0) root         (0)     1976 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.3/install.json
+-rwxr-xr-x   0 root         (0) root         (0)     3611 2023-07-27 04:44:02.000000 jupyterlab_s3_browser_uccps-0.10.3/package.json
+-rw-r--r--   0 root         (0) root         (0)      145 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)     2681 2023-07-27 06:23:12.000000 jupyterlab_s3_browser_uccps-0.10.3/setup.py
+-rwxr-xr-x   0 root         (0) root         (0)      556 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.3/tsconfig.json
+-rw-r--r--   0 root         (0) root         (0)   226989 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/yarn.lock
+-rw-r--r--   0 root         (0) root         (0)      736 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/setup.cfg
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/labextension/static/268.f31edca7f28c6bfffe28.js` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/268.f31edca7f28c6bfffe28.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/labextension/static/534.9645931ef1a95d5a9df1.js` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/534.9645931ef1a95d5a9df1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/labextension/static/742.e2d83637b4dbb625a240.js` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/742.e2d83637b4dbb625a240.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/labextension/static/remoteEntry.aa6024c5ea40b82c48e7.js` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/remoteEntry.aa6024c5ea40b82c48e7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/labextension/package.json` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/tests/test_get_s3.py` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/tests/test_get_s3.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/__init__.py` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/_version.py` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser/handlers.py` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         return boto3.resource(
             "s3",
             aws_access_key_id=config.client_id,
             aws_secret_access_key=config.client_secret,
             endpoint_url=config.endpoint_url,
             aws_session_token=config.session_token,
-            use_ssl=config.use_ssl,
+            verify=config.use_ssl,
         )
     else:
         return boto3.resource("s3")
 
 
 def _test_aws_s3_role_access():
     """
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/labextension/package.json` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/labextension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/tests/test_get_s3.py` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/tests/test_get_s3.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/__init__.py` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/_version.py` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps/handlers.py` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         return boto3.resource(
             "s3",
             aws_access_key_id=config.client_id,
             aws_secret_access_key=config.client_secret,
             endpoint_url=config.endpoint_url,
             aws_session_token=config.session_token,
-            use_ssl=config.use_ssl,
+            verify=config.use_ssl,
         )
     else:
         return boto3.resource("s3")
 
 
 def _test_aws_s3_role_access():
     """
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps.egg-info/PKG-INFO` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-s3-browser-uccps
-Version: 0.10.2
+Version: 0.10.3
 Summary: JupyterLab extension for browsing S3-compatible object storage
 Home-page: https://github.com/IBM/jupyterlab_s3_browser
 Author: James Reeve
 License: Apache-2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,S3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/jupyterlab_s3_browser_uccps.egg-info/SOURCES.txt` & `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -26,19 +26,14 @@
 jupyterlab_s3_browser_uccps.egg-info/PKG-INFO
 jupyterlab_s3_browser_uccps.egg-info/SOURCES.txt
 jupyterlab_s3_browser_uccps.egg-info/dependency_links.txt
 jupyterlab_s3_browser_uccps.egg-info/not-zip-safe
 jupyterlab_s3_browser_uccps.egg-info/requires.txt
 jupyterlab_s3_browser_uccps.egg-info/top_level.txt
 jupyterlab_s3_browser_uccps/labextension/package.json
-jupyterlab_s3_browser_uccps/labextension/static/268.f31edca7f28c6bfffe28.js
-jupyterlab_s3_browser_uccps/labextension/static/534.9645931ef1a95d5a9df1.js
-jupyterlab_s3_browser_uccps/labextension/static/742.e2d83637b4dbb625a240.js
-jupyterlab_s3_browser_uccps/labextension/static/remoteEntry.aa6024c5ea40b82c48e7.js
-jupyterlab_s3_browser_uccps/labextension/static/style.js
 jupyterlab_s3_browser_uccps/tests/__init__.py
 jupyterlab_s3_browser_uccps/tests/test_auth.py
 jupyterlab_s3_browser_uccps/tests/test_get_s3.py
 src/browser.ts
 src/contents.ts
 src/index.ts
 style/base.css
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/src/browser.ts` & `jupyterlab_s3_browser_uccps-0.10.3/src/browser.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/src/contents.ts` & `jupyterlab_s3_browser_uccps-0.10.3/src/contents.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/src/index.ts` & `jupyterlab_s3_browser_uccps-0.10.3/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/style/base.css` & `jupyterlab_s3_browser_uccps-0.10.3/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/style/bucket-dark.svg` & `jupyterlab_s3_browser_uccps-0.10.3/style/bucket-dark.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/style/bucket-light.svg` & `jupyterlab_s3_browser_uccps-0.10.3/style/bucket-light.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/LICENSE` & `jupyterlab_s3_browser_uccps-0.10.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/README.md` & `jupyterlab_s3_browser_uccps-0.10.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/package.json` & `jupyterlab_s3_browser_uccps-0.10.3/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/setup.py` & `jupyterlab_s3_browser_uccps-0.10.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 else:
     cmdclass["jsdeps"] = skip_if_exists(jstargets, js_command)
 
 #  long_description = (HERE / "README.md").read_text()
 
 setup_args = dict(
     name=name,
-    version="0.10.2",
+    version="0.10.3",
     url=pkg_json["homepage"],
     author=pkg_json["author"],
     description=pkg_json["description"],
     license=pkg_json["license"],
     packages=setuptools.find_packages(),
     cmdclass=cmdclass,
     platforms="Linux, Mac OS X, Windows",
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/tsconfig.json` & `jupyterlab_s3_browser_uccps-0.10.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/yarn.lock` & `jupyterlab_s3_browser_uccps-0.10.3/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.2/PKG-INFO` & `jupyterlab_s3_browser_uccps-0.10.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_s3_browser_uccps
-Version: 0.10.2
+Version: 0.10.3
 Summary: JupyterLab extension for browsing S3-compatible object storage
 Home-page: https://github.com/IBM/jupyterlab_s3_browser
 Author: James Reeve
 License: Apache-2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,S3
 Platform: Linux
 Platform: Mac OS X
```

