# Comparing `tmp/shootpandora-ChatGPT-20230725.1.3.tar.gz` & `tmp/shootpandora-ChatGPT-20230725.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shootpandora-ChatGPT-20230725.1.3.tar", last modified: Wed Jul 26 09:45:53 2023, max compression
+gzip compressed data, was "shootpandora-ChatGPT-20230725.1.4.tar", last modified: Thu Jul 27 01:55:59 2023, max compression
```

## Comparing `shootpandora-ChatGPT-20230725.1.3.tar` & `shootpandora-ChatGPT-20230725.1.4.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.865728 shootpandora-ChatGPT-20230725.1.3/
--rw-rw-rw-   0        0        0    18431 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/LICENSE
--rw-rw-rw-   0        0        0      192 2023-07-24 09:18:37.000000 shootpandora-ChatGPT-20230725.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     7062 2023-07-26 09:45:53.863729 shootpandora-ChatGPT-20230725.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5472 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-20230725.1.3/README.md
--rw-rw-rw-   0        0        0      288 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/requirements.txt
--rw-rw-rw-   0        0        0       77 2023-07-26 09:40:20.000000 shootpandora-ChatGPT-20230725.1.3/requirements_api.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 09:45:53.865728 shootpandora-ChatGPT-20230725.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2547 2023-07-26 09:40:20.000000 shootpandora-ChatGPT-20230725.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.379728 shootpandora-ChatGPT-20230725.1.3/shootpandora_ChatGPT.egg-info/
--rw-rw-rw-   0        0        0     7062 2023-07-26 09:45:52.000000 shootpandora-ChatGPT-20230725.1.3/shootpandora_ChatGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4634 2023-07-26 09:45:53.000000 shootpandora-ChatGPT-20230725.1.3/shootpandora_ChatGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 09:45:52.000000 shootpandora-ChatGPT-20230725.1.3/shootpandora_ChatGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2023-07-26 09:45:52.000000 shootpandora-ChatGPT-20230725.1.3/shootpandora_ChatGPT.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      400 2023-07-26 09:45:52.000000 shootpandora-ChatGPT-20230725.1.3/shootpandora_ChatGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-26 09:45:52.000000 shootpandora-ChatGPT-20230725.1.3/shootpandora_ChatGPT.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.267732 shootpandora-ChatGPT-20230725.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.402727 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/
--rw-rw-rw-   0        0        0       57 2023-07-26 09:40:20.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/__init__.py
--rw-rw-rw-   0        0        0      112 2023-07-24 09:18:37.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.418728 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/bots/
--rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/bots/__init__.py
--rw-rw-rw-   0        0        0    17946 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/bots/legacy.py
--rw-rw-rw-   0        0        0    10683 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/bots/server.py
--rw-rw-rw-   0        0        0     2232 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/cloud_launcher.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.449727 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/exts/
--rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/exts/__init__.py
--rw-rw-rw-   0        0        0      540 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/exts/config.py
--rw-rw-rw-   0        0        0      968 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/exts/hooks.py
--rw-rw-rw-   0        0        0      502 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/exts/sentry.py
--rw-rw-rw-   0        0        0     1841 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/exts/token.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.311731 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.467729 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.277727 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.298735 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.574728 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/
--rw-rw-rw-   0        0        0   905465 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
--rw-rw-rw-   0        0        0    14115 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
--rw-rw-rw-   0        0        0     9531 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
--rw-rw-rw-   0        0        0   264961 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
--rw-rw-rw-   0        0        0    13157 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
--rw-rw-rw-   0        0        0    24146 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
--rw-rw-rw-   0        0        0    20480 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
--rw-rw-rw-   0        0        0     3232 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
--rw-rw-rw-   0        0        0      389 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
--rw-rw-rw-   0        0        0    11682 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
--rw-rw-rw-   0        0        0     2433 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
--rw-rw-rw-   0        0        0      462 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
--rw-rw-rw-   0        0        0   141402 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
--rw-rw-rw-   0        0        0   105264 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.585729 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/pages/
--rw-rw-rw-   0        0        0   305775 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
--rw-rw-rw-   0        0        0      250 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.590728 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/pages/chat/
--rw-rw-rw-   0        0        0   149542 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
--rw-rw-rw-   0        0        0    91461 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-rw-rw-   0        0        0     3926 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.596728 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/css/
--rw-rw-rw-   0        0        0   108647 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/css/ac221fb2caad35a6.css
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.612741 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
--rw-rw-rw-   0        0        0     2308 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
--rw-rw-rw-   0        0        0       77 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
--rw-rw-rw-   0        0        0     4159 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/apple-touch-icon.png
--rw-rw-rw-   0        0        0      730 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/favicon-16x16.png
--rw-rw-rw-   0        0        0     1292 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/favicon-32x32.png
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.755731 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/
--rw-rw-rw-   0        0        0     7716 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
--rw-rw-rw-   0        0        0     7656 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
--rw-rw-rw-   0        0        0    13296 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
--rw-rw-rw-   0        0        0    13208 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
--rw-rw-rw-   0        0        0    29912 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Main-Bold.woff
--rw-rw-rw-   0        0        0    19412 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
--rw-rw-rw-   0        0        0    19676 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Main-Italic.woff
--rw-rw-rw-   0        0        0    30772 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Main-Regular.woff
--rw-rw-rw-   0        0        0    18668 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
--rw-rw-rw-   0        0        0    18748 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Math-Italic.woff
--rw-rw-rw-   0        0        0    14408 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
--rw-rw-rw-   0        0        0    14112 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
--rw-rw-rw-   0        0        0    12316 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
--rw-rw-rw-   0        0        0    10588 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Script-Regular.woff
--rw-rw-rw-   0        0        0     6496 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Size1-Regular.woff
--rw-rw-rw-   0        0        0     6188 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Size2-Regular.woff
--rw-rw-rw-   0        0        0     4420 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Size3-Regular.woff
--rw-rw-rw-   0        0        0     5980 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Size4-Regular.woff
--rw-rw-rw-   0        0        0    16028 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
--rw-rw-rw-   0        0        0   324208 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/Signifier-Regular.otf
--rw-rw-rw-   0        0        0   210840 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/Sohne-Buch.otf
--rw-rw-rw-   0        0        0   230012 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/Sohne-Halbfett.otf
--rw-rw-rw-   0        0        0    30824 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/SohneMono-Buch.otf
--rw-rw-rw-   0        0        0    31116 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/SohneMono-Halbfett.otf
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.307727 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/images/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.308726 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/images/2022/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.761728 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/images/2022/11/
--rw-rw-rw-   0        0        0     1714 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/images/2022/11/ChatGPT.jpg
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.767730 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/templates/
--rw-rw-rw-   0        0        0    10835 2023-07-26 09:42:42.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/templates/chat.html
--rw-rw-rw-   0        0        0     7540 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/launcher.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.795728 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/migrations/
--rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/migrations/__init__.py
--rw-rw-rw-   0        0        0      262 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/migrations/database.py
--rw-rw-rw-   0        0        0      640 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/migrations/migrate.py
--rw-rw-rw-   0        0        0     4293 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/migrations/models.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.807728 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/migrations/scripts/
--rw-rw-rw-   0        0        0      904 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/migrations/scripts/20230308_01_7ctOr.sql
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.840728 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/openai/
--rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/openai/__init__.py
--rw-rw-rw-   0        0        0    12076 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/openai/api.py
--rw-rw-rw-   0        0        0     9090 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/openai/auth.py
--rw-rw-rw-   0        0        0      439 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/openai/token.py
--rw-rw-rw-   0        0        0     3532 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/openai/utils.py
--rw-rw-rw-   0        0        0        0 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-26 09:45:53.857728 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/turbo/
--rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/turbo/__init__.py
--rw-rw-rw-   0        0        0     6494 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/turbo/base.py
--rw-rw-rw-   0        0        0    12819 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.3/src/shootpandora/turbo/chat.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:59.281235 shootpandora-ChatGPT-20230725.1.4/
+-rw-rw-rw-   0        0        0    18431 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/LICENSE
+-rw-rw-rw-   0        0        0      192 2023-07-24 09:18:37.000000 shootpandora-ChatGPT-20230725.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     7062 2023-07-27 01:55:59.279228 shootpandora-ChatGPT-20230725.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5472 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-20230725.1.4/README.md
+-rw-rw-rw-   0        0        0      288 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/requirements.txt
+-rw-rw-rw-   0        0        0       77 2023-07-27 01:55:10.000000 shootpandora-ChatGPT-20230725.1.4/requirements_api.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 01:55:59.282229 shootpandora-ChatGPT-20230725.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     2547 2023-07-27 01:55:10.000000 shootpandora-ChatGPT-20230725.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:58.893229 shootpandora-ChatGPT-20230725.1.4/shootpandora_ChatGPT.egg-info/
+-rw-rw-rw-   0        0        0     7062 2023-07-27 01:55:58.000000 shootpandora-ChatGPT-20230725.1.4/shootpandora_ChatGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4634 2023-07-27 01:55:58.000000 shootpandora-ChatGPT-20230725.1.4/shootpandora_ChatGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 01:55:58.000000 shootpandora-ChatGPT-20230725.1.4/shootpandora_ChatGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2023-07-27 01:55:58.000000 shootpandora-ChatGPT-20230725.1.4/shootpandora_ChatGPT.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      400 2023-07-27 01:55:58.000000 shootpandora-ChatGPT-20230725.1.4/shootpandora_ChatGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-27 01:55:58.000000 shootpandora-ChatGPT-20230725.1.4/shootpandora_ChatGPT.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:58.797227 shootpandora-ChatGPT-20230725.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:58.917229 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/
+-rw-rw-rw-   0        0        0       57 2023-07-27 01:55:10.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/__init__.py
+-rw-rw-rw-   0        0        0      112 2023-07-24 09:18:37.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:58.931237 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/bots/
+-rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/bots/__init__.py
+-rw-rw-rw-   0        0        0    17946 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/bots/legacy.py
+-rw-rw-rw-   0        0        0    10683 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/bots/server.py
+-rw-rw-rw-   0        0        0     2232 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/cloud_launcher.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:58.952229 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/exts/
+-rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/exts/__init__.py
+-rw-rw-rw-   0        0        0      540 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/exts/config.py
+-rw-rw-rw-   0        0        0      968 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/exts/hooks.py
+-rw-rw-rw-   0        0        0      502 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/exts/sentry.py
+-rw-rw-rw-   0        0        0     1841 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/exts/token.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:58.835234 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:58.965232 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:58.806231 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:58.813228 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:59.050237 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/
+-rw-rw-rw-   0        0        0  1582498 2023-07-27 01:30:26.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
+-rw-rw-rw-   0        0        0    31366 2023-07-27 01:30:08.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
+-rw-rw-rw-   0        0        0    18471 2023-07-27 01:30:35.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
+-rw-rw-rw-   0        0        0   487275 2023-07-27 01:30:00.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
+-rw-rw-rw-   0        0        0    31000 2023-07-27 01:30:42.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
+-rw-rw-rw-   0        0        0    54437 2023-07-27 01:30:49.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
+-rw-rw-rw-   0        0        0    43027 2023-07-27 01:30:56.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
+-rw-rw-rw-   0        0        0     6762 2023-07-27 01:31:04.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
+-rw-rw-rw-   0        0        0      899 2023-07-27 01:30:15.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
+-rw-rw-rw-   0        0        0    22190 2023-07-27 01:31:11.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
+-rw-rw-rw-   0        0        0     5560 2023-07-27 01:31:17.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
+-rw-rw-rw-   0        0        0     1216 2023-07-27 01:31:23.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
+-rw-rw-rw-   0        0        0   339247 2023-07-27 01:31:31.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
+-rw-rw-rw-   0        0        0   225240 2023-07-27 01:31:39.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:59.060230 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/pages/
+-rw-rw-rw-   0        0        0   675027 2023-07-27 01:51:57.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
+-rw-rw-rw-   0        0        0      368 2023-07-27 01:52:02.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:59.066229 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/pages/chat/
+-rw-rw-rw-   0        0        0   340505 2023-07-27 01:51:24.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
+-rw-rw-rw-   0        0        0   179166 2023-07-27 01:31:47.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-rw-rw-   0        0        0     7447 2023-07-27 01:31:54.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:59.071231 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/css/
+-rw-rw-rw-   0        0        0   108647 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/css/ac221fb2caad35a6.css
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:59.078230 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
+-rw-rw-rw-   0        0        0     2663 2023-07-27 01:53:11.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
+-rw-rw-rw-   0        0        0       77 2023-07-27 01:53:19.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
+-rw-rw-rw-   0        0        0     4159 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/apple-touch-icon.png
+-rw-rw-rw-   0        0        0      730 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/favicon-16x16.png
+-rw-rw-rw-   0        0        0     1292 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/favicon-32x32.png
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:59.203232 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/
+-rw-rw-rw-   0        0        0     7716 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-rw-rw-   0        0        0     7656 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-rw-rw-   0        0        0    13296 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
+-rw-rw-rw-   0        0        0    13208 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
+-rw-rw-rw-   0        0        0    29912 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Main-Bold.woff
+-rw-rw-rw-   0        0        0    19412 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
+-rw-rw-rw-   0        0        0    19676 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Main-Italic.woff
+-rw-rw-rw-   0        0        0    30772 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Main-Regular.woff
+-rw-rw-rw-   0        0        0    18668 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
+-rw-rw-rw-   0        0        0    18748 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Math-Italic.woff
+-rw-rw-rw-   0        0        0    14408 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
+-rw-rw-rw-   0        0        0    14112 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
+-rw-rw-rw-   0        0        0    12316 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
+-rw-rw-rw-   0        0        0    10588 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Script-Regular.woff
+-rw-rw-rw-   0        0        0     6496 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Size1-Regular.woff
+-rw-rw-rw-   0        0        0     6188 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Size2-Regular.woff
+-rw-rw-rw-   0        0        0     4420 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Size3-Regular.woff
+-rw-rw-rw-   0        0        0     5980 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Size4-Regular.woff
+-rw-rw-rw-   0        0        0    16028 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
+-rw-rw-rw-   0        0        0   324208 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/Signifier-Regular.otf
+-rw-rw-rw-   0        0        0   210840 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/Sohne-Buch.otf
+-rw-rw-rw-   0        0        0   230012 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/Sohne-Halbfett.otf
+-rw-rw-rw-   0        0        0    30824 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/SohneMono-Buch.otf
+-rw-rw-rw-   0        0        0    31116 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/SohneMono-Halbfett.otf
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:58.833230 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/images/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:58.834228 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/images/2022/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:59.215230 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/images/2022/11/
+-rw-rw-rw-   0        0        0     1714 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/images/2022/11/ChatGPT.jpg
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:59.220230 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/templates/
+-rw-rw-rw-   0        0        0    11150 2023-07-27 01:46:40.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/templates/chat.html
+-rw-rw-rw-   0        0        0     7540 2023-07-24 09:19:09.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/launcher.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:59.238231 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/migrations/
+-rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/migrations/__init__.py
+-rw-rw-rw-   0        0        0      262 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/migrations/database.py
+-rw-rw-rw-   0        0        0      640 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/migrations/migrate.py
+-rw-rw-rw-   0        0        0     4293 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/migrations/models.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:59.241225 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/migrations/scripts/
+-rw-rw-rw-   0        0        0      904 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/migrations/scripts/20230308_01_7ctOr.sql
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:59.264229 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/openai/
+-rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/openai/__init__.py
+-rw-rw-rw-   0        0        0    12076 2023-07-24 09:18:38.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/openai/api.py
+-rw-rw-rw-   0        0        0     9090 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/openai/auth.py
+-rw-rw-rw-   0        0        0      439 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/openai/token.py
+-rw-rw-rw-   0        0        0     3532 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/openai/utils.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-27 01:55:59.275225 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/turbo/
+-rw-rw-rw-   0        0        0       25 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/turbo/__init__.py
+-rw-rw-rw-   0        0        0     6494 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/turbo/base.py
+-rw-rw-rw-   0        0        0    12819 2023-07-17 02:18:51.000000 shootpandora-ChatGPT-20230725.1.4/src/shootpandora/turbo/chat.py
```

### Comparing `shootpandora-ChatGPT-20230725.1.3/LICENSE` & `shootpandora-ChatGPT-20230725.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/PKG-INFO` & `shootpandora-ChatGPT-20230725.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shootpandora-ChatGPT
-Version: 20230725.1.3
+Version: 20230725.1.4
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/shoot82003/shootpandora
 Author: XiaoZhou Huang
 Author-email: shoot82003@qq.com
 Project-URL: Source, https://github.com/shoot82003/shootpandora
 Project-URL: Tracker, https://github.com/shoot82003/shootpandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shootpandora-ChatGPT Version: 20230725.1.3 Summary:
