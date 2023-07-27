# Comparing `tmp/ixbrl-viewer-1.2.1.tar.gz` & `tmp/ixbrl-viewer-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixbrl-viewer-1.2.1.tar", last modified: Wed Jul 26 21:18:26 2023, max compression
+gzip compressed data, was "ixbrl-viewer-1.2.2.tar", last modified: Thu Jul 27 15:24:31 2023, max compression
```

## Comparing `ixbrl-viewer-1.2.1.tar` & `ixbrl-viewer-1.2.2.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.687860 ixbrl-viewer-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.babelrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.655861 ixbrl-viewer-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.655861 ixbrl-viewer-1.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.github/ISSUE_TEMPLATE/questions.yml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.github/ISSUE_TEMPLATE/request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.655861 ixbrl-viewer-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.github/workflows/node-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.github/workflows/npm-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.github/workflows/puppeteer.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.github/workflows/python-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/COPYRIGHT.md
--rw-r--r--   0 runner    (1001) docker     (123)    16664 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-07-26 21:18:26.687860 ixbrl-viewer-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/PLUGINS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.655861 ixbrl-viewer-1.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.663860 ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/
--rw-r--r--   0 runner    (1001) docker     (123)    92632 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   149033 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml
--rw-r--r--   0 runner    (1001) docker     (123)  2413470 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm
--rw-r--r--   0 runner    (1001) docker     (123)   535018 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml
--rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1219995 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml
--rw-r--r--   0 runner    (1001) docker     (123)   858776 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml
--rw-r--r--   0 runner    (1001) docker     (123)    60067 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm
--rw-r--r--   0 runner    (1001) docker     (123)    68052 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm
--rw-r--r--   0 runner    (1001) docker     (123)  4343804 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.667860 ixbrl-viewer-1.2.1/examples/example_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/example_plugin/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   194458 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/example_plugin/example-plugin.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/example_plugin/extended-viewer.js
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/example_plugin/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    95416 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/example_plugin/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/example_plugin/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/example_plugin/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (123)   917698 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/ixbrl-viewer-demo.gif
--rw-r--r--   0 runner    (1001) docker     (123)    17954 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/review-mode.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.667860 ixbrl-viewer-1.2.1/examples/workiva-january-2023-8-k-ixbrl-viewer/
--rw-r--r--   0 runner    (1001) docker     (123)   222306 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm
--rw-r--r--   0 runner    (1001) docker     (123)   223016 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm
--rw-r--r--   0 runner    (1001) docker     (123)    56173 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    24833 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml
--rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.671861 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 21:18:26.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25725 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/iXBRLViewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/stubviewer.html
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.671861 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.671861 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/dist/
--rw-r--r--   0 runner    (1001) docker     (123)  1897286 2023-07-26 21:18:12.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-26 21:18:12.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/i18next-parser.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.651861 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.671861 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/fonts/cog.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/fonts/font-reduce.pe
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/fonts/print.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/fonts/viewer-icons-min.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.675861 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/html/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/html/fact-details.html
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/html/footnote-details.html
--rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/html/inspector.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.651861 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/i18n/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.675861 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/i18n/en/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/i18n/en/currencies.json
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/i18n/en/referenceparts.json
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.675861 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/i18n/es/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/i18n/es/currencies.json
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/i18n/es/referenceparts.json
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.675861 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/img/
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/img/arelle.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.679860 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/accordian.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/aspect.js
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/aspect.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/calculations.js
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/chart.js
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/chart.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/concept.js
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/concept.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/dialog.js
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/fact.js
--rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/fact.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/factset.js
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/factset.test.js
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/footnote.js
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/identifiers.js
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    44060 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/inspector.js
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/inspector.test.js
--rw-r--r--   0 runner    (1001) docker     (123)    85048 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/interact.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/ixnode.js
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/menu.js
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/messagebox.js
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/moment-jest.js
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/number-matcher.js
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/outline.js
--rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/outline.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/period.js
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/period.test.js
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/qname.js
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/report.js
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/report.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/search.js
--rw-r--r--   0 runner    (1001) docker     (123)    21034 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/search.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/summary.js
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/summary.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/tableExport.js
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/test-utils.js
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/unit.js
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/unit.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/util.js
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/util.test.js
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/validationreport.js
--rw-r--r--   0 runner    (1001) docker     (123)    34470 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/viewer.js
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/viewerOptions.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.683860 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/accordian.less
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/block-list.less
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/chart.less
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/clearfix.less
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/colours.less
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/common.less
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/components.less
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/core.less
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/dialog.less
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/fonts.less
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/form-controls.less
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/icons.less
--rw-r--r--   0 runner    (1001) docker     (123)    20550 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/inspector.less
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/loader.less
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/menu.less
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/summary.less
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/tabs.less
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/text-block-viewer.less
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/text-mixins.less
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/validation-report.less
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/viewer.less
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/version.js
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/webpack.common.js
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/webpack.dev.js
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/webpack.prod.js
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/iXBRLViewerPlugin/xhtmlserialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.683860 ixbrl-viewer-1.2.1/ixbrl_viewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-07-26 21:18:26.000000 ixbrl-viewer-1.2.1/ixbrl_viewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-07-26 21:18:26.000000 ixbrl-viewer-1.2.1/ixbrl_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:18:26.000000 ixbrl-viewer-1.2.1/ixbrl_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-26 21:18:26.000000 ixbrl-viewer-1.2.1/ixbrl_viewer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-26 21:18:26.000000 ixbrl-viewer-1.2.1/ixbrl_viewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-26 21:18:26.000000 ixbrl-viewer-1.2.1/ixbrl_viewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)   504607 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.683860 ixbrl-viewer-1.2.1/samples/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/samples/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/samples/Makefile-src
--rwxr-xr-x   0 runner    (1001) docker     (123)     4370 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/samples/build-viewer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/samples/fetch-sample-files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/samples/sample-files.list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.651861 ixbrl-viewer-1.2.1/samples/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.683860 ixbrl-viewer-1.2.1/samples/src/continuation/
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/samples/src/continuation/continuation.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.683860 ixbrl-viewer-1.2.1/samples/src/ixds-test/
--rw-r--r--   0 runner    (1001) docker     (123)    26111 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/samples/src/ixds-test/document1.html
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/samples/src/ixds-test/faurecia.html
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/samples/src/ixds-test/valeo.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.683860 ixbrl-viewer-1.2.1/samples/src/scrollable-div/
--rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/samples/src/scrollable-div/scrollable-div.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.683860 ixbrl-viewer-1.2.1/samples/src/xbrl-invalid-tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 21:18:26.687860 ixbrl-viewer-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.683860 ixbrl-viewer-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.687860 ixbrl-viewer-1.2.1/tests/puppeteer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.687860 ixbrl-viewer-1.2.1/tests/puppeteer/framework/
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/puppeteer/framework/core_elements.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.687860 ixbrl-viewer-1.2.1/tests/puppeteer/framework/page_objects/
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/puppeteer/framework/page_objects/doc_frame.js
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/puppeteer/framework/page_objects/fact_details_panel.js
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/puppeteer/framework/page_objects/search_panel.js
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/puppeteer/framework/page_objects/toolbar.js
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/puppeteer/framework/utils.js
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/puppeteer/framework/viewer_page.js
--rw-r--r--   0 runner    (1001) docker     (123)    61701 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/puppeteer/puppeteer_test_run_via_intellij.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.687860 ixbrl-viewer-1.2.1/tests/puppeteer/test_filings/
--rw-r--r--   0 runner    (1001) docker     (123)    21469 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/puppeteer/test_filings/filing_documents_smoke_test.zip
--rw-r--r--   0 runner    (1001) docker     (123)    18766 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/puppeteer/test_filings/highlights.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.687860 ixbrl-viewer-1.2.1/tests/puppeteer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/puppeteer/tests/fact_properties.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/puppeteer/tests/highlight.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/puppeteer/tests/search.test.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.687860 ixbrl-viewer-1.2.1/tests/puppeteer/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/puppeteer/tools/generate.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.687860 ixbrl-viewer-1.2.1/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:18:26.687860 ixbrl-viewer-1.2.1/tests/unit_tests/iXBRLViewerPlugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/unit_tests/iXBRLViewerPlugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py
--rw-r--r--   0 runner    (1001) docker     (123)    26993 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-07-26 21:17:25.000000 ixbrl-viewer-1.2.1/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.154666 ixbrl-viewer-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.babelrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.114666 ixbrl-viewer-1.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.114666 ixbrl-viewer-1.2.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/ISSUE_TEMPLATE/questions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/ISSUE_TEMPLATE/request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.118666 ixbrl-viewer-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/workflows/node-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/workflows/npm-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/workflows/puppeteer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/workflows/python-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/COPYRIGHT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16664 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-07-27 15:24:31.154666 ixbrl-viewer-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/PLUGINS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.118666 ixbrl-viewer-1.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.126666 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)    92632 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   149033 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  2413470 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm
+-rw-r--r--   0 runner    (1001) docker     (123)   535018 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1219995 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   858776 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    60067 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm
+-rw-r--r--   0 runner    (1001) docker     (123)    68052 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm
+-rw-r--r--   0 runner    (1001) docker     (123)  4343804 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.130666 ixbrl-viewer-1.2.2/examples/example_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/example_plugin/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   194458 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/example_plugin/example-plugin.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/example_plugin/extended-viewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/example_plugin/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95465 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/example_plugin/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/example_plugin/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/example_plugin/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)   917698 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/ixbrl-viewer-demo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    17954 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/review-mode.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.134666 ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)   222306 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm
+-rw-r--r--   0 runner    (1001) docker     (123)   223016 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm
+-rw-r--r--   0 runner    (1001) docker     (123)    56173 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    24833 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.134666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 15:24:30.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25725 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/iXBRLViewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/stubviewer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.134666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.138666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)  1897286 2023-07-27 15:24:14.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-27 15:24:14.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/i18next-parser.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.110666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.138666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/cog.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/font-reduce.pe
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/print.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/viewer-icons-min.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.138666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/html/fact-details.html
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/html/footnote-details.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/html/inspector.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.110666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.138666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/en/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/en/currencies.json
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/en/referenceparts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.138666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/es/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/es/currencies.json
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/es/referenceparts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.138666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/arelle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.146666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/accordian.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/aspect.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/aspect.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/calculations.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/chart.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/chart.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/concept.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/concept.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/dialog.js
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/fact.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/fact.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/factset.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/factset.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/footnote.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/identifiers.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44060 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/inspector.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/inspector.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)    85048 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/interact.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/ixnode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/menu.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/messagebox.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/moment-jest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/number-matcher.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/outline.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/outline.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/period.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/period.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/qname.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/report.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/report.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21034 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/search.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/summary.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/summary.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/tableExport.js
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/test-utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/unit.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/unit.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/util.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/util.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/validationreport.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34470 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/viewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/viewerOptions.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.146666 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/accordian.less
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/block-list.less
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/chart.less
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/clearfix.less
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/colours.less
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/common.less
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/components.less
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/core.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/dialog.less
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/fonts.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/form-controls.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/icons.less
+-rw-r--r--   0 runner    (1001) docker     (123)    20550 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/inspector.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/loader.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/menu.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/summary.less
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/tabs.less
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/text-block-viewer.less
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/text-mixins.less
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/validation-report.less
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/viewer.less
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/version.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/webpack.common.js
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/webpack.dev.js
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/webpack.prod.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/iXBRLViewerPlugin/xhtmlserialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-07-27 15:24:31.000000 ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-07-27 15:24:31.000000 ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:24:31.000000 ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 15:24:31.000000 ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 15:24:31.000000 ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 15:24:31.000000 ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   504607 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/Makefile-src
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4370 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/build-viewer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/fetch-sample-files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/sample-files.list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.114666 ixbrl-viewer-1.2.2/samples/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/samples/src/continuation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/src/continuation/continuation.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/samples/src/ixds-test/
+-rw-r--r--   0 runner    (1001) docker     (123)    26111 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/src/ixds-test/document1.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/src/ixds-test/faurecia.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/src/ixds-test/valeo.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/samples/src/scrollable-div/
+-rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/src/scrollable-div/scrollable-div.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/samples/src/xbrl-invalid-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 15:24:31.154666 ixbrl-viewer-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/puppeteer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/puppeteer/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/framework/core_elements.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/doc_frame.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/fact_details_panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/search_panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/toolbar.js
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/framework/utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/framework/viewer_page.js
+-rw-r--r--   0 runner    (1001) docker     (123)    61701 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/puppeteer_test_run_via_intellij.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/puppeteer/test_filings/
+-rw-r--r--   0 runner    (1001) docker     (123)    21469 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/test_filings/filing_documents_smoke_test.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    18766 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/test_filings/highlights.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/puppeteer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/tests/fact_properties.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/tests/highlight.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/tests/search.test.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/puppeteer/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/puppeteer/tools/generate.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.150666 ixbrl-viewer-1.2.2/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:24:31.154666 ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26993 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-07-27 15:23:20.000000 ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py
```

### Comparing `ixbrl-viewer-1.2.1/.github/ISSUE_TEMPLATE/bug.yml` & `ixbrl-viewer-1.2.2/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   - type: input
     id: version
     attributes:
       label: Version
       description: |
         What version of ixbrl-viewer are you using?
         - In the browser, right click + inspect
