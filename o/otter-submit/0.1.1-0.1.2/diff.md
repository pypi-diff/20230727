# Comparing `tmp/otter_submit-0.1.1.tar.gz` & `tmp/otter_submit-0.1.2.tar.gz`

## Comparing `otter_submit-0.1.1.tar` & `otter_submit-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,29 @@
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 otter_submit-0.1.1/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 otter_submit-0.1.1/.yarnrc.yml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 otter_submit-0.1.1/Untitled.ipynb
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 otter_submit-0.1.1/Untitled1.ipynb
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 otter_submit-0.1.1/install.json
--rw-r--r--   0        0        0   355868 2020-02-02 00:00:00.000000 otter_submit-0.1.1/package-lock.json
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 otter_submit-0.1.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 otter_submit-0.1.1/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 otter_submit-0.1.1/tsconfig.json
--rw-r--r--   0        0        0   285195 2020-02-02 00:00:00.000000 otter_submit-0.1.1/yarn.lock
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 otter_submit-0.1.1/otter_submit/_version.py
--rw-r--r--   0        0        0    20571 2020-02-02 00:00:00.000000 otter_submit-0.1.1/otter_submit/labextension/build_log.json
--rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 otter_submit-0.1.1/otter_submit/labextension/package.json
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 otter_submit-0.1.1/otter_submit/labextension/schemas/@otter-submit/submit-button/package.json.orig
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 otter_submit-0.1.1/otter_submit/labextension/schemas/@otter-submit/submit-button/plugin.json
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 otter_submit-0.1.1/otter_submit/labextension/static/lib_index_js.a552738018af89d94a0d.js
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 otter_submit-0.1.1/otter_submit/labextension/static/lib_index_js.a552738018af89d94a0d.js.map
--rw-r--r--   0        0        0    27506 2020-02-02 00:00:00.000000 otter_submit-0.1.1/otter_submit/labextension/static/remoteEntry.a0746d0f3a3846491d76.js
--rw-r--r--   0        0        0    26415 2020-02-02 00:00:00.000000 otter_submit-0.1.1/otter_submit/labextension/static/remoteEntry.a0746d0f3a3846491d76.js.map
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 otter_submit-0.1.1/otter_submit/labextension/static/style.js
--rw-r--r--   0        0        0    19371 2020-02-02 00:00:00.000000 otter_submit-0.1.1/otter_submit/labextension/static/style_index_js.eed68c68a11bc2d602a2.js
--rw-r--r--   0        0        0    14868 2020-02-02 00:00:00.000000 otter_submit-0.1.1/otter_submit/labextension/static/style_index_js.eed68c68a11bc2d602a2.js.map
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 otter_submit-0.1.1/schema/plugin.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 otter_submit-0.1.1/src/index.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 otter_submit-0.1.1/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 otter_submit-0.1.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 otter_submit-0.1.1/style/index.js
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 otter_submit-0.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 otter_submit-0.1.1/LICENSE
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 otter_submit-0.1.1/README.md
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 otter_submit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 otter_submit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 otter_submit-0.1.2/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 otter_submit-0.1.2/.yarnrc.yml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 otter_submit-0.1.2/install.json
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 otter_submit-0.1.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 otter_submit-0.1.2/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 otter_submit-0.1.2/tsconfig.json
+-rw-r--r--   0        0        0   285195 2020-02-02 00:00:00.000000 otter_submit-0.1.2/yarn.lock
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 otter_submit-0.1.2/otter_submit/_version.py
+-rw-r--r--   0        0        0    20571 2020-02-02 00:00:00.000000 otter_submit-0.1.2/otter_submit/labextension/build_log.json
+-rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 otter_submit-0.1.2/otter_submit/labextension/package.json
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 otter_submit-0.1.2/otter_submit/labextension/schemas/@otter-submit/submit-button/package.json.orig
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 otter_submit-0.1.2/otter_submit/labextension/schemas/@otter-submit/submit-button/plugin.json
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 otter_submit-0.1.2/otter_submit/labextension/static/lib_index_js.ec2676ba3debe7eaf44f.js
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 otter_submit-0.1.2/otter_submit/labextension/static/lib_index_js.ec2676ba3debe7eaf44f.js.map
+-rw-r--r--   0        0        0    27739 2020-02-02 00:00:00.000000 otter_submit-0.1.2/otter_submit/labextension/static/remoteEntry.edecc40756fbdb50f74b.js
+-rw-r--r--   0        0        0    26649 2020-02-02 00:00:00.000000 otter_submit-0.1.2/otter_submit/labextension/static/remoteEntry.edecc40756fbdb50f74b.js.map
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 otter_submit-0.1.2/otter_submit/labextension/static/style.js
+-rw-r--r--   0        0        0    19371 2020-02-02 00:00:00.000000 otter_submit-0.1.2/otter_submit/labextension/static/style_index_js.eed68c68a11bc2d602a2.js
+-rw-r--r--   0        0        0    14868 2020-02-02 00:00:00.000000 otter_submit-0.1.2/otter_submit/labextension/static/style_index_js.eed68c68a11bc2d602a2.js.map
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 otter_submit-0.1.2/schema/plugin.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 otter_submit-0.1.2/src/index.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 otter_submit-0.1.2/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 otter_submit-0.1.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 otter_submit-0.1.2/style/index.js
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 otter_submit-0.1.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 otter_submit-0.1.2/LICENSE
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 otter_submit-0.1.2/README.md
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 otter_submit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 otter_submit-0.1.2/PKG-INFO
```

### Comparing `otter_submit-0.1.1/package.json` & `otter_submit-0.1.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'0.1.2'"}*

