# Comparing `tmp/shootpandora-Cloud-20230725.1.3.tar.gz` & `tmp/shootpandora-Cloud-20230725.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shootpandora-Cloud-20230725.1.3.tar", last modified: Wed Jul 26 09:46:00 2023, max compression
+gzip compressed data, was "shootpandora-Cloud-20230725.1.4.tar", last modified: Thu Jul 27 01:56:05 2023, max compression
```

## Comparing `shootpandora-Cloud-20230725.1.3.tar` & `shootpandora-Cloud-20230725.1.4.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.740284 shootpandora-Cloud-20230725.1.3/
--rw-rw-rw-   0        0        0    18092 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/LICENSE
--rw-rw-rw-   0        0        0       89 2023-07-25 02:29:01.000000 shootpandora-Cloud-20230725.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2313 2023-07-26 09:46:00.741287 shootpandora-Cloud-20230725.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-07-25 02:30:59.000000 shootpandora-Cloud-20230725.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-26 09:46:00.746285 shootpandora-Cloud-20230725.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1837 2023-07-25 02:30:59.000000 shootpandora-Cloud-20230725.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.211284 shootpandora-Cloud-20230725.1.3/shootpandora_Cloud.egg-info/
--rw-rw-rw-   0        0        0     2313 2023-07-26 09:45:59.000000 shootpandora-Cloud-20230725.1.3/shootpandora_Cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7643 2023-07-26 09:46:00.000000 shootpandora-Cloud-20230725.1.3/shootpandora_Cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 09:45:59.000000 shootpandora-Cloud-20230725.1.3/shootpandora_Cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-26 09:45:59.000000 shootpandora-Cloud-20230725.1.3/shootpandora_Cloud.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.095285 shootpandora-Cloud-20230725.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.224287 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/
--rw-rw-rw-   0        0        0       54 2023-07-26 09:40:11.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.163288 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.247285 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.099283 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.136289 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.352284 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/
--rw-rw-rw-   0        0        0    69737 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js
--rw-rw-rw-   0        0        0   262802 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js
--rw-rw-rw-   0        0        0    74170 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/238-882950710bdd3e1e.js
--rw-rw-rw-   0        0        0    29389 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/271.f8fe486a0f5b221c.js
--rw-rw-rw-   0        0        0      657 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/2802bd5f-15923fb46be55b45.js
--rw-rw-rw-   0        0        0    23052 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/297-e180277ece10e844.js
--rw-rw-rw-   0        0        0   417248 2023-07-25 02:30:59.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/412-c00b85b4ef66af2f.js
--rw-rw-rw-   0        0        0   248252 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/435-2b015d294e66ccbc.js
--rw-rw-rw-   0        0        0    16805 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/564-f0043ba04d4fcd3d.js
--rw-rw-rw-   0        0        0     3092 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/68a27ff6-b1db347c50639918.js
--rw-rw-rw-   0        0        0  1085662 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/800-a82eb647282afb06.js
--rw-rw-rw-   0        0        0     8750 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/937-36e251f389e9e752.js
--rw-rw-rw-   0        0        0    26962 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/984-1278472924e49180.js
--rw-rw-rw-   0        0        0     1044 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/bd26816a-7ae54dd3357d90b4.js
--rw-rw-rw-   0        0        0   141071 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js
--rw-rw-rw-   0        0        0   121704 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/main-0438431c68fbeb27.js
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.379290 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.392288 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/
--rw-rw-rw-   0        0        0      461 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/cancel-164e4ecc13479ecd.js
--rw-rw-rw-   0        0        0      461 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/manage-c7a1640505b9cfd2.js
--rw-rw-rw-   0        0        0     2755 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-1457e593ce508c31.js
--rw-rw-rw-   0        0        0    21936 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/admin-810915a9e0227b64.js
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.120283 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.123282 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.395284 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/
--rw-rw-rw-   0        0        0     1344 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-b7d4a081f7ad5b5b.js
--rw-rw-rw-   0        0        0   987027 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/app-573ad0910def0e5d.js
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.432284 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/
--rw-rw-rw-   0        0        0     3189 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/error-9faed2db943661ab.js
--rw-rw-rw-   0        0        0      661 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-7b50f284300a7ff6.js
--rw-rw-rw-   0        0        0      611 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-47f3cd5abd2d99b6.js
--rw-rw-rw-   0        0        0     5527 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/login-267fffdf86e9e08a.js
--rw-rw-rw-   0        0        0     1069 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-5817b04f45f270e2.js
--rw-rw-rw-   0        0        0      596 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-060c0092bc682b49.js
--rw-rw-rw-   0        0        0      488 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/bypass-979cf95f72688cf4.js
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.436284 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/c/
--rw-rw-rw-   0        0        0     5629 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-5d264bebf7157821.js
--rw-rw-rw-   0        0        0      250 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/error-fdab57c4b88e5b1c.js
--rw-rw-rw-   0        0        0     5414 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/index-b00721778b6b9fff.js
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.443287 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/payments/
--rw-rw-rw-   0        0        0    20064 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/payments/success-c423ec16521d5906.js
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.446290 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/share/
--rw-rw-rw-   0        0        0     7543 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-1c5c5056584e8afb.js
--rw-rw-rw-   0        0        0      399 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/status-9047ec54adb32ef3.js
--rw-rw-rw-   0        0        0    91460 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-rw-rw-   0        0        0     4976 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/webpack-305aad91bdd6a592.js
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.450286 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/css/
--rw-rw-rw-   0        0        0   138266 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/css/59d85ffe80f6c774.css
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.461283 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/
--rw-rw-rw-   0        0        0     2375 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/buildManifest.js
--rw-rw-rw-   0        0        0       77 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/ssgManifest.js
--rw-rw-rw-   0        0        0     4159 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/apple-touch-icon.png
--rw-rw-rw-   0        0        0      730 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/favicon-16x16.png
--rw-rw-rw-   0        0        0     1292 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/favicon-32x32.png
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.152284 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.493285 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/
--rw-rw-rw-   0        0        0    34336 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff
--rw-rw-rw-   0        0        0    27412 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2
--rw-rw-rw-   0        0        0    35956 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff
--rw-rw-rw-   0        0        0    28532 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2
--rw-rw-rw-   0        0        0    35268 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff
--rw-rw-rw-   0        0        0    28060 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2
--rw-rw-rw-   0        0        0    37480 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff
--rw-rw-rw-   0        0        0    29824 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.613283 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/
--rw-rw-rw-   0        0        0    28076 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2
--rw-rw-rw-   0        0        0     6912 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2
--rw-rw-rw-   0        0        0     6908 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2
--rw-rw-rw-   0        0        0    11348 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2
--rw-rw-rw-   0        0        0    11316 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2
--rw-rw-rw-   0        0        0    25324 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2
--rw-rw-rw-   0        0        0    16780 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2
--rw-rw-rw-   0        0        0    16988 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2
--rw-rw-rw-   0        0        0    26272 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2
--rw-rw-rw-   0        0        0    16400 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2
--rw-rw-rw-   0        0        0    16440 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2
--rw-rw-rw-   0        0        0    12216 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2
--rw-rw-rw-   0        0        0    12028 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2
--rw-rw-rw-   0        0        0    10344 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2
--rw-rw-rw-   0        0        0     9644 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2
--rw-rw-rw-   0        0        0     5468 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2
--rw-rw-rw-   0        0        0     5208 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2
--rw-rw-rw-   0        0        0     3624 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2
--rw-rw-rw-   0        0        0     4928 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2
--rw-rw-rw-   0        0        0    13568 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.627289 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/signifier/
--rw-rw-rw-   0        0        0    56682 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2
--rw-rw-rw-   0        0        0    56021 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2
--rw-rw-rw-   0        0        0    56456 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2
--rw-rw-rw-   0        0        0    53009 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light.woff2
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.668285 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/
--rw-rw-rw-   0        0        0    34084 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2
--rw-rw-rw-   0        0        0    33350 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2
--rw-rw-rw-   0        0        0    40456 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2
--rw-rw-rw-   0        0        0    37996 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2
--rw-rw-rw-   0        0        0    38746 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2
--rw-rw-rw-   0        0        0    35690 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2
--rw-rw-rw-   0        0        0    28148 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2
--rw-rw-rw-   0        0        0    27437 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2
--rw-rw-rw-   0        0        0    28285 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2
--rw-rw-rw-   0        0        0      336 2023-07-25 02:29:01.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/manifest.json
--rw-rw-rw-   0        0        0     6133 2023-07-25 02:29:01.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/service-worker.js
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.682292 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/sweetalert2/
--rw-rw-rw-   0        0        0    19844 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/sweetalert2/bulma.min.css
--rw-rw-rw-   0        0        0    68840 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.158283 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/ulp/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.159289 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/ulp/react-components/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.161285 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.686284 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/css/
--rw-rw-rw-   0        0        0   233073 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:00.736284 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/templates/
--rw-rw-rw-   0        0        0     4903 2023-07-26 04:02:58.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/templates/404.html
--rw-rw-rw-   0        0        0     7436 2023-07-26 09:45:24.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/templates/chat.html
--rw-rw-rw-   0        0        0     4858 2023-07-26 04:01:14.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/templates/detail.html
--rw-rw-rw-   0        0        0    40476 2023-07-26 09:45:28.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/templates/login.html
--rw-rw-rw-   0        0        0     6122 2023-07-26 04:02:45.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/templates/share.html
--rw-rw-rw-   0        0        0        0 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/py.typed
--rw-rw-rw-   0        0        0    19767 2023-07-25 02:29:01.000000 shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/server.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:05.014229 shootpandora-Cloud-20230725.1.4/
+-rw-rw-rw-   0        0        0    18092 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/LICENSE
+-rw-rw-rw-   0        0        0       89 2023-07-25 02:29:01.000000 shootpandora-Cloud-20230725.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2313 2023-07-27 01:56:05.014229 shootpandora-Cloud-20230725.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-07-25 02:30:59.000000 shootpandora-Cloud-20230725.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-27 01:56:05.018235 shootpandora-Cloud-20230725.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1837 2023-07-25 02:30:59.000000 shootpandora-Cloud-20230725.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:03.683232 shootpandora-Cloud-20230725.1.4/shootpandora_Cloud.egg-info/
+-rw-rw-rw-   0        0        0     2313 2023-07-27 01:56:01.000000 shootpandora-Cloud-20230725.1.4/shootpandora_Cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7643 2023-07-27 01:56:02.000000 shootpandora-Cloud-20230725.1.4/shootpandora_Cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 01:56:01.000000 shootpandora-Cloud-20230725.1.4/shootpandora_Cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-27 01:56:01.000000 shootpandora-Cloud-20230725.1.4/shootpandora_Cloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:03.406229 shootpandora-Cloud-20230725.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:03.742234 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/
+-rw-rw-rw-   0        0        0       54 2023-07-27 01:55:18.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:03.570228 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:03.777228 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:03.458232 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:03.557233 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.009228 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/
+-rw-rw-rw-   0        0        0    69737 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js
+-rw-rw-rw-   0        0        0   262802 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js
+-rw-rw-rw-   0        0        0    74170 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/238-882950710bdd3e1e.js
+-rw-rw-rw-   0        0        0    29389 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/271.f8fe486a0f5b221c.js
+-rw-rw-rw-   0        0        0      657 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/2802bd5f-15923fb46be55b45.js
+-rw-rw-rw-   0        0        0    23052 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/297-e180277ece10e844.js
+-rw-rw-rw-   0        0        0   417248 2023-07-25 02:30:59.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/412-c00b85b4ef66af2f.js
+-rw-rw-rw-   0        0        0   248252 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/435-2b015d294e66ccbc.js
+-rw-rw-rw-   0        0        0    16805 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/564-f0043ba04d4fcd3d.js
+-rw-rw-rw-   0        0        0     3092 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/68a27ff6-b1db347c50639918.js
+-rw-rw-rw-   0        0        0  1085662 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/800-a82eb647282afb06.js
+-rw-rw-rw-   0        0        0     8750 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/937-36e251f389e9e752.js
+-rw-rw-rw-   0        0        0    26962 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/984-1278472924e49180.js
+-rw-rw-rw-   0        0        0     1044 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/bd26816a-7ae54dd3357d90b4.js
+-rw-rw-rw-   0        0        0   141071 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js
+-rw-rw-rw-   0        0        0   121704 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/main-0438431c68fbeb27.js
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.093234 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.108228 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/
+-rw-rw-rw-   0        0        0      461 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/cancel-164e4ecc13479ecd.js
+-rw-rw-rw-   0        0        0      461 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/manage-c7a1640505b9cfd2.js
+-rw-rw-rw-   0        0        0     2755 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-1457e593ce508c31.js
+-rw-rw-rw-   0        0        0    21936 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/admin-810915a9e0227b64.js
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:03.519228 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:03.520229 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.141228 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/
+-rw-rw-rw-   0        0        0     1344 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-b7d4a081f7ad5b5b.js
+-rw-rw-rw-   0        0        0   987027 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/app-573ad0910def0e5d.js
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.237232 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/
+-rw-rw-rw-   0        0        0     3189 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/error-9faed2db943661ab.js
+-rw-rw-rw-   0        0        0      661 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-7b50f284300a7ff6.js
+-rw-rw-rw-   0        0        0      611 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-47f3cd5abd2d99b6.js
+-rw-rw-rw-   0        0        0     5527 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/login-267fffdf86e9e08a.js
+-rw-rw-rw-   0        0        0     1069 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-5817b04f45f270e2.js
+-rw-rw-rw-   0        0        0      596 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-060c0092bc682b49.js
+-rw-rw-rw-   0        0        0      488 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/bypass-979cf95f72688cf4.js
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.251232 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/c/
+-rw-rw-rw-   0        0        0     5629 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-5d264bebf7157821.js
+-rw-rw-rw-   0        0        0      250 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/error-fdab57c4b88e5b1c.js
+-rw-rw-rw-   0        0        0     5414 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/index-b00721778b6b9fff.js
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.260231 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/payments/
+-rw-rw-rw-   0        0        0    20064 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/payments/success-c423ec16521d5906.js
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.266230 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/share/
+-rw-rw-rw-   0        0        0     7543 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-1c5c5056584e8afb.js
+-rw-rw-rw-   0        0        0      399 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/status-9047ec54adb32ef3.js
+-rw-rw-rw-   0        0        0    91460 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-rw-rw-   0        0        0     4976 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/webpack-305aad91bdd6a592.js
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.272236 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/css/
+-rw-rw-rw-   0        0        0   138266 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/css/59d85ffe80f6c774.css
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.327234 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/
+-rw-rw-rw-   0        0        0     2375 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/buildManifest.js
+-rw-rw-rw-   0        0        0       77 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/ssgManifest.js
+-rw-rw-rw-   0        0        0     4159 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/apple-touch-icon.png
+-rw-rw-rw-   0        0        0      730 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/favicon-16x16.png
+-rw-rw-rw-   0        0        0     1292 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/favicon-32x32.png
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:03.564228 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.430227 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/
+-rw-rw-rw-   0        0        0    34336 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff
+-rw-rw-rw-   0        0        0    27412 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2
+-rw-rw-rw-   0        0        0    35956 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff
+-rw-rw-rw-   0        0        0    28532 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2
+-rw-rw-rw-   0        0        0    35268 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff
+-rw-rw-rw-   0        0        0    28060 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2
+-rw-rw-rw-   0        0        0    37480 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff
+-rw-rw-rw-   0        0        0    29824 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.733233 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/
+-rw-rw-rw-   0        0        0    28076 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2
+-rw-rw-rw-   0        0        0     6912 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2
+-rw-rw-rw-   0        0        0     6908 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2
+-rw-rw-rw-   0        0        0    11348 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2
+-rw-rw-rw-   0        0        0    11316 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2
+-rw-rw-rw-   0        0        0    25324 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2
+-rw-rw-rw-   0        0        0    16780 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2
+-rw-rw-rw-   0        0        0    16988 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2
+-rw-rw-rw-   0        0        0    26272 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2
+-rw-rw-rw-   0        0        0    16400 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2
+-rw-rw-rw-   0        0        0    16440 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2
+-rw-rw-rw-   0        0        0    12216 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2
+-rw-rw-rw-   0        0        0    12028 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2
+-rw-rw-rw-   0        0        0    10344 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2
+-rw-rw-rw-   0        0        0     9644 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2
+-rw-rw-rw-   0        0        0     5468 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2
+-rw-rw-rw-   0        0        0     5208 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2
+-rw-rw-rw-   0        0        0     3624 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2
+-rw-rw-rw-   0        0        0     4928 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2
+-rw-rw-rw-   0        0        0    13568 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.751230 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/signifier/
+-rw-rw-rw-   0        0        0    56682 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2
+-rw-rw-rw-   0        0        0    56021 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2
+-rw-rw-rw-   0        0        0    56456 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2
+-rw-rw-rw-   0        0        0    53009 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light.woff2
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.910229 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/
+-rw-rw-rw-   0        0        0    34084 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2
+-rw-rw-rw-   0        0        0    33350 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2
+-rw-rw-rw-   0        0        0    40456 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2
+-rw-rw-rw-   0        0        0    37996 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2
+-rw-rw-rw-   0        0        0    38746 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2
+-rw-rw-rw-   0        0        0    35690 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2
+-rw-rw-rw-   0        0        0    28148 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2
+-rw-rw-rw-   0        0        0    27437 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2
+-rw-rw-rw-   0        0        0    28285 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2
+-rw-rw-rw-   0        0        0      336 2023-07-25 02:29:01.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/manifest.json
+-rw-rw-rw-   0        0        0     6133 2023-07-25 02:29:01.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/service-worker.js
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.920229 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/sweetalert2/
+-rw-rw-rw-   0        0        0    19844 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/sweetalert2/bulma.min.css
+-rw-rw-rw-   0        0        0    68840 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:03.567228 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/ulp/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:03.568229 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/ulp/react-components/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:03.569227 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:04.924230 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/css/
+-rw-rw-rw-   0        0        0   233073 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
+drwxrwxrwx   0        0        0        0 2023-07-27 01:56:05.007230 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/templates/
+-rw-rw-rw-   0        0        0     4915 2023-07-27 01:49:15.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/templates/404.html
+-rw-rw-rw-   0        0        0     7461 2023-07-27 01:39:58.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/templates/chat.html
+-rw-rw-rw-   0        0        0     4883 2023-07-27 01:40:05.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/templates/detail.html
+-rw-rw-rw-   0        0        0    40497 2023-07-27 01:47:58.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/templates/login.html
+-rw-rw-rw-   0        0        0     6134 2023-07-27 01:49:34.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/templates/share.html
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:59:44.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/py.typed
+-rw-rw-rw-   0        0        0    19767 2023-07-25 02:29:01.000000 shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/server.py
```

### Comparing `shootpandora-Cloud-20230725.1.3/LICENSE` & `shootpandora-Cloud-20230725.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/PKG-INFO` & `shootpandora-Cloud-20230725.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shootpandora-Cloud
-Version: 20230725.1.3
+Version: 20230725.1.4
 Summary: A package for shootpandora-ChatGPT
 Home-page: https://github.com/shoot82003/shootpandora-cloud
 Author: XiaoZhou Huang
 Author-email: shoot82003@qq.com
 Project-URL: Source, https://github.com/shoot82003/shootpandora-cloud
 Project-URL: Tracker, https://github.com/shoot82003/shootpandora-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
