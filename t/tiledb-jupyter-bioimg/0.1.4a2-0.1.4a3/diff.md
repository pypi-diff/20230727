# Comparing `tmp/tiledb_jupyter_bioimg-0.1.4a2.tar.gz` & `tmp/tiledb_jupyter_bioimg-0.1.4a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb_jupyter_bioimg-0.1.4a2.tar", last modified: Wed Jul 26 14:03:47 2023, max compression
+gzip compressed data, was "tiledb_jupyter_bioimg-0.1.4a3.tar", last modified: Thu Jul 27 08:38:32 2023, max compression
```

## Comparing `tiledb_jupyter_bioimg-0.1.4a2.tar` & `tiledb_jupyter_bioimg-0.1.4a3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:03:47.972896 tiledb_jupyter_bioimg-0.1.4a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-26 14:03:47.972896 tiledb_jupyter_bioimg-0.1.4a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-26 13:59:52.000000 tiledb_jupyter_bioimg-0.1.4a2/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:03:47.972896 tiledb_jupyter_bioimg-0.1.4a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:03:47.968896 tiledb_jupyter_bioimg-0.1.4a2/src/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/src/embed.ts
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/src/version.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/src/widget.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:03:47.968896 tiledb_jupyter_bioimg-0.1.4a2/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/style/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:03:47.968896 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:03:47.968896 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:03:47.972896 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4.svg
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/468.720ed03247c90f307866.js
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/744.75e221d7275b67ed293a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/747.6f54d04ff1f3fe09aea9.js
--rw-r--r--   0 runner    (1001) docker     (123)   790041 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   536613 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/remoteEntry.f4c9c19f87e7a37fdb5b.js
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-26 14:02:49.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    86073 2023-07-26 14:03:11.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:03:47.968896 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-26 14:03:47.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-26 14:03:47.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:03:47.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:01:33.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 14:03:47.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 14:03:47.000000 tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-26 13:56:13.000000 tiledb_jupyter_bioimg-0.1.4a2/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:38:32.636464 tiledb_jupyter_bioimg-0.1.4a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-27 08:38:32.636464 tiledb_jupyter_bioimg-0.1.4a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-27 08:34:06.000000 tiledb_jupyter_bioimg-0.1.4a3/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 08:38:32.636464 tiledb_jupyter_bioimg-0.1.4a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:38:32.624464 tiledb_jupyter_bioimg-0.1.4a3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/src/embed.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/src/widget.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:38:32.628464 tiledb_jupyter_bioimg-0.1.4a3/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:38:32.628464 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:38:32.628464 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:38:32.636464 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/468.720ed03247c90f307866.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/744.76d7c7825d9e5b8b9e5b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/747.6f54d04ff1f3fe09aea9.js
+-rw-r--r--   0 runner    (1001) docker     (123)   790041 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   536613 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/remoteEntry.93be46de878c6c06707d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-27 08:37:26.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86073 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:38:32.628464 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-27 08:38:32.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-27 08:38:32.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 08:38:32.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 08:35:59.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 08:38:32.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 08:38:32.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/tsconfig.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/LICENSE` & `tiledb_jupyter_bioimg-0.1.4a3/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.4a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb_jupyter_bioimg
-Version: 0.1.4a2
+Version: 0.1.4a3
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/README.md` & `tiledb_jupyter_bioimg-0.1.4a3/README.md`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/package.json` & `tiledb_jupyter_bioimg-0.1.4a3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.1.4-alpha.3'"}*

```diff
@@ -101,9 +101,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.4-alpha.2"
+    "version": "0.1.4-alpha.3"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/setup.py` & `tiledb_jupyter_bioimg-0.1.4a3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,15 @@
     author="TileDB",
     description="A jupyterlab extension to visualize bioimages in TileDB format",
     long_description= long_description,
     long_description_content_type="text/markdown",
     cmdclass= cmdclass,
     packages=setuptools.find_packages(),
     install_requires=[
-        "ipywidgets>=7",
-        "jupyterlab>=3.5.0",
+        "ipywidgets>=7"
     ],
     zip_safe=False,
     include_package_data=True,
     python_requires=">=3.6",
     license="BSD-3-Clause",
     platforms="Linux, Mac OS X, Windows",
     keywords=["Jupyter", "JupyterLab", "JupyterLab3"],
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/src/index.ts` & `tiledb_jupyter_bioimg-0.1.4a3/src/index.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/src/version.ts` & `tiledb_jupyter_bioimg-0.1.4a3/src/version.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/src/widget.ts` & `tiledb_jupyter_bioimg-0.1.4a3/src/widget.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/_version.py` & `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/_version.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/package.json` & `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745833333333334%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.93be46de878c6c06707d.js'}}",*

 * * "'version'": "'0.1.4-alpha.3'"}*

