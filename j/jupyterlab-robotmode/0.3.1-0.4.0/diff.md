# Comparing `tmp/jupyterlab_robotmode-0.3.1.tar.gz` & `tmp/jupyterlab_robotmode-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_robotmode-0.3.1.tar", last modified: Wed Mar 17 12:36:56 2021, max compression
+gzip compressed data, was "jupyterlab_robotmode-0.4.0.tar", last modified: Thu Jul 27 13:01:33 2023, max compression
```

## Comparing `jupyterlab_robotmode-0.3.1.tar` & `jupyterlab_robotmode-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,41 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-03-17 12:36:56.820814 jupyterlab_robotmode-0.3.1/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1512 2020-12-04 13:49:38.000000 jupyterlab_robotmode-0.3.1/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)      388 2021-01-05 10:04:59.000000 jupyterlab_robotmode-0.3.1/MANIFEST.in
--rw-rw-r--   0 martin    (1000) martin    (1000)     2141 2021-03-17 12:36:56.819814 jupyterlab_robotmode-0.3.1/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     1045 2021-03-15 08:20:43.000000 jupyterlab_robotmode-0.3.1/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)      201 2021-01-05 10:04:59.000000 jupyterlab_robotmode-0.3.1/install.json
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-03-17 12:36:56.817814 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode/
--rw-rw-r--   0 martin    (1000) martin    (1000)      176 2021-01-05 10:04:59.000000 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      459 2021-01-05 10:04:59.000000 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode/_version.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-03-17 12:36:56.818814 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode/labextension/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2490 2021-03-17 12:36:56.000000 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode/labextension/package.json
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-03-17 12:36:56.818814 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode/labextension/static/
--rw-rw-r--   0 martin    (1000) martin    (1000)     8814 2021-03-17 12:36:56.000000 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode/labextension/static/480.4ec31ba8d7115e17188a.js
--rw-rw-r--   0 martin    (1000) martin    (1000)      276 2021-03-17 12:36:56.000000 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode/labextension/static/568.abb06746a29814ce5b35.js
--rw-rw-r--   0 martin    (1000) martin    (1000)     6108 2021-03-17 12:36:56.000000 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode/labextension/static/remoteEntry.09511d7e294e827882b9.js
--rw-rw-r--   0 martin    (1000) martin    (1000)      118 2021-03-17 12:36:55.000000 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode/labextension/static/style.js
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-03-17 12:36:56.818814 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2141 2021-03-17 12:36:56.000000 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      729 2021-03-17 12:36:56.000000 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2021-03-17 12:36:56.000000 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2021-03-15 08:28:19.000000 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode.egg-info/not-zip-safe
--rw-rw-r--   0 martin    (1000) martin    (1000)       21 2021-03-17 12:36:56.000000 jupyterlab_robotmode-0.3.1/jupyterlab_robotmode.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     2374 2021-03-17 12:32:52.000000 jupyterlab_robotmode-0.3.1/package.json
--rw-rw-r--   0 martin    (1000) martin    (1000)      153 2021-01-05 10:04:59.000000 jupyterlab_robotmode-0.3.1/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2021-03-17 12:36:56.820814 jupyterlab_robotmode-0.3.1/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)     2271 2021-01-05 10:04:59.000000 jupyterlab_robotmode-0.3.1/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2021-03-17 12:36:56.819814 jupyterlab_robotmode-0.3.1/src/
--rw-rw-r--   0 martin    (1000) martin    (1000)      214 2021-01-05 10:04:59.000000 jupyterlab_robotmode-0.3.1/src/index.ts
--rw-rw-r--   0 martin    (1000) martin    (1000)    17446 2021-03-17 12:27:32.000000 jupyterlab_robotmode-0.3.1/src/mode.ts
--rw-rw-r--   0 martin    (1000) martin    (1000)      731 2021-01-05 10:04:59.000000 jupyterlab_robotmode-0.3.1/src/plugin.ts
--rw-rw-r--   0 martin    (1000) martin    (1000)      406 2021-03-15 08:20:43.000000 jupyterlab_robotmode-0.3.1/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:01:33.926174 jupyterlab_robotmode-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/.yarnrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-27 13:01:33.926174 jupyterlab_robotmode-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:01:33.926174 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:01:33.926174 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-27 13:01:30.000000 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:01:33.926174 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-27 13:01:30.000000 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode/labextension/static/480.00e5f6c8a59de2f63f89.js
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-27 13:01:30.000000 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode/labextension/static/568.980f4f5aedf3c209f942.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-07-27 13:01:30.000000 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode/labextension/static/73.f05d0042f204e45c45d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-07-27 13:01:30.000000 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode/labextension/static/remoteEntry.72b66241ab942c2073a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-27 13:01:28.000000 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 13:01:30.000000 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:01:33.926174 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-27 13:01:33.000000 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-27 13:01:33.000000 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:01:33.000000 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:01:31.000000 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 13:01:33.000000 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 13:01:33.000000 jupyterlab_robotmode-0.4.0/jupyterlab_robotmode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:01:33.926174 jupyterlab_robotmode-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:01:33.926174 jupyterlab_robotmode-0.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/src/icons.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    21503 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/src/mode.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/src/plugin.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/src/tokens.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/src/typings.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:01:33.926174 jupyterlab_robotmode-0.4.0/style/
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/style/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-27 13:00:00.000000 jupyterlab_robotmode-0.4.0/tsconfigbase.json
```

### Comparing `jupyterlab_robotmode-0.3.1/LICENSE` & `jupyterlab_robotmode-0.4.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2020, MarketSquare
+Copyright (c) 2022, MarketSquare
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `jupyterlab_robotmode-0.3.1/PKG-INFO` & `jupyterlab_robotmode-0.4.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,49 @@
-Metadata-Version: 2.1
-Name: jupyterlab_robotmode
-Version: 0.3.1
-Summary: A JupyterLab extensions which adds CodeMirror mode for Robot Framework syntax
-Home-page: https://github.com/MarketSquare/jupyterlab_robotmode
-Author: MarketSquare
-License: BSD-3-Clause
-Description: # MarketSquare jupyterlab_robotmode
-        
-        [![binder-badge]][binder] [![pypi-badge]][pypi] [![conda-badge]][conda] [![npm-badge]][npm]
-        
-        A JupyterLab extensions which adds CodeMirror mode for Robot Framework syntax
-        
-        ## Prerequisites
-        
-        * JupyterLab
-        
-        ## Installation
-        
-        ### For JupyterLab 3
-        
-        ```bash
-        pip install jupyterlab_robotmode
-        ```
-        
-        or
-        
-        ```bash
-        conda install jupyterlab_robotmode -c conda-forge
-        ```
-        
-        ### For JupyterLab <=2
-        
-        ```bash
-        jupyter labextension install @marketsquare/jupyterlab_robotmode
-        ```
-        
-        [binder-badge]: https://mybinder.org/badge_logo.svg
-        [binder]: https://mybinder.org/v2/gh/MarketSquare/jupyterlab_robotmode/HEAD?urlpath=lab
-        [pypi]: https://pypi.org/project/jupyterlab-robotmode
-        [pypi-badge]: https://img.shields.io/pypi/v/jupyterlab_robotmode
-        [npm-badge]: https://img.shields.io/npm/v/@marketsquare/jupyterlab_robotmode
-        [npm]: https://www.npmjs.com/package/@marketsquare/jupyterlab_robotmode
-        [conda-badge]: https://img.shields.io/conda/vn/conda-forge/jupyterlab_robotmode
-        [conda]: https://anaconda.org/conda-forge/jupyterlab_robotmode
-        
-Keywords: Jupyter,JupyterLab
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# MarketSquare jupyterlab_robotmode
+
+[![binder-badge]][binder] [![pypi-badge]][pypi] [![conda-badge]][conda]
+[![npm-badge]][npm]
+
+A JupyterLab extension which adds CodeMirror mode for Robot Framework syntax
+
+![a screenshot of JupyterLab with Robot Framework files and launchers][screenshot]
+
+## Prerequisites
+
+- JupyterLab
+
+## Installation
+
+### For JupyterLab>3
+
+> **Note**: Support for JupyterLab 4 and Notebook 7 is in the planning stage: see
+> discussion on [#14].
+
+```bash
+pip install jupyterlab_robotmode
+```
+
+or
+
+```bash
+conda install jupyterlab_robotmode -c conda-forge
+```
+
+### For JupyterLab <=2
+
+> **Note**: This will pull a significantly older, unmaintained version of the extension.
+
+```bash
+jupyter labextension install @marketsquare/jupyterlab_robotmode
+```
+
+[binder-badge]: https://mybinder.org/badge_logo.svg
+[binder]: https://mybinder.org/v2/gh/MarketSquare/jupyterlab_robotmode/HEAD?urlpath=lab
+[pypi]: https://pypi.org/project/jupyterlab-robotmode
+[pypi-badge]: https://img.shields.io/pypi/v/jupyterlab_robotmode
+[npm-badge]: https://img.shields.io/npm/v/@marketsquare/jupyterlab_robotmode
+[npm]: https://www.npmjs.com/package/@marketsquare/jupyterlab_robotmode
+[conda-badge]: https://img.shields.io/conda/vn/conda-forge/jupyterlab_robotmode
+[conda]: https://anaconda.org/conda-forge/jupyterlab_robotmode
+[screenshot]:
+  https://user-images.githubusercontent.com/45380/162342746-48561188-5859-4469-8634-3c4fd13cdef5.png
+[#14]: https://github.com/MarketSquare/jupyterlab_robotmode/issues/14
```

