# Comparing `tmp/telemetry_router-0.1.11.tar.gz` & `tmp/telemetry_router-0.1.9.tar.gz`

## Comparing `telemetry_router-0.1.11.tar` & `telemetry_router-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/.copier-answers.yml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/CHANGELOG.md
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/RELEASE.md
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/install.json
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/tsconfig.json
--rw-r--r--   0        0        0   221121 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/yarn.lock
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/jupyter-config/nb-config/telemetry_router.json
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/jupyter-config/server-config/telemetry_router.json
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/src/consumer.ts
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/src/handler.ts
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/src/index.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/style/index.js
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/telemetry_router/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/telemetry_router/_version.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/telemetry_router/application.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/telemetry_router/handlers.py
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/telemetry_router/labextension/package.json
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/telemetry_router/labextension/static/0.392de5078e6b617e0d18.js
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/telemetry_router/labextension/static/747.3ba83e0acd2b381f34b2.js
--rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/telemetry_router/labextension/static/remoteEntry.29f9dbdee8943f528a7b.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/telemetry_router/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/telemetry_router/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/.gitignore
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/LICENSE
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/README.md
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/pyproject.toml
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 telemetry_router-0.1.11/PKG-INFO
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/.copier-answers.yml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/RELEASE.md
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/install.json
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/tsconfig.json
+-rw-r--r--   0        0        0   220879 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/yarn.lock
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/jupyter-config/nb-config/telemetry_router.json
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/jupyter-config/server-config/telemetry_router.json
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/src/handler.ts
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/src/index.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/style/index.js
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/telemetry_router/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/telemetry_router/_version.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/telemetry_router/application.py
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/telemetry_router/handlers.py
+-rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/telemetry_router/labextension/package.json
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/telemetry_router/labextension/static/747.3ba83e0acd2b381f34b2.js
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/telemetry_router/labextension/static/763.7fc2a1794f2943f4acb5.js
+-rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/telemetry_router/labextension/static/remoteEntry.07a29c704af1bfd3164a.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/telemetry_router/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/telemetry_router/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/README.md
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 telemetry_router-0.1.9/PKG-INFO
```

### Comparing `telemetry_router-0.1.11/RELEASE.md` & `telemetry_router-0.1.9/RELEASE.md`

 * *Files identical despite different names*

### Comparing `telemetry_router-0.1.11/package.json` & `telemetry_router-0.1.9/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'0.1.9'"}*

```diff
@@ -188,9 +188,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.11"
+    "version": "0.1.9"
 }
```

### Comparing `telemetry_router-0.1.11/tsconfig.json` & `telemetry_router-0.1.9/tsconfig.json`

 * *Files identical despite different names*

### Comparing `telemetry_router-0.1.11/yarn.lock` & `telemetry_router-0.1.9/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1207,159 +1207,159 @@
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: e834bcc5c0dee3eecb5362b3f10187e80908b6a293ebacf5750547a64b57ec710a068497334f109ecf4e5ea05e09e7e9c00e48ebbd30050673ea67b0929e5398
   languageName: node
   linkType: hard
 
-"@lumino/algorithm@npm:^2.0.0, @lumino/algorithm@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@lumino/algorithm@npm:2.0.1"
-  checksum: cbf7fcf6ee6b785ea502cdfddc53d61f9d353dcb9659343511d5cd4b4030be2ff2ca4c08daec42f84417ab0318a3d9972a17319fa5231693e109ab112dcf8000
+"@lumino/algorithm@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "@lumino/algorithm@npm:2.0.0"
+  checksum: 663edf536e94397b449c6a2643a735e602fbb396dec86b56ad1193a768dce27c6e7da5ad0384aa90086ea44cbb64dde3f9d565e9fd81858f1eb0c6b4253f3b94
   languageName: node
   linkType: hard
 
 "@lumino/application@npm:^2.1.1":
-  version: 2.2.1
-  resolution: "@lumino/application@npm:2.2.1"
+  version: 2.2.0
+  resolution: "@lumino/application@npm:2.2.0"
   dependencies:
-    "@lumino/commands": ^2.1.3
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/widgets": ^2.3.0
-  checksum: a33e661703728440bc7d2ddb4674261f4de0d20eb8c9846646cbd6debac03b5c65e78d739a500903550fd83b8f47b47fa82ec178c97bc9967ca3ac4014075cde
+    "@lumino/commands": ^2.1.2
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/widgets": ^2.2.0
+  checksum: b62da44b21d110c5d3478a49549326974b59325b8c60a58905d8e5ef08210273cd013cb60387d1f082fb79377a230278e2cf63e345491b0a54c75fdcc6164a68
   languageName: node
   linkType: hard
 
-"@lumino/collections@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@lumino/collections@npm:2.0.1"
+"@lumino/collections@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "@lumino/collections@npm:2.0.0"
   dependencies:
-    "@lumino/algorithm": ^2.0.1
-  checksum: 8a29b7973a388a33c5beda0819dcd2dc2aad51a8406dcfd4581b055a9f77a39dc5800f7a8b4ae3c0bb97ae7b56a7a869e2560ffb7a920a28e93b477ba05907d6
+    "@lumino/algorithm": ^2.0.0
+  checksum: 4a7fc3571e92a1368a1ef01300ad7b6e0d4ff13cb78b89533d5962eea66d4a7550e15d8b80fa3ab1816b1a89382f35015f9dddf72ab04654c17e5b516b845d8f
   languageName: node
   linkType: hard
 