+Metadata-Version: 2.1 Name: shootpandora-ChatGPT Version: 20230725.1.4 Summary:
 A command-line interface to ChatGPT Home-page: https://github.com/shoot82003/
 shootpandora Author: XiaoZhou Huang Author-email: shoot82003@qq.com Project-
 URL: Source, https://github.com/shoot82003/shootpandora Project-URL: Tracker,
 https://github.com/shoot82003/shootpandora/issues Keywords: OpenAI ChatGPT
 ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301 Classifier: Development Status ::
 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Web Environment Classifier: Framework :: Flask Classifier:
```

### Comparing `shootpandora-ChatGPT-20230725.1.3/README.md` & `shootpandora-ChatGPT-20230725.1.4/README.md`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/setup.py` & `shootpandora-ChatGPT-20230725.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     url='https://github.com/shoot82003/shootpandora',
     packages=find_packages('src'),
     package_dir={'shootpandora': 'src/shootpandora'},
     include_package_data=True,
     install_requires=requirements,
     extras_require={
         'api': requirements_api,
-        'cloud': ['shootpandora-cloud~=20230725.1.3'],
+        'cloud': ['shootpandora-cloud~=20230725.1.4'],
     },
     entry_points={
         'console_scripts': [
             'shootpandora = shootpandora.launcher:run',
             'shootpandora-cloud = shootpandora.cloud_launcher:run',
         ]
     },
```

