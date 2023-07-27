# Comparing `tmp/gmpacket-0.1.3.tar.gz` & `tmp/gmpacket-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmpacket-0.1.3.tar", last modified: Wed Apr 12 17:47:41 2023, max compression
+gzip compressed data, was "gmpacket-0.1.4.tar", last modified: Thu Jul 27 17:02:23 2023, max compression
```

## Comparing `gmpacket-0.1.3.tar` & `gmpacket-0.1.4.tar`

### file list

```diff
@@ -1,121 +1,28 @@
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.960767 gmpacket-0.1.3/
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      155 2023-04-12 17:41:09.000000 gmpacket-0.1.3/.gitignore
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      761 2023-04-10 20:24:32.000000 gmpacket-0.1.3/DISCLAIMER.md
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      179 2023-04-10 20:24:32.000000 gmpacket-0.1.3/LICENSE.md
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)       63 2023-04-12 17:23:01.000000 gmpacket-0.1.3/MANIFEST.in
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2083 2023-04-12 17:47:41.959819 gmpacket-0.1.3/PKG-INFO
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1312 2023-04-10 20:24:32.000000 gmpacket-0.1.3/README.md
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.474021 gmpacket-0.1.3/docs/
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      230 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/.buildinfo
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-11 20:38:42.000000 gmpacket-0.1.3/docs/.nojekyll
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.494982 gmpacket-0.1.3/docs/_sources/
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      892 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/dev.md.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2377 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/examples.md.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1449 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_sources/geojson.md.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1229 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/getting_started.md.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2014 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/index.md.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     4864 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/pydantic_demo.md.txt
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.543528 gmpacket-0.1.3/docs/_sources/specification/
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1322 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/base.md.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1969 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/event.md.txt
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.556911 gmpacket-0.1.3/docs/_sources/specification/features/
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      123 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/features/index.md.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     3722 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/features/metrics_dict.md.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1975 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/features/station.md.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     5817 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/features/streams_traces.md.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      150 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/index.md.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     4561 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/provenance.md.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2096 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_sources/terms.md.txt
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.792101 gmpacket-0.1.3/docs/_static/
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    53968 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_static/GMP.png
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     4418 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    14810 2023-04-11 20:38:41.000000 gmpacket-0.1.3/docs/_static/basic.css
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      313 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/check-solid.svg
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     9031 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/clipboard.min.js
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      411 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/copy-button.svg
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2060 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/copybutton.css
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     8472 2023-04-11 20:38:41.000000 gmpacket-0.1.3/docs/_static/copybutton.js
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2698 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/copybutton_funcs.js
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.794758 gmpacket-0.1.3/docs/_static/css/
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)       65 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_static/css/custom.css
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1266 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/debug.css
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)   476986 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_static/demo-dark.png
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)   452305 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_static/demo-light.png
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)   775827 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_static/demo.png
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     4472 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/doctools.js
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      444 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_static/documentation_options.js
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      286 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/file.png
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)   288580 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/jquery-3.6.0.js
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    89501 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/jquery.js
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     4758 2023-04-11 20:38:41.000000 gmpacket-0.1.3/docs/_static/language_data.js
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)       90 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/minus.png
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    39364 2023-04-11 19:40:39.000000 gmpacket-0.1.3/docs/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2110 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_static/pied-piper-admonition.css
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)       90 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/plus.png
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    21072 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_static/pygments.css
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      182 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_static/readthedocs-dummy.js
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.816776 gmpacket-0.1.3/docs/_static/scripts/
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-11 19:40:39.000000 gmpacket-0.1.3/docs/_static/scripts/furo-extensions.js
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     5265 2023-04-11 19:40:39.000000 gmpacket-0.1.3/docs/_static/scripts/furo.js
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      187 2023-04-11 19:40:39.000000 gmpacket-0.1.3/docs/_static/scripts/furo.js.LICENSE.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    28242 2023-04-11 19:40:39.000000 gmpacket-0.1.3/docs/_static/scripts/furo.js.map
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    18215 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/searchtools.js
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     6034 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/skeleton.css
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     4712 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/sphinx_highlight.js
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.847359 gmpacket-0.1.3/docs/_static/styles/
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     5529 2023-04-11 19:40:39.000000 gmpacket-0.1.3/docs/_static/styles/furo-extensions.css
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     7809 2023-04-11 19:40:39.000000 gmpacket-0.1.3/docs/_static/styles/furo-extensions.css.map
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    48697 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_static/styles/furo.css
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    73615 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_static/styles/furo.css.map
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2589 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/tabs.css
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      551 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/tabs.js
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    68420 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/underscore-1.13.1.js
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    19530 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/underscore.js
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    16698 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/dev.html
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    16877 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/examples.html
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    13090 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/genindex.html
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    18777 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/geojson.html
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    18471 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/getting_started.html
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    15851 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/index.html
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      963 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/objects.inv
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    53563 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/pydantic_demo.html
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    13318 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/search.html
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    15652 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/searchindex.js
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.878280 gmpacket-0.1.3/docs/specification/
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    16749 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/specification/base.html
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    18425 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/specification/event.html
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.904471 gmpacket-0.1.3/docs/specification/features/
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    14629 2023-04-11 21:09:34.000000 gmpacket-0.1.3/docs/specification/features/index.html
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    22987 2023-04-11 21:09:34.000000 gmpacket-0.1.3/docs/specification/features/metrics_dict.html
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    19060 2023-04-11 21:09:34.000000 gmpacket-0.1.3/docs/specification/features/station.html
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    26764 2023-04-11 21:09:34.000000 gmpacket-0.1.3/docs/specification/features/streams_traces.html
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    14977 2023-04-11 21:09:34.000000 gmpacket-0.1.3/docs/specification/index.html
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    29758 2023-04-11 21:09:34.000000 gmpacket-0.1.3/docs/specification/provenance.html
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    16658 2023-04-11 21:09:34.000000 gmpacket-0.1.3/docs/terms.html
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.915513 gmpacket-0.1.3/gmpacket/
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)       42 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/README.md
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/__init__.py
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.236879 gmpacket-0.1.3/gmpacket/data/
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.954565 gmpacket-0.1.3/gmpacket/data/examples/
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    19404 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/data/examples/borehole_example.json
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    10956 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/data/examples/example1.json
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    14499 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/data/examples/multichannel_example.json
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    32064 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/data/examples/sps-100-200-example.json
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     6059 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/feature.py
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     6268 2023-04-11 15:22:05.000000 gmpacket-0.1.3/gmpacket/packet.py
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     5155 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/provenance.py
--rwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)     9164 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/scan.py
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      123 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/utils.py
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     8719 2023-04-11 15:21:44.000000 gmpacket-0.1.3/gmpacket/validate.py
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.920894 gmpacket-0.1.3/gmpacket.egg-info/
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2083 2023-04-12 17:47:41.000000 gmpacket-0.1.3/gmpacket.egg-info/PKG-INFO
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     3030 2023-04-12 17:47:41.000000 gmpacket-0.1.3/gmpacket.egg-info/SOURCES.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)        1 2023-04-12 17:47:41.000000 gmpacket-0.1.3/gmpacket.egg-info/dependency_links.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      383 2023-04-12 17:47:41.000000 gmpacket-0.1.3/gmpacket.egg-info/requires.txt
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)        9 2023-04-12 17:47:41.000000 gmpacket-0.1.3/gmpacket.egg-info/top_level.txt
--rwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)     2604 2023-04-10 20:24:32.000000 gmpacket-0.1.3/install.sh
-drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.958476 gmpacket-0.1.3/notebooks/
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    26271 2023-04-10 20:24:32.000000 gmpacket-0.1.3/notebooks/pydantic_demo.ipynb
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1256 2023-04-12 17:28:33.000000 gmpacket-0.1.3/pyproject.toml
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)       38 2023-04-12 17:47:41.960991 gmpacket-0.1.3/setup.cfg
--rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      483 2023-04-12 17:20:26.000000 gmpacket-0.1.3/setup.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-07-27 17:02:23.531838 gmpacket-0.1.4/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      179 2023-07-27 15:27:18.000000 gmpacket-0.1.4/LICENSE.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       63 2023-07-27 15:27:18.000000 gmpacket-0.1.4/MANIFEST.in
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     2094 2023-07-27 17:02:23.531838 gmpacket-0.1.4/PKG-INFO
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1329 2023-07-27 15:27:18.000000 gmpacket-0.1.4/README.md
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-07-27 17:02:23.527838 gmpacket-0.1.4/gmpacket/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-07-27 17:01:23.000000 gmpacket-0.1.4/gmpacket/__init__.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-07-27 17:02:23.527838 gmpacket-0.1.4/gmpacket/data/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-07-27 17:02:23.531838 gmpacket-0.1.4/gmpacket/data/examples/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    19404 2023-07-27 15:27:18.000000 gmpacket-0.1.4/gmpacket/data/examples/borehole_example.json
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10956 2023-07-27 15:27:18.000000 gmpacket-0.1.4/gmpacket/data/examples/example1.json
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14499 2023-07-27 15:27:18.000000 gmpacket-0.1.4/gmpacket/data/examples/multichannel_example.json
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    32064 2023-07-27 15:27:18.000000 gmpacket-0.1.4/gmpacket/data/examples/sps-100-200-example.json
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5391 2023-07-27 15:27:18.000000 gmpacket-0.1.4/gmpacket/feature.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6110 2023-07-27 15:27:18.000000 gmpacket-0.1.4/gmpacket/packet.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4734 2023-07-27 15:27:18.000000 gmpacket-0.1.4/gmpacket/provenance.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     9164 2023-07-27 15:27:18.000000 gmpacket-0.1.4/gmpacket/scan.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      123 2023-07-27 15:27:18.000000 gmpacket-0.1.4/gmpacket/utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8719 2023-07-27 15:27:18.000000 gmpacket-0.1.4/gmpacket/validate.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-07-27 17:02:23.531838 gmpacket-0.1.4/gmpacket.egg-info/
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     2094 2023-07-27 17:02:23.000000 gmpacket-0.1.4/gmpacket.egg-info/PKG-INFO
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      533 2023-07-27 17:02:23.000000 gmpacket-0.1.4/gmpacket.egg-info/SOURCES.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2023-07-27 17:02:23.000000 gmpacket-0.1.4/gmpacket.egg-info/dependency_links.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      486 2023-07-27 17:02:23.000000 gmpacket-0.1.4/gmpacket.egg-info/requires.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        9 2023-07-27 17:02:23.000000 gmpacket-0.1.4/gmpacket.egg-info/top_level.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1556 2023-07-27 15:27:18.000000 gmpacket-0.1.4/pyproject.toml
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2023-07-27 17:02:23.531838 gmpacket-0.1.4/setup.cfg
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       64 2023-07-27 15:27:18.000000 gmpacket-0.1.4/setup.py
```

### Comparing `gmpacket-0.1.3/PKG-INFO` & `gmpacket-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: gmpacket
-Version: 0.1.3
+Version: 0.1.4
 Summary: ANSS Ground Motion Packet
