# Comparing `tmp/jupyterlab_s3_browser_uccps-0.10.3.tar.gz` & `tmp/jupyterlab_s3_browser_uccps-0.10.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jupyterlab_s3_browser_uccps-0.10.3.tar", last modified: Thu Jul 27 06:23:29 2023, max compression
+gzip compressed data, was "dist/jupyterlab_s3_browser_uccps-0.10.4.tar", last modified: Thu Jul 27 07:58:51 2023, max compression
```

## Comparing `jupyterlab_s3_browser_uccps-0.10.3.tar` & `jupyterlab_s3_browser_uccps-0.10.4.tar`

### file list

```diff
@@ -1,57 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyter-config/
--rwxr-xr-x   0 root         (0) root         (0)       96 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyter-config/jupyterlab_s3_browser.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/
--rw-r--r--   0 root         (0) root         (0)     6842 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/268.f31edca7f28c6bfffe28.js
--rw-r--r--   0 root         (0) root         (0)    10952 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/534.9645931ef1a95d5a9df1.js
--rw-r--r--   0 root         (0) root         (0)     1499 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/742.e2d83637b4dbb625a240.js
--rw-r--r--   0 root         (0) root         (0)     7245 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/remoteEntry.aa6024c5ea40b82c48e7.js
--rw-r--r--   0 root         (0) root         (0)      164 2023-07-27 06:23:28.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/style.js
--rwxr-xr-x   0 root         (0) root         (0)     3753 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 05:34:11.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-07-27 05:34:11.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/tests/test_auth.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-07-27 05:34:11.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/tests/test_get_s3.py
--rwxr-xr-x   0 root         (0) root         (0)     2026 2023-07-27 05:38:35.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      523 2023-07-27 05:34:11.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/_version.py
--rw-r--r--   0 root         (0) root         (0)    12122 2023-07-27 06:22:45.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/labextension/
--rwxr-xr-x   0 root         (0) root         (0)     3753 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/labextension/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/tests/test_auth.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/tests/test_get_s3.py
--rwxr-xr-x   0 root         (0) root         (0)     2026 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/__init__.py
--rw-r--r--   0 root         (0) root         (0)      523 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/_version.py
--rw-r--r--   0 root         (0) root         (0)    12082 2023-07-27 06:22:55.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/
--rw-r--r--   0 root         (0) root         (0)      736 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1513 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 04:48:27.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      121 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/src/
--rwxr-xr-x   0 root         (0) root         (0)     5344 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/src/browser.ts
--rwxr-xr-x   0 root         (0) root         (0)    12368 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/src/contents.ts
--rwxr-xr-x   0 root         (0) root         (0)     1767 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/src/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/style/
--rw-r--r--   0 root         (0) root         (0)     2146 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/style/base.css
--rw-r--r--   0 root         (0) root         (0)     2456 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.3/style/bucket-dark.svg
--rw-r--r--   0 root         (0) root         (0)     2401 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.3/style/bucket-light.svg
--rwxr-xr-x   0 root         (0) root         (0)       25 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/style/index.css
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/style/index.js
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.3/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)      457 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.3/MANIFEST.in
--rwxr-xr-x   0 root         (0) root         (0)     1976 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.3/README.md
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.3/install.json
--rwxr-xr-x   0 root         (0) root         (0)     3611 2023-07-27 04:44:02.000000 jupyterlab_s3_browser_uccps-0.10.3/package.json
--rw-r--r--   0 root         (0) root         (0)      145 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)     2681 2023-07-27 06:23:12.000000 jupyterlab_s3_browser_uccps-0.10.3/setup.py
--rwxr-xr-x   0 root         (0) root         (0)      556 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.3/tsconfig.json
--rw-r--r--   0 root         (0) root         (0)   226989 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.3/yarn.lock
--rw-r--r--   0 root         (0) root         (0)      736 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 06:23:29.000000 jupyterlab_s3_browser_uccps-0.10.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyter-config/
+-rwxr-xr-x   0 root         (0) root         (0)      102 2023-07-27 07:57:17.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyter-config/jupyterlab_s3_browser.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/labextension/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/labextension/static/
+-rw-r--r--   0 root         (0) root         (0)     6866 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/labextension/static/268.9f7aa0158cdfda8baf56.js
+-rw-r--r--   0 root         (0) root         (0)    10952 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/labextension/static/534.9645931ef1a95d5a9df1.js
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/labextension/static/742.e2d83637b4dbb625a240.js
+-rw-r--r--   0 root         (0) root         (0)     7245 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/labextension/static/remoteEntry.a9b108e22db5ac7c4504.js
+-rw-r--r--   0 root         (0) root         (0)      164 2023-07-27 07:58:50.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/labextension/static/style.js
+-rwxr-xr-x   0 root         (0) root         (0)     3771 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/labextension/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/tests/test_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/tests/test_get_s3.py
+-rwxr-xr-x   0 root         (0) root         (0)     2026 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      523 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/_version.py
+-rw-r--r--   0 root         (0) root         (0)    12082 2023-07-27 06:22:55.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      736 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 04:48:27.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/src/
+-rwxr-xr-x   0 root         (0) root         (0)     5356 2023-07-27 07:57:02.000000 jupyterlab_s3_browser_uccps-0.10.4/src/browser.ts
+-rwxr-xr-x   0 root         (0) root         (0)    12374 2023-07-27 07:57:46.000000 jupyterlab_s3_browser_uccps-0.10.4/src/contents.ts
+-rwxr-xr-x   0 root         (0) root         (0)     1773 2023-07-27 07:57:35.000000 jupyterlab_s3_browser_uccps-0.10.4/src/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/style/
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.4/style/base.css
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.4/style/bucket-dark.svg
+-rw-r--r--   0 root         (0) root         (0)     2401 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.4/style/bucket-light.svg
+-rwxr-xr-x   0 root         (0) root         (0)       25 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.4/style/index.css
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.4/style/index.js
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.4/LICENSE
+-rwxr-xr-x   0 root         (0) root         (0)      457 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.4/MANIFEST.in
+-rwxr-xr-x   0 root         (0) root         (0)     1976 2023-07-27 05:34:06.000000 jupyterlab_s3_browser_uccps-0.10.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      215 2023-07-27 07:58:03.000000 jupyterlab_s3_browser_uccps-0.10.4/install.json
+-rwxr-xr-x   0 root         (0) root         (0)     3629 2023-07-27 07:56:23.000000 jupyterlab_s3_browser_uccps-0.10.4/package.json
+-rw-r--r--   0 root         (0) root         (0)      145 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.4/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)     2687 2023-07-27 07:58:41.000000 jupyterlab_s3_browser_uccps-0.10.4/setup.py
+-rwxr-xr-x   0 root         (0) root         (0)      556 2023-07-27 03:55:27.000000 jupyterlab_s3_browser_uccps-0.10.4/tsconfig.json
+-rw-r--r--   0 root         (0) root         (0)   226989 2023-07-27 03:55:43.000000 jupyterlab_s3_browser_uccps-0.10.4/yarn.lock
+-rw-r--r--   0 root         (0) root         (0)      736 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 07:58:51.000000 jupyterlab_s3_browser_uccps-0.10.4/setup.cfg
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/268.f31edca7f28c6bfffe28.js` & `jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/labextension/static/268.9f7aa0158cdfda8baf56.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -78,15 +78,15 @@
                         content: e.content
                     }
                 }
                 pathToJupyterContents(e) {
                     let t;
                     return e !== o.currentPath && "file" !== o.availableContentTypes[e] && (o.showingError && o.hideErrorMessage(), o.showDirectoryLoadingSpinner()), "file" !== o.availableContentTypes[e] ? (o.currentPath = e, t = this.jupyterPathToS3Path(e, !0)) : t = this.jupyterPathToS3Path(e, !1), new Promise(((r, n) => {
                         const s = d.ServerConnection.makeSettings();
-                        d.ServerConnection.makeRequest(l.URLExt.join(s.baseUrl, "jupyterlab_s3_browser/files", t), {}, s).then((t => {
+                        d.ServerConnection.makeRequest(l.URLExt.join(s.baseUrl, "jupyterlab_s3_browser_uccps/files", t), {}, s).then((t => {
                             t.json().then((t => {
                                 if (t.error) {
                                     const e = `Server returned status code ${t.error}. Error message: ${t.message}.`;
                                     return console.error(e), o.showErrorMessage(e), n(e), []
                                 }
                                 if (Array.isArray(t)) o.hideDirectoryLoadingSpinner(), t.forEach((e => {
                                     o.availableContentTypes[e.path] = e.type
@@ -173,15 +173,15 @@
                         const t = document.querySelector("#s3form"),
                             r = new FormData(t),
                             o = {};
                         r.forEach(((e, t) => {
                             o[t] = e
                         }));
                         const n = d.ServerConnection.makeSettings();
-                        d.ServerConnection.makeRequest(l.URLExt.join(n.baseUrl, "jupyterlab_s3_browser/auth"), {
+                        d.ServerConnection.makeRequest(l.URLExt.join(n.baseUrl, "jupyterlab_s3_browser_uccps/auth"), {
                             method: "POST",
                             body: JSON.stringify(o)
                         }, n).then((t => {
                             t.json().then((t => {
                                 if (t.success) this.layout.removeWidget(b), this.layout.addWidget(e), e.model.refresh();
                                 else {
                                     let e = t.message;
@@ -227,27 +227,27 @@
                     }, m.h.button({
                         onclick: e,
                         className: "jp-mod-accept jp-mod-styled"
                     }, "Connect"))))
                 }, e.checkIfAuthenicated = function() {
                     return new Promise(((e, t) => {
                         const r = d.ServerConnection.makeSettings();
-                        d.ServerConnection.makeRequest(l.URLExt.join(r.baseUrl, "jupyterlab_s3_browser/auth"), {
+                        d.ServerConnection.makeRequest(l.URLExt.join(r.baseUrl, "jupyterlab_s3_browser_uccps/auth"), {
                             method: "GET"
                         }, r).then((t => {
                             t.json().then((t => {
                                 e(t.authenticated)
                             }))
                         }))
                     }))
                 }
             }(g || (g = {}));
             const S = "s3-filebrowser",
                 w = {
-                    id: "jupyterlab_s3_browser:drive",
+                    id: "jupyterlab_s3_browser_uccps:drive",
                     requires: [i.IDocumentManager, a.IFileBrowserFactory, n.ILayoutRestorer, s.ISettingRegistry],
                     activate: function(e, t, r, o, n) {
                         const s = new u(e.docRegistry);
                         t.services.contents.addDrive(s);
                         const i = r.createFileBrowser(S, {
                                 driveName: s.name,
                                 state: null,
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/534.9645931ef1a95d5a9df1.js` & `jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/labextension/static/534.9645931ef1a95d5a9df1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/742.e2d83637b4dbb625a240.js` & `jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/labextension/static/742.e2d83637b4dbb625a240.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/static/remoteEntry.aa6024c5ea40b82c48e7.js` & `jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/labextension/static/remoteEntry.a9b108e22db5ac7c4504.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -42,19 +42,19 @@
         }), r
     }, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        268: "f31edca7f28c6bfffe28",
+        268: "9f7aa0158cdfda8baf56",
         534: "9645931ef1a95d5a9df1",
         742: "e2d83637b4dbb625a240"
     } [e] + ".js?v=" + {
-        268: "f31edca7f28c6bfffe28",
+        268: "9f7aa0158cdfda8baf56",
         534: "9645931ef1a95d5a9df1",
         742: "e2d83637b4dbb625a240"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/labextension/package.json` & `jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.995876736111111%*

 * *Differences: {"'jupyterlab'": "{'discovery': {'server': {'base': {'name': 'jupyterlab_s3_browser_uccps'}}}, "*

 * *                 "'outputDir': 'jupyterlab_s3_browser_uccps/labextension', '_build': {'load': "*

 * *                 "'static/remoteEntry.a9b108e22db5ac7c4504.js'}}",*

 * * "'scripts'": "{'clean:labextension': 'rimraf jupyterlab_s3_browser_uccps/labextension'}"}*

```diff
@@ -46,29 +46,29 @@
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/IBM/jupyterlab_s3_browser",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.aa6024c5ea40b82c48e7.js",
+            "load": "static/remoteEntry.a9b108e22db5ac7c4504.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
-                    "name": "jupyterlab_s3_browser"
+                    "name": "jupyterlab_s3_browser_uccps"
                 },
                 "managers": [
                     "pip"
                 ]
             }
         },
         "extension": true,
-        "outputDir": "jupyterlab_s3_browser/labextension"
+        "outputDir": "jupyterlab_s3_browser_uccps/labextension"
     },
     "keywords": [
         "s3",
         "cloud",
         "object",
         "storage",
         "jupyter",
@@ -95,15 +95,15 @@
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
         "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf jupyterlab_s3_browser/labextension",
+        "clean:labextension": "rimraf jupyterlab_s3_browser_uccps/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "eslint": "jlpm run eslint:check --fix",
         "eslint:check": "eslint . --ext .ts,.tsx",
         "install:extension": "jupyter labextension develop --overwrite .",
         "precommit": "lint-staged",
         "prettier": "prettier --write '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "cd test && ./run-tests.sh",
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/tests/test_get_s3.py` & `jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/tests/test_get_s3.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/__init__.py` & `jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,24 +35,23 @@
         help="The client ID for the S3 api",
     )
     client_secret = Unicode(
         default_value=environ.get("JUPYTERLAB_S3_SECRET_ACCESS_KEY", ""),
         config=True,
         help="The client secret for the S3 api",
     )
-
     session_token = Unicode(
         default_value=environ.get("JUPYTERLAB_S3_SESSION_TOKEN", ""),
         config=True,
         help="(Optional) Token if you use STS as auth method",
     )
     use_ssl = Unicode(
         default_value=environ.get("JUPYTERLAB_S3_USE_SSL", ""),
         config=True,
-        help="Whether or not to use SSL"
+        help="Whether or not to use SSL",
     )
 
 
 
 def _load_jupyter_server_extension(server_app):
     """Registers the API handler to receive HTTP requests from the frontend extension.
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/_version.py` & `jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser/handlers.py` & `jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,14 @@
                 config = self.config
                 if config.endpoint_url and config.client_id and config.client_secret:
                     test_s3_credentials(
                         config.endpoint_url,
                         config.client_id,
                         config.client_secret,
                         config.session_token,
-                        config.use_ssl,
                     )
                     logging.debug("...successfully authenticated")
 
                     # If no exceptions were encountered during testS3Credentials,
                     # then assume we're authenticated
                     authenticated = True
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps/labextension/package.json` & `jupyterlab_s3_browser_uccps-0.10.4/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9906684027777778%*

 * *Differences: {"'jupyterlab'": "{'discovery': {'server': {'base': {'name': 'jupyterlab_s3_browser_uccps'}}}, "*

 * *                 "'outputDir': 'jupyterlab_s3_browser_uccps/labextension', delete: ['_build']}",*

 * * "'scripts'": "{'clean:labextension': 'rimraf jupyterlab_s3_browser_uccps/labextension'}"}*

```diff
@@ -44,31 +44,26 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "schema/**/*.{json,}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/IBM/jupyterlab_s3_browser",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.aa6024c5ea40b82c48e7.js",
-            "style": "./style"
-        },
         "discovery": {
             "server": {
                 "base": {
-                    "name": "jupyterlab_s3_browser"
+                    "name": "jupyterlab_s3_browser_uccps"
                 },
                 "managers": [
                     "pip"
                 ]
             }
         },
         "extension": true,
-        "outputDir": "jupyterlab_s3_browser/labextension"
+        "outputDir": "jupyterlab_s3_browser_uccps/labextension"
     },
     "keywords": [
         "s3",
         "cloud",
         "object",
         "storage",
         "jupyter",
@@ -95,15 +90,15 @@
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
         "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf jupyterlab_s3_browser/labextension",
+        "clean:labextension": "rimraf jupyterlab_s3_browser_uccps/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "eslint": "jlpm run eslint:check --fix",
         "eslint:check": "eslint . --ext .ts,.tsx",
         "install:extension": "jupyter labextension develop --overwrite .",
         "precommit": "lint-staged",
         "prettier": "prettier --write '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "cd test && ./run-tests.sh",
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/PKG-INFO` & `jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-s3-browser-uccps
-Version: 0.10.3
+Version: 0.10.4
 Summary: JupyterLab extension for browsing S3-compatible object storage
 Home-page: https://github.com/IBM/jupyterlab_s3_browser
 Author: James Reeve
 License: Apache-2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,S3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/jupyterlab_s3_browser_uccps.egg-info/SOURCES.txt` & `jupyterlab_s3_browser_uccps-0.10.4/jupyterlab_s3_browser_uccps.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,36 +4,29 @@
 install.json
 package.json
 pyproject.toml
 setup.py
 tsconfig.json
 yarn.lock
 jupyter-config/jupyterlab_s3_browser.json
-jupyterlab_s3_browser/__init__.py
-jupyterlab_s3_browser/_version.py
-jupyterlab_s3_browser/handlers.py
-jupyterlab_s3_browser/labextension/package.json
-jupyterlab_s3_browser/labextension/static/268.f31edca7f28c6bfffe28.js
-jupyterlab_s3_browser/labextension/static/534.9645931ef1a95d5a9df1.js
-jupyterlab_s3_browser/labextension/static/742.e2d83637b4dbb625a240.js
-jupyterlab_s3_browser/labextension/static/remoteEntry.aa6024c5ea40b82c48e7.js
-jupyterlab_s3_browser/labextension/static/style.js
-jupyterlab_s3_browser/tests/__init__.py
-jupyterlab_s3_browser/tests/test_auth.py
-jupyterlab_s3_browser/tests/test_get_s3.py
 jupyterlab_s3_browser_uccps/__init__.py
 jupyterlab_s3_browser_uccps/_version.py
 jupyterlab_s3_browser_uccps/handlers.py
 jupyterlab_s3_browser_uccps.egg-info/PKG-INFO
 jupyterlab_s3_browser_uccps.egg-info/SOURCES.txt
 jupyterlab_s3_browser_uccps.egg-info/dependency_links.txt
 jupyterlab_s3_browser_uccps.egg-info/not-zip-safe
 jupyterlab_s3_browser_uccps.egg-info/requires.txt
 jupyterlab_s3_browser_uccps.egg-info/top_level.txt
 jupyterlab_s3_browser_uccps/labextension/package.json
+jupyterlab_s3_browser_uccps/labextension/static/268.9f7aa0158cdfda8baf56.js
+jupyterlab_s3_browser_uccps/labextension/static/534.9645931ef1a95d5a9df1.js
+jupyterlab_s3_browser_uccps/labextension/static/742.e2d83637b4dbb625a240.js
+jupyterlab_s3_browser_uccps/labextension/static/remoteEntry.a9b108e22db5ac7c4504.js
+jupyterlab_s3_browser_uccps/labextension/static/style.js
 jupyterlab_s3_browser_uccps/tests/__init__.py
 jupyterlab_s3_browser_uccps/tests/test_auth.py
 jupyterlab_s3_browser_uccps/tests/test_get_s3.py
 src/browser.ts
 src/contents.ts
 src/index.ts
 style/base.css
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/src/browser.ts` & `jupyterlab_s3_browser_uccps-0.10.4/src/browser.ts`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
       const formData = new FormData(form);
       const formDataJSON: any = {};
       (formData as any).forEach((value: string, key: string) => {
         formDataJSON[key] = value;
       });
       const settings = ServerConnection.makeSettings();
       ServerConnection.makeRequest(
-        URLExt.join(settings.baseUrl, 'jupyterlab_s3_browser/auth'),
+        URLExt.join(settings.baseUrl, 'jupyterlab_s3_browser_uccps/auth'),
         {
           method: 'POST',
           body: JSON.stringify(formDataJSON)
         },
         settings
       ).then(response => {
         response.json().then(data => {
@@ -160,15 +160,15 @@
    * Returns true if the user is already authenticated
    * against an s3 object storage instance.
    */
   export function checkIfAuthenicated(): Promise<boolean> {
     return new Promise((resolve, reject) => {
       const settings = ServerConnection.makeSettings();
       ServerConnection.makeRequest(
-        URLExt.join(settings.baseUrl, 'jupyterlab_s3_browser/auth'),
+        URLExt.join(settings.baseUrl, 'jupyterlab_s3_browser_uccps/auth'),
         {
           method: 'GET'
         },
         settings
       ).then(response => {
         response.json().then(res => {
           resolve(res.authenticated);
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/src/contents.ts` & `jupyterlab_s3_browser_uccps-0.10.4/src/contents.ts`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     }
 
     return new Promise((resolve, reject) => {
       const settings = ServerConnection.makeSettings(); // can be stored as class var
       // s3path = s3path.substring(1, s3path.length)
 
       ServerConnection.makeRequest(
-        URLExt.join(settings.baseUrl, 'jupyterlab_s3_browser/files', s3path),
+        URLExt.join(settings.baseUrl, 'jupyterlab_s3_browser_uccps/files', s3path),
         {},
         settings
       ).then(response => {
         response
           .json()
           .then((content: any) => {
             if (content.error) {
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/src/index.ts` & `jupyterlab_s3_browser_uccps-0.10.4/src/index.ts`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  * S3 filebrowser plugin state namespace.
  */
 const NAMESPACE = 's3-filebrowser';
 
 /**
  * The ID for the plugin.
  */
-const PLUGIN_ID = 'jupyterlab_s3_browser:drive';
+const PLUGIN_ID = 'jupyterlab_s3_browser_uccps:drive';
 
 /**
  * The JupyterLab plugin for the S3 Filebrowser.
  */
 const fileBrowserPlugin: JupyterFrontEndPlugin<void> = {
   id: PLUGIN_ID,
   requires: [
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/style/base.css` & `jupyterlab_s3_browser_uccps-0.10.4/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/style/bucket-dark.svg` & `jupyterlab_s3_browser_uccps-0.10.4/style/bucket-dark.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/style/bucket-light.svg` & `jupyterlab_s3_browser_uccps-0.10.4/style/bucket-light.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/LICENSE` & `jupyterlab_s3_browser_uccps-0.10.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/README.md` & `jupyterlab_s3_browser_uccps-0.10.4/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/setup.py` & `jupyterlab_s3_browser_uccps-0.10.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     str(lab_path / "package.json"),
 ]
 
 package_data_spec = {
     name: ["*"],
 }
 
-labext_name = "jupyterlab-s3-browser"
+labext_name = "jupyterlab-s3-browser-uccps"
 
 data_files_spec = [
     ("share/jupyter/labextensions/%s" % labext_name, str(lab_path), "**"),
     ("share/jupyter/labextensions/%s" % labext_name, str(HERE), "install.json"),
     (
         "etc/jupyter/jupyter_server_config.d",
         "jupyter-config/jupyter_server_config.d",
@@ -65,15 +65,15 @@
 else:
     cmdclass["jsdeps"] = skip_if_exists(jstargets, js_command)
 
 #  long_description = (HERE / "README.md").read_text()
 
 setup_args = dict(
     name=name,
-    version="0.10.3",
+    version="0.10.4",
     url=pkg_json["homepage"],
     author=pkg_json["author"],
     description=pkg_json["description"],
     license=pkg_json["license"],
     packages=setuptools.find_packages(),
     cmdclass=cmdclass,
     platforms="Linux, Mac OS X, Windows",
```

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/tsconfig.json` & `jupyterlab_s3_browser_uccps-0.10.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/yarn.lock` & `jupyterlab_s3_browser_uccps-0.10.4/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_s3_browser_uccps-0.10.3/PKG-INFO` & `jupyterlab_s3_browser_uccps-0.10.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_s3_browser_uccps
-Version: 0.10.3
+Version: 0.10.4
 Summary: JupyterLab extension for browsing S3-compatible object storage
 Home-page: https://github.com/IBM/jupyterlab_s3_browser
 Author: James Reeve
 License: Apache-2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,S3
 Platform: Linux
 Platform: Mac OS X
```

