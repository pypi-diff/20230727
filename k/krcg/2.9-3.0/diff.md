# Comparing `tmp/krcg-2.9.tar.gz` & `tmp/krcg-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/krcg-2.9.tar", last modified: Tue Feb 16 09:35:39 2021, max compression
+gzip compressed data, was "krcg-3.0.tar", last modified: Thu Jul 27 18:44:03 2023, max compression
```

## Comparing `krcg-2.9.tar` & `krcg-3.0.tar`

### file list

```diff
@@ -1,96 +1,103 @@
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.659711 krcg-2.9/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     9567 2021-02-16 09:35:39.000000 krcg-2.9/CHANGELOG.rst
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1073 2021-02-16 09:35:39.000000 krcg-2.9/LICENSE
--rw-r--r--   0 lpanhaleux   (501) staff       (20)      249 2021-02-16 09:35:39.000000 krcg-2.9/MANIFEST.in
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    18607 2021-02-16 09:35:39.659942 krcg-2.9/PKG-INFO
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    14496 2021-02-16 09:35:39.000000 krcg-2.9/README.md
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.639412 krcg-2.9/krcg/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.000000 krcg-2.9/krcg/__init__.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    10992 2021-02-16 09:35:39.000000 krcg-2.9/krcg/analyzer.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    38165 2021-02-16 09:35:39.000000 krcg-2.9/krcg/cards.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    11505 2021-02-16 09:35:39.000000 krcg-2.9/krcg/config.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    15443 2021-02-16 09:35:39.000000 krcg-2.9/krcg/deck.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1735 2021-02-16 09:35:39.000000 krcg-2.9/krcg/logging.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    23805 2021-02-16 09:35:39.000000 krcg-2.9/krcg/parser.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1841 2021-02-16 09:35:39.000000 krcg-2.9/krcg/rulings.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     6067 2021-02-16 09:35:39.000000 krcg-2.9/krcg/sets.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3431 2021-02-16 09:35:39.000000 krcg-2.9/krcg/twda.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     9731 2021-02-16 09:35:39.000000 krcg-2.9/krcg/utils.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2926 2021-02-16 09:35:39.000000 krcg-2.9/krcg/vtes.py
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.659554 krcg-2.9/krcg.egg-info/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2116 2021-02-16 09:35:39.000000 krcg-2.9/krcg.egg-info/SOURCES.txt
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.640780 krcg-2.9/rulings/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.000000 krcg-2.9/rulings/__init__.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)   288493 2021-02-16 09:35:39.000000 krcg-2.9/rulings/cards-rulings.yaml
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    21300 2021-02-16 09:35:39.000000 krcg-2.9/rulings/general-rulings.yaml
--rw-r--r--   0 lpanhaleux   (501) staff       (20)   100957 2021-02-16 09:35:39.000000 krcg-2.9/rulings/rulings-links.yaml
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1247 2021-02-16 09:35:39.660610 krcg-2.9/setup.cfg
--rw-r--r--   0 lpanhaleux   (501) staff       (20)       39 2021-02-16 09:35:39.000000 krcg-2.9/setup.py
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.659329 krcg-2.9/twda_fix/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1906 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2010hunrb.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3219 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2010pwbla1.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1781 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2010pwblaQ.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1727 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2during.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)      998 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2eclastq.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1776 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2gothenburg.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1321 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2gothenburgapr.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1615 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2newyork.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1262 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2orccon2.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1921 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2pariseq.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2615 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2sydney.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1807 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2torrancejan.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1627 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2ukqualifier.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1957 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2watfordapr.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2248 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k2watfordmay.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)      945 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3cadaverous.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2022 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3ec.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1958 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3frenchecq.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2326 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3gothenburgblizzard.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2252 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3helsinki5.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2939 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3italyqualifier.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1921 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3psmilwaukee.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2206 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3rome.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1509 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3sdgothenburg.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1321 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3tcithaca.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1698 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k3winnipegapril.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2091 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k4gks.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1967 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k4littlesister.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1594 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k4norms.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2483 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k4volkerpit.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1611 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k5blackutrecht.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3963 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k5dcqualifier.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2090 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k5dreamboston.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1712 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k5leicesteraug.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1643 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k5ropecon.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1832 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k5valhallajuly.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1337 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k6aussiechamp.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2077 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k6faceaface.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2176 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k6nerq-templecon.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1144 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k6praxispoitiers.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1545 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k6sonarba.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2295 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k7campeonatojuizforano.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2309 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k7comjust.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1209 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k7palmaqual.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3394 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k7woaboston.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1618 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k8sequeenslandcq.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3021 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k8torunminiq.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1682 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/2k9mojlp.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2278 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/Brian.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/__init__.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1324 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/ckgc2k.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3903 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/crusadelisbon2k1.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1775 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/dallas.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1901 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/damnans.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3327 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/darbyla2k1.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1292 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/gothenburg2k1.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2324 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/joshphiladelphia.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2039 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/leedec99.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1430 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/lurequebec2k1.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1753 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/matt-alamut.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1616 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/palma2k1.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1970 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/portoct99.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2706 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/quebec.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2207 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/rob.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2015 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/swkc.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1965 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/theobell2k1.html
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2961 2021-02-16 09:35:39.000000 krcg-2.9/twda_fix/watford-ts.html
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2023-07-27 18:44:03.574808 krcg-3.0/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    13232 2023-07-27 18:44:03.000000 krcg-3.0/CHANGELOG.rst
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1073 2023-07-27 18:44:03.000000 krcg-3.0/LICENSE
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)      261 2023-07-27 18:44:03.000000 krcg-3.0/MANIFEST.in
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    16937 2023-07-27 18:44:03.574897 krcg-3.0/PKG-INFO
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    16110 2023-07-27 18:44:03.000000 krcg-3.0/README.md
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2023-07-27 18:44:03.563917 krcg-3.0/cards/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2023-07-27 18:44:03.000000 krcg-3.0/cards/__init__.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)      484 2023-07-27 18:44:03.000000 krcg-3.0/cards/__main__.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)   350195 2023-07-27 18:44:03.000000 krcg-3.0/cards/vtescrypt.csv
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)   857992 2023-07-27 18:44:03.000000 krcg-3.0/cards/vteslib.csv
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    15503 2023-07-27 18:44:03.000000 krcg-3.0/cards/vteslibmeta.csv
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2330 2023-07-27 18:44:03.000000 krcg-3.0/cards/vtessets.csv
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2023-07-27 18:44:03.565337 krcg-3.0/krcg/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2023-07-27 18:44:03.000000 krcg-3.0/krcg/__init__.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    10994 2023-07-27 18:44:03.000000 krcg-3.0/krcg/analyzer.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    52367 2023-07-27 18:44:03.000000 krcg-3.0/krcg/cards.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    11538 2023-07-27 18:44:03.000000 krcg-3.0/krcg/config.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    19220 2023-07-27 18:44:03.000000 krcg-3.0/krcg/deck.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    26989 2023-07-27 18:44:03.000000 krcg-3.0/krcg/parser.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2657 2023-07-27 18:44:03.000000 krcg-3.0/krcg/rulings.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    22458 2023-07-27 18:44:03.000000 krcg-3.0/krcg/seating.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     6846 2023-07-27 18:44:03.000000 krcg-3.0/krcg/sets.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3266 2023-07-27 18:44:03.000000 krcg-3.0/krcg/twda.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     9735 2023-07-27 18:44:03.000000 krcg-3.0/krcg/utils.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3667 2023-07-27 18:44:03.000000 krcg-3.0/krcg/vtes.py
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2023-07-27 18:44:03.574719 krcg-3.0/krcg.egg-info/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2231 2023-07-27 18:44:03.000000 krcg-3.0/krcg.egg-info/SOURCES.txt
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2023-07-27 18:44:03.565963 krcg-3.0/rulings/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2023-07-27 18:44:03.000000 krcg-3.0/rulings/__init__.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)   344992 2023-07-27 18:44:03.000000 krcg-3.0/rulings/cards-rulings.yaml
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    33499 2023-07-27 18:44:03.000000 krcg-3.0/rulings/general-rulings.yaml
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)   129448 2023-07-27 18:44:03.000000 krcg-3.0/rulings/rulings-links.yaml
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1307 2023-07-27 18:44:03.575421 krcg-3.0/setup.cfg
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)       39 2023-07-27 18:44:03.000000 krcg-3.0/setup.py
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2023-07-27 18:44:03.574563 krcg-3.0/twda_fix/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1906 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2010hunrb.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3219 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2010pwbla1.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1781 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2010pwblaQ.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1727 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k2during.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)      998 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k2eclastq.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1776 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k2gothenburg.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1321 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k2gothenburgapr.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1615 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k2newyork.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1262 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k2orccon2.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1921 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k2pariseq.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2615 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k2sydney.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1807 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k2torrancejan.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1627 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k2ukqualifier.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1957 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k2watfordapr.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2248 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k2watfordmay.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)      945 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k3cadaverous.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2022 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k3ec.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1958 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k3frenchecq.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2326 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k3gothenburgblizzard.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2252 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k3helsinki5.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2939 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k3italyqualifier.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1921 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k3psmilwaukee.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2206 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k3rome.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1509 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k3sdgothenburg.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1321 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k3tcithaca.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1698 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k3winnipegapril.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2091 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k4gks.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1967 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k4littlesister.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1594 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k4norms.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2483 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k4volkerpit.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1611 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k5blackutrecht.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3963 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k5dcqualifier.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2090 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k5dreamboston.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1712 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k5leicesteraug.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1643 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k5ropecon.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1832 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k5valhallajuly.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1337 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k6aussiechamp.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2077 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k6faceaface.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2176 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k6nerq-templecon.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1144 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k6praxispoitiers.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1545 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k6sonarba.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2295 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k7campeonatojuizforano.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2309 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k7comjust.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1209 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k7palmaqual.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3394 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k7woaboston.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1618 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k8sequeenslandcq.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3021 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k8torunminiq.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1682 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/2k9mojlp.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2278 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/Brian.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/__init__.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1324 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/ckgc2k.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3903 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/crusadelisbon2k1.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1775 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/dallas.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1901 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/damnans.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3327 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/darbyla2k1.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1292 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/gothenburg2k1.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2324 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/joshphiladelphia.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2039 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/leedec99.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1430 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/lurequebec2k1.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1753 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/matt-alamut.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1616 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/palma2k1.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1970 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/portoct99.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2706 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/quebec.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2207 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/rob.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2015 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/swkc.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1965 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/theobell2k1.html
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2961 2023-07-27 18:44:03.000000 krcg-3.0/twda_fix/watford-ts.html
```

### Comparing `krcg-2.9/CHANGELOG.rst` & `krcg-3.0/CHANGELOG.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,203 @@
 Changelog
 =========
 
+3.0 (2023-07-27)
+----------------
+
+- **BREAKING CHANGES:**
+    * Add set info for reprints (HttB and KoT)
+    * Seating: Now handles any `Hashable` for players (not just integers).
+      `krcg.seating.get_rounds` now takes a list of `Hashable` instead
+      as input parameter of an integer.
+
+- Migrated depreacted pkg_resources to importlib.resources
+- Shadows of Berlin and Echoes of Gehenna
+
+2.36 (2023-04-17)
+-----------------
+
+- Added 2022 Promo
+
+
+2.35 (2023-02-19)
+-----------------
+
+- Fix cards CSV files parsing to allow
+  partial load of supplementary files (eg. test)
+
+
+2.34 (2023-01-04)
+-----------------
+
+- Fix TWDA parsing for evolutions, eg. Theo Bell (G6)
+
+
+2.33 (2022-11-21)
+-----------------
+
+- Fix Deck.from_url
+
+
+2.32 (2022-11-20)
+-----------------
+
+- Fix VDB links (new format)
+
+
+2.31 (2022-11-16)
+-----------------
+
+- Card: add `ordered_set` to indicate the order of sets by release date
+- Card: add `_set`, the VEKN original value
+- Card: artists order (from VEKN file) is now preserved
+- Technical: improved methods typing
+
+2.30 (2022-11-14)
+-----------------
+
+- Add 2022 European GP Promo
+- Add Fall of London
+
+2.29 (2022-10-04)
+-----------------
+
+- Add Third: Starter Kit precons
+
+
+2.28 (2022-08-25)
+-----------------
+
+- Add variants to crypt cards information (base, advanced, evolution)
+
+
+2.27 (2022-08-24)
+-----------------
+
+- Additional rulings
+
+
+2.26 (2022-08-23)
+-----------------
+
+- Add minimal JSON serialization Deck.to_minimal_json()
+
+
+2.25 (2022-05-21)
+-----------------
+
+- Add New Blood
+- Add the possibility to use KRCG cards files instead of the official VEKN ones
+
+
+2.24 (2022-05-19)
+-----------------
+
+- Ignore cards with a zero count when importing a deck from Amaranth URL
+- Fix corner case on seating computation (player in list but not playing)
+
+2.23 (2022-04-11)
+-----------------
+
+- Update VDB Domain name (now vdb.im)
+
+
+2.22 (2022-04-01)
+-----------------
+
+- Fix TWDA parsing
+- Fix VDB URL parsing
+- Added generic decklist parsing from URL
+
+
+2.21 (2022-01-17)
+-----------------
+
+- Rename Thaumaturgy to Blood Sorcery
+- Improve seating methods
+- Add 2021 SAC Promo set
+- Additional rulings
+
+
+2.20 (2021-12-04)
+-----------------
+
+- Add Banu Haqim and Ministry clans
+  (Assamite and Follower of Set can still be used and are equivalent)
+- Change card name management (and JSON) to cope with vampires "evolutions"
+  from V5 Anarch (same vampire, higher group)
+- Seating: any form of round can now be optimised (4-players table can be anywhere)
+- Seating: now transparantly handles players who don't play all the rounds
+- Deck format: fix LackeyCCG format (quotes in card names)
+- Additional rulings
+
+2.19 (2021-10-12)
+-----------------
+
+- Fix parsing of viz trigram (deck lists parser)
+
+
+2.18 (2021-08-27)
+-----------------
+
+- Additional rulings
+
+
+2.17 (2021-08-22)
+-----------------
+
+- Take VEKN CSV changes into account (sets renamed)
+- Add a diff feature for cards, to compare CSV versions.
+
+
+2.16 (2021-07-22)
+-----------------
+
+- Additional rulings
+- VDB "deck in URL" format for decks
+- Fixed an error when loading a VDB deck
+
+
+2.15 (2021-07-09)
+-----------------
+
+- Fix logging properly: logging is not configured by the lib anymore
+
+
+2.14 (2021-07-08)
+-----------------
+
+- Fix logging issue (quickfix)
+
+
+2.13 (2021-07-08)
+-----------------
+
+- Additional rulings
+- Parser is now FELDB compatible
+
+
+2.12 (2021-04-02)
+-----------------
+
+- Added a seating module to compute optimal seatings for tournaments
+- Additional rulings
+
+2.11 (2021-03-18)
+-----------------
+
+- Fix Talley, The Hound card name
+
+
+2.10 (2021-03-02)
+-----------------
+
+- Fix Lackey format: now handles quotes in names properly
+- Additional rulings
+
 2.9 (2021-02-16)
 ----------------
 
 - Additional rulings
 
 
 2.8 (2021-02-01)
@@ -57,15 +250,15 @@
 - Ensure Python 3.7 compatibility
 
 
 2.0 (2020-12-20)
 ----------------
 
 - BREAKING CHANGES:
-  
+
   * No more pickling, the init phase is new
   * Static files generation is now performed in a separated project: krcg-static
   * Projects using this library (CLI, API, bot, ...) are now in separate repositories
 
 - Use JSON files from static.krcg.org for fast init (see krcg-static)
 - Use VEKN sets CSV to parse and provide clear set information on cards
 - Retrieve a deck list from an Amaranth UID
```

### Comparing `krcg-2.9/LICENSE` & `krcg-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `krcg-2.9/PKG-INFO` & `krcg-3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,439 +1,480 @@
 Metadata-Version: 2.1
 Name: krcg
-Version: 2.9
-Summary: "CLI, web API and Discord bot for VTES cards and TWDA.",
+Version: 3.0
+Summary: CLI, web API and Discord bot for VTES cards and TWDA.
 Home-page: http://github.com/lionel-panhaleux/krcg
 Author: lionelpx
 Author-email: lionel.panhaleux@gmail.com
-License: "MIT"
-Description: # KRCG
-        
-        [![PyPI version](https://badge.fury.io/py/krcg.svg)](https://badge.fury.io/py/krcg)
-        [![Validation](https://github.com/lionel-panhaleux/krcg/workflows/Validation/badge.svg)](https://github.com/lionel-panhaleux/krcg/actions)
-        [![Coverage](https://api.codacy.com/project/badge/Grade/32d1b809494e4935967608f13f52004a)](https://app.codacy.com/manual/lionel-panhaleux/krcg?utm_source=github.com&utm_medium=referral&utm_content=lionel-panhaleux/krcg&utm_campaign=Badge_Grade_Dashboard)
-        [![Python version](https://img.shields.io/badge/python-3.8-blue)](https://www.python.org/downloads/)
-        [![License](https://img.shields.io/badge/License-MIT-blue)](https://opensource.org/licenses/MIT)
-        [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
-        
-        A Python package build to serve as an interface for
-        the VEKN [official card texts](http://www.vekn.net/card-lists)
-        and the [Tournament Winning Deck Archive (TWDA)](http://www.vekn.fr/decks/twd.htm).
-        
-        It also contains an ever-growing list of cards rulings, that is kept up to date
-        thanks to the hard work of our contributors.
-        
-        Portions of the materials are the copyrights and trademarks of Paradox Interactive AB,
-        and are used with permission. All rights reserved.
-        For more information please visit [white-wolf.com](http://www.white-wolf.com).
-        
-        ![Dark Pack](https://raw.githubusercontent.com/lionel-panhaleux/krcg/master/dark-pack.png)
-        
-        ## Offspring projects
-        
-        The KRCG library has been used in multiple _offpsring_ projects:
-        
-        -   [krcg-cli](https://github.com/lionel-panhaleux/krcg-cli) is a convenient
-            Command Line Interface over the library
-        
-        -   [krcg-static](https://github.com/lionel-panhaleux/krcg-static)
-            is used to generate easy-to-use static files for web developers.
-            It is available online at [static.krcg.org](https://static.krcg.org)
-        
-        -   [krcg-api](https://github.com/lionel-panhaleux/krcg-api)
-            is a free RESTful web API exposing to get the most out of the library for web project.
-            It is available online at [v2.api.krcg.org](https://v2.api.krcg.org)
-        
-        -   [krcg-bot](https://github.com/lionel-panhaleux/krcg-bot) is a friendly Discord bot
-            that provides official card text and rulings for free.
-            It is [available for free](https://discordapp.com/oauth2/authorize?client_id=703921850270613505&scope=bot).
-        
-        ## Installation
-        
-        [Python 3](https://www.python.org/downloads/) is required.
-        
-        Use pip to install the `krcg` tool:
-        
-        ```bash
-        pip install krcg
-        ```
-        
-        ## Using the library
-        
-        KRCG is a Python library for VTES.
-        The code is well-documented and can be explored using Python's built-in `help` function.
-        
-        Here are a few quickstart examples to showcase how the library can be used:
-        
-        ### VTES
-        
-        `krcg.vtes.VTES` is the cards library. It needs to be loaded using the `VTES.load()`
-        method. Note that this loads the data from a the very efficient
-        [KRCG static](https://static.krcg.org) server, where it's already available
-        in JSON format for free, for anyone who would want to play with it.
-        
-        Alternatively, you can use `VTES.load_from_vekn()` if you want to load directly
-        from the official [VEKN CSV files](https://www.vekn.net/card-lists),
-        although that's a bit slower. That's actually the way [krcg-static] does it to generate
-        the static JSON files used for the standard load.
-        
-        Then you can play around with VTES to access cards, complete card names or search.
-        
-        ```python
-        >>> from krcg.vtes import VTES
-        >>> VTES.load()
-        >>> VTES["Alastor"].to_json()
-        {
-          'id': 100038,
-          'name': 'Alastor'
-          '_name': 'Alastor',
-          'url': 'https://static.krcg.org/card/alastor.jpg',
-          'types': ['Political Action'],
-          'card_text': (
-            'Requires a justicar or Inner Circle member.\n'
-            'Choose a ready Camarilla vampire. If this referendum is successful, '
-            'search your library for an equipment card and place this card and the equipment '
-            'on the chosen vampire. Pay half the cost (round down) of the equipment. '
-            'This vampire may enter combat with any vampire controlled by another Methuselah '
-            'as a +1 stealth Ⓓ action. This vampire cannot commit diablerie. '
-            'A vampire may have only one Alastor.'),
-          'artists': ['Monte Moore'],
-          'sets': {
-            'Gehenna': [{'release_date': '2004-05-17', 'rarity': 'Rare'}],
-            'Kindred Most Wanted': [{'release_date': '2005-02-21', 'precon': 'Alastors', 'copies': 1}],
-            'Keepers of Tradition': [{'release_date': '2008-11-19', 'rarity': 'Rare'}]},
-         'rulings': {
-           'text': [
-             'If the given weapon costs blood, the target Alastor pays the cost. [LSJ 20040518]',
-              'Requirements do not apply. [ANK 20200901]'
-            ],
-            'links': {
-              '[LSJ 20040518]': 'https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/4emymfUPwAM/B2SCC7L6kuMJ',
-              '[ANK 20200901]': 'http://www.vekn.net/forum/rules-questions/78830-alastor-and-ankara-citadel#100653'
-            }
-          }
-        }
-        >>> VTES.complete("pentex")
-        ['Pentex™ Loves You!',
-         'Pentex™ Subversion',
-         'Enzo Giovanni, Pentex Board of Directors',
-         'Enzo Giovanni, Pentex Board of Directors (ADV)',
-         'Harold Zettler, Pentex Director']
-         >>> VTES.search(type=["political action"], sect=["anarch"], artist=["Drew Tucker"])
-        {<#100790 Free States Rant>}
-        >>> VTES.search(precon=["Fifth Edition: Nosferatu"])
-        {<#201534 Aunt Linda>,
-         <#201536 Baixinho>,
-         <#201537 Belinde>,
-         <#100301 Carrion Crows>,
-         <#100308 Cats' Guidance>,
-         <#102213 Creeping Sabotage>,
-         <#100515 Deep Song>,
-         <#100698 Fame>,
-         <#100863 Guard Dogs>,
-         <#100866 Guardian Angel>,
-         <#100897 Haven Uncovered>,
-         <#201549 Horace Radcliffe>,
-         <#100959 Immortal Grapple>,
-         <#100995 Instinctive Reaction>,
-         <#201553 Larissa Moreira>,
-         <#201555 Lenny Burkhead>,
-         <#101125 Lost in Crowds>,
-         <#101254 Murder of Crows>,
-         <#101321 On the Qui Vive>,
-         <#101483 Preternatural Strength>,
-         <#102214 Protected District>,
-         <#101550 Raven Spy>,
-         <#101564 Rebel>,
-         <#102215 Roundhouse>,
-         <#201568 Ryan>,
-         <#101808 Slum Hunting Ground>,
-         <#101811 Smiling Jack, The Anarch>,
-         <#101945 Taste of Vitae>,
-         <#201545 The Dowager>,
-         <#101070 The Labyrinth>,
-         <#102216 The Warrens>,
-         <#102065 Underbridge Stray>,
-         <#102113 Vessel>,
-         <#102149 Warsaw Station>,
-         <#201573 Wauneka>}
-         >>> VTES.search(set=["Sword of Caine"], rarity=["Rare"])
-        {<#100167 Black Hand Emissary>,
-         <#100314 Census Taker>,
-         <#100360 Cloak of Blood>,
-         <#100589 Drink the Blood of Ahriman>,
-         <#100590 Drop Point Network>,
-         <#100655 Epiphany>,
-         <#100757 Follow the Blood>,
-         <#100787 Framing an Ancient Grudge>,
-         <#100865 Guarded Rubrics>,
-         <#101024 Joseph Pander>,
-         <#101111 Liquefy the Mortal Coil>,
-         <#101161 Mantle of the Bestial Majesty>,
-         <#101446 Praetorian Backer>,
-         <#101489 Prison of the Mind>,
-         <#101658 Ruins of Ceoris>,
-         <#101724 Seraph's Second>,
-         <#102057 The Uncoiling>,
-         <#102022 Tribunal Judgment>,
-         <#102027 Trophy: Chosen>,
-         <#102158 Watchtower: The Wolves Feed>}
-        ```
-        
-        ### TWDA, Analyzer and Deck
-        
-        `krcg.twda.TWDA` is the interface to the TWDA. It needs to be loaded in the same way
-        as the `VTES` instance, using the `TWDA.load()` method. That time, using
-        `TWDA.load_from_vekn()` instead is considerably slower.
-        
-        Once loaded, it can be used to browse the decks in it.
-        
-        ```python
-        >>> from krcg.twda import TWDA
-        >>> TWDA.load()
-        >>> TWDA["2019ecday2pf"]
-        <Deck #2019ecday2pf: Finnish Politics>
-        >>> print(TWDA["2019ecday2pf"].to_txt())
-        EC 2019 - Day 2
-        Paris, France
-        August 18th 2019
-        3R+F
-        50 players
-        Otso Saariluoma
-        
-        -- 2gw8.5 + 1.5vp in the final
-        
-        Deck Name: Finnish Politics
-        
-        Crypt (12 cards, min=4, max=38, avg=5.75)
-        -----------------------------------------
-        4x Anarch Convert     1 -none-                     Caitiff:ANY
-        3x Nana Buruku        8 ANI POT PRE                Guruhi:4
-        2x Nangila Were       9 ANI POT PRE obf ser        Guruhi:4
-        1x Enkidu, The Noah  11 ANI CEL OBF POT PRO for    Gangrel antitribu:4
-        1x Black Annis        9 OBF POT ani pro            Nosferatu antitribu:4
-        1x Andre LeRoux       3 aus                        Toreador:5
-        
-        Library (65 cards)
-        Master (26; 6 trifle)
-        4x Anarch Revolt
-        1x Archon Investigation
-        6x Ashur Tablets
-        1x Dreams of the Sphinx
-        1x Fame
-        1x Giant's Blood
-        1x Information Highway
-        1x Mbare Market, Harare
-        2x Pentex(TM) Subversion
-        1x Powerbase: Luanda
-        1x Powerbase: Montreal
-        5x Villein
-        1x Wider View
-        
-        Action (5)
-        3x Deep Song
-        1x Entrancement
-        1x Well-Marked
-        
-        Retainer (1)
-        1x Mr. Winthrop
-        
-        Reaction (6)
-        1x Cats' Guidance
-        1x Delaying Tactics
-        2x On the Qui Vive
-        2x Sense the Savage Way
-        
-        Combat (26)
-        1x Canine Horde
-        5x Carrion Crows
-        1x Glancing Blow
-        5x Immortal Grapple
-        1x Mighty Grapple
-        1x Slam
-        1x Stunt Cycle
-        4x Taste of Vitae
-        2x Thrown Sewer Lid
-        4x Torn Signpost
-        1x Undead Strength
-        
-        Event (1)
-        1x Dragonbound
-        
-        >>> from datetime import date
-        >>> len([d for d in TWDA.values() if date(2019, 1, 1) < d.date < date(2020, 1, 1) and d.players_count >= 25])
-        27
-        ```
-        
-        The `krcg.analyzer` can provide some statistics over a collection of decks:
-        
-        ```python
-        >>> from krcg.analyzer import Analyzer
-        >>> # You can analyze the whole TWDA, or a fragment of it, or any collection of decks
-        >>> A = Analyzer([d for d in TWDA.values() if date(2019, 1, 1) < d.date < date(2020, 1, 1)])
-        >>> # A blank refresh will provide basic statistics
-        >>> A.refresh()
-        >>> A.played.most_common(5)
-        [(<#100588 Dreams of the Sphinx>, 101),
-         (<#101384 Pentex™ Subversion>, 96),
-         (<#101321 On the Qui Vive>, 86),
-         (<#102121 Villein>, 83),
-         (<#100824 Giant's Blood>, 74)]
-        >>> A.average[VTES["Villein"]]
-        4.409638554216869
-        >>> A.variance[VTES["Villein"]]
-        3.6876179416461032
-        >>> # Refreshing with a list of cards will compute cards affinity using similar decks
-        >>> # similarity=1 tells the engine to select decks that contains all provided cards
-        >>> A.refresh(VTES["Aid from Bats"], similarity=1)
-        >>> # now the candidates method can be used
-        >>> A.candidates(VTES["Aid from Bats"])[:5]
-        [(<#100515 Deep Song>, 1.0000000000000002),
-         (<#100301 Carrion Crows>, 1.0000000000000002),
-         (<#101945 Taste of Vitae>, 0.7777777777777779),
-         (<#200185 Beetleman>, 0.6666666666666667),
-         (<#100698 Fame>, 0.6666666666666667)]
-        ```
-        
-        And finally, the `krcg.deck.Deck` class can be useful to parse and manipulate any deck.
-        
-        ```python
-        >>> from krcg.deck import Deck
-        >>> with open("First_Blood_Nosferatu.txt") as f:
-        >>>     deck = Deck.from_txt(f)
-        >>> deck.crypt
-        [(<#200549 Gustaphe Brunnelle>, 2),
-         (<#200571 Harold Tanner>, 2),
-         (<#200696 Jeremy "Wix" Wyzchovsky>, 2),
-         (<#201116 Petra>, 2),
-         (<#200185 Beetleman>, 2),
-         (<#200190 Benjamin Rose>, 2)]
-        >>> deck.library
-        [(<#100698 Fame>, 2),
-         (<#100070 Animalism>, 2),
-         (<#101015 J. S. Simmons, Esq.>, 1),
-         (<#101070 The Labyrinth>, 1),
-         (<#101073 Laptop Computer>, 2),
-         (<#101125 Lost in Crowds>, 6),
-         (<#100093 Army of Rats>, 2),
-         (<#101550 Raven Spy>, 4),
-         (<#101808 Slum Hunting Ground>, 1),
-         (<#100199 Blood Doll>, 6),
-         (<#100029 Aid from Bats>, 12),
-         (<#100308 Cats' Guidance>, 4),
-         (<#100362 Cloak the Gathering>, 6),
-         (<#100390 Computer Hacking>, 4)]
-        >>> # fetch a deck from Amaranth UID
-        >>> deck = Deck.from_amaranth("4d3aa426-70da-44b7-8cb7-92377a1a0dbd")
-        >>> deck.name
-        'First Blood: Tremere'
-        >>> deck.crypt
-        [(<Card #201020 Muhsin Samir>, 2),
-         (<Card #201213 Rutor>, 2),
-         (<Card #201388 Troius>, 2),
-         (<Card #201501 Zane>, 2),
-         (<Card #200025 Aidan Lyle>, 2),
-         (<Card #200280 Claus Wegener>, 2)]
-        >>> print(deck.to_txt("lackey"))
-        1	Academic Hunting Ground
-        1	Arcane Library
-        4	Blood Doll
-        1	Chantry
-        2	Vast Wealth
-        12	Govern the Unaligned
-        1	Thadius Zho
-        4	.44 Magnum
-        1	Ivory Bow
-        2	Sport Bike
-        1	Charnas the Imp
-        6	Bonding
-        4	Enhanced Senses
-        5	Forced Awakening
-        5	On the Qui Vive
-        4	Precognition
-        4	Spirit's Touch
-        8	Telepathic Misdirection
-        8	Apportation
-        10	Theft of Vitae
-        2	Walk of Flame
-        Crypt:
-        2	Muhsin Samir
-        2	Rutor
-        2	Troius
-        2	Zane
-        2	Aidan Lyle
-        2	Claus Wegener
-        ```
-        
-        ## Contribute
-        
-        Feel free to submit pull requests, they will be merged as long as they pass the tests.
-        Do not hestitate to submit issues or vote on them if you want a feature implemented.
-        
-        ### Design considerations
-        
-        The package uses no database by design.
-        The TWDA, search engine and cards dict are kept in memory for better performances.
-        The whole library generates a memory footprint between 128MB and 256MB.
-        
-        The package uses external data sources for card list, so that it needs not be updated
-        when new sets are released or official VEKN CSV files are changed: it can use
-        new data sets as soon as they're available.
-        
-        ### Contribute Rulings (non-developers)
-        
-        Please do not hestitate to contribute rulings: all help is welcome.
-        
-        Open an [issue](https://github.com/lionel-panhaleux/krcg/issues)
-        with a ruling you think should be added,
-        provide a link to an online post by one of the rules directors:
-        
-        -   From 2016-12-04 onward, [Vincent Ripoll (ANK)](http://www.vekn.net/forum/news-and-announcements/75402-new-inner-circle-vekn-board-of-directors#79470)
-        -   From 2011-07-06 onward, [Pascal Bertrand (PIB)](https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/VzRGZO_Iuto/BjJGRVvJ5Z8J)
-        -   From 1998-06-22 onward, [L. Scott Johnson (LSJ)](https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/RIX1tLgOFjg/xKikfSarfd8J)
-        -   From 1994-12-15 onward, [Thomas R Wylie (TOM)](https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Dm_gIP3YvUs/qTyKyq2NWv4J)
-        
-        ### Contribute Rulings (developers)
-        
-        Feel free to contribute rulings as Pull Requests directly, this is very appreciated.
-        
-        Add the ruling link to
-        [rulings-links.yaml](https://github.com/lionel-panhaleux/krcg/blob/master/rulings/rulings-links.yaml),
-        and the ruling itself to
-        [cards-rulings.yaml](https://github.com/lionel-panhaleux/krcg/blob/master/rulings/cards-rulings.yaml) or
-        [general-rulings.yaml](https://github.com/lionel-panhaleux/krcg/blob/master/rulings/general-rulings.yaml)
-        depending on the case.
-        
-        The format is mostly self-explanatory:
-        
-        -   Cards are reference by ID and name in the format `ID|Name`.
-        
-        -   Card names inside rulings text should be between bracers, eg. `{.44 Magnum}`
-        
-        -   Individual rulings in `cards-rulings.yaml` must provide one or more references
-            to ruling links at the end of the text, between brackets, eg `[LSJ 20100101]`
-        
-        In doing so, please follow the following guidelines:
-        
-        -   Keep the YAML files clean and alphabetically sorted (you can use a YAML formatter)
-        
-        -   Make the rulings as concise as possible
-        
-        -   Prefix the ruling with the discipline level and/or type the ruling applies to (if any),
-            eg. prefix with `[PRO] [COMBAT]` if the ruling applies only to the card played in combat at superior Protean.
-        
-        -   Adapt the ruling wording to the cards it applies to (ie. use masculine/feminin forms)
-        
-        -   You can run the tests with the `pytest` command to check everything is OK
-        
+License: MIT
 Keywords: vampire vtes vekn wod ccg twd
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Games/Entertainment
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# KRCG
+
+[![PyPI version](https://badge.fury.io/py/krcg.svg)](https://badge.fury.io/py/krcg)
+[![Validation](https://github.com/lionel-panhaleux/krcg/workflows/Validation/badge.svg)](https://github.com/lionel-panhaleux/krcg/actions)
+[![Coverage](https://api.codacy.com/project/badge/Grade/32d1b809494e4935967608f13f52004a)](https://app.codacy.com/manual/lionel-panhaleux/krcg?utm_source=github.com&utm_medium=referral&utm_content=lionel-panhaleux/krcg&utm_campaign=Badge_Grade_Dashboard)
+[![Python version](https://img.shields.io/badge/python-3.8-blue)](https://www.python.org/downloads/)
+[![License](https://img.shields.io/badge/License-MIT-blue)](https://opensource.org/licenses/MIT)
+[![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
+
+A Python package build to serve as an interface for
+the VEKN [official card texts](http://www.vekn.net/card-lists)
+and the [Tournament Winning Deck Archive (TWDA)](http://www.vekn.fr/decks/twd.htm).
+
+It also contains an ever-growing list of cards rulings, that is kept up to date
+thanks to the hard work of our contributors.
+
+Portions of the materials are the copyrights and trademarks of Paradox Interactive AB,
+and are used with permission. All rights reserved.
+For more information please visit [white-wolf.com](http://www.white-wolf.com).
+
+![Dark Pack](https://raw.githubusercontent.com/lionel-panhaleux/krcg/master/dark-pack.png)
+
+## Offspring projects
+
+The KRCG library has been used in multiple _offpsring_ projects:
+
+-   [krcg-cli](https://github.com/lionel-panhaleux/krcg-cli) is a convenient
+    Command Line Interface over the library
+
+-   [krcg-static](https://github.com/lionel-panhaleux/krcg-static)
+    is used to generate easy-to-use static files for web developers.
+    It is available online at [static.krcg.org](https://static.krcg.org)
+
+-   [krcg-api](https://github.com/lionel-panhaleux/krcg-api)
+    is a free RESTful web API exposing to get the most out of the library for web project.
+    It is available online at [v2.api.krcg.org](https://v2.api.krcg.org)
+
+-   [krcg-bot](https://github.com/lionel-panhaleux/krcg-bot) is a friendly Discord bot
+    that provides official card text and rulings for free.
+    It is [available for free](https://discordapp.com/oauth2/authorize?client_id=703921850270613505&scope=bot).
+
+## Installation
+
+[Python 3](https://www.python.org/downloads/) is required.
+
+Use pip to install the `krcg` tool:
+
+```bash
+pip install krcg
+```
+
+## Using the library
+
+KRCG is a Python library for VTES.
+The code is well-documented and can be explored using Python's built-in `help` function.
+
+Here are a few quickstart examples to showcase how the library can be used:
+
+### VTES
+
+`krcg.vtes.VTES` is the cards library. It needs to be loaded using the `VTES.load()`
+method. Note that this loads the data from the
+[KRCG static](https://static.krcg.org) server, where it's already available
+in JSON format for free, for anyone who would want to play with it.
+
+Alternatively, you can use `VTES.load_from_vekn()` if you want to load directly
+from the official [VEKN CSV files](https://www.vekn.net/card-lists),
+although that's a bit slower. That's actually the way [krcg-static] does it to generate
+the static JSON files used for the standard load.
+
+Then you can play around with VTES to access cards, complete card names or search.
+
+```python
+>>> from krcg.vtes import VTES
+>>> VTES.load()
+>>> VTES["Alastor"].to_json()
+{
+  'id': 100038,
+  'name': 'Alastor'
+  '_name': 'Alastor',
+  'url': 'https://static.krcg.org/card/alastor.jpg',
+  'types': ['Political Action'],
+  'card_text': (
+    'Requires a justicar or Inner Circle member.\n'
+    'Choose a ready Camarilla vampire. If this referendum is successful, '
+    'search your library for an equipment card and place this card and the equipment '
+    'on the chosen vampire. Pay half the cost (round down) of the equipment. '
+    'This vampire may enter combat with any vampire controlled by another Methuselah '
+    'as a +1 stealth Ⓓ action. This vampire cannot commit diablerie. '
+    'A vampire may have only one Alastor.'),
+  'artists': ['Monte Moore'],
+  'sets': {
+    'Gehenna': [{'release_date': '2004-05-17', 'rarity': 'Rare'}],
+    'Kindred Most Wanted': [{'release_date': '2005-02-21', 'precon': 'Alastors', 'copies': 1}],
+    'Keepers of Tradition': [{'release_date': '2008-11-19', 'rarity': 'Rare'}]},
+ 'rulings': {
+   'text': [
+     'If the given weapon costs blood, the target Alastor pays the cost. [LSJ 20040518]',
+      'Requirements do not apply. [ANK 20200901]'
+    ],
+    'links': {
+      '[LSJ 20040518]': 'https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/4emymfUPwAM/B2SCC7L6kuMJ',
+      '[ANK 20200901]': 'http://www.vekn.net/forum/rules-questions/78830-alastor-and-ankara-citadel#100653'
+    }
+  }
+}
+>>> VTES.complete("pentex")
+['Pentex™ Loves You!',
+ 'Pentex™ Subversion',
+ 'Enzo Giovanni, Pentex Board of Directors',
+ 'Enzo Giovanni, Pentex Board of Directors (ADV)',
+ 'Harold Zettler, Pentex Director']
+ >>> VTES.search(type=["political action"], sect=["anarch"], artist=["Drew Tucker"])
+{<#100790 Free States Rant>}
+>>> VTES.search(precon=["Fifth Edition: Nosferatu"])
+{<#201534 Aunt Linda>,
+ <#201536 Baixinho>,
+ <#201537 Belinde>,
+ <#100301 Carrion Crows>,
+ <#100308 Cats' Guidance>,
+ <#102213 Creeping Sabotage>,
+ <#100515 Deep Song>,
+ <#100698 Fame>,
+ <#100863 Guard Dogs>,
+ <#100866 Guardian Angel>,
+ <#100897 Haven Uncovered>,
+ <#201549 Horace Radcliffe>,
+ <#100959 Immortal Grapple>,
+ <#100995 Instinctive Reaction>,
+ <#201553 Larissa Moreira>,
+ <#201555 Lenny Burkhead>,
+ <#101125 Lost in Crowds>,
+ <#101254 Murder of Crows>,
+ <#101321 On the Qui Vive>,
+ <#101483 Preternatural Strength>,
+ <#102214 Protected District>,
+ <#101550 Raven Spy>,
+ <#101564 Rebel>,
+ <#102215 Roundhouse>,
+ <#201568 Ryan>,
+ <#101808 Slum Hunting Ground>,
+ <#101811 Smiling Jack, The Anarch>,
+ <#101945 Taste of Vitae>,
+ <#201545 The Dowager>,
+ <#101070 The Labyrinth>,
+ <#102216 The Warrens>,
+ <#102065 Underbridge Stray>,
+ <#102113 Vessel>,
+ <#102149 Warsaw Station>,
+ <#201573 Wauneka>}
+ >>> VTES.search(set=["Sword of Caine"], rarity=["Rare"])
+{<#100167 Black Hand Emissary>,
+ <#100314 Census Taker>,
+ <#100360 Cloak of Blood>,
+ <#100589 Drink the Blood of Ahriman>,
+ <#100590 Drop Point Network>,
+ <#100655 Epiphany>,
+ <#100757 Follow the Blood>,
+ <#100787 Framing an Ancient Grudge>,
+ <#100865 Guarded Rubrics>,
+ <#101024 Joseph Pander>,
+ <#101111 Liquefy the Mortal Coil>,
+ <#101161 Mantle of the Bestial Majesty>,
+ <#101446 Praetorian Backer>,
+ <#101489 Prison of the Mind>,
+ <#101658 Ruins of Ceoris>,
+ <#101724 Seraph's Second>,
+ <#102057 The Uncoiling>,
+ <#102022 Tribunal Judgment>,
+ <#102027 Trophy: Chosen>,
+ <#102158 Watchtower: The Wolves Feed>}
+```
+
+### TWDA, Analyzer and Deck
+
+`krcg.twda.TWDA` is the interface to the TWDA. It needs to be loaded in the same way
+as the `VTES` instance, using the `TWDA.load()` method. That time, using
+`TWDA.load_from_vekn()` instead is considerably slower.
+
+Once loaded, it can be used to browse the decks in it.
+
+```python
+>>> from krcg.twda import TWDA
+>>> TWDA.load()
+>>> TWDA["2019ecday2pf"]
+<Deck #2019ecday2pf: Finnish Politics>
+>>> print(TWDA["2019ecday2pf"].to_txt())
+EC 2019 - Day 2
+Paris, France
+August 18th 2019
+3R+F
+50 players
+Otso Saariluoma
+
+-- 2gw8.5 + 1.5vp in the final
+
+Deck Name: Finnish Politics
+
+Crypt (12 cards, min=4, max=38, avg=5.75)
+-----------------------------------------
+4x Anarch Convert     1 -none-                     Caitiff:ANY
+3x Nana Buruku        8 ANI POT PRE                Guruhi:4
+2x Nangila Were       9 ANI POT PRE obf ser        Guruhi:4
+1x Enkidu, The Noah  11 ANI CEL OBF POT PRO for    Gangrel antitribu:4
+1x Black Annis        9 OBF POT ani pro            Nosferatu antitribu:4
+1x Andre LeRoux       3 aus                        Toreador:5
+
+Library (65 cards)
+Master (26; 6 trifle)
+4x Anarch Revolt
+1x Archon Investigation
+6x Ashur Tablets
+1x Dreams of the Sphinx
+1x Fame
+1x Giant's Blood
+1x Information Highway
+1x Mbare Market, Harare
+2x Pentex(TM) Subversion
+1x Powerbase: Luanda
+1x Powerbase: Montreal
+5x Villein
+1x Wider View
+
+Action (5)
+3x Deep Song
+1x Entrancement
+1x Well-Marked
+
+Retainer (1)
+1x Mr. Winthrop
+
+Reaction (6)
+1x Cats' Guidance
+1x Delaying Tactics
+2x On the Qui Vive
+2x Sense the Savage Way
+
+Combat (26)
+1x Canine Horde
+5x Carrion Crows
+1x Glancing Blow
+5x Immortal Grapple
+1x Mighty Grapple
+1x Slam
+1x Stunt Cycle
+4x Taste of Vitae
+2x Thrown Sewer Lid
+4x Torn Signpost
+1x Undead Strength
+
+Event (1)
+1x Dragonbound
+
+>>> from datetime import date
+>>> len([d for d in TWDA.values() if date(2019, 1, 1) < d.date < date(2020, 1, 1) and d.players_count >= 25])
+27
+```
+
+The `krcg.analyzer` can provide some statistics over a collection of decks:
+
+```python
+>>> from krcg.analyzer import Analyzer
+>>> # You can analyze the whole TWDA, or a fragment of it, or any collection of decks
+>>> A = Analyzer([d for d in TWDA.values() if date(2019, 1, 1) < d.date < date(2020, 1, 1)])
+>>> # A blank refresh will provide basic statistics
+>>> A.refresh()
+>>> A.played.most_common(5)
+[(<#100588 Dreams of the Sphinx>, 101),
+ (<#101384 Pentex™ Subversion>, 96),
+ (<#101321 On the Qui Vive>, 86),
+ (<#102121 Villein>, 83),
+ (<#100824 Giant's Blood>, 74)]
+>>> A.average[VTES["Villein"]]
+4.409638554216869
+>>> A.variance[VTES["Villein"]]
+3.6876179416461032
+>>> # Refreshing with a list of cards will compute cards affinity using similar decks
+>>> # similarity=1 tells the engine to select decks that contains all provided cards
+>>> A.refresh(VTES["Aid from Bats"], similarity=1)
+>>> # now the candidates method can be used
+>>> A.candidates(VTES["Aid from Bats"])[:5]
+[(<#100515 Deep Song>, 1.0000000000000002),
+ (<#100301 Carrion Crows>, 1.0000000000000002),
+ (<#101945 Taste of Vitae>, 0.7777777777777779),
+ (<#200185 Beetleman>, 0.6666666666666667),
+ (<#100698 Fame>, 0.6666666666666667)]
+```
+
+The `krcg.seating` module provides functions to compute optimal seatings:
+
+```python
+>>> from krcg import seating
+>>> # permutations gives you the list of players for each round
+>>> seating.permutations(12, 3)
+[[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+ [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+ [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]]
+>>> # things get funny when you have 6, 7 or 11 players: you need more rounds
+>>> # but not all players play every round
+>>> seating.permutations(7, 3)
+[[4, 5, 6, 7],
+ [1, 2, 3, 7],
+ [3, 4, 5, 6],
+ [1, 2, 6, 7],
+ [1, 2, 3, 4, 5]]
+>>> # you can use the Round class to get tables from the permutations
+>>> [seating.Round(p) for p in seating.permutations(14, 3)]
+[[[1, 2, 3, 4, 5], [6, 7, 8, 9, 10], [11, 12, 13, 14]],
+ [[1, 2, 3, 4, 5], [6, 7, 8, 9, 10], [11, 12, 13, 14]],
+ [[1, 2, 3, 4, 5], [6, 7, 8, 9, 10], [11, 12, 13, 14]]]
+>>> # and the optimise function to search for an optimal seating
+>>> result, score = seating.optimise(seating.permutations(12, 3), iterations=50000)
+>>> result
+[[[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12]],
+ [[2, 9, 6, 10], [12, 8, 1, 5], [3, 7, 4, 11]],
+ [[11, 5, 10, 1], [6, 4, 12, 7], [8, 3, 9, 2]]]
+>>> # score.rules gives a score over the nine official rules for optimal seating
+>>> score.rules
+[0, 0, 0.0, 9, 0, 0, 0, 1.118033988749895, 2]
+>>> # you can inspect violations individualy
+>>> # for example rule #4 (players are opponents twice) has 9 violations, to see them:
+>>> score.R4
+[[1, 5], [2, 3], [2, 9], [3, 4], [4, 7], [5, 8], [6, 7], [9, 10], [10, 11]]
+>>> # for more details about the Score structure, check the docstring
+>>> help(seating.Score)
+```
+
+And finally, the `krcg.deck.Deck` class can be useful to parse and manipulate any deck.
+
+```python
+>>> from krcg.deck import Deck
+>>> with open("First_Blood_Nosferatu.txt") as f:
+>>>     deck = Deck.from_txt(f)
+>>> deck.crypt
+[(<#200549 Gustaphe Brunnelle>, 2),
+ (<#200571 Harold Tanner>, 2),
+ (<#200696 Jeremy "Wix" Wyzchovsky>, 2),
+ (<#201116 Petra>, 2),
+ (<#200185 Beetleman>, 2),
+ (<#200190 Benjamin Rose>, 2)]
+>>> deck.library
+[(<#100698 Fame>, 2),
+ (<#100070 Animalism>, 2),
+ (<#101015 J. S. Simmons, Esq.>, 1),
+ (<#101070 The Labyrinth>, 1),
+ (<#101073 Laptop Computer>, 2),
+ (<#101125 Lost in Crowds>, 6),
+ (<#100093 Army of Rats>, 2),
+ (<#101550 Raven Spy>, 4),
+ (<#101808 Slum Hunting Ground>, 1),
+ (<#100199 Blood Doll>, 6),
+ (<#100029 Aid from Bats>, 12),
+ (<#100308 Cats' Guidance>, 4),
+ (<#100362 Cloak the Gathering>, 6),
+ (<#100390 Computer Hacking>, 4)]
+>>> # fetch a deck from Amaranth UID
+>>> deck = Deck.from_amaranth("4d3aa426-70da-44b7-8cb7-92377a1a0dbd")
+>>> deck.name
+'First Blood: Tremere'
+>>> deck.crypt
+[(<Card #201020 Muhsin Samir>, 2),
+ (<Card #201213 Rutor>, 2),
+ (<Card #201388 Troius>, 2),
+ (<Card #201501 Zane>, 2),
+ (<Card #200025 Aidan Lyle>, 2),
+ (<Card #200280 Claus Wegener>, 2)]
+>>> print(deck.to_txt("lackey"))
+1	Academic Hunting Ground
+1	Arcane Library
+4	Blood Doll
+1	Chantry
+2	Vast Wealth
+12	Govern the Unaligned
+1	Thadius Zho
+4	.44 Magnum
+1	Ivory Bow
+2	Sport Bike
+1	Charnas the Imp
+6	Bonding
+4	Enhanced Senses
+5	Forced Awakening
+5	On the Qui Vive
+4	Precognition
+4	Spirit's Touch
+8	Telepathic Misdirection
+8	Apportation
+10	Theft of Vitae
+2	Walk of Flame
+Crypt:
+2	Muhsin Samir
+2	Rutor
+2	Troius
+2	Zane
+2	Aidan Lyle
+2	Claus Wegener
+```
+
+## Contribute
+
+Feel free to submit pull requests, they will be merged as long as they pass the tests.
+Do not hestitate to submit issues or vote on them if you want a feature implemented.
+
+### Design considerations
+
+The package uses no database by design.
+The TWDA, search engine and cards dict are kept in memory for better performances.
+The whole library generates a memory footprint between 128MB and 256MB.
+
+The package uses external data sources for card list, so that it needs not be updated
+when new sets are released or official VEKN CSV files are changed: it can use
+new data sets as soon as they're available.
+
+### Contribute Rulings (non-developers)
+
+Please do not hestitate to contribute rulings: all help is welcome.
+
+Open an [issue](https://github.com/lionel-panhaleux/krcg/issues)
+with a ruling you think should be added,
+provide a link to an online post by one of the rules directors:
+
+-   From 2016-12-04 onward, [Vincent Ripoll (ANK)](http://www.vekn.net/forum/news-and-announcements/75402-new-inner-circle-vekn-board-of-directors#79470)
+-   From 2011-07-06 onward, [Pascal Bertrand (PIB)](https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/VzRGZO_Iuto/BjJGRVvJ5Z8J)
+-   From 1998-06-22 onward, [L. Scott Johnson (LSJ)](https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/RIX1tLgOFjg/xKikfSarfd8J)
+-   From 1994-12-15 onward, [Thomas R Wylie (TOM)](https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Dm_gIP3YvUs/qTyKyq2NWv4J)
+
+### Contribute Rulings (developers)
+
+Feel free to contribute rulings as Pull Requests directly, this is very appreciated.
+
+Add the ruling link to
+[rulings-links.yaml](https://github.com/lionel-panhaleux/krcg/blob/master/rulings/rulings-links.yaml),
+and the ruling itself to
+[cards-rulings.yaml](https://github.com/lionel-panhaleux/krcg/blob/master/rulings/cards-rulings.yaml) or
+[general-rulings.yaml](https://github.com/lionel-panhaleux/krcg/blob/master/rulings/general-rulings.yaml)
+depending on the case.
+
+The format is mostly self-explanatory:
+
+-   Cards are reference by ID and name in the format `ID|Name`.
+
+-   Card names inside rulings text should be between bracers, eg. `{.44 Magnum}`
+
+-   Individual rulings in `cards-rulings.yaml` must provide one or more references
+    to ruling links at the end of the text, between brackets, eg `[LSJ 20100101]`
+
+In doing so, please follow the following guidelines:
+
+-   Keep the YAML files clean and alphabetically sorted (you can use a YAML formatter)
+
+-   Make the rulings as concise as possible
+
+-   Prefix the ruling with the discipline level and/or type the ruling applies to (if any),
+    eg. prefix with `[PRO] [COMBAT]` if the ruling applies only to the card played in combat at superior Protean.
+
+-   Adapt the ruling wording to the cards it applies to (ie. use masculine/feminin forms)
+
+-   You can run the tests with the `pytest` command to check everything is OK
```

### Comparing `krcg-2.9/README.md` & `krcg-3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 The code is well-documented and can be explored using Python's built-in `help` function.
 
 Here are a few quickstart examples to showcase how the library can be used:
 
 ### VTES
 
 `krcg.vtes.VTES` is the cards library. It needs to be loaded using the `VTES.load()`
-method. Note that this loads the data from a the very efficient
+method. Note that this loads the data from the
 [KRCG static](https://static.krcg.org) server, where it's already available
 in JSON format for free, for anyone who would want to play with it.
 
 Alternatively, you can use `VTES.load_from_vekn()` if you want to load directly
 from the official [VEKN CSV files](https://www.vekn.net/card-lists),
 although that's a bit slower. That's actually the way [krcg-static] does it to generate
 the static JSON files used for the standard load.
@@ -282,14 +282,53 @@
 [(<#100515 Deep Song>, 1.0000000000000002),
  (<#100301 Carrion Crows>, 1.0000000000000002),
  (<#101945 Taste of Vitae>, 0.7777777777777779),
  (<#200185 Beetleman>, 0.6666666666666667),
  (<#100698 Fame>, 0.6666666666666667)]
 ```
 
+The `krcg.seating` module provides functions to compute optimal seatings:
+
+```python
+>>> from krcg import seating
+>>> # permutations gives you the list of players for each round
+>>> seating.permutations(12, 3)
+[[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+ [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
+ [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]]
+>>> # things get funny when you have 6, 7 or 11 players: you need more rounds
+>>> # but not all players play every round
+>>> seating.permutations(7, 3)
+[[4, 5, 6, 7],
+ [1, 2, 3, 7],
+ [3, 4, 5, 6],
+ [1, 2, 6, 7],
+ [1, 2, 3, 4, 5]]
+>>> # you can use the Round class to get tables from the permutations
+>>> [seating.Round(p) for p in seating.permutations(14, 3)]
+[[[1, 2, 3, 4, 5], [6, 7, 8, 9, 10], [11, 12, 13, 14]],
+ [[1, 2, 3, 4, 5], [6, 7, 8, 9, 10], [11, 12, 13, 14]],
+ [[1, 2, 3, 4, 5], [6, 7, 8, 9, 10], [11, 12, 13, 14]]]
+>>> # and the optimise function to search for an optimal seating
+>>> result, score = seating.optimise(seating.permutations(12, 3), iterations=50000)
+>>> result
+[[[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12]],
+ [[2, 9, 6, 10], [12, 8, 1, 5], [3, 7, 4, 11]],
+ [[11, 5, 10, 1], [6, 4, 12, 7], [8, 3, 9, 2]]]
+>>> # score.rules gives a score over the nine official rules for optimal seating
+>>> score.rules
+[0, 0, 0.0, 9, 0, 0, 0, 1.118033988749895, 2]
+>>> # you can inspect violations individualy
+>>> # for example rule #4 (players are opponents twice) has 9 violations, to see them:
+>>> score.R4
+[[1, 5], [2, 3], [2, 9], [3, 4], [4, 7], [5, 8], [6, 7], [9, 10], [10, 11]]
+>>> # for more details about the Score structure, check the docstring
+>>> help(seating.Score)
+```
+
 And finally, the `krcg.deck.Deck` class can be useful to parse and manipulate any deck.
 
 ```python
 >>> from krcg.deck import Deck
 >>> with open("First_Blood_Nosferatu.txt") as f:
 >>>     deck = Deck.from_txt(f)
 >>> deck.crypt
```

### Comparing `krcg-2.9/krcg/analyzer.py` & `krcg-3.0/krcg/analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 """
 from typing import Callable, Iterable, List, Tuple
 import collections
 import itertools
 import random
 
 from . import deck
-from . import logging
+import logging
 
 Candidates = List[Tuple[str, float]]
 
-logger = logging.logger
+logger = logging.getLogger("krcg")
 
 
 class AnalysisError(Exception):
     pass
 
 
 class Analyzer(object):
@@ -38,15 +38,15 @@
             self.spoilers = {
                 name: count / len(self.decks)
                 for name, count in collections.Counter(
                     itertools.chain.from_iterable(d.keys() for d in self.decks)
                 ).items()
                 if count > len(self.decks) / 4
             }
-            logger.debug("Spoilers: {}", self.spoilers)
+            logger.debug("Spoilers: %s", self.spoilers)
         else:
             self.spoilers = {}
         self.examples = None
         self.played = None
         self.average = None
         self.variance = None
         self.affinity = None
@@ -73,15 +73,15 @@
         # but do not pick a spoiler (card played in more than 25% decks).
         if not args:
             args = [
                 [c for c, _ in self.played.most_common() if c not in self.spoilers][
                     random.randrange(100)
                 ]
             ]
-            logger.info("Randomly selected {}", args[0])
+            logger.info("Randomly selected %s", args[0])
         # build crypt first, then library
         self.build_deck_part(*args, condition=Analyzer.is_crypt)
         self.refresh(condition=Analyzer.is_library)
         self.build_deck_part(condition=Analyzer.is_library)
         # add example decks reference in description
         self.deck.comments = "Inspired by:\n" + "\n".join(
             f" - {example.id:<20} {example.name or '(No Name)'}"
@@ -159,15 +159,15 @@
                 >= similarity
             ]
         else:
             self.examples = self.decks
         if not self.examples:
             logger.error("No example in TWDA")
             raise AnalysisError()
-        logger.info("Refresh examples ({})", len(self.examples))
+        logger.info("Refresh examples (%s)", len(self.examples))
         self.played = collections.Counter()
         for example in self.examples:
             self.played.update(card for card, _ in example.cards(condition))
         self.affinity = collections.defaultdict(collections.Counter)
         for card in reference:
             self.refresh_affinity(card, condition)
         # compute average number played for each card
@@ -274,12 +274,12 @@
                     break
             # score candidates by affinity
             candidates = self.candidates(*(self.deck.keys() or args))
             if not candidates:
                 logger.info("No more candidates")
                 return
             next_card, score = candidates[0]
-            logger.info("Selected {} ({:.2f})", next_card, score)
+            logger.info("Selected %s (%.2f)", next_card, score)
             count = min(self.cards_left, round(self.average[next_card]))
             self.deck.update({next_card: count})
             self.cards_left -= count
             self.refresh_affinity(next_card, condition)
```

### Comparing `krcg-2.9/krcg/cards.py` & `krcg-3.0/krcg/cards.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,44 @@
-from typing import Dict, List, Set, Tuple
+from typing import Counter, Dict, Generator, List, Set, Tuple
 import collections
 import collections.abc
 import copy
+import csv
 import datetime
 import functools
+import importlib.resources
+import io
 import itertools
+import os
 import re
 import requests
 import urllib.request
 import warnings
 
 from . import config
 from . import rulings
 from . import sets
 from . import utils
 
 
+LOCAL_CARDS = os.getenv("LOCAL_CARDS")
+
+
 class Card(utils.i18nMixin, utils.NamedMixin):
     #: official cards renaming not registered in cards "Aka" field
     _AKA = {
-        "Mask of a Thousand Faces": ["mask of 1,000 faces"],
+        101179: ["mask of 1,000 faces"],
+    }
+    #: VEKN CSV uses old clan names for retro-compatibility
+    _CLAN_RENAMES = {
+        "Assamite": "Banu Haqim",
+        "Follower of Set": "Ministry",
+    }
+    _DISC_RENAMES = {
+        "Thaumaturgy": "Blood Sorcery",
     }
     #: Actual ban dates
     _BAN_MAP = {
         "1995": datetime.date(1995, 11, 1),  # RTR 19951006
         "1997": datetime.date(1997, 7, 1),  # RTR 19970701
         "1999": datetime.date(1999, 4, 1),  # RTR 19990324
         "2005": datetime.date(2005, 1, 1),  # RTR 20041205
@@ -35,15 +50,15 @@
     _DISC_MAP = {
         # special case for vampires with no discipline (eg. Anarch Convert)
         "-none-": None,
         # these are not disciplines but treat them that way
         "striga": "striga",
         "maleficia": "maleficia",
         "flight": "flight",
-        "vision": "vin",  # avoid coollision with visceratika
+        "vision": "vin",  # avoid collision with visceratika
         # standard list
         "judgment": "jud",
         "innocence": "inn",
         "martyrdom": "mar",
         "defense": "def",
         "redemption": "red",
         "vengeance": "ven",
@@ -169,40 +184,64 @@
             "PM": "Malkavian antitribu",
         },
         "Third": {
             "PTr": "Tremere antitribu",
             "PB": "Brujah antitribu",
             "PM": "Malkavian antitribu",
             "PTz": "Tzimisce",
+            "SKB": "Starter Kit Brujah antitribu",
+            "SKM": "Starter Kit Malkavian antitribu",
+            "SKTr": "Starter Kit Tremere antitribu",
+            "SKTz": "Starter Kit Tzimisce",
         },
         "Tenth": {"A": "Tin A", "B": "Tin B"},
         "Anthology": {"LARP": "EC Berlin Edition"},
         "BSC": {"X": ""},
         "POD": {
             "DTC": "DriveThruCards",
         },
         "Promo-20181004": {"HB": "Humble Bundle"},
+        "TU": {
+            "A": "Bundle 1",
+            "B": "Bundle 2",
+        },
+        "V5A": {
+            "PB": "Brujah",
+            "PMin": "Ministry",
+            "PBh": "Banu Haqim",
+            "PG": "Gangrel",
+        },
+        "NB": {
+            "PM": "Malkavian",
+            "PN": "Nosferatu",
+            "PTo": "Toreador",
+            "PTr": "Tremere",
+            "PV": "Ventrue",
+        },
     }
     _REPRINTS_RELEASE_DATE = {
         ("KoT", "Reprint Bundle 1"): datetime.date(2018, 5, 5),
         ("KoT", "Reprint Bundle 2"): datetime.date(2018, 5, 5),
         ("HttB", "Reprint Bundle 1"): datetime.date(2018, 7, 14),
         ("HttB", "Reprint Bundle 2"): datetime.date(2018, 7, 14),
+        ("TU", "Bundle 1"): datetime.date(2021, 7, 9),
+        ("TU", "Bundle 2"): datetime.date(2021, 7, 9),
     }
     _ARTISTS_FIXES = {
         "Alejandro Collucci": "Alejandro Colucci",
         "Chet Masterz": "Chet Masters",
         "Dimple": 'Nicolas "Dimple" Bigot',
         "EM Gist": "E.M. Gist",
         "G. Goleash": "Grant Goleash",
         "Ginés Quiñonero": "Ginés Quiñonero-Santiago",
         "Glenn Osterberger": "Glen Osterberger",
         "Heather Kreiter": "Heather V. Kreiter",
         "Jeff Holt": 'Jeff "el jefe" Holt',
         "L. Snelly": "Lawrence Snelly",
+        "Martín de Diego Sábada": "Martín de Diego",
         "Mathias Tapia": "Matias Tapia",
         "Mattias Tapia": "Matias Tapia",
         "Matt Mitchell": "Matthew Mitchell",
         "Mike Gaydos": "Michael Gaydos",
         "Mike Weaver": "Michael Weaver",
         "Nicolas Bigot": 'Nicolas "Dimple" Bigot',
         "Pat McEvoy": "Patrick McEvoy",
@@ -225,51 +264,149 @@
         self.clans = []
         self.capacity = None
         self.capacity_change = None
         self.disciplines = []
         self.combo = None
         self.multidisc = None
         self.card_text = ""
+        # original VEKN value: use `sets` instead for more accessible info
+        self._set = ""
         self.sets = {}
         self.scans = {}
         self.banned = None
         self.artists = []
         self.adv = None
         self.group = None
         self.title = None
         self.pool_cost = None
         self.blood_cost = None
         self.conviction_cost = None
         self.burn_option = None
         self.flavor_text = None
         self.draft = None
+        # enriched properties (not directly in original CSV, but convenient)
+        self.ordered_sets = []  # sets in release order
+        self.has_advanced = None  # same vampire appears as advanced in the same group
+        self.has_evolution = None  # same vampire appears in a higher group
+        self.is_evolution = None  # same vampire appears in a lower group
+        self.variants = {}  # variants of the same vampire (base, adv, evolution)
+        self.name_variants = []  # variations you want to match when parsing a decklist
         self.rulings = {"text": [], "links": {}}
 
+    def diff(self, rhs) -> Dict[str, Tuple[str, str]]:
+        res = {}
+        if self.name != rhs.name:
+            res["name"] = [self.name, rhs.name]
+        if self.card_text != rhs.card_text:
+            res["card_text"] = [self.card_text, rhs.card_text]
+        if set(self.types) != set(rhs.types):
+            res["types"] = [self.types, rhs.types]
+        if set(self.clans) != set(rhs.clans):
+            res["clans"] = [self.clans, rhs.clans]
+        if set(self.disciplines) - {"viz", "vin"} != set(rhs.disciplines) - {
+            "viz",
+            "vin",
+        }:
+            res["disciplines"] = [self.disciplines, rhs.disciplines]
+        if (self.capacity or 0) != (rhs.capacity or 0):
+            res["capacity"] = [self.capacity, rhs.capacity]
+        if bool(self.adv) != bool(rhs.adv):
+            res["adv"] = [self.adv, rhs.adv]
+        if bool(self.banned) != bool(rhs.banned):
+            res["banned"] = [self.banned, rhs.banned]
+        if self.group != rhs.group:
+            res["group"] = [self.group, rhs.group]
+        if self.pool_cost != rhs.pool_cost:
+            res["pool_cost"] = [self.pool_cost, rhs.pool_cost]
+        if self.blood_cost != rhs.blood_cost:
+            res["blood_cost"] = [self.blood_cost, rhs.blood_cost]
+        if self.conviction_cost != rhs.conviction_cost:
+            res["conviction_cost"] = [self.conviction_cost, rhs.conviction_cost]
+        if bool(self.burn_option) != bool(rhs.burn_option):
+            res["burn_option"] = [self.burn_option, rhs.burn_option]
+        if (self.flavor_text or "") != (rhs.flavor_text or ""):
+            res["flavor_text"] = [self.flavor_text, rhs.flavor_text]
+        return res
+
     @property
     @functools.lru_cache(1)
     def vekn_name(self) -> str:
         """VEKN names as used in legacy decklists tools."""
         assert self.id, "Card is not initialized"
         ret = self._name
-        if self.adv:
-            ret += " (ADV)"
+        suffix = self.get_suffix(minimal=True)
+        if suffix:
+            ret += f" ({suffix})"
+        return ret
+
+    @property
+    @functools.lru_cache(1)
+    def web_name(self) -> str:
+        """Name used for filenames on web applications."""
+        assert self.id, "Card is not initialized"
+        ret = self._name
+        suffix = self.get_suffix()
+        if suffix:
+            ret += f" ({suffix})"
+        return ret
+
+    @property
+    @functools.lru_cache(1)
+    def usual_name(self) -> str:
+        """Unique name, as printed plus minimal suffix for unicity."""
+        assert self.id, "Card is not initialized"
+        ret = self.printed_name
+        suffix = self.get_suffix(minimal=True)
+        if suffix:
+            ret += f" ({suffix})"
         return ret
 
     @property
     @functools.lru_cache(1)
     def name(self) -> str:
+        """Unique name for the card."""
+        ret = self.printed_name
+        suffix = self.get_suffix()
+        if suffix:
+            ret += f" ({suffix})"
+        return ret
+
+    @property
+    @functools.lru_cache(1)
+    def printed_name(self) -> str:
         """Actual real name printed on the card."""
         assert self.id, "Card is not initialized"
         ret = self._name
         if ret[-5:] == ", The":
             ret = "The " + ret[:-5]
-        ret = ret.replace("(TM)", "™")
+        return ret.replace("(TM)", "™")
+
+    @property
+    @functools.lru_cache(1)
+    def _key(self) -> str:
+        """Used internally for advanced / evolutions / variants computations"""
+        if self.group == "ANY":
+            key = "ANY"
+        else:
+            key = f"G{self.group}"
         if self.adv:
-            ret += " (ADV)"
-        return ret
+            key += " ADV"
+        return key
+
+    def get_suffix(self, minimal=False) -> str:
+        suffixes = []
+        if self.group and (self.is_evolution or not minimal):
+            if self.group == "ANY":
+                prefix = ""
+            else:
+                prefix = "G"
+            suffixes.append(f"{prefix}{self.group}")
+        if self.adv:
+            suffixes.append("ADV")
+        return " ".join(suffixes)
 
     @property
     @functools.lru_cache(1)
     def crypt(self) -> bool:
         """True if this is a crypt card."""
         return set(self.types) & {"Imbued", "Vampire"}
 
@@ -279,161 +416,232 @@
         return not self.crypt
 
     def to_json(self) -> Dict:
         """Return a compact dict representation of the card, for JSON serialization."""
         return utils.json_pack(
             {
                 k: v
-                for k, v in list(self.__dict__.items()) + [("name", self.name)]
+                for k, v in list(self.__dict__.items())
+                # add usual names for convenience
+                + [("name", self.name), ("printed_name", self.printed_name)]
                 if k not in ["crypt", "library", "vekn_name"]
             }
         )
 
     def from_json(self, state: Dict) -> None:
         """Get the card form a dict."""
+        # remove convenience names to avoid overriding the properties
+        state.pop("name", None)
+        state.pop("printed_name", None)
         self.__dict__.update(state)
 
     def from_vekn(
-        self, data: Dict[str, str], set_dict: Dict[str, sets.Set] = sets.DEFAULT_SET_MAP
+        self,
+        data: Dict[str, str],
+        set_dict: Dict[str, sets.Set] = sets.DEFAULT_SET_MAP,
+        default_set: str = None,
     ) -> None:
         """Read a card from a dict generated from a VEKN official CSV.
 
         Args:
             set_dict: A map of the sets, indexed by abbreviation
             data: Dict of the CSV line
         """
 
         def split(field, sep):
-            return [s for s in map(str.strip, data[field].split(sep)) if s]
+            return [s for s in map(str.strip, data.get(field, "").split(sep)) if s]
 
         def str_or_none(field):
-            return data[field] or None if field in data else None
+            return data[field].replace("@", "") or None if field in data else None
 
         def bool_or_none(field):
             return bool(data[field]) if field in data else None
 
         def int_or_none(field):
             try:
                 return int(data[field]) if data.get(field) else None
             except ValueError:
                 warnings.warn(f"expected an integer for {field}: {data}")
 
         self.id = int(data["Id"])
         self._name = data["Name"]
+        self._set = str_or_none("Set") or default_set
         self.aka = split("Aka", ";")
-        self.types = split("Type", "/")
-        self.clans = split("Clan", "/")
+        self.types = [a.replace("@", "") for a in split("Type", "/")]
+        self.clans = [a.replace("@", "") for a in split("Clan", "/")]
+        for i in range(len(self.clans)):
+            if self.clans[i] in self._CLAN_RENAMES:
+                self.clans[i] = self._CLAN_RENAMES[self.clans[i]]
         capacity = data.get("Capacity")
         if capacity and re.search(r"^[^\d]", capacity):
             self.capacity_change = capacity
         else:
             self.capacity = int_or_none("Capacity")
         # disciplines
         discipline_key = "Discipline" if "Discipline" in data else "Disciplines"
         if "/" in data[discipline_key]:
             self.multidisc = True
         if "&" in data[discipline_key]:
             self.combo = True
         for s in re.split(r"[\s/&]+", data[discipline_key]):
+            s = s.replace("@", "")
             # distinguish vision (vin) from visceratika (vis)
             if s.lower() == "vis" and "Imbued" in self.types:
                 s = "vin"
             s = Card._DISC_MAP.get(s.lower(), s)
             if s:
                 self.disciplines.append(s)
         # braces have been used in the CSV to denote last card text change
         self.card_text = (
-            data["Card Text"].replace("(D)", "Ⓓ").replace("{", "").replace("}", "")
+            data["Card Text"]
+            .replace("(D)", "Ⓓ")
+            .replace("{", "")
+            .replace("}", "")
+            .replace("@", "")
         )
+        if "{" in data["Card Text"]:
+            self.text_change = True
+        else:
+            self.text_change = False
+        for old_name, new_name in self._CLAN_RENAMES.items():
+            self.card_text = self.card_text.replace(old_name, new_name)
+        for old_name, new_name in self._DISC_RENAMES.items():
+            self.card_text = self.card_text.replace(old_name, new_name)
         self.banned = (
-            self._BAN_MAP[data["Banned"]].isoformat() if data["Banned"] else None
+            self._BAN_MAP[data["Banned"]].isoformat() if data.get("Banned") else None
         )
-        self.artists = sorted(  # some cards have duplicated artists, eg. Ashur Tablets
-            set(
+        # remove potential duplicated artists (eg. Ashur Tablets)
+        # collections.Counter to keep the order (ordered dict with convenient init)
+        self.artists = list(
+            collections.Counter(
                 self._ARTISTS_FIXES.get(s, s)
-                for s in map(str.strip, re.split(r"[;,&]+(?!\sJr\.)", data["Artist"]))
+                for s in map(
+                    str.strip, re.split(r"[;,&]+(?!\sJr\.)", data.get("Artist", ""))
+                )
                 if s
-            )
+            ).keys()
         )
         self.adv = bool_or_none("Adv")
         # group can be "any"
         self.group = str_or_none("Group")
         self.title = str_or_none("Title")
         if self.title and self.title[0] not in ["1", "2", "3", "4", "5"]:
             self.title = self.title.title()
         self.pool_cost = str_or_none("Pool Cost")  # can be X
         self.blood_cost = str_or_none("Blood Cost")  # can be X
         self.conviction_cost = str_or_none("Conviction Cost")  # str for consistency
         self.burn_option = bool_or_none("Burn Option")
         self.flavor_text = data["Flavor Text"] if "Flavor Text" in data else None
         self.draft = data["Draft"] if "Draft" in data else None
+
         # computations last: some properties (ie. name) are cached,
         # only use them once everything else is set
         self.sets = dict(
-            Card._decode_set(set_dict, rarity)
-            for rarity in map(str.strip, data["Set"].split(","))
-            if rarity
+            itertools.chain.from_iterable(
+                Card._decode_set(set_dict, rarity)
+                for rarity in map(
+                    str.strip,
+                    itertools.chain.from_iterable(
+                        s.split(";")
+                        for s in data.get("Set", default_set).split(",")
+                        if s
+                    ),
+                )
+                if rarity
+            )
         )
-        if not self.sets:
+        if self.sets:
+            self.ordered_sets = sorted(
+                [s for s in self.sets.keys() if set_dict[s].release_date],
+                key=lambda x: set_dict[x].release_date,
+            )
+        else:
             warnings.warn(f"no set found for {self}")
+        # some cards have one set, no date, eg. playtest cards
+        if self.sets and not self.ordered_sets:
+            self.ordered_sets = list(self.sets.keys())
         self.scans = {
             name: self._compute_url(
                 expansion=(
                     {
                         "2019 Promo Pack 1": "promo-pack-1",
+                        "2020 Promo Pack 2": "promo-pack-2",
+                        "2021 Kickstarter Promo": "kickstarter-promo",
                         "2018 Humble Bundle": "humble-bundle",
                     }.get(name, "promo")
                     if set_dict[name].abbrev in set(sets.SetMap.PROMOS)
-                    else name.lower().replace(":", "").replace(" ", "-")
+                    else name.lower()
+                    .replace(":", "")
+                    .replace(" ", "-")
+                    .replace("(", "")
+                    .replace(")", "")
                 )
             )
             for name in self.sets.keys()
         }
         self.url = self._compute_url()
 
-    def _compute_url(self, lang: str = None, expansion: str = None):
+    def _compute_url(self, lang: str = None, expansion: str = None) -> str:
         """Compute image URL for given language."""
         return (
             config.KRCG_STATIC_SERVER
             + "/card/"
             + (f"set/{expansion}/" if expansion else "")
             + (f"{lang[:2]}/" if lang else "")
+            + re.sub(r"[^\w\d]", "", utils.normalize(self.web_name))
+            + ".jpg"
+        )
+
+    def _compute_legacy_url(self, lang: str = None, expansion: str = None) -> str:
+        """Compute legacy image URL for given language."""
+        return (
+            config.KRCG_STATIC_SERVER
+            + "/card/"
+            + (f"set/{expansion}/" if expansion else "")
+            + (f"{lang[:2]}/" if lang else "")
             + re.sub(r"[^\w\d]", "", utils.normalize(self.vekn_name))
             + ".jpg"
         )
 
     @staticmethod
     def _decode_set(
         set_dict: Dict[str, sets.Set], expansion: str
-    ) -> Tuple[str, List[Dict]]:
+    ) -> Generator[None, None, Tuple[str, List[Dict]]]:
         """Decode a set string from official CSV.
 
         From Jyhad:R2 to {"Jyhad": {"rarity": "Rare", "frequency": 2}}
         """
         match = re.match(
             r"^(?P<abbrev>[a-zA-Z0-9-]+):?(?P<rarity>[a-zA-Z0-9/½]+)?$",
             expansion,
         )
         if not match:
             warnings.warn(f"failed to parse set: {expansion}")
-            return expansion, []
+            yield expansion, []
         match = match.groupdict()
         abbrev = match["abbrev"]
         try:
             date = set_dict[abbrev].release_date
         except KeyError:
             warnings.warn(f"unknown set: {abbrev}")
             date = None
         rarities = (match["rarity"] or "").split("/")
         ret = [
             r
             for r in map(lambda a: Card._decode_rarity(a, abbrev, date), rarities)
             if r
         ]
-        return set_dict[abbrev].name, ret
+        reprints, ret = Card._partition(
+            ret, lambda r: r.get("precon", "").startswith("Reprint ")
+        )
+        for r in reprints:
+            r["precon"] = r["precon"][8:]
+        if reprints:
+            yield (set_dict[abbrev].name + " Reprint", reprints)
+        yield (set_dict[abbrev].name, ret)
 
     @staticmethod
     def _decode_rarity(rarity: str, abbrev: str, date: str) -> dict:
         """Decode the rarity tag after expansion abbreviation."""
         match = re.match(
             r"^(?P<base>[a-zA-Z]+)?(?P<count>[0-9½]+)?$",
             rarity,
@@ -450,16 +658,18 @@
         code = Card._RARITY_BOOSTER_CODES.get(base)
         if code:
             ret["rarity"] = code
         else:
             code = Card._RARITY_PRECON_CODES.get(abbrev, {}).get(base)
             if code:
                 ret["precon"] = code
-            elif code is None:
-                warnings.warn(f"unknown base: {base} in {rarity}")
+            elif code is None and abbrev[:5] != "Promo":
+                # promo "origins" can be there, but it's largely inconsistent
+                # eg. Promo-20230531:Chapters
+                warnings.warn(f"unknown base: {base} in {abbrev}:{rarity}")
                 return
         # fix release date for reprints
         if (abbrev, code) in Card._REPRINTS_RELEASE_DATE:
             ret["release_date"] = Card._REPRINTS_RELEASE_DATE[
                 (abbrev, code)
             ].isoformat()
         count = match["count"]
@@ -475,31 +685,43 @@
                     ret["frequency"] = count
                 except KeyError:
                     warnings.warn(f"unknown frequency {count} in {rarity}")
             else:
                 ret["copies"] = count
         return ret
 
+    @staticmethod
+    def _partition(iterable, condition):
+        """Partition iterable given a condition: returns matching, not matching"""
+        lhs = []
+        rhs = []
+        for it in iterable:
+            if condition(it):
+                lhs.append(it)
+            else:
+                rhs.append(it)
+        return lhs, rhs
+
 
 class CardMap(utils.FuzzyDict):
     """A fuzzy dict specialized for cards.
 
     Cards are index both by ID (int) and a number of name variations (str).
     Iterating over the CardMap will return each card (values) once, not the keys.
     len() will also return the number of unique cards, not the count of name variations.
     """
 
-    _VEKN_CSV = (
+    _VEKN_CSV = [
         "http://www.vekn.net/images/stories/downloads/vtescsv_utf8.zip",
         [
             "vtessets.csv",
             "vtescrypt.csv",
             "vteslib.csv",
         ],
-    )
+    ]
     _VEKN_CSV_I18N = {
         "fr-FR": (
             "http://www.vekn.net/images/stories/downloads/"
             "french/vtescsv_utf8.fr-FR.zip",
             [
                 "vtessets.fr-FR.csv",
                 "vtescrypt.fr-FR.csv",
@@ -517,15 +739,15 @@
         ),
     }
 
     def __init__(self, aliases: Dict[str, str] = None):
         """Use config.ALIASES as aliases"""
         super().__init__(aliases=config.ALIASES if aliases is None else aliases)
 
-    def __iter__(self):
+    def __iter__(self) -> Generator[Card, None, None]:
         """When iterating only, return each card once."""
         for key, card in self.items():
             if isinstance(key, int):
                 yield card
 
     def __len__(self):
         """Count the number of different cards in Map."""
@@ -534,34 +756,69 @@
     def load(self) -> None:
         """Load VTES cards from KRCG static."""
         r = requests.request("GET", config.KRCG_STATIC_SERVER + "/data/vtes.json")
         r.raise_for_status()
         self.clear()
         self.from_json(r.json())
 
-    def add(self, card: Card) -> None:
-        """Add a card to the map, with all name variatoins.
+    def _map_names(self) -> None:
+        """Add name and variations access for all cards."""
+        cards = list(self)
+        for card in cards:
+            self[card.name] = card
+            for variant in card.name_variants:
+                self[variant] = card
+            # to avoid fuzzy matching translated names,
+            # they're added as aliases only
+            for _lang, name in card.i18n_variants("name"):
+                self.add_alias(name, card.id)
+            for _lang, variants in card.i18n_variants("name_variants"):
+                for variant in variants:
+                    self.add_alias(variant, card.id)
+            for name in Card._AKA.get(card.id, []):
+                self[name] = self[card.id]
 
-        Can be called multiple times for a single card, for translations.
-        """
-        self[card.id] = card
-        self._add_variants(card._name, card)
-        for name in card.aka:
-            self._add_variants(name, card)
-        for _lang, name in card.i18n_variants("name"):
-            # to avoid fuzzy matching translated names, they're added as aliases only
-            self._add_name_and_shortcuts(name, card, alias=True)
-        for aka in Card._AKA.get(card.name, []):
-            self[aka] = card
+    def load_from_files(
+        self, *files: io.BufferedIOBase, set_abbrev: str = None
+    ) -> None:
+        """Load from local files. We don't expect a sets file, nor translation files."""
+        files = [
+            csv.DictReader(io.TextIOWrapper(f, encoding="utf-8-sig")) for f in files
+        ]
+        for line in itertools.chain.from_iterable(files):
+            card = Card()
+            card.from_vekn(line, default_set=set_abbrev)
+            self[card.id] = card
+        self._set_enriched_properties()
+        self._map_names()
 
-    def load_from_vekn(self):
+    def load_from_vekn(self) -> None:
         """Load from official VEKN CSV files."""
         set_dict = sets.SetMap()
         # download the zip files containing the official CSV
-        main_files = utils.get_zip_csv(self._VEKN_CSV[0], *self._VEKN_CSV[1])
+        if LOCAL_CARDS:
+            main_files = [
+                csv.DictReader(
+                    importlib.resources.files("cards")
+                    .joinpath("vtessets.csv")
+                    .read_text("utf-8-sig"),
+                ),
+                csv.DictReader(
+                    importlib.resources.files("cards")
+                    .joinpath("vtescrypt.csv")
+                    .read_text("utf-8-sig"),
+                ),
+                csv.DictReader(
+                    importlib.resources.files("cards")
+                    .joinpath("vteslib.csv")
+                    .read_text("utf-8-sig"),
+                ),
+            ]
+        else:
+            main_files = utils.get_zip_csv(self._VEKN_CSV[0], *self._VEKN_CSV[1])
         i18n_files = {
             lang: utils.get_zip_csv(url, *filenames)
             for lang, (url, filenames) in self._VEKN_CSV_I18N.items()
         }
         # load sets
         for line in main_files[0]:
             set_ = sets.Set()
@@ -570,80 +827,162 @@
         for lang, files in i18n_files.items():
             for line in files[0]:
                 set_dict[line["Abbrev"]].i18n_set(lang, {"name": line["Full Name"]})
         # load cards
         for line in itertools.chain.from_iterable(main_files[1:]):
             card = Card()
             card.from_vekn(line, set_dict)
-            self.add(card)
+            self[card.id] = card
         for lang, files in i18n_files.items():
             for line in itertools.chain.from_iterable(files[1:]):
                 name = line.pop("Name")
                 cid = int(line.pop("Id"))
                 line["Name"] = line.pop("Name " + lang)
                 card = self[cid]
                 if card._name != name:
                     warnings.warn(f"{name} does not match {cid} in {lang} translation")
+                card_text = line["Card Text"].replace("(D)", "Ⓓ")
+                for old_name, new_name in card._CLAN_RENAMES.items():
+                    card_text = card_text.replace(old_name, new_name)
                 trans = {
                     "name": line["Name"],
                     "url": card._compute_url(lang[:2]),
-                    "card_text": line["Card Text"].replace("(D)", "Ⓓ"),
+                    "card_text": card_text,
                     "sets": {
                         set_name: set_dict[set_name].i18n(lang[:2], "name")
                         for set_name in card.sets.keys()
                         if set_name in set_dict
                     },
                 }
                 if "Flavor Text" in line:
                     trans["flavor_text"] = line["Flavor Text"]
                 card.i18n_set(lang[:2], trans)
-                self.add(card)
         urllib.request.urlcleanup()
+        self._set_enriched_properties()
+        # all name variants computed, now we can map all those name in the dict
+        self._map_names()
+
+    def _set_enriched_properties(self) -> None:
+        """Set enriched properties on cards.
+
+        This method sets addition information related to the cards
+        that are not in the original CSV:
+        - card.name_variants
+        - card.has_advanced
+        - card.has_evolution
+        - card.is_evolution
+        - card.variants
+        """
+        # first compute, for cards with same name (crypt cards only),
+        # which were the one to appear first (first_group)
+        same_name = collections.defaultdict(list)
+        for card in self:
+            same_name[card._name].append(card)
+        same_name = {k: v for k, v in same_name.items() if len(v) > 1}
+        for name, cards in same_name.items():
+            groups = collections.defaultdict(list)
+            variants = {}
+            for card in cards:
+                groups[card.group].append(card)
+                variants[card._key] = card.id
+            groups = sorted(groups.items(), key=lambda a: a[0])
+
+            for i, (_group, cards) in enumerate(groups):
+                if len(cards) > 1:
+                    assert sum(bool(c.adv) for c in cards) == 1, "bad advanced mark"
+                for card in cards:
+                    if not card.adv and len(cards) > 1:
+                        card.has_advanced = True
+                    if i < len(groups) - 1:
+                        card.has_evolution = True
+                    if i > 0:
+                        card.is_evolution = True
+                    card.variants = {
+                        k: v for k, v in variants.items() if k != card._key
+                    }
+
+        # now compute variants - cards in first_group can omit the group suffix
+        # advanced version can never omit the suffix
+        for card in self:
+            name_variants = list(self._variants(card._name, card))
+            name_variants = name_variants[1:]  # first name is the actual name
+            card.name_variants.extend(name_variants)
+            # registered official AKA (old name / previous version)
+            for name in card.aka:
+                card.name_variants.extend(self._variants(name, card))
+            # translations variants are registered in their respective i18 dict
+            for lang, name in card.i18n_variants("name"):
+                name_variants = list(self._variants(name, card))
+                name_variants = name_variants[1:]  # first name is the actual name
+                card.i18n_set(lang, {"name_variants": name_variants})
+
+    def _variants(self, name, card) -> Generator[str, None, None]:
+        suffix = card.get_suffix()
+        if suffix:
+            suffix = f" ({suffix})"
+        else:
+            suffix = ""
+        yield from self._word_variants(name, suffix)
+        if suffix and not card.is_evolution:
+            if card.adv:
+                yield from self._word_variants(name, " (ADV)")
+            else:
+                yield from self._word_variants(name, "")
+
+    def _word_variants(self, name, suffix) -> Generator[str, None, None]:
+        if "(TM)" in name:
+            yield from self._word_variants(name.replace("(TM)", "™"), suffix)
+        if name[-5:] == ", The":
+            yield from self._comma_splits("The " + name[:-5], suffix)
+        yield from self._comma_splits(name, suffix)
+        if name[:4] == "The ":
+            yield from self._comma_splits(name[4:] + ", The", suffix)
+
+    def _comma_splits(self, name, suffix) -> Generator[str, None, None]:
+        while True:
+            yield name + suffix
+            name = name.rsplit(",", 1)
+            if len(name) < 2:
+                break
+            name = name[0]
+            if len(name) <= self.threshold:
+                break
 
     def load_rulings(self) -> None:
         """Load card rulings from package YAML files."""
         for ruling in rulings.RulingReader():
             for cid, name in ruling.cards:
                 if self[cid].name != name:
                     warnings.warn(f"Rulings: {name} does not match {self[cid]}")
                 self[cid].rulings["text"].append(ruling.text)
                 for ref, link in ruling.links.items():
                     self[cid].rulings["links"][ref] = link
+            for card_reference in re.findall(r"{[^}]+}", ruling.text):
+                card_reference = card_reference[1:-1]
+                if card_reference not in self:
+                    warnings.warn(
+                        f"Rulings: {cid}|{name} mentions unknown card {card_reference}"
+                    )
+                if self[card_reference].usual_name != card_reference:
+                    warnings.warn(
+                        f"Rulings: {cid}|{name} mentions {card_reference} "
+                        f"instead of '{self[card_reference].name}'"
+                    )
 
     def to_json(self) -> Dict:
-        """Return a compact dict representation for JSON serialization."""
+        """Return a compact list representation for JSON serialization."""
         return [card.to_json() for card in self]
 
-    def from_json(self, state: Dict):
-        """Initialize from a JSON dict."""
+    def from_json(self, state: Dict) -> None:
+        """Initialize from a JSON list."""
         for dict_ in state:
             card = Card()
             card.from_json(dict_)
-            self.add(card)
-
-    def _add_variants(self, name: str, card: Card):
-        """Add all variants of the name."""
-        self._add_name_and_shortcuts(name, card)
-        if name[-5:].lower() == ", the":
-            self._add_name_and_shortcuts("the " + name[:-5], card)
-
-    def _add_name_and_shortcuts(self, name: str, card: Card, alias: bool = False):
-        """Add the name and shortcuts (splitting comma-separated qualifiers)."""
-        suffix = " (ADV)" if card.adv else ""
-        while True:
-            if alias:
-                self.add_alias(name + suffix, card.name)
-            else:
-                self[name + suffix] = card
-            name = name.rsplit(",", 1)
-            if len(name) < 2:
-                return
-            name = name[0]
-            if len(name) <= self.threshold:
-                return
+            self[card.id] = card
+        self._map_names()
 
 
 class CardTrie:
     """A helper class for text search inside a card.
 
     Combines results from multiple languages
     """
@@ -659,15 +998,15 @@
 
     def add(self, card: Card) -> None:
         """Add a card to the tries."""
         self.tries["en"].add(getattr(card, self.attribute, ""), card)
         for lang, trans in card.i18n_variants(self.attribute):
             self.tries[lang[:2]].add(trans, card)
 
-    def search(self, text: str, lang: str = None) -> Dict[str, collections.Counter]:
+    def search(self, text: str, lang: str = None) -> Dict[str, Counter[Card]]:
         """Search for `text`, in english and optional `lang`.
 
         Returns:
             A dict of scored results as {lang: Counter}, with no duplicates.
             If the same card is matched in multiple both `lang` and english,
             prefer the `lang` version.
         """
@@ -736,14 +1075,15 @@
     _TITLES = {
         "Camarilla": {"Primogen", "Prince", "Justicar", "Inner Circle", "Imperator"},
         "Sabbat": {"Bishop", "Archbishop", "Cardinal", "Regent", "Priscus"},
         "Anarch": {"Baron"},
         "Laibon": {"Magaji", "Kholo"},
     }
     _ALL_TITLES = sum(map(list, _TITLES.values()), [])
+    _LEGACY_CLANS = {v: k for k, v in Card._CLAN_RENAMES.items()}
     trie_dimensions = [
         "name",
         "card_text",
         "flavor_text",
     ]
     set_dimensions = [
         "type",
@@ -771,26 +1111,26 @@
         for attr in self.set_dimensions:
             setattr(self, attr, collections.defaultdict(set))
         # caches
         self._all = set()
         self._set_dimensions_enums = None
         self._normalized_set_enum_map = None
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         return bool(self._all)
 
-    def clear(self):
+    def clear(self) -> None:
         """Clear content."""
         for attr in self.set_dimensions + self.trie_dimensions:
             try:
                 getattr(self, attr).clear()
             except TypeError:
                 pass
 
-    def add(self, card: Card):
+    def add(self, card: Card) -> None:
         """Add a card to the engine."""
         self._set_dimensions_enums = None
         self._normalized_set_enum_map = None
         self._all.add(card)
         self.name.add(card)
         for type_ in card.types:
             self.type[type_].add(card)
@@ -807,14 +1147,16 @@
             self.bonus["Trifle"].add(card)
         if card.crypt:
             self.type["Crypt"].add(card)
         else:
             self.type["Library"].add(card)
         for clan in card.clans:
             self.clan[clan].add(card)
+            if clan in self._LEGACY_CLANS:
+                self.clan[self._LEGACY_CLANS[clan]].add(card)
         if not card.clans:
             self.clan["none"].add(card)
         if card.group:
             try:
                 self.group[int(card.group)].add(card)
             except ValueError:  # group "any"
                 for i in range(1, self._MAX_GROUP + 1):
@@ -835,19 +1177,19 @@
         self._handle_disciplines(card)
         self._handle_sect(card)
         self._handle_stealth_intercept(card)
         self._handle_titles(card)
         self._handle_exceptions(card)
 
     @property
-    def dimensions(self):
+    def dimensions(self) -> List[str]:
         return self.trie_dimensions + self.set_dimensions + ["text"]
 
     @property
-    def set_dimensions_enums(self):
+    def set_dimensions_enums(self) -> Dict[str, List[str]]:
         if not self._set_dimensions_enums:
             self._set_dimensions_enums = {
                 attr: sorted(set(getattr(self, attr).keys()))
                 for attr in self.set_dimensions
             }
         return self._set_dimensions_enums
 
@@ -910,15 +1252,15 @@
                     m.keys()
                     for m in getattr(self, dim).search(text, lang=lang).values()
                 )
             )
         return result
 
     @property
-    def _normalized_map(self):
+    def _normalized_map(self) -> Dict[str, Dict[str, str]]:
         """Used by __call__ (the search itself) to match set dimensions values
 
         This allows to match values case insensitively
         but still return the value with the original case.
 
         This way, self.set_dimensions_enums has proper casing and can be displayed
         to a user without additional processing.
@@ -926,23 +1268,23 @@
         if not self._normalized_set_enum_map:
             self._normalized_set_enum_map = {
                 dim: {utils.normalize(v): v for v in getattr(self, dim)}
                 for dim in self.set_dimensions
             }
         return self._normalized_set_enum_map
 
-    def _handle_text(self, card):
+    def _handle_text(self, card) -> None:
         """Helper handling card text."""
         self.card_text.add(card)
         if card.flavor_text:
             self.flavor_text.add(card)
         if card.draft:
             self.bonus["draft"].add(card.draft, card)
 
-    def _handle_disciplines(self, card):
+    def _handle_disciplines(self, card) -> None:
         """Helper handling card disciplines."""
         for discipline in card.disciplines:
             self.discipline[discipline].add(card)
             self.discipline[discipline.lower()].add(card)
         if not card.disciplines:
             self.discipline["none"].add(card)
         elif card.library and len(card.disciplines) > 1:
@@ -952,15 +1294,15 @@
         if "[FLIGHT]" in card.card_text:
             self.discipline["flight"].add(card)
         if card.combo:
             self.discipline["combo"].add(card)
         if card.multidisc:
             self.discipline["choice"].add(card)
 
-    def _handle_sect(self, card):
+    def _handle_sect(self, card) -> None:
         """Helper handling sects."""
         if card.crypt:
             if re.search(r"^(\[MERGED\] )?Sabbat", card.card_text):
                 self.sect["Sabbat"].add(card)
             if re.search(r"^(\[MERGED\] )?Camarilla", card.card_text):
                 self.sect["Camarilla"].add(card)
             if re.search(r"^(\[MERGED\] )?Laibon", card.card_text):
@@ -980,35 +1322,39 @@
                 r"Requires a( ready|n)( (I|i)ndependent or)? (A|a)narch",
                 card.card_text,
             ):
                 self.sect["Anarch"].add(card)
             if re.search(r"Requires a( ready|n) (I|i)ndependent", card.card_text):
                 self.sect["Independent"].add(card)
 
-    def _handle_stealth_intercept(self, card):
+    def _handle_stealth_intercept(self, card) -> None:
         """Helper handling stealth and intercept."""
         if re.search(r"\+(\d|X)\s+(i|I)ntercept", card.card_text):
             self.bonus["Intercept"].add(card)
         # do not include stealthed actions as stealth cards
         if re.search(r"\+(\d|X)\s+(s|S)tealth (?!Ⓓ|action|political)", card.card_text):
             self.bonus["Stealth"].add(card)
         # stealth/intercept maluses count has bonus of the other
         if not set(card.types) & {"Master", "Vampire", "Imbued"}:
             if re.search(r"-(\d|X)\s+(s|S)tealth", card.card_text):
                 self.bonus["Intercept"].add(card)
+            if re.search(r"(s|S)tealth\s+to\s+(0|zero)", card.card_text):
+                self.bonus["Intercept"].add(card)
             if re.search(r"-(\d|X)\s+(i|I)ntercept", card.card_text):
                 self.bonus["Stealth"].add(card)
+            if re.search(r"(i|I)ntercept\s+to\s+(0|zero)", card.card_text):
+                self.bonus["Stealth"].add(card)
         # list reset stealth as intercept
         if re.search(r"stealth .* to 0", card.card_text):
             self.bonus["Intercept"].add(card)
         # list block denials as stealth
         if re.search(r"attempt fails", card.card_text):
             self.bonus["Stealth"].add(card)
 
-    def _handle_titles(self, card):
+    def _handle_titles(self, card) -> None:
         """Helper handling titles, votes and city."""
         if card.title:
             self.title[card.title].add(card)
             self.bonus["Votes"].add(card)
         if re.search(r"(\d|X)\s+(v|V)ote", card.card_text):
             self.bonus["Votes"].add(card)
         for title in re.findall(
@@ -1044,19 +1390,19 @@
             if re.search(r"Requires a( ready)? titled vampire", card.card_text):
                 for title in self._ALL_TITLES + ["1 vote", "2 votes"]:
                     self.title[title].add(card)
             if re.search(r"Requires a( ready)? (M|m)agaji", card.card_text):
                 self.title["Magaji"].add(card)
                 self.sect["Laibon"].add(card)
 
-    def _handle_exceptions(self, card):
+    def _handle_exceptions(self, card) -> None:
         """Search exceptions not handled automatically."""
         # The Baron has his name in card text, but is not an Anarch Baron.
-        if card.name == "The Baron":
+        if card.id == 200167:  # "The Baron"
             self.sect["Anarch"].remove(card)
             self.title["Baron"].remove(card)
         # Gwen has another set of disciplines under condition
-        elif card.name == "Gwen Brand":
+        elif card.id == 200553:  # "Gwen Brand"
             self.discipline["ANI"].add(card)
             self.discipline["AUS"].add(card)
             self.discipline["CHI"].add(card)
             self.discipline["FOR"].add(card)
```

### Comparing `krcg-2.9/krcg/config.py` & `krcg-3.0/krcg/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,14 +262,15 @@
     "2k8sanfranqual",  # 59 cards listed
     "2k8pwbsla2",  # 91 cards listed
     "2k6faceaface",  # 91 cards listed
     "2k4virolaxboston",  # 91 cards listed
     "2k4edith",  # 91 cards listed
     "2k4pariscup",  # 11 crypt cards listed
     "2k3nycanarch",  # 91 cards listed
+    "ckgc2k",  # 91 cards listed
     "saveface2k1",  # 91 cards listed
     "genconuk2k1-treasure",  # 91 cards listed
     "jd32000",  # 91 cards listed
     "dog",  # 100 cards listed
     "matt-alamut",  # 91 cards listed
     "stevewampler",  # 59 cards listed
 }
```

### Comparing `krcg-2.9/krcg/deck.py` & `krcg-3.0/krcg/deck.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Deck class: serialization and card access under conditions"""
 from typing import Callable, Generator, Optional, TextIO
 import arrow
 import collections
 import datetime
 import email.utils
-import requests
 import itertools
+import logging
+import re
+import requests
 import unidecode
-
+import urllib.parse
 
 from . import config
-from . import logging
 from . import parser
 from . import vtes
 from . import utils
 
 
-logger = logging.logger
+logger = logging.getLogger("krcg")
 
 
 class Deck(collections.Counter):
     """A VTES deck, including meta information such as date, author and comments."""
 
     def __init__(self, *args, **kwargs):
         self.id = kwargs.pop("id", None)
@@ -71,66 +72,110 @@
         ret = cls(id=uid, author=r.get("author", None))
         ret.name = r.get("title", None)
         ret.comments = r.get("description", "")
         ret.date = arrow.get(r["modified"]).date()
         if not vtes.VTES:
             vtes.VTES.load()
         for cid, count in r["cards"].items():
+            count = int(count)
+            if count <= 0:
+                continue
             ret[vtes.VTES.amaranth[cid]] = count
         return ret
 
     @classmethod
     def from_vdb(cls, uid: str):
         """Fetch a deck from VDB."""
-        r = requests.get("https://vdb.smeea.casa/api/deck/" + uid)
+        r = requests.get("https://vdb.im/api/deck/" + uid)
         r.raise_for_status()
-        r = r.json()[uid]
+        r = r.json()
+        logger.debug("VDB replied: %s", r)
         ret = cls(id=uid, author=r.get("author", r.get("owner", None)))
         ret.name = r.get("name", None)
         ret.comments = r.get("description", "")
-        ret.date = email.utils.parsedate_to_datetime(r["timestamp"]).date()
+        ret.date = (
+            email.utils.parsedate_to_datetime(r["timestamp"]).date()
+            if ("timestamp" in r)
+            else None
+        )
         if not vtes.VTES:
             vtes.VTES.load()
-        for cid, data in itertools.chain(r["crypt"].items(), r["library"].items()):
-            ret[vtes.VTES[int(cid)]] = data["q"]
+        for cid, count in r["cards"].items():
+            count = int(count)
+            if count <= 0:
+                continue
+            ret[vtes.VTES[int(cid)]] = count
         return ret
 
+    @classmethod
+    def from_url(cls, url: str):
+        """Fetch from any deckbuilding website"""
+        result = urllib.parse.urlparse(url)
+        if result.netloc == "amaranth.vtes.co.nz":
+            if result.fragment.startswith("deck/"):
+                return cls.from_amaranth(result.fragment[5:])
+            raise ValueError("Unknown Amaranth URL format")
+        elif result.netloc in {"vdb.smeea.casa", "vdb.im"}:
+            if not result.path.startswith("/decks"):
+                raise ValueError("Unknown VDB URL path")
+            params = urllib.parse.parse_qs(result.query)
+            if "id" in params:
+                return cls.from_vdb(params["id"][0])
+            elif result.fragment:
+                ret = cls()
+                ret.name = params.get("name", None)
+                ret.author = params.get("author", None)
+                ret.comments = params.get("description", "")
+                if not vtes.VTES:
+                    vtes.VTES.load()
+                for item in result.fragment.split(";"):
+                    card, count = item.split("=", 1)
+                    count = int(count)
+                    if count <= 0:
+                        continue
+                    ret[vtes.VTES[int(card)]] = count
+                return ret
+            elif result.path.startswith("/decks/"):
+                return cls.from_vdb(result.path[7:])
+            raise ValueError("Unknown VDB URL format")
+        raise ValueError("Unknown deck URL provider")
+
     def check(self) -> bool:
         """Check a deck conforms to the rules IRT cards count
 
         Does not check grouping nor banished cards
 
         Returns:
             True if the deck checks out
         """
         res = True
         library_count = self.cards_count(lambda c: c.library)
         crypt_count = self.cards_count(lambda c: c.crypt)
         if library_count < 60:
             logger.warning(
-                "deck has too few cards ({count}) [{repr}]",
-                id=self.id,
-                count=library_count,
-                repr=self,
+                "deck %s has too few cards (%s) [%s]",
+                self.id,
+                library_count,
+                self,
             )
             res = False
         if library_count > 90:
             logger.warning(
-                "deck has too many cards ({count}) [{repr}]",
-                id=self.id,
-                count=library_count,
-                repr=self,
+                "deck %s has too many cards (%s) [%s]",
+                self.id,
+                library_count,
+                self,
             )
             res = False
         if crypt_count < 12:
             logger.warning(
-                "deck is missing crypt cards ({count}) [{repr}]",
-                id=self.id,
-                count=crypt_count,
-                repr=self,
+                "deck %s is missing crypt cards (%s) [%s]",
+                self.id,
+                crypt_count,
+                self,
             )
             res = False
         return res
 
     def to_json(self) -> dict:
         """Return a compact dict representation for JSON serialization."""
         ret = {
@@ -138,25 +183,25 @@
             "event": self.event,
             "event_link": self.event_link,
             "place": self.place,
             "date": self.date.isoformat() if self.date else None,
             "tournament_format": self.tournament_format,
             "players_count": self.players_count,
             "player": self.player,
-            "score": self.score,
+            "score": str(self.score) if self.score else None,
             "name": self.name,
             "author": self.author,
             "comments": self.comments,
             "crypt": {
                 "count": self.cards_count(lambda c: c.crypt),
                 "cards": [
                     {
                         "id": card.id,
                         "count": count,
-                        "name": card.name,
+                        "name": card.usual_name,
                         "comments": self.cards_comments.get(card),
                     }
                     for card, count in self.cards(lambda c: c.crypt)
                 ],
             },
             "library": {"count": self.cards_count(lambda c: c.library), "cards": []},
         }
@@ -177,28 +222,39 @@
                         "count": count,
                         "name": card.name,
                         "comments": self.cards_comments.get(card),
                     }
                 )
         return utils.json_pack(ret)
 
+    def to_minimal_json(self) -> dict:
+        ret = {
+            "id": self.id,
+            "name": self.name,
+            "cards": {str(card.id): count for card, count in self.cards() if count},
+        }
+        return utils.json_pack(ret)
+
     def from_json(self, state) -> None:
         """Initialize from a JSON dict generated by the `to_json()` method."""
         self.id = state.get("id")
         self.event = state.get("event")
         self.place = state.get("place")
         if "date" in state:
             self.date = datetime.date.fromisoformat(state["date"])
         self.tournament_format = state.get("tournament_format")
         self.players_count = state.get("players_count")
         self.player = state.get("player")
-        self.score = state.get("score")
+        self.score = DeckScore(state.get("score")) if state.get("score") else None
         self.name = state.get("name")
         self.author = state.get("author")
         self.comments = state.get("comments")
+        for card_id, count in state.get("cards", {}).items():
+            c = vtes.VTES[int(card_id)]
+            self[c] = count
         for card in state.get("crypt", {}).get("cards", []):
             c = vtes.VTES[card["id"]]
             self[c] = card["count"]
             if card.get("comments"):
                 self.cards_comments[c] = card["comments"]
         for section in state.get("library", {}).get("cards", []):
             for card in section["cards"]:
@@ -414,15 +470,67 @@
         for _, cards in self._sorted_library():
             for card, count in cards:
                 lines.append(f"{count}x {card.vekn_name}")
         return "\n".join(lines)
 
     def _to_txt_lackey(self) -> str:
         """Format used by LackeyCCG."""
+
+        def lackerize(name):
+            return unidecode.unidecode(card.vekn_name)
+
         lines = []
         for _, cards in self._sorted_library():
             for card, count in cards:
-                lines.append(f"{count}\t{unidecode.unidecode(card.vekn_name)}")
+                lines.append(f"{count}\t{lackerize(card.vekn_name)}")
         lines.append("Crypt:")
         for card, count in self.crypt:
-            lines.append(f"{count}\t{unidecode.unidecode(card.vekn_name)}")
+            lines.append(f"{count}\t{lackerize(card.vekn_name)}")
         return "\n".join(lines)
+
+    def to_vdb(self) -> str:
+        """Generating vdb.smeaa.casa link to deck"""
+        link = "https://vdb.im/decks?"
+        link += urllib.parse.urlencode(
+            {
+                "name": self.name or "New KRCG Deck",
+                "author": self.author or self.player or "KRCG",
+            }
+        )
+        link += "#"
+        for card, count in self.crypt:
+            link += f"{card.id}={count};"
+        for _, cards in self._sorted_library():
+            for card, count in cards:
+                link += f"{card.id}={count};"
+        return link[:-1]
+
+
+class DeckScore:
+    def __init__(self, s: Optional[str] = None):
+        self.game_wins = None
+        self.round_vps = None
+        self.finals_vps = None
+        if s is None:
+            return
+        score = re.match(
+            r"(\s*-?-?\s*(?P<game_wins>\d)\s*gw\s*"
+            r"(?P<round_vps>\d+(\.|,)?\d?)\s*(vp)?\s*)?"
+            r"(\s*-?-?\s*(?P<plus_mark>\+)?\s*(?P<finals_vps>\d(\.|,)?\d?)\s*"
+            r"(?(plus_mark).?|vp))?",
+            s.lower(),
+        )
+        if score.end() < 1:
+            raise ValueError("No score information")
+        self.game_wins = score.group("game_wins")
+        self.round_vps = score.group("round_vps")
+        self.finals_vps = score.group("finals_vps")
+
+    def __str__(self):
+        ret = ""
+        if self.game_wins:
+            ret += f"{self.game_wins}GW"
+        if self.round_vps:
+            ret += f"{self.round_vps}"
+        if self.finals_vps:
+            ret += f"+{self.finals_vps}"
+        return ret
```

### Comparing `krcg-2.9/krcg/parser.py` & `krcg-3.0/krcg/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Deck list parser.
 
 It handles the legacy TWDA: many tricky formats used through this historic document.
 Only modifiy this file if you know what you're doing, and proceed with caution.
 """
 from typing import TextIO, Tuple
+import datetime
 import enum
+import logging
 import math
 import re
 
 import arrow
 
 from . import config
-from . import logging
+from . import deck
 from . import vtes
 from . import utils
 
 
-logger = logging.logger
+logger = logging.getLogger("krcg")
 
 #: classic headers in deck lists
 _HEADERS = [
     "actin",
     "action",
     "acton",
     "allies",
@@ -123,14 +125,15 @@
 # special case for "channel 10" to avoid parsing 10x "channel".
 # "local 1111" and such are OK: we only consider max 2 digits as valid.
 _NAME = r"(?P<name>channel 10|.+?)(,\s*$)?"
 # only match a crypt tail if a card count was present in the head
 _DISCIPLINE_TRIGRAM = "|".join(
     [
         "-none-",
+        "none",
         "abo",
         "ani",
         "aus",
         "cel",
         "chi",
         "dai",
         "def",
@@ -158,14 +161,15 @@
         "tha",
         "thn",
         "val",
         "ven",
         "vic",
         "vin",
         "vis",
+        "viz",
     ]
 )
 _TITLE = "|".join(
     [
         "primogen",
         "prince",
         "justicar",
@@ -194,14 +198,16 @@
         "blood brother",
         "toreador",
         "giovanni",
         "ahrimane",
         "akunanse",
         "brujah",
         "assamite",
+        "banu haqim",
+        "ministry",
         "follower of set",
         "brujah antitribu",
         "guruhi",
         "toreador antitribu",
         "tzimisce",
         "malkavian",
         "gangrel",
@@ -231,19 +237,18 @@
         "abomination",
         "martyr",
         "innocent",
         "judge",
         "redeemer",
     ]
 )
-_CRYPT_TAIL = (
-    r"(?(ante_count)(?P<crypt_tail>\s+\d{1,2}\s+"
-    + r"({}|{}|{}|\s|:|\d{{1,2}}|any)*)|%NOMATCH%)?".format(
-        _DISCIPLINE_TRIGRAM, _TITLE, _CLAN
-    )
+_CRYPT_TAIL = r"(?(ante_count)(?P<crypt_tail>\s+(\d{{1,2}}|{})\s+".format(
+    _DISCIPLINE_TRIGRAM
+) + r"({}|{}|{}|\s|:|g?\d{{1,2}}|any|g\*)*)|%NOMATCH%)?".format(
+    _DISCIPLINE_TRIGRAM, _TITLE, _CLAN
 )
 _PUNCTUATED_TRAIT = "|".join(
     [
         "defense",
         "fligh",
         "gargoyle",
         "innocence",
@@ -254,14 +259,15 @@
         "vengeance",
         "vision",
         "mage",
         "mummy",
         "bane mummy",
         "wraith",
         "hunter",
+        "giovanni",
         "goblin",
         "changeling",
         # this one pften appears after double dashes in legacy deck lists:
         # Bang Nakh -- Tiger's Claws
         # catch it here to avoid putting it in comments,
         # there's a matching alias in config.ALIASES
         "tiger's claws",
@@ -281,15 +287,14 @@
         "brujah",
         "brujah antitribu",
         "caitiff",
         "daughter of cacophony",
         "follower of set",
         "gangrel",
         "gangrel antitribu",
-        "giovanni",
         "guruhi",
         "harbinger of skulls",
         "ishtarri",
         "kiasyd",
         "lasombra",
         "malkavian",
         "malkavian antitribu",
@@ -367,14 +372,22 @@
 # The full-fledged regular expression used to parse a line in a decklist
 _RE = (
     f"^{_PUNCTUATION}({_ANTE_COUNT})?{_PUNCTUATION}{_NAME}{_CRYPT_TAIL}"
     f"({_POST_COUNT})?({_TRAIT})?{_COMMENT}?\\s*$"
 )
 
 
+class LineLogAdapter(logging.LoggerAdapter):
+    """Log line and deck"""
+
+    def process(self, msg, kwargs):
+        self.extra.update(kwargs.get("extra", {}))
+        return "[%6s][%s] %s" % (self.extra["line"], self.extra["deck"], msg), kwargs
+
+
 class Mark(enum.Enum):
     """A comment Mark."""
 
     LINE = enum.auto()
     MULTILINE = enum.auto()
     PREFACE = enum.auto()
     END = enum.auto()
@@ -423,15 +436,15 @@
         # if may be a parsing error
         if not self.mark:
             match = re.match(
                 f"{_PUNCTUATION}{_ANTE_COUNT}(x|X|\\*|-|_|\\s)+(\\w|\\d|\\s|:|'|,)+\\(",
                 self.string.split("\n", 1)[0],
             )
             if match:
-                logger.warning('failed to parse "{}"', self.log)
+                logger.warning('failed to parse "%s"', self.log)
                 self.string = ""
 
     @property
     def log(self) -> str:
         """Log-friendly version of the comment (cropped at 83 chars)"""
         res = self.string.replace("\n", " ").strip()
         if len(res) > 83:
@@ -454,70 +467,98 @@
     """
 
     def __init__(self, deck):
         self.current_comment = None
         self.preface = True
         self.separator = False  # used only for additional checks on the TWDA
         self.deck = deck
+        self.logger = logger
+
+    @property
+    def _previous_line(self):
+        return (getattr(self.logger, "extra", {}).get("line") or 1) - 1
 
     def parse(self, input: TextIO, offset: int = 0, twda: bool = False) -> None:
         """Parse given stream.
 
         Args:
             offset: offset to add when parsing part of a bigger stream (for logs)
             twda: if true, parse for TWDA headers
         """
         if not vtes.VTES:
             vtes.VTES.load()
         for index, line in enumerate(input, 1):
-            logger.extra["line"] = index + offset
-            logger.extra["deck"] = self.deck.id
+            self.logger = LineLogAdapter(
+                logger, {"line": index + offset, "deck": self.deck.id}
+            )
             self.parse_line(index, line, twda)
         # finalize current_comment if any
         self.comment("", mark=Mark.END)
 
         # a wrong card count can be a good indication of a parsing error
         if not twda or self.deck.id not in config.TWDA_CHECK_DECK_FAILS:
             self.deck.check()
-        logger.extra["line"] = None
-        logger.extra["deck"] = None
 
     def parse_line(self, index: int, line: str, twda: bool):
         """Parse a line of text."""
         # remove head/tail and misplaced spaces around punctuation for easy parsing
         line = line.rstrip()
         line = line.replace(" :", ":")
         line = line.replace("( ", "(")
         line = line.replace(" )", ")")
-        if twda and self.preface:
-            if self.parse_twda_headers(index, line):
+        if self.preface:
+            if twda and self.parse_twda_headers(index, line):
                 return
+            if self.parse_headers(index, line):
+                return
+        else:
+            # Always put a date, so if no date was parsed in headers,
+            # just put today as the date
+            if not self.deck.date:
+                self.deck.date = datetime.date.today()
+                if twda:
+                    self.logger.warning("No date found, using today")
+            # author is only set if different than player
+            if self.deck.author and not self.deck.player:
+                self.deck.player = self.deck.author
+                self.deck.author = None
+            if self.deck.author == self.deck.player:
+                self.deck.author = None
         card, count = self.get_card(line, twda)
         if card and count:
             self.deck.update({card: count})
 
     def parse_twda_headers(self, index: int, line: str):
         """Parse a line of text for TWDA headers."""
-        if index < 4:
-            if index == 1:
-                self.deck.event = line
-            elif index == 2:
-                self.deck.place = line
-            elif index == 3:
+        if index == 1:
+            self.deck.event = line
+            return True
+        # third line should always be the date, but it has happened that some
+        # submissions lack this field, misformat it,
+        # or omit the location (2nd line) for online events
+        if not self.deck.date:
+            try:
                 self.deck.date = arrow.get(line, "MMMM Do YYYY").date()
+                return True
+            except arrow.parser.ParserMatchError:
+                if index == 3:
+                    self.logger.warning("Unable to parse date header: %s", line)
+                pass
+        if index == 2:
+            self.deck.place = line
             return True
         if not self.deck.tournament_format:
             try:
-                self.deck.tournament_format = re.match(r"^\s*(\d+R\+F)", line).group(1)
+                self.deck.tournament_format = re.match(r"\s*(\d+R\+F)", line).group(1)
                 return True
             except AttributeError:
                 pass
         if not self.deck.players_count:
             try:
-                players_count = re.match(r"^\s*(\d+|\?+)\s*player", line).group(1)
+                players_count = re.match(r"\s*(\d+|\?+)\s*player", line).group(1)
                 self.deck.players_count = int(players_count)
                 return True
             except AttributeError:
                 pass
             except ValueError:
                 return True
         # Ignore Organizer line (rare inclusion)
@@ -537,62 +578,90 @@
         # remove comments on player's name
         if not self.deck.player:
             player = re.sub(r"\s*\([^\)]*\)", "", line.strip())
             player = re.sub(r"\s*--\s+.*", "", player)
             if player:
                 self.deck.player = player
             return True
+        return False
+
+    def parse_headers(self, index: int, line: str):
+        description = re.match(r"^\s*(D|d)escription\s*:?\s*", line)
+        if description:
+            line = line[description.end() :]
         if not self.deck.score:
             try:
-                score = re.match(
-                    r"-?-?\s*((?P<round_wins>\d)\s*(G|g)(W|w)\s*"
-                    r"(?P<round_vps>\d(\.|,)?\d?)\s*((v|V)(p|P))?\s*\+?\s*)?"
-                    r"(?P<final>\d(\.|,)?\d?)\s*(v|V)(p|P)",
-                    line,
+                self.deck.score = deck.DeckScore(line)
+                return True
+            except (AttributeError, ValueError):
+                pass
+        if not self.deck.name:
+            try:
+                self.deck.name = (
+                    re.match(r"^\s*((d|D)eck)?\s?(n|N)ame\s*:\s*(?P<name>.*)$", line)
+                    .group("name")
+                    .strip()
                 )
-                if score.group("round_wins"):
-                    self.deck.score = "{}gw{} + {}vp in the final".format(
-                        score.group("round_wins"),
-                        score.group("round_vps"),
-                        score.group("final"),
+                return True
+            except (AttributeError, ValueError):
+                pass
+        if not self.deck.author:
+            try:
+                self.deck.author = (
+                    re.match(
+                        r"\s*(((c|C)reated|(d|D)eck)\s*(b|B)y|"
+                        r"(a|A)uthors?|(c|C)reators?)\s*(:|\s)\s*(?P<author>.*)$",
+                        line,
                     )
-                else:
-                    self.deck.score = "{}vp in the final".format(score.group("final"))
+                    .group("author")
+                    .strip()
+                )
                 return True
             except AttributeError:
                 pass
-        if not self.deck.name:
+        if not self.deck.player:
             try:
-                self.deck.name = re.match(
-                    r"^\s*((d|D)eck)?\s?(n|N)ame\s*:\s*(?P<name>.*)$", line
-                ).group("name")
+                self.deck.player = (
+                    re.match(
+                        r"\s*((p|P)layed\s*(b|B)y)|((p|P)layer)\s*(:|\s)\s*"
+                        r"(?P<player>.*)$",
+                        line,
+                    )
+                    .group("player")
+                    .strip()
+                )
                 return True
             except AttributeError:
                 pass
-        if not self.deck.author:
+        if not self.deck.date:
             try:
-                self.deck.author = re.match(
-                    r"(((c|C)reated|(d|D)eck)\s*(b|B)y|"
-                    r"(a|A)uthors?|(c|C)reators?)\s*(:|\s)\s*(?P<author>.*)$",
-                    line,
-                ).group("author")
+                self.deck.date = arrow.get(line, "MMMM Do YYYY").date()
                 return True
-            except AttributeError:
+            except arrow.parser.ParserMatchError:
                 pass
 
     def get_card(self, line: str, twda: bool = False) -> Tuple[object, int]:
         """Try to find a card and count, register possible comment."""
         if re.match(_HEADERS_RE, utils.normalize(line)):
             return None, 0
         card, name, count, comment, mark = None, None, 0, "", None
         match = re.match(_RE, utils.normalize(line))
         # count before a card name is most common and easier to parse
         if match:
             name = match.group("name")
             count = int(match.group("ante_count") or 0)
+            # get the group from the crypt tail
+            group = None
+            tail = match.group("crypt_tail")
+            if tail:
+                try:
+                    group = int(tail[-1])
+                except ValueError:
+                    pass
+
         if name:
             if not count:
                 # do not match name with no count prefix during the preface
                 # since card names are often found in preface comments and
                 # we expect a clean first line, either a prefixed crypt card (TWDA)
                 # or a prefixed card anyway (Lackey, JOL, etc.)
                 if self.preface:
@@ -600,29 +669,38 @@
                 else:
                     count = int(match.group("post_count") or 1)
                     if not match.group("count_mark"):
                         # Be wary of disciplines: they are sometimes headers, but
                         # distinguishing them from actual Master discipline cards
                         # is not decidable so we log and ignore the line
                         if name.strip(" :()[]-_*=") in _DISCIPLINES:
-                            logger.warning('improper discipline "{}"', line)
+                            self.logger.warning('improper discipline "%s"', line)
                             return None, 0
+            # for evolutions (eg. Theo Bell (G6)) the name in TWDA
+            # might not contain the group, we need to rely on the group in crypt tail
+            if name and group and name[-1] != ")":
+                name += f" (g{group})"
             try:
                 card = vtes.VTES[name]
-                if name == "raven" and card.name == "Camille Devereux, The Raven":
+                # special case for Camille / Raven to keep them distinct if the decklist
+                # predates the merge of the two crypt cards
+                if (
+                    name in ["raven", "raven (g1)"]
+                    and card.name == "Camille Devereux, The Raven (G1)"
+                ):
                     self.deck.raven = count
             except KeyError:
                 count = 0
         # do not match a card inside a marked multiline comment
         if (
             card
             and self.current_comment
             and self.current_comment.mark == Mark.MULTILINE
         ):
-            logger.warning('discarded match "{}" inside comment "{}"', name, line)
+            self.logger.warning('discarded match "%s" inside comment "%s"', name, line)
             card, count = None, 0
         # do not match crypt tail expression on a library card
         if card and match.group("crypt_tail") and not card.crypt:
             card, count = None, 0
         # do not match post count on a crypt card
         if card and match.group("post_count") and card.crypt:
             card, count = None, 0
@@ -688,33 +766,43 @@
         if (
             (card or not comment)
             and not self.preface
             and self.current_comment
             and not self.current_comment.multiline
             and not self.current_comment.mark
         ):
-            logger.warning(
-                'failed to parse "{}"',
-                self.current_comment.log,
-                extra={"line": (logger.extra.get("line") or 1) - 1},
-            )
+            # TODO use regexes
+            if self.current_comment.string.startswith(
+                "This deck was last saved"
+            ) or self.current_comment.string.startswith("http"):
+                self.logger.debug(
+                    'ignoring tail comment "%s"',
+                    self.current_comment.log,
+                    extra={"line": self._previous_line},
+                )
+            else:
+                self.logger.warning(
+                    'failed to parse "%s"',
+                    self.current_comment.log,
+                    extra={"line": self._previous_line},
+                )
             self.current_comment = None
         # log unmarked multiline comments in the middle of the list
         # they happen a lot in the TWDA, but checking them may be needed
         if (
             (card or mark)
             and self.current_comment
             and self.current_comment.multiline
             and self.current_comment.mark != Mark.MULTILINE
             and not self.preface
         ):
             logger.debug(
-                'unexpected multiline comment "{}"',
+                'unexpected multiline comment "%s"',
                 self.current_comment.log,
-                extra={"line": (logger.extra.get("line") or 1) - 1},
+                extra={"line": self._previous_line},
             )
         # if this is a new comment block, register the previous comment on the deck
         if self.current_comment and (
             mark == Mark.END
             or (
                 (card or not self.preface)
                 # if the comment is multiline and we did not parse a new card, continue
```

### Comparing `krcg-2.9/krcg/rulings.py` & `krcg-3.0/krcg/rulings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Rulings parsing.
 """
 from typing import Generator, Tuple
-import pkg_resources
+import importlib.resources
 import re
 import warnings
 import yaml
 
 
 class Ruling:
     """Simple class representing a ruling."""
@@ -17,35 +17,55 @@
 
 
 class RulingReader:
     """Reader to load KRCG YAML rulings files."""
 
     def __init__(self):
         self.links = yaml.safe_load(
-            pkg_resources.resource_string("rulings", "rulings-links.yaml")
+            importlib.resources.files("rulings")
+            .joinpath("rulings-links.yaml")
+            .read_text("utf-8")
         )
 
     def __iter__(self):
         """Yield Ruling instances"""
         for card, rulings in yaml.safe_load(
-            pkg_resources.resource_string("rulings", "cards-rulings.yaml")
+            importlib.resources.files("rulings")
+            .joinpath("cards-rulings.yaml")
+            .read_text("utf-8")
         ).items():
             for ruling in rulings:
                 ret = Ruling()
                 ret.cards = [_card_id_name(card)]
                 ret.text = ruling
-                ret.links = dict(self._get_link(ret.text))
+                if not ret.text or not isinstance(ret.text, str):
+                    warnings.warn(f"absent or misformed text in '{card}' ruling")
+                try:
+                    ret.links = dict(self._get_link(ret.text))
+                except KeyError:
+                    warnings.warn(f"Ruling: link not found for `{card}`")
+                    raise
                 yield ret
         for ruling in yaml.safe_load(
-            pkg_resources.resource_string("rulings", "general-rulings.yaml")
+            importlib.resources.files("rulings")
+            .joinpath("general-rulings.yaml")
+            .read_text("utf-8")
         ):
             ret = Ruling()
             ret.cards = [_card_id_name(card) for card in ruling["cards"]]
             ret.text = ruling["ruling"]
-            ret.links = dict(self._get_link(ret.text))
+            if not ret.text or not isinstance(ret.text, str):
+                warnings.warn(
+                    f"absent or misformed text in general ruling for {ret.cards}"
+                )
+            try:
+                ret.links = dict(self._get_link(ret.text))
+            except KeyError:
+                warnings.warn(f"Ruling: link not found for general ruling `{ret.text}`")
+                raise
             yield ret
 
     def _get_link(self, text: str) -> Generator:
         """Yield (reference, link) tuples from rulink text."""
         references = re.findall(r"\[[a-zA-Z]+\s[0-9-]+\]", text)
         if not references:
             warnings.warn(f"no reference in ruling: {text}")
```

### Comparing `krcg-2.9/krcg/sets.py` & `krcg-3.0/krcg/sets.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,23 @@
         self.company = data["Company"]
 
 
 class SetMap(dict):
     """A dict of all sets, index by Abbreviation and English name."""
 
     PROMOS = {
+        "Promo-20230531": ["2023 Promo", "2023-05-31"],
+        "Promo-20221022": ["2022 Promo", "2022-10-22"],
+        "Promo-20220730": ["2022 European GP Promo", "2022-07-30"],
+        "Promo-20211113": ["2021 SAC Promo", "2021-11-13"],
+        "Promo-20211015": ["2021 Promo Pack 3", "2021-10-15"],
+        "Promo-20210709": ["2021 Kickstarter Promo", "2021-07-09"],
+        "Promo-20210701": ["2021 Kickstarter Promo", "2021-07-01"],
+        "Promo-20210331": ["2021 Mind’s Eye Theatre Promo", "2021-03-31"],
+        "Promo-20210310": ["2021 Resellers Promo", "2021-03-31"],
         "Promo-20191123": ["2020 GP Promo", "2020-11-23"],
         "Promo-20201030": ["V5 Polish Edition promo", "2020-10-30"],
         "Promo-20201123": ["2020 GP Promo", "2020-11-23"],
         "Promo-20200511": ["2020 Promo Pack 2", "2020-05-11"],
         "Promo-20191027": ["2019 ACC Promo", "2019-10-27"],
         "Promo-20191005": ["2019 AC Promo", "2019-10-05"],
         "Promo-20190818": ["2019 EC Promo", "2019-08-18"],
@@ -46,14 +55,15 @@
         "Promo-20190601": ["2019 SAC Promo", "2019-06-01"],
         "Promo-20190615": ["2019 NAC Promo", "2019-06-15"],
         "Promo-20190629": ["2019 Grand Prix Promo", "2019-06-15"],
         "Promo-20190408": ["2019 Promo Pack 1", "2019-04-08"],
         "Promo-20181004": ["2018 Humble Bundle", "2018-10-04"],
         "Promo-20150219": ["2015 Storyline Rewards", "2015-02-19"],
         "Promo-20150221": ["2015 Storyline Rewards", "2015-02-21"],
+        "Promo-20150215": ["2015 Storyline Rewards", "2015-02-15"],
         "Promo-20150214": ["2015 Storyline Rewards", "2015-02-14"],
         "Promo-20150211": ["2015 Storyline Rewards", "2015-02-11"],
         "Promo-20150216": ["2015 Storyline Rewards", "2015-02-16"],
         "Promo-20150220": ["2015 Storyline Rewards", "2015-02-20"],
         "Promo-20150218": ["2015 Storyline Rewards", "2015-02-18"],
         "Promo-20150217": ["2015 Storyline Rewards", "2015-02-17"],
         "Promo-20150213": ["2015 Storyline Rewards", "2015-02-13"],
@@ -93,14 +103,16 @@
         "Promo-20020811": ["Sabbat War promo", "2002-08-11"],
         "Promo-20020704": ["Camarilla Edition promo", "2002-07-04"],
         "Promo-20020201": ["Winter 2002 Storyline promo", "2002-02-01"],
         "Promo-20011201": ["Bloodlines promo", "2001-12-01"],
         "Promo-20010428": ["Final Nights promo", "2001-04-28"],
         "Promo-20010302": ["Final Nights promo", "2001-03-02"],
         "Promo-19960101": ["1996 Promo", "1996-01-01"],
+        "HttB-R": ["Heirs to the Blood Reprint", "2018-07-14"],
+        "KoT-R": ["Keepers of Tradition Reprint", "2018-05-05"],
     }
 
     def __init__(self):
         super().__init__()
         self.add(Set(abbrev="POD", name="Print on Demand"))
         for abbrev, (name, release_date) in self.PROMOS.items():
             self.add(Set(abbrev=abbrev, name=name, release_date=release_date))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `krcg-2.9/krcg/twda.py` & `krcg-3.0/krcg/twda.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 If it has not been initialized, TWDA will evaluate to False.
 TWDA must be configured with `TWDA.configure()` before being used.
 """
 from typing import List, TextIO
 import collections
 import html
 import io
-import pkg_resources  # part of setuptools
+import logging
+import importlib.resources
 import re
 
 import requests
 
 from . import config
-from . import logging
 from . import deck
 from . import utils
 from . import vtes
 
-logger = logging.logger
+logger = logging.getLogger("krcg")
 
 
 class _TWDA(collections.OrderedDict):
     """An OrderedDict of the TWDA. Parsing TWDA.html is the hard part.
 
     Attributes:
         by_author (dict): Decks indexed by author
@@ -65,29 +65,24 @@
         id_, buffer, offset = "", None, 0
         for index, line in enumerate(source, 1):
             try:
                 id_ = re.match(r"^<a id=([^\s]*)\s", line).group(1)
             except AttributeError:
                 pass
             # new decklist
-            if re.match(r"^<hr><pre>$", line):
+            if re.match(r"^<hr><pre>\s*$", line):
                 buffer = io.StringIO()
                 offset = index
             # whole decklist fetched, parse it
             elif re.match(r"^</pre>", line):
                 buffer.seek(0)
                 # replace with a version of our own for the worst cases
-                if pkg_resources.resource_exists("twda_fix", f"{id_}.html"):
-                    buffer = io.StringIO(
-                        html.unescape(
-                            pkg_resources.resource_string(
-                                "twda_fix", f"{id_}.html"
-                            ).decode("utf-8")
-                        )
-                    )
+                fix_file = importlib.resources.files("twda_fix").joinpath(f"{id_}.html")
+                if fix_file.is_file():
+                    buffer = io.StringIO(html.unescape(fix_file.read_text("utf-8")))
                 self[id_] = deck.Deck.from_txt(buffer, id=id_, offset=offset, twda=True)
             elif buffer:
                 buffer.write(html.unescape(line))
         self._init()
         logger.info("TWDA loaded")
 
     def _init(self) -> None:
```

### Comparing `krcg-2.9/krcg/utils.py` & `krcg-3.0/krcg/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
     Sequence,
     Tuple,
 )
 import collections
 import csv
 import difflib
 import io
+import logging
 import re
 import unidecode
 import urllib.request
 import zipfile
 
-from . import logging
 
-logger = logging.logger
+logger = logging.getLogger("krcg")
 
 
 def normalize(s: Any):
     """Normalize a string for indexing: unidecode and lowercase."""
     if not isinstance(s, str):
         return s
     return unidecode.unidecode(s).lower().strip()
@@ -75,15 +75,15 @@
         if len(key) < self.threshold:
             return None
         result = difflib.get_close_matches(
             key, self._sequence_keys(), n=1, cutoff=self.cutoff
         )
         if result:
             result = result[0]
-            logger.info('"{}" matched "{}"', key, result)
+            logger.info('"%s" matched "%s"', key, result)
             return result
         return None
 
     def _sequence_keys(self) -> List[Sequence]:
         """Return all keys that are sequences and can be fuzzy matched."""
         if not self._keys_cache:
             self._keys_cache = [
```

### Comparing `krcg-2.9/krcg/vtes.py` & `krcg-3.0/krcg/vtes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module provides the `VTES` singleton: the VTES cards library.
 
 If it has not been initialized, VTES will evaluate to False.
 VTES must be configured with `VTES.configure()` before being used.
 """
-from typing import Dict, List
+from typing import Dict, Generator, List, Set, Tuple, Union
 import functools
+import io
 import requests
 
 from . import cards
 
 
 class _VTES:
     """VTES cards database"""
@@ -25,80 +26,93 @@
 
     def __contains__(self, key):
         return key in self._cards
 
     def __len__(self) -> int:
         return len(self._cards)
 
-    def __iter__(self):
+    def __iter__(self) -> Generator[cards.Card, None, None]:
         return self._cards.__iter__()
 
-    def to_json(self):
-        return [c.to_json() for c in self._cards]
+    def to_json(self) -> dict:
+        return self._cards.to_json()
 
-    def from_json(self, state):
+    def from_json(self, state) -> None:
         self.clear()
-        for c in state:
-            card = cards.Card()
-            card.from_json(c)
-            self._cards.add(card)
+        self._cards.from_json(state)
 
-    def get(self, key, default=None):
+    def get(self, key, default=None) -> cards.Card:
         return self._cards.get(key)
 
     def clear(self) -> None:
         self._cards.clear()
         self._search.clear()
 
     def load(self) -> None:
         """Load from KRCG static"""
         self.clear()
         self._cards.load()
 
-    def load_from_vekn(self):
+    def load_from_vekn(self) -> None:
         """Load the card database from vekn.net, with translations and rulings"""
         self.clear()
         self._cards.load_from_vekn()
         self._cards.load_rulings()
 
+    def load_from_files(self, *files: io.TextIOBase, set_abbrev: str = None) -> None:
+        self._cards.load_from_files(*files, set_abbrev=set_abbrev)
+
+    def diff(self, url) -> Dict[cards.Card, Union[str, Tuple[str, str]]]:
+        """Compute a diff from previous VEKN CSV files."""
+        old_cards = cards.CardMap()
+        old_cards._VEKN_CSV[0] = url
+        old_cards.load_from_vekn()
+        res = {c: "NEW" for c in self._cards if c.id not in old_cards}
+        for c in self._cards:
+            if c.id in old_cards:
+                diff = old_cards[c.id].diff(c)
+                if diff:
+                    res[c] = diff
+        return res
+
     @property
     @functools.lru_cache(1)
-    def amaranth(self):
+    def amaranth(self) -> Dict[int, cards.Card]:
         """Amaranth IDs card map."""
         r = requests.get("http://static.krcg.org/data/amaranth_ids.json")
         r.raise_for_status()
         return {k: self[v] for k, v in r.json().items()}
 
-    def complete(self, text: str, lang: str = "en") -> List:
+    def complete(self, text: str, lang: str = "en") -> List[str]:
         """Card name completion.
 
         Matches on the start of the name are returned first,
         other matches are returned alphabetically.
 
         Args:
             text: Parts of the name (can contain spaces)
 
         Returns:
             A sorted list of results, from most likely to less likely
         """
         self._init_search()
         ret = self._search.name.search(text, lang)
         ret = [
-            (card.name if lang == "en" else card.i18n(lang, "name"), score)
+            (card.usual_name if lang == "en" else card.i18n(lang, "name"), score)
             for lang, card_score in ret.items()
             for card, score in card_score.items()
         ]
         return [x[0] for x in sorted(ret, key=lambda x: (-x[1], x[0]))]
 
     @property
     def search_dimensions(self) -> Dict[str, List[str]]:
         self._init_search()
         return self._search.set_dimensions_enums
 
-    def search(self, **kwargs):
+    def search(self, **kwargs) -> Dict[str, Set[cards.Card]]:
         self._init_search()
         return self._search(**kwargs)
 
     def _init_search(self) -> None:
         """Initialize search and completion"""
         if not self._search:
             for c in self._cards:
```

### Comparing `krcg-2.9/krcg.egg-info/SOURCES.txt` & `krcg-3.0/krcg.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+cards/__init__.py
+cards/__main__.py
+cards/vtescrypt.csv
+cards/vteslib.csv
+cards/vteslibmeta.csv
+cards/vtessets.csv
 krcg/__init__.py
 krcg/analyzer.py
 krcg/cards.py
 krcg/config.py
 krcg/deck.py
-krcg/logging.py
 krcg/parser.py
 krcg/rulings.py
+krcg/seating.py
 krcg/sets.py
 krcg/twda.py
 krcg/utils.py
 krcg/vtes.py
 rulings/__init__.py
 rulings/cards-rulings.yaml
 rulings/general-rulings.yaml
```

### Comparing `krcg-2.9/rulings/cards-rulings.yaml` & `krcg-3.0/rulings/cards-rulings.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,3143 +1,3650 @@
 ---
 100001|.44 Magnum:
-  - "Provides only ony maneuver each combat, even if the bearer changes. [LSJ 19980302-2]"
+  - Provides only ony maneuver each combat, even if the bearer changes. [LSJ 19980302-2]
+100002|419 Operation:
+  - You can burn the edge to burn the card if it has no counter. [ANK 20221011-3]
 100003|Aaron's Feeding Razor:
-  - "The effect is not optional. [RTR 19980707] [LSJ 19980722]"
+  - The effect is not optional. [RTR 19980707] [LSJ 19980722]
 100004|Abactor:
   - '"Successful resolution" means the action must not be blocked and the vampire must have gained blood. If the vampire cannot gain blood (eg., {Vampiric Disease}, {Ex Nihilo}), the blood hunt is not called even if the action is not blocked. [LSJ 20090411]'
-  - "This is not a diablerie. Neither {Rebirth} nor {Carlton Van Wyk}'s ability can be used. [LSJ 20090724] [ANK 20180129-1]"
+  - This is not a diablerie. Neither {Rebirth} nor {Carlton Van Wyk}'s ability can be used. [LSJ 20090724] [ANK 20180129-1]
   - "The Blood Hunt referendum is still a Blood Hunt: {Lay Low} can be used, {Trophy: Diablerie} would prevent the referendum. [LSJ 20091026] [LSJ 20100112]"
-  - 'The Blood Hunt referendum is part of the action resolution. Cards that are played "after a successful action" or "after resolution" must be played after the referendum. {Heidelberg Castle, Germany} can not be used before the referendum. [LSJ 20100112] [PIB 20121028]'
+  - The Blood Hunt referendum is part of the action resolution. Cards that are played "after a successful action" or "after resolution" must be played after the referendum. {Heidelberg Castle, Germany} can not be used before the referendum. [LSJ 20100112] [PIB 20121028]
 100005|Abandoning the Flesh:
-  - "Cannot be played when burned as a result of a Blood Hunt referendum. [LSJ 20070417]"
-  - "Will not trigger the {Soul Gem of Etrius} since the vampire is removed from the game instead of being burned. [LSJ 20021010]"
+  - Cannot be played when burned as a result of a Blood Hunt referendum. [LSJ 20070417]
+  - Will not trigger the {Soul Gem of Etrius} since the vampire is removed from the game instead of being burned. [LSJ 20021010]
 100006|Abbot:
-  - "The +1 intercept applies to Ⓓ actions against cards controlled by the controller. It does not apply to Ⓓ actions against another Methusalah. [LSJ 20061222]"
+  - The +1 intercept applies to actions directed at cards controlled by the controller. It does not apply to actions directed at other Methuselahs. [LSJ 20061222]
 100007|Abjure:
-  - "Can be used by an incapacitated Imbued. [LSJ 20081016]"
+  - Can be used by an incapacitated Imbued. [LSJ 20081016]
 100008|Ablative Skin:
-  - "Cannot be used to prevent damage that cannot be prevented by cards that require Fortitude. [LSJ 19990216]"
+  - Cannot be used to prevent damage that cannot be prevented by cards that require Fortitude. [LSJ 19990216]
 100009|Abombwe:
-  - "The requirements are ignored if the card is not played in the normal fashion (eg. diablerie or {Bima}). [LSJ 20051116-2]"
+  - The requirements are ignored if the card is not played in the normal fashion (eg. diablerie or {Bima}). [LSJ 20051116-2]
 100010|Abomination:
-  - "Can be played by burning a werewolf that has been recruited the same turn. [RTR 20180303]"
+  - Can be played by burning a werewolf that has been recruited the same turn. [RTR 20180303]
 100011|Absimiliard's Army:
-  - "Putting the top card of your library in play as a ghoul does not count as playing the card. [LSJ 20040531]"
-  - "The card used to represent the ally is face up, but the name on that card is ignored if something goes looking for a card by name. They do not contest. [LSJ 20040623] [LSJ 20071003]"
-  - "A burned ghoul is removed from the game but is still burned first, triggering cards such as {Tension in the Ranks}. [LSJ 20090920]"
-  - "The Ghouls are not mortal, they are monsters. [ANK 20200203-2]"
+  - Putting the top card of your library in play as a ghoul does not count as playing the card. [LSJ 20040531]
+  - The card used to represent the ally is face up, but the name on that card is ignored if something goes looking for a card by name. They do not contest. [LSJ 20040623] [LSJ 20071003]
+  - A burned ghoul is removed from the game but is still burned first, triggering cards such as {Tension in the Ranks}. [LSJ 20090920]
 100013|Absorb the Mind:
-  - "Can be played against a vampire with no blood. [RTR 20010711]"
+  - Can be played against a vampire with no blood. [RTR 20010711]
 100014|Abyssal Hunter:
-  - "If ranged aggravated damage is inflicted at close range against him, he burns. [PIB 20110818]"
+  - Burns if ranged aggravated damage is inflicted on it at close range. [PIB 20110818]
+  - If he burns an ally with his action, this counts as a directed action burning an ally (eg. for Trophies). [ANK 20220507]
 100018|Aching Beauty:
-  - "The pool loss occurs if the block would be successful, even if the action is ended (eg. {Change of Target} or {Obedience}) or made unblockable ({Horrific Countenance}) at this point. [RTR 19991206] [LSJ 20091125]"
-  - "The cost is cumulative if a vampire has multiple copies of the card on him. [LSJ 19980225]"
+  - The pool loss occurs if the block would be successful, even if the action is ended (eg. {Change of Target} or {Obedience}) or made unblockable ({Horrific Countenance}) at this point. [RTR 19991206] [LSJ 20091125]
+  - Burn pool effects are cumulative. [LSJ 19980225]
 100023|The Admonitions:
-  - 'Cannot be used when a card is played, to draw a card that would cancel it "as it is played". [RTR 20040501]'
-  - "If you are the only Methuselah to control a Sabbat vampire, you keep control of The Admonitions each turn. [LSJ 20031121]"
+  - Cannot be used when a card is played, to draw a card that would cancel it "as it is played". [RTR 20040501]
+  - If you are the only Methuselah to control a Sabbat vampire, you keep control of The Admonitions each turn. [LSJ 20031121]
 100024|Agate Talisman:
-  - "Can be equipped by a vampire with capacity less than 4, although he cannot lock it to get a vote. [LSJ 20030607]"
+  - Can be equipped by a vampire with capacity less than 4, although they cannot lock it to get a vote. [LSJ 20030607]
 100025|Agent of Power:
-  - "Is unique and provides a discipline even when it was not played in the normal fashion (eg. diablerie, {Deviki Prasanta}, {Bima}). [LSJ 20071001-1] [LSJ 20100422]"
-  - 'If used as a placeholder to represent something else, its text does not apply (including the "Unique" part). A {Shock Troops} vampire would simply be a non-unique 1-cap Sabbat with no clan and no discipline. [LSJ 20071001-1]'
-  - "If you play Agent of Power on a vampire and that vampire plays a {Dual Form} at superior [PRO], the Dual Form gains the Discipline provided by the Agent of Power and keeps it once the Agent of Power burns. [LSJ 20071005-1]"
+  - Is unique and provides a discipline even when it was not played in the normal fashion (eg. diablerie, {Deviki Prasanta}, {Bima}). [LSJ 20071001-1] [LSJ 20100422]
+  - If used as a placeholder to represent something else, its text does not apply (including the "Unique" part). A {Shock Troops} vampire would simply be a non-unique 1-cap Sabbat with no clan and no discipline. [LSJ 20071001-1]
+  - If you play Agent of Power on a vampire and that vampire plays a {Dual Form} at superior [PRO], the Dual Form gains the Discipline provided by the Agent of Power and keeps it once the Agent of Power burns. [LSJ 20071005-1]
+100027|Ahriman's Demesne:
+  - "[OBT] The opponent does not go to torpor, {Undead Persistence} cannot be played. [LSJ 20040608] "
 100029|Aid from Bats:
   - "[ANI] The press can only be used during the current round. [TOM 19960521]"
 100038|Alastor:
-  - "If the given weapon costs blood, the target Alastor pays the cost. [LSJ 20040518]"
-  - "Requirements do not apply. [ANK 20200901]"
+  - If the weapon retrieved costs blood, that cost is paid by the vampire chosen by the vote. [LSJ 20040518]
+  - Requirements do not apply. If a discipline is required (eg. {Inscription}) and the Alastor vampire does not have it, the inferior version is used. [ANK 20200901] [LSJ 20040518-2]
 100043|Amaranth:
-  - "Effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]"
-  - 'If both minions want to play a card "when a vampire should go into torpor", acting minion goes first. If played first, {Undead Persistence} would prevent the opponent to play {Amaranth} and vice-versa. [RTR 20010710]'
+  - If both minions want to play a card "when a vampire should go into torpor", the acting minion goes first. If played first, {Undead Persistence} would prevent the opponent to play {Amaranth} and vice-versa. [RTR 20010710]
 100045|Ambulance:
-  - 'If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]'
-  - 'If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
-  - 'An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]'
+  - If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]
+  - If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]
+  - An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]
   - '"continue as if unblocked" moves the action card from the ash heap (where it went when the action was blocked) to limbo (where it should be if the action is not blocked). If the action card is not in the ash heap, then the action cannot be continued. [LSJ 20070808-1]'
 100046|Ambush:
-  - "If the target unlocks and the action is not blocked, it is successful but has no effect. [LSJ 20070411] [LSJ 20090514]"
+  - If the target unlocks and the action is not blocked, it is successful but has no effect. [LSJ 20070411] [LSJ 20090514]
 100047|Amria:
-  - "The press can only be used during the current round. [TOM 19960521]"
+  - The press can only be used during the current round. [TOM 19960521]
 100051|Ananasi Vampirephile:
-  - "When setting the range for the round, no other effect can be used to reset the range. Skip the determine range step on that round, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]"
-  - "Can use {Pack Alpha} to put a retainer requiring [ani] in play. [LSJ 20060417]"
+  - When setting the range for the round, no other effect can be used to reset the range. Skip the determine range step on that round, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]
+  - Can use {Pack Alpha} to put a retainer requiring [ani] in play. [LSJ 20060417]
 100052|The Anarch Free Press:
-  - "A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]"
+  - A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]
 100055|Anarch Revolt:
-  - "The cost is cumulative if they are multiple copies in play. [LSJ 19980225]"
+  - The cost is cumulative if they are multiple copies in play. [LSJ 19980225]
+  - If a Methuselah controls no ready Anarch by the end of the unlock phase, they must burn 1 pool, even if they had a ready Anarch at some point during the unlock phase. [LSJ 20080106]
 100058|Anarch Troublemaker:
-  - "Can lock a vampire that is already locked. [PIB 20121031]"
+  - Can lock a vampire that is already locked. [PIB 20121031]
 100060|Anathema:
-  - "Burns the target vampire when the target is reduced to zero blood in combat, regardless of the source of the loss. [RTR 19980623]"
+  - Burns the target vampire when the target is reduced to zero blood in combat, regardless of the source of the loss. [RTR 19980623]
   - "Will not burn a vampire for entering a combat with zero blood: there must be an actual blood loss. [RTR 19980623]"
-  - "Multiple Anathemas don't multiply the pool gain. Once one Anathema resolves it burns the vampire and the others are burned before they get to resolve. [LSJ 20021117]"
-  - "Damage done by combat effects after combat ends do not trigger Anathema. [LSJ 19980225]"
+  - Diablerie does not trigger Anathema. [LSJ 20021122-2] [ANK 20211112]
+  - Does not trigger if the vampire is burned by aggravated damage during damage resolution. [LSJ 20021120]
+  - Damage done by combat effects after combat ends do not trigger Anathema. [LSJ 19980225]
+  - Multiple Anathemas don't multiply the pool gain. Once one Anathema resolves it burns the vampire and the others are burned before they get to resolve. [LSJ 20021117]
+  - It is controlled by the controller of the minion it's on - it is not removed when another Methuselah is ousted. [PIB 20121028]
 100063|The Ancestor's Talisman:
-  - "The effect is not optional. [RTR 19980707] [LSJ 19980722]"
+  - The effect is not optional. [RTR 19980707] [LSJ 19980722]
 100064|Ancient Influence:
-  - "Applies a pool gain then a pool loss. {Poison Pill} register a 5 pool loss in all cases, a Methusalah cannot withdraw even if the total was positive. [ANK 20180813]"
+  - Applies a pool gain then a pool loss. {Poison Pill} register a 5 pool loss in all cases, a Methuselah cannot withdraw even if the total was positive. [ANK 20180813]
 100066|Anesthetic Touch:
-  - "Does not end combat as a strike; it ends combat after strike resolution. It is still just a hand strike. [LSJ 20011210-1]"
-  - "A dodge won't prevent combat from ending after strike resolution. [LSJ 20011210-2]"
-  - "Does not end combat until after strike resolution, so the damage can be prevented or healed as normal. [LSJ 20011210-3]"
+  - Does not end combat as a strike; it ends combat after strike resolution. It is still just a hand strike. [LSJ 20011210-1]
+  - A dodge won't prevent combat from ending after strike resolution. [LSJ 20011210-2]
+  - Does not end combat until after strike resolution, so the damage can be prevented or healed as normal. [LSJ 20011210-3]
 100067|Angel of Berlin:
-  - "May be played after a block is successful before combat begins. [LSJ 20060410]"
-"100071|The Ankara Citadel, Turkey":
-  - "Concerning the cost of the cards, multiplications and divisions are applied first, followed by additions and substractions. [RTR 20070707]"
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
+  - May be played after a block is successful before combat begins. [LSJ 20060410]
+100071|The Ankara Citadel, Turkey:
+  - Concerning the cost of the cards, multiplications and divisions are applied first, followed by additions and substractions. [RTR 20070707]
 100076|Apparition:
-  - "Can be played at any time in combat, even if there is no damage to prevent yet. [LSJ 20010315]"
+  - Can be played at any time in combat, even if there is no damage to prevent yet. [LSJ 20010315]
   - "[CHI] Prevents up to 2 damage, it can prevent less. [RTR 20041202]"
   - "[CHI] Can prevent 1 damage twice on separated strikes in the same round. [ANK 20200318]"
 100078|Approximation of Loyalty:
-  - '[pre] Cards and effects that can be played "as the action is announced" (and only them) can be played before it. [ANK 20190425]'
-100080|Arcane Appraiser:
-  - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
+  - '[pre] Cards and effects that are played "as the action is announced" must be played before playing "regular" action modifier or reaction cards. [ANK 20190425]'
+  - "[pre] Replace the action card (if any) before playing it. [ANK 20181208]"
+  - '[PRE] Cards are not replaced until all effects played "as a card is played" are resolved. [LSJ 20061013]'
+  - '[PRE] If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
+  - "[PRE] The card is still considered played. The same reaction cannot be played again by the same minion. [LSJ 19980212] [LSJ 20061207]"
+  - "[PRE] Must be played right after the reaction card to cancel is played. Another modifier cannot be played in between. [LSJ 20061207]"
+100083|Arcanum Investigator:
+  - His action is directed against the Methuselah controlling the equipment, not the minion it's on. [LSJ 20090324]"
 100084|Archon:
-  - "If a vampire blocks an Archon, he or she burns 1 blood regardless of which action the Archon was taking. [RTR 19960221]"
-  - "Multiple Archon cards provide different actions: if the vampire manage to unlock during the minion phase, he can perform the two actions. [RTR 20030519]"
-  - "The cost is cumulative if a vampire has multiple copies of the card on him. [LSJ 19980225]"
+  - If a vampire blocks an Archon, they burn 1 blood regardless of which action the Archon was taking. [RTR 19960221]
+  - "Each copy of this card provides its own action: if the vampire manage to unlock during the minion phase, he can perform the action more than once (once per copy). [RTR 20030519]"
+  - Burn blood effects are cumulative. [LSJ 19980225]
+  - A vampire with no blood can still block, they burn what they can. [LSJ 19970707]
 100085|Archon Investigation:
-  - "Must be played after blocks are declined, playing it implicitly declines block attempts. [LSJ 20070203]"
-  - 'Must be played before action resolution, before any modifier or reaction played "as the action would be successful" are played (eg. cannot be played after a {Spying Mission} on the vampire triggers). [LSJ 19980105]'
-  - "Targets the bleeding vampire (eg. costs one more against {Secure Haven}, cannot be played on {Mimir}). [LSJ 20010817] [PIB 20131013]"
+  - Must be played after blocks are declined, playing it implicitly declines block attempts. [LSJ 20070203]
+  - Must be played before action resolution, before any modifier or reaction played "as the action would be successful" are played (eg. cannot be played after a {Spying Mission} on the vampire triggers). [LSJ 19980105]
+  - Targets the bleeding vampire (eg. costs one more against {Secure Haven}, cannot be played on {Mimir}). [LSJ 20010817] [PIB 20131013]
 100087|Armor of Caine's Fury:
   - "[VAL] Prevents up to 2 damage, it can prevent less. [RTR 20041202]"
   - "[VAL] Can prevent 2 damage per round, from any strike, can prevent 2 times 1 damage from two different strikes. [ANK 20180117]"
+100088|Armor of Terra:
+  - "[vic], [VIC] Can be used by a non-slave Gragoyle. [LSJ 20011204-2]"
 100089|Armor of Vitality:
-  - "Prevents up to 3 damage, it can be used to prevent less. [RTR 20041202]"
-  - "Cannot be used if there is no damage to prevent. [LSJ 20001114]"
-  - "Unused prevention does not carry over. [LSJ 20001114]"
+  - Prevents up to 3 damage, it can be used to prevent less. [RTR 20041202]
+  - Cannot be used if there is no damage to prevent. [LSJ 20001114]
+  - Unused prevention does not carry over. [LSJ 20001114]
 100092|Army of Apparitions:
   - "[chi] Cannot be used during a referendum that is automatically passing. [PIB 20150105] [LSJ 19980107]"
+  - "[CHI] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {The Path of Paradox}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 100096|The Art of Love:
-  - "Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
+  - Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]
+  - Effects applied during the discard phase are applied before you return the ally. If you lose control of the ally before that, you do not return it. [ANK 20210313]
 100097|The Art of Memory:
-  - "The effect is applied after resolving the action, including after all combats. [LSJ 20031112]"
-  - "Can be used ot retrieve the action card itself (if any). [LSJ 20041115]"
+  - The effect is applied after resolving the action, including after all combats. [LSJ 20031112]
+  - Can be used ot retrieve the action card itself (if any). [LSJ 20041115]
 100100|Art's Traumatic Essence:
-  - "The action has no effect if the target is not unlocked anymore when it resolves. It is still considered successful and must be paid. [ANK 20181121]"
+  - The action has no effect if the target is not unlocked anymore when it resolves. It is still considered successful and must be paid. [ANK 20181121]
 100103|Asanbonsam Ghoul:
-  - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
-  - "If another effect also sets the range, the first to resolve has priority (eg. {Squirrel's Balance} resolves before, {Neutral Guard} resolves after). [PIB 20120214]"
+  - If another effect also sets the range, the first to resolve has priority (eg. {Squirrel Balance} resolves before, {Neutral Guard} resolves after). [PIB 20120214]
 100105|Ashes to Ashes:
   - "[thn], [THN] The end of combat is triggered by the vampire going to torpor - this can be interrupted by cards such as {Undying Tenacity} or {Undead Persistence}, but the vampire would still be wounded. [LSJ 20021122]"
   - "[thn], [THN] Cards that can be played at the end of combat (eg. {Amaranth}, {Decapitate}) can be played before combat ends. [LSJ 20011214-4]"
   - "[for] If played on a diablerie attempt (eg. {Amaranth}), the diablerie is unsuccessful. Another {Amaranth} can be played. [LSJ 19970224] [LSJ 20011214-4]"
-  - "[for] If played by an ally, the ally is burned instead of going to torpor. [ANK 20170412] [RBK 20181001-163]"
+  - "[for] If played by an ally, the ally is burned instead of going to torpor. [ANK 20170412] [RBK 20200701-6]"
   - "[for] Cannot be played when burned as a result of a Blood Hunt referendum. [LSJ 20070417]"
 100106|Ashur Tablets:
-  - "Can be played with no card in the ash heap. [PIB 20130119]"
+  - Can be played with no card in the ash heap. [PIB 20130119]
   - "Is played without announcing targets: they are only chosen once the third copy get into play. [LSJ 20091030]"
+100111|Aura Absorption:
+  - "[aus][REACTION] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Helena (ADV)}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 100112|Aura of Invincibility:
-  - "If the initial referendum does not pass, then the card is not put into play and the vampire playing it is not sent to torpor. [LSJ 20040730]"
+  - If the initial referendum does not pass, then the card is not put into play and the vampire playing it is not sent to torpor. [LSJ 20040730]
+  - Goes to the ash heap when played, if it has been removed when the referendum passes, it has no effect. [ANK 20220805]
 100117|Autonomic Mastery:
   - "[DOM] Is a hand strike, and its resolution is simultaneous with the opponent's strike, unlike a normal combat ends strike. The opponent's strike do damage. [LSJ 20071112]"
 100120|Aye:
-  - "Any frenzy card that targets/selects/chooses/affects the minion when played, is considered being played on the minion. [LSJ 20051113]"
+  - Any frenzy card that targets/selects/chooses/affects the minion when played, is considered being played on the minion. [LSJ 20051113]
+100121|Baal's Bloody Talons:
+  - The weapon does not burn if it is temporarily out of play (eg. {Kerrie}, {Dagger}). [LSJ 20100211-2]
 100123|Backflip:
-  - "The press can only be used during the current round. [TOM 19960521]"
+  - The press can only be used during the current round. [TOM 19960521]
 100124|Backstab:
-  - "Can be played at any time before strike resolution, including after both minions have selected their strikes. [LSJ 20000215]"
+  - Can be played at any time before strike resolution, including after both minions have selected their strikes. [LSJ 20000215]
 100125|Backstep:
-  - "The press can only be used during the current round. [TOM 19960521]"
+  - The press can only be used during the current round. [TOM 19960521]
 100127|Baleful Doll:
-  - "The bearer (if he unlocks normally) unlocks at the beginning of the unlock phase, before this effect can be used. [PIB 20151009] [RBK 20181001-4]"
+  - The bearer (if he unlocks normally) unlocks at the beginning of the unlock phase, before this effect can be used. [PIB 20151009] [RBK 20200701-1]
 100128|Baltimore Purge:
-  - "There is no time to use other effects between the choosing of the vampires and those vampires going to torpor. [LSJ 20050111]"
-  - "The effect during the unlock phase is not an action, you can choose a vampire with a {Secure Haven} on him. [PIB 20121028]"
+  - There is no time to use other effects between the choosing of the vampires and those vampires going to torpor. [LSJ 20050111]
+  - The effect during the unlock phase is not an action, you can choose a vampire with a {Secure Haven} on them. [PIB 20121028]
+  - If you control a ready Lasombra, the chosen vampires may not be older than the acting vampire. [ANK 20210529]
 100129|Bamba:
-  - "You only fetch one discipline card in total, not one in each of hand, library and ash heap. [LSJ 20090528-1]"
+  - You only fetch one discipline card in total, not one in each of hand, library and ash heap. [LSJ 20090528-1]
 100131|Banishment:
-  - "A banished vampire can return to play when it again has blood >= capacity on it at the end of its Methuselah's influence phase. [TOM 19951209]"
-  - "A banished vampire will remember all effects that had been applied to him, just as contested vampires do. This includes gained or lost titles. [RTR 20000501]"
-  - '"for the rest of the game" effects pointing at the Banished vampire from other sources will resume if and when the vampire comes back into play. [TOM 19960210]'
+  - Is not directed (eg. {Secure Haven} offers no protection). [ANK 20221019-3]
+  - A banished vampire can return to play when it again has blood >= capacity on it at the end of its Methuselah's influence phase. [TOM 19951209]
+  - A banished vampire will remember all effects that had been applied to them, just as contested vampires do. This includes gained or lost titles. [RTR 20000501]
+  - Cards on the banished vampire that change their capacity do not apply while uncontrolled, but additional blood for increased capacity does not drain off when they get controlled as these effects resume. [PIB 20140122]
+  - All cards on the vampire come back unlocked. [LSJ 20060908]
+  - Continuous effects targeting the banished vampire (eg. {The Rack}) resume if and when the vampire comes back into play. [TOM 19960210] [LSJ 20010809-2] [LSJ 20010809-3]
   - '"breaking any temporary control effects" means the vampire is placed in his last permanent controller''s uncontrolled region. [RTR 20000501]'
-  - "If the vampire is permanently controlled by a Methusalah other than his owner, it goes to that Methusalah uncontrolled region and is still controlled by him. It is removed from the game if that Methusalah is ousted and kept in game if his owner is ousted. [ANK 20200408-2]"
+  - If the vampire is permanently controlled by a Methuselah other than his owner, it goes to that Methuselah uncontrolled region and is still controlled by them. It is removed from the game if that Methuselah is ousted and kept in game if his owner is ousted. [ANK 20200408-2]
 100133|Banshee Ironwail:
-  - "Triggering the burn blood effect does not force the minion to strike with the weapon. [LSJ 19971215]"
+  - Triggering the burn blood effect does not force the minion to strike with the weapon. [LSJ 19971215]
+  - If a block is successful, the blood is burned before any other effect can be used (eg. {Promise of 1528}). REVERSAL of earlier rulings. [ANK 20210627]
 100134|Barrenness:
-  - "[mal] is unaffected by {Orun}. [MAL] is affected by {Orun}. [ANK 20180719-1]"
-  - "The burn option can be used if all your vampires with [mal] are in torpor. [LSJ 20091203]"
+  - "[mal] is unaffected by {Orun}. [MAL] is affected by {Orun} (add and substract before applying the minimum of 1). [ANK 20180719-1]"
+  - The burn option can be used if all your vampires with [mal] are in torpor. [LSJ 20091203]
 100135|The Barrens:
-  - 'Cannot be used when a card is played to draw a card that would cancel it "as it is played". [RTR 20040501]'
+  - Cannot be used when a card is played to draw a card that would cancel it "as it is played". [RTR 20040501]
 100137|Baseball Bat:
-  - "If put into play in a special way (eg. using {Concealed Weapon}), it is replaced immediately. [LSJ 20080702-2]"
-  - "If played normally, it is not replaced if {Gift of Bellona} is played after being blocked. [ANK 20200517-3]"
+  - If put into play in a special way (eg. using {Concealed Weapon}), it is replaced immediately. [LSJ 20080702-2]
+  - If played normally, it is not replaced if {Gift of Bellona} is played after being blocked. [ANK 20200517-3]
 100142|Bauble:
-  - "If it is burned by another mean than its effect, the weapon is not burned. [LSJ 20090113-1]"
-  - "It cannot be burned if the target equipment is not in play. [RTR 20080808]"
-  - "Still cannot be burned if the target equipment was burned and somehow returned to play. [LSJ 20040726] [ANK 20191031]"
+  - If it is burned by another mean than its effect, the weapon is not burned. [LSJ 20090113-1]
+  - It cannot be burned if the target equipment is not in play. [RTR 20080808]
+  - Still cannot be burned if the target equipment was burned and somehow returned to play. [LSJ 20040726] [ANK 20191031-2]
 100144|Bear-Baiting:
-  - "Damage is environmental. [RTR 19970630]"
+  - Damage is environmental. [RTR 19970630]
+  - Cannot be played if the blocker's crypt is empty. [LSJ 20031107]
   - "{Change of Target} can be played after Bear-Baiting (younger, older, or the same age). [LSJ 20040312]"
-  - "If the combat is canceled, the action is still blocked, {Mask of a Thousand Faces} cannot be used to continue it, but an effect can be used to continue the action as if unblocked (eg. {Crypt's Sons}, {Momentary Delay}). [LSJ 20090322] [ANK 20181003] [LSJ 20010803-2]"
+  - If the combat is canceled, the action is still blocked, {Mask of a Thousand Faces} cannot be used to continue it, but an effect can be used to continue the action as if unblocked (eg. {Crypt's Sons}, {Momentary Delay}). [LSJ 20090322] [ANK 20181003] [LSJ 20010803-2]
 100146|Beast Meld:
-  - '[ANI][PRO] Cards and effects that can be played "as the action is announced" (and only them) can be played before it. [ANK 20190425]'
+  - "[ani][pro] The damage prevention can only be used if the block is successful, and only in the resulting (block-induced) combat. It does not carry over to a follow-up combat (eg. [CEL] {Psyche!}). [LSJ 20010813] [LSJ 20010819-2]"
+  - "[ani][pro] The damage prevention is provided again if a second block happens on the same action (eg. after [PRO] {Form of Mist}). [LSJ 20010814-2]"
+  - '[ANI][PRO] Cards and effects that are played "as the action is announced" must be played before playing "regular" action modifier or reaction cards. [ANK 20190425]'
+  - "[ANI][PRO] Replace the action card (if any) before playing it. [ANK 20181208]"
+100147|The Becoming:
+  - If moved to the uncontrolled region (eg. by {Banishment}), it continues to be a vampire and can be influenced as a 1 capacity vampire. [RTR 19990712] [LSJ 20090625]
 100153|Bestial Vengeance:
-  - "Damage is environmental. [RTR 19970630]"
-  - "Bestial Vengeance's damage is inflicted whether or not the opposing minion's strike burns the retainer. [LSJ 20090616]"
+  - Damage is environmental. [RTR 19970630]
+  - Bestial Vengeance's damage is inflicted whether or not the opposing minion's strike burns the retainer. [LSJ 20090616]
 100156|Betrayer:
-  - "The affected Methuselah is named when the card is played. [RTR 19980928]"
-  - "Each of their turns, the person subjected to Betrayer can name a vampire. If the guess is correct, Betrayer is burned. [RTR 19941109]"
-  - "Is cumulative. A player can be damaged by multiple Betrayers each turn. A Methuselah targeted by more than one Betrayer would have to pay 1 pool for each Betrayer in order to burn them, even if the same vampire is the betrayer in each case. [RTR 19941109]"
-  - "If the vampire chosen for Betrayer is burned, so is Betrayer. If the vampire chosen for Betrayer becomes contested, Betrayer is nullified until the contest is resolved, at which time the Betrayer is reactivated. If a player takes control of the vampire that is the target of the betrayer, that player takes the pool loss. [RTR 19941109]"
-  - "You select an uncontrolled vampire when you play the card. If you have a choice (more than one of your uncontrolled vampires is controlled by the other Methuselah), you still have to choose just one of them to be the Betrayer. [LSJ 19990419]"
+  - The affected Methuselah is named when the card is played. [RTR 19980928]
+  - Each of their turns, the person subjected to Betrayer can name a vampire. If the guess is correct, Betrayer is burned. [RTR 19941109]
+  - "Is cumulative: a player can be damaged by multiple Betrayers each turn. A Methuselah targeted by more than one Betrayer would have to pay 1 pool for each Betrayer in order to burn them, even if the same vampire is the betrayer in each case. [RTR 19941109]"
+  - If the vampire chosen for Betrayer is burned, so is Betrayer. If the vampire chosen for Betrayer becomes contested, Betrayer is nullified until the contest is resolved, at which time the Betrayer is reactivated. If a player takes control of the vampire that is the target of the betrayer, that player takes the pool loss. [RTR 19941109]
+  - You select an uncontrolled vampire when you play the card. If you have a choice (more than one of your uncontrolled vampires is controlled by the other Methuselah), you still have to choose just one of them to be the Betrayer. [LSJ 19990419]
 100159|Big Game:
   - '"that minion" refers to the target and "this minion" to the acting minion. [ANK 20180518]'
 100160|Bima:
-  - "The discipline needs not be announced when Bima is played. The replacement card can be used if it is a discipline. [PIB 20150418]"
+  - The discipline needs not be announced when Bima is played. The replacement card can be used if it is a discipline. [PIB 20150418]
   - '"that Discipline" refers to the card on Bima. If the card is no longer there, then the effect cannot be used. [LSJ 20071006]'
-  - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
-  - "If it uses its last life to pay for an action, the action still resolves fully. If that leads to an oust, the oust is resolved before resolving effects triggered by the fact that the Bima burns. [LSJ 20080512]"
+  - If it uses its last life to pay for an action, the action still resolves fully. If that leads to an oust, the oust is resolved before resolving effects triggered by the fact that the Bima burns. [LSJ 20080512]
 100161|Bind the Night-Walker:
-  - "The action ends immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719]"
+  - The action ends immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719]
+  - The action has reached resolution, so is subject to NRA (Non Repeatable Action) rules. [ANK 20211015]
 100166|Black Gloves:
-  - "Damage done to the bearer is environmental. [LSJ 19970801]"
+  - Damage done to the bearer is environmental. [LSJ 19970801]
 100171|Black Sunrise:
-  - "Can be used by a vampire who is already attempting to block. [ANK 20181122-2]"
-  - '[QUI] Does not ignore the normal prey, predator or target restrictions. Read: "This vampire unlocks and attempts to block". [ANK 20180623]'
+  - Can be used by a vampire who is already attempting to block. [ANK 20181122-2]
+  - "[QUI] Cannot be used if the vampire cannot attempt to block the action (eg. {Daring the Dawn}). [LSJ 20010714-2]"
+  - "[QUI] Does not ignore the normal prey, predator or target restrictions. [ANK 20180623]"
+  - "[QUI] The block attempt and subsequent combat still happen if the action lacks a suitable target because of the unlock (eg. {Ambush}). [LSJ 20090514]"
 100172|The Black Throne:
-  - "The contract effect can be used even if the target is burned or if the contract is burned when the target leaves the ready region (eg. {Priority Contract}). [PIB 20150512]"
-  - "The contract effect can be used if a minion with a contract leaves the ready region because his controller is ousted. [ANK 20180129-2]"
+  - The contract effect can be used even if the target is burned or if the contract is burned when the target leaves the ready region (eg. {Priority Contract}). [PIB 20150512]
+  - The contract effect can be used if a minion with a contract leaves the ready region because his controller is ousted. [ANK 20180129-2]
 100174|Blade Clot:
-  - "Multiple clot counters can be placed on the same vampires if he his hit multiple times. When rescued by an older vampire, all clot counters are burned. [PIB 20150122]"
+  - Multiple clot counters can be placed on the same vampires if he his hit multiple times. When rescued by an older vampire, all clot counters are burned. [PIB 20150122]
 100176|Blade of Enoch:
-  - "Can be equipped by a vampire with capacity less than 6, although he cannot use it to strike and does not gain immunity to frenzy cards. [LSJ 20030607]"
+  - Can be equipped by a vampire with capacity less than 6, although he cannot use it to strike and does not gain immunity to frenzy cards. [LSJ 20030607]
 100177|Blanket of Night:
   - "[OBT] Can only be played by the controller of the acting minion. [LSJ 19990425]"
   - "[OBT] Multiple copies can be played by different minions on the same action. [ANK 20200515]"
 100180|Blessed Blade:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
-  - "A minion who maneuvers with a weapon (eg. {Blade of Bellona}) may still use Blessed Blade to strike with that weapon as his initial strike that round. [ANK 20180704] [LSJ 20050304]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
+  - A minion who maneuvers with a weapon (eg. {Blade of Bellona}) may still use Blessed Blade to strike with that weapon as his initial strike that round. [ANK 20180704] [LSJ 20050304]
+  - '[val][REFLEX] Cards are not replaced during the "as played" window. [LSJ 20061013]'
+  - '[val][REFLEX] If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
+100181|Blessed Resilience:
+  - Only a controlled vampire can be burned from play. Uncontrolled and contested vampires do not qualify. [ANK 20210813]
 100182|Blessing of Chaos:
-  - "The prohibition to play certain cards applies from the moment the vampire attempts to block until the end of the action, even if he fails to block. [LSJ 20080818]"
+  - The prohibition to play certain cards applies from the moment the vampire attempts to block until the end of the action, even if he fails to block. [LSJ 20080818]
 100183|Blessing of Durga Syn:
-  - "Cannot be used if there is no equipment to steal. [RTR 19980928]"
+  - Cannot be used if there is no equipment to steal. [RTR 19980928]
 100184|Blessing of the Beast:
-  - "The number of cards to put on it is announced when the card is played, they must be in hand before drawing the replacement for this card. [PIB 20150428] [LSJ 20100206-2]"
+  - The number of cards to put on it is announced when the card is played, they must be in hand before drawing the replacement for this card. [PIB 20150428] [LSJ 20100206-2]
 100185|Blessing of the Name:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 100189|Bliss:
   - "[dom][pre] [COMBAT] Can be used during a combat by a vampire in torpor. [LSJ 20020416]"
-  - "[dom][pre] [COMBAT][REACTION] Can be played by a minion of a Methusalah not involved in the current combat. [ANK 20181101]"
+  - "[dom][pre] [COMBAT][REACTION] Can be played by a minion of a Methuselah not involved in the current combat. [ANK 20181101]"
+  - '[dom][pre] [COMBAT][REACTION] Cards are not replaced during the "as played" window. [LSJ 20061013]'
+  - '[dom][pre] [COMBAT][REACTION] If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
 100190|Blissful Agony:
   - "[val] Damage is environmental. [RTR 19970630]"
   - '[val] Damage is inflicted even against a dodge. A "strike: combat ends" ends combat before damage is applied, as will a combattant going to torpor during first strike. [RTR 19941109] [TOM 19951216] [PIB 20140324] [ANK 20200422]'
   - "[VAL] If dodged, there is no new combat. [LSJ 20051020]"
+  - "[VAL] Cannot be played against an ally. [PIB 20111105]"
   - "[VAL] In the new combat, the opponent goes first. [LSJ 20011214-3] [LSJ 20031212]"
   - "[VAL] Cannot be used to start a new combat if there is already a pending combat queued. [RTR 20020501]"
   - "[VAL] Cannot be used to start a new combat with a vampire on his way to torpor. [LSJ 20100604-1]"
+  - "[VAL] If both vampires play it, the acting Methuselah decides which resolves first. The other is lost. [PIB 20120225] [LSJ 20011215]"
   - "[ani] Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
 100192|Blood Agony:
-  - "Must be played before strike resolution and damage prevention in order to affect the current strike (can be played after both strikes have been chosen). [RTR 19960112]"
+  - Must be played before strike resolution and damage prevention in order to affect the current strike (can be played after both strikes have been chosen). [RTR 19960112]
 100195|Blood Brother Ambush:
-  - "Can be used by a Brujah Antitribu taking an action while in torpor. If this happens, the blocker loses the opportunity to commit diablerie. [RTR 20010710]"
-  - "No other modifier can be played afterwards, combat begins immediately. [LSJ 20010806-2]"
+  - Can be used by a Brujah Antitribu taking an action while in torpor. If this happens, the blocker loses the opportunity to commit diablerie. [RTR 20010710]
+  - No other modifier can be played afterwards, combat begins immediately. [LSJ 20010806-2]
+  - "The vampire playing it is not considered having burned a minion (eg. for {Taking the Skin: Minion}), but the opponent is. [LSJ 20090922] [ANK 20220916]"
 100199|Blood Doll:
-  - "Can be used when the vampire is in torpor. [PIB 20150522]"
+  - Can be used when the vampire is in torpor. [PIB 20150522]
 100201|Blood Fury:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
-  - "Does not protect the target from self-inflicted damage from a weapon. [LSJ 19980216]"
-  - "If the opponent dodges this strike, his weapons are unaffected and do damage this round. [LSJ 20040928]"
-  - "A weapon strike done with first strike is unaffected (unless Soul Burn is used with first strike too). [LSJ 20040928]"
-  - "Only nullify the weapon damage when it resolves, an opponent can successfully use {Rötschreck} after declaring a strike with {Ivory Bow}. [ANK 20170519]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
+  - Does not protect the target from self-inflicted damage from a weapon. [LSJ 19980216]
+  - If the opponent dodges this strike, his weapons are unaffected and do damage this round. [LSJ 20040928]
+  - A weapon strike done with first strike is unaffected (unless Soul Burn is used with first strike too). [LSJ 20040928]
+  - Only nullify the weapon damage when it resolves, an opponent can successfully use {Rötschreck} after declaring a strike with {Ivory Bow}. [ANK 20170519]
+  - The opponent cannot play [for] prevention cards (eg. for cycling). [LSJ 20050628]
 100203|Blood of Acid:
-  - "Damage from Blood of Acid is environmental. [RTR 19970630] [LSJ 20020708]"
-  - "Environmental damage is not counted by Blood of Acid. [RTR 19970630]"
-  - "Damage is applied even if the wielder goes to torpor as a result of the opponent's strike. [PIB 20150426]"
-  - "Proceed with strikes damage prevention (acting player first), then the target can prevent Blood of Acid damage, if any. All the damage is applied (and the blood lost) at once, after all preventions.[ANK 20170427] [LSJ 20040805]"
+  - Damage from Blood of Acid is environmental. [RTR 19970630] [LSJ 20020708]
+  - Environmental damage is not counted by Blood of Acid. [RTR 19970630]
+  - Damage is applied even if the wielder goes to torpor as a result of the opponent's strike. [PIB 20150426]
+  - Proceed with strikes damage prevention (acting player first), then the target can prevent Blood of Acid damage, if any. All the damage is applied (and the blood lost) at once, after all preventions.[ANK 20170427] [LSJ 20040805]
   - "The damage is done after the strike damage is done: a single instantaneous prevention card (eg. {Soak}) cannot prevent both, although lingering damage prevention (eg. {Apparition}) could. [ANK 20200517-2]"
 100205|Blood of the Cobra:
   - "[QUI] If the chosen strike says to make a hand strike or a melee weapon strike, then the strike is ranged, but the hand or melee weapon portion of the strike is still only effective at close range. [RTR 20010710]"
 100208|Blood Rage:
   - "[THA] Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
-  - "If the opponent dodges this strike, his weapons are unaffected and do damage this round. [LSJ 20040928]"
-  - "Does not protect the target from self-inflicted damage from a weapon. [LSJ 19980216]"
+  - If the opponent dodges this strike, his weapons are unaffected and do damage this round. [LSJ 20040928]
+  - Does not protect the target from self-inflicted damage from a weapon. [LSJ 19980216]
+  - The opponent cannot play [for] prevention cards (eg. for cycling). [LSJ 20050628]
 100209|Blood Shield:
-  - "The blood is burned by the opponent when the owner prevents damage, immediately, before loosing blood to heal strike damage. Depending on the sequencing order, it can be before or after he has the opportunity to play damage prevention himself. [LSJ 20090528-1]"
+  - The blood is burned by the opponent when the owner prevents damage, immediately, before loosing blood to heal strike damage. Depending on the sequencing order, it can be before or after he has the opportunity to play damage prevention themselves. [LSJ 20090528-1]
 100212|Blood Tears of Kephran:
-  - "Prevents up to 2 damage, it can be used to prevent less. [RTR 20041202]"
+  - Prevents up to 2 damage, it can be used to prevent less. [RTR 20041202]
 100213|Blood Tempering:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 100214|Blood to Water:
-  - "Must be played after range is chosen, can be played before or after strikes are chosen. [ANK 20200703] [LSJ 20031008]"
+  - Must be played after range is chosen, can be played before or after strikes are chosen. [ANK 20200703] [LSJ 20031008]
+100215|Blood Trade:
+  - Does not prevent {Consanguineous Boon} to be played. [LSJ 20040531-2]
+100216|Blood Turnip:
+  - The transferred blood or life is converted to the fitting type (blood or life) depending on the opponent (vampire or ally). [LSJ 20080704]
+  - When entering combat with an opposing Anarch, they get the blood and decide where Blood Turnip goes (the blood does not follow the Blood Turnip). [LSJ 20080704]
 100217|Blood Weakens:
-  - "You do not replace cards that require a discipline during any action. [ANK 20201015]"
+  - You do not replace cards that require a discipline during any action. [ANK 20201015]
 100218|Bloodbath:
-  - "The target does not get an extra vote if it already has or subsequently gains a title. If the target loses his title, then he again gets his extra vote. [LSJ 19970224]"
+  - The target does not get an extra vote if it already has or subsequently gains a title. If the target loses his title, then he again gets his extra vote. [LSJ 19970224]
 100219|Bloodform:
   - "[VIC] The press can only be used during the current round. [TOM 19960521]"
   - "[VIC] Immune means damage is not inflicted, even if non-preventable or outside combat. [LSJ 20010627] [LSJ 20010629] [LSJ 20090304-1]"
 100221|Blooding by the Code:
-  - "Can be played on a vampire with superior Valeren [VAL]. [LSJ 20051012]"
+  - Can be played on a vampire with superior Valeren [VAL]. [LSJ 20051012]
 100224|Bloodstorm of Chorazin:
-  - "The action ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20200207]"
+  - The action ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20200207]
 100228|Body Arsenal:
-  - "Must be played before strike resolution and damage prevention in order to affect the current strike. (can be played after both strikes have been chosen) [RTR 19960112]"
+  - Must be played before strike resolution and damage prevention in order to affect the current strike. (can be played after both strikes have been chosen) [RTR 19960112]
 100229|Body Bag:
-  - "Can be equipped by a non-Anarch and would still count as a haven, although the rest of his effect does not apply. [LSJ 20030607]"
+  - Can be equipped by a non-Anarch and would still count as a haven, although the rest of his effect does not apply. [LSJ 20030607]
 100231|Body of Sun:
   - "[pro] Damage done to the striking minion is environmental. [LSJ 19970801]"
 100232|Bollix:
+  - '[pre] Cards are not replaced during the "as played" window. [LSJ 20061013]'
+  - '[pre] If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
   - "[tha] Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - "[tha] The opponent cannot play [for] prevention cards (eg. for cycling). [LSJ 20050628]"
 100233|Bomb:
-  - "Using the provided action does not force the minion to strike with it if he is blocked. [LSJ 19971215]"
-  - "Damage done to the bearer is environmental. [LSJ 19970801]"
-  - "The provided action ends with no effect if the acting minion does not possess the equipment when the action resolves. It is still considered successful if not blocked. [RTR 19960221] [LSJ 20020926]"
+  - Using the provided action does not force the minion to strike with it if he is blocked. [LSJ 19971215]
+  - Damage done to the bearer is environmental. [LSJ 19970801]
+  - The provided action ends with no effect if the acting minion does not possess the equipment when the action resolves. It is still considered successful if not blocked. [RTR 19960221] [LSJ 20020926]
   - 'When used as a strike, it does not burn if combat ends before it resolves (eg. if the opponent uses a "strike: combat ends"). [LSJ 19981006] [LSJ 20001127-2] [LSJ 20010806-1]'
 100235|Bond with the Mountain:
   - "[tha] The press can only be used during the current round. [TOM 19960521]"
   - "[vis] [VIS] The unlock effect takes place before the end of combat. [RTR 19970630]"
   - "[vis] [VIS] The vampires still unlock if an effect continues the combat or begins a new combat. [RTR 20020501] [LSJ 20030717]"
 100236|Bonding:
   - "[DOM] Cannot be used if you do not need the stealth at the time you play it. [TOM 19951109]"
   - "[DOM] Cannot be used to increase the stealth of a non-bleed action. [LSJ 19980824] [RTR 19941109]"
 100237|Bone Spur:
-  - "Must be played before strike resolution and damage prevention in order to affect the current strike. (can be played after both strikes have been chosen) [RTR 19960112]"
+  - Must be played before strike resolution and damage prevention in order to affect the current strike. (can be played after both strikes have been chosen) [RTR 19960112]
 100238|Bonecraft:
-  - "The rest of the effect applies if the damage is prevented, it does not if it is dodged. [LSJ 19990106-2]"
+  - The rest of the effect applies if the damage is prevented, it does not if it is dodged. [LSJ 19990106-2]
 100239|The Book of Going Forth by Night:
-  - "Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
+  - Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]
+  - Does not apply to Imbued getting incapacitated. [ANK 20220816]
 100241|Botched Move:
-  - "Damage is environmental. [RTR 19970630]"
-  - "Can be played against any combat card, even those played at the end of the round. [LSJ 20070214]"
+  - Damage is environmental. [RTR 19970630]
+  - Can be played against any combat card, even those played at the end of the round. [LSJ 20070214]
+  - Is not affected by a {Dark Influences} in play. [LSJ 20081120-2]
 100245|Brainwash:
-  - "Transfers may not be made to the vampire - neither to put blood on nor to move blood off. [RTR 19950413]"
+  - Only transfers are forbidden, other mouvements are not affected (eg. {Govern the Unaligned} at superior [DOM]). The vampire can become controlled if it reaches capacity, Brainwash stays on it (if {Banishment} is used, the effect resumes). [LSJ 20010211]
+  - You can only target a vampire by position, the target Methuselah can shuffle their crypt. If you have no clue (tokens, cards) about a previously revealed vampire's position, you have to take a bet. In case multiple copies of the same vampire are subject to different effects, the controller must track them, but they can do it secretly (eg. {Banishment} was used on one that would benefit from {The Rack} if controlled again). [LSJ 20040728]
 100250|Breath of the Dragon:
-  - "Damage done to the striking minion is environmental. [LSJ 19970801]"
+  - Damage done to the striking minion is environmental. [LSJ 19970801]
+100253|Brick Laying:
+  - "[POT] If it burns an ally as a result, this counts as a Ⓓ action burning an ally (eg. Trophies, {Predator's Transformation}). [ANK 20220507]"
 100254|Brigitte Gebauer:
-  - "She can lock to use her ability the turn she is recruited. [ANK 20180517]"
+  - She can lock to use her ability the turn she is recruited. [ANK 20180517]
 100257|Brother's Blood:
-  - "Can be played even if there is no damage yet, can be used to heal and prevent destruction at the same time. [LSJ 20100527]"
+  - Can be played even if there is no damage yet, can be used to heal and prevent destruction at the same time. [LSJ 20100527]
 100260|Brujah Debate:
-  - "If more than one Brujah shares the highest capacity amount, the controller chooses which of them to lock during her master phase. [LSJ 19980224]"
-  - "Can lock a locked Brujah. [LSJ 20010508]"
+  - If more than one Brujah shares the highest capacity amount, the controller chooses which of them to lock during her master phase. [LSJ 19980224]
+  - Can lock a locked Brujah. [LSJ 20010508]
 100261|Brujah Frenzy:
-  - "Cannot be played if there is no suitable minion for the Brujah to enter combat with. [RTR 19980928]"
-  - "There is no time to play further action modifiers or reactions before combat begins. [TOM 19950829]"
+  - Cannot be played if there is no suitable minion for the Brujah to enter combat with. [RTR 19980928]
+  - There is no time to play further action modifiers or reactions before combat begins. [TOM 19950829]
   - "Only causes the affected Brujah to enter combat with a second minion: that minion is not considered to be blocking the Brujah in any way. [RTR 19950906]"
-  - 'Must select a "ready, unlocked minion" to send the Brujah into combat with. It cannot be played if there are no such minions. [RTR 19951110]'
-  - "Can only be played on a ready acting Brujah. [RTR 19980623]"
+  - Must select a "ready, unlocked minion" to send the Brujah into combat with. It cannot be played if there are no such minions. [RTR 19951110]
+  - Can only be played on a ready acting Brujah. [RTR 19980623]
 100264|Brute Force:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 100267|Bundi:
-  - "Preventing damage with it does not force the minion to strike with it. [LSJ 19971215]"
-  - "Inherits all of the properties of the base hand strike. [TOM 19960225] [LSJ 20071020]"
-  - "Effects that affect or improve hand strikes can be used on its strike. [LSJ 20071020]"
+  - Preventing damage with it does not force the minion to strike with it. [LSJ 19971215]
+  - Inherits all of the properties of the base hand strike. [TOM 19960225] [LSJ 20071020]
+  - Effects that affect or improve hand strikes can be used on its strike. [LSJ 20071020]
   - 'Cannot be used with a strike card that reads: "Strike: make a hand strike." but can be use it with a strike card that reads "strike: make a weapon strike" (eg. {Brute Force}). In that case, the strike is still considered a hand strike (ie. can be chosen if {Immortal Grapple} has been played) [LSJ 20080702-1] [LSJ 20090114]'
 100271|Burning Wrath:
-  - "All the damage is aggravated. [LSJ 20020122]"
+  - All the damage is aggravated. [LSJ 20020122]
 100273|Burst of Sunlight:
-  - "Damage done to the striking minion is environmental. [LSJ 19970801]"
+  - Damage done to the striking minion is environmental. [LSJ 19970801]
 100274|Business Pressure:
-  - "Each Methuselah must decide how much pool to burn for it during the resolution of the effect. It does not give an ability for the rest of the political action. However, there can be some give and take during the resolution of the effect. For example, each Methuselah can choose to burn one pool at a time as pool is burned for votes. [RTR 19960530]"
+  - Each Methuselah must decide how much pool to burn for it during the resolution of the effect. It does not give an ability for the rest of the political action. However, there can be some give and take during the resolution of the effect. For example, each Methuselah can choose to burn one pool at a time as pool is burned for votes. [RTR 19960530]
 100275|Cadet:
-  - "The target vampire is not Black Hand if he is not Sabbat. [LSJ 20070322]"
+  - The target vampire is not Black Hand if he is not Sabbat. [LSJ 20070322]
+100279|Call of the Hungry Dead:
+  - "[NEC] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {The Path of Bone}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 100280|Call the Great Beast:
-  - "The action to put a counter on the card is an action that requires Baali. [LSJ 20050112]"
+  - The action to put a counter on the card is an action that requires Baali. [LSJ 20050112]
+  - The action to put the 11th counter on it is an action to put a vampire into play, a sterile vampire cannot do it (eg. {Blood Cult Awareness Network} gives it -1 stealth). [LSJ 20060815] [LSJ 20011212]
 100281|Call the Lamprey:
   - "[OBT] Can be played against a vampire with no blood. [RTR 20010711]"
 100282|Call the Wild Hunt:
-  - "At superior, you choose X and then discard that many animals form your hand and cannot use any animals drawn to replace the ones you are discarding as further discards. [LSJ 20060215]"
-  - "The damage inflicted by the superior is environmental damage. [LSJ 20060217]"
+  - Does not render immune to a previously-played Frenzy card. [LSJ 20040210]
+  - "[ANI][PRO] you choose X and then discard that many animals form your hand and cannot use any animals drawn to replace the ones you are discarding as further discards. [LSJ 20060215]"
+  - "[ANI][PRO] The damage is environmental. [LSJ 20060217]"
 100284|Camarilla Exemplary:
-  - "Burn blood effects are cumulative. [LSJ 19980225]"
-  - "A vampire with no blood can still block, he burns what he can. [LSJ 19970707]"
-  - "The same vampire can be chosen multiple times if multiple copies are played. [LSJ 19970707]"
+  - Burn blood effects are cumulative. [LSJ 19980225]
+  - A vampire with no blood can still block, they burn what they can. [LSJ 19970707]
+  - The same vampire can be chosen multiple times if multiple copies are played. [LSJ 19970707]
 100286|Camarilla Vitae Slave:
-  - "The vampire keeps his chosen Discipline at superior until his controller's next unlock phase even if the retainer is burned or stolen. [LSJ 19970224]"
+  - The vampire keeps his chosen Discipline at superior until his controller's next unlock phase even if the retainer is burned or stolen. [LSJ 19970224]
 100287|Camera Phone:
-  - "The provided action ends with no effect if the acting minion does not possess the equipment when the action resolves. It is still considered successful if not blocked. [RTR 19960221]"
+  - The provided action ends with no effect if the acting minion does not possess the equipment when the action resolves. It is still considered successful if not blocked. [RTR 19960221]
 100289|Can't Take it with You:
-  - "Each Methuselah burns 1 pool for each equipment, each location and each retainer. [LSJ 20071005-2]"
+  - Each Methuselah burns 1 pool for each equipment, each location and each retainer. [LSJ 20071005-2]
 100290|Canine Horde:
   - "[ANI] Cannot be used if there is no equipment to destroy. [RTR 19980928]"
 100292|Capitalist:
-  - 'Cards and effects that can be played "after resolution" (and only them) can be played after the gain blood effect. [ANK 20190113]'
+  - Cards and effects that can be played "after resolution" (and only them) can be played after the gain blood effect. [ANK 20190113]
 100293|Car Bomb:
-  - "Is to be used when the action is announced. [PIB 20150820]"
-  - "If the action ends, no other action modifier or reaction can be played afterwards. [RTR 20180719]"
+  - Is to be used when the action is announced. [PIB 20150820]
+  - The action fails. Action modifiers and reactions can be played afterwards (eg. {Zephyr}). [RTR 20180719] [ANK 20220118]
+  - The action has reached resolution, so is subject to NRA (Non Repeatable Action) rules. [ANK 20211015]
 100298|Carlton Van Wyk:
-  - "He can use his ability to burn a vampire who has committed diablerie the turn she is recruited. [ANK 20180517]"
+  - He can use his ability to burn a vampire who has committed diablerie the turn she is recruited. [ANK 20180517]
 100303|Carver's Meat Packing and Storage:
-  - "The effect to burn a hostage counter can be done only once per turn. [ANK 20200729] [RBK 20181001-11]"
-100306|Catacombs:
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
+  - The effect to burn a hostage counter can be done only once per turn. [ANK 20200729] [RBK 20200701-4]
 100307|Catatonic Fear:
   - "[PRE] Damage is done by the vampire (not environmental). [RTR 19970630] [LSJ 19990723]"
   - "[PRE] The damage is inflicted after the end of combat. [RTR 19970630]"
   - "[PRE] If the combat continues or a new combat begins, no damage is done. [RTR 20020501]"
   - "[PRE] If the strike is dodged, no damage is done. [LSJ 19980526] [RTR 20041202] [LSJ 20070124]"
   - "[PRE] Is a damage dealing strike and can be modified by effects like {Target Vitals} or {Dam the Heart's River}.  [ANK 20170111] [LSJ 20071011]"
 100308|Cats' Guidance:
   - "[ani] Is played after combat [RTR 19980623]"
   - "[ani] Can not be played if the vampire is in torpor, for example if he went into torpor during the combat resulting from the block. [LSJ 20000103]"
 100309|Cauldron of Blood:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 100310|Cavalier:
-  - 'Cards and effects that can be played "after resolution" (and only them) can be played after the unlock effect. [ANK 20190113]'
-  - "Takes the modified cost into account if it has been modified (eg. by {The Slow Withering} or {The Ankara Citadel, Turkey}). [PIB 20150725] [LSJ 20100429]"
+  - Cards and effects that can be played "after resolution" (and only them) can be played after the unlock effect. [ANK 20190113]
+  - Takes the modified cost into account if it has been modified (eg. by {The Slow Withering} or {The Ankara Citadel, Turkey}). [PIB 20150725] [LSJ 20100429]
 100316|Chain of Command:
-  - "Cannot bring more than one copy of a unique vampire out, by the rule prohibiting self-contesting. [LSJ 20040722]"
-  - "If a commanded vampire is burned (eg. {Daring the Dawn}), he is not brought back to the crypt. [LSJ 20040616]"
+  - Cannot bring more than one copy of a unique vampire out, by the rule prohibiting self-contesting. [LSJ 20040722]
+  - If a commanded vampire is burned (eg. {Daring the Dawn}), he is not brought back to the crypt. [LSJ 20040616]
+  - If none of the vampires can bleed (eg. {Aabbt Kindred}), they all go to the bottom of the crypt. [LSJ 20040518-2]
 100319|Chalice of Kinship:
-  - "The provided action ends with no effect, if the acting minion does not possess the equipment when the action resolves. It is still considered successful if not blocked. [RTR 19960221]"
+  - The provided action ends with no effect, if the acting minion does not possess the equipment when the action resolves. It is still considered successful if not blocked. [RTR 19960221]
 100320|Chameleon:
   - "Cannot be used on a vampire who merged last turn: merging is not entering play. [PIB 20150728]"
-  - "Can be used on one of your own vampire to make it Anarch. [LSJ 20080803-2]"
+  - Can be used on one of your own vampire to make it Anarch. [LSJ 20080803-2]
 100321|Chameleon's Colors:
   - "[spi] The optional press can only be used during the current round. [TOM 19960521]"
   - '[SPI] If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]'
-  - '[SPI] If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
+  - '[SPI] If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
   - '[SPI] An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]'
   - '[SPI] "continue as if unblocked" moves the action card from the ash heap (where it went when the action was blocked) to limbo (where it should be if the action is not blocked). If the action card is not in the ash heap, then the action cannot be continued. [LSJ 20070808-1]'
   - '[SPI] If the combat continues or a new combat occurs, the "action continues as if unblocked" effect is lost. [LSJ 19980109] [RTR 20020501]'
 100322|Champion:
   - "[REACTION] Can be used only when reactions can be used (unlocked or with a wake effect). It does not count as playing a reaction card. [LSJ 20070403] [LSJ 20070413]"
   - "[REACTION] The action still continues until the end of combat. The acting minion stays the same, effects applied during the action still applies during combat. [LSJ 20070217]"
   - "[REACTION] Modifiers and reactions that can be used at the end/after an action can still be used after combat. [LSJ 20041022]"
+  - "[REACTION] The action has reached resolution, so is subject to NRA (Non Repeatable Action) rules. [ANK 20211015]"
 100323|Change of Target:
-  - "The action has reached resolution, so is subject to NRA (Non Repeatable Action) rules. [LSJ 20070709]"
-  - 'Actions without card (provided by the rulebook) are not "the same" as actions provided by cards (played or in play). [LSJ 20060522]  [LSJ 20060824] [LSJ 20080725] [LSJ 20090617]'
+  - The action has reached resolution, so is subject to NRA (Non Repeatable Action) rules. [LSJ 20070709]
+  - Actions without card (provided by the rulebook) are not "the same" as actions provided by cards (played or in play). [LSJ 20060522]  [LSJ 20060824] [LSJ 20080725] [LSJ 20090617]
   - "Actions without card (provided by the rulebook) can be repeated if they have different targets. Equipping from a minion targets the equipments: if one equipment is the same, the action is the same. [RTR 19950509] [LSJ 20080710] [ANK 20200502]"
-  - "Actions provided by cards in play are not the same if the card is not the same, even if the cards have the same name. [LSJ 20080725]"
-  - "Is played after a minion successfully blocks but before the blocker is locked and combat begins. It cannot be used if the action is ended without being blocked. [LSJ 19980224] [RTR 19991206]"
-  - "Effects triggered when the action is blocked are still applied (eg. {Unleash Hell's Fury}, {Truth of Blood}, {Aching Beauty}). [RTR 19991206]"
-  - "No other modifier can be played afterwards: the action is ended, it cannot be modified anymore. [LSJ 20010803-1] [RTR 20180719]"
-  - "If the acting minion was performing a mandatory action, he unlocks and is stuck and cannot act: he should but cannot take the mandatory action. [LSJ 19980112]"
-  - "If used when blocked while leaving torpor, the action ends immediately and the blocker does not get an opportunity for diablerie. [LSJ 20050105-2]"
+  - Actions provided by different cards in play are not the same, even if the cards have the same name. [LSJ 20080725]
+  - Is played after a minion successfully blocks, before the blocker is locked and combat begins. It cannot be used if the action is ended without being blocked. [LSJ 19980224] [RTR 19991206]
+  - Effects triggered when the action is blocked are still applied (eg. {Unleash Hell's Fury}, {Truth of Blood}, {Aching Beauty}). [RTR 19991206]
+  - "No other modifier or reaction can be played afterwards: the action has ended. [LSJ 20010803-1] [RTR 20180719]"
+  - If the card prevents the acting minion from performing a mandatory action, he is stuck and cannot act. [LSJ 19980112]
+  - If used while leaving torpor, the blocker does not get an opportunity for diablerie. [LSJ 20050105-2]
 100325|Changeling Skin Mask:
-  - "The superior Obfuscate is not optional. [RTR 19980707] [LSJ 19980722]"
+  - The superior Obfuscate is not optional. [RTR 19980707] [LSJ 19980722]
 100326|Chanjelin Ward:
-  - "Applies to an action if any one of its targets would be enough to enable his effect. [LSJ 20080809-2] [KOT 20081119]"
+  - Applies to an action if any one of its targets would be enough to enable his effect. [LSJ 20080809-2] [KOT 20081119]
 100328|Channeling the Beast:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 100330|Charge of the Buffalo:
   - "[for] If the target unlocks and the action is not blocked, it is successful but has no effect. [LSJ 20070411] [LSJ 20090514]"
-  - "No other effect can be used to reset the range. Skip the determine range step on that round, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]"
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - No other effect can be used to reset the range. Skip the determine range step on that round, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
+100333|Charismatic Aura:
+  - '[aus][pre] Cards are not replaced during the "as played" window. [LSJ 20061013]'
+  - '[aus][pre] If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
+  - "[aus][pre] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Adana de Sforza}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 100334|Charming Lobby:
-  - 'During the referendum that passes automatically, no "during a political action" and "during a referendum" effect can be played and effects that operate on the number of votes that the referendum passed by have no effect. [LSJ 19980107]'
-  - "A bloodhunt vote does not qualify. [TOM 19950921]"
-  - "The next referendum (passing automatically) can be called by another Methuselah's vampire. [PIB 20110719]"
-  - 'Cannot be used on effects that allow to play a political action card "as if from hand" (eg. {Echo of Harmonies}) [ANK 20201029]'
-  - "If used on a political action card in hand, that card must be announced and in hand when Charming Lobby is played, before it is replaced, but need not to be shown: it can be kept apart face down. [ANK 20180925-2] [LSJ 20101210] [LSJ 20100130]"
-  - "If used on a political action card in hand, that card cannot be canceled as it is played (eg. by {Direct Intervention}). [LSJ 20090113-3]"
-  - "If {Delaying Tactics} is used, the chosen political action card (if any) goes back into its owner's hand, and other minions are forbidden to perform Charming Lobby. [ANK 20201029-2] [LSJ 20030426]"
-  - "The requirements and cost of the political action card (if any) apply. If the cost is X, X is chosen at resolution. [LSJ 20100819]"
-  - "The cost of the political action card (if any) is not a cost of the action (eg. {Ravnos Carnival} cannot be used to pay it). [LSJ 20091021]"
-  - 'If played by an ally "as a vampire", they can call a referendum listed on a political action card in hand. [RTR 20020501]'
-  - 'Is a political action but not a "political action card" [POLITICAL ACTION] (eg. {Luna Giovanni}''s ability cannot target it, it cannot be discarded for a vote). [LSJ 20070927] [LSJ 20050407]'
+  - During the referendum that passes automatically, no "during a political action" and "during a referendum" effect can be played and effects that operate on the number of votes that the referendum passed by have no effect. [LSJ 19980107]
+  - The next referendum (passing automatically) can be called by another Methuselah's vampire. [PIB 20110719]
+  - Cannot be used on effects that allow to play a political action card "as if from hand" (eg. {Echo of Harmonies}) [ANK 20201029]
+  - "If used on a political action card in hand, that card must be announced and in hand when Charming Lobby is played, before it is replaced, but need not to be shown: it can be kept apart face down. If the action is canceled or failed, the political action card stays in hand. [ANK 20220704] [ANK 20180925-2] [LSJ 20101210] [LSJ 20100130]"
+  - If used on a political action card in hand, that card is considered "played" when the action reaches successful resolution and provides its inherent vote. [ANK 20220704]
+  - If used on a political action card in hand, that card cannot be canceled as it is played (eg. by {Direct Intervention}). [LSJ 20090113-3]
+  - If {Delaying Tactics} is used, the chosen political action card (if any) goes back into its owner's hand, and other minions are forbidden to perform Charming Lobby. [ANK 20201029-2] [LSJ 20030426]
+  - The requirements and cost of the political action card (if any) apply. If the cost is X, X is chosen at resolution. [ANK 20220704] [LSJ 20100819]
+  - The cost of the political action card (if any) is not a cost of the action (eg. {Ravnos Carnival} cannot be used to pay it). [LSJ 20091021]
+  - A bloodhunt referendum following a diablerie is not a referendum called by a vampire. [TOM 19950921]
+  - If played by an ally "as a vampire", they can call a referendum listed on a political action card in hand. [RTR 20020501]
+  - Is a political action but not a "political action card" [POLITICAL ACTION] (eg. {Luna Giovanni}'s ability cannot target it, it cannot be discarded for a vote). [ANK 20220704][LSJ 20070927] [LSJ 20050407]
 100335|Charnas the Imp:
-  - "Does nothing to an empty vampire which unlocks in torpor. [RTR 19941109]"
-  - "Cannot be damaged by host, but does not stop host from using effects which would normally damage it. [RTR 19941109]"
+  - Does nothing to an empty vampire which unlocks in torpor. [RTR 19941109]
+  - Cannot be damaged by host, but does not stop host from using effects which would normally damage it. [RTR 19941109]
   - "Is not burn if the controller of the vampire it is on id ousted: it is removed from the game. [ANK 20180408]"
 100340|Children of Stone:
-  - 'This is an "equip action" [TOM 19960130]'
+  - This is an "equip action" [TOM 19960130]
 100344|Chiropteran Marauder:
   - "[VIC] Must be played before strike resolution and damage prevention in order to affect the current strike (can be played after both strikes have been chosen). [RTR 19960112]"
+  - "[VIC] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {The Path of Metamorphosis}, {Dragos}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 100347|Church of the Order of St. Blaise:
-  - 'Can put counters on locations that use "blood" or "pool" counters. [PIB 20110712-1]'
+  - Can put counters on locations that use "blood" or "pool" counters. [PIB 20110712-1] [LSJ 20040518-2]
 100352|Claiming the Body:
-  - "The action ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20200207]"
+  - The action ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20200207]
 100353|Clan Impersonation:
-  - "Does not remove any slave status. [LSJ 20030511]"
-  - "Does not changes the sect. [RTR 20201130]"
-  - "When removed, the vampire goes back to its underlying clan. [RTR 20201130] [ANK 20200415]"
-  - "If the vampire changes clan to a clan inappropriate for his title, he loses its benefit until his clan is appropriate. He immediately yields the title if it is contested or he receives a new one. [RTR 20201130] [LSJ 20060904]"
+  - Does not remove any slave status. [LSJ 20030511]
+  - Does not changes the sect. [RTR 20201130]
+  - When removed, the vampire goes back to its underlying clan. [RTR 20201130] [ANK 20200415]
+  - If the vampire changes clan to a clan inappropriate for his title, he loses its benefit until his clan is appropriate. He immediately yields the title if it is contested or he receives a new one. [RTR 20201130] [LSJ 20060904]
 100354|Clan Loyalty:
-  - "The blocking minion is not locked [ANK 20180321]"
+  - The blocking minion is not locked [ANK 20180321]
+100355|Clandestine Contract:
+  - The action to put the card in play and the one once the card is in play are different (a vampire can take both in the same turn if they unlock in between). [ANK 20220910]
 100356|Claws of the Dead:
-  - "[pro] Must be played before strike resolution and damage prevention in order to affect the current strike. (can be played after both strikes have been chosen) [RTR 19960112]"
+  - "[pro] Must be played before strike resolution and damage prevention in order to affect the current strike. Can be played after both strikes have been chosen. [RTR 19960112]"
 100358|Cleave:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
-  - "The effect lasts until the end of the action. [LSJ 20060412]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
+  - The effect lasts until the end of the action. [LSJ 20060412]
+  - The weapon does not burn if it is temporarily out of play (eg. {Kerrie}, {Dagger}). The active Methuselah order the effects at the end of the action as they wish. [LSJ 20100211-2]
 100359|Clio's Kiss:
   - "[tem] The card to retrieve must be announced when declaring the action. [LSJ 20010627]"
 100362|Cloak the Gathering:
   - "[OBF] Can only be played by the controller of the acting minion. [LSJ 19990425]"
   - "[OBF] Can be played by a locked vampire. [RTR 19941109] [LSJ 19980210]"
   - "[OBF] Multiple copies can be played by different minions on the same action. [ANK 20200515]"
 100374|Codex of the Edenic Groundskeepers:
-  - "Allies (including Imbued) cannot use the provided action as they have no blood to pay with. [PIB 20151101]"
+  - Allies (including Imbued) cannot use the provided action as they have no blood to pay with. [PIB 20151101]
 100376|Cold Aura:
-  - "No other effect can be used to reset the range. Skip the determine range step on that round, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]"
+  - No other effect can be used to reset the range. Skip the determine range step on that round, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]
   - "[NEC] The press can only be used during the current round. [TOM 19960521]"
 100377|Collapse the Arches:
   - "[tha] The press can only be used during the current round. [TOM 19960521]"
+  - "[vis], [VIS] Does not prevent the opponent from dodging, the dodge just has no effect. [LSJ 20030902-2] [LSJ 20060808-1]"
 100378|Coma:
+  - Only effective at close range. [RBK 20200701-10] [LSJ 20000110]
+  - The opponent is wounded (if they play {Undying Tenacity}, they go to torpor after combat). [LSJ 20090622-2]
   - '[DEM] The "does not unlock as normal" effect is redundant with being infernal. If the minion is infernal, its controller can still pay a pool to unlock them. [LSJ 20050114]'
+100381|Command of the Beast:
+  - "[DOM] A limited bleed modifier can be played before or after. [LSJ 20100218] [RTR 20180511-2]"
 100388|Compel the Spirit:
-  - "Can only be played if the ally or retainer is in the ash heap, not if he was moved elsewhere. [RTR 19980928] [LSJ 19980929]"
-  - "The ally or retainer retrieved is considered a new ally or retainer for all game purposes. In particular, he is not bound to not repeat an action his previous incarnation has already performed this turn. [LSJ 20010627]"
-  - "Requirements need not to be met. If the ally requires a discipline, the inferior version is used. If the cost is X (eg. {Reanimated Corpse}), X is zero. [LSJ 20071015] [LSJ 20100302-1]"
-  - "Cannot be used if the ally in the ash heap was representing something else while in play (eg. {Khazar's Diary (Endless Night)}, {Absimiliard's Army}). [LSJ 20071014]"
+  - Can only be played if the ally or retainer is in the ash heap, not if he was moved elsewhere. [RTR 19980928] [LSJ 19980929]
+  - The ally or retainer retrieved is considered a new ally or retainer for all game purposes. In particular, he is not bound to not repeat an action his previous incarnation has already performed this turn. [LSJ 20010627]
+  - Requirements need not to be met. If the ally requires a discipline, the inferior version is used. If the cost is X (eg. {Reanimated Corpse}), X is zero. [LSJ 20071015] [LSJ 20100302-1]
+  - Cannot be used if the ally in the ash heap was representing something else while in play (eg. {Khazar's Diary (Endless Night)}). [LSJ 20071014]
 100389|Compress:
   - "[pot] Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+100391|Conceal:
+  - Is directed against the Methuselah controlling the equipment or location, not the minion it's on. [LSJ 20090324]
 100392|Concealed Weapon:
   - "The weapon must be announced and in hand when the card is played, before it is replaced, but need not to be shown: it can be kept apart face down. [LSJ 19991207] [ANK 20180925-2] [LSJ 20100130]"
-  - 'A weapon''s "current damage" is the amount of damage that it would inflict if used as a strike against a generic opponent. [RTR 19980623]'
-  - "Strength or other bonus from the minion or other cards in play are not counted for the damage limit. [LSJ 20020821] [LSJ 20020904]"
-  - 'Cost reductions that are not limited to cards "played" apply before checking for card cost (eg. {Black Cat} can use Concealed Weapon to equip with a {Combat Shotgun}). [LSJ 20080125] [ANK 20181216]'
-  - "Paying from another source (eg. {Alan Sovereign (ADV)}) does not reduce the cost as seen by Concealed Weapon. [LSJ 20080125]"
+  - A weapon's "current damage" is the amount of damage that it would inflict if used as a strike against a generic opponent. [RTR 19980623]
+  - Strength or other bonus from the minion or other cards in play are not counted for the damage limit. [LSJ 20020821] [LSJ 20020904]
+  - Cost modifications that are not limited to cards "played" apply before checking for card cost (eg. {Black Cat} can equip with a {Combat Shotgun}, {Centralized Background Check} makes {.44 Magnum} too costly). [LSJ 20040701] [LSJ 20080125] [ANK 20181216]
+  - Paying from another source (eg. {Alan Sovereign (ADV)}) does not reduce the cost as seen by Concealed Weapon. [LSJ 20080125]
 100394|Concoction of Vitality:
-  - "Can be used after declaring an action using a discipline (eg. {Govern the Unaligned}). [LSJ 20100402]"
+  - Can be used after declaring an action using a discipline (eg. {Govern the Unaligned}). [LSJ 20100402]
 100396|Condemn the Sins of the Father:
-  - "Is directed at all Methusalah controlling one of the chosen targets. [KOT 20081119] [ANK 20180917]"
+  - Is directed at all Methuselah controlling one of the chosen targets. [KOT 20081119] [ANK 20180917]
 "100400|Condemnation: Mute":
-  - "Only affects votes, and not ballots. [PIB 20110802]"
+  - Only affects votes, and not ballots. [PIB 20110802]
 100405|Confusion:
   - "[DEM] Can only be used during a bleed action. [ANK 20171023] [RTR 19941109]"
 100412|Conscripted Statue:
   - "[vis] Damage is environmental. [RTR 19970630]"
   - '[vis] Damage is inflicted even against a dodge. A "strike: combat ends" ends combat before damage is applied, as will a combattant going to torpor during first strike. [RTR 19941109] [TOM 19951216] [PIB 20140324] [ANK 20200422]'
+  - "[VIS] The vampire playing it is not considered having burned a minion (eg. for {Taking the Skin: Minion}, but the opponent is. [LSJ 20090922] [ANK 20220916]"
 100414|Conservative Agitation:
-  - "Cannot allocate all X points to a single Methusalah, but you can allocate points to yourself. [LSJ 20000622]"
-  - "Can allocate more points than a Methusalah has pool. [LSJ 20020819]"
+  - Cannot allocate all X points to a single Methuselah, but you can allocate points to yourself. [LSJ 20000622]
+  - Can allocate more points than a Methuselah has pool. [LSJ 20020819]
 100415|Consignment to Duat:
   - "[ser] Can target a vampire with no blood. [RTR 20010711]"
+  - "[ser] If it burns an ally as a result, this counts as a Ⓓ action burning an ally (eg. Trophies, {Predator's Transformation}). [ANK 20220507]"
+100418|Contagion:
+  - "[DAI] Stealing the minion is part of the strike resolution, it does not happen if the strike is not selected and it can be dodged. [ANK 20200909] [LSJ 20040130]"
 100423|Coordinate Attacks:
-  - "Must be played after the presses are handled and can be played if the round ends prematurely. [RTR 20030519]"
-100427|Corpse Balloon:
-  - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
+  - Must be played after the presses are handled and can be played if the round ends prematurely. [RTR 20030519]
 100428|Corpse Minion:
-  - "May be used any number of times during a single action. [TOM 19960109]"
+  - May be used any number of times during a single action. [TOM 19960109]
 100429|Corrupt Construction:
-  - "If recruited in the normal fashion, the card will have been replaced by the time the ally enters play. In other cases however, it won't have been and the Methuselah will have to work with only the cards in hand (or ash heap) to add life to it before replacing. [LSJ 20070707]"
-  - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
+  - If recruited in the normal fashion, the card will have been replaced by the time the ally enters play. In other cases however, it won't have been and the Methuselah will have to work with only the cards in hand (or ash heap) to add life to it before replacing. [LSJ 20070707]
 100432|Coterie Tactics:
-  - "Cannot be used if the vampires cannot attempt to block the action (eg. {Daring the Dawn}). [LSJ 20010714-2]"
-  - "The block attempt and subsequent combat still happen if the action lacks a suitable target because of the unlock (eg. {Ambush}). [LSJ 20090514]"
+  - Cannot be used if the vampires cannot attempt to block the action (eg. {Daring the Dawn}). [LSJ 20010714-2]
+  - Does not ignore the normal prey, predator or target restrictions. [ANK 20180623]
+  - The block attempt and subsequent combat still happen if the action lacks a suitable target because of the unlock (eg. {Ambush}). [LSJ 20090514]
 100433|Council of Seraphim:
-  - "The burn option cannot be used if all your Seraph are in torpor. [LSJ 20091204]"
+  - The burn option cannot be used if all your Seraph are in torpor. [LSJ 20091204]
+100434|Courier:
+  - Needs not be unlocked to let you look at a card. [LSJ 20001102]
+  - Multiple Courier can look at and discard the top library card in succession. [LSJ 20001102]
+  - One Courier only lets you look at the top library card once per bleed. [LSJ 20001102-2]
 100435|The Coven:
-  - "Can be locked during damage resolution, but not while healing damage or preventing destruction (you cannot take 2, lock The Coven, then take the rest). [PIB 20121031]"
-  - "The predator must take control of it when he gets the the opportunity to play effects. If a players declares his turn ends, he does not get the opportunity to use it before it is moved to his predator, even retroactively if the mandatory effect was forgotten. [LSJ 20100723] [PIB 20111002]"
+  - Can be locked during damage resolution, but not while healing damage or preventing destruction (you cannot take 2, lock The Coven, then take the rest). [PIB 20121031]
+  - The predator must take control of it when he gets the the opportunity to play effects. If the controller declares his turn ends, he does not get the opportunity to use The Coven before it is moved to his predator, even retroactively if the mandatory effect was forgotten. [LSJ 20100723] [PIB 20111002]
 100439|Crawling Chamber:
   - "[VIS] Damage is environmental. [RTR 19970630]"
 100440|Create Gargoyle:
-  - "Only requires one clan or the other (Tremere or Tremere antitribu) to be played. [ANK 20190203]"
+  - Only requires one clan or the other (Tremere or Tremere antitribu) to be played. [ANK 20190203]
 100441|Creation Rites:
-  - "If moved to the uncontrolled region, it continues to be a vampire and can be influenced. [RTR 19990712]"
+  - If moved to the uncontrolled region, it continues to be a vampire and can be influenced. [RTR 19990712]
 100446|CrimethInc.:
-  - "Can be played if the action is unblocked even if it has no effect due to lack of a suitable target. [LSJ 20070411]"
+  - Can be played if the action is unblocked even if it has no effect due to lack of a suitable target. [LSJ 20070411]
+  - An action requiring a Baron (eg. {Open War}) is an action requiring an Anarch. [LSJ 20080603] [LSJ 20050128]
 100449|The Crocodile Temple:
-  - "Cannot be used if the action ousted you. [ANK 20180326]"
+  - Cannot be used if the action ousted you. [ANK 20180326]
 100450|Crocodile's Tongue:
-  - "The canceled block isn't successful or unsuccessful. It is simply canceled. [LSJ 20110419]"
+  - The canceled block isn't successful or unsuccessful. It is simply canceled. [LSJ 20110419]
 100474|The Crusader Sword:
-  - "Can be equipped by a minion who cannot use it. [LSJ 20030607]"
+  - Can be equipped by a minion who cannot use it. [LSJ 20030607]
 100475|Cry Wolf:
-  - "His ability continues to apply fully if he is not a werewolf (eg. {Pressing Flesh}). [LSJ 20100212]"
+  - His ability continues to apply fully if he is not a werewolf (eg. {Pressing Flesh}). [LSJ 20100212]
+  - If he unlocks after having performed his mandatory action, he's free to take any action. [LSJ 20090226]
 100476|Crypt's Sons:
-  - "If used to cancel combat, the blocking minion is still locked. [LSJ 20080611] [ANK 20210131]"
-  - "If used to cancel combat, reactions cards pertaining to that combat (eg. {Obedience}) cannot be used afterwards. [ANK 20210131]"
-  - 'If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [LSJ 20080611] [ANK 20190116]'
-  - 'If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
+  - If used to cancel combat, the blocking minion is still locked. [LSJ 20080611] [ANK 20210131]
+  - If used to cancel combat, reactions cards pertaining to that combat (eg. {Obedience}) cannot be used afterwards. [ANK 20210131]
+  - If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [LSJ 20080611] [ANK 20190116]
+  - If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]
   - '"continue as if unblocked" moves the action card from the ash heap (where it went when the action was blocked) to limbo (where it should be if the action is not blocked). If the action card is not in the ash heap, then the action cannot be continued. [LSJ 20070808-1]'
+100477|Cryptic Mission:
+  - If used on an ally and it burns as a result, this counts as a Ⓓ action burning an ally (eg. Trophies, {Predator's Transformation}). [ANK 20220507]
 100478|Cryptic Rider:
-  - 'During the referendum that passes automatically, no "during a political action" and "during a referendum" effect can be played and effects that operate on the number of votes that the referendum passed by have no effect. [LSJ 19980107]'
-  - "Can be used after a referendum that is automatically passing. [PIB 20150105] [LSJ 19980107]"
+  - During the referendum that passes automatically, no "during a political action" and "during a referendum" effect can be played and effects that operate on the number of votes that the referendum passed by have no effect. [LSJ 19980107]
+  - Can be used after a referendum that is automatically passing. [PIB 20150105] [LSJ 19980107]
 100483|Curse of Nitocris:
-  - "Only moves when a Methuselah gets the Edge who does not already have the Edge. [LSJ 19971006]"
-100484|D'habi Revenant:
-  - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
+  - Only moves when a Methuselah gets the Edge who does not already have the Edge. [LSJ 19971006]
+100485|Dabbler:
+  - Cannot be used if the action is canceled. [ANK 20220411]
+  - Takes into account all the cards played, even if they are canceled. [ANK 20220411]
 100486|Daemonic Possession:
-  - "This is not a directed action, even when targeting another Methusalah's ash heap. [LSJ 20010627] [ANK 20181129]"
+  - This is not a directed action, even when targeting another Methuselah's ash heap. [LSJ 20010627] [ANK 20181129]
 100488|Dagon's Call:
-  - "Both the strike and the environmental damage would get boosted by {Dam the Heart's River}. [PIB 20150520]"
+  - Both the strike and the environmental damage would get boosted by {Dam the Heart's River}. [PIB 20150520]
   - "[QUI] Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
 100489|Dam the Heart's River:
-  - "Adding damage to strikes which are not damage dealing strikes will not deal damage [RTR 19960221]"
-  - "The additional damage is the same type as the strike's damage. [RTR 19970630]"
-  - "Applies to environmental damage inflicted to the opposing minion. [ANK 20181128]"
-  - "Applies to damage played in combat that are resolved after combat (eg. {Catatonic Fear}). [ANK 20170111] [LSJ 20071011]"
+  - The opponent is the one affected by frenzy (eg. for {Blade of Enoch}). [ANK 20220409]
+  - Adding damage to strikes which are not damage dealing strikes will not deal damage [RTR 19960221]
+  - The additional damage is the same type as the strike's damage. [RTR 19970630]
+  - Applies to environmental damage inflicted to the opposing minion. [ANK 20181128]
+  - Applies to damage played in combat that are resolved after combat (eg. {Catatonic Fear}). [ANK 20170111] [LSJ 20071011]
   - "[QUI] The opponent must pay 1 blood to use a strike that provides a maneuver if he plays it when choosing range. [ANK 20181026]"
 100490|The Damned:
-  - 'The acting player decides the order of (and can play other) "after resolving the action" effects. [ANK 20180206]'
+  - The acting player decides the order of (and can play other) "after resolving the action" effects. [ANK 20180206]
 100492|Daring the Dawn:
-  - "If the action is blocked, damage is applied after combat [RTR 19980623]"
+  - If the action is blocked, damage is applied after combat [RTR 19980623]
+  - The damage is applied if the action reaches resolution, even if it ends before combat (eg. {Mirror Walk}, {Change of Target}, {Red Herring}) or has no effect (eg. because cost cannot be paid). [ANK 20220331] [ANK 20210124] [LSJ 20020927] [LSJ 20021115] [ANK 20221011-2]
+  - The damage is not applied if the action is canceled before resolution (eg. {Tangle Atropos' Hand}, {The Kiss of Ra}). [ANK 20220401] [ANK 20211015] [ANK 20210124]
 100493|Dark Influences:
-  - 'If the canceled card had a "Do Not Replace Until" clause on it (or alternate replacement like {Steely Tenacity}), that clause is canceled as well and the card is replaced normally. [LSJ 20011023] [LSJ 20080630]'
-  - "If used to cancel an action, the action is not performed in respect to section 6.1 of the rules and the minion is free to attempt the same action again. [LSJ 19980212]"
-  - "If used to cancel a limited effect (bleed, additional strike), then the limit is not triggered and another limited effect can be used. [LSJ 20030224]"
-  - "The card is still considered played. The same reaction or modifier cannot be played again by the same minion. Another Aim card can not be played once one has been canceled, nor any other card which text prohibits to be played more than once. [LSJ 19980212] [ANK 20190104]"
-  - "Can only cancel minion cards played from the hand in the normal fashion (eg. not weapons played via {Disguised Weapon} or allies from {Piper}). [RTR 20001020]"
+  - If the canceled card had a "Do Not Replace Until" clause on it (or alternate replacement like {Steely Tenacity}), that clause is canceled as well and the card is replaced normally. [LSJ 20011023] [LSJ 20080630]
+  - If used to cancel an action, the action is not performed in respect to section 3 of the rules. [LSJ 19980212]
+  - If used to cancel a limited effect (bleed, additional strike), then the limit is not triggered and another limited effect can be used. [LSJ 20030224]
+  - The card is still considered played. The same reaction or modifier cannot be played again by the same minion. Another Aim card can not be played once one has been canceled, nor any other card which text prohibits to be played more than once. [LSJ 19980212] [ANK 20190104]
+  - Can only cancel minion cards played from the hand in the normal fashion (eg. not weapons played via {Disguised Weapon} or allies from {Piper}). [RTR 20001020]
 100496|Darkling Trickery:
-  - "[MYT] Damage is environmental. [RTR 19970630] [LSJ19971028]"
   - '[MYT] Damage is inflicted even against a dodge. A "strike: combat ends" ends combat before damage is applied, as will a combattant going to torpor during first strike. [RTR 19941109] [TOM 19951216] [PIB 20140324] [ANK 20200422]'
-"100499|Dartmoor, England":
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
+100497|Darkness Within:
+  - 'The blood is removed during strike resolution, before mending damage. It is not removed if a "strike: combat ends" resolves. [LSJ 20051123]'
+  - The effect is ordered against steal blood effects (eg. {Theft of Vitae}) by the acting minion's controller. [LSJ 20020301]
+100498|Darksight:
+  - Goes to the ash heap when played, if it has been removed when the vampire blocks, it has no effect. [ANK 20220805]
 100501|Dawn Operation:
-  - "Only applies to damage done in combat, not damage done after combat like {Catatonic Fear}. [LSJ 20020314] [PIB 20130319]"
-  - "Applies to environmental and retainer damage too. [PIB 20150603-1]"
+  - Only applies to damage done in combat, not damage done after combat like {Catatonic Fear}. [LSJ 20020314] [PIB 20130319]
+  - Applies to environmental and retainer damage too. [PIB 20150603-1]
 100503|Dead Hand:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
+  - "[NEC] The opponent cannot play [for] prevention cards (eg. for cycling). [LSJ 20050628]"
 100510|Death Seeker:
-  - "If used to cancel a strike, another strike is chosen. [LSJ 20100206]"
-  - 'If the canceled card had a "Do Not Replace Until" clause on it (or alternate replacement like {Steely Tenacity}), that clause is canceled as well and the card is replaced normally. [LSJ 20011023] [LSJ 20080630]'
-  - "If used to cancel a limited effect (additional strike), then the limit is not triggered and another limited effect can be used. [LSJ 20100206] [LSJ 20030224]"
-  - "Can only cancel minion cards played from the hand in the normal fashion (eg. not weapons played via {Disguised Weapon}). [RTR 20001020]"
-  - "When used to cancel a card play at the end of a round or when combat would end, counts as having been played during that ending round. [ANK 20180910-2]"
+  - If used to cancel a strike, another strike is chosen. [LSJ 20100206]
+  - If the canceled card had a "Do Not Replace Until" clause on it (or alternate replacement like {Steely Tenacity}), that clause is canceled as well and the card is replaced normally. [LSJ 20011023] [LSJ 20080630]
+  - If used to cancel a limited effect (additional strike), then the limit is not triggered and another limited effect can be used. [LSJ 20100206] [LSJ 20030224]
+  - Can only cancel minion cards played from the hand in the normal fashion (eg. not weapons played via {Disguised Weapon}). [RTR 20001020]
+  - 'Can be used to cancel a card play at the end of a round (eg. {Disarm}) or "when combat would end" (eg. {Psyche!}): it then counts as having been played during that ending round. [ANK 20180910-2] [ANK 20191221]'
 100511|Decapitate:
   - "[pot] Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
   - '"when a vampire is going into torpor" and "when a vampire should go into torpor" are the same window. If both minions want to play a card, acting minion goes first. If played first, {Undead Persistence} would prevent the opponent to play {Decapitate} and vice-versa. [RTR 20010710]'
 100514|Deep Cover Agent:
-  - "The burn option can be used if all your Seraph are in torpor. [LSJ 20091203]"
+  - The burn option can be used if all your Seraph are in torpor. [LSJ 20091203]
 100515|Deep Song:
   - "[ANI] The lock and enter combat effects are simultaneous. Both are lost if the action ends before that (eg. {Obedience}). [ANK 20200702]"
+  - "[ANI] If another effect changes the acting minion in combat later on, it takes precedence (eg. {Nar-Sheptha}). [ANK 20211022]"
 100516|Deer Rifle:
-  - "The optional maneuvers cannot be used if the strike cannot be used (eg. {Hidden Lurker}). [LSJ 20021028]"
+  - The optional maneuvers cannot be used if the strike cannot be used (eg. {Hidden Lurker}). [LSJ 20021028]
 100517|Defender of the Haven:
-  - "Only requires one clan or the other (Tremere or Tremere antitribu) to be played. [ANK 20190203]"
+  - Only requires one clan or the other (Tremere or Tremere antitribu) to be played. [ANK 20190203]
 100518|Deflection:
-  - "Cannot be used to direct a bleed to a Methuselah who would be an invalid target for a bleed. [RTR 19950622]"
-  - "Declaring that one is not blocking is implicit in playing Deflection. [LSJ 20000507]"
-  - 'Must be played before action resolution, ie. before any modifier or reaction played "as the action/bleed would be successful" are played. It cannot be played after a {Spying Mission} on the vampire triggers. [LSJ 19980105]'
+  - Cannot be used to direct a bleed to a Methuselah who would be an invalid target for a bleed. [RTR 19950622]
+  - Declaring that one is not blocking is implicit in playing Deflection. [LSJ 20000507]
+  - Must be played before action resolution, ie. before any modifier or reaction played "as the action/bleed would be successful" are played. It cannot be played after a {Spying Mission} on the vampire triggers. [LSJ 19980105]
+  - "Can be played when failing to block because of stealth: it is still declining to block. [ANK 20211003]"
 100519|Delaying Tactics:
-  - "May be played before, during, or after votes and ballots have been cast. [LSJ 19980130]"
-  - "The acting minion is still considered to have taken a political action, so cannot perform another in the same turn. [RTR 19970630]"
-  - "If played on a referendum called by a {Charming Lobby}, the political action card (if any) is retrieved and other minions are forbidden to perform a {Charming Lobby}. [ANK 20201029-2] [LSJ 20030426]"
-  - "Will only retrieve a political action card played from the hand (eg. it does not retrieve an in-play {Rumors of Gehenna} in the referendum to burn it or the card chosen by {Bujo}). [LSJ 20041130] [LSJ 20100527]"
-  - "It retrieves the political action card before it is burned (eg. if it was played from {The Erciyes Fragments}, it is still returned into its owner's hand). [LSJ 20050324]"
+  - May be played before, during, or after votes and ballots have been cast. [LSJ 19980130]
+  - The acting minion is still considered to have taken a political action, so cannot perform another in the same turn. [RTR 19970630]
+  - If played on a referendum called by a {Charming Lobby}, the political action card (if any) is retrieved and other minions are forbidden to perform a {Charming Lobby}. [ANK 20201029-2] [LSJ 20030426]
+  - Will only retrieve a political action card played from the hand (eg. it does not retrieve an in-play {Rumors of Gehenna} in the referendum to burn it or the card chosen by {Bujo}). [LSJ 20041130] [LSJ 20100527]
+  - It retrieves the political action card before it is burned (eg. if it was played from {The Erciyes Fragments}, it is still returned into its owner's hand). [LSJ 20050324]
 100526|Depravity:
-  - "The +1 strength is always in effect, not just during diablerie attempts. [RTR 19961113]"
+  - The +1 strength is always in effect, not just during diablerie attempts. [RTR 19961113]
 100527|Derange:
-  - "Cannot be moved to a Malkavian nor to a Malkavian antitribu vampire. [LSJ 19970224]"
-  - "The clan is set when the card is played, it does not depend on the clan of the vampire that has the card on them. [LSJ 20070707]"
-  - "Does not change the sect of the target. [RTR 20201130]"
-  - "If the target changes clan to a clan inappropriate for his title, he loses its benefit until his clan is appropriate. He immediately yields the title if it is contested or he receives a new one. [RTR 20201130] [LSJ 20060904]"
-  - "When removed, the vampire goes back ot its underlying clan. [RTR 20201130] [ANK 20200415]"
-  - "Only requires one clan or the other (Malkavian or Malkavian antitribu) to be played. [ANK 20190203]"
+  - Cannot be moved to a Malkavian nor to a Malkavian antitribu vampire. [LSJ 19970224]
+  - The clan is set when the card is played, it does not depend on the clan of the vampire that has the card on them. [LSJ 20070707]
+  - Does not change the sect of the target. [RTR 20201130]
+  - If the target changes clan to a clan inappropriate for his title, he loses its benefit until his clan is appropriate. He immediately yields the title if it is contested or he receives a new one. [RTR 20201130] [LSJ 20060904]
+  - When removed, the vampire goes back ot its underlying clan. [RTR 20201130] [ANK 20200415]
+  - Only requires one clan or the other (Malkavian or Malkavian antitribu) to be played. [ANK 20190203]
 100528|Descent into Darkness:
-  - "Breaks any temporary control effects, so the vampire is given, face down and out of play, to his current permanent controller, with the Descent into Darkness card which, as a minion card, is then controlled by that permanent controller. [LSJ 20040526]"
-  - "Damage inflicted after the action resolution (eg. {Daring the Dawn}) are not applied. [LSJ 20040616]"
+  - Breaks any temporary control effects, so the vampire is given, face down and out of play, to his current permanent controller, with the Descent into Darkness card which, as a minion card, is then controlled by that permanent controller. [LSJ 20040526]
+  - Damage inflicted after the action resolution (eg. {Daring the Dawn}) are not applied. [LSJ 20040616]
+  - If played by an ally, the ally can never come back. [LSJ 20060124]
+  - All cards on the vamipre come back unlocked. [LSJ 20060908]
+  - The vampire will remember all effects that had been applied to him, just as contested vampires do. This includes gained or lost titles. [RTR 20000501] [LSJ 20060908]
+  - Cards and effects targeting the vampire (eg. {The Rack}) will resume if and when the vampire comes back into play. [TOM 19960211] [LSJ 20010809-2] [LSJ 20010809-3] [LSJ 20060908]
 100532|Detect Authority:
   - "[ani] If the action ends, no action modifier or reaction can be played afterwards. [RTR 20180719]"
+  - "[ani] Not usable against actions targeting an equipment or retainer, they do not target the minion. [LSJ 20090324]"
+100534|Determine:
+  - Cannot be used to cancel an action card after using a reaction to "unlock and attempt to block". [LSJ 20021011]
+  - If used to cancel a card that had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]
 100536|Deviki Prasanta:
-  - "Cannot put a Discipline card on a vampire if it could normally not be put on him (eg. because he already has the superior level of that discipline). [ANK 20200320]"
-  - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
+  - Cannot put a Discipline card on a vampire if it could normally not be put on him (eg. because he already has the superior level of that discipline). [ANK 20200320]
+"100537|Devil-Channel: Back":
+  - "[abo] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {High Orun}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 "100538|Devil-Channel: Feet":
-  - "The press can only be used during the current round. [TOM 19960521]"
+  - The press can only be used during the current round. [TOM 19960521]
 100541|Día de los Muertos:
-  - 'During the referendum that passes automatically, no "during a political action" and "during a referendum" effect can be played and effects that operate on the number of votes that the referendum passed by have no effect. [LSJ 19980107]'
+  - During the referendum that passes automatically, no "during a political action" and "during a referendum" effect can be played and effects that operate on the number of votes that the referendum passed by have no effect. [LSJ 19980107]
+100542|Diabolic Lure:
+  - "[DAI] The opponent burns pool wether or not the pact counters reach capacity. [LSJ 20100205-2] [ANK 20221007]"
 100543|The Diamond Thunderbolt:
-  - 'If used to cancel a card that has a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
+  - If used to cancel a card that has a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]
   - "If used to cancel the change of control of a {Corruption} action, only the control change is prevented: the corruption counters are burned. [LSJ 20070222-2]"
-  - "The cost of the change of control effect is still paid. Any bids made are paid. Any counters burned are still burned. [LSJ 20040518]"
-  - "Will not extend temporary change of control effects when they expire. [LSJ 20040518]"
+  - The cost of the change of control effect is still paid. Any bids made are paid. Any counters burned are still burned. [LSJ 20040518] [LSJ 20040518-2]
+  - Will not extend temporary change of control effects when they expire. [LSJ 20040518] [LSJ 20040518-2]
 100545|Direct Intervention:
-  - 'If the canceled card had a "Do Not Replace Until" clause on it (or alternate replacement like {Steely Tenacity}), that clause is canceled as well and the card is replaced normally. [LSJ 20011023] [LSJ 20080630]'
-  - "If used to cancel an action, the action is not performed in respect to section 6.1 of the rules and the minion is free to attempt the same action again. [LSJ 19980212]"
-  - "If used to cancel a limited effect (bleed, additional strike), then the limit is not triggered and another limited effect can be used. [LSJ 20030224]"
-  - "The card is still considered played. The same reaction or modifier cannot be played again by the same minion. Another Aim card can not be played once one has been canceled, nor any other card which text prohibits to be played more than once. [LSJ 19980212] [ANK 20190104]"
-  - "Can only cancel minion cards played from the hand in the normal fashion (eg. not weapons played via {Disguised Weapon} or allies from {Piper}). [RTR 20001020]"
+  - If the canceled card had a "Do Not Replace Until" clause on it (or alternate replacement like {Steely Tenacity}), that clause is canceled as well and the card is replaced normally. [LSJ 20011023] [LSJ 20080630]
+  - If used to cancel an action, the action is not performed in respect to section 3 of the rules and the minion is free to attempt the same action again. [LSJ 19980212]
+  - If used to cancel a limited effect (bleed, additional strike), then the limit is not triggered and another limited effect can be used. [LSJ 20030224]
+  - The card is still considered played. The same reaction or modifier cannot be played again by the same minion. Another Aim card can not be played once one has been canceled, nor any other card which text prohibits to be played more than once. [LSJ 19980212] [ANK 20190104]
+  - Can only cancel minion cards played from the hand in the normal fashion (eg. not weapons played via {Disguised Weapon} or allies from {Piper}). [RTR 20001020]
 100547|Dirty Little Secrets:
-  - "If the Methuselah you are bleeding does not burn any pool due to another effect, then she does not burn any cards from her library either. [LSJ 19970224]"
+  - If the Methuselah you are bleeding does not burn any pool due to another effect, then she does not burn any cards from her library either. [LSJ 19970224]
 100548|Dis Pater:
-  - 'Only effects played "when the action is/would be successful" can be played afterwards. (eg. {Deflection}, {Archon Investigation} or {Conditioning} can only be used before). [LSJ 20050422]'
+  - Only effects played "when the action is/would be successful" can be played afterwards. (eg. {Deflection}, {Archon Investigation} or {Conditioning} can only be used before). [LSJ 20050422]
 100549|Disarm:
-  - "Must be played after the presses are handled and can be played if the round ends prematurely. [RTR 20030519]"
-  - 'Can be played before or after effects that are played at the end of the round or "when the combat would end" (eg. [AUS] {Telepathic Tracking}). Can be played after [CEL] {Psyche!} [LSJ 20021113] [ANK 20191219] [ANK 20180910-1]'
+  - Must be played after the presses are handled and can be played if the round ends prematurely. [RTR 20030519]
+  - Environmental damages (eg. {Carrion Crows}) do not count. [LSJ 20010812]
+  - Can be played before or after effects that are played at the end of the round or "when the combat would end" (eg. [AUS] {Telepathic Tracking}). Can be played before or after [CEL] {Psyche!}. [LSJ 20021113] [ANK 20191219] [ANK 20180910-1]
 100550|Disarming Presence:
-  - "Locking is a side effect, not a cost. Locked vampires can still vote. [RTR 19941109]"
-  - "Vampires are locked when they cast their votes. [RTR 19970425]"
+  - Locking is a side effect, not a cost. Locked vampires can still vote. [RTR 19941109]
+  - Vampires are locked when they cast their votes. [RTR 19970425]
 100551|Discern:
   - "[REACTION] Can be used only when reactions can be used (unlocked or with a wake effect). It does not count as playing a reaction card. [LSJ 20070403] [LSJ 20070413]"
+100554|Disengage:
+  - " The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Dragos}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 100555|Disguised Weapon:
-  - "The weapon is announced when the card is played, it must be in hand but need not to be shown. You can put the card apart face down when announcing it. [LSJ 19991207] [ANK 20180925-2]"
-  - "If used to equip and contest a unique weapon already in play, neither weapon is available for use during the combat. If the opposing minion had already chosen that weapon as his strike, then the strike has no effect. [LSJ 19980319]"
+  - The weapon is announced when the card is played, it must be in hand but need not to be shown. You can put the card apart face down when announcing it. [LSJ 19991207] [ANK 20180925-2]
+  - If used to equip and contest a unique weapon already in play, neither weapon is available for use during the combat. If the opposing minion had already chosen that weapon as his strike, then the strike has no effect. [LSJ 19980319]
 100557|Disputed Territory:
-  - "Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
-  - "If used to steal an equipment representing a location, it can be placed on any minion controlled by the new controller. [RTR 19960112]"
-  - 'If used to "change" the control of a location or equipment representing a location to the same Methusalah, the location cannot be moved to another minion controlled by the same Methusalah. [LSJ 19971002]'
+  - Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]
+  - If used to steal an equipment representing a location, it can be placed on any minion controlled by the new controller. [RTR 19960112]
+  - If used to "change" the control of a location or equipment representing a location to the same Methuselah, the location cannot be moved to another minion controlled by the same Methuselah. [LSJ 19971002]
 100558|Dissolution:
   - "[PRO] The press can only be used during the current round. [TOM 19960521]"
 100559|Distant Friend:
-  - "Cannot be burned during a referendum that is automatically passing. [PIB 20150105] [LSJ 19980107]"
+  - Cannot be burned during a referendum that is automatically passing. [PIB 20150105] [LSJ 19980107]
+100562|Dive into Madness:
+  - "[dem] can be played by a vampire with superior Dementation [DEM]. [PIB 20130311]"
 100563|Diversion:
   - "[tha] can target a vampire with no blood. [RTR 20010711]"
+100565|Divine Image:
+  - "[SER] A limited bleed modifier can be played before or after. [LSJ 20100218] [RTR 20180511-2]"
 100568|Dog Pack:
   - 'If put on a minion after an opponent as declared a "strike: combat ends" (eg. using {Pack Alpha} or {Summon Spirit Beast}), the opponent''s strike has no effect. [ANK 20190412]'
 100570|Domain Challenge:
-  - "Locked minions are counted after the referendum is completed. [RTR 19941109]"
+  - Locked minions are counted after the referendum is completed. [RTR 19941109]
 100571|Domain of Evernight:
   - "[tem] Only applies to damage done in combat, not damage done after combat like {Catatonic Fear}. [LSJ 20020314] [PIB 20130319]"
-  - '[TEM] Cards and effects that can be played "after resolution" (and only them) can be played after it. [ANK 20190425]'
+  - '[TEM] Is played after resolution, but still during the action. Action modifiers and effects that can be played "after resolution" can be played before or after it. [LSJ 19981028] [ANK 20190425]'
 100573|Dominate Kine:
   - "[DOM] If used to steal an equipment representing a location, it can be placed on any minion controlled by the new controller. [RTR 19960112]"
 100575|Donate:
   - "[REACTION] Can be used only when reactions can be used (unlocked or with a wake effect). It does not count as playing a reaction card. [LSJ 20070403] [LSJ 20070413]"
 100576|Donnybrook:
   - "[ser] can target a minion with less than 2 blood or life. [RTR 20010711]"
 100578|Draba:
   - "[CHI] Effectively gives a -X stealth modifier to the action, where X is the amount of stealth reduced by Draba at the time it was played. [RTR 20030519]"
   - "[CHI] Can be played by a minion who is not attempting to block the action. [ANK 20190628]"
   - "[CHI] Can be played on a minion with no or negative stealth, in which case it has no effect. [LSJ 20021211]"
-  - "If another Methusalah is the target, he must declare whether he attempts or declines to block before Draba can be used ([chi]) or played ([CHI]). [PIB 20150820] [ANK 20200607]"
+  - If another Methuselah is the target, he must declare whether he attempts or declines to block before Draba can be used ([chi]) or played ([CHI]). [PIB 20150820] [ANK 20200607]
 100579|Draeven Softfoot:
-  - "He can lock to use his ability the turn he is recruited. [ANK 20180517]"
+  - He can lock to use his ability the turn he is recruited. [ANK 20180517]
 100580|Dragon's Breath Rounds:
   - 'Does not burn the gun if combat ends before the strike resolves (eg. {Rötschreck} or if the opponent uses a "strike: combat ends"). [LSJ 19981006] [LSJ 20001127-2]'
 100582|Drain Essence:
-  - "Can target a minion with less blood or life than the amount stolen. [RTR 20010711]"
+  - Can target a minion with less blood or life than the amount stolen. [RTR 20010711]
 100584|Draught of the Soul:
   - "[COMBAT] If a minion is burned in combat, his opponent his always considered to have burned him. [LSJ 20090922]"
   - "[ACTION MODIFIER] If the minion is burned because of a referendum or as a side-effect of the action, this does not count as the acting minion burning him. (eg. {War Ghoul} when recruited, {Brigitte Gebauer} using her last life, {Kamiri wa Itherero}'s ability). [RTR 19960124] [LSJ 20090922] [ANK 20181022]"
   - "[ACTION MODIFIER] If played on a diablerie, can be played before or after getting a Discipline card (if any), but must be played before the Blood Hunt. [RTR 19991206]"
 100585|Drawing Out the Beast:
   - "[ANI] The additional damage done during the press step is environmental. [RTR 19970630]"
 100588|Dreams of the Sphinx:
-  - "Cannot move blood to Imbued in the uncontrolled region. [LSJ 20070516]"
-  - 'Cannot be used when a card is played to draw a card that would cancel it "as it is played". [RTR 20040501]'
-  - "Cards that are not replaced count against the hand size. [ANK 20180318]"
+  - Cannot move blood to Imbued in the uncontrolled region. [LSJ 20070516]
+  - Cannot be used when a card is played to draw a card that would cancel it "as it is played". [RTR 20040501]
+  - Cards that are not replaced count against the hand size. [ANK 20180318]
+  - The hand size bonus ends during the discard phase, it can be ordered as the acting Methuselah wishes against other end-of-turn and discard phase effects, following normal sequencing rules. [LSJ 20020904-2]
+100589|Drink the Blood of Ahriman:
+  - During the unlock phase, the controller chooses between burning 1 blood or the card. Reversal of previous rulings. [ANK 20220503]
 100591|Drum of Xipe Totec:
-  - "The minion cannot use the discipline nor the maneuver provided if some effect prevents him to use the equipment (eg. {Drawing Out the Beast}). [RTR 20010710]"
+  - The minion cannot use the discipline nor the maneuver provided if some effect prevents him to use the equipment (eg. {Drawing Out the Beast}). [RTR 20010710]
 100592|Dual Form:
   - "[PRO] A vampire's capacity can never be reduced below one. [RTR 19990712]"
   - "[PRO] The disciplines are copied when the action resolves, including any additional disciplines (eg. {Seal of Veddartha}). Disciplines gained after the action are not copied. [ANK 20170226]"
+  - "[PRO] Only the clan, sect, capacity and disciplines are copied. Titles and other traits like Infernal or Scarce are not. [LSJ 20050116]"
+  - "[PRO] The reduction in capacity happens first: the copy also has a reduced capacity. [LSJ 20050116]"
   - "[PRO] If one of the pair leaves the ready region, the other is burned. That burning of the other won't cause the first to burn. [LSJ 20050117]"
-  - "[PRO] If they are more than two Dual Forms of the same vampires, all the other are burned when one leaves the ready region, whatever chain they form. [LSJ 20050117]"
-  - "[PRO] If more than one go to torpor at the same time (eg. from {Edged Illusion}), the controller chooses which one he keeps. [LSJ 20050805]"
+  - "[PRO] If they are more than two Dual Forms of the same vampires, all the others are burned when one leaves the ready region, whatever chain they form. [LSJ 20050117]"
+  - "[PRO] If more than one go to torpor at the same time (eg. from {Edged Illusion}), the controller chooses which one they keep. [LSJ 20050805]"
   - "[PRO] The reduction in capacity is permanent, even if the Dual Form is burned. It still applies in the uncontrolled region if the vampire gets back into it. [LSJ 20051103]"
 100596|Dust to Dust:
-  - "The press and maneuver can only be used during the current round. [TOM 19960521]"
+  - The press and maneuver can only be used during the current round. [TOM 19960521]
 100597|Dust Up:
   - "[ani] [pot] Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - "[cel] The additional strike is not optional: you cannot play it for the dodge only if you already played it for a (limited) additional strike this round. [ANK 20220204]"
+  - "[ani] Does not prevent the opponent from dodging, the dodge just has no effect. [LSJ 20030902-2] [LSJ 20060808-1]"
 100598|Eagle's Sight:
   - "[AUS] Only affects the rule restricting who gets to block an action. The vampire must still meet all other requirements to block. In particular, {Blood Bond}, {Day Operation}, {Seduction} and prior decision not to block are not circumvented. [RTR 19950413] [RTR 20020501]"
   - "[AUS] Only applies to one block attempt. If the action later continues as if unblocked (eg.{Form of Mist}), another one is needed. [LSJ 20030227]"
+100599|Ears of the Hare:
+  - "[pro] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {The Path of the Feral Heart}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 100601|Earth Meld:
   - "[PRO] The vampire still unlocks if an effect continues the combat or begins a new combat. [RTR 20020501]"
+100604|Earthshock:
+  - Can be used at long range to target a retainer, even if their employer has flight [FLIGHT]. [LSJ 20060509]
+  - Does not prevent the opponent from dodging, the dodge just has no effect. [LSJ 20030902-2] [LSJ 20060808-1]
 100607|Eccentric Billionaire:
-  - 'The "lock to reduce the cost" effect can be used when the action is announced or when the cost is paid. [LSJ 20090705] [ANK 20170605]'
-  - "He can lock to use his ability the turn he is recruited. [ANK 20180517]"
+  - The "lock to reduce the cost" effect can be used when the action is announced or when the cost is paid. [LSJ 20090705] [ANK 20170605]
+  - He can lock to use his ability the turn he is recruited. [ANK 20180517]
 100608|Echo of Harmonies:
   - "[mel] [MEL] Can only be played by the controller of the acting minion. [LSJ 19990425]"
   - "[mel] [MEL] Can be played by a locked vampire. [LSJ 19980210]"
   - "[mel] [MEL] Multiple copies can be played by different minions on the same action. [ANK 20200515]"
   - "[MEL] Cannot be used if no political action card was played or if it is not in the ash heap (eg. cannot retrieve a {National Guard Support} when its text is used to burn it). [LSJ 20020911]"
   - "[MEL] The effect is lost if the political action card is not in the ash heap when it resolves (eg. if {Delaying Tactics} is used}). [LSJ 20050804]"
   - "[MEL] When the retained political action is played, requirements must be met, it provides 1 vote and can be canceled as it is played. [LSJ 20100426] [LSJ 20091128] [LSJ 20011205]"
   - "[MEL] The retained political action can not be played with {Charming Lobby}. [ANK 20201029]"
 100610|Ecstasy:
   - '[SER] The acting player decides the order of (and can play other) "after resolving the action" effects. [ANK 20180206]'
 100615|Edged Illusion:
   - "[CHI] If some minions cannot be targeted because of another effect, the action will simply have no effect on the things it cannot target. [RTR 20080808]"
 100618|Elder Intervention:
-  - "Can be used during any bleed attempt made against you, not just ones declared against you. [RTR 19960530]"
+  - Can be used during any bleed attempt made against you, not just ones declared against you. [RTR 19960530]
+100620|Elder Library:
+  - If there is another copy in play, it enters contest without modifying the hand size. [ANK 20221028]
 100623|The Eldest Command Undeath:
-  - "If you play {Voter Captivation} on the referendum, you can move up to 2 counters to your pool, and 0 to your vampire. [LSJ 20081002]"
+  - If you play {Voter Captivation} on the referendum, you can move up to 2 counters to your pool, and 0 to your vampire. [LSJ 20081002]
 100625|Elemental Stoicism:
   - "[for] Cannot be used if there is no damage to prevent. [LSJ 20001114]"
 100627|Elixir of Distillation:
-  - "Does not burn if combat ends before it resolves. [LSJ 20001127-2] [LSJ 20010806-1] [LSJ 19981006]"
+  - Does not burn if combat ends before it resolves. [LSJ 20001127-2] [LSJ 20010806-1] [LSJ 19981006]
 100628|Eluding the Arms of Morpheus:
-  - "Can be used by a vampire who is already attempting to block. [ANK 20181122-2]"
+  - Can be used by a vampire who is already attempting to block. [ANK 20181122-2]
+  - Cannot be used if the vampire cannot attempt to block the action (eg. {Daring the Dawn}). [LSJ 20010714-2]
 100634|Emerald Legionnaire:
-  - "His ability cannot be used from the ash heap, he needs to be ready. [ANK 20180511-1]"
-  - "When using his ability to put another one into play, it does not require a ready Harbinger, the pool cost of the new one is not paid, the new one can act this turn and can use his ability to bring another one immediately. [ANK 20180509]"
+  - His ability cannot be used from the ash heap, he needs to be ready. [ANK 20180511-1]
+  - When using his ability to put another one into play, it does not require a ready Harbinger, the pool cost of the new one is not paid, the new one can act this turn and can use his ability to bring another one immediately. [ANK 20180509]
 100635|Emergency Powers:
-  - "The burn option can be used if all your Seraph are in torpor. [LSJ 20091203]"
+  - The burn option can be used if all your Seraph are in torpor. [LSJ 20091203]
 100639|Empowering the Puppet King:
-  - "Can only be played by the controller of the acting minion. [LSJ 19990425]"
+  - Can only be played by the controller of the acting minion. [LSJ 19990425]
 100641|Enchanted Marionette:
-  - "The effect is not optional. [RTR 19980707] [LSJ 19980722]"
+  - The effect is not optional. [RTR 19980707] [LSJ 19980722]
 100645|Enkil Cog:
-  - "If locked to take an action and the action is canceled as it is played (not if it is canceled after, eg. with {Tangle Atropos' Hand}), it stays locked and the minion can choose to take an action again or let the Cog effect be lost. [LSJ 20081213-1] [ANK 20210124]"
+  - If locked to take an action and the action is canceled as it is played (not if it is canceled after, eg. with {Tangle Atropos' Hand}), it stays locked and the minion can choose to take an action again or let the Cog effect be lost. [LSJ 20081213-1] [ANK 20210124]
 100646|Ennoia's Theater:
-  - "Only requires one clan or the other (Gangrel or Gangrel antitribu) to be played. [ANK 20190203]"
-  - "Can be used at any moment during the influence phase to get the additional transfer. [RTR 20180303]"
+  - Only requires one clan or the other (Gangrel or Gangrel antitribu) to be played. [ANK 20190203]
+  - Can be used at any moment during the influence phase to get the additional transfer. [RTR 20180303]
 100647|Enrage:
   - "[PRE] If the vampire cannot burn 2 blood, he cannot attempt an action other than hunt or enter combat. [ANK 20180327]"
+  - "[PRE] If the vampire it is on attempts an action and it is canceled (eg. {Direct Intervention}) they do not burn 2 blood. [LSJ 20090208]"
 100648|Ensconced:
   - "[VIS][REACTION] The action still continues until the end of combat. The acting minion stays the same, effects applied during the action still applies during combat. [LSJ 20070217]"
   - "[VIS][REACTION] Modifiers and reactions that can be used at the end/after an action can still be used after combat. [LSJ 20041022]"
 100650|Enticement:
-  - "Is directed at your prey. [LSJ 20010807]"
-  - "If the edge is lost during the action (eg. {High Priest Angra Mainyu}), the prey takes no damage but you still cannot bleed anymore this turn. [LSJ 20100527]"
+  - Is directed at your prey. [LSJ 20010807]
+  - If the edge is lost during the action (eg. {High Priest Angra Mainyu}), the prey takes no damage but you still cannot bleed anymore this turn. [LSJ 20100527]
+100651|Entombment:
+  - Only effective at close range. [RBK 20200701-10] [LSJ 20000110]
+  - "[OBT] The opponent is wounded (if they play {Undying Tenacity}, they go to torpor after combat). [LSJ 20090622-2]"
 100656|The Erciyes Fragments:
-  - 'Cannot be used when a card is played to draw a card that would cancel it "as it is played". [RTR 20040501]'
-  - "If used to play a political action and {Delaying Tactics} is played, the political action card goes to its owner's hand. [LSJ 20050322]"
-  - "All other players can see which card is selected from the ash heap. [ANK 20200523]"
+  - Cannot be used when a card is played to draw a card that would cancel it "as it is played". [RTR 20040501]
+  - If used to play a political action and {Delaying Tactics} is played, the political action card goes to its owner's hand. [LSJ 20050322]
+  - All other players can see which card is selected from the ash heap. [ANK 20200523]
 100658|Erosion:
-  - "Erosion resets a minion's base strength. Any modifiers, including inherent modifiers, are applied to the new base. If another effect like {Torn Signpost} later resets the base damage again, then the new amount wins out. [LSJ 19971211-2]"
+  - Erosion resets a minion's base strength. Any modifiers, including inherent modifiers, are applied to the new base. If another effect like {Torn Signpost} later resets the base damage again, then the new amount wins out. [LSJ 19971211-2]
 100661|Escaped Mental Patient:
-  - "Must choose when declaring strike between a normal hand strike or the aggravated hand strike his ability gives him. [ANK 20190717-2]"
-  - 'Does not burn at the end of combat if another effect let him make a hand strike at +1 damage. "If he does so" only applies if his own effect is used directly. [LSJ 20001127-2] [RTR 20020501]'
-  - "Does not burn at the end of combat if his strike does not resolve (eg. if his opponent uses a strike: combat ends). [LSJ 20001127-2] [LSJ 20010627]"
+  - Must choose when declaring strike between a normal hand strike or the aggravated hand strike his ability gives him. [ANK 20190717-2]
+  - Does not burn at the end of combat if another effect let him make a hand strike at +1 damage. "If he does so" only applies if his own effect is used directly. [LSJ 20001127-2] [RTR 20020501]
+  - "Does not burn at the end of combat if his strike does not resolve (eg. if his opponent uses a strike: combat ends or {Rötschreck} is played). [LSJ 20001127-2] [LSJ 20010627] [LSJ 20070508]"
+  - If his strike resolves, he cannot be saved from burning (with eg. {Heaven's Gate} of {Left for Dead}). [LSJ 20070507] [LSJ 20021205]
 100665|The Eternal Mask:
-  - "You cannot use the effect to burn the card and the vampire if the vampire is no longer in play to be burned. [LSJ 20070928-1]"
-  - "You still cannot burn it if the vampire that was brought back was burned and later returned to play. [LSJ 20040726] [ANK 20191031]"
-  - "[SER] is not a directed action, even when targeting another Methusalah's ash heap. [LSJ 20010627] [ANK 20181129]"
-  - "If The Eternal Mask is burned by something else than its own effect (including when the vampire it is on is burned), the vampire that has been brought back is unaffected. [LSJ 20071206] [LSJ 20090725]"
+  - You cannot use the effect to burn the card and the vampire if the vampire is no longer in play to be burned. [LSJ 20070928-1]
+  - You still cannot burn it if the vampire that was brought back was burned and later returned to play. [LSJ 20040726] [ANK 20191031-2]
+  - "[SER] is not a directed action, even when targeting another Methuselah's ash heap. [LSJ 20010627] [ANK 20181129]"
+  - If The Eternal Mask is burned by something else than its own effect (including when the vampire it is on is burned), the vampire that has been brought back is unaffected. [LSJ 20071206] [LSJ 20090725]
 100666|Eternal Vigilance:
-  - "Cannot be used if the vampire cannot attempt to block the action (eg. {Daring the Dawn}). [LSJ 20010714-2]"
-  - "The block attempt and subsequent combat still happen if the action lacks a suitable target because of the unlock (eg. {Ambush}). [LSJ 20090514]"
+  - Cannot be used if the vampire cannot attempt to block the action (eg. {Daring the Dawn}). [LSJ 20010714-2]
+  - When used to block, does not ignore the normal prey, predator or target restrictions. [ANK 20180623]
+  - The block attempt and subsequent combat still happen if the action lacks a suitable target because of the unlock (eg. {Ambush}). [LSJ 20090514]
 100667|The Eternals of Sirius:
-  - "Pay the cost at the same time you gain pool from it, you do not get ousted in between. [LSJ 20020620] [LSJ 20080612]"
+  - Pay the cost at the same time you gain pool from it, you do not get ousted in between (ie. can be played when at 4 pool). [LSJ 20020620] [LSJ 20080612]
+  - You must be able to pay the cost to play it (ie. cannot be played when at 3 pool). [ANK 20210714-2]
 100668|Evil Eye:
-  - "The burn option can be used if all your vampires with [mal] are in torpor. [LSJ 20091203]"
+  - The burn option can be used if all your vampires with [mal] are in torpor. [LSJ 20091203]
 100669|Ex Nihilo:
-  - "During the unlock phase, the blood must be paid if able: the vampire cannot decide to burn instead. [PIB 20121013]"
-  - "If the owner treats aggravated damage as normal, he is immune to them too. [LSJ 20040120]"
+  - During the master phase, the controller chooses between paying the blood or burning the vampire. Reversal of previous rulings. [ANK 20220503]
+  - Any effect that would give more blood to the vampire is a gain of blood, so does not apply (eg. {Heidelberg Castle, Germany}). [ANK 20221019-2]
+  - If the owner treats aggravated damage as normal, he is immune to them too. [LSJ 20040120]
 100675|Extortion:
-  - "Is usable by a locked vampire [LSJ 20010725]"
+  - Is usable by a locked vampire [LSJ 20010725]
 100676|Extremis Boon:
-  - "The pool of the highest bidder goes to the target Methusalah. The loosers do not lose pool. [LSJ 20031121-1]"
-  - "The starting bid must be enough to keep the target into play. [ANK 20190827]"
+  - The pool of the highest bidder goes to the target Methuselah. The loosers do not lose pool. [LSJ 20031121-1]
+  - The starting bid must be enough to keep the target into play. [ANK 20190827]
 100680|Eyes of Argus:
   - "[AUS] The vampire need not attempt to block nor play further reaction cards: that is merely an option. [TOM 19951129]"
   - "[AUS] Can be played after action resolution to use a reaction card (eg. {Fast Reaction} after combat). [LSJ 20091123]"
 100683|Eyes of the Beast:
   - "[PRO] The maneuver is only available during the action in which Eyes of the Beast was played. [ANK 20191108]"
   - "[PRO] If the action is blocked but continues after combat (eg. with {Form of Mist}) and the reacting vampire blocks again, he gets the maneuver again. [ANK 20191108]"
 100687|Faceless Night:
   - "[OBF] A minion attempting to block before it is played cannot back out. [LSJ 20081202]"
   - "[OBF] A minion that has attempted to block but failed before it was played is not affected. [ANK 20190509]"
   - '[OBF] The lock of the minion happens at action resolution. He can play a reaction before that (eg. {Deflection}), and he still locks if he unlocked before that (eg. with {Guard Dogs}). Only cards that can be played "after action resolution" can be played after the lock happens. [ANK 20171017]'
+100689|Fae Contortion:
+  - '[myt] [REFLEX] Cards are not replaced during the "as played" window. [LSJ 20061013]'
+  - '[myt] [REFLEX] If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
 100690|Faerie Wards:
   - '[MYT] The "does not unlock as normal" effect is redundant with being infernal. If the minion is infernal, its controller can still pay a pool to unlock them. [LSJ 20050114]'
   - "[myt], [MYT] Modifiers and reactions that can be used at the end/after an action can still be used afterwards. [LSJ 20041022]"
 100694|Falcon's Eye:
+  - "[ani] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Dragos}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
   - "[SPI] Only affects the rule restricting who gets to block an action. The vampire must still meet all other requirements to block. In particular, {Blood Bond}, {Day Operation}, {Seduction} and prior decision not to block are not circumvented. [RTR 19950413] [LSJ 20020112] [RTR 20020501]"
   - "[SPI] Only applies to one block attempt. If the action later continues as if unblocked (eg.{Form of Mist}), another one is needed. [LSJ 20030227]"
 100695|Fall of the Camarilla:
-  - "Cards that change a vampire's sect to Camarilla can still be played, but he becomes Independant until the Fall is removed from play. [LSJ 20040519]"
-  - "Is a temporary effect that overrides the underlying sect. The most recent override takes precendence, but if a more recent would set the sect to Camarilla, it sets it to Independant instead while the Fall is in play. If the Fall leaves play, the vampire retrieves his underlying sect. [LSJ 20080510] [LSJ 20100811] [ANK 20190619]"
-  - "Vampires with a Camarilla title lose the benefit from it until they becomre Camarilla again. They immediately yield the title if it is contested or if they receives a new one. [LSJ 20060904]"
+  - Cards that change a vampire's sect to Camarilla can still be played, but he becomes Independant until the Fall is removed from play. [LSJ 20040519]
+  - Is a temporary effect that overrides the underlying sect. The most recent override takes precendence, but if a more recent would set the sect to Camarilla, it sets it to Independant instead while the Fall is in play. If the Fall leaves play, the vampire retrieves his underlying sect. [LSJ 20080510] [LSJ 20100811] [ANK 20190619]
+  - Vampires with a Camarilla title lose the benefit from it until they becomre Camarilla again. They immediately yield the title if it is contested or if they receives a new one. [LSJ 20060904]
 100696|Fall of the Sabbat:
-  - "Cards that change a vampire's sect to Sabbat can still be played, but he becomes Independant until the Fall is removed from play. [LSJ 20040519]"
-  - "Is a temporary effect that overrides the underlying sect. The most recent override takes precendence, but if a more recent would set the sect to Sabbat, it sets it to Independant instead while the Fall is in play. If the Fall leaves play, the vampire retrieves his underlying sect. [LSJ 20080510] [LSJ 20100811] [ANK 20190619]"
-  - "Vampires with a Sabbat title lose the benefit from it until they becomre Sabbat again. They immediately yield the title if it is contested or if they receives a new one. [LSJ 20060904]"
+  - Cards that change a vampire's sect to Sabbat can still be played, but he becomes Independant until the Fall is removed from play. [LSJ 20040519]
+  - Is a temporary effect that overrides the underlying sect. The most recent override takes precendence, but if a more recent would set the sect to Sabbat, it sets it to Independant instead while the Fall is in play. If the Fall leaves play, the vampire retrieves his underlying sect. [LSJ 20080510] [LSJ 20100811] [ANK 20190619]
+  - Vampires with a Sabbat title lose the benefit from it until they becomre Sabbat again. They immediately yield the title if it is contested or if they receives a new one. [LSJ 20060904]
 100697|False Resonance:
   - "[CHI] Cannot be used to get stealth then cancel the [aus] card that provided intercept to the blocking minion. [ANK 20180201]"
+100698|Fame:
+  - Paying a pool during the unlock phase can be ordered with other unlock effects by the acting Methuselah, but must be handled before another Methuselah has the opportunity to use an unlock effect. [LSJ 20010121]
 100699|Familial Bond:
-  - "Cannot be played if intercept is not required (as per the rules, section 6.2.2). [ANK 20200329]"
-  - 'A locked vampire cannot use the "lock to fight" effect, even if he uses a wake effect. [PIB 20121107]'
+  - Cannot be played if intercept is not required (as per the rules, section 6.2.2). [ANK 20200329]
+  - A locked vampire cannot use the "lock to fight" effect, even if he uses a wake effect. [PIB 20121107]
 100703|Far Mastery:
-  - "Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
+  - Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]
 100704|Fast Hands:
-  - "Cannot be used if there is no weapon to steal. [RTR 19980928]"
+  - Cannot be used if there is no weapon to steal. [RTR 19980928]
 100705|Fast Reaction:
-  - "Effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]"
-  - "Cannot be used to start a new combat if there is already a pending combat queued. [RTR 20020501]"
+  - Effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]
+  - Cannot be used to start a new combat if there is already a pending combat queued. [RTR 20020501]
 100706|Fata Amria:
-  - '[CHI] [REACTION] Cards and effects that can be played "after resolution" (and only them) can be played after it. [ANK 20190425]'
+  - '[CHI] [REACTION] Is played after resolution, but still during the action. Action modifiers and effects that can be played "after resolution" can be played before or after it. [LSJ 19981028] [ANK 20190425]'
+  - The target can burn it at unlock even if they're already unlocked, but cannot burn it if they do not unlock as normal (eg. {Sensory Deprivation}). [LSJ 20010814-3] [LSJ 20020109]
+  - Does not prevent the opponent from dodging, the dodge just has no effect. [LSJ 20030902-2] [LSJ 20060808-1]
 100709|FBI Special Affairs Division:
-  - "Does not trigger if the ally is saved by {Left for Dead}. [PIB 20121028]"
-  - "Does not trigger if the ally is considered the acting minion during the combat (eg. {Nar-Sheptha}). [ANK 20180913-2]"
-  - "Does trigger if the ally burns by himself at the end of combat (eg. {Escaped Mental Patient}). [LSJ 20100527]"
+  - Does not trigger if the ally is saved by {Left for Dead}. [PIB 20121028]
+  - Does not trigger if the ally is considered the acting minion during the combat (eg. {Nar-Sheptha}). [ANK 20180913-2]
+  - Does trigger if the ally burns by himself at the end of combat (eg. {Escaped Mental Patient}). [LSJ 20100527]
 100710|Fear of Mekhet:
-  - "Can be moved (not played) on a vampire in torpor. [ANK 20210109]"
+  - Can be moved (not played) on a vampire in torpor. [ANK 20210109]
 100718|Feline Saboteur:
-  - "[ANI][OBF] The chosen Methusalah discards, then burn 4 cards, then replace the discarded card. [ANK 20180725]"
+  - "[ANI][OBF] The chosen Methuselah discards, then burn 4 cards, then replace the discarded card. [ANK 20180725]"
 100723|Festivo dello Estinto:
-  - "The hunt bonus applies to non-standard hunt actions, it comes from the blood bank not from the target of the hunt [RTR 20030519]"
-  - "A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]"
+  - The hunt bonus applies to non-standard hunt actions, it comes from the blood bank not from the target of the hunt [RTR 20030519]
+  - A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]
 100725|Field Training:
-  - "Is a change of the actual sect. A temporary effect overriding the sect has precendence and if it does, this card burns (eg. {Writ of Acceptance}). [LSJ 20100811]"
-  - "If the target changes sect to a sect inappropriate for his title, he loses its benefit until his sect is appropriate. He immediately yields the title if it is contested or he receives a new one. [LSJ 20060904]"
-  - "The acting vampire must have a superior discipline to choose from. [ANK 20180731-2]"
+  - Is a change of the actual sect. A temporary effect overriding the sect has precendence and if it does, this card burns (eg. {Writ of Acceptance}). [LSJ 20100811]
+  - If the target changes sect to a sect inappropriate for his title, he loses its benefit until his sect is appropriate. He immediately yields the title if it is contested or he receives a new one. [LSJ 20060904]
+  - The acting vampire must have a superior discipline to choose from. [ANK 20180731-2]
 100728|Filchware's Pawn Shop:
-  - "Cannot be used to replay a card that can be played only once in a game. [LSJ 20040518]"
+  - Cannot be used to replay a card that can be played only once in a game. [LSJ 20040518]
 100730|Final Loosening:
   - "[for] Modifiers and reactions that can be used at the end/after an action can still be used afterwards. [LSJ 20041022]"
 100733|Fire Dance:
-  - "The target vampire is chosen when the action is announced. [RTR 19970425]"
+  - The target vampire is chosen when the action is announced. [RTR 19970425]
 "100737|First Tradition: The Masquerade":
-  - "One or the other condition must be met fully for it to be burned. It is not burned if the controller skips two turns and pay 4 pool to play two other. [LSJ 20031011]"
-  - "The burn pool effect is cumulative with other copies (if there are two of them, you burn 4 pool to play your turn), the controller skipping a turn counts towards all his copies. [RTR 19941222]"
+  - One or the other condition must be met fully for it to be burned. It is not burned if the controller skips two turns and pay 4 pool to play two other. [LSJ 20031011]
+  - The burn pool effect is cumulative with other copies (if there are two of them, you burn 4 pool to play your turn), the controller skipping a turn counts towards all his copies. [RTR 19941222]
 100740|Flames of Insurrection:
-  - "If two Anarchs are in combat and both go to torpor, both controllers can benefit from the effect. [ANK 20180627-2]"
+  - If two Anarchs are in combat and both go to torpor, both controllers can benefit from the effect. [ANK 20180627-2]
+100741|Flames of the Netherworld:
+  - "[tha] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Uta Kovacs}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 100743|Flaming Candle:
-  - "Is not burned if another effect make the vampire burn 1 blood upon action declaration. [RTR 20020501]"
-  - 'If it has been equipped or played already, an effect can still "put it into play" provided it is not an "equip" action (eg. {Kiss of Lachesis}, {Grasp the Ghostly}). [LSJ 20060209]'
+  - Is not burned if another effect make the vampire burn 1 blood upon action declaration. [RTR 20020501]
+  - If it has been equipped or played already, an effect can still "put it into play" provided it is not an "equip" action (eg. {Kiss of Lachesis}, {Grasp the Ghostly}). [LSJ 20060209]
+  - Once in play, it can be moved (eg. {Heidelberg Castle, Germany}), or equipped by another minion from the minion who has it. [ANK 20221103]
 100745|Flash Grenade:
-  - 'If the opponent dodges, the "is locked and does not unlock as normal" effect do not apply, but it still burns. [RTR 20041202] [LSJ 20060808]'
-  - 'If the combat continues or a new combat begins, the "is locked and does not unlock as normal" effect do not apply, but it still burns. [RTR 20020501] [LSJ 20040601], '
+  - If the opponent dodges, the "is locked and does not unlock as normal" effect do not apply, but it still burns. [RTR 20041202] [LSJ 20060808]
+  - 'If the combat continues or a new combat begins, the "is locked and does not unlock as normal" effect do not apply, but it still burns. [RTR 20020501] [LSJ 20040602], '
+  - If the opponent unlocks before combat ends (eg. {Majesty}), the Grenade locks them again after it ends. [LSJ 20040601]
   - 'Still burns when used if the opponent uses a "strike: combat ends" too. It does not if combat ends before strike resolution (eg. {Rötschreck}). [LSJ 20001127-2] [LSJ 20010806-1]'
 100747|Fleetness:
   - "[CEL] If the target unlocks and the action is not blocked, it is successful but has no effect. [LSJ 20070411] [LSJ 20090514]"
 100749|Flesh of Marble:
-  - "The vampire preventing the damage can choose which one of the damage he does not prevent, normal or aggravated. [LSJ 20021001]"
+  - "[pro] Cannot be used to prevent aggravated damage, even if the minion treats them as normal damage (eg. {Skin of Night}). [LSJ 20040812-2] [PIB 20130327]"
+  - "[PRO] The vampire preventing the damage can choose which one of the damage he does not prevent, normal or aggravated. [LSJ 20021001]"
 100750|Fleshcraft:
-  - "The action to burn Fleshcraft suffers the -1 stealth penalty as well, so is usually at zero stealth to start (or -1 stealth if superior [VIC]). [LSJ 19970224]"
-  - "The rest of the effect applies if the damage is prevented, it does not if it is dodged. [LSJ 19990106-2]"
+  - The action to burn Fleshcraft suffers the -1 stealth penalty as well, so is usually at zero stealth to start (or -1 stealth if superior [VIC]). [LSJ 19970224]
+  - The rest of the effect applies if the damage is prevented, it does not if it is dodged. [LSJ 19990106-2]
 100751|Flow Within the Mountain:
   - '[VIS] If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]'
-  - '[VIS] If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
+  - '[VIS] If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
   - '[VIS] An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]'
   - '[VIS] "continue as if unblocked" moves the action card from the ash heap (where it went when the action was blocked) to limbo (where it should be if the action is not blocked). If the action card is not in the ash heap, then the action cannot be continued. [LSJ 20070808-1]'
   - '[VIS] If the combat continues or a new combat begins, the "action continues as if unblocked" effect is lost. [LSJ 19980109] [RTR 20020501]'
 100755|Folderol:
-  - "[MYT] If another Methusalah is the target, he must declare whether he attempts or declines to block before Folderol can be played. [PIB 20150820]"
+  - "[aus] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Helena (ADV)}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
+  - "[MYT] If another Methuselah is the target, he must declare whether he attempts or declines to block before Folderol can be played. [PIB 20150820]"
 100756|Follow the Alpha:
-  - "Effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]"
-  - "Cannot be used to start a new combat if there is already a pending combat queued. [RTR 20020501]"
+  - Effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]
+  - Cannot be used to start a new combat if there is already a pending combat queued. [RTR 20020501]
 100757|Follow the Blood:
-  - "If played on a vampire who successfully hunts with a {Perfectionist}, {Perfectionist} grants the blood before combat. [LSJ 20110308]"
-  - 'Is played after resolution, but still during the action. Cards and effects that played "after resolution" (eg. {Freak Drive}) can be played before it, but not after. [LSJ 19981028] [LSJ 20100206-2]'
+  - If played on a vampire who successfully hunts with a {Perfectionist}, {Perfectionist} grants the blood before combat. [LSJ 20110308]
+  - Is played after resolution, but still during the action. Cards and effects that played "after resolution" (eg. {Freak Drive}) can be played before it, but not after. [LSJ 19981028] [LSJ 20100206-2]
 100758|Force of Personality:
-  - '[PRE] [ACTION MODIFIER] Cards and effects that can be played "as the action is announced" (and only them) can be played before it. [ANK 20190425]'
+  - '[PRE] [ACTION MODIFIER] Cards and effects that are played "as the action is announced" must be played before playing "regular" action modifier or reaction cards. [ANK 20190425]'
+  - "[PRE] [ACTION MODIFIER] Replace the action card (if any) before playing it. [ANK 20181208]"
 100759|Force of Will:
-  - "If the action does not reach resolution (eg. {The Kiss of Ra}), the damage is not done. If the action merely ends (eg. {Change of Target}) or has no effect (eg. because cost cannot be paid), the damage occurs as normal. [RTR 20020501] [LSJ 20020927] [ANK 20210124]"
+  - The damage is applied if the action reaches resolution, even if it ends before combat (eg. {Mirror Walk}, {Change of Target}, {Red Herring}) or has no effect (eg. because cost cannot be paid). [ANK 20220331] [ANK 20210124] [LSJ 20020927] [LSJ 20021115] [ANK 20221011-2]
+  - The damage is not applied if the action is canceled before resolution (eg. {Tangle Atropos' Hand}, {The Kiss of Ra}). [ANK 20220401] [ANK 20211015] [ANK 20210124]
   - "{Mask of a Thousand Faces} cannot be used to take over, since it requires an unlocked vampire and the action requires a locked one. [LSJ 20020927]"
+  - Cards usable after action resolution (eg. {Freak Drive}) can be played before or after the damage is taken. [LSJ 20010715]
 100760|Forced Awakening:
   - "The vampire need not attempt to block nor play further reaction cards: that is merely an option. [TOM 19951129]"
-  - "If he fails to block, the vampire only burns a blood when the action begins to resolve (successfully or not). He can pay for reactions after declining to block, before burning a blood. [LSJ 19990421]"
-  - "Can be played after action resolution to use a reaction card (eg. {Fast Reaction} after combat). [LSJ 20091123]"
-  - "The vampire needs not pay a blood if he successfully blocks, even if the action continues as if unblocked after the block (eg. {Form of Mist}). [LSJ 20070417]"
+  - If he fails to block, the vampire only burns a blood when the action begins to resolve (successfully or not). He can pay for reactions after declining to block, before burning a blood. [LSJ 19990421]
+  - Can be played after action resolution to use a reaction card (eg. {Fast Reaction} after combat). [LSJ 20091123]
+  - The vampire needs not pay a blood if he successfully blocks, even if the action continues as if unblocked after the block (eg. {Form of Mist}). [LSJ 20070417]
 100761|Forced March:
-  - '[cel][for] Cards and effects that can be played "after resolution" (and only them) can be played after it. [ANK 20190425]'
-  - "Can be used to unlock if the action is unblocked, even if it has no effect due to lack of a suitable target. [LSJ 20070411]"
+  - '[cel][for] Is played after resolution, but still during the action. Action modifiers and effects that can be played "after resolution" can be played before or after it. [LSJ 19981028] [ANK 20190425]'
+  - Can be used to unlock if the action is successful, even if it has no effect due to lack of a suitable target. [LSJ 20070411]
 100763|Forearm Block:
-  - "Prevents up to 2 damage, it can be used to prevent less. [RTR 20041202]"
+  - Prevents up to 2 damage, it can be used to prevent less. [RTR 20041202]
 100764|Foresee:
-  - 'If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]'
-  - 'If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
-  - 'An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]'
+  - If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]
+  - If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]
+  - An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]
   - '"continue as if unblocked" moves the action card from the ash heap (where it went when the action was blocked) to limbo (where it should be if the action is not blocked). If the action card is not in the ash heap, then the action cannot be continued. [LSJ 20070808-1]'
 100765|Foreshadowing Destruction:
-  - "[DOM] Can be played against a target with 10 or more pool and does not count against the limit in this case: it will only have a lingering effect (+3 bleed if the target happens to have 9 or less). [PIB 20110817]"
-  - "[DOM] When played against a target with 10 or more pool, it can be played alongside another bleed modifier that counts against the limit, and it would provide its +3 bonus in addition to that other bleed modifier if the target happens to have 9 or less. [PIB 20110817]"
+  - "[DOM] Can be played against a target with 10 or more pool and does not count against the limit in this case: it will only have a lingering effect (+3 bleed if the target happens to have 9 or less). [PIB 20110817] [ANK 20191031]"
+  - "[DOM] If the bleed bonus is lost during the action (eg. {Deflection} to another target), it does not count against the limit anymore and an additional bleed modifier can be used. [ANK 20191031] [ANK 20211019-2]"
 100766|Forest of Shadows:
-  - "May be used anytime it is unlocked, even if it has been used previously during the same action (it must be unlocked by some method, of course). [TOM 19960109]"
+  - May be used anytime it is unlocked, even if it has been used previously during the same action (it must be unlocked by some method, of course). [TOM 19960109]
 100767|Forger's Hammer:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 100771|Form of Mist:
   - '[PRO] If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]'
-  - '[PRO] If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
+  - '[PRO] If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
   - '[PRO] An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]'
   - '[PRO] "continue as if unblocked" moves the action card from the ash heap (where it went when the action was blocked) to limbo (where it should be if the action is not blocked). If the action card is not in the ash heap, then the action cannot be continued. [LSJ 20070808-1]'
   - '[PRO] If the combat continues or a new combat begins, the "action continues as if unblocked" effect is lost and the blood is not paid. [LSJ 19980109] [RTR 20020501] [LSJ 20031123]'
 100778|Foul Blood:
-  - "A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]"
+  - A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]
 100784|Fractured Armament:
-  - "Cannot be used if there is no equipment to destroy. [RTR 19980928]"
+  - Cannot be used if there is no equipment to destroy. [RTR 19980928]
   - "[pot] Is not a damaging strike. [LSJ 19970225]"
   - "[POT] Is a damaging strike. [LSJ 19970225]"
 100785|Fragment of the Book of Nod:
-  - 'Cannot be used when a card is played to draw a card that would cancel it "as it is played". [RTR 20040501]'
+  - Cannot be used when a card is played to draw a card that would cancel it "as it is played". [RTR 20040501]
 100788|Freak Drive:
   - "[FOR] Is played after all combats are handled. Can be played from torpor. [RTR 19980623] [LSJ 20030103] [ANK 20180906]"
   - "[for] Can be played if the action is unblocked even if it has no effect due to lack of a suitable target. [LSJ 20070411]"
   - "[for] Is played after the action resolves. (eg. if played after equipping {Learjet}, you draw an additional card). [PIB 20150915]"
 100790|Free States Rant:
-  - "If there are insuffient targets to which to allocate all of the points allowed, then the card cannot be played. [LSJ 20010810]"
+  - If there are insuffient targets to which to allocate all of the points allowed, then the card cannot be played. [LSJ 20010810]
 100791|Frenzy:
-  - "Only prevents the use of equipment after it is played - it will not cancel the effects of equipment used before it is played. [TOM 19960326]"
+  - Only prevents the use of equipment after it is played - it will not cancel the effects of equipment used before it is played. [TOM 19960326]
 100793|From a Sinking Ship:
-  - "Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
+  - Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]
+100794|Frontal Assault:
+  - If you play more than one, you gain and loose pool for all of them (they stack). [LSJ 20061018]
 100798|Galaric's Legacy:
-  - "Is a change of the actual sect. A temporary effect overriding the sect has precendence and if it does, this card burns (eg. {Writ of Acceptance}). [LSJ 20100811]"
-  - "If the target changes sect to a sect inappropriate for his title, he loses its benefit until his sect is appropriate. He immediately yields the title if it is contested or he receives a new one. [LSJ 20060904]"
+  - Is a change of the actual sect. A temporary effect overriding the sect has precendence and if it does, this card burns (eg. {Writ of Acceptance}). [LSJ 20100811]
+  - If the target changes sect to a sect inappropriate for his title, he loses its benefit until his sect is appropriate. He immediately yields the title if it is contested or he receives a new one. [LSJ 20060904]
 100799|Gambit Accepted:
-  - "If the controller of a Gambit in play withdraws, his or her predator gets a VP from the Gambit (the Methuselah who withdraws still gets a VP for withdrawing, of course). [RTR 20040501]"
+  - If the controller of a Gambit in play withdraws, his or her predator gets a VP from the Gambit (the Methuselah who withdraws still gets a VP for withdrawing, of course). [RTR 20040501]
 100801|Games of Instinct:
-  - "The gain blood effect is applied after combats ends, no combat card can be played afterwards. The acting player chooses the order of after-combat effects. [LSJ 20100324]"
+  - The gain blood effect is applied after combats ends, no combat card can be played afterwards. The acting player chooses the order of after-combat effects. [LSJ 20100324]
 100805|Gangrel Conspiracy:
-  - "May be played before, during, or after votes and ballots have been cast. [LSJ 19980130]"
+  - Can only be played if a Blood Hunt referendum succeeds, after votes and ballots have been cast. [LSJ 20081203-2]
 100808|Gargoyle Slave:
-  - 'Does not count as a "slave" nor as a "Gargoyle" for game purposes. He is just an ally. [LSJ 20011210-4]'
+  - Does not count as a "slave" nor as a "Gargoyle" for game purposes. He is just an ally. [LSJ 20011210-4]
+100810|Garrote:
+  - The ability to burn an opponent going to torpor is not part of the strike. It can be used if the opponent dodges the strike but is still going to torpor. [ANK 20210612] [LSJ 20020416-2]
 100812|Gather:
-  - "Only usable to move the target vampire from your uncontrolled region to your ready region. It cannot rescue a vampire from torpor. [LSJ 20030520-1]"
+  - Only usable to move the target vampire from your uncontrolled region to your ready region. It cannot rescue a vampire from torpor. [LSJ 20030520-1]
 100813|Gear Up:
   - "[nec] The card to retrieve must be announced when declaring the action. [LSJ 20010627]"
 100814|Gemini's Mirror:
-  - "Does not protect the minion's equipment, retainers, or any other cards on him. Just him and his blood. [LSJ 20031118]"
+  - Does not protect the minion's equipment, retainers, or any other cards on him. Just him and his blood. [LSJ 20031118]
 100816|Ghost-Eater:
-  - "This is not a directed action, even when targeting another Methusalah's ash heap. [LSJ 20010627] [ANK 20181129]"
+  - This is not a directed action, even when targeting another Methuselah's ash heap. [LSJ 20010627] [ANK 20181129]
 100817|Ghoul Escort:
-  - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
-  - "Cannot be used if blocked when leaving torpor, as no combat would happen. [ANK 20181122-1]"
-100818|Ghoul Messenger:
-  - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
+  - Cannot be used if blocked when leaving torpor, as no combat would happen. [ANK 20181122-1]
 100819|Ghoul Retainer:
-  - 'The Ghoul is never the "bearer" of the weapon that it uses. Any side-effect of using the weapon is applied to the employing minion, as normal. [TOM 19951114]'
-  - "Is not mortal, is a monster. [ANK 20200203-2]"
+  - The Ghoul is never the "bearer" of the weapon that it uses. Any side-effect of using the weapon is applied to the employing minion, as normal. [TOM 19951114]
+  - Damage is not inflicted at long range. [ANK 20210929]
 100820|Ghouled:
-  - 'The ally is recruited as a mortal and changed to a ghoul afterwards (eg. {Sunset Strip, Hollywood} can be used to reduce its cost). His "starting life" is still the base mortal amount. [LSJ 20030520-2]'
-100821|Ghouled Street Thug:
-  - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
-100822|The Ghouls of Plaza Morería:
-  - "Are not mortal, are a monster. [ANK 20200203-2]"
+  - The ally is recruited as a mortal and changed to a ghoul afterwards (eg. {Sunset Strip, Hollywood} can be used to reduce its cost). His "starting life" is still the base mortal amount. [LSJ 20030520-2]
+  - Goes to the ash heap when played, if it has been removed when the action succeeds, it has no effect. [ANK 20220805]
 100823|Gianna di Canneto:
-  - "She can use her ability to burn an equipment an opponent has commited to use as a strike (eg. by using the maneuver of a {.44 MAgnum}). In this case the opponent strike has no effect. [PIB 20141026]"
-  - "She can lock to use her ability the turn she is recruited. [ANK 20180517]"
+  - She can use her ability to burn an equipment an opponent has commited to use as a strike (eg. by using the maneuver of a {.44 Magnum}). In this case the opponent strike has no effect. [PIB 20141026]
+  - 'She cannot use her ability to inflict damage if a "Strike: combat ends" was used, or if combat ends due to first strike aggravated damage. [ANK 20211130]'
+  - She can lock to use her ability the turn she is recruited. [ANK 20180517]
 100824|Giant's Blood:
-  - "Cannot target an uncontrolled vampire. [LSJ 20061109]"
+  - Cannot target an uncontrolled vampire. [LSJ 20061109]
 100825|Gift of Bellona:
   - "[val] Can be used when fetching a weapon from another minion, even if other equipments are also retrieved. [ANK 20170326]"
 100827|Gift of Proteus:
-  - "The number of cards to put on it is announced when the action is declared, they must be in hand before drawing the replacement for this card. [PIB 20150428]"
-  - "At action resolution, the number of cards declared must be put on the card. If there are less cards available (eg. {Form of Mist} was played to continue the action), then all of them are put on the Gift. [PIB 20150428]"
+  - The number of cards to put on it is announced when the action is declared, they must be in hand before drawing the replacement for this card. [PIB 20150428]
+  - At action resolution, the number of cards declared must be put on the card. If there are less cards available (eg. {Form of Mist} was played to continue the action), then all of them are put on the Gift. [PIB 20150428]
 100828|Gift of Sleep:
   - "[obe] [ACTION MODIFIER][REACTION] The action ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20200207]"
 100832|Giulia Giovanni Abruzzina:
-  - "When setting the range for the round, no other effect can be used to reset the range. Skip the determine range step this round, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]"
-  - "She can lock to use her ability the turn she is recruited. [ANK 20180517]"
+  - When setting the range for the round, no other effect can be used to reset the range. Skip the determine range step this round, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]
+  - She can lock to use her ability the turn she is recruited. [ANK 20180517]
 100834|Glancing Blow:
-  - "Cannot be used if there is no damage to prevent. [LSJ 20001114]"
+  - Cannot be used if there is no damage to prevent. [LSJ 20001114]
 100836|Glaser Rounds:
-  - "Must wait until the second time a given gun is used in a given combat to play it. [RTR 19941109]"
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Must wait until the second time a given gun is used in a given combat to play it. [RTR 19941109]
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
+100839|Glutton:
+  - Can be used to unlock a ready Ishtarri with no blood. [LSJ 19970707]
 100840|Go Anarch:
-  - "Is not the default action, no blood is paid to become Anarch. [ANK 20181017]"
-  - "Is a change of the actual sect. A temporary effect overriding the sect has precendence and if it does, this card burns (eg. {Writ of Acceptance}). [LSJ 20100811]"
-  - "If the target changes sect to a sect inappropriate for his title, he loses its benefit until his sect is appropriate. He immediately yields the title if it is contested or he receives a new one. [LSJ 20060904]"
-"100843|Goodnight, Sweet Prince":
-  - "Can be used on your own crypt. [TOM 19960419]"
+  - Is not the default action, no blood is paid to become Anarch. [ANK 20181017]
+  - Is a change of the actual sect. A temporary effect overriding the sect has precendence and if it does, this card burns (eg. {Writ of Acceptance}). [LSJ 20100811]
+  - If the target changes sect to a sect inappropriate for his title, he loses its benefit until his sect is appropriate. He immediately yields the title if it is contested or he receives a new one. [LSJ 20060904]
+100841|Goblinism:
+  - "[pot] The action is directed at the Methuselah controlling the location, undirected if you control it. [RBK 20200701-9] [LSJ 20090324]"
+100843|Goodnight, Sweet Prince:
+  - Can be used on your own crypt. [TOM 19960419]
 100844|Goth Band:
-  - "The counter moved to your master card by Goth Band is transformed into the type of counter normally used by the target master card. [RTR 19970306]"
-  - "Your Goth Band cannot move a counter from a card you control. [RTR 19980707]"
+  - The counter moved to your master card by Goth Band is transformed into the type of counter normally used by the target master card. [RTR 19970306]
+  - Your Goth Band cannot move a counter from a card you control. [RTR 19980707]
 100845|Govern the Unaligned:
   - "[DOM] You do not reveal the target vampire. [LSJ 20010108]"
 100849|The Grandest Trick:
-  - 'The vampire as an ally has no "starting life" trait so {Vagabond Mystic} cannot give him life. [LSJ 20011214-1]'
-  - 'If the vampire has an ability to play Discipline-requiring cards "as if" he has that Discipline ({Ian Forestal}, for example), then the vampire may use that ability even while he is treated as an ally. In that case, he is treated just as an ally with that ability would be treated (spends life for blood costs, for example). Similarly for {Mata Hari}''s ability. [LSJ 20070301]'
+  - The vampire as an ally has no "starting life" trait so {Vagabond Mystic} cannot give him life. [LSJ 20011214-1]
+  - If the vampire has an ability to play Discipline-requiring cards "as if" he has that Discipline ({Ian Forestal}, for example), then the vampire may use that ability even while he is treated as an ally. In that case, he is treated just as an ally with that ability would be treated (spends life for blood costs, for example). Similarly for {Mata Hari}'s ability. [LSJ 20070301]
   - "{Left for Dead} can be used on the vampire. [LSJ 20100527]"
 100850|Grasp of the Python:
-  - "The press can only be used during the current round. [TOM 19960521]"
+  - The press can only be used during the current round. [TOM 19960521]
 100851|Grasp the Ghostly:
-  - "If the equipment is burned before it runs out of pathos counters, it goes to its owner's ash heap and is not removed from the game. [LSJ 20060209]"
+  - If the equipment is burned before it runs out of pathos counters, it goes to its owner's ash heap and is not removed from the game. [LSJ 20060209]
+100853|Great Symposium:
+  - Search the crypt for only one Kiasyd, not any number. [ANK 20210304]
+  - The search can fail, you still get to distribute 3 blood. [LSJ 20100306]
 100855|Gregory Winter:
-  - "Can use his action on a vampire with no blood. [RTR 20010711]"
-  - "Is not mortal, is a monster. [ANK 20200203-2]"
+  - Can use his action on a vampire with no blood. [RTR 20010711]
+100856|Gremlins:
+  - "[myt] Is directed against the Methuselah controlling the equipment, not the minion it's on. [LSJ 20090324]"
 100857|Grenade:
-  - "Damage done to the bearer is environmental. [LSJ 19970801]"
-  - "Does not burn nor inflict damage if combat ends before it resolves. [LSJ 20001127-2] [LSJ 20010806-1][LSJ 19981006]"
+  - Damage done to the bearer is environmental. [LSJ 19970801]
+  - Does not burn nor inflict damage if combat ends before it resolves. [LSJ 20001127-2] [LSJ 20010806-1] [LSJ 19981006]
 100858|Grey Thorne:
-  - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
+  - Can play cards requiring [cel] or [pot] but not both. [ANK 20180731-1]
 100861|Groundfighting:
-  - "Can cancel cards preventing the use of equipment if the target has a weapon. [LSJ 20050221]"
-  - 'Cannot cancel maneuvering, setting the range or strikes that "cannot be dodge". [LSJ 20050221]'
-  - "Cannot cancel that prevents additional strikes. [LSJ 20050221]"
-  - "Cannot cancel a card that removes the ability to strike completely. [LSJ 20050222]"
-  - "Can cancel superior {Thoughts Betrayed} and {Shape Mastery} (when the latter is used to cancel a strike). [LSJ 20050224-2]"
-  - "Cannot cancel a card that destroys or steals an equipment or weapon. [LSJ 20050221]"
-  - "Cannot cancel a card restricting the use of disciplines. [LSJ 20050221]"
-  - 'If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
+  - The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Salvador Garcia}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]
+  - Can cancel cards preventing the use of equipment if the target has a weapon. [LSJ 20050221]
+  - Cannot cancel maneuvering, setting the range or strikes that "cannot be dodge". [LSJ 20050221]
+  - Cannot cancel a card that prevents additional strikes or removes the ability to strike completely. [LSJ 20050221]
+  - Can cancel superior {Thoughts Betrayed} and {Shape Mastery} (when the latter is used to cancel a strike). [LSJ 20050224-2]
+  - Cannot cancel a card that destroys or steals an equipment or weapon. [LSJ 20050221]
+  - Cannot cancel a card restricting the use of disciplines. [LSJ 20050221]
 100862|Growing Fury:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
+100863|Guard Dogs:
+  - "[ANI] The maneuver can only be used if the block is successful, and only in the resulting (block-induced) combat. It does not carry over to a follow-up combat (eg. [CEL] {Psyche!}). [LSJ 20010813] [LSJ 20010819-2]"
+  - "[ANI] The maneuver is provided again if a second block happens on the same action (eg. after [PRO] {Form of Mist}). [LSJ 20010814-2]"
 100864|Guard Duty:
-  - "Cannot be used to unlock if the vampire cannot attempt to block the action (eg. {Daring the Dawn}). [LSJ 20010714-2]"
-  - "If used to unlock, the block attempt and subsequent combat still happen if the action lacks a suitable target because of the unlock (eg. {Ambush}). [LSJ 20090514]"
+  - Cannot be used to unlock if the vampire cannot attempt to block the action (eg. {Daring the Dawn}). [LSJ 20010714-2]
+  - When used to block, does not ignore the normal prey, predator or target restrictions. [ANK 20180623]
+  - If used to unlock, the block attempt and subsequent combat still happen if the action lacks a suitable target because of the unlock (eg. {Ambush}). [LSJ 20090514]
 100865|Guarded Rubrics:
-  - "The provided action ends with no effect, if the acting minion does not possess the equipment when the action resolves. It is still considered successful if not blocked. [RTR 19960221]"
-100867|Guardian Ghoul:
-  - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
+  - The provided action ends with no effect, if the acting minion does not possess the equipment when the action resolves. It is still considered successful if not blocked. [RTR 19960221]
 100868|Guardian Vigil:
-  - "Must be played before block is successful, but can be played after the acting Methusalah declined to add stealth. [ANK 20180926]"
-  - 'All effects apply for the duration of the action. They still apply if the action "continues as if unblocked". [ANK 20181127]'
-  - "Can be used by a vampire who is already attempting to block. [ANK 20181122-2]"
+  - Must be played before block is successful, but can be played after the acting Methuselah declined to add stealth. [ANK 20180926]
+  - All effects apply for the duration of the action. They still apply if the action "continues as if unblocked" (eg. [PRO] {Form of Mist}) and, if [aus] was used, the maneuver is provided again. [LSJ 20010814-2] [ANK 20181127]
+  - Can be used by a vampire who is already attempting to block. [ANK 20181122-2]
+  - "[aus] The maneuver can only be used if the block is successful, and only in the resulting (block-induced) combat. It does not carry over to a follow-up combat (eg. [CEL] {Psyche!}). [LSJ 20010813] [LSJ 20010819-2]"
 100871|Gurchon Hall:
-  - "You need two ready vampires to gain blood. [PIB 20130221]"
+  - You need two ready vampires to gain blood. [PIB 20130221]
 100872|Guru:
-  - "The blood is gained after the referendum effects are applied. [LSJ 20090115-2]"
+  - The blood is gained after the referendum effects are applied. [LSJ 20090115-2]
+100876|Hackerspace:
+  - A counter is added when {Anarch Convert} enters play, before using his ability. If he uses his ability to make a non-anarch vampire anarch, a second counter is added. [ANK 20210410]
+100878|Hall of Hades' Court:
+  - '[tem] [ACTION MODIFIER][REACTION] Cards are not replaced during the "as played" window. [LSJ 20061013]'
+  - '[tem] [ACTION MODIFIER][REACTION] If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
+100879|Hall of Mirrors:
+  - "[CHI] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {The Path of Paradox}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 100882|Hand of Conrad:
-  - "The minion cannot use the discipline provided if some effect prevents him to use the equipment (eg. {Drawing Out the Beast}). [RTR 20010710]"
+  - The minion cannot use the discipline provided if some effect prevents him to use the equipment (eg. {Drawing Out the Beast}). [RTR 20010710]
 "100884|Haqim's Law: Judgment":
-  - "The provided action is considered as an action that requires an Anarch or an Independant. (eg {CrimethInc.} can be used). [ANK 20180529]"
+  - The provided action is considered as an action that requires an Anarch or an Independant. (eg {CrimethInc.} can be used). [ANK 20180529]
 100886|Harass:
-  - "If the action is not blocked and the target does not meet the requirements anymore, it is successful but has no effect. [LSJ 20070411] [LSJ 20090514]"
+  - If the action is not blocked and the target does not meet the requirements anymore, it is successful but has no effect. [LSJ 20070411] [LSJ 20090514]
 100887|Hard Case:
-  - "The block needs to be successful, so the blocking minion is locked. [ANK 20190708]"
+  - The block needs to be successful, so the blocking minion is locked. [ANK 20190708]
 100892|Hatchling:
-  - "The created vampire is not unique. [LSJ 20100221]"
+  - The created vampire is not unique. [LSJ 20100221]
+100893|Haunt:
+  - "[NEC] The action is directed at the Methuselah controlling the location, undirected if you control it. [RBK 20200701-9] [LSJ 20090324]"
 100896|Haven Hunting:
-  - "Effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]"
-  - "Cannot be used to start a new combat if there is already a pending combat queued. [RTR 20020501]"
+  - Effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]
+  - Cannot be used to start a new combat if there is already a pending combat queued. [RTR 20020501]
 100899|Hay Ride:
-  - "Must be played after combat if the action is blocked [RTR 19980623]"
+  - Must be played after combat if the action is blocked [RTR 19980623]
 100900|Haymaker:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 100901|Healing Touch:
   - "[OBE] Is not the default action, no blood is paid for the rescue. [ANK 20181017]"
 100907|Heaven's Gate:
   - "[nec] Cannot be used if there is no damage to prevent. [LSJ 20001114]"
-"100908|Heidelberg Castle, Germany":
+  - "[obe] / [OBE] Forbids any combat with the ally afterwards. Cards that would start a new combat cannot be played (eg. {Psyche!}, {Bum's Rush}). [ANK 20220429]"
+100908|Heidelberg Castle, Germany:
   - 'May not be locked "in response" to an effect: all effects are instantaneous except for actions and certain combat effects. [LSJ 20010110] [LSJ 20050111]'
-  - "Cannot be used to put a card on a vampire who is prohibited to have it (eg. an equipment on {Enkidu, The Noah}). [LSJ 19980831]"
-  - "Cannot be used before damage is inflicted after action resolution (eg. {Force of will}, {Daring the Dawn}): this is still during the action. [ANK 20171124]"
+  - Cannot be used to put a card on a vampire who is prohibited to have it (eg. an equipment on {Enkidu, The Noah}). [LSJ 19980831]
+  - "Cannot be used before damage is inflicted after action resolution (eg. {Force of Will}, {Daring the Dawn}): this is still during the action. [ANK 20171124]"
   - "Cannot be used after a diablerie or an {Abactor} resolution and before the Blood Hunt: the Blood Hunt is part of the action although it is independant from it. [LSJ 20090722-2] [LSJ 20030618]"
   - "Can be used to move more blood than the target can hold: the excess goes to the blood bank. [ANK 20170804]"
-100911|Hellhound:
-  - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
+  - Can be used between two actions during another Methuselah's turn. [ANK 20210608]
+100910|Hell-for-Leather:
+  - "[cel] A limited additional strike can be played before or after. [LSJ 20001206] [ANK 20211124]"
 100912|Herald of Topheth:
-  - 'Can use {Charming Lobby} to call a referendum "as a vampire". [RTR 20020501]'
-  - "If it uses its last life to pay for an action, the action still resolves fully. If that leads to an oust, the oust is resolved before resolving effects triggered by the fact that the Herald burns. [LSJ 20080512]"
+  - Can use {Charming Lobby} to call a referendum "as a vampire". [RTR 20020501]
+  - If it uses its last life to pay for an action, the action still resolves fully. If that leads to an oust, the oust is resolved before resolving effects triggered by the fact that the Herald burns. [LSJ 20080512]
+100913|Heroic Might:
+  - The strikes it provides are Potence [pot] strikes (eg. they benefit from {Increased Strength}). [LSJ 20081120-2]
 100916|Hidden Lurker:
-  - "Effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]"
-  - "Cannot be used to start a new combat if there is already a pending combat queued. [RTR 20020501]"
-  - "Can only be played by the controller of the acting minion. [LSJ 19990425]"
-  - "Cannot be used to enter combat with a vampire on his way to torpor. [LSJ 20100604-1]"
+  - Effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]
+  - Cannot be used to start a new combat if there is already a pending combat queued. [RTR 20020501]
+  - Can only be played by the controller of the acting minion. [LSJ 19990425]
+  - Cannot be used to enter combat with a vampire on his way to torpor. [LSJ 20100604-1]
 100918|Hidden Strength:
-  - "The 'X' in card text refers to the cost of the card. [LSJ 19970224]"
-  - "Prevents up to X+1 damage, it can prevent less. [RTR 20041202]"
+  - The 'X' in card text refers to the cost of the card. [LSJ 19970224]
+  - Prevents up to X+1 damage, it can prevent less. [RTR 20041202]
   - "[FOR] The press can only be used during the current round. [TOM 19960521]"
 100919|Hide:
   - "[REACTION] Can be used only when reactions can be used (unlocked or with a wake effect). It does not count as playing a reaction card. [LSJ 20070403] [LSJ 20070413]"
   - "[REACTION] Modifiers and reactions that can be used at the end/after an action can still be used afterwards. [LSJ 20041022]"
-  - '[ACTION MODIFIER] [1 CONVICTION] Cards and effects that can be played "as the action is announced" (and only them) can be played before it. [ANK 20190425]'
+  - '[ACTION MODIFIER] [1 CONVICTION] Cards and effects that are played "as the action is announced" must be played before playing "regular" action modifier or reaction cards. [ANK 20190425]'
 100920|Hide the Heart:
   - "[val] If the action fails, modifiers and reactions that can be used at the end/after an action can still be used afterwards. [LSJ 20041022]"
   - "[val] An ally has life, not blood, he cannot pay. [LSJ 20050216] [ANK 20190701]"
-  - "[val], [VAL] If another Methusalah is the target, he must declare whether he attempts or declines to block before Hide the Heart can be played. [LSJ 20100507] [PIB 20150820]"
+  - "[val], [VAL] Sequencing applies. For example, if another Methuselah is targeted by the action, they must declare if they attempt or decline to block before you can play Hide the Heart. [LSJ 20100507] [PIB 20150820] [RBK 20200701-2]"
+100921|Hide the Mind:
+  - Cannot be used to cancel a card that could be played with [aus] but has not been (eg. {Anesthetic Touch} play with [obe]). [PIB 20130704]
+100924|High Aye:
+  - The discard effect happens after action resolution (and all combats, if any). [LSJ 20060426]
 100925|High Ground:
-  - "When setting the range for the round, no other effect can be used to reset the range. Skip the determine range step this round, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]"
+  - When setting the range for the round, no other effect can be used to reset the range. Skip the determine range step this round, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]
 100935|Horrid Reality:
-  - "If no weapon can be found, the cost is still paid. [TOM 19951212-1]"
-  - "If the weapon retrieved has requirements that the vampire does not meet, then it is burned. [RTR 20010710]"
-  - "If a copy of a unique card already in play is retrieved, then the weapon is contested until the end of combat. It becomes uncontested during the next appropriate unlock phase. [TOM 19951212-1]"
-  - "The weapon is burned or returned to the library if it is still in play, even if it is not on the minion anymore (eg. {Rowan Ring}, {Wooden Stake}). [LSJ 20001019]"
+  - If no weapon can be found, the cost is still paid. [TOM 19951212-1]
+  - If the weapon retrieved has requirements that the vampire does not meet, then it is burned. [RTR 20010710]
+  - If a copy of a unique card already in play is retrieved, then the weapon is contested until the end of combat. It becomes uncontested during the next appropriate unlock phase. [TOM 19951212-1]
+  - The weapon is burned or returned to the library if it is still in play, even if it is not on the minion anymore (eg. {Rowan Ring}, {Wooden Stake}). [LSJ 20001019]
+100937|Horseshoes:
+  - If used on an ally and it burns as a result, this counts as a Ⓓ action burning an ally (eg. Trophies, {Predator's Transformation}). [ANK 20220507]
 100938|Hospital Food:
-  - "The action is successful even if no blood is gained. [LSJ 20050720-2]"
+  - The action is successful even if no blood is gained. [LSJ 20050720-2]
 100939|Hostile Takeover:
-  - "The bidding is conducted in an open format, similar to a referendum. The player who played the card conducts the auction. [LSJ 19990104]"
+  - The bidding is conducted in an open format, similar to a referendum. The player who played the card conducts the auction. [LSJ 19990104]
 100944|Hunger Moon:
-  - "A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]"
+  - A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]
 100947|I am Legion:
   - "[DAI][OBF] Can be used to gain a pool after a successful action, without cancelling an [aus] card. [LSJ 20100902-2]"
+  - '[dai][obf], [DAI][OBF] Cards are not replaced during the "as played" window. [LSJ 20061013]'
+  - '[dai][obf], [DAI][OBF] If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
 100948|Ignis Fatuus:
-  - "If another Methusalah is the target, he must declare whether he attempts or declines to block before Ignis Fatuus can be played. [PIB 20150820] [ANK 20200607]"
+  - If another Methuselah is the target, he must declare whether he attempts or declines to block before Ignis Fatuus can be played. [PIB 20150820] [ANK 20200607]
 100949|Ignore the Searing Flames:
   - "[DAI] Immune means damage is not inflicted, even if non-preventable or outside combat. [LSJ 20010627] [LSJ 20010629] [LSJ 20090304-1]"
+  - "[DAI] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {The Textbook Damnation}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 100951|Illegal Search and Seizure:
-  - 'A weapon''s "current damage" is the amount of damage that it would inflict if used as a strike by the bearer against a generic opponent. [RTR 19980623]'
+  - A weapon's "current damage" is the amount of damage that it would inflict if used as a strike by the bearer against a generic opponent. [RTR 19980623]
 100954|Illusions of the Kindred:
-  - "If the combat continues nonetheless, the card has no effect (no crypt card is drawn, no new combat occurs afterwards). [RTR 20020501]"
-  - "Queues a combat. No other combat can be queued afterwards. [LSJ 19971003]"
-  - "Cannot be used if there is already another combat queued. [RTR 20020501]"
-  - "Cannot be played when your crypt is empty. [RTR 20000501]"
-  - "If the illusionary vampire does not enter combat, then he or she is removed from the game at the end of the current action. [LSJ 19991110]"
-  - "If the illusionary vampire is burned in combat, the acting Methuselah chooses whether he is sent to the ash heap or removed from the game. [RTR 20001020]"
-  - "If the illusionary vampire is burned via blood hunt referendum (because it played {Amaranth}) in the combat, it goes to the ash heap and cannot be removed from the game. [PIB 20110810]"
-  - "Even if he has the same name as a vampire in play, the illusonary vampire is considered another vampire for all purposes. [LSJ 20100213]"
-  - "If the card drawn is an imbued, the imbued would briefly come into play, become incapacitated, and then be removed from the game. [LSJ 20060323]"
-  - "If the vampire playing it goes to torpor (eg. {Outside the Hourglass}), the new combat still occurs. [ANK 20180104]"
+  - If the combat continues nonetheless (eg. {Telepathic Tracking}), the card has no effect (no crypt card is drawn, no new combat occurs afterwards). [RTR 20020501]
+  - Queues a combat. No other combat can be queued afterwards (eg. {Psyche!} cannot be used). [LSJ 19971003]
+  - Cannot be used if there is already another combat queued. [RTR 20020501]
+  - Cannot be played when your crypt is empty. [RTR 20000501]
+  - If the illusionary vampire does not enter combat, then he or she is removed from the game at the end of the current action. [LSJ 19991110]
+  - If the illusionary vampire is burned in combat (aggravated damage or blood hunt referendum after an {Amaranth}), it goes to the ash heap and cannot be removed from the game. [PIB 20110810]
+  - Even if he has the same name as a vampire in play, the illusonary vampire is considered another vampire for all purposes (eg. {Jimmy Dunn}'s ability does not trigger). [LSJ 20100213] [LSJ 19991110]
+  - If the illusionary vampire has a title, he can use the votes (eg. in a Blood Hunt referendum) even if there is another instance of the title in play. [LSJ 20030419]
+  - If the card drawn is an imbued, the imbued would briefly come into play, become incapacitated, and then be removed from the game. [LSJ 20060323]
+  - If the vampire playing it goes to torpor (eg. {Outside the Hourglass}), the new combat still occurs. [ANK 20180104]
 100956|Ilomba:
-  - "His effect applies to each point of damage. (eg. if 3 damage is done to him, the minion it is on burns 3). [ANK 20180525]"
-  - "If damage is done simultaneously to Ilomba and its owner, the controller chooses the order of resolution. [LSJ 20090617-2]"
+  - His effect applies to each point of damage. (eg. if 3 damage is done to him, the minion it is on burns 3). [ANK 20180525]
+  - If damage is done simultaneously to Ilomba and its owner, the controller chooses the order of resolution. [LSJ 20090617-2]
+  - If grabbed by a "this vampire employs" effect (not the normal employ action), the vampire receiving Ilomba does not get to move Ilomba on to a new target. [LSJ 20090824] [LSJ 20051121]
 100957|Immaculate Vitae:
-  - "A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]"
+  - A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]
 100959|Immortal Grapple:
-  - "If a minion is committed to using a strike other than a hand strike (e.g. used a maneuver from a gun), then he gets no strike. [TOM 19951217]"
-  - "Is still considered played if it is canceled as it is played (eg. {Charismatic Aura}). A second one cannot be played in the same round as its card text forbids it. [ANK 20200525-2]"
-  - "The press can only be used during the current round. [TOM 19960521]"
+  - If a minion is committed to using a strike other than a hand strike (e.g. used a maneuver from a gun), then he gets no strike. [TOM 19951217]
+  - Is still considered played if it is canceled as it is played (eg. {Charismatic Aura}). A second one cannot be played in the same round as its card text forbids it. [ANK 20200525-2]
+  - The press can only be used during the current round. [TOM 19960521]
+100962|Imposing Phantasm:
+  - The opposing minion get their blood back even if they changed controller. [ANK 20220525]
 100964|Improvised Flamethrower:
-  - "If any ranged damage is inflicted at long range, even if it is prevented or ignored, the Flamethrower will burn and inflict damage. [LSJ 20040802]"
+  - If any ranged damage is inflicted at long range, even if it is prevented or ignored, the Flamethrower will burn and inflict damage. [LSJ 20040802]
 100965|Improvised Tactics:
   - "[pot] Is a strike that requires Potence, so would be enhanced by {Increased Strength}. [LSJ 20030611]"
 100966|Impundulu:
-  - "Can use his action on a vampire with no blood. [RTR 20010711]"
-  - "If he uses his ability to steal blood or life from one of his controller's minions, the action is undirected. [ANK 20180917]"
-"100968|Inbase Discotek, Frankfurt":
-  - "The hunt bonus applies to non-standard hunt actions, it comes from the blood bank not from the target of the hunt [RTR 20030519]"
-  - "A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]"
+  - Can use his action on a vampire with no blood. [RTR 20010711]
+  - If he uses his ability to steal blood or life from one of his controller's minions, the action is undirected. [ANK 20180917]
+100968|Inbase Discotek, Frankfurt:
+  - The hunt bonus applies to non-standard hunt actions, it comes from the blood bank not from the target of the hunt [RTR 20030519]
+  - A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]
 100969|Inceptor:
-  - "The cards can be played using the inferior version of the discipline. [LSJ 20090508]"
-  - "Can be used to meet one (not both) of the Discipline requirements of a multi-Discipline card. [LSJ 20090508]"
+  - The cards can be played using the inferior version of the discipline. [LSJ 20090508]
+  - Can be used to meet one (not both) of the Discipline requirements of a multi-Discipline card. [LSJ 20090508]
 100971|Increased Strength:
-  - "The additional damage is the same type as the strike's damage. [RTR 19970630]"
+  - The additional damage is the same type as the strike's damage. [RTR 19970630]
 100972|Incriminating Videotape:
-  - "If it is stolen, then the chosen minion is unable to block the new possessor of the Videotape (and can now block whoever used to have it). If it is removed from play, its effect ends. [TOM 19960114]"
+  - If it is stolen, then the chosen minion is unable to block the new possessor of the Videotape (and can now block whoever used to have it). If it is removed from play, its effect ends. [TOM 19960114]
 100973|Indomitability:
   - "[FOR] The press can only be used during the current round. [TOM 19960521]"
   - "[for] Cannot be used if there is no damage to prevent. [LSJ 20001114]"
-100974|Inevitability of the Void:
-  - "The cards to remove must be chosen when announcing the action. [LSJ 20100527]"
+100975|Infamous Insurgent:
+  - It does not require an anarch so it cannot be played on vampires that can fake requirements for you (eg. {Mata Hari}). [ANK 20220718]
 100977|Infection:
   - "[THA] Must be played after the presses are handled and can be played if the round ends prematurely. [RTR 20030519]"
 100978|Infernal Familiar:
-  - "Can be used to meet one (not both) of the normal Discipline requirements of a multi-Discipline card. [LSJ 20011217]"
-  - "No counter is added if the vampire uses a game effect other than the Familiar to play a card that requires a Discipline he or she does not have. [RTR 20020501]"
+  - Can be used to meet one (not both) of the normal Discipline requirements of a multi-Discipline card. [LSJ 20011217]
+  - No counter is added if the vampire uses another game effect (eg. {Ian Forestal}, another {Infernal Familiar}) to play a card that requires a Discipline they do not have. [RTR 20020501] [LSJ 20100517]
 100980|Infernal Pursuit:
   - "[CEL] The card you discard need not be one of the cards that you just drew. [TOM 19950924]"
   - "[CEL] If canceled as it is played, its effect is not applied and only one card is drawn as a replacement. [LSJ 20021022]"
   - "[CEL] Once successfully played, if a subsequent combat card played by this minion gets canceled as it is played, an additional card is drawn for replacement. [ANK 20191211]"
   - "[CEL] If multiple cards are replaced, replace and discard one by one. [ANK 20180925-1] [LSJ 20100506]"
   - "[CEL] Effects that make you discard (eg. {Nicomedes}) are subject to Infernal Pursuit. [ANK 20180925-1]"
 100981|Infernal Servitor:
-  - 'The "can act the turn it is recruited" text does not let him act during an opponent turn if it was recruited then (eg. using {Madness Network}). [ANK 20200813-3]'
+  - The "can act the turn it is recruited" text does not let him act during an opponent turn if it was recruited then (eg. using {Madness Network}). [ANK 20200813-3]
 100989|Inscription:
-  - "The vampire receiving the card must meet all of the requirements of the card other than the Thaumaturgy requirement. The vampire playing the Inscription need not meet any of the requirements (other than the Thaumaturgy needed to play Inscription in the first place). [LSJ 20031116]"
-  - 'If the card put on it has any "Do not replace" effect, it is ignored both when Inscription is played and when it is burned to use the card. [ANK 20180627-1]'
+  - The vampire receiving the card must meet all of the requirements of the card other than the Thaumaturgy requirement. The vampire playing the Inscription need not meet any of the requirements (other than the Thaumaturgy needed to play Inscription in the first place). [LSJ 20031116]
+  - If the card put on it has any "Do not replace" effect, it is ignored both when Inscription is played and when it is burned to use the card. [ANK 20180627-1]
   - "When burned, the card put on it is not considered to be played normally: if it is a modifier the minion can still use the same modifier himself. [ANK 20180627-1]"
 100992|Inspire Greatness:
-  - "Can only be played by the controller of the acting minion. [LSJ 19990425]"
-  - "Can be played by a locked vampire. [LSJ 19980210]"
-  - "Multiple copies can be played by different minions on the same action. [ANK 20200515]"
+  - Can only be played by the controller of the acting minion. [LSJ 19990425]
+  - Can be played by a locked vampire. [LSJ 19980210]
+  - Multiple copies can be played by different minions on the same action. [ANK 20200515]
+  - Effects, modifiers and reaction to modify stealth or intercept can be plated afterwards. [ANK 20210926]
 100994|Instantaneous Transformation:
-  - "[FOR][CEL] Can be played if the action is unblocked even if it has no effect due to lack of a suitable target. [LSJ 20070411]"
+  - "[CEL][PRO] Can be played if the action is unblocked even if it has no effect due to lack of a suitable target. [LSJ 20070411]"
+100995|Instinctive Reaction:
+  - "[ANI] The maneuver can only be used if the block is successful, and only in the resulting (block-induced) combat. It does not carry over to a follow-up combat (eg. [CEL] {Psyche!}). [LSJ 20010813] [LSJ 20010819-2]"
+  - "[ANI] The maneuver is provided again if a second block happens on the same action (eg. after [PRO] {Form of Mist}). [LSJ 20010814-2]"
 100998|Internal Recursion:
-  - "Is played before the combat begins. [LSJ 20020204]"
+  - Is played before the combat begins. [LSJ 20020204]
   - "[pre] The blocking vampire do not unlock if the vampire uses another effect to end combat as a strike. [RTR 20020501]"
 101000|Into the Fire:
-  - "Is a change of the actual sect. A temporary effect overriding the sect has precendence. [LSJ 20100811]"
-  - "If the target changes sect to a sect inappropriate for his title, he loses its benefit until his sect is appropriate. He immediately yields the title if it is contested or he receives a new one. [LSJ 20060904]"
-"101002|Inveraray, Scotland":
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
+  - Is a change of the actual sect. A temporary effect overriding the sect has precendence. [LSJ 20100811]
+  - If the target changes sect to a sect inappropriate for his title, he loses its benefit until his sect is appropriate. He immediately yields the title if it is contested or he receives a new one. [LSJ 20060904]
 101005|Invoke Poison Glands:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 101008|Iron Glare:
   - "[pot][pre] Cannot be used during a referendum that is automatically passing. [PIB 20150105] [LSJ 19980107]"
+101009|Iron Heart:
+  - Cannot be used to cancel a card that could be played with [pre] (or [dom]) but has not been (eg. {Virtuosa} play with [mel]). [PIB 20130704]
 101013|Island of Yiaros:
-  - "Provides no additional strength to a Priscus for his ballots. [RTR 19970630]"
+  - Provides no additional strength to a Priscus for his ballots. [RTR 19970630]
 101016|Jack of Both Sides:
-  - 'Requirements must be met but this does not count as an action "requiring" anything. [LSJ 20100303] [ANK 20180817]'
-  - "Does not prevent the acting vampire to play the equipment or retainer directly this turn if he unlocks (not the same action). [ANK 20180817]"
+  - Requirements must be met but this does not count as an action "requiring" anything. [LSJ 20100303] [ANK 20180817]
+  - Does not prevent the acting vampire to play the equipment or retainer directly this turn if he unlocks (not the same action). [ANK 20180817]
 101019|Jake Washington:
-  - "Is not an ally in the ash heap (eg. {Compel the Spirit} cannot be played on him). [LSJ 20020115] [LSJ 20030128]"
-  - 'His "starting life amount" is 1 ({Vagabond Mystic} cannot give hime more life). [LSJ 20030520-2]'
+  - Is not an ally in the ash heap (eg. {Compel the Spirit} cannot be played on him). [LSJ 20071014] [LSJ 20020115] [LSJ 20030128]
+  - His "starting life amount" is 1 ({Vagabond Mystic} cannot give hime more life). [LSJ 20030520-2]
 101020|Jar of Skin Eaters:
-  - "Only requires one clan or the other (Tremere or Tremere antitribu) to be played. [ANK 20190203]"
-  - "Using the Jar action does not force the minion to strike with it if he is blocked. [LSJ 19971215]"
-  - "The provided action ends with no effect if the acting minion does not possess the equipment when the action resolves. It is still considered successful if not blocked. [RTR 19960221]"
+  - Only requires one clan or the other (Tremere or Tremere antitribu) to be played. [ANK 20190203]
+  - Using the Jar action does not force the minion to strike with it if he is blocked. [LSJ 19971215]
+  - The provided action ends with no effect if the acting minion does not possess the equipment when the action resolves. It is still considered successful if not blocked. [RTR 19960221]
   - "{Ghoul Retainer} is not the bearer so he can use the Jar even if it has no counter on it. [ANK 20171003]"
   - 'When used as a strike, it does not burn if combat ends before it resolves (eg. if the opponent uses a "strike: combat ends"). [LSJ 20001127-2] [LSJ 20010806-1] [LSJ 19981006]'
 101021|Jar the Soul:
   - "Does not damage vampires: an empty vampire will simply attempt to burn blood and fail. [TOM 19951212-2]"
-  - "If an ally is targeted, it will only be locked - it will not lose a life even if the superior version is used. [RTR 19971201]"
+  - "[SER] If it burns an ally as a result, this counts as a Ⓓ action burning an ally (eg. Trophies, {Predator's Transformation}). [ANK 20220507]"
 101023|The Jones:
   - "[ser] The press can only be used during the current round. [TOM 19960521]"
+  - '[SER] Cards are not replaced during the "as played" window. [LSJ 20061013]'
+  - '[SER] If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
+101026|Journal of Hrorsh:
+  - Equipping it does not put a counter on it [LSJ 20100207-2]
 "101028|Judgment: Camarilla Segregation":
-  - "If multiple copies of the card are in play, one must pay for each of them (they stack). [ANK 20200703-4]"
-  - "The effect must be applied during the unlock phase, but other effects can be applied before. If an effect applied before burns the last non-Camarilla vampire, no pool is lost. [ANK 20181016]"
+  - If multiple copies of the card are in play, one must pay for each of them (they stack). [ANK 20200703-4]
+  - The effect must be applied during the unlock phase, but other effects can be applied before. If an effect applied before burns the last non-Camarilla vampire, no pool is lost. [ANK 20181016]
 101031|Justicar Retribution:
-  - "Counts the bleed amount that each vampire would have when attempting to bleed his prey. [RTR 19980623]"
+  - Counts the bleed amount that each vampire would have when attempting to bleed his prey. [RTR 19980623]
 101033|Karavalanisha Vrana:
-  - "The provided action ends with no effect if the acting minion does not possess the equipment when the action resolves. It is still considered successful if not blocked. [RTR 19960221]"
+  - The provided action ends with no effect if the acting minion does not possess the equipment when the action resolves. It is still considered successful if not blocked. [RTR 19960221]
 101035|Kaymakli Fragment:
   - "Does not make the vampire Sabbat nor infernal: it merely gives the option to such vampires. [PIB 20150809]"
+  - Coutinuous effects stop tracking cards shuffled back into the crypt. Any previous effect affecting one of the crypt card is voided. [LSJ 20071014]
 101039|Kerrie:
-  - "The damage done from the ranged strike is damage from the weapon, so it can be modified by effects that modify melee weapon damage. [LSJ 20051220]"
+  - The damage done from the ranged strike is damage from the weapon, so it can be modified by effects that modify melee weapon damage. [LSJ 20051220]
 101040|Kevlar Vest:
-  - "Prevents up to 2 damage from gun strikes, it can be used to prevent less. [RTR 20041202]"
-  - "Can be used to prevent the damage from two separated gun strikes doing one damage each. [LSJ 20081210]"
+  - Prevents up to 2 damage from gun strikes, it can be used to prevent less. [RTR 20041202]
+  - Can be used to prevent the damage from two separated gun strikes doing one damage each. [LSJ 20081210]
+101041|Keystone Kine:
+  - "[obf] The ally is chosen at action resolution (not declaration). [LSJ 20080608]"
+  - "[obf] This counts as a Ⓓ action burning the ally (eg. for trophies). [LSJ 20080608]"
+  - "[obf] The cost of an imbued is their starting life (cost to influence). Note this is not a cost to recruit (see {Kindred Segregation}). [ANK 20220528]"
 "101044|The Khabar: Honor":
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 101046|Khazar's Diary (Endless Night):
-  - "The action to put a minion from any ash heap into play is not a directed action, even when targeting another Methusalah's ash heap. [LSJ 20010627] [ANK 20181129]"
-  - "Wraiths minions can act the turn they are put into play. [LSJ 20080426]"
-  - "Minions put into play by the Diary go back to their owner's ash heap when burned. [PIB 20130128-2]"
-"101048|Khobar Towers, Al-Khubar":
-  - "If used on an ally with a cost of X, X pool are gained. The value of X is the one set when the ally was recruited . [ANK 20170716] [RTR 20020501]"
-  - "The effect is ordered as the acting Methusalah wishes during his unlock phase (eg. can be used on {Nocturn} before it burns). [ANK 20170625]"
+  - The action to put a minion from any ash heap into play is not a directed action, even when targeting another Methuselah's ash heap. [LSJ 20010627] [ANK 20181129]
+  - Wraiths minions can act the turn they are put into play. [LSJ 20080426]
+  - Minions put into play by the Diary go back to their owner's ash heap when burned. They do not count has allies burned from play (eg. for {Pressing Flesh}). [PIB 20130128-2] [LSJ 20100325-2]
+101048|Khobar Towers, Al-Khubar:
+  - If used on an ally with a cost of X, X pool are gained. The value of X is the one set when the ally was recruited . [ANK 20170716] [RTR 20020501]
+  - The effect is ordered as the acting Methuselah wishes during his unlock phase (eg. can be used on {Nocturn} before it burns). [ANK 20170625]
 101049|Kindred Coercion:
-  - "Cannot 'change' the votes of vampires who haven't voted yet, but can cancel the votes of vampires who haven't voted yet and change the votes of vampires who have voted. [RTR 19991001]"
+  - "[dom] Can force a vampire who has not voted yet to keep abstaining. [RTR 19991001]"
+  - "[DOM] Playable on an abstaining vampire: it does not force them to vote, but restricts their choice if they do. [RTR 19991001] [LSJ 20030828]"
+101051|Kindred Manipulation:
+  - "Playable on an abstaining vampire: it does not force them to vote, but restricts their choice if they do. [RTR 19991001] [LSJ 20030828]"
 101053|Kindred Segregation:
-  - "Only requires that the pool cost be paid in order to keep the ally. Blood costs, if any, need not be repaid to keep an ally. [RTR 20010710]"
-  - "Can be called even if there are no allies in play. [RTR 20010710]"
-  - "One can decide to burn an ally with no pool cost (not paying zero). [ANK 20190724]"
+  - Only requires the pool cost to be paid in order to keep the ally. Allies with blood costs can be kept by paying 0 pool. [RTR 20010710]
+  - Can be called even if there are no allies in play. [RTR 20010710]
+  - One can decide to burn an ally with no pool cost (not paying zero). [ANK 20190724]
+  - Imbued can be kept by paying 0 pool, as they have a "pool cost to recruit" of zero. [LSJ 20060409]
 101054|Kindred Society Games:
-  - "If a vampire has two copies of Kindred Society Games, each copy exerts its own effect. Unlocking the vampire normally would require a total of 2 blood. If the vampire does not unlock normally, both Games are moved to other vampire(s), although the vampire could burn 1 blood to prevent one of the Games from moving on. [RTR 19951017]"
+  - If a vampire has two copies of Kindred Society Games, each copy exerts its own effect. Unlocking the vampire normally would require a total of 2 blood. If the vampire does not unlock normally, both Games are moved to other vampire(s), although the vampire could burn 1 blood to prevent one of the Games from moving on. [RTR 19951017]
 101056|Kine Resources Contested:
-  - "Cannot allocate 4 points to a single Methusalah, but you can allocate points to yourself. [LSJ 20000622]"
-  - "Can allocate more points than a Methusalah has pool. [LSJ 20020819]"
+  - Cannot allocate 4 points to a single Methuselah, but you can allocate points to yourself. [LSJ 20000622]
+  - Can allocate more points than a Methuselah has pool. [LSJ 20020819]
 101057|King of the Mountain:
   - "[FOR] Damage dealt to the opponent is environmental. [RTR 19970630] [LSJ 19970801]"
 101062|The Kiss of Ra:
-  - "Can be played by an acting vampire in torpor. [LSJ 19970325]"
+  - Can be played by an acting vampire in torpor. [LSJ 19970325]
   - "No reaction or modifier can be played afterwards: the action ends immediately. [RTR 20180719]"
-  - "The action has not reached resolution. The same vampire can undertake the same action again, but not if it was blocked then continued before (eg. [PRO] {Form of Mist}). [LSJ 20070709] [LSJ 20090220] [ANK 20210124]"
-  - "The action was still taken (eg. counts against {Enkil Cog} of [OBF] {Veil the Legion}). [ANK 20210124]"
+  - The action has not reached resolution, it is effectively canceled. The same vampire can undertake the same action again, but not if it was blocked then continued before (eg. [PRO] {Form of Mist}). [ANK 20211015] [ANK 20210124] [LSJ 20090220] [LSJ 20070709]
+  - The action was still taken (eg. counts against {Enkil Cog} of [OBF] {Veil the Legions}). [ANK 20210124]
 101066|Kraken's Kiss:
   - "[VIC] The strike to steal 2 blood can be used on a minion with less than 2 blood or life. [RTR 20010711]"
   - "[VIC] The press can only be used during the current round. [TOM 19960521]"
   - "[VIC] The strike to steal blood is ranged (eg. {The Dracon} steals one more). [PIB 20150603-2]"
 101071|Lam Into:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
   - "[vic] The press can only be used during the current round. [TOM 19960521]"
 101074|Last Stand:
-  - "When an oust occurs, effects (eg. {Perfectionist}) and Action Modifiers (eg. {Freak Drive}) can be played after action resolution, before it ends and the new turn begins. [LSJ 20090731]"
-  - "When an oust occurs, the current minion phase ends (eg. {Tupdog} burns). [LSJ 20090731]"
+  - When an oust occurs, effects (eg. {Perfectionist}) and Action Modifiers (eg. {Freak Drive}) can be played after action resolution, before it ends and the new turn begins. [LSJ 20090731]
+  - When an oust occurs, the current minion phase ends (eg. {Tupdog} burns). [LSJ 20090731]
   - "When an oust occurs, there is no discard phase: the new turns begins immediately (eg. {The Unmasking} is not replaced). [LSJ 20090731]"
+101075|Lay Low:
+  - The anarch can return to play when it again has blood >= capacity on it at the end of its Methuselah's influence phase. [TOM 19951209] [ANK 20210630]
+  - The anarch will remember all effects that had been applied to him, just as contested vampires do. This includes gained or lost titles. [RTR 20000501] [ANK 20210630]
+  - '"for the rest of the game" effects pointing at the anarch from other sources will resume if and when the vampire comes back into play. [TOM 19960210] [ANK 20210630]'
+  - '"breaking any temporary control effects" means the anarch is placed in his last permanent controller''s uncontrolled region. [RTR 20000501] [ANK 20210630]'
+  - If the vampire is permanently controlled by a Methuselah other than his owner, it goes to that Methuselah uncontrolled region and is still controlled by him. It is removed from the game if that Methuselah is ousted and kept in game if his owner is ousted. [ANK 20200408-2] [ANK 20210630]
 101077|Lead Fist:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
+101078|Leadership Vacuum:
+  - The votes include bonus votes from cards or ability (eg. {Eze, The Demon Prince}, {Firebrand}) but not conditional votes (eg. {Sundown}, {Aura of Invincibility}). [ANK 20211009] [LSJ 20040518-2]
+  - Priscus ballots are not taken into account. [ANK 20211009] [LSJ 20041025]
+  - Changing the numbers on counters on the card does not change the X value (eg. {Goth Band}). [ANK 20221024]
 101080|Learjet:
-  - "If a card played by the minion with Learjet has a delayed replacement, the additional card is drawn when the replacement is drawn. [PIB 20110718]"
-  - "The additional replacement is optionnal, you get to see the normal replacement before you decide to draw the additional card. [LSJ 20050224-4]"
+  - If a card played by the minion with Learjet has a delayed replacement, the additional card is drawn when the replacement is drawn. [PIB 20110718]
+  - The additional replacement is optionnal, you get to see the normal replacement before you decide to draw the additional card. [LSJ 20050224-4]
 101083|Leech:
-  - "Can target a vampire with no blood [RTR 20010711]"
-  - "Does not stack with similar effects to provide superior [POT] (eg. {Putrescent Servitude}). [ANK 20180111]"
+  - Can target a vampire with no blood [RTR 20010711]
+  - Does not stack with similar effects to provide superior [POT] (eg. {Putrescent Servitude}). [ANK 20180111]
 101084|Left for Dead:
-  - "Effects to begin a new combat cannot be used on the Left for Dead ally as he is not ready. [LSJ 20020509]"
+  - Effects to begin a new combat cannot be used on the Left for Dead ally as he is not ready. [LSJ 20020509]
 101085|Legacy:
-  - "The burn option can be used if all your unmerged advanced vampires are in torpor. [LSJ 20091203]"
+  - The burn option can be used if all your unmerged advanced vampires are in torpor. [LSJ 20091203]
 101086|Legacy of Caine:
-  - "The vampire must take the action directed at a vampire, even if no vampire has any blood left. [LSJ 19970224]"
-  - "When hunting on a target that has no blood to steal, the hunt action will simply have no effect, stealing zero blood. [LSJ 19970224]"
-  - "The vampire cannot hunt if there are no vampires at all. [LSJ 19970224]"
-  - 'If the vampire with the card "cannot gain blood", then the stolen blood is moved to the blood bank when he hunts. [LSJ 20010809-1]'
-  - "Cannot choose to target a vampire when using another non-standard hunt action (eg. {Abactor}). [LSJ 20090606] [ANK 20190707]"
+  - The vampire must take the action directed at a vampire, even if no vampire has any blood left. [LSJ 19970224]
+  - When hunting on a target that has no blood to steal, the hunt action will simply have no effect, stealing zero blood. [LSJ 19970224]
+  - The vampire cannot hunt if there are no vampires at all. [LSJ 19970224]
+  - If the vampire with the card "cannot gain blood", then the stolen blood is moved to the blood bank when he hunts. [LSJ 20010809-1]
+  - Cannot choose to target a vampire when using another non-standard hunt action (eg. {Abactor}). [LSJ 20090606] [ANK 20190707]
 101087|Legacy of Pander:
-  - "Multiple copies in play give only 1 vote in total to non-titled Panders. [LSJ 20010819] [PIB 20130722]"
+  - Multiple copies in play give only 1 vote in total to non-titled Panders. [LSJ 20010819] [PIB 20130722]
 101088|Legacy of Power:
-  - "May be used if one of your vampires is in combat with an ally. In this case, your vampire goes into torpor and the ally is unaffected. [RTR 19960112]"
-  - "Is played during combat. Combat cards can be played to continue combat or begin a new combat. [ANK 20200109]"
-  - "If the combat continues or a new combat begins (eg. {Psyche!}), the vampires do not go into torpor. [RTR 20020501] [LSJ 20021126]"
+  - May be used if one of your vampires is in combat with an ally. In this case, your vampire goes into torpor and the ally is unaffected. [RTR 19960112]
+  - Is played during combat. Combat cards can be played to continue combat or begin a new combat. [ANK 20200109]
+  - If the combat continues or a new combat begins (eg. {Psyche!}), the vampires do not go into torpor. [RTR 20020501] [LSJ 20021126]
 101090|Legend of the Leopard:
-  - "Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
+  - Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]
 101091|Legendary Vampire:
   - "Cannot be used on a vampire who merged last turn: merging is not entering play. [LSJ 20030519-2]"
 101095|Lesser Boon:
-  - "Effects that depend on the successful block do not see the block as successful. [RTR 20080808]"
+  - Effects that depend on the successful block do not see the block as successful. [RTR 20080808]
+101098|Leverage:
+  - A limited bleed modifier can be played before or after. [LSJ 20100218] [RTR 20180511-2]
 101100|Libertas:
-  - "The additional cost does not apply once the minion has failed to block, so it does not apply to the cost of the action card. [LSJ 20080818]"
+  - The additional cost does not apply once the minion has failed to block, so it does not apply to the cost of the action card. [LSJ 20080818]
 101103|Life Boon:
-  - "If a player is saved more than once by Life Boon, the various Boons reserve a series of victory points, rather than competing with each other for a single victory point. [RTR 19951017]"
-  - "If a player has gone to negative pool, the Life Boon player must give her enough pool to compensate for that. [RTR 19970630]"
-  - "If the target receives half of a victory point, then the Methuselah who played the Boon receives that half. The Boon is not burned until a total of one victory point has been awarded. [RTR 19991206]"
-  - "If the effect ousting the target simultaneously ousts the target's prey (eg. {Kine Resources Contested}), the victory point goes to the Mathusalah who played Life Boon and the target gets 6 pool. [LSJ 20021029]"
+  - If a player is saved more than once by Life Boon, the various Boons reserve a series of victory points, rather than competing with each other for a single victory point. [RTR 19951017]
+  - If a player has gone to negative pool, the Life Boon player must give her enough pool to compensate for that. [RTR 19970630]
+  - If the target receives half of a victory point, then the Methuselah who played the Boon receives that half. The Boon is not burned until a total of one victory point has been awarded. [RTR 19991206]
+  - If the effect ousting the target simultaneously ousts the target's prey (eg. {Kine Resources Contested}), the victory point goes to the Mathusalah who played Life Boon and the target gets 6 pool. [LSJ 20021029]
 101109|Lily Prelude:
-  - "Can allocate more points than a Methusalah has pool. [LSJ 20020819]"
+  - Can allocate more points than a Methuselah has pool. [LSJ 20020819]
 101110|The Line:
-  - "Can be locked when the action is announced or when the cost is paid. [ANK 20170605]"
-  - "Can be used to reduce the cost in blood of a recruit ally (eg. {Shambling Hordes}) or employ retainer action. [ANK 20181007]"
-  - 'Cannot be used by an ally acting "as a vampire". [ANK 20200605]'
+  - Can be locked when the action is announced or when the cost is paid. [ANK 20170605]
+  - Can reduce the cost in blood (not in pool) of any action (ally, retainer, equipment, political). [ANK 20181007]
+  - Cannot be used by an ally acting "as a vampire". [ANK 20200605]
 101112|Liquidation:
-  - "Is not playable if you have less than 7 cards in your library. [LSJ 20070901]"
-101114|Living Manse:
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
-101117|Local 1111:
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
+  - Is not playable if you have less than 7 cards in your library. [LSJ 20070901]
 101118|Lock:
-  - "Once in play, applies to an action if any one of its targets would be enough to enable his effect. [LSJ 20080809-2] [KOT 20081119]"
+  - Once in play, applies to an action if any one of its targets would be enough to enable his effect. [LSJ 20080809-2] [KOT 20081119]
+101119|Loki's Gift:
+  - "[PRO] The blood burned is not affected by effects modifying the hunt amount (eg. {Ariadne}). [ANK 20220809]"
 101121|Loner:
-  - "Only considers the minions controlled during the influence phase. It does not care if minions you no longer control acted this turn. [LSJ 20060616-1]"
+  - Only considers the minions controlled during the influence phase. It does not care if minions you no longer control acted this turn. [LSJ 20060616-1]
 101123|Lord of Serenity:
   - "[for] Is not the default action, no blood is paid for the rescue. [ANK 20181017]"
+101124|Loss:
+  - "[qui] Is directed against the Methuselah controlling the equipment or location, not the minion it's on. [LSJ 20090324]"
 101126|Lost in Translation:
-  - 'Must be played before action resolution, ie. before any modifier or reaction played "as the action/bleed would be successful" are played. It cannot be played after a {Spying Mission} on the vampire triggers. [LSJ 19980105]'
+  - Must be played before action resolution, ie. before any modifier or reaction played "as the action/bleed would be successful" are played. It cannot be played after a {Spying Mission} on the vampire triggers. [LSJ 19980105]
+  - "Can be played when failing to block because of stealth: it is still declining to block. [ANK 20211003]"
 101128|Loving Agony:
   - "[ani] Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
   - "[val] [VAL] Damage is done by the vampire (not environmental). [RTR 19970630] [LSJ 19990723]"
   - "[val] [VAL] If the combat continues or a new combat begins, no damage is done. The vampire can still burn 1 blood to unlock. [RTR 20020501]"
   - "[val] [VAL] If the strike is dodged, no damage is done. [LSJ 19980526] [RTR 20041202] [PIB 20130319]"
   - "[val] [VAL] Is a damage dealing strike and can be modified by effects like {Target Vitals} or {Dam the Heart's River}. [PIB 20130319]"
   - "[VAL] The blood to unlock can be paid until the end of combat, including after other effects that are played at the end of round. [ANK 20180618]"
 101130|Loyalist:
-  - "If the Loyalist vampire's votes are changed to be in favor, the votes granted by Loyalist are silenced (not cast). [LSJ 20031115]"
+  - If the Loyalist vampire's votes are changed to be in favor, the votes granted by Loyalist are silenced (not cast). [LSJ 20031115]
 101131|Lucky Blow:
-  - "Adding damage to strikes which are not damage dealing strikes will not deal damage [RTR 19960221]"
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
-  - "You cannot use another strike card as the hand strike for Lucky Blow. [LSJ 20010627]"
+  - Adding damage to strikes which are not damage dealing strikes will not deal damage [RTR 19960221]
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
+  - You cannot use another strike card as the hand strike for Lucky Blow. [LSJ 20010627]
 101132|Lunatic Eruption:
-  - "The mandatory attack action must be taken before any non-mandatory actions. [LSJ 20001127]"
-  - "If the minion it is on has entered combat and unlocks, he is free to take any other action. [ANK 20200227]"
+  - The mandatory attack action must be taken before any non-mandatory actions. [LSJ 20001127]
+  - If the minion it is on has entered combat and unlocks, he is free to take any other action. [LSJ 20090226] [ANK 20200227]
+  - If a minion has two of those, he is stuck and cannot act. [LSJ 20041103]
+  - The action to burn it is directed at the Methuselah who controls the minion it is on. It is undirected if it is yourself. [LSJ 20010328]
 101134|Lure of the Serpent:
-  - "Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
-"101135|Lyndhurst Estate, New York":
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
+  - Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]
 101136|Maabara:
-  - "All other players can see which card is selected from the ash heap. [ANK 20200523]"
+  - All other players can see which card is selected from the ash heap. [ANK 20200523]
 101137|Machine Blitz:
-  - 'A weapon''s "current damage" is the amount of damage that it would inflict if used as a strike by the bearer against a generic opponent at the appropriate range. [RTR 19980623]'
-  - 'The "current damage" amount is set when Machine Blitz is announced. [LSJ 19970224]'
+  - A weapon's "current damage" is the amount of damage that it would inflict if used as a strike by the bearer against a generic opponent at the appropriate range. [RTR 19980623]
+  - The "current damage" amount is set when Machine Blitz is announced. [LSJ 19970224]
   - "Does not count as using the weapon: no restriction nor side-effect apply (eg. {Bomb} is not burned, {Sawed-Off Shotgun} can be used multiple times). [LSJ 20010806-1]"
-  - "Does not inflict aggravated damage if the target weapon does. [LSJ 20010806-1]"
+  - Does not inflict aggravated damage if the target weapon does. [LSJ 20010806-1]
 101139|Madness Network:
-  - "Malkavians do not have to be ready to take an action via the Network. (i.e. a Torpored Malk could rescue himself from Torpor) [RTR 19950509]"
-  - "A non-Malkavian cannot use {Mask of a Thousand Faces} to assume the action of a Malkavian on someone else's turn. [LSJ 19981007]"
-  - "If a Malkavian has no blood, he may declare an action during another Methuselah's turn but, if he does, that action must be a hunt action. [LSJ 20060508]"
-  - "Any locked Malkavian on the table can use a wake effect to attempt to block the action to burn the Madness Network. [LSJ 20041022-2]."
+  - Malkavians do not have to be ready to take an action via the Network. (i.e. a Torpored Malk could rescue himself from Torpor) [RTR 19950509]
+  - A non-Malkavian cannot use {Mask of a Thousand Faces} to assume the action of a Malkavian on someone else's turn. [LSJ 19981007]
+  - If a Malkavian has no blood, he may declare an action during another Methuselah's turn but, if he does, that action must be a hunt action. [LSJ 20060508]
+  - Any locked Malkavian on the table can use a wake effect to attempt to block the action to burn the Madness Network. [LSJ 20041022-2].
 101141|Madrigal:
   - "[MEL] Will have no effect if the vampire who played it abstains, even if he is forced to abstain. The effect operates on the final disposition of the vampire's votes at the time the votes are tallied. [LSJ 20020123]"
   - "[MEL] When used as an action modifier, the acting vampire gains one blood if he does not abstain, as he can only vote in agreement with himself. [LSJ 20020123]"
 101143|Magic of the Smith:
-  - "This is an equip action. [TOM 19960130]"
-  - "You do not search your library until the action is successful. [TOM 19951107]"
-  - "The equipment need not be declared, it is chosen upon resolution. [PIB 20150315]"
+  - This is an equip action. [TOM 19960130]
+  - You do not search your library until the action is successful. [TOM 19951107]
+  - The equipment need not be declared, it is chosen upon resolution. [PIB 20150315]
+  - Can fetch an equipment that is a location when in play. [LSJ 19971001-2]
 101144|Majesty:
   - "[PRE] The vampire still unlocks if an effect continues the combat or begins a new combat. [RTR 20020501]"
 101145|Major Boon:
-  - 'Only modifiers and reactions that can be played "when the action/bleed would be successful" can be played after Major Boon is played or burned. [LSJ 20090205]'
-  - "Cannot be played in succession. The loss from the play of a Major Boon is due to a card effect, not a bleed. So a second cannot be played to Boon the first. [RTR 19960530]"
-  - 'Multiple Major Boons in play cannot be burned on the same bleed action - after the first is burned, "you" are no longer the Methuselah burning pool. [LSJ 19990218]'
+  - Only modifiers and reactions that can be played "when the action/bleed would be successful" can be played after Major Boon is played or burned. [LSJ 20090205]
+  - Cannot be played in succession. The loss from the play of a Major Boon is due to a card effect, not a bleed. So a second cannot be played to Boon the first. [RTR 19960530]
+  - Multiple Major Boons in play cannot be burned on the same bleed action - after the first is burned, "you" are no longer the Methuselah burning pool. [LSJ 19990218]
 101146|Make an Example:
-  - "The action ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20200207]"
-  - "Can be used by a locked vampire. [PIB 20150720] [RTR 19941109]"
-  - "Cannot be used by a vampire in torpor. [PIB 20150720] [RTR 19970306]"
+  - The action ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20200207]
+  - Can be used by a locked vampire. [PIB 20150720] [RTR 19941109]
+  - Cannot be used by a vampire in torpor. [PIB 20150720] [RTR 19970306]
 101147|Make the Misere:
-  - "If the target unlocks and the action is not blocked, it is successful but has no effect. [LSJ 20070411] [LSJ 20090514]"
+  - If the target unlocks and the action is not blocked, it is successful but has no effect. [LSJ 20070411] [LSJ 20090514]
 101150|Malkavian Dementia:
-  - "Does not require control of a ready Malkavian. [RTR 19951124]"
-  - "The loss of control happens at the start of unlock phase, before unlocking. This can not be ordered among other unlock effects, the Malkavian is not unlocked. [ANK 20200129] [LSJ 20091208] [RTR 19951017]"
+  - Does not require control of a ready Malkavian. [RTR 19951124]
+  - The loss of control happens at the start of unlock phase, before unlocking. This can not be ordered among other unlock effects, the Malkavian is not unlocked. [ANK 20200129] [LSJ 20091208] [RTR 19951017]
 "101151|Malkavian Derangement: Alternate Personality":
-  - "Modifier and reactions that can be used at the end/after an action can still be used after the action fails. [LSJ 20041022]"
+  - Modifier and reactions that can be used at the end/after an action can still be used after the action fails. [LSJ 20041022]
 101156|Malkavian Rider Clause:
-  - 'During the referendum that passes automatically, no "during a political action" and "during a referendum" effect can be played and effects that operate on the number of votes that the referendum passed by have no effect. [LSJ 19980107]'
+  - During the referendum that passes automatically, no "during a political action" and "during a referendum" effect can be played and effects that operate on the number of votes that the referendum passed by have no effect. [LSJ 19980107]
 101158|Malkavian Time Auction:
-  - "Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
+  - Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]
+  - Bidding continues until noone wants to bid. You do not participate in the bid. [LSJ 20030604]
+  - If an equipment, retainer or location on a minion changes controller, the new controller chooses a new target they control for them. [LSJ 20030606]
 101159|Malleable Visage:
-  - 'Does not change the acting minion (for purposes of the "No Repeat Actions" rule, among other things) and may be played by a minion who is not capable of taking the action. [LSJ 20011023] [RTR 20020501]'
-  - "Requires a ready, unlocked vampire. [RTR 20010710]"
+  - Does not change the acting minion (for purposes of the "No Repeat Actions" rule, among other things) and may be played by a minion who is not capable of taking the action. [LSJ 20011023] [RTR 20020501]
+  - Requires a ready, unlocked vampire. [RTR 20010710]
 101160|Manstopper Rounds:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
-101164|Marijava Ghoul:
-  - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
-101165|Marijava Thuggee:
-  - "Is not mortal, is a monster. [ANK 20200203-2] [LSJ 20060515]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 101169|Marked Path:
-  - "Can be burned during an action that targets only part of the Methusalah that were targeted by the first action. [LSJ 20100527]"
+  - Can be burned during an action that targets only part of the Methuselah that were targeted by the first action. [LSJ 20100527]
+101174|Martinelli's Ring:
+  - The bearer cannot use [ser] or [dem] cards on themselves (eg. {Mummify}). [LSJ 20080212]
 101175|Martyr's Resilience:
-  - "Can be used by a vampire in torpor. [LSJ 20020416]"
-  - "Can be played by a minion of a Methusalah not involved in the current combat. [ANK 20181101]"
-  - "Cannot be used if there is no damage to prevent. [LSJ 20001114]"
+  - Can be used by a vampire in torpor. [LSJ 20020416]
+  - Can be played by a minion of a Methuselah not involved in the current combat. [ANK 20181101]
+  - Cannot be used if there is no damage to prevent. [LSJ 20001114]
   - "[AUS][FOR] Prevents up to X+1 damage, it can prevent less. [RTR 20041202]"
   - "[AUS][FOR] Unused prevention does not carry over. [LSJ 20001114]"
+  - "[AUS][FOR] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Una}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
+101178|Mask Empathy:
+  - "[PRE] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Adana de Sforza}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 101179|Mask of a Thousand Faces:
-  - "Can only be played by the controller of the acting minion. [LSJ 19990425]"
-  - "Cannot be used to take over an action granted by an equipment the masked minion has, even if the masking vampire also has the same equipment. [LSJ 20020926]"
-  - "The action remains the same. All action modifiers remain in effect, but inherent modifiers (a minion's inherent +1 bleed for example) do not. Other effects applied to the action also carry over to the new masking vampire. [RTR 19951110] [LSJ 19971201] [RTR 20030519] [LSJ 20030521]"
-  - "Cannot be used to mask an action if the masking vampire is not capable of taking that action, nor if any effect (modifier, reaction, {Aching Beauty}, inherent stealth), has been played on this action that could not have been played if the masking minion were the acting minion (not counting blood spent). [RTR 19980623] [RTR 20030519] [LSJ 20030520] [RTR 20041202]"
-  - "Can be used after the action is blocked and before the block resolution (eg. {Venenation} can be played both before and after). [LSJ 20010803]"
-  - "Can be used after blocks are declined if the masked minion was benefiting from an effect that made him unblockable, even if the masking minion does not benefit from the same effect (eg. {Toreador Grand Ball}, {Nakhthorheb}). [PIB 20150924-1] [PIB 20150930]"
-  - "Cannot be used to take over an action requiring a locked minion like {Force of Will}, since Mask requires an unlocked vampire. [LSJ 20020927]"
-  - "Cannot be used during the resolution of an action, like during a referendum or during combat. [LSJ 19980825]"
-  - "A minion attempting to block before is still attempting to block after. [LSJ 19990106]"
-  - "The masking vampire can play a modifier already played by the masked minion. He cannot use a limited effect (ie. bleed enhancer) if a limited effect has already been used on the action. [ANK 20190117-1]"
-  - "Multiple copies can be played by different vampires on the same action. [ANK 20200515]"
+  - Can only be played by the controller of the acting minion. [LSJ 19990425]
+  - Cannot be used to take over an action granted by an equipment the masked minion has, even if the masking vampire also has the same equipment. [LSJ 20020926]
+  - The action remains the same. All action modifiers remain in effect, but inherent modifiers (a minion's inherent +1 bleed for example) do not. All other effects carry over to the new masking vampire. [RTR 19951110] [LSJ 19971201] [RTR 20030519] [LSJ 20030521] [ANK 20210309]
+  - Cannot be used to mask an action if the masking vampire is not capable of taking that action, nor if any effect (modifier, reaction, {Aching Beauty}, inherent stealth), has been played on this action that could not have been played if the masking minion were the acting minion (not counting blood spent). [RTR 19980623] [RTR 20030519] [LSJ 20030520] [RTR 20041202]
+  - Can be used after the action is blocked and before the block resolution (eg. {Venenation} can be played both before and after). [LSJ 20010803]
+  - Can be used after blocks are declined if the masked minion was benefiting from an effect that made him unblockable, even if the masking minion does not benefit from the same effect (eg. {Toreador Grand Ball}, {Nakhthorheb}). [PIB 20150924-1] [PIB 20150930]
+  - Cannot be used to take over an action requiring a locked minion like {Force of Will}, since Mask requires an unlocked vampire. [LSJ 20020927]
+  - Cannot be used during the resolution of an action, like during a referendum or during combat. [LSJ 19980825]
+  - A minion attempting to block before is still attempting to block after. [LSJ 19990106]
+  - The masking vampire can play a modifier already played by the masked minion. He cannot use a limited effect (ie. bleed enhancer) if a limited effect has already been used on the action. [ANK 20190117-1]
+  - Multiple copies can be played by different vampires on the same action. [ANK 20200515]
+  - "[OBF] Cannot be used if no stealth is needed yet. [LSJ 20060409]"
 101180|Masochism:
   - "[FOR] The additional counter is added after the presses are handled. It is added if the round ends prematurely and conditions are met. [RTR 20030519]"
 101181|Masque of Judas:
   - "[aus][obf] The press can only be used during the current round. [TOM 19960521]"
 101183|Masquerade Endangered:
-  - "Multiple copies may be played by different Methusalahs after a single action, but all would be burned during the vampire's next unlock phase. [TOM 19950921]"
-  - "A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]"
+  - Multiple copies may be played by different Methuselahs after a single action, but all would be burned during the vampire's next unlock phase. [TOM 19950921]
+  - A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]
 101184|Masquerade Enforcement:
-  - "Does not affect merging (base with advanced vampire cards). [LSJ 20030527]"
+  - Does not affect merging (base with advanced vampire cards). [LSJ 20030527]
 101185|Mass Reality:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
-  - "Multiple copies stack their bonuses. [LSJ 20020904]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
+  - Multiple copies stack their bonuses. [LSJ 20020904]
 101192|The Meddling of Semsith:
-  - "Will stay in play (uselessly) when the target is burned. [LSJ 20021008]"
-  - "Cards that are not replaced count against the hand size (eg. successive combats against {Raptor} stack the non-replaced cards). [ANK 20180318]"
+  - Stays in play and still reduces your handsize when the target is ousted. [LSJ 20021008]
+  - Is removed from play and its effect cancelled if the Methuselah who played it is ousted. [LSJ 20021008]
+  - Cards that are not replaced count against the hand size (eg. successive combats against {Raptor} stack the non-replaced cards). [ANK 20180318]
 101195|Melange:
-  - "Can be put on an ally. [RTR 20020501]"
-  - "Must be burned when attempting a bleed, before its resolution (eg. {Archon Investigation} can be played afterwards). [ANK 20180531]"
+  - Once in play, must be burned when attempting a bleed, before its resolution (eg. {Archon Investigation} can be played afterwards). [ANK 20180531]
+  - Goes to the ash heap when played, if it has been removed when the vampire blocks, it has no effect. [ANK 20220805]
 101196|Meld with the Land:
   - "[vic] The unlock effect occurs when the strike resolves, before the combat ends. [RTR 19970630] [RTR 20020501]"
   - "[vic] The opponent still unlocks if an effect continues the combat or begins a new combat. [RTR 20020501] [LSJ 20030717]"
 101200|Memory's Fading Glimpse:
-  - "Any cards on the target minion are burned. [SFC 19960919]"
+  - Any cards on the target minion are burned. [SFC 19960919]
 101201|Mental Maze:
-  - "The action ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20200207]"
-  - "Can be played if the requirement was met at the time of block, even if an older slave replaced the acting vampire since. [ANK 20171212]"
+  - The action ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20200207]
+  - Can be played if the requirement was met at the time of block, even if an older slave replaced the acting vampire since. [ANK 20171212]
 101204|Mercy for the Weak:
-  - "The blood gain takes place after the end of combat. [RTR 19970630]"
-  - "The blood is not gained if an effect continues the combat or begins a new combat. [RTR 20020501]"
+  - The blood gain takes place after the end of combat. [RTR 19970630]
+  - The blood is not gained if an effect continues the combat or begins a new combat. [RTR 20020501]
 101205|Mesmerize:
-  - "Cannot be used if there is no equipment to steal. [RTR 19980928]"
+  - Cannot be used if there is no equipment to steal. [RTR 19980928]
 101209|Mighty Grapple:
   - "[POT] Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
   - "[POT] The optional press can only be used during the current round. [TOM 19960521]"
+101210|Millicent Smith, Puritan Vampire Hunter:
+  - If an action is blocked, no other effect can be used (eg. {Crypt's Sons}) before resolving Millicent's delayed effect. However, effects that trigger at the same moment (eg. {Unleash Hell's Fury}) are still applied and ordered by the acting Methuselah. [ANK 20210627] [ANK 20211207] [ANK 20220116]
 101211|Mind Numb:
-  - "The action has no effect if the target is not unlocked anymore when it resolves. It is still considered successful and must be paid. [ANK 20181121]"
+  - The action has no effect if the target is not unlocked anymore when it resolves. It is still considered successful and must be paid. [ANK 20181121]
 101214|Mind of the Wilds:
   - "The blocking minion is prohibited to strike: combat ends for the duration of the action (during any round of any combat). [LSJ 20100308]"
 101215|Mind Rape:
   - "[DOM] Can be played on a locked vampire. [PIB 20150412]"
   - "[DOM] Can be burned to take control of the target at any point during the appropriate minion phase. It does not have to be done before non-mandatory actions. [LSJ 20001201]"
-  - "[DOM] Is removed if its controller (the Methusalah who played it) is ousted (rulings before 2008-11-19 have been reversed). [ANK 20181110]"
-  - "[DOM] The stolen minion is removed from the game when he should return to a Methusalah who has been ousted. [ANK 20181110]"
+  - "[DOM] Is removed if its controller (the Methuselah who played it) is ousted (rulings before 2008-11-19 have been reversed). [ANK 20181110]"
+  - "[DOM] The stolen minion is removed from the game when he should return to a Methuselah who has been ousted. [ANK 20181110]"
   - "[DOM] The stolen minion returns to his previous controller even if he is in torpor (but stays in torpor). [LSJ 20010119]"
 101217|Minion Tap:
-  - "Pay the cost (if any, eg. {Secure Haven} or {Villein} on the target) at the same time you gain pool from it, you do not get ousted in between. [LSJ 20020620]"
-  - "If the target has less blood at resolution than the amount annouced, you take what you can. [LSJ 20100216]"
+  - Pay the cost (if any, eg. {Secure Haven} or {Villein} on the target) at the same time you gain pool from it, you do not get ousted in between. [LSJ 20020620]
+  - If the target has less blood at resolution than the amount annouced, you take what you can. [LSJ 20100216]
 101218|Ministry:
-  - "The additional intercept is gained or lost if the acting vampire changes sect during the action (eg. with {The Red Question} or {Mask of a Thousand Faces}). [ANK 20190416]"
+  - The additional intercept is gained or lost if the acting vampire changes sect during the action (eg. with {The Red Question} or {Mask of a Thousand Faces}). [ANK 20190416]
 101219|Minor Boon:
-  - "A bleed from this vampire cannot be redirected to you either. [PIB 20130711]"
+  - A bleed from this vampire cannot be redirected to you either. [PIB 20130711]
 101220|Minor Curse:
-  - "The burn option can be used if all your vampires with [mal] are in torpor. [LSJ 20091203]"
+  - The burn option can be used if all your vampires with [mal] are in torpor. [LSJ 20091203]
 101222|Mirror Image:
   - '[CHI] If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]'
-  - '[CHI] If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
+  - '[CHI] If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
   - '[CHI] An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]'
   - '[CHI] "continue as if unblocked" moves the action card from the ash heap (where it went when the action was blocked) to limbo (where it should be if the action is not blocked). If the action card is not in the ash heap, then the action cannot be continued. [LSJ 20070808-1]'
   - '[CHI] If the combat continues or a new combat begins, the "action continues as if unblocked" effect is lost. [LSJ 19980109] [RTR 20020501]'
 101223|Mirror Walk:
   - "[THA] The would be blocker is locked even if he benefits from an effect that prevents him to lock when he blocks. He is not locked from the block, but from Mirror Walk's effect. [ANK 20191204]"
-  - "[THA] If the action is blocked, it ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20200207]"
+  - "[THA] If the action is blocked, it ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards (eg. {Freak Drive}, slave rule, {Sowing Dissension}). [RTR 20180719] [ANK 20200207] [ANK 20210627]"
+  - "[THA] If the action is blocked, no other effect can be used (eg. {Crypt's Sons}, {Promise of 1528}) before resolving Mirror Walk delayed effect. However, effects that trigger at the same moment (eg. {Banshee Ironwail}) are still applied and ordered by the acting Methuselah. [ANK 20210627] [ANK 20211207] [ANK 20220116]"
 101224|Mirror's Visage:
   - "[chi] The action ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20200207]"
 101227|Mistaken Identity:
   - "No reaction or modifier can be played afterwards: the action ends immediately. [RTR 20180719]"
 101230|Mob Rule:
-  - "Each Methuselah must decide how much blood to burn for it during the resolution. It does not give an ability for the rest of the political action. However, there can be some give and take during the resolution. For example, Methuselahs can choose to burn one blood at a time and wait to see what the others do. [LSJ 20030602]"
+  - Each Methuselah must decide how much blood to burn for it during the resolution. It does not give an ability for the rest of the political action. However, there can be some give and take during the resolution. For example, Methuselahs can choose to burn one blood at a time and wait to see what the others do. [LSJ 20030602]
+101232|Mokolé Blood:
+  - If there is another copy in play, the cards are put on it before it enters contest. [ANK 20221028] [LSJ 20090428-1]
 101233|The Mole:
   - "[ani] Can be used by a vampire who is already attempting to block. [ANK 20181122-2]"
+101234|Mole's Tunneling:
+  - "[SPI] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {The Path of Harmony}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 101235|Molotov Cocktail:
   - "If the opponent strikes: combat ends, this strike is not resolved and the Cocktail is not put on this minion, even if combat continues thanks to another effect like {Relentless Reaper}. [ANK 20200203-1]"
 101236|Momentary Delay:
-  - 'If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]'
-  - 'If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
-  - 'An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]'
+  - If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]
+  - If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]
+  - An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]
   - '"continue as if unblocked" moves the action card from the ash heap (where it went when the action was blocked) to limbo (where it should be if the action is not blocked). If the action card is not in the ash heap, then the action cannot be continued. [LSJ 20070808-1]'
-  - "Can be used if a Slave locked to enter combat instead of the blocking minion, if the other conditions are met. [ANK 20200114]"
-  - 'Is played after resolution, but still during the action. Cards and effects that played "after resolution" (eg. {Freak Drive}) can be played before it, but not after. [LSJ 19981028] [LSJ 20100206-2]'
+  - Can be used if a Slave locked to enter combat instead of the blocking minion, if the other conditions are met. [ANK 20200114]
+  - Is played after resolution, but still during the action. Cards and effects that played "after resolution" (eg. {Freak Drive}) can be played before it, but not after. [LSJ 19981028] [LSJ 20100206-2]
 101241|Monomancy:
-  - "The card is not put on the target vampire if he or she uses another effect than Monomancy to end combat. [RTR 20020501]"
+  - The card is not put on the target vampire if he or she uses another effect than Monomancy to end combat. [RTR 20020501]
 101244|Morphean Blow:
   - "[val] If the combat continues or a new combat begins, the card is not put on the opposing minion, he can act and block. [RTR 20020501]"
+  - "[val] If the strike is dodged, the card is not put on the opposing minion. [RTR 20041202]"
   - '[VAL] If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]'
-  - '[VAL] If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
+  - '[VAL] If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
   - '[VAL] An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]'
   - '[VAL] "continue as if unblocked" moves the action card from the ash heap (where it went when the action was blocked) to limbo (where it should be if the action is not blocked). If the action card is not in the ash heap, then the action cannot be continued. [LSJ 20070808-1]'
-  - '[VAL] If the combat continues or a new combat begins, the \"action continues as if unblocked\" effect is lost. [LSJ 19980109] [RTR 20020501]'
+  - '[VAL] If the combat continues or a new combat begins, the "action continues as if unblocked" effect is lost. [LSJ 19980109] [RTR 20020501]'
 101245|Mouthpiece:
   - "[DOM] Can only be played by the controller of the acting minion. [LSJ 19990425]"
   - "[DOM] Can be played by a locked vampire. [LSJ 19980210]"
   - "[DOM] Multiple copies can be played by different minions on the same action. [ANK 20200515]"
   - "[DOM] Cannot be used to let the target play a [dom] action card. [LSJ 20100527]"
 101251|Mummify:
-  - "The unlock effect takes place before the end of combat. The rest of the effect takes place after the end of combat. [RTR 19970630]"
-  - "If combat continues or a new combat begins, the vampire unlocks but does not go to torpor. [RTR 20020501] [LSJ 20020505]"
+  - The unlock effect takes place before the end of combat. The rest of the effect takes place after the end of combat. [RTR 19970630]
+  - If combat continues or a new combat begins, the vampire unlocks but does not go to torpor. [RTR 20020501] [LSJ 20020505]
 101254|Murder of Crows:
-  - "Are neither mortal nor monster. [ANK 20200203-2] [LSJ 20060515]"
+  - Are neither mortal nor monster. [ANK 20200203-2] [LSJ 20060515]
 101255|Muricia's Call:
-  - "Requirements must be met to employ the retainer. [LSJ 20100303]"
-  - "Does not prevent the acting vampire to play the equipment directly this turn if he unlocks (not the same action). [ANK 20180817]"
+  - Requirements must be met to employ the retainer. [LSJ 20100303]
+  - Does not prevent the acting vampire to play the equipment directly this turn if he unlocks (not the same action). [ANK 20180817]
 101258|Mustajib:
-  - "The target vampire is not Black Hand if he is not Sabbat. [LSJ 20070322]"
+  - The target vampire is not Black Hand if he is not Sabbat. [LSJ 20070322]
 101259|My Enemy's Enemy:
   - '[AUS] Must be played before action resolution, ie. before any modifier or reaction played "as the action/bleed would be successful" are played. It cannot be played after a {Spying Mission} on the vampire triggers. [LSJ 19980105]'
   - "[AUS] Can be played if there is only two players in the game. The target of the bleed is unchanged, there is no new block opportunity. [LSJ 20060525]"
+  - "[AUS] Can be played when failing to block because of stealth: it is still declining to block. [ANK 20211003]"
+101261|Mylan Horseed:
+  - His action to unlock is undirected if the target is a vampire controlled by it's controller, directed otherwise. [PIB 20121028]
 101263|The Name Forgotten:
-  - "Each Methuselah must find as many copies of the vampire as possible when searching. [LSJ 20050611]"
+  - Each Methuselah must find as many copies of the vampire as possible when searching. [LSJ 20050611]
+101264|Nar-Sheptha:
+  - If burned in combat, her effect ceases immediately and the acting minion returns to normal for the rest of the combat. [ANK 20211022]
+  - Supersedes previous effects that changed the acting minion for the combat (eg. {Deep Song}). [ANK 20211022]
 101268|Necrosis:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
   - "[THN] If the strike is dodged, environmental damage is not applied. [ANK 20200517]"
   - "[THN] The environmental damage is not strike damage (eg. {Target Vitals} does not add to the environmental damage). [ANK 20201228-2]"
 101269|Neebi:
-  - "When setting the range for the round, no other effect can be used to reset the range, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]"
+  - When setting the range for the round, no other effect can be used to reset the range, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]
 101272|Nephandus:
-  - "His life total can exceed his starting life capacity (it is the case for all allies). [ANK 20171109]"
-  - "Damage reduction applies to damage done outside of or after combat if it comes from a strike (eg. {Catatonic Fear}). [LSJ 20080630] [ANK 20170111]"
-  - "Damage reduction does not apply to environmental damage (eg. {Carrion Crows}). [PIB 20111017] [LSJ 20010626]"
-  - "Damage reduction applies to unpreventable damage. [LSJ 20100519]"
-  - "Additional damage provided by Aim cards are not reduced separately. [LSJ 20091123-2]"
-  - "Damage done by a weapon is reduced if it is wielded by the opposing minion. [LSJ 20091123-2]"
+  - His life total can exceed his starting life capacity (it is the case for all allies). [ANK 20171109]
+  - Damage reduction applies to damage done outside of or after combat if it comes from a strike (eg. {Catatonic Fear}). [LSJ 20080630] [ANK 20170111]
+  - Damage reduction does not apply to environmental damage (eg. {Carrion Crows}). [PIB 20111017] [LSJ 20010626]
+  - Damage reduction applies to unpreventable damage. [LSJ 20100519]
+  - Additional damage provided by Aim cards are not reduced separately. [LSJ 20091123-2]
+  - Damage done by a weapon is reduced if it is wielded by the opposing minion. [LSJ 20091123-2]
 101275|Netwar:
-  - "[aus] If another Methusalah is the target, he must declare whether he attempts or declines to block before Netwar can be played. [LSJ 20100507] [ANK 20210131-1]"
+  - "[aus] If another Methuselah is the target, he must declare whether he attempts or declines to block before Netwar can be played. [LSJ 20100507] [ANK 20210131-1]"
   - "[chi] Can be used by a vampire who is already attempting to block. [ANK 20181122-2]"
 101276|Neutral Guard:
-  - "If another effect also sets the range, the first to resolve has priority (eg. {Squirrel's Balance} and {Asanbonsam Ghoul} resolve before). [PIB 20120214]"
+  - If another effect also sets the range, the first to resolve has priority (eg. {Squirrel Balance} and {Asanbonsam Ghoul} resolve before). [PIB 20120214]
 101279|The New Inquisition:
-  - "When a vampire goes to torpor, the card is replaced before any other effect (eg. before losing pool to {Fame}). [LSJ 20100527]"
+  - When a vampire goes to torpor, the card is replaced before any other effect (eg. before losing pool to {Fame}). [LSJ 20100527]
 101280|New Management:
-  - "Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
-  - "Can be used on one of your own location. [LSJ 20080803-2]"
+  - Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]
+  - Can be used on one of your own location. [LSJ 20080803-2]
 101285|Nightmares upon Nightmares:
-  - "Mortal allies are not affected, and vampires with capacity above the number of Gehenna cards in play are not affected. [LSJ 20040415]"
+  - You cannot end your unlock phase or pass the impulse if you control a minion you haven't locked or burned a card for. [ANK 20210322]
+  - You can handle the effect by locking an already locked minion, then use his Infernal trait to unlock them. [ANK 20210322-2]
+  - Mortal allies are not affected, and vampires with capacity above the number of Gehenna cards in play are not affected. [LSJ 20040415]
 101287|Nightstick:
-  - "Can prevent up to 3 damage, it can prevent less. [RTR 20041202]"
+  - Can prevent up to 3 damage, it can prevent less. [RTR 20041202]
+  - Both strikes are only effective at close range. [ANK 20220814-2]
 101290|No Confidence:
-  - '"loses the benefit" means he gets no vote, is note considered titled, and yields the title immediately if it would contest. [LSJ 20080602] [RBK 20181001-10]'
+  - Is not a card requiring an Anarch. [LSJ 20080812]
+  - '"loses the benefit" means he gets no vote, is not considered titled, and yields the title immediately if it would contest. [LSJ 20080602] [RBK 20200701-3]'
+101291|No Secrets From the Magaji:
+  - It still burns if a block is attempted and then an effect prevents the block (eg. {Daring the Dawn}). [LSJ 20090810]
+  - It does not provide the ability to play reaction cards while locked (this is not a wake). [LSJ 20070208]
 101293|Nocturn:
-  - 'The "can act the turn it is recruited" text does not let him act during an opponent''s turn if it was recruited then (eg. using {Madness Network}). [ANK 20200813-3] [ANK 20200930]'
+  - The "can act the turn it is recruited" text does not let him act during an opponent's turn if it was recruited then (eg. using {Madness Network}). [ANK 20200813-3] [ANK 20200930]
 101295|Nod:
-  - "Choose for each equipment which minion will receive it, then transfer all the equipment accordingly. [ANK 20190717-1]"
+  - Choose for each equipment which minion will receive it, then transfer all the equipment accordingly. [ANK 20190717-1]
 101296|Nose of the Hound:
   - "[aus], [spi] If the target unlocks and the action is not blocked, it is successful but has no effect. [LSJ 20070411] [LSJ 20090514]"
 101302|Nosferatu Putrescence:
-  - "Can be used by a vampire in torpor. [LSJ 20020416]"
-  - "Can be played by a minion of a Methusalah not involved in the current combat. [ANK 20181101]"
+  - Can be used by a vampire in torpor. [LSJ 20020416]
+  - Can be played by a minion of a Methuselah not involved in the current combat. [ANK 20181101]
 101305|NRA PAC:
-  - "Does not affect equip actions performed prior to its arrival in play. [LSJ 20061218]"
+  - Does not affect equip actions performed prior to its arrival in play. [LSJ 20061218]
+  - The minions who performed an equip action when it was in play unlock at the end of turn regardless of wether NRA PAC is still in play or not. [LSJ 20080619]
+101306|NSA Trio:
+  - Only applies once each turn for the first eligible combat. [LSJ 20050215]
 101309|Obedience:
-  - "The action has reached resolution, so is subject to NRA (Non Repeatable Action) rules. [LSJ 20070709]"
-  - 'Actions without card (provided by the rulebook) are not "the same" as actions provided by cards (played or in play). [LSJ 20060522]  [LSJ 20060824] [LSJ 20080725] [LSJ 20090617]'
+  - The action has reached resolution, so is subject to NRA (Non Repeatable Action) rules. [LSJ 20070709]
+  - Actions without card (provided by the rulebook) are not "the same" as actions provided by cards (played or in play). [LSJ 20060522]  [LSJ 20060824] [LSJ 20080725] [LSJ 20090617]
   - "Actions without card (provided by the rulebook) can be repeated if they have different targets. Equipping from a minion targets the equipments: if one equipment is the same, the action is the same. [RTR 19950509] [LSJ 20080710] [ANK 20200502]"
-  - "Actions provided by cards in play are not the same if the card is not the same, even if the cards have the same name. [LSJ 20080725]"
-  - "Can be played by an unlocked older vampire to avoid a new combat queued after a preceding combat, if the opponent is still the acting vampire. [LSJ 19991025]"
-  - "The action ends unsuccessfuly immediately, combat does not happen, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20170105] [ANK 20200207]"
-  - "Cannot be played if the opponent is not the acting vampire, for example if a slave took his place. [ANK 20171212]"
+  - Actions provided by cards in play are not the same if the card is not the same, even if the cards have the same name. [LSJ 20080725]
+  - Can be played by an unlocked older vampire to avoid a new combat queued after a preceding combat, if the opponent is still the acting vampire. [LSJ 19991025]
+  - The action ends unsuccessfuly immediately, combat does not happen, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20170105] [ANK 20200207]
+  - Cannot be played if the opponent is not the acting vampire, for example if a slave took his place. [ANK 20171212]
 101315|Of Noble Blood:
-  - "Is a Ⓓ action if a vampire controlled by another Methusalah is chosen. [ANK 20190606]"
+  - Is a directed action if a vampire controlled by another Methuselah is chosen. [ANK 20190606]
 101317|Ohoyo Hopoksia (Bastet):
-  - "If her ability is used when a minion blocks an action, the blocking minion still locks for the block. [ANK 20200714]"
+  - If her ability is used when a minion blocks an action, the blocking minion still locks for the block. [ANK 20200714]
 101320|Omael Kuman:
-  - "When setting the range for the round, no other effect can be used to reset the range. Skip the determine range step this round, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]"
+  - When setting the range for the round, no other effect can be used to reset the range. Skip the determine range step this round, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]
 101321|On the Qui Vive:
   - "The vampire need not attempt to block nor play further reaction cards: that is merely an option. [TOM 19951129]"
-  - "Can be played after action resolution to use a reaction card (eg. {Fast Reaction} after combat). [LSJ 20091123]"
+  - Can be played after action resolution to use a reaction card (eg. {Fast Reaction} after combat). [LSJ 20091123]
 101322|Open Dossier:
-  - "Can be used by a vampire who is already attempting to block. [ANK 20181122-2]"
+  - Can be used by a vampire who is already attempting to block. [ANK 20181122-2]
 101325|Ophidian Gaze:
-  - '[SER][PRE] Can be used to cancel an action modifier player "after the action/referendum is successful" (eg. {Voter Captivatoin} or {Freak Drive}). [ANK 20180909]'
+  - '[SER][PRE] Can be used to cancel an action modifier player "after the action/referendum is successful" (eg. {Voter Captivation} or {Freak Drive}). [ANK 20180909]'
+  - '[SER][PRE] Cards are not replaced during the "as played" window. [LSJ 20061013]'
+  - '[SER][PRE] If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
 101330|Orgy of Blood:
-  - "Can be used by a vampire going to torpor or about to be burned. [LSJ 20100721]"
+  - Can be used by a vampire going to torpor or about to be burned. [LSJ 20100721]
 101331|Orun:
-  - "A vampire with multiple Oruns will only burn one Orun if he successfully bleeds for 2 or more. [LSJ 20090603]"
+  - A vampire with multiple Oruns will only burn one Orun if he successfully bleeds for more than 2. [LSJ 20090603]
 101333|Ossian:
-  - "His life total can exceed his starting life capacity (it is the case for all allies). [ANK 20171109]"
-  - "The life is gained after the presses are handled. It is gained if the round ends prematurely. [RTR 20030519]"
-  - "The Auspex [aus] special applies to whatever the current action is, not just to his special enter combat action. [LSJ 20050201]"
-  - "If Auspex [aus] was used to block him, the blocker can use an effect to set the range, but not a {Sniper Rifle} as it would require him to strike with it, which he cannot. [LSJ 20100827]"
+  - His life total can exceed his starting life capacity (it is the case for all allies). [ANK 20171109]
+  - The life is gained after the presses are handled. It is gained if the round ends prematurely. [RTR 20030519]
+  - The Auspex [aus] special applies to whatever the current action is, not just to his special enter combat action. [LSJ 20050201]
+  - If Auspex [aus] was used to block him, the blocker can use an effect to set the range, but not a {Sniper Rifle} as it would require him to strike with it, which he cannot. [LSJ 20100827]
+  - If no Auspex [aus] was used previously, an Auspex [aus] strike can be used (eg. {Charismatic Aura}). [ANK 20210614]
 101334|Oubliette:
-  - "[OBT] If the combat continues or a new combat begins, no damage is done. [RTR 20020501]"
-  - "[OBT] If the strike is dodged, no damage is done. [LSJ 19980526] [RTR 20041202]"
-  - "[OBT] Is a damage dealing strike and can be modified by other effects like {Target Vitals} or {Dam the Heart's River}, even if they are done after combat. [ANK 20170111] [PIB 20130319]"
+  - "[OBT] If the combat continues or a new combat begins, no blood is burned. [RTR 20020501]"
+  - "[OBT] If the strike is dodged, no blood is burned. [LSJ 19980526] [RTR 20041202]"
+  - "[OBT] Does not inflict damage (eg. does not benefit from {Target Vitals}). [LSJ 20080226]"
 101336|Out of the Frying Pan:
-  - "Is a change of the actual sect. A temporary effect overriding the sect has precendence. [LSJ 20100811]"
-  - "If the target changes sect to a sect inappropriate for his title, he loses its benefit until his sect is appropriate. He immediately yields the title if it is contested or he receives a new one. [LSJ 20060904]"
+  - Is a change of the actual sect. A temporary effect overriding the sect has precendence. [LSJ 20100811]
+  - If the target changes sect to a sect inappropriate for his title, he loses its benefit until his sect is appropriate. He immediately yields the title if it is contested or he receives a new one. [LSJ 20060904]
 101338|Outside the Hourglass:
-  - "No other effect can be used before the damage prevention window, it begins immediately. [ANK 20170930]"
-  - "Both minions can play prevention and non-prevention pre-range effects during the damage prevention window. [ANK 20170930]"
-  - "The damage is applied even if the combat ends prematurely (eg. {Illusions of the Kindred}) [ANK 20180104] [LSJ 19971110]"
+  - The damage is inflicted by the minion (not environmental). [PIB 20120426]
+  - Both minions can play prevention and non-prevention pre-range effects before mending the damage. If another pre-range damaging effect is played then, all damages are prevented and mended together. [ANK 20170930]
+  - The damage is applied even if the combat ends prematurely (eg. {Illusions of the Kindred}) [ANK 20180104] [LSJ 19971110]
 101342|Pack Alpha:
-  - "Requirements (clan, discipline) apply. [LSJ 20051207]"
-101345|Palatial Estate:
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
+  - Requirements (clan, discipline) apply. [LSJ 20051207]
+101348|Panacea:
+  - "[aus] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Helena (ADV)}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 101349|Pandora's Whisper:
-  - "The card to retrieve must be announced when declaring the action. [LSJ 20010627]"
+  - The card to retrieve must be announced when declaring the action. [LSJ 20010627]
 101353|Parity Shift:
-  - "Can not be played if there is no legal target (no other Methusalah with more pool than you). [ANK 20191228]"
-  - "The pool awarded can be used to play {Life Boon} to save the target from an oust. [LSJ 20100527]"
-  - "If the target has less than 3 pool when referendum passes, the Methusalah calling the referendum chooses how to distribute within the bounds of the terms. [LSJ 20010606]"
+  - Can not be played if there is no legal target (no other Methuselah with more pool than you). [ANK 20191228]
+  - The pool awarded can be used to play {Life Boon} to save the target from an oust. [LSJ 20100527]
+  - If the target has less than 3 pool when referendum passes, the Methuselah calling the referendum chooses how to distribute within the bounds of the terms. [LSJ 20010606]
+  - Changes in pool during the referendum (after terms are chosen) do not affect the outcome. [LSJ 20041004]
+"101357|Patagia: Flaps Allowing Limited Flight":
+  - Can only be used when the vampire its on is in combat himself. [ANK 20221021]
 101380|Peace Treaty:
-  - "Only requires that the pool cost be paid in order to keep the weapon. Blood costs, if any, need not be repaid to keep a weapon. [RTR 20010710]"
-  - "Can be called even if there are no weapons in play. [RTR 20010710]"
-  - "One can decide to burn a weapon with no pool cost (not paying zero). [ANK 20190724]"
+  - Only requires that the pool cost be paid in order to keep the weapon. Blood costs, if any, need not be repaid to keep a weapon. [RTR 20010710]
+  - Can be called even if there are no weapons in play. [RTR 20010710]
+  - One can decide to burn a weapon with no pool cost (not paying zero). [ANK 20190724]
 101381|Peacemaker:
-  - 'If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]'
-  - 'If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
+  - If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]
+  - If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]
   - '"continue as if unblocked" moves the action card from the ash heap (where it went when the action was blocked) to limbo (where it should be if the action is not blocked). If the action card is not in the ash heap, then the action cannot be continued. [LSJ 20070808-1]'
 101383|Pentex™ Loves You!:
   - "The ability to increase bleed is treated as an action modifier: it can be used at any time during the action. [LSJ 19970718]"
-"101385|Père Lachaise, France":
-  - "The vampire retrieved need only be in your ash heap. It does not have to be a vampire that you had first controlled. [LSJ 20040812]"
-  - "The crypt card on it is out of play and should be face down. [LSJ 20040812]"
+101385|Père Lachaise, France:
+  - The vampire retrieved need only be in your ash heap. It does not have to be a vampire that you had first controlled. [LSJ 20040812]
+  - The crypt card on it is out of play and should be face down. [LSJ 20040812]
 101388|Perfectionist:
   - "No blood can be gained if a reaction card is played and canceled as it is played: it has still been played. [LSJ 20070330]"
-  - 'Cards and effects that can be played "after resolution" can be played after the gain blood effect. [ANK 20190113]'
-  - "The blood can be gained if the action is unblocked even if it has no effect (due to lack of a suitable target, for example). [LSJ 20070411]"
+  - Cards and effects that can be played "after resolution" can be played after the gain blood effect. [ANK 20190113]
+  - The blood can be gained if the action is unblocked even if it has no effect (due to lack of a suitable target, for example). [LSJ 20070411]
 101395|Personal Scourge:
-  - "If the opponent dodges this strike, his weapons are unaffected and do damage this round. [LSJ 20040928]"
-  - "Does not protect the target from self-inflicted damage from a weapon. [LSJ 19980216]"
+  - If the opponent dodges this strike, his weapons are unaffected and do damage this round. [LSJ 20040928]
+  - Does not protect the target from self-inflicted damage from a weapon. [LSJ 19980216]
   - "[DEM] The press can only be used during the current round. [TOM 19960521]"
-"101400|Pier 13, Port of Baltimore":
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
 101401|Piper:
-  - "When used to recruit an ally, the ally cannot act this turn. [LSJ 20080630] [RTR 20180303]"
-  - "This is not an action, so cost reductions refering to an action like {Charisma} or {Erichtho} do not apply. [LSJ 20090115-1] [ANK 20170309]"
-  - "This does not count as performing the action to recruit this ally in respect to section 6.1 of the rules. The same vampire can recruit the same ally the normal way later this turn if he unlocks (and/or Piper it a second time). [LSJ 20080815]"
-  - "When recruiting an ally or retainer whose effect depend on Discipline level, the chosen vampire decides in respect to his disciplines the normal way. [LSJ 20080803]"
-  - 'The ally card is not "played" by the vampire (eg. {Louhi}''s ability cannot cancel it). [ANK 20201229]'
+  - When used to recruit an ally, the ally cannot act this turn. [LSJ 20080630] [RTR 20180303]
+  - This is not an action, so cost reductions refering to an action like {Charisma} or {Erichtho} do not apply. [LSJ 20090115-1] [ANK 20170309]
+  - This does not count as performing the action to recruit this ally in respect to section 3 of the rules. The same vampire can recruit the same ally the normal way later this turn if he unlocks (and/or Piper it a second time). [LSJ 20080815]
+  - When recruiting an ally or retainer whose effect depend on Discipline level, the chosen vampire decides in respect to his disciplines the normal way. [LSJ 20080803]
+  - The ally card is not "played" by the vampire (eg. {Louhi}'s ability cannot cancel it). [ANK 20201229]
 101405|Pocket Out of Time:
-  - "If used to start a new combat, effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]"
-  - "Cannot be used to start a new combat if there is already a pending combat queued. [RTR 20020501]"
+  - "[obt] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {The Path of Night}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
+  - "[TEM] Cannot be used to start a new combat if there is already a pending combat queued. [RTR 20020501]"
+  - "[TEM] Cannot be used to start a new combat if the opponent is not ready. [ANK 20220429]"
 101406|Poison Pill:
-  - 'Any decrease in pool (burning, paying, ...) is considered "loosing pool". [ANK 20180719-2]'
+  - Any decrease in pool (burning, paying, ...) is considered "loosing pool". [ANK 20180719-2]
+  - Gaining pool does not count as a negative loss. If a vote entails both a gain and a loss (eg. {Ancient Influence}), only the loss is counted, not the difference. [ANK 20180813] [LSJ 20041025]
 101416|Political Seizure:
-  - "If you yield the Political Seizure, the location it was contesting does not come into play under your control. [LSJ 19980223]"
+  - If you yield the Political Seizure, the location it was contesting does not come into play under your control. [LSJ 19980223]
 101418|Political Struggle:
-  - "The acting vampire gains X votes if the vampire with this card is burned, no matter how that vampire is burned. [LSJ 19990119]"
-  - "If the victim is burned by diablerie, the votes gained from Political Struggle are gained before the blood hunt referendum. [LSJ 20050707]"
+  - The acting vampire gains X votes if the vampire with this card is burned, no matter how that vampire is burned. [LSJ 19990119]
+  - If the victim is burned by diablerie, the votes gained from Political Struggle are gained before the blood hunt referendum. [LSJ 20050707]
+  - The votes include bonus votes from cards or ability (eg. {Eze, The Demon Prince}, {Firebrand}) but not conditional votes (eg. {Sundown}, {Aura of Invincibility}). [ANK 20211009] [LSJ 20040518-2]
+  - Priscus ballots are not taken into account. [ANK 20211009] [LSJ 20041025]
 101420|Port Authority:
   - "The cards are replaced before unlocking cards: other unlock effects cannot be ordered before. [ANK 20200129] [LSJ 20091208]"
 101422|The Portrait:
-  - "If the revealed vampire is between 7 and 10 capacity and the acting vampire has bled this turn already, he simply unlocks and the remainder of the effect is lost. [LSJ 20021118]"
+  - If the revealed vampire is between 7 and 10 capacity and the acting vampire has bled this turn already, he simply unlocks and the remainder of the effect is lost. [LSJ 20021118]
+101423|Possession:
+  - Any continuous effect having been applied to the vampire before is lost when they go in the ash heap. [LSJ 20040726]
 101425|Potio Martyrium:
-  - "Only requires one clan or the other (Tremere or Tremere antitribu) to be played. [ANK 20190203]"
-  - "The damage is done during combat, the opponent can use combat cards to prevent it. [LSJ 20100205]"
-  - "The damage does not depend on range. [ANK 20181024]"
+  - Only requires one clan or the other (Tremere or Tremere antitribu) to be played. [ANK 20190203]
+  - The damage is done during combat, the opponent can use combat cards to prevent it. [LSJ 20100205]
+  - The damage does not depend on range. [ANK 20181024]
 101426|Pounce:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
-  - "Damage done to the striking minion is environmental. [LSJ 19970801]"
-  - "The press can only be used during the current round. [TOM 19960521]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
+  - Damage done to the striking minion is environmental. [LSJ 19970801]
+  - The press can only be used during the current round. [TOM 19960521]
+101428|Power of All:
+  - Cannot be played during combat. [LSJ 20080618]
+  - Cannot be used to cancel an action card after using a reaction to "unlock and attempt to block". [LSJ 20021011]
+  - Other reaction cards (eg. wake effects) cannot be used if there is no action. [PIB 20120808]
+  - If used to cancel an action, the action is not performed in respect to section 3 of the rules. [LSJ 19980212]
+  - If used to cancel a limited effect (bleed, additional strike), then the limit is not triggered and another limited effect can be used. [LSJ 20030224]
+  - Can only cancel minion cards played from the hand in the normal fashion (eg. not weapons played via {Disguised Weapon} or allies from {Piper}). [RTR 20001020]
 101429|Power of One:
   - "[pre] Can only be used during a bleed action. [ANK 20171023] [RTR 19941109]"
+  - "[pot] A limited bleed modifier can be played before or after. [LSJ 20100218] [RTR 20180511-2]"
 101430|Power Structure:
-  - "Cannot be used during a Blood Hunt referendum, since there is no political action. [ANK 20190707]"
+  - Cannot be used during a Blood Hunt referendum, since there is no political action. [ANK 20190707]
 "101431|Powerbase: Barranquilla":
   - "{Church of the Order of St. Blaise} may be used to add a counter to it before it burns if it has zero counters. [LSJ 20050105-1]"
 "101432|Powerbase: Berlin":
-  - "Blood moved to it by a Ventrue action comes from the Ventrue. [LSJ 19970414]"
+  - Blood moved to it by a Ventrue action comes from the Ventrue. [LSJ 19970414]
+"101435|Powerbase: Los Angeles":
+  - A card requiring a Baron (eg. {Open War}) is a card requiring an Anarch. [LSJ 20080603] [LSJ 20050128]
 "101440|Powerbase: New York":
-  - "The action to steal the blood from your powerbase cannot be attempted by your own vampires. [RTR 19980928]"
-"101448|Praxis Seizure: Athens":
-  - "The additional capacity is lost if the title is lost. [TOM 19960210]"
-"101450|Praxis Seizure: Barcelona":
-  - "The additional capacity is lost if the title is lost. [TOM 19960210]"
-"101451|Praxis Seizure: Berlin":
-  - "The additional capacity is lost if the title is lost. [TOM 19960210]"
-"101453|Praxis Seizure: Brussels":
-  - "The additional capacity is lost if the title is lost. [TOM 19960210]"
-"101454|Praxis Seizure: Cairo":
-  - "The additional capacity is lost if the title is lost. [TOM 19960210]"
-"101460|Praxis Seizure: Geneva":
-  - "The additional capacity is lost if the title is lost. [TOM 19960210]"
-"101461|Praxis Seizure: Glasgow":
-  - "The additional capacity is lost if the title is lost. [TOM 19960210]"
-"101466|Praxis Seizure: Monaco":
-  - "The additional capacity is lost if the title is lost. [TOM 19960210]"
-"101467|Praxis Seizure: Paris":
-  - "The additional capacity is lost if the title is lost. [TOM 19960210]"
-"101468|Praxis Seizure: Rome":
-  - "The additional capacity is lost if the title is lost. [TOM 19960210]"
-"101470|Praxis Seizure: Stockholm":
-  - "The additional capacity is lost if the title is lost. [TOM 19960210]"
+  - The action to steal the blood from your powerbase cannot be attempted by your own vampires. [RTR 19980928]
 101475|Precognition:
-  - "The damage prevention can only be used if the block is successful, and only in the resulting (block-induced) combat. [LSJ 20010813]"
+  - "[AUS] The damage prevention can only be used if the block is successful, and only in the resulting (block-induced) combat. [LSJ 20010813]"
+  - "[AUS] The prevention does not carry over to a follow-up combat (eg. [CEL] {Psyche!}). [LSJ 20010819-2]"
+  - "[AUS] The prevention is provided again if a second block happens on the same action (eg. after [PRO] {Form of Mist}). [LSJ 20010814-2]"
 101479|Predator's Transformation:
-  - '[abo] [ACTION MODIFIER] Cards and effects that can be played "as the action is announced" (and only them) can be played before it. [ANK 20190425]'
+  - "[abo] [ACTION MODIFIER] Any directed action that ends up burning an ally counts as a directed action burning an ally (eg. {Horseshoes}). [ANK 20220507]"
+  - '[abo] [ACTION MODIFIER] Cards and effects that are played "as the action is announced" must be played before playing "regular" action modifier or reaction cards. [ANK 20190425]'
+  - "[abo] [ACTION MODIFIER] Replace the action card (if any) before playing it. [ANK 20181208]"
 101481|Pressing Flesh:
-  - "This is not a directed action, even when targeting another Methusalah's ash heap. [LSJ 20010627] [ANK 20181129]"
-  - "Requirements need not to be met. If the ally requires a discipline, the inferior version is used. If the cost is X (eg. {Reanimated Corpse}), X is zero. [LSJ 20071015] [LSJ 20100302-1]"
+  - This is not a directed action, even when targeting another Methuselah's ash heap. [LSJ 20010627] [ANK 20181129]
+  - Requirements need not to be met. If the ally requires a discipline, the inferior version is used. If the cost is X (eg. {Reanimated Corpse}), X is zero. [LSJ 20071015] [LSJ 20100302-1]
+  - Can be used on an Imbued, it comes back as a zombie ally and is not an Imbued anymore. It has no Creed and cannot use Virtues, nor does it get Convictions. [LSJ 20100211]
+  - A card burned while representing something else (eg. an ally raised by {Khazar's Diary (Endless Night)}) is not a valid target. [LSJ 20100325-2]
 101482|Preternatural Evasion:
   - "[CEL] The blood is burned when playing the card. [ANK 20200703-2]"
+  - "[CEL] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Mitru the Hunter}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 101485|Primal Instincts:
-  - "If the strike is canceled, the rest of the effect is also canceled. [RTR 20040501]"
+  - If the strike is canceled, the rest of the effect is also canceled. [RTR 20040501]
 101486|Principia Discordia:
   - "[qui] can target a vampire with no blood. [RTR 20010711]"
   - "[ser] can target a vampire with no blood.[RTR 20010711]"
   - "[ser] If the target unlocks and the action is not blocked, it is successful but has no effect. [LSJ 20070411] [LSJ 20090514]"
+  - "[aus] is directed against the Methuselah controlling the equipment, not the minion it's on. [LSJ 20090324]"
 101487|Priority Contract:
-  - "Can be burned to get 3 pool when a minion leaves the ready region because his controller is ousted. [ANK 20180129-2]"
+  - Can be burned to get 3 pool when a minion leaves the ready region because his controller is ousted. [ANK 20180129-2]
 101493|Projectile:
-  - "A minion who maneuvers with a gun may still use Projectile to shoot with that gun as his initial strike that round. [LSJ 20050304]"
-  - "Cannot be used to strike with a weapon whose strike isn't ranged. [LSJ 20050224-3]"
+  - A minion who maneuvers with a gun may still use Projectile to shoot with that gun as his initial strike that round. [LSJ 20050304]
+  - Cannot be used to strike with a weapon whose strike isn't ranged. [LSJ 20050224-3]
+  - Does not prevent the opponent from dodging, the dodge just has no effect. [LSJ 20030902-2] [LSJ 20060808-1]
 101494|Promise of 1528:
-  - "The action ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20200207]"
+  - The action ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20200207]
 101500|Protected Resources:
-  - "All cards which modify the bleed amount are applied before Protected Resources's effect. [TOM 19960413]"
+  - All cards which modify the bleed amount are applied before Protected Resources's effect. [TOM 19960413]
   - "Does not alter the bleed amount: it merely limits the maximum amount of pool the target of the bleed burns for the successful bleed. [LSJ 20030211]"
-  - "If you perform a bleed action that resolves as a bleed for 0, you don't burn your Protected Resources. [LSJ 20030701-1]"
+  - If you perform a bleed action that resolves as a bleed for 0, you don't burn your Protected Resources. [LSJ 20030701-1]
 101501|Protection Racket:
-  - "The additional intercept is gained or lost if the acting vampire changes sect during the action (eg. with {The Red Question} or {Mask of a Thousand Faces}). [ANK 20190416]"
+  - The additional intercept is gained or lost if the acting vampire changes sect during the action (eg. with {The Red Question} or {Mask of a Thousand Faces}). [ANK 20190416]
 101503|Provision of the Silsila:
-  - "Can be used even if the target is burned ot if the contract is burned when the target leaves the ready region (eg. {Priority Contract}). [PIB 20150512]"
+  - Can be used even if the target is burned ot if the contract is burned when the target leaves the ready region (eg. {Priority Contract}). [PIB 20150512]
 101504|Proxy Kissed:
-  - "Can be played on a vampire who already has a Proxy Kissed (and was moved to uncontrolled and re-influenced). [LSJ 20050720-1]"
-  - "Is played during your turn in the influence phase, counts against the master phase of your next turn and prohibits you to play a second out-of-turn master card before your next master phase. [PIB 20150524]"
+  - Can be played on a vampire who already has a Proxy Kissed (and was moved to uncontrolled and re-influenced). [LSJ 20050720-1]
+  - Is played during your turn in the influence phase, counts against the master phase of your next turn and prohibits you to play a second out-of-turn master card before your next master phase. [PIB 20150524]
 101507|Psyche!:
+  - "[CEL] Cannot be played if the opponent is going to torpor. [ANK 20220429]"
   - "[CEL] Effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]"
   - "[CEL] Cannot be played if there is already a combat queued. [RTR 20020501]"
   - "[CEL] Is played during combat, when combat is about to end. It must be played after the presses are handled and can be played if the round ends prematurely. [RTR 20030519], [PIB 20111202]"
   - '[CEL] Replacements effects that are played when a combat "would end" (eg. Telepathic Tracking) cannot be play afterwards. [ANK 20191219]'
-  - "Can be retrieved by {Marthe Dizier} (reversal of previous ruling). [PIB 20111208]"
+  - '[CEL] Can be played before of after effects that are played "at the end of combat". [LSJ 20021113] [ANK 20191219] [ANK 20180910-1]'
+  - Can be retrieved by {Marthe Dizier} (reversal of previous rulings). [PIB 20111208]
 101511|Psychomachia:
-  - "The blocker is not locked. [LSJ 20030902-1]"
+  - The blocker is not locked. [LSJ 20030902-1]
   - "[pre]: The action has reached resolution, so is subject to NRA (Non Repeatable Action) rules. [RTR 20020501] [LSJ 20070709]"
 101515|Pulled Fangs:
-  - "Counts up damage successfully inflicted during the round by the minions, retainers do not count. [TOM 19950304]"
-  - "Must be played after the presses are handled and can be played if the round ends prematurely. [RTR 20030519]"
-  - 'Can be played before or after effects that are played at the end of the round or "when the combat would end" (eg. [AUS] {Telepathic Tracking}). Can be played after [CEL] {Psyche!} [LSJ 20021113] [ANK 20191219] [ANK 20180910-1]'
+  - Counts up damage successfully inflicted during the round by the minions, retainers and environmental damage do not count. [TOM 19950304] [LSJ 20010812]
+  - Must be played after the presses are handled and can be played if the round ends prematurely. [RTR 20030519]
+  - Can be played before or after effects that are played at the end of the round or "when the combat would end" (eg. [AUS] {Telepathic Tracking}). Can be played before or after [CEL] {Psyche!} [LSJ 20021113] [ANK 20191219] [ANK 20180910-1]
   - "A total of two actions must be performed (by whomever) to remove it. Vampires A and B can both take the action, then it is removed. [ANK 20170202-2] "
 101524|Pushing the Limit:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 101525|Putrefaction:
   - "[THN] Damage is environmental. [RTR 19970630]"
   - "[thn] [THN] It can still be burned if the vampire is already prevented from unlocking as normal by another effect. [RTR 20070707]"
 101526|Putrescent Servitude:
-  - "Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
-  - "Does not stack with similar effects to provide superior [POT] (eg. {Leech}). [ANK 20180111]"
+  - Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]
+  - Does not stack with similar effects to provide superior [POT] (eg. {Leech}). [ANK 20180111]
+101532|Quickness:
+  - "[CEL] A limited additional strike can be played before or after. [LSJ 20001206] [ANK 20211124]"
 101533|Quicksilver Contemplation:
   - "[aus][tem] [ACTION MODIFIER][REACTION] Cannot be burned during a referendum that is automatically passing. [PIB 20150105] [LSJ 19980107]"
+  - "[AUS][TEM] A limited bleed modifier can be played before or after. [LSJ 20100218] [RTR 20180511-2]"
 101536|The Rack:
-  - "May not select a new target just for falling out of contention. [RTR 19960112]"
-  - "Will not target a new copy of the same vampire if the original is burned or yielded. [TOM 19960122]"
-  - "Can provide blood if the target is in torpor, not if it is not controlled (eg. after a {Banishment}). [PIB 20150522] [LSJ 20010623]"
-  - "Tracks the target if it leaves the game by contesting or {Banishment}: if the target gets back into play, The Rack gives it blood again. [LSJ 20010809-2]"
-  - "If the target is stolen, the new controller chooses if the vampires gains blood during The Rack controllers unlock phase. [ANK 20200130-2]"
+  - May not select a new target just for falling out of contention. [RTR 19960112]
+  - Will not target a new copy of the same vampire if the original is burned or yielded. [TOM 19960122]
+  - Can provide blood if the target is in torpor, not if it is not controlled (eg. after a {Banishment}). [PIB 20150522] [LSJ 20010623]
+  - "Tracks the target if it leaves the game by contesting or {Banishment}: if the target gets back into play, The Rack gives it blood again. [LSJ 20010809-2] [LSJ 20010809-3]"
+  - If the target is stolen, the new controller chooses if the vampires gains blood during The Rack controllers unlock phase. [ANK 20200130-2]
 101543|Rapid Healing:
-  - "Is not the default action, no blood is paid to leave torpor. [ANK 20181017]"
-  - 'Is a "leave torpor" action. [LSJ 19980126]'
+  - Is not the default action, no blood is paid to leave torpor. [ANK 20181017]
+  - Is a "leave torpor" action. [LSJ 19980126]
 101545|Raptor:
-  - "If combat ends and a new combat start (eg. [CEL] {Psyche!}), the opponent redraws and discard again. [LSJ 20030530]"
+  - If combat ends and a new combat start (eg. [CEL] {Psyche!}), the opponent redraws and discard again. [LSJ 20030530]
 101546|Rastacourere:
-  - "Does not affect the Prisci sub-referendum. [LSJ 20041202]"
+  - Does not affect the Prisci sub-referendum. [LSJ 20041202]
 101552|Ravnos Cache:
-  - "The blood may be used in place of pool or blood, as appropriate to the cost of the equipment. [RTR 19960112]"
+  - The blood may be used in place of pool or blood, as appropriate to the cost of the equipment. [RTR 19960112]
 101553|Ravnos Carnival:
-  - "A Ravnos can attempt an action that he cannot pay for himself if the cost can be paid with the Carnival's help. [LSJ 20050408]"
-  - "How many counters are used from the Carnival must be annouced as part of the terms of the action. [RTR 20111202]"
-  - "Cannot be used to pay for the cost of a cardless action or of an action provided by a card in play. [ANK 20180109] [LSJ 20070224]"
+  - A Ravnos can attempt an action that he cannot pay for himself if the cost can be paid with the Carnival's help. [LSJ 20050408]
+  - How many counters are used from the Carnival must be annouced as part of the terms of the action. [RTR 20111202]
+  - Cannot be used to pay for the cost of a cardless action or of an action provided by a card in play. [ANK 20180109] [LSJ 20070224]
 101554|Raw Recruit:
-  - "The created vampire is not unique. [LSJ 20100221]"
-  - "Blood, equipments and other cards on the initial target are burned. [LSJ 20100302-2]"
+  - The created vampire is not unique. [LSJ 20100221]
+  - Blood, equipments and other cards on the initial target are burned. [LSJ 20100302-2]
+101555|Rayzeel's Song:
+  - "[ani] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Dragos}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 101557|React with Conviction:
-  - "If used to cancel a {Corruption} action, then the action is canceled in its entirety and the corruption counters are not burned. [LSJ 20070222-1]"
-  - 'If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
+  - If used to cancel an action, the action is not performed, the minion stays unlocked (and can try the same action again). [LSJ 20060425]
+  - If used to cancel a {Corruption} action, then the action is canceled in its entirety and the corruption counters are not burned. [LSJ 20070222-1]
+  - If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]
+  - Can be used to cancel all action cards, including employ retainer, recruit ally and political action. [ANK 20200813-2]
 101559|Read the Winds:
   - "[ANI][AUS] Can be used by a vampire who is already attempting to block. [ANK 20181122-2]"
 101561|Reality Mirror:
-  - "Cannot be used to bypass restrictions (like Clan restriction or any other play restriction). [LSJ 20020426]"
+  - Cannot be used to bypass restrictions (like Clan restriction or any other play restriction). [LSJ 20020426]
+101563|Reanimated Corpse:
+  - Looses all its pathos counters if it is burned. If it is brought back with X being zero (eg. {Compel the Spirit}), it has no pathos counter and burns immediately. [LSJ 20071015]
 101565|Rebirth:
-  - "Cannot be used following an {Amaranth} or an {Abactor} as they are not diablerie actions. [ANK 20190701]"
+  - Cannot be used following an {Amaranth} or an {Abactor} as they are not diablerie actions. [ANK 20190701]
 101567|Reckless Agitation:
-  - "Cannot allocate 6 points to a single Methusalah, but you can allocate points to yourself. [LSJ 20000622]"
-  - "Can allocate more points than a Methusalah has pool. [LSJ 20020819]"
+  - Cannot allocate 6 points to a single Methuselah, and you cannot allocate points to yourself. [LSJ 20000622] [LSJ 20100129]
+  - Can allocate more points than a Methuselah has pool. [LSJ 20020819]
 101571|Recure of the Homeland:
-  - "Is not the default action, no blood is paid to leave torpor. [ANK 20181017]"
+  - Is not the default action, no blood is paid to leave torpor. [ANK 20181017]
+101572|Recurring Contemplation:
+  - "[TEM] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {The Ankara Citadel, Turkey}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 101573|Red Herring:
-  - "The action has reached resolution, so is subject to NRA (Non Repeatable Action) rules. [LSJ 20070709]"
-  - 'Actions without card (provided by the rulebook) are not "the same" as actions provided by cards (played or in play). [LSJ 20060522]  [LSJ 20060824] [LSJ 20080725] [LSJ 20090617]'
+  - The action has reached resolution, so is subject to NRA (Non Repeatable Action) rules. [LSJ 20070709] [ANK 20221011-2]
+  - Actions without card (provided by the rulebook) are not "the same" as actions provided by cards (played or in play). [LSJ 20060522]  [LSJ 20060824] [LSJ 20080725] [LSJ 20090617]
   - "Actions without card (provided by the rulebook) can be repeated if they have different targets. Equipping from a minion targets the equipments: if one equipment is the same, the action is the same. [RTR 19950509] [LSJ 20080710] [ANK 20200502]"
-  - "Actions provided by cards in play are not the same if the card is not the same, even if the cards have the same name. [LSJ 20080725]"
+  - Actions provided by cards in play are not the same if the card is not the same, even if the cards have the same name. [LSJ 20080725]
 101575|The Red Question:
-  - "Is a change of the actual sect. A temporary effect overriding the sect has precendence and if it does, this card burns (eg. {Writ of Acceptance}). [LSJ 20100811]"
-  - "If the target changes sect to a sect inappropriate for his title, he loses its benefit until his sect is appropriate. He immediately yields the title if it is contested or he receives a new one. [LSJ 20060904]"
-  - 'Does not make the action an action that "makes this vampire anarch" (eg. {CrimethInc.} cannot be played). [ANK 20180125]'
-  - "The burn option cannot be used if you have a non-titled, non-Anarch vampire in torpor. [LSJ 20091204]"
+  - Is a change of the actual sect. A temporary effect overriding the sect has precendence and if it does, this card burns (eg. {Writ of Acceptance}). [LSJ 20100811]
+  - If the target changes sect to a sect inappropriate for his title, he loses its benefit until his sect is appropriate. He immediately yields the title if it is contested or he receives a new one. [LSJ 20060904]
+  - Does not make the action an action that "makes this vampire anarch" (eg. {CrimethInc.} cannot be played). [ANK 20180125]
+  - The burn option cannot be used if you have a non-titled, non-Anarch vampire in torpor. [LSJ 20091204]
 101578|Redirection:
-  - 'Must be played before action resolution, ie. before any modifier or reaction played "as the action/bleed would be successful" are played. It cannot be played after a {Spying Mission} on the vampire triggers. [LSJ 19980105]'
+  - Must be played before action resolution, ie. before any modifier or reaction played "as the action/bleed would be successful" are played. It cannot be played after a {Spying Mission} on the vampire triggers. [LSJ 19980105]
+  - "Can be played when failing to block because of stealth: it is still declining to block. [ANK 20211003]"
 101579|Redistribution:
-  - "Cannot target an uncontrolled Blood Brother. [LSJ 20061109]"
+  - Cannot target an uncontrolled Blood Brother. [LSJ 20061109]
 101581|Reform Body:
-  - "If the vampire saves himself from diablerie, the diablerie is considered unsuccessful. The diablerist gets nothing from the victim, and no Blood Hunt is called. [LSJ 19970224]"
-  - "Cannot be played by vampires who aren't controlled. [LSJ 19970224]"
-  - "Cannot be played when burned as a result of a Blood Hunt referendum. [LSJ 20070417]"
+  - If the vampire saves himself from diablerie, the diablerie is considered unsuccessful. The diablerist gets nothing from the victim, and no Blood Hunt is called. [LSJ 19970224]
+  - Cannot be played by vampires who aren't controlled. [LSJ 19970224]
+  - Cannot be played when burned as a result of a Blood Hunt referendum. [LSJ 20070417]
 101582|Reformation:
   - "[chi] Cannot be used if there is no equipment to destroy. [RTR 19980928]"
-101587|Regent:
-  - 'It is a title card, so it is out of play if the title is contested, and the "enter combat" action is not usable when the card is not in play. [LSJ 20070808-2]'
+  - "[dom] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Salvador Garcia}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 101588|Rego Motum:
-  - "Prevents up to 2 or 4 damage, it can be used to prevent less. [RTR 20041202]"
-  - "Cannot be used if there is no damage to prevent. [LSJ 20001114]"
-  - "Unused prevention does not carry over. [LSJ 20001114]"
+  - Prevents up to 2 or 4 damage, it can be used to prevent less. [RTR 20041202]
+  - Cannot be used if there is no damage to prevent. [LSJ 20001114]
+  - Unused prevention does not carry over. [LSJ 20001114]
 101589|Reindoctrination:
-  - "Only requires one clan or the other (Tremere or Tremere antitribu) to be played. [ANK 20190203]"
+  - Only requires one clan or the other (Tremere or Tremere antitribu) to be played. [ANK 20190203]
+101591|Reins of Power:
+  - Applies a pool gain then a pool loss. {Poison Pill} ignores the gain and only takes the loss into account, a Methuselah cannot withdraw even if the total was positive. [ANK 20180813]
 101595|Relentless Reaper:
   - "[for] Cannot be used if there is no damage to prevent. [LSJ 20001114]"
   - "[THN] Effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]"
   - "[THN] Cannot be played after [CEL] {Psyche!}. When played before, combat continues and {Psyche!} can only be played at the end of it. [ANK 20191219]"
   - '[THN] Must be played after presses, can be played if the round ends prematurely and can be played before or after effects that are played "at then of the round" (eg. {Taste of Vitae}). [LSJ 20021113] [RTR 20030519] [ANK 20180910-1]'
+  - "[THN] The burn blood effect is not reduced by effects that reduce the cost of the card. The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 101602|Renegade Garou:
-  - "The additional strike is mandatory. [PIB 20121028]"
+  - The additional strike is mandatory. [PIB 20121028]
 101603|Renewed Vigor:
-  - "[obe], [OBE]: Is undirected if you control the target, directed to the controller of the target otherwise. [PIB 20121210]"
+  - "[obe], [OBE]: Is undirected if you control the target, directed at the controller of the target otherwise. [PIB 20121210]"
 101605|Repo Man:
-  - "Paying for the equipment found is not optional if a ready minion meet the requirements. If paying the cost will oust the controlling Methuselah, then she is ousted. [RTR 19941109] [RTR 20010710]"
+  - Paying for the equipment found is not optional if a ready minion meet the requirements. If paying the cost will oust the controlling Methuselah, then she is ousted. [RTR 19941109] [RTR 20010710]
 101606|Repulsion:
   - "[OBE] Can be used even if the stealth is not currently needed. [LSJ 20011214-2]"
-  - '[pre] Cards and effects that can be played "as the action is announced" (and only them) can be played before it. [ANK 20190425]'
+  - '[pre] Cards and effects that are played "as the action is announced" must be played before playing "regular" action modifier or reaction cards. [ANK 20190425]'
+  - "[pre] Replace the action card (if any) before playing it. [ANK 20181208]"
 101608|Resilience:
-  - "Cannot be used if there is no damage to prevent. [LSJ 20001114]"
-  - "Prevents up to 3 non-aggravated damage, it can be used to prevent less. [RTR 20041202]"
-  - "Unused prevention does not carry over. [LSJ 20001114]"
+  - Cannot be used if there is no damage to prevent. [LSJ 20001114]
+  - Prevents up to 3 non-aggravated damage, it can be used to prevent less. [RTR 20041202]
+  - Unused prevention does not carry over. [LSJ 20001114]
+  - "[FOR] Cannot be used to prevent aggravated damage, even if the minion treats them as normal damage (eg. {Skin of Night}). [LSJ 20040812-2] [PIB 20130327]"
 101609|Resilient Mind:
-  - "Can be used when a {Form of Corruption} is put into play to protect that vampire from that {Form of Corruption}. [LSJ 20031223]"
+  - Can be used when a {Form of Corruption} is put into play to protect that vampire from that {Form of Corruption}. [LSJ 20031223]
 101610|Resist Earth's Grasp:
   - "[cel] [COMBAT] If used to maneuver, the optional press can only be used during the current round. [TOM 19960521]"
 101614|Restricted Vitae:
-  - "A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]"
+  - A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]
 101615|Restructure:
-  - "Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
+  - Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]
 101616|Resume the Coil:
-  - "Is not the default action, no blood is paid to leave torpor or rescue from torpor. [ANK 20181017]"
+  - Is not the default action, no blood is paid to leave torpor or rescue from torpor. [ANK 20181017]
 101617|Resurrection:
-  - "Can only resurrect allies or retainers burned from play. Discards and blocked actions do not qualify. [LSJ 20011216-1]"
+  - Can only resurrect allies or retainers burned from play. Discards and blocked actions do not qualify. [LSJ 20011216-1]
+101623|Revelation of Despair:
+  - "[SER] When the acting minion gets stolen, the block still happens and the blocking minion locks. [ANK 20220127]"
 101624|Revelation of Ecstasy:
-  - "Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
-  - "Can target a locked minion. [ANK 20170303]"
+  - Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]
+  - Can target a locked minion. [ANK 20170303]
 101626|Revelation of Wrath:
-  - "Must be played after the presses are handled and can be played if the round ends prematurely. [RTR 20030519]"
-  - "Does not count environmental damage. [ANK 20200925]"
-  - "Can be played by a vampire going to torpor. Can be played by a vampire who is about to burn. [ANK 20201122] [ANK 20200926]"
-  - "Does not allow to take control of the opponent. [ANK 20200925]"
+  - Must be played after the presses are handled and can be played if the round ends prematurely. [RTR 20030519]
+  - Does not count environmental damage. [ANK 20200925]
+  - Can be played by a vampire going to torpor. Can be played by a vampire who is about to burn. [ANK 20201122] [ANK 20200926]
+  - Does not allow to take control of the opponent. [ANK 20200925] [ANK 20211105]
 101627|Revelations:
   - "[aus] You do not get to see the card drawn as replacement. [PIB 20121031]"
 101631|Revolutionary Council:
-  - "Unlocked Anarchs are chosen when choosing terms. They still count if they get locked during the vote. [LSJ 20081203]"
+  - Unlocked Anarchs are chosen when choosing terms. They still count if they get locked during the vote. [LSJ 20081203]
 101633|Rewind Time:
   - "[tem] Can be used to cancel all action cards, including employ retainer, recruit ally and political action. [ANK 20200813-2]"
   - '[tem] Cannot be used to cancel the action card after using a reaction to "unlock and attempt to block". [LSJ 20021011]'
   - '[tem] If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
-  - "[TEM] Other reaction cards (eg. wake effects) cannot be used as there is no action. [PIB 20120808]"
+  - "[TEM] Other reaction cards (eg. wake effects) cannot be used if there is no action. [PIB 20120808]"
+  - "[TEM] Cannot be played during combat. [LSJ 20080618]"
 101634|Riddle Phantastique:
-  - "If put into play with no counters, it burns immediately. [LSJ 20070307]"
+  - If put into play with no counters, it burns immediately. [LSJ 20070307]
 101635|Righteous Aura:
-  - "The card is burned before the vampire leaves the ready region (eg. it is burned if {Banishment} is used on the vampire it is on) [ANK 20180511-1]"
+  - The card is burned before the vampire leaves the ready region (eg. it is burned if {Banishment} is used on the vampire it is on) [ANK 20180511-1]
 101636|Rigor Mortis:
   - "[thn], [THN] The press can only be used during the current round. [TOM 19960521]"
 101637|Riposte:
   - "[cel] [CEL] The damage is dealt just after the combat ends. [RTR 19970630]"
   - "[cel] [CEL] The damage is only dealt if the strike was resolved at close range. [LSJ 19970915]"
   - "[cel] [CEL] If the strike is dodged, no damage is done. [LSJ 19980526] [RTR 20041202]"
   - "[cel] [CEL] If the combat continues or a new combat begins, no damage is done. [RTR 20020501]"
   - "[cel] [CEL] Is a damage dealing strike and can be modified by other effects like {Target Vitals} or {Dam the Heart's River}, even if they are done after combat.  [ANK 20170111] [PIB 20130319]"
 101640|The Rising:
-  - 'Anything that would increase the pool amount is considered "gaining pool". [ANK 20181105]'
-  - "Methusalahs do not gain the pool granted by a bleed action (eg. {Kindred Spirit}) if they do not have the edge or a VP beforehand. [LSJ 20100206-2]"
-  - "Methusalahs gain the pool granted by an effect after a successful bleed action (eg. {The unnamed}), since they get the edge before the effect kicks in. [LSJ 20100210-2]"
-  - "When ousting their prey, Methusalahs decide if they gain the VP before or after gaining the pool. [LSJ 20100208]"
+  - Anything that would increase the pool amount is considered "gaining pool". [ANK 20181105]
+  - Methuselahs do not gain the pool granted by a bleed action (eg. {Kindred Spirits}) if they do not have the edge or a VP beforehand. [LSJ 20100206-2]
+  - Methuselahs gain the pool granted by an effect after a successful bleed action (eg. {The unnamed}), since they get the edge before the effect kicks in. [LSJ 20100210-2]
+  - When ousting their prey, Methuselahs decide if they gain the VP before or after gaining the pool. [LSJ 20100208]
   - "{Off Kilter}'s additional pool cannot be gained if you do not have a VP (edge is burned before pool is gained). [LSJ 20100207]"
 101642|Ritual of the Bitter Rose:
-  - "Can be played after a diablerie, before the blood hunt. [ANK 20201228]"
+  - Can be played after a diablerie, before the blood hunt. [ANK 20201228]
 101649|Rolling with the Punches:
   - "[for] Cannot be used if there is no damage to prevent. [LSJ 20001114]"
+  - "[FOR] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Una}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 101650|Rom Gypsy:
-  - "He can lock to use his ability the turn he is recruited. [ANK 20180517]"
+  - He can lock to use his ability the turn he is recruited. [ANK 20180517]
 101652|Root of Vitality:
   - "[vic] Is not the default action, no blood is paid for the rescue. [ANK 20181017]"
 101654|Rötschreck:
-  - "Can only be played during the strike announcement phase, on the opponent, when a minion attempts to make a strike that is effective at the current range and would inflict aggravated damage to this opponent, even if the opponent treats aggravated damage as normal. [RTR 19961113] [RTR 19980623] [RTR 19980928] [RTR 20041202] [ANK 20200130-1]"
+  - Is played on the vampire that would receive the aggravated damage. [RTR 19980623]
+  - Can only be played after declaration of a strike, before resolution. It can be played before or after the opponent's strike is announced. [LSJ 19990217] [RTR 20041202]
+  - Cannot be played if a non-strike effect would inflict aggravated damage (eg. {Outside the Hourglass} with {Domain of Evernight}). REVERSAL of a 2011 ruling. [ANK 20220114]
+  - Cannot be played if the damage is not effective at the current range [RTR 19980928] [ANK 20211102]
+  - "Can be played and is effective even if the opponent has announced a Strike: Dodge or Strike: Combat Ends. [LSJ 20011005] [ANK 20211102]"
+  - Can be played and is effective even if the opponent treats aggravated damage as normal. [ANK 20200130-1]
   - "Combat ends immediately, strikes are not resolved (including strike: combat ends), damage prevention cannot be played, and a second Rötschreck cannot be played. [LSJ 19990217] [LSJ 20020715] [LSJ 20060803]"
-  - "Can be played before or after the opponent's strike is announced. [LSJ 19990217]"
-  - 'Combat cards usable "when the opposing vampire is going / should go into torpor" cannot be used. [LSJ 20020402]'
-  - "If the combat continues or a new combat begins, the card is put on the vampire, he is not locked and does not go to torpor. He still does not unlock as normal. [RTR 20020501] [LSJ 20071009]"
-  - 'The "does not unlock as normal" effect stops if Rötschreck is burned or removed. [ANK 20191025]'
+  - Combat cards usable "when the opposing vampire is going / should go into torpor" cannot be used. [LSJ 20020402]
+  - If the combat continues or a new combat begins, the card is put on the vampire, he is not locked and does not go to torpor. He still does not unlock as normal. [RTR 20020501] [LSJ 20071009]
+  - The "does not unlock as normal" effect stops if Rötschreck is burned or removed. [ANK 20191025]
 101655|Rowan Ring:
-  - "Adding damage to the Ring strike will not deal damage. [RTR 19960221]"
-  - 'Only usable at close range. Damage prevention cannot be used against it, but dodge and "strike: combat ends" will avoid the effect. [LSJ 19980219]'
-  - 'If placed on a minion that cannot have equipment, the Ring is burned. The "does not unlock as normal" effect still applies. [LSJ 19980831]'
-  - 'The "does not unlock as normal" effect continues to apply if the Ring is burned or moved. [LSJ 19980831]'
-101658|Ruins of Ceoris:
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
-"101660|Ruins of Villers Abbey, Belgium":
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
+  - Adding damage to the Ring strike will not deal damage. [RTR 19960221]
+  - Only usable at close range. Damage prevention cannot be used against it. [LSJ 19980219]
+  - If the opponent dodges or ends combat, they avoid the effect and the ring stays. [LSJ 19980219] [ANK 20220923]'
+  - If the strike is inflicted, the opponent is wounded (if they play {Undying Tenacity}, they go to torpor after combat). [LSJ 20090622-2]
+  - If placed on a minion that cannot have equipment, the Ring is burned. The "does not unlock as normal" effect still applies. [LSJ 19980831]
+  - The "does not unlock as normal" effect continues to apply if the Ring is burned or moved. [LSJ 19980831]
+101659|Ruins of Charizel:
+  - Only works when unlocking minions using their Infernal ability (eg. not with {Path of Evil Revelations} nor {Metro Underground}). [LSJ 20050228-2]
 101664|Rutor's Hand:
-  - 'If the vampire is stolen before "your next turn", the Hand will not allow the vampire an extra unlock until a Methuselah begins a turn with the vampire with the Hand under her control. [LSJ 20031106]'
+  - If the vampire is stolen before "your next turn", the Hand will not allow the vampire an extra unlock until a Methuselah begins a turn with the vampire with the Hand under her control. [LSJ 20031106]
 101665|Saatet-ta:
-  - "She can lock to use her ability the turn she is recruited. [ANK 20180517]"
+  - She can lock to use her ability the turn she is recruited. [ANK 20180517]
 101667|Sabbat Priest:
-  - "Burn blood effects are cumulative. [LSJ 19980225]"
-  - "A vampire with no blood can still block, he burns what he can. [LSJ 19970707]"
-  - "The same vampire can be chosen multiple times if multiple copies are played. [LSJ 19970707]"
+  - Burn blood effects are cumulative. [LSJ 19980225]
+  - A vampire with no blood can still block, he burns what he can. [LSJ 19970707]
+  - The same vampire can be chosen multiple times if multiple copies are played. [LSJ 19970707]
 101668|Sabbat Threat:
-  - "You can gain pool from the Edge before burning it to remove the threat counters, and loose no pool to the threat counters. [TOM 19951214-1]"
-"101670|Sacré-Cœur Cathedral, France":
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
+  - You can gain pool from the Edge before burning it to remove the threat counters, and loose no pool to the threat counters. [TOM 19951214-1]
+101671|Sacrifice:
+  - "Does not require a specific clan: vampires that can play cards as if they were of a required clan (eg. {Mata Hari}) cannot use their ability to match a target's clan. [LSJ 20100526]"
 101672|Sacrificial Lamb:
-  - "If the target has a {Soul Gem of Etrius}, the Gem effet applies and it cannot be transfered. [LSJ 19970516]"
+  - If the target has a {Soul Gem of Etrius}, the Gem effect applies and it cannot be transfered. [LSJ 19970516]
+  - If the target does not burn (eg. {Byzar}'s ability) then no blood is gained and no equipment transfered. [LSJ 20100423]
 101675|Samuel Haight:
-  - 'He cannot "steal equipment as a strike" if there is no equipment to steal. [RTR 19980928]'
-"101676|San Lorenzo de El Escorial, Spain":
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
-101677|San Nicolás de los Servitas:
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
+  - He cannot "steal equipment as a strike" if there is no equipment to steal. [RTR 19980928]
 101681|The Sargon Fragment:
-  - "When using the provided action, the card to retrieve must be named when declaring the action. [LSJ 20010627]"
-  - "Upon resolution, any copy of the named card in the ash heap can be fetched. [LSJ 20050228]"
+  - When using the provided action, the card to retrieve must be named when declaring the action. [LSJ 20010627]
+  - Upon resolution, any copy of the named card in the ash heap can be fetched. [LSJ 20050228]
+101683|Savannah Runner:
+  - "[cel] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {High Orun}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 101684|Save Face:
-  - "Can be used by a vampire in torpor. [LSJ 20020416]"
-  - "Can be played by a minion of a Methusalah not involved in the current combat. [ANK 20181101]"
-  - "The gain blood effect is applied after combats ends, no combat card can be played afterwards. The acting player chooses the order of after-combat effects. [LSJ 20071116]"
+  - Can be used by a vampire in torpor. [LSJ 20020416]
+  - Can be played by a minion of a Methuselah not involved in the current combat. [ANK 20181101]
+  - The gain blood effect is applied after combats ends, no combat card can be played afterwards. The acting player chooses the order of after-combat effects. [LSJ 20071116]
 101688|Scarlet Lore:
   - "[nec] The card to retrieve must be announced when declaring the action. [LSJ 20010627]"
 101689|Scattershot:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 101691|Scobax:
   - "[STR] If the action ends, no other action modifier or reaction can be played afterwards. [RTR 20180719]"
-  - "If another Methusalah is the target, he must declare whether he attempts or declines to block before Scobax can be played. [PIB 20150820] [ANK 20200607]"
+  - "[STR] If the action ends, it has reached resolution, so is subject to NRA (Non Repeatable Action) rules. [ANK 20211015]"
+  - If another Methuselah is the target, he must declare whether he attempts or declines to block before Scobax can be played. [PIB 20150820] [ANK 20200607]
 101692|Scorn of Adonis:
-  - "May be played at any time during the voting process, and will retroactively cause the loss of pool to Methuselahs voting 'no' before it is played, as well as to Methuselahs voting 'no' after it is played. [RTR 19951110]"
-  - "Each Scorn played may only cause the loss of one pool to a given Methuselah, regardless of how may 'no' votes that Methuselah casts. [RTR 19951110]"
+  - May be played at any time during the voting process, and will retroactively cause the loss of pool to Methuselahs voting 'no' before it is played, as well as to Methuselahs voting 'no' after it is played. [RTR 19951110]
+  - Each Scorn played may only cause the loss of one pool to a given Methuselah, regardless of how may 'no' votes that Methuselah casts. [RTR 19951110]
 101693|Scorpion Sting:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
+  - "[ANI] Does not prevent the opponent from dodging, the dodge just has no effect. [LSJ 20030902-2] [LSJ 20060808-1]"
 101694|Scorpion's Touch:
-  - "If it is declared with first strike and if the opposing minion declared a strike based on strength, that minion’s strength is decreased by Scorpion’s Touch when it resolves. [PIB 20110830]"
-  - "You cannot play another strike card to serve as the hand strike for Scorpion's Touch. [LSJ 20010627]"
+  - If it is declared with first strike and if the opposing minion declared a strike based on strength, that minion’s strength is decreased by Scorpion’s Touch when it resolves. [PIB 20110830]
+  - You cannot play another strike card to serve as the hand strike for Scorpion's Touch. [LSJ 20010627]
 101697|Scourge of the Enochians:
-  - "If the option to burn a vampire is used, the card goes to the predator immediately, even if there is still a mandatory effect to resolve. If not, the predator must take the card when he has the opportunity to play an effect, after the acting Methusalah applied other mandatory effects (eg. losing blood to {Dragonbound}). [ANK 20200508-1]"
+  - If the option to burn a vampire is used, the card goes to the predator immediately, even if there is still a mandatory effect to resolve. If not, the predator must take the card when he has the opportunity to play an effect, after the acting Methuselah applied other mandatory effects (eg. losing blood to {Dragonbound}). [ANK 20200508-1]
+101701|Scry the Hearthstone:
+  - "[vis] The maneuver can only be used if the block is successful, and only in the resulting (block-induced) combat. It does not carry over to a follow-up combat (eg. [CEL] {Psyche!}). [LSJ 20010813] [LSJ 20010819-2]"
+  - "[vis] The maneuver is provided again if a second block happens on the same action (eg. after [PRO] {Form of Mist}). [LSJ 20010814-2]"
+  - '[VIS] Cards are not replaced during the "as played" window. [LSJ 20061013]'
+  - '[VIS] If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
 101702|Scrying of Secrets:
-  - 'Cards and effects that can be played "after resolution" (and only them) can be played after it. [ANK 20190425] [ANK 20190113]'
+  - Cards and effects that can be played "after resolution" (and only them) can be played after it. [ANK 20190425] [ANK 20190113]
 101703|Seal of Veddartha:
   - "Can be equipped by a vampire with capacity less than 6: he cannot use it to bleed but the disciplines bonus applies. [LSJ 20030607] [ANK 20180801]"
 "101706|Second Tradition: Domain":
-  - 'Can be used by a locked a vampire who is already attempting to block (eg. if he played a wake effect before)". [ANK 20181122-2]'
-  - "Cannot be used if the vampire cannot attempt to block the action (eg. {Daring the Dawn}). [LSJ 20010714-2]"
-  - "The block attempt and subsequent combat still happen if the action lacks a suitable target because of the unlock (eg. {Ambush}). [LSJ 20090514]"
+  - Can be used by a locked a vampire who is already attempting to block (eg. if he played a wake effect before)". [ANK 20181122-2]
+  - Cannot be used if the vampire cannot attempt to block the action (eg. {Daring the Dawn}). [LSJ 20010714-2]
+  - Does not ignore the normal prey, predator or target restrictions. [ANK 20180623]
+  - The block attempt and subsequent combat still happen if the action lacks a suitable target because of the unlock (eg. {Ambush}). [LSJ 20090514]
+  - The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {The Ankara Citadel, Turkey}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]
 101707|Secret Horde:
-  - "If put into play with no counters (X=0), it burns immediately. [LSJ 20070308]"
+  - If put into play with no counters (X=0), it burns immediately. [LSJ 20070308]
+101710|Secret Passage:
+  - When burned to make an action fail, the action has reached resolution, so is subject to NRA (Non Repeatable Action) rules. [ANK 20211015]
 101711|Secure Haven:
-  - "All Methuselahs, including the target vampire's controller, must pay one extra pool when playing Master cards on the target minion. [TOM 19951208-1]"
-  - "Adds one to the cost of the master card targetting the vampire, cost reductions from other effects do apply. [LSJ 20070829-1]"
+  - All Methuselahs, including the target vampire's controller, must pay one extra pool when playing Master cards on the target minion. [TOM 19951208-1]
+  - Adds one to the cost of the master card targetting the vampire, cost reductions from other effects do apply. [LSJ 20070829-1]
   - 'Choosing is targeting: cards that "choose" the vampire like {The Rack}, {Toreador Grand Ball}, {Piper} or {Tend the Flock} are considered to target it, their cost is increased. Actions that choose the vampire cannot be played against him (eg. {Propaganda}, {Spirit Marionette}, {Shattering Crescendo}) [LSJ 20031010] [LSJ 20090319] [ANK 20180907]'
-  - 'Actions that target retainers, equipment, or other cards on the minion are allowed, as are actions that target cards not on the minion, even if such cards have "named" or "chosen" that minion. [TOM 19951208-1] [LSJ 19980302-1]'
-  - "If contested, it will not be burned when the target (vampire) goes to torpor, nor will it be burned if it enters play while the target vampire is in torpor. [RTR 19960124]"
+  - Actions that target retainers, equipment, or other cards on the minion are allowed, as are actions that target cards not on the minion, even if such cards have "named" or "chosen" that minion. [TOM 19951208-1] [LSJ 19980302-1]
+  - If contested, it will not be burned when the target (vampire) goes to torpor, nor will it be burned if it enters play while the target vampire is in torpor. [RTR 19960124]
 101714|Selective Silence:
-  - "[QUI] no other effect can be used to reset the range, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]"
-  - "[QUI] The blood is not the cost of Selective Silence, it is the cost of using the mandatory range-setting effect. The cost is not reduced by cards reducing [qui] or combat cards cost, the card cannot be used by a vampire who has less than one blood. [LSJ 19970224]"
+  - "[QUI] No other effect can be used to reset the range, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]"
+  - "[QUI] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {The Path of Blood}). The card cannot be played if the minion cannot afford to burn the blood. [LSJ 19970224] [ANK 20210226]"
 101717|Sense the Savage Way:
   - "[ANI] Can be used by a vampire who is already attempting to block. [ANK 20181122-2]"
+  - "[ANI] Cannot be used if the vampire cannot attempt to block the action (eg. {Daring the Dawn}). [LSJ 20010714-2]"
+  - "[ANI] Does not ignore the normal prey, predator or target restrictions. [ANK 20180623]"
+  - "[ANI] The block attempt and subsequent combat still happen if the action lacks a suitable target because of the unlock (eg. {Ambush}). [LSJ 20090514]"
 101720|Sense Vitality:
   - "[val], [VAL] Is not the default action, no blood is paid for the rescue. [ANK 20181017]"
 101721|Sensory Deprivation:
-  - "Can target an unlocked minion, does not prevent a minion to wake or unlock in a non-normal way (eg. {Freak Drive}, {Sense the Savage Way}). [PIB 20150111]"
-  - "Once the vampire who played it leaves play, the effect stops. It does not kick back in if the vampire comes back (eg. after a {Banishment}). [PIB 20140107] [LSJ 20010807-2]"
+  - Can target an unlocked minion, does not prevent a minion to wake or unlock in a non-normal way (eg. {Freak Drive}, {Sense the Savage Way}). [PIB 20150111]
+  - Once the vampire who played it leaves play, the effect stops. It does not kick back in if the vampire comes back (eg. after a {Banishment}). [PIB 20140107] [LSJ 20010807-2]
 101724|Seraph's Second:
-  - "Can be used to unlock a vampire who has just successfully resolved an action to become Black Hand. [LSJ 20070702]"
+  - Can be used to unlock a vampire who has just successfully resolved an action to become Black Hand. [LSJ 20070702]
 101727|Serpent's Numbing Kiss:
   - "[PRE][SER] The additional effect takes place after the end of combat, including the blood burn. [RTR 19970630] [ANK 20180420-1] [ANK 20200705]"
   - '[PRE][SER] The "does not unlock as normal" effect is redundant with being infernal. If the minion is infernal, its controller can still pay a pool to unlock them. [LSJ 20050114]'
   - "[PRE][SER] If the combat continues or a new combat begins, no blood is burned, the card cannot be put on the opposing minion and he is not locked. [RTR 20020501] [ANK 20200705]"
   - "[PRE][SER] If the strike is dodged, the card is not put on the opposing minion and he is not locked. [RTR 20041202]"
   - "[PRE][SER] Burning 1 blood is mandatory, not a choice. [ANK 20180420-2]"
+  - "[PRE][SER] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {The Path of Typhon}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 101730|Set's Call:
-  - "Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
-  - "The acting vampire's controller is the one who makes the choices pertaining to the ally or retainer entry in play. [LSJ 20030701-2]"
+  - Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]
+  - The acting vampire's controller is the one who makes the choices pertaining to the ally or retainer entry in play. [LSJ 20030701-2]
 101731|Set's Curse:
-  - "Can be used on a target that cannot be burned (eg. {Ilomba}), but then it is not put into play. [ANK 20190422]"
-  - "Can be used on a target that is shuffled in library after it is burned (eg. {Kherebutu}), both effects are applied normally. [ANK 20200813]"
+  - Can be used on a target that cannot be burned (eg. {Ilomba}), but then it is not put into play. [ANK 20190422]
+  - Can be used on a target that is shuffled in library after it is burned (eg. {Kherebutu}), both effects are applied normally. [ANK 20200813]
+  - Once in play, is an ally with a cost of zero. [LSJ 20080804]
 101733|Shackles of Enkidu:
-  - "If placed on a minion that cannot have equipment or weapon, the Shackles are burned. [LSJ 19980831]"
+  - If placed on a minion that cannot have equipment or weapon, the Shackles are burned. [LSJ 19980831]
   - '"The shackled minion" refers to the minion the card is placed upon (not the Gangrel the card is put on with the equip action). [TOM 19951212-2]'
-  - "Once placed on a minion, even as a result of diablerie or theft, the Shackles will harm the minion they are on. [LSJ 19990602]"
-  - 'An ally does not suffer the "burn 2 blood" effect from being shackled. [RTR 19971201]'
-  - "Are controlled by the Methuselah who controls the vampire who used it; changing the controller of the vampire changes who controls the Shackles. (errata) [RTR 19960708]"
-  - 'Are still considered as an equipment after they are "activated". [LSJ 20100527]'
+  - Once placed on a minion, even as a result of diablerie or theft, the Shackles will harm the minion they are on. [LSJ 19990602]
+  - An ally does not suffer the "burn 2 blood" effect from being shackled. [RTR 19971201]
+  - Are controlled by the Methuselah who controls the vampire who used it; changing the controller of the vampire changes who controls the Shackles. (errata) [RTR 19960708]
+  - Are still considered as an equipment after they are "activated". [LSJ 20100527]
 101735|Shadow Body:
   - '[OBT] If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]'
-  - '[OBT] If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
+  - '[OBT] If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
   - '[OBT] An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]'
   - '[OBT] "continue as if unblocked" moves the action card from the ash heap (where it went when the action was blocked) to limbo (where it should be if the action is not blocked). If the action card is not in the ash heap, then the action cannot be continued. [LSJ 20070808-1]'
   - '[OBT] If the combat continues or a new combat occurs, the "action continues as if unblocked" effect is lost. [LSJ 19980109] [RTR 20020501]'
 101736|Shadow Boxing:
-  - 'If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]'
-  - 'If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
-  - 'An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]'
+  - If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]
+  - If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]
+  - An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]
   - '"continue as if unblocked" moves the action card from the ash heap (where it went when the action was blocked) to limbo (where it should be if the action is not blocked). If the action card is not in the ash heap, then the action cannot be continued. [LSJ 20070808-1]'
-  - "Cannot be used if a Slave locked to enter combat instead of the blocking minion. [ANK 20200114]"
+  - "[OBF][POT][ACTION MODIFIER] Cannot be used by a Slave that entered combat instead of the acting minion. [ANK 20200114]"
+  - "[OBF][POT][ACTION MODIFIER] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Adana de Sforza}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 101737|Shadow Court Satyr:
-  - "Cannot use an effect that requires two or more Disciplines. [LSJ 20021216]"
-  - "Can choose to use any single discipline effect of a split discipline card, each time he uses it. [LSJ 20021210-2]"
-  - "Can only use the combat card when he is in combat. [LSJ 20060502]"
-  - "If the card combat card is moved, the Satyr cannot use it as if played from your hand anymore, even if it was moved on him (eg. {Weighted Walking Stick}) [LSJ 20010716] [LSJ]"
-  - "The card on him cannot be canceled as it is played when he plays it as if from your hand. [LSJ 20010716]"
-  - "The card put on him is not into play. [ANK 20190629]"
-  - 'Only plays the card "as a vampire" if it costs blood or require a discipline: he cannot play {Taste of Vitae}. [LSJ 20000128]'
-  - "If he ends up in torpor (eg. by using {Reform Body}), he cannot leave or be rescued. Going into torpor instead of being burned does not give him life back: if he has no life, he burns again immediately. [LSJ 20000128]"
+  - Cannot use an effect that requires two or more Disciplines. [LSJ 20021216]
+  - Can choose to use any single discipline effect of a split discipline card, each time he uses it. [LSJ 20021210-2]
+  - Can only use the combat card when he is in combat. [LSJ 20060502]
+  - If the card combat card is moved, the Satyr cannot use it as if played from your hand anymore, even if it was moved on him (eg. {Weighted Walking Stick}) [LSJ 20010716]
+  - The card on him cannot be canceled as it is played when he plays it as if from your hand (eg. {Direct Intervention}), except if it is part of the card effect (eg. {Target Vitals}). [LSJ 20010716] [ANK 20221011]
+  - The card put on him is not into play. [ANK 20190629]
+  - He can play any card "as a vampire" even if it does not require a discipline (eg. {Taste of Vitae}). REVERSAL of previous rulings. [LSJ 20080717]
+  - He cannot use a card to commit diablerie (eg. {Amaranth}) [LSJ 20080717] [RTR 19970630]
+  - If a card he plays as a vampire sends him to torpor (eg. by using {Reform Body}), he burns. REVERSAL of previous rulings. [LSJ 20060409]
+  - If he takes aggravated damage from a card he plays as a vampire (eg. {Burst of Sunlight}), he loses one life but does not go to torpor. [LSJ 20060409]
 101738|Shadow Feint:
-  - "Will not prohibit the opposing minion from choosing dodge as his strike, and, if chosen, the dodge will still resolve. The dodge simply has no effect on the Shadow Feinted strike. [LSJ 20030902-2]"
+  - "[CEL][OBF] Does not prevent the opponent from dodging, the dodge just has no effect. [LSJ 20030902-2] [LSJ 20060808-1]"
 101741|Shadow of the Wolf:
-  - "The +1 damage only applies to the additional strike. [LSJ 19970331]"
+  - The +1 damage only applies to the additional strike. [LSJ 19970331]
   - "[PRO] The press can only be used during the current round. [TOM 19960521]"
 101744|Shadow Step:
   - "[OBT] No other effect can be used to reset the range afterwards, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]"
-  - "[OBT] The two blood are not the cost of Shadow Step, they are the cost of using the mandatory range-setting effect. The cost is not reduced by cards reducing [obt] or combat cards cost, the card cannot be used by a vampire who has less than two blood. [LSJ 19970224]"
+  - "[OBT] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {The Path of Night}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 101745|Shadow Strike:
   - "[OBT] The press can only be used during the current round. [TOM 19960521]"
+101746|Shadow Twin:
+  - "[OBT] has no additional effect on a retainer. [LSJ 20010303]"
 101751|Shambling Hordes:
-  - "The acting vampire's controller can choose not to remove a minion from his or her ash heap and thus burn the Shambling Hordes. [LSJ 20030701-2]"
-  - 'The damage the strike does is determined when the strike resolution begins, before the Hordes loses life from any opposing "burn life" or "steal life" effect. Damage done before strike resolution, e.g. with First Strike, will reduce the damage done by the Hordes. [LSJ 20030307]'
+  - The acting vampire's controller can choose not to remove a minion from his or her ash heap and thus burn the Shambling Hordes. [LSJ 20030701-2]
+  - The damage the strike does is determined when the strike resolution begins, before the Hordes loses life from any opposing "burn life" or "steal life" effect. Damage done before strike resolution, e.g. with First Strike, will reduce the damage done by the Hordes. [LSJ 20030307]
 101752|Shame:
-  - "Damage is environmental. [RTR 19970630]"
+  - Damage is environmental. [RTR 19970630]
 101758|Shattered Mirror:
-  - "The action ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20200207]"
+  - The action ends unsuccessfuly immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719] [ANK 20200207]
 101760|Shattering Blow:
-  - "Cannot be used if there is no equipment to destroy. [RTR 19980928]"
+  - Cannot be used if there is no equipment to destroy. [RTR 19980928]
+101761|Shattering Crescendo:
+  - "[mel], [MEL] Requires to have the second in hand to play it. [LSJ 20100208-2] [LSJ 20100823]"
 101765|Shepherd's Innocence:
-  - "[ANI] Is directed at all Methusalah controlling a card that require Animalism [ani]. [LSJ 20080809-1] [KOT 20081119]"
+  - "[ANI] Is directed at all Methuselah controlling a card that require Animalism [ani]. [LSJ 20080809-1] [KOT 20081119]"
   - "[ANI] Retainers and Equipments you control can also be rearranged. [LSJ 20080803-2] [LSJ 19981102]"
 101767|Shilmulo Tarot:
-  - "There is no limit to the number of cards it can store. [PIB 20110712-2]"
+  - There is no limit to the number of cards it can store. [PIB 20110712-2]
+  - If there is another copy in play, the cards are put on it before it enters contest. [ANK 20221028] [LSJ 20090428-1]
 101770|Shotgun Ritual:
   - "[THA] The press can only be used during the current round. [TOM 19960521]"
 101771|Shoulder Drop:
-  - "Is played and inflicts damage after the strikes have been resolved and inflicted damage, before any other pair of strikes and before the press step. [ANK 20171226]"
+  - Is played and inflicts damage after the strikes have been resolved and inflicted damage, before any other pair of strikes and before the press step. [ANK 20171226]
 101773|Shroud Mastery:
-  - '[NEC] Cards and effects that can be played "as the action is announced" (and only them) can be played before it. [ANK 20190425]'
+  - '[NEC] Cards and effects that are played "as the action is announced" must be played before playing "regular" action modifier or reaction cards. [ANK 20190425]'
+  - "[NEC] Replace the action card (if any) before playing it. [ANK 20181208]"
 101779|Sideslip:
   - "[CEL] Cannot be used if there is no damage to prevent. [LSJ 20001114]"
 101781|The Signet of King Saul:
   - "{Unleash Hell's Fury} cannot block the bearer. [ANK 20190501]"
 101783|Sins of the Cauchemar:
   - "[AUS] Can be played even if no block attempt is made, several minions can play it on the same action. [LSJ 19990611]"
 101784|Siphon:
-  - "Vampires with no blood can be chosen [RTR 20010711] [PIB 20110725]"
-  - "The cards are chosen when the action is successful, not as part of the terms of the action. [PIB 20110725]"
+  - Vampires with no blood can be chosen [RTR 20010711] [PIB 20110725]
+  - The cards are chosen when the action is successful, not as part of the terms of the action. [PIB 20110725]
   - "The Siphon card of the current action cannot be moved back in hand: it is in limbo (not in the ash heap) when resolving. [PIB 20110725]"
 101785|Sire's Index Finger:
-  - "Losing the use of the Finger won't make the vampire vulnerable to a previously-played Frenzy card, and gaining it won't render him immune to a previously-played Frenzy card. [LSJ 20040210]"
+  - Losing the use of the Finger won't make the vampire vulnerable to a previously-played Frenzy card, and gaining it won't render him immune to a previously-played Frenzy card. [LSJ 20040210]
 101786|Siren's Lure:
+  - "[cel] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Mitru the Hunter}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
   - "[mel] [MEL] Can only be played by the controller of the acting minion. [LSJ 19990425]"
   - "[mel] [MEL] Cannot be played to queue a second combat after a combat is already set up for later (e.g. by a previous Siren's Lure). [LSJ 20020125]"
   - "[mel] [MEL] Other effects that queue a combat cannot be used until the new combat begins. [LSJ 20021121]"
   - "[mel] [MEL] Combat does not occur if the action ends prematurely. [LSJ 20090826]"
   - "[mel] [MEL] The new combat is still part of the action (eg. {Heidelberg Castle, Germany} cannot be used between combats). [ANK 20170918-2]"
 101790|Skin of Night:
   - "[FOR] Cannot be used if there is no damage to prevent. [LSJ 20001114]"
 101791|Skin of Rock:
-  - "Cannot be used if there is no damage to prevent. [LSJ 20001114]"
-  - "Unused prevention does not carry over. [LSJ 20001114]"
+  - Cannot be used if there is no damage to prevent. [LSJ 20001114]
+  - Unused prevention does not carry over. [LSJ 20001114]
 101794|Skin of the Chameleon:
-  - '[tha] Cards and effects that can be played "as the action is announced" (and only them) can be played before it. [ANK 20190425]'
+  - '[tha] Cards and effects that are played "as the action is announced" must be played before playing "regular" action modifier or reaction cards. [ANK 20190425]'
+  - "[tha] Replace the action card (if any) before playing it. [ANK 20181208]"
 101797|Slake the Thirst:
-  - "If multiple effects make you gain blood, even due to a single card (eg. {Redistribution}), you choose on which effect to apply Slake the Thirst. [LJS 20100203]"
+  - If multiple effects make you gain blood, even due to a single card (eg. {Redistribution}), you choose on which effect to apply Slake the Thirst. [LJS 20100203]
   - "[san] Can be played multiple times on the same blood gain (eg. {Taste of Vitae}). [LSJ 20100206-2]"
-  - "Can be played after a diablerie, before the blood hunt. [ANK 20201228]"
+  - Can be played after a diablerie, before the blood hunt ([san] after {Amaranth}, [SAN] after a normal diablerie). [ANK 20201228]
+  - Can be played at any time blood is gained, including after action resolution (eg. {Games of Instinct}, {Perfectionist}). [LSJ 20100325]
 101798|Slam:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 101805|The Sleeping Mind:
   - "[DOM] Does not prevent wake effects to be played (eg. {Wake with Evening's Freshness}), but does prevent unlock after action resolution (eg. {Freak Drive} or [ani] {Cats' Guidance}). [PIB 20150703]"
 101806|Sleight of Hand:
-  - 'This is an "equip action" [TOM 19960130]'
+  - This is an "equip action" [TOM 19960130]
 101807|The Slow Withering:
-  - "The additional cost is paid at the same time the normal cost is paid. [ANK 20190625]"
-"101811|Smiling Jack, The Anarch":
-  - "Each other player must burn a pool or a vampire blood for each counter on Jack. Failing to burn a blood from an empty vampire will not lessen the obligation. [LSJ 19971212]"
-  - "Other Methusalah can pay with any combination of pool and different vampires to meet the total number of counters. [ANK 20181006]"
+  - The additional cost is paid at the same time the normal cost is paid. [ANK 20190625]
+101809|Smash and Grab:
+  - "[ani] If used on an ally and it burns as a result, this counts as a Ⓓ action burning an ally (eg. Trophies, {Predator's Transformation}). [ANK 20220507]"
+101811|Smiling Jack, The Anarch:
+  - Each other player must burn a pool or a vampire blood for each counter on Jack. Failing to burn a blood from an empty vampire will not lessen the obligation. [LSJ 19971212]
+  - Other Methuselah can pay with any combination of pool and different vampires to meet the total number of counters. [ANK 20181006]
+101813|Smoke and Mirrors:
+  - "[chi] The maneuver can only be used if the block is successful, and only in the resulting (block-induced) combat. It does not carry over to a follow-up combat (eg. [CEL] {Psyche!}). [LSJ 20010813] [LSJ 20010819-2]"
+  - "[chi] The maneuver is provided again if a second block happens on the same action (eg. after [PRO] {Form of Mist}). [LSJ 20010814-2]"
 101814|Smoke Grenade:
   - 'Still burns when used if the opponent uses a "strike: combat ends" too. It does not burn if combat ends before strike resolution (eg. {Rötschreck}). [LSJ 20001127-2] [LSJ 20010806-1]'
-  - "Still burns if the combat continues or a new combat begins. [RTR 20020501] [LSJ 20040601]"
+  - Still burns if the combat continues or a new combat begins. [RTR 20020501] [LSJ 20040602]
 101816|Sniper Rifle:
-  - "When setting the range for the round, no other effect can be used to reset the range, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]"
-  - "The bearer is not commited to use it if he or she uses another effect to set the range. [RTR 20020501]"
-  - "If a new combat occurs due to an effect like {Psyche!}, the Rifle can not be used to set the range. [LSJ 20010814]"
-  - "If a Slave locks to enter combat instead of a blocking minion, he cannot use the Rifle to set the range [ANK 20200115]"
-  - "The ability to set the range can only be used if the weapon was equipped when blocking (eg. not when using {Disguised Weapon} after the block). [LSJ 20021028]"
+  - When setting the range for the round, no other effect can be used to reset the range, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]
+  - The bearer is not commited to use it if he or she uses another effect to set the range. [RTR 20020501]
+  - If a new combat occurs due to an effect like {Psyche!}, the Rifle can not be used to set the range. [LSJ 20010814]
+  - If a Slave locks to enter combat instead of a blocked minion, the opponent cannot use the Rifle to set the range [ANK 20200115]
+  - The ability to set the range can only be used if the weapon was equipped when blocking (eg. not when using {Disguised Weapon} after the block). [LSJ 20021028]
 101817|Soak:
-  - "Cannot be used if there is no damage to prevent. [LSJ 20001114]"
-  - "Prevents up to 2 or 4 non-aggravated damage, it can prevent less. [RTR 20041202]"
-  - "Unused prevention does not carry over. [LSJ 20001114]"
+  - Cannot be used if there is no damage to prevent. [LSJ 20001114]
+  - Prevents up to 2 or 4 non-aggravated damage, it can prevent less. [RTR 20041202]
+  - Unused prevention does not carry over. [LSJ 20001114]
 101820|Social Ladder:
-  - "Can be played with no older vampire in the uncontrolled region, though the ready vampire would be removed and his blood lost. [LSJ 20041015]"
+  - Can be played with no older vampire in the uncontrolled region, though the ready vampire would be removed and his blood lost. [LSJ 20041015]
 101828|Songs of the Distant Vitae:
   - "[QUI] A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]"
 101829|Soul Burn:
-  - "If the opponent dodges this strike, his weapons are unaffected and do damage this round. [LSJ 20040928]"
-  - "A weapon strike done with first strike is unaffected (unless Soul Burn is used with first strike too). [LSJ 20040928]"
-  - "Does not protect the target from self-inflicted damage from a weapon. [LSJ 19980216]"
-  - "Only nullify the weapon damage when it resolves, an opponent can successfully use {Rötschreck} after declaring a strike with {Ivory Bow}. [ANK 20170519]"
+  - If the opponent dodges this strike, his weapons are unaffected and do damage this round. [LSJ 20040928]
+  - A weapon strike done with first strike is unaffected (unless Soul Burn is used with first strike too). [LSJ 20040928]
+  - Does not protect the target from self-inflicted damage from a weapon. [LSJ 19980216]
+  - Only nullify the weapon damage when it resolves, an opponent can successfully use {Rötschreck} after declaring a strike with {Ivory Bow}. [ANK 20170519]
+  - The opponent cannot play [for] prevention cards (eg. for cycling). [LSJ 20050628]
 101832|Soul Gem of Etrius:
-  - "If the new vampire is the same as the one who burned, he is still considered a new vampire for all purposes. (eg. he can bleed even if the previous version has already bled this turn) [LSJ 20100213]"
-  - "Functions even if the bearer (now burned) was prohibited from using equipments (eg. because of {Drawing out the Beast}). [LSJ 20010729]"
-  - "If the drawn vampire (B) is younger and would be put into play with Gem but is burned instead (self-contestinging, for example), then the Gem activates again, drawing a new vampire (C) and comparing his capacity to B's capacity. [RTR 20010710] [LSJ 20030918]"
-  - "Can grab an imbued. In that case, the imbued is either placed in the uncontrolled region or placed empty into the incapacitated region with the Gem, as determined by his starting life. [LSJ 20060323]"
-  - "Still produces its full effect if the new younger vampire cannoot use equipment (eg. {Beast, The Leatherface of Detroit}). [LSJ 20100527]"
+  - If the new vampire is the same as the one who burned, he is still considered a new vampire for all purposes. (eg. he can bleed even if the previous version has already bled this turn) [LSJ 20100213]
+  - "Does not trigger if the bearer is removed from the game (eg. {Golconda: Inner Peace}) [LSJ 20000113]"
+  - Functions even if the bearer (now burned) was prohibited from using equipments (eg. because of {Drawing Out the Beast}). [LSJ 20010729]
+  - If the drawn vampire (B) is younger and would be put into play with Gem but is burned instead (self-contestinging, for example), then the Gem activates again, drawing a new vampire (C) and comparing his capacity to B's capacity. [RTR 20010710] [LSJ 20030918]
+  - Can grab an imbued. In that case, the imbued is either placed in the uncontrolled region or placed empty into the incapacitated region with the Gem, as determined by his starting life. [LSJ 20060323]
+  - Still produces its full effect if the new younger vampire cannot use equipment (eg. {Beast, The Leatherface of Detroit}). [LSJ 20100527]
 101833|Soul of the Earth:
-  - "Only requires one clan or the other (Tremere or Tremere antitribu) to be played. [ANK 20190203]"
+  - Only requires one clan or the other (Tremere or Tremere antitribu) to be played. [ANK 20190203]
+  - Reduction applies to allies or retainers recruited in a non-normal way (eg. {Piper}). [ANK 20210928]
 101836|Soul Stealing:
   - "[COMBAT] If a minion is burned in combat, his opponent his always considered to have burned him. [LSJ 20090922]"
   - "[ACTION MODIFIER] If the minion is burned because of a referendum or as a side-effect of the action, this does not count as the acting minion burning him. (eg. {War Ghoul} when recruited, {Brigitte Gebauer} using her last life, {Kamiri wa Itherero}'s ability). [RTR 19960124] [LSJ 20090922] [ANK 20181022]"
   - "[ACTION MODIFIER] If played on a diablerie, can be played before or after getting a Discipline card (if any), but must be played before the Blood Hunt. [RTR 19991206]"
 101838|Sowing Dissension:
-  - "Is a Ⓓ action against all other Methusalahs [PIB 20150821] [RTR 20080808]"
+  - Is an action directed at all other Methuselahs [PIB 20150821] [RTR 20080808]
 101840|Speak with Spirits:
   - "[SPI] Can be used by a vampire who is already attempting to block. [ANK 20181122-2]"
 101841|Special Report:
-  - 'Can be used on a vampire who is already attempting to block". [ANK 20181122-2]'
+  - Can be used on a vampire who is already attempting to block". [ANK 20181122-2]
 101845|Spell of Life:
-  - 'The mummies put into play are unique by card name. The name is "in play" for anything that cares. They will contest unique minions of the same name, vampire or allies. If one is {Nefertiti}, then {Aabbt Kindred} will be able to take directed actions. [LSJ 20070928-2] [LSJ 20071001-2]'
+  - The copies you burn need not be ones you control. [LSJ 20090428]
+  - The mummies put into play are unique by card name. The name is "in play" for anything that cares. They contest unique minions of the same name, vampire or allies. If one is {Nefertiti}, then {Aabbt Kindred} will be able to take directed actions. [LSJ 20070928-2] [LSJ 20071001-2]
+  - The mummies do not contest non-unique vampires (eg. {Aabbt Kindred}), but two mummies made of the same non-unique vampire contest one another. [LSJ 20070928-2]
+  - If one of the mummy is burned, the card goes to the ash heap where it counts as a vampire (eg. {Possession} can be used, but not {Compel the Spirit}). [LSJ 20071014]
+  - The mummies are not affected by {Wormwood}. [LSJ 20100716]
 101847|Spirit Claws:
   - "[pro] Must be played before strike resolution (and damage prevention) in order to affect the current strike [RTR 19960112]"
   - "[SPI][PRO] The [pro] and [spi][pro] versions do not contest with it. [ANK 20180630]"
 101848|Spirit Marionette:
   - "[OBE] Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
   - "[OBE] The mandatory bleed action must be performed before any non-mandatory actions. [LSJ 20011216-2]"
+  - "[OBE] The mandatory bleed can be performed by playing a card (eg. {Computer Hacking}). [LSJ 20021121-2]"
   - "[OBE] If the bleed is canceled, the vampire still returns to its original controller. [RTR 20020501]"
   - '[OBE] "After resolution" effects are applied before the target vampire is returned to his or her previous controller. [LSJ 20030219]'
-  - "[OBE] The action has no effect if the target is not unlocked anymore when it resolves. It is still considered successful and must be paid. [ANK 20181121]"
-  - "[OBE] The minion is removed from the game when he should return to a Methusalah who has been ousted. [ANK 20181110]"
+  - "[OBE] The action has no effect if the target is not unlocked anymore when it resolves. It is still considered successful and must be paid. [ANK 20181121] [LSJ 20021122-3]"
+  - "[OBE] The minion is removed from the game when he should return to a Methuselah who has been ousted. [ANK 20181110]"
+101850|Spirit's Touch:
+  - "[AUS] The maneuver can only be used if the block is successful, and only in the resulting (block-induced) combat. It does not carry over to a follow-up combat (eg. [CEL] {Psyche!}). [LSJ 20010813] [LSJ 20010819-2]"
+  - "[AUS] The maneuver is provided again if a second block happens on the same action (eg. after [PRO] {Form of Mist}). [LSJ 20010814-2]"
 101853|Spiritual Protector:
-  - "Does not restrict the opposing minion if no block occurred. [TOM 19951208-2]"
-  - "Does not restrict the ability of retainers to use equipment. [RTR 19960112]"
+  - Does not restrict the opposing minion if no block occurred. [TOM 19951208-2]
+  - Does not restrict the ability of retainers to use equipment. [RTR 19960112]
 101857|Spying Mission:
-  - "Is played if you know the bleed is successful, after you would normally play reactions and action modifiers. [TOM 19960226-2]"
-  - 'No reaction can be played afterwards to make the bleed unsuccessful and "beat" the Spying Mission. [TOM 19960303] [TOM 19960226-2]'
-  - "Once in play, it must be burned on the next successful bleed against the same Methuselah, it cannot be used to increase an unsuccesful bleed of zero. [TOM 19950620]"
-  - "The bleed it is played on is considered unsuccessful. Previous Spying Missions won't trigger during that action. [RTR 19960530]"
-  - "{Archon Investigation} cannot be played after a Spying Mission is burned for +2 bleed, since the bleed is already resolved at that point. [LSJ 19980105]"
-  - '{Mask of a Thousand Faces} cannot be played after playing a superior Spying Mission because Spying Mission is played "when the action resolves". [LSJ 19980105]'
-  - "Is played when a bleed would be successful, before resolution. [LSJ 20110502]"
+  - Is played if you know the bleed is successful, after you would normally play reactions and action modifiers. [TOM 19960226-2]
+  - No reaction can be played afterwards to make the bleed unsuccessful and "beat" the Spying Mission. [TOM 19960303] [TOM 19960226-2]
+  - Once in play, it must be burned on the next successful bleed against the same Methuselah, it cannot be used to increase an unsuccesful bleed of zero. [TOM 19950620]
+  - The bleed it is played on is considered unsuccessful. Previous Spying Missions won't trigger during that action. [RTR 19960530]
+  - "{Archon Investigation} cannot be played after a Spying Mission is burned for +2 bleed, since the bleed is about to resolve at that point. [LSJ 19980105]"
+  - '{Mask of a Thousand Faces} cannot be played after playing a superior Spying Mission because Spying Mission is played "when the action would resolve". [LSJ 19980105]'
+  - Is played when a bleed would be successful, before resolution. [LSJ 20110502]
+  - If it is cancelled (eg. {Direct Intervention}), it is too late for the target to play reactions. If the cost of the cancellation ousts a player, handle the oust before resolving the bleed. [LSJ 20050607] [LSJ 20050608]
 101858|Squirrel Balance:
-  - '[cel] Cards and effects that can be played "as the action is announced" (and only them) can be played before it. [ANK 20190425]'
-  - "If another effect also sets the range, the first to resolve has priority (eg. {Asanbonsam Ghoul} and {Neutral Guard} resolve after). [PIB 20120214]"
+  - '[cel] Cards and effects that are played "as the action is announced" must be played before playing "regular" action modifier or reaction cards. [ANK 20190425]'
+  - "[cel] Replace the action card (if any) before playing it. [ANK 20181208]"
+  - If another effect also sets the range, the first to resolve has priority (eg. {Asanbonsam Ghoul} and {Neutral Guard} resolve after). [PIB 20120214]
 101860|Starshell Grenade Launcher:
-  - "Using the Launcher to reduce stealth does not force the minion to strike with it if he blocks. [LSJ 19971215]"
+  - Using the Launcher to reduce stealth does not force the minion to strike with it if he blocks. [LSJ 19971215]
 101861|Starvation of Marena:
-  - "The press can only be used during the current round. [TOM 19960521]"
+  - The press can only be used during the current round. [TOM 19960521]
 101862|Static Virtue:
   - "For a Laibon moved into the ready region in the last influence phase, you must retrieve Aye and Orun in pairs: the same number of Aye as Orun. [LSJ 20051127]"
 101869|Steely Tenacity:
   - "[ani] [COMBAT] Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
   - "[ani] [COMBAT] The press can only be used during the current round. [TOM 19960521]"
   - "[dom], [qui] [ACTION] Is not replaced if the action is blocked: it is replaced when the action ends, after all combats. [LSJ 20001120]"
 101872|Stolen Police Cruiser:
-  - "Can be equipped by a non-Anarch and would count as a vehicle, although the rest of his effect does not apply. [LSJ 20030607]"
-  - "Equipping it does not count as an action requiring an Anarch (eg. for {CrimethInc.}). [ANK 20170918]"
+  - Can be equipped by a non-Anarch and would count as a vehicle, although the rest of his effect does not apply. [LSJ 20030607]
+  - Equipping it does not count as an action requiring an Anarch (eg. for {CrimethInc.}). [ANK 20170918]
+101875|Stone Travel:
+  - "[obt] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {The Path of Night}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 101876|Stonestrength:
-  - "Unused prevention does not carry over. [LSJ 20001114]"
+  - Unused prevention does not carry over. [LSJ 20001114]
   - "[VIS] Cannot be used if there is no damage to prevent. [LSJ 20001114]"
 101877|Storage Annex:
-  - "If it is stolen, the card on it goes with it and the new controller will be able to take it in hand. The card is returned to the owner's ash heap or library if it would be moved to an ash heap or library. [LSJ 20001031] [PIB 20121220]"
-  - "Cannot be played if it is the only card in your hand. [LSJ 20100527]"
-  - "The card on it goes to the controller's hand, regardless of where the new card comes from (eg. {Agaitas, The Scholar of Antiquities} face-up cards). [PIB 20150224]"
+  - If it is stolen, the card on it goes with it and the new controller will be able to take it in hand. The card is returned to the owner's ash heap or library if it would be moved to an ash heap or library. [LSJ 20001031] [PIB 20121220]
+  - Cannot be played if it is the only card in your hand. [LSJ 20100527]
+  - The card on it goes to the controller's hand, regardless of where the new card comes from (eg. {Agaitas, The Scholar of Antiquities} face-up cards). [PIB 20150224]
 101878|Storm Sewers:
-  - "If another effect also sets the range, the first to resolve has priority. [PIB 20120214]"
+  - If another effect also sets the range, the first to resolve has priority. [PIB 20120214]
 101879|Strained Vitae Supply:
-  - "The effect only applies to the default hunt action provided by the rulebook. [PIB 20120204]"
+  - The effect only applies to the default hunt action provided by the rulebook. [PIB 20120204]
 101881|The Stranger Among Us:
-  - "Shuffle your crypt afterwards. [LSJ 20020304-1]"
+  - Shuffle your crypt afterwards. [LSJ 20020304-1]
 101882|Street Cred:
-  - "Must be played after the presses are handled and can be played if the round ends prematurely. [RTR 20030519]"
-  - 'Can be played before or after effects that are played at the end of the round or "when the combat would end" (eg. [AUS] {Telepathic Tracking}). Can be played after [CEL] {Psyche!} [LSJ 20021113] [ANK 20191219] [ANK 20180910-1]'
+  - Must be played after the presses are handled and can be played if the round ends prematurely. [RTR 20030519]
+  - Can be played before or after effects that are played at the end of the round or "when the combat would end" (eg. [AUS] {Telepathic Tracking}). Can be played after [CEL] {Psyche!} [LSJ 20021113] [ANK 20191219] [ANK 20180910-1]
 101885|Strike at the True Flesh:
   - "[QUI] The additional damage is the same type as the strike's damage. [TOM 19960225] [RTR 19970630]"
 101886|Strike with Conviction:
-  - "If the action to bleed is blocked or canceled, Strike with Conviction is not burned. [LSJ 20060421] [RTR 20111202]"
+  - If the action to bleed is blocked or canceled, Strike with Conviction is not burned. [LSJ 20060421] [RTR 20111202]
 101887|Strix:
   - '[STR] The bleed is considered successful and the Edge gained. The action is resolved before entering combat, effects happening "after action resolution" happen after combat. [ANK 20200221]'
-  - "The burn option can be used if all your vampires with [str] are in torpor. [LSJ 20091203]"
+  - The burn option can be used if all your vampires with [str] are in torpor. [LSJ 20091203]
 101888|Stunt Cycle:
   - "[POT] Prevents up to 2 damage, it can prevent less. [RTR 20041202]"
 101889|Stutter-Step:
-  - "It is both a hand strike and a dodge. It cannot be used if only hand strikes or only dodges are allowed. [LSJ 20010919]"
-  - "The dodge part protects from the opponent's strike (even if done with First Strike), the hand strike part inflicts damage during the normal strike resolution. [ANK 20180913-1]"
+  - It is both a hand strike and a dodge. It cannot be used if only hand strikes or only dodges are allowed. [LSJ 20010919]
+  - The dodge part protects from the opponent's strike (even if done with First Strike), the hand strike part inflicts damage during the normal strike resolution. [ANK 20180913-1]
 101892|Succubus:
-  - "Can use her action on a vampire with no blood. [RTR 20010711]"
+  - Can use her action on a vampire with no blood. [RTR 20010711]
+  - If she steals a life from an ally and it burns, this counts as a Ⓓ action burning an ally (eg. for Trophies). [ANK 20220507]
 101894|Succulent Vitae:
   - "[QUI] The hunt bonus applies to non-standard hunt actions, blood comes from the target of the hunt. [RTR 20030519] [RTR 20180511]"
-  - "A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]"
+  - A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]
 101895|Sudario Refraction:
-  - "The chosen cards are named when the action is declared. The current Sudario cannot be part of them. [LSJ 20050422] [LSJ 20090722]"
-  - "Any copy of the named card can be fetched upon resolution. [LSJ 20090722]"
-  - "If no copy of a named card is in the ash heap upon resolution (eg. {The Erciyes Fragments} was used to take it), the effect still resolves for the other copies and the acting Methusalah discards 3 cards. [LSJ 20090722]"
+  - The chosen cards are named when the action is declared. The current Sudario cannot be part of them. [LSJ 20050422] [LSJ 20090722]
+  - Any copy of the named card can be fetched upon resolution. [LSJ 20090722]
+  - If no copy of a named card is in the ash heap upon resolution (eg. {The Erciyes Fragments} was used to take it), the effect still resolves for the other copies and the acting Methuselah discards 3 cards. [LSJ 20090722]
+  - If the library is empty and the hand is not full, you draw the returned cards up to hand size before discarding at random. [LSJ 20080612-2]
 101896|Sudden Reversal:
-  - "Can only cancel master cards that are played from the hand in the normal fashion. [RTR 20001020]"
-  - "If used to cancel a Trifle, the target does not get an extra Master Phase Action from the canceled Trifle. [LSJ 20090126] [RBK 20181001-162]"
+  - Can only cancel master cards that are played from the hand in the normal fashion. [RTR 20001020]
+  - If used to cancel a Trifle, the target does not get an extra Master Phase Action from the canceled Trifle. [LSJ 20090126] [RBK 20200701-5]
 101897|Summon History:
-  - "Requirements do not apply. If the card is an ally, it can act this turn. [LSJ 20100204]"
-  - "You must decide the value of X (blood cost) when playing the card. [LSJ 20100314]"
+  - Requirements do not apply. If the card is an ally, it can act this turn. [LSJ 20100204]
+  - You must decide the value of X (blood cost) when playing the card. [LSJ 20100314]
+  - If used to fetch a card with a variable cost of X, X is zero (eg. {Reanimated Corpse}), whatever cost was announced and paid for Summon History. [PIB 20111101]
 101898|Summon Soul:
   - "[NEC] Is removed from play as part of the resolution, it cannot be retrieved by {Shroudsight}. [ANK 20170331]"
 101902|The Summoning:
   - "[PRE] Is not the same action as the recruitment of the ally. You could perform both actions in the same turn with the same vampire. [PIB 20110915-2]"
-"101904|Sunset Strip, Hollywood":
-  - 'The "lock to reduce the cost" effect can be used when the action is announced or when the cost is paid. [LSJ 20090705]'
+  - "[PRE] The requirements and cost of the ally do not count as requirements nor cost for the action (eg. you cannot use {CrimethInc.} even if the ally requires an Anarch). [LSJ 20100725]"
+  - "[PRE] When used to recruit an ally, the ally cannot act this turn. [LSJ 20080630] [RTR 20180303]"
+  - '[PRE] The ally card is not "played" by the vampire (eg. {Louhi}''s ability cannot cancel it). [ANK 20201229]'
+101904|Sunset Strip, Hollywood:
+  - The "lock to reduce the cost" effect can be used when the action is announced or when the cost is paid. [LSJ 20090705]
+  - "Allows to play a card that could otherwise not be aforded: in this case it must be locked when the action is announced. [LSJ 20030917] [LSJ 20090705]"
 101906|Supernatural Resistance:
-  - "If used to cancel the opposing minion's strike, that minion must still choose a strike and could play the same one again. [LSJ 20090818]"
-  - 'If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
+  - If used to cancel the opposing minion's strike, that minion must still choose a strike and could play the same one again. [LSJ 20090818]
 101907|Suppressing Fire:
-  - "Can only be played by the controller of the acting minion. [LSJ 19990425]"
-  - "Multiple copies can be played by different minions on the same action. [ANK 20200515]"
+  - Can only be played by the controller of the acting minion. [LSJ 19990425]
+  - Multiple copies can be played by different minions on the same action. [ANK 20200515]
 101908|Surge:
   - "[REACTION] Can be used only when reactions can be used (unlocked or with a wake effect). It does not count as playing a reaction card. [LSJ 20070403] [LSJ 20070413]"
 101910|Survivalist:
-  - "He can lock to use his ability the turn he is recruited. [ANK 20180517]"
+  - He can lock to use his ability the turn he is recruited. [ANK 20180517]
 101914|Swarm:
-  - 'If grabbed by a "this vampire employs" effect (not the normal employ action), the vampire receiving the Swarm does not get to move the Swarm on to a new target. [LSJ 20051121]'
-  - "If the action to employ the Swarm is blocked, the Swarm goes on the acting minion immediately, before combat, if any. [LSJ 20090601]"
+  - If grabbed by a "this vampire employs" effect (not the normal employ action), the vampire receiving the Swarm does not get to move the Swarm on to a new target. [LSJ 20051121]
+  - If the action to employ the Swarm is blocked, the Swarm goes on the acting minion immediately, before combat, if any. [LSJ 20090601]
 101919|Sword of Judgment:
-  - "You get the additional strike even if you don't use the weapon's strike [LSJ 20030213-2]"
+  - You get the additional strike even if you don't use the weapon's strike [LSJ 20030213-2]
 101920|Sword of Nuln:
-  - "If the target has only one blood left, he pays what he can, still fails to heal the damage and goes to torpor empty. [LSJ 20090901] [LSJ 20030522-2]"
-  - "Aggravated damage are not healed by default, so they are not doubled. If the target can heal them (eg. {Repair the Undead Flesh}), he must pay double. [LSJ 20031219] [LSJ 20100527]"
-  - "If the wielder uses {Taste of Vitae}, he gains as much blood as the opponent has lost. [PIB 20130415]"
+  - If the target has only one blood left, he pays what he can, still fails to heal the damage and goes to torpor empty. [LSJ 20090901] [LSJ 20030522-2]
+  - Aggravated damage are not healed by default, so they are not doubled. If the target can heal them (eg. {Repair the Undead Flesh}), he must pay double. [LSJ 20031219] [LSJ 20100527]
+  - If the wielder uses {Taste of Vitae}, he gains as much blood as the opponent has lost. [PIB 20130415]
 101921|Sword of the Righteous:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 101925|Tainted Spring:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 101926|Tainted Vitae:
-  - "A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]"
+  - A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]
 "101928|Taking the Skin: Minion":
   - "[abo] [COMBAT] If a minion is burned in combat, his opponent his always considered to have burned him. [LSJ 20090922]"
-  - "[abo] [ACTION MODIFIER] If the minion is burned because of a referendum or as a side-effect of the action, this does not count as the acting minion burning him. (eg. {War Ghoul} when recruited, {Brigitte Gebauer} using her last life, {Kamiri wa Itherero}'s ability). [RTR 19960124] [LSJ 20090922] [ANK 20181022]"
+  - "[abo] [ACTION MODIFIER] If the minion is burned because of a referendum or as a side-effect of the action, this does not count as the acting minion burning him. (eg. {War Ghoul} when recruited, {Brigitte Gebauer} using her last life, {Kamiri wa Itherero}'s ability, {Blood Brother Ambush}). [RTR 19960124] [LSJ 20090922] [ANK 20181022] [ANK 20220916]"
   - "[abo] [ACTION MODIFIER] If played on a diablerie, can be played before or after getting a Discipline card (if any), but must be played before the Blood Hunt. [RTR 19991206]"
-"101930|Talaq, The Immortal":
-  - "While he can play cards that require [qui] or [tha], he does not actually have those Disciplines. He does not benefit from {Tremere Convocation}, for example. [LSJ 19980303]"
+101930|Talaq, The Immortal:
+  - While he can play cards that require [qui] or [tha], he does not actually have those Disciplines. He does not benefit from {Tremere Convocation}, for example. [LSJ 19980303]
 101931|Talbot's Chainsaw:
-  - "The press is mandatory. [LSJ 19980823]"
-  - "Using the Chainsaw action to enter combat or preventing damage with it does not force the minion to strike with it. [LSJ 19971215]"
-  - "The damage inflicted during the unlock phase is weapon damage, it is neither inflicted by the wearer nor environmental. {Mictlantecuhtli} can be chosen and would take no damage. [LSJ 20090304-1] [LSJ 20100514]"
+  - The press is mandatory. [LSJ 19980823]
+  - Using the Chainsaw action to enter combat or preventing damage with it does not force the minion to strike with it. [LSJ 19971215]
+  - The damage inflicted during the unlock phase is weapon damage, it is neither inflicted by the wearer nor environmental. {Mictlantecuhtli} can be chosen and would take no damage. [LSJ 20090304-1] [LSJ 20100514]
 101932|Talith:
   - 'The "strike: destroy weapon" cannot be chosen if there is no weapon to destroy. [RTR 19980928]'
 101934|Taming the Beast:
   - "[abo] Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
 101935|Tangle Atropos' Hand:
   - "No reaction or modifier can be played afterwards: the action ends immediately. [RTR 20180719]"
-  - "The action has not reached resolution. The same vampire can undertake the same action again, but not if it was blocked then continued before (eg. [PRO] {Form of Mist}). [LSJ 20070709] [LSJ 20090220] [ANK 20210124]"
-  - "The action was still taken (eg. counts against {Enkil Cog} or [OBF] {Veil the Legion}). [ANK 20210124]"
+  - The action has not reached resolution. The same vampire can undertake the same action again, but not if it was blocked then continued before (eg. [PRO] {Form of Mist}). [LSJ 20070709] [LSJ 20090220] [ANK 20210124]
+  - The action was still taken (eg. counts against {Enkil Cog} or [OBF] {Veil the Legions}). [ANK 20210124]
 101938|Target Hand:
-  - "Is played during the Strike phase (6.4.3) even if you commit to a strike in the Determine Range phase (6.4.2) (eg. {Thrown Gate}). Cannot be played if the strike cannot be chosen anymore during the Strike phase (eg. {Immortal Grapple}). [LSJ 20080409]"
-  - "If it is canceled, any blood cost (eg. {Terror Frenzy}) has to be paid. [PIB 20121031]"
+  - Is played during the Strike phase even if you commit to a strike in the Determine Range phase (eg. {Thrown Gate}). Cannot be played if the strike cannot be chosen anymore during the Strike phase (eg. {Immortal Grapple}). [LSJ 20080409]
+  - If it is canceled, any blood cost (eg. {Terror Frenzy}) has to be paid. [PIB 20121031]
 101939|Target Head:
-  - "Is played during the Strike phase (6.4.3) even if you commit to a strike in the Determine Range phase (6.4.2) (eg. {Thrown Gate}). Cannot be played if the strike cannot be chosen anymore during the Strike phase (eg. {Immortal Grapple}). [LSJ 20080409]"
-  - "When setting the range for the round, no other effect can be used to reset the range. Skip the determine range step on that round, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]"
-  - "The additional damage is the same type as the strike's damage. [RTR 19970630]"
-  - "If it is canceled, any blood cost (eg. {Terror Frenzy}) has to be paid. [PIB 20121031]"
+  - Is played during the Strike phase even if you commit to a strike in the Determine Range phase (eg. {Thrown Gate}). Cannot be played if the strike cannot be chosen anymore during the Strike phase (eg. {Immortal Grapple}). [LSJ 20080409]
+  - When setting the range for the round, no other effect can be used to reset the range. Skip the determine range step on that round, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]
+  - The additional damage is the same type as the strike's damage. [RTR 19970630]
+  - If it is canceled, any blood cost (eg. {Terror Frenzy}) has to be paid. [PIB 20121031]
 101940|Target Leg:
-  - "Is played during the Strike phase (6.4.3) even if you commit to a strike in the Determine Range phase (6.4.2) (eg. {Thrown Gate}). Cannot be played if the strike cannot be chosen anymore during the Strike phase (eg. {Immortal Grapple}). [LSJ 20080409]"
-  - "If it is canceled, any blood cost (eg. {Terror Frenzy}) has to be paid. [PIB 20121031]"
+  - Is played during the Strike phase even if you commit to a strike in the Determine Range phase (eg. {Thrown Gate}). Cannot be played if the strike cannot be chosen anymore during the Strike phase (eg. {Immortal Grapple}). [LSJ 20080409]
+  - If it is canceled, any blood cost (eg. {Terror Frenzy}) has to be paid. [PIB 20121031]
 101941|Target Retainer:
-  - "Is played during the Strike phase (6.4.3) even if you commit to a strike in the Determine Range phase (6.4.2) (eg. {Thrown Gate}). Cannot be played if the strike cannot be chosen anymore during the Strike phase (eg. {Immortal Grapple}). [LSJ 20080409]"
-  - "If it is canceled, the strike resolves with the default target. [ANK 20200311]"
-  - "If it is canceled, any blood cost (eg. {Terror Frenzy}) has to be paid. [PIB 20121031]"
+  - Is played during the Strike phase even if you commit to a strike in the Determine Range phase (eg. {Thrown Gate}). Cannot be played if the strike cannot be chosen anymore during the Strike phase (eg. {Immortal Grapple}). [LSJ 20080409]
+  - If it is canceled, the strike resolves with the default target. [ANK 20200311]
+  - If it is canceled, any blood cost (eg. {Terror Frenzy}) has to be paid. [PIB 20121031]
 101942|Target Vitals:
-  - "Is played during the Strike phase (6.4.3) even if you commit to a strike in the Determine Range phase (6.4.2) (eg. {Thrown Gate}). Cannot be played if the strike cannot be chosen anymore during the Strike phase (eg. {Immortal Grapple}). [LSJ 20080409]"
-  - "The additional damage is the same type as the strike's damage. [RTR 19970630]"
-  - "If it is canceled, any blood cost (eg. {Terror Frenzy}) has to be paid. [PIB 20121031]"
-  - "Can be played on a dodge or a combat ends, but does not add damage in that case. [PIB 20130319]"
+  - Is played during the Strike phase even if you commit to a strike in the Determine Range phase (eg. {Thrown Gate}). Cannot be played if the strike cannot be chosen anymore during the Strike phase (eg. {Immortal Grapple}). [LSJ 20080409]
+  - The additional damage is the same type as the strike's damage. [RTR 19970630]
+  - If it is canceled, any blood cost (eg. {Terror Frenzy}) has to be paid. [PIB 20121031]
+  - Can be played on a dodge or a combat ends, but does not add damage in that case. [PIB 20130319]
 101945|Taste of Vitae:
-  - "Must be played after the presses are handled and can be played if the round ends prematurely. [RTR 20030519]"
-  - 'Can be played before or after effects that are played at the end of the round or "when the combat would end" (eg. [AUS] {Telepathic Tracking}). Can be played after [CEL] {Psyche!} [LSJ 20021113] [ANK 20191219] [ANK 20180910-1]'
-  - "Can be played if the opponent was burned. [LSJ 20031201-2]"
+  - Cannot be played against an ally. [PIB 20121028]
+  - Must be played after the presses are handled and can be played if the round ends prematurely. [RTR 20030519]
+  - Can be played before or after effects that are played at the end of the round or "when the combat would end" (eg. [AUS] {Telepathic Tracking}). Can be played after [CEL] {Psyche!} [LSJ 20021113] [ANK 20191219] [ANK 20180910-1]
+  - Can be played if the opponent was burned. [LSJ 20031201-2]
 101946|Tattoo Signal:
-  - "The burn option can be used if all your Seraph are in torpor. [LSJ 20091203]"
+  - The burn option can be used if all your Seraph are in torpor. [LSJ 20091203]
+  - You cannot use the burn option if you have a ready Seraph, even if they already have a Tattoo Signal. [LSJ 20070410]
 101947|Taunt the Caged Beast:
   - "[ANI] The prey goes first in the combat (for declaring maneuvers, strikes, presses). [LSJ 20070319]"
 101948|Telepathic Counter:
-  - "Must be played before the bleed can be considered successful (eg. before [OBF] {Spying Mission}), but can be played before or after block attempts. [TOM 19960303] [LSJ 20061212]"
+  - Must be played before the bleed can be considered successful (eg. before [OBF] {Spying Mission}), but can be played before or after block attempts. [TOM 19960303] [LSJ 20061212]
 101949|Telepathic Misdirection:
   - '[AUS] Must be played before action resolution, ie. before any modifier or reaction played "as the action/bleed would be successful" are played. It cannot be played after a {Spying Mission} on the vampire triggers. [LSJ 19980105]'
+  - "[AUS] Can be played when failing to block because of stealth: it is still declining to block. [ANK 20211003]"
 101950|Telepathic Tracking:
   - "[AUS] Effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]"
   - "[AUS] Cannot be played after [CEL] {Psyche!}. When played before, combat continues and {Psyche!} can only be played at the end of it. [ANK 20191219]"
   - '[AUS] Must be played after presses, can be played if the round ends prematurely and can be played before or after effects that are played "at then of the round" (eg. {Taste of Vitae}). [LSJ 20021113] [RTR 20030519] [ANK 20180910-1]'
+  - '[AUS] Can be played before of after effects that are played "at the end of combat". [LSJ 20021113] [ANK 20191219] [ANK 20180910-1]'
 101951|Telepathic Vote Counting:
-  - "May be played before, during, or after votes and ballots have been cast. [LSJ 19980130]"
+  - May be played before, during, or after votes and ballots have been cast. [LSJ 19980130]
 101952|Templar:
-  - "Multiple Templar cards provide different actions: if the vampire manage to unlock during the minion phase, he can perform the two actions. [RTR 20030519]"
+  - "Each copy of this card provides its own action: if the vampire manage to unlock during the minion phase, he can perform the action more than once (once per copy). [RTR 20030519]"
 101954|Temptation:
-  - "If used to steal a vampire in combat, combat ends. Any damage yet to resolve still resolves before the change of control. [LSJ 20020618]"
-  - "The stolen minion is removed from the game when he should return to a Methusalah who has been ousted. [ANK 20181110]"
-  - "The stolen minion returns to his previous controller even if he is in torpor (but stays in torpor). [LSJ 20010119]"
-  - "If played on one of your own vampires, the action is undirected. Its effect can be used to unlock the vampire. [LSJ 20010828] [ANK 20180917]"
+  - If used to steal a vampire in combat, combat ends. Any damage yet to resolve still resolves before the change of control. [LSJ 20020618]
+  - The stolen minion is removed from the game when he should return to a Methuselah who has been ousted. [ANK 20181110]
+  - The stolen minion returns to his previous controller even if he is in torpor (but stays in torpor). [LSJ 20010119]
+  - If played on one of your own vampires, the action is undirected. Its effect can be used to unlock the vampire. [LSJ 20010828] [ANK 20180917]
   - "Multiple Temptations on the same minion are handled separately: effects do not stask, stealing the minion only burns the counters on one of them. [LSJ 20010227]"
   - "No effect can be used between the decision to burn the counters and the moment the vampire changes control: the effect is resolved at once. (eg. {Shalmath} cannot untap). [PIB 20121028]"
-  - "If used to steal a minion attempting to block, the block attempt fails. [LSJ 20080326]"
-  - "If used to steal a minion targeted by an action, the action continues with the same target. Methusalahs who declined to block do not get another opportunity. If the target is not legal anymore (eg. [DOM] {Slaughtering the Herd}), the action ends with no effect. [LSJ 20020725]"
-  - "If used to steal a minion during an action, Methusalahs who declined to block are still declining to block. The new controller, if he is eligible and has not declined to block yet, can block with the stolen minion even if the previous controller has declined to block. [PIB 20150501]"
+  - If used to steal a minion attempting to block, the block attempt fails. [LSJ 20080326]
+  - If used to steal a minion targeted by an action, the action continues with the same target. Methuselahs who declined to block do not get another opportunity. If the target is not legal anymore (eg. [DOM] {Slaughtering the Herd}), the action ends with no effect. [LSJ 20020725]
+  - If used to steal a minion during an action, Methuselahs who declined to block are still declining to block. The new controller, if he is eligible and has not declined to block yet, can block with the stolen minion even if the previous controller has declined to block. [PIB 20150501]
 101956|Tend the Flock:
-  - "The blood comes from the blood bank. [ANK 20190511]"
+  - The blood comes from the blood bank. [ANK 20190511]
 101957|Tenebrous Form:
   - "[OBT] A minion previously attempting to block can resign his attempt and pay no blood. [LSJ 20031121-2]"
   - "[OBT] An ally has life, not blood, he cannot pay. [LSJ 20050216] [ANK 20190701]"
+101958|Tension in the Ranks:
+  - Pool is not paid when an imbued is incapacitated. [LSJ 20060409-2]
 101960|Terror Frenzy:
   - "[ANI] It affects card costs, cost reductions from other effects do apply. [LSJ 20070829-1]"
+  - "[ANI] Also affects the cost of combat cards played at then of a round or combat (eg. {Disarm}, {Telepathic Tracking}, {Psyche!}, {Taste of Vitae}). [ANK 20191221]"
 101961|Terrorists:
-  - 'The provided action is an "equip action" [TOM 19960130]'
+  - The provided action is an "equip action" [TOM 19960130]
 101964|Thanks for the Donation:
-  - "If your prey cannot afford to contest, she pays what she has, she is ousted, and you still yield. [RTR 20010710]"
+  - If your prey cannot afford to contest, she pays what she has, she is ousted, and you still yield. [RTR 20010710]
 101966|Theft of Vitae:
-  - "Can target a minion with less blood or life than the amount stolen. [RTR 20010711]"
-  - "If both opponents play Theft of Vitae, they resolve simultaneously: blood amounts are adjusted by the total of gain and loss and no blood wear off. [ANK 20200123]"
+  - Can target a minion with less blood or life than the amount stolen. [RTR 20010711]
+  - "If both opponents play Theft of Vitae, they resolve simultaneously: blood amounts are adjusted by the total of gain and loss and no blood wear off. [ANK 20200123] [LSJ 20041027]"
 101968|Therbold Realty:
-  - "The reduction applies to equipments that are locations (eg. {Palatial Estate}). [LSJ 20080107]"
+  - The reduction applies to equipments that are locations (eg. {Palatial Estate}). [LSJ 20080107]
 101969|Thicker than Blood:
-  - "The vampire coming out of uncontrolled keeps the cards and blood he has, if any. [LSJ 20100206-2]"
+  - The vampire coming out of uncontrolled keeps the cards and blood he has, if any. [LSJ 20100206-2]
 101971|Thin-Blooded Seer:
-  - "When computing the cost of a card, multiplications and divisions are applied first, followed by additions and substractions. [PIB 20150917] [RTR 20070707]"
+  - When computing the cost of a card, multiplications and divisions are applied first, followed by additions and substractions. [PIB 20150917] [RTR 20070707]
 "101973|Third Tradition: Progeny":
-  - "The decision to move blood on the Progeny or not is taken upon resolution. [PIB 20150418]"
-  - "The Progeny gets the default Sect of the clan of its progenitor, even if the progenitor himself is not a member of that sect. [ANK 20200117]"
+  - The decision to move blood on the Progeny or not is taken upon resolution. [PIB 20150418]
+  - The Progeny is Camarilla Sect. [RTR 20201130]
+101974|Thirst:
+  - The hunt needs to be successful for a vampire to avoid the effect. [LSJ 20050727]
 101975|Those Who Endure Judge:
-  - 'If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]'
-  - 'If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
+  - If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]
+  - If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]
 101976|Thoughts Betrayed:
   - "[dom] Damage is environmental. [RTR 19970630] [ANK 20200422]"
   - '[dom] Damage is inflicted even against a dodge. A "strike: combat ends" ends combat before damage is applied, as will a combattant going to torpor during first strike. [RTR 19941109] [TOM 19951216] [PIB 20140324] [ANK 20200422]'
+  - "[DOM] Cards that merely provide the ability to strike (eg. {.44 Magnum}), are allowed. [ANK 20210928-2]"
+  - "[DOM] Strike cards that are played during the Determine Range step because they provide a maneuver (eg. {Aid from Bats}) are not allowed. [ANK 20210928-2]"
 101979|Three's a Crowd:
-  - "The press can only be used during the current round. [TOM 19960521]"
+  - The press can only be used during the current round. [TOM 19960521]
 101983|Thrown Sewer Lid:
   - "[POT] The press can only be used during the current round. [TOM 19960521]"
 101985|Tinglestripe:
   - "[MYT] The optional maneuver cannot be used if the strike cannot be used (eg. {Hidden Lurker}). [LSJ 20021028]"
 101988|Tongue of the Serpent:
-  - "Can target a minion with less blood than the amount stolen. [RTR 20010711]"
+  - Can target a minion with less blood than the amount stolen. [RTR 20010711]
 101989|Toreador Grand Ball:
-  - 'The same vampire can serve as the "second Toreador" for multiple Toreador Grand Balls. [TOM 19960528]'
-  - "The first Toreador chosen for the Toreador Grand Ball is unblockable on all non-bleed actions. This remains true even after the vampire attempts a bleed. [LSJ 19970814]"
+  - The same vampire can serve as the "second Toreador" for multiple Toreador Grand Balls. [TOM 19960528]
+  - The first Toreador chosen for the Toreador Grand Ball is unblockable on all non-bleed actions. This remains true even after the vampire attempts a bleed. [LSJ 19970814]
 101991|Toreador's Bane:
   - '[mel] [MEL] If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]'
-  - '[mel] [MEL] If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
+  - '[mel] [MEL] If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
   - '[mel] [MEL] An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]'
   - '[mel] [MEL] "continue as if unblocked" moves the action card from the ash heap (where it went when the action was blocked) to limbo (where it should be if the action is not blocked). If the action card is not in the ash heap, then the action cannot be continued. [LSJ 20070808-1]'
   - '[mel] [MEL] If the combat continues or a new combat occurs, the "action continues as if unblocked" effect is lost. [LSJ 19980109] [RTR 20020501]'
+101993|Torn Signpost:
+  - Sets base strength. It can reduce the base strength of a minion (eg. {Rock Cat}). [PIB 20130303]
+  - Any "+X strength" effect adds to it. [LSJ 20100813]
 101995|Torrent:
   - '[CEL] If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]'
-  - '[CEL] If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
+  - '[CEL] If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
   - '[CEL] An action cannot continue "as if unblocked" after a combat resulting from a successful action. [RTR 19970630]'
   - '[CEL] "continue as if unblocked" moves the action card from the ash heap (where it went when the action was blocked) to limbo (where it should be if the action is not blocked). If the action card is not in the ash heap, then the action cannot be continued. [LSJ 20070808-1]'
   - '[CEL] If the combat continues or a new combat occurs, the "action continues as if unblocked" effect is lost. [LSJ 19980109] [RTR 20020501]'
 101996|Tortured Confession:
-  - "Not usable by vampires burned in combat, either. [RTR 19950622]"
+  - Not usable by vampires burned in combat, either. [RTR 19950622]
 101998|Touch of Clarity:
-  - "Can be used as an action modifier by a non-acting ready unlocked minion controlled by the controller of the acting minion. [LSJ 20090425] [LSJ 19990425]"
+  - Can be used as an action modifier by a non-acting ready unlocked minion controlled by the controller of the acting minion. [LSJ 20090425] [LSJ 19990425]
 102008|Tranquility:
   - "[DOM] The press can only be used during the current round. [TOM 19960521]"
 102011|Transfusion:
   - "[THN] Requirements do not apply when taking control of a card already in play. [TOM 19960226-1]"
   - "[THN] Environmental damage do not qualify, only damage inflicted by the acting vampire. [ANK 20200517]"
 102012|Trap:
-  - "The provided press must be handled first. Another press cannot be used to continue (eg. {Boxed In}) if there's already a press to continue. [ANK 20200525-1]"
+  - The provided press must be handled first. Another press cannot be used to continue (eg. {Boxed In}) if there's already a press to continue. [ANK 20200525-1]
+  - A minion that cannot play or use presses (eg. {Mukhtar Bey}) can play it and does provide the presses, the minion is not the one pressing. [LSJ 20040521]
 102013|Travelers Obey the Tenets:
-  - 'The acting player decides the order of (and can play other) "after resolving the action" effects. [ANK 20180206]'
+  - The acting player decides the order of (and can play other) "after resolving the action" effects. [ANK 20180206]
 102014|Treachery:
   - "[pre] The pool is burned after the referendum effects are applied, including any oust and pool gained from it. [LSJ 20090115-2]"
   - "[PRE] The pool is burned when the votes are tallied, before applying the referendum effects. [RTR 20010710]"
+102016|Treat the Sick Mind:
+  - '[OBE] [REACTION] Cards are not replaced during the "as played" window. [LSJ 20061013]'
+  - "[OBE] [REACTION] Cannot be played during combat. [LSJ 20080618]"
+  - '[OBE] [REACTION] Cannot be used to cancel an action card after using a reaction to "unlock and attempt to block". [LSJ 20021011]'
+  - '[OBE] [REACTION] If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
 102017|The Treatment:
-  - "Does nothing to the target Prince if the Prince is in Torpor with zero blood. [TOM 19960423]"
-  - "Will cease functioning if the vampire it is on loses his Prince title. It will resume working if the vampire becomes a Prince again. [LSJ 19980209]"
+  - Does nothing to the target Prince if the Prince is in Torpor with zero blood. [TOM 19960423]
+  - Will cease functioning if the vampire it is on loses his Prince title. It will resume working if the vampire becomes a Prince again. [LSJ 19980209]
+102023|Tribute to the Master:
+  - Can be played with no ready vampire. [ANK 20210717]
 102025|Triole's Revenge:
-  - "The Ventrue is burned only if the hunt isn't blocked, he still burns if the benefit of the hunt is reduced to zero. [TOM 19951212-3]"
+  - The Ventrue is burned only if the hunt isn't blocked, he still burns if the benefit of the hunt is reduced to zero. [TOM 19951212-3]
 102026|Trochomancy:
-  - "The cards are removed immediately. [PIB 20120525]"
-  - "The cards to remove must be chosen when announcing the action. [LSJ 20100527]"
+  - The cards to remove are chosen by the player playing it. There is no order to the ash heap. [LSJ 20090710]
+  - The cards are removed immediately. [PIB 20120525]
 "102027|Trophy: Chosen":
-  - "If the recipient of the Trophy chooses to burn it, there is no other effect. He does not unlock and does not gain the four blood. [LSJ 20070309-1]"
+  - If the recipient of the Trophy chooses to burn it, there is no other effect. He does not unlock and does not gain the four blood. [LSJ 20070309-1]
 "102029|Trophy: Diablerie":
   - "May be retrieved when diablerizing a Red List vampire prior to the blood hunt referendum: it protects the vampire in that referendum. All copies on the vampire are then burned at the end of that action. [LSJ 20050222]"
 "102031|Trophy: Domain":
-  - "Cannot be used to unlock if the vampire cannot attempt to block the action (eg. {Daring the Dawn}). [LSJ 20010714-2]"
-  - "If used to unlock, the block attempt and subsequent combat still happen if the action lacks a suitable target because of the unlock (eg. {Ambush}). [LSJ 20090514]"
+  - Cannot be used to unlock if the vampire cannot attempt to block the action (eg. {Daring the Dawn}). [LSJ 20010714-2]
+  - When used to block, does not ignore the normal prey, predator or target restrictions. [ANK 20180623]
+  - When used to block, the block attempt and subsequent combat still happen if the action lacks a suitable target because of the unlock (eg. {Ambush}). [LSJ 20090514]
 "102032|Trophy: Hunting Ground":
-  - "Is a non-derivative hunting ground (ie. taken into account by {Poacher's Hunting Ground}), even if not active yet. [ANK 20170430] [LSJ 20080610]"
+  - Is a non-derivative hunting ground (ie. taken into account by {Poacher's Hunting Ground}), even if not active yet. [ANK 20170430] [LSJ 20080610]
 102044|Truth of a Thousand Lies:
   - '[SER] Cards and effects that can be played "after resolution" (and only them) can be played after it. [ANK 20190425]'
 102047|Tunnel Runner:
-  - "Damage done from stealing blood to the Runner is environmental. [RTR 19970630] [LSJ19971028]"
+  - Damage done from stealing blood to the Runner is environmental. [RTR 19970630] [LSJ19971028]
   - "Damage done from stealing blood is done at the same time strike damage is done: a single instantaneous prevention card (eg. {Soak}) can prevent both. [ANK 20200517-2]"
 102051|Twisting the Knife:
   - "[POT] The press can only be used during the current round. [TOM 19960521]"
 102058|Uncontrollable Rage:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
-  - "All the damage is aggravated. [LSJ 20011204]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
+  - All the damage is aggravated. [LSJ 20011204]
 102060|Undead Persistence:
   - "[for] The vampire can play cards which are not usable by vampires going to torpor. [LSJ 19970303]"
   - "[for] Only provides one press for the current round, not the ones after that. [ANK 20180110]"
   - "[for] Cannot be used twice by the same vampire during the same combat: because of the first, the vampire is not going into torpor and does not meet the requirement to play it anymore. [LSJ 20030214]"
   - '[for] If an effect causes a new combat to occur at the end of combat, then the "go to torpor" effect will be delayed until after that new combat. However, the vampire will no longer benefit from Undead Persistence in the new combat, so it will end immediately with the vampire not ready unless he plays a new Undead Persistence in the new combat. [LSJ 20030214] [ANK 20190624]'
   - "[FOR] Cannot be used if there is no damage to prevent. [LSJ 20001114]"
   - "[FOR] Prevents up to 2 damage, it can be used to prevent less. [RTR 20041202]"
   - "[FOR] Unused prevention does not carry over. [LSJ 20001114]"
 102061|Undead Strength:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 102063|Under Siege:
-  - "Cannot be used to unlock if the vampire cannot attempt to block the action (eg. {Daring the Dawn}). [LSJ 20010714-2]"
-  - "The block attempt and subsequent combat still happen if the action lacks a suitable target because of the unlock (eg. {Ambush}). [LSJ 20090514]"
-  - "Can be used for intercept even if the vampire is already unlocked. [PIB 20150216]"
-  - "Can be used by a vampire who is already attempting to block. [ANK 20181122-2]"
+  - Cannot be used to unlock if the vampire cannot attempt to block the action (eg. {Daring the Dawn}). [LSJ 20010714-2]
+  - When used to block, does not ignore the normal prey, predator or target restrictions. [ANK 20180623]
+  - The block attempt and subsequent combat still happen if the action lacks a suitable target because of the unlock (eg. {Ambush}). [LSJ 20090514]
+  - Can be used for intercept even if the vampire is already unlocked. [PIB 20150216]
+  - Can be used by a vampire who is already attempting to block. [ANK 20181122-2]
 102065|Underbridge Stray:
-  - "He can burn 1 life to give a minion you control a press the turn he is recruited. [ANK 20180517]"
+  - He can burn 1 life to give a minion you control a press the turn he is recruited. [ANK 20180517]
 102067|Undue Influence:
-  - "Cannot be played with no vampire in the uncontrolled region. [LSJ 20060623]"
+  - Cannot be played with no vampire in the uncontrolled region. [LSJ 20060623]
 102068|Undying Tenacity:
   - "[for] The vampire can play cards which are not usable by vampires going to torpor. [LSJ 19970303]"
 102069|Undying Thirst:
-  - "If the vampire is empty, he must either hunt or diablerize, this is a mandatory action. [LSJ 20081213-2]"
+  - If the vampire is empty, he must either hunt or diablerize, this is a mandatory action. [LSJ 20081213-2]
+  - Has no effect on a vampire that cannot commit diablerie (eg. because of {Humanitas}). [LSJ 20050324-2]
 102071|Unflinching Persistence:
   - "[for] Cannot be used if there is no damage to prevent. [LSJ 20001114]"
 102072|Unholy Penance:
   - "[PRE] The additional effect takes place after the end of combat. [RTR 19970630]"
 102074|Unity:
-  - "You can cut however you want (eg. count cards, cut only one or two). [LSJ 20060413]"
+  - You can cut however you want (eg. count cards, cut only one or two). [LSJ 20060413]
 102076|Unleash Hell's Fury:
-  - "If the block is successful, the aggravated damage is inflicted and the card burned even if the action is ended before block resolution. [LSJ 20100301]"
-  - "If {The Kiss of Ra} or {Elder Impersonation} are used, the block does not happen. It is not locked if {Faceless Night} was played. [LSJ 20100210]"
-  - "Can attempt to block even if locked. [LSJ 20100210]"
-  - "The burn option can be used if all your infernal vampires are in torpor. [LSJ 20091203]"
+  - If the action is blocked, no other effect can be used (eg. {Crypt's Sons}, {Change of Target}) before burning Unleash Hell's Fury and inflicting aggravated damage. However, effects that trigger at the same moment (eg. {Banshee Ironwail}) are still applied and ordered by the acting Methuselah. [ANK 20210627] [ANK 20211207] [ANK 20220116]""
+  - If the block is successful, the aggravated damage is inflicted and the card burned even if the action is ended (eg. {Mirror Walk}) before block resolution. [LSJ 20100301] [ANK 20220116]
+  - If {The Kiss of Ra} or {Elder Impersonation} are used, the block does not happen. [LSJ 20100210]
+  - Unleash Hell's Fury is not locked if {Faceless Night} was played. Also, it can attempt to block even if locked. [LSJ 20100210]
+  - Once it's attempting to block, its intercept can be affected by other cards normally (eg. {KRCG News Radio}). [ANK 20211112-2]
+  - The burn option can be used if all your infernal vampires are in torpor. [LSJ 20091203]
+  - The fact it is Unique has no bearing on the burn option. You cannot use the burn option if you have an infernal vampire ready, even if you already have an Unleash Hell's Fury in play. [LJS 20100203-2]
 102078|Unlicensed Taxicab:
-  - "Offers the additional stealth on actions to equip it from another friendly minion as well, even with other equipment in the same action. [LSJ 20060222]"
+  - Offers the additional stealth on actions to equip it from another friendly minion as well, even with other equipment in the same action. [LSJ 20060222]
 102081|Unseen Hibernation:
   - "[abo] The action ends immediately, no other action modifier or reaction can be played afterwards. [RTR 20180719]"
+  - "[abo] The action has reached resolution, so is subject to NRA (Non Repeatable Action) rules. [ANK 20211015]"
 102082|Unwholesome Bond:
-  - "Cannot be used by {Angelo} or {New Blood} on a uncontrolled vampire with no circle designation, even another {Angelo} or {New Blood}. [LSJ 20050927]"
+  - Can be used by {Angelo} or {New Blood} on a uncontrolled vampire with no circle designation, even another {Angelo} or {New Blood}. Multiple uncontrolled Angelos or New Bloods are in distinct "circle of one" though, so you have to choose one. [LSJ 20050927] [ANK 20211113]
 102087|Vagabond Mystic:
-  - "He can lock to use his ability the turn he is recruited. [ANK 20180517]"
+  - He can lock to use his ability the turn he is recruited. [ANK 20180517]
+  - His ability cannot be used in the middle of a single damage resolution step. [LSJ 20001111]
 102088|Vampiric Disease:
-  - 'At the beginning of the unlock phase, an afflicted vampires unlocks and burns a blood before effects that are applied "during" the unlock phase. [ANK 20180702]'
-  - "Unlocking an already unlocked vampire does not trigger the effect. [ANK 20170227] [LSJ 20020408]"
+  - At the beginning of the unlock phase, an afflicted vampires unlocks and burns a blood before effects that are applied "during" the unlock phase. [ANK 20180702]
+  - Unlocking an already unlocked vampire does not trigger the effect. [ANK 20170227] [LSJ 20020408]
+  - The counter is placed after range is determined, before strikes are chosen (defensive strikes like dodge or combat ends do not avoid it). [ANK 20210422] [LSJ 20040830]
 102089|Vampiric Speed:
   - "[CEL] The press can only be used during the current round. [TOM 19960521]"
 102092|Vast Wealth:
-  - 'The provided action is an "equip action" [TOM 19960130] [RTR 19960124]'
-  - "You only search your library if the action is successful. [TOM 19951107]"
-  - "Paying for the equipment found is not optional. If paying the cost will oust the controlling Methuselah, then she is ousted. [RTR 19941109] [RTR 20010710]"
-  - "If the equipment cannot be legally placed on the vampire, it is burned without cost. [TOM 19950407]"
-  - "Vast Wealth's ability is not usable if the vampire does not share the same controller as Vast Wealth. [RTR 19951017]"
-  - "You do not show cards when you search. [PIB 20121028]"
+  - The provided action is an "equip action" [TOM 19960130] [RTR 19960124]
+  - You only search your library if the action is successful. [TOM 19951107]
+  - Paying for the equipment found is not optional. If paying the cost will oust the controlling Methuselah, then she is ousted. [RTR 19941109] [RTR 20010710]
+  - If the equipment cannot be legally placed on the vampire, it is burned without cost. [TOM 19950407]
+  - Vast Wealth's ability is not usable if the vampire does not share the same controller as Vast Wealth. [RTR 19951017]
+  - You do not show cards when you search. [PIB 20121028]
 102093|Vaticination:
-  - "You do not get to see the card drawn as replacement. [PIB 20121031]"
+  - You do not get to see the card drawn as replacement. [PIB 20121031]
 102095|Veil of Darkness:
-  - "The card that has no effect still counts as played, if it was an action, the vampire is not locked and can perform another (or the same) action. [LSJ 20090323]"
-  - 'Does not affect allies who play cards requiring a Discipline "as a vampire". [LSJ 20050606]'
+  - The card that has no effect still counts as played, if it was an action, the vampire is not locked and can perform another (or the same) action. [LSJ 20090323]
+  - Does not affect allies who play cards requiring a Discipline "as a vampire". [LSJ 20050606]
+  - The effect needs to be applied before anyone has an opportunity to play another cancelation effect (eg. {Direct Intervention}). [LSJ 20100728] [LSJ 20090213]
 102097|Veil the Legions:
-  - "Can only be played by the controller of the acting minion. [LSJ 19990425]"
+  - Can only be played by the controller of the acting minion. [LSJ 19990425]
+  - '[OBF] If an action is canceled after it has been played (eg. {Tangle Atropos'' Hand} but not {Direct Intervention}) it still counts as "one of the next X actions". [ANK 20210124]'
 102098|Veiled Sight:
   - "[CHI] The strike can be used on a minion with no blood. [RTR 20010711]"
   - "[CHI] The strike is not ranged. [TOM 19951215-2]"
 102099|Veles' Hunt:
-  - "Modifiers and reactions can be played during and after the referendum (eg. {Voter Captivation}, {Delaying Tactics}). [LSJ 20081202-2]"
+  - Modifiers and reactions can be played during and after the referendum (eg. {Voter Captivation}, {Delaying Tactics}). [LSJ 20081202-2]
 102100|Velvet Tongue:
-  - "If an effect causes a minion to be unable to cast votes or ballots during a referendum, that minion is forced to abstain, whether he or she had already cast votes or ballots or not. [PIB 20141226]"
+  - "[ser] Putting a corruption counter on a minion does not give you an opportunity to steal it. [ANK 20200925] [ANK 20211105]"
 102103|Veneficti:
-  - "The burn option can be used if all your infernal vampires are in torpor. [LSJ 20091203]"
+  - The burn option can be used if all your infernal vampires are in torpor. [LSJ 20091203]
 102104|Venenation:
-  - "Modifiers that are played before block resolution like {Change of Target} can be played after Venenation. [ANK 20190524] [LSJ 20020126]"
-  - "If the combat is canceled by Venenation, the action is still blocked, {Mask of a Thousand Faces} cannot be used to continue it, but an effect can be used to continue the action as if unblocked (eg. {Crypt's Sons}, {Momentary Delay}). [ANK 20181003] [LSJ 20010803-2]"
+  - Modifiers that are played before block resolution like {Change of Target} can be played after Venenation. [ANK 20190524] [LSJ 20020126]
+  - If the combat is canceled by Venenation, the action is still blocked, the blocking minion locks. {Mask of a Thousand Faces} cannot be used to continue it, but an effect can be used to continue the action as if unblocked (eg. {Crypt's Sons}, {Momentary Delay}). [ANK 20181003] [LSJ 20010803-2] [ANK 20220127]
 102106|Vengeance of Samiel:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
+  - "[val], [VAL] Does not prevent the opponent from dodging, the dodge just has no effect. [LSJ 20030902-2] [LSJ 20060808-1]"
 102113|Vessel:
-  - "Can be used when the vampire is in torpor. [PIB 20150522]"
+  - Can be used when the vampire is in torpor. [PIB 20150522]
+102118|Victim of Habit:
+  - You can lock the card to remove less than three copies, but then the prey does not burn pool. [LSJ 20050408-2]
 102120|Vigilance:
-  - "[REACTION] [1 CONVICTION] Can be used only when reactions can be used (unlocked or with a wake effect). It does not count as playing a reaction card. [LSJ 20070403] [LSJ 20070413]"
+  - "[REACTION] [1 CONVICTION] Can be used only when reactions can be used (during an action). It does not count as playing a reaction card. [LSJ 20070403] [LSJ 20070413]"
   - '[ACTION MODIFIER] Cards and effects that can be played "after resolution" (and only them) can be played after its use. [ANK 20190425]'
 102121|Villein:
-  - "Pay the cost (if any) at the same time you gain pool from it, you do not get ousted in between. [LSJ 20020620]"
-  - "If the target has less blood at resolution than the amount annouced, you take what you can. [LSJ 20100216] [ANK 20180512-2]"
+  - Pay the cost (if any) at the same time you gain pool from it, you do not get ousted in between. [LSJ 20020620]
+  - You must be able to pay the cost to play it (eg. cannot play a third Villein with only 1 pool). [ANK 20210714]
+  - If the target has less blood at resolution than the amount annouced, you take what you can. [LSJ 20100216] [ANK 20180512-2]
 102124|Virtuosa:
-  - '[MEL] Cards and effects that can be played "as the action is announced" (and only them) can be played before it. [ANK 20190425]'
+  - '[MEL] Cards and effects that are played "as the action is announced" must be played before playing "regular" action modifier or reaction cards. [ANK 20190425]'
+  - "[MEL] Replace the action card (if any) before playing it. [ANK 20181208]"
 102126|Visit from the Capuchin:
-  - "Cannot be played if you have another one, even if it has only one counter left. [PIB 20121031]"
-  - "If another effect offers an alternative for card replacement (eg. {Steely Tenacity}), you choose which to apply. [ANK 20200905]"
+  - Cannot be played if you have another one, even if it has only one counter left. [PIB 20121031]
+  - If another effect offers an alternative for card replacement (eg. {Steely Tenacity}), you choose which to apply. [ANK 20200905]
 102128|Vivienne Géroux:
-  - "Cannot play cards requiring both [for] and [cel]. [ANK 20180731-1]"
+  - Can play cards requiring both [for] and [cel]. [ANK 20210719]
+102130|Voices of the Castle:
+  - "[tha] The burn blood effect is not reduced by effects that reduce the cost of the card (eg. {Uta Kovacs}). The card cannot be played if the minion cannot afford to burn the blood. [ANK 20210226]"
 102131|Voter Captivation:
-  - "Is played after the referendum is resolved. If the effect of the referendum ousts the acting Methuselah, there is no time to play it to prevent the ousting. [RTR 19951110]"
-  - 'Can be played before or after other cards that are played "after action resolution" or "if the action was successful". [LSJ 20070327]'
-  - "Can be used after a referendum that is automatically passing, but X is zero in this case. [PIB 20150105] [LSJ 19980107]"
+  - Is played after the referendum is resolved. If the effect of the referendum ousts the acting Methuselah, there is no time to play it to prevent the ousting. [RTR 19951110]
+  - Can be played before or after other cards that are played "after action resolution" or "if the action was successful". [LSJ 20070327]
+  - Can be used after a referendum that is automatically passing, but X is zero in this case. [PIB 20150105] [LSJ 19980107]
 102133|Vox Senis:
-  - 'May still be "canceled as it is played" when used as an out-of-turn master. [LSJ 20031201]'
+  - May still be "canceled as it is played" when used as an out-of-turn master. [LSJ 20031201]
 102135|Vulture's Buffet:
-  - "Is a hunt action. [ANK 20200421]"
-  - "Cannot be played if there is no minion or retainer in any Methusalah's ash heap. [ANK 20200420-3]"
-  - "Is undirected. [ANK 20180202]"
+  - Is a hunt action. [ANK 20200421]
+  - Cannot be played if there is no minion or retainer in any Methuselah's ash heap. [ANK 20200420-3]
+  - Is undirected. [ANK 20180202]
 102137|Wake with Evening's Freshness:
   - "The vampire need not attempt to block nor play further reaction cards: that is merely an option. [TOM 19951129]"
-  - "Can be played after action resolution to use a reaction card (eg. {Fast Reaction} after combat). [LSJ 20091123]"
+  - Can be played after action resolution to use a reaction card (eg. {Fast Reaction} after combat). [LSJ 20091123]
 102141|Walks-With-Might:
-  - "Only affects the cost of masters played by his controller. [LSJ 20081124-1]"
+  - Only affects the cost of masters played by his controller. [LSJ 20081124-1]
 102143|Wanderer's Counsel:
   - "[ACTION MODIFIER] A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]"
   - "[ACTION MODIFIER] The hunt bonus applies to non-standard hunt actions, blood comes from the target of the hunt. [RTR 20030519] [RTR 20180511]"
   - "[ACTION MODIFIER][REACTION] Cannot be used during a referendum that is automatically passing. [PIB 20150105] [LSJ 19980107]"
 102144|War Ghoul:
-  - "If you have no other allies and no retainers in play when it is recruited, then you burn it. [RTR 19961113]"
-  - "An ally or retainer must be burn when it comes into play, regardless of how it did come into play (eg. {Pressing Flesh}). [ANK 20170309-2]"
-  - 'Can use its ability to "lock and burn to burn a location" during an action that would steal it (eg. [PRE] {Entrancement}). The action will have no effect but is still successful if unblocked and must then be paid. [PIB 20121031]'
-  - 'Can use its ability to "lock and burn to burn a location" the turn it is recruited. [ANK 20180517]'
+  - If you have no other allies and no retainers in play when it is recruited, then you burn it. [RTR 19961113]
+  - An ally or retainer must be burn when it comes into play, regardless of how it did come into play (eg. {Pressing Flesh}). [ANK 20170309-2]
+  - Can use its ability to "lock and burn to burn a location" during an action that would steal it (eg. [PRE] {Entrancement}). The action will have no effect but is still successful if unblocked and must then be paid. [PIB 20121031]
+  - Can use its ability to "lock and burn to burn a location" the turn it is recruited. [ANK 20180517]
 102146|Warding the Beast:
   - "[val] Is not the default action, no blood is paid for the rescue. [ANK 20181017]"
 102149|Warsaw Station:
-  - "Can be burned after the annoucement of a diablerie action to bring the target Nosferatu out of torpor. The action will still be successful if unblocked, but will have no effect: no diablerie happen. [ANK 20181107]"
-  - "Can be burned during an action to bring back a vampire that was put into torpor during that action, but the action would end with no effect if an effect tries to continue it (eg. {Ambulance}). [LSJ 20090325-2]"
-  - "The unlock effect is applied after the action is resolved and the referendum (if any) concluded. If the acting vampire is not a Nosferatu anymore at that point, he does not unlock. [LSJ 20090216] [ANK 20180922]"
+  - "Can be burned after the annoucement of a diablerie action to bring the target Nosferatu out of torpor. The action will still be successful if unblocked, but will have no effect: no diablerie happen. [ANK 20220218] [ANK 20181107]"
+  - Can be burned during an action to bring back a vampire that was put into torpor during that action, but the action ends and cannot be continued (eg. with {Ambulance}). [ANK 20220218] [LSJ 20090325-2]
+  - The unlock effect is applied after the action is resolved and the referendum (if any) concluded. If the acting vampire is not a Nosferatu anymore at that point, he does not unlock. [LSJ 20090216] [ANK 20180922]
 102151|Wash:
-  - "If used to cancel a Trifle, the target does not get an extra Master Phase Action from the canceled Trifle. [ANK 20170124] [LSJ 20090126] [RBK 20181001-162]"
-  - "The additional Master Phase Action it provides does not count as a Trifle bonus, the target can get yet an additional Master Phase Action if they play a Trifle afterwards. [ANK 20170124] [LSJ 20090126]"
-  - "If used to cancel an out-of-turn master, that Methuselah still cannot play another out-of-turn master against the same master phase, even though the first was canceled and won't count against that master phase. [LSJ 20070309-2]"
-  - 'If the canceled card had a "Do Not Replace Until" clause on it, that clause is canceled as well and the card is replaced normally. [LSJ 20011023]'
-"102152|Wasserschloss Anif, Austria":
-  - "Can only receive blood from one Tremere on any given turn. [RTR 19960221]"
+  - If used to cancel a Trifle, the target does not get an extra Master Phase Action from the canceled Trifle. [ANK 20170124] [LSJ 20090126] [RBK 20200701-5]
+  - The additional Master Phase Action it provides does not count as a Trifle bonus, the target can get yet an additional Master Phase Action if they play a Trifle afterwards. [ANK 20170124] [LSJ 20090126]
+  - If used to cancel an out-of-turn master, that Methuselah still cannot play another out-of-turn master against the same master phase, even though the first was canceled and won't count against that master phase. [LSJ 20070309-2]
+102152|Wasserschloss Anif, Austria:
+  - Can only receive blood from one Tremere on any given turn. [RTR 19960221]
+102153|Waste Management Operation:
+  - If the library is empty and the hand not full, you draw immediately after using it. [ANK 20211201]
 102160|Wave of Insanity:
-  - "[DEM] Is directed at all Methusalah controlling an ally. [LSJ 20080809-1] [KOT 20081119]"
+  - "[DEM] Is directed at all Methuselah controlling an ally. [LSJ 20080809-1] [KOT 20081119]"
 102161|Wave of Lethargy:
-  - "Card text was changed in 2007, previous rulings do not apply. [ANK 20200408-1]"
+  - Card text was changed in 2007, previous rulings do not apply. [ANK 20200408-1]
 102162|Waxen Poetica:
   - 'Does not burn if combat ends before it resolves (eg. if the opponent uses a "strike: combat ends"). [LSJ 20001127-2] [LSJ 20010806-1] [LSJ 19981006]'
 102164|Weather Control:
-  - "Damage is environmental. [RTR 19970630]"
-  - "The damage is inflicted even if combat is subsequently ended before range (eg. by {Mariel, Lady Thunder}, {Alpha Glint}). [LSJ 19971110] [ANK 20190725]"
-  - "The minion can play other pre-range effects before applying the damage and opening the damage prevention window, but he has to apply damage before passing the opportunity to play effects to the next player. [ANK 20170930]"
-  - "Both minions have the opportunity to play prevention and non-prevention pre-range effects during the damage prevention window. [ANK 20170930]"
+  - The damage is environmental. [RTR 19970630]
+  - The damage is applied even if the combat ends prematurely (eg. by {Mariel, Lady Thunder}, {Alpha Glint}). [LSJ 19971110] [ANK 20190725]
+  - Both minions have the opportunity to play prevention and non-prevention pre-range effects before mending the damage. If another pre-range damaging effect is played then, all damages are prevented and mended together. [ANK 20170930]
 102165|Web of Knives Recruit:
-  - "It is not an action to put a vampire in play. [LSJ 20060616-2]"
+  - It is not an action to put a vampire in play (eg. {Blood Cult Awareness Network} does not give it -1 stealth). [LSJ 20060616-2]
 102166|Week of Nightmares:
-  - "Ravnos can target a Ravnos with no blood with the +1 stealth hunt action. [RTR 20010711]"
-  - "Cannot choose to target a vampire when using another non-standard hunt action (eg. {Abactor}). [LSJ 20090606] [ANK 20190707]"
+  - Ravnos can target a Ravnos with no blood with the +1 stealth hunt action. [RTR 20010711]
+  - Cannot choose to target a vampire when using another non-standard hunt action (eg. {Abactor}). [LSJ 20090606] [ANK 20190707]
 102168|Weigh the Heart:
-  - '[AUS][SER] Cards and effects that can be played "as the action is announced" (and only them) can be played before it. [ANK 20190425]'
-  - "[AUS][SER] If the action targets multiple Methusalah, you choose one minion, which must be controlled by one of the target Methusalah. [ANK 20180515]"
+  - '[AUS][SER] Cards and effects that are played "as the action is announced" must be played before playing "regular" action modifier or reaction cards. [ANK 20190425]'
+  - "[AUS][SER] If the action targets multiple Methuselah, you choose one minion, which must be controlled by one of the target Methuselah. [ANK 20180515]"
+  - "[AUS][SER] Replace the action card (if any) before playing it. [ANK 20181208]"
 102169|Weighted Walking Stick:
-  - "If the damage is reduced (eg. {Nephandus}), the corresponding token is not burned (contrary to prevented damage). [LSJ 20100519]"
-  - "Full damage is applied if there are any counter left, even just 1. [ANK 20201229-2]"
+  - If the damage is reduced (eg. {Nephandus}) or not inflicted (eg. {Blood Fury}), the corresponding token is not burned (contrary to prevented damage). [LSJ 20100519]
+  - Full damage is applied if there are any counter left, even just 1. [ANK 20201229-2]
 102171|Well-Aimed Car:
   - "[POT] The press can only be used during the current round. [TOM 19960521]"
 102173|Wendell Delburton:
-  - "Additional damage inherits all of the properties of the base damage. [TOM 19960225]"
+  - Additional damage inherits all of the properties of the base damage. [TOM 19960225]
 102175|Whispers from the Dead:
-  - "The card to retrieve must be announced when declaring the action. [LSJ 20010627]"
+  - The card to retrieve must be announced when declaring the action. [LSJ 20010627]
 102179|White Phosphorus Grenade:
-  - "Damage done to the bearer is environmental. [LSJ 19970801]"
-  - 'Does not burn if combat ends before it resolves (eg. if the opponent uses a "strike: combat ends"). [LSJ 20001127-2] [LSJ 20010806-1][LSJ 19981006]'
+  - Damage done to the bearer is environmental. [LSJ 19970801]
+  - 'Does not burn if combat ends before it resolves (eg. if the opponent uses a "strike: combat ends"). [LSJ 20001127-2] [LSJ 20010806-1] [LSJ 19981006]'
 102180|Wider View:
-  - "Cards removed from the game are public. [LSJ 20080314]"
+  - Cards removed from the game are public. [LSJ 20080314]
 102183|Will-o'-the-Wisp:
-  - '[CHI] Cards and effects that can be played "as the action is announced" (and only them) can be played before it. [ANK 20190425]'
-102184|Winchester Mansion:
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
+  - '[CHI] Cards and effects that are played "as the action is announced" must be played before playing "regular" action modifier or reaction cards. [ANK 20190425]'
+  - "[CHI] Replace the action card (if any) before playing it. [ANK 20181208]"
 102190|Wolf Claws:
-  - "[pro] Must be played before strike resolution (and damage prevention) in order to affect the current strike [RTR 19960112]"
+  - "[pro] Must be played before strike resolution and damage prevention in order to affect the current strike. Can be played after both strikes have been chosen. [RTR 19960112]"
 102192|Wooden Stake:
-  - 'If placed on a minion that cannot have equipment, the Stake is burned. The "does not unlock as normal" effect still applies. [LSJ 19980831]'
-  - 'The "does not unlock as normal" effect continues to apply if the Stake is burned or moved. [LSJ 19980831]'
+  - If placed on a minion that cannot have equipment, the Stake is burned. The "does not unlock as normal" effect still applies. [LSJ 19980831]
+  - The "does not unlock as normal" effect continues to apply if the Stake is burned or moved. [LSJ 19980831]
 102194|Wormwood:
-  - "Ceils the vampire's capacity, including effects that have changed it, to X. {Orun} adds to that X, or the vampire's capacity if it is lower, for cards played by other players. [LSJ 20051205]"
-  - 'When a vampire is influenced, the excess blood drains off before entering contest (if any) and before playing "as played/as he enters play" effects. [LSJ 20100902]'
+  - Ceils the vampire's capacity, including effects that have changed it, to X. {Orun} adds to that X, or the vampire's capacity if it is lower, for cards played by other players. [LSJ 20051205]
+  - When a vampire is influenced, the excess blood drains off before entering contest (if any) and before playing "as played/as he enters play" effects. [LSJ 20100902]
 102196|Writ of Acceptance:
-  - "The effect is not optional. [RTR 19980707]"
-  - "Is a temporary effect that overrides the underlying sect. The most recent override takes precendence. It stays active if another effect changes the underlying sect, like using the default action to become Anarch. [LSJ 20100811] [ANK 20190619]"
-  - "If the target changes sect to a sect inappropriate for his title, he loses its benefit until his sect is appropriate. He immediately yields the title if it is contested or he receives a new one. [LSJ 20060904]"
+  - The effect is not optional. [RTR 19980707]
+  - Is a temporary effect that overrides the underlying sect. The most recent override takes precendence. It stays active if another effect changes the underlying sect, like using the default action to become Anarch. [LSJ 20100811] [ANK 20190619]
+  - If the target changes sect to a sect inappropriate for his title, he loses its benefit until his sect is appropriate. He immediately yields the title if it is contested or he receives a new one. [LSJ 20060904]
 102198|XTC-Laced Blood:
-  - "A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]"
+  - A hunt is not successful if no blood is gained, even if the hunt action is still successful. [LSJ 20050720-2]
 102199|Yawp Court:
-  - "Damage inflicted at the end of combat is environmental. [RTR 19970630]"
-  - "If the acting minion is not ready after the combat, then the action ends and no referendum is conducted. [LSJ 20060902]"
-  - "If the acting vampire gets out of torpor immediately (eg. {Warsaw Station}), the action ends and no referendum is conducted. [LSJ 20090325-1]"
-  - 'The effect is applied after cards that are played "at the end of the round (eg. {Disarm}) or "when combat would end". If a combat ends and a new combat would begin, the damage is applied between the two combats and the referendum is conducted after all the combats if the acting vampire is still ready. [ANK 20180910-1] [LSJ 20060903]'
+  - Damage inflicted at the end of combat is environmental. [RTR 19970630]
+  - If the acting minion is not ready after the combat, then the action ends and no referendum is conducted. [LSJ 20060902]
+  - The action cost, if any, is paid before Yawp Court gets locked. [LSJ 20080201]
+  - If the acting vampire gets out of torpor immediately (eg. {Warsaw Station}), the action ends and no referendum is conducted. [LSJ 20090325-1]
+  - The effect is applied after cards that are played "at the end of the round (eg. {Disarm}) or "when combat would end". If a combat ends and a new combat would begin, the damage is applied between the two combats and the referendum is conducted after all the combats if the acting vampire is still ready. [ANK 20180910-1] [LSJ 20060903]
+102200|Year of Fortune:
+  - The bonus disappears if the card is burned (either burned by a referendum or if the controller is ousted). [PIB 20121028]
 102202|Young Bloods:
-  - "They may use their built-in action against a vampire with only 1 blood. If successful, that vampire burns his 1 blood. [LSJ 20070213]"
-  - "If the target of their ability unlocks and the action is not blocked, it is successful but has no effect. [LSJ 20070411] [LSJ 20090514]"
-102203|Zaire River Ferry:
-  - "May be put on any minion if the controller changes. If the new controller has no minions, it is burned. [RTR 19960112]"
+  - They may use their built-in action against a vampire with only 1 blood. If successful, that vampire burns his 1 blood. [LSJ 20070213]
+  - If the target of their ability unlocks and the action is not blocked, it is successful but has no effect. [LSJ 20070411] [LSJ 20090514]
+  - If they are burned by a strike, the blood gained from burning them is awarded after strike resolution (it cannot normally not be used to heal from their strike). [LSJ 20080212]
 102204|Zapaderin:
-  - "Can only be played by the controller of the acting minion. [LSJ 19990425]"
-  - "Multiple copies can be played by different minions on the same action. [ANK 20200515]"
+  - Can only be played by the controller of the acting minion. [LSJ 19990425]
+  - Multiple copies can be played by different minions on the same action. [ANK 20200515]
 102208|Zip Gun:
-  - "Damage done to the bearer is environmental. [LSJ 19970801]"
-  - "No damage is done to the bearer if he does not strike with the gun (eg. if it is destroyed with first strike). [LSJ 20100310]"
-200011|Adana de Sforza:
-  - "Card with multiple types (eg. Combat/Action Modifer) are considered of the type they are played as, not both. [PIB 20150924-2]"
-200017|Aeron:
-  - "The damage inflicted by his ability is environmental. [RTR 19970630] [LSJ 20070328]"
-  - "His ability to get a press can only be used during the press step. [PIB 20150121]"
-"200019|Agaitas, The Scholar of Antiquities":
-  - "Additional draws are not subject to his ability (eg. {Infernal Pursuit}, {Aura Reading}, {Learjet}). [LSJ 20011202]"
-  - "If Agaitas is burned while cards owned by your prey are still face-up in front of you, you can still play and discard them as normal, but you cannot draw in your prey's library until you control Agaitas anew. [LSJ 20100304]"
-  - "Cards from his ability that go into an ash heap, hand, or library always go into their owner's ash heap, hand, or library (eg. using {Heart of Nizchetus}). [RTR 19970425] [LSJ 20060921]"
-  - "A weapon available from his ability can be chose for a {Concealed Weapon}. [LSJ 20060913]"
-200033|Akram:
-  - "If his ability is used to start a new combat, effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]"
-  - "His ability cannot be used to start a new combat if there is already a pending combat queued. [RTR 20020501]"
-200049|Alexandra:
-  - "Can use her unlock ability at any point during the turn, including during a political action. [TOM 19960214]"
-  - "If she locks a Toreador who was attempting to block, then that block will fail. [TOM 19951007] [LSJ 19991025]"
-"200063|Alvaro, The Scion of Angelica":
-  - "He gains blood if he casts no vote, even if he has lost his title or is in torpor. [LSJ 20010526]"
-200068|Ambrogino Giovanni:
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-"200072|Amelia, The Blood Red Tears":
-  - "Her ability triggers after combat if she's still in play, even in torpor. If she is burned during combat, it does not trigger. [ANK 20200420-1]"
-  - "If multiple combats occur in the same action, the opposing minion burns 1 blood or life each time the combat ends. [ANK 20200420-1]"
-  - "In the case of {Free Fight}, the last opposing minion burns the blood. [ANK 20200420-1]"
-200074|Amisa:
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-200076|Anarch Convert:
-  - 'His "as he enters play" ability can be used before he enters contest if there is another one in play. [LSJ 20080526]'
-  - 'Can "convert" an already anarch vampire if he is not titled. [PIB 20121031]'
-200080|Andre LeRoux:
-  - "His ability can be used only once per successful bleed, but can be used multiple times on different bleeds during the same turn. [LSJ 20081123]"
-  - 'It is used in the "would/about to be successful" window like {Spying Mission}. [LSJ 20081123]'
-  - 'Only modifiers and reactions that can be played "when the action/bleed would be successful" can be played after it. [LSJ 20090205]'
-  - "He can use his ability on his own bleed to get (-1 +2) = +1 bleed. [LSJ 20081124-2]"
-  - "His ability cannot be used after {Spying Mission}. If his ability reduces a bleed to zero, it is no longer successful and {Spying Mission} cannot be used afterwards. [PIB 20150612]"
-200091|Angela Preston:
-  - "When she is influenced out, her ability to unlock a vampire can be used during the ongoing influence phase. [RTR 20180303]"
-200094|Angelo:
-  - "A vampire with no circle designation is in his own unique circle of one. Angelo cannot be seen as a member of such a circle. [LSJ 20020609]"
-  - "He cannot attempt an action to employ a retainer, nor strike to steal a retainer. [LSJ 20050315] [LSJ 20010210]"
-200103|Annabelle Triabell:
-  - "Her ability applies to all Toreadors, not just the ones in play at the time the action resolved. [LSJ 20030811]"
-200104|Annazir:
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-200106|Anneke:
-  - "Her ability only affects the rule restricting who gets to block an action. She must still meet all other requirements to block. In particular, {Blood Bond}, {Day Operation}, {Seduction} and prior decision not to block are not circumvented. [RTR 20020501] [LSJ 20041203]"
-200135|Arika:
-  - "Arika's prey can use a location during her unlock phase before burning it. [ANK 20200629]"
-  - "Arika's prey cannot end her unlock phase if she controls a location that she hasn't burned a pool for, even if she gained control of that location during that unlock phase. [LSJ 19990405]"
-200136|Arishat:
-  - "Her ability applies to Priscus votes and ballots. [LSJ 19971001]"
-  - "Her ability to force a vampire to abstain can cancel the votes and ballots of the vampire. [LSJ 20100311]"
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-200138|Armin Brenner:
-  - "His ability is applied after the referendum effects are applied, including any oust and pool gained from it. [LSJ 20090115-2]"
-200145|Asguresh:
-  - "If his ability is used to cancel a strike, another strike is chosen. [LSJ 20100206]"
-  - 'If a canceled card had a "Do Not Replace Until" clause on it (or alternate replacement like {Steely Tenacity}), that clause is canceled as well and the card is replaced normally. [LSJ 20011023] [LSJ 20080630]'
-  - "If his ability is used to cancel a limited effect (additional strike), then the limit is not triggered and another limited effect can be used. [LSJ 20100206] [LSJ 20030224]"
-  - "Can only cancel minion cards played from the hand in the normal fashion (eg. not weapons played via {Disguised Weapon}). [RTR 20001020]"
-200148|Astrid Thomas:
-  - "Her ability triggers when votes are tallied. [RTR 20001020]"
-  - "Tremere who have not yet voted can choose to abstain. [RTR 19941006]"
-  - "If her votes are canceled, the other Tremere votes are unaffected by her ability. [RTR 19960530]"
-200149|Augustus Giovanni:
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-"200155|Aziz, Dammar of Istanbul":
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-"200157|Baba Yaga, the Iron Hag":
-  - "Her ability applies when recruiting in a non-normal way (eg. {Pack Alpha}). [PIB 20150105-2]"
-200167|The Baron:
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-  - "Cannot play cards requiring a Baron. [PIB 20151116]"
-200168|Baron Dieudonne:
-  - "Cannot play cards requiring a Baron. [PIB 20151116]"
-"200179|Beast, The Leatherface of Detroit":
-  - "He cannot attempt an action to equip or employ, nor strike to steal an equipment or retainer. [LSJ 20050315] [LSJ 20010210]"
-  - "He can equip with an equipment that is a location when in play, but not by playing the card normally as it is an action card. (eg. Using {Vast Wealth} would work). [LSJ 20050315] [LSJ 20050413-1] [LSJ 20050413-2]"
-"200191|Bernard, the Scourge":
-  - "When using his ability, modifiers and reactions can be played during and after the referendum (eg. {Voter Captivation}, {Delaying Tactics}). [LSJ 20081202-2]"
-"200199|Bindusara, Historian of the Kindred":
-  - "He cannot perform his special action twice in the same turn, even to fetch different cards. [ANK 20200810]"
-  - "When using his special ability, requirements do not apply (eg. {Arcane Library} is put into play even if you have no ready Tremere). [ANK 20200810]"
-200201|Black Cat:
-  - 'The reduction applies for other effects that check the "cost" of equipment on her. [RTR 19941109]'
-  - "If she is equipped with something and that equipment is transferred to another minion, then it regains its normal pool value. Conversely, if a piece of equipment moves onto her, its effective pool cost is lowered by 1. [RTR 19941109]"
-200224|Brunhilde (ADV):
+  - Damage done to the bearer is environmental. [LSJ 19970801]
+  - No damage is done to the bearer if he does not strike with the gun (eg. if it is destroyed with first strike). [LSJ 20100310]
+"102226|Haqim's Law: Retribution":
+  - If used by a Banu Haqim and another takes the action over with {Mask of a Thousand Faces}, they cannot use it again. [ANK 20221102-2]
+102227|Hunger of Marduk:
+  - The provided strike can be chosen and used more than once during the round. [ANK 20220207]
+102232|The Platinum Protocol:
+  - "[pro] The minion getting the corruption counter is chosen at action resolution (not declaration). [LSJ 20080608]"
+  - "[pro] Putting a corruption counter on a minion does not give you an opportunity to steal it. [ANK 20200925] [ANK 20211105]"
+102236|The British Museum, London:
+  - Checks the card type in hand, reduction and unlock apply to equipments that are locations when in play. [ANK 20220824]
+  - The reduction applies to all valid equipments, even without using the unlock or not equipping from hand. [ANK 20221026]
+102238|Enhanced Coagulant:
+  - The card stays there if the strike is dodged [ANK 20220923]
+  - Cannot be used against an ally. [ANK 20221102]
+102242|Mobile HQ, Operation Antigen:
+  - The card is locked if used to enter combat, even if that action fails. [ANK 20221102]
+102244|The Shard, London:
+  - The cost reduction applies to minion cards, they are also played by the Methuselah. [ANK 20221102]
+200011|Adana de Sforza (G4):
+  - Card with multiple types (eg. Combat/Action Modifer) are considered of the type they are played as, not both. [PIB 20150924-2]
+200017|Aeron (G3):
+  - The damage inflicted by his ability is environmental. [RTR 19970630] [LSJ 20070328]
+  - His ability to get a press can only be used during the press step. [PIB 20150121]
+200019|Agaitas, The Scholar of Antiquities (G2):
+  - Additional draws are not subject to his ability (eg. {Infernal Pursuit}, {Aura Reading}, {Learjet}). [LSJ 20011202]
+  - If Agaitas is burned while cards owned by your prey are still face-up in front of you, you can still play and discard them as normal, but you cannot draw in your prey's library until you control Agaitas anew. [LSJ 20100304]
+  - Cards from his ability that go into an ash heap, hand, or library always go into their owner's ash heap, hand, or library (eg. using {Heart of Nizchetus}). [RTR 19970425] [LSJ 20060921]
+  - A weapon available from his ability can be chosen for a {Concealed Weapon}. [LSJ 20060913]
+200033|Akram (G2):
+  - If his ability is used to start a new combat, effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]
+  - His ability cannot be used to start a new combat if there is already a pending combat queued. [RTR 20020501]
+200044|Alejandro Aguirre (G3):
+  - If a card transforms the damage he inflicts to aggravated (eg. {True Faith}), this includes the damage from his ability. [ANK 20210620]
+200049|Alexandra (G2):
+  - Can use her unlock ability at any point during the turn, including during a political action. [TOM 19960214]
+  - If she locks a Toreador who was attempting to block, then that block will fail. [TOM 19951007] [LSJ 19991025]
+200063|Alvaro, The Scion of Angelica (G2):
+  - He gains blood if he casts no vote, even if he has lost his title or is in torpor. [LSJ 20010526]
+200068|Ambrogino Giovanni (G2):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+200070|Ambrosio Luis Monçada, Plenipotentiary (G2):
+  - Actions from minions of the same controller targeting him are undirected, so they are not affected by his ability. [LSJ 20030214-2]
+200072|Amelia, The Blood Red Tears (G3):
+  - Her ability triggers after combat if she's still in play, even in torpor. If she is burned during combat, it does not trigger. [ANK 20200420-1]
+  - If multiple combats occur in the same action, the opposing minion burns 1 blood or life each time the combat ends. [ANK 20200420-1]
+  - In the case of {Free Fight}, the last opposing minion burns the blood. [ANK 20200420-1]
+200074|Amisa (G2):
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+200076|Anarch Convert (ANY):
+  - His "as he enters play" ability can be used before he enters contest if there is another one in play. This is not self-contesting. [LSJ 20080526] [RTR 20180303] [ANK 20211214]
+  - Can "convert" an already anarch vampire if he is not titled. [PIB 20121031]
+200080|Andre LeRoux (G5):
+  - His ability can be used only once per successful bleed, but can be used multiple times on different bleeds during the same turn. [LSJ 20081123]
+  - It is used in the "would/about to be successful" window like {Spying Mission}. [LSJ 20081123]
+  - Only modifiers and reactions that can be played "when the action/bleed would be successful" can be played after it. [LSJ 20090205]
+  - He can use his ability on his own bleed to get (-1 +2) = +1 bleed. [LSJ 20081124-2]
+  - His ability cannot be used after {Spying Mission}. If his ability reduces a bleed to zero, it is no longer successful and {Spying Mission} cannot be used afterwards. [PIB 20150612]
+200086|Andrew Stuart (G4):
+  - His ability needs to be applied before anyone has an opportunity to play another cancelation effect (eg. {Direct Intervention}). [LSJ 20100728] [LSJ 20090213]
+200091|Angela Preston (G2):
+  - When she is influenced out, her ability to unlock a vampire can be used during the ongoing influence phase. [RTR 20180303]
+200094|Angelo (G3):
+  - A vampire with no circle designation is in his own unique circle of one. [LSJ 20020609] [ANK 20211113]
+  - Angelo can be in the "unique circle of one" of any vampire, including another copy of himself. Two uncontrolled Angelo are in different circles, an active Angelo has to choose (eg. for {Unwholesome Bond}). [ANK 20211113]
+  - He cannot attempt an action to employ a retainer, nor strike to steal a retainer. [LSJ 20050315] [LSJ 20010210]
+200103|Annabelle Triabell (G3):
+  - Her ability applies to all Toreadors, not just the ones in play at the time the action resolved. [LSJ 20030811]
+200104|Annazir (G5):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+  - He cannot perform the action provided by his ability twice in the same turn. [ANK 20220615]
+  - The action provided by his ability is directed against the Methuselah controlling the equipment or location, not the minion it's on. [LSJ 20090324]"
+200106|Anneke (G1):
+  - Her ability only affects the rule restricting who gets to block an action. She must still meet all other requirements to block. In particular, {Blood Bond}, {Day Operation}, {Seduction} and prior decision not to block are not circumvented. [RTR 20020501] [LSJ 20041203]
+200116|Antonio d'Erlette (G4):
+  - "Cost reductions apply (eg. {Powerbase: Tshwane}), except if they require an action (eg. {Charisma}). [LSJ 20090920-2] [RTR 20070707]"
+200135|Arika (G2):
+  - Arika's prey can use a location during her unlock phase before burning it. [ANK 20200629]
+  - Arika's prey cannot end her unlock phase if she controls a location that she hasn't burned a pool for, even if she gained control of that location during that unlock phase. [LSJ 19990405]
+200136|Arishat (G6):
+  - Her ability applies to Priscus votes and ballots. [LSJ 19971001]
+  - Her ability to force a vampire to abstain can cancel the votes and ballots of the vampire. [LSJ 20100311]
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+200138|Armin Brenner (G4):
+  - His ability is applied after the referendum effects are applied, including any oust and pool gained from it. [LSJ 20090115-2]
+200145|Asguresh (G5):
+  - If his ability is used to cancel a strike, another strike is chosen. [LSJ 20100206]
+  - If a canceled card had a "Do Not Replace Until" clause on it (or alternate replacement like {Steely Tenacity}), that clause is canceled as well and the card is replaced normally. [LSJ 20011023] [LSJ 20080630]
+  - If his ability is used to cancel a limited effect (additional strike), then the limit is not triggered and another limited effect can be used. [LSJ 20100206] [LSJ 20030224]
+  - Can only cancel minion cards played from the hand in the normal fashion (eg. not weapons played via {Disguised Weapon}). [RTR 20001020]
+200148|Astrid Thomas (G1):
+  - Her ability triggers when votes are tallied. [RTR 20001020]
+  - Tremere who have not yet voted can choose to abstain. [RTR 19941006]
+  - If her votes are canceled, the other Tremere votes are unaffected by her ability. [RTR 19960530]
+200149|Augustus Giovanni (G2):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+200155|Aziz, Dammar of Istanbul (G2):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+200157|Baba Yaga, the Iron Hag (G5):
+  - Her ability applies when she recruits or employs a retainer or ally in a non-normal way (eg. {Pack Alpha}). [PIB 20150105-2]
+200167|The Baron (G2):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+  - Cannot play cards requiring a Baron. [PIB 20151116]
+200168|Baron Dieudonne (G4):
+  - Cannot play cards requiring a Baron. [PIB 20151116]
+200179|Beast, The Leatherface of Detroit (G2):
+  - He cannot attempt an action to equip or employ, nor strike to steal an equipment or retainer. [LSJ 20050315] [LSJ 20010210]
+  - He can equip with an equipment that is a location when in play, but not by playing the card normally as it is an action card. (eg. Using {Vast Wealth} would work). [LSJ 20050315] [LSJ 20050413-1] [LSJ 20050413-2]
+200191|Bernard, the Scourge (G4):
+  - When using his ability, modifiers and reactions can be played during and after the referendum (eg. {Voter Captivation}, {Delaying Tactics}). [LSJ 20081202-2]
+200199|Bindusara, Historian of the Kindred (G2):
+  - He cannot perform his special action twice in the same turn, even to fetch different cards. [ANK 20200810]
+  - When using his special ability, requirements do not apply (eg. {Arcane Library} is put into play even if you have no ready Tremere). [ANK 20200810]
+200201|Black Cat (G1):
+  - The reduction applies for other effects that check the "cost" of equipment on her. [RTR 19941109]
+  - If she is equipped with something and that equipment is transferred to another minion, then it regains its normal pool value. Conversely, if a piece of equipment moves onto her, its effective pool cost is lowered by 1. [RTR 19941109]
+200224|Brunhilde (G3 ADV):
   - "[MERGED] Is Anarch Baron. If the base version was the one in play, it changes sect as it is merged. [ANK 20180524]"
-200229|Byzar:
-  - "His ability will make a diablerie unsuccessful (blood and equipment stay on him). [LSJ 20100228]"
-200232|Cailean:
-  - "When setting the range for the round, no other effect can be used to reset the range, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]"
-200242|The Capuchin:
-  - "If he burns, he looses all cards and counters on him, all cards and effects lose track of him and he is considered a new vampire for all game purposes (eg. {The Rack} do not target him anymore). [ANK 20200417]"
-  - "If his controller is not his original owner and he burns, he goes to his original owner ash heap, breaking all control effect, then to his owner's uncontrolled area. The Methusalah who was controlling him when he burned gets the additional transfers. [ANK 20200417]"
-200245|Carlotta Giovanni:
-  - "The card being retrieved is announced when the action is declared. [LSJ 19970922]"
-200247|Carmine Giovanni:
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-  - "Her additional life ability applies and her stealth ability can be used when she is in torpor. [LSJ 20011022] [LSJ 20100902-2]"
-200269|Chaundice:
-  - "Can use her ability to prevent 4 damage on a single strike. [LSJ 20100708]"
-200288|Conrad Adoula:
-  - "Card with multiple types (eg. Reaction/Action Modifer) are considered of the type they are played as, not both. [PIB 20150924-2]"
-200297|Count Zaroff:
-  - "His ability can be used more than once each turn. [RTR 20180511]"
-200314|Dancin' Dana (ADV):
+200229|Byzar (G6):
+  - His ability will make a diablerie unsuccessful (blood and equipment stay on him). [LSJ 20100228]
+  - When he burns from aggravated damage, additional damage is lost. [ANK 20210424]
+  - If {Amaranth} burns him and he comes back in torpor, another {Amaranth} can be played. [ANK 20210424]
+200232|Cailean (G2):
+  - When setting the range for the round, no other effect can be used to reset the range, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]
+200242|The Capuchin (G5):
+  - If he burns, he looses all cards and counters on him, all cards and effects lose track of him and he is considered a new vampire for all game purposes (eg. {The Rack} does not target him anymore). [ANK 20200417]
+  - If his controller is not his original owner and he burns, he goes to his original owner ash heap, breaking all control effect, then to his owner's uncontrolled area. The Methuselah who was controlling him when he burned gets the additional transfers. [ANK 20200417]
+200245|Carlotta Giovanni (G2):
+  - The card being retrieved is announced when the action is declared. [LSJ 19970922]
+200247|Carmine Giovanni (G4):
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+  - Her additional life ability applies and her stealth ability can be used when she is in torpor. [LSJ 20011022] [LSJ 20100902-2]
+200249|Carolina Vález (G5):
+  - She is immune to unlock damage from allies like {Abyssal Hunter} and {Wendell Delburton} [ANK 20210228]
+200269|Chaundice (G4):
+  - Can use her ability to prevent 4 damage on a single strike. [LSJ 20100708]
+200288|Conrad Adoula (G4):
+  - Card with multiple types (eg. Reaction/Action Modifer) are considered of the type they are played as, not both. [PIB 20150924-2]
+200297|Count Zaroff (G5):
+  - His ability can be used more than once each turn. [RTR 20180511]
+200314|Dancin' Dana (G1 ADV):
   - "[MERGED] Is Anarch. If the base version was the one in play, it changes sect as it is merged. [ANK 20180524]"
-200316|Danielle Diron:
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-200333|Demdemeh:
-  - 'The animal retainers turned into allies keep their current life counters and remember their original "starting life", for effects that notice "starting life". The retainers'' special abilities are lost. [LSJ 20051116-1]'
-200335|Democritus:
-  - "Does not affect the cost to contest titles, since it is paid in vampire blood, not pool. [RTR 19950509]"
-200357|Dominique:
-  - "If a location costs X blood, it would take X vandal counters to burn it. [LSJ 20001118]"
-200360|Don Caravelli:
-  - "His ability to give a press can only be used during the press step. [PIB 20150121]"
-200363|Don Michael Antonio Giovanni:
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-200364|Dónal O'Connor:
-  - "An empty blocking vampire may still block and will try and fail to burn a blood if the block is successful. [TOM 19951215-1]"
-  - "The blocking vampire burns 1 blood immediately upon successfully blocking Donal, regardless of whether combat begins. [RTR 19960530]"
-200365|Donald Cargill:
-  - "His ability is applied after the referendum effects are applied, including any oust and pool gained from it. [LSJ 20090115-2]"
-  - "His ability is still applied if the predator is ousted by the referendum effects. [LSJ 20090115-2]"
-"200381|Dr. Morrow, The Skindoctor":
-  - "Multiple graft counters may be placed on the same minion, but they have no additional effect. A minion with one or more graft counters gets -1 stealth, not -X stealth. [LSJ 20070306]"
-200383|Dr. Solomon Grey:
-  - "You burn one pool before he enters contest if there is another one in play. [LSJ 20080526]"
-200386|Dragos:
-  - "If his opponent plays superior {Terror Frenzy}, Dragos has to burn one blood for each combat card he plays in that combat. [LSJ 19990223]"
-200389|Drozodny:
-  - "When using his ability, the card to retrieve must be announced when declaring the action. [LSJ 20010627]"
-200401|Edith Blount:
-  - "Edith may burn a blood to give {Enid Blount} stealth multiple times each action. [LSJ 20040617]"
-200403|Edward Vignes:
-  - "His ability cannot be used if the action is blocked. [LSJ 20041022]"
-200417|Ellison Humboldt:
-  - "Can use his ability only once per referendum. [ANK 20180307-2] [RBK 20181001-11]"
-"200424|Enkidu, The Noah":
-  - "He cannot attempt an action to equip nor strike to steal an equipment. [LSJ 20050315] [LSJ 20010210]"
-  - "He can equip with an equipment that is a location when in play. [LSJ 20050315]"
-200427|Epikasta Rigatos:
-  - "Can only retrieve a card played during that same action. [ANK 20180628]"
-  - "Can only retrieve cards played the normal way, ie. not put into play as a result of another card (eg. {Concealed Weapon} or {Charming Lobby}). [LSJ 20090430] [ANK 20180628]"
-200434|Erlik:
-  - 'His "as he enters play" ability can be used before he enters contest (not after) if there is another one in play. [LSJ 20080526] [LSJ 20100902] [ANK 20180626-1]'
-200438|Ethan Locke:
-  - "Ethan's Ⓓ action is directed at the controller of the skill card, not the controller of the vampire. [LSJ 19970224]"
-  - "When he steals a master Discipline card, his controller becomes the controller of the Discipline card. [LSJ 19990709]"
-200439|Étienne Fauberge:
-  - "Allies have no blood, they cannot take Ⓓ actions against him, except if they are acting as a vampire. [LSJ 20030815]"
-200443|Eurayle Gelasia Mylonas:
-  - "Her ability is undirect if you control the target, directed to the controller of the target otherwise. [PIB 20121210]"
-200450|Ezmerelda:
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-200452|Fabrizia Contreraz:
-  - "She only gets her votes if your prey controls a ready Camarilla vampire. [PIB 20150713]"
-200485|Frondator:
-  - "The cost to rescue from torpor is reduced even if paid by the rescuee. This is not optional. [LSJ 20020304-2] [PIB 20110918]"
-200498|Gem Ghastly:
-  - "When playing a card requiring a Ventrue, she is treated as a such for all effects of the card, and only them, including duration effects. She is not treated as such for effects the card has from being in play. [ANK 20190228]"
-200503|Gengis (ADV):
+200316|Danielle Diron (G3):
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+200327|De Sade (G5):
+  - His ability applies only to the first time a vampire casts hist votes, not if they change afterwards (eg. {Kindred Manipulation}). [ANK 20221019]
+200333|Demdemeh (G4):
+  - The animal retainers turned into allies keep their current life counters and remember their original "starting life", for effects that notice "starting life". The retainers' special abilities are lost, as well as any continuous effect affecting them (eg. bonus from {Tainted Spring}). [LSJ 20051116-1] [LSJ 20081213-3]
+200335|Democritus (G1):
+  - Does not affect the cost to contest titles, since it is paid in vampire blood, not pool. [RTR 19950509]
+200357|Dominique (G2):
+  - If a location costs X blood, it would take X vandal counters to burn it. [LSJ 20001118]
+200360|Don Caravelli (G5):
+  - His ability to give a press can only be used during the press step. [PIB 20150121]
+200363|Don Michael Antonio Giovanni (G4):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+200364|Dónal O'Connor (G2):
+  - An empty blocking vampire may still block and will try and fail to burn a blood if the block is successful. [TOM 19951215-1]
+  - The blocking vampire burns 1 blood immediately upon successfully blocking Donal, regardless of whether combat begins. [RTR 19960530]
+200365|Donald Cargill (G5):
+  - His ability is applied after the referendum effects are applied, including any oust and pool gained from it. [LSJ 20090115-2]
+  - His ability is still applied if the predator is ousted by the referendum effects. [LSJ 20090115-2]
+200381|Dr. Morrow, The Skindoctor (G5):
+  - Multiple graft counters may be placed on the same minion, but they have no additional effect. A minion with one or more graft counters gets -1 stealth, not -X stealth. [LSJ 20070306]
+200383|Dr. Solomon Grey (G5):
+  - You burn one pool before he enters contest if there is another one in play. [LSJ 20080526]
+200386|Dragos (G2):
+  - If his opponent plays superior {Terror Frenzy}, Dragos does not burn one additional blood for combat card he plays (reversal of previous rulings). [LSJ 20090107]
+  - A "burn blood" effect on a combat card is not a cost (eg. {Chiropteran Marauder}), it is unaffected by his ability. [LSJ 20090107] [LSJ 20070829-3]
+200389|Drozodny (G5):
+  - When using his ability, the card to retrieve must be announced when declaring the action. [LSJ 20010627]
+200401|Edith Blount (G3):
+  - Edith may burn a blood to give {Enid Blount} stealth multiple times each action. [LSJ 20040617]
+200403|Edward Vignes (G3):
+  - His ability cannot be used if the action is blocked. [LSJ 20041022]
+200417|Ellison Humboldt (G3):
+  - Can use his ability only once per referendum. [ANK 20180307-2] [RBK 20200701-4]
+200424|Enkidu, The Noah (G4):
+  - He cannot attempt an action to equip nor strike to steal an equipment. [LSJ 20050315] [LSJ 20010210]
+  - He can equip with an equipment that is a location when in play. [LSJ 20050315]
+200427|Epikasta Rigatos (G4):
+  - Can only retrieve a card played during that same action. [ANK 20180628]
+  - Can only retrieve cards played the normal way, ie. not put into play as a result of another card (eg. {Concealed Weapon} or {Charming Lobby}). [LSJ 20090430] [ANK 20180628]
+200434|Erlik (G3):
+  - His "as he enters play" ability can be used before he enters contest (not after) if there is another one in play. [LSJ 20080526] [LSJ 20100902] [ANK 20180626-1]
+200438|Ethan Locke (G2):
+  - Ethan's action is directed at the controller of the skill card, not the controller of the vampire. [LSJ 19970224]
+  - When he steals a master Discipline card, his controller becomes the controller of the Discipline card. [LSJ 19990709]
+200439|Étienne Fauberge (G3):
+  - Allies have no blood, they cannot take directed actions against him, except if they are acting as a vampire. [LSJ 20030815]
+200443|Eurayle Gelasia Mylonas (G4):
+  - Her ability is undirect if you control the target, directed to the controller of the target otherwise. [PIB 20121210]
+200448|Eze, The Demon Prince (G3):
+  - His unlock ability is mandatory, it is applied even if the action unlocks him already. [LSJ 20051211]
+200450|Ezmerelda (G2):
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+200452|Fabrizia Contreraz (G4):
+  - She only gets her votes if your prey controls a ready Camarilla vampire. [PIB 20150713]
+200459|Fatima al-Faqadi (G2):
+  - Can only use her ability when she is in combat herself. [ANK 20221021]
+200485|Frondator (G4):
+  - The cost to rescue from torpor is reduced even if paid by the rescuee. This is not optional. [LSJ 20020304-2] [PIB 20110918]
+200498|Gem Ghastly (G5):
+  - When playing a card requiring a Ventrue, she is treated as a such for all effects of the card, and only them, including duration effects. She is not treated as such for effects the card has from being in play. [ANK 20190228]
+200501|Genevieve (G2):
+  - Her votes and ballots must be cast on the same side (for or against). [RBK 20200701-8] [LSJ 20051113-2]
+200503|Gengis (G3 ADV):
   - "[MERGED] Is Anarch. If the base version was the one in play, it changes sect as it is merged. [ANK 20180524]"
-200508|Gerald Windham:
-  - "His ability gives him votes but no title. [ANK 20190725]"
-200528|Goratrix:
-  - "Can steal 2 blood or life. [ANK 20190701]"
-200529|Goratrix (ADV):
+200504|Genina, The Red Poet (G3):
+  - She cannot play {Lay Low}. [ANK 20220810]
+200508|Gerald Windham (G5):
+  - His ability gives him votes but no title. [ANK 20190725]
+200528|Goratrix (G2):
+  - Can steal 2 blood or life. [ANK 20190701]
+200529|Goratrix (G2 ADV):
   - "[MERGED] Is Camarilla. If the base version was the one in play, it changes sect as it is merged. If it had an anarch token, it is burned. [ANK 20180524]"
-200534|Gratiano:
-  - "If {Fall of the Sabbat} is in play, Priscii do not benefit from their title and have no ballot. The Priscii subreferendum still happens and Gratiano benefits from his bonus ballot. [LSJ 20040519]"
-200545|Guillaume Giovanni:
-  - "His ability is not triggered when playing a Unique Location for contest. [LSJ 20080107]"
-200560|Hagar Stone:
-  - 'The "do not replace" effect stacks with whatever "do not replace" clause the card itself has, so that the longest one wins out. [LSJ 20070320-1]'
-200578|Hazimel:
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-200585|Helen Fairchild:
-  - "She cannot attempt an action to equip nor strike to steal an equipment. [LSJ 20050315] [LSJ 20010210]"
-  - "She can equip with an equipment that is a location when in play. [LSJ 20050315]"
-200587|Helena (ADV):
+200534|Gratiano (G2):
+  - If {Fall of the Sabbat} is in play, Priscii do not benefit from their title and have no ballot. The Priscii subreferendum still happens and Gratiano benefits from his bonus ballot. [LSJ 20040519]
+  - His votes (if any) and ballots must be cast on the same side (for or against). [RBK 20200701-8] [LSJ 20051113-2]
+200545|Guillaume Giovanni (G4):
+  - His ability is not triggered when playing a Unique Location for contest. [LSJ 20080107]
+200560|Hagar Stone (G5):
+  - The "do not replace" effect stacks with whatever "do not replace" clause the card itself has, so that the longest one wins out. [LSJ 20070320-1]
+200578|Hazimel (G4):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+200585|Helen Fairchild (G6):
+  - She cannot attempt an action to equip nor strike to steal an equipment. [LSJ 20050315] [LSJ 20010210]
+  - She can equip with an equipment that is a location when in play. [LSJ 20050315]
+200587|Helena (G3 ADV):
   - "[MERGED] Is Independant. If the base version was the one in play, it changes sect as it is merged. If it had an anarch token, it is burned. [ANK 20180524]"
   - "[MERGED] Immune means damage is not inflicted, even if non-preventable or outside combat. [LSJ 20010627] [LSJ 20010629] [LSJ 20090304-1]"
-200604|Horatio Ballard:
-  - "Cannot use his special ability to become a Prince if he has changed sect and is no longer Camarilla. [LSJ 20030202]"
-200606|Horrock:
-  - "Card with disciplines choices (eg. [pro]/[obf]) are considered of the discipline they are played as. [PIB 20150924-2]"
-200607|Howler:
-  - "She cannot attempt an action to equip a weapon nor strike to steal a weapon. [LSJ 20050315] [LSJ 20010210]"
-200608|Hrothulf:
-  - "Only burns the Edge if the action is successful. [LSJ 20030519]"
-200612|Hukros:
-  - "He can accumulate as many cards as he likes with his special, at the rate of one each unlock. [LSJ 20070320-2]"
-200616|Ian Forestal:
-  - "His ability can be used to meet one (not both) of the normal Discipline requirements of a multi-Discipline card. [LSJ 20011217]"
-200625|Igo the Hungry:
-  - "His ability only applies to the default rulebook hunt action (eg. he gets {Loki's Gift} +1 stealth). [PIB 20150820-2]"
-200630|Imanna:
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-200632|Inez "Nurse216" Villagrande:
-  - 'Her "as she enters play" ability can be used before she enters contest if there is another one in play. [LSJ 20080526]'
-200634|Ingrid Rossler:
-  - "When she is influenced out, her bonus transfers do not apply for the ongoing influence phase. [RTR 20180303]"
-200666|Jalal Sayad:
-  - "If his ability is used to start a new combat, effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]"
-  - "His ability cannot be used to start a new combat if there is already a pending combat queued. [RTR 20020501]"
-200668|Jamal:
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-200670|Jan Pieterzoon (ADV):
+200590|Henry Taylor (G3):
+  - A card with multiple types (eg. {Swallowed by the Night}) needs to have been played as a combat card to be eligible. [LSJ 20031221]
+200592|Hermana Hambrienta Mayor (G4):
+  - If influenced with more blood than her capacity, the blood drain off before her ability forces her to burn 2. [LSJ 20051126]
+200593|Hermana Hambrienta Menor (G4):
+  - If influenced with more blood than her capacity, the blood drain off before her ability forces her to burn 2. [LSJ 20051126]
+200604|Horatio Ballard (G3):
+  - Cannot use his special ability to become a Prince if he has changed sect and is no longer Camarilla. [LSJ 20030202]
+200606|Horrock (G3):
+  - Card with disciplines choices (eg. [pro]/[obf]) are considered of the discipline they are played as. [PIB 20150924-2]
+200607|Howler (G2):
+  - She cannot attempt an action to equip a weapon nor strike to steal a weapon. [LSJ 20050315] [LSJ 20010210]
+200608|Hrothulf (G3):
+  - Only burns the Edge if the action is successful. [LSJ 20030519]
+200612|Hukros (G4):
+  - He can accumulate as many cards as he likes with his special, at the rate of one each unlock. [LSJ 20070320-2]
+200616|Ian Forestal (G2):
+  - His ability can be used to meet one (not both) of the normal Discipline requirements of a multi-Discipline card. [LSJ 20011217]
+200625|Igo the Hungry (G1):
+  - His ability only applies to the default rulebook hunt action (eg. he gets {Loki's Gift} +1 stealth). [PIB 20150820-2]
+200630|Imanna (G6):
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+200632|Inez "Nurse216" Villagrande (G4):
+  - Her "as she enters play" ability can be used before she enters contest if there is another one in play. [LSJ 20080526]
+200634|Ingrid Rossler (G2):
+  - When she is influenced out, her bonus transfers do not apply for the ongoing influence phase. [RTR 20180303]
+200665|Jaggedy Andy (G4):
+  - If he goes to torpor and their controller cannot discard two cards, they discard as many as they can. [ANK 20211010]
+200666|Jalal Sayad (G2):
+  - If his ability is used to start a new combat, effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501]
+  - His ability cannot be used to start a new combat if there is already a pending combat queued. [RTR 20020501]
+200668|Jamal (G5):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+200670|Jan Pieterzoon (G2 ADV):
   - "[MERGED] Is Independant. If the base version was the one in play, it changes sect as it is merged. If it had an anarch token, it is burned. [ANK 20180524]"
-200671|Jane Sims:
-  - "Card with multiple types (eg. Combat/Action Modifer) are considered of the type they are played as, not both. [PIB 20150924-2]"
-200678|Jaroslav Pascek:
-  - "When using the action provided by his ability, if some minions cannot be targeted because of another effect, the action will simply have no effect on the things it cannot target. [RTR 20080808]"
-200688|Jenna Cross:
-  - "If a cost reduction applies (eg. {Salvador Garcia}), the controller can choose to apply it first so that her ability does not kick in. [ANK 20200709]"
-200705|Jimmy Dunn:
-  - "If a second Jimmy Dunn is brought out during an action, and the first Jimmy (if he has Vicissitude) plays {Reform Body}, the first Jimmy will go to torpor (from Reform Body), but will then be burned anyhow, since he cannot be contested. [LSJ 19990719] [RTR 19991001]"
-  - 'If a second Jimmy Dunn is brought out during an action, the acting vampire is not considered to be "burning" the first Jimmy. [LSJ 19990719] [RTR 19991001]'
-  - "If a non-contesting second copy of Jimmy enters play (via {Illusions of the Kindred}, for example), the first Jimmy won't burn himself. [LSJ 19991110]"
-200720|Josef von Bauren:
-  - "His ability can be used multiple times if one hase multiple discard phase actions. [ANK 20190725]"
-200742|Kahina the Sorceress:
-  - "Her ability inflicts a total of one damage to a a minion with one or more corruption counters. [LSJ 20030820]"
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-200753|Karen Suadela:
-  - "She keeps her title if {Fall of the Camarilla} is played. She can be chosen for {Recalled to the Founder}, but does not burn. Allies still benefit trom {The Unmasking} intercept when trying to block her. [LSJ 20081120-2]"
-200754|Karif al Numair:
-  - "His ability applies when he is in torpor. [LSJ 20011022] [LSJ 20100902-2]"
-200758|Karsh (ADV):
+200671|Jane Sims (G4):
+  - Card with multiple types (eg. Combat/Action Modifer) are considered of the type they are played as, not both. [PIB 20150924-2]
+200678|Jaroslav Pascek (G3):
+  - When using the action provided by his ability, if some minions cannot be targeted because of another effect, the action will simply have no effect on the things it cannot target. [RTR 20080808]
+200688|Jenna Cross (G4):
+  - If a cost reduction applies (eg. {Salvador Garcia}), the controller can choose to apply it first so that her ability does not kick in. [ANK 20200709]
+200705|Jimmy Dunn (G2):
+  - Can be influenced out if you already control one. [RTR 20180303]
+  - If a second Jimmy Dunn is brought out during an action, and the first Jimmy (if he has Vicissitude) plays {Reform Body}, the first Jimmy will go to torpor (from Reform Body), but will then be burned anyhow, since he cannot be contested. [LSJ 19990719] [RTR 19991001]
+  - If a second Jimmy Dunn is brought out during an action, the acting vampire is not considered to be "burning" the first Jimmy. [LSJ 19990719] [RTR 19991001]
+  - If a non-contesting second copy of Jimmy enters play (via {Illusions of the Kindred}, for example), the first Jimmy won't burn himself. [LSJ 19991110]
+200720|Josef von Bauren (G4):
+  - His ability can be used multiple times if one hase multiple discard phase actions. [ANK 20190725]
+200742|Kahina the Sorceress (G3):
+  - Her ability inflicts a total of one damage to a a minion with one or more corruption counters. [LSJ 20030820]
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+200753|Karen Suadela (G5):
+  - She keeps her title if {Fall of the Camarilla} is played. She can be chosen for {Recalled to the Founder}, but does not burn. Allies still benefit trom {The Unmasking} intercept when trying to block her. [LSJ 20081120-2]
+200754|Karif al Numair (G5):
+  - His ability applies when he is in torpor. [LSJ 20011022] [LSJ 20100902-2]
+200758|Karsh (G3 ADV):
   - "[MERGED] Imperator is a unique Camarilla title worth 3 votes, it is the same as the one granted by {Imperator}. [ANK 20190407]"
-200759|Kashan:
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-200763|Kateline Nadasdy:
-  - "Her ability applies to Priscus votes and ballots. [LSJ 19971001]"
-  - "Her ability to force a vampire to abstain can cancel the votes and ballots of the vampire. [LSJ 20100311]"
-200770|Kemintiri (ADV):
+200759|Kashan (G4):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+200763|Kateline Nadasdy (G4):
+  - Her ability applies to Priscus votes and ballots. [LSJ 19971001]
+  - Her ability to force a vampire to abstain can cancel the votes and ballots of the vampire. [LSJ 20100311]
+200770|Kemintiri (G2 ADV):
   - "[MERGED] Keeps her title and votes if she changes sects. [LSJ 20010714]"
   - "[MERGED] When playing a card requiring Camarilla, Ventrue and/or justicar, she is treated as a such for all effects of the card, and only them, including duration effects. She is not treated as such for effects the card has from being in play. [ANK 20190228] [LSJ 20101013]"
+  - "[MERGED] If she plays a political action requiring a Justicar, she is not seen as such by other cards or effects during the referendum (eg. if another vampire plays {Closed Session} and she's not Camarilla she will not be able to vote. If she plays it, she can vote). [LSJ 20050128-2] [ANK 20221011-4] [RTR 20070707]"
   - "[MERGED] Does not enable you to play master cards, it only enables her to play certain minion cards. [LSJ 20050721]"
   - "[MERGED] When considered a justicar, she is also implicitly considered Camarilla. [LSJ 20050128]"
-"200773|Kephamos, High Priest of Marrakech":
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-200775|Kestrelle Hayes:
-  - "Gets +1 stealth on Ⓓ actions against multiple Methuselahs if one or more of the targets control no ready Sabbat vampire. [PIB 20150526] [RTR 20080808]"
-200798|Kyoko Shinsegawa:
-  - "The action provided is a hunt action and benefit from hunt bonuses. [LSJ 20030311] [LSJ 20090113-2]"
-  - "If other hunt actions are granted, she may choose from among those options. [LSJ 20060306]"
-  - "She cannot steal more blood than the target has when using a special hunt ability. [LSJ 20100915]"
-  - "Cannot choose to target a vampire when using another non-standard hunt action (eg. {Abactor}). [LSJ 20090606]"
-200804|Lady Constancia:
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-200811|Lambach (ADV):
-  - 'The provided action is an "equip action" [TOM 19960130]'
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
+200773|Kephamos, High Priest of Marrakech (G2):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+200775|Kestrelle Hayes (G5):
+  - Gets +1 stealth on actions directed at multiple Methuselahs if one or more of the targets control no ready Sabbat vampire. [PIB 20150526] [RTR 20080808]
+200780|Khay'tall, Snake of Eden (G2):
+  - If a minion gains a corruption counter after they cast their votes (eg. [ser] {Velvet Tongue}), their votes are cancelled and they're forced to abstain instead. [PIB 20141226]
+200793|Krassimir (G2):
+  - When he cancels an action, it has reached resolution, so is subject to NRA (Non Repeatable Action) rules. [LSJ 20011202-2]
+200798|Kyoko Shinsegawa (G3):
+  - The action provided by her ability is a hunt action and benefit from hunt bonuses. [LSJ 20030311] [LSJ 20090113-2]
+  - She can only perform the action provided by her ability once per turn. [PIB 20121112]
+  - If other hunt actions are granted, she may choose from among those options. [LSJ 20060306]
+  - She cannot steal more blood than the target has when using a special hunt ability. [LSJ 20100915]
+  - Cannot choose to target a vampire when using another non-standard hunt action (eg. {Abactor}). [LSJ 20090606]
+200804|Lady Constancia (G4):
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+200811|Lambach (G2 ADV):
+  - The provided action is an "equip action" [TOM 19960130]
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
   - "[MERGED] Is Independant. If the base version was the one in play, it changes sect as it is merged. If it had an anarch token, it is burned. [ANK 20180524]"
-200819|Lázár Dobrescu:
-  - "Cannot use his special ability if his controller has no vampires in her uncontrolled region. [LSJ 19990215]"
-200821|Lazarus (ADV):
+200819|Lázár Dobrescu (G2):
+  - Cannot use his special ability if his controller has no vampires in her uncontrolled region. [LSJ 19990215]
+200821|Lazarus (G1 ADV):
   - "[MERGED] His ability to get a press can only be used during the press step. [PIB 20150121]"
-200824|Le Dinh Tho:
-  - "When using his ability, you do not get to see the card drawn as replacement. [PIB 20121031]"
-200826|Leandro:
-  - "Choice is mandatory, there is no default. If all players forget, forcing one choice or the other on the victim is not a suitable remedy. [LSJ 20021210-1]"
-  - "When a Methusalah decides to get no transfer, he can still use other effects that put blood on his uncontrolled vampires (eg. [DOM] {Govern the Unaligned}, {Powerbase: Montreal}). [LSJ 20100527]"
-200840|Lisandro Giovanni:
-  - "When playing a card requiring a Ventrue antitribu or a Samedi, he is treated as a such for all effects of the card, and only them, including duration effects. He is not treated as such for effects the card has from being in play (eg. {Houngan} can be played on him, but he does not get blood and cannot lock to get blood). [ANK 20190228] [PIB 20141006]"
-  - "You can still use the burn options of cards with a requirement he could meet when you play them, but does not meet while in play. [LSJ 20050225]"
-  - "Cannot be treated as a Ventrue antitribu nor a Samedi while uncontrolled or in the crypt (eg. {Coroner's Contact} cannot fetch him). [PIB 20150530]"
-200856|Lord Tremere:
-  - "His unlocking ability can be used when he is in torpor. [LSJ 20011022] [LSJ 20100902-2]"
-200859|Lorrie Dunsirn:
-  - "Her press and additional strike are mandatory. [LSJ 20051016] [LSJ 20051017]"
-  - "She cannot attempt an action to equip or employ, nor strike to steal an equipment or retainer. [LSJ 20050315] [LSJ 20010210]"
-  - "She can equip with an equipment that is a location when in play. [LSJ 20050315]"
-200863|Louis Fortier (ADV):
+200824|Le Dinh Tho (G2):
+  - When using his ability, you do not get to see the card drawn as replacement. [PIB 20121031]
+200826|Leandro (G2):
+  - Choice is mandatory, there is no default. If all players forget, forcing one choice or the other on the victim is not a suitable remedy. [LSJ 20021210-1]
+  - "When a Methuselah decides to get no transfer, he can still use other effects that put blood on his uncontrolled vampires (eg. [DOM] {Govern the Unaligned}, {Powerbase: Montreal}). [LSJ 20100527]"
+200840|Lisandro Giovanni (G3):
+  - When playing a card requiring a Ventrue antitribu or a Samedi, he is treated as a such for all effects of the card, and only them, including duration effects. He is not treated as such for effects the card has from being in play (eg. {Houngan} can be played on him, but he does not get blood and cannot lock to get blood). [ANK 20190228] [PIB 20141006]
+  - You can still use the burn options of cards with a requirement he could meet when you play them, but does not meet while in play. [LSJ 20050225]
+  - Cannot be treated as a Ventrue antitribu nor a Samedi while uncontrolled or in the crypt (eg. {Coroner's Contact} cannot fetch him). [PIB 20150530]
+200844|Little Tailor of Prague (G2):
+  - His ability works on allies recruited in a non-standard way (eg. {Piper}). [ANK 20210913] [LSJ 20090116]
+200852|Lord Aaron Wesley Wilkshire (G4):
+  - The methusalem playing the frenzy card chooses if the cost is paid in blood or pool. [LSJ 20060831]
+200856|Lord Tremere (G5):
+  - His unlocking ability can be used when he is in torpor. [LSJ 20011022] [LSJ 20100902-2]
+200858|Lorenzo Detuono (G5):
+  - Cannot use his ability after {Amaranth} resolves. [ANK 20210705]
+200859|Lorrie Dunsirn (G4):
+  - Her press and additional strike are mandatory. [LSJ 20051016] [LSJ 20051017]
+  - She cannot attempt an action to equip or employ, nor strike to steal an equipment or retainer. [LSJ 20050315] [LSJ 20010210]
+  - She can equip with an equipment that is a location when in play. [LSJ 20050315]
+200863|Louis Fortier (G4 ADV):
   - "[MERGED] Is Anarch. If the base version was the one in play, it changes sect as it is merged. [ANK 20180524]"
-200865|Lubomira Hradok:
-  - "Lubomira is the one not to unlock as normal. [PIB 20110915-1]"
-200870|Lucian:
-  - "Cannot attempt to steal a piece of equipment that he is prohibited from having (eg. a second {Leather Jacket}). [LSJ 19980206]"
-  - "The stolen equipment cannot be used until the next round. [LSJ 19980206] [RBK 20181001-645]"
-"200871|Lucian, the Perfect":
-  - "Strikes that do not target him (dodge, combat ends) do not cost more. They do if they plan to damage him after combat (eg. [PRE] {Catatonic Fear}). They do not if they target a card on him (eg. {Target Retainer}, {Canine Horde}). [LSJ 20090528-2] [LSJ 20031118]"
-  - "Strikes the opponent commits to during the determine range phase (by using an optional maneuver) cost more, but the card itself does not (eg. {Jann Berger} pays 1 blood for a {Thrown Gate} played for the maneuver, but zero if he plays it when choosing his strike). [LSJ 20090529]"
-200885|Luna Giovanni:
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-  - "Her ability does not apply to the political action card played for a current action (it is in limbo). [LSJ 20070927]"
-200890|Lutz von Hohenzollern:
-  - "His ability is applied after the referendum effects are applied, including any oust and pool gained from it. [LSJ 20090115-2]"
-  - "His ability is still applied if his controller is ousted by the referendum effects. [LSJ 20090115-2]"
-"200891|Lydia, Grand Praetor":
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-200912|Marcia Felicia Licinia:
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-"200913|Marciana Giovanni, Investigator":
-  - "She can lock to grant herself the ability to burn blood for intercept. She would need a wake or unlock effect to attempt to block. [LSJ 20100527]"
-  - "The beneficiary of her ability can choose to burn a blood for intercept for the duration of the action. [LSJ 20100604-2] [LSJ 20100611]"
-  - "Her ability to give intercept can be used when she is in torpor. [LSJ 20010813-2]"
-200916|Marcus Vitel (ADV):
+200865|Lubomira Hradok (G5):
+  - Lubomira is the one not to unlock as normal. [PIB 20110915-1]
+200870|Lucian (G1):
+  - Cannot attempt to steal a piece of equipment that he is prohibited from having (eg. a second {Leather Jacket}). [LSJ 19980206]
+  - The stolen equipment cannot be used until the next round. [LSJ 19980206] [RBK 20200701-7]
+200871|Lucian, the Perfect (G4):
+  - Strikes that do not target him (dodge, combat ends) do not cost more. They do if they plan to damage him after combat (eg. [PRE] {Catatonic Fear}). They do not if they target a card on him (eg. {Target Retainer}, {Canine Horde}). [LSJ 20090528-2] [LSJ 20031118]
+  - Strikes the opponent commits to during the determine range phase (by using an optional maneuver) cost more, but the card itself does not (eg. {Jann Berger} pays 1 blood for a {Thrown Gate} played for the maneuver, but zero if he plays it when choosing his strike). [LSJ 20090529]
+200885|Luna Giovanni (G5):
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+  - Her ability does not apply to the political action card played for a current action (it is in limbo). [LSJ 20070927]
+200890|Lutz von Hohenzollern (G4):
+  - His ability is applied after the referendum effects are applied, including any oust and pool gained from it. [LSJ 20090115-2]
+  - His ability is not applied if his controller is ousted by the referendum effects (reversal of previous rulings). [ANK 20220808]
+200891|Lydia, Grand Praetor (G6):
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+200912|Marcia Felicia Licinia (G5):
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+200913|Marciana Giovanni, Investigator (G2):
+  - She can lock to grant herself the ability to burn blood for intercept. She would need a wake or unlock effect to attempt to block. [LSJ 20100527]
+  - The beneficiary of her ability can choose to burn a blood for intercept for the duration of the action. [LSJ 20100604-2] [LSJ 20100611]
+  - Her ability to give intercept can be used when she is in torpor. [LSJ 20010813-2]
+200916|Marcus Vitel (G3 ADV):
   - "[MERGED] Is Sabbat. If the base version was the one in play, it changes sect as it is merged. If it had an anarch token, it is burned. [ANK 20180524]"
-200921|Marguerite Foccart (ADV):
+200921|Marguerite Foccart (G4 ADV):
   - "[MERGED] Is Anarch. If the base version was the one in play, it changes sect as it is merged. [ANK 20180524]"
-200927|Marie Faucigny:
-  - "The reduction applies to equipments that are locations (eg. {Palatial Estate}). [LSJ 20080109]"
-200928|Marie-Pierre:
-  - 'Her ability must be used after combat has ended, cards that are played "when the combat would end" or "when combat is about to end" are played before that. [ANK 20180928-2]'
-  - "When using her ability to enter combat she is not acting and cannot play action modifiers. {Obedience} cannot be played by the opponent. [ANK 20180929]"
-  - "When using her ability to enter combat, effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501] [ANK 20180928-2]"
-"200929|Mariel, Lady Thunder":
-  - "If she locks to end combat, the damage is applied just after the combat ends. [RTR 19970630]"
-  - "Her ability to end combat can be used when she is in torpor. [LSJ 20011022]"
-200935|Maris Streck:
-  - "Can use her ability multiple times each action. [LSJ 20020926] [ANK 20180307-2]"
-200942|Marthe Dizier:
-  - "Her ability can only move cards from the ash heap that were played in the normal manner. If the card was put in play in some other way, it cannot be retrieved by her special. [LSJ 20041119]"
-  - "A card canceled as it is played is still considered played, she can retrieve it. [LSJ 19980212] [ANK 20190701]"
-200945|Marty Lechtansi:
-  - "His ability to get a press can only be used during the press step. [PIB 20150121]"
-200955|Mata Hari:
-  - "Orun and Aye cards cannot be placed on her as long as she's not a Laibon. [LSJ 20110611]"
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-  - "When playing a card requiring a sect and/or a clan, she is treated as a such for all effects of the card, and only them, including duration effects. She is not treated as such for effects the card has from being in play. [ANK 20190228]"
-  - "When playing a card requiring a sect, her title makes her a titled vampire of that sect (eg. she can play {Hand Intervention}). [LSJ 20050526]"
-  - "If her capacity is above 10 when playing {Call the Great Beast}, she burns and it is put into play. If her capacity is less, the card is put on her with tokens equal to her capacity, but she will not be able to add counters to it later on. [ANK 20180723]"
-  - "You can still use the burn options of cards with a requirement she could meet when you play them, but does not meet while in play. [LSJ 20050225]"
-  - "Her ability do not let her fulfill card requirements if they are not played normally, like when using {Concealed Weapon} for an equipment or {Piper} or {The Summoning} for an ally. [LSJ 20050119]"
-"200960|Matteus, Flesh Sculptor":
-  - "Can use his ability to get intercept multiple times during the same action. [ANK 20180307-2]"
-"200964|Maureen, Dark Priestess":
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-200966|Maxwell:
-  - "Cannot use his ability to become a Prince if he has changed sect and is no longer Camarilla. [LSJ 20030202]"
-200976|Menele (ADV):
+200927|Marie Faucigny (G3):
+  - The reduction applies to equipments that are locations (eg. {Palatial Estate}). [LSJ 20080109]
+200928|Marie-Pierre (G6):
+  - Her ability must be used after combat has ended, cards that are played "when the combat would end" or "when combat is about to end" are played before that. [ANK 20180928-2]
+  - When using her ability to enter combat she is not acting and cannot play action modifiers. {Obedience} cannot be played by the opponent. [ANK 20180929]
+  - When using her ability to enter combat, effects that end combat and then do something else after combat (include continuing the action as if unblocked) will be lost, except for unlock effects. [LSJ 19980109] [RTR 20020501] [ANK 20180928-2]
+200929|Mariel, Lady Thunder (G1):
+  - If she locks to end combat, the damage is applied just after the combat ends. [RTR 19970630]
+  - Her ability to end combat can be used when she is in torpor. [LSJ 20011022]
+200935|Maris Streck (G3):
+  - Can use her ability multiple times each action. [LSJ 20020926] [ANK 20180307-2]
+  - Can use her ability while locked. [ANK 20220705]
+200942|Marthe Dizier (G3):
+  - Her ability can only move cards from the ash heap that were played in the normal manner. If the card was put in play in some other way, it cannot be retrieved by her special. [LSJ 20041119]
+  - A card canceled as it is played is still considered played, she can retrieve it. [LSJ 19980212] [ANK 20190701]
+  - She can retrieve {Psyche!} (reversal of previous rulings). [PIB 20111208]
+200945|Marty Lechtansi (G1):
+  - His ability to get a press can only be used during the press step. [PIB 20150121]
+200955|Mata Hari (G4):
+  - Orun and Aye cards cannot be placed on her as long as she's not a Laibon. [LSJ 20110611]
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+  - When playing a card requiring a sect and/or a clan, she is treated as a such for all effects of the card, and only them, including duration effects. She is not treated as such for effects the card has from being in play. [ANK 20190228]
+  - When playing a card requiring a sect, her title makes her a titled vampire of that sect (eg. she can play {Hand Intervention}). [LSJ 20050526]
+  - If her capacity is above 10 when playing {Call the Great Beast}, she burns and it is put into play. If her capacity is less, the card is put on her with tokens equal to her capacity, but she will not be able to add counters to it later on. [ANK 20180723]
+  - You can still use the burn options of cards with a requirement she could meet when you play them, but does not meet while in play. [LSJ 20050225]
+  - Her ability do not let her fulfill card requirements if they are not played normally, like when using {Concealed Weapon} for an equipment or {Piper} or {The Summoning} for an ally. [LSJ 20050119]
+200960|Matteus, Flesh Sculptor (G2):
+  - Can use his ability to get intercept multiple times during the same action. [ANK 20180307-2]
+200964|Maureen, Dark Priestess (G4):
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+200966|Maxwell (G3):
+  - Cannot use his ability to become a Prince if he has changed sect and is no longer Camarilla. [LSJ 20030202]
+200976|Menele (G3 ADV):
   - "[MERGED] Is Independant. If the base version was the one in play, it changes sect as it is merged. If it had an anarch token, it is burned. [ANK 20180524]"
-200979|Merrill Molitor:
-  - "The damage he treats as normal is handled before any aggravated damage that is being treated as aggravated damage. [LSJ 20030213]"
-  - "If an aggravated damage is inflicted with {Target Vitals}, the additional damages are still aggravated. [LSJ 20100527]"
-200981|Michael diCarlo:
-  - "When setting the range for the round, no other effect can be used to reset the range, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]"
-200982|Michael Luther:
-  - "His ability is only usable once each referendum, even if he unlocks somehow during the referendum. [LSJ 20041207]"
-200995|Miriam Benyona:
-  - "The cost to rescue from torpor is reduced even if paid by the rescuee. This is not optional. [LSJ 20020304-2]"
-201006|Montano:
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-"201017|Muaziz, Archon of Ulugh Beg":
-  - "Her ability does not apply to the {Blood Hunt} card. [TOM 19960604]"
-"201026|Mustafa, The Heir":
-  - "If two Methuselahs want to use abilities to alter Mustafa's votes at the same time, whoever uses the ability first has priority. Whoever uses it last has the final say on his votes. [LSJ 20090304-2]"
-201030|Nahir:
-  - "The hand size is still +X if Nahir is in torpor. [ANK 20191218]"
-  - "Can use her ability multiple times during the same master phase if there are multiple master phase actions. [ANK 20191218]"
-201043|Neferu:
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-  - "Cannot use her ability to force an abstaining vampire to vote. [ANK 20190731]"
-201044|Nehemiah:
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-201045|Nehsi:
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-201049|Nergal (ADV):
-  - "Card with multiple types (eg. Reaction/Action Modifer) are considered of the type they are played as, not both. [PIB 20150924-2]"
-201052|New Blood:
-  - "A vampire with no circle designation is in his own unique circle of one. New blood cannot choose to be part of such a circle. [LSJ 20020609]"
-  - 'Cannot choose to be part of the "Inner Circle" and get the title. The Inner Circle title and a Blood Brothers circle are different things. [ANK 20190117-2]'
-"201087|Owain Evans, The Wanderer":
-  - "His ability can only be used once each unlock, even if control of Owain changes during that unlock phase. [LSJ 20040127]"
-  - "His ability can only be used when his controller has the opportunity to play effects. The acting player has to apply all mandatory effects (eg. lose pool to {Anarch Revolt}) before passing the opportunity to play effects to another player. [LSJ 20100723]"
-201094|Pariah:
-  - "Can use card-provided undirected hunt actions (eg. {Vulture's Buffet}). [ANK 20180202]"
-  - "His ability still applies when in torpor. [LSJ 20011022] [LSJ 20100902-2]"
-"201098|Patrizia Giovanni, Collector of Secrets":
-  - "When using her ability, the card to retrieve must be announced when declaring the action. [LSJ 20010627]"
-201103|Paul "Sixofswords29" Moreton:
-  - "When he is influenced out, his ability can be used during the ongoing influence phase. [RTR 20180303]"
-201112|Petaniqua:
-  - "Additional damage done before range by her ability is environmental. [RTR 19970630]"
-201113|Petaniqua (ADV):
-  - "When recruit a werewolf ally, she is treated as a meeting the requirements for all effects of the card, and only them, including duration effects. She is not treated as meeting the requirements for effects the card has from being in play. [ANK 20190228]"
-  - "You can still use the burn options of cards with a requirement she could meet when you play them, but does not meet while in play. [LSJ 20050225]"
-  - "Her ability do not let her fulfill card requirements if they are not played normally, like when using {Piper}. [LSJ 20050119]"
-  - "Her ability to get a press can only be used during the press step. [PIB 20150121]"
+200979|Merrill Molitor (G1):
+  - The damage he treats as normal is handled before any aggravated damage that is being treated as aggravated damage. [LSJ 20030213]
+  - If an aggravated damage is inflicted with {Target Vitals}, the additional damages are still aggravated. [LSJ 20100527]
+200981|Michael diCarlo (G4):
+  - When setting the range for the round, no other effect can be used to reset the range, but other pre-range effects can be played afterwards. [RTR 19970630] [ANK 20180720]
+200982|Michael Luther (G3):
+  - His ability is only usable once each referendum, even if he unlocks somehow during the referendum. [LSJ 20041207]
+200983|Michaela (G5):
+  - Can only use her ability when she is in combat herself. [ANK 20221021]
+200995|Miriam Benyona (G2):
+  - The cost to rescue from torpor is reduced even if paid by the rescuee. This is not optional. [LSJ 20020304-2]
+201006|Montano (G3):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+  - His ability to provide stealth can be used while locked or in torpor. [ANK 20220705] [LSJ 20100705]
+201017|Muaziz, Archon of Ulugh Beg (G2):
+  - Her ability does not apply to the {Blood Hunt} card. [TOM 19960604]
+201021|Mukhtar Bey (G4):
+  - He can play {Trap} and it provides presses. [LSJ 20040521]
+201026|Mustafa, The Heir (G4):
+  - If two Methuselahs want to use abilities to alter Mustafa's votes at the same time, whoever uses the ability first has priority. Whoever uses it last has the final say on his votes. [LSJ 20090304-2]
+201030|Nahir (G3):
+  - The hand size is still +X if Nahir is in torpor. [ANK 20191218]
+  - Can use her ability multiple times during the same master phase if there are multiple master phase actions. [ANK 20191218]
+201033|Nakhthorheb (G4):
+  - If the block succeeds and the blocking minion gets a corruption counter (eg. {Venenation}), Nakhthorheb is still blocked. [LSJ 20071021]
+201043|Neferu (G4):
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+  - Cannot use her ability to force an abstaining vampire to vote. [ANK 20190731]
+201044|Nehemiah (G4):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+201045|Nehsi (G2):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+201048|Nergal (G5):
+  - If he plays a action he can only pay for with his ability, he has to use his ability when the action resolves (even if a {Deflection} was played on a bleed). [LSJ 20091021-2]
+  - If he lost a blood during the course of an action that he could have paid for when announced, he can choose wether or not to use his ability to be able to pay for it. [LSJ 20091021-2]
+  - If he cannot pay for the action even with his ability, his ability is not considered used for the action (even if it was announced). [LSJ 20091021-2]
+  - If a card he plays is cancelled as it played and no cost is paid, his ability is not considered used for the turn. [LSJ 20091021-2]
+201049|Nergal (G5 ADV):
+  - Card with multiple types (eg. Reaction/Action Modifer) are considered of the type they are played as, not both. [PIB 20150924-2]
+201052|New Blood (ANY):
+  - A vampire with no circle designation is in his own "unique circle of one". [LSJ 20020609] [ANK 20211113]
+  - New Blood can be in the "unique circle of one" of any vampire, including another copy of himself. Two uncontrolled New Bloods are in different circles (eg. for {Unwholesome Bond}). [ANK 20211113]
+  - Cannot choose to be part of the "Inner Circle" and get the title. The Inner Circle title and a Blood Brothers circle are different things. [ANK 20190117-2]
+201087|Owain Evans, The Wanderer (G3):
+  - His ability can only be used once each unlock, even if control of Owain changes during that unlock phase. [LSJ 20040127]
+  - His ability can only be used when his controller has the opportunity to play effects. The acting player has to apply all mandatory effects (eg. lose pool to {Anarch Revolt}) before passing the opportunity to play effects to another player. [LSJ 20100723]
+201094|Pariah (G2):
+  - Can use card-provided undirected hunt actions (eg. {Vulture's Buffet}). [ANK 20180202]
+  - His ability still applies when in torpor. [LSJ 20011022] [LSJ 20100902-2]
+201095|Parmenides (G2):
+  - He comes back as the unlock phase begins and unlocks as normal. [LSJ 20010622]
+  - If two are influenced in the same turn, the second is burned (self-contestinging on the predator's end). [LSJ 20010623-2]
+  - If the owner is ousted before Parmenides comes back, the predator keeps control of him indefinitely. [LSJ 20021111]
+201098|Patrizia Giovanni, Collector of Secrets (G2):
+  - When using her ability, the card to retrieve must be announced when declaring the action. [LSJ 20010627]
+201102|Paul Forrest, False Prophet (G4):
+  - His ability can be used while locked or in torpor. [ANK 20220705] [LSJ 20100705]
+201103|Paul "Sixofswords29" Moreton (G4):
+  - When he is influenced out, his ability can be used during the ongoing influence phase. [RTR 20180303]
+201112|Petaniqua (G4):
+  - Additional damage done before range by her ability is environmental. [RTR 19970630]
+201113|Petaniqua (G4 ADV):
+  - When recruit a werewolf ally, she is treated as a meeting the requirements for all effects of the card, and only them, including duration effects. She is not treated as meeting the requirements for effects the card has from being in play. [ANK 20190228]
+  - You can still use the burn options of cards with a requirement she could meet when you play them, but does not meet while in play. [LSJ 20050225]
+  - Her ability do not let her fulfill card requirements if they are not played normally, like when using {Piper}. [LSJ 20050119]
+  - Her ability to get a press can only be used during the press step. [PIB 20150121]
   - "[MERGED] Is Independant. If the base version was the one in play, it changes sect as it is merged. If it had an anarch token, it is burned. [ANK 20180524]"
-201121|Philip van Vermeer IV:
-  - "When playing a card requiring a Ventrue, he is treated as a such for all effects of the card, and only them, including duration effects. He is not treated as such for effects the card has from being in play. [ANK 20190228]"
-  - "His ability do not let him fulfill card requirements if they are not played normally, like when using {Piper} to recruit an ally. [LSJ 20050119]"
-201123|Phillipe Rigaud:
+201121|Philip van Vermeer IV (G2):
+  - When playing a card requiring a Ventrue, he is treated as a such for all effects of the card, and only them, including duration effects. He is not treated as such for effects the card has from being in play. [ANK 20190228]
+  - His ability do not let him fulfill card requirements if they are not played normally, like when using {Piper} to recruit an ally. [LSJ 20050119]
+201123|Phillipe Rigaud (G4):
   - 'If he cannot commit diablerie, then his card text does not force him to: he is not "stuck", he is free to take any other legal action. [LSJ 20050514]'
-201127|Pochtli:
-  - "When using his ability, the card to retrieve must be announced when declaring the action. [LSJ 20010627]"
-201129|Porphyrion:
-  - 'His "as he enters play" ability can be used before he enters contest if there is another one in play. [LSJ 20080526]'
-201132|Prejudice:
-  - "Can only use his ability when he is bleeding. [ANK 20180514]"
-  - "He is the one to get the bleed bonus. [ANK 20180511-2]"
-201136|Pugfar:
-  - "His ability to give a press can only be used during the press step. [PIB 20150121]"
-201138|Qawiyya el-Ghaduba:
-  - "Her ability can be used only once per minion phase. [ANK 20190207] [RBK 20181001-11]"
-"201144|Quincy, The Trapper":
-  - "His ability means he must perform the same action twice in two different turns. Tokens can be used to keep track of it if players agree. [ANK 20170202]"
-"201147|Rabbat, The Sewer Goddess":
-  - "Her hunt ability may be used even when she is at full capacity. One blood goes to your pool directly even if it would have exceeded her capacity. [LSJ 20050331]"
-201148|Rachel Brandywine:
-  - "When using her ability, make all discards and redraws first, then shuffle the discards back into the library. [RTR 20030519]"
-201160|Randall:
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-201164|Raphael Catarari:
+  - As long as there is an opportunity for diablerie, he must attempt it, even if he did so already and unlocked. [ANK 20211010]
+201127|Pochtli (G2):
+  - When using his ability, the card to retrieve must be announced when declaring the action. [LSJ 20010627]
+201129|Porphyrion (G5):
+  - His "as he enters play" ability can be used before he enters contest if there is another one in play. [LSJ 20080526]
+201132|Prejudice (G4):
+  - Can only use his ability when he is bleeding. [ANK 20180514]
+  - He is the one to get the bleed bonus. [ANK 20180511-2]
+201136|Pugfar (G2):
+  - His ability to give a press can only be used during the press step. [PIB 20150121]
+201138|Qawiyya el-Ghaduba (G5):
+  - Her ability can be used only once per minion phase. [ANK 20190207] [RBK 20200701-4]
+201144|Quincy, The Trapper (G3):
+  - His ability means he must perform the same action twice in two different turns. Tokens can be used to keep track of it if players agree. [ANK 20170202]
+201147|Rabbat, The Sewer Goddess (G4):
+  - Her hunt ability may be used even when she is at full capacity. One blood goes to your pool directly even if it would have exceeded her capacity. [LSJ 20050331]
+  - If she strikes to send a vampire to torpor, that vampire is wounded (if they play {Undying Tenacity}, they go to torpor after combat). [LSJ 20090622-2]
+201148|Rachel Brandywine (G3):
+  - When using her ability, make all discards and redraws first, then shuffle the discards back into the library. [RTR 20030519]
+201160|Randall (G4):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+201164|Raphael Catarari (G4):
   - 'Unlocking is the first thing to do in the unlock phase: if he is odd, gaining one blood later in the unlock phase will not let him "unlock as normal" this turn. [LSJ 20060911]'
-201173|Reg Driscoll:
-  - "His ability is activated after he equips with the equipment. He cannot use his ability to move the {Eye of Hazimel}. [LSJ 20060221]"
-  - "You may move all or none the equipment he gets to just one minion, but you cannot split. [LSJ 20050217] [LSJ 20090622]"
-"201175|Regina Giovanni, The Right Hand of Augustus":
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-201181|Reverend Adams (ADV):
+201173|Reg Driscoll (G2):
+  - His ability is activated after he equips with the equipment. He cannot use his ability to move the {Eye of Hazimel}. [LSJ 20060221]
+  - You may move all or none the equipment he gets to just one minion, but you cannot split. [LSJ 20050217] [LSJ 20090622]
+201175|Regina Giovanni, The Right Hand of Augustus (G2):
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+201181|Reverend Adams (G4 ADV):
   - "[MERGED] Is Camarilla. If the base version was the one in play, it changes sect as it is merged. If it had an anarch token, it is burned. [ANK 20180524]"
-"201184|Rex, The Necronomist":
-  - "Card with multiple types (eg. Combat/Action Modifer) are considered of the type they are played as, not both. [PIB 20150924-2]"
-201189|Rico Loco:
-  - "The damage he takes during the master phase from his ability is environmental. [RTR 19970630]"
-201235|Santaleous:
-  - "Can use his ability to cancel a master card multiple times each turn. [ANK 20200420-2]"
-201240|Sargon:
-  - "His controller gets the Edge after the effects of the successful action are applied. If it is a referendum, he gets the Edge after the referendum is concluded. [LSJ 20011222]"
-201243|Sarrasine (ADV):
+201184|Rex, The Necronomist (G2):
+  - Card with multiple types (eg. Combat/Action Modifer) are considered of the type they are played as, not both. [PIB 20150924-2]
+201189|Rico Loco (G4):
+  - The damage he takes during the master phase from his ability is environmental. [RTR 19970630]
+201235|Santaleous (G5):
+  - Can use his ability to cancel a master card multiple times each turn. [ANK 20200420-2]
+  - When using his ability, the cost of the canceled card must still be paid. [LSJ 20090601-2]
+201240|Sargon (G2):
+  - His controller gets the Edge after the action resolves. If it is a referendum, he gets the Edge after the referendum is concluded. [LSJ 20011222] [ANK 20221028-2]
+201243|Sarrasine (G2 ADV):
   - "[MERGED] Is Camarilla. If the base version was the one in play, it changes sect as it is merged. If it had an anarch token, it is burned. [ANK 20180524]"
-"201245|Sascha Vykos, The Angel of Caine (ADV)":
-  - "When using his ability to draw, discard afterwards. [ANK 20190707]"
-201253|Scout Youngwood:
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-  - "Card with multiple types (eg. Reaction/Action Modifer) are considered of the type they are played as, not both. [PIB 20150924-2]"
-201260|Sela (ADV):
+  - "[MERGED] Putting a corruption counter on a minion does not give you an opportunity to steal it. [ANK 20200925] [ANK 20211105]"
+201245|Sascha Vykos, The Angel of Caine (G2 ADV):
+  - When using his ability to draw, discard afterwards. [ANK 20190707]
+201253|Scout Youngwood (G6):
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+  - Card with multiple types (eg. Reaction/Action Modifer) are considered of the type they are played as, not both. [PIB 20150924-2]
+201257|Sébastien Goulet (G3):
+  - His ability works on allies recruited in a non-standard way (eg. {Piper}). [ANK 20210913] [LSJ 20090116]
+201260|Sela (G2 ADV):
   - "[MERGED] Is Sabbat Archbishop of Rome. [ANK 20180524]"
-201269|Seterpenre:
-  - 'His "as he enters play" ability can be used before he enters contest if there is another one in play. [LSJ 20080526]'
-201282|Shemti:
-  - "The damage inflicted by his ability is environmental. [RTR 19970630]"
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-  - 'The acting player decides the order of (and can play other) "after resolving the action" effects. [ANK 20180206]'
-201299|Smallpox Griet:
-  - "Damages from pox counters are environmental. [RTR 19970630]"
-  - "The opponent gets a pox counter every time Smallpox successfully inflicts hand damage in consecutive rounds. [PIB 20141210]"
-201306|Sonja Blue:
+201265|Seren Sukardi (G4):
+  - If he strikes to send a vampire to torpor, that vampire is wounded (if they play {Undying Tenacity}, they go to torpor after combat). [LSJ 20090622-2]
+201267|Sergei Voshkov, The Eye (G5):
+  - When using his ability, you do not get to see the card drawn as replacement. [ANK 20211020] [PIB 20121031]
+201269|Seterpenre (G5):
+  - His "as he enters play" ability can be used before he enters contest if there is another one in play. [LSJ 20080526]
+201282|Shemti (G5):
+  - The damage inflicted by his ability is environmental. [RTR 19970630]
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+  - The acting player decides the order of (and can play other) "after resolving the action" effects. [ANK 20180206]
+201299|Smallpox Griet (G3):
+  - Damages from pox counters are environmental. [RTR 19970630]
+  - The opponent gets a pox counter every time Smallpox successfully inflicts hand damage in consecutive rounds. [PIB 20141210]
+201306|Sonja Blue (G4):
   - '"block as an ally" only affects the "who can block this action" check. She can play cards that require Disicplines when blocking "as an ally". [LSJ 20050224-1]'
   - "{The Unmasking} will not give her intercept. [LSJ 20060503]"
-  - "When contesting her, the new copy provides 4 pool, then the old copy is removed from the game (for leaving play due to contest). The new copy remains face down, out-of-play, ready to be turned face up during her next unlock phase. [LSJ 20070829-2]"
-201310|Spiridonas:
+  - When contesting her, the new copy provides 4 pool, then the old copy is removed from the game (for leaving play due to contest). The new copy remains face down, out-of-play, ready to be turned face up during her next unlock phase. [LSJ 20070829-2]
+201310|Spiridonas (G2):
   - "His special ability is treated as an action modifier as far as timing goes: it can be used after the block attempts are concluded. [SFC 19960819]"
-201326|Sundown (ADV):
+201326|Sundown (G3 ADV):
   - "[MERGED] His ability to force a vampire to abstain applies to Priscus votes and ballots. [LSJ 19971001]"
   - "[MERGED] His ability to force a vampire to abstain can cancel the votes and ballots of the vampire. [LSJ 20100311]"
   - "[MERGED] Is Anarch. If the base version was the one in play, it changes sect as it is merged. [ANK 20180524]"
-"201327|Sutekh, The Dark God":
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-201331|Synesios:
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
+  - "[MERGED] Can use his ability while locked. [ANK 20220705]"
+201327|Sutekh, The Dark God (G2):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+201331|Synesios (G2):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
   - "His ability do not allow his owner to play more than one Master: Out of Turn between two master phases. [ANK 20191004]"
-201332|Synner-G:
-  - "His ability applies when equipping in a non-normal way (eg. {Pier 13, Port of Baltimore}). [PIB 20150105-2]"
-201334|T.J.:
-  - "Must be unlocked with at least 2 blood to use his ability. [ANK 20200508-2] [RBK 20181001-11]"
-"201337|Talley, the Hound":
-  - "Gets his +1 intercept if an action has any one target that would be enough to enable his effect. [RTR 20080808] [KOT 20081119]"
-"201344|Tariq, The Silent":
-  - "His capacity is reduced immediately when he get controlled, before it can be merged with the advanced version. [ANK 20190522]"
-"201345|Tariq, The Silent (ADV)":
-  - "His capacity is reduced immediately when he get controlled, before it can be merged with the base version. [ANK 20190522]"
+201332|Synner-G (G5):
+  - His ability applies when equipping in a non-normal way (eg. {Pier 13, Port of Baltimore}). [PIB 20150105-2]
+201334|T.J. (G4):
+  - Must be unlocked with at least 2 blood to use his ability. [ANK 20200508-2] [RBK 20200701-4]
+201337|Talley, The Hound (G2):
+  - Gets his +1 intercept if an action has any one target that would be enough to enable his effect. [RTR 20080808] [KOT 20081119]
+201344|Tariq, The Silent (G2):
+  - His capacity is reduced immediately when he get controlled, before it can be merged with the advanced version. [ANK 20190522]
+201345|Tariq, The Silent (G2 ADV):
+  - His capacity is reduced immediately when he get controlled, before it can be merged with the base version. [ANK 20190522]
   - "[MERGED] When he merges (in whatever way), he becomes independant and any Anarch token is burned. [ANK 20180523]"
-"201348|Tatiana Stepanova, Alastor":
-  - "When playing a card requiring Brujah or Gangrel, she is treated as a such for all effects of the card, and only them, including duration effects. She is not treated as such for effects the card has from being in play. [ANK 20190228]"
-  - "Her ability do not let her fulfill card requirements if they are not played normally, like when using {Piper} or {The Summoning} to recruit an ally. [LSJ 20050119]"
-"201352|Tegyrius, Vizier":
-  - "Allegiance counters continue to function even if Tegyrius leaves play. [LSJ 20010616] [LSJ 20030522-1]"
+201348|Tatiana Stepanova, Alastor (G4):
+  - When playing a card requiring Brujah or Gangrel, she is treated as a such for all effects of the card, and only them, including duration effects. She is not treated as such for effects the card has from being in play. [ANK 20190228]
+  - Her ability do not let her fulfill card requirements if they are not played normally, like when using {Piper} or {The Summoning} to recruit an ally. [LSJ 20050119]
+201352|Tegyrius, Vizier (G2):
+  - Allegiance counters continue to function even if Tegyrius leaves play. [LSJ 20010616] [LSJ 20030522-1]
   - "The allegiance counter is a continuous effect: an Assamite with it stays Camarilla even if he changes his underlying sect (eg. rulebook action to become anarch). [ANK 20180626-2]"
-"201354|Teresita, The Godmother":
-  - "She gains or looses intercept if the acting vampire changes sect during the action (eg. with {The Red Question} or {Mask of a Thousand Faces}). [ANK 20190416]"
-201355|Tereza Rostas:
-  - "She cannot steal the Edge if it is uncontrolled. [TOM 19951214-2]"
-  - "If the target of the action burns the Edge during the action, her controller still gets the Edge if the action succeeds. [RTR 19980623]"
-201359|Terry:
-  - "Her ability to get a press can only be used during the press step. [PIB 20150121]"
-201363|Theo Bell (ADV):
+201354|Teresita, The Godmother (G3):
+  - She gains or looses intercept if the acting vampire changes sect during the action (eg. with {The Red Question} or {Mask of a Thousand Faces}). [ANK 20190416]
+201355|Tereza Rostas (G2):
+  - She cannot steal the Edge if it is uncontrolled. [TOM 19951214-2]
+  - If the target of the action burns the Edge during the action, her controller still gets the Edge if the action succeeds. [RTR 19980623]
+201359|Terry (G2):
+  - Her ability to get a press can only be used during the press step. [PIB 20150121]
+201363|Theo Bell (G2 ADV):
   - "[MERGED] Is Independant. If the base version was the one in play, it changes sect as it is merged. If it had an anarch token, it is burned. [ANK 20180524]"
-"201365|Thetmes, Caliph of Alamut":
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-201370|Thucimia:
-  - "Keeps her title and votes if she changes sects. [LSJ 20010714]"
-201382|Topaz:
-  - "Her ability applies when equipping in a non-normal way (eg. {Concealed Weapon}). [PIB 20150105-2]"
-201383|Tori Longwood:
-  - "Her ability still applies when in torpor. [LSJ 20011022] [LSJ 20100902-2]"
-201386|Travis "Traveler72" Miller:
-  - "Must announce which conviction he burns as part of the terms of the action granted by his ability. [RTR 20111202]"
-201387|Troglodytia:
-  - "If the master card is not replaced immediately (eg. {Wash}), you look at then hand without the replacement card. [ANK 20180512]"
-201390|Tryphosa:
-  - "The additional blood cost is not paid if the action does not succeed. [PIB 20121031]"
-201393|Tupdog:
-  - "Card with disciplines choices (eg. [vis]/[tha]) are considered of the discipline they are played as. [PIB 20150924-2]"
-"201413|Ur-Shulgi, The Shepherd":
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-201415|Uriah Winter:
-  - "Can still defect if in torpor, and will remain in torpor if he does so. [RTR 19941109]"
-"201422|Valerius Maior, Hell's Fool (ADV)":
-  - "The prohibition to play certain cards applies from the moment he attempts to block until the end of the action, even if he fails to block. [LSJ 20080818]"
-"201434|Velya, The Flayer":
-  - "His ability to get a press can only be used during the press step. [PIB 20150121]"
-201436|Verbruch:
-  - 'His "as he enters play" ability can be used before he enters contest if there is another one in play. [LSJ 20080526]'
-201439|Victor Gerard:
-  - "When playing a card requiring a Camarilla vampire or a Prince, he is treated as a such for all effects of the card, and only them, including duration effects. He is not treated as such for effects the card has from being in play. [ANK 20190228]"
-201440|Victor Pelletier:
-  - 'His "as he enters play" ability can be used before he enters contest (not after) if there is another one in play. [LSJ 20080526] [LSJ 20100902]'
-201446|Vidal Jarbeaux:
-  - "When meeting a requirement to play a card, he is treated as such for all the effects of the card, and only them, including duration effects. He is not treated as meeting the requirements for effects the card has from being in play. [ANK 20200703-3] [ANK 20190228] [LSJ 20101013]"
-  - "If a card he plays is canceled as it is played, he is still considered having used the requirement, if any. [ANK 20200710]"
-  - "He can meet any title as well as non-requirements (eg. non-Red List), but cannot meet requirements that are not vampire traits (eg. Mortal, unlocked, older, ..) [LSJ 20081120-1]"
-  - "When meeting a title requirement, he is considered as a vampire of the underlying sect. [LSJ 20050128]"
-  - "He can meet the requirements for his controller to play any card, including Master cards. [LSJ 20091015] [PIB 20130128]"
-  - 'He cannot fulfill a non-vampire trait requirement (eg. Gehenna), but he can fulfill the "Red List" or "Flight" requirements. [LSJ 20091016]'
-  - "Striga and Maleficia are not vampire traits. [LSJ 20100226]"
-201456|Vlad Tepes:
-  - "When playing a card requiring a title or a sect, he is treated as a such for all effects of the card, including duration effects. (eg. he can {Archon} himself and use its effect later) [ANK 20201028] [ANK 20190228] [LSJ 20101013]"
-  - "He can use a card in play as if he had a title or a sect, but cannot use it if it would provide unrequired stealth or intercept (eg. he cannot use {No Secrets From the Magaji} to attempt to block a vampire acting with no stealth). [ANK 20180403]"
-  - "His ability do not let him fulfill card requirements if they are not played normally, like when using {Piper} to recruit an ally. [LSJ 20050119]"
-  - "When meeting a title requirement, he is considered as a vampire of the underlying sect. [LSJ 20050128]"
-  - "When meeting a requirement, the controller can choose how he meets it (eg. he can play {Anarch Secession} as a Prince of any city, even a made-up one). [PIB 20150306] [PIB 20150307]"
-  - "He can use a card requiring a sect or titled to be played (eg. use {Abbot} intercept bonus as a Sabbat vampire, perform {Archon} action to burn it as a Prince or Justicar). [PIB 20150306]"
+201365|Thetmes, Caliph of Alamut (G2):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+201370|Thucimia (G4):
+  - Keeps her title and votes if she changes sects. [LSJ 20010714]
+201376|Toby (G4):
+  - His ability can be used while locked or in torpor. [ANK 20220705] [LSJ 20100705]
+201382|Topaz (G4):
+  - Her ability applies when equipping in a non-normal way (eg. {Concealed Weapon}). [PIB 20150105-2]
+  - When using her abilty, pay only for the original equipment. Neither costs nor requirements apply for the one taken from the prey's hand. [LSJ 20080702-4]
+201383|Tori Longwood (G2):
+  - Her ability still applies when in torpor. [LSJ 20011022] [LSJ 20100902-2]
+201386|Travis "Traveler72" Miller (G4):
+  - Must announce which conviction he burns as part of the terms of the action granted by his ability. [RTR 20111202]
+201387|Troglodytia (G4):
+  - If the master card is not replaced immediately (eg. {Wash}), you look at then hand without the replacement card. [ANK 20180512]
+201390|Tryphosa (G4):
+  - The additional blood cost is not paid if the action does not succeed. [PIB 20121031]
+201393|Tupdog (G3):
+  - Card with disciplines choices (eg. [vis]/[tha]) are considered of the discipline they are played as. [PIB 20150924-2]
+201413|Ur-Shulgi, The Shepherd (G2):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+201415|Uriah Winter (G1):
+  - Can still defect if in torpor, and will remain in torpor if he does so. [RTR 19941109]
+201422|Valerius Maior, Hell's Fool (G4 ADV):
+  - The prohibition to play certain cards applies from the moment he attempts to block until the end of the action, even if he fails to block. [LSJ 20050607-1] [LSJ 20080818]
+201434|Velya, The Flayer (G3):
+  - His ability to get a press can only be used during the press step. [PIB 20150121]
+201436|Verbruch (G5):
+  - His "as he enters play" ability can be used before he enters contest if there is another one in play. [LSJ 20080526]
+201439|Victor Gerard (G2):
+  - When playing a card requiring a Camarilla vampire or a Prince, he is treated as a such for all effects of the card, and only them, including duration effects. He is not treated as such for effects the card has from being in play. [ANK 20190228]
+201440|Victor Pelletier (G4):
+  - His "as he enters play" ability can be used before he enters contest (not after) if there is another one in play. [LSJ 20080526] [LSJ 20100902]
+201446|Vidal Jarbeaux (G5):
+  - When meeting a requirement to play a card, he is treated as such for all the effects of the card, and only them, including duration effects. He is not treated as meeting the requirements for effects the card has from being in play. [ANK 20200703-3] [ANK 20190228] [LSJ 20101013]
+  - If a card he plays is canceled as it is played, he is still considered having used the requirement, if any. [ANK 20200710]
+  - He can meet any title as well as non-requirements (eg. non-Red List), but cannot meet requirements that are not vampire traits (eg. Mortal, unlocked, older, ..) [LSJ 20081120-1]
+  - When meeting a title requirement, he is considered as a vampire of the underlying sect. [LSJ 20050128]
+  - He can meet the requirements for his controller to play any card, including Master cards. [LSJ 20091015] [PIB 20130128]
+  - He cannot fulfill a non-vampire trait requirement (eg. Gehenna), but he can fulfill the "Red List" or "Flight" requirements. [LSJ 20091016]
+  - Striga and Maleficia are not vampire traits. [LSJ 20100226]
+  - When meeting a requirement, the controller can choose how he meets it (eg. he can play {Anarch Secession} as a Prince of any city, even a made-up one). [PIB 20150306] [PIB 20150307]
+  - He can meet a given generic requirement (eg. Prince) only once, however he decides to meet it (eg. city choice). [ANK 20210812]
+  - He must choose a title when playing a card required a "titled" vampire (eg. {Rubicon}), but can only choose each title once. He can choose the non-descript "X votes" title, but only once. [ANK 20211019]
+201456|Vlad Tepes (G3):
+  - When playing a card requiring a title or a sect, he is treated as a such for all effects of the card, including duration effects. (eg. he can {Archon} himself and use its effect later) [ANK 20201028] [ANK 20190228] [LSJ 20101013]
+  - He can use {No Secrets From the Magaji} to attempt to block a vampire acting with no stealth. REVERSAL from previous rulings. [ANK 20210903]
+  - His ability do not let him fulfill card requirements if they are not played normally, like when using {Piper} to recruit an ally. [LSJ 20050119]
+  - When meeting a title requirement, he is considered as a vampire of the underlying sect. [LSJ 20050128]
+  - When meeting a requirement, the controller can choose how he meets it (eg. he can play {Anarch Secession} as a Prince of any city, even a made-up one). [PIB 20150306] [PIB 20150307]
+  - He can use a card requiring a sect or titled to be played (eg. use {Abbot} intercept bonus as a Sabbat vampire, perform {Archon} action to burn it as a Prince or Justicar). [PIB 20150306]
   - "He cannot use a card as a vampire of a sect or with a title if the card does not require the sect or title to be played. (eg. he cannot benefit from {Powerbase: Madrid} as a Sabbat vampire) [PIB 20150306]"
-201460|Vulture:
-  - "His ability applies when equipping in a non-normal way (eg. {Pier 13, Port of Baltimore}). [PIB 20150105-2]"
-201462|Walker Grimes:
-  - "His special ability only affects the cost of masters played by his controller. [LSJ 20081124-1]"
-201463|Wamukota:
-  - 'If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]'
-  - 'If the action continues "as if unblocked", Methusalah that had declined to block before do not get another opportunity to block. [ANK 20190116]'
+201460|Vulture (G2):
+  - His ability applies when equipping in a non-normal way (eg. {Pier 13, Port of Baltimore}). [PIB 20150105-2]
+201462|Walker Grimes (G5):
+  - His special ability only affects the cost of masters played by his controller. [LSJ 20081124-1]
+201463|Wamukota (G4):
+  - If the action continues "as if unblocked", all action modifiers and reaction cards are still in effect, even those pertaining to a successful block. [RTR 19941109] [ANK 20190116]
+  - If the action continues "as if unblocked", Methuselah that had declined to block before do not get another opportunity to block. [ANK 20190116]
   - '"continue as if unblocked" moves the action card from the ash heap (where it went when the action was blocked) to limbo (where it should be if the action is not blocked). If the action card is not in the ash heap, then the action cannot be continued. [LSJ 20070808-1]'
-  - "His ability to end combat can be used when he is in torpor. [LSJ 20011022]"
-201471|Winterlich:
-  - "When recruit a changeling ally, he is treated as a meeting the requirements for all effects of the card, and only them, including duration effects. He is not treated as meeting the requirements for effects the card has from being in play. [ANK 20190228]"
-  - "You can still use the burn options of cards with a requirement he could meet when you play them, but does not meet while in play. [LSJ 20050225]"
-  - "His ability do not let him fulfill card requirements if they are not played normally, like when using {Piper}. [LSJ 20050119]"
-201477|Xaviar:
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
-201478|Xaviar (ADV):
+  - His ability to end combat can be used when he is in torpor. [LSJ 20011022]
+201464|Watenda (G2):
+  - The cost he pays takes into account any cost modification that applies for the opposing minion. [LSJ 20091124]
+  - When canceling a card, he pays any pool cost in blood. [LSJ 20071015-2]
+  - He can use his ability even if he's going to torpor. [LSJ 20021007]
+  - Can only use his ability when he is in combat himself. [ANK 20221021]
+201467|White Lily (G4):
+  - Requirements need to be met. [LSJ 20080702-3]
+  - Can only use her ability when she is in combat herself. [ANK 20221021]
+201471|Winterlich (G6):
+  - When recruit a changeling ally, he is treated as a meeting the requirements for all effects of the card, and only them, including duration effects. He is not treated as meeting the requirements for effects the card has from being in play. [ANK 20190228]
+  - You can still use the burn options of cards with a requirement he could meet when you play them, but does not meet while in play. [LSJ 20050225]
+  - His ability do not let him fulfill card requirements if they are not played normally, like when using {Piper}. [LSJ 20050119]
+201477|Xaviar (G3):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+201478|Xaviar (G3 ADV):
   - "[MERGED] Is Camarilla. If the base version was the one in play, it changes sect as it is merged. If it had an anarch token, it is burned. [ANK 20180524]"
-"201480|Xeper, Sultan of Lepers":
-  - "Is not titled. If he gets a title, his additional votes are added to the ones provided by the title. [LSJ 20100601]"
-201486|Yazid Tamari (ADV):
+201480|Xeper, Sultan of Lepers (G6):
+  - Is not titled. If he gets a title, his additional votes are added to the ones provided by the title. [LSJ 20100601]
+201486|Yazid Tamari (G3 ADV):
   - "[MERGED] Is Anarch Black Hand Seraph. If the base version was the one in play, it changes sect as it is merged. [ANK 20180524] [LSJ 20031121-3]"
-201499|Zack North (ADV):
+201499|Zack North (G1 ADV):
   - "[MERGED] Is Anarch. If the base version was the one in play, it changes sect as it is merged. [ANK 20180524]"
-"201502|Zayyat, The Sandstorm":
-  - "Keeps his title and votes if he changes sects. [LSJ 20010714]"
+201502|Zayyat, The Sandstorm (G3):
+  - Keeps his title and votes if he changes sects. [LSJ 20010714]
+201506|Zhenga (G4):
+  - She can choose the order in which the allies brought by her ability come into play (eg. bring a first ally, then {War Ghoul} second burning the first one). [LSJ 20060530-1]
+  - The allies brought into play by her ability are not "played in the normal way" (eg. {Direct Intervention} cannot be used to counter them). [LSJ 20060530-2]
+201574|Kuyén (G6):
+  - His ability works on allies recruited in a non-standard way (eg. {Piper}). [ANK 20210913] [LSJ 20090116]
+201576|Aline Gädeke (G6):
+  - Can unlock after a vampire performs an action to become Anarch. [ANK 20220814]
+201585|Elen Kamjian (G6):
+  - If she unlocks after having performed her mandatory bleed, she is free to take any action. [LSJ 20090226] [ANK 20211009-2]
+  - Another bleed action (eg. {Flurry of Action}) does not count as the bleed action her ability forces her to take. [ANK 20211009-2]
+  - If her ability makes a bleed mandatory but she has performed a bleed already this turn, she is stuck and cannot act. [ANK 20211009-2]
+201608|Nonu Dis (G6):
+  - His ability can be used only once per master phase. [ANK 20220617]
+201613|Theo Bell (G6):
+  - Can be merged with {Theo Bell (ADV)} if you get to control one (eg. {Graverobbing}). [ANK 20220805-2]
+201627|Evan Klein (G6):
+  - Actions from minions of the same controller targeting him are undirected, so they are not affected by his ability. [LSJ 20030214-2]
+201641|The Guardian (G6):
+  - When using his ability, the opponent is the acting minion and play their combat effects first. [ANK 20221102]
```

### Comparing `krcg-2.9/rulings/rulings-links.yaml` & `krcg-3.0/rulings/rulings-links.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 ANK 20180206: http://www.vekn.net/forum/rules-questions/76404-timing-of-shemti-s-special-and-ecstasy#85223
 ANK 20180307-1: http://www.vekn.net/forum/rules-questions/76452-ballot-vs-fee-stake#85610
 ANK 20180307-2: http://www.vekn.net/forum/rules-questions/76451-ellison-humboldt-and-matteus-flesh-sculptor?start=0#85598
 ANK 20180318: http://www.vekn.net/forum/rules-questions/76464-dnr-counts-against-hand-size-meddling-of-semsith-and-raptor#85841
 ANK 20180321: http://www.vekn.net/forum/rules-questions/76378-clan-loyalty?start=12#85923
 ANK 20180326: http://www.vekn.net/forum/rules-questions/76477-crocodile-temple-vs-oust#86050
 ANK 20180327: http://www.vekn.net/forum/rules-questions/76480-enrage-and-burning-blood#86056
-ANK 20180403: http://www.vekn.net/forum/rules-questions/76491-no-secrets-from-vlad-tepes#86137
 ANK 20180408: http://www.vekn.net/forum/rules-questions/76500-charnas-the-imp#86191
 ANK 20180509: http://www.vekn.net/forum/rules-questions/76585-emerald-legionnaire-and-hos-requirement?start=0#86672
 ANK 20180511-1: http://www.vekn.net/forum/rules-questions/76594-lost-kindred-faq#86769
 ANK 20180511-2: http://www.vekn.net/forum/rules-questions/76592-prejudice-special-ability#86767
 ANK 20180420-1: http://www.vekn.net/forum/rules-questions/76522-majesty-against-serpent-s-numbing-kiss#86272
 ANK 20180420-2: http://www.vekn.net/forum/rules-questions/76522-majesty-against-serpent-s-numbing-kiss#86278
 ANK 20180512: http://www.vekn.net/forum/rules-questions/76599-troglodytia-special-vs-wash#86842
@@ -156,21 +155,24 @@
 ANK 20190717-2: http://www.vekn.net/forum/rules-questions/77798-announcing-strikes-and-intention#95865
 ANK 20190724: http://www.vekn.net/forum/rules-questions/77810-a-monthly-doubts-for-rookie#95945
 ANK 20190725: https://www.vekn.net/forum/rules-questions/77813-card-questions#95969
 ANK 20190731: http://www.vekn.net/forum/rules-questions/77812-abstain-from-voting?start=6#96048
 ANK 20190827: http://www.vekn.net/forum/rules-questions/77911-how-does-extremis-boon-actually-work?start=6#96572
 ANK 20191004: http://www.vekn.net/forum/rules-questions/77994-synesios#97241
 ANK 20191025: http://www.vekn.net/forum/rules-questions/78050-roetschreck-controler-is-ousted#97560
-ANK 20191031: http://www.vekn.net/forum/rules-questions/11417-eternal-mask-khobar-towers?start=6#97642
+ANK 20191031: https://www.vekn.net/2-uncategorised/465-vampire-elder-kindred-network-newsletter-october-2019
+ANK 20191031-2: http://www.vekn.net/forum/rules-questions/11417-eternal-mask-khobar-towers?start=6#97642
 ANK 20191108: http://www.vekn.net/forum/rules-questions/78081-eyes-of-the-beast#97710
 ANK 20191204: http://www.vekn.net/forum/rules-questions/78164-mirror-walk-change-and-guardian-vigil?start=6#98139
 ANK 20191211: http://www.vekn.net/forum/rules-questions/78193-di-against-a-combat-card-with-infernal-pursuit-active#98215
 ANK 20191218: http://www.vekn.net/forum/rules-questions/62700-re-nahir-and-research-counters?start=6#98297
 ANK 20191219: http://www.vekn.net/forum/rules-questions/78241-relentless-reaper-vs-blissful-agony-and-scheduled-combat-rulings-ambiguity#98308
+ANK 20191221: https://www.vekn.net/forum/rules-questions/76990-correct-order-impulse-for-combat-cards-after-combat#90516
 ANK 20191228: http://www.vekn.net/forum/rules-questions/78262-parity-shift-without-target#98358
+ANK 20200909: https://www.vekn.net/forum/rules-questions/78845-contagion-corruption-counters-vs-strike-dodge#100726
 ANK 20200107: http://www.vekn.net/forum/rules-questions/70520-re-lutz-ruling?start=6#98454
 ANK 20200109: http://www.vekn.net/forum/rules-questions/78291-legacy-of-power-and-continue-combat-effects-like-psyche#98484
 ANK 20200114: http://www.vekn.net/forum/rules-questions/78321-slave-rule-and-acting-minion#98584
 ANK 20200115: http://www.vekn.net/forum/rules-questions/78321-slave-rule-and-acting-minion?start=6#98594
 ANK 20200117: http://www.vekn.net/forum/rules-questions/77058-progeny-sect-change#98629
 ANK 20200123: http://www.vekn.net/forum/rules-questions/78373-theft-of-vitae-vs-theft-of-vitae#98717
 ANK 20200129: http://www.vekn.net/forum/rules-questions/78701-replace-during-unlock-and-other-unlock-effects#100210
@@ -237,14 +239,116 @@
 ANK 20201228-2: https://www.vekn.net/forum/rules-questions/78954-necrosis-and-target-vitals?start=0#101314
 ANK 20201229: https://www.vekn.net/forum/rules-questions/78959-louhi-and-piper#101325
 ANK 20201229-2: https://www.vekn.net/forum/rules-questions/78958-weighted-walking-stick-with-1-counter-remaining#101326
 ANK 20210109: https://www.vekn.net/forum/rules-questions/78983-fear-of-mekhet-and-torpor#101392
 ANK 20210124: https://www.vekn.net/forum/rules-questions/79001-the-question-of-the-month-action-fizzles#101492
 ANK 20210131: https://www.vekn.net/forum/rules-questions/79008-crypt-s-sons-lock-and-obedience#101525
 ANK 20210131-1: https://www.vekn.net/forum/rules-questions/79007-netwar-timing#101527
+ANK 20210226: https://www.vekn.net/forum/rules-questions/79045-paths-and-burn-blood-requrement?start=18#101726
+ANK 20210228: https://www.vekn.net/forum/rules-questions/56821-re-carolina-valez-immunity?start=6#101741
+ANK 20210304: https://www.vekn.net/forum/rules-questions/79058-great-symposium#101761
+ANK 20210309: https://www.vekn.net/forum/rules-questions/79063-daring-the-dawn-and-then-mask-of-a-thousand-faces#101805
+ANK 20210309-2: https://www.vekn.net/forum/rules-questions/79005-rulebook-gaining-votes?start=6#101807
+ANK 20210309-3: https://www.vekn.net/forum/rules-questions/79065-master-cards-attached-to-a-stolen-minion#101806
+ANK 20210313: https://www.vekn.net/forum/rules-questions/79072-until-the-end-vs-during-art-of-love-steals-informant#101841
+ANK 20210322: https://www.vekn.net/forum/rules-questions/79080-nightmares-upon-nightmares#101906
+ANK 20210322-2: https://www.vekn.net/forum/rules-questions/79080-nightmares-upon-nightmares?start=6#101910
+ANK 20210410: https://www.vekn.net/forum/rules-questions/74696-hackerspace-question?start=6#102019
+ANK 20210422: https://www.vekn.net/forum/rules-questions/79111-vampiric-disease-and-dodge#102098
+ANK 20210424: https://www.vekn.net/forum/rules-questions/79121-burning-byzar-during-combat#102140
+ANK 20210529: https://www.vekn.net/forum/technical-matters/79155-baltimore-purge#102348
+ANK 20210608: https://www.vekn.net/forum/rules-questions/79166-correct-time-to-use-heidelberg-castle-germany-for-non-acting-player?start=12#102425
+ANK 20210612: https://www.vekn.net/forum/rules-questions/79173-confirmation-needed-about-garrote?start=6#102470
+ANK 20210614: https://www.vekn.net/forum/rules-questions/79177-ossian-vs-charismatic-aura#102483
+ANK 20210620: https://www.vekn.net/forum/rules-questions/79186-alejandro-aguirre-true-faith#102522
+ANK 20210627: https://www.vekn.net/forum/rules-questions/79192-mirror-walk-and-slave?start=12#102578
+ANK 20210630: https://www.vekn.net/forum/rules-questions/79205-lay-low-vs-banishment#102601
+ANK 20210705: https://www.vekn.net/forum/rules-questions/79211-lorenzo-detuono-timing-questions#102632
+ANK 20210714: https://www.vekn.net/forum/rules-questions/79224-can-i-do-a-3rd-villein-in-a-vampire-if-i-have-only-1-pool-remaining#102697
+ANK 20210714-2: https://www.vekn.net/forum/rules-questions/79217-clarification-needed-on-eternals-of-sirius-rulings?start=6#102696
+ANK 20210717: https://www.vekn.net/forum/rules-questions/79228-tribute-to-the-master#102716
+ANK 20210719: https://www.vekn.net/forum/rules-questions/76877-vivienne-geroux-and-anarh-cards?start=6#102731
+ANK 20210812: https://www.vekn.net/forum/rules-questions/79278-vidal-jarbeaux-cards-requiring-prince#102892
+ANK 20210813: https://www.vekn.net/forum/rules-questions/79279-might-of-the-camarilla-burned-from-play#102903
+ANK 20210903: https://www.vekn.net/forum/rules-questions/76491-no-secrets-from-vlad-tepes?start=30#103038
+ANK 20210913: https://www.vekn.net/forum/rules-questions/79322-piper-and-sebastien-goulet#103113
+ANK 20210926: https://www.vekn.net/forum/rules-questions/79337-eluding-the-arms-of-morpheus-after-block-declare?start=18#103333
+ANK 20210928: https://www.vekn.net/forum/rules-questions/79364-combo-piper-x-soul-of-earth#103363
+ANK 20210928-2: https://www.vekn.net/forum/rules-questions/79330-thoughts-betrayed-and-hunger-of-marduk?start=12#103364
+ANK 20210929: https://www.vekn.net/forum/generic-v-tes-discussion/75623-ghoul-retainer?start=12#103386
+ANK 20211003: https://www.vekn.net/forum/rules-questions/79372-fail-to-block-and-telepathic-misdirection#103416
+ANK 20211009: https://www.vekn.net/forum/rules-questions/79388-political-struggle-and-victim-priscus#103481
+ANK 20211009-2: https://www.vekn.net/forum/rules-questions/79335-elen-camjian-second-action?start=6#103483
+ANK 20211010: https://www.vekn.net/forum/rules-questions/79335-elen-camjian-second-action?start=6#103500
+ANK 20211015: https://www.vekn.net/forum/rules-questions/79389-when-does-nra-apply-not-apply?start=6#103563
+ANK 20211019: https://www.vekn.net/forum/rules-questions/79278-vidal-jarbeaux-cards-requiring-prince#103598
+ANK 20211019-2: https://www.vekn.net/forum/rules-questions/79390-sup-foreshadoing-destruction-when-the-target-has-10-or-more-pool?start=6#103593
+ANK 20211020: https://www.vekn.net/forum/rules-questions/79416-sergei-voshkov-the-eye#103610
+ANK 20211022: https://www.vekn.net/forum/rules-questions/79422-nar-sheptha#103636
+ANK 20211026: https://www.vekn.net/forum/rules-questions/79432-rotschreck-and-non-strike-agravated-damage#103671
+ANK 20211102: https://www.vekn.net/forum/rules-questions/79447-rotschreck-and-dodge#103743
+ANK 20211105: https://www.vekn.net/forum/rules-questions/79460-sarrasin-corruption-and-effect-triggers#103791
+ANK 20211112: https://www.vekn.net/forum/rules-questions/79475-amaranth-anathema#103872
+ANK 20211112-2: https://www.vekn.net/forum/rules-questions/79478-unleash-hell-s-fury-and-extra-intercept#103870
+ANK 20211113: https://www.vekn.net/forum/rules-questions/79465-unwholesome-bond-angelo-circle-of-one-new-blood-and-circle#103879
+ANK 20211124: https://www.vekn.net/forum/rules-questions/79501-addition-strikes#103982
+ANK 20211127: https://www.vekn.net/forum/rules-questions/76687-retainers-inflicting-damage-environmental?start=6#104017
+ANK 20211130: https://www.vekn.net/forum/rules-questions/66960-re-gianna-di-canneto?start=6#104061
+ANK 20211201: https://www.vekn.net/forum/rules-questions/79519-waste-management-operations-no-cards-in-the-library-and-in-the-hand#104074
+ANK 20211207: https://www.vekn.net/forum/rules-questions/79528-crypt-s-sons-versus-unleash-hell-s-fury?start=6#104139
+ANK 20211214: https://www.vekn.net/forum/rules-questions/79542-anarch-convert?start=6#104185
+ANK 20220114: https://www.vekn.net/forum/rules-questions/79432-rotschreck-and-non-strike-agravated-damage?start=12#104475
+ANK 20220116: https://www.vekn.net/forum/rules-questions/79600-unleash-hell-s-fury-and-other-delayed-triggered-effects#104488
+ANK 20220118: https://www.vekn.net/forum/rules-questions/79389-when-does-nra-apply-not-apply?start=6#104506
+ANK 20220127: https://www.vekn.net/forum/rules-questions/79615-burn-counter-to-gain-control-of-steal-a-minion#104588
+ANK 20220204: https://www.vekn.net/forum/rules-questions/79634-multi-dust-up-question#104626
+ANK 20220207: https://www.vekn.net/forum/rules-questions/79639-hunger-of-marduk-and-additional-strike#104645
+ANK 20220218: https://www.vekn.net/forum/rules-questions/79001-the-question-of-the-month-action-fizzles?start=12#104697
+ANK 20220331: https://www.vekn.net/forum/rules-questions/79720-daring-the-dawn-and-mirror-walk#104919
+ANK 20220401: https://www.vekn.net/forum/rules-questions/79720-daring-the-dawn-and-mirror-walk?start=6#104927
+ANK 20220409: https://www.vekn.net/forum/rules-questions/79728-blade-of-enoch-user-playing-dam-the-heart-s-river?start=0#104966
+ANK 20220411: https://www.vekn.net/forum/rules-questions/79730-dabbler-and-direct-intervention#104995
+ANK 20220429: https://www.vekn.net/forum/rules-questions/79754-heavens-gate-new-wording#105112
+ANK 20220503: https://www.vekn.net/forum/rules-questions/39040-re-ex-nihilo-can-i-choose-to-burn-my-minion#105161
+ANK 20220507: https://www.vekn.net/forum/rules-questions/79763-damage-lifeloss-d-actions-and-trophies-predators-tranformation#105200
+ANK 20220525: https://www.vekn.net/forum/rules-questions/79777-lorenzo-detuono-and-imposing-phantasm#105316
+ANK 20220528: https://www.vekn.net/forum/rules-questions/76455-keystone-kine-and-imbued?start=18#105328
+ANK 20220615: https://www.vekn.net/forum/rules-questions/72394-re-kaymakli-fragment?start=6#105476
+ANK 20220617: https://www.vekn.net/forum/rules-questions/79835-nonu-dis-and-during-x-do-y#105494
+ANK 20220704: https://www.vekn.net/forum/rules-questions/79890-charming-lobby-a-political-action-card-krc?start=0#105616
+ANK 20220705: https://www.vekn.net/forum/rules-questions/79895-question-regarding-using-a-minion-card-text-ability-when-locked#105630
+ANK 20220718: https://www.vekn.net/forum/rules-questions/79913-mata-hari-and-infamous-insurgent#105762
+ANK 20220805: https://www.vekn.net/forum/rules-questions/79939-attachable-modifiers-reactions-being-removed-prior-to-attachment#105881
+ANK 20220805-2: https://www.vekn.net/forum/rules-questions/79934-merging-group-2-theo-bell-and-group-6-theo-bell-and-similar-cases#105886
+ANK 20220808: https://www.vekn.net/forum/rules-questions/79952-when-does-lutz-ability-trigger#105913
+ANK 20220809: https://www.vekn.net/forum/rules-questions/79949-loki-s-gift-hunt-bonus#105914
+ANK 20220810: https://www.vekn.net/forum/rules-questions/79955-lay-low-vs-genina-the-red-poet#105932
+ANK 20220814: https://www.vekn.net/forum/rules-questions/79950-aline-gaedeke?start=12#105964
+ANK 20220814-2: https://www.vekn.net/forum/rules-questions/79960-nightstick-and-defensive-strikes?start=6#105963
+ANK 20220816: https://www.vekn.net/forum/rules-questions/79967-the-book-of-going-forth-by-night-and-imbued#105993
+ANK 20220824: https://www.vekn.net/forum/rules-questions/79986-the-british-museum-london-and-pier-13-port-of-baltimore?start=6#106118
+ANK 20220910: https://www.vekn.net/forum/rules-questions/80021-clandestine-contrac-x-forced-march-freak#106314
+ANK 20220916: https://www.vekn.net/forum/rules-questions/80030-blood-brother-ambush-taking-the-skin-minion#106354
+ANK 20220923: https://www.vekn.net/forum/rules-questions/80044-enhanced-coagulant-vs-dodge#106405
+ANK 20221007: https://www.vekn.net/forum/rules-questions/80064-diabolic-lure-superior-burn-pool#106494
+ANK 20221011: https://www.vekn.net/forum/rules-questions/80070-thoughts-betrayed-vs-shadow-court-satyr?start=6#106537
+ANK 20221011-2: https://www.vekn.net/forum/rules-questions/79984-force-of-wil-and-daring-the-dawn-vs-red-herring#106538
+ANK 20221011-3: https://www.vekn.net/forum/rules-questions/74643-419-operation-with-no-counters#106539
+ANK 20221011-4: https://www.vekn.net/forum/rules-questions/79988-keminitiri-closed-session#106540
+ANK 20221019: https://www.vekn.net/forum/rules-questions/80100-de-sades-special-and-kindred-manipulation#106609
+ANK 20221019-2: https://www.vekn.net/forum/rules-questions/80101-blood-moved-by-heidelberg-castle-is-considered-a-gain-for-ex-nihilo-purposes#106607
+ANK 20221019-3: https://www.vekn.net/forum/rules-questions/21158-re-secure-haven-banishment?start=6#106615
+ANK 20221021: https://www.vekn.net/forum/rules-questions/80108-patagia#106628
+ANK 20221024: https://www.vekn.net/forum/rules-questions/80110-goth-band-and-leadership-vacuum#106640
+ANK 20221026: https://www.vekn.net/forum/rules-questions/80117-the-british-museum-london#106651
+ANK 20221028: https://www.vekn.net/forum/rules-questions/80119-contesting-mokole-blood#106671
+ANK 20221028-2: https://www.vekn.net/forum/rules-questions/80122-the-shard-london-and-sargon#106673
+ANK 20221102: https://www.vekn.net/forum/rules-questions/80129-fall-of-london-card-rules-questions#106688
+ANK 20221102-2: https://www.vekn.net/forum/rules-questions/80130-motf-hl-retribution#106694
+ANK 20221103: https://www.vekn.net/forum/rules-questions/80131-can-a-flaming-candle-be-moved-by-a-heidelberg-castle-germany#106697
 CTM 20100114: http://web.archive.org/web/20100114131747/http://white-wolf.com/vtes/migration.html
 KOT 20081119: http://www.vekn.net/card-lists/140-keepers-of-tradition
 LSJ 19970224: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/80KRDjVFkyg/TBJso9Ra_9QJ
 LSJ 19970225: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/xcp3faFaHZ8/_3NVdFJ3Tv4J
 LSJ 19970303: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/CiDrKyoNEBA/Tx55C65lJqgJ
 LSJ 19970325: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/R-t138q8688/Zj1Y_jlq29AJ
 LSJ 19970331: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/WXd9ALw9Xig/_REMI5bEeggJ
@@ -253,14 +357,15 @@
 LSJ 19970707: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/KWekwiRSa2I/9pS17rzBBDYJ
 LSJ 19970718: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/QujjxfQHYzw/S4tNTm4gpi8J
 LSJ 19970801: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/7ZnLKTdPEn4/6L-nVarAJwMJ
 LSJ 19970814: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Xd6HOjnqBpw/_wNl-bMoKiAJ
 LSJ 19970915: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/in3R3mQs5Do/41KNa8aVpV0J
 LSJ 19970922: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/k0Lih9MQf3U/VEkGLwInIq8J
 LSJ 19971001: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/_Yu65rf2qE4/TqY70rjSogYJ
+LSJ 19971001-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/RY_nhdykKP0/m/9boDeD_qAXAJ
 LSJ 19971002: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/RY_nhdykKP0/fOdKJtOy4kgJ
 LSJ 19971003: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/mUZ2704tVsk/K4b9NjIeDhwJ
 LSJ 19971006: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/2to9jkow98Q/loNTF9VNuc8J
 LSJ 19971028: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/ZKsbLYnas2A/oZJrA3kx208J
 LSJ 19971110: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/IlQdghRurtM/STZjah9cGbAJ
 LSJ 19971201: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/0I7KUhvhAig/kLiqzfugXTwJ
 LSJ 19971211-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/hMiAmGQ0RdI/FyEqqJN4ndcJ
@@ -316,306 +421,398 @@
 LSJ 19990709: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/F131j-4dabU/gS8SFKNu02oJ
 LSJ 19990719: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/kKtW2qo6ACE/4hs5tbGDC1cJ
 LSJ 19990723: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/6Lx2jnw7hMA/tMpV0CndVxwJ
 LSJ 19991025: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/R94tyTGJ6VQ/KxvkGm1aon8J
 LSJ 19991110: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/5hDqAMewLtg/fib2UDF58CUJ
 LSJ 19991207: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/aQaOTYwC-fg/vdyo09QZoicJ
 LSJ 20000103: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/0KEYzv22kjs/H4MWvI5F_hEJ
-LSJ 20000128: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/0VhG11O0s4M/fBQ_wsMkKtMJ
+LSJ 20000110: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/e8-mp_OMsjw/m/8j8xS9GPK3MJ
+LSJ 20000113: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/-qvB4bbD-rE/m/0EUdps3thQQJ
 LSJ 20000215: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/8to3EBsk-iY/jFT-RgP3WjEJ
 LSJ 20000309: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/ykAzsCzPkvg/bVefVZeCoQwJ
 LSJ 20000507: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/6-sMg4Wo7KE/s0fQkYbR5_QJ
 LSJ 20000622: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/znQHUWouQkw/-T_Tx-YRwrAJ
 LSJ 20001019: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/bSH8Q_kDhNQ/eHEX6PmfaB0J
 LSJ 20001031: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/y8LNZhRyXO0/m/EJzinwvnFoYJ
+LSJ 20001102: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/LlPyLJjLdx0/m/mXimdmP14GEJ
+LSJ 20001102-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/LlPyLJjLdx0/m/eVTwHPkEgOMJ
+LSJ 20001111: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/m23Hj3OW2A4/m/n23vvkXo6AkJ
 LSJ 20001114: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/qXSlM7Grq1c/cSDoQ9mw0z4J
 LSJ 20001118: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/r59jQZbWMi0/kesQz7kYbD0J
 LSJ 20001120: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Br8FPS5mRn4/2tbPhQquS7gJ
 LSJ 20001127: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/XgeLMemLbj0/pLPfOn3ijkkJ
 LSJ 20001127-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/KInac4MQMuA/m/LnpxH08HVbMJ
 LSJ 20001201: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/BPHZsY3p20E/S6HiRebyeX0J
+LSJ 20001206: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/kFIO74LxqFQ/m/U1Dtf3f4CPgJ
 LSJ 20010108: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/0gIA9tBZgIU/X-iiXNaoNVgJ
 LSJ 20010119: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/XB0IvK7I6PQ/foA7igsB8EEJ
 LSJ 20010110: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Vtm465mblX4/B6pCvotsfFsJ
 LSJ 20010210: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/NtMa5w_NVOE/jtpqcS6CwpIJ
+LSJ 20010211: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Fd9tcsKTzjE/m/dtIxb5Mof50J
 LSJ 20010227: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/rdkVAtZFC2I/rW1nXhSsyVcJ
+LSJ 20010303: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/OjxDSCbB6i4/m/xmsYv7Y27w4J
 LSJ 20010315: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/m9CrEOn1veo/gmx_Nou4BTQJ
+LSJ 20010328: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/VMAMljUO4NE/m/BHgmaN_3HRkJ
 LSJ 20010508: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/mvfdiWb-edk/P_8P7VblmR0J
 LSJ 20010526: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/0Sy3xNbjYeU/m/VAbmQA5axSQJ
 LSJ 20010606: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/2Dj_N6wtifI/j_bddYqDbOYJ
 LSJ 20010616: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/h7gnHNBFliE/MsfJ0qqv_jsJ
+LSJ 20010622: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/65IHHAii7ms/m/kyS0uVtsbNMJ
 LSJ 20010623: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/GN5MqcCTOo8/7ll40gxjFWYJ
+LSJ 20010623-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/65IHHAii7ms/m/uoIs8B1vdToJ
 LSJ 20010626: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/tkCRUBRp82E/m/Xz54yldDdycJ
 LSJ 20010627: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/NhNCVCCDyU0/I5Yph3-UUPsJ
 LSJ 20010629: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/MhHKBY7II78/m/EyI_ise9M-kJ
+LSJ 20010710: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/GsI1UyH54jU/m/x9LfDZX1vR4J
 LSJ 20010714: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/-xrhpMEiMrw/Vnr8QIyt41cJ
 LSJ 20010714-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/9U-jt3p3R_Q/WxDJwkgc25kJ
+LSJ 20010715: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/u91PfJOfOjE/m/BS264hmTIEgJ
 LSJ 20010716: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/x2EdFtlPs8Q/IPCbfV2Qct0J
 LSJ 20010725: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/2b0ITKe-WkE/ZI6UN0Lz-DoJ
 LSJ 20010729: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/RkvrP5tplXA/Wr-EQ_G0g_IJ
 LSJ 20010803: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/s1lJEsLMf-8/m/3CwIMglRboIJ
 LSJ 20010803-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/5QuGIF5ERUI/nGJoAyeiOJQJ
 LSJ 20010803-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/s1lJEsLMf-8/3CwIMglRboIJ
 LSJ 20010806-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/PuawBcgSIKI/D7zOKJXQDbMJ
 LSJ 20010806-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/5QuGIF5ERUI/3iHzZVBOjG4J
 LSJ 20010807: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/OPwaYA5R060/TUn6g3C5rQ0J
 LSJ 20010807-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/9ggmJcK2De0/m/XZKoCd27pf4J
 LSJ 20010809-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/LB6Zg4bEggc/g5eYOHiKrvUJ
 LSJ 20010809-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/9ggmJcK2De0/2xW0xE2SzisJ
+LSJ 20010809-3: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/gLl8F0zcCF0/m/cR8nsUweLQIJ
 LSJ 20010810: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/FUXkrq3B_O8/pimj1Vvw7WIJ
+LSJ 20010812: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/uXGLWUAuByc/m/omHFVEtV-A0J
 LSJ 20010813: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/8MR4bq0Cxj4/f_rAOuj3CboJ
 LSJ 20010813-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/zkKhvgZy9hA/m/8uH5sgbQaSoJ
 LSJ 20010814: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/z7uYIO39YCo/aufoimHncvQJ
+LSJ 20010814-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/8MR4bq0Cxj4/m/SH4dKuz8qO0J
+LSJ 20010814-3: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/4U6VYR9kBTA/m/1OjgFwTysAYJ
 LSJ 20010816: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/cRr13JeFGjE/l3kD2PHqpJQJ
 LSJ 20010817: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/wDLAn-jfdC8/HgbGe1OuZrwJ
 LSJ 20010819: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/2dXfHhG98Rs/RMqiA8RXDncJ
+LSJ 20010819-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/8MR4bq0Cxj4/m/YgNsk8nGcREJ
 LSJ 20010828: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/KoP_nqv-feM/faZPeRBTL_QJ
 LSJ 20010919: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/08AhThj0IxI/ZmMxUKqbymIJ
+LSJ 20011005: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/9fyH2X1YGAQ/m/r8ZViiGnRzoJ
+LSJ 20011015: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/ZXW0ScxTsBA/m/OvbMemV2oXUJ
 LSJ 20011022: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/KMg4MwD-Jn0/m/Vl-TD6DfyhoJ
 LSJ 20011023: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/2GOLIrXAF8M/P4T3Dj6UNL0J
 LSJ 20011202: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/gyzUP4TCq6M/D-u3Uzdy6SMJ
+LSJ 20011202-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/qnVBhys6loo/m/5IuE9b3iTyoJ
 LSJ 20011204: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/LFm6fYzoUhA/dkWYGi9nw4cJ
+LSJ 20011204-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/0gKrr9ChclY/m/WYNIe2IgrCoJ
 LSJ 20011205: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/dkK2L81_cYk/mj0NOMJAGucJ
 LSJ 20011210-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/mUwzyHLcAx8/BFFVIH0Ha2kJ
 LSJ 20011210-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/mUwzyHLcAx8/GghxO9mnnTIJ
 LSJ 20011210-3: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/mUwzyHLcAx8/u4tViuMvZDUJ
 LSJ 20011210-4: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/WT1LwCFnU9A/T4bZS_BQXGUJ
+LSJ 20011212: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/3jinbBVvqIE/m/9QaMi2N1VeoJ
 LSJ 20011214-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/m2zsNI0McoE/-izuxRCo9VQJ
 LSJ 20011214-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/TinQ8ywzIHU/-zW_hcYbiD4J
 LSJ 20011214-3: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/9WJX_WF656A/2V1mYoHPB6IJ
 LSJ 20011214-4: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/RSCjaaZXY28/IQxqjgU_oUsJ
+LSJ 20011215: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/9WJX_WF656A/m/LpUwuigFmJkJ
 LSJ 20011216-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/xwirj771uGM/0w1qJBEabFEJ
 LSJ 20011216-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/eYJFjfISdPY/LplHHT2EZ68J
 LSJ 20011217: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/vZ13bh7FEvQ/KaZlbqc4LO0J
 LSJ 20011222: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/DlCBJmB2fzY/HVLdn4Hr9uIJ
 LSJ 20011227: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/vmLYOzOcbKk/Es7UfevBY-sJ
+LSJ 20020109: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/3aWGnESUYi0/m/8CQ3HDk-SrMJ
 LSJ 20020112: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/9yhb-ToEzL8/Eq59W8cS65YJ
 LSJ 20020115: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/wG_tDLgfZso/6mKkp7Rw3OcJ
 LSJ 20020122: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/IBZTtnqENJA/_S_AQxZO7xUJ
 LSJ 20020123: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/F2PELnDgM_g/t6YG7lvcmyoJ
 LSJ 20020125: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/dF5BNipvcQ8/aB0krwu_PMAJ
 LSJ 20020126: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Fhm2Zi2RZRU/K4FiHLWuSbMJ
 LSJ 20020204: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/DDjGFeolsxg/bM64eWo1jCEJ
+LSJ 20020301: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/HgmPj9MEdiQ/m/P_y2T-_6MH4J
 LSJ 20020304-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/oDdTAxootPQ/REL0GysRZrEJ
 LSJ 20020304-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/L-8OGYP5xsE/h5WnSofVrfUJ
 LSJ 20020314: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/1uKDkopJTRo/w7d5OktOJhYJ
 LSJ 20020402: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/eQCXHND3j5o/LMv8SYYE3OoJ
 LSJ 20020408: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/4LXlqwmGQGc/m/S8aQ4et5KMIJ
 LSJ 20020416: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/XS0Z0P5qaew/5hv141ZGzTIJ
+LSJ 20020416-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/tEC5uN8yqUE/m/czJYA-Pt00sJ
+LSJ 20020425: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/_Rh8P34zTZo/m/u-WavRjp5uYJ
 LSJ 20020426: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/xFGNrTa9CPk/FNTh_ouCem8J
 LSJ 20020429: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/7ZfedGTVt9g/kQnfy7J_UYkJ
 LSJ 20020505: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/ka9MajuWTAo/M4oCzY97K_kJ
 LSJ 20020509: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/-dqteu2lStc/0b9C4HuqvUgJ
 LSJ 20020609: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Q_Lk0DPHqC8/nAfGfCvsISgJ
 LSJ 20020618: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/DVGe6EsiMZ4/2-t1mFMkAX0J
 LSJ 20020620: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/WoXWzLYaFSY/ug3CHnpMCUQJ
 LSJ 20020708: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/KK_YwtQwA_A/mah4T5BCrqUJ
 LSJ 20020715: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/-FBxPz-oms0/OV6b9Cc6nl4J
 LSJ 20020725: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/wCPFIH_g5ZE/inchZQXKRrsJ
 LSJ 20020729: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Tn1wLMpNbbA/-h07t8dtp6YJ
 LSJ 20020819: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/WONdURITUdk/9EnfVPy0P-MJ
 LSJ 20020821: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/o_nBNZraMvE/g0xPNLGquKIJ
 LSJ 20020904: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Qmi4hFk6QqE/VmoU2tfLMgEJ
+LSJ 20020904-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/ObuKimgcCpI/m/PVsmKoSZueoJ
 LSJ 20020911: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/_lLSO5aevoM/7BXDmpWjdLIJ
 LSJ 20020926: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/C7vgb-0Mcbo/6UHJsQjBs9wJ
 LSJ 20020927: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/wg3PH7vOs1s/gYFNbAwk84gJ
 LSJ 20021001: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/FW-bmZpIM68/gLoYcvpUB7UJ
+LSJ 20021007: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/wkyqKMka_F0/m/PY1IegrQszUJ
 LSJ 20021008: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Mc3xfym_uw8/zY9ipcHSXF8J
 LSJ 20021010: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/IAamJNEJAug/iztHSQVIUcYJ
 LSJ 20021011: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/9WWIzxek9Nc/PlIwI11sNpkJ
 LSJ 20021022: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/WIXqYpkKuj8/lDWFfFjwn8YJ
 LSJ 20021028: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/g0GGiVIxyis/m/35WA-O9XrroJ
 LSJ 20021029: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Fzf1e2xsywo/9bQkJCP9VQcJ
+LSJ 20021111: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Y6_dPn4ONCA/m/xkVBf0DCQM0J
 LSJ 20021113: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/df2P8YHZex8/mGCmsxDjI_YJ
+LSJ 20021115: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/35vszszGZOA/m/GXrurZ9Rw-oJ
 LSJ 20021117: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/4TgUatcTtdk/HfuRL6wM8IcJ
 LSJ 20021118: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/AhLw5v3abjU/L4d8Qv_C2osJ
+LSJ 20021120: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/4TgUatcTtdk/m/OUN021UtXV8J
 LSJ 20021121: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/UddkVI7G8iA/qqR2EMYZKIYJ
+LSJ 20021121-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Nc72KRVbd-g/m/22PbqShf7AMJ
 LSJ 20021122: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/LieFYA_gyFo/Ma_4_gNijmoJ
+LSJ 20021122-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/1hL0-URtroc/m/iF5fPuJC39IJ
+LSJ 20021122-3: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Nc72KRVbd-g/m/_Jb9Sn3xP3cJ
 LSJ 20021126: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/9Ui7pesvu5g/P4p-nKZa6lQJ
 LSJ 20021128: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/6rqhybcysh8/m/hU-qIp2on-YJ
+LSJ 20021205: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/0MhU0auTJO4/m/39sI3Lpp-6MJ
 LSJ 20021210-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/kOZf54CTBUU/rVsPlZzjfpcJ
 LSJ 20021210-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/e5fb3G1uruM/jtWcouG1oWMJ
 LSJ 20021211: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/-J07wvmidOA/gPQ5ngEZ6HcJ
 LSJ 20021216: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Ej5bSsK__Ig/lnH8iRgZVWkJ
 LSJ 20030103: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/TUDO_4FwdyY/DWOwgQL850gJ
 LSJ 20030128: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/d25nONe01WY/xqfEs_qwc7gJ
 LSJ 20030202: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/ox7A8EvaNJo/5CyLJo7pmUYJ
 LSJ 20030211: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/xhpVMShX6qc/6KDcgiFIxhMJ
 LSJ 20030213: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/j6cuQ6pFJSA/F-A_hlBMpd0J
 LSJ 20030213-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Jwj7VjhFU5o/m/VbR1wZ23gvIJ
 LSJ 20030214: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/A3U-Dy1yx8Y/2LHXvLrmybwJ
+LSJ 20030214-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/nU7PaMBymtY/m/ELcjZX2caJUJ
 LSJ 20030219: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/ugfckv9DAbo/w5UP-Ch-u5MJ
 LSJ 20030224: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/67261v339Ds/um8V7VVp2Y4J
 LSJ 20030227: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/c9KLhUd-Isg/Zz0zAzvZ8TYJ
 LSJ 20030307: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/zhdj4jnSdrM/tAU_FosRtbwJ
 LSJ 20030311: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/MEiIvNrW1tE/ByXcnD9kP04J
+LSJ 20030419: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/A0mvllC-tgs/m/GqjZTFN9SvMJ
 LSJ 20030426: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/JmGLxQmAF6s/LrO51CS3CgoJ
+LSJ 20030502: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/qBa9CvBwqNA/m/ZuBgMjNgb6EJ
 LSJ 20030511: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/qSKbZFF7F2A/0_Wt6FIxdqsJ
 LSJ 20030514: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/rpmELY0yqYo/MQpM_6DYmfUJ
 LSJ 20030519: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/E6Jz8m3iKrA/BoCMzQoGzyQJ
 LSJ 20030519-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/mi8M1lSCLqo/Rdg9SU5nA6QJ
 LSJ 20030520: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/wltIoG3qv_I/m/8-SFgJp_hmUJ
 LSJ 20030520-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Z2fW6tgT5u0/QVtombu2I6QJ
 LSJ 20030520-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/GcymCHOJDVY/bM6Z5o-beQgJ
 LSJ 20030521: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Ude2or4n9nI/6u41LfeOpQQJ
 LSJ 20030522-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/_krZG-uPtzc/94US5l81edwJ
 LSJ 20030522-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/iBfBo7CQn4Q/-0EK5GbgRZUJ
 LSJ 20030527: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/1hViTSXv544/nOXqGMitwP0J
 LSJ 20030530: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/SZehI8SwAc4/shpyPIdsHxUJ
 LSJ 20030602: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/dy31XE695_M/4UCERLZkIDgJ
+LSJ 20030604: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/qzKS4OGBgbo/m/jk080A7XCM4J
+LSJ 20030606: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/qzKS4OGBgbo/m/ST8O8A0s-JMJ
 LSJ 20030607: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/DG7s60pwv1U/FPqlZYJ3upcJ
 LSJ 20030611: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/B6tpOePX23k/QOleeYB1UXEJ
 LSJ 20030618: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/AdfUNNicx-Y/SDYFb37pS-wJ
 LSJ 20030701-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/8pVaGxWYeyA/hDIxE9ipPCgJ
 LSJ 20030701-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/EFBCP5QI3D4/oU1yyA3yV04J
 LSJ 20030717: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/IkMD8wfAcqw/2OdnRU3Q1AQJ
 LSJ 20030804: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/xvDRXblcRuE/dJykGOlpw2oJ
 LSJ 20030811: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Ivy3fm45bb4/7AYdBH7VI9QJ
 LSJ 20030815: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/sf1U7vnVE-o/m/VjhroQN1NP4J
 LSJ 20030820: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Zjmffk-EbJw/m/ExNZqDUNQt8J
+LSJ 20030828: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/enVCjRhydLo/m/tj5HN0_n98gJ
 LSJ 20030902-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/GkOWrvV3r-A/nPLKDnFUO2wJ
 LSJ 20030902-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/mgZt4f2LyOg/FCeKmePPkxwJ
+LSJ 20030917: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/i3Ugq5AQWFI/m/TxPoXM78hFAJ
 LSJ 20030918: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Lae6k2AG-1c/GOqdTox6CRsJ
 LSJ 20031008: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/JUnIGIrb3pw/m/EOo-cGykdmYJ
 LSJ 20031010: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/clifT98_Zrk/aQ4cGuJnT9wJ
 LSJ 20031011: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/GZZJjzAeuxU/HtZKyNDKiOAJ
 LSJ 20031106: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/bFZCLXzzOeM/n1C6p6xw1O0J
+LSJ 20031107: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/NvxFMexSI7E/m/K57vIUVqMAQJ
 LSJ 20031112: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/NW4HWUWlzDI/qDPeTd5ZuugJ
 LSJ 20031115: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/quF7butlINo/XVswJuKMke4J
 LSJ 20031116: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/RQBw8EnnD5s/NpdTwIuChy8J
 LSJ 20031118: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/9IzmBh8PWe0/J1F_TzPbITsJ
 LSJ 20031121: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/JQO1RBmvV_o/jrmvVW9GH8oJ
 LSJ 20031121-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/cfs3xTrlpWw/7qfMkeQbcMkJ
 LSJ 20031121-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/1khXmKPU0ws/Je_X4gvv72kJ
 LSJ 20031121-3: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/JQO1RBmvV_o/-U5iv7M12vAJ
 LSJ 20031123: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/HvM2cHJ6yIo/jsb4iRoNdWkJ
 LSJ 20031201: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Mi_j7sUsZZw/ScJPKbfiCAgJ
 LSJ 20031201-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/6lN9MbBeL1E/m/C5qoUyYbEhkJ
 LSJ 20031212: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/dOATNbVuaqs/g8FtHUHX1kUJ
 LSJ 20031219: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/leLLrcPsiBY/cnSR-CQGqdMJ
+LSJ 20031221: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/OJW-3jpaM04/m/LLYmjhAWO7kJ
 LSJ 20031223: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/aX7VSvx7StE/eMGh6jnFA2gJ
 LSJ 20040120: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/5zBRtwg6lpU/MMisbKi7_Z0J
 LSJ 20040127: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/2b3SFZyo3ik/2hwET6zRCykJ
+LSJ 20040130: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/wvuR79dNCDU/m/z4C2L5NCgg8J
 LSJ 20040210: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/FWzKVXDEJ5k/ITxevWshkYIJ
 LSJ 20040312: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/1mgJQkrFNlc/k87rUTTAWFYJ
 LSJ 20040415: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/XTya9MiAiqc/4cejLmkUwEMJ
 LSJ 20040518: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/4emymfUPwAM/B2SCC7L6kuMJ
+LSJ 20040518-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/4emymfUPwAM/m/JF_o7OOoCbkJ
 LSJ 20040519: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/fz-EAPmmqZY/bj4sR5CxnmQJ
+LSJ 20040521: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Giv8nDnYVGo/m/RODFe7KlT1UJ
 LSJ 20040526: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/M3hDKK2JSWw/Z-W3F1vO8fYJ
 LSJ 20040531: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/oTb4vsFNi1s/pCwoAggb97UJ
+LSJ 20040531-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/6K2TqucrNzg/m/41EuHsVjHlYJ
 LSJ 20040601: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/bEvYg3Za-fc/p0CSDyi5MWkJ
+LSJ 20040602: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/bEvYg3Za-fc/m/eK2rBRFelmoJ
+LSJ 20040608: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/p1uCHeAO7ak/m/n7qfDGYXuu4J
 LSJ 20040616: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/jQkkiC3I8P8/m/uDZ--HnPtf0J
 LSJ 20040617: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/WxJVsEWWmbc/gbOBOI7T9kwJ
 LSJ 20040623: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/PlPp5igHOEg/6IOQqMJA53gJ
+LSJ 20040701: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/O7cT51Yl2Uk/m/RvMWaiqAFS8J
 LSJ 20040722: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/z3Tfg9PZVNo/TAasVyubnpsJ
 LSJ 20040726: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/LlqCB6LN64g/k98Xj1pwjPcJ
+LSJ 20040728: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/LlqCB6LN64g/m/SUqRp4DoJIEJ
 LSJ 20040730: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/vCZw1_QnhfE/6dxskyrN040J
 LSJ 20040802: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/b6V_OGl-TgE/bi8evHga9X8J
 LSJ 20040805: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/WuER8RUMzTE/OmQhmQFkFLkJ
 LSJ 20040812: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/n_0DGDsWG0E/lxG2zMPetwAJ
+LSJ 20040812-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/E7D1cVmAdqQ/m/MvPApbrT14gJ
+LSJ 20040830: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/KHMhiNiSKo4/m/MCfo9aA-EjcJ
 LSJ 20040928: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/GBcR6aNjIk4/DXPyqBM1R8kJ
+LSJ 20041004: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/UZbyxuVsTJE/m/47dqvgl6t2QJ
 LSJ 20041015: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/jonKzp3f8wA/Dgropqbf_WwJ
 LSJ 20041022: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/gqhND6kd2wE/LDmEotxa_4kJ
 LSJ 20041022-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/UAhJ3vWLyMM/m/gp04WTgORSQJ
+LSJ 20041025: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/sbfkGmojYao/m/obMvk67O5PYJ
+LSJ 20041026: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/54Zr4RUuVx8/m/fJCT8qW_90EJ
+LSJ 20041027: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/BHeGvhd4yEA/m/SdKih5fV34wJ
+LSJ 20041103: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/MiPHVp-NmCA/m/P323pUaD4DwJ
 LSJ 20041115: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/ZCmZl5xUhis/m/YoKKqsiFLFgJ
 LSJ 20041119: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/HMV_pN5mJhQ/tzkinpwUq-MJ
 LSJ 20041130: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/6uTPqRg387A/fa9DW8-Hu38J
 LSJ 20041202: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/8MwcrUpCdBc/E5hnEF8WU8UJ
 LSJ 20041203: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/_iogrCkrCmc/hTkREMXGFR0J
 LSJ 20041207: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/6oC7FtG2Ac4/lI5hqeuSioIJ
 LSJ 20050105-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/vze_ZUJmzu8/cSZJ6ku_bSsJ
 LSJ 20050105-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/sAErRDiSXfU/GMQXJ7TvOrsJ
 LSJ 20050111: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/lnW6nMIX-Vw/iVd07z5jvu8J
 LSJ 20050112: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/p-v5jrPSEUc/3LsqQl9ZFLkJ
 LSJ 20050114: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/JWiZmyC2Y6s/q6JHYrE1zKYJ
+LSJ 20050116: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/yX5rqVaarvs/m/w6JXnFytdq4J
 LSJ 20050117: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/yX5rqVaarvs/Ih0zSqVPCpgJ
 LSJ 20050119: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/NKWhBnp7uP4/6_56LlSV658J
 LSJ 20050128: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/HVy8iPUxNbI/ZHGTnprQjGUJ
+LSJ 20050128-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/HVy8iPUxNbI/m/jXmrJxMaJ9MJ
 LSJ 20050201: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/YRp5TkzBJtA/r1YYYNte2gwJ
+LSJ 20050215: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/nxlYFsU10Uo/m/Teu243qv5JgJ
 LSJ 20050216: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/5_rUFgufFc4/7OVVD0KpnS4J
 LSJ 20050217: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/RhZo11Io6wQ/1u8j1gtUJ44J
 LSJ 20050221: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/ms3eqcaR37Y/0ABXbBPcfpcJ
 LSJ 20050222: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/pwPVmNg8hDY/DB4eM98iptkJ
 LSJ 20050224-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/enxwleC-ZKw/zDDSPMF8FOYJ
 LSJ 20050224-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/ms3eqcaR37Y/GkYdPiu4aHQJ
 LSJ 20050224-3: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/tzl6213crbI/HlnYVX9L3fAJ
 LSJ 20050224-4: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/LATlh09TuhA/m/oAcvZ7MfWCIJ
 LSJ 20050225: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/OjszbddbvxM/eKkxVIJPoG4J
 LSJ 20050228: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/UHEZEmX22jA/6_EZbs5DKb8J
+LSJ 20050228-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/xBb9HQz2KPo/m/sKirLvafQqUJ
 LSJ 20050304: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/X5JZBbSIj3U/CBdkcQ-rAesJ
 LSJ 20050315: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/COcJX2hHP-E/YLUW8FaGP0kJ
 LSJ 20050322: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/vhSqnoAt_Bs/ARfTKxaZII0J
+LSJ 20050322-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/jiavUD9IgIA/m/SuMUFkb5uLMJ
 LSJ 20050324: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/vhSqnoAt_Bs/m/4yurSS3iyqAJ
+LSJ 20050324-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/aIzKlsTs51k/m/D07dQjMzaj4J
 LSJ 20050331: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/J0CgOqvbfEk/P1VelhBkcr8J
 LSJ 20050407: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/fDl3t2lJ3Pc/m/pdmWZOwllPMJ
 LSJ 20050408: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/idZy8QCxBT0/ymQE3s1kEkoJ
+LSJ 20050408-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/1TXRhYopt70/m/74vkJl3Fh4wJ
 LSJ 20050413-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/1TXRhYopt70/OZMBb0AlfOUJ
 LSJ 20050413-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/1TXRhYopt70/YnL8Fiaim0IJ
 LSJ 20050422: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/nJPfMOuTBtw/COytKb_oEM4J
 LSJ 20050503: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/GZI8NXQ76d0/o16kURwaEpkJ
 LSJ 20050514: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/9803Eu3PvDs/4xj8UAK_LZAJ
 LSJ 20050526: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/x98guZkL_CQ/m/5JmxFmAbm2IJ
 LSJ 20050606: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/IkZS3ikg7y8/TrHmf3-jPvEJ
+LSJ 20050607: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/WLv9R8wA0Ow/m/gQyOMb3fEKQJ
+LSJ 20050607-1: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/vet0HGRxtXQ/m/gRJalPv4lLoJ
+LSJ 20050608: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/WLv9R8wA0Ow/m/dyAPpxSMoSYJ
 LSJ 20050611: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/8GYIKyvuCZE/ivBTcweeiQQJ
+LSJ 20050628: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/lN3eieA3xgs/m/c4ZoOWHUsPEJ
 LSJ 20050707: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/S5UbigI9faM/7RcuPKon0R0J
 LSJ 20050720-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/mXvDlPLD0xc/__oHDkVhntkJ
 LSJ 20050720-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/1vbIkgvKDJ0/3ErIIMXFgPIJ
 LSJ 20050721: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/g39H3dwXqvc/R0kKrr7JDasJ
+LSJ 20050727: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/QfVIg4fJP38/m/wMJU5oik9G8J
 LSJ 20050804: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Xqa8boGP7C8/m/fpfYjwbay0QJ
 LSJ 20050805: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/mJzy9HKytEc/gt6s2WzEqUMJ
 LSJ 20050927: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/oLMw6SSSgmA/-iwdHzdBMF8J
 LSJ 20051012: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/oxZkE2Bfw3g/m/mXGC9ZlZNzIJ
 LSJ 20051016: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/s_At5syL66k/1eGsxyhDn1YJ
 LSJ 20051017: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/s_At5syL66k/bCvu2ks001gJ
 LSJ 20051020: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/jqPoW66sEkY/m/RH3yS-8MQCoJ
 LSJ 20051103: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/BD7KIWBI0Cs/g8vJICHAu7oJ
 LSJ 20051113: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/L-ctaLucuKU/dG0EKdSd4g0J
+LSJ 20051113-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/O2cgcyCHBSI/m/7vfAvsEbiU8J
 LSJ 20051116-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/MfGC7sJ8vh8/9ylhc34zFesJ
 LSJ 20051116-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/5Bovsb8I6R0/_KIlJky3D5oJ
 LSJ 20051121: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/51XITiJtdjo/A9jSHsxBX8QJ
+LSJ 20051123: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Ww3zSY8cVNs/m/QVDV21-IjysJ
+LSJ 20051126: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/dDgHGEG18D0/m/OMk_F9bKqW4J
 LSJ 20051127: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/1rIDrVs8Eyg/GN6WCp2IRUgJ
 LSJ 20051205: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/K-RE-nTJ_Cg/Ao3LhiAPXk4J
 LSJ 20051207: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/H_Tuv0uJt1w/ccPPm2lSjyIJ
+LSJ 20051211: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/TuwXiJ8A9mo/m/Ef_5xj46lA8J
 LSJ 20051220: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/bIcX7F3wzf0/Oi91XAFSwKUJ
+LSJ 20060124: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/PBEBNFH61ik/m/Fp2dosujs5YJ
 LSJ 20060209: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/ZuOfZorIhhU/m/X5G1JfqDPhcJ
 LSJ 20060215: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/BhecJx5BqtQ/nqEdwFmnQnwJ
 LSJ 20060217: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/BhecJx5BqtQ/MjBL57IRDjQJ
 LSJ 20060221: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/OC41YQYfJO4/g_y0RPVpXNkJ
 LSJ 20060222: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Gv-gf5sAJxM/4scio5aXDCkJ
 LSJ 20060306: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/H-W0Wqx3t9w/jgTHm_Ac8dwJ
 LSJ 20060323: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/taLKfNyQ3Kc/Av7TF4lHvpUJ
+LSJ 20060409: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/gsFQXsCGTG4/m/q5H8FvuKksIJ
+LSJ 20060409-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/lWdr_Ym-UIg/m/t_xVzJIXW18J
 LSJ 20060410: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/jr8wSeSchsc/xIIeqsJxHrIJ
 LSJ 20060412: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/DuZXjDEQ9cE/Q4MdfMG2eFUJ
 LSJ 20060413: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/3A3y_02b0SM/m/qbc6r19b128J
 LSJ 20060417: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/bW_XZDS-9iw/u_WVQXNXK0kJ
 LSJ 20060421: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/5_Y7HxiR7wo/qLgr38ocXA8J
+LSJ 20060425: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/U34QDob4Vco/m/hcaMIn9W88kJ
+LSJ 20060426: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/4e6z1_JWIzA/m/oMQz7oVR1O8J
 LSJ 20060502: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/EksUAQcZeS8/uZRZ-a29rJcJ
 LSJ 20060503: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/ckLtVMUM4QA/YrTPgsyEHCkJ
 LSJ 20060508: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/5uz0i-W7BjM/xMfwRHMhvW4J
+LSJ 20060509: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/KBFnBRrOGB4/m/7ZYNQnvZ5tEJ
 LSJ 20060515: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/bzusnKlnYr8/OSMvzE7YjokJ
 LSJ 20060522: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/2f0wF9CECu8/SZn9iGo-LOQJ
 LSJ 20060525: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/0HqW_TzbJlM/WZecj55DSCkJ
+LSJ 20060530-1: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/7ezcZoziFWw/m/bkivGTQIO3wJ
+LSJ 20060530-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/7ezcZoziFWw/m/G07cu5_UZnQJ
 LSJ 20060616-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/YfU6gWr_rzw/u50SFeBMpoEJ
 LSJ 20060616-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/YGA7bnOj04Y/wOVi6CvB8Z0J
 LSJ 20060623: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/mfgW0TeoLNM/e_QgbzZCqa8J
 LSJ 20060803: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/z8Nd8EFQsKc/sP8_LxnEpEIJ
 LSJ 20060808: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/ncZn3knH-Uo/sBjnMxAk1msJ
+LSJ 20060808-1: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/7oK-hKbOs9g/m/EGeyVt3vfl4J
+LSJ 20060815: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/nxExSHh-QjA/m/QFBqiTmg3scJ
 LSJ 20060824: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/zsZTYTbRVRI/VmMfnKWuMlMJ
+LSJ 20060831: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/wdVbwFZo8Jg/m/U8P1de7moZ0J
 LSJ 20060902: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/QAKz6Qtr7Ts/JpnA6qgxS2oJ
 LSJ 20060903: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/QAKz6Qtr7Ts/kyhzKIdtR54J
 LSJ 20060904: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/L9D4GK0yNv8/H9vnUciv2psJ
+LSJ 20060908: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/CTy2GjM6-Dc/m/9OPulYVGaFcJ
 LSJ 20060911: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/oznDQgIFZ-I/dU2xMMkxPwsJ
 LSJ 20060913: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/GpSAQnN6GnY/m/6EqRGDT3u08J
 LSJ 20060921: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Lj1GDLBmOWQ/m/-ZbHv_NcqW4J
+LSJ 20061013: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/6w8K3yDtBH0/m/M_SZH9Id8n8J
+LSJ 20061018: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Prc45fTQd9Y/m/uvFhSQKCBakJ
 LSJ 20061109: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/b3K7k1mRyno/8pWeDHZpbw8J
+LSJ 20061207: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/nqcrJlhg4Ng/m/qQu7p-LLhfAJ
 LSJ 20061212: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/h3onVZ1NqpQ/JYIxdaT9wMEJ
 LSJ 20061218: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/DTBI6LkPdZ4/m/Qtu3QUPERdIJ
 LSJ 20061222: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/WUKedBpp_h0/m/LpJkrGZWvg0J
 LSJ 20070124: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/5YMceht1KTk/LhhbEr_dlU8J
 LSJ 20070203: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/37EYK3FA30k/QynliahgIzQJ
+LSJ 20070208: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/ssk96EKyqjQ/m/VfgesEwO2FwJ
 LSJ 20070213: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/r1DkV0T8y00/Sh3T4mXd5ZYJ
 LSJ 20070214: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/o_BltcAJ_So/r_uEap9msOYJ
 LSJ 20070217: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/HkKuwBe9LRk/3GccpU4eaK8J
 LSJ 20070222-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/jBrfK77gayo/fnk0EgSpN8AJ
 LSJ 20070222-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/jBrfK77gayo/X4wqXnwhzDoJ
 LSJ 20070224: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/lJBIPgsqNDg/Xoa0o6DDlWMJ
 LSJ 20070301: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/-CeFWHQ2wXE/TtbyH4rAcoIJ
@@ -628,192 +825,254 @@
 LSJ 20070320-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/goUs4JXcqMw/-o_yFpUV-TIJ
 LSJ 20070320-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/QPCnTltI2Rk/_DIkIPJSPTgJ
 LSJ 20070322: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Ww-4rYJxi4w/P3QchWVq2o4J
 LSJ 20070327: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/YInnFoJPx2Q/NFvi36RWFrkJ
 LSJ 20070328: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/3o0R9bLjrQk/9TjsEa_VnhAJ
 LSJ 20070330: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/gsI3SYz2g3o/Fj3x7Kn32HEJ
 LSJ 20070403: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/TJ2ktt_1tjk/fdH_x9tDmN8J
+LSJ 20070410: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/NCJeinNxGfo/m/-_dXQoBdDysJ
 LSJ 20070411: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/umdINigMKqs/l6GFRVKdkMsJ
 LSJ 20070412: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/umdINigMKqs/vY4r8FjrEyQJ
 LSJ 20070413: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/umdINigMKqs/lfUAxTnfttIJ
 LSJ 20070417: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/ecDUqbSUsNg/m/3W9aOm0MfYEJ
+LSJ 20070507: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/FOLkbrSh0Ns/m/wdtfyqkD26MJ
+LSJ 20070508: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/FOLkbrSh0Ns/m/Kbt2Ox1GBI8J
 LSJ 20070516: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/zalQ_AHTpAY/vODJ6Q6CluUJ
 LSJ 20070702: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Y8fFI0VCwfw/e1xrXrq8T5gJ
 LSJ 20070707: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/ZtRk5z2TcoI/gJWD0dT3kUwJ
 LSJ 20070709: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/qKrJPLXBFFw/hE5z511E_PgJ
 LSJ 20070808-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/jzMOxZ9oxOs/o0X7GUFmii0J
 LSJ 20070808-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/gaFBeSrs7fU/v0VVEOJd2HYJ
 LSJ 20070829-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/sVXZw1J43ik/OByFPgQsynwJ
 LSJ 20070829-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/drn7wHaGugQ/QqaYmjAf2UYJ
+LSJ 20070829-3: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/sVXZw1J43ik/m/J018OOhbEoQJ
 LSJ 20070901: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/EouVnC0MuH4/_b3gw2Hqxb8J
 LSJ 20070927: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/VaSQ7JL2N2Y/m/BenDHsAETG4J
 LSJ 20070928-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/duRrP46XygI/h3Ogu8JeQ-wJ
 LSJ 20070928-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/duRrP46XygI/FrFYvbUYFf0J
 LSJ 20071001-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/bb9ac-kN5WY/l8mfTxW6a6gJ
 LSJ 20071001-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/XoMeEYJw1ZA/zVM8X9aZlgQJ
 LSJ 20071003: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/duRrP46XygI/zAHBdn4JnNQJ
 LSJ 20071005-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Ugcdb0ljZrU/J3Gqxj_615gJ
 LSJ 20071005-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Pwt8I_uj4GM/DmSZbjSFqwIJ
 LSJ 20071006: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Ugcdb0ljZrU/RAS1IrL9FM0J
 LSJ 20071009: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/vSI2MhyB710/QweM8isk3f0J
 LSJ 20071011: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/GSQqnAEBkgU/gFKF1ltY4JEJ
 LSJ 20071014: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Bom6ae7qjbI/OznLIo66qgsJ
 LSJ 20071015: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Bom6ae7qjbI/1ov2qqChTdMJ
+LSJ 20071015-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Ei307R78l4A/m/sZzwphkIbH4J
 LSJ 20071020: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/ap2IBEgm0gI/sL_XyMwDK4cJ
+LSJ 20071021: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/E6FhLDRCIL4/m/VYR_7Kcf70oJ
 LSJ 20071112: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/2fFyhL6YqI0/-zsMEGtt4qEJ
 LSJ 20071116: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/ZPsShBUBWZI/MJ9zobOVjHkJ
 LSJ 20071206: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/B-5oDAJrwiI/ui9coMgXYUMJ
+LSJ 20080106: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/q4s1P6ozsW8/m/N9wEQl5sgTgJ
 LSJ 20080107: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/XpZ6F53jK-c/m/wB6HHGzgFi4J
 LSJ 20080109: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/XpZ6F53jK-c/m/EQWCLO72MbsJ
 LSJ 20080125: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/HcCobkGPcFI/GlBdNwMvAjwJ
+LSJ 20080201: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/y5Uoc7nEulU/m/Nbp6ZMfhj1wJ
+LSJ 20080212: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Yg1nZfgkpGM/m/OxDoRLREnewJ
+LSJ 20080226: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/NAfcSQEiLXY/m/GyMO2byB0AkJ
 LSJ 20080314: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/GqHN0I3c8Sc/m/PsOWtyMWjXsJ
 LSJ 20080326: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/KUQEznVQlOU/e_6GMg__zdMJ
 LSJ 20080409: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/jrN1Pc_Quk0/XwWAWfq_KRIJ
 LSJ 20080426: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/VIV521VtVfk/m/qQRxntT52F4J
 LSJ 20080510: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/67g8kq3F_uw/MAAoEV0Jf_kJ
 LSJ 20080512: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/z2DGSFph6sM/IjJB89nbtlsJ
 LSJ 20080526: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/zO3l3b76rjQ/da5R20AzyO4J
 LSJ 20080602: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Y7CLzywq1Lk/m/LXmN17pA7_UJ
+LSJ 20080603: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/9usl4idp-pY/m/LuT1iK1b4QIJ
+LSJ 20080608: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/j5ShUmUt-vM/m/E0CqmXp_R0IJ
 LSJ 20080610: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/EhVw3OReUfM/m/_cPn7mi3dTAJ
 LSJ 20080611: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/gvb3uijtpZw/m/ZRX2hunjsRYJ
 LSJ 20080612: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/THFR8YTXxGI/ocQc4IRWP1AJ
+LSJ 20080612-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/dVIBPf6EX_8/m/km-qYBcG_qYJ
+LSJ 20080618: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/9FAkwIsuYZc/m/gCoYa59TEGIJ
+LSJ 20080619: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/-JNytF94ST8/m/jOxRkvh8RGwJ
 LSJ 20080630: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/nvuXBpEaKAA/ymiC3yAQVOwJ
 LSJ 20080702-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/JtLgB7Apqq0/lWdtq38KJ-wJ
 LSJ 20080702-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/sCHpPQkjeAE/8N5_G2gMHAIJ
+LSJ 20080702-3: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/sCHpPQkjeAE/m/SLhxvwuWksMJ
+LSJ 20080702-4: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/sCHpPQkjeAE/m/9GGAf6TbiP0J
+LSJ 20080704: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/x1Y9FN8_Umc/m/UldJJICdotkJ
 LSJ 20080710: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/f1NpGhdtk-E/MEbLGzSGessJ
+LSJ 20080717: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/DMsE6V84GWI/m/af5Oggz9XlQJ
 LSJ 20080725: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/jWWCwKnran0/6JxzHnKdJkkJ
 LSJ 20080803: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/VgARso4nY7w/cAl0o7WpblAJ
 LSJ 20080803-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/OknxGrvlaNk/m/khteZ5WaNE4J
+LSJ 20080804: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/hVrshXQpuW0/m/fI_DIfQBNaIJ
 LSJ 20080805: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/SIbzFAwWDKs/BDkEg19txtoJ
 LSJ 20080809-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/1jW6GXrIRSU/7ywPFR39rb4J
 LSJ 20080809-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/1jW6GXrIRSU/6SpheeDqQeUJ
+LSJ 20080812: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/1mAsWziLz6A/m/wnxA8qxJMhkJ
 LSJ 20080815: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/0_1JBbdwi74/c1GepnS4ylEJ
 LSJ 20080818: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/O5HUPRkKY-k/IVBZIwrEtboJ
 LSJ 20081002: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/OUYG4nuy3Oo/MsxvJfM9vuQJ
 LSJ 20081016: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/GizIs4K_HiY/sCutpP29EgIJ
 LSJ 20081120-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/e2PNDpg-l_c/zsGPhfQgLL8J
 LSJ 20081120-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/e2PNDpg-l_c/wqEDxGHKJQgJ
 LSJ 20081123: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/_Pb29pBJ1kU/8ugWH0lVOtoJ
 LSJ 20081124-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Fp4wSGFJ7N4/GQlX8JKdT04J
 LSJ 20081124-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/_Pb29pBJ1kU/CY9xPesQBVIJ
 LSJ 20081202: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/GMxeDWiDXP8/twr__FgYvmMJ
 LSJ 20081202-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/hlK89M1M9rk/m/k2mbokPTCccJ
 LSJ 20081203: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/gaskAJqA-mE/m/GpuegB2W0IgJ
+LSJ 20081203-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/hlK89M1M9rk/m/qNtOFQfDK-oJ
 LSJ 20081210: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/pUUGH1nSKpc/aRxHUjHMxZsJ
 LSJ 20081213-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/MNmJu12AU8I/Pol1P9fWMmoJ
 LSJ 20081213-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/0Yf2s-qrWpM/0u8svYOAZ3cJ
+LSJ 20081213-3: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/cbZ2jl8-yGQ/m/OJljr9wcC4sJ
+LSJ 20090107: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/qPDLvbgqfCg/m/DlRVFoE_C64J
 LSJ 20090113-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/iZC_oiiXgTk/vKVo4bOt3MMJ
 LSJ 20090113-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/e48eViCqYSk/X7ZEE3k3MvEJ
 LSJ 20090113-3: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/8FHCL4AQblI/m/DejFKS9wmXUJ
 LSJ 20090114: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/fZIdIRDDxdo/dtdSNVk_IIkJ
 LSJ 20090115-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/RQ3ARP9Kvfk/dBN_M7SnIHAJ
 LSJ 20090115-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/rSaiVPMbpvY/ZYG3cYIdQZkJ
+LSJ 20090116: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/RQ3ARP9Kvfk/m/e-o1t79x1gUJ
 LSJ 20090126: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/3Cd-DNfT7yQ/m/-BfYOkP1OUUJ
 LSJ 20090205: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/l5bUtHOejmc/Ksw_nyldc3QJ
+LSJ 20090208: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/07gUFmSeIxU/m/yIrwcMsATB4J
+LSJ 20090213: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/hkTPcLPgZk4/m/WPZLiL2A91sJ
 LSJ 20090216: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/wU4YAwE6wlI/k24LcDxJEecJ
 LSJ 20090220: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/JMgZa9jdrc4/kdM4QIf5LE0J
+LSJ 20090226: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/f7pLAO9n--U/m/u6Q1HaHK2rUJ
 LSJ 20090304-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/B7EQiAVOr1Q/gg-GkqQBRp8J
 LSJ 20090304-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/PcbRGxbYQUY/eOqxJaT85dwJ
 LSJ 20090319: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/G1w6TeymEnQ/QS78VbaUmgIJ
 LSJ 20090322: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/tROpvfFdgBI/qDwA9JTPMxgJ
 LSJ 20090323: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/bG4PSmditm4/wR15DaRI8KUJ
+LSJ 20090324: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Zc_ogoVhsug/m/tJ2VBYI7resJ
 LSJ 20090325-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/5CW9tD5OfGk/nydaMm7gqNsJ
 LSJ 20090325-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/5CW9tD5OfGk/wzlh-bhnTQcJ
 LSJ 20090411: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/2aJf9bN7ZGc/YRt70QmwFLkJ
 LSJ 20090425: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/oL7Jflmkx48/RzAzPMSq1XcJ
+LSJ 20090428: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/BmA4xsXoEXc/m/rAIXsI8ycG4J
+LSJ 20090428-1: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/887DQTpntKI/m/hYSLzUDm5iUJ
 LSJ 20090430: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/2STzSnaSgxU/CVRMrvVPQmMJ
 LSJ 20090508: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/B7dz3qoIITQ/0YV5PNQvijsJ
 LSJ 20090514: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/PKQ6lQUBUOI/m/Zra43F1WXGcJ
 LSJ 20090528-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/63JZWOiuAIQ/qx6_7pyDQEsJ
 LSJ 20090528-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/LpFSLRuWONA/m0Alg1iD6gEJ
 LSJ 20090529: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/LpFSLRuWONA/daxDmJiGX0AJ
 LSJ 20090601: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/bKo8zb6lBeU/R6rVeXZN8DUJ
+LSJ 20090601-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/RkEUabeJNdM/m/JEGebBucNfEJ
 LSJ 20090603: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/LpFSLRuWONA/Ma_3LtLeyCAJ
 LSJ 20090606: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/-hy9E1u2t_o/CPU8rltzhesJ
 LSJ 20090616: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/6DEbXHjKGhE/1T4TclVRikoJ
 LSJ 20090617: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/OMTF0_ZqUL0/ijdnbYacuNkJ
 LSJ 20090617-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/ClO_zsSSgVU/m/TBaLfhQUN_8J
 LSJ 20090622: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/6B8fFRz2030/1wg9mm0HxvUJ
+LSJ 20090622-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/1zt1SZb2TIk/m/CYNhVovmlk8J
+LSJ 20090625: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/C3daj-vYqu4/m/2V2yTyLebHEJ
 LSJ 20090705: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/3Ekxk6uQ_wo/Y25g9tS6qSoJ
+LSJ 20090710: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/PBi3na64nkw/m/KOY1R8yWBsIJ
 LSJ 20090722: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/r-N65rA52uo/OXW8xk1r1iMJ
 LSJ 20090722-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Ry0xU4IuJmQ/6WqoTXkzrVUJ
 LSJ 20090724: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/1vJy-UKWR7Y/EOp-bsntrngJ
 LSJ 20090725: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/isG743Sws-8/cjTJkGtfl_gJ
 LSJ 20090731: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/y6f0s6tUtqs/H3dk4qr4nfkJ
+LSJ 20090810: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/g3ukXdsh8xo/m/0qTp2vtFVz8J
 LSJ 20090818: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/jkKBGVLmFHc/YXwYthjI7isJ
+LSJ 20090824: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/vWBysQ7L4fM/m/SA1wFRHusXAJ
 LSJ 20090826: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/KTwa1Hf_gHI/IlgyfFaqqeEJ
 LSJ 20090901: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/9BZPgQH9PFk/ulMGheX3NTIJ
 LSJ 20090920: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/mCPE3I6343Y/KqkCJgjur5IJ
+LSJ 20090920-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/nbgHtblc8jc/m/vdxPu5hPxGIJ
 LSJ 20090922: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/UdvGbJqOeo4/qFeNdWilXzUJ
 LSJ 20091015: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/pqa7mYZ6NEM/HhxAS7Rh3JwJ
 LSJ 20091016: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/pqa7mYZ6NEM/yvS8jE0ncrQJ
 LSJ 20091021: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/B_MVmqTcUXE/m/0-IIMaTSfq0J
+LSJ 20091021-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/x5oG5J7Egtg/m/yafJrZAoqjgJ
 LSJ 20091026: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/rPfGPwFH0_E/A8kRzU_POnoJ
 LSJ 20091030: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/ZKuCyTayYbc/m/5nMjLpX4DuMJ
 LSJ 20091113: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/8V-0-G9cMZA/6fOCEeru3bMJ
 LSJ 20091123: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Yt7LsvWFwiM/op6oRS8SLiYJ
 LSJ 20091123-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/_IwgQEvViWQ/m/1g36C5Y2BSoJ
+LSJ 20091124: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/8vjraZYKabg/m/IzhUlEDx1f0J
 LSJ 20091125: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/1dYtrdRjRI8/Iz5qzFYoboQJ
 LSJ 20091128: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/-IxzB0bvhKU/m/ogGuu7J80R4J
 LSJ 20091203: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/JBdmMh1udN8/5f5UX4qfOMMJ
 LSJ 20091204: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/JBdmMh1udN8/1bdYBRBxCAEJ
 LSJ 20091208: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/ptHbJM9MlVI/m/O61W2JkI_rIJ
 LSJ 20100112: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/SJu0kgw_2tE/p5cshF90vkEJ
+LSJ 20100129: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/X8Uu7Sk56P4/m/fgP7NfnDpCkJ
 LSJ 20100130: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/X8Uu7Sk56P4/twUvR4ZnBBkJ
 LJS 20100203: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/HQD-UNP7Y0s/cHxAnD8Z9dwJ
+LJS 20100203-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/tKnhKlDo8lk/m/6k8b2vok7_kJ
 LSJ 20100204: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/o5Xnzc8G774/yovVizGngKsJ
 LSJ 20100205: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/owQe9egif0U/84l6snr9RWIJ
+LSJ 20100205-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/tKb2e3940BI/m/2Uwzk6TJtJ8J
 LSJ 20100206: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/cAGrXqpO-YQ/m/GJHdeYt0GdUJ
 LSJ 20100206-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/reXyybyIYX8/m/jeCyjdiZ5T4J
 LSJ 20100207: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/wt2kuUJXoRI/m/LVO2J4dRxoIJ
+LSJ 20100207-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/VpXj3lre1BQ/m/Ou4J4lv8mSAJ
 LSJ 20100208: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/wt2kuUJXoRI/m/CyHXMb-Cn_0J
+LSJ 20100208-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/KX8dFqkrgjA/m/84tj0DROcmAJ
 LSJ 20100210: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/HHJfsSbIEf0/6UxQ3UJT9aEJ
 LSJ 20100210-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/wt2kuUJXoRI/m/XbHSJHMfk08J
+LSJ 20100211: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/pL63VXEPGME/m/gBjYSBLMwlYJ
+LSJ 20100211-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/pL63VXEPGME/m/n2dEkxwYyjcJ
 LSJ 20100212: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/NIIFHQg_x1c/e5cReQuEqxYJ
 LSJ 20100213: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/vXDkYrTmkws/sKy3jXz7AB4J
 LSJ 20100216: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/nrXTh1XKJJ8/KF7iiXQk3jsJ
+LSJ 20100218: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/x-uJChHi76Y/m/F92fWI7WwaEJ
 LSJ 20100221: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/TojSBPeGCFw/0FaCEfqRs3QJ
 LSJ 20100226: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/JnycCGrNQmY/CCqxwTVXpbEJ
 LSJ 20100228: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/yDeGOj1RBuU/k2CfIfBk770J
 LSJ 20100301: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/TcUDpHnvW8M/YznjkbV3JLoJ
 LSJ 20100302-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/jmmm0WRUPvs/ny5F1OnSUsEJ
 LSJ 20100302-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/b2cW6X-RQMs/RY2Zrzk6Ga0J
 LSJ 20100303: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/jmmm0WRUPvs/x9pv1OmWFS4J
 LSJ 20100304: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/UAllw82N9fw/Xl1zGn7t-3cJ
+LSJ 20100306: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Utho_j61pPQ/m/gcnXxAaIl6wJ
 LSJ 20100308: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/-euEN_y8ius/yrDIv--PZfsJ
 LSJ 20100310: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/hYN6L3COpqw/RPdTARngQLgJ
 LSJ 20100311: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Ogc7-acbMFs/cJsbFPUiReIJ
 LSJ 20100314: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/MeBSRw3OJC0/QZbO0FOx7roJ
 LSJ 20100324: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/PWhoejXDuuA/4E1wohx0oHwJ
+LSJ 20100325: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/PWhoejXDuuA/m/5565uQm2dpEJ
+LSJ 20100325-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/aC6OOfaulbM/m/svWv9UqH6isJ
 LSJ 20100402: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/BNPERBLJwRc/ynUIJFJ0EZcJ
 LSJ 20100422: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/tMEimr0yxLA/RWgvaOj6i9UJ
+LSJ 20100423: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/YnQCu0GeMhc/m/ET__SGvjD7QJ
 LSJ 20100426: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/BN3xmoZ0W1A/m/ui4w2OyGLjAJ
 LSJ 20100429: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/OUcf-1EMXXA/DOGZdKnJ1zgJ
 LSJ 20100506: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/H6Jm74N0v7k/zPi11g24bBUJ
 LSJ 20100507: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/vJQTPYtp-Eg/m/6_nkxd28-v8J
 LSJ 20100514: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Mz_fcIldfAY/m/Ys_W0MtwqLgJ
+LSJ 20100517: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/88K5Hd0NxlU/m/zaGQhDET3F0J
 LSJ 20100519: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/criytfhw97o/sj9_vGAi-xQJ
+LSJ 20100526: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/ch0oKrlxX30/m/MiuMxqszAUgJ
 LSJ 20100527: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Tr3X4DsZr-8/O06iXN6LtzsJ
 LSJ 20100601: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/R7YgwD0VlUQ/lhGLnME9m2IJ
 LSJ 20100604-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Tr3X4DsZr-8/DMXtyDoNqLIJ
 LSJ 20100604-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Tr3X4DsZr-8/fF0rs8s_YYEJ
 LSJ 20100611: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Tr3X4DsZr-8/6XTlnrJSM8EJ
+LSJ 20100705: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Dm_Zqyjdx8s/m/Fw-T7QAU8mkJ
 LSJ 20100708: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/7SxYC8-8654/VzSEX3LuKKEJ
+LSJ 20100716: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/HpOnoF-LrLU/m/MPw6hA_njd8J
 LSJ 20100721: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/Z9QNJ6SPIJM/m/g0uHQFp6G_QJ
 LSJ 20100723: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/0u5KQWiutdg/lAZoy4vIwiIJ
+LSJ 20100725: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/9d1zMZfsfNo/m/l3fbDtbr9xwJ
+LSJ 20100728: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/mzzPS-cOprI/m/BRBR4OBUOaQJ
 LSJ 20100811: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/kGKWcs3k6vI/Uwx7TGC8lgYJ
+LSJ 20100813: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/nOb3cmvA_3U/m/0UJqPZGujHsJ
 LSJ 20100819: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/x_u1Qtiguzg/m/FZjjjIQu-FoJ
+LSJ 20100823: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/cHdOwueG71I/m/BTBYvTZhrAUJ
 LSJ 20100827: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/cnJrGIiDqpw/KfaS7kEfk_8J
 LSJ 20100902: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/SM2_578Th0U/-GX0pSP_rCcJ
 LSJ 20100902-2: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/mFpx91METxM/m/ETLGtyQfvksJ
+LSJ 20100909: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/9Mn1QueD1I4/m/5hwidUeZH6EJ
 LSJ 20100915: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/lFLocuKV8NI/TcAPvYUfrWcJ
 LSJ 20101013: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/hpFRDAmtSbA/m/httYmI5wpB8J
 LSJ 20101210: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/QTAA0y6cANI/m/gU0hztzp8mUJ
-LSJ 20110308: https://www.boardgamegeek.com/thread/628087/article/6401929
-LSJ 20110419: https://www.boardgamegeek.com/thread/643948/article/6634732
+LSJ 20010121: https://boardgamegeek.com/thread/609699/article/6142361#6142361
+LSJ 20110308: https://boardgamegeek.com/thread/628087/article/6401929
+LSJ 20110419: https://boardgamegeek.com/thread/643948/article/6634732
 LSJ 20110502: https://boardgamegeek.com/thread/648695/article/6701545
 LSJ 20110611: https://boardgamegeek.com/thread/662413/article/6920306
 PIB 20110712-1: http://www.vekn.net/forum/rules-questions/6182-counters-question#6188
 PIB 20110712-2: http://www.vekn.net/forum/rules-questions/6199-shilmulo-question#6200
 PIB 20110718: http://www.vekn.net/forum/rules-questions/6435-learjet-question#6436
 PIB 20110719: http://www.vekn.net/forum/rules-questions/6445-charming-loby-q#6450
 PIB 20110725: http://www.vekn.net/forum/rules-questions/6728-announcing-siphon#6740
@@ -824,36 +1083,46 @@
 PIB 20110818: http://www.vekn.net/forum/rules-questions/8475-q-question-about-abbysal-hunter#8477
 PIB 20110830: http://www.vekn.net/forum/rules-questions/9340-first-strike--strength-reduction#9345
 PIB 20110915-1: http://www.vekn.net/forum/rules-questions/10264-lubomira-hradok-clarification#10266
 PIB 20110915-2: http://www.vekn.net/forum/rules-questions/10248-summoning#10250
 PIB 20110918: http://www.vekn.net/forum/rules-questions/10458-frondator#10459
 PIB 20111017: http://www.vekn.net/forum/rules-questions/12104-archon-in-3-pool-and-carrion-crows-vs-nephandus#12110
 PIB 20111002: http://www.vekn.net/forum/rules-questions/8235-re-coven-timing?start=18#11317
+PIB 20111101: https://www.vekn.net/forum/rules-questions/12975-summon-history-reanimated-corpse#13169
+PIB 20111105: https://www.vekn.net/forum/rules-questions/13042-blissful-agony-vs-allies?start=6#13409
 PIB 20111202: http://www.vekn.net/forum/rules-questions/16788-new-psyche-and-telepathic-tracking#16794
 PIB 20111208: http://www.vekn.net/forum/rules-questions/16769-rules-team-rulings-02-dec-11?limit=10&start=40#17547
 PIB 20120204: http://www.vekn.net/index.php/forum/6-rules-questions/22233-strained-vitae-supply-vs-lokis-gift#22343
 PIB 20120214: http://www.vekn.net/forum/rules-questions/22906-re-set-the-range?start=12#22999
+PIB 20120225: https://www.vekn.net/forum/rules-questions/24105-blissful-agony-vs-blissful-agony#24106
+PIB 20120426: https://www.vekn.net/forum/rules-questions/27863-disarm-vs-combat-ends?start=6#28739
 PIB 20120525: http://www.vekn.net/forum/rules-questions/31158-trochomancy-bounce#31163
 PIB 20120808: http://www.vekn.net/forum/rules-questions/34265-rules-tweak-suggestion-rewind-time-et-al?start=12#34448
 PIB 20121013: http://www.vekn.net/forum/rules-questions/39040-ex-nihilo-can-i-choose-to-burn-my-minion#39041
 PIB 20121028: http://www.vekn.net/forum/rules-questions/39816-ec-2012-can-you-answer-these?start=6#39843
 PIB 20121031: http://www.vekn.net/forum/rules-questions/39816-ec-2012-can-you-answer-these?start=18#39908
 PIB 20121107: http://www.vekn.net/forum/rules-questions/40504-familial-bond#40540
+PIB 20121112: https://www.vekn.net/forum/rules-questions/40755-kyoko-s-hunt-action#40831
 PIB 20121210: http://www.vekn.net/forum/rules-questions/42498-does-eurayle-s-special-cost-her-blood-while-targeting-hazimel?start=18#42659
 PIB 20121220: http://www.vekn.net/forum/rules-questions/43188-storage-annex-changes-control?start=6#43199
 PIB 20130119: http://www.vekn.net/forum/rules-questions/44197-ashur-tablets-for-zero#44229
 PIB 20130128: http://www.vekn.net/forum/rules-questions/43572-can-i-put-infernal-pact-on-vidal-jarbeaux?start=36#44503
 PIB 20130128-2: http://www.vekn.net/forum/rules-questions/44232-khazar-s-diary-question#44504
 PIB 20130221: https://www.vekn.net/forum/rules-questions/45439-gurchon-hall#45443
+PIB 20130303: https://www.vekn.net/forum/rules-questions/45620-rock-cat-vs-torn-signpost#45626
+PIB 20130311: https://www.vekn.net/forum/rules-questions/46009-dive-into-madness#46013
 PIB 20130319: http://www.vekn.net/forum/rules-questions/46164-catatonic-fear-and-loving-agony#46168
+PIB 20130327: https://www.vekn.net/forum/rules-questions/46279-soak-vs-treat-agg-damage-as-normal-damage#46285
 PIB 20130415: http://www.vekn.net/forum/rules-questions/46989-sword-of-nuln-taste-of-vitae#46991
+PIB 20130704: https://www.vekn.net/forum/rules-questions/50982-iron-heart-vs-virtuosa#50984
 PIB 20130711: http://www.vekn.net/forum/rules-questions/51279-big-boon-bounce?fbclid=IwAR3-kLQKFt415mAPpGL0sYpi4yx6ZzJbiyP57z3R6nkIW7V-g0F93z_ob-s#51307
 PIB 20130722: http://www.vekn.net/forum/rules-questions/52017-legacy-of-pander#52019
 PIB 20131013: http://www.vekn.net/forum/rules-questions/55220-mimir-and-archon-investigation?start=0#55238
 PIB 20140107: https://www.vekn.net/forum/rules-questions/58277-sensory-deprivation-and-banishment#58286
+PIB 20140122: https://www.vekn.net/forum/rules-questions/58586-banishment-and-master-discipline#58772
 PIB 20140324: https://www.vekn.net/forum/rules-questions/60259-carrion-crows-first-strike-strikes-not-anaesthetic-touch?start=0#60260
 PIB 20141006: http://www.vekn.net/forum/rules-questions/66061-houngan-on-lisandro#66084
 PIB 20141026: http://www.vekn.net/forum/rules-questions/66960-gianna-di-canneto#66971
 PIB 20141210: http://www.vekn.net/forum/rules-questions/67940-smallpox-griet-and-additional-strikes#68077
 PIB 20141226: http://www.vekn.net/forum/6-rules-questions/66453-double-velvet-tongue-qcannot-cast-votes-or-ballotsq?limit=10&start=20#66964
 PIB 20150105: http://www.vekn.net/forum/rules-questions/68465-voting-is-complicated#68493
 PIB 20150105-2: http://www.vekn.net/forum/rules-questions/68482-topaz-successfully-equips-baby-yaga-successfully-employs#68483
@@ -892,20 +1161,24 @@
 PIB 20150917: http://www.vekn.net/forum/rules-questions/73156-corner-case-thin-blooded-seer-question#73166
 PIB 20150924-1: http://www.vekn.net/forum/rules-questions/73292-toreador-grand-ball-mask-of-1000-faces#73306
 PIB 20150924-2: http://www.vekn.net/forum/rules-questions/73293-adana-de-sforza-combo-cards#73307
 PIB 20150930: http://www.vekn.net/forum/rules-questions/73292-toreador-grand-ball-mask-of-1000-faces?start=18#73448
 PIB 20151009: http://www.vekn.net/forum/rules-questions/73577-baleful-doll#73580
 PIB 20151101: http://www.vekn.net/forum/rules-questions/73992-imbued-and-blood-costs-general-mechanics#73995
 PIB 20151116: http://www.vekn.net/forum/rules-questions/74317-the-not-anarch-barons#74327
-RBK 20181001-4: http://www.vekn.net/rulebook/4-unlock-phase
-RBK 20181001-10: http://www.vekn.net/rulebook/10-vampire-sects
-RBK 20181001-11: http://www.vekn.net/rulebook/11-special-terms
-RBK 20181001-162: http://www.vekn.net/rulebook#1.6.2.mastercards
-RBK 20181001-163: http://www.vekn.net/rulebook#1.6.3.minioncards
-RBK 20181001-645: http://www.vekn.net/rulebook#6.4.5.strikeeffects
+RBK 20200701-1: https://www.vekn.net/rulebook#unlock-phase
+RBK 20200701-2: https://www.vekn.net/rulebook#sequencing
+RBK 20200701-3: https://www.vekn.net/rulebook/6-vampire-sects
+RBK 20200701-4: https://www.vekn.net/rulebook#wording-templates
+RBK 20200701-5: https://www.vekn.net/rulebook#trifle
+RBK 20200701-6: https://www.vekn.net/rulebook#allies
+RBK 20200701-7: https://www.vekn.net/rulebook#steal-equipment
+RBK 20200701-8: https://www.vekn.net/rulebook#gaining-votes
+RBK 20200701-9: https://www.vekn.net/rulebook#who-may-attempt-to-block
+RBK 20200701-10: https://www.vekn.net/rulebook#resolve-strike
 RTR 19941006: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/HUipqz0LFSw/pY6uEa3f8-gJ
 RTR 19941101: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/HUipqz0LFSw/pY6uEa3f8-gJ
 RTR 19941109: https://groups.google.com/d/msg/rec.games.deckmaster/_6CXoKTSLnw/FdG67-3HEAQJ
 RTR 19941128: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/HUipqz0LFSw/pY6uEa3f8-gJ
 RTR 19941222: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/19Ys4rdQPQw/bijoNa8Z8FsJ
 RTR 19950413: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/zB2vyPBnO6g/i1myM9tD54AJ
 RTR 19950509: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/_LKyR7pdMig/ZvwdGmIwUnsJ
@@ -947,14 +1220,15 @@
 RTR 20071204: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/uqlirlrTXis/m/Aq0HEAV-AugJ
 RTR 20080808: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/1jW6GXrIRSU/8QTYL98kB0gJ
 RTR 20111202: http://www.vekn.net/forum/rules-questions/16769-rules-team-rulings-02-dec-11#16769
 RTR 20130422: http://www.vekn.net/forum/rules-questions/47377-rules-team-rulings-22-apr-2013#47377
 RTR 20160119: http://www.vekn.net/forum/news-and-announcements/74630-anarchs-unbound-released#74945
 RTR 20180303: http://www.vekn.net/forum/rules-questions/76447-rules-team-rulings-rtr-03-03-2018#85536
 RTR 20180511: http://www.vekn.net/forum/rules-questions/76595-rules-team-rulings-rtr-11-05-2018#86780
+RTR 20180511-2: https://www.vekn.net/forum/rules-questions/76595-rules-team-rulings-rtr-11-05-2018?start=30#86840
 RTR 20180719: https://www.blackchantry.com/2018/07/18/rules-team-rulings-rtr-19-07-2018/
 RTR 20200705: https://www.blackchantry.com/2020/07/05/about-diversity-and-inclusivity-including-vekn-rules-team-rulings-05-07-2020/
 RTR 20201130: https://www.blackchantry.com/2020/12/25/rtr-30-11-2020/
 SFC 19960819: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/G40EE8vCBB8/Bj3qpDZ_VLkJ
 SFC 19960919: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/_UxVq0Lrg2U/xlsK8NogrW4J
 TOM 19950304: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/DYxpGPWoSaE/05x_CdfRdLgJ
 TOM 19950407: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/FWVnIu3zLAQ/ODGlyMGc_hgJ
@@ -980,14 +1254,15 @@
 TOM 19951216: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/0G-jqB_fcyE/8jUhfCXRtPUJ
 TOM 19951217: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Y2_A66iRqMc/LkT-8j5cz2cJ
 TOM 19960109: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/gB3xexVAV0s/zGnkjIMjyJsJ
 TOM 19960114: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/cOqrGO0UrSw/5pDhn3YVyG4J
 TOM 19960122: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/d3n3StNS7no/Wwj5SYMQPskJ
 TOM 19960130: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/wF82VdVPlm0/MmFo2E7lrY8J
 TOM 19960210: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/PiOmH08RyVw/CqzTRcOLDNIJ
+TOM 19960211: https://groups.google.com/g/rec.games.trading-cards.jyhad/c/PiOmH08RyVw/m/9jI1_ASoupIJ
 TOM 19960214: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/AP9ub18aVjg/5zCfEMIz3ZEJ
 TOM 19960225: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/0LLTOfvyVbM/ih72_C-LriwJ
 TOM 19960226-1: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/16y-ZD7Xats/oMeZDnSFdYAJ
 TOM 19960226-2: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/SEU6ztVpR94/Qfct6YcvnQwJ
 TOM 19960303: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/SEU6ztVpR94/F8NmjGw8ml8J
 TOM 19960326: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/8DA9p_p5v8s/lJlHFYXPTBYJ
 TOM 19960413: https://groups.google.com/d/msg/rec.games.trading-cards.jyhad/Gm-NLCP6bF0/sVxss5F1bBYJ
```

### Comparing `krcg-2.9/setup.cfg` & `krcg-3.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 [metadata]
 name = krcg
-version = 2.9
+version = 3.0
 author = lionelpx
 author_email = lionel.panhaleux@gmail.com
 url = http://github.com/lionel-panhaleux/krcg
-description = "CLI, web API and Discord bot for VTES cards and TWDA.",
+description = CLI, web API and Discord bot for VTES cards and TWDA.
 long_description = file: README.md
 long_description_content_type = text/markdown
-license = "MIT"
+license = MIT
 keywords = vampire vtes vekn wod ccg twd
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
+	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Games/Entertainment
 
 [options]
+python_requires = >=3.8
 zip_safe = True
 include_package_data = True
 packages = find:
 setup_requires = 
 	setuptools
 install_requires = 
 	arrow
 	pyyaml
+	numpy
 	requests
 	setuptools
 	unidecode
 
 [options.extras_require]
 dev = 
 	certifi
 	coverage
 	codacy-coverage
 	black
-	doc8
 	flake8
 	ipython
 	pytest
 	zest.releaser[recommended]
 
 [options.packages.find]
 exclude =
```

### Comparing `krcg-2.9/twda_fix/2010hunrb.html` & `krcg-3.0/twda_fix/2010hunrb.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2010pwbla1.html` & `krcg-3.0/twda_fix/2010pwbla1.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2010pwblaQ.html` & `krcg-3.0/twda_fix/2010pwblaQ.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k2during.html` & `krcg-3.0/twda_fix/2k2during.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k2eclastq.html` & `krcg-3.0/twda_fix/2k2eclastq.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k2gothenburg.html` & `krcg-3.0/twda_fix/2k2gothenburg.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k2gothenburgapr.html` & `krcg-3.0/twda_fix/2k2gothenburgapr.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k2newyork.html` & `krcg-3.0/twda_fix/2k2newyork.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k2orccon2.html` & `krcg-3.0/twda_fix/2k2orccon2.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k2pariseq.html` & `krcg-3.0/twda_fix/2k2pariseq.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k2sydney.html` & `krcg-3.0/twda_fix/2k2sydney.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k2torrancejan.html` & `krcg-3.0/twda_fix/2k2torrancejan.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k2ukqualifier.html` & `krcg-3.0/twda_fix/2k2ukqualifier.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k2watfordapr.html` & `krcg-3.0/twda_fix/2k2watfordapr.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k2watfordmay.html` & `krcg-3.0/twda_fix/2k2watfordmay.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k3cadaverous.html` & `krcg-3.0/twda_fix/2k3cadaverous.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k3ec.html` & `krcg-3.0/twda_fix/2k3ec.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k3frenchecq.html` & `krcg-3.0/twda_fix/2k3frenchecq.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k3gothenburgblizzard.html` & `krcg-3.0/twda_fix/2k3gothenburgblizzard.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k3helsinki5.html` & `krcg-3.0/twda_fix/2k3helsinki5.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k3italyqualifier.html` & `krcg-3.0/twda_fix/2k3italyqualifier.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k3psmilwaukee.html` & `krcg-3.0/twda_fix/2k3psmilwaukee.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k3rome.html` & `krcg-3.0/twda_fix/2k3rome.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k3sdgothenburg.html` & `krcg-3.0/twda_fix/2k3sdgothenburg.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k3tcithaca.html` & `krcg-3.0/twda_fix/2k3tcithaca.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k3winnipegapril.html` & `krcg-3.0/twda_fix/2k3winnipegapril.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k4gks.html` & `krcg-3.0/twda_fix/2k4gks.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k4littlesister.html` & `krcg-3.0/twda_fix/2k4littlesister.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k4norms.html` & `krcg-3.0/twda_fix/2k4norms.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k4volkerpit.html` & `krcg-3.0/twda_fix/2k4volkerpit.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k5blackutrecht.html` & `krcg-3.0/twda_fix/2k5blackutrecht.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k5dcqualifier.html` & `krcg-3.0/twda_fix/2k5dcqualifier.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k5dreamboston.html` & `krcg-3.0/twda_fix/2k5dreamboston.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k5leicesteraug.html` & `krcg-3.0/twda_fix/2k5leicesteraug.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k5ropecon.html` & `krcg-3.0/twda_fix/2k5ropecon.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k5valhallajuly.html` & `krcg-3.0/twda_fix/2k5valhallajuly.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k6aussiechamp.html` & `krcg-3.0/twda_fix/2k6aussiechamp.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k6faceaface.html` & `krcg-3.0/twda_fix/2k6faceaface.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k6nerq-templecon.html` & `krcg-3.0/twda_fix/2k6nerq-templecon.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k6praxispoitiers.html` & `krcg-3.0/twda_fix/2k6praxispoitiers.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k6sonarba.html` & `krcg-3.0/twda_fix/2k6sonarba.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k7campeonatojuizforano.html` & `krcg-3.0/twda_fix/2k7campeonatojuizforano.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k7comjust.html` & `krcg-3.0/twda_fix/2k7comjust.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k7palmaqual.html` & `krcg-3.0/twda_fix/2k7palmaqual.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k7woaboston.html` & `krcg-3.0/twda_fix/2k7woaboston.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k8sequeenslandcq.html` & `krcg-3.0/twda_fix/2k8sequeenslandcq.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k8torunminiq.html` & `krcg-3.0/twda_fix/2k8torunminiq.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/2k9mojlp.html` & `krcg-3.0/twda_fix/2k9mojlp.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/Brian.html` & `krcg-3.0/twda_fix/Brian.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/ckgc2k.html` & `krcg-3.0/twda_fix/ckgc2k.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/crusadelisbon2k1.html` & `krcg-3.0/twda_fix/crusadelisbon2k1.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/dallas.html` & `krcg-3.0/twda_fix/dallas.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/damnans.html` & `krcg-3.0/twda_fix/damnans.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/darbyla2k1.html` & `krcg-3.0/twda_fix/darbyla2k1.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/gothenburg2k1.html` & `krcg-3.0/twda_fix/gothenburg2k1.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/joshphiladelphia.html` & `krcg-3.0/twda_fix/joshphiladelphia.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/leedec99.html` & `krcg-3.0/twda_fix/leedec99.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/lurequebec2k1.html` & `krcg-3.0/twda_fix/lurequebec2k1.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/matt-alamut.html` & `krcg-3.0/twda_fix/matt-alamut.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/palma2k1.html` & `krcg-3.0/twda_fix/palma2k1.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/portoct99.html` & `krcg-3.0/twda_fix/portoct99.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/quebec.html` & `krcg-3.0/twda_fix/quebec.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/rob.html` & `krcg-3.0/twda_fix/rob.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/swkc.html` & `krcg-3.0/twda_fix/swkc.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/theobell2k1.html` & `krcg-3.0/twda_fix/theobell2k1.html`

 * *Files identical despite different names*

### Comparing `krcg-2.9/twda_fix/watford-ts.html` & `krcg-3.0/twda_fix/watford-ts.html`

 * *Files identical despite different names*