```diff
@@ -171,12 +171,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.1",
+    "version": "0.1.2",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `otter_submit-0.1.1/tsconfig.json` & `otter_submit-0.1.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `otter_submit-0.1.1/yarn.lock` & `otter_submit-0.1.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `otter_submit-0.1.1/otter_submit/labextension/build_log.json` & `otter_submit-0.1.2/otter_submit/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999993348233291%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'@otter-submit/submit-button': {'version': "*

 * *      "'0.1.2'}}}}}}"}*

```diff
@@ -622,15 +622,15 @@
                             "import": false,
                             "requiredVersion": "^2.0.1",
                             "singleton": true
                         },
                         "@otter-submit/submit-button": {
                             "import": "/Users/sean/Documents/cb/otter-submit/lib/index.js",
                             "singleton": true,
-                            "version": "0.1.1"
+                            "version": "0.1.2"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^18.2.0",
                             "singleton": true
                         },
                         "react-dom": {
```

### Comparing `otter_submit-0.1.1/otter_submit/labextension/package.json` & `otter_submit-0.1.2/otter_submit/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9795833333333333%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.edecc40756fbdb50f74b.js'}}",*

 * * "'version'": "'0.1.2'"}*

```diff
@@ -103,15 +103,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/data-8/otter-submit",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.a0746d0f3a3846491d76.js",
+            "load": "static/remoteEntry.edecc40756fbdb50f74b.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "otter_submit/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -176,12 +176,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.1",
+    "version": "0.1.2",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `otter_submit-0.1.1/otter_submit/labextension/schemas/@otter-submit/submit-button/package.json.orig` & `otter_submit-0.1.2/otter_submit/labextension/schemas/@otter-submit/submit-button/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'0.1.2'"}*

```diff
@@ -171,12 +171,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.1",
+    "version": "0.1.2",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `otter_submit-0.1.1/otter_submit/labextension/static/lib_index_js.a552738018af89d94a0d.js` & `otter_submit-0.1.2/otter_submit/labextension/static/lib_index_js.ec2676ba3debe7eaf44f.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -17,14 +17,19 @@
                     "default": () => (__WEBPACK_DEFAULT_EXPORT__)
                     /* harmony export */
                 });
                 /* harmony import */
                 var _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @jupyterlab/notebook */ "webpack/sharing/consume/default/@jupyterlab/notebook");
                 /* harmony import */
                 var _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_0__);