-"@lumino/commands@npm:^2.1.1, @lumino/commands@npm:^2.1.3":
-  version: 2.1.3
-  resolution: "@lumino/commands@npm:2.1.3"
+"@lumino/commands@npm:^2.1.1, @lumino/commands@npm:^2.1.2":
+  version: 2.1.2
+  resolution: "@lumino/commands@npm:2.1.2"
   dependencies:
-    "@lumino/algorithm": ^2.0.1
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/domutils": ^2.0.1
-    "@lumino/keyboard": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    "@lumino/virtualdom": ^2.0.1
-  checksum: e4e3ee279f2a5e8d68e4ce142c880333f5542f90c684972402356936ecb5cf5e07163800b59e7cb8c911cbdb4e5089edcc5dd2990bc8db10c87517268de1fc5d
+    "@lumino/algorithm": ^2.0.0
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+    "@lumino/domutils": ^2.0.0
+    "@lumino/keyboard": ^2.0.0
+    "@lumino/signaling": ^2.1.1
+    "@lumino/virtualdom": ^2.0.0
+  checksum: c0b5ce8c5e1a86a98a90f54bb07b74742748110cf3362b86ff8328c1b5475c4dc05f1c4c9f50bf79e51c4e2ddc5cd69d6194f3d39dd5b58f357b0f30758bf35b
   languageName: node
   linkType: hard
 
-"@lumino/coreutils@npm:^1.11.0 || ^2.0.0, @lumino/coreutils@npm:^1.11.0 || ^2.1.1, @lumino/coreutils@npm:^2.1.1, @lumino/coreutils@npm:^2.1.2":
-  version: 2.1.2
-  resolution: "@lumino/coreutils@npm:2.1.2"
-  checksum: 7865317ac0676b448d108eb57ab5d8b2a17c101995c0f7a7106662d9fe6c859570104525f83ee3cda12ae2e326803372206d6f4c1f415a5b59e4158a7b81066f
+"@lumino/coreutils@npm:^1.11.0 || ^2.0.0, @lumino/coreutils@npm:^1.11.0 || ^2.1.1, @lumino/coreutils@npm:^2.1.1":
+  version: 2.1.1
+  resolution: "@lumino/coreutils@npm:2.1.1"
+  checksum: dfdeb2b0282caae17b6c3edfebadf4ce7c75fc879fa60cacfef9b154412f4b35e4ffd95b1833b99d8dacb99aaaa04513570129ae2024c3f33e2677a01f0576ce
   languageName: node
   linkType: hard
 
-"@lumino/disposable@npm:^1.10.0 || ^2.0.0, @lumino/disposable@npm:^2.1.1, @lumino/disposable@npm:^2.1.2":
-  version: 2.1.2
-  resolution: "@lumino/disposable@npm:2.1.2"
+"@lumino/disposable@npm:^1.10.0 || ^2.0.0, @lumino/disposable@npm:^2.1.1":
+  version: 2.1.1
+  resolution: "@lumino/disposable@npm:2.1.1"
   dependencies:
-    "@lumino/signaling": ^2.1.2
-  checksum: ac2fb2bf18d0b2939fda454f3db248a0ff6e8a77b401e586d1caa9293b3318f808b93a117c9c3ac27cd17aab545aea83b49108d099b9b2f5503ae2a012fbc6e2
+    "@lumino/signaling": ^2.1.1
+  checksum: ed6cdfe13f3346178a087690d4e7baeccaed7e73ca23cb239765202409f5c01b4729a4058b4717f963462ee9ef2e5cb14ad1974e3163741267290edc3715c85c
   languageName: node
   linkType: hard
 
-"@lumino/domutils@npm:^2.0.0, @lumino/domutils@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@lumino/domutils@npm:2.0.1"
-  checksum: 61fa0ab226869dfbb763fc426790cf5a43b7d6f4cea1364c6dd56d61c44bff05eea188d33ff847449608ef58ed343161bee15c19b96f35410e4ee35815dc611a
+"@lumino/domutils@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "@lumino/domutils@npm:2.0.0"
+  checksum: 4a146bfc1006d5fd00ccecc61d9803965d269c15c48c892fd87216336ce967f0db91f31203c5616c83d260224cddf25af4abb6704a6770757d19e44068f690bf
   languageName: node
   linkType: hard
 
-"@lumino/dragdrop@npm:^2.1.1, @lumino/dragdrop@npm:^2.1.3":
-  version: 2.1.3
-  resolution: "@lumino/dragdrop@npm:2.1.3"
+"@lumino/dragdrop@npm:^2.1.1, @lumino/dragdrop@npm:^2.1.2":
+  version: 2.1.2
+  resolution: "@lumino/dragdrop@npm:2.1.2"
   dependencies:
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-  checksum: d5f7eb4cc9f9a084cb9af10f02d6741b25d683350878ecbc324e24ba9d4b5246451a410e2ca5fff227aab1c191d1e73a2faf431f93e13111d67a4e426e126258
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+  checksum: 7ac64ec11423ec89fea937aa6c9ca818933ee98e775e500018a0a948f32171932033a1e302a48395cbe9bfeaa635acde2393fd935db14d7b1d569ca6a1daaa77
   languageName: node
   linkType: hard
 