### Comparing `shootpandora-ChatGPT-20230725.1.3/shootpandora_ChatGPT.egg-info/PKG-INFO` & `shootpandora-ChatGPT-20230725.1.4/shootpandora_ChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shootpandora-ChatGPT
-Version: 20230725.1.3
+Version: 20230725.1.4
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/shoot82003/shootpandora
 Author: XiaoZhou Huang
 Author-email: shoot82003@qq.com
 Project-URL: Source, https://github.com/shoot82003/shootpandora
 Project-URL: Tracker, https://github.com/shoot82003/shootpandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shootpandora-ChatGPT Version: 20230725.1.3 Summary:
+Metadata-Version: 2.1 Name: shootpandora-ChatGPT Version: 20230725.1.4 Summary:
 A command-line interface to ChatGPT Home-page: https://github.com/shoot82003/
 shootpandora Author: XiaoZhou Huang Author-email: shoot82003@qq.com Project-
 URL: Source, https://github.com/shoot82003/shootpandora Project-URL: Tracker,
 https://github.com/shoot82003/shootpandora/issues Keywords: OpenAI ChatGPT
 ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301 Classifier: Development Status ::
 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Web Environment Classifier: Framework :: Flask Classifier:
```

### Comparing `shootpandora-ChatGPT-20230725.1.3/shootpandora_ChatGPT.egg-info/SOURCES.txt` & `shootpandora-ChatGPT-20230725.1.4/shootpandora_ChatGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/bots/legacy.py` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/bots/legacy.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/bots/server.py` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/bots/server.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/cloud_launcher.py` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/cloud_launcher.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/exts/config.py` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/exts/config.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/exts/hooks.py` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/exts/hooks.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/exts/token.py` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/exts/token.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/_next/static/css/ac221fb2caad35a6.css` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/_next/static/css/ac221fb2caad35a6.css`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/apple-touch-icon.png` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/favicon-16x16.png` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/favicon-32x32.png` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Main-Bold.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Main-Italic.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Main-Regular.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Math-Italic.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Script-Regular.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Size1-Regular.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Size2-Regular.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Size3-Regular.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Size4-Regular.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/Signifier-Regular.otf` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/Signifier-Regular.otf`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/Sohne-Buch.otf` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/Sohne-Buch.otf`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/Sohne-Halbfett.otf` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/Sohne-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/SohneMono-Buch.otf` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/SohneMono-Buch.otf`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/fonts/SohneMono-Halbfett.otf` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/fonts/SohneMono-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/static/images/2022/11/ChatGPT.jpg` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/static/images/2022/11/ChatGPT.jpg`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/flask/templates/chat.html` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/flask/templates/chat.html`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     <meta name="description" content="A conversational AI system that listens, learns, and challenges"/>
     <meta property="og:title" content="ChatGPT"/>
     <meta property="og:description" content="A conversational AI system that listens, learns, and challenges"/>
     <meta property="og:url" content="https://chat.openai.com"/>
     <link rel="preload" href="/_next/static/css/ac221fb2caad35a6.css" as="style"/>
     <link rel="stylesheet" href="/_next/static/css/ac221fb2caad35a6.css" data-n-g=""/>
     <noscript data-n-css=""></noscript>
-    <script>window.__shootpandora_base='{{shootpandora_base|safe}}';window.__shootpandora_sentry={{shootpandora_sentry|lower}};</script>
+    <script>window.__shootpandora_base='{{shootpandora_base|safe}}';window.__shootpandora_sentry='{{shootpandora_sentry|lower}}';</script>
     <script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script>
     <script src="/_next/static/chunks/webpack-c9a868e8e0796ec6.js" defer=""></script>
     <script src="/_next/static/chunks/framework-7a789ee31d2a7534.js" defer=""></script>
     <script src="/_next/static/chunks/main-149b337e061b4d04.js" defer=""></script>
     <script src="/_next/static/chunks/pages/_app-aaa11de1926dcafe.js" defer=""></script>
     <script src="/_next/static/chunks/68a27ff6-1185184b61bc22d0.js" defer=""></script>
     <script src="/_next/static/chunks/1f110208-44a6f43ddc5e9011.js" defer=""></script>
@@ -132,9 +132,18 @@
                 </div>
             </div>
         </div>
     </div>
     <div class="absolute top-0 left-0 right-0 z-[2]"></div>
 </div>
 <script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"user":{"id":"user-000000000000000000000000","name":"admin@openai.com","email":"admin@openai.com","image":null,"picture":null,"groups":[]},"serviceStatus":{},"userCountry":"US","geoOk":true,"serviceAnnouncement":{"paid":{},"public":{}},"isUserInCanPayGroup":true},"__N_SSP":true},"page":"/chat/[[...chatId]]","query":{{query|tojson|safe}},"buildId":"olf4sv64FWIcQ_zCGl90t","isFallback":false,"gssp":true,"scriptLoader":[]}</script>
+<script>
+    var _hmt = _hmt || [];
+    (function() {
+      var hm = document.createElement("script");
+      hm.src = "https://hm.baidu.com/hm.js?3b8cb49fc337ed33a9d021523be12fec";
+      var s = document.getElementsByTagName("script")[0]; 
+      s.parentNode.insertBefore(hm, s);
+    })();
+</script>    
 </body>
 </html>
```

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/launcher.py` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/launcher.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/migrations/migrate.py` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/migrations/models.py` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/migrations/models.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/migrations/scripts/20230308_01_7ctOr.sql` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/migrations/scripts/20230308_01_7ctOr.sql`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/openai/api.py` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/openai/api.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/openai/auth.py` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/openai/auth.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/openai/utils.py` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/openai/utils.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/turbo/base.py` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/turbo/base.py`

 * *Files identical despite different names*

### Comparing `shootpandora-ChatGPT-20230725.1.3/src/shootpandora/turbo/chat.py` & `shootpandora-ChatGPT-20230725.1.4/src/shootpandora/turbo/chat.py`

 * *Files identical despite different names*

