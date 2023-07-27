# Comparing `tmp/ixbrl-viewer-1.2.2.tar.gz` & `tmp/ixbrl-viewer-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixbrl-viewer-1.2.2.tar", last modified: Thu Jul 27 15:24:31 2023, max compression
+gzip compressed data, was "ixbrl-viewer-1.3.0.tar", last modified: Thu Jul 27 19:45:32 2023, max compression
```

## Comparing `ixbrl-viewer-1.2.2.tar` & `ixbrl-viewer-1.3.0.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.154666 ixbrl-viewer-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.babelrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.114666 ixbrl-viewer-1.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.114666 ixbrl-viewer-1.2.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/ISSUE_TEMPLATE/questions.yml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/ISSUE_TEMPLATE/request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.118666 ixbrl-viewer-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/workflows/node-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/workflows/npm-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/workflows/puppeteer.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/workflows/python-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/COPYRIGHT.md
--rw-r--r--   0 runner    (1001) docker     (123)    16664 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-07-27 15:24:31.154666 ixbrl-viewer-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/PLUGINS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.118666 ixbrl-viewer-1.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.126666 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/
--rw-r--r--   0 runner    (1001) docker     (123)    92632 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   149033 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml
--rw-r--r--   0 runner    (1001) docker     (123)  2413470 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm
--rw-r--r--   0 runner    (1001) docker     (123)   535018 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml
--rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1219995 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml
--rw-r--r--   0 runner    (1001) docker     (123)   858776 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml
--rw-r--r--   0 runner    (1001) docker     (123)    60067 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm
--rw-r--r--   0 runner    (1001) docker     (123)    68052 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm
--rw-r--r--   0 runner    (1001) docker     (123)  4343804 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.130666 ixbrl-viewer-1.2.2/examples/example_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/example_plugin/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   194458 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/example_plugin/example-plugin.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/example_plugin/extended-viewer.js
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/example_plugin/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    95465 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/example_plugin/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/example_plugin/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/example_plugin/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (123)   917698 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/ixbrl-viewer-demo.gif
--rw-r--r--   0 runner    (1001) docker     (123)    17954 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/review-mode.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.134666 ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/
--rw-r--r--   0 runner    (1001) docker     (123)   222306 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm
--rw-r--r--   0 runner    (1001) docker     (123)   223016 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm
--rw-r--r--   0 runner    (1001) docker     (123)    56173 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    24833 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml
--rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.134666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 15:24:30.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25725 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/iXBRLViewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/stubviewer.html
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.134666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.138666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/dist/
--rw-r--r--   0 runner    (1001) docker     (123)  1897286 2023-07-27 15:24:14.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-27 15:24:14.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/i18next-parser.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.110666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.138666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/cog.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/font-reduce.pe
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/print.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/viewer-icons-min.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.138666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/html/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/html/fact-details.html
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/html/footnote-details.html
--rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/html/inspector.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.110666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.138666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/en/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/en/currencies.json
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/en/referenceparts.json
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.138666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/es/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/es/currencies.json
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/es/referenceparts.json
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.138666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/arelle.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.146666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/accordian.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/aspect.js
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/aspect.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/calculations.js
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/chart.js
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/chart.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/concept.js
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/concept.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/dialog.js
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/fact.js
--rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/fact.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/factset.js
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/factset.test.js
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/footnote.js
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/identifiers.js
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    44060 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/inspector.js
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/inspector.test.js
--rw-r--r--   0 runner    (1001) docker     (123)    85048 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/interact.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/ixnode.js
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/menu.js
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/messagebox.js
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/moment-jest.js
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/number-matcher.js
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/outline.js
--rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/outline.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/period.js
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/period.test.js
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/qname.js
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/report.js
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/report.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/search.js
--rw-r--r--   0 runner    (1001) docker     (123)    21034 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/search.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/summary.js
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/summary.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/tableExport.js
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/test-utils.js
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/unit.js
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/unit.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/util.js
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/util.test.js
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/validationreport.js
--rw-r--r--   0 runner    (1001) docker     (123)    34470 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/viewer.js
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/viewerOptions.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.146666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/accordian.less
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/block-list.less
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/chart.less
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/clearfix.less
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/colours.less
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/common.less
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/components.less
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/core.less
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/dialog.less
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/fonts.less
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/form-controls.less
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/icons.less
--rw-r--r--   0 runner    (1001) docker     (123)    20550 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/inspector.less
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/loader.less
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/menu.less
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/summary.less
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/tabs.less
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/text-block-viewer.less
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/text-mixins.less
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/validation-report.less
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/viewer.less
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/version.js
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/webpack.common.js
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/webpack.dev.js
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/webpack.prod.js
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/xhtmlserialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-07-27 15:24:31.000000 ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-07-27 15:24:31.000000 ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:24:31.000000 ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 15:24:31.000000 ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 15:24:31.000000 ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 15:24:31.000000 ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)   504607 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/samples/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/Makefile-src
--rwxr-xr-x   0 runner    (1001) docker     (123)     4370 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/build-viewer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/fetch-sample-files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/sample-files.list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.114666 ixbrl-viewer-1.2.2/samples/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/samples/src/continuation/
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/src/continuation/continuation.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/samples/src/ixds-test/
--rw-r--r--   0 runner    (1001) docker     (123)    26111 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/src/ixds-test/document1.html
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/src/ixds-test/faurecia.html
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/src/ixds-test/valeo.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/samples/src/scrollable-div/
--rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/src/scrollable-div/scrollable-div.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/samples/src/xbrl-invalid-tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 15:24:31.154666 ixbrl-viewer-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/puppeteer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/puppeteer/framework/
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/framework/core_elements.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/doc_frame.js
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/fact_details_panel.js
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/search_panel.js
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/toolbar.js
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/framework/utils.js
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/framework/viewer_page.js
--rw-r--r--   0 runner    (1001) docker     (123)    61701 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/puppeteer_test_run_via_intellij.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/puppeteer/test_filings/
--rw-r--r--   0 runner    (1001) docker     (123)    21469 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/test_filings/filing_documents_smoke_test.zip
--rw-r--r--   0 runner    (1001) docker     (123)    18766 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/test_filings/highlights.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/puppeteer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/tests/fact_properties.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/tests/highlight.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/tests/search.test.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/puppeteer/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/tools/generate.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.154666 ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py
--rw-r--r--   0 runner    (1001) docker     (123)    26993 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.babelrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.204800 ixbrl-viewer-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.204800 ixbrl-viewer-1.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/ISSUE_TEMPLATE/questions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/ISSUE_TEMPLATE/request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.208800 ixbrl-viewer-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/workflows/node-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/workflows/npm-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/workflows/puppeteer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/workflows/python-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/COPYRIGHT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/PLUGINS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.208800 ixbrl-viewer-1.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.216801 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)    92632 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   149033 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  2413470 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm
+-rw-r--r--   0 runner    (1001) docker     (123)   535018 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1219995 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   858776 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    60067 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm
+-rw-r--r--   0 runner    (1001) docker     (123)    68052 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm
+-rw-r--r--   0 runner    (1001) docker     (123)  4343804 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.224801 ixbrl-viewer-1.3.0/examples/example_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/example_plugin/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   194458 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/example_plugin/example-plugin.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/example_plugin/extended-viewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/example_plugin/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95465 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/example_plugin/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/example_plugin/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/example_plugin/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)   917698 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/ixbrl-viewer-demo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    17954 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/review-mode.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.224801 ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)   222306 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm
+-rw-r--r--   0 runner    (1001) docker     (123)   223016 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm
+-rw-r--r--   0 runner    (1001) docker     (123)    56173 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    24833 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.228801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 19:45:31.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25873 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/iXBRLViewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/stubviewer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.228801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.228801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)   859288 2023-07-27 19:45:12.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-27 19:45:12.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/i18next-parser.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.200800 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.228801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/cog.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/font-reduce.pe
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/print.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/viewer-icons-min.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.228801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/html/fact-details.html
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/html/footnote-details.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/html/inspector.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.200800 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.228801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/en/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/en/currencies.json
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/en/referenceparts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.228801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/es/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/es/currencies.json
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/es/referenceparts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.232801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/arelle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.236801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/accordian.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/aspect.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/aspect.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/calculations.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/chart.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/concept.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/concept.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/dialog.js
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/fact.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/fact.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/factset.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/factset.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/footnote.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/identifiers.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44285 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/inspector.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/inspector.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)    85048 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/interact.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/ixnode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/menu.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/messagebox.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/moment-jest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/number-matcher.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/outline.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/outline.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/period.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/period.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/qname.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/report.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/report.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21034 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/search.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/summary.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/summary.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/tableExport.js
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/test-utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/unit.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/unit.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/util.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/util.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/validationreport.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34470 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/viewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/viewerOptions.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.240801 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/accordian.less
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/block-list.less
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/chart.less
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/clearfix.less
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/colours.less
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/common.less
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/components.less
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/core.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/dialog.less
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/fonts.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/form-controls.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/icons.less
+-rw-r--r--   0 runner    (1001) docker     (123)    20550 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/inspector.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/loader.less
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/menu.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/summary.less
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/tabs.less
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/text-block-viewer.less
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/text-mixins.less
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/validation-report.less
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/viewer.less
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/version.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/webpack.common.js
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/webpack.dev.js
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/webpack.prod.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/iXBRLViewerPlugin/xhtmlserialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.240801 ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-07-27 19:45:32.000000 ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-07-27 19:45:32.000000 ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:45:32.000000 ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 19:45:32.000000 ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 19:45:32.000000 ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 19:45:32.000000 ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   492586 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.240801 ixbrl-viewer-1.3.0/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/Makefile-src
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4370 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/build-viewer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/fetch-sample-files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/sample-files.list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.200800 ixbrl-viewer-1.3.0/samples/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.240801 ixbrl-viewer-1.3.0/samples/src/continuation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/src/continuation/continuation.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/samples/src/ixds-test/
+-rw-r--r--   0 runner    (1001) docker     (123)    26111 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/src/ixds-test/document1.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/src/ixds-test/faurecia.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/src/ixds-test/valeo.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/samples/src/scrollable-div/
+-rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/src/scrollable-div/scrollable-div.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/samples/src/xbrl-invalid-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/puppeteer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/puppeteer/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/framework/core_elements.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/doc_frame.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/fact_details_panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/search_panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/toolbar.js
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/framework/utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/framework/viewer_page.js
+-rw-r--r--   0 runner    (1001) docker     (123)    61701 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/puppeteer_test_run_via_intellij.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/puppeteer/test_filings/
+-rw-r--r--   0 runner    (1001) docker     (123)    21469 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/test_filings/filing_documents_smoke_test.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    18766 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/test_filings/highlights.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/puppeteer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/tests/fact_properties.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/tests/highlight.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/tests/search.test.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/puppeteer/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/puppeteer/tools/generate.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:45:32.244801 ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26993 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-07-27 19:44:29.000000 ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py
```

### Comparing `ixbrl-viewer-1.2.2/.github/ISSUE_TEMPLATE/bug.yml` & `ixbrl-viewer-1.3.0/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/.github/dependabot.yml` & `ixbrl-viewer-1.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/.github/workflows/node-tests.yml` & `ixbrl-viewer-1.3.0/.github/workflows/node-tests.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/.github/workflows/npm-package.yml` & `ixbrl-viewer-1.3.0/.github/workflows/npm-package.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/.github/workflows/puppeteer.yml` & `ixbrl-viewer-1.3.0/.github/workflows/puppeteer.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/.github/workflows/python-package.yml` & `ixbrl-viewer-1.3.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/.github/workflows/python-tests.yml` & `ixbrl-viewer-1.3.0/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/LICENSE` & `ixbrl-viewer-1.3.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -213,67 +213,14 @@
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION 
 WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 
 
