# Comparing `tmp/ait_gui-2.4.0.tar.gz` & `tmp/ait_gui-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ait_gui-2.4.0.tar", max compression
+gzip compressed data, was "ait_gui-2.4.1.tar", max compression
```

## Comparing `ait_gui-2.4.0.tar` & `ait_gui-2.4.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1074 2018-04-09 15:24:05.000000 ait_gui-2.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1969 2023-07-27 00:06:35.511125 ait_gui-2.4.0/README.rst
--rw-r--r--   0        0        0    45141 2023-07-26 22:50:05.507124 ait_gui-2.4.0/ait/gui/__init__.py
--rw-r--r--   0        0        0      769 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/bin/__init__.py
--rw-r--r--   0        0        0      249 2023-07-26 21:44:34.678072 ait_gui-2.4.0/ait/gui/bin/ait_example.py
--rw-r--r--   0        0        0     6665 2022-12-14 23:56:46.266769 ait_gui-2.4.0/ait/gui/openmct_adapter/ait_integration.js
--rw-r--r--   0        0        0     2478 2018-12-12 22:20:01.000000 ait_gui-2.4.0/ait/gui/openmct_adapter/example_ait_telem_fetch.js
--rw-r--r--   0        0        0       30 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/.babelrc
--rw-r--r--   0        0        0       40 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/.jshintrc
--rw-r--r--   0        0        0    52225 2022-12-14 23:56:46.267155 ait_gui-2.4.0/ait/gui/static/build/0292d248d009b01cf97cefdfa39c3cf3.svg
--rw-r--r--   0        0        0    15360 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/build/0a0697bc7da165088daf16abaa2b0b96.eot
--rw-r--r--   0        0        0    18028 2023-07-26 23:35:26.420515 ait_gui-2.4.0/ait/gui/static/build/448c34a56d699c29117adc64c43affeb.woff2
--rw-r--r--   0        0        0   108738 2023-07-26 23:35:26.420474 ait_gui-2.4.0/ait/gui/static/build/89889688147bd7575d6327160d64e760.svg
--rw-r--r--   0        0        0   162971 2023-07-26 23:35:26.420548 ait_gui-2.4.0/ait/gui/static/build/ait.bundle.css
--rw-r--r--   0        0        0   658979 2023-07-26 23:37:52.340499 ait_gui-2.4.0/ait/gui/static/build/ait.bundle.js
--rw-r--r--   0        0        0    45404 2023-07-26 23:35:26.420315 ait_gui-2.4.0/ait/gui/static/build/e18bbf611f2a2e43afc071aa2f4e1512.ttf
--rw-r--r--   0        0        0    20127 2023-07-26 23:35:26.420421 ait_gui-2.4.0/ait/gui/static/build/f4769f9bdb7466be65088239c12046d1.eot
--rw-r--r--   0        0        0    23424 2023-07-26 23:35:26.420267 ait_gui-2.4.0/ait/gui/static/build/fa2772327f55d8198301fdb8bcfc8158.woff
--rw-r--r--   0        0        0       55 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/css/ait/gui/Clock.css
--rw-r--r--   0        0        0     2630 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/css/ait/gui/Command.css
--rw-r--r--   0        0        0      650 2018-12-12 22:20:01.000000 ait_gui-2.4.0/ait/gui/static/css/ait/gui/Field.css
--rw-r--r--   0        0        0     2333 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/css/ait/gui/Messages.css
--rw-r--r--   0        0        0      491 2022-12-14 23:56:46.267406 ait_gui-2.4.0/ait/gui/static/css/ait/gui/Playback.css
--rw-r--r--   0        0        0      163 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/css/ait/gui/Plot.css
--rw-r--r--   0        0        0      282 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/css/ait/gui/Query.css
--rw-r--r--   0        0        0     1471 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/css/ait/gui/Script.css
--rw-r--r--   0        0        0     2158 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/css/ait/gui/Search.css
--rw-r--r--   0        0        0     1153 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/css/ait/gui/Sequence.css
--rw-r--r--   0        0        0     1256 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/css/ait/gui/Status.css
--rw-r--r--   0        0        0     1662 2022-12-14 23:56:46.267592 ait_gui-2.4.0/ait/gui/static/css/ait/gui/TabSet.css
--rw-r--r--   0        0        0     6546 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/css/typeahead.css
--rw-r--r--   0        0        0   106260 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/fonts/FontAwesome.otf
--rw-r--r--   0        0        0    68875 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   355981 2022-12-14 23:56:46.269215 ait_gui-2.4.0/ait/gui/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   138204 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    81284 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    64464 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0    20335 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0        0        0    62927 2022-12-14 23:56:46.269642 ait_gui-2.4.0/ait/gui/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0        0        0    41280 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0        0        0    23320 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0        0        0     4519 2019-08-20 18:41:51.553422 ait_gui-2.4.0/ait/gui/static/index.css
--rw-r--r--   0        0        0    12841 2022-12-14 23:52:07.537977 ait_gui-2.4.0/ait/gui/static/index.html
--rw-r--r--   0        0        0      954 2018-09-07 23:40:51.000000 ait_gui-2.4.0/ait/gui/static/index.js
--rw-r--r--   0        0        0     3187 2018-09-11 20:49:34.000000 ait_gui-2.4.0/ait/gui/static/js/ait/cmd.js
--rw-r--r--   0        0        0     7949 2021-03-10 17:25:54.272312 ait_gui-2.4.0/ait/gui/static/js/ait/dtype.js
--rw-r--r--   0        0        0     1591 2022-12-14 23:56:46.269863 ait_gui-2.4.0/ait/gui/static/js/ait/events.js
--rw-r--r--   0        0        0     5004 2018-09-11 21:26:36.000000 ait_gui-2.4.0/ait/gui/static/js/ait/evr.js
--rw-r--r--   0        0        0     3287 2022-12-14 23:56:46.270068 ait_gui-2.4.0/ait/gui/static/js/ait/format.js
--rw-r--r--   0        0        0     4258 2022-12-14 23:56:46.270270 ait_gui-2.4.0/ait/gui/static/js/ait/gui/Clock.js
--rw-r--r--   0        0        0    33698 2022-12-14 23:56:46.270566 ait_gui-2.4.0/ait/gui/static/js/ait/gui/Command.js
--rw-r--r--   0        0        0    15796 2022-12-14 23:56:46.270819 ait_gui-2.4.0/ait/gui/static/js/ait/gui/Field.js
--rw-r--r--   0        0        0     3573 2018-06-21 20:28:33.000000 ait_gui-2.4.0/ait/gui/static/js/ait/gui/Messages.js
--rw-r--r--   0        0        0    11272 2020-04-30 17:03:57.189860 ait_gui-2.4.0/ait/gui/static/js/ait/gui/Playback.js
--rw-r--r--   0        0        0    17615 2020-06-16 16:38:39.964042 ait_gui-2.4.0/ait/gui/static/js/ait/gui/Plot.js
--rw-r--r--   0        0        0    12406 2018-06-21 20:28:33.000000 ait_gui-2.4.0/ait/gui/static/js/ait/gui/Query.js
--rw-r--r--   0        0        0    20750 2022-12-14 23:56:46.271081 ait_gui-2.4.0/ait/gui/static/js/ait/gui/Script.js
--rw-r--r--   0        0        0    12402 2021-01-20 21:06:10.896566 ait_gui-2.4.0/ait/gui/static/js/ait/gui/Search.js
--rw-r--r--   0        0        0     6020 2018-06-21 20:28:33.000000 ait_gui-2.4.0/ait/gui/static/js/ait/gui/Sequence.js
--rw-r--r--   0        0        0     8941 2018-07-12 21:35:05.000000 ait_gui-2.4.0/ait/gui/static/js/ait/gui/Status.js
--rw-r--r--   0        0        0    12332 2022-12-14 23:56:46.272135 ait_gui-2.4.0/ait/gui/static/js/ait/gui/TabSet.js
--rw-r--r--   0        0        0     5222 2018-06-21 20:28:33.000000 ait_gui-2.4.0/ait/gui/static/js/ait/gui/Util.js
--rw-r--r--   0        0        0     6195 2022-12-14 23:56:46.272405 ait_gui-2.4.0/ait/gui/static/js/ait/gui/index.js
--rw-r--r--   0        0        0     1152 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/js/ait/index.js
--rw-r--r--   0        0        0     3772 2022-12-14 23:56:46.272642 ait_gui-2.4.0/ait/gui/static/js/ait/packets.js
--rw-r--r--   0        0        0     1496 2022-12-14 23:56:46.272824 ait_gui-2.4.0/ait/gui/static/js/ait/time.js
--rw-r--r--   0        0        0    11997 2021-01-20 21:06:10.899859 ait_gui-2.4.0/ait/gui/static/js/ait/tlm.js
--rw-r--r--   0        0        0     1780 2020-06-16 16:38:39.967861 ait_gui-2.4.0/ait/gui/static/js/ait/util.js
--rw-r--r--   0        0        0     2568 2022-12-14 23:56:46.273028 ait_gui-2.4.0/ait/gui/static/overrides.css
--rw-r--r--   0        0        0   244724 2023-07-26 23:37:52.341827 ait_gui-2.4.0/ait/gui/static/package-lock.json
--rw-r--r--   0        0        0     1021 2023-07-26 23:57:48.495676 ait_gui-2.4.0/ait/gui/static/package.json
--rw-r--r--   0        0        0       60 2022-12-14 23:56:46.273406 ait_gui-2.4.0/ait/gui/static/test/mocha.opts
--rw-r--r--   0        0        0     2552 2018-12-12 16:12:35.000000 ait_gui-2.4.0/ait/gui/static/test/test_clock.js
--rw-r--r--   0        0        0     1966 2018-09-11 20:49:34.000000 ait_gui-2.4.0/ait/gui/static/test/test_cmd.js
--rw-r--r--   0        0        0     3504 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/test/test_command.js
--rw-r--r--   0        0        0     3871 2018-09-11 21:26:36.000000 ait_gui-2.4.0/ait/gui/static/test/test_evr.js
--rw-r--r--   0        0        0     6669 2019-01-09 21:17:38.000000 ait_gui-2.4.0/ait/gui/static/test/test_field.js
--rw-r--r--   0        0        0     3802 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/test/test_messages.js
--rw-r--r--   0        0        0     2262 2018-05-16 21:01:17.000000 ait_gui-2.4.0/ait/gui/static/webpack.config.js
--rw-r--r--   0        0        0     2326 2023-07-27 00:04:33.027794 ait_gui-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     2898 1970-01-01 00:00:00.000000 ait_gui-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2018-04-09 15:24:05.000000 ait_gui-2.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     1969 2023-07-27 00:06:35.511125 ait_gui-2.4.1/README.rst
+-rw-r--r--   0        0        0    45141 2023-07-26 22:50:05.507124 ait_gui-2.4.1/ait/gui/__init__.py
+-rw-r--r--   0        0        0      769 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/bin/__init__.py
+-rw-r--r--   0        0        0      249 2023-07-26 21:44:34.678072 ait_gui-2.4.1/ait/gui/bin/ait_example.py
+-rw-r--r--   0        0        0     6665 2022-12-14 23:56:46.266769 ait_gui-2.4.1/ait/gui/openmct_adapter/ait_integration.js
+-rw-r--r--   0        0        0     2478 2018-12-12 22:20:01.000000 ait_gui-2.4.1/ait/gui/openmct_adapter/example_ait_telem_fetch.js
+-rw-r--r--   0        0        0       30 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/.babelrc
+-rw-r--r--   0        0        0       40 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/.jshintrc
+-rw-r--r--   0        0        0    52225 2022-12-14 23:56:46.267155 ait_gui-2.4.1/ait/gui/static/build/0292d248d009b01cf97cefdfa39c3cf3.svg
+-rw-r--r--   0        0        0    15360 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/build/0a0697bc7da165088daf16abaa2b0b96.eot
+-rw-r--r--   0        0        0    18028 2023-07-26 23:35:26.420515 ait_gui-2.4.1/ait/gui/static/build/448c34a56d699c29117adc64c43affeb.woff2
+-rw-r--r--   0        0        0   108738 2023-07-26 23:35:26.420474 ait_gui-2.4.1/ait/gui/static/build/89889688147bd7575d6327160d64e760.svg
+-rw-r--r--   0        0        0   162971 2023-07-26 23:35:26.420548 ait_gui-2.4.1/ait/gui/static/build/ait.bundle.css
+-rw-r--r--   0        0        0   658979 2023-07-26 23:37:52.340499 ait_gui-2.4.1/ait/gui/static/build/ait.bundle.js
+-rw-r--r--   0        0        0    45404 2023-07-26 23:35:26.420315 ait_gui-2.4.1/ait/gui/static/build/e18bbf611f2a2e43afc071aa2f4e1512.ttf
+-rw-r--r--   0        0        0    20127 2023-07-26 23:35:26.420421 ait_gui-2.4.1/ait/gui/static/build/f4769f9bdb7466be65088239c12046d1.eot
+-rw-r--r--   0        0        0    23424 2023-07-26 23:35:26.420267 ait_gui-2.4.1/ait/gui/static/build/fa2772327f55d8198301fdb8bcfc8158.woff
+-rw-r--r--   0        0        0       55 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/css/ait/gui/Clock.css
+-rw-r--r--   0        0        0     2630 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/css/ait/gui/Command.css
+-rw-r--r--   0        0        0      650 2018-12-12 22:20:01.000000 ait_gui-2.4.1/ait/gui/static/css/ait/gui/Field.css
+-rw-r--r--   0        0        0     2333 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/css/ait/gui/Messages.css
+-rw-r--r--   0        0        0      491 2022-12-14 23:56:46.267406 ait_gui-2.4.1/ait/gui/static/css/ait/gui/Playback.css
+-rw-r--r--   0        0        0      163 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/css/ait/gui/Plot.css
+-rw-r--r--   0        0        0      282 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/css/ait/gui/Query.css
+-rw-r--r--   0        0        0     1471 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/css/ait/gui/Script.css
+-rw-r--r--   0        0        0     2158 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/css/ait/gui/Search.css
+-rw-r--r--   0        0        0     1153 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/css/ait/gui/Sequence.css
+-rw-r--r--   0        0        0     1256 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/css/ait/gui/Status.css
+-rw-r--r--   0        0        0     1662 2022-12-14 23:56:46.267592 ait_gui-2.4.1/ait/gui/static/css/ait/gui/TabSet.css
+-rw-r--r--   0        0        0     6546 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/css/typeahead.css
+-rw-r--r--   0        0        0   106260 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/fonts/FontAwesome.otf
+-rw-r--r--   0        0        0    68875 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   355981 2022-12-14 23:56:46.269215 ait_gui-2.4.1/ait/gui/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   138204 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    81284 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    64464 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0    20335 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0        0        0    62927 2022-12-14 23:56:46.269642 ait_gui-2.4.1/ait/gui/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0        0        0    41280 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0        0        0    23320 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0        0        0     4519 2019-08-20 18:41:51.553422 ait_gui-2.4.1/ait/gui/static/index.css
+-rw-r--r--   0        0        0    12841 2022-12-14 23:52:07.537977 ait_gui-2.4.1/ait/gui/static/index.html
+-rw-r--r--   0        0        0      954 2018-09-07 23:40:51.000000 ait_gui-2.4.1/ait/gui/static/index.js
+-rw-r--r--   0        0        0     3187 2018-09-11 20:49:34.000000 ait_gui-2.4.1/ait/gui/static/js/ait/cmd.js
+-rw-r--r--   0        0        0     7949 2021-03-10 17:25:54.272312 ait_gui-2.4.1/ait/gui/static/js/ait/dtype.js
+-rw-r--r--   0        0        0     1591 2022-12-14 23:56:46.269863 ait_gui-2.4.1/ait/gui/static/js/ait/events.js
+-rw-r--r--   0        0        0     5004 2018-09-11 21:26:36.000000 ait_gui-2.4.1/ait/gui/static/js/ait/evr.js
+-rw-r--r--   0        0        0     3287 2022-12-14 23:56:46.270068 ait_gui-2.4.1/ait/gui/static/js/ait/format.js
+-rw-r--r--   0        0        0     4258 2022-12-14 23:56:46.270270 ait_gui-2.4.1/ait/gui/static/js/ait/gui/Clock.js
+-rw-r--r--   0        0        0    33698 2022-12-14 23:56:46.270566 ait_gui-2.4.1/ait/gui/static/js/ait/gui/Command.js
+-rw-r--r--   0        0        0    15796 2022-12-14 23:56:46.270819 ait_gui-2.4.1/ait/gui/static/js/ait/gui/Field.js
+-rw-r--r--   0        0        0     3573 2018-06-21 20:28:33.000000 ait_gui-2.4.1/ait/gui/static/js/ait/gui/Messages.js
+-rw-r--r--   0        0        0    11272 2020-04-30 17:03:57.189860 ait_gui-2.4.1/ait/gui/static/js/ait/gui/Playback.js
+-rw-r--r--   0        0        0    17615 2020-06-16 16:38:39.964042 ait_gui-2.4.1/ait/gui/static/js/ait/gui/Plot.js
+-rw-r--r--   0        0        0    12406 2018-06-21 20:28:33.000000 ait_gui-2.4.1/ait/gui/static/js/ait/gui/Query.js
+-rw-r--r--   0        0        0    20750 2022-12-14 23:56:46.271081 ait_gui-2.4.1/ait/gui/static/js/ait/gui/Script.js
+-rw-r--r--   0        0        0    12402 2021-01-20 21:06:10.896566 ait_gui-2.4.1/ait/gui/static/js/ait/gui/Search.js
+-rw-r--r--   0        0        0     6020 2018-06-21 20:28:33.000000 ait_gui-2.4.1/ait/gui/static/js/ait/gui/Sequence.js
+-rw-r--r--   0        0        0     8941 2018-07-12 21:35:05.000000 ait_gui-2.4.1/ait/gui/static/js/ait/gui/Status.js
+-rw-r--r--   0        0        0    12332 2022-12-14 23:56:46.272135 ait_gui-2.4.1/ait/gui/static/js/ait/gui/TabSet.js
+-rw-r--r--   0        0        0     5222 2018-06-21 20:28:33.000000 ait_gui-2.4.1/ait/gui/static/js/ait/gui/Util.js
+-rw-r--r--   0        0        0     6195 2022-12-14 23:56:46.272405 ait_gui-2.4.1/ait/gui/static/js/ait/gui/index.js
+-rw-r--r--   0        0        0     1152 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/js/ait/index.js
+-rw-r--r--   0        0        0     3772 2022-12-14 23:56:46.272642 ait_gui-2.4.1/ait/gui/static/js/ait/packets.js
+-rw-r--r--   0        0        0     1496 2022-12-14 23:56:46.272824 ait_gui-2.4.1/ait/gui/static/js/ait/time.js
+-rw-r--r--   0        0        0    11997 2021-01-20 21:06:10.899859 ait_gui-2.4.1/ait/gui/static/js/ait/tlm.js
+-rw-r--r--   0        0        0     1780 2020-06-16 16:38:39.967861 ait_gui-2.4.1/ait/gui/static/js/ait/util.js
+-rw-r--r--   0        0        0     2568 2022-12-14 23:56:46.273028 ait_gui-2.4.1/ait/gui/static/overrides.css
+-rw-r--r--   0        0        0   244724 2023-07-26 23:37:52.341827 ait_gui-2.4.1/ait/gui/static/package-lock.json
+-rw-r--r--   0        0        0     1021 2023-07-27 00:07:20.851535 ait_gui-2.4.1/ait/gui/static/package.json
+-rw-r--r--   0        0        0       60 2022-12-14 23:56:46.273406 ait_gui-2.4.1/ait/gui/static/test/mocha.opts
+-rw-r--r--   0        0        0     2552 2018-12-12 16:12:35.000000 ait_gui-2.4.1/ait/gui/static/test/test_clock.js
+-rw-r--r--   0        0        0     1966 2018-09-11 20:49:34.000000 ait_gui-2.4.1/ait/gui/static/test/test_cmd.js
+-rw-r--r--   0        0        0     3504 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/test/test_command.js
+-rw-r--r--   0        0        0     3871 2018-09-11 21:26:36.000000 ait_gui-2.4.1/ait/gui/static/test/test_evr.js
+-rw-r--r--   0        0        0     6669 2019-01-09 21:17:38.000000 ait_gui-2.4.1/ait/gui/static/test/test_field.js
+-rw-r--r--   0        0        0     3802 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/test/test_messages.js
+-rw-r--r--   0        0        0     2262 2018-05-16 21:01:17.000000 ait_gui-2.4.1/ait/gui/static/webpack.config.js
+-rw-r--r--   0        0        0     2326 2023-07-27 00:07:30.333690 ait_gui-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2898 1970-01-01 00:00:00.000000 ait_gui-2.4.1/PKG-INFO
```

### Comparing `ait_gui-2.4.0/LICENSE.txt` & `ait_gui-2.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/README.rst` & `ait_gui-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/__init__.py` & `ait_gui-2.4.1/ait/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/bin/__init__.py` & `ait_gui-2.4.1/ait/gui/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/openmct_adapter/ait_integration.js` & `ait_gui-2.4.1/ait/gui/openmct_adapter/ait_integration.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/openmct_adapter/example_ait_telem_fetch.js` & `ait_gui-2.4.1/ait/gui/openmct_adapter/example_ait_telem_fetch.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/build/0292d248d009b01cf97cefdfa39c3cf3.svg` & `ait_gui-2.4.1/ait/gui/static/build/0292d248d009b01cf97cefdfa39c3cf3.svg`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/build/0a0697bc7da165088daf16abaa2b0b96.eot` & `ait_gui-2.4.1/ait/gui/static/build/0a0697bc7da165088daf16abaa2b0b96.eot`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/build/448c34a56d699c29117adc64c43affeb.woff2` & `ait_gui-2.4.1/ait/gui/static/build/448c34a56d699c29117adc64c43affeb.woff2`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/build/89889688147bd7575d6327160d64e760.svg` & `ait_gui-2.4.1/ait/gui/static/build/89889688147bd7575d6327160d64e760.svg`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/build/ait.bundle.css` & `ait_gui-2.4.1/ait/gui/static/build/ait.bundle.css`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/build/ait.bundle.js` & `ait_gui-2.4.1/ait/gui/static/build/ait.bundle.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/build/e18bbf611f2a2e43afc071aa2f4e1512.ttf` & `ait_gui-2.4.1/ait/gui/static/build/e18bbf611f2a2e43afc071aa2f4e1512.ttf`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/build/f4769f9bdb7466be65088239c12046d1.eot` & `ait_gui-2.4.1/ait/gui/static/build/f4769f9bdb7466be65088239c12046d1.eot`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/build/fa2772327f55d8198301fdb8bcfc8158.woff` & `ait_gui-2.4.1/ait/gui/static/build/fa2772327f55d8198301fdb8bcfc8158.woff`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/css/ait/gui/Command.css` & `ait_gui-2.4.1/ait/gui/static/css/ait/gui/Command.css`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/css/ait/gui/Field.css` & `ait_gui-2.4.1/ait/gui/static/css/ait/gui/Field.css`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/css/ait/gui/Messages.css` & `ait_gui-2.4.1/ait/gui/static/css/ait/gui/Messages.css`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/css/ait/gui/Script.css` & `ait_gui-2.4.1/ait/gui/static/css/ait/gui/Script.css`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/css/ait/gui/Search.css` & `ait_gui-2.4.1/ait/gui/static/css/ait/gui/Search.css`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/css/ait/gui/Sequence.css` & `ait_gui-2.4.1/ait/gui/static/css/ait/gui/Sequence.css`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/css/ait/gui/Status.css` & `ait_gui-2.4.1/ait/gui/static/css/ait/gui/Status.css`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/css/ait/gui/TabSet.css` & `ait_gui-2.4.1/ait/gui/static/css/ait/gui/TabSet.css`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/css/typeahead.css` & `ait_gui-2.4.1/ait/gui/static/css/typeahead.css`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/fonts/FontAwesome.otf` & `ait_gui-2.4.1/ait/gui/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/fonts/fontawesome-webfont.eot` & `ait_gui-2.4.1/ait/gui/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/fonts/fontawesome-webfont.svg` & `ait_gui-2.4.1/ait/gui/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/fonts/fontawesome-webfont.ttf` & `ait_gui-2.4.1/ait/gui/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/fonts/fontawesome-webfont.woff` & `ait_gui-2.4.1/ait/gui/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/fonts/fontawesome-webfont.woff2` & `ait_gui-2.4.1/ait/gui/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/fonts/glyphicons-halflings-regular.eot` & `ait_gui-2.4.1/ait/gui/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/fonts/glyphicons-halflings-regular.svg` & `ait_gui-2.4.1/ait/gui/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/fonts/glyphicons-halflings-regular.ttf` & `ait_gui-2.4.1/ait/gui/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/fonts/glyphicons-halflings-regular.woff` & `ait_gui-2.4.1/ait/gui/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/index.css` & `ait_gui-2.4.1/ait/gui/static/index.css`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/index.html` & `ait_gui-2.4.1/ait/gui/static/index.html`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/index.js` & `ait_gui-2.4.1/ait/gui/static/index.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/cmd.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/cmd.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/dtype.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/dtype.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/events.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/events.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/evr.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/evr.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/format.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/format.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/gui/Clock.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/gui/Clock.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/gui/Command.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/gui/Command.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/gui/Field.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/gui/Field.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/gui/Messages.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/gui/Messages.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/gui/Playback.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/gui/Playback.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/gui/Plot.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/gui/Plot.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/gui/Query.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/gui/Query.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/gui/Script.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/gui/Script.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/gui/Search.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/gui/Search.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/gui/Sequence.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/gui/Sequence.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/gui/Status.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/gui/Status.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/gui/TabSet.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/gui/TabSet.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/gui/Util.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/gui/Util.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/gui/index.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/gui/index.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/index.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/index.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/packets.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/packets.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/time.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/time.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/tlm.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/tlm.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/js/ait/util.js` & `ait_gui-2.4.1/ait/gui/static/js/ait/util.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/overrides.css` & `ait_gui-2.4.1/ait/gui/static/overrides.css`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/package-lock.json` & `ait_gui-2.4.1/ait/gui/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/package.json` & `ait_gui-2.4.1/ait/gui/static/package.json`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/test/test_clock.js` & `ait_gui-2.4.1/ait/gui/static/test/test_clock.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/test/test_cmd.js` & `ait_gui-2.4.1/ait/gui/static/test/test_cmd.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/test/test_command.js` & `ait_gui-2.4.1/ait/gui/static/test/test_command.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/test/test_evr.js` & `ait_gui-2.4.1/ait/gui/static/test/test_evr.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/test/test_field.js` & `ait_gui-2.4.1/ait/gui/static/test/test_field.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/test/test_messages.js` & `ait_gui-2.4.1/ait/gui/static/test/test_messages.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/ait/gui/static/webpack.config.js` & `ait_gui-2.4.1/ait/gui/static/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ait_gui-2.4.0/pyproject.toml` & `ait_gui-2.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ait-gui"
-version = "2.4.0"
+version = "2.4.1"
 description = """\
     A framework for building a custom website for realtime telemetry \
     monitoring, commanding, and other MOS operations, built atop the \
     AIT Core libraries.\
     """
 license = "MIT"
 readme = "README.rst"
```

### Comparing `ait_gui-2.4.0/PKG-INFO` & `ait_gui-2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ait-gui
-Version: 2.4.0
+Version: 2.4.1
 Summary: A framework for building a custom website for realtime telemetry monitoring, commanding, and other MOS operations, built atop the AIT Core libraries.
 Home-page: https://github.com/NASA-AMMOS/AIT-GUI
 License: MIT
 Author: AMMOS Instrument Toolkit Development Team
 Author-email: ait-pmc@googlegroups.com
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

