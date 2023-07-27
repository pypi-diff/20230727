# Comparing `tmp/jupyter_viz_extension-0.2.2.tar.gz` & `tmp/jupyter_viz_extension-0.2.3.tar.gz`

## Comparing `jupyter_viz_extension-0.2.2.tar` & `jupyter_viz_extension-0.2.3.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/.yarnrc.yml
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/install.json
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/tsconfig.json
--rw-r--r--   0        0        0   231366 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/yarn.lock
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter-config/nb-config/jupyter_viz_extension.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter-config/server-config/jupyter_viz_extension.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/_version.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/__init__.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/cmd.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/paraview.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/trame.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/user.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/package.json
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/plugin.json
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/747.9c4710b3d6c36a34214f.js
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/759.6e640b9e09625b3f48df.js
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js
--rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/remoteEntry.027b522a580a66176974.js
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/style.js
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/jupyter_viz_extension/share/launch_paraview.in
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/schema/plugin.json
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/src/components.tsx
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/src/dialogs.tsx
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/src/handler.ts
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/src/index.tsx
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/src/paraview.tsx
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/src/trame.tsx
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/style/base.css
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/style/collapsible.css
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/style/index.js
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/.gitignore
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/LICENSE
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/README.md
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/.yarnrc.yml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/CHANGELOG.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/install.json
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/tsconfig.json
+-rw-r--r--   0        0        0   231366 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/yarn.lock
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter-config/nb-config/jupyter_viz_extension.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter-config/server-config/jupyter_viz_extension.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/_version.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/trame_model.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/__init__.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/cmd.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/paraview.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/trame.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/user.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/package.json
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/plugin.json
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/747.e893f2b2bb7591fde94c.js
+-rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/759.b87504abaef54983a24e.js
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/remoteEntry.e49408fc099f9436f8e2.js
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/jupyter_viz_extension/share/launch_paraview.in
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/schema/plugin.json
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/src/components.tsx
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/src/dialogs.tsx
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/src/handler.ts
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/src/index.tsx
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/src/paraview.tsx
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/src/trame.tsx
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/style/base.css
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/style/collapsible.css
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/style/index.js
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/README.md
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_viz_extension-0.2.3/PKG-INFO
```

### Comparing `jupyter_viz_extension-0.2.2/package.json` & `jupyter_viz_extension-0.2.3/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.3'"}*

```diff
@@ -178,9 +178,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.2"
+    "version": "0.2.3"
 }
```

### Comparing `jupyter_viz_extension-0.2.2/tsconfig.json` & `jupyter_viz_extension-0.2.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/yarn.lock` & `jupyter_viz_extension-0.2.3/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/jupyter_viz_extension/__init__.py` & `jupyter_viz_extension-0.2.3/jupyter_viz_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/cmd.py` & `jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/cmd.py`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/paraview.py` & `jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/paraview.py`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/jupyter_viz_extension/handlers/user.py` & `jupyter_viz_extension-0.2.3/jupyter_viz_extension/handlers/user.py`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/package.json` & `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e49408fc099f9436f8e2.js'}}",*

 * * "'version'": "'0.2.3'"}*

```diff
@@ -106,15 +106,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/github_username/jupyter-viz-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.027b522a580a66176974.js",
+            "load": "static/remoteEntry.e49408fc099f9436f8e2.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_viz_extension"
                 },
@@ -183,9 +183,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.2"
+    "version": "0.2.3"
 }
```

### Comparing `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig` & `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/schemas/jupyter-viz-extension/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.3'"}*

```diff
@@ -178,9 +178,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.2"
+    "version": "0.2.3"
 }
```