-"@lumino/keyboard@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@lumino/keyboard@npm:2.0.1"
-  checksum: cf33f13427a418efd7cc91061233321e860d5404f3d86397781028309bef86c8ad2d88276ffe335c1db0fe619bd9d1e60641c81f881696957a58703ee4652c3e
+"@lumino/keyboard@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "@lumino/keyboard@npm:2.0.0"
+  checksum: 3852ba51f437b1c1d7e552a0f844592a05e04dd5012070dc6e4384c58965d1ebf536c6875c1b7bae03cde3c715ddc36cd290992fcefc1a8c39094194f4689fdd
   languageName: node
   linkType: hard
 
-"@lumino/messaging@npm:^2.0.0, @lumino/messaging@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@lumino/messaging@npm:2.0.1"
+"@lumino/messaging@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "@lumino/messaging@npm:2.0.0"
   dependencies:
-    "@lumino/algorithm": ^2.0.1
-    "@lumino/collections": ^2.0.1
-  checksum: 964c4651c374b17452b4252b7d71500b32d2ecd87c192fc5bcf5d3bd1070661d78d07edcac8eca7d1d6fd50aa25992505485e1296d6dd995691b8e349b652045
+    "@lumino/algorithm": ^2.0.0
+    "@lumino/collections": ^2.0.0
+  checksum: 1e82dcf9b110834d4342dc63dfeac0ee780880fb99051bd82d00a1f83afd91b276c1cea5af85a414d92c527adc365d54f20ec780123b562f89c5a2cd3e96bf81
   languageName: node
   linkType: hard
 
 "@lumino/polling@npm:^2.1.1":
-  version: 2.1.2
-  resolution: "@lumino/polling@npm:2.1.2"
+  version: 2.1.1
+  resolution: "@lumino/polling@npm:2.1.1"
   dependencies:
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/signaling": ^2.1.2
-  checksum: fa9b401e6dbeb8f31d7e3ba485e8ef1e0c92b3f2da086239c0ed49931026f5d3528709193c93e031e35ac624fb4bbbfcdcbaa0e25eb797f36e2952e5cd91e9e3
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+    "@lumino/signaling": ^2.1.1
+  checksum: 69177b26d5fc541e72533cbe7d7f7999eea541d392f1082d20dbd9e1797e7d46fba47bae9c65c06f9ccb2780cbae636e9354d9bf4423b5e1020754d4b07d4f6b
   languageName: node
   linkType: hard
 
-"@lumino/properties@npm:^2.0.0, @lumino/properties@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@lumino/properties@npm:2.0.1"
-  checksum: c50173a935148cc4148fdaea119df1d323ee004ae16ab666800388d27e9730345629662d85f25591683329b39f0cdae60ee8c94e8943b4d0ef7d7370a38128d6
+"@lumino/properties@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "@lumino/properties@npm:2.0.0"
+  checksum: 81187a11a779eed4e20ff0035e77dee99bd271b0cf649096c4e8809dd6bdd06955b1a974bc1a115e536f8d2840b30183bb78a362b2c6991824477df6d17e6c59
   languageName: node
   linkType: hard
 
-"@lumino/signaling@npm:^1.10.0 || ^2.0.0, @lumino/signaling@npm:^2.1.1, @lumino/signaling@npm:^2.1.2":
-  version: 2.1.2
-  resolution: "@lumino/signaling@npm:2.1.2"
+"@lumino/signaling@npm:^1.10.0 || ^2.0.0, @lumino/signaling@npm:^2.1.1":
+  version: 2.1.1
+  resolution: "@lumino/signaling@npm:2.1.1"
   dependencies:
-    "@lumino/algorithm": ^2.0.1
-    "@lumino/coreutils": ^2.1.2
-  checksum: ad7d7153db57980da899c43e412e6130316ef30b231a70250e7af49058db16cadb018c1417a2ea8083d83c48623cfe6b705fa82bf10216b1a8949aed9f4aca4e
+    "@lumino/algorithm": ^2.0.0
+    "@lumino/coreutils": ^2.1.1
+  checksum: 283ad4239b8577f68aca3d0b2606f73cc1c775f84cab25cf49aa6cd195f0d87949ef43fdff03b38b5a49ebbf2468581c6786d5f8b6159a04b2051260be5eab86
   languageName: node
   linkType: hard
 
-"@lumino/virtualdom@npm:^2.0.0, @lumino/virtualdom@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@lumino/virtualdom@npm:2.0.1"
+"@lumino/virtualdom@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "@lumino/virtualdom@npm:2.0.0"
   dependencies:
-    "@lumino/algorithm": ^2.0.1
-  checksum: cf59b6f15b430e13e9e657b7a0619b9056cd9ea7b2a87f407391d071c501b77403c302b6a66dca510382045e75b2e3fe551630bb391f1c6b33678057d4bec164
+    "@lumino/algorithm": ^2.0.0
+  checksum: 6fc1d88e7d4a656be7664ccfc5745eb1d4e3d2034db0b11ad6abefcc642f22d265003eef0e1d02bca2e42b6da127123118c631369006f78e88a08885a6f36c25
   languageName: node
   linkType: hard
 
-"@lumino/widgets@npm:^1.37.2 || ^2.1.1, @lumino/widgets@npm:^2.1.1, @lumino/widgets@npm:^2.3.0":
-  version: 2.3.0
-  resolution: "@lumino/widgets@npm:2.3.0"
+"@lumino/widgets@npm:^1.37.2 || ^2.1.1, @lumino/widgets@npm:^2.1.1, @lumino/widgets@npm:^2.2.0":
+  version: 2.2.0
+  resolution: "@lumino/widgets@npm:2.2.0"
   dependencies:
