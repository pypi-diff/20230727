# Comparing `tmp/preppipe-0.0.1.post117.tar.gz` & `tmp/preppipe-0.0.1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preppipe-0.0.1.post117.tar", last modified: Thu Jul 27 17:17:58 2023, max compression
+gzip compressed data, was "preppipe-0.0.1.post3.tar", last modified: Sat Dec 25 09:30:24 2021, max compression
```

## Comparing `preppipe-0.0.1.post117.tar` & `preppipe-0.0.1.post3.tar`

### file list

```diff
@@ -1,107 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.843215 preppipe-0.0.1.post117/
--rw-r--r--   0 runner    (1001) docker     (123)    20765 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 17:17:58.843215 preppipe-0.0.1.post117/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/develop_bootstrap.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.831215 preppipe-0.0.1.post117/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   112854 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/docs/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.831215 preppipe-0.0.1.post117/docs/image/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4639 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/docs/image/logo.png
--rwxr-xr-x   0 runner    (1001) docker     (123)   109431 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/preppipe.ico
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/preppipe_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-27 17:17:58.843215 preppipe-0.0.1.post117/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.827215 preppipe-0.0.1.post117/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.831215 preppipe-0.0.1.post117/src/preppipe/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-27 17:17:58.000000 preppipe-0.0.1.post117/src/preppipe/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.835215 preppipe-0.0.1.post117/src/preppipe/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/analysis/icfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/analysis/passes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.835215 preppipe-0.0.1.post117/src/preppipe/analysis/vnmodel/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/analysis/vnmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/analysis/vnmodel/assetusage.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/analysis/vnmodel/passes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/analysis/vnmodel/timemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/analysis/vnmodel/vnsaydump.py
--rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/commontypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.835215 preppipe-0.0.1.post117/src/preppipe/frontend/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2014 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/CommandParse.g4
--rwxr-xr-x   0 runner    (1001) docker     (123)     1350 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/CommandScan.g4
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.835215 preppipe-0.0.1.post117/src/preppipe/frontend/_antlr_generated/
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/_antlr_generated/CommandParseLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/_antlr_generated/CommandParseListener.py
--rw-r--r--   0 runner    (1001) docker     (123)    24157 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/_antlr_generated/CommandParseParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/_antlr_generated/CommandParseVisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/_antlr_generated/CommandScanLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/_antlr_generated/CommandScanListener.py
--rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/_antlr_generated/CommandScanParser.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/_antlr_generated/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/_antlr_generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37804 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/commandsemantics.py
--rw-r--r--   0 runner    (1001) docker     (123)    29974 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/commandsyntaxparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    65365 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/opendocument.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.839215 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/SayScan.g4
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.839215 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/_antlr_generated/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/_antlr_generated/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/_antlr_generated/SayScanLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18647 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/_antlr_generated/SayScanParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/_antlr_generated/SayScanVisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/_antlr_generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/passes.py
--rw-r--r--   0 runner    (1001) docker     (123)    39157 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/vnast.py
--rw-r--r--   0 runner    (1001) docker     (123)   119785 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/vncodegen.py
--rw-r--r--   0 runner    (1001) docker     (123)    61059 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/vnparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/vnsayscan.py
--rw-r--r--   0 runner    (1001) docker     (123)    23125 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/frontend/vnmodel/vnutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/imageexpr.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/inputmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)   142422 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/irbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/irdataop.py
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/language.py
--rw-r--r--   0 runner    (1001) docker     (123)    13101 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/nameresolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    42360 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/pipeline_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.839215 preppipe-0.0.1.post117/src/preppipe/renpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/renpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25428 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/renpy/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    51799 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/renpy/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)    21249 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/renpy/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/renpy/passes.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/renpy/preppipert.rpy
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/testbench.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.839215 preppipe-0.0.1.post117/src/preppipe/transform/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/transform/passes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.839215 preppipe-0.0.1.post117/src/preppipe/transform/vnmodel/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/transform/vnmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/transform/vnmodel/passes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/transform/vnmodel/vnblocksorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/transform/vnmodel/vnentryinference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/transform/vnmodel/vnlongsaysplitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.843215 preppipe-0.0.1.post117/src/preppipe/util/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/util/antlr4util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/util/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/util/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/util/graphtrait.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/util/nameconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/util/typo.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/util/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)    68622 2023-07-27 17:17:36.000000 preppipe-0.0.1.post117/src/preppipe/vnmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:17:58.835215 preppipe-0.0.1.post117/src/preppipe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 17:17:58.000000 preppipe-0.0.1.post117/src/preppipe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-27 17:17:58.000000 preppipe-0.0.1.post117/src/preppipe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:17:58.000000 preppipe-0.0.1.post117/src/preppipe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-27 17:17:58.000000 preppipe-0.0.1.post117/src/preppipe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 17:17:58.000000 preppipe-0.0.1.post117/src/preppipe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.760685 preppipe-0.0.1.post3/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/src/preppipe/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2021-12-25 09:30:24.000000 preppipe-0.0.1.post3/src/preppipe/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2543 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/commontypes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/src/preppipe/documentimport/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/documentimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9105 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/documentimport/opendocument.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7795 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/documentmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/src/preppipe/enginesupport/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/enginesupport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6485 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/enginesupport/enginesupport.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31191 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/enginesupport/renpy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3177 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/visualnovelmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/src/preppipe/vnexport/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/vnexport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3899 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/vnexport/renpy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/src/preppipe/vnimport/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/vnimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2076 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/vnimport/document.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    34366 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/vnmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/src/preppipe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2021-12-25 09:30:24.000000 preppipe-0.0.1.post3/src/preppipe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2021-12-25 09:30:24.000000 preppipe-0.0.1.post3/src/preppipe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-25 09:30:24.000000 preppipe-0.0.1.post3/src/preppipe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-12-25 09:30:24.000000 preppipe-0.0.1.post3/src/preppipe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-25 09:30:24.000000 preppipe-0.0.1.post3/src/preppipe.egg-info/top_level.txt
```

### Comparing `preppipe-0.0.1.post117/LICENSE` & `preppipe-0.0.1.post3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2022 PrepPipe's Contributors
+   Copyright [yyyy] [name of copyright owner]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `preppipe-0.0.1.post117/PKG-INFO` & `preppipe-0.0.1.post3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: preppipe
-Version: 0.0.1.post117
+Version: 0.0.1.post3
 Summary: Document to Visual Novel generator
 Home-page: https://github.com/PrepPipe/preppipe-python
 Author: Shengjie Xu
 Author-email: xsj617603321@gmail.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/PrepPipe/preppipe-python/issues
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 1 - Planning
-Requires-Python: >=3.10
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PrepPipe
 
 Document TODO
 
 Experimental project. Do not use for production (for now).
 
+
+
```