-Home-page: https://github.com/SCEDC/ground-motion-packet
-Author: Ellen Yu, Lijam Hagos, Jamie Steidl, Eric Thompson, Bruce Worden
-Author-email: Mike Hearne <mhearne@usgs.gov>, Eric Thompson <ethompson@usgs.gov>, Ellen Yu <eyu@caltech.edu>
+Author-email: Mike Hearne <mhearne@usgs.gov>, Eric Thompson <ethompson@usgs.gov>, Ellen Yu <eyu@caltech.edu>, Lijam Hagos <lijam.hagos@conservation.ca.gov>, Jamie Steidl <steidl@ucsb.edu>, Bruce Worden <cbworden@contractor.usgs.gov>
 License: License
         =======
         
         This is free and unencumbered software released into the public domain. It is 
         distributed under the terms of the Unlicense described here:
         http://unlicense.org/
         
@@ -34,11 +32,11 @@
 format should be able to be used by any application that uses ground motion 
 metrics including, but not limited to, ShakeMap. The GMP format is not meant to 
 describe station metadata or site installation. The purpose of the metadata 
 included in the GMP format is to provide high-level information regarding the 
 suitability of the data for common engineering/seismological applications.
 
 ## Documentation
-[User Documentation](https://scedc.github.io/ground-motion-packet/index.html)
+[User Documentation](https://ghsc.code-pages.usgs.gov/esi/ground-motion-packet/)
 
 ## Demo
-[Sample Jupyter notebook](https://github.com/SCEDC/ground-motion-packet/blob/main/gmpacket/GMP-demo.ipynb)
+[Sample Jupyter notebook](https://code.usgs.gov/ghsc/esi/ground-motion-packet/-/blob/main/notebooks/pydantic_demo.ipynb)
```

### Comparing `gmpacket-0.1.3/README.md` & `gmpacket-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 format should be able to be used by any application that uses ground motion 
 metrics including, but not limited to, ShakeMap. The GMP format is not meant to 
 describe station metadata or site installation. The purpose of the metadata 
 included in the GMP format is to provide high-level information regarding the 
 suitability of the data for common engineering/seismological applications.
 
 ## Documentation
-[User Documentation](https://scedc.github.io/ground-motion-packet/index.html)
+[User Documentation](https://ghsc.code-pages.usgs.gov/esi/ground-motion-packet/)
 
 ## Demo
-[Sample Jupyter notebook](https://github.com/SCEDC/ground-motion-packet/blob/main/gmpacket/GMP-demo.ipynb)
+[Sample Jupyter notebook](https://code.usgs.gov/ghsc/esi/ground-motion-packet/-/blob/main/notebooks/pydantic_demo.ipynb)
```

### Comparing `gmpacket-0.1.3/gmpacket/data/examples/borehole_example.json` & `gmpacket-0.1.4/gmpacket/data/examples/borehole_example.json`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.3/gmpacket/data/examples/example1.json` & `gmpacket-0.1.4/gmpacket/data/examples/example1.json`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.3/gmpacket/data/examples/multichannel_example.json` & `gmpacket-0.1.4/gmpacket/data/examples/multichannel_example.json`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.3/gmpacket/data/examples/sps-100-200-example.json` & `gmpacket-0.1.4/gmpacket/data/examples/sps-100-200-example.json`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.3/gmpacket/feature.py` & `gmpacket-0.1.4/gmpacket/feature.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # stdlib imports
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Union
 
 # third party imports
 import numpy as np
-from pydantic import BaseModel, root_validator
+from pydantic import BaseModel, ConfigDict, model_validator
 
 # local imports
 from gmpacket.utils import datetime_to_iso8601
 
 
 class CosmosCode(Enum):
     FIBERGLASS_SHELTER = (1, "Small fiberglass shelter")
@@ -61,47 +61,41 @@
 
 class MetricProperties(BaseModel):
     """Represent a ground motion packet MetricProperties object."""
 
     description: str
     name: str
     units: str
-    provenance_ids: Optional[List[str]]
-    time_of_peak: Optional[datetime]
+    provenance_ids: Optional[List[str]] = None
+    time_of_peak: Optional[datetime] = None
 
 
 class MetricDimensions(BaseModel):
     """Represent a ground motion packet MetricDimensions object."""
 
     number: int
     names: List[str]
     units: List[str]
     axis_values: List[List[float]]
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     def check_dimensions(cls, values):
         ndims = values["number"]
         assert len(values["names"]) == ndims
         return values
 
 
 class Metric(BaseModel):
     """Represent a ground motion packet Metric object."""
 
     properties: MetricProperties
-    dimensions: Optional[MetricDimensions]  # required when metric is an array
+    dimensions: Optional[MetricDimensions] = None  # required when metric is an array
     values: Union[List[List[float]], List[float], float]
 
-    class Config:
-        json_encoders = {
-            # custom output conversion for datetime
-            datetime: datetime_to_iso8601
-        }
-
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     def check_dimensions(cls, values):
         if "dimensions" in values and values["dimensions"] is not None:
             if "number" in values["dimensions"]:
                 ndims = values["dimensions"]["number"]
             else:
                 ndims = values["dimensions"].number
             assert ndims == np.array(values["values"]).ndim
@@ -115,41 +109,29 @@
     location_code: str
     as_recorded: bool
     azimuth: float
     dip: float
     start_time: datetime
     end_time: datetime
 
-    class Config:
-        json_encoders = {
-            # custom output conversion for datetime
-            datetime: datetime_to_iso8601
-        }
-
 
 class Trace(BaseModel):
     """Represent a ground motion packet Trace object."""
 
     properties: TraceProperties
     metrics: List[Metric]
 
-    class Config:
-        json_encoders = {
-            # custom output conversion for datetime
-            datetime: datetime_to_iso8601
-        }
-
 
 class StreamHousing(BaseModel):
     """Represent a ground motion packet StreamHousing object."""
 
     cosmos_code: int
     description: str
     stream_depth: float
-    stream_location: Optional[str]
+    stream_location: Optional[str] = None
 
     @classmethod
     def from_enum(cls, code: CosmosCode, depth: float, location: str = ""):
         cosmos_code, description = CosmosCode(code).value
         return cls(
             cosmos_code=cosmos_code,
             description=description,
@@ -179,43 +161,31 @@
 
 class Stream(BaseModel):
     """Represent a ground motion packet Stream object."""
 
     properties: StreamProperties
     traces: List[Trace]
 
-    class Config:
-        json_encoders = {
-            # custom output conversion for datetime
-            datetime: datetime_to_iso8601
-        }
-
 
 class FeatureGeometry(BaseModel):
     """Represent a ground motion packet FeatureGeometry object."""
 
-    type = "Point"
+    type: str = "Point"
     coordinates: List[float]
 
 
 class FeatureProperties(BaseModel):
     """Represent a ground motion packet FeatureProperties object."""
 
     network_code: str
     station_code: str
-    name: Optional[str]
+    name: Optional[str] = None
     streams: List[Stream]
-    structure_reference_orientation: Optional[int]
+    structure_reference_orientation: Optional[int] = None
 
 
 class Feature(BaseModel):
     """Represent a ground motion packet Feature object."""
 
-    type = "Feature"
+    type: str = "Feature"
     geometry: FeatureGeometry
     properties: FeatureProperties
-
-    class Config:
-        json_encoders = {
-            # custom output conversion for datetime
-            datetime: datetime_to_iso8601
-        }
```

### Comparing `gmpacket-0.1.3/gmpacket/packet.py` & `gmpacket-0.1.4/gmpacket/packet.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datetime import datetime
 from typing import List, Optional
 
 # third party imports
 import numpy as np
 import pandas as pd
 from geopy import distance
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 
 # local imports
 from gmpacket.feature import Feature
 from gmpacket.provenance import Provenance
 from gmpacket.utils import datetime_to_iso8601
 
 
@@ -35,37 +35,28 @@
 
     @classmethod
     def from_params(cls, id, time, magnitude, lat, lon, depth):
         props = {"id": id, "time": time, "magnitude": magnitude}
         geometry = {"type": "Point", "coordinates": [lon, lat, depth * 1000]}
         return cls(properties=props, geometry=geometry)
 
-    class Config:
-        json_encoders = {
-            # custom output conversion for datetime
-            datetime: datetime_to_iso8601
-        }
+    # model_config: ConfigDict = ConfigDict(json_encoders={datetime: datetime_to_iso8601})
 
 
 class GroundMotionPacket(BaseModel):
     """Represent a high level ground motion packet object."""
 
-    type = "FeatureCollection"
+    type: str = "FeatureCollection"
     version: str
     creation_time: datetime = datetime.utcnow()
     event: Optional[Event]
     provenance: Provenance
     features: List[Feature]
 
-    class Config:
-        anystr_strip_whitespace = True
-        json_encoders = {
-            # custom output conversion for datetime
-            datetime: datetime_to_iso8601
-        }
+    model_config: ConfigDict = ConfigDict(str_strip_whitespace=True)
 
     @classmethod
     def load_from_json(cls, filename):
         with open(filename, "rt") as f:
             data = json.load(f)
         return cls(**data)
```

### Comparing `gmpacket-0.1.3/gmpacket/provenance.py` & `gmpacket-0.1.4/gmpacket/provenance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,106 +1,94 @@
 from typing import Dict
 
-from pydantic import BaseModel, EmailStr, Field, validator
+from pydantic import BaseModel, ConfigDict, EmailStr, Field, field_validator
 
 
 class Website(BaseModel):
     """Represent a ground motion packet Website object."""
 
     url: str = Field(alias="$")
     site_type: str = Field(alias="type", default="xsd:anyURI")
 
-    class Config:
-        # ensure that we can populate by the Python variable names, instead of
-        # names like "$"
-        allow_population_by_field_name = True
+    model_config: ConfigDict = ConfigDict(populate_by_name=True)
 
 
 class OrganizationAgent(BaseModel):
     """Represent a ground motion packet OrganizationAgent object."""
 
     label: str = Field(alias="prov:label", default=None)
-    prov_type: Dict = Field(
+    type: Dict = Field(
         alias="prov:type",
         default={"$": "prov:Organization", "type": "prov:QUALIFIED_NAME"},
     )
     name: str = Field(alias="seis_prov:name")
     role: str = Field(alias="seis_prov:role")
     website: Website = Field(alias="seis_prov:website")
 
-    class Config:
-        allow_population_by_field_name = True
+    model_config: ConfigDict = ConfigDict(populate_by_name=True)
 
     @classmethod
     def from_params(cls, name: str, role: str, website: Website, label: str = None):
         if label is None:
             label = name
         thisobj = cls(label=label, name=name, role=role, website=website)
-        thisobj.__dict__["prov:type"] = thisobj.__dict__["prov_type"]
-        thisobj.__dict__.pop("prov_type")
         return thisobj
 
 
 class SoftwareAgent(BaseModel):
     """Represent a ground motion packet SoftwareAgent object."""
 
     label: str = Field(alias="prov:label", default=None)
-    prov_type: Dict = Field(
+    type: Dict = Field(
         alias="prov:type",
         default={"$": "prov:SoftwareAgent", "type": "prov:QUALIFIED_NAME"},
     )
     name: str = Field(alias="seis_prov:software_name")
     version: str = Field(alias="seis_prov:software_version")
     website: Website = Field(alias="seis_prov:website")
 
-    class Config:
-        allow_population_by_field_name = True
+    model_config: ConfigDict = ConfigDict(populate_by_name=True)
 
     @classmethod
     def from_params(cls, name: str, version: str, website: Website, label: str = None):
         if label is None:
             label = name
         thisobj = cls(label=label, name=name, version=version, website=website)
-        thisobj.__dict__["prov:type"] = thisobj.__dict__["prov_type"]
-        thisobj.__dict__.pop("prov_type")
         return thisobj
 
 
 class PersonAgent(BaseModel):
     """Represent a ground motion packet PersonAgent object."""
 
     label: str = Field(alias="prov:label")
-    prov_type: Dict = Field(
+    type: Dict = Field(
         alias="prov:type", default={"$": "prov:Person", "type": "prov:QUALIFIED_NAME"}
     )
     name: str = Field(alias="seis_prov:name")
     email: EmailStr = Field(alias="seis_prov:email")
     role: str = Field(alias="seis_prov:role")
 
-    class Config:
-        allow_population_by_field_name = True
+    model_config: ConfigDict = ConfigDict(populate_by_name=True)
 
     @classmethod
     def from_params(cls, name: str, email: str, role: str, label: str = None):
         if label is None:
             label = name
         thisobj = cls(label=label, name=name, email=email, role=role)
-        thisobj.__dict__["prov:type"] = thisobj.__dict__["prov_type"]
-        thisobj.__dict__.pop("prov_type")
         return thisobj
 
 
 class Provenance(BaseModel):
     """Represent a ground motion packet Provenance object."""
 
-    prefix = {"seis_prov": "http://seisprov.org/seis_prov/0.1/#"}
+    prefix: dict = {"seis_prov": "http://seisprov.org/seis_prov/0.1/#"}
     # agent: Optional[Dict[str, Agent]]
     agent: dict
 
-    @validator("agent")
+    @field_validator("agent")
     def get_agent_dict(cls, input):
         """Check elements of input dictionary to make sure they are all *Agent types"""
         if not isinstance(input, dict):
             raise ValueError("agent attribute of Provenance must be a dictionary.")
         agents = {}
         agent_types = (OrganizationAgent, SoftwareAgent, PersonAgent)
         for key, value in input.items():
```

### Comparing `gmpacket-0.1.3/gmpacket/scan.py` & `gmpacket-0.1.4/gmpacket/scan.py`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.3/gmpacket/validate.py` & `gmpacket-0.1.4/gmpacket/validate.py`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.3/gmpacket.egg-info/PKG-INFO` & `gmpacket-0.1.4/gmpacket.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: gmpacket
-Version: 0.1.3
+Version: 0.1.4
 Summary: ANSS Ground Motion Packet
-Home-page: https://github.com/SCEDC/ground-motion-packet
-Author: Ellen Yu, Lijam Hagos, Jamie Steidl, Eric Thompson, Bruce Worden
-Author-email: Mike Hearne <mhearne@usgs.gov>, Eric Thompson <ethompson@usgs.gov>, Ellen Yu <eyu@caltech.edu>
+Author-email: Mike Hearne <mhearne@usgs.gov>, Eric Thompson <ethompson@usgs.gov>, Ellen Yu <eyu@caltech.edu>, Lijam Hagos <lijam.hagos@conservation.ca.gov>, Jamie Steidl <steidl@ucsb.edu>, Bruce Worden <cbworden@contractor.usgs.gov>
 License: License
         =======
         
         This is free and unencumbered software released into the public domain. It is 
         distributed under the terms of the Unlicense described here:
         http://unlicense.org/
         
@@ -34,11 +32,11 @@
 format should be able to be used by any application that uses ground motion 
 metrics including, but not limited to, ShakeMap. The GMP format is not meant to 
 describe station metadata or site installation. The purpose of the metadata 
 included in the GMP format is to provide high-level information regarding the 
 suitability of the data for common engineering/seismological applications.
 
 ## Documentation
-[User Documentation](https://scedc.github.io/ground-motion-packet/index.html)
+[User Documentation](https://ghsc.code-pages.usgs.gov/esi/ground-motion-packet/)
 
 ## Demo
-[Sample Jupyter notebook](https://github.com/SCEDC/ground-motion-packet/blob/main/gmpacket/GMP-demo.ipynb)
+[Sample Jupyter notebook](https://code.usgs.gov/ghsc/esi/ground-motion-packet/-/blob/main/notebooks/pydantic_demo.ipynb)
```

### Comparing `gmpacket-0.1.3/pyproject.toml` & `gmpacket-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 name = "gmpacket"
 dynamic = ["version"]
 description = "ANSS Ground Motion Packet"
 authors = [
     {name = "Mike Hearne", email="mhearne@usgs.gov"},
     {name = "Eric Thompson", email="ethompson@usgs.gov"},
     {name = "Ellen Yu", email="eyu@caltech.edu"},
+    {name = "Lijam Hagos", email="lijam.hagos@conservation.ca.gov"},
+    {name = "Jamie Steidl", email="steidl@ucsb.edu"},
+    {name = "Bruce Worden", email="cbworden@contractor.usgs.gov"},
 ]
 
 license = {file = "LICENSE.md"}
 readme = "README.md"
 requires-python = "<=3.11"
 
 keywords = ["ground motion", "earthquake"]
 
 
 dependencies = [
     "geopy>=2.1.0",
     "pandas>=1.4.0",
-    "pydantic[email]>=1.10.0",
+    "pydantic[email]>=2.0",
+    "setuptools-scm>=6.3.2",
 ]
 
 [tool.setuptools]
 packages = ["gmpacket"]
 
 
 
@@ -38,26 +42,26 @@
     "deepdiff>=5.7.0",
     "openpyxl>=3.0.9",
     "pytest>=6.2",
     "pytest-cov>=2.12.0",
 
 ]
 doc = [
-    "sphinx>3.0.0",
-    "requests>=2",
-    "furo",
-    "myst-nb",
-    "myst-parser",
-    "altair",
-    "nbsphinx",
-    "recommonmark",
-    "sphinx-autoapi",
-    "sphinx-copybutton",
-    "sphinx-inline-tabs",
-    "sphinxcontrib-programoutput"
+    "sphinx>5.0.0",
+    "requests>=2.28.2",
+    "furo>=2023.3.27",
+    "myst-nb>=0.17.2",
+    "myst-parser>=0.18.1",
+    "altair>=4.2.2",
+    "nbsphinx>=0.9.1",
+    "recommonmark>=0.7.1",
+    "sphinx-autoapi>=2.1.0",
+    "sphinx-copybutton>=0.5.2",
+    "sphinx-inline-tabs>=2023.4.21",
+    "sphinxcontrib-programoutput>=0.17"
 ]
 build = [
     "build",
     "twine",
 ]
 
 [build-system]
```