-        - Scroll to the bottom of the `<body>` tag and find the script tag containing the version eg: `<script type="text/javascript" src="https://cdn-prod.wdesk.com/ixbrl-viewer/<version>/ixbrlviewer.js"></script>`
+        - Scroll to the bottom of the `<body>` tag and find the script tag containing the version eg: `<script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js"></script>`
       placeholder: e.g. 1.1.43
     validations:
       required: true
   - type: dropdown
     id: browsers
     attributes:
       label: With which browsers are you experiencing the bug?
```

### Comparing `ixbrl-viewer-1.2.1/.github/dependabot.yml` & `ixbrl-viewer-1.2.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/.github/workflows/node-tests.yml` & `ixbrl-viewer-1.2.2/.github/workflows/node-tests.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/.github/workflows/npm-package.yml` & `ixbrl-viewer-1.2.2/.github/workflows/npm-package.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/.github/workflows/puppeteer.yml` & `ixbrl-viewer-1.2.2/.github/workflows/puppeteer.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/.github/workflows/python-package.yml` & `ixbrl-viewer-1.2.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/.github/workflows/python-tests.yml` & `ixbrl-viewer-1.2.2/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/LICENSE` & `ixbrl-viewer-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/Makefile` & `ixbrl-viewer-1.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/NOTICE` & `ixbrl-viewer-1.2.2/NOTICE`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/PKG-INFO` & `ixbrl-viewer-1.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixbrl-viewer
-Version: 1.2.1
+Version: 1.2.2
 Summary: The Arelle iXBRL Viewer allows iXBRL reports to be viewed interactively in a web browser.
 Author-email: "arelle.org" <support@arelle.org>
 License: Apache-2.0
 Project-URL: Homepage, https://arelle.org/
 Project-URL: Downloads, https://arelle.org/arelle/pub/
 Project-URL: Documentation, https://arelle.org/arelle/documentation/
 Project-URL: Blog, https://arelle.org/arelle/blog/
@@ -76,18 +76,18 @@
 ## Accessing the JavaScript viewer application
 
 ### Accessing via the CDN
 
 The JavaScript file is available via a CDN. It can be accessed via the following url:
 
 ```text
