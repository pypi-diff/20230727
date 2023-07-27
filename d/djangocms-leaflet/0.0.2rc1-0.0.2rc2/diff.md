# Comparing `tmp/djangocms_leaflet-0.0.2rc1.tar.gz` & `tmp/djangocms_leaflet-0.0.2rc2.tar.gz`

## Comparing `djangocms_leaflet-0.0.2rc1.tar` & `djangocms_leaflet-0.0.2rc2.tar`

### file list

```diff
@@ -1,37 +1,56 @@
--rw-r--r--   0        0        0    58671 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/package-lock.json
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/package.json
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/webpack.config.js
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/assets/src/leaflet.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/__about__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/apps.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/cms_plugins.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/models.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/migrations/0001_initial.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/migrations/__init__.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png
--rw-r--r--   0        0        0   169468 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png
--rw-r--r--   0        0        0   174858 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/webpack/leaflet.bundle.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/webpack/leaflet.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/templates/djangocms_leaflet/map.html
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/templates/djangocms_leaflet/marker.html
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/tests/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/.gitignore
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/LICENSE.txt
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/README.md
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/pyproject.toml
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc1/PKG-INFO
+-rw-r--r--   0        0        0    58673 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/package-lock.json
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/package.json
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/webpack.config.js
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/assets/src/leaflet.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/__about__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/apps.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/cms_plugins.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/models.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/migrations/0001_initial.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/migrations/__init__.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-black.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-black.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-blue.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-blue.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-gold.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-gold.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-green.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-green.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-grey.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-grey.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-orange.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-orange.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-red.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-red.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-violet.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-violet.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-yellow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-yellow.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-black.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-black.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-blue.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-blue.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-gold.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-gold.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-green.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-green.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-grey.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-grey.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-orange.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-orange.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-red.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-red.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-violet.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-violet.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-yellow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-yellow.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-shadow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-shadow.png
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png
+-rw-r--r--   0        0        0   169468 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png
+-rw-r--r--   0        0        0   174912 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/leaflet.bundle.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/leaflet.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/templates/djangocms_leaflet/map.html
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/templates/djangocms_leaflet/marker.html
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/tests/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/.gitignore
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/README.md
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/pyproject.toml
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/PKG-INFO
```