-    "@lumino/algorithm": ^2.0.1
-    "@lumino/commands": ^2.1.3
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/domutils": ^2.0.1
-    "@lumino/dragdrop": ^2.1.3
-    "@lumino/keyboard": ^2.0.1
-    "@lumino/messaging": ^2.0.1
-    "@lumino/properties": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    "@lumino/virtualdom": ^2.0.1
-  checksum: a8559bd3574b7fc16e7679e05994c515b0d3e78dada35786d161f67c639941d134e92ce31d95c2e4ac06709cdf83b0e7fb4b6414a3f7779579222a2fb525d025
+    "@lumino/algorithm": ^2.0.0
+    "@lumino/commands": ^2.1.2
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/disposable": ^2.1.1
+    "@lumino/domutils": ^2.0.0
+    "@lumino/dragdrop": ^2.1.2
+    "@lumino/keyboard": ^2.0.0
+    "@lumino/messaging": ^2.0.0
+    "@lumino/properties": ^2.0.0
+    "@lumino/signaling": ^2.1.1
+    "@lumino/virtualdom": ^2.0.0
+  checksum: 963c0e54102b786a9cbf3467041c9f6f5c275af751afc311ebeba30d56516767c463c425e321bb389eaa66726dfc4420119a9a58573dcbf3110aba9515c80606
   languageName: node
   linkType: hard
 
 "@nodelib/fs.scandir@npm:2.1.5":
   version: 2.1.5
   resolution: "@nodelib/fs.scandir@npm:2.1.5"
   dependencies:
@@ -1490,21 +1490,21 @@
   version: 15.7.5
   resolution: "@types/prop-types@npm:15.7.5"
   checksum: 5b43b8b15415e1f298243165f1d44390403bb2bd42e662bca3b5b5633fdd39c938e91b7fce3a9483699db0f7a715d08cef220c121f723a634972fdf596aec980
   languageName: node
   linkType: hard
 
 "@types/react@npm:^18.0.26":
-  version: 18.2.17
-  resolution: "@types/react@npm:18.2.17"
+  version: 18.2.16
+  resolution: "@types/react@npm:18.2.16"
   dependencies:
     "@types/prop-types": "*"
     "@types/scheduler": "*"
     csstype: ^3.0.2
-  checksum: 150516b31bd98b635e4a56bcf2af007330b35cccb6e35e902f46a47f0e81e30c46cdacc095e91051bdf2f33e4846e7e62fd51b67e064dc7d15c00e15dfa449d5
+  checksum: 3d4fdc12509e0098e0dbb4bacdea53e8ccc6632e9df63d9f2711c77aa81ce3b2bb9c76d087f284034b25fd7245680167f4832bf6e4df960c5af2634b52adfd0c
   languageName: node
   linkType: hard
 
 "@types/scheduler@npm:*":
   version: 0.16.3
   resolution: "@types/scheduler@npm:0.16.3"
   checksum: 2b0aec39c24268e3ce938c5db2f2e77f5c3dd280e05c262d9c2fe7d890929e4632a6b8e94334017b66b45e4f92a5aa42ba3356640c2a1175fa37bef2f5200767
@@ -2571,17 +2571,17 @@
     lodash: ^4.17.4
     semver: ^5.4.1
   checksum: d77be45cb72d79a429c64d8f8f7603fea681d182fb795459a3d4afa608faad9a923378a7e80c6855f465263e1983140b6fc3682bd0213228b8cd7906ab4b934d
   languageName: node
   linkType: hard
 
 "electron-to-chromium@npm:^1.4.431":
-  version: 1.4.474
-  resolution: "electron-to-chromium@npm:1.4.474"
-  checksum: 16e55823064dfa6f64088a3d5124c0c5c2a577c981a35e58199a2baa6a237b4d9505ddf406d4c8761cabdf6f7b347013a57a887883781dfb04d1940f8be379b0
+  version: 1.4.471
+  resolution: "electron-to-chromium@npm:1.4.471"
+  checksum: c62ac1f2e9e0395b3095899c7d07a723611a6ca9bc754935101f9f659d7fc3f564f4e47cacb5639abdc172265db041923679942c72055fc8d6522e1b57f755df
   languageName: node
   linkType: hard
 
 "emoji-regex@npm:^8.0.0":
   version: 8.0.0
   resolution: "emoji-regex@npm:8.0.0"
   checksum: d4c5c39d5a9868b5fa152f00cada8a936868fd3367f33f71be515ecee4c803132d11b31a6222b2571b1e5f7e13890156a94880345594d0ce7e3c9895f560f192
@@ -2724,21 +2724,21 @@
   version: 4.0.0
   resolution: "escape-string-regexp@npm:4.0.0"
   checksum: 98b48897d93060f2322108bf29db0feba7dd774be96cd069458d1453347b25ce8682ecc39859d4bca2203cc0ab19c237bcc71755eff49a0f8d90beadeeba5cc5
   languageName: node
   linkType: hard
 
 "eslint-config-prettier@npm:^8.8.0":
-  version: 8.9.0
-  resolution: "eslint-config-prettier@npm:8.9.0"
+  version: 8.8.0
+  resolution: "eslint-config-prettier@npm:8.8.0"
   peerDependencies:
     eslint: ">=7.0.0"
   bin:
     eslint-config-prettier: bin/cli.js
