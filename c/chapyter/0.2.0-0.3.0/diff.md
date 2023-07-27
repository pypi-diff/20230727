# Comparing `tmp/chapyter-0.2.0.tar.gz` & `tmp/chapyter-0.3.0.tar.gz`

## Comparing `chapyter-0.2.0.tar` & `chapyter-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,33 @@
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 chapyter-0.2.0/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 chapyter-0.2.0/.yarnrc.yml
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 chapyter-0.2.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 chapyter-0.2.0/babel.config.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 chapyter-0.2.0/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 chapyter-0.2.0/jest.config.js
--rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 chapyter-0.2.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 chapyter-0.2.0/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 chapyter-0.2.0/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 chapyter-0.2.0/tsconfig.test.json
--rw-r--r--   0        0        0   362904 2020-02-02 00:00:00.000000 chapyter-0.2.0/yarn.lock
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 chapyter-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 chapyter-0.2.0/chapyter/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 chapyter-0.2.0/chapyter/_version.py
--rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 chapyter-0.2.0/chapyter/magic.py
--rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 chapyter-0.2.0/chapyter/programs.py
--rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 chapyter-0.2.0/chapyter/labextension/package.json
--rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 chapyter-0.2.0/chapyter/labextension/schemas/@shannon-shen/chapyter/package.json.orig
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 chapyter-0.2.0/chapyter/labextension/static/568.0a4b756444d1e43aa84c.js
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 chapyter-0.2.0/chapyter/labextension/static/747.217e756827eb66a6f3d4.js
--rw-r--r--   0        0        0     6961 2020-02-02 00:00:00.000000 chapyter-0.2.0/chapyter/labextension/static/remoteEntry.d053f9dc5154f37a9b90.js
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 chapyter-0.2.0/chapyter/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 chapyter-0.2.0/chapyter/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0   842385 2020-02-02 00:00:00.000000 chapyter-0.2.0/examples/chapyter-starter.png
--rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 chapyter-0.2.0/examples/starter-Copy1.ipynb
--rw-r--r--   0        0        0    13814 2020-02-02 00:00:00.000000 chapyter-0.2.0/examples/starter-Copy2.ipynb
--rw-r--r--   0        0        0    22135 2020-02-02 00:00:00.000000 chapyter-0.2.0/examples/starter-Copy3.ipynb
--rw-r--r--   0        0        0    12211 2020-02-02 00:00:00.000000 chapyter-0.2.0/examples/starter.ipynb
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 chapyter-0.2.0/src/index.ts
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 chapyter-0.2.0/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 chapyter-0.2.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 chapyter-0.2.0/style/index.js
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 chapyter-0.2.0/.gitignore
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 chapyter-0.2.0/LICENSE
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 chapyter-0.2.0/README.md
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 chapyter-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 chapyter-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 chapyter-0.3.0/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 chapyter-0.3.0/.yarnrc.yml
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 chapyter-0.3.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 chapyter-0.3.0/babel.config.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 chapyter-0.3.0/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 chapyter-0.3.0/jest.config.js
+-rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 chapyter-0.3.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 chapyter-0.3.0/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 chapyter-0.3.0/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 chapyter-0.3.0/tsconfig.test.json
+-rw-r--r--   0        0        0   364822 2020-02-02 00:00:00.000000 chapyter-0.3.0/yarn.lock
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/_version.py
+-rw-r--r--   0        0        0    12863 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/magic.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/programs.py
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/labextension/package.json
+-rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/labextension/schemas/@shannon-shen/chapyter/package.json.orig
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/labextension/static/568.630c95d80cb75b8352da.js
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/labextension/static/747.217e756827eb66a6f3d4.js
+-rw-r--r--   0        0        0     6961 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/labextension/static/remoteEntry.674ce065681604c8f0d3.js
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 chapyter-0.3.0/chapyter/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    12382 2020-02-02 00:00:00.000000 chapyter-0.3.0/examples/01-quick-start.ipynb
+-rw-r--r--   0        0        0    12599 2020-02-02 00:00:00.000000 chapyter-0.3.0/examples/02-configure-chapyter.ipynb
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 chapyter-0.3.0/src/index.ts
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 chapyter-0.3.0/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 chapyter-0.3.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 chapyter-0.3.0/style/index.js
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 chapyter-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 chapyter-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 chapyter-0.3.0/README.md
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 chapyter-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 chapyter-0.3.0/PKG-INFO
```

### Comparing `chapyter-0.2.0/RELEASE.md` & `chapyter-0.3.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `chapyter-0.2.0/jest.config.js` & `chapyter-0.3.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `chapyter-0.2.0/package.json` & `chapyter-0.3.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'0.3.0'"}*

```diff
@@ -182,12 +182,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0",
+    "version": "0.3.0",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `chapyter-0.2.0/tsconfig.json` & `chapyter-0.3.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `chapyter-0.2.0/yarn.lock` & `chapyter-0.3.0/yarn.lock`

 * *Files 2% similar despite different names*

