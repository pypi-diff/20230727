# Comparing `tmp/text_quality-0.2.0.tar.gz` & `tmp/text_quality-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_quality-0.2.0.tar", last modified: Thu Jul 27 14:16:05 2023, max compression
+gzip compressed data, was "text_quality-0.2.2.tar", last modified: Thu Jul 27 14:59:49 2023, max compression
```

## Comparing `text_quality-0.2.0.tar` & `text_quality-0.2.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.977377 text_quality-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-27 14:15:57.000000 text_quality-0.2.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-27 14:15:57.000000 text_quality-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25899 2023-07-27 14:15:57.000000 text_quality-0.2.0/LICENSE_NL_OPENTAAL.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-27 14:15:57.000000 text_quality-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 14:15:57.000000 text_quality-0.2.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-27 14:16:05.977377 text_quality-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-07-27 14:15:57.000000 text_quality-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-27 14:15:57.000000 text_quality-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.949376 text_quality-0.2.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-27 14:15:57.000000 text_quality-0.2.0/scripts/classify_text_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-27 14:16:05.981377 text_quality-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 14:15:57.000000 text_quality-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.953377 text_quality-0.2.0/text_quality/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.953377 text_quality-0.2.0/text_quality/classifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/classifier/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.945376 text_quality-0.2.0/text_quality/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.953377 text_quality-0.2.0/text_quality/data/classifier/
--rw-r--r--   0 runner    (1001) docker     (123)    31726 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/classifier/pipeline_nn.joblib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.957377 text_quality-0.2.0/text_quality/data/dicts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.961377 text_quality-0.2.0/text_quality/data/dicts/hunspell/
--rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/hunspell/de.aff
--rw-r--r--   0 runner    (1001) docker     (123)  1116164 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/hunspell/de.dic
--rw-r--r--   0 runner    (1001) docker     (123)   201526 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/hunspell/fr.aff
--rw-r--r--   0 runner    (1001) docker     (123)  1222092 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/hunspell/fr.dic
--rw-r--r--   0 runner    (1001) docker     (123)    46575 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/hunspell/nl.aff
--rw-r--r--   0 runner    (1001) docker     (123)  2491328 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/hunspell/nl.dic
--rw-r--r--   0 runner    (1001) docker     (123)  1910341 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/lb.txt
--rw-r--r--   0 runner    (1001) docker     (123)   769888 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/nl_voc.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.965377 text_quality-0.2.0/text_quality/data/qgrams/
--rw-r--r--   0 runner    (1001) docker     (123) 11463434 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/qgrams/nl_voc.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.977377 text_quality-0.2.0/text_quality/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/featurize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.977377 text_quality-0.2.0/text_quality/feature/scorer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/scorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/scorer/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/scorer/garbage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/scorer/q_gram.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/scorer/scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.977377 text_quality-0.2.0/text_quality/page/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/page/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/page/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.953377 text_quality-0.2.0/text_quality.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-27 14:16:05.000000 text_quality-0.2.0/text_quality.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-27 14:16:05.000000 text_quality-0.2.0/text_quality.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:16:05.000000 text_quality-0.2.0/text_quality.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:16:05.000000 text_quality-0.2.0/text_quality.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-27 14:16:05.000000 text_quality-0.2.0/text_quality.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-27 14:16:05.000000 text_quality-0.2.0/text_quality.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:49.527153 text_quality-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-27 14:59:37.000000 text_quality-0.2.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-27 14:59:37.000000 text_quality-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25899 2023-07-27 14:59:37.000000 text_quality-0.2.2/LICENSE_NL_OPENTAAL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-27 14:59:37.000000 text_quality-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 14:59:37.000000 text_quality-0.2.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-27 14:59:49.527153 text_quality-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-27 14:59:37.000000 text_quality-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-27 14:59:37.000000 text_quality-0.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:49.503153 text_quality-0.2.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-27 14:59:37.000000 text_quality-0.2.2/scripts/classify_text_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-27 14:59:49.527153 text_quality-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 14:59:37.000000 text_quality-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:49.503153 text_quality-0.2.2/text_quality/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:49.503153 text_quality-0.2.2/text_quality/classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/classifier/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:49.499153 text_quality-0.2.2/text_quality/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:49.503153 text_quality-0.2.2/text_quality/data/classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)    31726 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/data/classifier/pipeline_nn.joblib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:49.507153 text_quality-0.2.2/text_quality/data/dicts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:49.511153 text_quality-0.2.2/text_quality/data/dicts/hunspell/
+-rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/data/dicts/hunspell/de.aff
+-rw-r--r--   0 runner    (1001) docker     (123)  1116164 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/data/dicts/hunspell/de.dic
+-rw-r--r--   0 runner    (1001) docker     (123)   201526 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/data/dicts/hunspell/fr.aff
+-rw-r--r--   0 runner    (1001) docker     (123)  1222092 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/data/dicts/hunspell/fr.dic
+-rw-r--r--   0 runner    (1001) docker     (123)    46575 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/data/dicts/hunspell/nl.aff
+-rw-r--r--   0 runner    (1001) docker     (123)  2491328 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/data/dicts/hunspell/nl.dic
+-rw-r--r--   0 runner    (1001) docker     (123)  1910341 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/data/dicts/lb.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   769888 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/data/dicts/nl_voc.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:49.515153 text_quality-0.2.2/text_quality/data/qgrams/
+-rw-r--r--   0 runner    (1001) docker     (123) 11463434 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/data/qgrams/nl_voc.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:49.527153 text_quality-0.2.2/text_quality/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/feature/featurize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:49.527153 text_quality-0.2.2/text_quality/feature/scorer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/feature/scorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/feature/scorer/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/feature/scorer/garbage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/feature/scorer/q_gram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/feature/scorer/scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/feature/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:49.527153 text_quality-0.2.2/text_quality/page/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/page/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/page/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-27 14:59:37.000000 text_quality-0.2.2/text_quality/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:49.503153 text_quality-0.2.2/text_quality.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-27 14:59:49.000000 text_quality-0.2.2/text_quality.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-27 14:59:49.000000 text_quality-0.2.2/text_quality.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:59:49.000000 text_quality-0.2.2/text_quality.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:59:49.000000 text_quality-0.2.2/text_quality.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-27 14:59:49.000000 text_quality-0.2.2/text_quality.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-27 14:59:49.000000 text_quality-0.2.2/text_quality.egg-info/top_level.txt
```

### Comparing `text_quality-0.2.0/LICENSE` & `text_quality-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/LICENSE_NL_OPENTAAL.txt` & `text_quality-0.2.2/LICENSE_NL_OPENTAAL.txt`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/PKG-INFO` & `text_quality-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_quality
-Version: 0.2.0
+Version: 0.2.2
 Summary: A package to determine the quality of a a digitized text, from a handwritten script or scanned print (HTR/OCR output).
 Home-page: https://github.com/laHTeR/htr-quality-classifier
 Author: Carsten Schnober
 Author-email: c.schnober@esciencecenter.nl
 Project-URL: Bug Tracker, https://github.com/laHTeR/htr-quality-classifier/issues
 Keywords: htr,ocr
 Classifier: Development Status :: 3 - Alpha
@@ -28,15 +28,14 @@
 A package to determine the quality of a a digitized text, from a handwritten script or scanned print (HTR/OCR output).
 
 The current pipeline is tuned on (historic) Dutch language, and will not perform well on other languages.
 However, the [underlying model](https://jdmdh.episciences.org/10239) has been used for other (Germanic) languages, and can be adapted and applied to texts of other languages and time periods.
 
 <img src="./qrcode.svg" width=100 height=100>
 
-
 ## Examples
 
 Good quality (not necessarily perfect):
 
 ```
 Van
 Malacca den 29 maart 1.