-  checksum: a675d0dabd76b700ef2d062b5ec6a634e105a8e8c070f95281fd2ccb614527fac60b4c758132058c50f0521fd19313f1f5be45ce9ebf081f2e5f77ae6eb7d8db
+  checksum: 1e94c3882c4d5e41e1dcfa2c368dbccbfe3134f6ac7d40101644d3bfbe3eb2f2ffac757f3145910b5eacf20c0e85e02b91293d3126d770cbf3dc390b3564681c
   languageName: node
   linkType: hard
 
 "eslint-plugin-prettier@npm:^5.0.0":
   version: 5.0.0
   resolution: "eslint-plugin-prettier@npm:5.0.0"
   dependencies:
@@ -2902,27 +2902,27 @@
     signal-exit: ^3.0.3
     strip-final-newline: ^2.0.0
   checksum: fba9022c8c8c15ed862847e94c252b3d946036d7547af310e344a527e59021fd8b6bb0723883ea87044dc4f0201f949046993124a42ccb0855cae5bf8c786343
   languageName: node
   linkType: hard
 
 "execa@npm:^7.1.1":
-  version: 7.2.0
-  resolution: "execa@npm:7.2.0"
+  version: 7.1.1
+  resolution: "execa@npm:7.1.1"
   dependencies:
     cross-spawn: ^7.0.3
     get-stream: ^6.0.1
     human-signals: ^4.3.0
     is-stream: ^3.0.0
     merge-stream: ^2.0.0
     npm-run-path: ^5.1.0
     onetime: ^6.0.0
     signal-exit: ^3.0.7
     strip-final-newline: ^3.0.0
-  checksum: 14fd17ba0ca8c87b277584d93b1d9fc24f2a65e5152b31d5eb159a3b814854283eaae5f51efa9525e304447e2f757c691877f7adff8fde5746aae67eb1edd1cc
+  checksum: 21fa46fc69314ace4068cf820142bdde5b643a5d89831c2c9349479c1555bff137a291b8e749e7efca36535e4e0a8c772c11008ca2e84d2cbd6ca141a3c8f937
   languageName: node
   linkType: hard
 
 "fast-deep-equal@npm:^3.1.1, fast-deep-equal@npm:^3.1.3":
   version: 3.1.3
   resolution: "fast-deep-equal@npm:3.1.3"
   checksum: e21a9d8d84f53493b6aa15efc9cfd53dd5b714a1f23f67fb5dc8f574af80df889b3bce25dc081887c6d25457cce704e636395333abad896ccdec03abaf1f3f9d
@@ -5498,22 +5498,22 @@
   peerDependencies:
     stylelint: ^15.10.0
   checksum: 536249800c04b48a9c354067765f042713982e8222be17bb897a27d26546e50adfb87e6f1e4541807d720de3554345da99ab470e13e8d7ab0ab326c73ae3df61
   languageName: node
   linkType: hard
 
 "stylelint-prettier@npm:^4.0.0":
-  version: 4.0.1
-  resolution: "stylelint-prettier@npm:4.0.1"
+  version: 4.0.0
+  resolution: "stylelint-prettier@npm:4.0.0"
   dependencies:
     prettier-linter-helpers: ^1.0.0
   peerDependencies:
     prettier: ">=3.0.0"
     stylelint: ">=15.8.0"
-  checksum: 25d38f0f0c5fd9687b8f4f1a48db1da8a697c5b5fa6e26971c2825ba9166e15d376a2a0d9344aa485ef2a0c2c3b476a1da81f17608eff6f474523771e55ba523
+  checksum: 3e7cff833e30b1eab9ae6e82f1b0a3596fd3dd214489d71d37b0899e677ae9d50cc74c4c1bbb3b1275903f03c1401b2ca6f8c1cf2631108363d3e7845d7b6300
   languageName: node
   linkType: hard
 
 "stylelint@npm:^15.10.1":
   version: 15.10.2
   resolution: "stylelint@npm:15.10.2"
   dependencies:
```

### Comparing `telemetry_router-0.1.11/src/handler.ts` & `telemetry_router-0.1.9/src/handler.ts`

 * *Files identical despite different names*

### Comparing `telemetry_router-0.1.11/src/index.ts` & `telemetry_router-0.1.9/src/index.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin,
 } from '@jupyterlab/application';
 
+import { requestAPI } from './handler'
+
 import { NotebookPanel } from '@jupyterlab/notebook';
 
 import { INotebookContent } from '@jupyterlab/nbformat';
 
 import { Token } from '@lumino/coreutils';
 