```diff
@@ -27,53 +27,53 @@
   resolution: "@babel/code-frame@npm:7.22.5"
   dependencies:
     "@babel/highlight": ^7.22.5
   checksum: cfe804f518f53faaf9a1d3e0f9f74127ab9a004912c3a16fda07fb6a633393ecb9918a053cb71804204c1b7ec3d49e1699604715e2cfb0c9f7bc4933d324ebb6
   languageName: node
   linkType: hard
 
-"@babel/compat-data@npm:^7.22.5, @babel/compat-data@npm:^7.22.6":
-  version: 7.22.6
-  resolution: "@babel/compat-data@npm:7.22.6"
-  checksum: b88631143a2ebdb75e5bac47984e950983294f1739c2133f32569c6f2fcee85f83634bb6cf4378afb44fa8eb7877d11e48811d1e6a52afa161f82276ffdc3fb4
+"@babel/compat-data@npm:^7.22.5, @babel/compat-data@npm:^7.22.6, @babel/compat-data@npm:^7.22.9":
+  version: 7.22.9
+  resolution: "@babel/compat-data@npm:7.22.9"
+  checksum: bed77d9044ce948b4327b30dd0de0779fa9f3a7ed1f2d31638714ed00229fa71fc4d1617ae0eb1fad419338d3658d0e9a5a083297451e09e73e078d0347ff808
   languageName: node
   linkType: hard
 
 "@babel/core@npm:^7.10.2, @babel/core@npm:^7.11.6, @babel/core@npm:^7.12.3":
-  version: 7.22.8
-  resolution: "@babel/core@npm:7.22.8"
+  version: 7.22.9
+  resolution: "@babel/core@npm:7.22.9"
   dependencies:
     "@ampproject/remapping": ^2.2.0
     "@babel/code-frame": ^7.22.5
-    "@babel/generator": ^7.22.7
-    "@babel/helper-compilation-targets": ^7.22.6
-    "@babel/helper-module-transforms": ^7.22.5
+    "@babel/generator": ^7.22.9
+    "@babel/helper-compilation-targets": ^7.22.9
+    "@babel/helper-module-transforms": ^7.22.9
     "@babel/helpers": ^7.22.6
     "@babel/parser": ^7.22.7
     "@babel/template": ^7.22.5
     "@babel/traverse": ^7.22.8
     "@babel/types": ^7.22.5
-    "@nicolo-ribaudo/semver-v6": ^6.3.3
     convert-source-map: ^1.7.0
     debug: ^4.1.0
     gensync: ^1.0.0-beta.2
     json5: ^2.2.2
-  checksum: 75ed701c14ad17070382ae1dd166f7534b31f2c71e00995a5f261ee2398ee96335b0736573b8ff24ab6e3e6f5814ee2a48fa11ab90fabcd3dfc70ea87c5f30a6
+    semver: ^6.3.1
+  checksum: 7bf069aeceb417902c4efdaefab1f7b94adb7dea694a9aed1bda2edf4135348a080820529b1a300c6f8605740a00ca00c19b2d5e74b5dd489d99d8c11d5e56d1
   languageName: node
   linkType: hard
 
-"@babel/generator@npm:^7.22.7, @babel/generator@npm:^7.7.2":
-  version: 7.22.7
-  resolution: "@babel/generator@npm:7.22.7"
+"@babel/generator@npm:^7.22.7, @babel/generator@npm:^7.22.9, @babel/generator@npm:^7.7.2":
+  version: 7.22.9
+  resolution: "@babel/generator@npm:7.22.9"
   dependencies:
     "@babel/types": ^7.22.5
     "@jridgewell/gen-mapping": ^0.3.2
     "@jridgewell/trace-mapping": ^0.3.17
     jsesc: ^2.5.1
-  checksum: cee15558888bdf5564e19cfaf95101b2910fa425f30cc1a25ac9b8621bd62b63544eb1b36ad89c80b5e41915699219f78712cab128d1f7e3da6a21fbf4143927
+  checksum: 7c9d2c58b8d5ac5e047421a6ab03ec2ff5d9a5ff2c2212130a0055e063ac349e0b19d435537d6886c999771aef394832e4f54cd9fc810100a7f23d982f6af06b
   languageName: node
   linkType: hard
 
 "@babel/helper-annotate-as-pure@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-annotate-as-pure@npm:7.22.5"
   dependencies:
@@ -87,73 +87,73 @@
   resolution: "@babel/helper-builder-binary-assignment-operator-visitor@npm:7.22.5"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: d753acac62399fc6dd354cf1b9441bde0c331c2fe792a4c14904c5e5eafc3cac79478f6aa038e8a51c1148b0af6710a2e619855e4b5d54497ac972eaffed5884
   languageName: node
   linkType: hard
 
-"@babel/helper-compilation-targets@npm:^7.22.5, @babel/helper-compilation-targets@npm:^7.22.6":
-  version: 7.22.6
-  resolution: "@babel/helper-compilation-targets@npm:7.22.6"
+"@babel/helper-compilation-targets@npm:^7.22.5, @babel/helper-compilation-targets@npm:^7.22.6, @babel/helper-compilation-targets@npm:^7.22.9":
+  version: 7.22.9
+  resolution: "@babel/helper-compilation-targets@npm:7.22.9"
   dependencies:
-    "@babel/compat-data": ^7.22.6
+    "@babel/compat-data": ^7.22.9
     "@babel/helper-validator-option": ^7.22.5
-    "@nicolo-ribaudo/semver-v6": ^6.3.3
     browserslist: ^4.21.9
     lru-cache: ^5.1.1
+    semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: c7788c48099c4f0edf2adeb367a941a930d39ed7453140ceb10d7114c4091922adf56d3cdd832050fd4501f25e872886390629042ddd365d3bce2ecad69ed394
+  checksum: ea0006c6a93759025f4a35a25228ae260538c9f15023e8aac2a6d45ca68aef4cf86cfc429b19af9a402cbdd54d5de74ad3fbcf6baa7e48184dc079f1a791e178
   languageName: node
   linkType: hard
 
 "@babel/helper-create-class-features-plugin@npm:^7.22.5":
-  version: 7.22.6
-  resolution: "@babel/helper-create-class-features-plugin@npm:7.22.6"
+  version: 7.22.9
+  resolution: "@babel/helper-create-class-features-plugin@npm:7.22.9"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
     "@babel/helper-environment-visitor": ^7.22.5
     "@babel/helper-function-name": ^7.22.5
     "@babel/helper-member-expression-to-functions": ^7.22.5
     "@babel/helper-optimise-call-expression": ^7.22.5
-    "@babel/helper-replace-supers": ^7.22.5
+    "@babel/helper-replace-supers": ^7.22.9
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
     "@babel/helper-split-export-declaration": ^7.22.6
-    "@nicolo-ribaudo/semver-v6": ^6.3.3
+    semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: 10412e8a509a607cde6137288d3f12b1f91acd374e29e6dd6a277b67217e9f4c932a0acd89eeda837c8432916df775a8af6321aeb8d8b131ccdbf7688208dda1
+  checksum: 6c2436d1a5a3f1ff24628d78fa8c6d3120c40285aa3eda7815b1adbf8c5951e0dd73d368cf845825888fa3dc2f207dadce53309825598d7c67953e5ed9dd51d2
   languageName: node
   linkType: hard
 
 "@babel/helper-create-regexp-features-plugin@npm:^7.18.6, @babel/helper-create-regexp-features-plugin@npm:^7.22.5":
-  version: 7.22.6
-  resolution: "@babel/helper-create-regexp-features-plugin@npm:7.22.6"
+  version: 7.22.9
+  resolution: "@babel/helper-create-regexp-features-plugin@npm:7.22.9"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
-    "@nicolo-ribaudo/semver-v6": ^6.3.3
     regexpu-core: ^5.3.1
+    semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: a26df33a08bc603177cc4a59d067740bd7156c05d6b519bf28cdd2f07f653be2a7f37d8dd93b85e620f20ad90da1b8dbe4d7c6cf5262e67f713904e811b7ffd2
+  checksum: 87cb48a7ee898ab205374274364c3adc70b87b08c7bd07f51019ae4562c0170d7148e654d591f825dee14b5fe11666a0e7966872dfdbfa0d1b94b861ecf0e4e1
   languageName: node
   linkType: hard
 
-"@babel/helper-define-polyfill-provider@npm:^0.4.1":
-  version: 0.4.1
-  resolution: "@babel/helper-define-polyfill-provider@npm:0.4.1"
+"@babel/helper-define-polyfill-provider@npm:^0.4.2":
+  version: 0.4.2
+  resolution: "@babel/helper-define-polyfill-provider@npm:0.4.2"
   dependencies:
     "@babel/helper-compilation-targets": ^7.22.6
     "@babel/helper-plugin-utils": ^7.22.5
     debug: ^4.1.1
     lodash.debounce: ^4.0.8
     resolve: ^1.14.2
   peerDependencies:
-    "@babel/core": ^7.4.0-0
-  checksum: 712b440cdd343ac7c4617225f91b0a9db5a7b1c96356b720e011af64ad6c4da9c66889f8d2962a0a2ae2e4ccb6a9b4a210c4a3c8c8ff103846b3d93b61bc6634
+    "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
+  checksum: 1f6dec0c5d0876d278fe15b71238eccc5f74c4e2efa2c78aaafa8bc2cc96336b8e68d94cd1a78497356c96e8b91b8c1f4452179820624d1702aee2f9832e6569
   languageName: node
   linkType: hard
 
 "@babel/helper-environment-visitor@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-environment-visitor@npm:7.22.5"
   checksum: 248532077d732a34cd0844eb7b078ff917c3a8ec81a7f133593f71a860a582f05b60f818dc5049c2212e5baa12289c27889a4b81d56ef409b4863db49646c4b1
@@ -193,27 +193,26 @@
   resolution: "@babel/helper-module-imports@npm:7.22.5"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: 9ac2b0404fa38b80bdf2653fbeaf8e8a43ccb41bd505f9741d820ed95d3c4e037c62a1bcdcb6c9527d7798d2e595924c4d025daed73283badc180ada2c9c49ad
   languageName: node
   linkType: hard
 
-"@babel/helper-module-transforms@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/helper-module-transforms@npm:7.22.5"
+"@babel/helper-module-transforms@npm:^7.22.5, @babel/helper-module-transforms@npm:^7.22.9":
+  version: 7.22.9
+  resolution: "@babel/helper-module-transforms@npm:7.22.9"
   dependencies:
     "@babel/helper-environment-visitor": ^7.22.5
     "@babel/helper-module-imports": ^7.22.5
     "@babel/helper-simple-access": ^7.22.5
-    "@babel/helper-split-export-declaration": ^7.22.5
+    "@babel/helper-split-export-declaration": ^7.22.6
     "@babel/helper-validator-identifier": ^7.22.5
-    "@babel/template": ^7.22.5
-    "@babel/traverse": ^7.22.5
-    "@babel/types": ^7.22.5
-  checksum: 8985dc0d971fd17c467e8b84fe0f50f3dd8610e33b6c86e5b3ca8e8859f9448bcc5c84e08a2a14285ef388351c0484797081c8f05a03770bf44fc27bf4900e68
+  peerDependencies:
+    "@babel/core": ^7.0.0
+  checksum: 2751f77660518cf4ff027514d6f4794f04598c6393be7b04b8e46c6e21606e11c19f3f57ab6129a9c21bacdf8b3ffe3af87bb401d972f34af2d0ffde02ac3001
   languageName: node
   linkType: hard
 
 "@babel/helper-optimise-call-expression@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-optimise-call-expression@npm:7.22.5"
   dependencies:
@@ -226,38 +225,36 @@
   version: 7.22.5
   resolution: "@babel/helper-plugin-utils@npm:7.22.5"
   checksum: c0fc7227076b6041acd2f0e818145d2e8c41968cc52fb5ca70eed48e21b8fe6dd88a0a91cbddf4951e33647336eb5ae184747ca706817ca3bef5e9e905151ff5
   languageName: node
   linkType: hard
 
 "@babel/helper-remap-async-to-generator@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/helper-remap-async-to-generator@npm:7.22.5"
+  version: 7.22.9
+  resolution: "@babel/helper-remap-async-to-generator@npm:7.22.9"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
     "@babel/helper-environment-visitor": ^7.22.5
-    "@babel/helper-wrap-function": ^7.22.5
-    "@babel/types": ^7.22.5
+    "@babel/helper-wrap-function": ^7.22.9
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: 1e51dcff1c22e97ea3d22034b77788048eb6d8c6860325bd7a1046b7a7135730cefd93b5c96fd9839d76031095d5ffb6f0cd6ee90a5d69a4c7de980d7f4623d9
+  checksum: 05538079447829b13512157491cc77f9cf1ea7e1680e15cff0682c3ed9ee162de0c4862ece20a6d6b2df28177a1520bcfe45993fbeccf2747a81795a7c3f6290
   languageName: node
   linkType: hard
 
-"@babel/helper-replace-supers@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/helper-replace-supers@npm:7.22.5"
+"@babel/helper-replace-supers@npm:^7.22.5, @babel/helper-replace-supers@npm:^7.22.9":
+  version: 7.22.9
+  resolution: "@babel/helper-replace-supers@npm:7.22.9"
   dependencies:
     "@babel/helper-environment-visitor": ^7.22.5
     "@babel/helper-member-expression-to-functions": ^7.22.5
     "@babel/helper-optimise-call-expression": ^7.22.5
-    "@babel/template": ^7.22.5
-    "@babel/traverse": ^7.22.5
-    "@babel/types": ^7.22.5
-  checksum: af29deff6c6dc3fa2d1a517390716aa3f4d329855e8689f1d5c3cb07c1b898e614a5e175f1826bb58e9ff1480e6552885a71a9a0ba5161787aaafa2c79b216cc
+  peerDependencies:
+    "@babel/core": ^7.0.0
+  checksum: d41471f56ff2616459d35a5df1900d5f0756ae78b1027040365325ef332d66e08e3be02a9489756d870887585ff222403a228546e93dd7019e19e59c0c0fe586
   languageName: node
   linkType: hard
 
 "@babel/helper-simple-access@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-simple-access@npm:7.22.5"
   dependencies:
@@ -271,15 +268,15 @@
   resolution: "@babel/helper-skip-transparent-expression-wrappers@npm:7.22.5"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: 1012ef2295eb12dc073f2b9edf3425661e9b8432a3387e62a8bc27c42963f1f216ab3124228015c748770b2257b4f1fda882ca8fa34c0bf485e929ae5bc45244
   languageName: node
   linkType: hard
 
-"@babel/helper-split-export-declaration@npm:^7.22.5, @babel/helper-split-export-declaration@npm:^7.22.6":
+"@babel/helper-split-export-declaration@npm:^7.22.6":
   version: 7.22.6
   resolution: "@babel/helper-split-export-declaration@npm:7.22.6"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: e141cace583b19d9195f9c2b8e17a3ae913b7ee9b8120246d0f9ca349ca6f03cb2c001fd5ec57488c544347c0bb584afec66c936511e447fd20a360e591ac921
   languageName: node
   linkType: hard
@@ -301,23 +298,22 @@
 "@babel/helper-validator-option@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-validator-option@npm:7.22.5"
   checksum: bbeca8a85ee86990215c0424997438b388b8d642d69b9f86c375a174d3cdeb270efafd1ff128bc7a1d370923d13b6e45829ba8581c027620e83e3a80c5c414b3
   languageName: node
   linkType: hard
 
-"@babel/helper-wrap-function@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/helper-wrap-function@npm:7.22.5"
+"@babel/helper-wrap-function@npm:^7.22.9":
+  version: 7.22.9
+  resolution: "@babel/helper-wrap-function@npm:7.22.9"
   dependencies:
     "@babel/helper-function-name": ^7.22.5
     "@babel/template": ^7.22.5
-    "@babel/traverse": ^7.22.5
     "@babel/types": ^7.22.5
-  checksum: a4ba2d7577ad3ce92fadaa341ffce3b0e4b389808099b07c80847f9be0852f4b42344612bc1b3d1b796ffb75be56d5957c5c56a1734f6aee5ccbb7cd9ab12691
+  checksum: 037317dc06dac6593e388738ae1d3e43193bc1d31698f067c0ef3d4dc6f074dbed860ed42aa137b48a67aa7cb87336826c4bdc13189260481bcf67eb7256c789
   languageName: node
   linkType: hard
 
 "@babel/helpers@npm:^7.22.6":
   version: 7.22.6
   resolution: "@babel/helpers@npm:7.22.6"
   dependencies:
@@ -1202,19 +1198,19 @@
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: c042070f980b139547f8b0179efbc049ac5930abec7fc26ed7a41d89a048d8ab17d362200e204b6f71c3c20d6991a0e74415e1a412a49adc8131c2a40c04822e
   languageName: node
   linkType: hard
 
 "@babel/preset-env@npm:^7.10.2":
-  version: 7.22.7
-  resolution: "@babel/preset-env@npm:7.22.7"
+  version: 7.22.9
+  resolution: "@babel/preset-env@npm:7.22.9"
   dependencies:
-    "@babel/compat-data": ^7.22.6
-    "@babel/helper-compilation-targets": ^7.22.6
+    "@babel/compat-data": ^7.22.9
+    "@babel/helper-compilation-targets": ^7.22.9
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/helper-validator-option": ^7.22.5
     "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression": ^7.22.5
     "@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining": ^7.22.5
     "@babel/plugin-proposal-private-property-in-object": 7.21.0-placeholder-for-preset-env.2
     "@babel/plugin-syntax-async-generators": ^7.8.4
     "@babel/plugin-syntax-class-properties": ^7.12.13
@@ -1280,37 +1276,37 @@
     "@babel/plugin-transform-typeof-symbol": ^7.22.5
     "@babel/plugin-transform-unicode-escapes": ^7.22.5
     "@babel/plugin-transform-unicode-property-regex": ^7.22.5
     "@babel/plugin-transform-unicode-regex": ^7.22.5
     "@babel/plugin-transform-unicode-sets-regex": ^7.22.5
     "@babel/preset-modules": ^0.1.5
     "@babel/types": ^7.22.5
-    "@nicolo-ribaudo/semver-v6": ^6.3.3
     babel-plugin-polyfill-corejs2: ^0.4.4
     babel-plugin-polyfill-corejs3: ^0.8.2
     babel-plugin-polyfill-regenerator: ^0.5.1
     core-js-compat: ^3.31.0
+    semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: eabde70e450dd54f57997b0f92317f69f268e9a1f85b13f5ef5540d2a38cfae5620bd8e48ddffb547c55fbd2f17673276e6eb9411d6b5fb82e3422faf44cb6cf
+  checksum: 6caa2897bbda30c6932aed0a03827deb1337c57108050c9f97dc9a857e1533c7125b168b6d70b9d191965bf05f9f233f0ad20303080505dff7ce39740aaa759d
   languageName: node
   linkType: hard
 
 "@babel/preset-modules@npm:^0.1.5":
-  version: 0.1.5
-  resolution: "@babel/preset-modules@npm:0.1.5"
+  version: 0.1.6
+  resolution: "@babel/preset-modules@npm:0.1.6"
   dependencies:
     "@babel/helper-plugin-utils": ^7.0.0
     "@babel/plugin-proposal-unicode-property-regex": ^7.4.4
     "@babel/plugin-transform-dotall-regex": ^7.4.4
     "@babel/types": ^7.4.4
     esutils: ^2.0.2
   peerDependencies:
-    "@babel/core": ^7.0.0-0
-  checksum: 8430e0e9e9d520b53e22e8c4c6a5a080a12b63af6eabe559c2310b187bd62ae113f3da82ba33e9d1d0f3230930ca702843aae9dd226dec51f7d7114dc1f51c10
+    "@babel/core": ^7.0.0-0 || ^8.0.0-0 <8.0.0
+  checksum: 9700992d2b9526e703ab49eb8c4cd0b26bec93594d57c6b808967619df1a387565e0e58829b65b5bd6d41049071ea0152c9195b39599515fddb3e52b09a55ff0
   languageName: node
   linkType: hard
 
 "@babel/regjsgen@npm:^0.8.0":
   version: 0.8.0
   resolution: "@babel/regjsgen@npm:0.8.0"
   checksum: 89c338fee774770e5a487382170711014d49a68eb281e74f2b5eac88f38300a4ad545516a7786a8dd5702e9cf009c94c2f582d200f077ac5decd74c56b973730
@@ -1333,15 +1329,15 @@
     "@babel/code-frame": ^7.22.5
     "@babel/parser": ^7.22.5
     "@babel/types": ^7.22.5
   checksum: c5746410164039aca61829cdb42e9a55410f43cace6f51ca443313f3d0bdfa9a5a330d0b0df73dc17ef885c72104234ae05efede37c1cc8a72dc9f93425977a3
   languageName: node
   linkType: hard
 
-"@babel/traverse@npm:^7.22.5, @babel/traverse@npm:^7.22.6, @babel/traverse@npm:^7.22.8":
+"@babel/traverse@npm:^7.22.6, @babel/traverse@npm:^7.22.8":
   version: 7.22.8
   resolution: "@babel/traverse@npm:7.22.8"
   dependencies:
     "@babel/code-frame": ^7.22.5
     "@babel/generator": ^7.22.7
     "@babel/helper-environment-visitor": ^7.22.5
     "@babel/helper-function-name": ^7.22.5
@@ -1370,27 +1366,27 @@
   version: 0.2.3
   resolution: "@bcoe/v8-coverage@npm:0.2.3"
   checksum: 850f9305536d0f2bd13e9e0881cb5f02e4f93fad1189f7b2d4bebf694e3206924eadee1068130d43c11b750efcc9405f88a8e42ef098b6d75239c0f047de1a27
   languageName: node
   linkType: hard
 
 "@codemirror/autocomplete@npm:^6.0.0, @codemirror/autocomplete@npm:^6.3.2, @codemirror/autocomplete@npm:^6.5.1, @codemirror/autocomplete@npm:^6.7.1":
-  version: 6.8.1
-  resolution: "@codemirror/autocomplete@npm:6.8.1"
+  version: 6.9.0
+  resolution: "@codemirror/autocomplete@npm:6.9.0"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.6.0
     "@lezer/common": ^1.0.0
   peerDependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
-  checksum: 8599cd91defa3fea5276a7f9aff43ced323d9c4401dfb867e43608ba72ded48cb458256c5c784949a6332c0c20ba2fedac16a5708335cd809d269e4ea5076957
+  checksum: a5f661944c75f40b02c90a193c9a459c0fd7e335c0ac5973420c19157dfb46010f573c2b70731591fe477e7a2ad10121ff3ae394a72d450946d7b886c28b0368
   languageName: node
   linkType: hard
 
 "@codemirror/commands@npm:^6.2.3":
   version: 6.2.4
   resolution: "@codemirror/commands@npm:6.2.4"
   dependencies:
@@ -1501,15 +1497,15 @@
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.0.0
     "@lezer/php": ^1.0.0
   checksum: c003a29a426486453fdfddbf7302982fa2aa7f059bf6f1ce4cbf08341b0162eee5e2f50e0d71c418dcd358491631780156d846fe352754d042576172c5d86721
   languageName: node
   linkType: hard
 
-"@codemirror/lang-python@npm:^6.1.2":
+"@codemirror/lang-python@npm:^6.1.3":
   version: 6.1.3
   resolution: "@codemirror/lang-python@npm:6.1.3"
   dependencies:
     "@codemirror/autocomplete": ^6.3.2
     "@codemirror/language": ^6.8.0
     "@lezer/python": ^1.1.4
   checksum: 65a0276a4503e4e3b70dd28d1c93ef472632b6d2c4bf3ae92d305d14ee8cf60b0bbbf62d5ceb51294de9598d9e2d42eafcde26f317ee7b90d0a11dfa863c1d1a
@@ -1574,19 +1570,19 @@
     "@lezer/lr": ^1.0.0
     style-mod: ^4.0.0
   checksum: 64408d996641931fa4c6b892e17ee1fdaee0f63d3d84c019a6ea7b1e6d1c774f92357b95c2ebaed60545062b795b72d0a058c03578b2bf4023c87726e97b5d2f
   languageName: node
   linkType: hard
 
 "@codemirror/legacy-modes@npm:^6.3.2":
-  version: 6.3.2
-  resolution: "@codemirror/legacy-modes@npm:6.3.2"
+  version: 6.3.3
+  resolution: "@codemirror/legacy-modes@npm:6.3.3"
   dependencies:
     "@codemirror/language": ^6.0.0
-  checksum: fa5f5477fb9e19267251e2ecd3de8c1a4c2512813555bb60111dce3951f2c3f6080a2985a573b7542534ba1d2c34115f7e39ee23fdf8f6f81db6f8ce447c1efc
+  checksum: 3cd32b0f011b0a193e0948e5901b625f38aa6d9a8b24344531d6e142eb6fbb3e6cb5969429102044f3d04fbe53c4deaebd9f659c05067a0b18d17766290c9e05
   languageName: node
   linkType: hard
 
 "@codemirror/lint@npm:^6.0.0":
   version: 6.4.0
   resolution: "@codemirror/lint@npm:6.4.0"
   dependencies:
@@ -1612,21 +1608,21 @@
   version: 6.2.1
   resolution: "@codemirror/state@npm:6.2.1"
   checksum: d12a321d0471b264b9d3259042bff913a8b939e8d28d408ff452004538a71ca9d5329df3f8a1d8a9183f5b42a7ef5b200737bcab1065714f5ae8e0a5ba9d59d3
   languageName: node
   linkType: hard
 
 "@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.2.2, @codemirror/view@npm:^6.6.0, @codemirror/view@npm:^6.9.6":
-  version: 6.14.1
-  resolution: "@codemirror/view@npm:6.14.1"
+  version: 6.15.3
+  resolution: "@codemirror/view@npm:6.15.3"
   dependencies:
     "@codemirror/state": ^6.1.4
     style-mod: ^4.0.0
     w3c-keyname: ^2.2.4
-  checksum: 19114ee05b3795ebe07a69cf00c36e8351b3500ce105b8412d90e757d459f71370ead3de852f0fda069041803276e6c38e6f1f943f77e85c9b5c279ab7fa1c4a
+  checksum: 048949b1b493a962904a7f77661a939f7c1893a7381022756a135f5dd8daf667f498be1b81da9c37c0e8de85b078ad987c2f75318385c520ed83c95da6313e95
   languageName: node
   linkType: hard
 
 "@csstools/selector-specificity@npm:^2.0.2":
   version: 2.2.0
   resolution: "@csstools/selector-specificity@npm:2.2.0"
   peerDependencies:
@@ -1650,17 +1646,17 @@
   peerDependencies:
     eslint: ^6.0.0 || ^7.0.0 || >=8.0.0
   checksum: cdfe3ae42b4f572cbfb46d20edafe6f36fc5fb52bf2d90875c58aefe226892b9677fef60820e2832caf864a326fe4fc225714c46e8389ccca04d5f9288aabd22
   languageName: node
   linkType: hard
 
 "@eslint-community/regexpp@npm:^4.4.0":
-  version: 4.5.1
-  resolution: "@eslint-community/regexpp@npm:4.5.1"
-  checksum: 6d901166d64998d591fab4db1c2f872981ccd5f6fe066a1ad0a93d4e11855ecae6bfb76660869a469563e8882d4307228cebd41142adb409d182f2966771e57e
+  version: 4.6.2
+  resolution: "@eslint-community/regexpp@npm:4.6.2"
+  checksum: a3c341377b46b54fa228f455771b901d1a2717f95d47dcdf40199df30abc000ba020f747f114f08560d119e979d882a94cf46cfc51744544d54b00319c0f2724
   languageName: node
   linkType: hard
 
 "@eslint/eslintrc@npm:^2.1.0":
   version: 2.1.0
   resolution: "@eslint/eslintrc@npm:2.1.0"
   dependencies:
@@ -2049,88 +2045,88 @@
     "@lumino/signaling": ^1.10.0 || ^2.0.0
     y-protocols: ^1.0.5
     yjs: ^13.5.40
   checksum: 739f9630940466b3cfcd7b742dd06479f81772ca13f863d057af0bbb5e318829506969066ab72977e7c721644982b5c8f88cf44e1ae81955ed1c27e87632d1f2
   languageName: node
   linkType: hard
 
-"@jupyterlab/application@npm:^4.0.0, @jupyterlab/application@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/application@npm:4.0.2"
+"@jupyterlab/application@npm:^4.0.0, @jupyterlab/application@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/application@npm:4.0.3"
   dependencies:
     "@fortawesome/fontawesome-free": ^5.12.0
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/docregistry": ^4.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/statedb": ^4.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
+    "@jupyterlab/apputils": ^4.1.3
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/docregistry": ^4.0.3
+    "@jupyterlab/rendermime": ^4.0.3
+    "@jupyterlab/rendermime-interfaces": ^3.8.3
+    "@jupyterlab/services": ^7.0.3
+    "@jupyterlab/statedb": ^4.0.3
+    "@jupyterlab/translation": ^4.0.3
+    "@jupyterlab/ui-components": ^4.0.3
     "@lumino/algorithm": ^2.0.0
     "@lumino/application": ^2.1.1
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/polling": ^2.1.1
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
-  checksum: 5709b59c794e481d6e9b6c5575042c569f38058b6fc2a2c1d2831bdd0d1b0ff4df60c17132753ed8d9be1e2a28e4a0a18310d2b80e8ff5812fdaccbb1ee18bce
+  checksum: 25443512d8df22bc87899ed944c9d7ea6c233501173ddd6316d9f0fda0faa523b38b9973f98aeb519a138649839d1d61e19d54f28b229e20485f90d11495eaae
   languageName: node
   linkType: hard
 
-"@jupyterlab/apputils@npm:^4.1.2":
-  version: 4.1.2
-  resolution: "@jupyterlab/apputils@npm:4.1.2"
+"@jupyterlab/apputils@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/apputils@npm:4.1.3"
   dependencies:
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/settingregistry": ^4.0.2
-    "@jupyterlab/statedb": ^4.0.2
-    "@jupyterlab/statusbar": ^4.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/observables": ^5.0.3
+    "@jupyterlab/rendermime-interfaces": ^3.8.3
+    "@jupyterlab/services": ^7.0.3
+    "@jupyterlab/settingregistry": ^4.0.3
+    "@jupyterlab/statedb": ^4.0.3
+    "@jupyterlab/statusbar": ^4.0.3
+    "@jupyterlab/translation": ^4.0.3
+    "@jupyterlab/ui-components": ^4.0.3
     "@lumino/algorithm": ^2.0.0
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/domutils": ^2.0.0
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.1
     "@types/react": ^18.0.26
     react: ^18.2.0
     sanitize-html: ~2.7.3
-  checksum: 89a445478b54d1132e753022a81393dd3e53f7f36de2d9e905ece3bae911382ddff6afc16c4b649646b1a125c774ccc83fa4d92e29a48a423d4410a4a5554bb4
+  checksum: c67b42e665edc71faf2e8c3eee2a90b6b80d6c1f06100802abec0ccb8ca8ba141b5705e5f186e73f03467ad1aeede71e9c9c77dbff8f316c7d1cd5f8ba39672e
   languageName: node
   linkType: hard
 
-"@jupyterlab/attachments@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/attachments@npm:4.0.2"
+"@jupyterlab/attachments@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/attachments@npm:4.0.3"
   dependencies:
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
+    "@jupyterlab/nbformat": ^4.0.3
+    "@jupyterlab/observables": ^5.0.3
+    "@jupyterlab/rendermime": ^4.0.3
+    "@jupyterlab/rendermime-interfaces": ^3.8.3
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
-  checksum: 178d6abf3ff0767d87f78a79470760cf0025c3171e65dfd9a07916f3f6322f1080a21985ccdfdfeeec6fb73fb9aac9179cc413c43e4e33a45bcbcefa6cb97714
+  checksum: 389b73436a258829ec559d8112f7ce50afa74041c67d30613a9ccabb6fb2af1bf0cf12f840780c31dff1627aae788bd23be06c77e6c63c0d641537989615169d
   languageName: node
   linkType: hard
 
 "@jupyterlab/builder@npm:^4.0.0":
-  version: 4.0.2
-  resolution: "@jupyterlab/builder@npm:4.0.2"
+  version: 4.0.3
+  resolution: "@jupyterlab/builder@npm:4.0.3"
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/application": ^2.1.1
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/domutils": ^2.0.0
@@ -2157,505 +2153,505 @@
     terser-webpack-plugin: ^5.3.7
     webpack: ^5.76.1
     webpack-cli: ^5.0.1
     webpack-merge: ^5.8.0
     worker-loader: ^3.0.2
   bin:
     build-labextension: lib/build-labextension.js
-  checksum: bb3ecbde5b2207d38577ad4f49af3b92a68b093d56b9eb1611fa967e553aab3e899a6e651edf90834e1b2d9ced57078e976ac03791178104962325423da25e7e
+  checksum: 7d6402f859bc43cf7baa90893e57bd8d421716256c51fe72b1f80f4b471446e918d77912babe9bfac87a4edcc2ae3d6434334688f13414d293ff340266607b46
   languageName: node
   linkType: hard
 
-"@jupyterlab/cells@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/cells@npm:4.0.2"
+"@jupyterlab/cells@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/cells@npm:4.0.3"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/attachments": ^4.0.2
-    "@jupyterlab/codeeditor": ^4.0.2
-    "@jupyterlab/codemirror": ^4.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/documentsearch": ^4.0.2
-    "@jupyterlab/filebrowser": ^4.0.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/outputarea": ^4.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/toc": ^6.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
+    "@jupyterlab/apputils": ^4.1.3
+    "@jupyterlab/attachments": ^4.0.3
+    "@jupyterlab/codeeditor": ^4.0.3
+    "@jupyterlab/codemirror": ^4.0.3
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/documentsearch": ^4.0.3
+    "@jupyterlab/filebrowser": ^4.0.3
+    "@jupyterlab/nbformat": ^4.0.3
+    "@jupyterlab/observables": ^5.0.3
+    "@jupyterlab/outputarea": ^4.0.3
+    "@jupyterlab/rendermime": ^4.0.3
+    "@jupyterlab/services": ^7.0.3
+    "@jupyterlab/toc": ^6.0.3
+    "@jupyterlab/translation": ^4.0.3
+    "@jupyterlab/ui-components": ^4.0.3
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/domutils": ^2.0.0
     "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/polling": ^2.1.1
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: 92aa9ced743b41fbe5c0d3700762e3f825c9b01fb9b5684c909de330a62561a7b05af27390ca5993f905ec7141fa01072446b51232a8616181dd4eaed178b77f
+  checksum: 48b835ba839f3cf565de0b7181e2404ddf928fc20ec966039fa7680fe6b9d72a66a612da31a62f7821312f11ac571790293b10488e4946e69448ac1be32c3433
   languageName: node
   linkType: hard
 
-"@jupyterlab/codeeditor@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/codeeditor@npm:4.0.2"
+"@jupyterlab/codeeditor@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/codeeditor@npm:4.0.3"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/statusbar": ^4.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/nbformat": ^4.0.3
+    "@jupyterlab/observables": ^5.0.3
+    "@jupyterlab/statusbar": ^4.0.3
+    "@jupyterlab/translation": ^4.0.3
+    "@jupyterlab/ui-components": ^4.0.3
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: 61b638011acd21195fcd53b3b1f1df54abef0e0db85937f41f3a323cc6df75bcd63261739518bfd82b6bf45f638a090687cb43c2b66880546cff3e962d2e5994
+  checksum: 9e2da69f4bc579ff3d66a863f805b0a2edf1de8590139874767d349aff3e29e50a490fba92242a9c593f33144b6349c1d5a03eee4894ba7ed448593b12bb90eb
   languageName: node
   linkType: hard
 
-"@jupyterlab/codemirror@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/codemirror@npm:4.0.2"
+"@jupyterlab/codemirror@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/codemirror@npm:4.0.3"
   dependencies:
     "@codemirror/autocomplete": ^6.5.1
     "@codemirror/commands": ^6.2.3
     "@codemirror/lang-cpp": ^6.0.2
     "@codemirror/lang-css": ^6.1.1
     "@codemirror/lang-html": ^6.4.3
     "@codemirror/lang-java": ^6.0.1
     "@codemirror/lang-javascript": ^6.1.7
     "@codemirror/lang-json": ^6.0.1
     "@codemirror/lang-markdown": ^6.1.1
     "@codemirror/lang-php": ^6.0.1
-    "@codemirror/lang-python": ^6.1.2
+    "@codemirror/lang-python": ^6.1.3
     "@codemirror/lang-rust": ^6.0.1
     "@codemirror/lang-sql": ^6.4.1
     "@codemirror/lang-wast": ^6.0.1
     "@codemirror/lang-xml": ^6.0.2
     "@codemirror/language": ^6.6.0
     "@codemirror/legacy-modes": ^6.3.2
     "@codemirror/search": ^6.3.0
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/codeeditor": ^4.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/documentsearch": ^4.0.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/translation": ^4.0.2
+    "@jupyterlab/codeeditor": ^4.0.3
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/documentsearch": ^4.0.3
+    "@jupyterlab/nbformat": ^4.0.3
+    "@jupyterlab/translation": ^4.0.3
     "@lezer/common": ^1.0.2
     "@lezer/generator": ^1.2.2
     "@lezer/highlight": ^1.1.4
     "@lezer/markdown": ^1.0.2
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
     yjs: ^13.5.40
-  checksum: 1ddf08979874fc522eb88de6a743129640c5721410a8c6feb58d2e37b35ebcdeee5c217890e7f9561a595ca8b1c9b4a222b07da5e2e95c1e2dcd8c467378c50d
+  checksum: 6c68d49f515a32df8a13a258d30dca01dfd7a77086d0df729d825bac618c4805bb210f2b9b672cde027c20543dc7384c514c12c4a5aedc66dd8b56f638b51569
   languageName: node
   linkType: hard
 
-"@jupyterlab/coreutils@npm:^6.0.2":
-  version: 6.0.2
-  resolution: "@jupyterlab/coreutils@npm:6.0.2"
+"@jupyterlab/coreutils@npm:^6.0.3":
+  version: 6.0.3
+  resolution: "@jupyterlab/coreutils@npm:6.0.3"
   dependencies:
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
     minimist: ~1.2.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.4
-  checksum: c2e9b9bf7227f68bb6b91044d2ac3808a872ac967e22f6aee10241d5dbc78a19deee65f91dd87c080f63170a760c96c99cb31e0e0b6f32c6341e432d781355ce
+  checksum: c151b724f283477a92676520fd8009765d772c0bd2716d8648d0c79a56c402b6832609c870dd8ba683218d25a8c05ef769801e4699cedb989caadd99dff1ffe8
   languageName: node
   linkType: hard
 
-"@jupyterlab/docmanager@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/docmanager@npm:4.0.2"
+"@jupyterlab/docmanager@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/docmanager@npm:4.0.3"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/docregistry": ^4.0.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/statusbar": ^4.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
+    "@jupyterlab/apputils": ^4.1.3
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/docregistry": ^4.0.3
+    "@jupyterlab/services": ^7.0.3
+    "@jupyterlab/statusbar": ^4.0.3
+    "@jupyterlab/translation": ^4.0.3
+    "@jupyterlab/ui-components": ^4.0.3
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: dca1f56209608a82eebb0a365657f955bc8c546d66e00ec7747e753e3c76c8c0a5ed24b51736d157d2ed9d8264dc69545221e8fc2aa6af3eb6ec7eb4fd537a69
+  checksum: 2ce21005c918275e5bbd63a54d6cb89a4b2bbf6d9aa8ec0a3b172c48cce98a31d83bbd10c8a2211394ec41c60b782ab73b7dc3481de23bfc89be631cfa43cb5e
   languageName: node
   linkType: hard
 
-"@jupyterlab/docregistry@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/docregistry@npm:4.0.2"
+"@jupyterlab/docregistry@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/docregistry@npm:4.0.3"
   dependencies:
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/codeeditor": ^4.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
+    "@jupyterlab/apputils": ^4.1.3
+    "@jupyterlab/codeeditor": ^4.0.3
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/observables": ^5.0.3
+    "@jupyterlab/rendermime": ^4.0.3
+    "@jupyterlab/rendermime-interfaces": ^3.8.3
+    "@jupyterlab/services": ^7.0.3
+    "@jupyterlab/translation": ^4.0.3
+    "@jupyterlab/ui-components": ^4.0.3
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
-  checksum: b88c6a6ab7825aff95541c8a9f4381ccee4533e8c5bda588538c8a110dd8c6cb413e73345bc8fbf74aebe9fed4f9d298de6efa08378212869510e81ccb9f10ca
+  checksum: 3b3256c4b4755c58b3f290403ef49e3ebc6bebb8c17f882a2cc58dfd40a596bc427ba41e60a610ce6c90fc5b4cbd552502ce56a6654b85fb35283bdaed58b861
   languageName: node
   linkType: hard
 
-"@jupyterlab/documentsearch@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/documentsearch@npm:4.0.2"
+"@jupyterlab/documentsearch@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/documentsearch@npm:4.0.3"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
+    "@jupyterlab/apputils": ^4.1.3
+    "@jupyterlab/translation": ^4.0.3
+    "@jupyterlab/ui-components": ^4.0.3
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/polling": ^2.1.1
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: d621722648f8d0e9c17c4df093bf02de0b3c5c1e8cb4b4b46482114700c4ca47dbb35831d2f046b0a28c950c6cd7442cdd791357af87d6e4df5da3b347d463e0
+  checksum: fcf8c50a60e2b265901b27749f63b52f17467950da863f8b766d30038a63aa896de4352ea5eb1221f82ec0abf11be424c13f17d0b912e758e456e596e2927b1f
   languageName: node
   linkType: hard
 
-"@jupyterlab/filebrowser@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/filebrowser@npm:4.0.2"
+"@jupyterlab/filebrowser@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/filebrowser@npm:4.0.3"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/docmanager": ^4.0.2
-    "@jupyterlab/docregistry": ^4.0.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/statedb": ^4.0.2
-    "@jupyterlab/statusbar": ^4.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
+    "@jupyterlab/apputils": ^4.1.3
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/docmanager": ^4.0.3
+    "@jupyterlab/docregistry": ^4.0.3
+    "@jupyterlab/services": ^7.0.3
+    "@jupyterlab/statedb": ^4.0.3
+    "@jupyterlab/statusbar": ^4.0.3
+    "@jupyterlab/translation": ^4.0.3
+    "@jupyterlab/ui-components": ^4.0.3
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/domutils": ^2.0.0
     "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/polling": ^2.1.1
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: ae5426f6811488cb90538f8ec74fa87d4ead847a2727ba64d35b4b2d81e6058bc6340853affedb2e4e7362627453b8dd1e108142a425bc039745714058ce5d73
+  checksum: 30c2447cfe76fb2d1c3d1c88136b842f8d0f46451d4082ecc1a26496e35f5309a956468af18b2b0ac42a72c9bd14a1ddd050d434c6d9740b468956a6bb989086
   languageName: node
   linkType: hard
 
-"@jupyterlab/lsp@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/lsp@npm:4.0.2"
+"@jupyterlab/lsp@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/lsp@npm:4.0.3"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/codeeditor": ^4.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/docregistry": ^4.0.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/translation": ^4.0.2
+    "@jupyterlab/apputils": ^4.1.3
+    "@jupyterlab/codeeditor": ^4.0.3
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/docregistry": ^4.0.3
+    "@jupyterlab/services": ^7.0.3
+    "@jupyterlab/translation": ^4.0.3
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
     lodash.mergewith: ^4.6.1
     vscode-jsonrpc: ^6.0.0
     vscode-languageserver-protocol: ^3.17.0
     vscode-ws-jsonrpc: ~1.0.2
-  checksum: 476517f4cd9ce7758638f96c1037f26d758ec8e102d87b9472cbaa6208d94bcfc1da0ec853202761f6542404a034932657b14f82e2355d312b3f0c5c140cfbfd
+  checksum: f80084ef6a5337d768281d6d9029e303c0867ced6449301708be76d32a411de7e4d41ca290b92596ef206456533e8132d1221cd1d2feee7ad341b2b998ddc766
   languageName: node
   linkType: hard
 
-"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/nbformat@npm:4.0.2"
+"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/nbformat@npm:4.0.3"
   dependencies:
     "@lumino/coreutils": ^2.1.1
-  checksum: cccd1c7fd8717ccece1f7642f3f7218103c3baa479fce85666770719b3359116e5279cdd97e2b584122a793b437fc9ece7055d1da27ad35a090f90398a76d59f
+  checksum: e7c3fc81fdd934d66b4b92aa44b82e40dff73248b54772d0a4501a7dd5e1ea76754931548f8e591e7f03bfad2f4409a34838424bd34f9abb0be11d213f2e129a
   languageName: node
   linkType: hard
 
-"@jupyterlab/notebook@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/notebook@npm:4.0.2"
+"@jupyterlab/notebook@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/notebook@npm:4.0.3"
   dependencies:
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/cells": ^4.0.2
-    "@jupyterlab/codeeditor": ^4.0.2
-    "@jupyterlab/codemirror": ^4.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/docregistry": ^4.0.2
-    "@jupyterlab/documentsearch": ^4.0.2
-    "@jupyterlab/lsp": ^4.0.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/settingregistry": ^4.0.2
-    "@jupyterlab/statusbar": ^4.0.2
-    "@jupyterlab/toc": ^6.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
+    "@jupyterlab/apputils": ^4.1.3
+    "@jupyterlab/cells": ^4.0.3
+    "@jupyterlab/codeeditor": ^4.0.3
+    "@jupyterlab/codemirror": ^4.0.3
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/docregistry": ^4.0.3
+    "@jupyterlab/documentsearch": ^4.0.3
+    "@jupyterlab/lsp": ^4.0.3
+    "@jupyterlab/nbformat": ^4.0.3
+    "@jupyterlab/observables": ^5.0.3
+    "@jupyterlab/rendermime": ^4.0.3
+    "@jupyterlab/services": ^7.0.3
+    "@jupyterlab/settingregistry": ^4.0.3
+    "@jupyterlab/statusbar": ^4.0.3
+    "@jupyterlab/toc": ^6.0.3
+    "@jupyterlab/translation": ^4.0.3
+    "@jupyterlab/ui-components": ^4.0.3
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/domutils": ^2.0.0
     "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: 053cde5377aceac7ff6fe30e734354df1839cbf84bfd19f7d3992a1aaddcd66f5c8470bb2537c94b28dfdb194dfdacfaa38207fd2d4989b0575b27c20396bbfe
+  checksum: 1388bea973c093b82ac110bf115f342fb5e2cae9c855f0704f08882df8a3714566fccefbb3d85903fdb30170bae4fdfd29b3785473850bb3e91e8cdfc3658265
   languageName: node
   linkType: hard
 
-"@jupyterlab/observables@npm:^5.0.2":
-  version: 5.0.2
-  resolution: "@jupyterlab/observables@npm:5.0.2"
+"@jupyterlab/observables@npm:^5.0.3":
+  version: 5.0.3
+  resolution: "@jupyterlab/observables@npm:5.0.3"
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
-  checksum: 6d206873f3e2bfd95267fde6fae565eef5c1f7df93dc0a27091ea3eceea5cbded6c8b90eb5d4311e3b6158385455ed358602cb4b3daee717f6cc195b259cfb24
+  checksum: fe1283852967092dfdf95407135e723c107ba1e4ce502f6b0c10bed575f8e11d08190a6f078f5e2b937e5f4f1996351df8ee9b2bd523fb106b728dd6b3dc15ac
   languageName: node
   linkType: hard
 
-"@jupyterlab/outputarea@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/outputarea@npm:4.0.2"
+"@jupyterlab/outputarea@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/outputarea@npm:4.0.3"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/translation": ^4.0.2
+    "@jupyterlab/apputils": ^4.1.3
+    "@jupyterlab/nbformat": ^4.0.3
+    "@jupyterlab/observables": ^5.0.3
+    "@jupyterlab/rendermime": ^4.0.3
+    "@jupyterlab/rendermime-interfaces": ^3.8.3
+    "@jupyterlab/services": ^7.0.3
+    "@jupyterlab/translation": ^4.0.3
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
-  checksum: 8387b93e7b6bf1a63495eef8a7746870e4210818ff26af5c8ecdf4b9e78433ec47b58ddaa5ab11fbf5cf143802b23a186c90589974cd408cae95330fa3960f32
+  checksum: bd4a60ea43cd3117c8cc6b6aee094f0a4e37c3635051fbf13857669547847ce52f6e186cb2c329893e333e6113998899a9d5fa90727926a73223d5082c936471
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime-interfaces@npm:^3.8.2":
-  version: 3.8.2
-  resolution: "@jupyterlab/rendermime-interfaces@npm:3.8.2"
+"@jupyterlab/rendermime-interfaces@npm:^3.8.3":
+  version: 3.8.3
+  resolution: "@jupyterlab/rendermime-interfaces@npm:3.8.3"
   dependencies:
     "@lumino/coreutils": ^1.11.0 || ^2.1.1
     "@lumino/widgets": ^1.37.2 || ^2.1.1
-  checksum: e1164a4ad7654e5e8af0c1c2f1c8938f01a4bd07e04ff788e8b3adfaa9cb7ef07118c44513648c69263929e1658f02dcbab7aac776c6071228b0b80c8ca4e65a
+  checksum: aeb055196099e29eff78e98e904e3dac10255ac4693ed0d99022d08fe3de4dd792e66c06f6e11f110be2276e9ba36ae15b8a08e6fb1b4c25e774d5525199b5d3
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/rendermime@npm:4.0.2"
+"@jupyterlab/rendermime@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/rendermime@npm:4.0.3"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/translation": ^4.0.2
+    "@jupyterlab/apputils": ^4.1.3
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/nbformat": ^4.0.3
+    "@jupyterlab/observables": ^5.0.3
+    "@jupyterlab/rendermime-interfaces": ^3.8.3
+    "@jupyterlab/services": ^7.0.3
+    "@jupyterlab/translation": ^4.0.3
     "@lumino/coreutils": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     lodash.escape: ^4.0.1
-  checksum: 6118adf39cfe3c5918c9b677ff5d8dbe97ce469427f9969e1d16fba944b53d6e6c9d2c1e2deaaf928cdb94222a8941c7bb7cfc81693683fd07c08e92bc3d6cea
+  checksum: 8e5d390ee84eb0f2017b80c2ccf4dc318ef53c3ebb52e84056d76b2bccbcb755190b7712e99936ad0610f03fe4b0a9a0f2f5ed854e21856c0cc39371ce1fad01
   languageName: node
   linkType: hard
 
-"@jupyterlab/services@npm:^7.0.2":
-  version: 7.0.2
-  resolution: "@jupyterlab/services@npm:7.0.2"
+"@jupyterlab/services@npm:^7.0.3":
+  version: 7.0.3
+  resolution: "@jupyterlab/services@npm:7.0.3"
   dependencies:
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/settingregistry": ^4.0.2
-    "@jupyterlab/statedb": ^4.0.2
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/nbformat": ^4.0.3
+    "@jupyterlab/settingregistry": ^4.0.3
+    "@jupyterlab/statedb": ^4.0.3
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/polling": ^2.1.1
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     ws: ^8.11.0
-  checksum: 4a4b5328f2f50ec1d501f67d63fbfb329f37a6c090227e0aecdbbb7316d9df0e5891af47cb948958e9307a0afc52f0ddf05c2be7acb9e2f44e54cf568dc3b90c
+  checksum: 94277bdf4c6645145c09dcf41fbcf49528cb4c0e283fc7b596184615d7a0127b9129097f877455af85bf26e2110aee61f664e3cce9497f573c00a5dd90e5d0fd
   languageName: node
   linkType: hard
 
-"@jupyterlab/settingregistry@npm:^4.0.0, @jupyterlab/settingregistry@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/settingregistry@npm:4.0.2"
+"@jupyterlab/settingregistry@npm:^4.0.0, @jupyterlab/settingregistry@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/settingregistry@npm:4.0.3"
   dependencies:
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/statedb": ^4.0.2
+    "@jupyterlab/nbformat": ^4.0.3
+    "@jupyterlab/statedb": ^4.0.3
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
     "@rjsf/utils": ^5.1.0
     ajv: ^8.12.0
     json5: ^2.2.3
   peerDependencies:
     react: ">=16"
-  checksum: c2e019f70a4f19cf99bc2029c136197f2a750f319e16f8605a6f8d690b6930ac32e24678b090a09f9e949e540cf6b4214d3d3597ec119bd6896db3b456ac6299
+  checksum: 3874fa5a318c1301dc152c569a43de846ec3157fb1083b22a92571e5632749317361e5caaba513359db6fb8e8e3804b7d7ccff5058eb25dcc55af59d76c03d20
   languageName: node
   linkType: hard
 
-"@jupyterlab/statedb@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/statedb@npm:4.0.2"
+"@jupyterlab/statedb@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/statedb@npm:4.0.3"
   dependencies:
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
-  checksum: 88fc80914f4c128ae6b0630ffe97111cc95a8edc4f34e749615aa8396262d74efcc82e02d0c7c2dcd0268b7cc35a0bfbd7455a4b6cb9203bcad488e1cbad5c25
+  checksum: 07f625988489565704e5b90069111dee255ed62bec2784f1a1ea57192b850beab733b8f19d0f0ebfc83fbad2a3479e6180f00554f1560bd6bb641b019356961f
   languageName: node
   linkType: hard
 
-"@jupyterlab/statusbar@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/statusbar@npm:4.0.2"
+"@jupyterlab/statusbar@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/statusbar@npm:4.0.3"
   dependencies:
-    "@jupyterlab/ui-components": ^4.0.2
+    "@jupyterlab/ui-components": ^4.0.3
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: d792eb8fca00ac5ec7d5abcb3694db5c80706ec468aa4a9bef543f02a788d80ca2a9b81def0a846da14aed22dbd4ceffe0c95c0047c5025c2e5d69fc55f739b9
+  checksum: 41319c4b7f22ecef701fc006b83de0963f65c7fab98a3d0020861df2c76cc6832dc044500f01bbc8a20f85d025573d3850d6edcf412be2fcb9091bbe7debd04e
   languageName: node
   linkType: hard
 
-"@jupyterlab/testing@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/testing@npm:4.0.2"
+"@jupyterlab/testing@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/testing@npm:4.0.3"
   dependencies:
     "@babel/core": ^7.10.2
     "@babel/preset-env": ^7.10.2
-    "@jupyterlab/coreutils": ^6.0.2
+    "@jupyterlab/coreutils": ^6.0.3
     "@lumino/coreutils": ^2.1.1
     "@lumino/signaling": ^2.1.1
     child_process: ~1.0.2
     deepmerge: ^4.2.2
     fs-extra: ^10.1.0
     identity-obj-proxy: ^3.0.0
     jest: ^29.2.0
     jest-environment-jsdom: ^29.3.0
     jest-junit: ^15.0.0
     node-fetch: ^2.6.0
     simulate-event: ~1.4.0
     ts-jest: ^29.1.0
   peerDependencies:
     typescript: ">=4.3"
-  checksum: 8876d6633956fda7d3e6eb97dcb987e42adbce89faadba36bbb71e30475fe23ebb4d6f2765454abc0c21c0c1f52d6eb864c6be28fdd77937a5c970e9bc214749
+  checksum: a69e405d9faa36f48d58b2dc08ad7961adf043d33b834180afe6fb4ced3fa917418c831b3fc233c65f7ec92666828a418fe3135d4502980122763189b103a007
   languageName: node
   linkType: hard
 
 "@jupyterlab/testutils@npm:^4.0.0":
-  version: 4.0.2
-  resolution: "@jupyterlab/testutils@npm:4.0.2"
+  version: 4.0.3
+  resolution: "@jupyterlab/testutils@npm:4.0.3"
   dependencies:
-    "@jupyterlab/application": ^4.0.2
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/notebook": ^4.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/testing": ^4.0.2
-  checksum: fdefc6f702057846db258b59a7a9e03fa6bcc3746c5604a6432c0136c35b392db88bb33bade5e74c975076e32a091ce649fa53bf86762629aa5f991b2439d663
+    "@jupyterlab/application": ^4.0.3
+    "@jupyterlab/apputils": ^4.1.3
+    "@jupyterlab/notebook": ^4.0.3
+    "@jupyterlab/rendermime": ^4.0.3
+    "@jupyterlab/testing": ^4.0.3
+  checksum: 8194b2551d7c921aa53c18f24d53e0a29fb8a60e4b4c66cd5873da15bf7c36910874de39f4750f42c0340419548cb8917cdfa9f69fa7cce55e6d604e85244dab
   languageName: node
   linkType: hard
 
-"@jupyterlab/toc@npm:^6.0.2":
-  version: 6.0.2
-  resolution: "@jupyterlab/toc@npm:6.0.2"
+"@jupyterlab/toc@npm:^6.0.3":
+  version: 6.0.3
+  resolution: "@jupyterlab/toc@npm:6.0.3"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/docregistry": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
+    "@jupyterlab/apputils": ^4.1.3
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/docregistry": ^4.0.3
+    "@jupyterlab/observables": ^5.0.3
+    "@jupyterlab/rendermime": ^4.0.3
+    "@jupyterlab/translation": ^4.0.3
+    "@jupyterlab/ui-components": ^4.0.3
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: de36885b17d7fa067a89f84cbdeb48ecc7c90acd6b7596745c8c96b652f6853e5d744d04dab82746f94eeea65b090c32a6153191d182c2b4d969a4834c6ec8c3
+  checksum: 8098824692a3e5ac786d476b7c14abc4adbef0db3f0f38143969594dd4fd3069f92335ac417fc45d42d1577d3555791c6aecdf2361acb22d3902b93b899b31f0
   languageName: node
   linkType: hard
 
-"@jupyterlab/translation@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/translation@npm:4.0.2"
+"@jupyterlab/translation@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/translation@npm:4.0.3"
   dependencies:
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/statedb": ^4.0.2
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/rendermime-interfaces": ^3.8.3
+    "@jupyterlab/services": ^7.0.3
+    "@jupyterlab/statedb": ^4.0.3
     "@lumino/coreutils": ^2.1.1
-  checksum: 8f229be773607988509d059097c30bf8fbc8191d5b027221658436b2f539f6904ea48e7998276da7c52cdacd0821ea4cbdfd12ad0650ce0213525217d8735bf4
+  checksum: 255868017c500e32e97bdfcff02ded6352f03bc64928b77c0d34ae9c735093c6c0d6e448501cb14466996ff5ebdaaa6071d262a6f49ba6b06ea58cfac122c95d
   languageName: node
   linkType: hard
 
-"@jupyterlab/ui-components@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/ui-components@npm:4.0.2"
+"@jupyterlab/ui-components@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/ui-components@npm:4.0.3"
   dependencies:
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
-    "@jupyterlab/translation": ^4.0.2
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/observables": ^5.0.3
+    "@jupyterlab/rendermime-interfaces": ^3.8.3
+    "@jupyterlab/translation": ^4.0.3
     "@lumino/algorithm": ^2.0.0
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/polling": ^2.1.1
     "@lumino/properties": ^2.0.0
@@ -2665,15 +2661,15 @@
     "@rjsf/core": ^5.1.0
     "@rjsf/utils": ^5.1.0
     react: ^18.2.0
     react-dom: ^18.2.0
     typestyle: ^2.0.4
   peerDependencies:
     react: ^18.2.0
-  checksum: 5e941c557609e2cec3df3cb42de358c13f73f3cd0a3b0ce6c5d473dc8d7d09772d8dc35f843f9ef1b6619700fa4a403979a93aae047517efa5d9385a8f90eac7
+  checksum: c64afe7a0c932e42d4a00f874d499c52b4bac9794965f6146307922c086ea88e245bdcd346211f808f60ba3985f30c01138cfa6f5b1acc290d07ef04404f91a7
   languageName: node
   linkType: hard
 
 "@lezer/common@npm:^1.0.0, @lezer/common@npm:^1.0.2":
   version: 1.0.3
   resolution: "@lezer/common@npm:1.0.3"
   checksum: cc90dc2f0aeaebeb3fe886cbd27f8b1e8bee817d8c2efff178604807debd68c5db820fd23afb830962780063d21891afbdf564420221faca2822e77bc6327184
@@ -2718,41 +2714,41 @@
   dependencies:
     "@lezer/common": ^1.0.0
   checksum: 411a702394c4c996b7d7f145a38f3a85a8cc698b3918acc7121c629255bb76d4ab383753f69009e011dc415210c6acbbb5b27bde613259ab67e600b29397b03b
   languageName: node
   linkType: hard
 
 "@lezer/html@npm:^1.3.0":
-  version: 1.3.5
-  resolution: "@lezer/html@npm:1.3.5"
+  version: 1.3.6
+  resolution: "@lezer/html@npm:1.3.6"
   dependencies:
     "@lezer/common": ^1.0.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 19fcf262d06a89d8a1d3c6c825585f4b555dbdeaf60179fbe00164f72c0dbdf8cde8057172fd3660b13be63f0dcf1380cea9196ade7c1a9bc58a2aecd2b03125
+  checksum: 1d3af781660968505e5083a34f31ea3549fd5f3949227fa93cc318bca61bce76ffe977bd875624ba938a2039834ec1a33df5d365e94c48131c85dd26f980d92c
   languageName: node
   linkType: hard
 
 "@lezer/java@npm:^1.0.0":
   version: 1.0.4
   resolution: "@lezer/java@npm:1.0.4"
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: 97f5a2c2d733afba5dc57a0da9a97515b19b5e63bb5937717dac4e8c9baed74d15c0cb5c1580858b678931f11d517c56d89f903968fa48931f9c62e2ea67a107
   languageName: node
   linkType: hard
 
 "@lezer/javascript@npm:^1.0.0":
-  version: 1.4.4
-  resolution: "@lezer/javascript@npm:1.4.4"
+  version: 1.4.5
+  resolution: "@lezer/javascript@npm:1.4.5"
   dependencies:
     "@lezer/highlight": ^1.1.3
     "@lezer/lr": ^1.3.0
-  checksum: 29797dbb4c0632718cc5a3d0c6baeefe4240562f8b1ef1f60c58d0481c53ac4bbbac354369aa95e4131dfe0bbc4464bc025620f58f01739bd896974bb08dbad5
+  checksum: 1402075c58f7344a3024f75253c8dabc7049d51b65480af194f081044be21434261c8a4db4ccf42629a2bfc838104838c8d87a58693134ee5660c122b63b4b72
   languageName: node
   linkType: hard
 
 "@lezer/json@npm:^1.0.0":
   version: 1.0.1
   resolution: "@lezer/json@npm:1.0.1"
   dependencies:
@@ -2965,23 +2961,14 @@
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
   checksum: 963c0e54102b786a9cbf3467041c9f6f5c275af751afc311ebeba30d56516767c463c425e321bb389eaa66726dfc4420119a9a58573dcbf3110aba9515c80606
   languageName: node
   linkType: hard
 
-"@nicolo-ribaudo/semver-v6@npm:^6.3.3":
-  version: 6.3.3
-  resolution: "@nicolo-ribaudo/semver-v6@npm:6.3.3"
-  bin:
-    semver: bin/semver.js
-  checksum: 8290855b1591477d2298364541fda64fafd4acc110b387067a71c9b05f4105c0a4ac079857ae9cd107c42ee884e8724a406b5116f069575e02d7ab87a35a5272
-  languageName: node
-  linkType: hard
-
 "@nodelib/fs.scandir@npm:2.1.5":
   version: 2.1.5
   resolution: "@nodelib/fs.scandir@npm:2.1.5"
   dependencies:
     "@nodelib/fs.stat": 2.0.5
     run-parallel: ^1.1.9
   checksum: a970d595bd23c66c880e0ef1817791432dbb7acbb8d44b7e7d0e7a22f4521260d4a83f7f9fd61d44fda4610105577f8f58a60718105fb38352baed612fd79e59
@@ -3018,41 +3005,41 @@
   version: 0.11.0
   resolution: "@pkgjs/parseargs@npm:0.11.0"
   checksum: 6ad6a00fc4f2f2cfc6bff76fb1d88b8ee20bc0601e18ebb01b6d4be583733a860239a521a7fbca73b612e66705078809483549d2b18f370eb346c5155c8e4a0f
   languageName: node
   linkType: hard
 
 "@rjsf/core@npm:^5.1.0":
-  version: 5.9.0
-  resolution: "@rjsf/core@npm:5.9.0"
+  version: 5.10.0
+  resolution: "@rjsf/core@npm:5.10.0"
   dependencies:
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     markdown-to-jsx: ^7.2.1
     nanoid: ^3.3.6
     prop-types: ^15.8.1
   peerDependencies:
     "@rjsf/utils": ^5.8.x
     react: ^16.14.0 || >=17
-  checksum: 52406fcf560af51cb5b45ce95eb826ff1ad4ed1366c70b16b16137455f6b252cef507f76f139524228e12ccf2d49816b3538747431886476574ac2911f29aac1
+  checksum: 11ff7f07e31ba13c1c6cb5e9aee94c4a5916a3f0013cb19fdeaea9254a77b50acee05d531a70adf92ee8a2024525916b20bb1af79d7afaadbd212a6124a57e5a
   languageName: node
   linkType: hard
 
 "@rjsf/utils@npm:^5.1.0":
-  version: 5.9.0
-  resolution: "@rjsf/utils@npm:5.9.0"
+  version: 5.10.0
+  resolution: "@rjsf/utils@npm:5.10.0"
   dependencies:
     json-schema-merge-allof: ^0.8.1
     jsonpointer: ^5.0.1
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     react-is: ^18.2.0
   peerDependencies:
     react: ^16.14.0 || >=17
-  checksum: f1a1070539b24763b64631bb8d0d16a504fa46f029775a34e57c47e58b913b07e2869b45de6c993745a6320df3b6571f101abc2d07be59054a971e43facae6ea
+  checksum: 5f44334598cfee3c2bf9a9561680e9c91abce9240ddf54cdb800fbbbb69b182fa7cc1839127558b3661aadbb185fba676eb3189352c8a8b5eea83d0b46987fa7
   languageName: node
   linkType: hard
 
 "@shannon-shen/chapyter@workspace:.":
   version: 0.0.0-use.local
   resolution: "@shannon-shen/chapyter@workspace:."
   dependencies:
@@ -3165,20 +3152,20 @@
     "@types/eslint": "*"
     "@types/estree": "*"
   checksum: ea6a9363e92f301cd3888194469f9ec9d0021fe0a397a97a6dd689e7545c75de0bd2153dfb13d3ab532853a278b6572c6f678ce846980669e41029d205653460
   languageName: node
   linkType: hard
 
 "@types/eslint@npm:*":
-  version: 8.44.0
-  resolution: "@types/eslint@npm:8.44.0"
+  version: 8.44.1
+  resolution: "@types/eslint@npm:8.44.1"
   dependencies:
     "@types/estree": "*"
     "@types/json-schema": "*"
-  checksum: 2655f409a4ecdd64bb9dd9eb6715e7a2ac30c0e7f902b414e10dbe9d6d497baa5a0f13105e1f7bd5ad7a913338e2ab4bed1faf192a7a0d27d1acd45ba79d3f69
+  checksum: 8b45be72d3c22a1ee0b1cc7e7fb0e34e32bbf959e6b7e0e46d160c17894aedf159c1db5c85750f10068884c741eebc37a1cc7ea659de23a8df0c9a3203e2ff9d
   languageName: node
   linkType: hard
 
 "@types/estree@npm:*, @types/estree@npm:^1.0.0":
   version: 1.0.1
   resolution: "@types/estree@npm:1.0.1"
   checksum: e9aa175eacb797216fafce4d41e8202c7a75555bc55232dee0f9903d7171f8f19f0ae7d5191bb1a88cb90e65468be508c0df850a9fb81b4433b293a5a749899d
@@ -3216,20 +3203,20 @@
   dependencies:
     "@types/istanbul-lib-report": "*"
   checksum: f1ad54bc68f37f60b30c7915886b92f86b847033e597f9b34f2415acdbe5ed742fa559a0a40050d74cdba3b6a63c342cac1f3a64dba5b68b66a6941f4abd7903
   languageName: node
   linkType: hard
 
 "@types/jest@npm:^29.2.0":
-  version: 29.5.2
-  resolution: "@types/jest@npm:29.5.2"
+  version: 29.5.3
+  resolution: "@types/jest@npm:29.5.3"
   dependencies:
     expect: ^29.0.0
     pretty-format: ^29.0.0
-  checksum: 7d205599ea3cccc262bad5cc173d3242d6bf8138c99458509230e4ecef07a52d6ddcde5a1dbd49ace655c0af51d2dbadef3748697292ea4d86da19d9e03e19c0
+  checksum: e36bb92e0b9e5ea7d6f8832baa42f087fc1697f6cd30ec309a07ea4c268e06ec460f1f0cfd2581daf5eff5763475190ec1ad8ac6520c49ccfe4f5c0a48bfa676
   languageName: node
   linkType: hard
 
 "@types/jsdom@npm:^20.0.0":
   version: 20.0.1
   resolution: "@types/jsdom@npm:20.0.1"
   dependencies:
@@ -3251,17 +3238,17 @@
   version: 1.2.2
   resolution: "@types/minimist@npm:1.2.2"
   checksum: b8da83c66eb4aac0440e64674b19564d9d86c80ae273144db9681e5eeff66f238ade9515f5006ffbfa955ceff8b89ad2bd8ec577d7caee74ba101431fb07045d
   languageName: node
   linkType: hard
 
 "@types/node@npm:*":
-  version: 20.4.1
-  resolution: "@types/node@npm:20.4.1"
-  checksum: 22cbcc792f2eb636fe4188778ed0f32658ab872aa7fcb9847b3fa289a42b14b9f5e30c6faec50ef3c7adbc6c2a246926e5858136bb8b10c035a3fcaa6afbeed2
+  version: 20.4.5
+  resolution: "@types/node@npm:20.4.5"
+  checksum: 36a0304a8dc346a1b2d2edac4c4633eecf70875793d61a5274d0df052d7a7af7a8e34f29884eac4fbd094c4f0201477dcb39c0ecd3307ca141688806538d1138
   languageName: node
   linkType: hard
 
 "@types/normalize-package-data@npm:^2.4.0":
   version: 2.4.1
   resolution: "@types/normalize-package-data@npm:2.4.1"
   checksum: e87bccbf11f95035c89a132b52b79ce69a1e3652fe55962363063c9c0dae0fe2477ebc585e03a9652adc6f381d24ba5589cc5e51849df4ced3d3e004a7d40ed5
@@ -3286,21 +3273,21 @@
   version: 15.7.5
   resolution: "@types/prop-types@npm:15.7.5"
   checksum: 5b43b8b15415e1f298243165f1d44390403bb2bd42e662bca3b5b5633fdd39c938e91b7fce3a9483699db0f7a715d08cef220c121f723a634972fdf596aec980
   languageName: node
   linkType: hard
 
 "@types/react@npm:^18.0.26":
-  version: 18.2.14
-  resolution: "@types/react@npm:18.2.14"
+  version: 18.2.17
+  resolution: "@types/react@npm:18.2.17"
   dependencies:
     "@types/prop-types": "*"
     "@types/scheduler": "*"
     csstype: ^3.0.2
-  checksum: a6a5e8cc78f486b9020d1ad009aa6c56943c68c7c6376e0f8399e9cbcd950b7b8f5d73f00200f5379f5e58d31d57d8aed24357f301d8e86108cd438ce6c8b3dd
+  checksum: 150516b31bd98b635e4a56bcf2af007330b35cccb6e35e902f46a47f0e81e30c46cdacc095e91051bdf2f33e4846e7e62fd51b67e064dc7d15c00e15dfa449d5
   languageName: node
   linkType: hard
 
 "@types/scheduler@npm:*":
   version: 0.16.3
   resolution: "@types/scheduler@npm:0.16.3"
   checksum: 2b0aec39c24268e3ce938c5db2f2e77f5c3dd280e05c262d9c2fe7d890929e4632a6b8e94334017b66b45e4f92a5aa42ba3356640c2a1175fa37bef2f5200767
@@ -3359,131 +3346,131 @@
   dependencies:
     "@types/yargs-parser": "*"
   checksum: 5f3ac4dc4f6e211c1627340160fbe2fd247ceba002190da6cf9155af1798450501d628c9165a183f30a224fc68fa5e700490d740ff4c73e2cdef95bc4e8ba7bf
   languageName: node
   linkType: hard
 
 "@typescript-eslint/eslint-plugin@npm:^5.55.0":
-  version: 5.61.0
-  resolution: "@typescript-eslint/eslint-plugin@npm:5.61.0"
+  version: 5.62.0
+  resolution: "@typescript-eslint/eslint-plugin@npm:5.62.0"
   dependencies:
     "@eslint-community/regexpp": ^4.4.0
-    "@typescript-eslint/scope-manager": 5.61.0
-    "@typescript-eslint/type-utils": 5.61.0
-    "@typescript-eslint/utils": 5.61.0
+    "@typescript-eslint/scope-manager": 5.62.0
+    "@typescript-eslint/type-utils": 5.62.0
+    "@typescript-eslint/utils": 5.62.0
     debug: ^4.3.4
     graphemer: ^1.4.0
     ignore: ^5.2.0
     natural-compare-lite: ^1.4.0
     semver: ^7.3.7
     tsutils: ^3.21.0
   peerDependencies:
     "@typescript-eslint/parser": ^5.0.0
     eslint: ^6.0.0 || ^7.0.0 || ^8.0.0
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: d9e891fb43ccb75322fc40d58d02479f98bd3c962db71075438868b13f579643d714a24b5477a827be7ca2e7e9f6058c406241b6696a6395c6fcbd6de76e015c
+  checksum: fc104b389c768f9fa7d45a48c86d5c1ad522c1d0512943e782a56b1e3096b2cbcc1eea3fcc590647bf0658eef61aac35120a9c6daf979bf629ad2956deb516a1
   languageName: node
   linkType: hard
 
 "@typescript-eslint/parser@npm:^5.55.0":
-  version: 5.61.0
-  resolution: "@typescript-eslint/parser@npm:5.61.0"
+  version: 5.62.0
+  resolution: "@typescript-eslint/parser@npm:5.62.0"
   dependencies:
-    "@typescript-eslint/scope-manager": 5.61.0
-    "@typescript-eslint/types": 5.61.0
-    "@typescript-eslint/typescript-estree": 5.61.0
+    "@typescript-eslint/scope-manager": 5.62.0
+    "@typescript-eslint/types": 5.62.0
+    "@typescript-eslint/typescript-estree": 5.62.0
     debug: ^4.3.4
   peerDependencies:
     eslint: ^6.0.0 || ^7.0.0 || ^8.0.0
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: 2422bca03ecc6830700aaa739ec46b8e9ab6c0a47a67f140dc6b62a42a8b98997e73bce52c6a010b8a9b461211c46ba865d5b7f680a7823cf5c245d3b61f7fd5
+  checksum: d168f4c7f21a7a63f47002e2d319bcbb6173597af5c60c1cf2de046b46c76b4930a093619e69faf2d30214c29ab27b54dcf1efc7046a6a6bd6f37f59a990e752
   languageName: node
   linkType: hard
 
-"@typescript-eslint/scope-manager@npm:5.61.0":
-  version: 5.61.0
-  resolution: "@typescript-eslint/scope-manager@npm:5.61.0"
+"@typescript-eslint/scope-manager@npm:5.62.0":
+  version: 5.62.0
+  resolution: "@typescript-eslint/scope-manager@npm:5.62.0"
   dependencies:
-    "@typescript-eslint/types": 5.61.0
-    "@typescript-eslint/visitor-keys": 5.61.0
-  checksum: 6dfbb42c4b7d796ae3c395398bdfd2e5a4ae8aaf1448381278ecc39a1d1045af2cb452da5a00519d265bc1a5997523de22d5021acb4dbe1648502fe61512d3c6
+    "@typescript-eslint/types": 5.62.0
+    "@typescript-eslint/visitor-keys": 5.62.0
+  checksum: 6062d6b797fe1ce4d275bb0d17204c827494af59b5eaf09d8a78cdd39dadddb31074dded4297aaf5d0f839016d601032857698b0e4516c86a41207de606e9573
   languageName: node
   linkType: hard
 
-"@typescript-eslint/type-utils@npm:5.61.0":
-  version: 5.61.0
-  resolution: "@typescript-eslint/type-utils@npm:5.61.0"
+"@typescript-eslint/type-utils@npm:5.62.0":
+  version: 5.62.0
+  resolution: "@typescript-eslint/type-utils@npm:5.62.0"
   dependencies:
-    "@typescript-eslint/typescript-estree": 5.61.0
-    "@typescript-eslint/utils": 5.61.0
+    "@typescript-eslint/typescript-estree": 5.62.0
+    "@typescript-eslint/utils": 5.62.0
     debug: ^4.3.4
     tsutils: ^3.21.0
   peerDependencies:
     eslint: "*"
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: f0203fd48c6218f004dd73a9a71ba4cf97f015d0f13a7b3c821a3ba7ec814839bae270a1db589184ca7091fe54815a3171d1993e8a25200bf33e131bd6e855d4
+  checksum: fc41eece5f315dfda14320be0da78d3a971d650ea41300be7196934b9715f3fe1120a80207551eb71d39568275dbbcf359bde540d1ca1439d8be15e9885d2739
   languageName: node
   linkType: hard
 
-"@typescript-eslint/types@npm:5.61.0":
-  version: 5.61.0
-  resolution: "@typescript-eslint/types@npm:5.61.0"
-  checksum: d311ca2141f6bcb5f0f8f97ddbc218c9911e0735aaa30f0f2e64d518fb33568410754e1b04bf157175f8783504f8ec62a7ab53a66a18507f43edb1e21fe69e90
+"@typescript-eslint/types@npm:5.62.0":
+  version: 5.62.0
+  resolution: "@typescript-eslint/types@npm:5.62.0"
+  checksum: 48c87117383d1864766486f24de34086155532b070f6264e09d0e6139449270f8a9559cfef3c56d16e3bcfb52d83d42105d61b36743626399c7c2b5e0ac3b670
   languageName: node
   linkType: hard
 
-"@typescript-eslint/typescript-estree@npm:5.61.0":
-  version: 5.61.0
-  resolution: "@typescript-eslint/typescript-estree@npm:5.61.0"
+"@typescript-eslint/typescript-estree@npm:5.62.0":
+  version: 5.62.0
+  resolution: "@typescript-eslint/typescript-estree@npm:5.62.0"
   dependencies:
-    "@typescript-eslint/types": 5.61.0
-    "@typescript-eslint/visitor-keys": 5.61.0
+    "@typescript-eslint/types": 5.62.0
+    "@typescript-eslint/visitor-keys": 5.62.0
     debug: ^4.3.4
     globby: ^11.1.0
     is-glob: ^4.0.3
     semver: ^7.3.7
     tsutils: ^3.21.0
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: efe25a1b2774939c02cb9b388cf72efa672811f1c39a87ddd617937f63c2320551ce459ba69c6d022e33322594d40b9f2d2c6bc9937387718adc40dc5e57ea8e
+  checksum: 3624520abb5807ed8f57b1197e61c7b1ed770c56dfcaca66372d584ff50175225798bccb701f7ef129d62c5989070e1ee3a0aa2d84e56d9524dcf011a2bb1a52
   languageName: node
   linkType: hard
 
-"@typescript-eslint/utils@npm:5.61.0":
-  version: 5.61.0
-  resolution: "@typescript-eslint/utils@npm:5.61.0"
+"@typescript-eslint/utils@npm:5.62.0":
+  version: 5.62.0
+  resolution: "@typescript-eslint/utils@npm:5.62.0"
   dependencies:
     "@eslint-community/eslint-utils": ^4.2.0
     "@types/json-schema": ^7.0.9
     "@types/semver": ^7.3.12
-    "@typescript-eslint/scope-manager": 5.61.0
-    "@typescript-eslint/types": 5.61.0
-    "@typescript-eslint/typescript-estree": 5.61.0
+    "@typescript-eslint/scope-manager": 5.62.0
+    "@typescript-eslint/types": 5.62.0
+    "@typescript-eslint/typescript-estree": 5.62.0
     eslint-scope: ^5.1.1
     semver: ^7.3.7
   peerDependencies:
     eslint: ^6.0.0 || ^7.0.0 || ^8.0.0
-  checksum: 24efc1964e6c92db96fe0d9a390550e4f27e8f353e51a9b46bda03e6692ea5d40f398d539235a4ff0894e9e45dfcfb51df953ade2ae9d17a1421449625ce6f5a
+  checksum: ee9398c8c5db6d1da09463ca7bf36ed134361e20131ea354b2da16a5fdb6df9ba70c62a388d19f6eebb421af1786dbbd79ba95ddd6ab287324fc171c3e28d931
   languageName: node
   linkType: hard
 
-"@typescript-eslint/visitor-keys@npm:5.61.0":
-  version: 5.61.0
-  resolution: "@typescript-eslint/visitor-keys@npm:5.61.0"
+"@typescript-eslint/visitor-keys@npm:5.62.0":
+  version: 5.62.0
+  resolution: "@typescript-eslint/visitor-keys@npm:5.62.0"
   dependencies:
-    "@typescript-eslint/types": 5.61.0
+    "@typescript-eslint/types": 5.62.0
     eslint-visitor-keys: ^3.3.0
-  checksum: a8d589f61ddfc380787218da4d347e8f9aef0f82f4a93f1daee46786bda889a90961c7ec1b470db5e3261438a728fdfd956f5bda6ee2de22c4be2d2152d6e270
+  checksum: 976b05d103fe8335bef5c93ad3f76d781e3ce50329c0243ee0f00c0fcfb186c81df50e64bfdd34970148113f8ade90887f53e3c4938183afba830b4ba8e30a35
   languageName: node
   linkType: hard
 
 "@webassemblyjs/ast@npm:1.11.6, @webassemblyjs/ast@npm:^1.11.5":
   version: 1.11.6
   resolution: "@webassemblyjs/ast@npm:1.11.6"
   dependencies:
@@ -3938,14 +3925,28 @@
 "array-union@npm:^2.1.0":
   version: 2.1.0
   resolution: "array-union@npm:2.1.0"
   checksum: 5bee12395cba82da674931df6d0fea23c4aa4660cb3b338ced9f828782a65caa232573e6bf3968f23e0c5eb301764a382cef2f128b170a9dc59de0e36c39f98d
   languageName: node
   linkType: hard
 
+"arraybuffer.prototype.slice@npm:^1.0.1":
+  version: 1.0.1
+  resolution: "arraybuffer.prototype.slice@npm:1.0.1"
+  dependencies:
+    array-buffer-byte-length: ^1.0.0
+    call-bind: ^1.0.2
+    define-properties: ^1.2.0
+    get-intrinsic: ^1.2.1
+    is-array-buffer: ^3.0.2
+    is-shared-array-buffer: ^1.0.2
+  checksum: e3e9b2a3e988ebfeddce4c7e8f69df730c9e48cb04b0d40ff0874ce3d86b3d1339dd520ffde5e39c02610bc172ecfbd4bc93324b1cabd9554c44a56b131ce0ce
+  languageName: node
+  linkType: hard
+
 "arrify@npm:^1.0.1":
   version: 1.0.1
   resolution: "arrify@npm:1.0.1"
   checksum: 745075dd4a4624ff0225c331dacb99be501a515d39bcb7c84d24660314a6ec28e68131b137e6f7e16318170842ce97538cd298fc4cd6b2cc798e0b957f2747e7
   languageName: node
   linkType: hard
 
@@ -4009,46 +4010,46 @@
     "@types/babel__core": ^7.1.14
     "@types/babel__traverse": ^7.0.6
   checksum: 099b5254073b6bc985b6d2d045ad26fb8ed30ff8ae6404c4fe8ee7cd0e98a820f69e3dfb871c7c65aae0f4b65af77046244c07bb92d49ef9005c90eedf681539
   languageName: node
   linkType: hard
 
 "babel-plugin-polyfill-corejs2@npm:^0.4.4":
-  version: 0.4.4
-  resolution: "babel-plugin-polyfill-corejs2@npm:0.4.4"
+  version: 0.4.5
+  resolution: "babel-plugin-polyfill-corejs2@npm:0.4.5"
   dependencies:
     "@babel/compat-data": ^7.22.6
-    "@babel/helper-define-polyfill-provider": ^0.4.1
-    "@nicolo-ribaudo/semver-v6": ^6.3.3
+    "@babel/helper-define-polyfill-provider": ^0.4.2
+    semver: ^6.3.1
   peerDependencies:
-    "@babel/core": ^7.0.0-0
-  checksum: 0273f3d74ccbf78086a3b14bb11b1fb94933830f51c576a24229d75b3b91c8b357c3a381d4ab3146abf9b052fa4c33ec9368dd010ada9ee355e1d03ff64e1ff0
+    "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
+  checksum: 33a8e06aa54e2858d211c743d179f0487b03222f9ca1bfd7c4865bca243fca942a3358cb75f6bb894ed476cbddede834811fbd6903ff589f055821146f053e1a
   languageName: node
   linkType: hard
 
 "babel-plugin-polyfill-corejs3@npm:^0.8.2":
-  version: 0.8.2
-  resolution: "babel-plugin-polyfill-corejs3@npm:0.8.2"
+  version: 0.8.3
+  resolution: "babel-plugin-polyfill-corejs3@npm:0.8.3"
   dependencies:
-    "@babel/helper-define-polyfill-provider": ^0.4.1
+    "@babel/helper-define-polyfill-provider": ^0.4.2
     core-js-compat: ^3.31.0
   peerDependencies:
-    "@babel/core": ^7.0.0-0
-  checksum: 0bc3e9e0114eba18f4fea8a9ff5a6016cae73b74cb091290c3f75fd7b9e34e712ee26f95b52d796f283970d7c6256fb01196e3608e8db03f620e3389d56d37c6
+    "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
+  checksum: dcbb30e551702a82cfd4d2c375da2c317658e55f95e9edcda93b9bbfdcc8fb6e5344efcb144e04d3406859e7682afce7974c60ededd9f12072a48a83dd22a0da
   languageName: node
   linkType: hard
 
 "babel-plugin-polyfill-regenerator@npm:^0.5.1":
-  version: 0.5.1
-  resolution: "babel-plugin-polyfill-regenerator@npm:0.5.1"
+  version: 0.5.2
+  resolution: "babel-plugin-polyfill-regenerator@npm:0.5.2"
   dependencies:
-    "@babel/helper-define-polyfill-provider": ^0.4.1
+    "@babel/helper-define-polyfill-provider": ^0.4.2
   peerDependencies:
-    "@babel/core": ^7.0.0-0
-  checksum: 85a56d28b34586fbe482225fb6a9592fc793a459c5eea987a3427fb723c7aa2f76916348a9fc5e9ca48754ebf6086cfbb9226f4cd0cf9c6257f94553622562ed
+    "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
+  checksum: d962200f604016a9a09bc9b4aaf60a3db7af876bb65bcefaeac04d44ac9d9ec4037cf24ce117760cc141d7046b6394c7eb0320ba9665cb4a2ee64df2be187c93
   languageName: node
   linkType: hard
 
 "babel-preset-current-node-syntax@npm:^1.0.0":
   version: 1.0.1
   resolution: "babel-preset-current-node-syntax@npm:1.0.1"
   dependencies:
@@ -4229,17 +4230,17 @@
   version: 6.3.0
   resolution: "camelcase@npm:6.3.0"
   checksum: 8c96818a9076434998511251dcb2761a94817ea17dbdc37f47ac080bd088fc62c7369429a19e2178b993497132c8cbcf5cc1f44ba963e76782ba469c0474938d
   languageName: node
   linkType: hard
 
 "caniuse-lite@npm:^1.0.30001503":
-  version: 1.0.30001514
-  resolution: "caniuse-lite@npm:1.0.30001514"
-  checksum: ee2e90fe63cb59fb4a1515eb6b157f1c26d3ccba496b994b0f03088c39c282ee2fb8c160ad7b677ee196b5bb078b23f2f9474c32e4e47724f4d782de92bb8bbe
+  version: 1.0.30001517
+  resolution: "caniuse-lite@npm:1.0.30001517"
+  checksum: e4e87436ae1c4408cf4438aac22902b31eb03f3f5bad7f33bc518d12ffb35f3fd9395ccf7efc608ee046f90ce324ec6f7f26f8a8172b8c43c26a06ecee612a29
   languageName: node
   linkType: hard
 
 "chalk@npm:^2.0.0, chalk@npm:^2.3.0, chalk@npm:^2.4.1":
   version: 2.4.2
   resolution: "chalk@npm:2.4.2"
   dependencies:
@@ -4531,17 +4532,17 @@
     shebang-command: ^2.0.0
     which: ^2.0.1
   checksum: 671cc7c7288c3a8406f3c69a3ae2fc85555c04169e9d611def9a675635472614f1c0ed0ef80955d5b6d4e724f6ced67f0ad1bb006c2ea643488fcfef994d7f52
   languageName: node
   linkType: hard
 
 "css-functions-list@npm:^3.1.0":
-  version: 3.1.0
-  resolution: "css-functions-list@npm:3.1.0"
-  checksum: 8a7c9d4ae57cb2f01500263e65a21372048d359ca7aa6430a32a736fe2a421decfebe45e579124b9a158ec68aba2eadcd733e568495a7698240d9607d31f681b
+  version: 3.2.0
+  resolution: "css-functions-list@npm:3.2.0"
+  checksum: fe912ea852fad500aef9a4f04db9a0371c7b0eb1ac1a45fbd8df0156ae0538cee7492ebd620b9bb502fe5bf2b5ed3bf3c16b6659cf67c7144eff0b597bcc3891
   languageName: node
   linkType: hard
 
 "css-loader@npm:^6.7.1":
   version: 6.8.1
   resolution: "css-loader@npm:6.8.1"
   dependencies:
@@ -4810,17 +4811,17 @@
   version: 0.2.0
   resolution: "eastasianwidth@npm:0.2.0"
   checksum: 7d00d7cd8e49b9afa762a813faac332dee781932d6f2c848dc348939c4253f1d4564341b7af1d041853bc3f32c2ef141b58e0a4d9862c17a7f08f68df1e0f1ed
   languageName: node
   linkType: hard
 
 "electron-to-chromium@npm:^1.4.431":
-  version: 1.4.454
-  resolution: "electron-to-chromium@npm:1.4.454"
-  checksum: 26a756485b442be04a640b8733c3e0d1ad9630541e56906332b1a5f25ec0027647561ec98d0d2a5069a1aae3875c9751c6d1c6cb9ef400b2beabedc36da14ba1
+  version: 1.4.473
+  resolution: "electron-to-chromium@npm:1.4.473"
+  checksum: f7fe72d606d2256e020b1c9d1305af098c7798147f6293cc3f213b086c0982fc2121b3bcf65740e237c612089f435d722434c2419e994e434469d2d07a9feffa
   languageName: node
   linkType: hard
 
 "emittery@npm:^0.13.1":
   version: 0.13.1
   resolution: "emittery@npm:0.13.1"
   checksum: 2b089ab6306f38feaabf4f6f02792f9ec85fc054fda79f44f6790e61bbf6bc4e1616afb9b232e0c5ec5289a8a452f79bfa6d905a6fd64e94b49981f0934001c6
@@ -4910,24 +4911,25 @@
   dependencies:
     is-arrayish: ^0.2.1
   checksum: c1c2b8b65f9c91b0f9d75f0debaa7ec5b35c266c2cac5de412c1a6de86d4cbae04ae44e510378cb14d032d0645a36925d0186f8bb7367bcc629db256b743a001
   languageName: node
   linkType: hard
 
 "es-abstract@npm:^1.19.0, es-abstract@npm:^1.20.4":
-  version: 1.21.2
-  resolution: "es-abstract@npm:1.21.2"
+  version: 1.22.1
+  resolution: "es-abstract@npm:1.22.1"
   dependencies:
     array-buffer-byte-length: ^1.0.0
+    arraybuffer.prototype.slice: ^1.0.1
     available-typed-arrays: ^1.0.5
     call-bind: ^1.0.2
     es-set-tostringtag: ^2.0.1
     es-to-primitive: ^1.2.1
     function.prototype.name: ^1.1.5
-    get-intrinsic: ^1.2.0
+    get-intrinsic: ^1.2.1
     get-symbol-description: ^1.0.0
     globalthis: ^1.0.3
     gopd: ^1.0.1
     has: ^1.0.3
     has-property-descriptors: ^1.0.0
     has-proto: ^1.0.1
     has-symbols: ^1.0.3
@@ -4939,23 +4941,27 @@
     is-shared-array-buffer: ^1.0.2
     is-string: ^1.0.7
     is-typed-array: ^1.1.10
     is-weakref: ^1.0.2
     object-inspect: ^1.12.3
     object-keys: ^1.1.1
     object.assign: ^4.1.4
-    regexp.prototype.flags: ^1.4.3
+    regexp.prototype.flags: ^1.5.0
+    safe-array-concat: ^1.0.0
     safe-regex-test: ^1.0.0
     string.prototype.trim: ^1.2.7
     string.prototype.trimend: ^1.0.6
     string.prototype.trimstart: ^1.0.6
+    typed-array-buffer: ^1.0.0
+    typed-array-byte-length: ^1.0.0
+    typed-array-byte-offset: ^1.0.0
     typed-array-length: ^1.0.4
     unbox-primitive: ^1.0.2
-    which-typed-array: ^1.1.9
-  checksum: 037f55ee5e1cdf2e5edbab5524095a4f97144d95b94ea29e3611b77d852fd8c8a40e7ae7101fa6a759a9b9b1405f188c3c70928f2d3cd88d543a07fc0d5ad41a
+    which-typed-array: ^1.1.10
+  checksum: 614e2c1c3717cb8d30b6128ef12ea110e06fd7d75ad77091ca1c5dbfb00da130e62e4bbbbbdda190eada098a22b27fe0f99ae5a1171dac2c8663b1e8be8a3a9b
   languageName: node
   linkType: hard
 
 "es-module-lexer@npm:^1.2.1":
   version: 1.3.0
   resolution: "es-module-lexer@npm:1.3.0"
   checksum: 48fd9f504a9d2a894126f75c8b7ccc6273a289983e9b67255f165bfd9ae765d50100218251e94e702ca567826905ea2f7b3b4a0c4d74d3ce99cce3a2a606a238
@@ -5063,33 +5069,33 @@
     esrecurse: ^4.3.0
     estraverse: ^4.1.1
   checksum: 47e4b6a3f0cc29c7feedee6c67b225a2da7e155802c6ea13bbef4ac6b9e10c66cd2dcb987867ef176292bf4e64eccc680a49e35e9e9c669f4a02bac17e86abdb
   languageName: node
   linkType: hard
 
 "eslint-scope@npm:^7.2.0":
-  version: 7.2.0
-  resolution: "eslint-scope@npm:7.2.0"
+  version: 7.2.1
+  resolution: "eslint-scope@npm:7.2.1"
   dependencies:
     esrecurse: ^4.3.0
     estraverse: ^5.2.0
-  checksum: 64591a2d8b244ade9c690b59ef238a11d5c721a98bcee9e9f445454f442d03d3e04eda88e95a4daec558220a99fa384309d9faae3d459bd40e7a81b4063980ae
+  checksum: dccda5c8909216f6261969b72c77b95e385f9086bed4bc09d8a6276df8439d8f986810fd9ac3bd02c94c0572cefc7fdbeae392c69df2e60712ab8263986522c5
   languageName: node
   linkType: hard
 
 "eslint-visitor-keys@npm:^3.3.0, eslint-visitor-keys@npm:^3.4.1":
   version: 3.4.1
   resolution: "eslint-visitor-keys@npm:3.4.1"
   checksum: f05121d868202736b97de7d750847a328fcfa8593b031c95ea89425333db59676ac087fa905eba438d0a3c5769632f828187e0c1a0d271832a2153c1d3661c2c
   languageName: node
   linkType: hard
 
 "eslint@npm:^8.36.0":
-  version: 8.44.0
-  resolution: "eslint@npm:8.44.0"
+  version: 8.45.0
+  resolution: "eslint@npm:8.45.0"
   dependencies:
     "@eslint-community/eslint-utils": ^4.2.0
     "@eslint-community/regexpp": ^4.4.0
     "@eslint/eslintrc": ^2.1.0
     "@eslint/js": 8.44.0
     "@humanwhocodes/config-array": ^0.11.10
     "@humanwhocodes/module-importer": ^1.0.1
@@ -5108,42 +5114,40 @@
     fast-deep-equal: ^3.1.3
     file-entry-cache: ^6.0.1
     find-up: ^5.0.0
     glob-parent: ^6.0.2
     globals: ^13.19.0
     graphemer: ^1.4.0
     ignore: ^5.2.0
-    import-fresh: ^3.0.0
     imurmurhash: ^0.1.4
     is-glob: ^4.0.0
     is-path-inside: ^3.0.3
     js-yaml: ^4.1.0
     json-stable-stringify-without-jsonify: ^1.0.1
     levn: ^0.4.1
     lodash.merge: ^4.6.2
     minimatch: ^3.1.2
     natural-compare: ^1.4.0
     optionator: ^0.9.3
     strip-ansi: ^6.0.1
-    strip-json-comments: ^3.1.0
     text-table: ^0.2.0
   bin:
     eslint: bin/eslint.js
-  checksum: d06309ce4aafb9d27d558c8e5e5aa5cba3bbec3ce8ceccbc7d4b7a35f2b67fd40189159155553270e2e6febeb69bd8a3b60d6241c8f5ddc2ef1702ccbd328501
+  checksum: 3e6dcce5cc43c5e301662db88ee26d1d188b22c177b9f104d7eefd1191236980bd953b3670fe2fac287114b26d7c5420ab48407d7ea1c3a446d6313c000009da
   languageName: node
   linkType: hard
 
 "espree@npm:^9.6.0":
-  version: 9.6.0
-  resolution: "espree@npm:9.6.0"
+  version: 9.6.1
+  resolution: "espree@npm:9.6.1"
   dependencies:
     acorn: ^8.9.0
     acorn-jsx: ^5.3.2
     eslint-visitor-keys: ^3.4.1
-  checksum: 1287979510efb052a6a97c73067ea5d0a40701b29adde87bbe2d3eb1667e39ca55e8129e20e2517fed3da570150e7ef470585228459a8f3e3755f45007a1c662
+  checksum: eb8c149c7a2a77b3f33a5af80c10875c3abd65450f60b8af6db1bfcfa8f101e21c1e56a561c6dc13b848e18148d43469e7cd208506238554fb5395a9ea5a1ab9
   languageName: node
   linkType: hard
 
 "esprima@npm:^4.0.0, esprima@npm:^4.0.1":
   version: 4.0.1
   resolution: "esprima@npm:4.0.1"
   bin:
@@ -5255,23 +5259,23 @@
   version: 1.3.0
   resolution: "fast-diff@npm:1.3.0"
   checksum: d22d371b994fdc8cce9ff510d7b8dc4da70ac327bcba20df607dd5b9cae9f908f4d1028f5fe467650f058d1e7270235ae0b8230809a262b4df587a3b3aa216c3
   languageName: node
   linkType: hard
 
 "fast-glob@npm:^3.2.12, fast-glob@npm:^3.2.9":
-  version: 3.3.0
-  resolution: "fast-glob@npm:3.3.0"
+  version: 3.3.1
+  resolution: "fast-glob@npm:3.3.1"
   dependencies:
     "@nodelib/fs.stat": ^2.0.2
     "@nodelib/fs.walk": ^1.2.3
     glob-parent: ^5.1.2
     merge2: ^1.3.0
     micromatch: ^4.0.4
-  checksum: 20df62be28eb5426fe8e40e0d05601a63b1daceb7c3d87534afcad91bdcf1e4b1743cf2d5247d6e225b120b46df0b9053a032b2691ba34ee121e033acd81f547
+  checksum: b6f3add6403e02cf3a798bfbb1183d0f6da2afd368f27456010c0bc1f9640aea308243d4cb2c0ab142f618276e65ecb8be1661d7c62a7b4e5ba774b9ce5432e5
   languageName: node
   linkType: hard
 
 "fast-json-stable-stringify@npm:2.x, fast-json-stable-stringify@npm:^2.0.0, fast-json-stable-stringify@npm:^2.1.0":
   version: 2.1.0
   resolution: "fast-json-stable-stringify@npm:2.1.0"
   checksum: b191531e36c607977e5b1c47811158733c34ccb3bfde92c44798929e9b4154884378536d26ad90dfecd32e1ffc09c545d23535ad91b3161a27ddbb8ebe0cbecb
@@ -5516,15 +5520,15 @@
 "get-caller-file@npm:^2.0.5":
   version: 2.0.5
   resolution: "get-caller-file@npm:2.0.5"
   checksum: b9769a836d2a98c3ee734a88ba712e62703f1df31b94b784762c433c27a386dd6029ff55c2a920c392e33657d80191edbf18c61487e198844844516f843496b9
   languageName: node
   linkType: hard
 
-"get-intrinsic@npm:^1.0.2, get-intrinsic@npm:^1.1.1, get-intrinsic@npm:^1.1.3, get-intrinsic@npm:^1.2.0":
+"get-intrinsic@npm:^1.0.2, get-intrinsic@npm:^1.1.1, get-intrinsic@npm:^1.1.3, get-intrinsic@npm:^1.2.0, get-intrinsic@npm:^1.2.1":
   version: 1.2.1
   resolution: "get-intrinsic@npm:1.2.1"
   dependencies:
     function-bind: ^1.1.1
     has: ^1.0.3
     has-proto: ^1.0.1
     has-symbols: ^1.0.3
@@ -5933,15 +5937,15 @@
 "ignore@npm:^5.2.0, ignore@npm:^5.2.1":
   version: 5.2.4
   resolution: "ignore@npm:5.2.4"
   checksum: 3d4c309c6006e2621659311783eaea7ebcd41fe4ca1d78c91c473157ad6666a57a2df790fe0d07a12300d9aac2888204d7be8d59f9aaf665b1c7fcdb432517ef
   languageName: node
   linkType: hard
 
-"import-fresh@npm:^3.0.0, import-fresh@npm:^3.2.1":
+"import-fresh@npm:^3.2.1":
   version: 3.3.0
   resolution: "import-fresh@npm:3.3.0"
   dependencies:
     parent-module: ^1.0.0
     resolve-from: ^4.0.0
   checksum: 2cacfad06e652b1edc50be650f7ec3be08c5e5a6f6d12d035c440a42a8cc028e60a5b99ca08a77ab4d6b1346da7d971915828f33cdab730d3d42f08242d09baa
   languageName: node
@@ -6229,35 +6233,38 @@
   dependencies:
     has-symbols: ^1.0.2
   checksum: 92805812ef590738d9de49d677cd17dfd486794773fb6fa0032d16452af46e9b91bb43ffe82c983570f015b37136f4b53b28b8523bfb10b0ece7a66c31a54510
   languageName: node
   linkType: hard
 
 "is-typed-array@npm:^1.1.10, is-typed-array@npm:^1.1.9":
-  version: 1.1.10
-  resolution: "is-typed-array@npm:1.1.10"
+  version: 1.1.12
+  resolution: "is-typed-array@npm:1.1.12"
   dependencies:
-    available-typed-arrays: ^1.0.5
-    call-bind: ^1.0.2
-    for-each: ^0.3.3
-    gopd: ^1.0.1
-    has-tostringtag: ^1.0.0
-  checksum: aac6ecb59d4c56a1cdeb69b1f129154ef462bbffe434cb8a8235ca89b42f258b7ae94073c41b3cb7bce37f6a1733ad4499f07882d5d5093a7ba84dfc4ebb8017
+    which-typed-array: ^1.1.11
+  checksum: 4c89c4a3be07186caddadf92197b17fda663a9d259ea0d44a85f171558270d36059d1c386d34a12cba22dfade5aba497ce22778e866adc9406098c8fc4771796
   languageName: node
   linkType: hard
 
 "is-weakref@npm:^1.0.2":
   version: 1.0.2
   resolution: "is-weakref@npm:1.0.2"
   dependencies:
     call-bind: ^1.0.2
   checksum: 95bd9a57cdcb58c63b1c401c60a474b0f45b94719c30f548c891860f051bc2231575c290a6b420c6bc6e7ed99459d424c652bd5bf9a1d5259505dc35b4bf83de
   languageName: node
   linkType: hard
 
+"isarray@npm:^2.0.5":
+  version: 2.0.5
+  resolution: "isarray@npm:2.0.5"
+  checksum: bd5bbe4104438c4196ba58a54650116007fa0262eccef13a4c55b2e09a5b36b59f1e75b9fcc49883dd9d4953892e6fc007eef9e9155648ceea036e184b0f930a
+  languageName: node
+  linkType: hard
+
 "isexe@npm:^2.0.0":
   version: 2.0.0
   resolution: "isexe@npm:2.0.0"
   checksum: 26bf6c5480dda5161c820c5b5c751ae1e766c587b1f951ea3fcfc973bafb7831ae5b54a31a69bd670220e42e99ec154475025a468eae58ea262f813fdc8d1c62
   languageName: node
   linkType: hard
 
@@ -6292,21 +6299,21 @@
     istanbul-lib-coverage: ^3.2.0
     semver: ^6.3.0
   checksum: bf16f1803ba5e51b28bbd49ed955a736488381e09375d830e42ddeb403855b2006f850711d95ad726f2ba3f1ae8e7366de7e51d2b9ac67dc4d80191ef7ddf272
   languageName: node
   linkType: hard
 
 "istanbul-lib-report@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "istanbul-lib-report@npm:3.0.0"
+  version: 3.0.1
+  resolution: "istanbul-lib-report@npm:3.0.1"
   dependencies:
     istanbul-lib-coverage: ^3.0.0
-    make-dir: ^3.0.0
+    make-dir: ^4.0.0
     supports-color: ^7.1.0
-  checksum: 3f29eb3f53c59b987386e07fe772d24c7f58c6897f34c9d7a296f4000de7ae3de9eb95c3de3df91dc65b134c84dee35c54eee572a56243e8907c48064e34ff1b
+  checksum: fd17a1b879e7faf9bb1dc8f80b2a16e9f5b7b8498fe6ed580a618c34df0bfe53d2abd35bf8a0a00e628fb7405462576427c7df20bbe4148d19c14b431c974b21
   languageName: node
   linkType: hard
 
 "istanbul-lib-source-maps@npm:^4.0.0":
   version: 4.0.1
   resolution: "istanbul-lib-source-maps@npm:4.0.1"
   dependencies:
@@ -6314,33 +6321,33 @@
     istanbul-lib-coverage: ^3.0.0
     source-map: ^0.6.1
   checksum: 21ad3df45db4b81852b662b8d4161f6446cd250c1ddc70ef96a585e2e85c26ed7cd9c2a396a71533cfb981d1a645508bc9618cae431e55d01a0628e7dec62ef2
   languageName: node
   linkType: hard
 
 "istanbul-reports@npm:^3.1.3":
-  version: 3.1.5
-  resolution: "istanbul-reports@npm:3.1.5"
+  version: 3.1.6
+  resolution: "istanbul-reports@npm:3.1.6"
   dependencies:
     html-escaper: ^2.0.0
     istanbul-lib-report: ^3.0.0
-  checksum: 7867228f83ed39477b188ea07e7ccb9b4f5320b6f73d1db93a0981b7414fa4ef72d3f80c4692c442f90fc250d9406e71d8d7ab65bb615cb334e6292b73192b89
+  checksum: 44c4c0582f287f02341e9720997f9e82c071627e1e862895745d5f52ec72c9b9f38e1d12370015d2a71dcead794f34c7732aaef3fab80a24bc617a21c3d911d6
   languageName: node
   linkType: hard
 
 "jackspeak@npm:^2.0.3":
-  version: 2.2.1
-  resolution: "jackspeak@npm:2.2.1"
+  version: 2.2.2
+  resolution: "jackspeak@npm:2.2.2"
   dependencies:
     "@isaacs/cliui": ^8.0.2
     "@pkgjs/parseargs": ^0.11.0
   dependenciesMeta:
     "@pkgjs/parseargs":
       optional: true
-  checksum: e29291c0d0f280a063fa18fbd1e891ab8c2d7519fd34052c0ebde38538a15c603140d60c2c7f432375ff7ee4c5f1c10daa8b2ae19a97c3d4affe308c8360c1df
+  checksum: 7b1468dd910afc00642db87448f24b062346570b8b47531409aa9012bcb95fdf7ec2b1c48edbb8b57a938c08391f8cc01b5034fc335aa3a2e74dbcc0ee5c555a
   languageName: node
   linkType: hard
 
 "jest-changed-files@npm:^29.5.0":
   version: 29.5.0
   resolution: "jest-changed-files@npm:29.5.0"
   dependencies:
@@ -7208,20 +7215,20 @@
 "lru-cache@npm:^9.1.1 || ^10.0.0":
   version: 10.0.0
   resolution: "lru-cache@npm:10.0.0"
   checksum: 18f101675fe283bc09cda0ef1e3cc83781aeb8373b439f086f758d1d91b28730950db785999cd060d3c825a8571c03073e8c14512b6655af2188d623031baf50
   languageName: node
   linkType: hard
 
-"make-dir@npm:^3.0.0":
-  version: 3.1.0
-  resolution: "make-dir@npm:3.1.0"
+"make-dir@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "make-dir@npm:4.0.0"
   dependencies:
-    semver: ^6.0.0
-  checksum: 484200020ab5a1fdf12f393fe5f385fc8e4378824c940fba1729dcd198ae4ff24867bc7a5646331e50cead8abff5d9270c456314386e629acec6dff4b8016b78
+    semver: ^7.5.3
+  checksum: bf0731a2dd3aab4db6f3de1585cea0b746bb73eb5a02e3d8d72757e376e64e6ada190b1eddcde5b2f24a81b688a9897efd5018737d05e02e2a671dda9cff8a8a
   languageName: node
   linkType: hard
 
 "make-error@npm:1.x":
   version: 1.3.6
   resolution: "make-error@npm:1.3.6"
   checksum: b86e5e0e25f7f777b77fabd8e2cbf15737972869d852a22b7e73c17623928fccb826d8e46b9951501d3f20e51ad74ba8c59ed584f610526a48f8ccf88aaec402
@@ -7507,17 +7514,17 @@
   version: 5.0.0
   resolution: "minipass@npm:5.0.0"
   checksum: 425dab288738853fded43da3314a0b5c035844d6f3097a8e3b5b29b328da8f3c1af6fc70618b32c29ff906284cf6406b6841376f21caaadd0793c1d5a6a620ea
   languageName: node
   linkType: hard
 
 "minipass@npm:^5.0.0 || ^6.0.2 || ^7.0.0":
-  version: 7.0.1
-  resolution: "minipass@npm:7.0.1"
-  checksum: fedd1293f6a1b4e406c242a1cecfb75d0a81422bb2c365d999e33a88642fb68d70a89d95b550e08c640b3c0d9162829310e0c58b9b846b9218de25779818c709
+  version: 7.0.2
+  resolution: "minipass@npm:7.0.2"
+  checksum: 46776de732eb7cef2c7404a15fb28c41f5c54a22be50d47b03c605bf21f5c18d61a173c0a20b49a97e7a65f78d887245066410642551e45fffe04e9ac9e325bc
   languageName: node
   linkType: hard
 
 "minizlib@npm:^2.1.1, minizlib@npm:^2.1.2":
   version: 2.1.2
   resolution: "minizlib@npm:2.1.2"
   dependencies:
@@ -8093,21 +8100,21 @@
   version: 4.2.0
   resolution: "postcss-value-parser@npm:4.2.0"
   checksum: 819ffab0c9d51cf0acbabf8996dffbfafbafa57afc0e4c98db88b67f2094cb44488758f06e5da95d7036f19556a4a732525e84289a425f4f6fd8e412a9d7442f
   languageName: node
   linkType: hard
 
 "postcss@npm:^8.3.11, postcss@npm:^8.4.19, postcss@npm:^8.4.21":
-  version: 8.4.25
-  resolution: "postcss@npm:8.4.25"
+  version: 8.4.27
+  resolution: "postcss@npm:8.4.27"
   dependencies:
     nanoid: ^3.3.6
     picocolors: ^1.0.0
     source-map-js: ^1.0.2
-  checksum: 9ed3ab8af43ad5210c28f56f916fd9b8c9f94fbeaebbf645dcf579bc28bdd8056c2a7ecc934668d399b81fedb6128f0c4b299f931e50454964bc911c25a3a0a2
+  checksum: 1cdd0c298849df6cd65f7e646a3ba36870a37b65f55fd59d1a165539c263e9b4872a402bf4ed1ca1bc31f58b68b2835545e33ea1a23b161a1f8aa6d5ded81e78
   languageName: node
   linkType: hard
 
 "prelude-ls@npm:^1.2.1":
   version: 1.2.1
   resolution: "prelude-ls@npm:1.2.1"
   checksum: cd192ec0d0a8e4c6da3bb80e4f62afe336df3f76271ac6deb0e6a36187133b6073a19e9727a1ff108cd8b9982e4768850d413baa71214dd80c7979617dca827a
@@ -8359,15 +8366,15 @@
   resolution: "regenerator-transform@npm:0.15.1"
   dependencies:
     "@babel/runtime": ^7.8.4
   checksum: 2d15bdeadbbfb1d12c93f5775493d85874dbe1d405bec323da5c61ec6e701bc9eea36167483e1a5e752de9b2df59ab9a2dfff6bf3784f2b28af2279a673d29a4
   languageName: node
   linkType: hard
 
-"regexp.prototype.flags@npm:^1.4.3":
+"regexp.prototype.flags@npm:^1.5.0":
   version: 1.5.0
   resolution: "regexp.prototype.flags@npm:1.5.0"
   dependencies:
     call-bind: ^1.0.2
     define-properties: ^1.2.0
     functions-have-names: ^1.2.3
   checksum: c541687cdbdfff1b9a07f6e44879f82c66bbf07665f9a7544c5fd16acdb3ec8d1436caab01662d2fbcad403f3499d49ab0b77fbc7ef29ef961d98cc4bc9755b4
@@ -8517,14 +8524,26 @@
   resolution: "run-parallel@npm:1.2.0"
   dependencies:
     queue-microtask: ^1.2.2
   checksum: cb4f97ad25a75ebc11a8ef4e33bb962f8af8516bb2001082ceabd8902e15b98f4b84b4f8a9b222e5d57fc3bd1379c483886ed4619367a7680dad65316993021d
   languageName: node
   linkType: hard
 
+"safe-array-concat@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "safe-array-concat@npm:1.0.0"
+  dependencies:
+    call-bind: ^1.0.2
+    get-intrinsic: ^1.2.0
+    has-symbols: ^1.0.3
+    isarray: ^2.0.5
+  checksum: f43cb98fe3b566327d0c09284de2b15fb85ae964a89495c1b1a5d50c7c8ed484190f4e5e71aacc167e16231940079b326f2c0807aea633d47cc7322f40a6b57f
+  languageName: node
+  linkType: hard
+
 "safe-buffer@npm:^5.1.0, safe-buffer@npm:~5.2.0":
   version: 5.2.1
   resolution: "safe-buffer@npm:5.2.1"
   checksum: b99c4b41fdd67a6aaf280fcd05e9ffb0813654894223afb78a31f14a19ad220bba8aba1cb14eddce1fcfb037155fe6de4e861784eb434f7d11ed58d1e70dd491
   languageName: node
   linkType: hard
 
@@ -8609,28 +8628,28 @@
     ajv-formats: ^2.1.1
     ajv-keywords: ^5.1.0
   checksum: 26a0463d47683258106e6652e9aeb0823bf0b85843039e068b57da1892f7ae6b6b1094d48e9ed5ba5cbe9f7166469d880858b9d91abe8bd249421eb813850cde
   languageName: node
   linkType: hard
 
 "semver@npm:2 || 3 || 4 || 5, semver@npm:^5.4.1, semver@npm:^5.5.0":
-  version: 5.7.1
-  resolution: "semver@npm:5.7.1"
+  version: 5.7.2
+  resolution: "semver@npm:5.7.2"
   bin:
-    semver: ./bin/semver
-  checksum: 57fd0acfd0bac382ee87cd52cd0aaa5af086a7dc8d60379dfe65fea491fb2489b6016400813930ecd61fd0952dae75c115287a1b16c234b1550887117744dfaf
+    semver: bin/semver
+  checksum: fb4ab5e0dd1c22ce0c937ea390b4a822147a9c53dbd2a9a0132f12fe382902beef4fbf12cf51bb955248d8d15874ce8cd89532569756384f994309825f10b686
   languageName: node
   linkType: hard
 
-"semver@npm:^6.0.0, semver@npm:^6.3.0":
-  version: 6.3.0
-  resolution: "semver@npm:6.3.0"
+"semver@npm:^6.3.0, semver@npm:^6.3.1":
+  version: 6.3.1
+  resolution: "semver@npm:6.3.1"
   bin:
-    semver: ./bin/semver.js
-  checksum: 1b26ecf6db9e8292dd90df4e781d91875c0dcc1b1909e70f5d12959a23c7eebb8f01ea581c00783bbee72ceeaad9505797c381756326073850dc36ed284b21b9
+    semver: bin/semver.js
+  checksum: ae47d06de28836adb9d3e25f22a92943477371292d9b665fb023fae278d345d508ca1958232af086d85e0155aee22e313e100971898bbb8d5d89b8b1d4054ca2
   languageName: node
   linkType: hard
 
 "semver@npm:^7.3.4, semver@npm:^7.3.5, semver@npm:^7.3.7, semver@npm:^7.3.8, semver@npm:^7.5.3":
   version: 7.5.4
   resolution: "semver@npm:7.5.4"
   dependencies:
@@ -9052,15 +9071,15 @@
   resolution: "strip-indent@npm:3.0.0"
   dependencies:
     min-indent: ^1.0.0
   checksum: 18f045d57d9d0d90cd16f72b2313d6364fd2cb4bf85b9f593523ad431c8720011a4d5f08b6591c9d580f446e78855c5334a30fb91aa1560f5d9f95ed1b4a0530
   languageName: node
   linkType: hard
 
-"strip-json-comments@npm:^3.1.0, strip-json-comments@npm:^3.1.1":
+"strip-json-comments@npm:^3.1.1":
   version: 3.1.1
   resolution: "strip-json-comments@npm:3.1.1"
   checksum: 492f73e27268f9b1c122733f28ecb0e7e8d8a531a6662efbd08e22cccb3f9475e90a1b82cab06a392f6afae6d2de636f977e231296400d0ec5304ba70f166443
   languageName: node
   linkType: hard
 
 "style-loader@npm:^3.3.1, style-loader@npm:~3.3.1":
@@ -9289,24 +9308,24 @@
     uglify-js:
       optional: true
   checksum: 41705713d6f9cb83287936b21e27c658891c78c4392159f5148b5623f0e8c48559869779619b058382a4c9758e7820ea034695e57dc7c474b4962b79f553bc5f
   languageName: node
   linkType: hard
 
 "terser@npm:^5.16.8":
-  version: 5.18.2
-  resolution: "terser@npm:5.18.2"
+  version: 5.19.2
+  resolution: "terser@npm:5.19.2"
   dependencies:
     "@jridgewell/source-map": ^0.3.3
     acorn: ^8.8.2
     commander: ^2.20.0
     source-map-support: ~0.5.20
   bin:
     terser: bin/terser
-  checksum: 50988412533bfd5a07294df002d772ad5b1277a9d1164dd19c8876a2094ced7b78fcf36cb32122a9a5238ba2597d77178a2385dfc6c4d506622309493f613cf4
+  checksum: e059177775b4d4f4cff219ad89293175aefbd1b081252270444dc83e42a2c5f07824eb2a85eae6e22ef6eb7ef04b21af36dd7d1dd7cfb93912310e57d416a205
   languageName: node
   linkType: hard
 
 "test-exclude@npm:^6.0.0":
   version: 6.0.0
   resolution: "test-exclude@npm:6.0.0"
   dependencies:
@@ -9489,14 +9508,50 @@
 "type-fest@npm:^0.8.1":
   version: 0.8.1
   resolution: "type-fest@npm:0.8.1"
   checksum: d61c4b2eba24009033ae4500d7d818a94fd6d1b481a8111612ee141400d5f1db46f199c014766b9fa9b31a6a7374d96fc748c6d688a78a3ce5a33123839becb7
   languageName: node
   linkType: hard
 
+"typed-array-buffer@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "typed-array-buffer@npm:1.0.0"
+  dependencies:
+    call-bind: ^1.0.2
+    get-intrinsic: ^1.2.1
+    is-typed-array: ^1.1.10
+  checksum: 3e0281c79b2a40cd97fe715db803884301993f4e8c18e8d79d75fd18f796e8cd203310fec8c7fdb5e6c09bedf0af4f6ab8b75eb3d3a85da69328f28a80456bd3
+  languageName: node
+  linkType: hard
+
+"typed-array-byte-length@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "typed-array-byte-length@npm:1.0.0"
+  dependencies:
+    call-bind: ^1.0.2
+    for-each: ^0.3.3
+    has-proto: ^1.0.1
+    is-typed-array: ^1.1.10
+  checksum: b03db16458322b263d87a702ff25388293f1356326c8a678d7515767ef563ef80e1e67ce648b821ec13178dd628eb2afdc19f97001ceae7a31acf674c849af94
+  languageName: node
+  linkType: hard
+
+"typed-array-byte-offset@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "typed-array-byte-offset@npm:1.0.0"
+  dependencies:
+    available-typed-arrays: ^1.0.5
+    call-bind: ^1.0.2
+    for-each: ^0.3.3
+    has-proto: ^1.0.1
+    is-typed-array: ^1.1.10
+  checksum: 04f6f02d0e9a948a95fbfe0d5a70b002191fae0b8fe0fe3130a9b2336f043daf7a3dda56a31333c35a067a97e13f539949ab261ca0f3692c41603a46a94e960b
+  languageName: node
+  linkType: hard
+
 "typed-array-length@npm:^1.0.4":
   version: 1.0.4
   resolution: "typed-array-length@npm:1.0.4"
   dependencies:
     call-bind: ^1.0.2
     for-each: ^0.3.3
     is-typed-array: ^1.1.9
@@ -9878,16 +9933,16 @@
   version: 3.2.3
   resolution: "webpack-sources@npm:3.2.3"
   checksum: 989e401b9fe3536529e2a99dac8c1bdc50e3a0a2c8669cbafad31271eadd994bc9405f88a3039cd2e29db5e6d9d0926ceb7a1a4e7409ece021fe79c37d9c4607
   languageName: node
   linkType: hard
 
 "webpack@npm:^5.76.1":
-  version: 5.88.1
-  resolution: "webpack@npm:5.88.1"
+  version: 5.88.2
+  resolution: "webpack@npm:5.88.2"
   dependencies:
     "@types/eslint-scope": ^3.7.3
     "@types/estree": ^1.0.0
     "@webassemblyjs/ast": ^1.11.5
     "@webassemblyjs/wasm-edit": ^1.11.5
     "@webassemblyjs/wasm-parser": ^1.11.5
     acorn: ^8.7.1
@@ -9910,15 +9965,15 @@
     watchpack: ^2.4.0
     webpack-sources: ^3.2.3
   peerDependenciesMeta:
     webpack-cli:
       optional: true
   bin:
     webpack: bin/webpack.js
-  checksum: 726e7e05ab2e7c142609a673dd6aa1a711ed97f349418a2a393d650c5ddad172d191257f60e1e37f6b2a77261571c202aabd5ce9240791a686774f0801cf5ec2
+  checksum: 79476a782da31a21f6dd38fbbd06b68da93baf6a62f0d08ca99222367f3b8668f5a1f2086b7bb78e23172e31fa6df6fa7ab09b25e827866c4fc4dc2b30443ce2
   languageName: node
   linkType: hard
 
 "whatwg-encoding@npm:^2.0.0":
   version: 2.0.0
   resolution: "whatwg-encoding@npm:2.0.0"
   dependencies:
@@ -9981,25 +10036,24 @@
     is-number-object: ^1.0.4
     is-string: ^1.0.5
     is-symbol: ^1.0.3
   checksum: 53ce774c7379071729533922adcca47220228405e1895f26673bbd71bdf7fb09bee38c1d6399395927c6289476b5ae0629863427fd151491b71c4b6cb04f3a5e
   languageName: node
   linkType: hard
 
-"which-typed-array@npm:^1.1.9":
-  version: 1.1.9
-  resolution: "which-typed-array@npm:1.1.9"
+"which-typed-array@npm:^1.1.10, which-typed-array@npm:^1.1.11":
+  version: 1.1.11
+  resolution: "which-typed-array@npm:1.1.11"
   dependencies:
     available-typed-arrays: ^1.0.5
     call-bind: ^1.0.2
     for-each: ^0.3.3
     gopd: ^1.0.1
     has-tostringtag: ^1.0.0
-    is-typed-array: ^1.1.10
-  checksum: fe0178ca44c57699ca2c0e657b64eaa8d2db2372a4e2851184f568f98c478ae3dc3fdb5f7e46c384487046b0cf9e23241423242b277e03e8ba3dabc7c84c98ef
+  checksum: 711ffc8ef891ca6597b19539075ec3e08bb9b4c2ca1f78887e3c07a977ab91ac1421940505a197758fb5939aa9524976d0a5bbcac34d07ed6faa75cedbb17206
   languageName: node
   linkType: hard
 
 "which@npm:^1.2.9, which@npm:^1.3.1":
   version: 1.3.1
   resolution: "which@npm:1.3.1"
   dependencies:
@@ -10194,19 +10248,19 @@
     y18n: ^5.0.5
     yargs-parser: ^21.1.1
   checksum: 73b572e863aa4a8cbef323dd911d79d193b772defd5a51aab0aca2d446655216f5002c42c5306033968193bdbf892a7a4c110b0d77954a7fdf563e653967b56a
   languageName: node
   linkType: hard
 
 "yjs@npm:^13.5.0, yjs@npm:^13.5.40":
-  version: 13.6.6
-  resolution: "yjs@npm:13.6.6"
+  version: 13.6.7
+  resolution: "yjs@npm:13.6.7"
   dependencies:
     lib0: ^0.2.74
-  checksum: c69cb9a084aa433e813f6d0a191ebad5800a9a7098f7c6715952e4f8e5fc23270e3b8d7d747e1b0d0f1adca5f6efe01019654389eddb3977006814c4e2ff7ce6
+  checksum: 8e89257c8b565ab97cf3354fca2ce0b6bc3d1abe90b9d45a218a94b35da372c88d2411b353ed8ca03a6619004c4da76c96f7c203c38506c3758c9f8c1a730ca4
   languageName: node
   linkType: hard
 
 "yocto-queue@npm:^0.1.0":
   version: 0.1.0
   resolution: "yocto-queue@npm:0.1.0"
   checksum: f77b3d8d00310def622123df93d4ee654fc6a0096182af8bd60679ddcdfb3474c56c6c7190817c84a2785648cdee9d721c0154eb45698c62176c322fb46fc700
```