### Comparing `djangocms_leaflet-0.0.2rc1/package-lock.json` & `djangocms_leaflet-0.0.2rc2/package-lock.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989576816127912%*

 * *Differences: {"'packages'": "{'node_modules/@types/eslint': {'version': '8.44.1', 'resolved': "*

 * *               "'https://registry.npmjs.org/@types/eslint/-/eslint-8.44.1.tgz', 'integrity': "*

 * *               "'sha512-XpNDc4Z5Tb4x+SW1MriMVeIsMoONHCkWFMkR/aPJbzEsxqHy+4Glu/BqTdPrApfDeMaXbtNh6bseNgl5KaWrSg=='}, "*

 * *               "'node_modules/@types/node': {'version': '20.4.5', 'resolved': "*

 * *               "'https://registry.npmjs.org/@types/node/-/node-20.4.5.tgz', 'integrity': "*

 * *               "'sha512-rt40Nk13II9JwQBdeYqmb […]*

```diff
@@ -84,18 +84,18 @@
             "version": "0.3.18"
         },
         "node_modules/@types/eslint": {
             "dependencies": {
                 "@types/estree": "*",
                 "@types/json-schema": "*"
             },
-            "integrity": "sha512-PRVjQ4Eh9z9pmmtaq8nTjZjQwKFk7YIHIud3lRoKRBgUQjgjRmoGxxGEPXQkF+lH7QkHJRNr5F4aBgYCW0lqpQ==",
+            "integrity": "sha512-XpNDc4Z5Tb4x+SW1MriMVeIsMoONHCkWFMkR/aPJbzEsxqHy+4Glu/BqTdPrApfDeMaXbtNh6bseNgl5KaWrSg==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-8.40.2.tgz",
-            "version": "8.40.2"
+            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-8.44.1.tgz",
+            "version": "8.44.1"
         },
         "node_modules/@types/eslint-scope": {
             "dependencies": {
                 "@types/eslint": "*",
                 "@types/estree": "*"
             },
             "integrity": "sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==",
@@ -112,18 +112,18 @@
         "node_modules/@types/json-schema": {
             "integrity": "sha512-Hr5Jfhc9eYOQNPYO5WLDq/n4jqijdHNlDXjuAQkkt+mWdQR+XJToOHrsD4cPaMXpn6KO7y2+wM8AZEs8VpBLVA==",
             "peer": true,
             "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.12.tgz",
             "version": "7.0.12"
         },
         "node_modules/@types/node": {
-            "integrity": "sha512-wheIYdr4NYML61AjC8MKj/2jrR/kDQri/CIpVoZwldwhnIrD/j9jIU5bJ8yBKuB2VhpFV7Ab6G2XkBjv9r9Zzw==",
+            "integrity": "sha512-rt40Nk13II9JwQBdeYqmbn2Q6IVTA5uPhvSO+JVqdXw/6/4glI6oR9ezty/A9Hg5u7JH4OmYmuQ+XvjKm0Datg==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.3.3.tgz",
-            "version": "20.3.3"
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.4.5.tgz",
+            "version": "20.4.5"
         },
         "node_modules/@webassemblyjs/ast": {
             "dependencies": {
                 "@webassemblyjs/helper-numbers": "1.11.6",
                 "@webassemblyjs/helper-wasm-bytecode": "1.11.6"
             },
             "integrity": "sha512-IN1xI7PwOvLPgjcf180gC1bqn3q/QaOCwYUahIOhbYUu8KA/3tw2RT/T0Gidi1l7Hhj5D/INhJxiICObqpMu4Q==",
@@ -326,18 +326,18 @@
         "node_modules/acorn": {
             "bin": {
                 "acorn": "bin/acorn"
             },
             "engines": {
                 "node": ">=0.4.0"
             },
-            "integrity": "sha512-jaVNAFBHNLXspO543WnNNPZFRtavh3skAkITqD0/2aeMkKZTN+254PyhwxFYrk3vQ1xfY+2wbesJMs/JC8/PwQ==",
+            "integrity": "sha512-F0SAmZ8iUtS//m8DmCTA0jlh6TDKkHQyK6xc6V4KDTyZKA9dnvX9/3sRTVQrWm79glUAZbnmmNcdYwUIHWVybw==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.9.0.tgz",
-            "version": "8.9.0"
+            "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.10.0.tgz",
+            "version": "8.10.0"
         },
         "node_modules/acorn-import-assertions": {
             "integrity": "sha512-cmMwop9x+8KFhxvKrKfPYmN6/pKTYYHBqLa0DfvVZcKMJWNyWLnaqND7dx/qn66R7ewM1UX5XMaDVP5wlVTaVA==",
             "peer": true,
             "peerDependencies": {
                 "acorn": "^8"
             },
@@ -418,18 +418,18 @@
                     "url": "https://tidelift.com/funding/github/npm/caniuse-lite"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-2S9nK0G/mE+jasCUsMPlARhRCts1ebcp2Ji8Y8PWi4NDE1iRdLCnEPHkEfeBrGC45L4isBx5ur3IQ6yTE2mRZw==",
+            "integrity": "sha512-Vdhm5S11DaFVLlyiKu4hiUTkpZu+y1KA/rZZqVQfOD5YdDT/eQKlkt7NaE0WGOFgX32diqt9MiP9CAiFeRklaA==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001512.tgz",
-            "version": "1.0.30001512"
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001517.tgz",
+            "version": "1.0.30001517"
         },
         "node_modules/chrome-trace-event": {
             "engines": {
                 "node": ">=6.0"
             },
             "integrity": "sha512-p3KULyQg4S7NIHixdwbGX+nFHkoBiA4YQmyWtjb8XngSKV124nJmRysgAeujbUVb15vh+RvFUfCPqU7rXk+hZg==",
             "peer": true,
@@ -509,18 +509,18 @@
                 "node": ">=4"
             },
             "integrity": "sha512-/Tb/JcjK111nNScGob5MNtsntNM1aCNUDipB/TkwZFhyDrrE47SOx/18wF2bbjgc3ZzCSKW1T5nt5EbFoAz/Vg==",
             "resolved": "https://registry.npmjs.org/cssesc/-/cssesc-3.0.0.tgz",
             "version": "3.0.0"
         },
         "node_modules/electron-to-chromium": {
-            "integrity": "sha512-TxLRpRUj/107ATefeP8VIUWNOv90xJxZZbCW/eIbSZQiuiFANCx2b7u+GbVc9X4gU+xnbvypNMYVM/WArE1DNQ==",
+            "integrity": "sha512-JL+vQaO4/3mnE68YLaO6tS61YFTlQp8/9JJj1kMP0CL9GHjLYt8t3T0aA3sW3PvdiXjnVeaZ6Kf0mGtt9+2j+Q==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.449.tgz",
-            "version": "1.4.449"
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.472.tgz",
+            "version": "1.4.472"
         },
         "node_modules/enhanced-resolve": {
             "dependencies": {
                 "graceful-fs": "^4.2.4",
                 "tapable": "^2.2.0"
             },
             "engines": {
@@ -880,18 +880,18 @@
         "node_modules/neo-async": {
             "integrity": "sha512-Yd3UES5mWCSqR+qNT93S3UoYUkqAZ9lLg8a7g9rimsWmYGK8cVToA4/sF3RrshdyV3sAGMXVUmpMYOw+dLpOuw==",
             "peer": true,
             "resolved": "https://registry.npmjs.org/neo-async/-/neo-async-2.6.2.tgz",
             "version": "2.6.2"
         },
         "node_modules/node-releases": {
-            "integrity": "sha512-QzsYKWhXTWx8h1kIvqfnC++o0pEmpRQA/aenALsL2F4pqNVr7YzcdMlDij5WBnwftRbJCNJL/O7zdKaxKPHqgQ==",
+            "integrity": "sha512-uYr7J37ae/ORWdZeQ1xxMJe3NtdmqMC/JZK+geofDrkLUApKRHPd18/TxtBOJ4A0/+uUIliorNrfYV6s1b02eQ==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.12.tgz",
-            "version": "2.0.12"
+            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.13.tgz",
+            "version": "2.0.13"
         },
         "node_modules/overlapping-marker-spiderfier-leaflet": {
             "integrity": "sha512-U2biV2Ge0SU+4IEmq4BZOglvzA8Aj8G7/hp5v6lBnF9Kd3/Xf6ZEPsJyPOExtLvMxOqlrlTAfl55s6JJDND7Ew==",
             "resolved": "https://registry.npmjs.org/overlapping-marker-spiderfier-leaflet/-/overlapping-marker-spiderfier-leaflet-0.2.7.tgz",
             "version": "0.2.7"
         },
         "node_modules/p-limit": {
@@ -990,17 +990,17 @@
                     "url": "https://tidelift.com/funding/github/npm/postcss"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-M0RzbcI0sO/XJNucsGjvWU9ERWxb/ytp1w6dKtxTKgixdtQDq4rmx/g8W1hnaheq9jgwL/oyEdH5Bc4WwJKMqg==",
-            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.24.tgz",
-            "version": "8.4.24"
+            "integrity": "sha512-gY/ACJtJPSmUFPDCHtX78+01fHa64FaU4zaaWfuh1MhGJISufJAH4cun6k/8fwsHYeK4UQmENQK+tRLCFJE8JQ==",
+            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.27.tgz",
+            "version": "8.4.27"
         },
         "node_modules/postcss-modules-extract-imports": {
             "engines": {
                 "node": "^10 || ^12 || >= 14"
             },
             "integrity": "sha512-bdHleFnP3kZ4NYDhuGlVK+CMrQ/pqUm8bx/oGL93K6gVwiclvX5x0n76fYMKuIGKzlABOy13zsvqjb0f92TEXw==",
             "peerDependencies": {
@@ -1182,17 +1182,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.3.tgz",
-            "version": "7.5.3"
+            "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
+            "version": "7.5.4"
         },
         "node_modules/serialize-javascript": {
             "dependencies": {
                 "randombytes": "^2.1.0"
             },
             "integrity": "sha512-owoXEFjWRllis8/M1Q+Cw5k8ZH40e3zhp/ovX+Xr/vi1qj6QesbyXXViFbpNvWvPNAD62SutwEXavefrLJWj7w==",
             "peer": true,
@@ -1319,18 +1319,18 @@
                 "acorn": "^8.8.2",
                 "commander": "^2.20.0",
                 "source-map-support": "~0.5.20"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-Ah19JS86ypbJzTzvUCX7KOsEIhDaRONungA4aYBjEP3JZRf4ocuDzTg4QWZnPn9DEMiMYGJPiSOy7aykoCc70w==",
+            "integrity": "sha512-qC5+dmecKJA4cpYxRa5aVkKehYsQKc+AHeKl0Oe62aYjBL8ZA33tTljktDHJSaxxMnbI5ZYw+o/S2DxxLu8OfA==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.18.2.tgz",
-            "version": "5.18.2"
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.19.2.tgz",
+            "version": "5.19.2"
         },
         "node_modules/terser-webpack-plugin": {
             "dependencies": {
                 "@jridgewell/trace-mapping": "^0.3.17",
                 "jest-worker": "^27.4.5",
                 "schema-utils": "^3.1.1",
                 "serialize-javascript": "^6.0.1",
@@ -1452,23 +1452,23 @@
             "engines": {
                 "node": ">=10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-FROX3TxQnC/ox4N+3xQoWZzvGXSuscxR32rbzjpXgEzWudJFEJBpdlkkob2ylrv5yzzufD1zph1OoFsLtm6stQ==",
+            "integrity": "sha512-JmcgNZ1iKj+aiR0OvTYtWQqJwq37Pf683dY9bVORwVbUrDhLhdn/PlO2sHsFHPkj7sHNQF3JwaAkp49V+Sq1tQ==",
             "peer": true,
             "peerDependenciesMeta": {
                 "webpack-cli": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.88.1.tgz",
-            "version": "5.88.1"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.88.2.tgz",
+            "version": "5.88.2"
         },
         "node_modules/webpack-cli": {
             "bin": {
                 "webpack-cli": "bin/cli.js"
             },
             "dependencies": {
                 "@discoveryjs/json-ext": "^0.5.0",
```

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/cms_plugins.py` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/models.py` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/migrations/0001_initial.py` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/static/webpack/leaflet.bundle.js` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/leaflet.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5451,10 +5451,13 @@
             h = i.n(a),
             l = i(216),
             u = i.n(l),
             c = i(589),
             d = i.n(c),
             p = i(984),
             _ = {};
-        _.styleTagTransform = d(), _.setAttributes = h(), _.insert = r().bind(null, "head"), _.domAPI = o(), _.insertStyleElement = u(), e()(p.Z, _), p.Z && p.Z.locals && p.Z.locals, i(841)
+        _.styleTagTransform = d(), _.setAttributes = h(), _.insert = r().bind(null, "head"), _.domAPI = o(), _.insertStyleElement = u(), e()(p.Z, _), p.Z && p.Z.locals && p.Z.locals;
+        var f = i(841),
+            m = i.n(f);
+        window.OverlappingMarkerSpiderfier = m()
     })()
 })();