-exceljs
-
-
-Copyright (c) 2014-2017 Guyon Roche
-
-
-Permission is hereby granted, free of charge, to any person obtaining a copy 
-of this software and associated documentation files (the "Software"), to deal 
-in the Software without restriction, including without limitation the rights 
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell 
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-The above copyright notice and this permission notice shall be included in all 
-copies or substantial portions of the Software.
-
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-
-
-
-
-file-saver
-Copyright © 2016 [Eli Grey][1].
-
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
-and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
-THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-  
-[1]: http://eligrey.com
-
-
-
-
 interactjs
 
 Copyright (c) 2012-2017 Taye Adeyemi <dev@taye.me>
 
 
 Permission is hereby granted, free of charge, to any person 
 obtaining a copy of this software and associated 
@@ -432,8 +379,34 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF 
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. 
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY 
 CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+
+
+
+write-excel-file
+
+Copyright (c) 2018 gitlab.com/catamphetamine
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
 ---
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ixbrl-viewer-1.2.2/Makefile` & `ixbrl-viewer-1.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/NOTICE` & `ixbrl-viewer-1.3.0/NOTICE`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/PKG-INFO` & `ixbrl-viewer-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixbrl-viewer
-Version: 1.2.2
+Version: 1.3.0
 Summary: The Arelle iXBRL Viewer allows iXBRL reports to be viewed interactively in a web browser.
 Author-email: "arelle.org" <support@arelle.org>
 License: Apache-2.0
 Project-URL: Homepage, https://arelle.org/
 Project-URL: Downloads, https://arelle.org/arelle/pub/
 Project-URL: Documentation, https://arelle.org/arelle/documentation/
 Project-URL: Blog, https://arelle.org/arelle/blog/
```

### Comparing `ixbrl-viewer-1.2.2/PLUGINS.md` & `ixbrl-viewer-1.3.0/PLUGINS.md`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/README.md` & `ixbrl-viewer-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/README.md` & `ixbrl-viewer-1.3.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd` & `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml` & `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm` & `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml` & `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg` & `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml` & `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml` & `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm` & `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm` & `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm` & `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm` & `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm` & `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm` & `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm` & `ixbrl-viewer-1.3.0/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/example_plugin/README.md` & `ixbrl-viewer-1.3.0/examples/example_plugin/README.md`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/example_plugin/example-plugin.gif` & `ixbrl-viewer-1.3.0/examples/example_plugin/example-plugin.gif`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/example_plugin/extended-viewer.js` & `ixbrl-viewer-1.3.0/examples/example_plugin/extended-viewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/example_plugin/package-lock.json` & `ixbrl-viewer-1.3.0/examples/example_plugin/package-lock.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/example_plugin/webpack.config.js` & `ixbrl-viewer-1.3.0/examples/example_plugin/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/ixbrl-viewer-demo.gif` & `ixbrl-viewer-1.3.0/examples/ixbrl-viewer-demo.gif`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/review-mode.png` & `ixbrl-viewer-1.3.0/examples/review-mode.png`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm` & `ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm` & `ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm` & `ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd` & `ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml` & `ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml` & `ixbrl-viewer-1.3.0/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/__init__.py` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,18 @@
                       dest="useStubViewer",
                       help="Use stub viewer for faster loading of inspector (requires web server)")
     parser.add_option("--viewer-suffix",
                       action="store",
                       default="",
                       dest="viewerBasenameSuffix",
                       help="Suffix for basename of viewer files")
+    parser.add_option("--package-download-url",
+                      action="store",
+                      dest="packageDownloadURL",
+                      help="URL where the original report package can be downloaded.  This will be available to the user as a download link in the viewer.")
     parser.add_option("--zip-viewer-output",
                       action="store_true",
                       default=False,
                       dest="zipViewerOutput",
                       help="Converts the viewer output into a self contained zip")
     featureGroup = OptionGroup(parser, "Viewer Features",
                             "See viewer README for information on enabling/disabling features.")