### Comparing `preppipe-0.0.1.post117/setup.cfg` & `preppipe-0.0.1.post3/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -9,34 +9,24 @@
 project_urls = 
 	Bug Tracker = https://github.com/PrepPipe/preppipe-python/issues
 license = Apache-2.0
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
-	Development Status :: 1 - Planning
 
 [options]
-include_package_data = True
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.10
+python_requires = >=3.6
 install_requires = 
-	llist
-	odfpy
 	pillow
+	odfpy
 	pydub
-	numpy
-	ghostscript
-	editdistance
-	bidict
-	pypinyin
-	graphviz
-	antlr4-python3-runtime >= 4.10
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `preppipe-0.0.1.post117/src/preppipe.egg-info/PKG-INFO` & `preppipe-0.0.1.post3/src/preppipe.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: preppipe
-Version: 0.0.1.post117
+Version: 0.0.1.post3
 Summary: Document to Visual Novel generator
 Home-page: https://github.com/PrepPipe/preppipe-python
 Author: Shengjie Xu
 Author-email: xsj617603321@gmail.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/PrepPipe/preppipe-python/issues
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 1 - Planning
-Requires-Python: >=3.10
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PrepPipe
 
 Document TODO
 
 Experimental project. Do not use for production (for now).
 
+
+
```