-https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js
+https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
 ```
 
-Where `<version tag>` is the current version of ixbrl-viewer you are using. For instance [1.0.0][CDN].
+Where `<version>` is the current version of ixbrl-viewer you are using. For instance [1.2.0][CDN].
 
 ### Accessing via Github
 
 When a new version of ixbrl-viewer is released, the javascript is included as a
 release asset. The asset can be found on the releases [page][ixbrlviewer-github-releases] for each version of
 the ixbrl-viewer.  
 
@@ -97,15 +97,15 @@
 2. Install the dependencies for javascript by running: `npm install`.  This
    command must be run from within the `ixbrl-viewer directory` (i.e. the root
    of your checkout of the repository).
 3. Run `npm run prod`. This will create the ixbrlviewer.js in the
    iXBRLViewerPlugin/viewer/dist directory.
 
 [ixbrlviewer-github]: https://github.com/Arelle/ixbrl-viewer
-[CDN]: https://cdn-prod.wdesk.com/ixbrl-viewer/1.0.0/ixbrlviewer.js
+[CDN]: https://cdn.jsdelivr.net/npm/ixbrl-viewer@1.2.0/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
 [ixbrlviewer-github-releases]: https://github.com/Arelle/ixbrl-viewer/releases/tag/0.1.58
 [arelle-download]: http://arelle.org/pub
 
 ## JavaScript Versioning
 
 The ixbrl-viewer plugin embeds processed XBRL metadata in the HTML that has a specific format read
 by the JavaScript. The metadata produced by a version will be broken if a major version bump is
@@ -125,15 +125,15 @@
 5. You should now have a **Save iXBRL Viewer instance** on the **Tools** menu.
 6. Open the ixbrl filing zip in Arelle
 7. Select **Save iXBRL Viewer instance** option on the **Tools** menu
 8. Provide a **script URL** to the **ixbrlviewer.js** file.
 
    This url can be one of the following:
 
-   1. `https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js`
+   1. `https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js`
    2. A relative url to the downloaded ixviewer.js from github
    3. A relative url to the locally built ixviewer.js
 
 9. Save the viewer iXBRL file to a new file in the newly created directory by
    selecting **Browse**, browsing to the directory, and providing a file name.
 
 10. You should now be able to open the created file in Chrome, and the iXBRL viewer
@@ -148,24 +148,24 @@
 ## Producing an ixbrl-viewer via the Arelle command line
 
 ### Preparing an iXBRL file via the command line
 
 The plugin can also be used on the command line:
 
 ```shell