```

### Comparing `shootpandora-Cloud-20230725.1.3/README.md` & `shootpandora-Cloud-20230725.1.4/README.md`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/setup.py` & `shootpandora-Cloud-20230725.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/shootpandora_Cloud.egg-info/PKG-INFO` & `shootpandora-Cloud-20230725.1.4/shootpandora_Cloud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shootpandora-Cloud
-Version: 20230725.1.3
+Version: 20230725.1.4
 Summary: A package for shootpandora-ChatGPT
 Home-page: https://github.com/shoot82003/shootpandora-cloud
 Author: XiaoZhou Huang
 Author-email: shoot82003@qq.com
 Project-URL: Source, https://github.com/shoot82003/shootpandora-cloud
 Project-URL: Tracker, https://github.com/shoot82003/shootpandora-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
```

### Comparing `shootpandora-Cloud-20230725.1.3/shootpandora_Cloud.egg-info/SOURCES.txt` & `shootpandora-Cloud-20230725.1.4/shootpandora_Cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/238-882950710bdd3e1e.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/238-882950710bdd3e1e.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/271.f8fe486a0f5b221c.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/271.f8fe486a0f5b221c.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/2802bd5f-15923fb46be55b45.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/2802bd5f-15923fb46be55b45.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/297-e180277ece10e844.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/297-e180277ece10e844.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/412-c00b85b4ef66af2f.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/412-c00b85b4ef66af2f.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/435-2b015d294e66ccbc.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/435-2b015d294e66ccbc.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/564-f0043ba04d4fcd3d.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/564-f0043ba04d4fcd3d.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/68a27ff6-b1db347c50639918.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/68a27ff6-b1db347c50639918.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/800-a82eb647282afb06.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/800-a82eb647282afb06.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/937-36e251f389e9e752.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/937-36e251f389e9e752.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/984-1278472924e49180.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/984-1278472924e49180.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/bd26816a-7ae54dd3357d90b4.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/bd26816a-7ae54dd3357d90b4.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/main-0438431c68fbeb27.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/main-0438431c68fbeb27.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-1457e593ce508c31.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-1457e593ce508c31.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/admin-810915a9e0227b64.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/admin-810915a9e0227b64.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-b7d4a081f7ad5b5b.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-b7d4a081f7ad5b5b.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/app-573ad0910def0e5d.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/app-573ad0910def0e5d.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/error-9faed2db943661ab.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/error-9faed2db943661ab.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-7b50f284300a7ff6.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-7b50f284300a7ff6.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-47f3cd5abd2d99b6.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-47f3cd5abd2d99b6.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/login-267fffdf86e9e08a.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/login-267fffdf86e9e08a.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-5817b04f45f270e2.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-5817b04f45f270e2.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-060c0092bc682b49.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-060c0092bc682b49.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-5d264bebf7157821.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-5d264bebf7157821.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/index-b00721778b6b9fff.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/index-b00721778b6b9fff.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/payments/success-c423ec16521d5906.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/payments/success-c423ec16521d5906.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-1c5c5056584e8afb.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-1c5c5056584e8afb.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/chunks/webpack-305aad91bdd6a592.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/chunks/webpack-305aad91bdd6a592.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/css/59d85ffe80f6c774.css` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/css/59d85ffe80f6c774.css`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/buildManifest.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/buildManifest.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/apple-touch-icon.png` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/favicon-16x16.png` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/favicon-32x32.png` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/signifier/signifier-light.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/service-worker.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/service-worker.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/sweetalert2/bulma.min.css` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/sweetalert2/bulma.min.css`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css`

 * *Files identical despite different names*

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/templates/404.html` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/templates/404.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <meta charSet="utf-8"/>
   <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no"/>
   <link rel="manifest" href="/manifest.json">
   <meta property="og:title" content="ChatGPT"/>
   <meta property="og:image" content="https://chat.openai.com/images/chatgpt-share-og.png"/>
   <meta property="og:description" content="A conversational AI system that listens, learns, and challenges"/>
   <meta property="og:url" content="https://chat.openai.com"/>
-  <title>404: This page could not be found</title>
+  <title>shootchat.top黄晓周的ChatGPT----404页面</title>
   <meta name="next-head-count" content="8"/>
   <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png"/>
   <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png"/>
   <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png"/>
   <link rel="preconnect" href="{{api_prefix|safe}}"/>
   <link rel="preload" href="/fonts/soehne/soehne-buch.woff2" as="font" crossorigin=""/>
   <link rel="preload" href="/fonts/soehne/soehne-halbfett.woff2" as="font" crossorigin=""/>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/templates/chat.html` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/templates/chat.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!DOCTYPE html>
 <html>
     <head>
         <meta charSet="utf-8"/>