### Comparing `chapyter-0.2.0/chapyter/__init__.py` & `chapyter-0.3.0/chapyter/__init__.py`

 * *Files identical despite different names*

### Comparing `chapyter-0.2.0/chapyter/programs.py` & `chapyter-0.3.0/chapyter/programs.py`

 * *Files identical despite different names*

### Comparing `chapyter-0.2.0/chapyter/labextension/package.json` & `chapyter-0.3.0/chapyter/labextension/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9795833333333333%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.674ce065681604c8f0d3.js'}}",*

 * * "'version'": "'0.3.0'"}*

```diff
@@ -105,15 +105,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/chapyter/chapyter",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.d053f9dc5154f37a9b90.js",
+            "load": "static/remoteEntry.674ce065681604c8f0d3.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "chapyter/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -187,12 +187,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0",
+    "version": "0.3.0",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `chapyter-0.2.0/chapyter/labextension/schemas/@shannon-shen/chapyter/package.json.orig` & `chapyter-0.3.0/chapyter/labextension/schemas/@shannon-shen/chapyter/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'0.3.0'"}*

```diff
@@ -182,12 +182,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0",
+    "version": "0.3.0",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `chapyter-0.2.0/chapyter/labextension/static/568.0a4b756444d1e43aa84c.js` & `chapyter-0.3.0/chapyter/labextension/static/568.630c95d80cb75b8352da.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 "use strict";
 (self.webpackChunk_shannon_shen_chapyter = self.webpackChunk_shannon_shen_chapyter || []).push([
     [568], {
         568: (e, t, l) => {
             l.r(t), l.d(t, {
                 default: () => r
             });
-            var n = l(919),
-                o = l(850);
+            var n = l(861),
+                o = l(882);
             const d = "jp-chapyter-chat-executing";
 
             function a(e) {
                 if ((0, o.isCodeCellModel)(e.model)) {
                     let t = e.model.getMetadata("ChapyterCell") || null;
                     if (t && "generated" === t.cellType) return !1
                 }
@@ -66,15 +66,15 @@
                                     }(o.content, e.model.executionCount);
                                     t && (t.model.setMetadata("ChapyterCell", {
                                         cellType: "generated",
                                         linkedCellId: e.model.id
                                     }), console.log(l), l || (i(o.content, t.model.id), n.NotebookActions.run(o.content, o.sessionContext), t.inputHidden = !0), i(o.content, t.model.id), l || n.NotebookActions.selectBelow(o.content), e.model.setMetadata("ChapyterCell", {
                                         cellType: "original",
                                         linkedCellId: t.model.id
-                                    }), e.addClass("jp-chapyter-chat"), e.toggleClass(d), t.addClass("jp-chapyter-assistance"))
+                                    }), e.addClass("jp-chapyter-chat"), e.removeClass(d), t.addClass("jp-chapyter-assistance"))
                                 }
                             }
                         }
                     })), n.NotebookActions.executionScheduled.connect(((e, l) => {
                         var n;
                         let o = l.cell;
                         if (s(o) && a(o)) {
```

### Comparing `chapyter-0.2.0/chapyter/labextension/static/747.217e756827eb66a6f3d4.js` & `chapyter-0.3.0/chapyter/labextension/static/747.217e756827eb66a6f3d4.js`

 * *Files identical despite different names*

### Comparing `chapyter-0.2.0/chapyter/labextension/static/remoteEntry.d053f9dc5154f37a9b90.js` & `chapyter-0.3.0/chapyter/labextension/static/remoteEntry.674ce065681604c8f0d3.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, o, a, i, u, s, l, f, d, c, h, p, v, b, g, m, y, w, S, j = {
-            875: (e, r, t) => {
+            983: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -43,18 +43,18 @@
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        568: "0a4b756444d1e43aa84c",
+        568: "630c95d80cb75b8352da",
         747: "217e756827eb66a6f3d4"
     } [e] + ".js?v=" + {
-        568: "0a4b756444d1e43aa84c",
+        568: "630c95d80cb75b8352da",
         747: "217e756827eb66a6f3d4"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => E.e(568).then((() => () => E(568))),
                         from: i,
                         eager: !1
                     })
-                })("@shannon-shen/chapyter", "0.2.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("@shannon-shen/chapyter", "0.3.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -219,18 +219,18 @@
         "undefined" != typeof console && console.warn && console.warn(e)
     }, p = (e, r, t, n) => {
         h(c(e, r, t, n))
     }, v = e => (e.loaded = 1, e.get()), g = (b = e => function(r, t, n, o) {
         var a = E.I(r);
         return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
     })(((e, r, t, n) => (i(e, t), v(d(r, t, n) || p(r, e, t, n) || u(r, t))))), m = b(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), y = {}, w = {
-        850: () => g("default", "@jupyterlab/cells", [1, 4, 0, 2]),
-        919: () => m("default", "@jupyterlab/notebook", [1, 4, 0, 2])
+        861: () => m("default", "@jupyterlab/notebook", [1, 4, 0, 3]),
+        882: () => g("default", "@jupyterlab/cells", [1, 4, 0, 3])
     }, S = {
-        568: [850, 919]
+        568: [861, 882]
     }, E.f.consumes = (e, r) => {
         E.o(S, e) && S[e].forEach((e => {
             if (E.o(y, e)) return r.push(y[e]);
             var t = r => {
                     y[e] = 0, E.m[e] = t => {
                         delete E.c[e], t.exports = r()
                     }
@@ -277,10 +277,10 @@
                     u && u(E)
                 }
                 for (r && r(t); s < a.length; s++) o = a[s], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_shannon_shen_chapyter = self.webpackChunk_shannon_shen_chapyter || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), E.nc = void 0;
-    var _ = E(875);
+    var _ = E(983);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@shannon-shen/chapyter"] = _
 })();
```

### Comparing `chapyter-0.2.0/chapyter/labextension/static/third-party-licenses.json` & `chapyter-0.3.0/chapyter/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `chapyter-0.2.0/examples/starter-Copy2.ipynb` & `chapyter-0.3.0/examples/01-quick-start.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9607412191197213%*

 * *Differences: {"'cells'": "{0: {'source': ['## The Magic Commands in `Chapyter`']}, 1: {'execution_count': 1, "*

 * *            "'outputs': [], 'source': ['%load_ext chapyter\\n', '# You might want to create an "*

 * *            "`.env` file in the current\\n', '# directory that contains\\n', '# "*

 * *            "OPENAI_API_KEY=sk-xxxx\\n', '# OPENAI_ORGANIZATION=org-xxxx\\n', '# For other ways "*

 * *            "for configurations, including how to use Azure OpenAI APIs, \\n', '# you can check "*

 * *            "the 02-configure-chapyter. […]*

```diff
@@ -1,135 +1,141 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": 1,
-            "id": "b34ae35c-c3cb-4b98-8484-e242554dd49d",
-            "metadata": {
-                "editable": true,
-                "slideshow": {
-                    "slide_type": ""
-                },
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "%load_ext dotenv\n",
-                "%dotenv\n",
-                "\n",
-                "# We have an `.env` file that specifies the OPENAI_API_KEY and OPENAI_ORGANIZATION\n",
-                "# You might need to run \"pip install python-dotenv\"."
-            ]
-        },
-        {
             "cell_type": "markdown",
             "id": "c1271f63-22c4-4151-83ae-0ea36be59c17",
             "metadata": {},
             "source": [
-                "### The Magic Command "
+                "## The Magic Commands in `Chapyter`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 1,
             "id": "305f5dfc-d2e5-44eb-b6b5-4850e86274f4",
             "metadata": {
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/shannon/projects/2307_ChatGPT_Kernel/chapyter-latest/examples\n"
-                    ]
-                }
-            ],
+            "outputs": [],
+            "source": [
+                "%load_ext chapyter\n",
+                "# You might want to create an `.env` file in the current\n",
+                "# directory that contains\n",
+                "# OPENAI_API_KEY=sk-xxxx\n",
+                "# OPENAI_ORGANIZATION=org-xxxx\n",
+                "# For other ways for configurations, including how to use Azure OpenAI APIs, \n",
+                "# you can check the 02-configure-chapyter.ipynb notebook for more details."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "a4caec9f-71d7-4674-9e4c-29279981fed2",
+            "metadata": {},
             "source": [
-                "%load_ext chapyter"
+                "PS: You will see neat UIs if you download and execute the following cells one by one in jupyterlab. \n",
+                "![chapyter-starter.png](https://www.szj.io/assets/files/data/chapyter-starter.png)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "bb8888ac-5bec-4c62-9de6-21d45ce89ff1",
             "metadata": {},
             "source": [
                 "### `%%chat`: start coding in natural language"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "id": "effc4a91-fc5e-42c9-b576-e0c37ecd4478",
             "metadata": {
                 "ChapyterCell": {
                     "cellType": "original",
-                    "linkedCellId": "784dfe7a-e6f5-4ba0-b9af-d55cc35fb7af"
+                    "linkedCellId": "93c33a3e-710a-4472-922c-1458d98c32d0"
                 }
             },
             "outputs": [],
             "source": [
-                "%%chat -s\n",
+                "%%chat \n",
                 "list all the files in the current directory"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "id": "784dfe7a-e6f5-4ba0-b9af-d55cc35fb7af",
+            "execution_count": 5,
+            "id": "93c33a3e-710a-4472-922c-1458d98c32d0",
             "metadata": {
                 "ChapyterCell": {
                     "cellType": "generated",
                     "linkedCellId": "effc4a91-fc5e-42c9-b576-e0c37ecd4478"
                 }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "['test', '.env', 'starter-Copy2.ipynb', '.ipynb_checkpoints', 'starter.ipynb', 'starter-Copy1.ipynb']\n"
+                    ]
+                }
+            ],
             "source": [
-                "# Assistant Code for Cell [3]:\n",
+                "# Assistant Code for Cell [2]:\n",
                 "# Sure, here is the Python code to list all the files in the current directory:\n",
                 "import os\n",
                 "\n",
                 "files = os.listdir('.')\n",
                 "print(files)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "id": "29533815-5d55-4281-8446-f2e1b810b040",
             "metadata": {
                 "ChapyterCell": {
                     "cellType": "original",
-                    "linkedCellId": "64531dfa-b467-4b10-90b6-d5769b71cd3c"
+                    "linkedCellId": "84daa58f-c55d-4b75-8540-47eb6d0441df"
                 }
             },
             "outputs": [],
             "source": [
-                "%%chat -s\n",
+                "%%chat \n",
                 "\n",
                 "find the files in the current directory that has the longest file name "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "id": "64531dfa-b467-4b10-90b6-d5769b71cd3c",
+            "execution_count": 6,
+            "id": "84daa58f-c55d-4b75-8540-47eb6d0441df",
             "metadata": {
                 "ChapyterCell": {
                     "cellType": "generated",
                     "linkedCellId": "29533815-5d55-4281-8446-f2e1b810b040"
+                },
+                "jupyter": {
+                    "source_hidden": true
                 }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "starter-Copy2.ipynb\n"
+                    ]
+                }
+            ],
             "source": [
-                "# Assistant Code for Cell [4]:\n",
+                "# Assistant Code for Cell [3]:\n",
                 "# Sure, here is the Python code to find the file with the longest name in the current directory.\n",
                 "import os\n",
                 "\n",
                 "# Get all files in current directory\n",
                 "files = os.listdir('.')\n",
                 "\n",
                 "# Find the file with the longest name\n",
@@ -137,42 +143,53 @@
                 "\n",
                 "print(longest_file)\n",
                 "# This code will print the name of the file with the longest name in the current directory."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 4,
             "id": "7f055c4f-f714-4620-9e1e-d629ab8a4d87",
             "metadata": {
                 "ChapyterCell": {
                     "cellType": "original",
-                    "linkedCellId": "3e373672-9853-4e53-9e18-e9f80a425be5"
+                    "linkedCellId": "c2927cf9-766e-4c03-b039-5d6ece37d958"
                 }
             },
             "outputs": [],
             "source": [
-                "%%chat -s\n",
+                "%%chat \n",
                 "\n",
                 "Generate a dictionary that groups the files in the current folder based on their types"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "id": "3e373672-9853-4e53-9e18-e9f80a425be5",
+            "execution_count": 7,
+            "id": "c2927cf9-766e-4c03-b039-5d6ece37d958",
             "metadata": {
                 "ChapyterCell": {
                     "cellType": "generated",
                     "linkedCellId": "7f055c4f-f714-4620-9e1e-d629ab8a4d87"
+                },
+                "jupyter": {
+                    "source_hidden": true
                 }
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "{'': ['test', '.env', '.ipynb_checkpoints'], '.ipynb': ['starter-Copy2.ipynb', 'starter.ipynb', 'starter-Copy1.ipynb']}\n"
+                    ]
+                }
+            ],
             "source": [
-                "# Assistant Code for Cell [5]:\n",
+                "# Assistant Code for Cell [4]:\n",
                 "# Sure, here is a Python script that does that:\n",
                 "import os\n",
                 "\n",
                 "# Get all files in current directory\n",
                 "files = os.listdir('.')\n",
                 "\n",
                 "# Initialize an empty dictionary to store the file types and names\n",
@@ -200,54 +217,55 @@
             "metadata": {},
             "source": [
                 "### `%%chat -h` will add execution history into the prompt "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 8,
             "id": "57e0a283-95d9-410a-bcdb-9efde7d252b2",
             "metadata": {
                 "ChapyterCell": {
                     "cellType": "original",
-                    "linkedCellId": "480e4951-851f-44db-8ed0-e115472a8b0f"
+                    "linkedCellId": "2285fa4c-14ed-4d7f-861f-aba5c89d1daa"
                 }
             },
             "outputs": [],
             "source": [
                 "%%chat -h \n",
+                "\n",
                 "Define functions for the code above:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
-            "id": "480e4951-851f-44db-8ed0-e115472a8b0f",
+            "execution_count": 9,
+            "id": "2285fa4c-14ed-4d7f-861f-aba5c89d1daa",
             "metadata": {
                 "ChapyterCell": {
                     "cellType": "generated",
                     "linkedCellId": "57e0a283-95d9-410a-bcdb-9efde7d252b2"
                 },
                 "jupyter": {
                     "source_hidden": true
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "['test', '.env', '.ipynb_checkpoints', 'starter.ipynb', 'starter-Copy1.ipynb']\n",
-                        "starter-Copy1.ipynb\n",
-                        "{'': ['test', '.env', '.ipynb_checkpoints'], '.ipynb': ['starter.ipynb', 'starter-Copy1.ipynb']}\n"
+                        "['test', '.env', 'starter-Copy2.ipynb', '.ipynb_checkpoints', 'starter.ipynb', 'starter-Copy1.ipynb']\n",
+                        "starter-Copy2.ipynb\n",
+                        "{'': ['test', '.env', '.ipynb_checkpoints'], '.ipynb': ['starter-Copy2.ipynb', 'starter.ipynb', 'starter-Copy1.ipynb']}\n"
                     ]
                 }
             ],
             "source": [
-                "# Assistant Code for Cell [9]:\n",
+                "# Assistant Code for Cell [8]:\n",
                 "# Sure, here is how you can define functions for the code above:\n",
                 "import os\n",
                 "\n",
                 "def list_files():\n",
                 "    files = os.listdir('.')\n",
                 "    return files\n",
                 "\n",
@@ -279,53 +297,42 @@
             "metadata": {},
             "source": [
                 "### `%%chat -s` or `%%chat --safe` will invoke safe mode that won't execute the cells "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 6,
             "id": "f353789b-c8e7-467c-bce6-1ed02eb33fe9",
             "metadata": {
                 "ChapyterCell": {
                     "cellType": "original",
-                    "linkedCellId": "3cdad85a-64eb-466b-9ac4-4935f1548d1c"
+                    "linkedCellId": "54c09d95-8df0-41b5-89a2-28475f7d0c47"
                 }
             },
             "outputs": [],
             "source": [
                 "%%chat -s \n",
                 "\n",
                 "Generate a dictionary that groups the files in the current folder based on their types"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
-            "id": "3cdad85a-64eb-466b-9ac4-4935f1548d1c",
+            "execution_count": null,
+            "id": "54c09d95-8df0-41b5-89a2-28475f7d0c47",
             "metadata": {
                 "ChapyterCell": {
                     "cellType": "generated",
                     "linkedCellId": "f353789b-c8e7-467c-bce6-1ed02eb33fe9"
-                },
-                "jupyter": {
-                    "source_hidden": true
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "{'': ['test', '.env', '.ipynb_checkpoints'], '.ipynb': ['starter.ipynb', 'starter-Copy1.ipynb']}\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "# Assistant Code for Cell [15]:\n",
+                "# Assistant Code for Cell [6]:\n",
                 "# Sure, here is a Python script that does that:\n",
                 "import os\n",
                 "\n",
                 "# Get all files in current directory\n",
                 "files = os.listdir('.')\n",
                 "\n",
                 "# Initialize an empty dictionary to store the file types and names\n",
@@ -344,89 +351,67 @@
                 "    file_dict[file_type].append(file)\n",
                 "\n",
                 "print(file_dict)\n",
                 "# This script will print a dictionary where the keys are file extensions (like '.txt', '.py', etc.) and the values are lists of file names with that extension."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 1,
-            "id": "27f56967-2127-4029-95a4-902ace0d1ae8",
+            "cell_type": "markdown",
+            "id": "0e89ac15-bf8f-4763-bab0-2dcb089e96c3",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "ipython = get_ipython()"
+                "### `%%chatonly` allows you to talk to an agent in regular ways "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
-            "id": "20cbea8e-d62d-495a-9fac-167414774626",
+            "execution_count": 10,
+            "id": "fdebb778-26a4-4db4-9a74-9191d54516c3",
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "{'__name__': '__main__',\n",
-                            " '__doc__': 'Automatically created module for IPython interactive environment',\n",
-                            " '__package__': None,\n",
-                            " '__loader__': None,\n",
-                            " '__spec__': None,\n",
-                            " '__builtin__': <module 'builtins' (built-in)>,\n",
-                            " '__builtins__': <module 'builtins' (built-in)>,\n",
-                            " '_ih': ['', 'ipython = get_ipython()', 'ipython.user_ns'],\n",
-                            " '_oh': {},\n",
-                            " '_dh': [PosixPath('/Users/shannon/projects/2307_ChatGPT_Kernel/chapyter-latest/examples')],\n",
-                            " 'In': ['', 'ipython = get_ipython()', 'ipython.user_ns'],\n",
-                            " 'Out': {},\n",
-                            " 'get_ipython': <function IPython.core.getipython.get_ipython()>,\n",
-                            " 'exit': <IPython.core.autocall.ZMQExitAutocall at 0x10385b150>,\n",
-                            " 'quit': <IPython.core.autocall.ZMQExitAutocall at 0x10385b150>,\n",
-                            " 'open': <function io.open(file, mode='r', buffering=-1, encoding=None, errors=None, newline=None, closefd=True, opener=None)>,\n",
-                            " '_': '',\n",
-                            " '__': '',\n",
-                            " '___': '',\n",
-                            " '__session__': '/Users/shannon/projects/2307_ChatGPT_Kernel/chapyter-latest/examples/starter-Copy2.ipynb',\n",
-                            " 'collections': <module 'collections' from '/Users/shannon/miniconda3/envs/jupyterlab-extension-examples/lib/python3.11/collections/__init__.py'>,\n",
-                            " 'functools': <module 'functools' from '/Users/shannon/miniconda3/envs/jupyterlab-extension-examples/lib/python3.11/functools.py'>,\n",
-                            " 'itertools': <module 'itertools' (built-in)>,\n",
-                            " 'json': <module 'json' from '/Users/shannon/miniconda3/envs/jupyterlab-extension-examples/lib/python3.11/json/__init__.py'>,\n",
-                            " 'os': <module 'os' (frozen)>,\n",
-                            " 'Path': pathlib.Path,\n",
-                            " 'plt': <module 'matplotlib.pyplot' from '/Users/shannon/miniconda3/envs/jupyterlab-extension-examples/lib/python3.11/site-packages/matplotlib/pyplot.py'>,\n",
-                            " 'np': <module 'numpy' from '/Users/shannon/miniconda3/envs/jupyterlab-extension-examples/lib/python3.11/site-packages/numpy/__init__.py'>,\n",
-                            " 'pd': <module 'pandas' from '/Users/shannon/miniconda3/envs/jupyterlab-extension-examples/lib/python3.11/site-packages/pandas/__init__.py'>,\n",
-                            " 'requests': <module 'requests' from '/Users/shannon/miniconda3/envs/jupyterlab-extension-examples/lib/python3.11/site-packages/requests/__init__.py'>,\n",
-                            " 'sns': <module 'seaborn' from '/Users/shannon/miniconda3/envs/jupyterlab-extension-examples/lib/python3.11/site-packages/seaborn/__init__.py'>,\n",
-                            " 'pprint': <function rich.pretty.pprint(_object: Any, *, console: Optional[ForwardRef('Console')] = None, indent_guides: bool = True, max_length: Optional[int] = None, max_string: Optional[int] = None, max_depth: Optional[int] = None, expand_all: bool = False) -> None>,\n",
-                            " 'tqdm': tqdm.std.tqdm,\n",
-                            " 'ipython': <ipykernel.zmqshell.ZMQInteractiveShell at 0x103852950>,\n",
-                            " '_i': 'ipython = get_ipython()',\n",
-                            " '_ii': '',\n",
-                            " '_iii': '',\n",
-                            " '_i1': 'ipython = get_ipython()',\n",
-                            " '_i2': '\\nipython.user_ns'}"
-                        ]
-                    },
-                    "execution_count": 2,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "In the realm of code, where logic is the language,\n",
+                        "There exists a serpent, not of danger, but of change.\n",
+                        "Python, they call it, a creature of grace,\n",
+                        "In the world of programming, it's found its place.\n",
+                        "\n",
+                        "Lines of elegance, simplicity its charm,\n",
+                        "For beginners and experts, it causes no harm.\n",
+                        "From data science to web design,\n",
+                        "Its versatility is truly divine.\n",
+                        "\n",
+                        "Indentation matters, in its syntax so neat,\n",
+                        "Making code readable, a feat so sweet.\n",
+                        "With libraries abundant, like stars in the sky,\n",
+                        "The solutions it offers, they never run dry.\n",
+                        "\n",
+                        "In the heart of a coder, Python ignites a flame,\n",
+                        "Turning problems to solutions, that's the aim.\n",
+                        "From machine learning to artificial intelligence,\n",
+                        "It breaks all barriers, knows no resistance.\n",
+                        "\n",
+                        "Python, oh Python, in bytes we converse,\n",
+                        "Your presence in coding universe is diverse.\n",
+                        "In the dance of algorithms, you're a trusted partner,\n",
+                        "For many a programmer, you're the lantern.\n",
+                        "\n",
+                        "So here's to Python, a toast, a cheer,\n",
+                        "To a language we coders, hold so dear.\n",
+                        "In the world of technology, constantly in motion,\n",
+                        "Python flows like a smooth, steady ocean.\n"
+                    ]
                 }
             ],
             "source": [
-                "ipython.user_ns"
+                "%%chatonly\n",
+                "Can you write a poem for the python programming language? "
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "a228a51f-3291-4112-9570-a9e268b2f17b",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "extension",
             "language": "python",
             "name": "extension"
```

### Comparing `chapyter-0.2.0/src/index.ts` & `chapyter-0.3.0/src/index.ts`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
               // set the proper linked cell ID
               chatCell.model.setMetadata('ChapyterCell', {
                 cellType: 'original',
                 linkedCellId: assistanceCell.model.id
               });
 
               chatCell.addClass(CHAPYTER_CHAT_CELL);
-              chatCell.toggleClass(CHAPYTER_CHAT_CELL_EXECUTING);
+              chatCell.removeClass(CHAPYTER_CHAT_CELL_EXECUTING);
               assistanceCell.addClass(CHAPYTER_ASSISTANCE_CELL);
             }
           }
         }
       }
     });
```

### Comparing `chapyter-0.2.0/style/base.css` & `chapyter-0.3.0/style/base.css`

 * *Files identical despite different names*

### Comparing `chapyter-0.2.0/.gitignore` & `chapyter-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `chapyter-0.2.0/LICENSE` & `chapyter-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chapyter-0.2.0/pyproject.toml` & `chapyter-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,25 +24,14 @@
 dependencies = [
     "guidance", 
     "jupyterlab>=4.0",
     "python-dotenv",
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
-[tool.isort]
-profile = "black"
-line_length = 79
-multi_line_output = 3
-
-[tool.autopep8]
-max_line_length = 79
-in-place = true
-recursive = true
-aggressive = 3
-
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.metadata.hooks.nodejs]
 fields = ["description", "authors", "urls"]
 
 [tool.hatch.build.targets.sdist]
```

### Comparing `chapyter-0.2.0/PKG-INFO` & `chapyter-0.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,101 +1,61 @@
-Metadata-Version: 2.1
-Name: chapyter
-Version: 0.2.0
-Summary: A Natural Language-Based Python Program Interpreter
-Project-URL: Homepage, https://github.com/chapyter/chapyter
-Project-URL: Bug Tracker, https://github.com/chapyter/chapyter/issues
-Project-URL: Repository, https://github.com/chapyter/chapyter.git
-Author-email: chapyter <zejiangshen@gmail.com>
-License: BSD 3-Clause License
-        
-        Copyright (c) 2023, chapyter
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        1. Redistributions of source code must retain the above copyright notice, this
-           list of conditions and the following disclaimer.
-        
-        2. Redistributions in binary form must reproduce the above copyright notice,
-           this list of conditions and the following disclaimer in the documentation
-           and/or other materials provided with the distribution.
-        
-        3. Neither the name of the copyright holder nor the names of its
-           contributors may be used to endorse or promote products derived from
-           this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-License-File: LICENSE
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 4
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Requires-Dist: guidance
-Requires-Dist: jupyterlab>=4.0
-Requires-Dist: python-dotenv
-Description-Content-Type: text/markdown
-
 <div align="center">
   <img src="https://github.com/chapyter/chapyter/raw/main/.github/chapyter-logo.png" alt="Chapyter Logo" width="35%">
-  <h3 align="center">
-  Chapyter is a jupyterlab extension for NL"P": Natural Language-based Programming
-  </h3>
 </div>
 
-## Demo 
-<div align="center">
-<img src="https://github.com/chapyter/chapyter/raw/main/.github/chapyter-starter.png" alt="Chapyter Starter Demo" width="75%">
-</div>
+**[Please check our latest blogpost on Chapyter release.](https://www.szj.io/posts/chapyter)**
+
+## What is Chapyter 
+
+Chapyter is a JupyterLab extension that seamlessly connects GPT-4 to your coding environment. 
+It features a code interpreter that can translate your natural language description into Python code and automatically execute it. 
+By enabling "natural language programming" in your most familiar IDE, Chapyter can boost your productivity and empower you to explore many new ideas that you would not have tried otherwise.
+
+| Functionality |                                                                            Example                                                                           |
+| --- | --- | 
+| **Code generation from natural language and automatic execution** <br> Simply adding the magic command `%%chat` at the beginning of the cell of a natural language description of the task, the code is generated and the results are shown in a few seconds. | ![Code generation from natural language and automatic execution](https://github.com/chapyter/chapyter/raw/main/.github/example-1.gif) |
+| **Using coding history and execution output for code generation** <br> By adding the `--history` or `-h` flag in generation, chapyter can use the previous execution history and outputs to generate the appropriate visualization for the loaded IRIS dataset. |![Using coding history and execution output for code generation](https://github.com/chapyter/chapyter/raw/main/.github/example-2.gif)  |
+| **In-situ debugging and code editing** <br> The generated code might not be perfect and could contain bugs or errors. Since Chapyter is fully integrated into Jupyter Notebook, you can easily inspect the code and fix any errors or bugs (e.g., installing missing dependencies in this case) without leaving the IDE.  | ![In-situ debugging and code editing](https://github.com/chapyter/chapyter/raw/main/.github/example-3.gif)  |
+| **Transparency on the prompts and AI configuration and allows for customization** |  We release all the prompts used in our library and we are working on easy customization of the used prompts and settings. See in [chapyter/programs.py](https://github.com/chapyter/chapyter/blob/main/chapyter/programs.py). | 
+| **Privacy-first when using latest powerful AI** |  Since we are using OpenAI API, all the data sent to OpenAI will not be saved for training (see [OpenAI API Data Usage Policies](https://openai.com/policies/api-data-usage-policies)). As a comparison, whenever you are using Copilot or ChatGPT, your data will be somewhat cached and can be used for their training and analysis. | 
 
 ## Quick Start
  
 1. Installation 
     ```bash
     pip install chapyter   # Automatically installs the extension to jupyterlab
     pip uninstall chapyter # Uninstalls the extension from jupyterlab
     ```
     Note: It will upgrade the jupyterlab to ≥ 4.0. It might break your environments. 
 
-2. Usage: see [examples/starter.ipynb](examples/starter.ipynb) for a starter notebook. 
+2. Usage: see [examples/01-quick-start.ipynb](examples/01-quick-start.ipynb) for a starter notebook. 
 
     1. Set the proper `OPENAI_API_KEY` and `OPENAI_ORGANIZATION` in the environment variable 
     2. Use the magic command `%%chat` in a code cell: 
         ```
         %%chat -m gpt-4-0613 
         List all the files in the folder 
         ```
-       It will call gpt-4-0613 to generate the python code for listing all the files in the folder, and 
-       execute the generated code automatically. **In this case, this plugin serves as the interpreter that**
-       **translates the natural language to python code and execute it.** 
+       It will call gpt-4-0613 to generate the python code for listing all the files in the folder, and execute the generated code automatically. In this case, this plugin serves as the interpreter that translates the natural language to python code and execute it. 
 
 3. Examples: 
-    - [examples/starter.ipynb](examples/starter.ipynb) A starter notebook illustrating the basic functions of `chapyter`. 
+    - [examples/01-quick-start.ipynb](examples/01-quick-start.ipynb) illustrates the basic functions of `chapyter`, including how to use the magic command `%%chat`
+    - [examples/02-configure-chapyter.ipynb](examples/02-configure-chapyter.ipynb) shows how to customize `chapyter`:
+        - Use different default models (e.g., gpt-3.5-turbo instead of gpt-4)
+        - Use different types of API (now we support use the default OpenAI API or the Azure OpenAI API)
     
 ## Development Notes
 
+There are two major components in Chapyter: implementing the ipython magic command that handles the prompting and calling GPT-X models, and the frontend that listens to Chapyter cell execution and automatically executes the newly generated cell and updates the cell styles. The chart below illustrates the orchestration of the frontend and ipython kernel after a Chapyter cell is executed.
+
+![implementation](https://www.szj.io/posts/chapyter/implementation.png)
+
+
+### Details 
+
 1. NodeJS is needed to build the extension package.
 
 2. The `jlpm` command is JupyterLab's pinned version of [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
     ```bash
     # Clone the repo to your local environment
     # Change directory to the chapyter directory
@@ -117,8 +77,8 @@
     With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
 
 4. By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
     ```bash
     jupyter lab build --minimize=False
     ```
 
-5. Packaging and release: please refer to [RELEASE](RELEASE.md). 
+5. Packaging and release: please refer to [RELEASE](RELEASE.md).
```