-python3 Arelle/arelleCmdLine.py --plugins=<path to iXBRLViewerPlugin> -f ixbrl-report.html --save-viewer ixbrl-report-viewer.html --viewer-url https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js
+python3 Arelle/arelleCmdLine.py --plugins=<path to iXBRLViewerPlugin> -f ixbrl-report.html --save-viewer ixbrl-report-viewer.html --viewer-url https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
 ```
 
 Notes:
 
 * "Arelle/arelleCmdLine.py" should be the path to your installation of Arelle
 * The plugin path needs to an absolute file path to the ixbrl-viewer plugin
 * The viewer url can be one of the following:
 
-  1. `https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js`
+  1. `https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js`
   2. A relative url to the downloaded ixviewer.js from github
   3. A relative url to the locally built ixviewer.js
 
 ### Preparing an iXBRL document set
 
 The iXBRL Viewer supports Inline XBRL document sets.  This requires the `inlineXbrlDocumentSet` plugin.
 The input is specified using JSON in the following form:
@@ -180,27 +180,27 @@
   }
 ]
 ```
 
 The output must be specified as a directory.  For example:
 
 ```shell
-python3 Arelle/arelleCmdLine.py --plugins '/path/to/iXBRLViewerPlugin|inlineXbrlDocumentSet' -f '[{"ixds":[{"file":"document1.html"},{"file":"document2.html"}]}]'  --save-viewer out-dir --viewer-url https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js
+python3 Arelle/arelleCmdLine.py --plugins '/path/to/iXBRLViewerPlugin|inlineXbrlDocumentSet' -f '[{"ixds":[{"file":"document1.html"},{"file":"document2.html"}]}]'  --save-viewer out-dir --viewer-url https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
 ```
 
 Notes:
 
 * The first file specified is the "primary" file, and should be opened in a
   browser to use the viewer.  The other files will be loaded in separate tabs
   within the viewer.
 * "Arelle/arelleCmdLine.py" should be the path to your installation of Arelle
 * The plugin path needs to an absolute file path to the ixbrl-viewer plugin
 * The viewer url can be one of the following:
 
-  1. `https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js`
+  1. `https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js`
   2. A relative url to the downloaded ixviewer.js from github
   3. A relative url to the locally built ixviewer.js
 
 ### Using build-viewer.py
 
 As an alternative to the standard Arelle command line, the
 `samples/build-viewer.py` script can also be used.  To use the script, both the
```

### Comparing `ixbrl-viewer-1.2.1/PLUGINS.md` & `ixbrl-viewer-1.2.2/PLUGINS.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     loadPlugin();
 }
 ```
 
 The `ixbrl-viewer` project can be added as a dev dependency in `package.json`:
 
 ```
-   "devDependencies": {
-       "ixbrl-viewer": "Arelle/ixbrl-viewer"
-   }
+    "devDependencies": {
+        "ixbrl-viewer": "^1.2.0"
+    }
 ```
 
 This will cause the project to be fetched from github by `npm install`.
```

### Comparing `ixbrl-viewer-1.2.1/README.md` & `ixbrl-viewer-1.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,18 +43,18 @@
 ## Accessing the JavaScript viewer application
 
 ### Accessing via the CDN
 
 The JavaScript file is available via a CDN. It can be accessed via the following url:
 
 ```text
-https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js
+https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
 ```
 
-Where `<version tag>` is the current version of ixbrl-viewer you are using. For instance [1.0.0][CDN].
+Where `<version>` is the current version of ixbrl-viewer you are using. For instance [1.2.0][CDN].
 
 ### Accessing via Github
 
 When a new version of ixbrl-viewer is released, the javascript is included as a
 release asset. The asset can be found on the releases [page][ixbrlviewer-github-releases] for each version of
 the ixbrl-viewer.  
 
