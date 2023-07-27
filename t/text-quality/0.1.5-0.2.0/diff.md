# Comparing `tmp/text_quality-0.1.5.tar.gz` & `tmp/text_quality-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_quality-0.1.5.tar", last modified: Fri Apr 14 11:17:51 2023, max compression
+gzip compressed data, was "text_quality-0.2.0.tar", last modified: Thu Jul 27 14:16:05 2023, max compression
```

## Comparing `text_quality-0.1.5.tar` & `text_quality-0.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:51.370586 text_quality-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-14 11:17:42.000000 text_quality-0.1.5/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-04-14 11:17:42.000000 text_quality-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25899 2023-04-14 11:17:42.000000 text_quality-0.1.5/LICENSE_NL_OPENTAAL.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-14 11:17:42.000000 text_quality-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 11:17:42.000000 text_quality-0.1.5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-14 11:17:51.370586 text_quality-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-04-14 11:17:42.000000 text_quality-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-14 11:17:42.000000 text_quality-0.1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:51.346586 text_quality-0.1.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-14 11:17:42.000000 text_quality-0.1.5/scripts/classify_text_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-14 11:17:51.370586 text_quality-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 11:17:42.000000 text_quality-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:51.350586 text_quality-0.1.5/text_quality/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:51.350586 text_quality-0.1.5/text_quality/classifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/classifier/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:51.346586 text_quality-0.1.5/text_quality/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:51.350586 text_quality-0.1.5/text_quality/data/classifier/
--rw-r--r--   0 runner    (1001) docker     (123)    31726 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/data/classifier/pipeline_nn.joblib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:51.350586 text_quality-0.1.5/text_quality/data/dicts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:51.354586 text_quality-0.1.5/text_quality/data/dicts/hunspell/
--rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/data/dicts/hunspell/de.aff
--rw-r--r--   0 runner    (1001) docker     (123)  1116164 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/data/dicts/hunspell/de.dic
--rw-r--r--   0 runner    (1001) docker     (123)   201526 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/data/dicts/hunspell/fr.aff
--rw-r--r--   0 runner    (1001) docker     (123)  1222092 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/data/dicts/hunspell/fr.dic
--rw-r--r--   0 runner    (1001) docker     (123)    46575 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/data/dicts/hunspell/nl.aff
--rw-r--r--   0 runner    (1001) docker     (123)  2491328 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/data/dicts/hunspell/nl.dic
--rw-r--r--   0 runner    (1001) docker     (123)  1910341 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/data/dicts/lb.txt
--rw-r--r--   0 runner    (1001) docker     (123)   769888 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/data/dicts/nl_voc.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:51.358586 text_quality-0.1.5/text_quality/data/qgrams/
--rw-r--r--   0 runner    (1001) docker     (123) 11463434 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/data/qgrams/nl_voc.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:51.366586 text_quality-0.1.5/text_quality/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/feature/featurize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:51.370586 text_quality-0.1.5/text_quality/feature/scorer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/feature/scorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/feature/scorer/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/feature/scorer/garbage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/feature/scorer/q_gram.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/feature/scorer/scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/feature/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:51.370586 text_quality-0.1.5/text_quality/page/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/page/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/page/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-14 11:17:42.000000 text_quality-0.1.5/text_quality/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:17:51.350586 text_quality-0.1.5/text_quality.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-14 11:17:51.000000 text_quality-0.1.5/text_quality.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-14 11:17:51.000000 text_quality-0.1.5/text_quality.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:17:51.000000 text_quality-0.1.5/text_quality.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:17:51.000000 text_quality-0.1.5/text_quality.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-14 11:17:51.000000 text_quality-0.1.5/text_quality.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 11:17:51.000000 text_quality-0.1.5/text_quality.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.977377 text_quality-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-27 14:15:57.000000 text_quality-0.2.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-27 14:15:57.000000 text_quality-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25899 2023-07-27 14:15:57.000000 text_quality-0.2.0/LICENSE_NL_OPENTAAL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-27 14:15:57.000000 text_quality-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 14:15:57.000000 text_quality-0.2.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-27 14:16:05.977377 text_quality-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-07-27 14:15:57.000000 text_quality-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-27 14:15:57.000000 text_quality-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.949376 text_quality-0.2.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-27 14:15:57.000000 text_quality-0.2.0/scripts/classify_text_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-27 14:16:05.981377 text_quality-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 14:15:57.000000 text_quality-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.953377 text_quality-0.2.0/text_quality/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.953377 text_quality-0.2.0/text_quality/classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/classifier/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.945376 text_quality-0.2.0/text_quality/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.953377 text_quality-0.2.0/text_quality/data/classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)    31726 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/classifier/pipeline_nn.joblib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.957377 text_quality-0.2.0/text_quality/data/dicts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.961377 text_quality-0.2.0/text_quality/data/dicts/hunspell/
+-rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/hunspell/de.aff
+-rw-r--r--   0 runner    (1001) docker     (123)  1116164 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/hunspell/de.dic
+-rw-r--r--   0 runner    (1001) docker     (123)   201526 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/hunspell/fr.aff
+-rw-r--r--   0 runner    (1001) docker     (123)  1222092 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/hunspell/fr.dic
+-rw-r--r--   0 runner    (1001) docker     (123)    46575 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/hunspell/nl.aff
+-rw-r--r--   0 runner    (1001) docker     (123)  2491328 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/hunspell/nl.dic
+-rw-r--r--   0 runner    (1001) docker     (123)  1910341 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/lb.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   769888 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/dicts/nl_voc.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.965377 text_quality-0.2.0/text_quality/data/qgrams/
+-rw-r--r--   0 runner    (1001) docker     (123) 11463434 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/data/qgrams/nl_voc.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.977377 text_quality-0.2.0/text_quality/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/featurize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.977377 text_quality-0.2.0/text_quality/feature/scorer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/scorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/scorer/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/scorer/garbage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/scorer/q_gram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/scorer/scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/feature/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.977377 text_quality-0.2.0/text_quality/page/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/page/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/page/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-27 14:15:57.000000 text_quality-0.2.0/text_quality/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:05.953377 text_quality-0.2.0/text_quality.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-27 14:16:05.000000 text_quality-0.2.0/text_quality.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-27 14:16:05.000000 text_quality-0.2.0/text_quality.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:16:05.000000 text_quality-0.2.0/text_quality.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:16:05.000000 text_quality-0.2.0/text_quality.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-27 14:16:05.000000 text_quality-0.2.0/text_quality.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-27 14:16:05.000000 text_quality-0.2.0/text_quality.egg-info/top_level.txt
```

### Comparing `text_quality-0.1.5/LICENSE` & `text_quality-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/LICENSE_NL_OPENTAAL.txt` & `text_quality-0.2.0/LICENSE_NL_OPENTAAL.txt`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/PKG-INFO` & `text_quality-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_quality
-Version: 0.1.5
+Version: 0.2.0
 Summary: A package to determine the quality of a a digitized text, from a handwritten script or scanned print (HTR/OCR output).
 Home-page: https://github.com/laHTeR/htr-quality-classifier
 Author: Carsten Schnober
 Author-email: c.schnober@esciencecenter.nl
 Project-URL: Bug Tracker, https://github.com/laHTeR/htr-quality-classifier/issues
 Keywords: htr,ocr
 Classifier: Development Status :: 3 - Alpha
@@ -21,17 +21,59 @@
 Provides-Extra: publishing
 License-File: LICENSE
 License-File: LICENSE_NL_OPENTAAL.txt
 License-File: NOTICE
 
 # Text Quality
 
-This package determines the quality of a (digitized) page in terms of text quality.
+A package to determine the quality of a a digitized text, from a handwritten script or scanned print (HTR/OCR output).
+
+The current pipeline is tuned on (historic) Dutch language, and will not perform well on other languages.
+However, the [underlying model](https://jdmdh.episciences.org/10239) has been used for other (Germanic) languages, and can be adapted and applied to texts of other languages and time periods.
+
+<img src="./qrcode.svg" width=100 height=100>
+
+
+## Examples
+
+Good quality (not necessarily perfect):
+
+```
+Van
+Malacca den 29 maart 1.
+door zoo veel ruijmer handen te hebben,
+[…]
+Siac van waar op den 5=e deeser,
+na onse verschijde adhortaties, is over
+eeen gekomen
+zoo meede van Siac
+```
+
+Bad quality:
+```
+uijtkoops --
+winst suijverevense versis
+e ee
+,, 19
+1 oe
+na aftrek van
+5 p:s C: Commiss:s
+t 1a per 't geheel t p=s lb. off @'t geheeke
+[…]
+```
+
+## What's Missing
+
+- Pipelines for languages other than historic Dutch
+- Automatic training procedure for creating and update pipelines
+- Additional features such as publication year.
 
-## Usage
+See [this notebook](notebooks/quality.ipynb) for a semi-automated pipeline creation process.
+
+## How to use text_quality
 
 After [installation](#installation), use the [classify_text_quality.py](scripts/classify_text_quality.py) script to classify PageXML or plain text files.
 For instance, if you want to classify all `*.xml` files in the `pages/` directory, use the `--glob` argument:
 
 ```shell
 classify_text_quality.py --glob "page/*.xml" --output classifications.csv --output-scores
 ```
@@ -40,67 +82,62 @@
 
 1. Good quality
 2. Medium quality
 3. Bad quality
 
 All supported parameters:
 
-```shell
-classify_text_quality.py --help
+```console
+$ classify_text_quality.py --help
 usage: Classify the quality of a (digitized) text. [-h] [--input [FILE ...]] [--pagexml [FILE ...]] [--pagexml-glob PATTERN] [--output FILE] [--output-scores]
 
 options:
   -h, --help            show this help message and exit
   --output FILE, -o FILE
                         Output file; defaults to stdout.
   --output-scores       Output scores and text statistics.
 
 Input:
   --input [FILE ...], -i [FILE ...]
                         Plain text file(s) to classify. Use '-' for stdin.
   --pagexml [FILE ...]  Input file(s) in PageXML format.
   --pagexml-glob PATTERN, --glob PATTERN
                         A pattern to find a set of PageXML files, e.g. 'pagexml/*.xml'.
-(lahter) carstenschnober@Carstens-MacBook-Pro htr-quality-classifier % 
 ```
 
 ### Notes
 
 The pipeline might emit warnings like this:
 