-        <title>ChatGPT</title>
+        <title>shootchat.top黄晓周的ChatGPT</title>
         <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no"/>
         <link rel="manifest" href="/manifest.json">
         <meta property="og:title" content="ChatGPT"/>
         <meta property="og:image" content="https://chat.openai.com/images/chatgpt-share-og.png"/>
         <meta property="og:description" content="A conversational AI system that listens, learns, and challenges"/>
         <meta property="og:url" content="https://chat.openai.com"/>
         <meta name="next-head-count" content="8"/>
```

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/templates/detail.html` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/templates/detail.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!DOCTYPE html>
 <html>
     <head>
         <meta charSet="utf-8"/>
-        <title>ChatGPT</title>
+        <title>shootchat.top黄晓周的ChatGPT</title>
         <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no"/>
         <link rel="manifest" href="/manifest.json">
         <meta property="og:title" content="ChatGPT"/>
         <meta property="og:image" content="https://chat.openai.com/images/chatgpt-share-og.png"/>
         <meta property="og:description" content="A conversational AI system that listens, learns, and challenges"/>
         <meta property="og:url" content="https://chat.openai.com"/>
         <meta name="next-head-count" content="8"/>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/templates/login.html` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/templates/login.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!DOCTYPE html>
 <html>
     <head>
         <meta charset="utf-8"/>
-        <title>login_to_ChatGPT</title>
+        <title>无需复杂验证直接登陆ChatGPT</title>
         <meta http-equiv="X-UA-Compatible" content="IE=edge"/>
         <meta name="viewport" content="width=device-width, initial-scale=1"/>
         <meta name="robots" content="noindex, nofollow"/>
         <link rel="manifest" href="/manifest.json">
         <link rel="preconnect" href="{{api_prefix|safe}}"/>
         <link rel="stylesheet" href="/ulp/react-components/1.66.5/css/main.cdn.min.css"/>
         <link rel="stylesheet" href="/sweetalert2/bulma.min.css"/>
```

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/flask/templates/share.html` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/flask/templates/share.html`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     <head>
         <meta charSet="utf-8"/>
         <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no"/>
         <link rel="manifest" href="/manifest.json">
         <meta property="og:title" content="ChatGPT"/>
         <meta property="og:description" content="A conversational AI system that listens, learns, and challenges"/>
         <meta property="og:url" content="https://chat.openai.com"/>
-        <title>Hello and assistance</title>
+        <title>shootchat.top黄晓周的ChatGPT</title>
         <meta property="og:site_name" content="ChatGPT"/>
         <meta name="robots" content="noindex,nofollow"/>
         <meta property="og:title" content="Hello and assistance"/>
         <meta property="og:image" content="/images/chatgpt-share-og.png"/>
         <meta name="next-head-count" content="11"/>
         <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png"/>
         <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png"/>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `shootpandora-Cloud-20230725.1.3/src/shootpandora_cloud/server.py` & `shootpandora-Cloud-20230725.1.4/src/shootpandora_cloud/server.py`

 * *Files identical despite different names*