@@ -64,15 +64,15 @@
 2. Install the dependencies for javascript by running: `npm install`.  This
    command must be run from within the `ixbrl-viewer directory` (i.e. the root
    of your checkout of the repository).
 3. Run `npm run prod`. This will create the ixbrlviewer.js in the
    iXBRLViewerPlugin/viewer/dist directory.
 
 [ixbrlviewer-github]: https://github.com/Arelle/ixbrl-viewer
-[CDN]: https://cdn-prod.wdesk.com/ixbrl-viewer/1.0.0/ixbrlviewer.js
+[CDN]: https://cdn.jsdelivr.net/npm/ixbrl-viewer@1.2.0/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
 [ixbrlviewer-github-releases]: https://github.com/Arelle/ixbrl-viewer/releases/tag/0.1.58
 [arelle-download]: http://arelle.org/pub
 
 ## JavaScript Versioning
 
 The ixbrl-viewer plugin embeds processed XBRL metadata in the HTML that has a specific format read
 by the JavaScript. The metadata produced by a version will be broken if a major version bump is
@@ -92,15 +92,15 @@
 5. You should now have a **Save iXBRL Viewer instance** on the **Tools** menu.
 6. Open the ixbrl filing zip in Arelle
 7. Select **Save iXBRL Viewer instance** option on the **Tools** menu
 8. Provide a **script URL** to the **ixbrlviewer.js** file.
 
    This url can be one of the following:
 
-   1. `https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js`
+   1. `https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js`
    2. A relative url to the downloaded ixviewer.js from github
    3. A relative url to the locally built ixviewer.js
 
 9. Save the viewer iXBRL file to a new file in the newly created directory by
    selecting **Browse**, browsing to the directory, and providing a file name.
 
 10. You should now be able to open the created file in Chrome, and the iXBRL viewer
@@ -115,24 +115,24 @@
 ## Producing an ixbrl-viewer via the Arelle command line
 
 ### Preparing an iXBRL file via the command line
 
 The plugin can also be used on the command line:
 
 ```shell
-python3 Arelle/arelleCmdLine.py --plugins=<path to iXBRLViewerPlugin> -f ixbrl-report.html --save-viewer ixbrl-report-viewer.html --viewer-url https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js
+python3 Arelle/arelleCmdLine.py --plugins=<path to iXBRLViewerPlugin> -f ixbrl-report.html --save-viewer ixbrl-report-viewer.html --viewer-url https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
 ```
 
 Notes:
 
 * "Arelle/arelleCmdLine.py" should be the path to your installation of Arelle
 * The plugin path needs to an absolute file path to the ixbrl-viewer plugin
 * The viewer url can be one of the following:
 
-  1. `https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js`
+  1. `https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js`
   2. A relative url to the downloaded ixviewer.js from github
   3. A relative url to the locally built ixviewer.js
 
 ### Preparing an iXBRL document set
 
 The iXBRL Viewer supports Inline XBRL document sets.  This requires the `inlineXbrlDocumentSet` plugin.
 The input is specified using JSON in the following form:
@@ -147,27 +147,27 @@
   }
 ]
 ```
 
 The output must be specified as a directory.  For example:
 
 ```shell
-python3 Arelle/arelleCmdLine.py --plugins '/path/to/iXBRLViewerPlugin|inlineXbrlDocumentSet' -f '[{"ixds":[{"file":"document1.html"},{"file":"document2.html"}]}]'  --save-viewer out-dir --viewer-url https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js
+python3 Arelle/arelleCmdLine.py --plugins '/path/to/iXBRLViewerPlugin|inlineXbrlDocumentSet' -f '[{"ixds":[{"file":"document1.html"},{"file":"document2.html"}]}]'  --save-viewer out-dir --viewer-url https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
 ```
 
 Notes:
 
 * The first file specified is the "primary" file, and should be opened in a
   browser to use the viewer.  The other files will be loaded in separate tabs
   within the viewer.
 * "Arelle/arelleCmdLine.py" should be the path to your installation of Arelle
 * The plugin path needs to an absolute file path to the ixbrl-viewer plugin
 * The viewer url can be one of the following:
 
-  1. `https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js`
+  1. `https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js`
   2. A relative url to the downloaded ixviewer.js from github
   3. A relative url to the locally built ixviewer.js
 
 ### Using build-viewer.py
 
 As an alternative to the standard Arelle command line, the
 `samples/build-viewer.py` script can also be used.  To use the script, both the
```