### Comparing `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js` & `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/187.f44cc496302e8c70c5db.js`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/747.9c4710b3d6c36a34214f.js` & `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/747.e893f2b2bb7591fde94c.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,61 +1,61 @@
 "use strict";
 (self.webpackChunkjupyter_viz_extension = self.webpackChunkjupyter_viz_extension || []).push([
     [747], {
         150: (n, e, t) => {
             t.d(e, {
                 Z: () => c
             });
-            var r = t(645),
-                o = t.n(r),
+            var o = t(645),
+                r = t.n(o),
                 i = t(243),
-                a = o()((function(n) {
+                a = r()((function(n) {
                     return n[1]
                 }));
-            a.i(i.Z), a.push([n.id, ".juviz-sidepanel {\n  background: var(--jp-layout-color3);\n}\n\n.juviz-sidepanel-segment {\n  background: var(--jp-layout-color0);\n  color: var(--jp-content-font-color0);\n  padding: 10px;\n}\n\n.instance-list {\n  display: flex;\n  flex-direction: column;\n  row-gap: 10px;\n}\n\n.launch-button {\n  background: green;\n  color: white;\n  border: 0 solid green;\n  float: right;\n}\n\n.form-input {\n  margin-bottom: 12px;\n}\n", ""]);
+            a.i(i.Z), a.push([n.id, ".juviz-sidepanel {\n  background: var(--jp-layout-color3);\n}\n\n.juviz-sidepanel-segment {\n  background: var(--jp-layout-color0);\n  color: var(--jp-content-font-color0);\n  padding: 10px;\n}\n\n.instance-list {\n  display: flex;\n  flex-direction: column;\n  row-gap: 10px;\n}\n\n.instance-list li {\n  border: var(--jp-layout-color4) solid 2px;\n  padding: 5px;\n  display: flex;\n  flex-direction: row;\n}\n\n.launch-button {\n  background: green;\n  color: white;\n  border: 0 solid green;\n  float: right;\n  padding: 4px 8px;\n}\n\n.form-input {\n  margin-bottom: 12px;\n}\n\n.open-button {\n  width: 30%;\n  border: 0;\n  padding: 0;\n  background: var(--jp-layout-color2);\n  flex-shrink: 0;\n}\n\n.open-button:hover {\n  background-color: var(--jp-layout-color3);\n}\n\n.open-button:active {\n  color: white;\n  background-color: var(--jp-layout-color4);\n}", ""]);
             const c = a
         },
         243: (n, e, t) => {
             t.d(e, {
                 Z: () => i
             });
-            var r = t(645),
-                o = t.n(r)()((function(n) {
+            var o = t(645),
+                r = t.n(o)()((function(n) {
                     return n[1]
                 }));
-            o.push([n.id, ".Collapsible {\n  display: flex;\n  flex-direction: column;\n}\n\n.Collapsible__trigger {\n  background: var(--jp-layout-color2);\n  font-weight: 400;\n  text-decoration: none;\n  position: relative;\n  border: 1px solid var(--jp-border-color2);\n  padding: 10px;\n}\n\n.Collapsible__trigger::after {\n  content: url(\"data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' viewBox='0 0 18 18' data-icon='ui-components:caret-down' data-icon-id='f5537fa8-1a9a-4a78-8ef2-89c5dc9c297d'%3E%3Cg class='jp-icon3' fill='%23616161' shape-rendering='geometricPrecision'%3E%3Cpath d='M5.2,7.5L9,11.2l3.8-3.8H5.2z'%3E%3C/path%3E%3C/g%3E%3C/svg%3E\");\n  position: absolute;\n  right: 10px;\n  top: 10px;\n  display: block;\n  transition: transform 300ms;\n  color: var(--jp-content-font-color2);\n}\n\n.Collapsible__trigger.is-open::after {\n  content: url(\"data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' viewBox='0 0 18 18' data-icon='ui-components:caret-up' data-icon-id='56e43b00-063a-408d-8271-54b7f13cb275'%3E%3Cg class='jp-icon3' fill='%23616161' shape-rendering='geometricPrecision'%3E%3Cpath d='M5.2,10.5L9,6.8l3.8,3.8H5.2z'%3E%3C/path%3E%3C/g%3E%3C/svg%3E\");\n}\n\n.Collapsible__contentInner {\n  padding: 10px;\n  border: 1px solid var(--jp-border-color2);\n  border-top: 0;\n}\n", ""]);
-            const i = o
+            r.push([n.id, ".Collapsible {\n  display: flex;\n  flex-direction: column;\n}\n\n.Collapsible__trigger {\n  background: var(--jp-layout-color2);\n  font-weight: 400;\n  text-decoration: none;\n  position: relative;\n  border: 1px solid var(--jp-border-color2);\n  padding: 10px;\n}\n\n.Collapsible__trigger::after {\n  content: url(\"data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' viewBox='0 0 18 18' data-icon='ui-components:caret-down' data-icon-id='f5537fa8-1a9a-4a78-8ef2-89c5dc9c297d'%3E%3Cg class='jp-icon3' fill='%23616161' shape-rendering='geometricPrecision'%3E%3Cpath d='M5.2,7.5L9,11.2l3.8-3.8H5.2z'%3E%3C/path%3E%3C/g%3E%3C/svg%3E\");\n  position: absolute;\n  right: 10px;\n  top: 10px;\n  display: block;\n  transition: transform 300ms;\n  color: var(--jp-content-font-color2);\n}\n\n.Collapsible__trigger.is-open::after {\n  content: url(\"data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' viewBox='0 0 18 18' data-icon='ui-components:caret-up' data-icon-id='56e43b00-063a-408d-8271-54b7f13cb275'%3E%3Cg class='jp-icon3' fill='%23616161' shape-rendering='geometricPrecision'%3E%3Cpath d='M5.2,10.5L9,6.8l3.8,3.8H5.2z'%3E%3C/path%3E%3C/g%3E%3C/svg%3E\");\n}\n\n.Collapsible__contentInner {\n  padding: 10px;\n  border: 1px solid var(--jp-border-color2);\n  border-top: 0;\n}\n", ""]);
+            const i = r
         },
         645: n => {
             n.exports = function(n) {
                 var e = [];
                 return e.toString = function() {
                     return this.map((function(e) {
                         var t = n(e);
                         return e[2] ? "@media ".concat(e[2], " {").concat(t, "}") : t
                     })).join("")
-                }, e.i = function(n, t, r) {
+                }, e.i = function(n, t, o) {
                     "string" == typeof n && (n = [
                         [null, n, ""]
                     ]);
-                    var o = {};
-                    if (r)
+                    var r = {};
+                    if (o)
                         for (var i = 0; i < this.length; i++) {
                             var a = this[i][0];
-                            null != a && (o[a] = !0)
+                            null != a && (r[a] = !0)
                         }
                     for (var c = 0; c < n.length; c++) {
                         var l = [].concat(n[c]);
-                        r && o[l[0]] || (t && (l[2] ? l[2] = "".concat(t, " and ").concat(l[2]) : l[2] = t), e.push(l))
+                        o && r[l[0]] || (t && (l[2] ? l[2] = "".concat(t, " and ").concat(l[2]) : l[2] = t), e.push(l))
                     }
                 }, e
             }
         },
         379: (n, e, t) => {
-            var r, o = function() {
+            var o, r = function() {
                     var n = {};
                     return function(e) {
                         if (void 0 === n[e]) {
                             var t = document.querySelector(e);
                             if (window.HTMLIFrameElement && t instanceof window.HTMLIFrameElement) try {
                                 t = t.contentDocument.head
                             } catch (n) {
@@ -73,120 +73,120 @@
                     if (i[t].identifier === n) {
                         e = t;
                         break
                     } return e
             }
 
             function c(n, e) {
-                for (var t = {}, r = [], o = 0; o < n.length; o++) {
-                    var c = n[o],
+                for (var t = {}, o = [], r = 0; r < n.length; r++) {
+                    var c = n[r],
                         l = e.base ? c[0] + e.base : c[0],
                         s = t[l] || 0,
                         d = "".concat(l, " ").concat(s);
                     t[l] = s + 1;
                     var u = a(d),
                         p = {
                             css: c[1],
                             media: c[2],
                             sourceMap: c[3]
                         }; - 1 !== u ? (i[u].references++, i[u].updater(p)) : i.push({
                         identifier: d,
                         updater: g(p, e),
                         references: 1
-                    }), r.push(d)
+                    }), o.push(d)
                 }
-                return r
+                return o
             }
 
             function l(n) {
                 var e = document.createElement("style"),
-                    r = n.attributes || {};
-                if (void 0 === r.nonce) {
+                    o = n.attributes || {};
+                if (void 0 === o.nonce) {
                     var i = t.nc;
-                    i && (r.nonce = i)
+                    i && (o.nonce = i)
                 }
-                if (Object.keys(r).forEach((function(n) {
-                        e.setAttribute(n, r[n])
+                if (Object.keys(o).forEach((function(n) {
+                        e.setAttribute(n, o[n])
                     })), "function" == typeof n.insert) n.insert(e);
                 else {
-                    var a = o(n.insert || "head");
+                    var a = r(n.insert || "head");
                     if (!a) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
                     a.appendChild(e)
                 }
                 return e
             }
             var s, d = (s = [], function(n, e) {
                 return s[n] = e, s.filter(Boolean).join("\n")
             });
 
-            function u(n, e, t, r) {
-                var o = t ? "" : r.media ? "@media ".concat(r.media, " {").concat(r.css, "}") : r.css;
-                if (n.styleSheet) n.styleSheet.cssText = d(e, o);
+            function u(n, e, t, o) {
+                var r = t ? "" : o.media ? "@media ".concat(o.media, " {").concat(o.css, "}") : o.css;
+                if (n.styleSheet) n.styleSheet.cssText = d(e, r);
                 else {
-                    var i = document.createTextNode(o),
+                    var i = document.createTextNode(r),
                         a = n.childNodes;
                     a[e] && n.removeChild(a[e]), a.length ? n.insertBefore(i, a[e]) : n.appendChild(i)
                 }
             }
 
             function p(n, e, t) {
-                var r = t.css,
-                    o = t.media,
+                var o = t.css,
+                    r = t.media,
                     i = t.sourceMap;
-                if (o ? n.setAttribute("media", o) : n.removeAttribute("media"), i && "undefined" != typeof btoa && (r += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(i)))), " */")), n.styleSheet) n.styleSheet.cssText = r;
+                if (r ? n.setAttribute("media", r) : n.removeAttribute("media"), i && "undefined" != typeof btoa && (o += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(i)))), " */")), n.styleSheet) n.styleSheet.cssText = o;
                 else {
                     for (; n.firstChild;) n.removeChild(n.firstChild);
-                    n.appendChild(document.createTextNode(r))
+                    n.appendChild(document.createTextNode(o))
                 }
             }
             var f = null,
                 v = 0;
 
             function g(n, e) {
-                var t, r, o;
+                var t, o, r;
                 if (e.singleton) {
                     var i = v++;
-                    t = f || (f = l(e)), r = u.bind(null, t, i, !1), o = u.bind(null, t, i, !0)
-                } else t = l(e), r = p.bind(null, t, e), o = function() {
+                    t = f || (f = l(e)), o = u.bind(null, t, i, !1), r = u.bind(null, t, i, !0)
+                } else t = l(e), o = p.bind(null, t, e), r = function() {
                     ! function(n) {
                         if (null === n.parentNode) return !1;
                         n.parentNode.removeChild(n)
                     }(t)
                 };
-                return r(n),
+                return o(n),
                     function(e) {
                         if (e) {
                             if (e.css === n.css && e.media === n.media && e.sourceMap === n.sourceMap) return;
-                            r(n = e)
-                        } else o()
+                            o(n = e)
+                        } else r()
                     }
             }
             n.exports = function(n, e) {
-                (e = e || {}).singleton || "boolean" == typeof e.singleton || (e.singleton = (void 0 === r && (r = Boolean(window && document && document.all && !window.atob)), r));
+                (e = e || {}).singleton || "boolean" == typeof e.singleton || (e.singleton = (void 0 === o && (o = Boolean(window && document && document.all && !window.atob)), o));
                 var t = c(n = n || [], e);
                 return function(n) {
                     if (n = n || [], "[object Array]" === Object.prototype.toString.call(n)) {
-                        for (var r = 0; r < t.length; r++) {
-                            var o = a(t[r]);
-                            i[o].references--
+                        for (var o = 0; o < t.length; o++) {
+                            var r = a(t[o]);
+                            i[r].references--
                         }
                         for (var l = c(n, e), s = 0; s < t.length; s++) {
                             var d = a(t[s]);
                             0 === i[d].references && (i[d].updater(), i.splice(d, 1))
                         }
                         t = l
                     }
                 }
             }
         },
         747: (n, e, t) => {
             t.r(e);
-            var r = t(379),
-                o = t.n(r),
+            var o = t(379),
+                r = t.n(o),
                 i = t(150);
-            o()(i.Z, {
+            r()(i.Z, {
                 insert: "head",
                 singleton: !1
             }), i.Z.locals
         }
     }
 ]);
```

### Comparing `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/759.6e640b9e09625b3f48df.js` & `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/759.b87504abaef54983a24e.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 "use strict";
 (self.webpackChunkjupyter_viz_extension = self.webpackChunkjupyter_viz_extension || []).push([
     [759], {
         759: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => S
+                default: () => x
             });
             var a = n(303),
                 s = n(832),
                 i = n(271),
                 r = n.n(i),
-                o = n(628),
-                l = n.n(o),
+                l = n(628),
+                o = n.n(l),
                 c = n(344),
                 p = n(139);
             async function u(e, t = {}) {
                 const n = p.ServerConnection.makeSettings(),
                     a = c.URLExt.join(n.baseUrl, "jupyter-viz-extension", e);
                 let s;
                 try {
@@ -109,15 +109,15 @@
                     }), i.createElement(v, {
                         label: "Status",
                         value: this.props.state
                     }), i.createElement(v, {
                         label: "Time",
                         value: `${this.props.timeUsed} / ${this.props.timeLimit}`
                     }));
-                    return i.createElement(i.Fragment, null, i.createElement(l(), {
+                    return i.createElement(i.Fragment, null, i.createElement(o(), {
                         trigger: t
                     }, i.createElement(v, {
                         label: "Project",
                         value: this.props.account
                     }), i.createElement(v, {
                         label: "Partition",
                         value: this.props.partition
@@ -158,67 +158,66 @@
                         className: "instance-list"
                     }, this.state.instaces.map((e => i.createElement(g, Object.assign({}, e))))))
                 }
             }
             class b extends i.Component {
                 constructor(e) {
                     super(e), this.openInstance = () => {
-                        window.open(this.props.url, "_blank", "noreferrer")
+                        const e = p.ServerConnection.makeSettings(),
+                            t = c.URLExt.join(e.baseUrl, "proxy", String(this.props.port), "index.html");
+                        window.open(t, "_blank", "noreferrer")
                     }
                 }
                 render() {
-                    return i.createElement("div", null, i.createElement(l(), {
-                        trigger: "State: Running"
+                    return i.createElement("li", null, i.createElement("div", {
+                        style: {
+                            flexGrow: 1
+                        }
                     }, i.createElement(v, {
-                        label: "Connected To Backend",
-                        value: this.props.url
+                        label: "Port",
+                        value: `${this.props.port}`
                     }), i.createElement(v, {
-                        label: "Root Directory",
-                        value: this.props.path
+                        label: "Log File",
+                        value: this.props.log
                     })), i.createElement("button", {
+                        className: "open-button",
                         onClick: this.openInstance
                     }, "Open"))
                 }
             }
             class w extends i.Component {
                 constructor(e) {
                     super(e), this.launchInstance = async () => {
                         console.log("Launching trame app " + this.props.name);
                         const e = await u("trame", {
-                                method: "POST",
-                                body: JSON.stringify({
-                                    app_name: this.props.name
-                                })
-                            }),
-                            t = p.ServerConnection.makeSettings(),
-                            n = c.URLExt.join(t.baseUrl, "proxy", e.port.toString(), "index.html");
+                            method: "POST",
+                            body: JSON.stringify({
+                                app_name: this.props.name
+                            })
+                        });
                         this.setState({
-                            instances: [...this.state.instances, n]
+                            instances: [...this.state.instances, e]
                         }), await (0, a.showErrorMessage)("Success", `Launched new trame instance on port ${e.port}`)
                     }, this.state = {
-                        instances: []
+                        instances: this.props.instances
                     }
                 }
                 render() {
                     const e = i.createElement("div", null, i.createElement("b", null, " ", this.props.name, " "), i.createElement("br", null), "Running Instances: ", this.state.instances.length);
-                    return i.createElement(i.Fragment, null, i.createElement(l(), {
+                    return i.createElement(i.Fragment, null, i.createElement(o(), {
                         trigger: e
                     }, i.createElement(v, {
                         label: "Path",
                         value: this.props.path
                     }), i.createElement("h4", null, "Instances:", i.createElement("button", {
                         className: "launch-button",
                         onClick: this.launchInstance
                     }, "Launch")), i.createElement("div", {
                         className: "instance-list"
-                    }, this.state.instances.map((e => i.createElement(b, {
-                        name: this.props.name,
-                        path: this.props.path,
-                        url: e
-                    }))))))
+                    }, this.state.instances.map((e => i.createElement(b, Object.assign({}, e)))))))
                 }
             }
             class f extends i.Component {
                 constructor() {
                     super({}), this.fetchData = async () => {
                         this.setState({
                             apps: await u("trame")
@@ -227,21 +226,18 @@
                         apps: []
                     }, this.fetchData()
                 }
                 render() {
                     return i.createElement(i.Fragment, null, i.createElement("h3", null, "trame Apps:"), i.createElement("div", {
                         id: "trame-instances",
                         className: "instance-list"
-                    }, this.state.apps.map((e => i.createElement(w, {
-                        name: e.displayName,
-                        path: e.path
-                    })))))
+                    }, this.state.apps.map((e => i.createElement(w, Object.assign({}, e))))))
                 }
             }
-            const S = {
+            const x = {
                 id: "juviz-extension",
                 autoStart: !0,
                 activate: e => {
                     const t = new s.SplitPanel;
                     t.orientation = "vertical", t.id = "juviz-sidepanel", t.title.iconClass = "jp-ExtensionIcon jp-SideBar-tabIcon", t.title.caption = "JuWiz";
                     const n = a.ReactWidget.create(r().createElement(C, null));
                     n.addClass("juviz-sidepanel-segment"), t.addWidget(n);
```

### Comparing `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js` & `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/893.b4c09f80424627b87fe3.js`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/remoteEntry.027b522a580a66176974.js` & `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/remoteEntry.e49408fc099f9436f8e2.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v, b, g, m, y = {
+    var e, r, t, n, o, a, i, u, l, s, d, f, c, p, h, v, b, g, m, y = {
             299: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(271), t.e(759)]).then((() => () => t(759))),
                         "./extension": () => Promise.all([t.e(271), t.e(759)]).then((() => () => t(759))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -45,53 +45,53 @@
         for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         187: "f44cc496302e8c70c5db",
         271: "624d1e1a34fcab02d699",
-        747: "9c4710b3d6c36a34214f",
-        759: "6e640b9e09625b3f48df",
+        747: "e893f2b2bb7591fde94c",
+        759: "b87504abaef54983a24e",
         893: "b4c09f80424627b87fe3"
     } [e] + ".js?v=" + {
         187: "f44cc496302e8c70c5db",
         271: "624d1e1a34fcab02d699",
-        747: "9c4710b3d6c36a34214f",
-        759: "6e640b9e09625b3f48df",
+        747: "e893f2b2bb7591fde94c",
+        759: "b87504abaef54983a24e",
         893: "b4c09f80424627b87fe3"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyter-viz-extension:", j.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        i = f;
+                    var d = l[s];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
+                        i = d;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+            var f = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -113,15 +113,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("jupyter-viz-extension", "0.2.2", (() => Promise.all([j.e(271), j.e(759)]).then((() => () => j(759))))), u("react-collapsible", "2.10.0", (() => Promise.all([j.e(271), j.e(893)]).then((() => () => j(893)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyter-viz-extension", "0.2.3", (() => Promise.all([j.e(271), j.e(759)]).then((() => () => j(759))))), u("react-collapsible", "2.10.0", (() => Promise.all([j.e(271), j.e(893)]).then((() => () => j(893)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -171,63 +171,63 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
-                if ("u" == f) {
-                    if (!l || "u" != d) return !1
+                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
+                if ("u" == d) {
+                    if (!l || "u" != f) return !1
                 } else if (l)
-                    if (d == f)
+                    if (f == d)
                         if (u <= n) {
                             if (s != e[u]) return !1
                         } else {
                             if (o ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != f && "n" != f) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < d != o) return !1;
+                    if (u <= n || d < f != o) return !1;
                     l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, i = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || d(l(e, t, o, n)), p(e[t][o])
-    }, f = (e, r, t) => {
+        return a(n, o) || f(l(e, t, o, n)), c(e[t][o])
+    }, d = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, d = e => {
+    }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, o) {
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
         var a = j.I(r);
         return a && a.then ? a.then(e.bind(e, r, j.S[r], t, n, o)) : e(r, j.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), v = c(((e, r, t, n, o) => {
-        var a = r && j.o(r, t) && f(r, t, n);
-        return a ? p(a) : o()
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
+        var a = r && j.o(r, t) && d(r, t, n);
+        return a ? c(a) : o()
     })), b = {}, g = {
         271: () => h("default", "react", [1, 17, 0, 1]),
         139: () => h("default", "@jupyterlab/services", [1, 6, 6, 5]),
         303: () => h("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
         344: () => h("default", "@jupyterlab/coreutils", [1, 5, 6, 5]),
         628: () => v("default", "react-collapsible", [1, 2, 10, 0], (() => j.e(187).then((() => () => j(893))))),
         832: () => h("default", "@lumino/widgets", [1, 1, 37, 2])
```

### Comparing `jupyter_viz_extension-0.2.2/jupyter_viz_extension/labextension/static/third-party-licenses.json` & `jupyter_viz_extension-0.2.3/jupyter_viz_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/jupyter_viz_extension/share/launch_paraview.in` & `jupyter_viz_extension-0.2.3/jupyter_viz_extension/share/launch_paraview.in`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/src/dialogs.tsx` & `jupyter_viz_extension-0.2.3/src/dialogs.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 }
 
 function createInput(id: string, type: string, value: string, attributes: [string, string][] = []) {
   const input = document.createElement('input');
   input.type = type;
   input.id = id;
   input.value = value;
-  
+
   input.classList.add('form-input');
 
   for (const [option, value] of attributes) {
     input.setAttribute(option, value);
   }
 
   return input;
@@ -91,30 +91,30 @@
   }
 
   fetchUserData = async () => {
     const data = await requestAPI<{
       user: string,
       accounts: string[],
       partitions: string[]
-    }>('user')
+    }>('user');
 
     for (const account of data.accounts) {
       const optionElement = document.createElement('option');
       optionElement.value = account;
       optionElement.textContent = account;
       this._accountElement.appendChild(optionElement);
     }
 
     for (const partition of data.partitions) {
       const optionElement = document.createElement('option');
       optionElement.value = partition;
       optionElement.textContent = partition;
       this._partitionElement.appendChild(optionElement);
     }
-  }
+  };
 
   getValue(): ParaViewLaunchOptions {
     return {
       account: this._accountElement.value,
       partition: this._partitionElement.value,
       nodes: Number(this._nodesElement.value),
       timeLimit: this._timeElement.value,
```

### Comparing `jupyter_viz_extension-0.2.2/src/handler.ts` & `jupyter_viz_extension-0.2.3/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/src/index.tsx` & `jupyter_viz_extension-0.2.3/src/index.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/src/paraview.tsx` & `jupyter_viz_extension-0.2.3/src/paraview.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -65,28 +65,28 @@
 
   newInstance = async () => {
     const options = await showDialog({
       title: 'Launch a new ParaView instance',
       body: new ParaViewLauncherDialog()
     });
     console.log(options.value);
-    
+
     await requestAPI<Record<string, never>>('paraview', {
-        method: 'POST',
-        body: JSON.stringify(options.value)
-    })
+      method: 'POST',
+      body: JSON.stringify(options.value)
+    });
     await this.fetchData();
   };
 
   render() {
     return (
       <>
         <h3>
           Running ParaView backends:
-          <button className='launch-button' onClick={this.newInstance} >Launch</button>
+          <button className='launch-button' onClick={this.newInstance}>Launch</button>
         </h3>
         <div id='paraview-instances' className='instance-list'>
           {this.state.instaces.map((instance) => (
             <ParaViewInstance {...instance} />
           ))}
         </div>
       </>
```

### Comparing `jupyter_viz_extension-0.2.2/src/trame.tsx` & `jupyter_viz_extension-0.2.3/src/trame.tsx`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,109 @@
 import { URLExt } from '@jupyterlab/coreutils';
 import { ServerConnection } from '@jupyterlab/services';
-import { showErrorMessage } from '@jupyterlab/apputils'
+import { showErrorMessage } from '@jupyterlab/apputils';
 import * as React from 'react';
 import Collapsible from 'react-collapsible';
 import { Info } from './components';
 import { requestAPI } from './handler';
 
 
 type TrameAppOptions = {
   name: string;
   displayName: string;
   path: string;
-  instances: string[];
+  instances: TrameInstanceOptions[];
 };
 
 type TrameInstanceOptions = {
-  name: string;
-  path: string;
-  url: string;
+  port: number;
+  log: string;
 };
 
 
 class TrameAppInstance extends React.Component<TrameInstanceOptions> {
   constructor(props: TrameInstanceOptions) {
     super(props);
   }
 
   openInstance = () => {
-    window.open(this.props.url, '_blank', 'noreferrer');
+    const settings = ServerConnection.makeSettings();
+    const url = URLExt.join(settings.baseUrl, 'proxy', String(this.props.port), 'index.html');
+    window.open(url, '_blank', 'noreferrer');
   };
 
   render() {
     return (
-      <div>
-        <Collapsible trigger="State: Running">
-          <Info label="Connected To Backend" value={this.props.url} />
-          <Info label="Root Directory" value={this.props.path} />
-        </Collapsible>
-        <button onClick={this.openInstance}>Open</button>
-      </div>
+      <li>
+        <div style={{ flexGrow: 1 }}>
+          <Info label='Port' value={`${this.props.port}`} />
+          <Info label='Log File' value={this.props.log} />
+        </div>
+
+        <button className='open-button' onClick={this.openInstance}>Open</button>
+      </li>
     );
   }
 }
 
 
-class TrameApp extends React.Component<{name: string, path: string}, {instances: string[]}> {
-  constructor(props: {name: string, path: string}) {
+class TrameApp extends React.Component<TrameAppOptions, { instances: TrameInstanceOptions[] }> {
+  constructor(props: TrameAppOptions) {
     super(props);
     this.state = {
-      instances: []
-    }
+      instances: this.props.instances  // Initialize with existing instances. ToDo: Improve?
+    };
   }
-    
+
   launchInstance = async () => {
-    console.log('Launching trame app ' + this.props.name)
+    console.log('Launching trame app ' + this.props.name);
 
-    const response = await requestAPI<{port: number}>('trame', {
+    const instance = await requestAPI<TrameInstanceOptions>('trame', {
       method: 'POST',
       body: JSON.stringify({
         app_name: this.props.name
       })
     });
-    
-    const settings = ServerConnection.makeSettings();
-    // Use JupyterServerproxy for now
-    const url = URLExt.join(settings.baseUrl, 'proxy', response.port.toString(), 'index.html');
-      
+
     this.setState({
-      instances: [...this.state.instances, url]
+      instances: [...this.state.instances, instance]
     });
-    
-    await showErrorMessage('Success', `Launched new trame instance on port ${response.port}`);
-  }
+    await showErrorMessage('Success', `Launched new trame instance on port ${instance.port}`);
+  };
 
   render() {
     const title = (
       <div>
         <b> {this.props.name} </b><br />
         Running Instances: {this.state.instances.length}
       </div>
     );
 
     return (
       <>
         <Collapsible trigger={title}>
-          <Info label="Path" value={this.props.path} />
-          
+          <Info label='Path' value={this.props.path} />
+
           <h4>
             Instances:
-            <button className="launch-button" onClick={this.launchInstance} >Launch</button>
+            <button className='launch-button' onClick={this.launchInstance}>Launch</button>
           </h4>
-          <div className="instance-list">
-            {this.state.instances.map((url) => (
-              <TrameAppInstance
-                name={this.props.name}
-                path={this.props.path}
-                url={url}
-              />
+          <div className='instance-list'>
+            {this.state.instances.map(instance => (
+              <TrameAppInstance {...instance} />
             ))}
           </div>
         </Collapsible>
       </>
     );
   }
 }
 
 
-export class TrameSidepanelSegment extends React.Component<Record<string, never>,
-  { apps: TrameAppOptions[] }> {
+export class TrameSidepanelSegment extends React.Component<Record<string, never>, { apps: TrameAppOptions[] }> {
   constructor() {
     super({});
     this.state = { apps: [] };
     this.fetchData();
   }
 
   fetchData = async () => {
@@ -120,19 +112,16 @@
     });
   };
 
   render() {
     return (
       <>
         <h3>trame Apps:</h3>
-        <div id="trame-instances" className="instance-list">
+        <div id='trame-instances' className='instance-list'>
           {this.state.apps.map((app) => (
-            <TrameApp
-              name={app.displayName}
-              path={app.path}
-            />
+            <TrameApp {...app} />
           ))}
         </div>
       </>
     );
   }
 }
```

### Comparing `jupyter_viz_extension-0.2.2/style/collapsible.css` & `jupyter_viz_extension-0.2.3/style/collapsible.css`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/.gitignore` & `jupyter_viz_extension-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/LICENSE` & `jupyter_viz_extension-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/README.md` & `jupyter_viz_extension-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/pyproject.toml` & `jupyter_viz_extension-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_viz_extension-0.2.2/PKG-INFO` & `jupyter_viz_extension-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_viz_extension
-Version: 0.2.2
+Version: 0.2.3
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/github_username/jupyter-viz-extension
 Project-URL: Bug Tracker, https://github.com/github_username/jupyter-viz-extension/issues
 Project-URL: Repository, https://github.com/github_username/jupyter-viz-extension.git
 Author-email: Jonathan Windgassen <j.windgassen@fz-juelich.de>
 License: BSD 3-Clause License
```

