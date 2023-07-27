# Comparing `tmp/noether-1.0.0.tar.gz` & `tmp/noether-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noether-1.0.0.tar", last modified: Sun Jul 23 17:13:55 2023, max compression
+gzip compressed data, was "noether-1.0.1.tar", last modified: Thu Jul 27 10:52:32 2023, max compression
```

## Comparing `noether-1.0.0.tar` & `noether-1.0.1.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-23 17:13:55.263338 noether-1.0.0/
--rw-r--r--   0 yunruse    (501) staff       (20)     1064 2023-07-23 11:11:28.000000 noether-1.0.0/LICENSE.txt
--rw-r--r--   0 yunruse    (501) staff       (20)     3473 2023-07-23 17:13:55.262670 noether-1.0.0/PKG-INFO
--rw-r--r--   0 yunruse    (501) staff       (20)     2899 2023-07-23 17:11:56.000000 noether-1.0.0/README.md
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-23 17:13:55.179701 noether-1.0.0/noether/
--rw-r--r--   0 yunruse    (501) staff       (20)     3760 2023-07-23 11:11:28.000000 noether-1.0.0/noether/Multiplication.py
--rw-r--r--   0 yunruse    (501) staff       (20)      119 2023-07-23 11:11:28.000000 noether-1.0.0/noether/__init__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2164 2023-07-23 11:11:28.000000 noether-1.0.0/noether/__main__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1430 2023-07-23 11:11:28.000000 noether-1.0.0/noether/_tokenizers.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-23 17:13:55.191361 noether-1.0.0/noether/catalogue/
--rw-r--r--   0 yunruse    (501) staff       (20)     1140 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/__init__.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-23 17:13:55.196982 noether-1.0.0/noether/catalogue/conventional/
--rw-r--r--   0 yunruse    (501) staff       (20)      145 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/conventional/__init__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2872 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/conventional/conventional.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2425 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/conventional/imperial.py
--rw-r--r--   0 yunruse    (501) staff       (20)      634 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/conventional/typographic.py
--rw-r--r--   0 yunruse    (501) staff       (20)     5950 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/dimensions.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1048 2023-07-23 16:18:14.000000 noether-1.0.0/noether/catalogue/fundamental.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-23 17:13:55.206439 noether-1.0.0/noether/catalogue/historic/
--rw-r--r--   0 yunruse    (501) staff       (20)      110 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/historic/__init__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2485 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/historic/ancient_greek.units.py
--rw-r--r--   0 yunruse    (501) staff       (20)     4233 2023-07-23 17:13:44.000000 noether-1.0.0/noether/catalogue/historic/ancient_greek_.py
--rw-r--r--   0 yunruse    (501) staff       (20)      567 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/historic/mts.units.py
--rw-r--r--   0 yunruse    (501) staff       (20)      792 2023-07-23 17:13:44.000000 noether-1.0.0/noether/catalogue/historic/mts_.py
--rw-r--r--   0 yunruse    (501) staff       (20)      456 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/historic/scientific.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-23 17:13:55.212544 noether-1.0.0/noether/catalogue/humorous/
--rw-r--r--   0 yunruse    (501) staff       (20)       73 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/humorous/__init__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2377 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/humorous/fictional.py
--rw-r--r--   0 yunruse    (501) staff       (20)      820 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/humorous/potrzebie.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1080 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/humorous/unusual.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-23 17:13:55.222058 noether-1.0.0/noether/catalogue/info/
--rw-r--r--   0 yunruse    (501) staff       (20)       97 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/info/__init__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2610 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/info/comparison.py
--rw-r--r--   0 yunruse    (501) staff       (20)      282 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/info/dimension.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2152 2023-07-23 16:35:16.000000 noether-1.0.0/noether/catalogue/info/spectrum.py
--rw-r--r--   0 yunruse    (501) staff       (20)      355 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/info/unit_context.py
--rw-r--r--   0 yunruse    (501) staff       (20)      476 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/info/unit_value.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2304 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/prefixes.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-23 17:13:55.238716 noether-1.0.0/noether/catalogue/scientific/
--rw-r--r--   0 yunruse    (501) staff       (20)     2804 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/scientific/CODATA.py
--rw-r--r--   0 yunruse    (501) staff       (20)      216 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/scientific/__init__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1354 2023-07-23 16:12:45.000000 noether-1.0.0/noether/catalogue/scientific/astronomy.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1640 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/scientific/cgs.py
--rw-r--r--   0 yunruse    (501) staff       (20)      290 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/scientific/climate.py
--rw-r--r--   0 yunruse    (501) staff       (20)      752 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/scientific/constants.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1803 2023-07-23 16:20:54.000000 noether-1.0.0/noether/catalogue/scientific/data.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2411 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/scientific/essential.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2797 2023-07-23 11:11:28.000000 noether-1.0.0/noether/catalogue/scientific/si.py
--rw-r--r--   0 yunruse    (501) staff       (20)     4883 2023-07-23 11:11:28.000000 noether-1.0.0/noether/config.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-23 17:13:55.254302 noether-1.0.0/noether/core/
--rw-r--r--   0 yunruse    (501) staff       (20)     3934 2023-07-23 11:11:28.000000 noether-1.0.0/noether/core/Catalogue.py
--rw-r--r--   0 yunruse    (501) staff       (20)     3940 2023-07-23 16:32:04.000000 noether-1.0.0/noether/core/Dimension.py
--rw-r--r--   0 yunruse    (501) staff       (20)    12450 2023-07-23 16:31:59.000000 noether-1.0.0/noether/core/Measure.py
--rw-r--r--   0 yunruse    (501) staff       (20)      471 2023-07-23 11:11:28.000000 noether-1.0.0/noether/core/MeasureInfo.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1293 2023-07-23 11:11:28.000000 noether-1.0.0/noether/core/MeasureRelative.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1652 2023-07-23 11:11:28.000000 noether-1.0.0/noether/core/Prefix.py
--rw-r--r--   0 yunruse    (501) staff       (20)     4752 2023-07-23 16:37:02.000000 noether-1.0.0/noether/core/Unit.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1179 2023-07-23 11:11:28.000000 noether-1.0.0/noether/core/UnitSet.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1898 2023-07-23 11:11:28.000000 noether-1.0.0/noether/core/_DisplayHandler.py
--rw-r--r--   0 yunruse    (501) staff       (20)      271 2023-07-23 11:11:28.000000 noether-1.0.0/noether/core/__init__.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-23 17:13:55.261368 noether-1.0.0/noether/core/units/
--rw-r--r--   0 yunruse    (501) staff       (20)     1257 2023-07-23 11:11:28.000000 noether-1.0.0/noether/core/units/AffineUnit.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1524 2023-07-23 11:11:28.000000 noether-1.0.0/noether/core/units/GeometricUnit.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2002 2023-07-23 16:31:44.000000 noether-1.0.0/noether/core/units/LinearUnit.py
--rw-r--r--   0 yunruse    (501) staff       (20)      516 2023-07-23 11:11:28.000000 noether-1.0.0/noether/core/units/PrefixedUnit.py
--rw-r--r--   0 yunruse    (501) staff       (20)      180 2023-07-23 11:11:28.000000 noether-1.0.0/noether/core/units/__init__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2020 2023-07-23 16:40:01.000000 noether-1.0.0/noether/display.py
--rw-r--r--   0 yunruse    (501) staff       (20)      974 2023-07-23 11:11:28.000000 noether-1.0.0/noether/errors.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1576 2023-07-23 11:11:28.000000 noether-1.0.0/noether/helpers.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-23 17:13:55.185640 noether-1.0.0/noether.egg-info/
--rw-r--r--   0 yunruse    (501) staff       (20)     3473 2023-07-23 17:13:55.000000 noether-1.0.0/noether.egg-info/PKG-INFO
--rw-r--r--   0 yunruse    (501) staff       (20)     2045 2023-07-23 17:13:55.000000 noether-1.0.0/noether.egg-info/SOURCES.txt
--rw-r--r--   0 yunruse    (501) staff       (20)        1 2023-07-23 17:13:55.000000 noether-1.0.0/noether.egg-info/dependency_links.txt
--rw-r--r--   0 yunruse    (501) staff       (20)        8 2023-07-23 17:13:55.000000 noether-1.0.0/noether.egg-info/top_level.txt
--rw-r--r--   0 yunruse    (501) staff       (20)      301 2023-07-23 11:11:28.000000 noether-1.0.0/pyproject.toml
--rw-r--r--   0 yunruse    (501) staff       (20)       38 2023-07-23 17:13:55.263541 noether-1.0.0/setup.cfg
--rw-r--r--   0 yunruse    (501) staff       (20)      807 2023-07-23 17:09:31.000000 noether-1.0.0/setup.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.878870 noether-1.0.1/
+-rw-r--r--   0 yunruse    (501) staff       (20)     1064 2023-07-23 17:43:49.000000 noether-1.0.1/LICENSE.txt
+-rw-r--r--   0 yunruse    (501) staff       (20)     3635 2023-07-27 10:52:32.878051 noether-1.0.1/PKG-INFO
+-rw-r--r--   0 yunruse    (501) staff       (20)     3061 2023-07-23 18:03:30.000000 noether-1.0.1/README.md
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.811092 noether-1.0.1/noether/
+-rw-r--r--   0 yunruse    (501) staff       (20)     3958 2023-07-27 10:51:03.000000 noether-1.0.1/noether/Multiplication.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      119 2023-07-23 17:43:49.000000 noether-1.0.1/noether/__init__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2164 2023-07-23 17:43:49.000000 noether-1.0.1/noether/__main__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1430 2023-07-27 10:21:44.000000 noether-1.0.1/noether/_tokenizers.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.820063 noether-1.0.1/noether/catalogue/
+-rw-r--r--   0 yunruse    (501) staff       (20)     1140 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/__init__.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.825851 noether-1.0.1/noether/catalogue/conventional/
+-rw-r--r--   0 yunruse    (501) staff       (20)      145 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/conventional/__init__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     3138 2023-07-27 10:21:27.000000 noether-1.0.1/noether/catalogue/conventional/conventional.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2524 2023-07-26 11:03:04.000000 noether-1.0.1/noether/catalogue/conventional/imperial.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      634 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/conventional/typographic.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     5950 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/dimensions.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1048 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/fundamental.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.833232 noether-1.0.1/noether/catalogue/historic/
+-rw-r--r--   0 yunruse    (501) staff       (20)      110 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/historic/__init__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2485 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/historic/ancient_greek.units.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     4233 2023-07-27 10:49:00.000000 noether-1.0.1/noether/catalogue/historic/ancient_greek_.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      567 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/historic/mts.units.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      792 2023-07-27 10:49:00.000000 noether-1.0.1/noether/catalogue/historic/mts_.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      456 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/historic/scientific.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.837338 noether-1.0.1/noether/catalogue/humorous/
+-rw-r--r--   0 yunruse    (501) staff       (20)       73 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/humorous/__init__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2377 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/humorous/fictional.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      820 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/humorous/potrzebie.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1080 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/humorous/unusual.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.844539 noether-1.0.1/noether/catalogue/info/
+-rw-r--r--   0 yunruse    (501) staff       (20)       97 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/info/__init__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2610 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/info/comparison.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      282 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/info/dimension.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2152 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/info/spectrum.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      355 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/info/unit_context.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      476 2023-07-26 10:15:46.000000 noether-1.0.1/noether/catalogue/info/unit_value.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2304 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/prefixes.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.858234 noether-1.0.1/noether/catalogue/scientific/
+-rw-r--r--   0 yunruse    (501) staff       (20)     2804 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/CODATA.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      216 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/__init__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1354 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/astronomy.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1640 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/cgs.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      290 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/climate.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      752 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/constants.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1803 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/data.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2411 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/essential.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2796 2023-07-26 10:54:35.000000 noether-1.0.1/noether/catalogue/scientific/si.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     4883 2023-07-24 12:28:18.000000 noether-1.0.1/noether/config.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.871126 noether-1.0.1/noether/core/
+-rw-r--r--   0 yunruse    (501) staff       (20)     4088 2023-07-27 10:51:03.000000 noether-1.0.1/noether/core/Catalogue.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     4395 2023-07-26 12:23:58.000000 noether-1.0.1/noether/core/Dimension.py
+-rw-r--r--   0 yunruse    (501) staff       (20)    10693 2023-07-26 10:13:13.000000 noether-1.0.1/noether/core/Measure.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      471 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/MeasureInfo.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1293 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/MeasureRelative.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1652 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/Prefix.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     5098 2023-07-26 10:13:13.000000 noether-1.0.1/noether/core/Unit.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1179 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/UnitSet.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2462 2023-07-26 10:13:13.000000 noether-1.0.1/noether/core/_DisplayHandler.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      271 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/__init__.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.877009 noether-1.0.1/noether/core/units/
+-rw-r--r--   0 yunruse    (501) staff       (20)     1257 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/units/AffineUnit.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1813 2023-07-26 12:27:47.000000 noether-1.0.1/noether/core/units/GeometricUnit.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2345 2023-07-24 12:28:18.000000 noether-1.0.1/noether/core/units/LinearUnit.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      516 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/units/PrefixedUnit.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      180 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/units/__init__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     3296 2023-07-26 13:08:12.000000 noether-1.0.1/noether/display.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      974 2023-07-23 17:43:49.000000 noether-1.0.1/noether/errors.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2076 2023-07-27 10:51:03.000000 noether-1.0.1/noether/gnu.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1576 2023-07-23 17:43:49.000000 noether-1.0.1/noether/helpers.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.814603 noether-1.0.1/noether.egg-info/
+-rw-r--r--   0 yunruse    (501) staff       (20)     3635 2023-07-27 10:52:32.000000 noether-1.0.1/noether.egg-info/PKG-INFO
+-rw-r--r--   0 yunruse    (501) staff       (20)     2060 2023-07-27 10:52:32.000000 noether-1.0.1/noether.egg-info/SOURCES.txt
+-rw-r--r--   0 yunruse    (501) staff       (20)        1 2023-07-27 10:52:32.000000 noether-1.0.1/noether.egg-info/dependency_links.txt
+-rw-r--r--   0 yunruse    (501) staff       (20)        8 2023-07-27 10:52:32.000000 noether-1.0.1/noether.egg-info/top_level.txt
+-rw-r--r--   0 yunruse    (501) staff       (20)      301 2023-07-23 17:43:49.000000 noether-1.0.1/pyproject.toml
+-rw-r--r--   0 yunruse    (501) staff       (20)       38 2023-07-27 10:52:32.879052 noether-1.0.1/setup.cfg
+-rw-r--r--   0 yunruse    (501) staff       (20)      807 2023-07-23 18:03:30.000000 noether-1.0.1/setup.py
```

### Comparing `noether-1.0.0/LICENSE.txt` & `noether-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/PKG-INFO` & `noether-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: noether
-Version: 1.0.0
+Version: 1.0.1
 Summary: Work with physical measurements and constants
 Home-page: https://github.com/yunruse/noether
 Author: Mia yun Ruse
 Author-email: mia@yunru.se
 Keywords: physics unit measure constant measurement uncertainty
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved
 Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Noether 1.0