### Comparing `ixbrl-viewer-1.2.1/examples/README.md` & `ixbrl-viewer-1.2.2/examples/README.md`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd` & `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630.xsd`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml` & `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_cal.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm` & `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_d2.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml` & `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_def.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg` & `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_g1.jpg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml` & `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_lab.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml` & `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/clx-20220630_pre.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm` & `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex21subsidiaries.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm` & `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex23accountingfirmc.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm` & `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex311ceocertificati.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm` & `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex312cfocertificati.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm` & `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex32ceocfocertifica.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm` & `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/fy22clxex992reconofeconomi.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm` & `ixbrl-viewer-1.2.2/examples/clorox-2022-10-K-ixbrl-viewer/ixbrl-viewer.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/example_plugin/README.md` & `ixbrl-viewer-1.2.2/examples/example_plugin/README.md`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/example_plugin/example-plugin.gif` & `ixbrl-viewer-1.2.2/examples/example_plugin/example-plugin.gif`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/example_plugin/extended-viewer.js` & `ixbrl-viewer-1.2.2/examples/example_plugin/extended-viewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/example_plugin/package-lock.json` & `ixbrl-viewer-1.2.2/examples/example_plugin/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998576388888889%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'ixbrl-viewer': '^1.2.0'}}, 'node_modules/ixbrl-viewer': "*

 * *               "{'version': '1.2.0', 'resolved': "*

 * *               "'https://registry.npmjs.org/ixbrl-viewer/-/ixbrl-viewer-1.2.0.tgz', 'integrity': "*

 * *               "'sha512-Qp7DdK8XrWZ6PAYW9iHOIr7tWeN52fbnNFdtyyYdSaUKuAtje8beewZ+J/uafoNc1hcQ3IxYelBKhaThilQ8sw==', "*

 * *               "delete: ['license']}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "lockfileVersion": 3,
     "name": "extended_ixbrl_viewer",
     "packages": {
         "": {
             "dependencies": {
-                "ixbrl-viewer": "Arelle/ixbrl-viewer"
+                "ixbrl-viewer": "^1.2.0"
             },
             "name": "extended_ixbrl_viewer",
             "version": "1.0.0"
         },
         "node_modules/@babel/runtime": {
             "dependencies": {
                 "regenerator-runtime": "^0.13.11"
@@ -1218,17 +1218,17 @@
                 "jquery-i18next": "^1.2.1",
                 "less": "^3.11.1",
                 "less-loader": "^6.0.0",
                 "lunr": "^2.3.8",
                 "moment": "^2.24.0",
                 "postcss-less": "^6.0.0"
             },
-            "license": "Apache-2.0",
-            "resolved": "git+ssh://git@github.com/Arelle/ixbrl-viewer.git#d09f16675cdda589619c935146665674eba874e4",
-            "version": "0.0.0"
+            "integrity": "sha512-Qp7DdK8XrWZ6PAYW9iHOIr7tWeN52fbnNFdtyyYdSaUKuAtje8beewZ+J/uafoNc1hcQ3IxYelBKhaThilQ8sw==",
+            "resolved": "https://registry.npmjs.org/ixbrl-viewer/-/ixbrl-viewer-1.2.0.tgz",
+            "version": "1.2.0"
         },
         "node_modules/jest-worker": {
             "dependencies": {
                 "@types/node": "*",
                 "merge-stream": "^2.0.0",
                 "supports-color": "^8.0.0"
             },
```

### Comparing `ixbrl-viewer-1.2.1/examples/example_plugin/webpack.config.js` & `ixbrl-viewer-1.2.2/examples/example_plugin/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/ixbrl-viewer-demo.gif` & `ixbrl-viewer-1.2.2/examples/ixbrl-viewer-demo.gif`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/review-mode.png` & `ixbrl-viewer-1.2.2/examples/review-mode.png`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm` & `ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31abylawsofworkivai.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm` & `ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/exhibit31bbylawsofworkivai.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm` & `ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/ixbrl-viewer.htm`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd` & `ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109.xsd`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml` & `ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_lab.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml` & `ixbrl-viewer-1.2.2/examples/workiva-january-2023-8-k-ixbrl-viewer/wk-20230109_pre.xml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/__init__.py` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/__init__.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/iXBRLViewer.py` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/iXBRLViewer.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/ui.py` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/ui.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -69049,15 +69049,15 @@
         }, _r.prototype.isReviewModeEnabled = function() {
             return this.isFeatureEnabled("review")
         }, _r.prototype._loadInspectorHTML = function() {
             t()(n(845)).prependTo("body");
             var e = n(610).toString();
             t()('<style id="ixv-style"></style>').prop("type", "text/css").text(e).appendTo("head"), t()('<link id="ixv-favicon" type="image/x-icon" rel="shortcut icon" />').attr("href", n(688)).appendTo("head");
             try {
-                t()(".inspector-foot .version").text("1.2.1")
+                t()(".inspector-foot .version").text("1.2.2")
             } catch (e) {}
         }, _r.prototype._reparentDocument = function() {
             var e = t()("#ixv #iframe-container"),
                 n = t()('<iframe title="iXBRL document view"/>').appendTo(e)[0],
                 r = n.contentDocument || n.contentWindow.document;
             r.open(), r.write("<!DOCTYPE html><html><head><title></title></head><body></body></html>"), r.close();
             var i = t()("title").text();
```

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/fonts/cog.svg` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/cog.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/fonts/font-reduce.pe` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/font-reduce.pe`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/fonts/print.svg` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/print.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/fonts/viewer-icons-min.woff` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/fonts/viewer-icons-min.woff`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/html/fact-details.html` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/html/fact-details.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/html/inspector.html` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/html/inspector.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/en/translation.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/i18n/es/translation.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/img/arelle.svg` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/arelle.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/img/favicon.ico` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/inline-viewer.png`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/inline-viewer.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.png`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/img/powered-by-workiva.svg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/accordian.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/accordian.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/aspect.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/aspect.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/aspect.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/aspect.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/calculations.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/calculations.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/chart.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/chart.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/chart.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/chart.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/concept.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/concept.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/concept.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/concept.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/dialog.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/dialog.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/docOrderIndex.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/fact.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/fact.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/fact.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/fact.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/factset.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/factset.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/factset.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/factset.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/footnote.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/footnote.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/identifiers.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/identifiers.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/identifiers.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/inspector.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/inspector.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/inspector.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/inspector.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/interact.min.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/interact.min.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/ixbrlviewer.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/ixnode.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/ixnode.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/menu.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/menu.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/messagebox.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/messagebox.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/moment-jest.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/moment-jest.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/number-matcher-preprocess.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/number-matcher.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/number-matcher.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/number-matcher.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/outline.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/outline.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/outline.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/outline.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/period.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/period.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/period.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/period.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/report.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/report.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/report.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/report.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/search.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/search.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/search.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/search.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/summary.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/summary.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/summary.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/summary.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/tableExport.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/tableExport.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/textblockviewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/unit.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/unit.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/unit.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/unit.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/util.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/util.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/util.test.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/util.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/validationreport.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/validationreport.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/js/viewer.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/js/viewer.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/accordian.less` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/accordian.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/chart.less` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/chart.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/colours.less` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/colours.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/dialog.less` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/dialog.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/form-controls.less` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/form-controls.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/icons.less` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/icons.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/inspector.less` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/inspector.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/loader.less` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/loader.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/menu.less` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/menu.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/summary.less` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/summary.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/tabs.less` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/tabs.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/src/less/viewer.less` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/src/less/viewer.less`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/webpack.common.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/webpack.common.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/viewer/webpack.dev.js` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/viewer/webpack.dev.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/iXBRLViewerPlugin/xhtmlserialize.py` & `ixbrl-viewer-1.2.2/iXBRLViewerPlugin/xhtmlserialize.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/ixbrl_viewer.egg-info/PKG-INFO` & `ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixbrl-viewer
-Version: 1.2.1
+Version: 1.2.2
 Summary: The Arelle iXBRL Viewer allows iXBRL reports to be viewed interactively in a web browser.
 Author-email: "arelle.org" <support@arelle.org>
 License: Apache-2.0
 Project-URL: Homepage, https://arelle.org/
 Project-URL: Downloads, https://arelle.org/arelle/pub/
 Project-URL: Documentation, https://arelle.org/arelle/documentation/
 Project-URL: Blog, https://arelle.org/arelle/blog/
@@ -76,18 +76,18 @@
 ## Accessing the JavaScript viewer application
 
 ### Accessing via the CDN
 
 The JavaScript file is available via a CDN. It can be accessed via the following url:
 
 ```text
-https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js
+https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
 ```
 
-Where `<version tag>` is the current version of ixbrl-viewer you are using. For instance [1.0.0][CDN].
+Where `<version>` is the current version of ixbrl-viewer you are using. For instance [1.2.0][CDN].
 
 ### Accessing via Github
 
 When a new version of ixbrl-viewer is released, the javascript is included as a
 release asset. The asset can be found on the releases [page][ixbrlviewer-github-releases] for each version of
 the ixbrl-viewer.  
 
@@ -97,15 +97,15 @@
 2. Install the dependencies for javascript by running: `npm install`.  This
    command must be run from within the `ixbrl-viewer directory` (i.e. the root
    of your checkout of the repository).
 3. Run `npm run prod`. This will create the ixbrlviewer.js in the
    iXBRLViewerPlugin/viewer/dist directory.
 
 [ixbrlviewer-github]: https://github.com/Arelle/ixbrl-viewer
-[CDN]: https://cdn-prod.wdesk.com/ixbrl-viewer/1.0.0/ixbrlviewer.js
+[CDN]: https://cdn.jsdelivr.net/npm/ixbrl-viewer@1.2.0/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
 [ixbrlviewer-github-releases]: https://github.com/Arelle/ixbrl-viewer/releases/tag/0.1.58
 [arelle-download]: http://arelle.org/pub
 
 ## JavaScript Versioning
 
 The ixbrl-viewer plugin embeds processed XBRL metadata in the HTML that has a specific format read
 by the JavaScript. The metadata produced by a version will be broken if a major version bump is
@@ -125,15 +125,15 @@
 5. You should now have a **Save iXBRL Viewer instance** on the **Tools** menu.
 6. Open the ixbrl filing zip in Arelle
 7. Select **Save iXBRL Viewer instance** option on the **Tools** menu
 8. Provide a **script URL** to the **ixbrlviewer.js** file.
 
    This url can be one of the following:
 
-   1. `https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js`
+   1. `https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js`
    2. A relative url to the downloaded ixviewer.js from github
    3. A relative url to the locally built ixviewer.js
 
 9. Save the viewer iXBRL file to a new file in the newly created directory by
    selecting **Browse**, browsing to the directory, and providing a file name.
 
 10. You should now be able to open the created file in Chrome, and the iXBRL viewer
@@ -148,24 +148,24 @@
 ## Producing an ixbrl-viewer via the Arelle command line
 
 ### Preparing an iXBRL file via the command line
 
 The plugin can also be used on the command line:
 
 ```shell
-python3 Arelle/arelleCmdLine.py --plugins=<path to iXBRLViewerPlugin> -f ixbrl-report.html --save-viewer ixbrl-report-viewer.html --viewer-url https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js
+python3 Arelle/arelleCmdLine.py --plugins=<path to iXBRLViewerPlugin> -f ixbrl-report.html --save-viewer ixbrl-report-viewer.html --viewer-url https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
 ```
 
 Notes:
 
 * "Arelle/arelleCmdLine.py" should be the path to your installation of Arelle
 * The plugin path needs to an absolute file path to the ixbrl-viewer plugin
 * The viewer url can be one of the following:
 
-  1. `https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js`
+  1. `https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js`
   2. A relative url to the downloaded ixviewer.js from github
   3. A relative url to the locally built ixviewer.js
 
 ### Preparing an iXBRL document set
 
 The iXBRL Viewer supports Inline XBRL document sets.  This requires the `inlineXbrlDocumentSet` plugin.
 The input is specified using JSON in the following form:
@@ -180,27 +180,27 @@
   }
 ]
 ```
 
 The output must be specified as a directory.  For example:
 
 ```shell