-import { Consumer, ConsoleLogger, MongoDBLogger } from './consumer';
-
-import { requestAPI } from './handler';
-
 const PLUGIN_ID = 'telemetry-router:plugin';
 
 export const ITelemetryRouter = new Token<ITelemetryRouter>(PLUGIN_ID)
 
 export interface ITelemetryRouter {
   loadNotebookPanel(notebookPanel: NotebookPanel): void;
-  publishEvent(event: Object): void;
+  consumeEventSignal(data: Object): void;
 }
 
 export class TelemetryRouter implements ITelemetryRouter {
   private sessionID?: string;
-  private sequence: number = 0;
+  private sequence: number;
   private notebookPanel?: NotebookPanel;
 
-  static registeredConsumers: Consumer[] = [];
-  static registerConsumer(consumer: Consumer) {
-    TelemetryRouter.registeredConsumers.push(consumer);
+  constructor() {
+    this.sequence = 0;
   }
 
   loadNotebookPanel(notebookPanel: NotebookPanel) {
     this.notebookPanel = notebookPanel
   }
 
-  async publishEvent(event: Object) {
+  async consumeEventSignal(event: Object) {
     // Check if session id received is equal to the stored session id &
     // Update sequence number accordingly
     if (this.sessionID === this.notebookPanel?.sessionContext.session?.id)
       this.sequence = this.sequence + 1
     else {
       this.sessionID = this.notebookPanel?.sessionContext.session?.id
       this.sequence = 0
@@ -54,34 +51,30 @@
         sessionID: this.sessionID,
         sequence: this.sequence,
         notebookPath: this.notebookPanel?.context.path,
         notebookContent: this.notebookPanel?.model?.toJSON() as INotebookContent
       },
     }
 
-    // Send to consumer
-    TelemetryRouter.registeredConsumers.forEach(consumer => {
-      consumer.consume(log);
-    });
+    // Post to database
+    console.log("Request", log)
+
+    let responseMongo = await requestAPI<any>('mongo', { method: 'POST', body: JSON.stringify(log) });
+
+    console.log('Response', responseMongo);
   }
 }
 
 const plugin: JupyterFrontEndPlugin<TelemetryRouter> = {
   id: PLUGIN_ID,
   description: 'A JupyterLab extension.',
   provides: ITelemetryRouter,
   autoStart: true,
-  activate: async (app: JupyterFrontEnd) => {
-    const version = await requestAPI<string>('version')
-    console.log(`${PLUGIN_ID}: ${version}`)
+  activate: (app: JupyterFrontEnd) => {
+    console.log('JupyterLab extension telemetry-router is activated!')
 
     const telemetryRouter = new TelemetryRouter()
-
-    // Register consumers for the router
-    new ConsoleLogger();
-    new MongoDBLogger();
-
     return telemetryRouter;
   }
 };
 
 export default plugin;
```

### Comparing `telemetry_router-0.1.11/telemetry_router/__init__.py` & `telemetry_router-0.1.9/telemetry_router/__init__.py`

 * *Files identical despite different names*

### Comparing `telemetry_router-0.1.11/telemetry_router/application.py` & `telemetry_router-0.1.9/telemetry_router/application.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 from jupyter_server.extension.application import ExtensionApp
 from traitlets import Unicode, Bool, Int
 
 class TelemetryRouterApp(ExtensionApp):
 
     name = "telemetry_router"
 
-    api = Unicode("").tag(config=True)
+    api_telemetry_url = Unicode("").tag(config=True)
     mongo_cluster = Unicode("").tag(config=True)
     mongo_db = Unicode("").tag(config=True)
     mongo_collection = Unicode("").tag(config=True)
 
     telemetry = Bool(None, allow_none=True).tag(config=True)
     save_interval = Int(10, allow_none=False).tag(config=True)
     
     def initialize_settings(self):
         try:
-            assert self.api, "The c.TelemetryRouterApp.api configuration setting must be set."
+            assert self.api_telemetry_url, "The c.TelemetryRouterApp.api_telemetry_url configuration setting must be set."
             assert self.mongo_cluster, "The c.TelemetryRouterApp.mongo_cluster configuration setting must be set."
 
-            self.api = self.api.strip()
+            self.api_telemetry_url = self.api_telemetry_url.strip()
             self.mongo_cluster = self.mongo_cluster.strip()
             self.mongo_db = self.mongo_db.strip()
             self.mongo_collection = self.mongo_collection.strip()
 
             if self.telemetry is None:
                 self.telemetry = False
```

### Comparing `telemetry_router-0.1.11/telemetry_router/handlers.py` & `telemetry_router-0.1.9/telemetry_router/handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,28 +13,33 @@
         super().__init__(*args, **kwargs)
 
     # The following decorator should be present on all verb methods (head, get, post,
     # patch, put, delete, options) to ensure only authorized user can request the
     # Jupyter server
     @tornado.web.authenticated
     def get(self, resource):
-        try:
-            self.set_header('Content-Type', 'application/json') 
-            if resource == 'version':
-                self.finish(json.dumps(__version__))
-            elif resource == 'env':
-                self.finish(json.dumps({
-                    'workspaceID': os.getenv('WORKSPACE_ID') if os.getenv('WORKSPACE_ID') is not None else 'UNDEFINED'
-                    }))
-            else:
-                self.set_status(404)
-        except Exception as e:
-            self.log.error(str(e))
-            self.set_status(500)
-            self.finish(json.dumps(str(e)))
+        pass
+        # try:
+        #     self.set_header('Content-Type', 'application/json')
+
+        #     if resource == 'config':
+        #         self.finish(json.dumps({
+        #             'telemetry' : self.extensionapp.telemetry,
+        #             'capture_notebook_events': self.extensionapp.capture_notebook_events,
+        #             'save_interval': self.extensionapp.save_interval,
+        #             'version':  __version__,
+        #             'workspace_id': os.getenv('WORKSPACE_ID') if os.getenv('WORKSPACE_ID') is not None else 'UNDEFINED'
+        #             }))
+        #     else:
+        #         self.set_status(404)
+
+        # except Exception as e:
+        #     self.log.error(str(e))
+        #     self.set_status(500)
+        #     self.finish(json.dumps(str(e)))
 
     @tornado.web.authenticated
     @tornado.gen.coroutine
     def post(self, resource):
         try:
             if resource == 'mongo':
 
@@ -64,15 +69,15 @@
             'log': log,
             'mongo_params': mongo_params
         })
 
         with Session() as s:
             req = Request(
                 'POST',
-                self.extensionapp.api + "/mongo",
+                self.extensionapp.api_telemetry_url + "/mongo",
                 data=data,
                 headers={
                     'content-type': 'application/json'
                     }
                 )
 
             prepped = s.prepare_request(req)