@@ -86,15 +90,16 @@
 def generateViewer(
         cntlr: Cntlr,
         saveViewerDest: Union[io.BytesIO, str],
         viewerURL: str = DEFAULT_VIEWER_PATH,
         showValidationMessages: bool = False,
         useStubViewer: bool = False,
         zipViewerOutput: bool = False,
-        features: Optional[list[str]] = None):
+        features: Optional[list[str]] = None,
+        packageDownloadURL: str = None):
     """
     Generate and save a viewer at the given destination (file, directory, or in-memory file) with the given viewer URL.
     If the viewer URL is a location on the local file system, a copy will be placed included in the output destination.
     :param cntlr: The arelle controller that contains the model to be included in the viewer
     :param saveViewerDest: The target that viewer data/files will be written to (path to file or directory, or a file object itself).
     :param viewerURL: The filepath or URL location of the viewer script.
     :param showValidationMessages: True if validation messages should be shown in the viewer.
@@ -130,15 +135,15 @@
     try:
         out = saveViewerDest
         if out:
             viewerBuilder = IXBRLViewerBuilder(modelXbrl)
             if features:
                 for feature in features:
                     viewerBuilder.enableFeature(feature)
-            iv = viewerBuilder.createViewer(scriptUrl=viewerURL, showValidations=showValidationMessages, useStubViewer=useStubViewer)
+            iv = viewerBuilder.createViewer(scriptUrl=viewerURL, showValidations=showValidationMessages, useStubViewer=useStubViewer, packageDownloadURL=packageDownloadURL)
             if iv is not None:
                 iv.save(out, zipOutput=zipViewerOutput, copyScriptPath=copyScriptPath)
     except IXBRLViewerBuilderError as ex:
         print(ex.message)
     except Exception as ex:
         cntlr.addToLog("Exception {} \nTraceback {}".format(ex, traceback.format_tb(sys.exc_info()[2])))
 
@@ -168,15 +173,16 @@
     generateViewer(
         cntlr,
         options.saveViewerDest or kwargs.get("responseZipStream"),
         options.viewerURL,
         options.validationMessages,
         options.useStubViewer,
         options.zipViewerOutput,
-        getFeaturesFromOptions(options)
+        getFeaturesFromOptions(options),
+        options.packageDownloadURL,
     )
 
 
 def iXBRLViewerMenuCommand(cntlr):
     from .ui import SaveViewerDialog
     if cntlr.modelManager is None or cntlr.modelManager.modelXbrl is None:
         cntlr.addToLog("No document loaded.")
```

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/iXBRLViewer.py` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/iXBRLViewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,15 @@
                 return True
         return False
 
     def getStubDocument(self):
         with open(os.path.join(os.path.dirname(__file__),"stubviewer.html")) as fin:
             return etree.parse(fin)
 
-    def createViewer(self, scriptUrl: str = DEFAULT_VIEWER_PATH, useStubViewer: bool = False, showValidations: bool = True) -> Optional[iXBRLViewer]:
+    def createViewer(self, scriptUrl: str = DEFAULT_VIEWER_PATH, useStubViewer: bool = False, showValidations: bool = True, packageDownloadURL: str = None) -> Optional[iXBRLViewer]:
         """
         Create an iXBRL file with XBRL data as a JSON blob, and script tags added.
         :param scriptUrl: The `src` value of the script tag that loads the viewer script.
         :param useStubViewer: True if stub document should be included in output.
         :param showValidations: True if validation errors should be included in output taxonomy data.
         :return: An iXBRLViewer instance that is ready to be saved.
         """
@@ -433,15 +433,18 @@
             docSetFiles = [ filename ]
             iv.addFile(iXBRLViewerFile("ixbrlviewer.html", xmlDocument))
             iv.addFile(iXBRLViewerFile(filename, dts.modelDocument.xmlDocument))
 
         else:
             xmlDocument = deepcopy(dts.modelDocument.xmlDocument)
             iv.addFile(iXBRLViewerFile('xbrlviewer.html', xmlDocument))
-        if os.path.dirname(self.dts.modelDocument.filepath).endswith('.zip'):
+
+        if packageDownloadURL is not None:
+            self.taxonomyData["filingDocuments"] = packageDownloadURL
+        elif os.path.dirname(self.dts.modelDocument.filepath).endswith('.zip'):
             filingDocZipPath = os.path.dirname(self.dts.modelDocument.filepath)
             filingDocZipName = os.path.basename(filingDocZipPath)
             iv.addFilingDoc(filingDocZipPath)
             self.taxonomyData["filingDocuments"] = filingDocZipName
 
         localDocs = defaultdict(set)
         for path, doc in dts.urlDocs.items():
```

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/ui.py` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/ui.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 /*!
+
+JSZip v3.10.1 - A JavaScript class for generating and reading zip files
+<http://stuartk.com/jszip>
+
+(c) 2009-2016 Stuart Knightley <stuart [at] stuartk.com>
+Dual licenced under the MIT license or GPLv3. See https://raw.github.com/Stuk/jszip/main/LICENSE.markdown.
+
+JSZip uses the library pako released under the MIT license :
+https://github.com/nodeca/pako/blob/main/LICENSE
+*/
+
+/*!
  * Chart.js v2.9.4
  * https://www.chartjs.org
  * (c) 2020 Chart.js Contributors
  * Released under the MIT License
  */
 
 /*!
- * Determine if an object is a Buffer
- *
- * @author   Feross Aboukhadijeh <https://feross.org>
- * @license  MIT
- */
-
-/*!
- * The buffer module from node.js, for the browser.
- *
- * @author   Feross Aboukhadijeh <https://feross.org>
- * @license  MIT
- */
-
-/*!
  * jQuery JavaScript Library v3.7.0
  * https://jquery.com/
  *
  * Copyright OpenJS Foundation and other contributors
  * Released under the MIT license
  * https://jquery.org/license
  *
@@ -82,42 +80,14 @@
  */
 
 /*!
  * lunr.utils
  * Copyright (C) 2020 Oliver Nightingale
  */
 
-/*! ExcelJS 21-08-2021 */
-
-/*! safe-buffer. MIT License. Feross Aboukhadijeh <https://feross.org/opensource> */
-
-/**
- * Character class utilities for XML NS 1.0 edition 3.
- *
- * @author Louis-Dominique Dubeau
- * @license MIT
- * @copyright Louis-Dominique Dubeau
- */
-
-/**
- * Character classes and associated utilities for the 2nd edition of XML 1.1.
- *
- * @author Louis-Dominique Dubeau
- * @license MIT
- * @copyright Louis-Dominique Dubeau
- */
-
-/**
- * Character classes and associated utilities for the 5th edition of XML 1.0.
- *
- * @author Louis-Dominique Dubeau
- * @license MIT
- * @copyright Louis-Dominique Dubeau
- */
-
 /**
  * lunr - http://lunrjs.com - A bit like Solr, but much smaller and not as bright - 2.3.9
  * Copyright (C) 2020 Oliver Nightingale
  * @license MIT
  */
 
 //! moment.js
```

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/cog.svg` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/cog.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/font-reduce.pe` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/font-reduce.pe`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/print.svg` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/print.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/viewer-icons-min.woff` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/fonts/viewer-icons-min.woff`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/html/fact-details.html` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/html/fact-details.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/html/inspector.html` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/html/inspector.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/arelle.svg` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/arelle.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/favicon.ico` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/accordian.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/accordian.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/aspect.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/aspect.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/aspect.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/aspect.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/calculations.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/calculations.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/chart.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/chart.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/chart.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/chart.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/concept.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/concept.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/concept.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/concept.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/dialog.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/dialog.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/fact.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/fact.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/fact.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/fact.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/factset.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/factset.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/factset.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/factset.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/footnote.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/footnote.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/identifiers.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/identifiers.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/inspector.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/inspector.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -192,15 +192,22 @@
         if (location.hash.startsWith("#f-")) {
             this.selectItem(location.hash.slice(3));
         }
     }
 
     handleMessage(event) {
         const jsonString = event.originalEvent.data;
-        const data = JSON.parse(jsonString);
+        let data;
+        try {
+            data = JSON.parse(jsonString);
+        } catch (e) {
+            // Silently ignore any non-JSON messages as write-excel-file sends
+            // messages to itself when exporting files.
+            return;
+        }
 
         if (data.task == 'SHOW_FACT') {
             this.selectItem(data.factId);
         } else {
             console.log("Not handling unsupported task message: " + jsonString);
         }
     }
```

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/inspector.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/inspector.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/interact.min.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/interact.min.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/ixnode.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/ixnode.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/menu.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/menu.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -42,20 +42,20 @@
         }
         item.appendTo(this._elt.find(".content"));
     }
 
     addDownloadButton(name, filename) {
         const menu = this;
         const item = $('<a></a>')
+            .addClass("item")
             .attr({
                 href: filename
             })
-            .prepend($('<input type="button">')
-                .prop("value", name)
-                .click(() => menu.close()));
+            .text(name)
+            .click(() => menu.close());
         this._add(item);
     }
 
     addCheckboxItem(name, callback, itemName, after, onByDefault) {
         const menu = this;
         const item = $("<label></label>")
             .addClass("menu-checkbox")
```

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/messagebox.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/messagebox.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/moment-jest.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/moment-jest.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/number-matcher.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/number-matcher.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/outline.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/outline.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/outline.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/outline.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/period.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/period.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/period.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/period.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/report.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/report.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/report.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/report.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/search.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/search.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/search.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/search.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/summary.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/summary.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/summary.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/summary.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/tableExport.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/tableExport.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,17 @@
 // See COPYRIGHT.md for copyright information
 
 import $ from 'jquery'
 import FileSaver from 'file-saver'
-import * as Excel from 'exceljs/dist/exceljs.min.js';
+import writeXlsxFile from 'write-excel-file'
 import {
     Fact
 } from './fact.js';
 
+
 export class TableExport {
     constructor(table, report) {
         this._table = table;
         this._report = report;
     }
 
     static addHandles(iframe, report) {
@@ -130,62 +131,61 @@
                 }
             }
         }
         return constantAspects;
     }
 
     _writeTable(data) {
-        const wb = new Excel.Workbook();
-        const ws = wb.addWorksheet('Table');
+        const excelRows = [];
+        const columns = [];
 
         let s = '';
         for (const [i, row] of data.entries()) {
+            const excelRow = [];
             for (const [j, cell] of row.entries()) {
-                const cc = ws.getRow(i + 1).getCell(j + 1);
+                const cc = {};
 
                 if (cell.type === 'fact') {
+                    columns[j] = {
+                        width: 18
+                    };
                     cc.value = Number(cell.fact.value());
-                    cc.numFmt = '#,##0';
-                    ws.getColumn(j + 1).width = 18;
+                    cc.type = Number;
+                    cc.format = '#,##0';
                     /* Make this an option - apply presentation signs */
                     if (cell.negative) {
                         cc.value = Math.abs(cc.value) * -1;
                     } else {
                         cc.value = Math.abs(cc.value);
                     }
-                    cc.border = {};
                     if (cell.topBorder) {
-                        cc.border.top = {
-                            style: "medium",
-                            color: {
-                                argb: 'FF000000'
-                            }
-                        };
+                        cc.topBorderStyle = 'medium';
+                        cc.topBorderColor = '#000000';
                     }
                     if (cell.bottomBorder) {
-                        cc.border.bottom = {
-                            style: "medium",
-                            color: {
-                                argb: 'FF000000'
-                            }
-                        };
+                        cc.bottomBorderStyle = 'medium';
+                        cc.bottomBorderColor = '#000000';
                     }
                 } else if (cell.type === 'aspectLabel') {
                     cc.value = cell.value;
+                    cc.type = String;
+
                 } else {
                     cc.value = cell.value;
-                    cc.font = {
-                        color: {
-                            argb: 'FF707070'
-                        }
-                    };
+                    cc.type = String;
+                    cc.color = '#707070';
                 }
+                excelRow.push(cc);
             }
+            excelRows.push(excelRow);
         }
-        return wb;
+        return {
+            columns: columns,
+            data: excelRows
+        };
     }
 
     exportTable() {
 
         const data = this._getRawTable();
         let rowLength = 0;
 
@@ -268,16 +268,14 @@
                 });
             }
             /* Insert row labels at start of row */
             data[k] = newCols.concat(data[k]);
         }
 
 
-        const wb = this._writeTable(data);
-        wb.xlsx.writeBuffer().then(data => {
-            const blob = new Blob([data], {
-                type: "application/octet-stream"
-            });
-            FileSaver.saveAs(blob, 'table.xlsx');
+        const excelData = this._writeTable(data);
+        writeXlsxFile(excelData.data, {
+            columns: excelData.columns,
+            fileName: 'table.xlsx'
         });
     }
 }
```

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/unit.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/unit.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/unit.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/unit.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/util.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/util.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/util.test.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/util.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/validationreport.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/validationreport.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/viewer.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/js/viewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/accordian.less` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/accordian.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/chart.less` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/chart.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/colours.less` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/colours.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/dialog.less` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/dialog.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/form-controls.less` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/form-controls.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/icons.less` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/icons.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/inspector.less` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/inspector.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/loader.less` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/loader.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/menu.less` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/menu.less`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // See COPYRIGHT.md for copyright information
 
 @import url("form-controls.less");
 
-#ixv {
+#ixv #inspector {
   .menu {
     position: absolute;
     right: 0;
     top: 0;
     line-height: @top-bar-height;
     cursor: pointer;
 
@@ -76,14 +76,23 @@
 
               position: absolute;
               top: 1.1rem;
               left: 1rem;
             }
           }
         }
+
+        a.item {
+          display: block;
+          color: @text;
+
+          &:hover {
+            text-decoration: none;
+          }
+        }
       }
     }
   }
 
   .toolbar-menu {
     .menu-checkbox {
       .wk-checkbox();
```

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/summary.less` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/summary.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/tabs.less` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/tabs.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/viewer.less` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/src/less/viewer.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/webpack.common.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/webpack.common.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/webpack.dev.js` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/viewer/webpack.dev.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/xhtmlserialize.py` & `ixbrl-viewer-1.3.0/iXBRLViewerPlugin/xhtmlserialize.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/PKG-INFO` & `ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixbrl-viewer
-Version: 1.2.2
+Version: 1.3.0
 Summary: The Arelle iXBRL Viewer allows iXBRL reports to be viewed interactively in a web browser.
 Author-email: "arelle.org" <support@arelle.org>
 License: Apache-2.0
 Project-URL: Homepage, https://arelle.org/
 Project-URL: Downloads, https://arelle.org/arelle/pub/
 Project-URL: Documentation, https://arelle.org/arelle/documentation/
 Project-URL: Blog, https://arelle.org/arelle/blog/
```

### Comparing `ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/SOURCES.txt` & `ixbrl-viewer-1.3.0/ixbrl_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/package-lock.json` & `ixbrl-viewer-1.3.0/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9969446634714492%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'write-excel-file': '^1.4.27', delete: ['exceljs', "*

 * *               "'file-saver']}}, 'node_modules/mkdirp': {'dev': True}, 'node_modules/rimraf': "*

 * *               "{'dev': True}, 'node_modules/xmlchars': {'dev': True}, "*

 * *               "'node_modules/write-excel-file': OrderedDict([('version', '1.4.27'), ('resolved', "*

 * *               "'https://registry.npmjs.org/write-excel-file/-/write-excel-file-1.4.27.tgz'), "*

 * *               "('integrity', "*

 * *               "'sha512 […]*

```diff
@@ -4,25 +4,24 @@
     "packages": {
         "": {
             "dependencies": {
                 "chart.js": "^2.9.3",
                 "core-js": "^3.31.1",
                 "css-loader": "^3.4.2",
                 "dateformat": "^5.0.3",
-                "exceljs": "^4.0.1",
-                "file-saver": "^2.0.2",
                 "i18next": "^20.3.2",
                 "interactjs": "^1.8.5",
                 "jquery": "^3.4.1",
                 "jquery-i18next": "^1.2.1",
                 "less": "^3.11.1",
                 "less-loader": "^6.0.0",
                 "lunr": "^2.3.8",
                 "moment": "^2.24.0",
-                "postcss-less": "^6.0.0"
+                "postcss-less": "^6.0.0",
+                "write-excel-file": "^1.4.27"
             },
             "devDependencies": {
                 "babel-core": "^6.26.3",
                 "babel-jest": "^29.6.1",
                 "babel-preset-env": "^1.7.0",
                 "base64-inline-loader": "^2.0.1",
                 "decimal.js": "^10.4.1",
@@ -997,51 +996,14 @@
             "optional": true,
             "os": [
                 "win32"
             ],
             "resolved": "https://registry.npmjs.org/@esbuild/win32-x64/-/win32-x64-0.18.17.tgz",
             "version": "0.18.17"
         },
-        "node_modules/@fast-csv/format": {
-            "dependencies": {
-                "@types/node": "^14.0.1",
-                "lodash.escaperegexp": "^4.1.2",
-                "lodash.isboolean": "^3.0.3",
-                "lodash.isequal": "^4.5.0",
-                "lodash.isfunction": "^3.0.9",
-                "lodash.isnil": "^4.0.0"
-            },
-            "integrity": "sha512-8iRn6QF3I8Ak78lNAa+Gdl5MJJBM5vRHivFtMRUWINdevNo00K7OXxS2PshawLKTejVwieIlPmK5YlLu6w4u8A==",
-            "resolved": "https://registry.npmjs.org/@fast-csv/format/-/format-4.3.5.tgz",
-            "version": "4.3.5"
-        },
-        "node_modules/@fast-csv/format/node_modules/@types/node": {
-            "integrity": "sha512-uq7O52wvo2Lggsx1x21tKZgqkJpvwCseBBPtX/nKQfpVlEsLOb11zZ1CRsWUKvJF0+lzuA9jwvA7Pr2Wt7i3xw==",
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-14.18.54.tgz",
-            "version": "14.18.54"
-        },
-        "node_modules/@fast-csv/parse": {
-            "dependencies": {
-                "@types/node": "^14.0.1",
-                "lodash.escaperegexp": "^4.1.2",
-                "lodash.groupby": "^4.6.0",
-                "lodash.isfunction": "^3.0.9",
-                "lodash.isnil": "^4.0.0",
-                "lodash.isundefined": "^3.0.1",
-                "lodash.uniq": "^4.5.0"
-            },
-            "integrity": "sha512-uRsLYksqpbDmWaSmzvJcuApSEe38+6NQZBUsuAyMZKqHxH0g1wcJgsKUvN3WC8tewaqFjBMMGrkHmC+T7k8LvA==",
-            "resolved": "https://registry.npmjs.org/@fast-csv/parse/-/parse-4.3.6.tgz",
-            "version": "4.3.6"
-        },
-        "node_modules/@fast-csv/parse/node_modules/@types/node": {
-            "integrity": "sha512-uq7O52wvo2Lggsx1x21tKZgqkJpvwCseBBPtX/nKQfpVlEsLOb11zZ1CRsWUKvJF0+lzuA9jwvA7Pr2Wt7i3xw==",
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-14.18.54.tgz",
-            "version": "14.18.54"
-        },
         "node_modules/@ffmpeg-installer/darwin-arm64": {
             "cpu": [
                 "arm64"
             ],
             "dev": true,
             "hasInstallScript": true,
             "integrity": "sha512-hYqTiP63mXz7wSQfuqfFwfLOfwwFChUedeCVKkBtl/cliaTM7/ePI9bVzfZ2c+dWu3TqCwLDRWNSJ5pqZl8otA==",
@@ -3671,57 +3633,32 @@
             "engines": {
                 "node": ">=10.0.0"
             },
             "integrity": "sha512-QHX8HLlncOLpy54mh+k/sWIFd0ThmRqwe9ZjELybGZK+tZ8rUb9VO0saKJUROTbE+KhzDUT7xziGpGrW8Kmd+g==",
             "resolved": "https://registry.npmjs.org/basic-ftp/-/basic-ftp-5.0.3.tgz",
             "version": "5.0.3"
         },
-        "node_modules/big-integer": {
-            "engines": {
-                "node": ">=0.6"
-            },
-            "integrity": "sha512-GPEid2Y9QU1Exl1rpO9B2IPJGHPSupF5GnVIP0blYvNOMer2bTvSWs1jGOUg04hTmu67nmLsQ9TBo1puaotBHg==",
-            "resolved": "https://registry.npmjs.org/big-integer/-/big-integer-1.6.51.tgz",
-            "version": "1.6.51"
-        },
         "node_modules/big.js": {
             "engines": {
                 "node": "*"
             },
             "integrity": "sha512-vyL2OymJxmarO8gxMr0mhChsO9QGwhynfuu4+MHTAW6czfq9humCB7rKpUjDd9YUiDPU4mzpyupFSvOClAwbmQ==",
             "resolved": "https://registry.npmjs.org/big.js/-/big.js-5.2.2.tgz",
             "version": "5.2.2"
         },
-        "node_modules/binary": {
-            "dependencies": {
-                "buffers": "~0.1.1",
-                "chainsaw": "~0.1.0"
-            },
-            "engines": {
-                "node": "*"
-            },
-            "integrity": "sha512-D4H1y5KYwpJgK8wk1Cue5LLPgmwHKYSChkbspQg5JtVuR5ulGckxfR62H3AE9UDkdMC8yyXlqYihuz3Aqg2XZg==",
-            "resolved": "https://registry.npmjs.org/binary/-/binary-0.3.0.tgz",
-            "version": "0.3.0"
-        },
         "node_modules/bl": {
             "dependencies": {
                 "buffer": "^5.5.0",
                 "inherits": "^2.0.4",
                 "readable-stream": "^3.4.0"
             },
             "integrity": "sha512-1W07cM9gS6DcLperZfFSj+bWLtaPGSOHWhPiGzXmvVJbRLdG82sH/Kn8EtW1VqWVA54AKf2h5k5BbnIbwF3h6w==",
             "resolved": "https://registry.npmjs.org/bl/-/bl-4.1.0.tgz",
             "version": "4.1.0"
         },
-        "node_modules/bluebird": {
-            "integrity": "sha512-iD3898SR7sWVRHbiQv+sHUtHnMvC1o3nW5rAcqnq3uOn07DSAppZYUkIGslDz6gXC7HfunPe7YVBgoEJASPcHA==",
-            "resolved": "https://registry.npmjs.org/bluebird/-/bluebird-3.4.7.tgz",
-            "version": "3.4.7"
-        },
         "node_modules/boolbase": {
             "dev": true,
             "integrity": "sha512-JZOSA7Mo9sNGB8+UjSgzdLtokWAky1zbztM3WRLCbZ70/3cTANmQmOdR7y2g+J0e2WXywy1yS468tY+IruqEww==",
             "resolved": "https://registry.npmjs.org/boolbase/-/boolbase-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/brace-expansion": {
@@ -3908,30 +3845,14 @@
             "version": "1.0.1"
         },
         "node_modules/buffer-from": {
             "integrity": "sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==",
             "resolved": "https://registry.npmjs.org/buffer-from/-/buffer-from-1.1.2.tgz",
             "version": "1.1.2"
         },
-        "node_modules/buffer-indexof-polyfill": {
-            "engines": {
-                "node": ">=0.10"
-            },
-            "integrity": "sha512-I7wzHwA3t1/lwXQh+A5PbNvJxgfo5r3xulgpYDB5zckTu/Z9oUK9biouBKQUjEqzaz3HnAT6TYoovmE+GqSf7A==",
-            "resolved": "https://registry.npmjs.org/buffer-indexof-polyfill/-/buffer-indexof-polyfill-1.0.2.tgz",
-            "version": "1.0.2"
-        },
-        "node_modules/buffers": {
-            "engines": {
-                "node": ">=0.2.0"
-            },
-            "integrity": "sha512-9q/rDEGSb/Qsvv2qvzIzdluL5k7AaJOTrw23z9reQthrbF7is4CtlT0DXyO1oei2DCp4uojjzQ7igaSHp1kAEQ==",
-            "resolved": "https://registry.npmjs.org/buffers/-/buffers-0.1.1.tgz",
-            "version": "0.1.1"
-        },
         "node_modules/call-bind": {
             "dependencies": {
                 "function-bind": "^1.1.1",
                 "get-intrinsic": "^1.0.2"
             },
             "dev": true,
             "funding": {
@@ -4025,25 +3946,14 @@
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
             "integrity": "sha512-Vdhm5S11DaFVLlyiKu4hiUTkpZu+y1KA/rZZqVQfOD5YdDT/eQKlkt7NaE0WGOFgX32diqt9MiP9CAiFeRklaA==",
             "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001517.tgz",
             "version": "1.0.30001517"
         },
-        "node_modules/chainsaw": {
-            "dependencies": {
-                "traverse": ">=0.3.0 <0.4"
-            },
-            "engines": {
-                "node": "*"
-            },
-            "integrity": "sha512-75kWfWt6MEKNC8xYXIdRpDehRYY/tNSgwKaJq+dbbDcxORuVrrQ+SEHoWsniVn9XPYfP4gmdWIeDk/4YNp1rNQ==",
-            "resolved": "https://registry.npmjs.org/chainsaw/-/chainsaw-0.1.0.tgz",
-            "version": "0.1.0"
-        },
         "node_modules/chalk": {
             "dependencies": {
                 "ansi-styles": "^3.2.1",
                 "escape-string-regexp": "^1.0.5",
                 "supports-color": "^5.3.0"
             },
             "dev": true,
@@ -4712,19 +4622,14 @@
             "engines": {
                 "node": ">=12.20"
             },
             "integrity": "sha512-Kvr6HmPXUMerlLcLF+Pwq3K7apHpYmGDVqrxcDasBg86UcKeTSNWbEzU8bwdXnxnR44FtMhJAxI4Bov6Y/KUfA==",
             "resolved": "https://registry.npmjs.org/dateformat/-/dateformat-5.0.3.tgz",
             "version": "5.0.3"
         },
-        "node_modules/dayjs": {
-            "integrity": "sha512-QvzAURSbQ0pKdIye2txOzNaHmxtUBXerpY0FJsFXUMKbIZeFm5ht1LS/jFsrncjnmtv8HsG0W2g6c0zUjZWmpA==",
-            "resolved": "https://registry.npmjs.org/dayjs/-/dayjs-1.11.9.tgz",
-            "version": "1.11.9"
-        },
         "node_modules/de-indent": {
             "dev": true,
             "integrity": "sha512-e/1zu3xH5MQryN2zdVaF0OrdNLUbvWxzMbi+iNA6Bky7l1RoP8a2fIbRocyHclXt/arDrrR6lL3TqFD9pMQTsg==",
             "resolved": "https://registry.npmjs.org/de-indent/-/de-indent-1.0.2.tgz",
             "version": "1.0.2"
         },
         "node_modules/debug": {
@@ -4961,44 +4866,14 @@
             "funding": {
                 "url": "https://github.com/fb55/domutils?sponsor=1"
             },
             "integrity": "sha512-H78uMmQtI2AhgDJjWeQmHwJJ2bLPD3GMmO7Zja/ZZh84wkm+4ut+IUnUdRa8uCGX88DiVx1j6FRe1XfxEgjEZA==",
             "resolved": "https://registry.npmjs.org/domutils/-/domutils-3.1.0.tgz",
             "version": "3.1.0"
         },
-        "node_modules/duplexer2": {
-            "dependencies": {
-                "readable-stream": "^2.0.2"
-            },
-            "integrity": "sha512-asLFVfWWtJ90ZyOUHMqk7/S2w2guQKxUI2itj3d92ADHhxUSbCMGi1f1cBcJ7xM1To+pE/Khbwo1yuNbMEPKeA==",
-            "resolved": "https://registry.npmjs.org/duplexer2/-/duplexer2-0.1.4.tgz",
-            "version": "0.1.4"
-        },
-        "node_modules/duplexer2/node_modules/readable-stream": {
-            "dependencies": {
-                "core-util-is": "~1.0.0",
-                "inherits": "~2.0.3",
-                "isarray": "~1.0.0",
-                "process-nextick-args": "~2.0.0",
-                "safe-buffer": "~5.1.1",
-                "string_decoder": "~1.1.1",
-                "util-deprecate": "~1.0.1"
-            },
-            "integrity": "sha512-8p0AUk4XODgIewSi0l8Epjs+EVnWiK7NoDIEGU0HhE7+ZyY8D1IMY7odu5lRrFXGg71L15KG8QrPmum45RTtdA==",
-            "resolved": "https://registry.npmjs.org/readable-stream/-/readable-stream-2.3.8.tgz",
-            "version": "2.3.8"
-        },
-        "node_modules/duplexer2/node_modules/string_decoder": {
-            "dependencies": {
-                "safe-buffer": "~5.1.0"
-            },
-            "integrity": "sha512-n/ShnvDi6FHbbVfviro+WojiFzv+s8MPMHBczVePfUpDJLwoLT0ht1l4YwBCbi8pJAveEEdnkHyPyTP/mzRfwg==",
-            "resolved": "https://registry.npmjs.org/string_decoder/-/string_decoder-1.1.1.tgz",
-            "version": "1.1.1"
-        },
         "node_modules/duplexify": {
             "dependencies": {
                 "end-of-stream": "^1.0.0",
                 "inherits": "^2.0.1",
                 "readable-stream": "^2.0.0",
                 "stream-shift": "^1.0.0"
             },
@@ -5310,33 +5185,14 @@
             "engines": {
                 "node": ">=0.8.x"
             },
             "integrity": "sha512-mQw+2fkQbALzQ7V0MY0IqdnXNOeTtP4r0lN9z7AAawCXgqea7bDii20AYrIBrFd/Hx0M2Ocz6S111CaFkUcb0Q==",
             "resolved": "https://registry.npmjs.org/events/-/events-3.3.0.tgz",
             "version": "3.3.0"
         },
-        "node_modules/exceljs": {
-            "dependencies": {
-                "archiver": "^5.0.0",
-                "dayjs": "^1.8.34",
-                "fast-csv": "^4.3.1",
-                "jszip": "^3.5.0",
-                "readable-stream": "^3.6.0",
-                "saxes": "^5.0.1",
-                "tmp": "^0.2.0",
-                "unzipper": "^0.10.11",
-                "uuid": "^8.3.0"
-            },
-            "engines": {
-                "node": ">=8.3.0"
-            },
-            "integrity": "sha512-hTAeo5b5TPvf8Z02I2sKIT4kSfCnOO2bCxYX8ABqODCdAjppI3gI9VYiGCQQYVcBaBSKlFDMKlAQRqC+kV9O8w==",
-            "resolved": "https://registry.npmjs.org/exceljs/-/exceljs-4.3.0.tgz",
-            "version": "4.3.0"
-        },
         "node_modules/execa": {
             "dependencies": {
                 "cross-spawn": "^7.0.3",
                 "get-stream": "^6.0.0",
                 "human-signals": "^2.1.0",
                 "is-stream": "^2.0.0",
                 "merge-stream": "^2.0.0",
@@ -5419,26 +5275,14 @@
             "funding": {
                 "url": "https://github.com/sponsors/sindresorhus"
             },
             "integrity": "sha512-nBF+F1rAZVCu/p7rjzgA+Yb4lfYXrpl7a6VmJrU8wF9I1CKvP/QwPNZHnOlwbTkY6dvtFIzFMSyQXbLoTQPRpA==",
             "resolved": "https://registry.npmjs.org/get-stream/-/get-stream-5.2.0.tgz",
             "version": "5.2.0"
         },
-        "node_modules/fast-csv": {
-            "dependencies": {
-                "@fast-csv/format": "4.3.5",
-                "@fast-csv/parse": "4.3.6"
-            },
-            "engines": {
-                "node": ">=10.0.0"
-            },
-            "integrity": "sha512-2RNSpuwwsJGP0frGsOmTb9oUF+VkFSM4SyLTDgwf2ciHWTarN0lQTC+F2f/t5J9QjW+c65VFIAAu85GsvMIusw==",
-            "resolved": "https://registry.npmjs.org/fast-csv/-/fast-csv-4.3.6.tgz",
-            "version": "4.3.6"
-        },
         "node_modules/fast-deep-equal": {
             "integrity": "sha512-f3qQ9oQy9j2AhBe/H9VC91wLmKBCCU/gDOnKNAYG5hswO7BLKj09Hc5HYNz9cGI++xlpDCIgDaitVs03ATR84Q==",
             "resolved": "https://registry.npmjs.org/fast-deep-equal/-/fast-deep-equal-3.1.3.tgz",
             "version": "3.1.3"
         },
         "node_modules/fast-fifo": {
             "dev": true,
@@ -5805,39 +5649,14 @@
             "optional": true,
             "os": [
                 "darwin"
             ],
             "resolved": "https://registry.npmjs.org/fsevents/-/fsevents-2.3.2.tgz",
             "version": "2.3.2"
         },
-        "node_modules/fstream": {
-            "dependencies": {
-                "graceful-fs": "^4.1.2",
-                "inherits": "~2.0.0",
-                "mkdirp": ">=0.5 0",
-                "rimraf": "2"
-            },
-            "engines": {
-                "node": ">=0.6"
-            },
-            "integrity": "sha512-WvJ193OHa0GHPEL+AycEJgxvBEwyfRkN1vhjca23OaPVMCaLCXTd5qAu82AjTcgP1UJmytkOKb63Ypde7raDIg==",
-            "resolved": "https://registry.npmjs.org/fstream/-/fstream-1.0.12.tgz",
-            "version": "1.0.12"
-        },
-        "node_modules/fstream/node_modules/rimraf": {
-            "bin": {
-                "rimraf": "bin.js"
-            },
-            "dependencies": {
-                "glob": "^7.1.3"
-            },
-            "integrity": "sha512-uWjbaKIK3T1OSVptzX7Nl6PvQ3qAGtKEtVRjRuazjfL3Bx5eI409VZSqgND+4UNnmzLVdPj9FqFJNPqBZFve4w==",
-            "resolved": "https://registry.npmjs.org/rimraf/-/rimraf-2.7.1.tgz",
-            "version": "2.7.1"
-        },
         "node_modules/function-bind": {
             "dev": true,
             "integrity": "sha512-yIovAzMX49sF8Yl58fSCWJ5svSLuaibPxXQJFLmBObTuCr0Mf1KiPopGM9NiFjiYBCbfaa2Fh6breQ6ANVTI0A==",
             "resolved": "https://registry.npmjs.org/function-bind/-/function-bind-1.1.1.tgz",
             "version": "1.1.1"
         },
         "node_modules/gensync": {
@@ -9162,19 +8981,14 @@
         },
         "node_modules/lines-and-columns": {
             "dev": true,
             "integrity": "sha512-7ylylesZQ/PV29jhEDl3Ufjo6ZX7gCqJr5F7PKrqc93v7fzSymt1BpwEU8nAUXs8qzzvqhbjhK5QZg6Mt/HkBg==",
             "resolved": "https://registry.npmjs.org/lines-and-columns/-/lines-and-columns-1.2.4.tgz",
             "version": "1.2.4"
         },
-        "node_modules/listenercount": {
-            "integrity": "sha512-3mk/Zag0+IJxeDrxSgaDPy4zZ3w05PRZeJNnlWhzFz5OkX49J4krc+A8X2d2M69vGMBEX0uyl8M+W+8gH+kBqQ==",
-            "resolved": "https://registry.npmjs.org/listenercount/-/listenercount-1.0.1.tgz",
-            "version": "1.0.1"
-        },
         "node_modules/loader-runner": {
             "engines": {
                 "node": ">=6.11.5"
             },
             "integrity": "sha512-3R/1M+yS3j5ou80Me59j7F9IMs4PXs3VqRrm0TU3AbKPxlmpoY1TNscJV/oGJXo8qCatFGTfDbY6W6ipGOYXfg==",
             "resolved": "https://registry.npmjs.org/loader-runner/-/loader-runner-4.3.0.tgz",
             "version": "4.3.0"
@@ -9216,75 +9030,35 @@
             "version": "4.2.0"
         },
         "node_modules/lodash.difference": {
             "integrity": "sha512-dS2j+W26TQ7taQBGN8Lbbq04ssV3emRw4NY58WErlTO29pIqS0HmoT5aJ9+TUQ1N3G+JOZSji4eugsWwGp9yPA==",
             "resolved": "https://registry.npmjs.org/lodash.difference/-/lodash.difference-4.5.0.tgz",
             "version": "4.5.0"
         },
-        "node_modules/lodash.escaperegexp": {
-            "integrity": "sha512-TM9YBvyC84ZxE3rgfefxUWiQKLilstD6k7PTGt6wfbtXF8ixIJLOL3VYyV/z+ZiPLsVxAsKAFVwWlWeb2Y8Yyw==",
-            "resolved": "https://registry.npmjs.org/lodash.escaperegexp/-/lodash.escaperegexp-4.1.2.tgz",
-            "version": "4.1.2"
-        },
         "node_modules/lodash.flatten": {
             "integrity": "sha512-C5N2Z3DgnnKr0LOpv/hKCgKdb7ZZwafIrsesve6lmzvZIRZRGaZ/l6Q8+2W7NaT+ZwO3fFlSCzCzrDCFdJfZ4g==",
             "resolved": "https://registry.npmjs.org/lodash.flatten/-/lodash.flatten-4.4.0.tgz",
             "version": "4.4.0"
         },
-        "node_modules/lodash.groupby": {
-            "integrity": "sha512-5dcWxm23+VAoz+awKmBaiBvzox8+RqMgFhi7UvX9DHZr2HdxHXM/Wrf8cfKpsW37RNrvtPn6hSwNqurSILbmJw==",
-            "resolved": "https://registry.npmjs.org/lodash.groupby/-/lodash.groupby-4.6.0.tgz",
-            "version": "4.6.0"
-        },
-        "node_modules/lodash.isboolean": {
-            "integrity": "sha512-Bz5mupy2SVbPHURB98VAcw+aHh4vRV5IPNhILUCsOzRmsTmSQ17jIuqopAentWoehktxGd9e/hbIXq980/1QJg==",
-            "resolved": "https://registry.npmjs.org/lodash.isboolean/-/lodash.isboolean-3.0.3.tgz",
-            "version": "3.0.3"
-        },
-        "node_modules/lodash.isequal": {
-            "integrity": "sha512-pDo3lu8Jhfjqls6GkMgpahsF9kCyayhgykjyLMNFTKWrpVdAQtYyB4muAMWozBB4ig/dtWAmsMxLEI8wuz+DYQ==",
-            "resolved": "https://registry.npmjs.org/lodash.isequal/-/lodash.isequal-4.5.0.tgz",
-            "version": "4.5.0"
-        },
-        "node_modules/lodash.isfunction": {
-            "integrity": "sha512-AirXNj15uRIMMPihnkInB4i3NHeb4iBtNg9WRWuK2o31S+ePwwNmDPaTL3o7dTJ+VXNZim7rFs4rxN4YU1oUJw==",
-            "resolved": "https://registry.npmjs.org/lodash.isfunction/-/lodash.isfunction-3.0.9.tgz",
-            "version": "3.0.9"
-        },
-        "node_modules/lodash.isnil": {
-            "integrity": "sha512-up2Mzq3545mwVnMhTDMdfoG1OurpA/s5t88JmQX809eH3C8491iu2sfKhTfhQtKY78oPNhiaHJUpT/dUDAAtng==",
-            "resolved": "https://registry.npmjs.org/lodash.isnil/-/lodash.isnil-4.0.0.tgz",
-            "version": "4.0.0"
-        },
         "node_modules/lodash.isplainobject": {
             "integrity": "sha512-oSXzaWypCMHkPC3NvBEaPHf0KsA5mvPrOPgQWDsbg8n7orZ290M0BmC/jgRZ4vcJ6DTAhjrsSYgdsW/F+MFOBA==",
             "resolved": "https://registry.npmjs.org/lodash.isplainobject/-/lodash.isplainobject-4.0.6.tgz",
             "version": "4.0.6"
         },
-        "node_modules/lodash.isundefined": {
-            "integrity": "sha512-MXB1is3s899/cD8jheYYE2V9qTHwKvt+npCwpD+1Sxm3Q3cECXCiYHjeHWXNwr6Q0SOBPrYUDxendrO6goVTEA==",
-            "resolved": "https://registry.npmjs.org/lodash.isundefined/-/lodash.isundefined-3.0.1.tgz",
-            "version": "3.0.1"
-        },
         "node_modules/lodash.truncate": {
             "dev": true,
             "integrity": "sha512-jttmRe7bRse52OsWIMDLaXxWqRAmtIUccAQ3garviCqJjafXOfNMO0yMfNpdD6zbGaTU0P5Nz7e7gAT6cKmJRw==",
             "resolved": "https://registry.npmjs.org/lodash.truncate/-/lodash.truncate-4.4.2.tgz",
             "version": "4.4.2"
         },
         "node_modules/lodash.union": {
             "integrity": "sha512-c4pB2CdGrGdjMKYLA+XiRDO7Y0PRQbm/Gzg8qMj+QH+pFVAoTp5sBpO0odL3FjoPCGjK96p6qsP+yQoiLoOBcw==",
             "resolved": "https://registry.npmjs.org/lodash.union/-/lodash.union-4.6.0.tgz",
             "version": "4.6.0"
         },
-        "node_modules/lodash.uniq": {
-            "integrity": "sha512-xfBaXQd9ryd9dlSDvnvI0lvxfLJlYAZzXomUYzLKtUeOQvOP5piqAWuGtrhWeqaXK9hhoM/iyJc5AV+XfsX3HQ==",
-            "resolved": "https://registry.npmjs.org/lodash.uniq/-/lodash.uniq-4.5.0.tgz",
-            "version": "4.5.0"
-        },
         "node_modules/loose-envify": {
             "bin": {
                 "loose-envify": "cli.js"
             },
             "dependencies": {
                 "js-tokens": "^3.0.0 || ^4.0.0"
             },
@@ -9576,14 +9350,15 @@
         "node_modules/mkdirp": {
             "bin": {
                 "mkdirp": "bin/cmd.js"
             },
             "dependencies": {
                 "minimist": "^1.2.6"
             },
+            "dev": true,
             "integrity": "sha512-FP+p8RB8OWpF3YZBCrP5gtADmtXApB5AMLn+vdyA+PyxCjrCs00mjyUozssO33cwDeT3wNGdLxJ5M//YqtHAJw==",
             "resolved": "https://registry.npmjs.org/mkdirp/-/mkdirp-0.5.6.tgz",
             "version": "0.5.6"
         },
         "node_modules/mkdirp-classic": {
             "dev": true,
             "integrity": "sha512-gKLcREMhtuZRwRAfqP3RFW+TK4JqApVBtOIftVgjuABpAtpxhPGaDcfvbhNvD0B8iD1oUr/txX35NjcaY6Ns/A==",
@@ -11340,14 +11115,15 @@
         "node_modules/rimraf": {
             "bin": {
                 "rimraf": "bin.js"
             },
             "dependencies": {
                 "glob": "^7.1.3"
             },
+            "dev": true,
             "funding": {
                 "url": "https://github.com/sponsors/isaacs"
             },
             "integrity": "sha512-JZkJMZkAGFFPP2YqXZXPbMlMBgsxzE8ILs4lMIX/2o0L9UBw9O/Y3o6wFw/i9YLapcUJWwqbi3kdxIPdC62TIA==",
             "resolved": "https://registry.npmjs.org/rimraf/-/rimraf-3.0.2.tgz",
             "version": "3.0.2"
         },
@@ -11390,25 +11166,14 @@
         },
         "node_modules/safer-buffer": {
             "dev": true,
             "integrity": "sha512-YZo3K82SD7Riyi0E1EQPojLz7kpepnSQI9IyPbHHg1XXXevb5dJI7tpyN2ADxGcQbHG7vcyRHk0cbwqcQriUtg==",
             "resolved": "https://registry.npmjs.org/safer-buffer/-/safer-buffer-2.1.2.tgz",
             "version": "2.1.2"
         },
-        "node_modules/saxes": {
-            "dependencies": {
-                "xmlchars": "^2.2.0"
-            },
-            "engines": {
-                "node": ">=10"
-            },
-            "integrity": "sha512-5LBh1Tls8c9xgGjw3QrMwETmTMVk0oFgvrFSvWx62llR2hcEInrKNZ2GZCCuuy2lvWrdl5jhbpeqc5hRYKFOcw==",
-            "resolved": "https://registry.npmjs.org/saxes/-/saxes-5.0.1.tgz",
-            "version": "5.0.1"
-        },
         "node_modules/schema-utils": {
             "dependencies": {
                 "@types/json-schema": "^7.0.5",
                 "ajv": "^6.12.4",
                 "ajv-keywords": "^3.5.2"
             },
             "engines": {
@@ -12327,25 +12092,14 @@
                 "xtend": "~4.0.1"
             },
             "dev": true,
             "integrity": "sha512-/mrRod8xqpA+IHSLyGCQ2s8SPHiCDEeQJSep1jqLYeEUClOFG2Qsh+4FU6G9VeqpZnGW/Su8LQGc4YKni5rYSQ==",
             "resolved": "https://registry.npmjs.org/through2/-/through2-2.0.5.tgz",
             "version": "2.0.5"
         },
-        "node_modules/tmp": {
-            "dependencies": {
-                "rimraf": "^3.0.0"
-            },
-            "engines": {
-                "node": ">=8.17.0"
-            },
-            "integrity": "sha512-76SUhtfqR2Ijn+xllcI5P1oyannHNHByD80W1q447gU3mp9G9PSpGdWmjUOHRDPiHYacIk66W7ubDTuPF3BEtQ==",
-            "resolved": "https://registry.npmjs.org/tmp/-/tmp-0.2.1.tgz",
-            "version": "0.2.1"
-        },
         "node_modules/tmpl": {
             "dev": true,
             "integrity": "sha512-3f0uOEAQwIqGuWW2MVzYg8fV/QNnc/IpuJNG837rLuczAaLVHslWHZQj4IGiEl5Hs3kkbhwL9Ab7Hrsmuj+Smw==",
             "resolved": "https://registry.npmjs.org/tmpl/-/tmpl-1.0.5.tgz",
             "version": "1.0.5"
         },
         "node_modules/to-absolute-glob": {
@@ -12460,22 +12214,14 @@
             "engines": {
                 "node": ">=12"
             },
             "integrity": "sha512-l7FvfAHlcmulp8kr+flpQZmVwtu7nfRV7NZujtN0OqES8EL4O4e0qqzL0DC5gAvx/ZC/9lk6rhcUwYvkBnBnYA==",
             "resolved": "https://registry.npmjs.org/tr46/-/tr46-3.0.0.tgz",
             "version": "3.0.0"
         },
-        "node_modules/traverse": {
-            "engines": {
-                "node": "*"
-            },
-            "integrity": "sha512-iawgk0hLP3SxGKDfnDJf8wTz4p2qImnyihM5Hh/sGvQ3K37dPi/w8sRhdNIxYA1TwFwc5mDhIJq+O0RsvXBKdQ==",
-            "resolved": "https://registry.npmjs.org/traverse/-/traverse-0.3.9.tgz",
-            "version": "0.3.9"
-        },
         "node_modules/trim-newlines": {
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "funding": {
                 "url": "https://github.com/sponsors/sindresorhus"
@@ -12634,53 +12380,14 @@
             "engines": {
                 "node": ">= 10.0.0"
             },
             "integrity": "sha512-hAZsKq7Yy11Zu1DE0OzWjw7nnLZmJZYTDZZyEFHZdUhV8FkH5MCfoU1XMaxXovpyW5nq5scPqq0ZDP9Zyl04oQ==",
             "resolved": "https://registry.npmjs.org/universalify/-/universalify-2.0.0.tgz",
             "version": "2.0.0"
         },
-        "node_modules/unzipper": {
-            "dependencies": {
-                "big-integer": "^1.6.17",
-                "binary": "~0.3.0",
-                "bluebird": "~3.4.1",
-                "buffer-indexof-polyfill": "~1.0.0",
-                "duplexer2": "~0.1.4",
-                "fstream": "^1.0.12",
-                "graceful-fs": "^4.2.2",
-                "listenercount": "~1.0.1",
-                "readable-stream": "~2.3.6",
-                "setimmediate": "~1.0.4"
-            },
-            "integrity": "sha512-ti4wZj+0bQTiX2KmKWuwj7lhV+2n//uXEotUmGuQqrbVZSEGFMbI68+c6JCQ8aAmUWYvtHEz2A8K6wXvueR/6g==",
-            "resolved": "https://registry.npmjs.org/unzipper/-/unzipper-0.10.14.tgz",
-            "version": "0.10.14"
-        },
-        "node_modules/unzipper/node_modules/readable-stream": {
-            "dependencies": {
-                "core-util-is": "~1.0.0",
-                "inherits": "~2.0.3",
-                "isarray": "~1.0.0",
-                "process-nextick-args": "~2.0.0",
-                "safe-buffer": "~5.1.1",
-                "string_decoder": "~1.1.1",
-                "util-deprecate": "~1.0.1"
-            },
-            "integrity": "sha512-8p0AUk4XODgIewSi0l8Epjs+EVnWiK7NoDIEGU0HhE7+ZyY8D1IMY7odu5lRrFXGg71L15KG8QrPmum45RTtdA==",
-            "resolved": "https://registry.npmjs.org/readable-stream/-/readable-stream-2.3.8.tgz",
-            "version": "2.3.8"
-        },
-        "node_modules/unzipper/node_modules/string_decoder": {
-            "dependencies": {
-                "safe-buffer": "~5.1.0"
-            },
-            "integrity": "sha512-n/ShnvDi6FHbbVfviro+WojiFzv+s8MPMHBczVePfUpDJLwoLT0ht1l4YwBCbi8pJAveEEdnkHyPyTP/mzRfwg==",
-            "resolved": "https://registry.npmjs.org/string_decoder/-/string_decoder-1.1.1.tgz",
-            "version": "1.1.1"
-        },
         "node_modules/update-browserslist-db": {
             "bin": {
                 "update-browserslist-db": "cli.js"
             },
             "dependencies": {
                 "escalade": "^3.1.1",
                 "picocolors": "^1.0.0"
@@ -12737,22 +12444,14 @@
             "version": "1.5.10"
         },
         "node_modules/util-deprecate": {
             "integrity": "sha512-EPD5q1uXyFxJpCrLnCc1nHnq3gOa6DZBocAIiI2TaSCA7VCJ1UJDMagCzIkXNsUYfD1daK//LTEQ8xiIbrHtcw==",
             "resolved": "https://registry.npmjs.org/util-deprecate/-/util-deprecate-1.0.2.tgz",
             "version": "1.0.2"
         },
-        "node_modules/uuid": {
-            "bin": {
-                "uuid": "dist/bin/uuid"
-            },
-            "integrity": "sha512-+NYs2QeMWy+GWFOEm9xnn6HCDp0l7QBD7ml8zLUmJ+93Q5NF0NocErnwkTkXVFNiX3/fpC6afS8Dhb/gz7R7eg==",
-            "resolved": "https://registry.npmjs.org/uuid/-/uuid-8.3.2.tgz",
-            "version": "8.3.2"
-        },
         "node_modules/v8-to-istanbul": {
             "dependencies": {
                 "@jridgewell/trace-mapping": "^0.3.12",
                 "@types/istanbul-lib-coverage": "^2.0.1",
                 "convert-source-map": "^1.6.0"
             },
             "dev": true,
@@ -13247,14 +12946,25 @@
             "version": "2.0.1"
         },
         "node_modules/wrappy": {
             "integrity": "sha512-l4Sp/DRseor9wL6EvV2+TuQn63dMkPjZ/sp9XkghTEbV9KlPS1xUsZ3u7/IQO4wxtcFB4bgpQPRcR3QCvezPcQ==",
             "resolved": "https://registry.npmjs.org/wrappy/-/wrappy-1.0.2.tgz",
             "version": "1.0.2"
         },
+        "node_modules/write-excel-file": {
+            "dependencies": {
+                "@babel/runtime": "^7.17.9",
+                "archiver": "^5.3.1",
+                "file-saver": "^2.0.5",
+                "jszip": "^3.9.1"
+            },
+            "integrity": "sha512-KZMdDzPZ4uRsLJTFj6DfXni1QOQIfE3O30vFiwW6xFVruBWm/F517BDyteBDqMKeTQAVzQGPUz7BmSFDe9qX0Q==",
+            "resolved": "https://registry.npmjs.org/write-excel-file/-/write-excel-file-1.4.27.tgz",
+            "version": "1.4.27"
+        },
         "node_modules/write-file-atomic": {
             "dependencies": {
                 "imurmurhash": "^0.1.4",
                 "signal-exit": "^3.0.7"
             },
             "dev": true,
             "engines": {
@@ -13291,14 +13001,15 @@
                 "node": ">=12"
             },
             "integrity": "sha512-ICP2e+jsHvAj2E2lIHxa5tjXRlKDJo4IdvPvCXbXQGdzSfmSpNVyIKMvoZHjDY9DP0zV17iI85o90vRFXNccRw==",
             "resolved": "https://registry.npmjs.org/xml-name-validator/-/xml-name-validator-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/xmlchars": {
+            "dev": true,
             "integrity": "sha512-JZnDKK8B0RCDw84FNdDAIpZK+JuJw+s7Lz8nksI7SIuU3UXJJslUthsi+uWBUYOwPFwW7W7PRLRfUKpxjtjFCw==",
             "resolved": "https://registry.npmjs.org/xmlchars/-/xmlchars-2.2.0.tgz",
             "version": "2.2.0"
         },
         "node_modules/xtend": {
             "dev": true,
             "engines": {
```

### Comparing `ixbrl-viewer-1.2.2/package.json` & `ixbrl-viewer-1.3.0/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'dependencies'": "{'write-excel-file': '^1.4.27', delete: ['exceljs', 'file-saver']}"}*

```diff
@@ -1,25 +1,24 @@
 {
     "author": "",
     "dependencies": {
         "chart.js": "^2.9.3",
         "core-js": "^3.31.1",
         "css-loader": "^3.4.2",
         "dateformat": "^5.0.3",
-        "exceljs": "^4.0.1",
-        "file-saver": "^2.0.2",
         "i18next": "^20.3.2",
         "interactjs": "^1.8.5",
         "jquery": "^3.4.1",
         "jquery-i18next": "^1.2.1",
         "less": "^3.11.1",
         "less-loader": "^6.0.0",
         "lunr": "^2.3.8",
         "moment": "^2.24.0",
-        "postcss-less": "^6.0.0"
+        "postcss-less": "^6.0.0",
+        "write-excel-file": "^1.4.27"
     },
     "description": "iXBRL Viewer",
     "devDependencies": {
         "babel-core": "^6.26.3",
         "babel-jest": "^29.6.1",
         "babel-preset-env": "^1.7.0",
         "base64-inline-loader": "^2.0.1",
```

### Comparing `ixbrl-viewer-1.2.2/pyproject.toml` & `ixbrl-viewer-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/samples/Makefile` & `ixbrl-viewer-1.3.0/samples/Makefile`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/samples/Makefile-src` & `ixbrl-viewer-1.3.0/samples/Makefile-src`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/samples/build-viewer.py` & `ixbrl-viewer-1.3.0/samples/build-viewer.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/samples/fetch-sample-files.py` & `ixbrl-viewer-1.3.0/samples/fetch-sample-files.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/samples/sample-files.list` & `ixbrl-viewer-1.3.0/samples/sample-files.list`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/samples/src/continuation/continuation.html` & `ixbrl-viewer-1.3.0/samples/src/continuation/continuation.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/samples/src/ixds-test/document1.html` & `ixbrl-viewer-1.3.0/samples/src/ixds-test/document1.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/samples/src/ixds-test/faurecia.html` & `ixbrl-viewer-1.3.0/samples/src/ixds-test/faurecia.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/samples/src/ixds-test/valeo.html` & `ixbrl-viewer-1.3.0/samples/src/ixds-test/valeo.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/samples/src/scrollable-div/scrollable-div.html` & `ixbrl-viewer-1.3.0/samples/src/scrollable-div/scrollable-div.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html` & `ixbrl-viewer-1.3.0/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/tests/puppeteer/framework/core_elements.js` & `ixbrl-viewer-1.3.0/tests/puppeteer/framework/core_elements.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/doc_frame.js` & `ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/doc_frame.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/fact_details_panel.js` & `ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/fact_details_panel.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/search_panel.js` & `ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/search_panel.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/toolbar.js` & `ixbrl-viewer-1.3.0/tests/puppeteer/framework/page_objects/toolbar.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/tests/puppeteer/framework/viewer_page.js` & `ixbrl-viewer-1.3.0/tests/puppeteer/framework/viewer_page.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/tests/puppeteer/puppeteer_test_run_via_intellij.jpg` & `ixbrl-viewer-1.3.0/tests/puppeteer/puppeteer_test_run_via_intellij.jpg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/tests/puppeteer/test_filings/filing_documents_smoke_test.zip` & `ixbrl-viewer-1.3.0/tests/puppeteer/test_filings/filing_documents_smoke_test.zip`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/tests/puppeteer/test_filings/highlights.zip` & `ixbrl-viewer-1.3.0/tests/puppeteer/test_filings/highlights.zip`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/tests/puppeteer/tests/fact_properties.test.js` & `ixbrl-viewer-1.3.0/tests/puppeteer/tests/fact_properties.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/tests/puppeteer/tests/highlight.test.js` & `ixbrl-viewer-1.3.0/tests/puppeteer/tests/highlight.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/tests/puppeteer/tests/search.test.js` & `ixbrl-viewer-1.3.0/tests/puppeteer/tests/search.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py` & `ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py` & `ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py` & `ixbrl-viewer-1.3.0/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py`

 * *Files identical despite different names*