-python3 Arelle/arelleCmdLine.py --plugins '/path/to/iXBRLViewerPlugin|inlineXbrlDocumentSet' -f '[{"ixds":[{"file":"document1.html"},{"file":"document2.html"}]}]'  --save-viewer out-dir --viewer-url https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js
+python3 Arelle/arelleCmdLine.py --plugins '/path/to/iXBRLViewerPlugin|inlineXbrlDocumentSet' -f '[{"ixds":[{"file":"document1.html"},{"file":"document2.html"}]}]'  --save-viewer out-dir --viewer-url https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js
 ```
 
 Notes:
 
 * The first file specified is the "primary" file, and should be opened in a
   browser to use the viewer.  The other files will be loaded in separate tabs
   within the viewer.
 * "Arelle/arelleCmdLine.py" should be the path to your installation of Arelle
 * The plugin path needs to an absolute file path to the ixbrl-viewer plugin
 * The viewer url can be one of the following:
 
-  1. `https://cdn-prod.wdesk.com/ixbrl-viewer/<version tag>/ixbrlviewer.js`
+  1. `https://cdn.jsdelivr.net/npm/ixbrl-viewer@<version>/iXBRLViewerPlugin/viewer/dist/ixbrlviewer.js`
   2. A relative url to the downloaded ixviewer.js from github
   3. A relative url to the locally built ixviewer.js
 
 ### Using build-viewer.py
 
 As an alternative to the standard Arelle command line, the
 `samples/build-viewer.py` script can also be used.  To use the script, both the