```

### Comparing `telemetry_router-0.1.11/telemetry_router/labextension/package.json` & `telemetry_router-0.1.9/telemetry_router/labextension/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9795833333333333%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.07a29c704af1bfd3164a.js'}}",*

 * * "'version'": "'0.1.9'"}*

```diff
@@ -103,15 +103,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/educational-technology-collective/telemetry-router",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.29f9dbdee8943f528a7b.js",
+            "load": "static/remoteEntry.07a29c704af1bfd3164a.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "telemetry_router"
                 },
@@ -193,9 +193,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.11"
+    "version": "0.1.9"
 }
```

### Comparing `telemetry_router-0.1.11/telemetry_router/labextension/static/0.392de5078e6b617e0d18.js` & `telemetry_router-0.1.9/telemetry_router/labextension/static/763.7fc2a1794f2943f4acb5.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,105 +1,67 @@
 "use strict";
 (self.webpackChunktelemetry_router = self.webpackChunktelemetry_router || []).push([
-    [0],
-    [(e, o, s) => {
-        s.r(o), s.d(o, {
-            ITelemetryRouter: () => d,
-            TelemetryRouter: () => h,
-            default: () => v
-        });
-        var t = s(930),
-            n = s(987),
-            r = s(790);
-        async function i(e = "", o = {}) {
-            const s = r.ServerConnection.makeSettings(),
-                t = n.URLExt.join(s.baseUrl, "telemetry-router", e);
-            let i;
-            try {
-                i = await r.ServerConnection.makeRequest(t, o, s)
-            } catch (e) {
-                throw new r.ServerConnection.NetworkError(e)
-            }
-            let c = await i.text();
-            if (c.length > 0) try {
-                c = JSON.parse(c)
-            } catch (e) {
-                console.log("Not a JSON response body.", i)
-            }
-            if (!i.ok) throw new r.ServerConnection.ResponseError(i, c.message || c);
-            return c
-        }
-        class c {
-            constructor() {
-                h.registerConsumer(this)
-            }
-            consume(e) {
-                console.log("Base", e)
-            }
-        }
-        class l extends c {
-            constructor() {
-                super()
-            }
-            consume(e) {
-                console.log("ConsoleLogger", e)
-            }
-        }
-        class u extends c {
-            constructor() {
-                super()
-            }
-            async consume(e) {
-                const o = {
-                    request: e,
-                    response: await i("mongo", {
+    [763], {
+        763: (e, o, t) => {
+            t.r(o), t.d(o, {
+                ITelemetryRouter: () => r,
+                TelemetryRouter: () => l,
+                default: () => a
+            });
+            var n = t(987),
+                s = t(790);
+            const i = "telemetry-router:plugin",
+                r = new(t(930).Token)(i);
+            class l {
+                constructor() {
+                    this.sequence = 0
+                }
+                loadNotebookPanel(e) {
+                    this.notebookPanel = e
+                }
+                async consumeEventSignal(e) {
+                    var o, t, i, r, l, a, c;
+                    this.sessionID === (null === (t = null === (o = this.notebookPanel) || void 0 === o ? void 0 : o.sessionContext.session) || void 0 === t ? void 0 : t.id) ? this.sequence = this.sequence + 1 : (this.sessionID = null === (r = null === (i = this.notebookPanel) || void 0 === i ? void 0 : i.sessionContext.session) || void 0 === r ? void 0 : r.id, this.sequence = 0);
+                    const u = {
+                        event: e,
+                        notebookState: {
+                            sessionID: this.sessionID,
+                            sequence: this.sequence,
+                            notebookPath: null === (l = this.notebookPanel) || void 0 === l ? void 0 : l.context.path,
+                            notebookContent: null === (c = null === (a = this.notebookPanel) || void 0 === a ? void 0 : a.model) || void 0 === c ? void 0 : c.toJSON()
+                        }
+                    };
+                    console.log("Request", u);
+                    let d = await async function(e = "", o = {}) {
+                        const t = s.ServerConnection.makeSettings(),
+                            i = n.URLExt.join(t.baseUrl, "telemetry-router", e);
+                        let r;
+                        try {
+                            r = await s.ServerConnection.makeRequest(i, o, t)
+                        } catch (e) {
+                            throw new s.ServerConnection.NetworkError(e)
+                        }
+                        let l = await r.text();
+                        if (l.length > 0) try {
+                            l = JSON.parse(l)
+                        } catch (e) {
+                            console.log("Not a JSON response body.", r)
+                        }
+                        if (!r.ok) throw new s.ServerConnection.ResponseError(r, l.message || l);
+                        return l
+                    }("mongo", {
                         method: "POST",
-                        body: JSON.stringify(e)
-                    })
-                };
-                console.log("MongoDBLogger", o)
-            }
-        }
-        const a = "telemetry-router:plugin",
-            d = new t.Token(a);
-        class h {
-            constructor() {
-                this.sequence = 0
-            }
-            static registerConsumer(e) {
-                h.registeredConsumers.push(e)
-            }
-            loadNotebookPanel(e) {
-                this.notebookPanel = e
-            }
-            async publishEvent(e) {
-                var o, s, t, n, r, i, c;
-                this.sessionID === (null === (s = null === (o = this.notebookPanel) || void 0 === o ? void 0 : o.sessionContext.session) || void 0 === s ? void 0 : s.id) ? this.sequence = this.sequence + 1 : (this.sessionID = null === (n = null === (t = this.notebookPanel) || void 0 === t ? void 0 : t.sessionContext.session) || void 0 === n ? void 0 : n.id, this.sequence = 0);
-                const l = {
-                    event: e,
-                    notebookState: {
-                        sessionID: this.sessionID,
-                        sequence: this.sequence,
-                        notebookPath: null === (r = this.notebookPanel) || void 0 === r ? void 0 : r.context.path,
-                        notebookContent: null === (c = null === (i = this.notebookPanel) || void 0 === i ? void 0 : i.model) || void 0 === c ? void 0 : c.toJSON()
-                    }
-                };
-                h.registeredConsumers.forEach((e => {
-                    e.consume(l)
-                }))
-            }
-        }
-        h.registeredConsumers = [];
-        const v = {
-            id: a,
-            description: "A JupyterLab extension.",
-            provides: d,
-            autoStart: !0,
-            activate: async e => {
-                const o = await i("version");
-                console.log(`${a}: ${o}`);
-                const s = new h;
-                return new l, new u, s
+                        body: JSON.stringify(u)
+                    });
+                    console.log("Response", d)
+                }
+            }
+            const a = {
+                id: i,
+                description: "A JupyterLab extension.",
+                provides: r,
+                autoStart: !0,
+                activate: e => (console.log("JupyterLab extension telemetry-router is activated!"), new l)
             }
         }
-    }]
+    }
 ]);
```

### Comparing `telemetry_router-0.1.11/telemetry_router/labextension/static/747.3ba83e0acd2b381f34b2.js` & `telemetry_router-0.1.9/telemetry_router/labextension/static/747.3ba83e0acd2b381f34b2.js`

 * *Files identical despite different names*

### Comparing `telemetry_router-0.1.11/telemetry_router/labextension/static/remoteEntry.29f9dbdee8943f528a7b.js` & `telemetry_router-0.1.9/telemetry_router/labextension/static/remoteEntry.07a29c704af1bfd3164a.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, o, a, i, u, l, s, f, d, c, p, h, v, m = {
             827: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(0).then((() => () => t(0))),
-                        "./extension": () => t.e(0).then((() => () => t(0))),
+                        "./index": () => t.e(763).then((() => () => t(763))),
+                        "./extension": () => t.e(763).then((() => () => t(763))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -43,19 +43,19 @@
         }), r
     }, g.d = (e, r) => {
         for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + "." + {
-        0: "392de5078e6b617e0d18",
-        747: "3ba83e0acd2b381f34b2"
+        747: "3ba83e0acd2b381f34b2",
+        763: "7fc2a1794f2943f4acb5"
     } [e] + ".js?v=" + {
-        0: "392de5078e6b617e0d18",
-        747: "3ba83e0acd2b381f34b2"
+        747: "3ba83e0acd2b381f34b2",
+        763: "7fc2a1794f2943f4acb5"
     } [e], g.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -102,19 +102,19 @@
                 var a = g.S[t],
                     i = "telemetry-router",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => g.e(0).then((() => () => g(0))),
+                        get: () => g.e(763).then((() => () => g(763))),
                         from: i,
                         eager: !1
                     })