@@ -45,14 +44,15 @@
 Siac van waar op den 5=e deeser,
 na onse verschijde adhortaties, is over
 eeen gekomen
 zoo meede van Siac
 ```
 
 Bad quality:
+
 ```
 uijtkoops --
 winst suijverevense versis
 e ee
 ,, 19
 1 oe
 na aftrek van
@@ -156,16 +156,16 @@
 (Customize these badges with your own links, and check <https://shields.io/> or <https://badgen.net/> to see which other badges are available.)
 
 | fair-software.eu recommendations | |
 | :-- | :--  |
 | (1/5) code repository              | [![github repo badge](https://img.shields.io/badge/github-repo-000.svg?logo=github&labelColor=gray&color=blue)](https://github.com/laHTeR/htr-quality-classifier) |
 | (2/5) license                      | [![github license badge](https://img.shields.io/github/license/laHTeR/htr-quality-classifier)](https://github.com/laHTeR/htr-quality-classifier) |
 | (3/5) community registry           | [![RSD](https://img.shields.io/badge/rsd-text_quality-00a3e3.svg)](https://research-software-directory.org/projects/lahter) [![workflow pypi badge](https://img.shields.io/pypi/v/text_quality.svg?colorB=blue)](https://pypi.python.org/project/text_quality/) |
-| (4/5) citation                     | [![DOI](https://zenodo.org/badge/DOI/<replace-with-created-DOI>.svg)](https://doi.org/<replace-with-created-DOI>) |
-| (5/5) checklist                    | [![workflow cii badge](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>/badge)](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>) |
+| (4/5) citation                     | [![DOI](https://zenodo.org/badge/617998039.svg)](https://doi.org/10.5281/zenodo.8189893) |
+| (5/5) checklist                    | [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7672/badge)](https://bestpractices.coreinfrastructure.org/projects/7672) |
 | howfairis                          | [![fair-software badge](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu) |
 | **Other best practices**           | &nbsp; |
 | Static analysis                    | [![workflow scq badge](https://sonarcloud.io/api/project_badges/measure?project=LAHTeR_htr-quality-classifier&metric=alert_status)](https://sonarcloud.io/dashboard?id=LAHTeR_htr-quality-classifier) |
 | Coverage                           | [![workflow scc badge](https://sonarcloud.io/api/project_badges/measure?project=LAHTeR_htr-quality-classifier&metric=coverage)](https://sonarcloud.io/dashboard?id=LAHTeR_htr-quality-classifier) |
 | Documentation                      | [![Documentation Status](https://readthedocs.org/projects/htr-quality-classifier/badge/?version=latest)](https://htr-quality-classifier.readthedocs.io/en/latest/?badge=latest) |
 | **GitHub Actions**                 | &nbsp; |
 | Build                              | [![build](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/build.yml/badge.svg)](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/build.yml) |
```

### Comparing `text_quality-0.2.0/README.md` & `text_quality-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 A package to determine the quality of a a digitized text, from a handwritten script or scanned print (HTR/OCR output).
 
 The current pipeline is tuned on (historic) Dutch language, and will not perform well on other languages.
 However, the [underlying model](https://jdmdh.episciences.org/10239) has been used for other (Germanic) languages, and can be adapted and applied to texts of other languages and time periods.
 
 <img src="./qrcode.svg" width=100 height=100>
 
-
 ## Examples
 
 Good quality (not necessarily perfect):
 
 ```
 Van
 Malacca den 29 maart 1.
@@ -20,14 +19,15 @@
 Siac van waar op den 5=e deeser,
 na onse verschijde adhortaties, is over
 eeen gekomen
 zoo meede van Siac
 ```
 
 Bad quality:
+
 ```
 uijtkoops --
 winst suijverevense versis
 e ee
 ,, 19
 1 oe
 na aftrek van
@@ -131,16 +131,16 @@
 (Customize these badges with your own links, and check <https://shields.io/> or <https://badgen.net/> to see which other badges are available.)
 
 | fair-software.eu recommendations | |
 | :-- | :--  |
 | (1/5) code repository              | [![github repo badge](https://img.shields.io/badge/github-repo-000.svg?logo=github&labelColor=gray&color=blue)](https://github.com/laHTeR/htr-quality-classifier) |
 | (2/5) license                      | [![github license badge](https://img.shields.io/github/license/laHTeR/htr-quality-classifier)](https://github.com/laHTeR/htr-quality-classifier) |
 | (3/5) community registry           | [![RSD](https://img.shields.io/badge/rsd-text_quality-00a3e3.svg)](https://research-software-directory.org/projects/lahter) [![workflow pypi badge](https://img.shields.io/pypi/v/text_quality.svg?colorB=blue)](https://pypi.python.org/project/text_quality/) |
-| (4/5) citation                     | [![DOI](https://zenodo.org/badge/DOI/<replace-with-created-DOI>.svg)](https://doi.org/<replace-with-created-DOI>) |
-| (5/5) checklist                    | [![workflow cii badge](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>/badge)](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>) |
+| (4/5) citation                     | [![DOI](https://zenodo.org/badge/617998039.svg)](https://doi.org/10.5281/zenodo.8189893) |
+| (5/5) checklist                    | [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7672/badge)](https://bestpractices.coreinfrastructure.org/projects/7672) |
 | howfairis                          | [![fair-software badge](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu) |
 | **Other best practices**           | &nbsp; |
 | Static analysis                    | [![workflow scq badge](https://sonarcloud.io/api/project_badges/measure?project=LAHTeR_htr-quality-classifier&metric=alert_status)](https://sonarcloud.io/dashboard?id=LAHTeR_htr-quality-classifier) |
 | Coverage                           | [![workflow scc badge](https://sonarcloud.io/api/project_badges/measure?project=LAHTeR_htr-quality-classifier&metric=coverage)](https://sonarcloud.io/dashboard?id=LAHTeR_htr-quality-classifier) |
 | Documentation                      | [![Documentation Status](https://readthedocs.org/projects/htr-quality-classifier/badge/?version=latest)](https://htr-quality-classifier.readthedocs.io/en/latest/?badge=latest) |
 | **GitHub Actions**                 | &nbsp; |
 | Build                              | [![build](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/build.yml/badge.svg)](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/build.yml) |
```

### Comparing `text_quality-0.2.0/scripts/classify_text_quality.py` & `text_quality-0.2.2/scripts/classify_text_quality.py`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/setup.cfg` & `text_quality-0.2.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	ocr
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = text_quality
 project_urls = 
 	Bug Tracker = https://github.com/laHTeR/htr-quality-classifier/issues
 url = https://github.com/laHTeR/htr-quality-classifier
-version = 0.2.0
+version = 0.2.2
 
 [options]
 zip_safe = False
 python_requires = >=3.9
 include_package_data = True
 packages = find:
 install_requires =
```

### Comparing `text_quality-0.2.0/text_quality/classifier/pipeline.py` & `text_quality-0.2.2/text_quality/classifier/pipeline.py`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/data/classifier/pipeline_nn.joblib` & `text_quality-0.2.2/text_quality/data/classifier/pipeline_nn.joblib`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/data/dicts/hunspell/de.aff` & `text_quality-0.2.2/text_quality/data/dicts/hunspell/de.aff`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/data/dicts/hunspell/de.dic` & `text_quality-0.2.2/text_quality/data/dicts/hunspell/de.dic`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/data/dicts/hunspell/fr.aff` & `text_quality-0.2.2/text_quality/data/dicts/hunspell/fr.aff`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/data/dicts/hunspell/fr.dic` & `text_quality-0.2.2/text_quality/data/dicts/hunspell/fr.dic`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/data/dicts/hunspell/nl.aff` & `text_quality-0.2.2/text_quality/data/dicts/hunspell/nl.aff`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/data/dicts/hunspell/nl.dic` & `text_quality-0.2.2/text_quality/data/dicts/hunspell/nl.dic`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/data/dicts/lb.txt` & `text_quality-0.2.2/text_quality/data/dicts/lb.txt`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/data/dicts/nl_voc.txt` & `text_quality-0.2.2/text_quality/data/dicts/nl_voc.txt`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/data/qgrams/nl_voc.txt` & `text_quality-0.2.2/text_quality/data/qgrams/nl_voc.txt`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/feature/featurize.py` & `text_quality-0.2.2/text_quality/feature/featurize.py`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/feature/scorer/dictionary.py` & `text_quality-0.2.2/text_quality/feature/scorer/dictionary.py`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/feature/scorer/garbage.py` & `text_quality-0.2.2/text_quality/feature/scorer/garbage.py`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/feature/scorer/q_gram.py` & `text_quality-0.2.2/text_quality/feature/scorer/q_gram.py`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/feature/tokenizer.py` & `text_quality-0.2.2/text_quality/feature/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/page/page.py` & `text_quality-0.2.2/text_quality/page/page.py`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality/settings.py` & `text_quality-0.2.2/text_quality/settings.py`

 * *Files identical despite different names*

### Comparing `text_quality-0.2.0/text_quality.egg-info/PKG-INFO` & `text_quality-0.2.2/text_quality.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-quality
-Version: 0.2.0
+Version: 0.2.2
 Summary: A package to determine the quality of a a digitized text, from a handwritten script or scanned print (HTR/OCR output).
 Home-page: https://github.com/laHTeR/htr-quality-classifier
 Author: Carsten Schnober
 Author-email: c.schnober@esciencecenter.nl
 Project-URL: Bug Tracker, https://github.com/laHTeR/htr-quality-classifier/issues
 Keywords: htr,ocr
 Classifier: Development Status :: 3 - Alpha
@@ -28,15 +28,14 @@
 A package to determine the quality of a a digitized text, from a handwritten script or scanned print (HTR/OCR output).
 
 The current pipeline is tuned on (historic) Dutch language, and will not perform well on other languages.
 However, the [underlying model](https://jdmdh.episciences.org/10239) has been used for other (Germanic) languages, and can be adapted and applied to texts of other languages and time periods.
 
 <img src="./qrcode.svg" width=100 height=100>
 
-
 ## Examples
 
 Good quality (not necessarily perfect):
 
 ```
 Van
 Malacca den 29 maart 1.
@@ -45,14 +44,15 @@
 Siac van waar op den 5=e deeser,
 na onse verschijde adhortaties, is over
 eeen gekomen
 zoo meede van Siac
 ```
 
 Bad quality:
+
 ```
 uijtkoops --
 winst suijverevense versis
 e ee
 ,, 19
 1 oe
 na aftrek van
@@ -156,16 +156,16 @@
 (Customize these badges with your own links, and check <https://shields.io/> or <https://badgen.net/> to see which other badges are available.)
 
 | fair-software.eu recommendations | |
 | :-- | :--  |
 | (1/5) code repository              | [![github repo badge](https://img.shields.io/badge/github-repo-000.svg?logo=github&labelColor=gray&color=blue)](https://github.com/laHTeR/htr-quality-classifier) |
 | (2/5) license                      | [![github license badge](https://img.shields.io/github/license/laHTeR/htr-quality-classifier)](https://github.com/laHTeR/htr-quality-classifier) |
 | (3/5) community registry           | [![RSD](https://img.shields.io/badge/rsd-text_quality-00a3e3.svg)](https://research-software-directory.org/projects/lahter) [![workflow pypi badge](https://img.shields.io/pypi/v/text_quality.svg?colorB=blue)](https://pypi.python.org/project/text_quality/) |
-| (4/5) citation                     | [![DOI](https://zenodo.org/badge/DOI/<replace-with-created-DOI>.svg)](https://doi.org/<replace-with-created-DOI>) |
-| (5/5) checklist                    | [![workflow cii badge](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>/badge)](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>) |
+| (4/5) citation                     | [![DOI](https://zenodo.org/badge/617998039.svg)](https://doi.org/10.5281/zenodo.8189893) |
+| (5/5) checklist                    | [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7672/badge)](https://bestpractices.coreinfrastructure.org/projects/7672) |
 | howfairis                          | [![fair-software badge](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu) |
 | **Other best practices**           | &nbsp; |
 | Static analysis                    | [![workflow scq badge](https://sonarcloud.io/api/project_badges/measure?project=LAHTeR_htr-quality-classifier&metric=alert_status)](https://sonarcloud.io/dashboard?id=LAHTeR_htr-quality-classifier) |
 | Coverage                           | [![workflow scc badge](https://sonarcloud.io/api/project_badges/measure?project=LAHTeR_htr-quality-classifier&metric=coverage)](https://sonarcloud.io/dashboard?id=LAHTeR_htr-quality-classifier) |
 | Documentation                      | [![Documentation Status](https://readthedocs.org/projects/htr-quality-classifier/badge/?version=latest)](https://htr-quality-classifier.readthedocs.io/en/latest/?badge=latest) |
 | **GitHub Actions**                 | &nbsp; |
 | Build                              | [![build](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/build.yml/badge.svg)](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/build.yml) |
```

### Comparing `text_quality-0.2.0/text_quality.egg-info/SOURCES.txt` & `text_quality-0.2.2/text_quality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