### Comparing `jupyterlab_robotmode-0.3.1/jupyterlab_robotmode/labextension/static/remoteEntry.09511d7e294e827882b9.js` & `jupyterlab_robotmode-0.4.0/jupyterlab_robotmode/labextension/static/remoteEntry.72b66241ab942c2073a5.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,256 +1,281 @@
 var _JUPYTERLAB;
-(_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@marketsquare/jupyterlab_robotmode"] = (() => {
+(() => {
     "use strict";
-    var e, r, t, o, n, a, i, u, l, s, f, d, p, c, h, v = {
-            109: (e, r, t) => {
+    var e, r, t, o, a, n, i, u, l, f, d, s, p, c, h, b, v = {
+            730: (e, r, t) => {
                 var o = {
-                        "./index": () => t.e(568).then((() => () => t(568))),
-                        "./extension": () => t.e(480).then((() => () => t(480)))
+                        "./index": () => Promise.all([t.e(73), t.e(568)]).then((() => () => t(568))),
+                        "./extension": () => Promise.all([t.e(73), t.e(480)]).then((() => () => t(480)))
                     },
-                    n = (e, r) => (t.R = r, r = t.o(o, e) ? o[e]() : Promise.resolve().then((() => {
+                    a = (e, r) => (t.R = r, r = t.o(o, e) ? o[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    n = (e, r) => {
                         if (t.S) {
-                            var o = t.S.default,
-                                n = "default";
-                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return t.S[n] = e, t.I(n, r)
+                            var o = "default",
+                                a = t.S[o];
+                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                            return t.S[o] = e, t.I(o, r)
                         }
                     };
                 t.d(r, {
-                    get: () => n,
-                    init: () => a
+                    get: () => a,
+                    init: () => n
                 })
             }
         },
-        b = {};
+        m = {};
 
-    function m(e) {
-        if (b[e]) return b[e].exports;
-        var r = b[e] = {
+    function g(e) {
+        var r = m[e];
+        if (void 0 !== r) return r.exports;
+        var t = m[e] = {
             exports: {}
         };
-        return v[e].call(r.exports, r, r.exports, m), r.exports
+        return v[e](t, t.exports, g), t.exports
     }
-    return m.m = v, m.d = (e, r) => {
-        for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
+    g.m = v, g.c = m, g.n = e => {
+        var r = e && e.__esModule ? () => e.default : () => e;
+        return g.d(r, {
+            a: r
+        }), r
+    }, g.d = (e, r) => {
+        for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        480: "4ec31ba8d7115e17188a",
-        568: "abb06746a29814ce5b35"
+    }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + "." + {
+        73: "f05d0042f204e45c45d0",
+        480: "00e5f6c8a59de2f63f89",
+        568: "980f4f5aedf3c209f942"
     } [e] + ".js?v=" + {
-        480: "4ec31ba8d7115e17188a",
-        568: "abb06746a29814ce5b35"
-    } [e], m.g = function() {
+        73: "f05d0042f204e45c45d0",
+        480: "00e5f6c8a59de2f63f89",
+        568: "980f4f5aedf3c209f942"
+    } [e], g.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@marketsquare/jupyterlab_robotmode:", m.l = (t, o, n) => {
+    }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@marketsquare/jupyterlab_robotmode:", g.l = (t, o, a, n) => {
         if (e[t]) e[t].push(o);
         else {
-            var a, i;
-            if (void 0 !== n)
-                for (var u = document.getElementsByTagName("script"), l = 0; l < u.length; l++) {
-                    var s = u[l];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
-                        a = s;
+            var i, u;
+            if (void 0 !== a)
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var d = l[f];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
+                        i = d;
                         break
                     }
                 }
-            a || (i = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, m.nc && a.setAttribute("nonce", m.nc), a.setAttribute("data-webpack", r + n), a.src = t), e[t] = [o];
-            var f = (r, o) => {
-                    a.onerror = a.onload = null, clearTimeout(d);
-                    var n = e[t];
-                    if (delete e[t], a.parentNode && a.parentNode.removeChild(a), n && n.forEach((e => e(o))), r) return r(o)
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [o];
+            var s = (r, o) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
+                    var a = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(o))), r) return r(o)
                 },
-                d = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
-                    target: a
+                    target: i
                 }), 12e4);
-            a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), i && document.head.appendChild(a)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
         }
+    }, g.r = e => {
+        "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
+            value: "Module"
+        }), Object.defineProperty(e, "__esModule", {
+            value: !0
+        })
     }, (() => {
-        m.S = {};
+        g.S = {};
         var e = {},
             r = {};
-        m.I = (t, o) => {
+        g.I = (t, o) => {
             o || (o = []);
-            var n = r[t];
-            if (n || (n = r[t] = {}), !(o.indexOf(n) >= 0)) {
-                if (o.push(n), e[t]) return e[t];
-                m.o(m.S, t) || (m.S[t] = {});
-                var a = m.S[t],
+            var a = r[t];
+            if (a || (a = r[t] = {}), !(o.indexOf(a) >= 0)) {
+                if (o.push(a), e[t]) return e[t];
+                g.o(g.S, t) || (g.S[t] = {});
+                var n = g.S[t],
                     i = "@marketsquare/jupyterlab_robotmode",
                     u = [];
-                switch (t) {
-                    case "default":
-                        ((e, r, t) => {
-                            var o = a[e] = a[e] || {},
-                                n = o[r];
-                            (!n || !n.loaded && i > n.from) && (o[r] = {
-                                get: () => m.e(568).then((() => () => m(568))),
-                                from: i
-                            })
-                        })("@marketsquare/jupyterlab_robotmode", "0.3.1")
-                }
-                return e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && ((e, r, t, o) => {
+                    var a = n[e] = n[e] || {},
+                        u = a[r];
+                    (!u || !u.loaded && (1 != !u.eager ? o : i > u.from)) && (a[r] = {
+                        get: () => Promise.all([g.e(73), g.e(568)]).then((() => () => g(568))),
+                        from: i,
+                        eager: !1
+                    })
+                })("@marketsquare/jupyterlab_robotmode", "0.4.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        m.g.importScripts && (e = m.g.location + "");
-        var r = m.g.document;
+        g.g.importScripts && (e = g.g.location + "");
+        var r = g.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var o = t.length - 1; o > -1 && !e;) e = t[o--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), g.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             o = t[1] ? r(t[1]) : [];
         return t[2] && (o.length++, o.push.apply(o, r(t[2]))), t[3] && (o.push([]), o.push.apply(o, r(t[3]))), o
     }, o = (e, r) => {
         e = t(e), r = t(r);
         for (var o = 0;;) {
             if (o >= e.length) return o < r.length && "u" != (typeof r[o])[0];
-            var n = e[o],
-                a = (typeof n)[0];
-            if (o >= r.length) return "u" == a;
+            var a = e[o],
+                n = (typeof a)[0];
+            if (o >= r.length) return "u" == n;
             var i = r[o],
                 u = (typeof i)[0];
-            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
-            if ("o" != a && "u" != a && n != i) return n < i;
+            if (n != u) return "o" == n && "n" == u || "s" == u || "u" == n;
+            if ("o" != n && "u" != n && a != i) return a < i;
             o++
         }
-    }, n = e => {
+    }, a = e => {
+        var r = e[0],
+            t = "";
         if (1 === e.length) return "*";
-        if (0 in e) {
-            var r = "",
-                t = e[0];
-            r += 0 == t ? ">=" : -1 == t ? "<" : 1 == t ? "^" : 2 == t ? "~" : t > 0 ? "=" : "!=";
-            for (var o = 1, a = 1; a < e.length; a++) o--, r += "u" == (typeof(u = e[a]))[0] ? "-" : (o > 0 ? "." : "") + (o = 2, u);
-            return r
+        if (r + .5) {
+            t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
+            for (var o = 1, n = 1; n < e.length; n++) o--, t += "u" == (typeof(u = e[n]))[0] ? "-" : (o > 0 ? "." : "") + (o = 2, u);
+            return t
         }
         var i = [];
-        for (a = 1; a < e.length; a++) {
-            var u = e[a];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : n(u))
+        for (n = 1; n < e.length; n++) {
+            var u = e[n];
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : a(u))
         }
         return l();
 
         function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, a = (e, r) => {
+    }, n = (e, r) => {
         if (0 in e) {
             r = t(r);
             var o = e[0],
-                n = o < 0;
-            n && (o = -o - 1);
+                a = o < 0;
+            a && (o = -o - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > o && !n : "" == d != n);
-                if ("u" == f) {
-                    if (!l || "u" != d) return !1
+                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > o && !a : "" == s != a);
+                if ("u" == d) {
+                    if (!l || "u" != s) return !1
                 } else if (l)
-                    if (d == f)
+                    if (s == d)
                         if (u <= o) {
-                            if (s != e[u]) return !1
+                            if (f != e[u]) return !1
                         } else {
-                            if (n ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (a ? f > e[u] : f < e[u]) return !1;
+                            f != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
-                    if (n || u <= o) return !1;
+                else if ("s" != s && "n" != s) {
+                    if (a || u <= o) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= o || f < d != n) return !1;
+                    if (u <= o || d < s != a) return !1;
                     l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                } else "s" != s && "n" != s && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? n(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
-        var t = m.S[e];
-        if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = g.S[e];
+        if (!t || !g.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && o(e, r) ? r : e), 0)
-    }, l = (e, r, t) => "Unsatisfied version " + r + " of shared singleton module " + e + " (required " + n(t) + ")", s = (e, r, t, o) => {
-        var n = u(e, t);
-        return a(o, n) || "undefined" != typeof console && console.warn && console.warn(l(t, n, o)), f(e[t][n])
-    }, f = e => (e.loaded = 1, e.get()), d = (e => function(r, t, o, n) {
-        var a = m.I(r);
-        return a && a.then ? a.then(e.bind(e, r, m.S[r], t, o, n)) : e(r, m.S[r], t, o)
-    })(((e, r, t, o) => (i(e, t), s(r, 0, t, o)))), p = {}, c = {
-        453: () => d("default", "@jupyterlab/codemirror", [1, 3, 0, 5])
-    }, h = {
-        480: [453]
-    }, m.f.consumes = (e, r) => {
-        m.o(h, e) && h[e].forEach((e => {
-            if (m.o(p, e)) return r.push(p[e]);
+    }, l = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(o) + ")", f = (e, r, t, o) => {
+        var a = u(e, t);
+        return n(o, a) || d(l(e, t, a, o)), s(e[t][a])
+    }, d = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, s = e => (e.loaded = 1, e.get()), p = (e => function(r, t, o, a) {
+        var n = g.I(r);
+        return n && n.then ? n.then(e.bind(e, r, g.S[r], t, o, a)) : e(r, g.S[r], t, o)
+    })(((e, r, t, o) => (i(e, t), f(r, 0, t, o)))), c = {}, h = {
+        745: () => p("default", "@jupyterlab/ui-components", [1, 3, 6, 5]),
+        71: () => p("default", "@jupyterlab/launcher", [1, 3, 6, 5]),
+        122: () => p("default", "@jupyterlab/filebrowser", [1, 3, 6, 5]),
+        235: () => p("default", "@jupyterlab/codemirror", [1, 3, 6, 5]),
+        303: () => p("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
+        535: () => p("default", "@jupyterlab/mainmenu", [1, 3, 6, 5]),
+        720: () => p("default", "@jupyterlab/translation", [1, 3, 6, 5])
+    }, b = {
+        73: [745],
+        480: [71, 122, 235, 303, 535, 720]
+    }, g.f.consumes = (e, r) => {
+        g.o(b, e) && b[e].forEach((e => {
+            if (g.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    p[e] = 0, v[e] = t => {
-                        delete b[e], t.exports = r()
+                    c[e] = 0, g.m[e] = t => {
+                        delete g.c[e], t.exports = r()
                     }
                 },
                 o = r => {
-                    delete p[e], v[e] = t => {
-                        throw delete b[e], r
+                    delete c[e], g.m[e] = t => {
+                        throw delete g.c[e], r
                     }
                 };
             try {
-                var n = c[e]();
-                n.then ? r.push(p[e] = n.then(t).catch(o)) : t(n)
+                var a = h[e]();
+                a.then ? r.push(c[e] = a.then(t).catch(o)) : t(a)
             } catch (e) {
                 o(e)
             }
         }))
     }, (() => {
         var e = {
             234: 0
         };
-        m.f.j = (r, t) => {
-            var o = m.o(e, r) ? e[r] : void 0;
+        g.f.j = (r, t) => {
+            var o = g.o(e, r) ? e[r] : void 0;
             if (0 !== o)
                 if (o) t.push(o[2]);
                 else {
-                    var n = new Promise(((t, n) => {
-                        o = e[r] = [t, n]
-                    }));
-                    t.push(o[2] = n);
-                    var a = m.p + m.u(r),
+                    var a = new Promise(((t, a) => o = e[r] = [t, a]));
+                    t.push(o[2] = a);
+                    var n = g.p + g.u(r),
                         i = new Error;
-                    m.l(a, (t => {
-                        if (m.o(e, r) && (0 !== (o = e[r]) && (e[r] = void 0), o)) {
-                            var n = t && ("load" === t.type ? "missing" : t.type),
-                                a = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + a + ")", i.name = "ChunkLoadError", i.type = n, i.request = a, o[1](i)
+                    g.l(n, (t => {
+                        if (g.o(e, r) && (0 !== (o = e[r]) && (e[r] = void 0), o)) {
+                            var a = t && ("load" === t.type ? "missing" : t.type),
+                                n = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + n + ")", i.name = "ChunkLoadError", i.type = a, i.request = n, o[1](i)
                         }
-                    }), "chunk-" + r)
+                    }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                for (var o, n, [a, i, u] = t, l = 0, s = []; l < a.length; l++) n = a[l], m.o(e, n) && e[n] && s.push(e[n][0]), e[n] = 0;
-                for (o in i) m.o(i, o) && (m.m[o] = i[o]);
-                for (u && u(m), r && r(t); s.length;) s.shift()()
+                var o, a, [n, i, u] = t,
+                    l = 0;
+                if (n.some((r => 0 !== e[r]))) {
+                    for (o in i) g.o(i, o) && (g.m[o] = i[o]);
+                    u && u(g)
+                }
+                for (r && r(t); l < n.length; l++) a = n[l], g.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_marketsquare_jupyterlab_robotmode = self.webpackChunk_marketsquare_jupyterlab_robotmode || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), m(109)
+    })();
+    var y = g(730);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@marketsquare/jupyterlab_robotmode"] = y
 })();
```

### Comparing `jupyterlab_robotmode-0.3.1/jupyterlab_robotmode.egg-info/PKG-INFO` & `jupyterlab_robotmode-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,79 @@
 Metadata-Version: 2.1
-Name: jupyterlab-robotmode
-Version: 0.3.1
-Summary: A JupyterLab extensions which adds CodeMirror mode for Robot Framework syntax
+Name: jupyterlab_robotmode
+Version: 0.4.0
+Summary: A JupyterLab extension which adds a CodeMirror mode for Robot Framework syntax
 Home-page: https://github.com/MarketSquare/jupyterlab_robotmode
 Author: MarketSquare
 License: BSD-3-Clause
-Description: # MarketSquare jupyterlab_robotmode
-        
-        [![binder-badge]][binder] [![pypi-badge]][pypi] [![conda-badge]][conda] [![npm-badge]][npm]
-        
-        A JupyterLab extensions which adds CodeMirror mode for Robot Framework syntax
-        
-        ## Prerequisites
-        
-        * JupyterLab
-        
-        ## Installation
-        
-        ### For JupyterLab 3
-        
-        ```bash
-        pip install jupyterlab_robotmode
-        ```
-        
-        or
-        
-        ```bash
-        conda install jupyterlab_robotmode -c conda-forge
-        ```
-        
-        ### For JupyterLab <=2
-        
-        ```bash
-        jupyter labextension install @marketsquare/jupyterlab_robotmode
-        ```
-        
-        [binder-badge]: https://mybinder.org/badge_logo.svg
-        [binder]: https://mybinder.org/v2/gh/MarketSquare/jupyterlab_robotmode/HEAD?urlpath=lab
-        [pypi]: https://pypi.org/project/jupyterlab-robotmode
-        [pypi-badge]: https://img.shields.io/pypi/v/jupyterlab_robotmode
-        [npm-badge]: https://img.shields.io/npm/v/@marketsquare/jupyterlab_robotmode
-        [npm]: https://www.npmjs.com/package/@marketsquare/jupyterlab_robotmode
-        [conda-badge]: https://img.shields.io/conda/vn/conda-forge/jupyterlab_robotmode
-        [conda]: https://anaconda.org/conda-forge/jupyterlab_robotmode
-        
-Keywords: Jupyter,JupyterLab
+Project-URL: Source, https://github.com/MarketSquare/jupyterlab_robotmode
+Project-URL: Tracker, https://github.com/MarketSquare/jupyterlab_robotmode/issues
+Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
+Classifier: Framework :: Jupyter :: JupyterLab
+Classifier: Framework :: Jupyter :: JupyterLab :: 3
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
+Classifier: Framework :: Robot Framework
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# MarketSquare jupyterlab_robotmode
+
+[![binder-badge]][binder] [![pypi-badge]][pypi] [![conda-badge]][conda]
+[![npm-badge]][npm]
+
+A JupyterLab extension which adds CodeMirror mode for Robot Framework syntax
+
+![a screenshot of JupyterLab with Robot Framework files and launchers][screenshot]
+
+## Prerequisites
+
+- JupyterLab
+
+## Installation
+
+### For JupyterLab>3
+
+> **Note**: Support for JupyterLab 4 and Notebook 7 is in the planning stage: see
+> discussion on [#14].
+
+```bash
+pip install jupyterlab_robotmode
+```
+
+or
+
+```bash
+conda install jupyterlab_robotmode -c conda-forge
+```
+
+### For JupyterLab <=2
+
+> **Note**: This will pull a significantly older, unmaintained version of the extension.
+
+```bash
+jupyter labextension install @marketsquare/jupyterlab_robotmode
+```
+
+[binder-badge]: https://mybinder.org/badge_logo.svg
+[binder]: https://mybinder.org/v2/gh/MarketSquare/jupyterlab_robotmode/HEAD?urlpath=lab
+[pypi]: https://pypi.org/project/jupyterlab-robotmode
+[pypi-badge]: https://img.shields.io/pypi/v/jupyterlab_robotmode
+[npm-badge]: https://img.shields.io/npm/v/@marketsquare/jupyterlab_robotmode
+[npm]: https://www.npmjs.com/package/@marketsquare/jupyterlab_robotmode
+[conda-badge]: https://img.shields.io/conda/vn/conda-forge/jupyterlab_robotmode
+[conda]: https://anaconda.org/conda-forge/jupyterlab_robotmode
+[screenshot]:
+  https://user-images.githubusercontent.com/45380/162342746-48561188-5859-4469-8634-3c4fd13cdef5.png
+[#14]: https://github.com/MarketSquare/jupyterlab_robotmode/issues/14
```

### Comparing `jupyterlab_robotmode-0.3.1/jupyterlab_robotmode.egg-info/SOURCES.txt` & `jupyterlab_robotmode-0.4.0/jupyterlab_robotmode.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,32 @@
+.yarnrc
 LICENSE
 MANIFEST.in
 README.md
 install.json
 package.json
 pyproject.toml
 setup.py
 tsconfig.json
+tsconfigbase.json
 jupyterlab_robotmode/__init__.py
 jupyterlab_robotmode/_version.py
 jupyterlab_robotmode.egg-info/PKG-INFO
 jupyterlab_robotmode.egg-info/SOURCES.txt
 jupyterlab_robotmode.egg-info/dependency_links.txt
 jupyterlab_robotmode.egg-info/not-zip-safe
+jupyterlab_robotmode.egg-info/requires.txt
 jupyterlab_robotmode.egg-info/top_level.txt
 jupyterlab_robotmode/labextension/package.json
-jupyterlab_robotmode/labextension/static/480.4ec31ba8d7115e17188a.js
-jupyterlab_robotmode/labextension/static/568.abb06746a29814ce5b35.js
-jupyterlab_robotmode/labextension/static/remoteEntry.09511d7e294e827882b9.js
+jupyterlab_robotmode/labextension/static/480.00e5f6c8a59de2f63f89.js
+jupyterlab_robotmode/labextension/static/568.980f4f5aedf3c209f942.js
+jupyterlab_robotmode/labextension/static/73.f05d0042f204e45c45d0.js
+jupyterlab_robotmode/labextension/static/remoteEntry.72b66241ab942c2073a5.js
 jupyterlab_robotmode/labextension/static/style.js
+jupyterlab_robotmode/labextension/static/third-party-licenses.json
+src/icons.ts
 src/index.ts
 src/mode.ts
-src/plugin.ts
+src/plugin.ts
+src/tokens.ts
+src/typings.d.ts
+style/icon.svg
```

### Comparing `jupyterlab_robotmode-0.3.1/src/mode.ts` & `jupyterlab_robotmode-0.4.0/src/mode.ts`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,69 @@
 /*
-  Copyright (c) 2020 MarketSquare
+  Copyright (c) 2022 MarketSquare
   Distributed under the terms of the BSD-3-Clause License
 */
 
 /*
   An implementation of syntax highlighting for robot framework 3.1.
 
   http://robotframework.org/robotframework/3.1/RobotFrameworkUserGuide.html
 
   When necessary, the source code is consulted and ultimately trusted:
 
   https://github.com/robotframework/robotframework
 */
 
-
 import { ICodeMirror } from '@jupyterlab/codemirror';
 
-import { ISimpleState, TSimpleStates, ISimpleMeta } from 'codemirror';
+import type { ISimpleState, ISimpleMeta } from 'codemirror';
+
+import { MIME_TYPE, MODE_LABEL, MODE_NAME, EXTENSIONS } from './tokens';
 
+/** Our custom state. */
+type TRobotState = ISimpleState<TState, TT>;
+
+/** Our overall states */
+export type TRobotStates = {
+  [key in TState]: TRobotState[];
+};
 
 /** All the possible states: pushing non-existing states == bad */
 export type TMainState = 'test_cases' | 'keywords' | 'settings' | 'variables';
 export type TState =
   | TMainState
+  | 'comment'
   | 'double_string'
+  | 'if_else_if_start'
+  | 'if_else_start'
+  | 'if_start'
+  | 'inline_if_start'
+  | 'inline_if_keyword_invoking'
+  | 'inline_if_start_keyword'
+  | 'inline_if_start_else'
+  | 'inline_if_else_keyword_invoking'
   | 'keyword_def'
-  | 'keyword_invocation'
   | 'keyword_invocation_no_continue'
+  | 'keyword_invocation'
   | 'library'
   | 'loop_body_old'
   | 'loop_start_new'
   | 'loop_start_old'
   | 'single_string'
   | 'start'
-  | 'tags'
   | 'tags_comma'
+  | 'tags'
+  | 'try_else_start'
+  | 'try_except_start'
+  | 'try_finally_start'
+  | 'try_start'
   | 'variable_index'
   | 'variable_property'
-  | 'variable';
+  | 'variable'
+  | 'while_start';
 
 /** the tokens we use */
 export enum TT {
   AM = 'atom',
   AT = 'attribute',
   BE = 'builtin.em',
   BI = 'builtin',
@@ -58,57 +80,50 @@
   SE = 'string.em',
   SH = 'string.header',
   SS = 'string.strong',
   SSE = 'string.strong.em',
   S2 = 'string-2',
   ST = 'string',
   TG = 'tag',
-  V2 = 'variable-2'
-}
-
-export function LINK(token: TT): TT {
-  return (token + '.link') as any;
+  V2 = 'variable-2',
 }
 
 /** helper function for compactly representing a rule */
-function r(
-  regex: RegExp,
-  token?: TT | TT[],
-  opt?: Partial<ISimpleState<string, any>>
-): ISimpleState<string, any> {
+function r(regex: RegExp, token?: TT | TT[], opt?: Partial<TRobotState>): TRobotState {
   return { regex, token, ...opt };
 }
 
 /** Possible Robot Framework table names. Group count is important.  */
 const TABLE_NAMES: { [key in TMainState]: RegExp } = {
   keywords: /(\|\s)?(\*+ *)(user keywords?|keywords?)( *\**)/i,
   settings: /(\|\s)?(\*+ *)(settings?)( *\**)/i,
   test_cases: /(\|\s)?(\*+ *)(tasks?|test cases?)( *\**)/i,
-  variables: /(\|\s)?(\*+ *)(variables?)( *\**)/i
+  variables: /(\|\s)?(\*+ *)(variables?)( *\**)/i,
 };
 
 /** Enumerate the possible rules  */
 const RULES_TABLE = Object.keys(TABLE_NAMES).map((next: TMainState) => {
   return r(TABLE_NAMES[next], [TT.BK, TT.HL, TT.HL, TT.HL], {
     next,
-    sol: true
+    sol: true,
   });
 });
 
 const RULE_COMMENT_POP = r(/#.*$/, TT.CM, { pop: true });
 
 /** Valid python operators */
 const VAR_OP = /[*\-+\\%&|=><!]/;
 /** Valid python numbers */
 const VAR_NUM = /0(b[01]+|o[0-7]+|x[0-9a-f]+)|(\d+)(\.\d+)?(e-?(\d+)(\.\d+)?)?/i;
 /**
     Valid python builtins
     Valid  way out at the end is a lookahead for VAR_OP, end or .
 */
-const VAR_BUILTIN = /(none|(cur|temp|exec)dir|\/|:|\\n|true|empty|false|null|space|test (name|documentation|status|message|tags)|prev test (name|status|message)|suite (name|source|documentation|status|message|metadata)|keyword (status|message)|(report|debug) file|log (file|level)|output (dir|file))(?=[.}]|\s+[*\-+\\%&|=><!])/i;
+const VAR_BUILTIN =
+  /(none|(cur|temp|exec)dir|\/|:|\\n|true|empty|false|null|space|test (name|documentation|status|message|tags)|prev test (name|status|message)|suite (name|source|documentation|status|message|metadata)|keyword (status|message)|(report|debug) file|log (file|level)|output (dir|file))(?=[.}]|\s+[*\-+\\%&|=><!])/i;
 
 /** a rule for the beginning of the variable state */
 const RULE_VAR_START = r(/[\$&@%]\{/, TT.V2, { push: 'variable' });
 /** a rule for the end of the variable state */
 const RULE_VAR_END = r(/\}/, TT.V2);
 
 /** a rule for a number */
@@ -119,81 +134,73 @@
 /** a rule for starting a double quote */
 const RULE_DOUBLE_STRING_START = r(/"/, TT.ST, { push: 'double_string' });
 
 /** a rule for capturing tags (and friends) in keyword/test/task definitions */
 const RULE_TAGS = r(
   /([|\s]*\s*)(\[\s*)(tags)(\s*\])(\s*\|?)/i,
   [TT.BK, TT.MT, TT.MT, TT.MT, TT.BK],
-  { sol: true, push: 'tags' }
+  { sol: true, push: 'tags' },
 );
 
 /** rule for special case of applying tags at the suite level */
-const RULE_SUITE_TAGS = r(
-  /(force tags|default tags)(\t+|  +)/i,
-  [TT.MT, null],
-  {
-    push: 'tags',
-    sol: true
-  }
-);
+const RULE_SUITE_TAGS = r(/(force tags|default tags)(\t+|  +)/i, [TT.MT, null], {
+  push: 'tags',
+  sol: true,
+});
 /** rule for special case of applying tags at the suite level (with pipes) */
 const RULE_SUITE_TAGS_PIPE = r(
   /(\| +)(force tags|default tags)( *\|?)/i,
   [TT.BK, TT.MT, TT.BK],
-  { sol: true, push: 'tags' }
+  { sol: true, push: 'tags' },
 );
 
 /** rule for bracketed settings of keyword/test/task */
 const RULE_SETTING_KEYWORD = r(
   /([|\s]*)(\[\s*)(setup|teardown|template)(\s*\])(\s*\|?)/i,
   [TT.BK, TT.MT, TT.MT, TT.MT, TT.BK],
-  { push: 'keyword_invocation_no_continue', sol: true }
+  { push: 'keyword_invocation_no_continue', sol: true },
 );
 
 /** rule for bracketed settings of keyword/test/task that include a keyword */
 const RULE_SUITE_SETTING_KEYWORD = r(
   /(suite setup|suite teardown|test setup|test teardown|test template|task setup|task teardown|task template)(\t+|  +)/i,
   [TT.MT, null],
-  { push: 'keyword_invocation', sol: true }
+  { push: 'keyword_invocation', sol: true },
 );
 
 /** rule for bracketed settings of keyword/test/task that include a keyword (with pipes) */
 const RULE_SUITE_SETTING_KEYWORD_PIPE = r(
   /(\| +)(suite setup|suite teardown|test setup|test teardown|test template|task setup|task teardown|task template)( +\|)/i,
   [TT.BK, TT.MT, TT.BK],
-  { push: 'keyword_invocation', sol: true }
+  { push: 'keyword_invocation', sol: true },
 );
 
 const RULE_SETTING_LIBRARY = r(/(library)(\t+|  +)/i, [TT.MT, null], {
   push: 'library',
-  sol: true
+  sol: true,
 });
 
-const RULE_SETTING_LIBRARY_PIPE = r(
-  /(\| +)(library)( +\|)/i,
-  [TT.BK, TT.MT, TT.BK],
-  {
-    push: 'library',
-    sol: true
-  }
-);
+const RULE_SETTING_LIBRARY_PIPE = r(/(\| +)(library)( +\|)/i, [TT.BK, TT.MT, TT.BK], {
+  push: 'library',
+  sol: true,
+});
 
 /** rule to escape the final closing bracket of a var at the end of a line */
 const RULE_LINE_ENDS_WITH_VAR = r(/\}\s*(?=$)/, TT.V2, { pop: true });
 
 const RULE_ELLIPSIS = r(/(\s*)(\.\.\.)/, [null, TT.BK], { sol: true });
 const RULE_NOT_ELLIPSIS_POP = r(/(?!\s*(\\|\.\.\.))/, null, {
   pop: true,
-  sol: true
+  sol: true,
 });
 
 const RULE_DOC_TAGS = r(/(Tags:)(\s*)/i, [TT.MT, null], { push: 'tags_comma' });
 
 /** collects the states that we build */
-const states: Partial<TSimpleStates> = {};
+const states: Partial<TRobotStates> = {};
 
 /** base isn't a state. these are the "normal business" that any state might use */
 const base = [
   ...RULES_TABLE,
   RULE_VAR_START,
   RULE_VAR_END,
   RULE_DOC_TAGS,
@@ -201,213 +208,261 @@
   r(/\|/, TT.BK),
   r(/#.*$/, TT.CM),
   r(/\\ +/, TT.BK),
   r(/\\(?=$)/, TT.BK),
   r(
     // a non-variable argument fragment before a variable before an equal
     /([^\s\$@&%=]((?!\t+|\s+\|\s+|  +)([^=]|\\=))*?)(?=[$@&%].*?[^ =\\]=($|  |[^=]|\s+\||\t))/,
-    TT.AT
+    TT.AT,
   ),
   r(
     // a non-variable argument fragment before an equal
     /([^\s\$@&%=]((?!\t+|\s+\|\s+|  +)([^=]|\\=))*?)(?==($|  |[^=]|\s+\||\t))/,
-    TT.AT
+    TT.AT,
   ),
-  r(/[^\s]+:(?!\/)/, TT.OP),
+  // r(/[^\s]+:(?!\/)/, TT.OP),  // this was generating false positives with TRY
   r(/(=!<>+\-*\/%)*==?/, TT.OP),
   r(/_\*.*?\*_/, TT.SSE),
   r(/\*.*?\*/, TT.SS),
   r(/\_.*?\_/, TT.SE),
   // this is pretty extreme, but seems to work
   r(/[^\s\$@%&]+/, TT.ST),
-  r(/[\$@%&](?!\{)/, TT.ST)
+  r(/[\$@%&](?!\{)/, TT.ST),
 ];
 
 /** the starting state (begining of a file) */
 states.start = [
   r(/(%%python)( module )?(.*)?/, [TT.MT, TT.KW, TT.V2], {
     mode: { spec: 'ipython' },
-    sol: true
+    sol: true,
   }),
   r(/(%%[^\s]*).*$/, TT.MT, { sol: true }),
-  ...base
+  ...base,
 ];
 
 /** settings states */
 states.settings = [
   RULE_SUITE_TAGS_PIPE,
   RULE_SUITE_TAGS,
   RULE_SUITE_SETTING_KEYWORD_PIPE,
   RULE_SUITE_SETTING_KEYWORD,
   RULE_SETTING_LIBRARY,
   RULE_SETTING_LIBRARY_PIPE,
   r(
     /(\|*\s*)(resource|variables|documentation|metadata|test timeout|task timeout)(\s*)/i,
     [TT.BK, TT.MT, null],
-    { sol: true }
+    { sol: true },
   ),
-  ...base
+  ...base,
 ];
 
 states.library = [
   RULE_NOT_ELLIPSIS_POP,
   RULE_ELLIPSIS,
   RULE_LINE_ENDS_WITH_VAR,
   r(
     /(WITH NAME)(\t+|  +| +\| +)([^\|\s]*)(\s*)(\|?)(\s*)(?=$)/,
     [TT.AM, TT.BK, TT.DF, null, TT.BK, null],
     {
-      pop: true
-    }
+      pop: true,
+    },
   ),
-  // r(/[^\}\|\s]*$/, TT.ST, { pop: true }),
-  ...base
+  ...base,
 ];
 
 /** rule for behavior-driven-development keywords */
 const RULE_START_BDD = r(
   /(\|\s*\|\s*|\s\s+)?(given|when|then|and|but)/i,
   [TT.BK, TT.BE],
   {
     push: 'keyword_invocation',
-    sol: true
-  }
+    sol: true,
+  },
 );
 /** rule for whitespace keywords */
 const RULE_KEY_START = r(/(\t+|  +)(?!\.\.\.)/, null, {
   push: 'keyword_invocation',
-  sol: true
+  sol: true,
 });
 /** rule for pipe keywords */
 const RULE_KEY_START_PIPE = r(
   /(\| )(\s*)(|[^\|\s][^\|]*)(\s*)( \|)(\s+)/,
   [TT.BK, null, TT.SH, null, TT.BK, null],
   {
     push: 'keyword_invocation',
-    sol: true
-  }
+    sol: true,
+  },
 );
+
 /** rule for for old-style loops (slashes) */
-const RULE_START_LOOP_OLD = r(
-  /(\s\|*\s*)(:FOR)(\s\|*\s*)/,
-  [null, TT.AM, null],
-  {
-    push: 'loop_start_old',
-    sol: true
-  }
-);
+const RULE_START_LOOP_OLD = r(/(\s\|*\s*)(:FOR)(\s\|*\s*)/, [null, TT.AM, null], {
+  push: 'loop_start_old',
+  sol: true,
+});
+
 /** rule for for new-style loops (slashes) */
-const RULE_START_LOOP_NEW = r(
-  /(\s\|*\s*)(FOR)(\s\|*\s*)/,
-  [null, TT.AM, null],
-  {
-    push: 'loop_start_new',
-    sol: true
-  }
+const RULE_START_LOOP_NEW = r(/(\s\|*\s*)(FOR)(\s\|*\s*)/, [null, TT.AM, null], {
+  push: 'loop_start_new',
+  sol: true,
+});
+
+/** rule for inline if keyword */
+const RULE_START_INLINE_IF = r(
+  /(\s*)(IF)(\s\|*\s*)(?=[^\s].*\s{2,})/,
+  [null, TT.AM as any, null],
+  { push: 'inline_if_start', sol: true },
 );
+
+/** rule for inline if keyword with assignment */
+const RULE_START_INLINE_IF_VAR = r(
+  /(\s+)(.*?)(\s+)(=)(\s+)(IF)(\s\|*\s*)(?=[^\s].*\s{2,})/,
+  [null, TT.V2, null, TT.OP, null, TT.AM as any, null],
+  { push: 'inline_if_start', sol: true },
+);
+
 /** rule for if keyword */
 const RULE_START_IF = r(
-  /(\s\|*\s*)(IF)(\s\|*\s*)/,
+  /(\s\|*\s*)(IF)(\s\|*\s*)(?![^\s].*\s{2,})/,
   [null, TT.AM, null],
   {
     push: 'if_start',
-    sol: true
-  }
+    sol: true,
+  },
 );
+
 /** rule for else if keyword */
-const RULE_START_ELSE_IF = r(
-  /(\s\|*\s*)(ELSE IF)(\s\|*\s*)/,
-  [null, TT.AM, null],
-  {
-    next: 'else_if_start',
-    sol: true
-  }
-);
+const RULE_START_IF_ELSE_IF = r(/(\s\|*\s*)(ELSE IF)(\s\|*\s*)/, [null, TT.AM, null], {
+  next: 'if_else_if_start',
+  sol: true,
+});
+
 /** rule for else keyword */
-const RULE_START_ELSE = r(
-  /(\s\|*\s*)(ELSE)/,
-  [null, TT.AM],
-  {
-    next: 'else_start',
-    sol: true
-  }
-);
+const RULE_START_IF_ELSE = r(/(\s\|*\s*)(ELSE)(?=$)/, [null, TT.AM], {
+  next: 'if_else_start',
+  sol: true,
+});
+
+/** rule for try keyword */
+const RULE_START_TRY = r(/(\s\|*\s*)(TRY)(?=$)/, [null, TT.AM], {
+  push: 'try_start',
+  sol: true,
+});
+
+/** rule for simple try/except */
+const RULE_START_EXCEPT = r(/(\s\|*\s*)(EXCEPT)/, [null, TT.AM], {
+  next: 'try_except_start',
+  sol: true,
+});
+
+/** rule for try/else keyword */
+const RULE_START_TRY_ELSE = r(/(\s\|*\s*)(ELSE)(?=$)/, [null, TT.AM], {
+  next: 'try_else_start',
+  sol: true,
+});
+
+/** rule for try/finally keyword */
+const RULE_START_FINALLY = r(/(\s\|*\s*)(FINALLY)/, [null, TT.AM], {
+  next: 'try_finally_start',
+  sol: true,
+});
+
+const RULE_START_WHILE = r(/(\s\|*\s*)(WHILE)/, [null, TT.AM], {
+  push: 'while_start',
+  sol: true,
+});
+
 /** rule for end keyword */
-const RULE_END = r(
-  /([\|\s]*\s*)(END)/,
-  [null, TT.AM],
-  { sol: true, pop: true },
-);
+const RULE_END = r(/([\|\s]*\s*)(END)(?=$)/, [null, TT.AM], {
+  sol: true,
+  pop: true,
+});
 
 const RULES_TAGS_COMMON = [
   r(/\s\|\s*/, TT.BK),
   RULE_COMMENT_POP,
   RULE_ELLIPSIS,
   RULE_NOT_ELLIPSIS_POP,
   RULE_VAR_START,
   RULE_LINE_ENDS_WITH_VAR,
   RULE_VAR_END,
-  r(/ +/, null)
+  r(/ +/, null),
 ];
 
 /** rules for capturing individual tags */
 states.tags = [
   ...RULES_TAGS_COMMON,
   r(/[^\$&%@]*?(?=(  +| \|))/, TT.TG),
   // fall back to single char
-  r(/[^\$&%@|]/, TT.TG)
+  r(/[^\$&%@|]/, TT.TG),
 ];
 
 /** rules for capturing tags inside docs */
 states.tags_comma = [
   ...RULES_TAGS_COMMON,
   r(/(,)(\s*)/, [TT.PC, null]),
   r(/[^\$&%@,]+(?=,$)/, TT.TG),
   // fall back to single char
-  r(/[^\$&%@|,]/, TT.TG)
+  r(/[^\$&%@|,]/, TT.TG),
 ];
 
 /** need to catch empty white lines pretty explicitly */
 const RULE_WS_LINE = r(/\s*(?=$)/, null, { sol: true });
 
 /** not a state. rules for starting keyword invocation */
 const RULES_KEYWORD_INVOKING = [
   RULE_START_BDD,
   RULE_KEY_START_PIPE,
   RULE_KEY_START,
   r(/\|\s(?=[^\s*]*\|)/, null, { sol: true, push: 'keyword_invocation' }),
-  r(/(?=[^\s*])/, null, { sol: true, push: 'keyword_invocation' })
+  r(/(?=[^\s*])/, null, { sol: true, push: 'keyword_invocation' }),
 ];
 
 const RULE_SETTING_SIMPLE = r(
   /(\t+|  +)(\[\s*)(arguments|documentation|return|timeout)(\s*\])(\s*)/i,
   [null, TT.MT, TT.MT, TT.MT, null],
-  { sol: true }
+  { sol: true },
 );
 
 const RULE_SETTING_SIMPLE_PIPE = r(
   /(\|)(\s+)([^|*]*)(\s+)(\|)(\s+)(\[\s*)(arguments|documentation|return|timeout)(\s*\])(\s*)(\|?)/i,
   [TT.BK, null, TT.SH, null, TT.BK, null, TT.MT, TT.MT, TT.MT, null, TT.BK],
-  { sol: true }
+  { sol: true },
 );
 
+/** rule for atomic control flow */
+const RULE_CONTROL_FLOW_ATOM = r(/(\s*)(BREAK|CONTINUE|RETURN)([\s\|]{2,}|$)/, [
+  null,
+  TT.AM,
+  null,
+]);
+
+/** rules for starting control flow blocks */
+const RULES_CONTROL_FLOW = [
+  RULE_CONTROL_FLOW_ATOM,
+  RULE_START_LOOP_OLD,
+  RULE_START_LOOP_NEW,
+  RULE_START_WHILE,
+  RULE_START_INLINE_IF_VAR,
+  RULE_START_INLINE_IF,
+  RULE_START_IF,
+  RULE_START_TRY,
+];
+
 /** rules for data rows inside a keyword table */
 states.keywords = [
   RULE_ELLIPSIS,
   RULE_TAGS,
   RULE_SETTING_KEYWORD,
   RULE_SETTING_SIMPLE,
   RULE_SETTING_SIMPLE_PIPE,
   r(/(?=[^\s$&%@*|]+)/, null, { sol: true, push: 'keyword_def' }),
-  RULE_START_LOOP_OLD,
-  RULE_START_LOOP_NEW,
-  RULE_START_IF,
+  ...RULES_CONTROL_FLOW,
   RULE_WS_LINE,
   ...RULES_KEYWORD_INVOKING,
-  ...base
+  ...base,
 ];
 
 /** a keyword name fragment before an inline variable */
 const KEYWORD_WORD_BEFORE_VAR = /([^\s]*?(?=[\$&%@]\{))/i;
 /** a keyword containing spaces before a separator */
 const KEYWORD_WORD_WITH_SPACES_BEFORE_SEP = /(?:[^\t\n\r\|])+?(?=$|\t|\n|\r|  +)/;
 /** a keyword name fragment before a separator */
@@ -419,161 +474,266 @@
   RULE_VAR_START,
   RULE_LINE_ENDS_WITH_VAR,
   RULE_VAR_END,
   r(/ /, null),
   r(KEYWORD_WORD_BEFORE_VAR, TT.DF),
   r(KEYWORD_WORD_BEFORE_SEP, TT.DF, { pop: true }),
   r(KEYWORD_WORD_BEFORE_WS, TT.DF),
-  r(/(?=$)/, null, { sol: true, pop: true })
+  r(/(?=$)/, null, { sol: true, pop: true }),
 ];
 
 /** A range as used in for loops */
-const RULE_RANGE = r(/([\|\s]*\s*)(IN)( RANGE| ENUMERATE| ZIP)?/, [
-  null,
-  TT.AM,
-  TT.AM
-]);
+const RULE_RANGE = r(/([\|\s]*\s*)(IN)( RANGE| ENUMERATE| ZIP)?/, [null, TT.AM, TT.AM]);
 
 states.loop_start_new = [
   RULE_RANGE,
   r(/[.]{3}/, TT.BK),
   RULE_VAR_START,
   r(/\}(?=$)/, TT.V2),
   RULE_VAR_END,
-  RULE_START_LOOP_NEW,
-  RULE_START_IF,
+  ...RULES_CONTROL_FLOW,
   RULE_END,
   RULE_WS_LINE,
   ...RULES_KEYWORD_INVOKING,
-  ...base
+  ...base,
+];
+
+/** the state when in an (ELSE)IF predictate */
+states.inline_if_start = [
+  RULE_ELLIPSIS,
+  r(/[\s\|]{2,}/, null, { next: 'inline_if_start_keyword' }),
+  RULE_NOT_ELLIPSIS_POP,
+  RULE_VAR_START,
+  r(/\}(?=$)/, TT.V2),
+  RULE_VAR_END,
+  ...base,
+];
+
+/** the state when in an ELSE( IF) object */
+states.inline_if_start_keyword = [
+  RULE_ELLIPSIS,
+  RULE_CONTROL_FLOW_ATOM,
+  RULE_NOT_ELLIPSIS_POP,
+  r(KEYWORD_WORD_BEFORE_VAR, TT.KW, { next: 'inline_if_keyword_invoking' }),
+  r(KEYWORD_WORD_WITH_SPACES_BEFORE_SEP, TT.KW, { next: 'inline_if_keyword_invoking' }),
+  r(KEYWORD_WORD_BEFORE_SEP, TT.KW, { next: 'inline_if_keyword_invoking' }),
+  r(KEYWORD_WORD_BEFORE_WS, TT.KW, { next: 'inline_if_keyword_invoking' }),
+];
+
+/** the state when in an ELSE( IF) object */
+states.inline_if_keyword_invoking = [
+  RULE_ELLIPSIS,
+  RULE_NOT_ELLIPSIS_POP,
+  r(/(\s\|*\s*)(ELSE IF)(\s\|*\s*)/, [null, TT.AM, null], { next: 'inline_if_start' }),
+  r(/(\s\|*\s*)(ELSE)(\s\|*\s*)/, [null, TT.AM, null], {
+    next: 'inline_if_start_else',
+  }),
+  RULE_VAR_START,
+  r(/\}(?=$)/, TT.V2),
+  RULE_VAR_END,
+  ...base,
+];
+
+states.inline_if_start_else = [
+  RULE_ELLIPSIS,
+  r(KEYWORD_WORD_BEFORE_VAR, TT.KW, { next: 'inline_if_else_keyword_invoking' }),
+  r(KEYWORD_WORD_WITH_SPACES_BEFORE_SEP, TT.KW, {
+    next: 'inline_if_else_keyword_invoking',
+  }),
+  r(KEYWORD_WORD_BEFORE_SEP, TT.KW, { next: 'inline_if_else_keyword_invoking' }),
+  r(KEYWORD_WORD_BEFORE_WS, TT.KW, { next: 'inline_if_else_keyword_invoking' }),
+  ...base,
+];
+
+states.inline_if_else_keyword_invoking = [
+  RULE_ELLIPSIS,
+  RULE_NOT_ELLIPSIS_POP,
+  RULE_VAR_START,
+  r(/\}(?=$)/, TT.V2),
+  RULE_VAR_END,
+  ...base,
 ];
 
 states.if_start = [
   r(/[.]{3}/, TT.BK),
   RULE_VAR_START,
   r(/\}(?=$)/, TT.V2),
   RULE_VAR_END,
-  RULE_START_LOOP_NEW,
-  RULE_START_IF,
-  RULE_START_ELSE_IF,
-  RULE_START_ELSE,
+  ...RULES_CONTROL_FLOW,
+  RULE_START_IF_ELSE_IF,
+  RULE_START_IF_ELSE,
   RULE_END,
   RULE_WS_LINE,
   ...RULES_KEYWORD_INVOKING,
-  ...base
+  ...base,
 ];
 
-states.else_if_start = [
+states.if_else_if_start = [
   r(/[.]{3}/, TT.BK),
   RULE_VAR_START,
   r(/\}(?=$)/, TT.V2),
   RULE_VAR_END,
-  RULE_START_LOOP_NEW,
-  RULE_START_IF,
-  RULE_START_ELSE_IF,
-  RULE_START_ELSE,
+  ...RULES_CONTROL_FLOW,
+  RULE_START_IF_ELSE_IF,
+  RULE_START_IF_ELSE,
   RULE_END,
   RULE_WS_LINE,
   ...RULES_KEYWORD_INVOKING,
-  ...base
+  ...base,
 ];
 
-states.else_start = [
-  RULE_START_LOOP_NEW,
-  RULE_START_IF,
+states.if_else_start = [
+  ...RULES_CONTROL_FLOW,
+  RULE_END,
+  RULE_WS_LINE,
+  ...RULES_KEYWORD_INVOKING,
+  ...base,
+];
+
+states.try_start = [
+  ...RULES_CONTROL_FLOW,
+  RULE_START_EXCEPT,
+  RULE_START_TRY_ELSE,
+  RULE_START_FINALLY,
   RULE_END,
   RULE_WS_LINE,
   ...RULES_KEYWORD_INVOKING,
-  ...base
+  ...base,
+];
+
+states.try_except_start = [
+  r(/[.]{3}/, TT.BK),
+  r(/AS/, TT.AM),
+  r(/(glob|regexp):/i, TT.BI),
+  RULE_VAR_START,
+  r(/\}(?=$)/, TT.V2),
+  RULE_VAR_END,
+  ...RULES_CONTROL_FLOW,
+  RULE_START_EXCEPT,
+  RULE_START_TRY_ELSE,
+  RULE_START_FINALLY,
+  RULE_END,
+  RULE_WS_LINE,
+  ...RULES_KEYWORD_INVOKING,
+  ...base,
+];
+
+states.try_else_start = [
+  ...RULES_CONTROL_FLOW,
+  RULE_START_FINALLY,
+  RULE_END,
+  RULE_WS_LINE,
+  ...RULES_KEYWORD_INVOKING,
+  ...base,
+];
+
+states.try_finally_start = [
+  ...RULES_CONTROL_FLOW,
+  RULE_END,
+  RULE_WS_LINE,
+  ...RULES_KEYWORD_INVOKING,
+  ...base,
+];
+
+states.while_start = [
+  r(/[.]{3}/, TT.BK),
+  r(/AS/, TT.AM),
+  r(/(glob|regexp):/i, TT.BI),
+  RULE_VAR_START,
+  r(/\}(?=$)/, TT.V2),
+  RULE_VAR_END,
+  ...RULES_CONTROL_FLOW,
+  RULE_END,
+  RULE_WS_LINE,
+  ...RULES_KEYWORD_INVOKING,
+  ...base,
 ];
 
 states.loop_start_old = [
   r(/(?=.*)/, null, { sol: true, next: 'loop_body_old' }),
   RULE_RANGE,
   RULE_VAR_START,
   r(/\}(?=$)/, TT.V2),
   RULE_VAR_END,
-  ...base
+  ...base,
 ];
 
 states.loop_body_old = [
-  ...RULES_KEYWORD_INVOKING.map(rule => {
+  ...RULES_KEYWORD_INVOKING.map((rule) => {
     return {
       ...rule,
       regex: new RegExp(
         /([\|\s]*\s*)(\\)/.source +
-          (rule.regex instanceof RegExp ? rule.regex.source : rule.regex)
+          (rule.regex instanceof RegExp ? rule.regex.source : rule.regex),
       ),
       token:
         rule.token instanceof Array
           ? [null, TT.BK, ...rule.token]
-          : [null, TT.BK, rule.token]
+          : [null, TT.BK, rule.token],
     };
   }),
   r(/(?=\s+[^\\])/, null, { pop: true, sol: true }),
-  ...base
+  ...base,
 ];
 
 const RULE_CASE_SETTING_SIMPLE = r(
   /(\t+|  +)(\[\s*)(documentation|timeout)(\s*\])(\s*)/i,
   [null, TT.MT, TT.MT, TT.MT, null],
-  { sol: true }
+  { sol: true },
 );
 
 const RULE_CASE_SETTING_SIMPLE_PIPE = r(
   /(\|)(\s+)([^|*]*)(\s+)(\|)(\s+)(\[\s*)(documentation|timeout)(\s*\])(\s*)(\|?)/i,
   [TT.BK, null, TT.SH, null, TT.BK, null, TT.MT, TT.MT, TT.MT, null, TT.BK],
-  { sol: true }
+  { sol: true },
 );
 
 /** rules for data rows inside test/task definition */
 states.test_cases = [
   ...RULES_TABLE,
   RULE_WS_LINE,
   RULE_ELLIPSIS,
   RULE_TAGS,
   RULE_SETTING_KEYWORD,
   RULE_CASE_SETTING_SIMPLE,
   RULE_CASE_SETTING_SIMPLE_PIPE,
-  RULE_START_LOOP_OLD,
-  RULE_START_LOOP_NEW,
-  RULE_START_IF,
+  ...RULES_CONTROL_FLOW,
   r(/([^|\s*].+?)(?=(\t|  +|$))/, TT.SH, { sol: true }),
   ...RULES_KEYWORD_INVOKING,
   r(/(\|\s+)([^\s*\|\.][^\|]*?)(\s*)(\|?$)/, [TT.BK, TT.SH, TT.BK], {
-    sol: true
+    sol: true,
   }),
   r(/(\| +)([^\|\s].+?)(\s*)( \| )/, [TT.BK, TT.SH, null, TT.BK], {
-    sol: true
+    sol: true,
   }),
-  ...base
+  ...base,
 ];
 
 /** rules for inside of an invoked keyword instance */
 states.keyword_invocation = [
   r(/( ?)(=)(\t+|  +|\s+\|)/, [null, TT.OP, null]),
   r(/(?=\s*$)/, null, { pop: true }),
-  r(/(\\|\.\.\.) +/, TT.BK, { pop: true }),
+  r(/(\\|\.\.\.) +/, TT.BK),
   RULE_VAR_START,
   RULE_LINE_ENDS_WITH_VAR,
   RULE_VAR_END,
   RULE_COMMENT_POP,
   r(/( \| |  +|\t+)(?=[$@&])/, TT.BK),
   r(/( \| |  +|\t+)/, TT.BK, { pop: true }),
   r(/ /, null),
   r(KEYWORD_WORD_BEFORE_VAR, TT.KW, { pop: true }),
   r(KEYWORD_WORD_WITH_SPACES_BEFORE_SEP, TT.KW, { pop: true }),
   r(KEYWORD_WORD_BEFORE_SEP, TT.KW, { pop: true }),
   r(KEYWORD_WORD_BEFORE_WS, TT.KW),
-  ...base
+  ...base,
 ];
 
 states.keyword_invocation_no_continue = [
   RULE_NOT_ELLIPSIS_POP,
-  ...states.keyword_invocation
+  ...states.keyword_invocation,
 ];
 
 /** curious rule for the variables table */
 states.variables = [...base];
 
 /** rules for inside of a variable reference */
 states.variable = [
@@ -584,15 +744,15 @@
   r(/(:)(.*?[^\\])(?=\}\s*$)/, [TT.OP, TT.S2], { pop: true }),
   r(/(:)(.*?[^\\])(?=\})/, [TT.OP, TT.S2]),
   r(/\./, TT.OP, { push: 'variable_property' }),
   r(/\[/, TT.BK, { next: 'variable_index' }),
   r(/\}(?=\[)/, TT.V2),
   r(/(?=\}\s*$)/, null, { pop: true }),
   r(/\}/, TT.V2, { pop: true }),
-  r(/[^\{\}\n:]/, TT.V2)
+  r(/[^\{\}\n:]/, TT.V2),
 ];
 
 /** rules for extended syntax in a variable reference */
 states.variable_property = [
   RULE_VAR_START,
   RULE_VAR_END,
   RULE_NUM,
@@ -602,72 +762,52 @@
   r(/\(/, TT.BK),
   r(/\)/, TT.BK, { pop: true }),
   r(/([a-z_][a-z_\d]*)(=)/i, [TT.V2, TT.OP]),
   r(/,/, TT.PC),
   r(/[^}](?=\})/, TT.PR, { pop: true }),
   r(/(\})(\s*(?=$|\n))/, [TT.BK, null], { pop: true }),
   r(/\t*(?=$|\n)/, null, { pop: true }),
-  r(/[^}]/, TT.PR)
+  r(/[^}]/, TT.PR),
 ];
 
 /** rules for strings with single quotes */
-states.single_string = [
-  r(/\\'/, TT.ST),
-  r(/'/, TT.ST, { pop: true }),
-  r(/./, TT.ST)
-];
+states.single_string = [r(/\\'/, TT.ST), r(/'/, TT.ST, { pop: true }), r(/./, TT.ST)];
 /** rules for strings with double quotes */
-states.double_string = [
-  r(/\\"/, TT.ST),
-  r(/"/, TT.ST, { pop: true }),
-  r(/./, TT.ST)
-];
+states.double_string = [r(/\\"/, TT.ST), r(/"/, TT.ST, { pop: true }), r(/./, TT.ST)];
 
 /** rules for square-bracketed index referencing */
 states.variable_index = [
   RULE_VAR_START,
   RULE_VAR_END,
   RULE_NUM,
   r(/\[/, TT.BK),
   r(/\](?=\])/, TT.BK),
   r(/(\])(\})( ?=?)/, [TT.BK, TT.V2, TT.OP], { pop: true }),
   r(/(\])(\[)/, TT.BK),
   r(/\]/, TT.BK, { pop: true }),
-  r(/[^\]]/, TT.ST)
+  r(/[^\]]/, TT.ST),
 ];
 
-
-/** well-known mime type for robot framework (pygments, etc.) */
-export const MIME_TYPE = 'text/x-robotframework';
-/** the canonical CodeMirror mode name */
-export const MODE_NAME = 'robotframework';
-/** the human-readable name of the CodeMirror mode */
-export const MODE_LABEL = 'robotframework';
-/** primary file extension */
-export const DEFAULT_EXTENSION = 'robot';
-/** all recognized file extensions */
-export const EXTENSIONS = [DEFAULT_EXTENSION, 'resource'];
-
 /** the actual exported function that will install the mode in CodeMirror */
 export function defineRobotMode({ CodeMirror }: ICodeMirror) {
-  const meta: ISimpleMeta<string, any> = {
+  const meta: ISimpleMeta<TState, TT> = {
     meta: {
       dontIndentStates: ['comment'],
-      lineComment: '#'
-    }
+      lineComment: '#',
+    },
   };
 
-  CodeMirror.defineSimpleMode<string, any>(MODE_NAME, {
+  CodeMirror.defineSimpleMode<TState, TT>(MODE_NAME, {
     ...states,
     // @ts-ignore: There is a compilation error for some reason
-    meta
+    meta,
   });
 
   CodeMirror.defineMIME(MIME_TYPE, MODE_NAME);
 
   CodeMirror.modeInfo.push({
     ext: EXTENSIONS,
     mime: MIME_TYPE,
     mode: MODE_NAME,
-    name: MODE_LABEL
+    name: MODE_LABEL,
   });
 }
```