+                /* harmony import */
+                var _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! @jupyterlab/ui-components */ "webpack/sharing/consume/default/@jupyterlab/ui-components");
+                /* harmony import */
+                var _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_1__);
+
 
                 /**
                  * The plugin registration information.
                  */
                 const plugin = {
                     id: '@otter-submit/submit-button:plugin',
                     description: 'A JupyterLab extension used to submit notebooks for grading to otter-service.',
@@ -39,14 +44,16 @@
                         var nbpanel;
                         notebookTracker.currentChanged.connect((tracker, panel) => {
                             nbpanel = panel;
                         });
                         // Add a command
                         commands.addCommand(command, {
                             label: "Submit for Grading",
+                            icon: _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_1__.fileUploadIcon,
+                            iconLabel: "Submit for Grading",
                             caption: 'Send your notebook to be graded',
                             execute: (args) => {
                                 var nb = nbpanel === null || nbpanel === void 0 ? void 0 : nbpanel.context.model.toJSON();
                                 var payload = JSON.stringify({
                                     'nb': nb
                                 });
                                 var otherParam = {
@@ -78,8 +85,8 @@
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.a552738018af89d94a0d.js.map
+//# sourceMappingURL=lib_index_js.ec2676ba3debe7eaf44f.js.map
```

### Comparing `otter_submit-0.1.1/otter_submit/labextension/static/lib_index_js.a552738018af89d94a0d.js.map` & `otter_submit-0.1.2/otter_submit/labextension/static/lib_index_js.ec2676ba3debe7eaf44f.js.map`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7857142857142857%*

 * *Differences: {"'file'": "'lib_index_js.ec2676ba3debe7eaf44f.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;AACwD;AACG;AAE3D;;GAEG;AACH,MAAM,MAAM,GAAgC;IAC1C,EAAE,EAAE,oCAAoC;IACxC,WAAW,EACT,+EAA+E;IACjF,SAAS,EAAE,IAAI;IACf,QAAQ,EAAE,CAAC,kEAAgB,CAAC;IAC5B,QAAQ,EAAE,CAAC,GAAoB,EAAE,eAAiC,EAAE,EAAE;QACpE,oBAAoB;QACpB,MAAM,EAAE,QAAQ,EAAE,GAAG,GAAG,CAAC;QACzB,MAAM,OAAO,GAAG,qBAAqB,CAAC;QACtC,IAAI,OAAa,CAAC;QAClB,eAAe,CAAC,cAAc,CAAC,OAAO,CAAC,CAAC,OAAO,EAAE,KAAK,EAAE,EAAE;YACxD,OAAO,GAAG,KAAK;QACjB,CAAC,CAAC;QAEF,gBAAgB;QAChB,QAAQ, […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "file": "lib_index_js.a552738018af89d94a0d.js",
-    "mappings": ";;;;;;;;;;;;;;;AACwD;AAExD;;GAEG;AACH,MAAM,MAAM,GAAgC;IAC1C,EAAE,EAAE,oCAAoC;IACxC,WAAW,EACT,+EAA+E;IACjF,SAAS,EAAE,IAAI;IACf,QAAQ,EAAE,CAAC,kEAAgB,CAAC;IAC5B,QAAQ,EAAE,CAAC,GAAoB,EAAE,eAAiC,EAAE,EAAE;QACpE,oBAAoB;QACpB,MAAM,EAAE,QAAQ,EAAE,GAAG,GAAG,CAAC;QACzB,MAAM,OAAO,GAAG,qBAAqB,CAAC;QACtC,IAAI,OAAa,CAAC;QAClB,eAAe,CAAC,cAAc,CAAC,OAAO,CAAC,CAAC,OAAO,EAAE,KAAK,EAAE,EAAE;YACxD,OAAO,GAAG,KAAK;QACjB,CAAC,CAAC;QAEF,gBAAgB;QAChB,QAAQ,CAAC,UAAU,CAAC,OAAO,EAAE;YAC3B,KAAK,EAAE,oBAAoB;YAC3B,OAAO,EAAE,iCAAiC;YAC1C,OAAO,EAAE,CAAC,IAAS,EAAE,EAAE;gBACrB,IAAI,EAAE,GAAG,OAAO,aAAP,OAAO,uBAAP,OAAO,CAAE,OAAO,CAAC,KAAK,CAAC,MAAM,EAAE,CAAC;gBAEzC,IAAI,OAAO,GAAG,IAAI,CAAC,SAAS,CAAC,EAAC,IAAI,EAAE,EAAE,EAAC,CAAC,CAAC;gBACzC,IAAI,UAAU,GAAG;oBACf,OAAO,EAAE,EAAC,cAAc,EAAE,kBAAkB,EAAC;oBAC7C,IAAI,EAAE,OAAO;oBACb,MAAM,EAAE,MAAM;iBACf,CAAC;gBAEF,KAAK,CAAC,wBAAwB,EAAE,UAAU,CAAC;oBACzC,mDAAmD;qBAClD,IAAI,CAAC,QAAQ,GAAE,GAAC,OAAO,QAAQ,CAAC,IAAI,EAAE,GAAC,CAAC;oBACzC,wFAAwF;qBACvF,IAAI,CAAC,IAAI,GAAE,GAAC,OAAO,CAAC,GAAG,CAAE,IAAI,CAAC,CAAC,CAAC,KAAK,CAAC,IAAI,CAAC,GAAC,CAAC,CAAC;YAEnD,CAAC;SACF,CAAC,CAAC;IACL,CAAC;CACF,CAAC;AAGF;;GAEG;AACH,iEAAe,MAAM,EAAC",
+    "file": "lib_index_js.ec2676ba3debe7eaf44f.js",
+    "mappings": ";;;;;;;;;;;;;;;;;AACwD;AACG;AAE3D;;GAEG;AACH,MAAM,MAAM,GAAgC;IAC1C,EAAE,EAAE,oCAAoC;IACxC,WAAW,EACT,+EAA+E;IACjF,SAAS,EAAE,IAAI;IACf,QAAQ,EAAE,CAAC,kEAAgB,CAAC;IAC5B,QAAQ,EAAE,CAAC,GAAoB,EAAE,eAAiC,EAAE,EAAE;QACpE,oBAAoB;QACpB,MAAM,EAAE,QAAQ,EAAE,GAAG,GAAG,CAAC;QACzB,MAAM,OAAO,GAAG,qBAAqB,CAAC;QACtC,IAAI,OAAa,CAAC;QAClB,eAAe,CAAC,cAAc,CAAC,OAAO,CAAC,CAAC,OAAO,EAAE,KAAK,EAAE,EAAE;YACxD,OAAO,GAAG,KAAK;QACjB,CAAC,CAAC;QAEF,gBAAgB;QAChB,QAAQ,CAAC,UAAU,CAAC,OAAO,EAAE;YAC3B,KAAK,EAAE,oBAAoB;YAC3B,IAAI,EAAE,qEAAc;YACpB,SAAS,EAAE,oBAAoB;YAC/B,OAAO,EAAE,iCAAiC;YAC1C,OAAO,EAAE,CAAC,IAAS,EAAE,EAAE;gBACrB,IAAI,EAAE,GAAG,OAAO,aAAP,OAAO,uBAAP,OAAO,CAAE,OAAO,CAAC,KAAK,CAAC,MAAM,EAAE,CAAC;gBAEzC,IAAI,OAAO,GAAG,IAAI,CAAC,SAAS,CAAC,EAAC,IAAI,EAAE,EAAE,EAAC,CAAC,CAAC;gBACzC,IAAI,UAAU,GAAG;oBACf,OAAO,EAAE,EAAC,cAAc,EAAE,kBAAkB,EAAC;oBAC7C,IAAI,EAAE,OAAO;oBACb,MAAM,EAAE,MAAM;iBACf,CAAC;gBAEF,KAAK,CAAC,wBAAwB,EAAE,UAAU,CAAC;oBACzC,mDAAmD;qBAClD,IAAI,CAAC,QAAQ,GAAE,GAAC,OAAO,QAAQ,CAAC,IAAI,EAAE,GAAC,CAAC;oBACzC,wFAAwF;qBACvF,IAAI,CAAC,IAAI,GAAE,GAAC,OAAO,CAAC,GAAG,CAAE,IAAI,CAAC,CAAC,CAAC,KAAK,CAAC,IAAI,CAAC,GAAC,CAAC,CAAC;YAEnD,CAAC;SACF,CAAC,CAAC;IACL,CAAC;CACF,CAAC;AAGF;;GAEG;AACH,iEAAe,MAAM,EAAC",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://@otter-submit/submit-button/./src/index.ts"
     ],
     "sourcesContent": [
-        "import { JupyterFrontEndPlugin, JupyterFrontEnd } from '@jupyterlab/application';\nimport { INotebookTracker } from '@jupyterlab/notebook';\n\n/**\n * The plugin registration information.\n */\nconst plugin: JupyterFrontEndPlugin<void> = {\n  id: '@otter-submit/submit-button:plugin',\n  description:\n    'A JupyterLab extension used to submit notebooks for grading to otter-service.',\n  autoStart: true,\n  requires: [INotebookTracker],\n  activate: (app: JupyterFrontEnd, notebookTracker: INotebookTracker) => {\n    // Nothing is needed\n    const { commands } = app;\n    const command = 'otter-submit:submit';\n    var nbpanel : any;\n    notebookTracker.currentChanged.connect((tracker, panel) => {\n      nbpanel = panel\n    })\n\n    // Add a command\n    commands.addCommand(command, {\n      label: \"Submit for Grading\",\n      caption: 'Send your notebook to be graded',\n      execute: (args: any) => {\n        var nb = nbpanel?.context.model.toJSON();\n\n        var payload = JSON.stringify({'nb': nb});\n        var otherParam = {\n          headers: {\"Content-Type\": \"application/json\"},\n          body: payload,\n          method: \"POST\"\n        };\n        \n        fetch('/services/otter_grade/', otherParam)\n          // processes the response (in this case grabs text)\n          .then(response=>{return response.text()})\n          // processes the output of previous line (calling it data, then doing something with it)\n          .then(data=>{console.log( data); alert(data)});\n\n      }\n    });\n  }\n};\n\n\n/**\n * Export the plugin as default.\n */\nexport default plugin;\n"
+        "import { JupyterFrontEndPlugin, JupyterFrontEnd } from '@jupyterlab/application';\nimport { INotebookTracker } from '@jupyterlab/notebook';\nimport { fileUploadIcon } from '@jupyterlab/ui-components';\n\n/**\n * The plugin registration information.\n */\nconst plugin: JupyterFrontEndPlugin<void> = {\n  id: '@otter-submit/submit-button:plugin',\n  description:\n    'A JupyterLab extension used to submit notebooks for grading to otter-service.',\n  autoStart: true,\n  requires: [INotebookTracker],\n  activate: (app: JupyterFrontEnd, notebookTracker: INotebookTracker) => {\n    // Nothing is needed\n    const { commands } = app;\n    const command = 'otter-submit:submit';\n    var nbpanel : any;\n    notebookTracker.currentChanged.connect((tracker, panel) => {\n      nbpanel = panel\n    })\n\n    // Add a command\n    commands.addCommand(command, {\n      label: \"Submit for Grading\",\n      icon: fileUploadIcon,\n      iconLabel: \"Submit for Grading\",\n      caption: 'Send your notebook to be graded',\n      execute: (args: any) => {\n        var nb = nbpanel?.context.model.toJSON();\n\n        var payload = JSON.stringify({'nb': nb});\n        var otherParam = {\n          headers: {\"Content-Type\": \"application/json\"},\n          body: payload,\n          method: \"POST\"\n        };\n        \n        fetch('/services/otter_grade/', otherParam)\n          // processes the response (in this case grabs text)\n          .then(response=>{return response.text()})\n          // processes the output of previous line (calling it data, then doing something with it)\n          .then(data=>{console.log( data); alert(data)});\n\n      }\n    });\n  }\n};\n\n\n/**\n * Export the plugin as default.\n */\nexport default plugin;\n"
     ],
     "version": 3
 }
```

### Comparing `otter_submit-0.1.1/otter_submit/labextension/static/remoteEntry.a0746d0f3a3846491d76.js` & `otter_submit-0.1.2/otter_submit/labextension/static/remoteEntry.edecc40756fbdb50f74b.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -182,15 +182,15 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_index_js": "a552738018af89d94a0d",
+                "lib_index_js": "ec2676ba3debe7eaf44f",
                 "style_index_js": "eed68c68a11bc2d602a2"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
     /******/
@@ -427,15 +427,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("@otter-submit/submit-button", "0.1.1", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("@otter-submit/submit-button", "0.1.2", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -828,24 +828,28 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 4, 0, 3]))
+            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 4, 0, 3])),
+            /******/
+            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 4, 0, 3]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "lib_index_js": [
                 /******/
-                "webpack/sharing/consume/default/@jupyterlab/notebook"
+                "webpack/sharing/consume/default/@jupyterlab/notebook",
+                /******/
+                "webpack/sharing/consume/default/@jupyterlab/ui-components"
                 /******/
             ]
             /******/
         };
         /******/
         __webpack_require__.f.consumes = (chunkId, promises) => {
             /******/
@@ -1072,8 +1076,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/@otter-submit/submit-button");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["@otter-submit/submit-button"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.a0746d0f3a3846491d76.js.map
+//# sourceMappingURL=remoteEntry.edecc40756fbdb50f74b.js.map
```

### Comparing `otter_submit-0.1.1/otter_submit/labextension/static/remoteEntry.a0746d0f3a3846491d76.js.map` & `otter_submit-0.1.2/otter_submit/labextension/static/remoteEntry.edecc40756fbdb50f74b.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8367346938775511%*

 * *Differences: {"'file'": "'remoteEntry.edecc40756fbdb50f74b.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.a0746d0f3a3846491d76.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,8EAA8E;WAC5G;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC1KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
+    "file": "remoteEntry.edecc40756fbdb50f74b.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,8EAA8E;WAC5G;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC5KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://@otter-submit/submit-button/webpack/container-entry",
         "webpack://@otter-submit/submit-button/webpack/bootstrap",
         "webpack://@otter-submit/submit-button/webpack/runtime/compat get default export",
         "webpack://@otter-submit/submit-button/webpack/runtime/define property getters",
@@ -25,22 +25,22 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn __webpack_require__.e(\"style_index_js\").then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"a552738018af89d94a0d\",\"style_index_js\":\"eed68c68a11bc2d602a2\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"ec2676ba3debe7eaf44f\",\"style_index_js\":\"eed68c68a11bc2d602a2\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"@otter-submit/submit-button:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"@otter-submit/submit-button\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@otter-submit/submit-button\", \"0.1.1\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"@otter-submit/submit-button\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@otter-submit/submit-button\", \"0.1.2\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,4,0,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,4,0,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,0,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"@otter-submit/submit-button\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunk_otter_submit_submit_button\"] = self[\"webpackChunk_otter_submit_submit_button\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/@otter-submit/submit-button\");\n",
         ""
     ],
     "version": 3
```

### Comparing `otter_submit-0.1.1/otter_submit/labextension/static/style_index_js.eed68c68a11bc2d602a2.js` & `otter_submit-0.1.2/otter_submit/labextension/static/style_index_js.eed68c68a11bc2d602a2.js`

 * *Files identical despite different names*

### Comparing `otter_submit-0.1.1/otter_submit/labextension/static/style_index_js.eed68c68a11bc2d602a2.js.map` & `otter_submit-0.1.2/otter_submit/labextension/static/style_index_js.eed68c68a11bc2d602a2.js.map`

 * *Files identical despite different names*

### Comparing `otter_submit-0.1.1/src/index.ts` & `otter_submit-0.1.2/src/index.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import { JupyterFrontEndPlugin, JupyterFrontEnd } from '@jupyterlab/application';
 import { INotebookTracker } from '@jupyterlab/notebook';
+import { fileUploadIcon } from '@jupyterlab/ui-components';
 
 /**
  * The plugin registration information.
  */
 const plugin: JupyterFrontEndPlugin<void> = {
   id: '@otter-submit/submit-button:plugin',
   description:
@@ -18,14 +19,16 @@
     notebookTracker.currentChanged.connect((tracker, panel) => {
       nbpanel = panel
     })
 
     // Add a command
     commands.addCommand(command, {
       label: "Submit for Grading",
+      icon: fileUploadIcon,
+      iconLabel: "Submit for Grading",
       caption: 'Send your notebook to be graded',
       execute: (args: any) => {
         var nb = nbpanel?.context.model.toJSON();
 
         var payload = JSON.stringify({'nb': nb});
         var otherParam = {
           headers: {"Content-Type": "application/json"},
```

### Comparing `otter_submit-0.1.1/.gitignore` & `otter_submit-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `otter_submit-0.1.1/LICENSE` & `otter_submit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `otter_submit-0.1.1/pyproject.toml` & `otter_submit-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `otter_submit-0.1.1/PKG-INFO` & `otter_submit-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter_submit
-Version: 0.1.1
+Version: 0.1.2
 Summary: A JupyterLab extension used to submit notebooks for grading to otter-service.
 Project-URL: Homepage, https://github.com/data-8/otter-submit
 Project-URL: Bug Tracker, https://github.com/data-8/otter-submit/issues
 Project-URL: Repository, https://github.com/jupyterlab/extension-examples.git
 Author: Project Jupyter Contributors
 License: BSD-3-Clause License
 License-File: LICENSE
@@ -26,14 +26,14 @@
 # Otter Submit
 
 This JupyterLab extension places a "Submit" button in the Jupyter Notebook header. The submit button is used to submit a notebook to otter-service for grading.
 
 ## Development
 Create your environment however you like:
 - mamba create -n otter-submit -c conda-forge python==3.11
-- mamba activate otter-submit
+- conda activate otter-submit
 
 Make changes and run these commands:
 - python3 -m pip install -ve .
 - jlpm run build
 - jupyter lab
```