+# Noether 1.0.1 (in development)
 
 [![PyPI](https://img.shields.io/pypi/v/noether?color=blue)](https://pypi.org/packages/noether)
 
 **Noether** is a unit-enriched Python package, akin to Wolfram Alpha or gnu `units`. It has a large (and expanding) catalogue of up-to-date units and constants, allowing code to be written directly in the units they are concerned with while also ensuring e.g. you don't mistakenly add an energy to a length.
 
 Just grab Python 3.10 or later and `pip install noether` to run!
 
@@ -86,17 +86,20 @@
 ```
 
 Use `conf.save()` to save to (by default) `~/.config/noether.toml`.
 
 
 ## For more, see...
 
-Check out [CONTRIBUTING.md](CONTRIBUTING.md) and [LICENSE.txt](LICENSE.txt) for info of that sort.
+- [CHANGELOG.md](https://github.com/yunruse/Noether/blob/release/CHANGELOG.md)
+- [CONTRIBUTING.md](https://github.com/yunruse/Noether/blob/release/CONTRIBUTING.md)
+- [LICENSE.txt](https://github.com/yunruse/Noether/blob/release/LICENSE.txt)
 
 Other tools for working with units include:
+
 - [Wolfram Alpha](https://www.wolframalpha.com), a comprehensive online intelligence engine
 - [gnu `units`](https://www.gnu.org/software/units/), a command-line tool you likely already have
 - [units](https://pypi.org/project/units/), a simple Python package for defining your own units
 - [unyt](https://pypi.org/project/unyt/), a Python package with numpy support
 
 ### 📚 _**Did you know?**_
```

### Comparing `noether-1.0.0/README.md` & `noether-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Noether 1.0
+# Noether 1.0.1 (in development)
 
 [![PyPI](https://img.shields.io/pypi/v/noether?color=blue)](https://pypi.org/packages/noether)
 
 **Noether** is a unit-enriched Python package, akin to Wolfram Alpha or gnu `units`. It has a large (and expanding) catalogue of up-to-date units and constants, allowing code to be written directly in the units they are concerned with while also ensuring e.g. you don't mistakenly add an energy to a length.
 
 Just grab Python 3.10 or later and `pip install noether` to run!
 
@@ -69,17 +69,20 @@
 ```
 
 Use `conf.save()` to save to (by default) `~/.config/noether.toml`.
 
 
 ## For more, see...
 
-Check out [CONTRIBUTING.md](CONTRIBUTING.md) and [LICENSE.txt](LICENSE.txt) for info of that sort.
+- [CHANGELOG.md](https://github.com/yunruse/Noether/blob/release/CHANGELOG.md)
+- [CONTRIBUTING.md](https://github.com/yunruse/Noether/blob/release/CONTRIBUTING.md)
+- [LICENSE.txt](https://github.com/yunruse/Noether/blob/release/LICENSE.txt)
 
 Other tools for working with units include:
+
 - [Wolfram Alpha](https://www.wolframalpha.com), a comprehensive online intelligence engine
 - [gnu `units`](https://www.gnu.org/software/units/), a command-line tool you likely already have
 - [units](https://pypi.org/project/units/), a simple Python package for defining your own units
 - [unyt](https://pypi.org/project/unyt/), a Python package with numpy support
 
 ### 📚 _**Did you know?**_
```

### Comparing `noether-1.0.0/noether/Multiplication.py` & `noether-1.0.1/noether/Multiplication.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,15 +26,21 @@
         if value is None:
             value = {}
         if not isinstance(value, dict):
             value = {value: 1}
         super().__init__(value)
 
     def items_positive_first(self):
-        return sorted(super().items(), key=lambda q: (-q[1], q[0]))
+        negative: list[tuple[T, Rational]] = []
+        for val, exp in self.items():
+            if exp < 0:
+                negative.append((val, exp))
+            else:
+                yield val, exp
+        yield from negative
 
     def __bool__(self):
         return any(x != 0 for x in self.values())
 
     def __hash__(self):
         return hash(tuple(sorted(self.items())))
 
@@ -73,27 +79,39 @@
         })
 
     # % Display
 
     def display(
         self, /,
         display_function: Callable[[T], str] = lambda x: str(x or 1),
+        *,
+        key: Callable[[tuple[T, Rational]], tuple] | None = None,
         use_slashes=True,
         drop_multiplication_signs=False,
         identity_string='1',
     ):
         '''
         Display e.g. x**2 * y**3 or meter / second.
         Returns identity_string if empty (multiplative identity, aka 1).
         '''
         if not self:
             return identity_string
 
+        if key is not None:
+            items = list(self.items())
+            items.sort(key=key)
+        else:
+            items = list(self.items_positive_first())
+
+        all_negative = all(exp < 0 for _, exp in items)
+        if all_negative:
+            use_slashes = False
+
         string = '1'
-        for name, exp in self.items():
+        for name, exp in items:
             if not exp:
                 continue
             symbol = '*'
             use_brackets = hasattr(exp, 'denominator') and exp.denominator != 1
             if use_slashes and not use_brackets and exp < 0:
                 symbol = '/'
                 exp = -exp
@@ -108,20 +126,7 @@
         if drop_multiplication_signs:
             string = string.replace(' * ', ' ')
 
         return string
 
     def __repr__(self):
         return '{}({})'.format(type(self).__name__, dict.__repr__(self))
-
-
-T_mult = TypeVar('T_mult', Real, Rational)
-
-
-class MultiplicationWithValue(Generic[T_mult], Multiplication[T_mult]):
-    '''
-    Multiplication with a value.
-    T must support multiplication and exponentiation.
-    '''
-
-    def value(self):
-        return prod(item ** exponent for item, exponent in self.items())
```

### Comparing `noether-1.0.0/noether/__main__.py` & `noether-1.0.1/noether/__main__.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/_tokenizers.py` & `noether-1.0.1/noether/_tokenizers.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/__init__.py` & `noether-1.0.1/noether/catalogue/__init__.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/conventional/conventional.py` & `noether-1.0.1/noether/catalogue/conventional/conventional.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from ..prefixes import SI_all, SI_large, SI_small
 from ..scientific import meter, second, kilogram, kelvin
 from ..scientific import radian, turn
 from ..scientific import turn
 from ..scientific import day, hour, minute
 from ..scientific import gram
+from ..scientific import standard_gravity
 
 # % Ratio
 percent = Unit(1/100, 'percent', '%')
 permille = Unit(1/1000, 'permille', '‰')
 ppm = parts_per_million = Unit(1/1_000_000, 'parts_per_million', 'ppm')
 proof = Unit(0.5, 'proof', '°', info='alcohol purity')
 karat = Unit(
@@ -72,14 +73,22 @@
 bpm = Unit(1 / minute, "beats per minute", "bpm")
 
 deg = degree = Unit(radian * pi / 180, "degree", ["°", "deg"])
 arcminute = arcmin = Unit(degree / 60, "arcminute", ["′", "arcmin"])
 arcsecond = arcsec = Unit(
     degree / 3600, "arcsecond", ["″", "arcsec"], SI_small)
 
+# % Mechanical
+
+horsepower = Unit(
+    standard_gravity * kilogram*75 * meter / second,
+    'horsepower', 'hp',
+    info="Metric horsepower, not to be confused with the"
+    " imperial horsepower which is slightly larger")
+
 
 # % Display
 Config.register('UNITS_conventional_time', True, '''\
 Display time in year & day & hour & minute & second.''')
 if conf.get('UNITS_conventional_time'):
     display(year & day & hour & minute & second)
```

### Comparing `noether-1.0.0/noether/catalogue/conventional/imperial.py` & `noether-1.0.1/noether/catalogue/conventional/imperial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 '''
 Imperial units.
 '''
 
+# TODO: #1 all of this nonsense
+
 from fractions import Fraction
 
 from noether.core import Unit, AffineUnit
 from noether.config import Config, conf
 
 from ..scientific import meter, kelvin, mercury
-from ..scientific import cm, gram, hour
+from ..scientific import cm, gram, hour, second
 from .conventional import liter
 
 Config.register('UNITS_country', 'us', '''\
 The country to define imperial units (and other niceties) from. (Use the ISO 3166 code.)
 ''')
 _USE_US_UNITS = conf.get('UNITS_country').lower() == 'us'
 
@@ -68,19 +70,20 @@
 
 hogshead = Unit(0, "hogshead", "hhd")  # TODO
 butt = Unit(hogshead * 2, "butt")  # y'all nerds
 
 
 # % Mass
 pound = lb = Unit(453.59237 * gram, "pound", "lb")
+poundal = Unit(lb * foot / second**2, "poundal", "pdl")
 
 oz = ounce = Unit(pound / 16, "ounce", "oz")
 grain = Unit(pound / 7000, "grain", "gr")
 
 stone = st = Unit(pound * 14, "stone", "st")
 imperial_ton = Unit(pound * 2240, "ton", "t")
 
 
-# Derived
+# % Derived
 
 inch_mercury = Unit(mercury * inch,
                     "inch_mercury", "inHg")
```

### Comparing `noether-1.0.0/noether/catalogue/conventional/typographic.py` & `noether-1.0.1/noether/catalogue/conventional/typographic.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/dimensions.py` & `noether-1.0.1/noether/catalogue/dimensions.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/fundamental.py` & `noether-1.0.1/noether/catalogue/fundamental.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/historic/ancient_greek.units.py` & `noether-1.0.1/noether/catalogue/historic/ancient_greek.units.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/historic/ancient_greek_.py` & `noether-1.0.1/noether/catalogue/historic/ancient_greek_.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/historic/mts.units.py` & `noether-1.0.1/noether/catalogue/historic/mts.units.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/historic/mts_.py` & `noether-1.0.1/noether/catalogue/historic/mts_.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/humorous/fictional.py` & `noether-1.0.1/noether/catalogue/humorous/fictional.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/humorous/potrzebie.py` & `noether-1.0.1/noether/catalogue/humorous/potrzebie.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/humorous/unusual.py` & `noether-1.0.1/noether/catalogue/humorous/unusual.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/info/comparison.py` & `noether-1.0.1/noether/catalogue/info/comparison.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/info/spectrum.py` & `noether-1.0.1/noether/catalogue/info/spectrum.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/prefixes.py` & `noether-1.0.1/noether/catalogue/prefixes.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/scientific/CODATA.py` & `noether-1.0.1/noether/catalogue/scientific/CODATA.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/scientific/astronomy.py` & `noether-1.0.1/noether/catalogue/scientific/astronomy.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/scientific/cgs.py` & `noether-1.0.1/noether/catalogue/scientific/cgs.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/scientific/constants.py` & `noether-1.0.1/noether/catalogue/scientific/constants.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/scientific/data.py` & `noether-1.0.1/noether/catalogue/scientific/data.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/scientific/essential.py` & `noether-1.0.1/noether/catalogue/scientific/essential.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/catalogue/scientific/si.py` & `noether-1.0.1/noether/catalogue/scientific/si.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 katal = kat = SI_d(Unit(catalytic_activity, 'katal', "kat", SI_all))
 
 
 # % Constants defined as part of SI
 
 # GCWM 3
 standard_gravity = Unit(
-    9.980665 * meter / second**2,
+    9.80665 * meter / second**2,
     "standard_gravity", "g", info="defined by convention")
 
 # GCWM 17
 speed_of_light = c = Unit(299_792_458 * meter / second, "c", "c")
 
 # GCWM 26 (2019 redefinition of the SI base units)
 electron_charge = e = Unit(
```

### Comparing `noether-1.0.0/noether/config.py` & `noether-1.0.1/noether/config.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/core/Catalogue.py` & `noether-1.0.1/noether/core/Catalogue.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             self.dimensions[name] = value
         elif isinstance(value, PrefixSet):
             self.prefix_sets[name] = value
             for prefix in value:
                 self._prefixes[prefix.prefix] = prefix
                 self._prefixes[prefix.symbol] = prefix
 
-    def get(self, name: str):
+    def get_unit(self, name: str):
         for col in (self.prefix_sets, self.dimensions, self.units_by_name):
             if name in col:
                 return col[name]
 
         for p, prefix in self._prefixes.items():
             if not name.startswith(p):
                 continue
@@ -72,16 +72,21 @@
                     continue
             return prefix.value * unit
 
         raise NameError(
             f'No unit (or prefixed unit)'
             f' with name {name!r} could be found.')
 
+    def get(self, name: str):
+        return self.get_unit(name)
+        # TODO: allow prefixes, numbers —
+        # anything `units` allows
+
     def __getitem__(self, name: str):
-        return self.get(name)
+        return self.get_unit(name)
 
     def units(self):
         return set(self.units_by_name.values())
 
     def prefixes(self):
         for prefix_set in self.prefix_sets.values():
             yield from prefix_set
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `noether-1.0.0/noether/core/Dimension.py` & `noether-1.0.1/noether/core/Dimension.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from noether.display import DISPLAY_REPR_CODE
 
 from ..config import conf
 
 
 BaseDimension = str
 DimInfo = namedtuple('DimInfo', ('order', 'symbol'))
+BaseDimDict = dict[BaseDimension, Rational]
 
 
 class Dimension(Multiplication[BaseDimension]):
     '''
     Dimension of a unit, such as time, speed or temperature.
     '''
 
@@ -27,30 +28,34 @@
     # Known composed dimension names
     _names: ClassVar[dict['Dimension', list[str]]] = dict()
 
     # Instantiation
 
     def __init__(
         self,
-        dimensions: dict[BaseDimension, Rational] | None = None,
+        dimensions: BaseDimension | BaseDimDict | None = None,
         *names: str
     ):
-        dimensions = dimensions or {}
-        well_formed = all(
-            isinstance(d, BaseDimension)
-            and d in type(self)._known_dimensions
-            for d, exp in dimensions.items()
-        )
-        if not well_formed:
-            raise TypeError(
-                "Malformed Dimension."
-                " Use e.g. `length = Dimension.new(...)`"
-                " and compose derived dimensions.")
+        dims: BaseDimDict = {}
+        if isinstance(dimensions, BaseDimension):
+            dims = {dimensions: 1}
+        elif isinstance(dimensions, dict):
+            dims = dimensions
+            well_formed = all(
+                isinstance(d, BaseDimension)
+                and d in type(self)._known_dimensions
+                for d, exp in dimensions.items()
+            )
+            if not well_formed:
+                raise TypeError(
+                    "Malformed Dimension."
+                    " Use e.g. `length = Dimension.new(...)`"
+                    " and compose derived dimensions.")
 
-        super().__init__(dimensions)
+        super().__init__(dims)
         self._names.setdefault(self, [])
         self._names[self].extend(names)
 
     @classmethod
     def new(
         cls,
         name: BaseDimension,
@@ -83,22 +88,31 @@
     #         |        _/
 
     @wraps(Multiplication.display)
     def display(self, **kwargs):
         kwargs.setdefault('identity_string', 'dimensionless')
         return super().display(**kwargs)
 
-    def as_symbols(self):
+    @property
+    def symbol(self):
         return super().display(
             display_function=lambda b: self._known_dimensions[b].symbol,
             drop_multiplication_signs=True,
             identity_string='1'
         )
 
     @property
+    def order(self):
+        if self.is_base_dimension():
+            k = list(self)[0]
+            return self._known_dimensions[k].order
+        # TODO: could this be more specific?
+        return 999
+
+    @property
     def names(self):
         # TODO: Fetch for equality..?
         return self._names[self]
 
     def name(self):
         if self.names:
             return self.names[0]
```

### Comparing `noether-1.0.0/noether/core/Measure.py` & `noether-1.0.1/noether/core/Measure.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 from dataclasses import dataclass
 from functools import total_ordering
 import operator
 from sys import version_info
 from typing import Callable, Optional, TypeVar, ClassVar, Generic, TYPE_CHECKING
 from noether.helpers import MeasureValue
 
-from noether.helpers import removeprefix
-
 from ..errors import NoetherError, DimensionError
 from ..config import Config, conf
-from ..display import DISPLAY_REPR_CODE, canonical_number
+from ..display import DISPLAY_REPR_CODE
 from .Prefix import Prefix
 from .Dimension import Dimension, dimensionless
 from .MeasureInfo import MeasureInfo
 
 if TYPE_CHECKING:
     from .Unit import Unit
     from .UnitSet import UnitSet
@@ -25,19 +23,14 @@
 OPENLINEAR = Config.register("measure_ignore_dimension", False, """\
 Allow any addition, even between incompatible units
 (eg metre and second)""")
 
 BARENUMBER = Config.register("measure_barenumber", False, """\
 Allow addition and subtraction of bare numbers to units""")
 
-UNCERTAINTY_OVERLAP = Config.register("uncertainty_compare_range_overlap", False, """\
-When comparing a Measure, compare on the uncertainty.
-For == this means 'do the ranges overlap';
-for < it means 'do the ranges not overlap'.""")
-
 UNCERTAINTY_SHORTHAND = Config.register("uncertainty_display_shorthand", False, """\
 Display e.g. 0.15(2) instead of 0.15 ± 0.02.""")
 
 T = TypeVar('T', int, MeasureValue)
 
 
 @dataclass(
@@ -99,20 +92,14 @@
 
     @property
     def epsilon(self):
         if self.stddev is None or not self._value:
             return None
         return self.stddev / self._value
 
-    @property
-    def bounds(self) -> tuple[T, T]:
-        if self.stddev is None:
-            return self._value, self._value
-        return self._value - self.stddev, self._value + self.stddev  # type: ignore
-
     # |\  |              |
     # | \ ||   ||/~\ /~\ |~~\/~/|/~\
     # |  \| \_/||   |   ||__/\/_|
 
     def __float__(self): return float(self._value)
     def __int__(self): return int(self._value)
     def __bool__(self): return bool(self._value)
@@ -159,30 +146,17 @@
 
     def _info(self):
         for handler in self.info_handlers:
             if conf.get(handler.__name__) and handler.should_display(self):
                 for i in handler.info(self):
                     yield i, handler.style
 
-    def display_unit(self) -> 'Unit | None':
-        from ._DisplayHandler import display
-        units = display.dimension_units.get(self.dim, [])
-        if units:
-            return units[-1]
-
-    def _as_composed_string(self) -> str:
+    def display_unit(self) -> 'Unit':
         from ._DisplayHandler import display
-
-        unit = self.dim.display(
-            display_function=lambda x: display._dimension_symbol[x],
-            drop_multiplication_signs=True,
-            identity_string='',
-        )
-
-        return removeprefix(unit, '1 ')  # avoid "2  1 / m"
+        return display.dimension_unit(self.dim)
 
     def __repr__(self):
         if conf.get(DISPLAY_REPR_CODE):
             return self._repr_code()
         return self.__noether__()
 
     def _repr_code(self):
@@ -190,24 +164,16 @@
         if self.stddev is not None:
             chunks.append(repr(self.stddev))
         if self.dim:
             chunks.append('dim=' + self.dim._repr_code())
 
         return 'Measure({})'.format(', '.join(chunks))
 
-    @staticmethod
-    def _repr_measure(measure: 'Measure'):
-        # Fallback if no unit found
-        n = canonical_number(measure._value, measure.stddev,
-                             conf.get(UNCERTAINTY_SHORTHAND))
-        s = measure._as_composed_string()
-        return f'{n} {s}'.strip()
-
     def __str__(self):
-        return (self.display_unit() or self)._repr_measure(self)
+        return self.display_unit()._repr_measure(self)
 
     def __noether__(self):
         info = ', '.join(i for i, _ in self._info())
         if info:
             info = '  # ' + info
         return str(self).strip() + info
 
@@ -273,30 +239,31 @@
     def __abs__(self):
         return self if self._value > 0 else -self  # type: ignore
 
     def __lin_cmp(self, other, op: Callable):
         if conf.get(OPENLINEAR):
             return
 
+        match op:
+            case operator.add: oper = "Addition"
+            case operator.sub: oper = "Subtraction"
+            case operator.mod: oper = "Modulo"
+            case operator.lt: oper = "Comparison"
+            case _: oper = "A linear operation"
+
         if isinstance(other, Measure):
             if self.dim != other.dim:
-                match op:
-                    case operator.add: oper = "Addition"
-                    case operator.sub: oper = "Subtraction"
-                    case operator.mod: oper = "Modulo"
-                    case operator.lt: oper = "Comparison"
-                    case _: oper = "A linear operation"
-
                 raise DimensionError(
                     self.dim, other.dim,
-                    f"{oper} only works on units of the same dimension. Enable conf.{OPENLINEAR} to bypass this.")
+                    f"{oper} only works on units of the same dimension."
+                    f" Enable conf.{OPENLINEAR} to bypass this.")
 
         elif not conf.get(BARENUMBER):
             raise NoetherError(
-                "A measure may not linearly operate on a number."
+                f"{oper} only works on Measures and Units."
                 f" Enable conf.{BARENUMBER} to bypass this.")
 
     def __lin(self, other: 'Measure[T] | Dimension | MeasureValue', op: Callable):
         self.__lin_cmp(other, op)
 
         value = self._value
         stddev = self.stddev
@@ -324,30 +291,19 @@
 
     # Equality and ordering
 
     def __eq__(self, other):
         if isinstance(other, Measure):
             if other.dim != self.dim and not conf.get(OPENLINEAR):
                 return False
-            if conf.get(UNCERTAINTY_OVERLAP):
-                s_min, s_max = self.bounds
-                o_min, o_max = other.bounds
-                return ((s_min <= o_min <= s_max) or
-                        (s_min <= o_max <= s_max) or
-                        (o_min <= s_min <= o_max) or
-                        (o_min <= s_max <= o_max))
             return self._value == other._value
 
     def __lt__(self, other):
         self.__lin_cmp(other, operator.lt)
         if isinstance(other, Measure):
-            if conf.get(UNCERTAINTY_OVERLAP):
-                s_min, s_max = self.bounds
-                o_min, o_max = other.bounds
-                return s_max < o_min
             return self._value < other._value
 
     #  /~~       |               |~~\ '      |
     # |  |   |(~~|~/~\|/~\ /~\   |   ||(~|~~\|/~~|\  /
     #  \__\_/|_) | \_/|   |   |  |__/ |_)|__/|\__| \/
     #                                    |        _/
```

### Comparing `noether-1.0.0/noether/core/MeasureRelative.py` & `noether-1.0.1/noether/core/MeasureRelative.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/core/Prefix.py` & `noether-1.0.1/noether/core/Prefix.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/core/Unit.py` & `noether-1.0.1/noether/core/Unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Unit - a subclass of Measure which has its own name(s) and symbol(s).
 
 Used in turn to display Measure.
 '''
 
 from datetime import timedelta
 from itertools import chain
-from noether.helpers import Rational, Real
+from noether.helpers import Rational, Real, removeprefix
 
 from ..errors import NoetherError
 from ..config import conf
 from ..display import DISPLAY_REPR_CODE, canonical_number
 from .Prefix import Prefix, PrefixSet
 from .Dimension import Dimension
 from .Measure import Measure, UNCERTAINTY_SHORTHAND
@@ -77,29 +77,40 @@
 
     def __truediv__(self, value: Measure | Real) -> Measure:
         return GeometricUnit(self) / value  # type: ignore
 
     def __pow__(self, value: Rational) -> Measure:
         return GeometricUnit(self) ** value
 
+    def _fallback_display(self) -> str:
+        from ._DisplayHandler import display
+
+        unit = self.dim.display(
+            display_function=lambda x: display._dimension_symbol[x],
+            drop_multiplication_signs=True,
+            identity_string='',
+        )
+
+        return removeprefix(unit, '1 ')  # avoid "2  1 / m"
+
     @property
     def symbol(self):
         if self.symbols:
             return self.symbols[0]
         if self.names:
             return self.names[0]
-        return self._as_composed_string()
+        return self._fallback_display()
 
     @property
     def name(self):
         if self.names:
             return self.names[0]
         if self.symbols:
             return self.symbols[0]
-        return self._as_composed_string()
+        return self._fallback_display()
 
     # |~~\ '      |
     # |   ||(~|~~\|/~~|\  /
     # |__/ |_)|__/|\__| \/
     #         |        _/
 
     def __repr__(self):
```

### Comparing `noether-1.0.0/noether/core/UnitSet.py` & `noether-1.0.1/noether/core/UnitSet.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/core/_DisplayHandler.py` & `noether-1.0.1/noether/core/_DisplayHandler.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,14 +20,33 @@
         self.dimension_units = dict()
         self._dimension_symbol = dict(dimensionless='')
 
         self.displays(*items)
 
     T = TypeVar('T', Unit, Dimension, 'UnitSet')
 
+    def dimension_unit(self, dim: Dimension):
+        units = self.dimension_units.get(dim, [])
+        if units:
+            return units[-1]
+
+        from noether.core.units import GeometricUnit, LinearUnit
+        from .Dimension import BaseDimension
+
+        def resolve(d: BaseDimension):
+            d2 = display.dimension_units[Dimension(d)][-1]
+            if isinstance(d2, LinearUnit):
+                return d2.units[-1]
+            return d2
+
+        return GeometricUnit({
+            resolve(d): exp
+            for d, exp in dim.items()
+        })
+
     def display(self, value: T) -> T:
         if isinstance(value, Dimension):
             self.dimensions.add(value)
 
         elif isinstance(value, Unit):
             self.dimension_units.setdefault(value.dim, [])
             self.dimension_units[value.dim].append(value)
```

### Comparing `noether-1.0.0/noether/core/units/AffineUnit.py` & `noether-1.0.1/noether/core/units/AffineUnit.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/core/units/GeometricUnit.py` & `noether-1.0.1/noether/core/units/GeometricUnit.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,29 +23,40 @@
         else:
             unit = unit_or_dict
             units = Multiplication(unit)
 
         super().__init__(unit)
         object.__setattr__(self, 'units', units)
 
+    @staticmethod
+    def _resolve_unit(u: Unit):
+        from .LinearUnit import LinearUnit
+        if isinstance(u, LinearUnit):
+            u = u.units[-1]
+
+        if isinstance(u, GeometricUnit):
+            return u.units
+        return u
+
     def __mul__(self, value: Unit):
         if isinstance(value, Unit):
-            v = value.units if isinstance(value, GeometricUnit) else value
-            return type(self)(self.units * v)
+            return type(self)(self.units * self._resolve_unit(value))
         return Measure.__mul__(self, value)
 
     def __truediv__(self, value: Unit):
         if isinstance(value, Unit):
-            v = value.units if isinstance(value, GeometricUnit) else value
-            return type(self)(self.units / v)
+            return type(self)(self.units / self._resolve_unit(value))
         return Measure.__truediv__(self, value)
 
     def __pow__(self, exponent: Rational):
         return type(self)(self.units ** exponent)
 
     @property
     def name(self):
-        return self.units.display()
+        return self.units.display(key=lambda q: (-q[1], q[0].dim.order))
 
     @property
     def symbol(self):
-        return self.units.display(lambda x: x.symbol)
+        return self.units.display(
+            lambda x: x.symbol,
+            key=lambda q: (-q[1], q[0].dim.order),
+            drop_multiplication_signs=True)
```

### Comparing `noether-1.0.0/noether/core/units/LinearUnit.py` & `noether-1.0.1/noether/core/units/LinearUnit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Iterable
 
-from noether.display import DISPLAY_REPR_CODE
+from noether.display import DISPLAY_REPR_CODE, canonical_number, plus_minus_symbol
 from ...config import conf
 from ..Measure import Measure
 from ..Unit import Unit
 
 
 # TODO: should & be replaced with +?
 # It would slightly make things confusing in fairness.
@@ -54,19 +54,28 @@
             return f'{self}[green italic]  # {self.dim.name()}'
         return str(self)
 
     def __str__(self):
         return ' & '.join([x.name for x in self.units])
 
     def _repr_measure(self, measure: Measure):
-        # TODO: handle stddev!
         value = measure._value
         chunks = []
         for i, unit in enumerate(self.units):
             if i == len(self.units)-1:
                 dv = value / unit._value
             else:
                 dv, value = divmod(value, unit._value)
             if dv:
-                chunks.append(f'{dv} {unit.symbol}')
+                chunks.append(f'{canonical_number(dv)} {unit.symbol}')
 
-        return ' + '.join(chunks)
+        result = ' + '.join(chunks)
+
+        if measure.stddev is not None:
+            for su in self.units:
+                if measure.stddev > su._value:
+                    break
+            pm = plus_minus_symbol()
+            dv = measure.stddev / su._value
+            result += f' {pm} {canonical_number(dv)} {su.symbol}'
+
+        return result
```

### Comparing `noether-1.0.0/noether/core/units/PrefixedUnit.py` & `noether-1.0.1/noether/core/units/PrefixedUnit.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/errors.py` & `noether-1.0.1/noether/errors.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether/helpers.py` & `noether-1.0.1/noether/helpers.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.0/noether.egg-info/PKG-INFO` & `noether-1.0.1/noether.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: noether
-Version: 1.0.0
+Version: 1.0.1
 Summary: Work with physical measurements and constants
 Home-page: https://github.com/yunruse/noether
 Author: Mia yun Ruse
 Author-email: mia@yunru.se
 Keywords: physics unit measure constant measurement uncertainty
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved
 Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Noether 1.0
+# Noether 1.0.1 (in development)
 
 [![PyPI](https://img.shields.io/pypi/v/noether?color=blue)](https://pypi.org/packages/noether)
 
 **Noether** is a unit-enriched Python package, akin to Wolfram Alpha or gnu `units`. It has a large (and expanding) catalogue of up-to-date units and constants, allowing code to be written directly in the units they are concerned with while also ensuring e.g. you don't mistakenly add an energy to a length.
 
 Just grab Python 3.10 or later and `pip install noether` to run!
 
@@ -86,17 +86,20 @@
 ```
 
 Use `conf.save()` to save to (by default) `~/.config/noether.toml`.
 
 
 ## For more, see...
 
-Check out [CONTRIBUTING.md](CONTRIBUTING.md) and [LICENSE.txt](LICENSE.txt) for info of that sort.
+- [CHANGELOG.md](https://github.com/yunruse/Noether/blob/release/CHANGELOG.md)
+- [CONTRIBUTING.md](https://github.com/yunruse/Noether/blob/release/CONTRIBUTING.md)
+- [LICENSE.txt](https://github.com/yunruse/Noether/blob/release/LICENSE.txt)
 
 Other tools for working with units include:
+
 - [Wolfram Alpha](https://www.wolframalpha.com), a comprehensive online intelligence engine
 - [gnu `units`](https://www.gnu.org/software/units/), a command-line tool you likely already have
 - [units](https://pypi.org/project/units/), a simple Python package for defining your own units
 - [unyt](https://pypi.org/project/unyt/), a Python package with numpy support
 
 ### 📚 _**Did you know?**_
```

### Comparing `noether-1.0.0/noether.egg-info/SOURCES.txt` & `noether-1.0.1/noether.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 noether/Multiplication.py
 noether/__init__.py
 noether/__main__.py
 noether/_tokenizers.py
 noether/config.py
 noether/display.py
 noether/errors.py
+noether/gnu.py
 noether/helpers.py
 noether.egg-info/PKG-INFO
 noether.egg-info/SOURCES.txt
 noether.egg-info/dependency_links.txt
 noether.egg-info/top_level.txt
 noether/catalogue/__init__.py
 noether/catalogue/dimensions.py
```

### Comparing `noether-1.0.0/setup.py` & `noether-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as f:
     long_description = f.read()
 
 packages = setuptools.find_packages()
 
 setuptools.setup(
     name="noether",
-    version="1.0.0",
+    version="1.0.1",
     author="Mia yun Ruse",
     author_email="mia@yunru.se",
     description="Work with physical measurements and constants",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yunruse/noether",
     packages=packages,
```