```diff
@@ -31,15 +31,15 @@
         "style/index.js",
         "dist/*.js"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f4c9c19f87e7a37fdb5b.js",
+            "load": "static/remoteEntry.93be46de878c6c06707d.js",
             "style": "./style"
         },
         "extension": "lib/index",
         "outputDir": "tiledb_jupyter_bioimg/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
@@ -106,9 +106,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.4-alpha.2"
+    "version": "0.1.4-alpha.3"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4.svg` & `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4.svg`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/468.720ed03247c90f307866.js` & `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/468.720ed03247c90f307866.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/744.75e221d7275b67ed293a.js` & `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/744.76d7c7825d9e5b8b9e5b.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -64,11 +64,11 @@
                         version: n,
                         exports: l
                     })
                 }
             }
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.4-alpha.2","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","tiledb","bioimaging","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js","dist/*.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension && jlpm run build:dist","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:dist":"NODE_OPTIONS=--max-old-space-size=4096 webpack --mode=production","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^5 || ^6","@jupyterlab/application":"^3 || ^4","@tiledb-inc/bioimage-viewer":"^0.1.6-alpha.0"},"devDependencies":{"@jupyterlab/builder":"^3 || ^4","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","ts-loader":"^9.2.5","typescript":"~5.1.6","webpack":"^5.88.1","webpack-cli":"^5.1.4"},"resolutions":{"@luma.gl/constants":"8.5.16","@luma.gl/core":"8.5.16","@luma.gl/engine":"8.5.16","@luma.gl/experimental":"8.5.16","@luma.gl/gltools":"8.5.16","@luma.gl/shadertools":"8.5.16","@luma.gl/webgl":"8.5.16","@deck.gl/aggregation-layers":"8.8.12","@deck.gl/core":"8.8.12","@deck.gl/carto":"8.8.12","@deck.gl/extensions":"8.8.12","@deck.gl/geo-layers":"8.8.12","@deck.gl/google-maps":"8.8.12","@deck.gl/mapbox":"8.8.12","@deck.gl/json":"8.8.12","@deck.gl/layers":"8.8.12","@deck.gl/mesh-layers":"8.8.12","@deck.gl/react":"8.8.12","capnp-ts":"0.4.0"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.lab.config.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.4-alpha.3","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","tiledb","bioimaging","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js","dist/*.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension && jlpm run build:dist","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:dist":"NODE_OPTIONS=--max-old-space-size=4096 webpack --mode=production","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^5 || ^6","@jupyterlab/application":"^3 || ^4","@tiledb-inc/bioimage-viewer":"^0.1.6-alpha.0"},"devDependencies":{"@jupyterlab/builder":"^3 || ^4","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","ts-loader":"^9.2.5","typescript":"~5.1.6","webpack":"^5.88.1","webpack-cli":"^5.1.4"},"resolutions":{"@luma.gl/constants":"8.5.16","@luma.gl/core":"8.5.16","@luma.gl/engine":"8.5.16","@luma.gl/experimental":"8.5.16","@luma.gl/gltools":"8.5.16","@luma.gl/shadertools":"8.5.16","@luma.gl/webgl":"8.5.16","@deck.gl/aggregation-layers":"8.8.12","@deck.gl/core":"8.8.12","@deck.gl/carto":"8.8.12","@deck.gl/extensions":"8.8.12","@deck.gl/geo-layers":"8.8.12","@deck.gl/google-maps":"8.8.12","@deck.gl/mapbox":"8.8.12","@deck.gl/json":"8.8.12","@deck.gl/layers":"8.8.12","@deck.gl/mesh-layers":"8.8.12","@deck.gl/react":"8.8.12","capnp-ts":"0.4.0"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.lab.config.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/747.6f54d04ff1f3fe09aea9.js` & `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/747.6f54d04ff1f3fe09aea9.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js` & `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js` & `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js.LICENSE.txt` & `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/remoteEntry.f4c9c19f87e7a37fdb5b.js` & `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/remoteEntry.93be46de878c6c06707d.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -46,22 +46,22 @@
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         446: "3bf34f45c93ace9c0f28",
         468: "720ed03247c90f307866",
-        744: "75e221d7275b67ed293a",
+        744: "76d7c7825d9e5b8b9e5b",
         747: "6f54d04ff1f3fe09aea9",
         774: "a72cd7bed5a733f86080",
         995: "7e5a9c38e396a47c7d4a"
     } [e] + ".js?v=" + {
         446: "3bf34f45c93ace9c0f28",
         468: "720ed03247c90f307866",
-        744: "75e221d7275b67ed293a",
+        744: "76d7c7825d9e5b8b9e5b",
         747: "6f54d04ff1f3fe09aea9",
         774: "a72cd7bed5a733f86080",
         995: "7e5a9c38e396a47c7d4a"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
@@ -121,15 +121,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : o > l.from)) && (a[r] = {
                             get: t,
                             from: o,
                             eager: !!n
                         })
                     },
                     d = [];
-                return "default" === t && (l("@tiledb-inc/bioimage-viewer", "0.1.6-alpha.0", (() => Promise.all([S.e(995), S.e(774), S.e(446)]).then((() => () => S(3774))))), l("@tiledb-inc/jupyter-bioimage-viewer", "0.1.4-alpha.2", (() => S.e(744).then((() => () => S(1744)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@tiledb-inc/bioimage-viewer", "0.1.6-alpha.0", (() => Promise.all([S.e(995), S.e(774), S.e(446)]).then((() => () => S(3774))))), l("@tiledb-inc/jupyter-bioimage-viewer", "0.1.4-alpha.3", (() => S.e(744).then((() => () => S(1744)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json` & `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg/render.py` & `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/render.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb-jupyter-bioimg
-Version: 0.1.4a2
+Version: 0.1.4a3
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/tiledb_jupyter_bioimg.egg-info/SOURCES.txt` & `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 tiledb_jupyter_bioimg.egg-info/not-zip-safe
 tiledb_jupyter_bioimg.egg-info/requires.txt
 tiledb_jupyter_bioimg.egg-info/top_level.txt
 tiledb_jupyter_bioimg/labextension/package.json
 tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4.svg
 tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
 tiledb_jupyter_bioimg/labextension/static/468.720ed03247c90f307866.js
-tiledb_jupyter_bioimg/labextension/static/744.75e221d7275b67ed293a.js
+tiledb_jupyter_bioimg/labextension/static/744.76d7c7825d9e5b8b9e5b.js
 tiledb_jupyter_bioimg/labextension/static/747.6f54d04ff1f3fe09aea9.js
 tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js
 tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js.LICENSE.txt
 tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js
 tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/remoteEntry.f4c9c19f87e7a37fdb5b.js
+tiledb_jupyter_bioimg/labextension/static/remoteEntry.93be46de878c6c06707d.js
 tiledb_jupyter_bioimg/labextension/static/style.js
 tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a2/tsconfig.json` & `tiledb_jupyter_bioimg-0.1.4a3/tsconfig.json`

 * *Files identical despite different names*