```

### Comparing `djangocms_leaflet-0.0.2rc1/src/djangocms_leaflet/templates/djangocms_leaflet/map.html` & `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/templates/djangocms_leaflet/map.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,119 +1,104 @@
 00000000: 7b25 206c 6f61 6420 7374 6174 6963 2063  {% load static c
 00000010: 6d73 5f74 6167 7320 7365 6b69 7a61 695f  ms_tags sekizai_
 00000020: 7461 6773 2069 3138 6e20 6c31 306e 2025  tags i18n l10n %
-00000030: 7d0a 7b25 2061 6464 746f 626c 6f63 6b20  }.{% addtoblock 
-00000040: 2263 7373 2220 7374 7269 7020 257d 0a7b  "css" strip %}.{
-00000050: 2320 3c6c 696e 6b20 6872 6566 3d22 7b25  # <link href="{%
-00000060: 2073 7461 7469 6320 2764 6a61 6e67 6f63   static 'djangoc
-00000070: 6d73 5f6c 6561 666c 6574 2f6c 6561 666c  ms_leaflet/leafl
-00000080: 6574 2e63 7373 2720 257d 2220 7265 6c3d  et.css' %}" rel=
-00000090: 2273 7479 6c65 7368 6565 7422 2074 7970  "stylesheet" typ
-000000a0: 653d 2274 6578 742f 6373 7322 3e20 237d  e="text/css"> #}
-000000b0: 0a7b 2520 656e 6461 6464 746f 626c 6f63  .{% endaddtobloc
-000000c0: 6b20 257d 0a0a 7b25 206c 6f63 616c 697a  k %}..{% localiz
-000000d0: 6520 6f66 6620 257d 207b 2320 6176 6f69  e off %} {# avoi
-000000e0: 6420 6465 6369 6d61 6c20 636f 6d6d 6120  d decimal comma 
-000000f0: 237d 0a7b 2520 6164 6474 6f62 6c6f 636b  #}.{% addtoblock
-00000100: 2022 6373 7322 2073 7472 6970 2025 7d0a   "css" strip %}.
-00000110: 3c73 7479 6c65 3e0a 0923 6d61 702d 7b7b  <style>..#map-{{
-00000120: 2069 6e73 7461 6e63 652e 6964 207d 7d20   instance.id }} 
-00000130: 7b0a 0909 6865 6967 6874 3a20 7b7b 2069  {...height: {{ i
-00000140: 6e73 7461 6e63 652e 6865 6967 6874 207d  nstance.height }
-00000150: 7d70 783b 0a09 096d 6172 6769 6e3a 2032  }px;...margin: 2
-00000160: 7265 6d3b 0a09 7d0a 3c2f 7374 796c 653e  rem;..}.</style>
-00000170: 0a7b 2520 656e 6461 6464 746f 626c 6f63  .{% endaddtobloc
-00000180: 6b20 257d 0a0a 3c64 6976 2069 643d 226d  k %}..<div id="m
-00000190: 6170 2d7b 7b20 696e 7374 616e 6365 2e69  ap-{{ instance.i
-000001a0: 6420 7d7d 223e 3c2f 6469 763e 0a0a 7b25  d }}"></div>..{%
-000001b0: 2061 6464 746f 626c 6f63 6b20 226a 7322   addtoblock "js"
-000001c0: 2073 7472 6970 2025 7d0a 7b23 203c 7363   strip %}.{# <sc
-000001d0: 7269 7074 2064 6566 6572 2073 7263 3d22  ript defer src="
-000001e0: 7b25 2073 7461 7469 6320 2764 6a61 6e67  {% static 'djang
-000001f0: 6f63 6d73 5f6c 6561 666c 6574 2f6c 6561  ocms_leaflet/lea
-00000200: 666c 6574 2e6a 7327 2025 7d22 3e3c 2f73  flet.js' %}"></s
-00000210: 6372 6970 743e 2023 7d0a 3c73 6372 6970  cript> #}.<scrip
-00000220: 7420 6465 6665 7220 7372 633d 227b 2520  t defer src="{% 
-00000230: 7374 6174 6963 2027 646a 616e 676f 636d  static 'djangocm
-00000240: 735f 6c65 6166 6c65 742f 7765 6270 6163  s_leaflet/webpac
-00000250: 6b2f 6c65 6166 6c65 742e 6275 6e64 6c65  k/leaflet.bundle
-00000260: 2e6a 7327 2025 7d22 3e3c 2f73 6372 6970  .js' %}"></scrip
-00000270: 743e 0a7b 2520 656e 6461 6464 746f 626c  t>.{% endaddtobl
-00000280: 6f63 6b20 257d 0a0a 7b25 2061 6464 746f  ock %}..{% addto
-00000290: 626c 6f63 6b20 226a 7322 2073 7472 6970  block "js" strip
-000002a0: 2025 7d0a 3c73 6372 6970 743e 0a09 7661   %}.<script>..va
-000002b0: 7220 6d61 700a 0924 2866 756e 6374 696f  r map..$(functio
-000002c0: 6e20 2829 207b 0a09 2020 2020 6d61 7020  n () {..    map 
-000002d0: 3d20 4c2e 6d61 7028 276d 6170 2d7b 7b20  = L.map('map-{{ 
-000002e0: 696e 7374 616e 6365 2e69 6420 7d7d 2729  instance.id }}')
-000002f0: 2e73 6574 5669 6577 285b 7b7b 2069 6e73  .setView([{{ ins
-00000300: 7461 6e63 652e 6c61 7469 7475 6465 207d  tance.latitude }
-00000310: 7d2c 207b 7b20 696e 7374 616e 6365 2e6c  }, {{ instance.l
-00000320: 6f6e 6769 7475 6465 207d 7d5d 2c20 7b7b  ongitude }}], {{
-00000330: 2069 6e73 7461 6e63 652e 7a6f 6f6d 5f6c   instance.zoom_l
-00000340: 6576 656c 207d 7d29 3b0a 0a20 2020 2020  evel }});..     
-00000350: 2020 204c 2e74 696c 654c 6179 6572 2827     L.tileLayer('
-00000360: 6874 7470 733a 2f2f 7b73 7d2e 7469 6c65  https://{s}.tile
-00000370: 2e6f 7065 6e73 7472 6565 746d 6170 2e6f  .openstreetmap.o
-00000380: 7267 2f7b 7a7d 2f7b 787d 2f7b 797d 2e70  rg/{z}/{x}/{y}.p
-00000390: 6e67 272c 207b 0a20 2020 2020 2020 2020  ng', {.         
-000003a0: 2020 2061 7474 7269 6275 7469 6f6e 3a20     attribution: 
-000003b0: 2726 636f 7079 3b20 3c61 2068 7265 663d  '&copy; <a href=
-000003c0: 2268 7474 7073 3a2f 2f77 7777 2e6f 7065  "https://www.ope
-000003d0: 6e73 7472 6565 746d 6170 2e6f 7267 2f63  nstreetmap.org/c
-000003e0: 6f70 7972 6967 6874 223e 4f70 656e 5374  opyright">OpenSt
-000003f0: 7265 6574 4d61 703c 2f61 3e20 636f 6e74  reetMap</a> cont
-00000400: 7269 6275 746f 7273 270a 2020 2020 2020  ributors'.      
-00000410: 2020 7d29 2e61 6464 546f 286d 6170 293b    }).addTo(map);
-00000420: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00000430: 2020 7b23 2068 7474 7073 3a2f 2f73 7461    {# https://sta
-00000440: 636b 6f76 6572 666c 6f77 2e63 6f6d 2f71  ckoverflow.com/q
-00000450: 7565 7374 696f 6e73 2f36 3439 3032 3137  uestions/6490217
-00000460: 312f 616e 6775 6c61 722d 3130 2d6c 6561  1/angular-10-lea
-00000470: 666c 6574 2d77 6562 7061 636b 2d62 7265  flet-webpack-bre
-00000480: 616b 696e 672d 7572 6c2d 746f 2d6d 6172  aking-url-to-mar
-00000490: 6b65 722d 6963 6f6e 2d70 6e67 2023 7d0a  ker-icon-png #}.
-000004a0: 2020 2020 2020 2020 2020 2020 6c65 7420              let 
-000004b0: 4465 6661 756c 7449 636f 6e20 3d20 4c2e  DefaultIcon = L.
-000004c0: 6963 6f6e 287b 0a09 2020 2020 2020 2020  icon({..        
-000004d0: 2020 6963 6f6e 5572 6c3a 2027 7b25 2020    iconUrl: '{%  
-000004e0: 7374 6174 6963 2022 646a 616e 676f 636d  static "djangocm
-000004f0: 735f 6c65 6166 6c65 742f 696d 6167 6573  s_leaflet/images
-00000500: 2f6c 6561 666c 6574 2d63 6f6c 6f72 2d6d  /leaflet-color-m
-00000510: 6172 6b65 7273 2f6d 6172 6b65 722d 6963  arkers/marker-ic
-00000520: 6f6e 2d32 782d 626c 7565 2e70 6e67 2220  on-2x-blue.png" 
-00000530: 257d 272c 0a09 2020 2020 2020 2020 2020  %}',..          
-00000540: 7368 6164 6f77 5572 6c3a 2027 7b25 2020  shadowUrl: '{%  
-00000550: 7374 6174 6963 2022 646a 616e 676f 636d  static "djangocm
-00000560: 735f 6c65 6166 6c65 742f 696d 6167 6573  s_leaflet/images
-00000570: 2f6c 6561 666c 6574 2d63 6f6c 6f72 2d6d  /leaflet-color-m
-00000580: 6172 6b65 7273 2f6d 6172 6b65 722d 7368  arkers/marker-sh
-00000590: 6164 6f77 2e70 6e67 2220 257d 272c 0a09  adow.png" %}',..
-000005a0: 0909 2020 6963 6f6e 5369 7a65 3a20 5b32  ..  iconSize: [2
-000005b0: 342c 3336 5d2c 0a09 0909 2020 6963 6f6e  4,36],....  icon
-000005c0: 416e 6368 6f72 3a20 5b31 322c 3336 5d0a  Anchor: [12,36].
-000005d0: 0909 097d 293b 0a20 2020 2020 2020 2020  ...});.         
-000005e0: 2020 204c 2e4d 6172 6b65 722e 7072 6f74     L.Marker.prot
-000005f0: 6f74 7970 652e 6f70 7469 6f6e 732e 6963  otype.options.ic
-00000600: 6f6e 203d 2044 6566 6175 6c74 4963 6f6e  on = DefaultIcon
-00000610: 3b0a 0a09 097b 2520 6966 2069 6e73 7461  ;....{% if insta
-00000620: 6e63 652e 7365 745f 6d61 726b 6572 2025  nce.set_marker %
-00000630: 7d0a 2020 2020 2020 2020 4c2e 6d61 726b  }.        L.mark
-00000640: 6572 285b 7b7b 2069 6e73 7461 6e63 652e  er([{{ instance.
-00000650: 6c61 7469 7475 6465 207d 7d2c 207b 7b20  latitude }}, {{ 
-00000660: 696e 7374 616e 6365 2e6c 6f6e 6769 7475  instance.longitu
-00000670: 6465 207d 7d5d 292e 6164 6454 6f28 6d61  de }}]).addTo(ma
-00000680: 7029 0a20 2020 2020 2020 2020 2020 202e  p).            .
-00000690: 6269 6e64 506f 7075 7028 277b 7b20 696e  bindPopup('{{ in
-000006a0: 7374 616e 6365 2e6e 616d 6520 7d7d 2729  stance.name }}')
-000006b0: 0a20 2020 2020 2020 2020 2020 202e 6f70  .            .op
-000006c0: 656e 506f 7075 7028 293b 0a09 097b 2520  enPopup();...{% 
-000006d0: 656e 6469 6620 257d 0a20 2020 207d 290a  endif %}.    }).
-000006e0: 3c2f 7363 7269 7074 3e0a 7b25 2065 6e64  </script>.{% end
-000006f0: 6164 6474 6f62 6c6f 636b 2025 7d0a 0a7b  addtoblock %}..{
-00000700: 2520 666f 7220 706c 7567 696e 2069 6e20  % for plugin in 
-00000710: 696e 7374 616e 6365 2e63 6869 6c64 5f70  instance.child_p
-00000720: 6c75 6769 6e5f 696e 7374 616e 6365 7320  lugin_instances 
-00000730: 257d 0a7b 2520 7265 6e64 6572 5f70 6c75  %}.{% render_plu
-00000740: 6769 6e20 706c 7567 696e 2025 7d0a 7b25  gin plugin %}.{%
-00000750: 2065 6e64 666f 7220 257d 0a7b 2520 656e   endfor %}.{% en
-00000760: 646c 6f63 616c 697a 6520 257d            dlocalize %}
+00000030: 7d0a 0a7b 2520 6c6f 6361 6c69 7a65 206f  }..{% localize o
+00000040: 6666 2025 7d20 7b23 2061 766f 6964 2064  ff %} {# avoid d
+00000050: 6563 696d 616c 2063 6f6d 6d61 2023 7d0a  ecimal comma #}.
+00000060: 7b25 2061 6464 746f 626c 6f63 6b20 2263  {% addtoblock "c
+00000070: 7373 2220 7374 7269 7020 257d 0a3c 7374  ss" strip %}.<st
+00000080: 796c 653e 0a09 236d 6170 2d7b 7b20 696e  yle>..#map-{{ in
+00000090: 7374 616e 6365 2e69 6420 7d7d 207b 0a09  stance.id }} {..
+000000a0: 0968 6569 6768 743a 207b 7b20 696e 7374  .height: {{ inst
+000000b0: 616e 6365 2e68 6569 6768 7420 7d7d 7078  ance.height }}px
+000000c0: 3b0a 0909 6d61 7267 696e 3a20 3272 656d  ;...margin: 2rem
+000000d0: 3b0a 097d 0a3c 2f73 7479 6c65 3e0a 7b25  ;..}.</style>.{%
+000000e0: 2065 6e64 6164 6474 6f62 6c6f 636b 2025   endaddtoblock %
+000000f0: 7d0a 0a3c 6469 7620 6964 3d22 6d61 702d  }..<div id="map-
+00000100: 7b7b 2069 6e73 7461 6e63 652e 6964 207d  {{ instance.id }
+00000110: 7d22 3e3c 2f64 6976 3e0a 0a7b 2520 6164  }"></div>..{% ad
+00000120: 6474 6f62 6c6f 636b 2022 6a73 2220 7374  dtoblock "js" st
+00000130: 7269 7020 257d 0a3c 7363 7269 7074 2064  rip %}.<script d
+00000140: 6566 6572 2073 7263 3d22 7b25 2073 7461  efer src="{% sta
+00000150: 7469 6320 2764 6a61 6e67 6f63 6d73 5f6c  tic 'djangocms_l
+00000160: 6561 666c 6574 2f77 6562 7061 636b 2f6c  eaflet/webpack/l
+00000170: 6561 666c 6574 2e62 756e 646c 652e 6a73  eaflet.bundle.js
+00000180: 2720 257d 223e 3c2f 7363 7269 7074 3e0a  ' %}"></script>.
+00000190: 7b25 2065 6e64 6164 6474 6f62 6c6f 636b  {% endaddtoblock
+000001a0: 2025 7d0a 0a7b 2520 6164 6474 6f62 6c6f   %}..{% addtoblo
+000001b0: 636b 2022 6a73 2220 7374 7269 7020 257d  ck "js" strip %}
+000001c0: 0a3c 7363 7269 7074 2064 6566 6572 3e0a  .<script defer>.
+000001d0: 7769 6e64 6f77 2e6f 6e6c 6f61 6420 3d20  window.onload = 
+000001e0: 6675 6e63 7469 6f6e 2829 207b 0a20 2020  function() {.   
+000001f0: 2063 6f6e 7374 206d 6170 203d 204c 2e6d   const map = L.m
+00000200: 6170 2827 6d61 702d 7b7b 2069 6e73 7461  ap('map-{{ insta
+00000210: 6e63 652e 6964 207d 7d27 292e 7365 7456  nce.id }}').setV
+00000220: 6965 7728 5b7b 7b20 696e 7374 616e 6365  iew([{{ instance
+00000230: 2e6c 6174 6974 7564 6520 7d7d 2c20 7b7b  .latitude }}, {{
+00000240: 2069 6e73 7461 6e63 652e 6c6f 6e67 6974   instance.longit
+00000250: 7564 6520 7d7d 5d2c 207b 7b20 696e 7374  ude }}], {{ inst
+00000260: 616e 6365 2e7a 6f6f 6d5f 6c65 7665 6c20  ance.zoom_level 
+00000270: 7d7d 293b 0a0a 2020 2020 4c2e 7469 6c65  }});..    L.tile
+00000280: 4c61 7965 7228 2768 7474 7073 3a2f 2f7b  Layer('https://{
+00000290: 737d 2e74 696c 652e 6f70 656e 7374 7265  s}.tile.openstre
+000002a0: 6574 6d61 702e 6f72 672f 7b7a 7d2f 7b78  etmap.org/{z}/{x
+000002b0: 7d2f 7b79 7d2e 706e 6727 2c20 7b0a 2020  }/{y}.png', {.  
+000002c0: 2020 2020 2020 6174 7472 6962 7574 696f        attributio
+000002d0: 6e3a 2027 2663 6f70 793b 203c 6120 6872  n: '&copy; <a hr
+000002e0: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
+000002f0: 6f70 656e 7374 7265 6574 6d61 702e 6f72  openstreetmap.or
+00000300: 672f 636f 7079 7269 6768 7422 3e4f 7065  g/copyright">Ope
+00000310: 6e53 7472 6565 744d 6170 3c2f 613e 2063  nStreetMap</a> c
+00000320: 6f6e 7472 6962 7574 6f72 7327 0a20 2020  ontributors'.   
+00000330: 207d 292e 6164 6454 6f28 6d61 7029 3b0a   }).addTo(map);.
+00000340: 0a20 2020 207b 2320 6874 7470 733a 2f2f  .    {# https://
+00000350: 7374 6163 6b6f 7665 7266 6c6f 772e 636f  stackoverflow.co
+00000360: 6d2f 7175 6573 7469 6f6e 732f 3634 3930  m/questions/6490
+00000370: 3231 3731 2f61 6e67 756c 6172 2d31 302d  2171/angular-10-
+00000380: 6c65 6166 6c65 742d 7765 6270 6163 6b2d  leaflet-webpack-
+00000390: 6272 6561 6b69 6e67 2d75 726c 2d74 6f2d  breaking-url-to-
+000003a0: 6d61 726b 6572 2d69 636f 6e2d 706e 6720  marker-icon-png 
+000003b0: 237d 0a20 2020 206c 6574 2044 6566 6175  #}.    let Defau
+000003c0: 6c74 4963 6f6e 203d 204c 2e69 636f 6e28  ltIcon = L.icon(
+000003d0: 7b0a 2020 2020 2020 2020 6963 6f6e 5572  {.        iconUr
+000003e0: 6c3a 2027 7b25 2020 7374 6174 6963 2022  l: '{%  static "
+000003f0: 646a 616e 676f 636d 735f 6c65 6166 6c65  djangocms_leafle
+00000400: 742f 696d 6167 6573 2f6c 6561 666c 6574  t/images/leaflet
+00000410: 2d63 6f6c 6f72 2d6d 6172 6b65 7273 2f6d  -color-markers/m
+00000420: 6172 6b65 722d 6963 6f6e 2d32 782d 626c  arker-icon-2x-bl
+00000430: 7565 2e70 6e67 2220 257d 272c 0a20 2020  ue.png" %}',.   
+00000440: 2020 2020 2073 6861 646f 7755 726c 3a20       shadowUrl: 
+00000450: 277b 2520 2073 7461 7469 6320 2264 6a61  '{%  static "dja
+00000460: 6e67 6f63 6d73 5f6c 6561 666c 6574 2f69  ngocms_leaflet/i
+00000470: 6d61 6765 732f 6c65 6166 6c65 742d 636f  mages/leaflet-co
+00000480: 6c6f 722d 6d61 726b 6572 732f 6d61 726b  lor-markers/mark
+00000490: 6572 2d73 6861 646f 772e 706e 6722 2025  er-shadow.png" %
+000004a0: 7d27 2c0a 2020 2020 2020 2020 6963 6f6e  }',.        icon
+000004b0: 5369 7a65 3a20 5b32 342c 2033 365d 2c0a  Size: [24, 36],.
+000004c0: 2020 2020 2020 2020 6963 6f6e 416e 6368          iconAnch
+000004d0: 6f72 3a20 5b31 322c 2033 365d 0a20 2020  or: [12, 36].   
+000004e0: 207d 293b 0a20 2020 204c 2e4d 6172 6b65   });.    L.Marke
+000004f0: 722e 7072 6f74 6f74 7970 652e 6f70 7469  r.prototype.opti
+00000500: 6f6e 732e 6963 6f6e 203d 2044 6566 6175  ons.icon = Defau
+00000510: 6c74 4963 6f6e 3b0a 0a20 2020 207b 2520  ltIcon;..    {% 
+00000520: 6966 2069 6e73 7461 6e63 652e 7365 745f  if instance.set_
+00000530: 6d61 726b 6572 2025 7d0a 2020 2020 2020  marker %}.      
+00000540: 2020 4c2e 6d61 726b 6572 285b 7b7b 2069    L.marker([{{ i
+00000550: 6e73 7461 6e63 652e 6c61 7469 7475 6465  nstance.latitude
+00000560: 207d 7d2c 207b 7b20 696e 7374 616e 6365   }}, {{ instance
+00000570: 2e6c 6f6e 6769 7475 6465 207d 7d5d 292e  .longitude }}]).
+00000580: 6164 6454 6f28 6d61 7029 0a20 2020 2020  addTo(map).     
+00000590: 2020 2020 2020 202e 6269 6e64 506f 7075         .bindPopu
+000005a0: 7028 277b 7b20 696e 7374 616e 6365 2e6e  p('{{ instance.n
+000005b0: 616d 6520 7d7d 2729 0a20 2020 2020 2020  ame }}').       
+000005c0: 2020 2020 202e 6f70 656e 506f 7075 7028       .openPopup(
+000005d0: 293b 0a20 2020 207b 2520 656e 6469 6620  );.    {% endif 
+000005e0: 257d 0a7d 0a3c 2f73 6372 6970 743e 0a7b  %}.}.</script>.{
+000005f0: 2520 656e 6461 6464 746f 626c 6f63 6b20  % endaddtoblock 
+00000600: 257d 0a0a 7b25 2066 6f72 2070 6c75 6769  %}..{% for plugi
+00000610: 6e20 696e 2069 6e73 7461 6e63 652e 6368  n in instance.ch
+00000620: 696c 645f 706c 7567 696e 5f69 6e73 7461  ild_plugin_insta
+00000630: 6e63 6573 2025 7d0a 7b25 2072 656e 6465  nces %}.{% rende
+00000640: 725f 706c 7567 696e 2070 6c75 6769 6e20  r_plugin plugin 
+00000650: 257d 0a7b 2520 656e 6466 6f72 2025 7d0a  %}.{% endfor %}.
+00000660: 7b25 2065 6e64 6c6f 6361 6c69 7a65 2025  {% endlocalize %
+00000670: 7d                                       }
```

### Comparing `djangocms_leaflet-0.0.2rc1/LICENSE.txt` & `djangocms_leaflet-0.0.2rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/README.md` & `djangocms_leaflet-0.0.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/pyproject.toml` & `djangocms_leaflet-0.0.2rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc1/PKG-INFO` & `djangocms_leaflet-0.0.2rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-leaflet
-Version: 0.0.2rc1
+Version: 0.0.2rc2
 Summary: django CMS plug-ins for the JavaScript map library Leaflet
 Project-URL: Documentation, https://github.com/MacLake/djangocms-leaflet#readme
 Project-URL: Issues, https://github.com/MacLake/djangocms-leaflet/issues
 Project-URL: Source, https://github.com/MacLake/djangocms-leaflet
 Author-email: Jens-Erik Weber <Jens-Erik.Weber@passiv.de>
 License-Expression: MIT
 License-File: LICENSE.txt
```