```

### Comparing `ixbrl-viewer-1.2.1/ixbrl_viewer.egg-info/SOURCES.txt` & `ixbrl-viewer-1.2.2/ixbrl_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/package-lock.json` & `ixbrl-viewer-1.2.2/package-lock.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/package.json` & `ixbrl-viewer-1.2.2/package.json`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/pyproject.toml` & `ixbrl-viewer-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/samples/Makefile` & `ixbrl-viewer-1.2.2/samples/Makefile`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/samples/Makefile-src` & `ixbrl-viewer-1.2.2/samples/Makefile-src`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/samples/build-viewer.py` & `ixbrl-viewer-1.2.2/samples/build-viewer.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/samples/fetch-sample-files.py` & `ixbrl-viewer-1.2.2/samples/fetch-sample-files.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/samples/sample-files.list` & `ixbrl-viewer-1.2.2/samples/sample-files.list`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/samples/src/continuation/continuation.html` & `ixbrl-viewer-1.2.2/samples/src/continuation/continuation.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/samples/src/ixds-test/document1.html` & `ixbrl-viewer-1.2.2/samples/src/ixds-test/document1.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/samples/src/ixds-test/faurecia.html` & `ixbrl-viewer-1.2.2/samples/src/ixds-test/faurecia.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/samples/src/ixds-test/valeo.html` & `ixbrl-viewer-1.2.2/samples/src/ixds-test/valeo.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/samples/src/scrollable-div/scrollable-div.html` & `ixbrl-viewer-1.2.2/samples/src/scrollable-div/scrollable-div.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html` & `ixbrl-viewer-1.2.2/samples/src/xbrl-invalid-tests/xbrl-invalid-test.html`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/tests/puppeteer/framework/core_elements.js` & `ixbrl-viewer-1.2.2/tests/puppeteer/framework/core_elements.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/tests/puppeteer/framework/page_objects/doc_frame.js` & `ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/doc_frame.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/tests/puppeteer/framework/page_objects/fact_details_panel.js` & `ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/fact_details_panel.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/tests/puppeteer/framework/page_objects/search_panel.js` & `ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/search_panel.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/tests/puppeteer/framework/page_objects/toolbar.js` & `ixbrl-viewer-1.2.2/tests/puppeteer/framework/page_objects/toolbar.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/tests/puppeteer/framework/viewer_page.js` & `ixbrl-viewer-1.2.2/tests/puppeteer/framework/viewer_page.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/tests/puppeteer/puppeteer_test_run_via_intellij.jpg` & `ixbrl-viewer-1.2.2/tests/puppeteer/puppeteer_test_run_via_intellij.jpg`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/tests/puppeteer/test_filings/filing_documents_smoke_test.zip` & `ixbrl-viewer-1.2.2/tests/puppeteer/test_filings/filing_documents_smoke_test.zip`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/tests/puppeteer/test_filings/highlights.zip` & `ixbrl-viewer-1.2.2/tests/puppeteer/test_filings/highlights.zip`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/tests/puppeteer/tests/fact_properties.test.js` & `ixbrl-viewer-1.2.2/tests/puppeteer/tests/fact_properties.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/tests/puppeteer/tests/highlight.test.js` & `ixbrl-viewer-1.2.2/tests/puppeteer/tests/highlight.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/tests/puppeteer/tests/search.test.js` & `ixbrl-viewer-1.2.2/tests/puppeteer/tests/search.test.js`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py` & `ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/mock_arelle.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py` & `ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/test_iXBRLViewer.py`

 * *Files identical despite different names*

### Comparing `ixbrl-viewer-1.2.1/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py` & `ixbrl-viewer-1.2.2/tests/unit_tests/iXBRLViewerPlugin/test_xhtmlserialize.py`

 * *Files identical despite different names*