-                })("telemetry-router", "0.1.11"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("telemetry-router", "0.1.9"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         g.g.importScripts && (e = g.g.location + "");
         var r = g.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -212,15 +212,15 @@
         var a = g.I(r);
         return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), p = {}, h = {
         790: () => c("default", "@jupyterlab/services", [1, 7, 0, 3]),
         930: () => c("default", "@lumino/coreutils", [1, 2, 0, 0]),
         987: () => c("default", "@jupyterlab/coreutils", [1, 6, 0, 3])
     }, v = {
-        0: [790, 930, 987]
+        763: [790, 930, 987]
     }, g.f.consumes = (e, r) => {
         g.o(v, e) && v[e].forEach((e => {
             if (g.o(p, e)) return r.push(p[e]);
             var t = r => {
                     p[e] = 0, g.m[e] = t => {
                         delete g.c[e], t.exports = r()
                     }
```

### Comparing `telemetry_router-0.1.11/telemetry_router/labextension/static/third-party-licenses.json` & `telemetry_router-0.1.9/telemetry_router/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `telemetry_router-0.1.11/.gitignore` & `telemetry_router-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `telemetry_router-0.1.11/LICENSE` & `telemetry_router-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `telemetry_router-0.1.11/README.md` & `telemetry_router-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `telemetry_router-0.1.11/pyproject.toml` & `telemetry_router-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `telemetry_router-0.1.11/PKG-INFO` & `telemetry_router-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telemetry_router
-Version: 0.1.11
+Version: 0.1.9
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/educational-technology-collective/telemetry-router
 Project-URL: Bug Tracker, https://github.com/educational-technology-collective/telemetry-router/issues
 Project-URL: Repository, https://github.com/educational-technology-collective/telemetry-router.git
 Author-email: mengyanw <mengyanw@umich.edu>
 License: BSD 3-Clause License
```