-```shell
+```console
 UserWarning: X does not have valid feature names, but MLPClassifier was fitted with feature names
 ```
 
 This is due to the internals of the [Scikit-Learn Pipeline object](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html), and can safely be ignored.
 
 The dependencies are pinned to specific versions.
 While this prevents implicit updated even for patch-level updated of required libraries, it prevents misleading warnings emitted by varying Scikit-Learn versions.
 Hence, requirement dependecies can be changed manually, if you are aware of these issues.
 
-## How to use text_quality
-
-A package to determine the quality of a a digitized text, from a handwritten script or scanned print (HTR/OCR output).
-
 The project setup is documented in [project_setup.md](project_setup.md). Feel free to remove this document (and/or the link to this document) if you don't need it.
 
 ## Installation
 
 To install the `text_quality` package:
 
-```console
-pip install text-quality
+```shell
+pip install -U text-quality
 ```
 
 Alternatively, install the package from GitHub repository:
 
-```console
+```shell
 git clone https://github.com/LAHTeR/htr-quality-classifier.git
 cd htr-quality-classifier
-python3 -m pip install .
+python3 -m pip install -U .
 ```
 
 ## Documentation
 
 [Readthedocs](https://htr-quality-classifier.readthedocs.io/en/latest/)
 
 ## Contributing
@@ -123,15 +160,15 @@
 | (1/5) code repository              | [![github repo badge](https://img.shields.io/badge/github-repo-000.svg?logo=github&labelColor=gray&color=blue)](https://github.com/laHTeR/htr-quality-classifier) |
 | (2/5) license                      | [![github license badge](https://img.shields.io/github/license/laHTeR/htr-quality-classifier)](https://github.com/laHTeR/htr-quality-classifier) |
 | (3/5) community registry           | [![RSD](https://img.shields.io/badge/rsd-text_quality-00a3e3.svg)](https://research-software-directory.org/projects/lahter) [![workflow pypi badge](https://img.shields.io/pypi/v/text_quality.svg?colorB=blue)](https://pypi.python.org/project/text_quality/) |
 | (4/5) citation                     | [![DOI](https://zenodo.org/badge/DOI/<replace-with-created-DOI>.svg)](https://doi.org/<replace-with-created-DOI>) |
 | (5/5) checklist                    | [![workflow cii badge](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>/badge)](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>) |
 | howfairis                          | [![fair-software badge](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu) |
 | **Other best practices**           | &nbsp; |
-| Static analysis                    | [![workflow scq badge](https://sonarcloud.io/api/project_badges/measure?project=htr-quality-classifier&metric=alert_status)](https://sonarcloud.io/dashboard?id=htr-quality-classifier) |
-| Coverage                           | [![workflow scc badge](https://sonarcloud.io/api/project_badges/measure?project=laHTeR_htr-quality-classifier&metric=coverage)](https://sonarcloud.io/dashboard?id=laHTeR_htr-quality-classifier) |
+| Static analysis                    | [![workflow scq badge](https://sonarcloud.io/api/project_badges/measure?project=LAHTeR_htr-quality-classifier&metric=alert_status)](https://sonarcloud.io/dashboard?id=LAHTeR_htr-quality-classifier) |
+| Coverage                           | [![workflow scc badge](https://sonarcloud.io/api/project_badges/measure?project=LAHTeR_htr-quality-classifier&metric=coverage)](https://sonarcloud.io/dashboard?id=LAHTeR_htr-quality-classifier) |
 | Documentation                      | [![Documentation Status](https://readthedocs.org/projects/htr-quality-classifier/badge/?version=latest)](https://htr-quality-classifier.readthedocs.io/en/latest/?badge=latest) |
 | **GitHub Actions**                 | &nbsp; |
 | Build                              | [![build](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/build.yml/badge.svg)](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/build.yml) |
 | Citation data consistency               | [![cffconvert](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/cffconvert.yml/badge.svg)](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/cffconvert.yml) |
 | SonarCloud                         | [![sonarcloud](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/sonarcloud.yml/badge.svg)](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/sonarcloud.yml) |
 | MarkDown link checker              | [![markdown-link-check](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/markdown-link-check.yml/badge.svg)](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/markdown-link-check.yml) |
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `text_quality-0.1.5/scripts/classify_text_quality.py` & `text_quality-0.2.0/scripts/classify_text_quality.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,42 +91,43 @@
             garbage_score=GarbageDetector(),
         ),
         tokenizer=tokenizer,
     )
     pipeline = Pipeline.from_file(PIPELINE_FILE, featurizer)
     if pipeline.features != featurizer.features:
         raise RuntimeError(
-            f"Pipline input features ({pipeline.features}) do not match scorers ({featurizer.features})."
+            f"Pipline input features ({pipeline.features})"
+            f"do not match scorers ({featurizer.features})."
         )
 
     text_inputs = {f.name: os.linesep.join(f.readlines()) for f in args.input}
 
     pagexml_inputs = {}
     for pagexml in chain(args.pagexml, glob.glob(args.pagexml_glob)):
         if pagexml in pagexml_inputs:
             logging.warning("Duplicate input file: '%s'", pagexml)
         try:
-            pagexml_inputs[pagexml] = Page.from_file(pagexml).get_text()
+            pagexml_inputs[pagexml] = Page.from_file(pagexml)
         except Exception as e:
             logging.error("Error parsing file '%s': %s", pagexml, str(e))
             pagexml_inputs[pagexml] = ""
 
     fieldnames = list(OutputRow.__annotations__.keys())
     if args.output_scores:
         fieldnames += list(ClassifierScores.__annotations__.keys())
 
     writer = csv.DictWriter(args.output, fieldnames=fieldnames)
     writer.writeheader()
 
-    for name, text in tqdm(
+    for name, page in tqdm(
         (text_inputs | pagexml_inputs).items(), desc="Processing", unit="file"
     ):
         if args.output_scores:
-            quality_class, classifier_scores = pipeline.classify_with_scores(text)
+            quality_class, classifier_scores = pipeline.classify_with_scores(page)
             row = (
                 OutputRow(filename=name, quality_class=quality_class)
                 | classifier_scores
             )
         else:
-            row = OutputRow(filename=name, quality_class=pipeline.classify(text))
+            row = OutputRow(filename=name, quality_class=pipeline.classify(page))
 
         writer.writerow(row)
```

### Comparing `text_quality-0.1.5/setup.cfg` & `text_quality-0.2.0/setup.cfg`

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
-version = 0.1.5
+version = 0.2.0
 
 [options]
 zip_safe = False
 python_requires = >=3.9
 include_package_data = True
 packages = find:
 install_requires =
```

### Comparing `text_quality-0.1.5/text_quality/data/classifier/pipeline_nn.joblib` & `text_quality-0.2.0/text_quality/data/classifier/pipeline_nn.joblib`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/text_quality/data/dicts/hunspell/de.aff` & `text_quality-0.2.0/text_quality/data/dicts/hunspell/de.aff`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/text_quality/data/dicts/hunspell/de.dic` & `text_quality-0.2.0/text_quality/data/dicts/hunspell/de.dic`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/text_quality/data/dicts/hunspell/fr.aff` & `text_quality-0.2.0/text_quality/data/dicts/hunspell/fr.aff`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/text_quality/data/dicts/hunspell/fr.dic` & `text_quality-0.2.0/text_quality/data/dicts/hunspell/fr.dic`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/text_quality/data/dicts/hunspell/nl.aff` & `text_quality-0.2.0/text_quality/data/dicts/hunspell/nl.aff`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/text_quality/data/dicts/hunspell/nl.dic` & `text_quality-0.2.0/text_quality/data/dicts/hunspell/nl.dic`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/text_quality/data/dicts/lb.txt` & `text_quality-0.2.0/text_quality/data/dicts/lb.txt`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/text_quality/data/dicts/nl_voc.txt` & `text_quality-0.2.0/text_quality/data/dicts/nl_voc.txt`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/text_quality/data/qgrams/nl_voc.txt` & `text_quality-0.2.0/text_quality/data/qgrams/nl_voc.txt`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/text_quality/feature/featurize.py` & `text_quality-0.2.0/text_quality/feature/featurize.py`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/text_quality/feature/scorer/dictionary.py` & `text_quality-0.2.0/text_quality/feature/scorer/dictionary.py`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/text_quality/feature/scorer/garbage.py` & `text_quality-0.2.0/text_quality/feature/scorer/garbage.py`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/text_quality/feature/scorer/q_gram.py` & `text_quality-0.2.0/text_quality/feature/scorer/q_gram.py`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/text_quality/feature/tokenizer.py` & `text_quality-0.2.0/text_quality/feature/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text_quality-0.1.5/text_quality/settings.py` & `text_quality-0.2.0/text_quality/settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,23 @@
+"""Global settings."""
+
 import os
 from pathlib import Path
+from typing import Optional
+
+
+MINIMUM_PAGE_LENGTH: int = 5
+"""Shorter texts are considered as empty."""
+
+EMPTY_PAGE_OUTPUT: Optional[int] = 0
+"""Output value for empty pages.
+If None, empty pages are handled through the standard pipeline."""
 
+SHORT_COLUMN_WIDTH: int = 5
+"""If all lines (columns) in a page are shorter than this it is considered broken."""
 
 ENCODING = "utf-8"
 """Encoding to be used throughout all text file processing operations."""
 
 LOG_LEVEL = os.getenv("LOG_LEVEL", "INFO")
 
 LINE_SEPARATOR = os.getenv("LINE_SEPARATOR", "\n")
```

### Comparing `text_quality-0.1.5/text_quality.egg-info/PKG-INFO` & `text_quality-0.2.0/text_quality.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-quality
-Version: 0.1.5
+Version: 0.2.0
 Summary: A package to determine the quality of a a digitized text, from a handwritten script or scanned print (HTR/OCR output).
 Home-page: https://github.com/laHTeR/htr-quality-classifier
 Author: Carsten Schnober
 Author-email: c.schnober@esciencecenter.nl
 Project-URL: Bug Tracker, https://github.com/laHTeR/htr-quality-classifier/issues
 Keywords: htr,ocr
 Classifier: Development Status :: 3 - Alpha
@@ -21,17 +21,59 @@
 Provides-Extra: publishing
 License-File: LICENSE
 License-File: LICENSE_NL_OPENTAAL.txt
 License-File: NOTICE
 
 # Text Quality
 
-This package determines the quality of a (digitized) page in terms of text quality.
+A package to determine the quality of a a digitized text, from a handwritten script or scanned print (HTR/OCR output).
+
+The current pipeline is tuned on (historic) Dutch language, and will not perform well on other languages.
+However, the [underlying model](https://jdmdh.episciences.org/10239) has been used for other (Germanic) languages, and can be adapted and applied to texts of other languages and time periods.
+
+<img src="./qrcode.svg" width=100 height=100>
+
+
+## Examples
+
+Good quality (not necessarily perfect):
+
+```
+Van
+Malacca den 29 maart 1.
+door zoo veel ruijmer handen te hebben,
+[…]
+Siac van waar op den 5=e deeser,
+na onse verschijde adhortaties, is over
+eeen gekomen
+zoo meede van Siac
+```
+
+Bad quality:
+```
+uijtkoops --
+winst suijverevense versis
+e ee
+,, 19
+1 oe
+na aftrek van
+5 p:s C: Commiss:s
+t 1a per 't geheel t p=s lb. off @'t geheeke
+[…]
+```
+
+## What's Missing
+
+- Pipelines for languages other than historic Dutch
+- Automatic training procedure for creating and update pipelines
+- Additional features such as publication year.
 
-## Usage
+See [this notebook](notebooks/quality.ipynb) for a semi-automated pipeline creation process.
+
+## How to use text_quality
 
 After [installation](#installation), use the [classify_text_quality.py](scripts/classify_text_quality.py) script to classify PageXML or plain text files.
 For instance, if you want to classify all `*.xml` files in the `pages/` directory, use the `--glob` argument:
 
 ```shell
 classify_text_quality.py --glob "page/*.xml" --output classifications.csv --output-scores
 ```
@@ -40,67 +82,62 @@
 
 1. Good quality
 2. Medium quality
 3. Bad quality
 
 All supported parameters:
 
-```shell
-classify_text_quality.py --help
+```console
+$ classify_text_quality.py --help
 usage: Classify the quality of a (digitized) text. [-h] [--input [FILE ...]] [--pagexml [FILE ...]] [--pagexml-glob PATTERN] [--output FILE] [--output-scores]
 
 options:
   -h, --help            show this help message and exit
   --output FILE, -o FILE
                         Output file; defaults to stdout.
   --output-scores       Output scores and text statistics.
 
 Input:
   --input [FILE ...], -i [FILE ...]
                         Plain text file(s) to classify. Use '-' for stdin.
   --pagexml [FILE ...]  Input file(s) in PageXML format.
   --pagexml-glob PATTERN, --glob PATTERN
                         A pattern to find a set of PageXML files, e.g. 'pagexml/*.xml'.
-(lahter) carstenschnober@Carstens-MacBook-Pro htr-quality-classifier % 
 ```
 
 ### Notes
 
 The pipeline might emit warnings like this:
 
-```shell
+```console
 UserWarning: X does not have valid feature names, but MLPClassifier was fitted with feature names
 ```
 
 This is due to the internals of the [Scikit-Learn Pipeline object](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html), and can safely be ignored.
 
 The dependencies are pinned to specific versions.
 While this prevents implicit updated even for patch-level updated of required libraries, it prevents misleading warnings emitted by varying Scikit-Learn versions.
 Hence, requirement dependecies can be changed manually, if you are aware of these issues.
 
-## How to use text_quality
-
-A package to determine the quality of a a digitized text, from a handwritten script or scanned print (HTR/OCR output).
-
 The project setup is documented in [project_setup.md](project_setup.md). Feel free to remove this document (and/or the link to this document) if you don't need it.
 
 ## Installation
 
 To install the `text_quality` package:
 
-```console
-pip install text-quality
+```shell
+pip install -U text-quality
 ```
 
 Alternatively, install the package from GitHub repository:
 
-```console
+```shell
 git clone https://github.com/LAHTeR/htr-quality-classifier.git
 cd htr-quality-classifier
-python3 -m pip install .
+python3 -m pip install -U .
 ```
 
 ## Documentation
 
 [Readthedocs](https://htr-quality-classifier.readthedocs.io/en/latest/)
 
 ## Contributing
@@ -123,15 +160,15 @@
 | (1/5) code repository              | [![github repo badge](https://img.shields.io/badge/github-repo-000.svg?logo=github&labelColor=gray&color=blue)](https://github.com/laHTeR/htr-quality-classifier) |
 | (2/5) license                      | [![github license badge](https://img.shields.io/github/license/laHTeR/htr-quality-classifier)](https://github.com/laHTeR/htr-quality-classifier) |
 | (3/5) community registry           | [![RSD](https://img.shields.io/badge/rsd-text_quality-00a3e3.svg)](https://research-software-directory.org/projects/lahter) [![workflow pypi badge](https://img.shields.io/pypi/v/text_quality.svg?colorB=blue)](https://pypi.python.org/project/text_quality/) |
 | (4/5) citation                     | [![DOI](https://zenodo.org/badge/DOI/<replace-with-created-DOI>.svg)](https://doi.org/<replace-with-created-DOI>) |
 | (5/5) checklist                    | [![workflow cii badge](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>/badge)](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>) |
 | howfairis                          | [![fair-software badge](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu) |
 | **Other best practices**           | &nbsp; |
-| Static analysis                    | [![workflow scq badge](https://sonarcloud.io/api/project_badges/measure?project=htr-quality-classifier&metric=alert_status)](https://sonarcloud.io/dashboard?id=htr-quality-classifier) |
-| Coverage                           | [![workflow scc badge](https://sonarcloud.io/api/project_badges/measure?project=laHTeR_htr-quality-classifier&metric=coverage)](https://sonarcloud.io/dashboard?id=laHTeR_htr-quality-classifier) |
+| Static analysis                    | [![workflow scq badge](https://sonarcloud.io/api/project_badges/measure?project=LAHTeR_htr-quality-classifier&metric=alert_status)](https://sonarcloud.io/dashboard?id=LAHTeR_htr-quality-classifier) |
+| Coverage                           | [![workflow scc badge](https://sonarcloud.io/api/project_badges/measure?project=LAHTeR_htr-quality-classifier&metric=coverage)](https://sonarcloud.io/dashboard?id=LAHTeR_htr-quality-classifier) |
 | Documentation                      | [![Documentation Status](https://readthedocs.org/projects/htr-quality-classifier/badge/?version=latest)](https://htr-quality-classifier.readthedocs.io/en/latest/?badge=latest) |
 | **GitHub Actions**                 | &nbsp; |
 | Build                              | [![build](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/build.yml/badge.svg)](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/build.yml) |
 | Citation data consistency               | [![cffconvert](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/cffconvert.yml/badge.svg)](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/cffconvert.yml) |
 | SonarCloud                         | [![sonarcloud](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/sonarcloud.yml/badge.svg)](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/sonarcloud.yml) |
 | MarkDown link checker              | [![markdown-link-check](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/markdown-link-check.yml/badge.svg)](https://github.com/laHTeR/htr-quality-classifier/actions/workflows/markdown-link-check.yml) |
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `text_quality-0.1.5/text_quality.egg-info/SOURCES.txt` & `text_quality-0.2.0/text_quality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

