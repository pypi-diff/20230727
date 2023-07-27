# Comparing `tmp/pyTMD-2.0.5.tar.gz` & `tmp/pyTMD-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTMD-2.0.5.tar", last modified: Wed Jun 14 19:11:59 2023, max compression
+gzip compressed data, was "pyTMD-2.0.6.tar", last modified: Thu Jul 27 19:41:18 2023, max compression
```

## Comparing `pyTMD-2.0.5.tar` & `pyTMD-2.0.6.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:11:59.154677 pyTMD-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-06-14 19:11:42.000000 pyTMD-2.0.5/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-14 19:11:42.000000 pyTMD-2.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     5545 2023-06-14 19:11:42.000000 pyTMD-2.0.5/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (122)      620 2023-06-14 19:11:42.000000 pyTMD-2.0.5/CONTRIBUTORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-06-14 19:11:42.000000 pyTMD-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-14 19:11:42.000000 pyTMD-2.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6785 2023-06-14 19:11:59.154677 pyTMD-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5883 2023-06-14 19:11:42.000000 pyTMD-2.0.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-14 19:11:42.000000 pyTMD-2.0.5/postBuild
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:11:59.138677 pyTMD-2.0.5/pyTMD/
--rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    20738 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/arguments.py
--rw-r--r--   0 runner    (1001) docker     (122)    43421 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/astro.py
--rw-r--r--   0 runner    (1001) docker     (122)     3376 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/calc_astrol_longitudes.py
--rw-r--r--   0 runner    (1001) docker     (122)     9072 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/check_tide_points.py
--rw-r--r--   0 runner    (1001) docker     (122)    43968 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/compute_tide_corrections.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    12861 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    16129 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/convert_crs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/convert_ll_xy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:11:59.150677 pyTMD-2.0.5/pyTMD/data/
--rwxr-xr-x   0 runner    (1001) docker     (122)    12369 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)  3539852 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/finals.all
--rwxr-xr-x   0 runner    (1001) docker     (122)    30345 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/historic_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)   130160 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/iers_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)    10666 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/leap-seconds.list
--rwxr-xr-x   0 runner    (1001) docker     (122)    78944 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/mean-pole.tab
--rwxr-xr-x   0 runner    (1001) docker     (122)   154820 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/merged_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)  6325011 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/opoleloadcoefcmcor.txt.gz
--rwxr-xr-x   0 runner    (1001) docker     (122)    41600 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/ser7.dat
--rw-r--r--   0 runner    (1001) docker     (122)     5849 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/tab5.2e.txt
--rw-r--r--   0 runner    (1001) docker     (122)   145678 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/tab5.3a.txt
--rw-r--r--   0 runner    (1001) docker     (122)   113660 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/tab5.3b.txt
--rw-r--r--   0 runner    (1001) docker     (122)    17529 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/eop.py
--rw-r--r--   0 runner    (1001) docker     (122)    15243 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:11:59.150677 pyTMD-2.0.5/pyTMD/io/
--rw-r--r--   0 runner    (1001) docker     (122)    43622 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/ATLAS.py
--rw-r--r--   0 runner    (1001) docker     (122)    31955 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/FES.py
--rw-r--r--   0 runner    (1001) docker     (122)    28562 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/GOT.py
--rw-r--r--   0 runner    (1001) docker     (122)    71516 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/OTIS.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4469 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/constituents.py
--rw-r--r--   0 runner    (1001) docker     (122)    66877 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/ocean_pole_tide.py
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/load_constituent.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4904 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/load_nodal_corrections.py
--rw-r--r--   0 runner    (1001) docker     (122)    42856 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)    61851 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/spatial.py
--rw-r--r--   0 runner    (1001) docker     (122)     2966 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/tidal_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (122)    59968 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/time.py
--rw-r--r--   0 runner    (1001) docker     (122)    11877 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)    49462 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:11:59.138677 pyTMD-2.0.5/pyTMD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6785 2023-06-14 19:11:58.000000 pyTMD-2.0.5/pyTMD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1555 2023-06-14 19:11:59.000000 pyTMD-2.0.5/pyTMD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 19:11:58.000000 pyTMD-2.0.5/pyTMD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-14 19:11:58.000000 pyTMD-2.0.5/pyTMD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-14 19:11:58.000000 pyTMD-2.0.5/pyTMD.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-06-14 19:11:42.000000 pyTMD-2.0.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-06-14 19:11:42.000000 pyTMD-2.0.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:11:59.154677 pyTMD-2.0.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/arcticdata_tides.py
--rw-r--r--   0 runner    (1001) docker     (122)    13977 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/aviso_fes_tides.py
--rw-r--r--   0 runner    (1001) docker     (122)    14779 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/compute_LPET_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)    18669 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/compute_LPT_displacements.py
--rw-r--r--   0 runner    (1001) docker     (122)    20990 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/compute_OPT_displacements.py
--rw-r--r--   0 runner    (1001) docker     (122)    19206 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/compute_SET_displacements.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    23194 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/compute_tidal_currents.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    23395 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/compute_tidal_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)    11560 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/reduce_OTIS_files.py
--rw-r--r--   0 runner    (1001) docker     (122)     5130 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/usap_cats_tides.py
--rw-r--r--   0 runner    (1001) docker     (122)     7926 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/verify_box_tpxo.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 19:11:59.154677 pyTMD-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3960 2023-06-14 19:11:42.000000 pyTMD-2.0.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-14 19:11:42.000000 pyTMD-2.0.5/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:41:18.467319 pyTMD-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-27 19:41:06.000000 pyTMD-2.0.6/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-07-27 19:41:06.000000 pyTMD-2.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     5545 2023-07-27 19:41:06.000000 pyTMD-2.0.6/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-07-27 19:41:06.000000 pyTMD-2.0.6/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-07-27 19:41:06.000000 pyTMD-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-07-27 19:41:06.000000 pyTMD-2.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6785 2023-07-27 19:41:18.467319 pyTMD-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5883 2023-07-27 19:41:06.000000 pyTMD-2.0.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-07-27 19:41:06.000000 pyTMD-2.0.6/postBuild
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:41:18.451319 pyTMD-2.0.6/pyTMD/
+-rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    20738 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43421 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/astro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3376 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/calc_astrol_longitudes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8966 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/check_tide_points.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43865 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/compute_tide_corrections.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    12861 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16026 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/convert_crs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/convert_ll_xy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:41:18.463319 pyTMD-2.0.6/pyTMD/data/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    12369 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/data/deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)  3546432 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/data/finals.all
+-rwxr-xr-x   0 runner    (1001) docker     (122)    30345 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/data/historic_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)   130160 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/data/iers_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10666 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/data/leap-seconds.list
+-rwxr-xr-x   0 runner    (1001) docker     (122)    79008 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/data/mean-pole.tab
+-rwxr-xr-x   0 runner    (1001) docker     (122)   155800 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/data/merged_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)  6325011 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/data/opoleloadcoefcmcor.txt.gz
+-rwxr-xr-x   0 runner    (1001) docker     (122)    34592 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/data/ser7.dat
+-rw-r--r--   0 runner    (1001) docker     (122)     5849 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/data/tab5.2e.txt
+-rw-r--r--   0 runner    (1001) docker     (122)   145678 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/data/tab5.3a.txt
+-rw-r--r--   0 runner    (1001) docker     (122)   113660 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/data/tab5.3b.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    17529 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/eop.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15243 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:41:18.463319 pyTMD-2.0.6/pyTMD/io/
+-rw-r--r--   0 runner    (1001) docker     (122)    43520 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/io/ATLAS.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31853 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/io/FES.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28457 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/io/GOT.py
+-rw-r--r--   0 runner    (1001) docker     (122)    71426 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/io/OTIS.py
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4602 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/io/constituents.py
+-rw-r--r--   0 runner    (1001) docker     (122)    66877 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/io/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/io/ocean_pole_tide.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/load_constituent.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4904 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/load_nodal_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42856 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    61629 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2966 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/tidal_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (122)    60055 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11877 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49462 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-27 19:41:06.000000 pyTMD-2.0.6/pyTMD/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:41:18.451319 pyTMD-2.0.6/pyTMD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6785 2023-07-27 19:41:18.000000 pyTMD-2.0.6/pyTMD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1555 2023-07-27 19:41:18.000000 pyTMD-2.0.6/pyTMD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 19:41:18.000000 pyTMD-2.0.6/pyTMD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-27 19:41:18.000000 pyTMD-2.0.6/pyTMD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-27 19:41:18.000000 pyTMD-2.0.6/pyTMD.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-27 19:41:06.000000 pyTMD-2.0.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-07-27 19:41:06.000000 pyTMD-2.0.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:41:18.467319 pyTMD-2.0.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-07-27 19:41:06.000000 pyTMD-2.0.6/scripts/arcticdata_tides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13977 2023-07-27 19:41:06.000000 pyTMD-2.0.6/scripts/aviso_fes_tides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14661 2023-07-27 19:41:06.000000 pyTMD-2.0.6/scripts/compute_LPET_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18551 2023-07-27 19:41:06.000000 pyTMD-2.0.6/scripts/compute_LPT_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20872 2023-07-27 19:41:06.000000 pyTMD-2.0.6/scripts/compute_OPT_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19088 2023-07-27 19:41:06.000000 pyTMD-2.0.6/scripts/compute_SET_displacements.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23076 2023-07-27 19:41:06.000000 pyTMD-2.0.6/scripts/compute_tidal_currents.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23277 2023-07-27 19:41:06.000000 pyTMD-2.0.6/scripts/compute_tidal_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11457 2023-07-27 19:41:06.000000 pyTMD-2.0.6/scripts/reduce_OTIS_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5130 2023-07-27 19:41:06.000000 pyTMD-2.0.6/scripts/usap_cats_tides.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7926 2023-07-27 19:41:06.000000 pyTMD-2.0.6/scripts/verify_box_tpxo.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-27 19:41:18.467319 pyTMD-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3960 2023-07-27 19:41:06.000000 pyTMD-2.0.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-27 19:41:06.000000 pyTMD-2.0.6/version.txt
```

### Comparing `pyTMD-2.0.5/.gitignore` & `pyTMD-2.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/CODE_OF_CONDUCT.rst` & `pyTMD-2.0.6/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/CONTRIBUTORS.rst` & `pyTMD-2.0.6/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/LICENSE` & `pyTMD-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/PKG-INFO` & `pyTMD-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTMD
-Version: 2.0.5
+Version: 2.0.6
 Summary: Tide Model Driver to read OTIS, GOT and FES formatted tidal solutions and make tidal predictions
 Home-page: https://github.com/tsutterley/pyTMD
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: Ocean Tides,Load Tides,Pole Tides,Tidal Prediction,OTIS,GOT,FES
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyTMD-2.0.5/README.rst` & `pyTMD-2.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/__init__.py` & `pyTMD-2.0.6/pyTMD/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/arguments.py` & `pyTMD-2.0.6/pyTMD/arguments.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/astro.py` & `pyTMD-2.0.6/pyTMD/astro.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/calc_astrol_longitudes.py` & `pyTMD-2.0.6/pyTMD/calc_astrol_longitudes.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/check_tide_points.py` & `pyTMD-2.0.6/pyTMD/check_tide_points.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,32 +64,29 @@
     Updated 09/2021: refactor to use model class for files and attributes
     Updated 07/2021: added check that tide model directory is accessible
     Updated 06/2021: add try/except for input projection strings
     Written 05/2021
 """
 from __future__ import print_function, annotations
 
+import logging
 import pathlib
-import warnings
 import numpy as np
 import scipy.interpolate
 
 import pyTMD.io
 import pyTMD.io.model
 import pyTMD.convert_crs
 import pyTMD.interpolate
 
 # attempt imports
 try:
     import pyproj
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("pyproj not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.debug("pyproj not available")
 
 # PURPOSE: compute tides at points and times using tide model algorithms
 def check_tide_points(x: np.ndarray, y: np.ndarray,
         DIRECTORY: str | pathlib.Path | None = None,
         MODEL: str | None = None,
         ATLAS_FORMAT: str = 'netcdf',
         GZIP: bool = False,
```

### Comparing `pyTMD-2.0.5/pyTMD/compute_tide_corrections.py` & `pyTMD-2.0.6/pyTMD/compute_tide_corrections.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,16 @@
     Updated 07/2020: added function docstrings, FES2014 and TPXO9-atlas-v2
         use merged delta time files combining biannual, monthly and daily files
     Updated 03/2020: added TYPE, TIME, FILL_VALUE and METHOD options
     Written 03/2020
 """
 from __future__ import print_function, annotations
 
+import logging
 import pathlib
-import warnings
 import numpy as np
 import scipy.interpolate
 import pyTMD.constants
 import pyTMD.eop
 import pyTMD.io
 import pyTMD.time
 import pyTMD.io.model
@@ -114,18 +114,15 @@
 import pyTMD.spatial
 import pyTMD.utilities
 
 # attempt imports
 try:
     import pyproj
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("pyproj not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.critical("pyproj not available")
 
 # PURPOSE: wrapper function for computing corrections
 def compute_corrections(
         x: np.ndarray, y: np.ndarray, delta_time: np.ndarray,
         CORRECTION: str = 'ocean',
         **kwargs
     ):
```

### Comparing `pyTMD-2.0.5/pyTMD/constants.py` & `pyTMD-2.0.6/pyTMD/constants.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/convert_crs.py` & `pyTMD-2.0.6/pyTMD/convert_crs.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,25 +43,22 @@
     Updated 07/2020: added function docstrings. changed function name
     Updated 03/2020: remove commented coordinate conversion functions
     Updated 11/2019: using pyproj for coordinate conversions
     Written 09/2017
 """
 from __future__ import annotations
 
-import warnings
+import logging
 import numpy as np
 
 # attempt imports
 try:
     import pyproj
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("pyproj not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.critical("pyproj not available")
 
 def convert_crs(
         i1: np.ndarray,
         i2: np.ndarray,
         PROJ: str,
         BF: str,
         EPSG: int | str = 4326
```

### Comparing `pyTMD-2.0.5/pyTMD/convert_ll_xy.py` & `pyTMD-2.0.6/pyTMD/convert_ll_xy.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/data/deltat.data` & `pyTMD-2.0.6/pyTMD/data/deltat.data`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/data/finals.all` & `pyTMD-2.0.6/pyTMD/data/finals.all`

 * *Files 0% similar despite different names*

```diff
@@ -17519,1303 +17519,1303 @@
 201219 59202.00 I  0.081217 0.000016  0.294917 0.000025  I-0.1784625 0.0000079 -0.2367 0.0055  I  -109.960    0.049    -6.330    0.117  0.081252  0.294893 -0.1784509  -109.955    -6.376  
 201220 59203.00 I  0.080071 0.000035  0.295229 0.000025  I-0.1783116 0.0000088 -0.0748 0.0050  I  -109.877    0.526    -6.166    0.071  0.080081  0.295269 -0.1783092  -109.755    -6.220  
 201221 59204.00 I  0.078889 0.000047  0.295493 0.000025  I-0.1782977 0.0000062  0.0416 0.0057  I  -109.949    0.491    -5.876    0.090  0.078855  0.295467 -0.1782871  -109.702    -5.936  
 201222 59205.00 I  0.077910 0.000045  0.295780 0.000018  I-0.1783938 0.0000071  0.1550 0.0052  I  -109.928    0.610    -5.645    0.074  0.077844  0.295794 -0.1783855  -109.670    -5.733  
 201223 59206.00 I  0.077249 0.000027  0.296066 0.000020  I-0.1785629 0.0000083  0.1341 0.0055  I  -110.129    0.610    -5.596    0.074  0.077211  0.296035 -0.1785628  -110.200    -5.518  
 201224 59207.00 I  0.076987 0.000027  0.296519 0.000020  I-0.1786356 0.0000084  0.0342 0.0058  I  -110.285    0.610    -5.558    0.074  0.077007  0.296472 -0.1786681  -110.461    -5.415  
 201225 59208.00 I  0.076677 0.000028  0.297249 0.000021  I-0.1786349 0.0000080 -0.0547 0.0057  I  -110.355    0.610    -5.423    0.074  0.076731  0.297278 -0.1786618  -110.570    -5.264  
-201226 59209.00 I  0.075986 0.000025  0.297953 0.000018  I-0.1785028 0.0000076 -0.2137 0.0050  I  -110.324    0.112    -5.248    0.181  0.076029  0.297933 -0.1785155  -110.588    -5.069  
-201227 59210.00 I  0.075021 0.000043  0.298714 0.000042  I-0.1782078 0.0000059 -0.3719 0.0045  I  -110.270    0.322    -5.191    0.160  0.075042  0.298659 -0.1782196  -110.593    -4.992  
-201228 59211.00 I  0.073953 0.000045  0.299954 0.000049  I-0.1777715 0.0000050 -0.4925 0.0038  I  -110.287    0.322    -5.339    0.160  0.074002  0.299890 -0.1777873  -110.681    -5.121  
-201229 59212.00 I  0.072644 0.000047  0.301496 0.000049  I-0.1772387 0.0000049 -0.5652 0.0035  I  -110.331    0.322    -5.616    0.160  0.072652  0.301612 -0.1772435  -110.800    -5.378  
-201230 59213.00 I  0.071189 0.000048  0.302560 0.000049  I-0.1766424 0.0000049 -0.6338 0.0036  I  -110.229    0.322    -5.859    0.160  0.071166  0.302626 -0.1766471  -110.575    -5.713  
-201231 59214.00 I  0.069768 0.000048  0.303113 0.000048  I-0.1759809 0.0000053 -0.6729 0.0037  I  -109.891    0.322    -5.959    0.160  0.069727  0.303062 -0.1760031  -110.137    -5.856  
-21 1 1 59215.00 I  0.068690 0.000048  0.304051 0.000048  I-0.1753340 0.0000055 -0.5999 0.0039  I  -109.393    0.322    -6.022    0.160  0.068654  0.303977 -0.1753760  -109.613    -5.841  
-21 1 2 59216.00 I  0.067679 0.000023  0.305442 0.000027  I-0.1748118 0.0000056 -0.4347 0.0043  I  -109.009    0.322    -5.936    0.160  0.067783  0.305455 -0.1748394  -109.207    -5.801  
-21 1 3 59217.00 I  0.066045 0.000027  0.306734 0.000016  I-0.1744728 0.0000065 -0.2448 0.0043  I  -108.783    0.413    -5.883    0.064  0.066068  0.306714 -0.1744761  -108.905    -5.788  
-21 1 4 59218.00 I  0.063870 0.000024  0.307763 0.000015  I-0.1743263 0.0000066 -0.0425 0.0047  I  -108.655    0.413    -5.865    0.064  0.063906  0.307809 -0.1743246  -108.696    -5.815  
-21 1 5 59219.00 I  0.061815 0.000023  0.308644 0.000017  I-0.1743799 0.0000069  0.1361 0.0047  I  -108.589    0.413    -5.821    0.064  0.061685  0.308623 -0.1743819  -108.543    -5.819  
-21 1 6 59220.00 I  0.060433 0.000026  0.309508 0.000021  I-0.1745738 0.0000066  0.2408 0.0047  I  -108.656    0.413    -5.700    0.064  0.060391  0.309503 -0.1746023  -108.462    -5.682  
-21 1 7 59221.00 I  0.059583 0.000028  0.310269 0.000025  I-0.1748355 0.0000064  0.2677 0.0046  I  -108.937    0.413    -5.516    0.064  0.059466  0.310304 -0.1748751  -108.581    -5.464  
-21 1 8 59222.00 I  0.058948 0.000030  0.311093 0.000027  I-0.1750599 0.0000065  0.1466 0.0047  I  -109.389    0.413    -5.362    0.064  0.059005  0.311054 -0.1750757  -108.877    -5.271  
-21 1 9 59223.00 I  0.058322 0.000025  0.311980 0.000025  I-0.1750871 0.0000069 -0.0995 0.0036  I  -109.834    0.322    -5.324    0.160  0.058270  0.311975 -0.1750823  -109.379    -5.254  
-21 110 59224.00 I  0.057967 0.000028  0.313028 0.000035  I-0.1748670 0.0000029 -0.3275 0.0037  I  -110.076    0.444    -5.397    0.164  0.058057  0.313002 -0.1748654  -109.768    -5.367  
-21 111 59225.00 I  0.057559 0.000029  0.314047 0.000035  I-0.1744634 0.0000027 -0.4616 0.0020  I  -110.037    0.444    -5.486    0.164  0.057636  0.314178 -0.1744765  -109.894    -5.482  
-21 112 59226.00 I  0.056937 0.000026  0.314674 0.000035  I-0.1739663 0.0000027 -0.5282 0.0024  I  -109.788    0.444    -5.528    0.164  0.057033  0.314438 -0.1739724  -109.829    -5.535  
-21 113 59227.00 I  0.056041 0.000028  0.315406 0.000034  I-0.1734174 0.0000040 -0.5635 0.0025  I  -109.115    0.926    -5.837    0.104  0.056028  0.315487 -0.1734272  -109.447    -5.630  
-21 114 59228.00 I  0.054983 0.000026  0.316091 0.000033  I-0.1728842 0.0000041 -0.4640 0.0029  I  -108.891    0.926    -5.894    0.104  0.054873  0.316051 -0.1729081  -108.989    -5.826  
-21 115 59229.00 I  0.054316 0.000024  0.316879 0.000035  I-0.1724694 0.0000042 -0.4245 0.0041  I  -108.680    0.926    -6.020    0.104  0.054335  0.316875 -0.1724606  -108.538    -6.095  
-21 116 59230.00 I  0.053770 0.000020  0.317807 0.000026  I-0.1720402 0.0000070 -0.3701 0.0041  I  -108.544    0.926    -6.084    0.104  0.053758  0.317833 -0.1721004  -108.364    -6.182  
-21 117 59231.00 I  0.053040 0.000023  0.318727 0.000025  I-0.1717660 0.0000071 -0.2053 0.0050  I  -108.570    0.783    -5.998    0.150  0.052962  0.318726 -0.1718081  -108.435    -6.070  
-21 118 59232.00 I  0.052519 0.000023  0.319449 0.000023  I-0.1715857 0.0000072 -0.1721 0.0060  I  -108.779    0.783    -5.819    0.150  0.052474  0.319502 -0.1715790  -108.695    -5.858  
-21 119 59233.00 I  0.052578 0.000020  0.320029 0.000019  I-0.1714164 0.0000096 -0.1550 0.0051  I  -109.085    0.544    -5.684    0.191  0.052506  0.319950 -0.1714126  -109.065    -5.679  
-21 120 59234.00 I  0.052771 0.000030  0.320923 0.000021  I-0.1712735 0.0000073 -0.1446 0.0060  I  -109.356    0.568    -5.642    0.154  0.052837  0.320909 -0.1712427  -109.276    -5.677  
-21 121 59235.00 I  0.052579 0.000030  0.321981 0.000019  I-0.1710897 0.0000073 -0.2468 0.0050  I  -109.497    0.568    -5.615    0.154  0.052498  0.321943 -0.1710484  -109.337    -5.704  
-21 122 59236.00 I  0.052404 0.000030  0.323093 0.000019  I-0.1707958 0.0000068 -0.3015 0.0047  I  -109.484    0.626    -5.582    0.027  0.052370  0.323115 -0.1707975  -109.260    -5.651  
-21 123 59237.00 I  0.052364 0.000029  0.324263 0.000018  I-0.1704792 0.0000059 -0.3788 0.0038  I  -109.372    0.626    -5.426    0.027  0.052397  0.324238 -0.1704758  -109.170    -5.507  
-21 124 59238.00 I  0.051875 0.000037  0.325653 0.000026  I-0.1700095 0.0000032 -0.5423 0.0034  I  -109.268    0.616    -5.367    0.100  0.051888  0.325635 -0.1700327  -109.121    -5.441  
-21 125 59239.00 I  0.051012 0.000036  0.327157 0.000026  I-0.1694151 0.0000032 -0.6442 0.0025  I  -109.235    0.616    -5.517    0.100  0.050946  0.327158 -0.1694247  -109.156    -5.579  
-21 126 59240.00 I  0.050368 0.000028  0.328701 0.000023  I-0.1687202 0.0000039 -0.7486 0.0026  I  -109.262    0.614    -5.810    0.117  0.050305  0.328651 -0.1687165  -109.246    -5.884  
-21 127 59241.00 I  0.050035 0.000030  0.330501 0.000024  I-0.1679551 0.0000041 -0.7412 0.0030  I  -109.142    0.734    -6.182    0.094  0.050009  0.330496 -0.1680026  -109.141    -6.231  
-21 128 59242.00 I  0.049907 0.000030  0.332424 0.000023  I-0.1673088 0.0000046 -0.5208 0.0031  I  -108.860    0.734    -6.397    0.094  0.049854  0.332424 -0.1673675  -108.815    -6.433  
-21 129 59243.00 I  0.049883 0.000030  0.334344 0.000023  I-0.1669113 0.0000047 -0.3069 0.0037  I  -108.454    0.734    -6.400    0.094  0.049925  0.334359 -0.1669073  -108.303    -6.429  
-21 130 59244.00 I  0.049606 0.000019  0.336136 0.000014  I-0.1666818 0.0000057 -0.1325 0.0035  I  -108.090    0.998    -6.271    0.025  0.049593  0.336126 -0.1666565  -107.964    -6.280  
-21 131 59245.00 I  0.049361 0.000021  0.337916 0.000014  I-0.1666882 0.0000051  0.1676 0.0038  I  -107.928    0.469    -6.151    0.029  0.049315  0.337874 -0.1666887  -107.846    -6.140  
-21 2 1 59246.00 I  0.049428 0.000021  0.339850 0.000014  I-0.1670133 0.0000050  0.4566 0.0037  I  -108.028    0.469    -6.129    0.029  0.049421  0.339866 -0.1670204  -107.967    -6.108  
-21 2 2 59247.00 I  0.049457 0.000017  0.341664 0.000012  I-0.1675605 0.0000054  0.6229 0.0034  I  -108.337    0.269    -6.177    0.031  0.049490  0.341692 -0.1675614  -108.292    -6.165  
-21 2 3 59248.00 I  0.049299 0.000021  0.343143 0.000016  I-0.1682174 0.0000047  0.6639 0.0036  I  -108.735    0.288    -6.205    0.033  0.049274  0.343178 -0.1681920  -108.630    -6.177  
-21 2 4 59249.00 I  0.049231 0.000021  0.344375 0.000016  I-0.1688356 0.0000047  0.5466 0.0033  I  -109.131    0.288    -6.153    0.033  0.049231  0.344351 -0.1688000  -108.983    -6.111  
-21 2 5 59250.00 I  0.049258 0.000021  0.345652 0.000016  I-0.1692841 0.0000046  0.3498 0.0033  I  -109.235    0.504    -5.972    0.047  0.049262  0.345628 -0.1692802  -109.304    -6.001  
-21 2 6 59251.00 I  0.049170 0.000017  0.346997 0.000014  I-0.1695316 0.0000047  0.1421 0.0029  I  -109.439    0.504    -5.910    0.047  0.049156  0.346983 -0.1696139  -109.483    -5.921  
-21 2 7 59252.00 I  0.049118 0.000021  0.348391 0.000015  I-0.1695770 0.0000035 -0.0395 0.0029  I  -109.437    0.480    -5.906    0.197  0.049075  0.348358 -0.1696850  -109.454    -5.901  
-21 2 8 59253.00 I  0.049360 0.000020  0.349883 0.000014  I-0.1694781 0.0000033 -0.1447 0.0025  I  -109.223    0.480    -5.954    0.197  0.049311  0.349885 -0.1694924  -109.221    -5.926  
-21 2 9 59254.00 I  0.049920 0.000018  0.351331 0.000010  I-0.1693298 0.0000037 -0.1234 0.0026  I  -108.917    0.474    -6.005    0.220  0.049922  0.351343 -0.1693373  -108.874    -5.989  
-21 210 59255.00 I  0.050595 0.000023  0.352614 0.000025  I-0.1692518 0.0000041 -0.0406 0.0028  I  -108.558    0.636    -6.185    0.159  0.050607  0.352626 -0.1692436  -108.510    -6.178  
-21 211 59256.00 I  0.051149 0.000023  0.353812 0.000028  I-0.1692585 0.0000041  0.0718 0.0029  I  -108.331    0.636    -6.405    0.159  0.051207  0.353801 -0.1692657  -108.257    -6.433  
-21 212 59257.00 I  0.051354 0.000025  0.354907 0.000029  I-0.1694104 0.0000040  0.2292 0.0033  I  -108.232    0.636    -6.604    0.159  0.051383  0.354941 -0.1694090  -108.111    -6.679  
-21 213 59258.00 I  0.051525 0.000021  0.355733 0.000029  I-0.1697177 0.0000051  0.3890 0.0034  I  -108.195    0.783    -6.705    0.037  0.051474  0.355706 -0.1697045  -108.084    -6.767  
-21 214 59259.00 I  0.051834 0.000021  0.356789 0.000029  I-0.1701828 0.0000054  0.5321 0.0036  I  -108.199    0.783    -6.693    0.037  0.051922  0.356756 -0.1701305  -108.104    -6.728  
-21 215 59260.00 I  0.051650 0.000038  0.358115 0.000029  I-0.1707346 0.0000052  0.5334 0.0039  I  -108.285    0.735    -6.635    0.126  0.051716  0.358143 -0.1706473  -108.193    -6.652  
-21 216 59261.00 I  0.050957 0.000035  0.359272 0.000019  I-0.1712267 0.0000056  0.4662 0.0037  I  -108.517    0.707    -6.519    0.169  0.050949  0.359283 -0.1711965  -108.366    -6.610  
-21 217 59262.00 I  0.050404 0.000044  0.360299 0.000023  I-0.1716582 0.0000054  0.3728 0.0039  I  -108.657    0.664    -6.566    0.192  0.050326  0.360338 -0.1716669  -108.536    -6.606  
-21 218 59263.00 I  0.050428 0.000044  0.361154 0.000022  I-0.1719340 0.0000054  0.1645 0.0037  I  -108.681    0.664    -6.596    0.192  0.050378  0.361154 -0.1719511  -108.669    -6.586  
-21 219 59264.00 I  0.050877 0.000044  0.362025 0.000023  I-0.1719960 0.0000052 -0.0174 0.0038  I  -108.591    0.664    -6.583    0.192  0.050885  0.361987 -0.1720228  -108.704    -6.521  
-21 220 59265.00 I  0.051397 0.000044  0.363041 0.000022  I-0.1718953 0.0000054 -0.2112 0.0035  I  -108.482    0.664    -6.576    0.192  0.051501  0.363070 -0.1719007  -108.603    -6.534  
-21 221 59266.00 I  0.051363 0.000034  0.363875 0.000026  I-0.1715594 0.0000047 -0.4477 0.0035  I  -108.412    0.560    -6.654    0.153  0.051463  0.363914 -0.1715820  -108.490    -6.656  
-21 222 59267.00 I  0.050693 0.000034  0.364572 0.000026  I-0.1710417 0.0000044 -0.5587 0.0032  I  -108.357    0.560    -6.853    0.153  0.050700  0.364562 -0.1710795  -108.387    -6.899  
-21 223 59268.00 I  0.049876 0.000022  0.365243 0.000019  I-0.1704541 0.0000044 -0.6334 0.0031  I  -108.311    0.558    -7.204    0.037  0.049836  0.365309 -0.1704677  -108.274    -7.237  
-21 224 59269.00 I  0.049504 0.000024  0.365612 0.000033  I-0.1698157 0.0000045 -0.5856 0.0032  I  -108.284    0.512    -7.501    0.056  0.049396  0.365588 -0.1698548  -108.271    -7.557  
-21 225 59270.00 I  0.049816 0.000024  0.366112 0.000033  I-0.1693325 0.0000047 -0.3888 0.0032  I  -108.245    0.512    -7.737    0.056  0.049801  0.366059 -0.1693475  -108.285    -7.804  
-21 226 59271.00 I  0.050257 0.000024  0.367137 0.000033  I-0.1690519 0.0000046 -0.1504 0.0042  I  -108.047    0.512    -7.815    0.056  0.050306  0.367069 -0.1690477  -108.145    -7.894  
-21 227 59272.00 I  0.050421 0.000019  0.368561 0.000029  I-0.1690420 0.0000069  0.1191 0.0034  I  -107.624    0.400    -7.688    0.073  0.050431  0.368528 -0.1690351  -107.687    -7.757  
-21 228 59273.00 I  0.050493 0.000030  0.370230 0.000030  I-0.1692889 0.0000051  0.3850 0.0042  I  -107.191    0.498    -7.448    0.051  0.050498  0.370227 -0.1693081  -107.188    -7.498  
-21 3 1 59274.00 I  0.050627 0.000030  0.371996 0.000030  I-0.1697917 0.0000048  0.5899 0.0034  I  -107.089    0.498    -7.289    0.051  0.050616  0.371982 -0.1697877  -107.024    -7.321  
-21 3 2 59275.00 I  0.050674 0.000028  0.373729 0.000013  I-0.1704083 0.0000045  0.6136 0.0037  I  -107.399    0.554    -7.314    0.025  0.050706  0.373771 -0.1703934  -107.298    -7.344  
-21 3 3 59276.00 I  0.050673 0.000032  0.375234 0.000021  I-0.1710068 0.0000057  0.6009 0.0036  I  -107.951    0.513    -7.500    0.040  0.050584  0.375262 -0.1710261  -107.867    -7.504  
-21 3 4 59277.00 I  0.051149 0.000032  0.376535 0.000021  I-0.1715739 0.0000055  0.4797 0.0041  I  -108.369    0.513    -7.639    0.040  0.051059  0.376549 -0.1715540  -108.333    -7.617  
-21 3 5 59278.00 I  0.052206 0.000032  0.377906 0.000021  I-0.1719077 0.0000058  0.1832 0.0049  I  -108.517    0.513    -7.643    0.040  0.052201  0.377870 -0.1718838  -108.535    -7.596  
-21 3 6 59279.00 I  0.053359 0.000021  0.379381 0.000018  I-0.1719593 0.0000082 -0.0562 0.0044  I  -108.460    0.388    -7.567    0.070  0.053360  0.379379 -0.1719881  -108.484    -7.535  
-21 3 7 59280.00 I  0.054611 0.000020  0.380848 0.000021  I-0.1718305 0.0000066 -0.1902 0.0052  I  -108.297    0.520    -7.505    0.067  0.054561  0.380833 -0.1718731  -108.315    -7.503  
-21 3 8 59281.00 I  0.056160 0.000020  0.382347 0.000020  I-0.1715956 0.0000065 -0.2743 0.0045  I  -108.045    0.520    -7.514    0.067  0.056191  0.382351 -0.1716080  -108.062    -7.541  
-21 3 9 59282.00 I  0.057603 0.000014  0.383893 0.000012  I-0.1713142 0.0000061 -0.2615 0.0047  I  -107.681    0.561    -7.620    0.066  0.057662  0.383909 -0.1713243  -107.722    -7.670  
-21 310 59283.00 I  0.058708 0.000022  0.385232 0.000024  I-0.1711055 0.0000067 -0.1501 0.0045  I  -107.335    0.555    -7.796    0.113  0.058750  0.385265 -0.1710993  -107.388    -7.839  
-21 311 59284.00 I  0.059636 0.000022  0.386403 0.000024  I-0.1710208 0.0000066 -0.0185 0.0047  I  -107.123    0.555    -7.985    0.113  0.059621  0.386346 -0.1710012  -107.198    -8.012  
-21 312 59285.00 I  0.060591 0.000022  0.387770 0.000024  I-0.1710743 0.0000066  0.1304 0.0054  I  -107.103    0.555    -8.082    0.113  0.060542  0.387744 -0.1710599  -107.204    -8.099  
-21 313 59286.00 I  0.061753 0.000021  0.389366 0.000023  I-0.1712815 0.0000085  0.2788 0.0045  I  -107.174    0.547    -8.025    0.147  0.061723  0.389349 -0.1712387  -107.275    -8.029  
-21 314 59287.00 I  0.063042 0.000027  0.391002 0.000023  I-0.1716048 0.0000061  0.3458 0.0052  I  -107.210    0.700    -7.872    0.112  0.063046  0.391028 -0.1715574  -107.295    -7.866  
-21 315 59288.00 I  0.064316 0.000028  0.392544 0.000023  I-0.1719443 0.0000061  0.3263 0.0040  I  -107.195    0.700    -7.758    0.112  0.064331  0.392504 -0.1719515  -107.259    -7.749  
-21 316 59289.00 I  0.065268 0.000023  0.394216 0.000012  I-0.1722294 0.0000052  0.2227 0.0040  I  -107.186    0.796    -7.770    0.068  0.065375  0.394218 -0.1722335  -107.205    -7.755  
-21 317 59290.00 I  0.065643 0.000032  0.395924 0.000023  I-0.1723712 0.0000053  0.0636 0.0037  I  -107.188    0.689    -7.868    0.054  0.065657  0.395943 -0.1724026  -107.211    -7.870  
-21 318 59291.00 I  0.065875 0.000032  0.397446 0.000023  I-0.1723768 0.0000053 -0.0351 0.0038  I  -107.149    0.689    -7.959    0.054  0.065853  0.397460 -0.1724204  -107.178    -7.981  
-21 319 59292.00 I  0.066215 0.000033  0.398951 0.000023  I-0.1722852 0.0000055 -0.1813 0.0044  I  -107.086    0.689    -8.020    0.054  0.066235  0.398938 -0.1722871  -107.117    -8.061  
-21 320 59293.00 I  0.066658 0.000028  0.400397 0.000025  I-0.1720139 0.0000069 -0.3283 0.0045  I  -107.068    0.577    -8.112    0.038  0.066580  0.400421 -0.1720284  -107.085    -8.161  
-21 321 59294.00 I  0.067553 0.000026  0.401827 0.000026  I-0.1716685 0.0000072 -0.3557 0.0050  I  -107.066    0.577    -8.273    0.038  0.067507  0.401767 -0.1716900  -107.075    -8.325  
-21 322 59295.00 I  0.068766 0.000031  0.403489 0.000036  I-0.1713111 0.0000071 -0.3572 0.0053  I  -106.926    0.589    -8.452    0.082  0.068766  0.403525 -0.1713132  -106.939    -8.503  
-21 323 59296.00 I  0.070031 0.000021  0.405080 0.000031  I-0.1709631 0.0000079 -0.3316 0.0043  I  -106.625    0.593    -8.520    0.104  0.070017  0.405095 -0.1709575  -106.635    -8.632  
-21 324 59297.00 I  0.071465 0.000025  0.406503 0.000040  I-0.1706728 0.0000048 -0.2313 0.0046  I  -106.321    0.624    -8.689    0.073  0.071509  0.406504 -0.1706787  -106.371    -8.750  
-21 325 59298.00 I  0.072760 0.000024  0.407850 0.000040  I-0.1705245 0.0000047 -0.0591 0.0034  I  -106.229    0.624    -8.931    0.073  0.072812  0.407873 -0.1705313  -106.284    -8.978  
-21 326 59299.00 I  0.073771 0.000024  0.408998 0.000039  I-0.1705845 0.0000048  0.2029 0.0034  I  -106.181    0.651    -9.218    0.013  0.073728  0.409056 -0.1705938  -106.226    -9.237  
-21 327 59300.00 I  0.074996 0.000024  0.409612 0.000038  I-0.1709260 0.0000048  0.4519 0.0030  I  -105.829    0.651    -9.270    0.013  0.074948  0.409668 -0.1709185  -105.910    -9.285  
-21 328 59301.00 I  0.076576 0.000020  0.409850 0.000029  I-0.1714805 0.0000035  0.6775 0.0029  I  -105.352    0.696    -9.043    0.042  0.076573  0.409823 -0.1714942  -105.462    -9.044  
-21 329 59302.00 I  0.078198 0.000020  0.410126 0.000028  I-0.1722523 0.0000032  0.8170 0.0039  I  -105.225    0.696    -8.743    0.042  0.078236  0.410129 -0.1722454  -105.357    -8.732  
-21 330 59303.00 I  0.079555 0.000028  0.410497 0.000019  I-0.1730457 0.0000070  0.7502 0.0039  I  -105.650    0.957    -8.667    0.060  0.079581  0.410456 -0.1730409  -105.788    -8.649  
-21 331 59304.00 I  0.080666 0.000028  0.411075 0.000018  I-0.1737247 0.0000071  0.5994 0.0049  I  -106.271    0.957    -8.848    0.060  0.080692  0.411065 -0.1737315  -106.343    -8.857  
-21 4 1 59305.00 I  0.081550 0.000028  0.411764 0.000019  I-0.1742217 0.0000068  0.3801 0.0048  I  -106.615    0.957    -9.053    0.060  0.081597  0.411745 -0.1742201  -106.573    -9.100  
-21 4 2 59306.00 I  0.082249 0.000028  0.412536 0.000019  I-0.1744835 0.0000066  0.1567 0.0048  I  -107.388    0.322    -8.989    0.160  0.082266  0.412527 -0.1744884  -106.526    -9.134  
-21 4 3 59307.00 I  0.082889 0.000027  0.413357 0.000019  I-0.1745525 0.0000069 -0.0144 0.0049  I  -107.155    0.322    -8.933    0.160  0.082863  0.413394 -0.1745594  -106.357    -9.054  
-21 4 4 59308.00 I  0.083738 0.000027  0.413939 0.000019  I-0.1744769 0.0000073 -0.1188 0.0040  I  -106.932    0.322    -8.908    0.160  0.083694  0.413955 -0.1744710  -106.265    -8.993  
-21 4 5 59309.00 I  0.084847 0.000015  0.414545 0.000017  I-0.1743709 0.0000039 -0.0553 0.0041  I  -106.781    0.394    -8.949    0.136  0.084866  0.414476 -0.1744009  -106.290    -8.990  
-21 4 6 59310.00 I  0.085827 0.000015  0.415612 0.000018  I-0.1744068 0.0000039  0.1295 0.0031  I  -106.586    0.394    -9.030    0.136  0.085863  0.415604 -0.1744328  -106.306    -9.021  
-21 4 7 59311.00 I  0.086622 0.000021  0.416791 0.000027  I-0.1746008 0.0000048  0.2270 0.0032  I  -106.259    0.567    -9.134    0.092  0.086636  0.416842 -0.1745974  -106.207    -9.070  
-21 4 8 59312.00 I  0.087296 0.000021  0.417766 0.000027  I-0.1748658 0.0000050  0.3396 0.0035  I  -105.883    0.567    -9.222    0.092  0.087374  0.417758 -0.1748862  -105.886    -9.192  
-21 4 9 59313.00 I  0.087570 0.000020  0.418809 0.000026  I-0.1752818 0.0000052  0.4574 0.0036  I  -105.647    0.567    -9.205    0.092  0.087621  0.418801 -0.1752874  -105.640    -9.234  
-21 410 59314.00 I  0.087454 0.000020  0.419882 0.000025  I-0.1757555 0.0000053  0.4997 0.0044  I  -105.632    0.567    -9.015    0.092  0.087511  0.419908 -0.1757729  -105.648    -9.045  
-21 411 59315.00 I  0.087102 0.000030  0.420737 0.000030  I-0.1762871 0.0000071  0.5598 0.0045  I  -105.744    0.671    -8.731    0.020  0.087081  0.420785 -0.1762939  -105.773    -8.744  
-21 412 59316.00 I  0.086813 0.000034  0.421361 0.000031  I-0.1768301 0.0000072  0.4850 0.0087  I  -105.837    0.671    -8.554    0.020  0.086768  0.421358 -0.1767986  -105.846    -8.552  
-21 413 59317.00 I  0.086943 0.000032  0.421880 0.000027  I-0.1772505 0.0000159  0.3905 0.0048  I  -105.850    0.832    -8.619    0.038  0.086839  0.421892 -0.1772455  -105.810    -8.603  
-21 414 59318.00 I  0.087728 0.000036  0.422443 0.000036  I-0.1776168 0.0000064  0.3131 0.0086  I  -105.795    0.646    -8.863    0.039  0.087692  0.422398 -0.1776055  -105.761    -8.851  
-21 415 59319.00 I  0.088781 0.000037  0.423227 0.000036  I-0.1778594 0.0000065  0.1837 0.0046  I  -105.720    0.646    -9.116    0.039  0.088768  0.423267 -0.1778557  -105.691    -9.111  
-21 416 59320.00 I  0.090124 0.000037  0.423823 0.000036  I-0.1779915 0.0000066  0.0760 0.0046  I  -105.716    0.646    -9.299    0.039  0.089996  0.423845 -0.1779907  -105.670    -9.299  
-21 417 59321.00 I  0.092133 0.000026  0.424366 0.000030  I-0.1780187 0.0000066 -0.0099 0.0039  I  -105.864    0.612    -9.475    0.039  0.092158  0.424284 -0.1780250  -105.805    -9.475  
-21 418 59322.00 I  0.094196 0.000026  0.425244 0.000033  I-0.1779752 0.0000043 -0.0851 0.0039  I  -106.075    0.380    -9.693    0.060  0.094246  0.425257 -0.1779868  -106.010    -9.693  
-21 419 59323.00 I  0.095895 0.000024  0.426267 0.000031  I-0.1778769 0.0000043 -0.0749 0.0033  I  -106.085    0.380    -9.876    0.060  0.095947  0.426181 -0.1779103  -106.040    -9.876  
-21 420 59324.00 I  0.097225 0.000017  0.427573 0.000020  I-0.1778450 0.0000049 -0.0060 0.0030  I  -105.785    0.285    -9.929    0.069  0.097266  0.427588 -0.1778571  -105.762    -9.917  
-21 421 59325.00 I  0.098224 0.000024  0.428912 0.000019  I-0.1778698 0.0000042  0.0776 0.0032  I  -105.261    0.557    -9.870    0.083  0.098245  0.428908 -0.1779160  -105.268    -9.880  
-21 422 59326.00 I  0.098991 0.000024  0.430096 0.000019  I-0.1780571 0.0000041  0.3321 0.0029  I  -105.021    0.557    -9.926    0.083  0.099005  0.430149 -0.1781298  -105.013    -9.959  
-21 423 59327.00 I  0.099556 0.000024  0.431144 0.000019  I-0.1785260 0.0000040  0.5627 0.0031  I  -105.023    0.614   -10.165    0.093  0.099573  0.431096 -0.1785406  -105.001   -10.212  
-21 424 59328.00 I  0.099852 0.000020  0.432027 0.000008  I-0.1791579 0.0000047  0.7196 0.0030  I  -104.955    0.614   -10.291    0.093  0.099809  0.432023 -0.1791390  -104.985   -10.413  
-21 425 59329.00 I  0.100027 0.000021  0.432773 0.000021  I-0.1799638 0.0000044  0.8722 0.0033  I  -104.770    0.614   -10.076    0.093  0.100034  0.432771 -0.1799364  -104.882   -10.281  
-21 426 59330.00 I  0.100443 0.000020  0.433376 0.000022  I-0.1808928 0.0000045  0.9964 0.0043  I  -104.878    0.614    -9.633    0.093  0.100355  0.433380 -0.1809123  -105.064    -9.917  
-21 427 59331.00 I  0.101372 0.000009  0.433875 0.000023  I-0.1818985 0.0000073  0.9465 0.0033  I  -105.482    0.322    -9.345    0.160  0.101324  0.433851 -0.1819026  -105.732    -9.702  
-21 428 59332.00 I  0.102663 0.000020  0.434401 0.000024  I-0.1827070 0.0000047  0.6604 0.0043  I  -106.178    0.885    -9.386    0.078  0.102654  0.434414 -0.1826964  -106.366    -9.670  
-21 429 59333.00 I  0.104017 0.000020  0.434850 0.000025  I-0.1832026 0.0000046  0.3244 0.0034  I  -106.422    0.885    -9.562    0.078  0.104008  0.434868 -0.1831982  -106.503    -9.731  
-21 430 59334.00 I  0.105400 0.000020  0.435243 0.000025  I-0.1833712 0.0000050  0.0346 0.0035  I  -106.116    0.885    -9.640    0.078  0.105404  0.435218 -0.1833833  -106.086    -9.707  
-21 5 1 59335.00 I  0.106807 0.000020  0.435778 0.000015  I-0.1833060 0.0000052 -0.1525 0.0033  I  -105.690    0.885    -9.740    0.078  0.106820  0.435779 -0.1833089  -105.624    -9.755  
-21 5 2 59336.00 I  0.108216 0.000033  0.436473 0.000031  I-0.1830888 0.0000043 -0.2717 0.0033  I  -105.419    0.693    -9.915    0.063  0.108188  0.436419 -0.1830909  -105.392    -9.936  
-21 5 3 59337.00 I  0.109805 0.000034  0.437431 0.000031  I-0.1827908 0.0000042 -0.3064 0.0031  I  -105.431    0.693   -10.107    0.063  0.109767  0.437441 -0.1827909  -105.435   -10.113  
-21 5 4 59338.00 I  0.111567 0.000031  0.438467 0.000030  I-0.1825196 0.0000045 -0.2103 0.0030  I  -105.603    0.511   -10.177    0.044  0.111592  0.438462 -0.1825243  -105.659   -10.174  
-21 5 5 59339.00 I  0.113353 0.000036  0.439376 0.000032  I-0.1823883 0.0000043 -0.0599 0.0030  I  -105.693    0.506   -10.108    0.074  0.113313  0.439364 -0.1823978  -105.759   -10.107  
-21 5 6 59340.00 I  0.115275 0.000036  0.440338 0.000031  I-0.1823976 0.0000039  0.0837 0.0030  I  -105.582    0.506    -9.986    0.074  0.115279  0.440309 -0.1824200  -105.659    -9.997  
-21 5 7 59341.00 I  0.117107 0.000036  0.441493 0.000032  I-0.1825578 0.0000042  0.2335 0.0033  I  -105.418    0.506    -9.835    0.074  0.117172  0.441478 -0.1825670  -105.509    -9.864  
-21 5 8 59342.00 I  0.118707 0.000025  0.442596 0.000015  I-0.1828233 0.0000054  0.2594 0.0033  I  -105.449    0.485    -9.602    0.106  0.118681  0.442646 -0.1827886  -105.519    -9.632  
-21 5 9 59343.00 I  0.120399 0.000028  0.443446 0.000022  I-0.1830472 0.0000052  0.1970 0.0038  I  -105.726    0.478    -9.312    0.104  0.120432  0.443435 -0.1830318  -105.761    -9.338  
-21 510 59344.00 I  0.121972 0.000027  0.444238 0.000022  I-0.1832221 0.0000053  0.1489 0.0046  I  -106.057    0.478    -9.133    0.104  0.122013  0.444253 -0.1832398  -106.060    -9.161  
-21 511 59345.00 I  0.123229 0.000020  0.444891 0.000022  I-0.1833553 0.0000076  0.1317 0.0033  I  -106.262    0.473    -9.228    0.103  0.123229  0.444950 -0.1833696  -106.211    -9.260  
-21 512 59346.00 I  0.124613 0.000032  0.445067 0.000030  I-0.1834401 0.0000040 -0.0216 0.0042  I  -106.177    0.567    -9.553    0.095  0.124570  0.445119 -0.1834050  -106.142    -9.592  
-21 513 59347.00 I  0.126411 0.000032  0.444946 0.000030  I-0.1833065 0.0000037 -0.1915 0.0027  I  -105.999    0.567    -9.895    0.095  0.126398  0.444900 -0.1833166  -105.971    -9.938  
-21 514 59348.00 I  0.128369 0.000032  0.445075 0.000030  I-0.1830974 0.0000037 -0.2405 0.0024  I  -105.893    0.567   -10.094    0.095  0.128393  0.445000 -0.1831001  -105.857   -10.138  
-21 515 59349.00 I  0.130315 0.000030  0.445427 0.000025  I-0.1828253 0.0000032 -0.2903 0.0025  I  -105.967    0.603   -10.185    0.089  0.130276  0.445421 -0.1828031  -105.951   -10.226  
-21 516 59350.00 I  0.132486 0.000031  0.445804 0.000025  I-0.1825352 0.0000034 -0.2851 0.0023  I  -106.176    0.603   -10.277    0.089  0.132466  0.445767 -0.1824802  -106.179   -10.311  
-21 517 59351.00 I  0.134862 0.000030  0.446309 0.000025  I-0.1822580 0.0000034 -0.2712 0.0027  I  -106.307    0.569   -10.370    0.088  0.134899  0.446354 -0.1822601  -106.327   -10.390  
-21 518 59352.00 I  0.137092 0.000016  0.446606 0.000014  I-0.1820292 0.0000043 -0.1480 0.0025  I  -106.224    0.520   -10.362    0.087  0.137096  0.446653 -0.1820734  -106.203   -10.375  
-21 519 59353.00 I  0.139427 0.000024  0.446466 0.000018  I-0.1819725 0.0000036  0.0067 0.0028  I  -105.845    0.634   -10.279    0.175  0.139382  0.446488 -0.1819842  -105.891   -10.264  
-21 520 59354.00 I  0.142025 0.000024  0.446224 0.000017  I-0.1820806 0.0000035  0.2754 0.0025  I  -105.577    0.634   -10.250    0.175  0.142062  0.446194 -0.1821300  -105.602   -10.265  
-21 521 59355.00 I  0.144476 0.000022  0.446098 0.000017  I-0.1825062 0.0000035  0.4926 0.0024  I  -105.539    0.718   -10.417    0.233  0.144518  0.446092 -0.1825058  -105.556   -10.433  
-21 522 59356.00 I  0.146580 0.000021  0.446140 0.000017  I-0.1830292 0.0000033  0.5998 0.0024  I  -105.826    0.718   -10.483    0.233  0.146638  0.446087 -0.1830591  -105.780   -10.527  
-21 523 59357.00 I  0.148355 0.000020  0.446242 0.000016  I-0.1837147 0.0000033  0.7335 0.0020  I  -106.169    0.718   -10.301    0.233  0.148357  0.446319 -0.1837359  -106.114   -10.345  
-21 524 59358.00 I  0.150036 0.000027  0.446009 0.000016  I-0.1844360 0.0000021  0.6865 0.0019  I  -106.735    0.421    -9.901    0.173  0.150055  0.446007 -0.1844377  -106.686    -9.942  
-21 525 59359.00 I  0.151660 0.000021  0.445543 0.000012  I-0.1850412 0.0000018  0.5000 0.0020  I  -107.568    0.330    -9.591    0.114  0.151671  0.445578 -0.1850358  -107.551    -9.625  
-21 526 59360.00 I  0.153129 0.000024  0.445153 0.000017  I-0.1854163 0.0000034  0.2543 0.0019  I  -108.292    0.350    -9.566    0.125  0.153177  0.445002 -0.1854186  -108.338    -9.587  
-21 527 59361.00 I  0.154588 0.000025  0.444717 0.000019  I-0.1855446 0.0000034 -0.0069 0.0024  I  -108.453    0.350    -9.691    0.125  0.154610  0.444641 -0.1855433  -108.444    -9.735  
-21 528 59362.00 I  0.156107 0.000025  0.444065 0.000021  I-0.1854044 0.0000035 -0.2624 0.0024  I  -108.034    0.350    -9.790    0.125  0.156083  0.444149 -0.1854061  -107.950    -9.866  
-21 529 59363.00 I  0.157801 0.000027  0.443394 0.000021  I-0.1850498 0.0000035 -0.4280 0.0039  I  -107.392    0.350    -9.920    0.125  0.157787  0.443296 -0.1850586  -107.322    -9.999  
-21 530 59364.00 I  0.159436 0.000025  0.443180 0.000025  I-0.1845912 0.0000070 -0.4651 0.0039  I  -106.884    0.585   -10.186    0.168  0.159496  0.443194 -0.1846181  -106.855   -10.257  
-21 531 59365.00 I  0.160789 0.000025  0.443015 0.000025  I-0.1841628 0.0000069 -0.3726 0.0044  I  -106.703    0.585   -10.462    0.168  0.160764  0.443056 -0.1841962  -106.711   -10.524  
-21 6 1 59366.00 I  0.162210 0.000022  0.442551 0.000021  I-0.1838648 0.0000053 -0.2239 0.0046  I  -106.860    0.540   -10.506    0.174  0.162221  0.442541 -0.1838763  -106.911   -10.562  
-21 6 2 59367.00 I  0.163436 0.000027  0.442187 0.000028  I-0.1837072 0.0000060 -0.0987 0.0042  I  -106.913    0.783   -10.298    0.152  0.163505  0.442197 -0.1837088  -107.189   -10.310  
-21 6 3 59368.00 I  0.164296 0.000028  0.441784 0.000026  I-0.1836624 0.0000064  0.0115 0.0044  I  -107.152    0.783    -9.973    0.152  0.164269  0.441835 -0.1836734  -107.307    -9.973  
-21 6 4 59369.00 I  0.165289 0.000026  0.441041 0.000026  I-0.1837099 0.0000065  0.0609 0.0049  I  -107.212    0.783    -9.733    0.152  0.165264  0.441101 -0.1837182  -107.243    -9.722  
-21 6 5 59370.00 I  0.166464 0.000022  0.439944 0.000022  I-0.1837431 0.0000075 -0.0130 0.0045  I  -107.329    0.783    -9.567    0.152  0.166494  0.439959 -0.1837435  -107.338    -9.564  
-21 6 6 59371.00 I  0.167460 0.000025  0.438784 0.000027  I-0.1836679 0.0000062 -0.1348 0.0049  I  -107.690    0.682    -9.409    0.147  0.167443  0.438760 -0.1837213  -107.712    -9.420  
-21 6 7 59372.00 I  0.168521 0.000025  0.437809 0.000027  I-0.1834729 0.0000062 -0.2582 0.0039  I  -108.186    0.682    -9.312    0.147  0.168452  0.437773 -0.1835146  -108.222    -9.335  
-21 6 8 59373.00 I  0.169998 0.000020  0.437051 0.000025  I-0.1831283 0.0000047 -0.4510 0.0039  I  -108.567    0.528    -9.408    0.133  0.169988  0.437038 -0.1831307  -108.616    -9.447  
-21 6 9 59374.00 I  0.171619 0.000019  0.436495 0.000025  I-0.1825775 0.0000047 -0.6239 0.0033  I  -108.705    0.528    -9.726    0.133  0.171662  0.436466 -0.1825961  -108.746    -9.756  
-21 610 59375.00 I  0.173021 0.000018  0.436104 0.000025  I-0.1819028 0.0000046 -0.7297 0.0033  I  -108.686    0.528   -10.082    0.133  0.173060  0.436107 -0.1819126  -108.720   -10.098  
-21 611 59376.00 I  0.174263 0.000018  0.435731 0.000026  I-0.1811023 0.0000045 -0.8827 0.0034  I  -108.648    0.528   -10.270    0.133  0.174245  0.435720 -0.1810931  -108.643   -10.282  
-21 612 59377.00 I  0.175426 0.000014  0.435396 0.000021  I-0.1801740 0.0000050 -0.9259 0.0033  I  -108.690    0.500   -10.255    0.125  0.175463  0.435402 -0.1802017  -108.645   -10.266  
-21 613 59378.00 I  0.176481 0.000017  0.435065 0.000026  I-0.1792664 0.0000049 -0.9215 0.0050  I  -108.837    0.576   -10.165    0.119  0.176463  0.435076 -0.1792824  -108.763   -10.171  
-21 614 59379.00 I  0.177520 0.000013  0.434808 0.000020  I-0.1783473 0.0000087 -0.8683 0.0049  I  -109.034    0.755   -10.115    0.109  0.177561  0.434800 -0.1783898  -108.931   -10.112  
-21 615 59380.00 I  0.178426 0.000016  0.434507 0.000020  I-0.1775772 0.0000084 -0.6731 0.0054  I  -109.150    0.755   -10.108    0.109  0.178436  0.434544 -0.1776041  -109.005   -10.092  
-21 616 59381.00 I  0.179178 0.000020  0.433937 0.000023  I-0.1769796 0.0000063 -0.5424 0.0052  I  -109.098    0.588   -10.093    0.194  0.179161  0.433958 -0.1769638  -109.007   -10.090  
-21 617 59382.00 I  0.180091 0.000020  0.433087 0.000022  I-0.1765126 0.0000063 -0.3510 0.0044  I  -108.952    0.588   -10.055    0.194  0.179975  0.433150 -0.1765219  -108.937   -10.073  
-21 618 59383.00 I  0.181590 0.000020  0.432042 0.000023  I-0.1762852 0.0000061 -0.1369 0.0048  I  -108.945    0.517   -10.053    0.237  0.181538  0.431985 -0.1762920  -108.971   -10.051  
-21 619 59384.00 I  0.183451 0.000017  0.431234 0.000019  I-0.1762106 0.0000073 -0.0075 0.0046  I  -109.137    0.517    -9.929    0.237  0.183459  0.431221 -0.1762499  -109.186    -9.941  
-21 620 59385.00 I  0.185268 0.000021  0.430719 0.000030  I-0.1762404 0.0000068  0.0325 0.0050  I  -109.632    0.551    -9.707    0.195  0.185268  0.430690 -0.1762848  -109.672    -9.715  
-21 621 59386.00 I  0.186989 0.000019  0.430322 0.000029  I-0.1762069 0.0000067 -0.1337 0.0059  I  -110.372    0.551    -9.448    0.195  0.187008  0.430371 -0.1762299  -110.397    -9.446  
-21 622 59387.00 I  0.188628 0.000015  0.429675 0.000027  I-0.1759532 0.0000097 -0.3595 0.0042  I  -111.155    0.595    -9.287    0.131  0.188612  0.429729 -0.1759694  -111.169    -9.304  
-21 623 59388.00 I  0.190264 0.000018  0.428664 0.000029  I-0.1754720 0.0000049 -0.6331 0.0054  I  -111.724    0.537    -9.382    0.207  0.190249  0.428692 -0.1754577  -111.740    -9.402  
-21 624 59389.00 I  0.192022 0.000018  0.427526 0.000028  I-0.1746658 0.0000048 -0.9703 0.0034  I  -111.835    0.537    -9.530    0.207  0.191984  0.427561 -0.1746551  -111.870    -9.570  
-21 625 59390.00 I  0.193853 0.000019  0.426262 0.000028  I-0.1735817 0.0000048 -1.1566 0.0029  I  -111.566    0.537    -9.610    0.207  0.193895  0.426260 -0.1736026  -111.627    -9.678  
-21 626 59391.00 I  0.195553 0.000018  0.424981 0.000016  I-0.1723891 0.0000033 -1.2333 0.0026  I  -111.155    0.482    -9.705    0.258  0.195529  0.424979 -0.1723902  -111.223    -9.764  
-21 627 59392.00 I  0.197258 0.000018  0.423973 0.000024  I-0.1711413 0.0000022 -1.2315 0.0020  I  -110.800    0.462    -9.941    0.204  0.197249  0.423941 -0.1711520  -110.867    -9.981  
-21 628 59393.00 I  0.199044 0.000018  0.423142 0.000024  I-0.1699718 0.0000022 -1.0928 0.0017  I  -110.650    0.462   -10.213    0.204  0.199016  0.423212 -0.1700013  -110.723   -10.241  
-21 629 59394.00 I  0.201029 0.000016  0.421984 0.000024  I-0.1689845 0.0000025 -0.8679 0.0017  I  -110.826    0.456   -10.267    0.157  0.201014  0.422014 -0.1689979  -110.903   -10.285  
-21 630 59395.00 I  0.203109 0.000020  0.420660 0.000025  I-0.1681932 0.0000025 -0.7716 0.0019  I  -111.273    0.479   -10.019    0.145  0.203151  0.420682 -0.1681557  -111.326   -10.039  
-21 7 1 59396.00 I  0.205014 0.000019  0.419362 0.000028  I-0.1674218 0.0000029 -0.7339 0.0020  I  -111.789    0.517    -9.646    0.129  0.205011  0.419357 -0.1674255  -111.755    -9.689  
-21 7 2 59397.00 I  0.206926 0.000018  0.418132 0.000027  I-0.1667251 0.0000031 -0.6970 0.0028  I  -112.018    0.517    -9.432    0.129  0.206921  0.418137 -0.1667352  -112.004    -9.464  
-21 7 3 59398.00 I  0.209057 0.000019  0.416937 0.000021  I-0.1659894 0.0000049 -0.7753 0.0033  I  -112.152    0.517    -9.376    0.129  0.209024  0.416956 -0.1660067  -112.140    -9.398  
-21 7 4 59399.00 I  0.211305 0.000020  0.415846 0.000021  I-0.1651665 0.0000058 -0.8776 0.0033  I  -112.382    0.517    -9.360    0.129  0.211331  0.415811 -0.1651797  -112.363    -9.373  
-21 7 5 59400.00 I  0.213431 0.000022  0.414953 0.000020  I-0.1641960 0.0000045 -1.0946 0.0042  I  -112.723    0.633    -9.330    0.126  0.213414  0.414996 -0.1642095  -112.694    -9.336  
-21 7 6 59401.00 I  0.215668 0.000019  0.414031 0.000017  I-0.1630151 0.0000062 -1.1983 0.0032  I  -113.021    0.761    -9.374    0.123  0.215650  0.414027 -0.1630892  -112.980    -9.377  
-21 7 7 59402.00 I  0.218075 0.000021  0.413124 0.000011  I-0.1618109 0.0000046 -1.2674 0.0039  I  -113.170    0.734    -9.580    0.106  0.218140  0.413172 -0.1618291  -113.113    -9.583  
-21 7 8 59403.00 I  0.220156 0.000020  0.412099 0.000012  I-0.1604572 0.0000046 -1.4059 0.0032  I  -113.205    0.734    -9.877    0.106  0.220214  0.412138 -0.1604574  -113.230    -9.877  
-21 7 9 59404.00 I  0.221843 0.000019  0.410737 0.000011  I-0.1590267 0.0000044 -1.4617 0.0031  I  -113.198    0.734   -10.080    0.106  0.221832  0.410821 -0.1590228  -113.321   -10.078  
-21 710 59405.00 I  0.223646 0.000018  0.409104 0.000012  I-0.1575676 0.0000042 -1.4161 0.0027  I  -113.183    0.734   -10.068    0.106  0.223600  0.409097 -0.1575892  -113.323   -10.077  
-21 711 59406.00 I  0.225635 0.000014  0.407654 0.000011  I-0.1562182 0.0000031 -1.2995 0.0027  I  -113.196    0.677    -9.898    0.069  0.225666  0.407615 -0.1562169  -113.312    -9.920  
-21 712 59407.00 I  0.227531 0.000014  0.406533 0.000013  I-0.1549740 0.0000034 -1.1666 0.0025  I  -113.293    0.677    -9.734    0.069  0.227521  0.406499 -0.1549674  -113.374    -9.766  
-21 713 59408.00 I  0.229294 0.000010  0.405747 0.000013  I-0.1538993 0.0000040 -0.9908 0.0024  I  -113.458    0.678    -9.695    0.071  0.229363  0.405735 -0.1538980  -113.495    -9.729  
-21 714 59409.00 I  0.230856 0.000009  0.405108 0.000017  I-0.1530134 0.0000035 -0.7520 0.0029  I  -113.569    0.657    -9.760    0.083  0.230852  0.405177 -0.1530567  -113.617    -9.794  
-21 715 59410.00 I  0.232361 0.000009  0.404156 0.000017  I-0.1524002 0.0000041 -0.4983 0.0027  I  -113.540    0.657    -9.819    0.083  0.232364  0.404183 -0.1524225  -113.614    -9.847  
-21 716 59411.00 I  0.233955 0.000011  0.403091 0.000017  I-0.1519930 0.0000040 -0.3159 0.0040  I  -113.512    0.546    -9.778    0.102  0.233932  0.403085 -0.1520045  -113.595    -9.787  
-21 717 59412.00 I  0.235533 0.000010  0.402265 0.000018  I-0.1517461 0.0000069 -0.2005 0.0030  I  -113.674    0.546    -9.604    0.102  0.235568  0.402256 -0.1517411  -113.759    -9.608  
-21 718 59413.00 I  0.236943 0.000012  0.401496 0.000018  I-0.1515306 0.0000044 -0.2694 0.0041  I  -114.202    0.578    -9.387    0.143  0.236938  0.401571 -0.1515176  -114.276    -9.388  
-21 719 59414.00 I  0.238377 0.000013  0.400302 0.000018  I-0.1511809 0.0000045 -0.4176 0.0035  I  -114.945    0.578    -9.260    0.143  0.238366  0.400312 -0.1511975  -115.015    -9.262  
-21 720 59415.00 I  0.239932 0.000015  0.398917 0.000013  I-0.1507021 0.0000054 -0.5459 0.0030  I  -115.568    0.589    -9.306    0.161  0.239941  0.398929 -0.1507114  -115.643    -9.312  
-21 721 59416.00 I  0.241374 0.000016  0.397610 0.000013  I-0.1500814 0.0000040 -0.6974 0.0034  I  -115.815    0.637    -9.469    0.166  0.241402  0.397614 -0.1500616  -115.876    -9.476  
-21 722 59417.00 I  0.242534 0.000016  0.396307 0.000012  I-0.1493035 0.0000040 -0.8605 0.0032  I  -115.708    0.637    -9.593    0.166  0.242550  0.396349 -0.1492653  -115.745    -9.604  
-21 723 59418.00 I  0.243564 0.000017  0.394841 0.000012  I-0.1483881 0.0000049 -0.9406 0.0041  I  -115.357    0.746    -9.613    0.173  0.243559  0.394850 -0.1483896  -115.468    -9.626  
-21 724 59419.00 I  0.244412 0.000016  0.393382 0.000010  I-0.1474753 0.0000072 -0.8618 0.0035  I  -115.261    0.746    -9.596    0.173  0.244504  0.393363 -0.1475216  -115.321    -9.619  
-21 725 59420.00 I  0.244597 0.000020  0.392090 0.000014  I-0.1467003 0.0000050 -0.6758 0.0043  I  -115.215    0.536    -9.688    0.131  0.244659  0.392108 -0.1467385  -115.265    -9.715  
-21 726 59421.00 I  0.244305 0.000018  0.390788 0.000014  I-0.1460940 0.0000048 -0.5790 0.0039  I  -115.222    0.536    -9.845    0.131  0.244282  0.390818 -0.1460743  -115.280    -9.873  
-21 727 59422.00 I  0.244044 0.000018  0.389187 0.000014  I-0.1455385 0.0000059 -0.4935 0.0033  I  -115.369    0.367    -9.888    0.090  0.244021  0.389282 -0.1455380  -115.457    -9.910  
-21 728 59423.00 I  0.244010 0.000017  0.386991 0.000015  I-0.1451205 0.0000046 -0.3673 0.0035  I  -115.722    0.385    -9.730    0.090  0.243957  0.387023 -0.1451164  -115.784    -9.750  
-21 729 59424.00 I  0.244337 0.000017  0.384572 0.000015  I-0.1447604 0.0000039 -0.3715 0.0030  I  -116.266    0.414    -9.501    0.089  0.244271  0.384533 -0.1447485  -116.221    -9.509  
-21 730 59425.00 I  0.245094 0.000020  0.382528 0.000015  I-0.1443673 0.0000039 -0.4062 0.0032  I  -116.564    0.414    -9.372    0.089  0.245054  0.382456 -0.1443684  -116.596    -9.367  
-21 731 59426.00 I  0.246002 0.000018  0.381140 0.000011  I-0.1439256 0.0000050 -0.5081 0.0027  I  -116.705    0.414    -9.378    0.089  0.246021  0.381094 -0.1439172  -116.756    -9.383  
-21 8 1 59427.00 I  0.246812 0.000022  0.380135 0.000014  I-0.1433414 0.0000037 -0.6392 0.0031  I  -116.769    0.673    -9.408    0.131  0.246780  0.380162 -0.1433541  -116.809    -9.429  
-21 8 2 59428.00 I  0.247743 0.000024  0.378992 0.000013  I-0.1426539 0.0000038 -0.7501 0.0026  I  -116.858    0.673    -9.379    0.131  0.247724  0.379020 -0.1426563  -116.864    -9.419  
-21 8 3 59429.00 I  0.248633 0.000025  0.377651 0.000013  I-0.1418323 0.0000037 -0.8876 0.0030  I  -116.993    0.702    -9.353    0.118  0.248665  0.377672 -0.1418281  -116.928    -9.418  
-21 8 4 59430.00 I  0.249331 0.000023  0.376205 0.000012  I-0.1408910 0.0000046 -0.9883 0.0029  I  -117.140    0.702    -9.454    0.118  0.249247  0.376225 -0.1408819  -117.087    -9.488  
-21 8 5 59431.00 I  0.250340 0.000021  0.374746 0.000013  I-0.1398595 0.0000045 -1.0775 0.0033  I  -117.244    0.702    -9.701    0.118  0.250318  0.374716 -0.1398588  -117.212    -9.692  
-21 8 6 59432.00 I  0.251511 0.000020  0.373438 0.000013  I-0.1387727 0.0000046 -1.0567 0.0036  I  -117.343    0.322    -9.921    0.160  0.251557  0.373439 -0.1388293  -117.228    -9.944  
-21 8 7 59433.00 I  0.252321 0.000016  0.372184 0.000011  I-0.1377548 0.0000057 -1.0100 0.0036  I  -117.054    0.322    -9.990    0.160  0.252384  0.372189 -0.1377997  -117.131   -10.037  
-21 8 8 59434.00 I  0.252520 0.000015  0.370923 0.000011  I-0.1367466 0.0000056 -0.9817 0.0041  I  -116.803    0.322    -9.864    0.160  0.252618  0.370959 -0.1367543  -116.976    -9.913  
-21 8 9 59435.00 I  0.251919 0.000016  0.369469 0.000015  I-0.1358304 0.0000059 -0.8364 0.0039  I  -116.669    0.559    -9.662    0.049  0.251958  0.369547 -0.1358220  -116.861    -9.698  
-21 810 59436.00 I  0.250919 0.000016  0.367462 0.000015  I-0.1350852 0.0000053 -0.6567 0.0039  I  -116.699    0.559    -9.559    0.049  0.250843  0.367504 -0.1350686  -116.860    -9.570  
-21 811 59437.00 I  0.250232 0.000018  0.365293 0.000020  I-0.1345114 0.0000051 -0.4937 0.0037  I  -116.835    0.493    -9.626    0.126  0.250176  0.365255 -0.1345085  -116.935    -9.605  
-21 812 59438.00 I  0.249912 0.000016  0.363353 0.000020  I-0.1341041 0.0000052 -0.3120 0.0036  I  -116.985    0.493    -9.777    0.126  0.249897  0.363348 -0.1341190  -117.018    -9.784  
-21 813 59439.00 I  0.249584 0.000016  0.361530 0.000019  I-0.1338379 0.0000052 -0.2790 0.0037  I  -117.141    0.493    -9.859    0.126  0.249586  0.361519 -0.1338317  -117.129    -9.917  
-21 814 59440.00 I  0.249171 0.000015  0.359752 0.000019  I-0.1335122 0.0000052 -0.3479 0.0042  I  -117.391    0.493    -9.789    0.126  0.249168  0.359749 -0.1335458  -117.340    -9.843  
-21 815 59441.00 I  0.248745 0.000011  0.358118 0.000015  I-0.1331296 0.0000065 -0.4545 0.0036  I  -117.789    0.358    -9.622    0.178  0.248726  0.358103 -0.1331531  -117.733    -9.659  
-21 816 59442.00 I  0.248383 0.000010  0.356528 0.000016  I-0.1325638 0.0000049 -0.6795 0.0038  I  -118.229    0.487    -9.489    0.154  0.248321  0.356538 -0.1325675  -118.199    -9.514  
-21 817 59443.00 I  0.248158 0.000008  0.354898 0.000012  I-0.1317591 0.0000041 -0.9390 0.0030  I  -118.499    0.527    -9.471    0.136  0.248130  0.354895 -0.1317488  -118.520    -9.488  
-21 818 59444.00 I  0.248038 0.000011  0.353268 0.000015  I-0.1307146 0.0000033 -1.1121 0.0027  I  -118.462    0.554    -9.533    0.137  0.248008  0.353279 -0.1307185  -118.546    -9.545  
-21 819 59445.00 I  0.247964 0.000011  0.351671 0.000015  I-0.1295676 0.0000035 -1.1872 0.0025  I  -118.183    0.554    -9.578    0.137  0.247978  0.351653 -0.1295488  -118.297    -9.587  
-21 820 59446.00 I  0.247724 0.000011  0.350066 0.000015  I-0.1283625 0.0000037 -1.1954 0.0025  I  -117.888    0.628    -9.550    0.138  0.247731  0.350108 -0.1283563  -117.988    -9.566  
-21 821 59447.00 I  0.247301 0.000012  0.348288 0.000016  I-0.1272359 0.0000037 -1.0264 0.0024  I  -117.607    0.628    -9.514    0.138  0.247290  0.348276 -0.1272649  -117.743    -9.514  
-21 822 59448.00 I  0.246848 0.000017  0.346515 0.000015  I-0.1263225 0.0000031 -0.8191 0.0024  I  -117.437    0.956    -9.510    0.137  0.246822  0.346558 -0.1263384  -117.577    -9.494  
-21 823 59449.00 I  0.246375 0.000017  0.344529 0.000014  I-0.1255772 0.0000032 -0.6734 0.0025  I  -117.338    0.956    -9.514    0.137  0.246343  0.344554 -0.1255763  -117.443    -9.485  
-21 824 59450.00 I  0.246054 0.000016  0.342245 0.000011  I-0.1249661 0.0000040 -0.5563 0.0027  I  -117.334    1.067    -9.451    0.136  0.245986  0.342232 -0.1249636  -117.347    -9.416  
-21 825 59451.00 I  0.246021 0.000028  0.340124 0.000013  I-0.1244586 0.0000044 -0.4570 0.0029  I  -117.522    1.021    -9.303    0.139  0.246006  0.340077 -0.1244735  -117.579    -9.295  
-21 826 59452.00 I  0.246037 0.000028  0.338300 0.000014  I-0.1240135 0.0000043 -0.4735 0.0030  I  -117.913    1.021    -9.158    0.139  0.246029  0.338309 -0.1240162  -118.019    -9.189  
-21 827 59453.00 I  0.246060 0.000029  0.336463 0.000014  I-0.1234930 0.0000042 -0.5457 0.0041  I  -118.605    0.533    -9.099    0.157  0.246039  0.336463 -0.1235117  -118.513    -9.184  
-21 828 59454.00 I  0.246070 0.000027  0.334743 0.000016  I-0.1228940 0.0000070 -0.7022 0.0030  I  -118.811    0.533    -9.128    0.157  0.246083  0.334712 -0.1228899  -118.761    -9.205  
-21 829 59455.00 I  0.246025 0.000028  0.333202 0.000023  I-0.1221072 0.0000044 -0.8028 0.0041  I  -118.832    0.610    -9.146    0.113  0.246022  0.333214 -0.1221387  -118.783    -9.190  
-21 830 59456.00 I  0.245765 0.000028  0.331656 0.000024  I-0.1212950 0.0000041 -0.8836 0.0028  I  -118.748    0.610    -9.101    0.113  0.245834  0.331664 -0.1212791  -118.708    -9.104  
-21 831 59457.00 I  0.245077 0.000018  0.329824 0.000023  I-0.1203297 0.0000036 -0.9952 0.0025  I  -118.699    0.627    -9.004    0.101  0.245060  0.329881 -0.1203267  -118.658    -9.011  
-21 9 1 59458.00 I  0.244343 0.000027  0.327816 0.000024  I-0.1193348 0.0000028 -1.0161 0.0022  I  -118.639    0.676    -9.125    0.106  0.244291  0.327776 -0.1193071  -118.650    -9.123  
-21 9 2 59459.00 I  0.243924 0.000027  0.325945 0.000023  I-0.1182801 0.0000026 -1.0892 0.0019  I  -118.539    0.676    -9.374    0.106  0.243859  0.325972 -0.1182574  -118.581    -9.390  
-21 9 3 59460.00 I  0.243863 0.000026  0.324212 0.000022  I-0.1172200 0.0000025 -0.9714 0.0019  I  -118.345    0.676    -9.635    0.106  0.243838  0.324135 -0.1172280  -118.364    -9.679  
-21 9 4 59461.00 I  0.243825 0.000024  0.322769 0.000014  I-0.1163420 0.0000028 -0.8397 0.0021  I  -118.130    0.696    -9.752    0.110  0.243924  0.322819 -0.1162657  -118.147    -9.782  
-21 9 5 59462.00 I  0.243251 0.000024  0.321179 0.000011  I-0.1155349 0.0000033 -0.7253 0.0021  I  -118.006    0.696    -9.656    0.110  0.243284  0.321221 -0.1154565  -117.995    -9.664  
-21 9 6 59463.00 I  0.242256 0.000023  0.319260 0.000016  I-0.1149350 0.0000031 -0.4800 0.0026  I  -118.010    0.523    -9.420    0.106  0.242288  0.319291 -0.1149183  -117.966    -9.415  
-21 9 7 59464.00 I  0.241133 0.000011  0.317267 0.000014  I-0.1145696 0.0000040 -0.2505 0.0025  I  -118.422    0.137    -9.192    0.101  0.241085  0.317267 -0.1145864  -118.054    -9.194  
-21 9 8 59465.00 I  0.240206 0.000014  0.315389 0.000023  I-0.1144301 0.0000040 -0.0327 0.0028  I  -118.246    0.411    -9.142    0.099  0.240168  0.315380 -0.1144389  -118.217    -9.134  
-21 9 9 59466.00 I  0.239548 0.000016  0.313676 0.000024  I-0.1144584 0.0000039  0.0478 0.0030  I  -118.133    0.411    -9.271    0.099  0.239509  0.313682 -0.1144456  -118.199    -9.278  
-21 910 59467.00 I  0.239101 0.000018  0.311975 0.000025  I-0.1144993 0.0000045  0.0492 0.0032  I  -118.027    0.604    -9.451    0.097  0.239055  0.311944 -0.1145001  -118.196    -9.493  
-21 911 59468.00 I  0.238934 0.000017  0.310406 0.000025  I-0.1145146 0.0000050 -0.0761 0.0034  I  -118.301    0.604    -9.573    0.097  0.238903  0.310398 -0.1145067  -118.376    -9.600  
-21 912 59469.00 I  0.239046 0.000018  0.309195 0.000024  I-0.1143199 0.0000052 -0.2829 0.0036  I  -118.546    0.626    -9.528    0.118  0.239057  0.309176 -0.1143417  -118.582    -9.536  
-21 913 59470.00 I  0.238924 0.000019  0.308180 0.000024  I-0.1139301 0.0000052 -0.5458 0.0041  I  -118.689    0.626    -9.376    0.118  0.239061  0.308241 -0.1139194  -118.703    -9.367  
-21 914 59471.00 I  0.238106 0.000025  0.306840 0.000016  I-0.1132437 0.0000063 -0.7627 0.0041  I  -118.690    0.641    -9.233    0.133  0.238135  0.306840 -0.1132542  -118.709    -9.209  
-21 915 59472.00 I  0.236805 0.000028  0.305453 0.000022  I-0.1124496 0.0000063 -0.8451 0.0045  I  -118.537    0.691    -9.159    0.186  0.236855  0.305424 -0.1124265  -118.563    -9.153  
-21 916 59473.00 I  0.235251 0.000027  0.304159 0.000021  I-0.1115777 0.0000063 -0.8549 0.0046  I  -118.262    0.691    -9.140    0.186  0.235175  0.304217 -0.1115600  -118.302    -9.166  
-21 917 59474.00 I  0.234103 0.000027  0.302451 0.000021  I-0.1107833 0.0000066 -0.7341 0.0059  I  -117.948    0.691    -9.140    0.186  0.234052  0.302470 -0.1107776  -117.983    -9.205  
-21 918 59475.00 I  0.233189 0.000026  0.300658 0.000018  I-0.1101546 0.0000100 -0.4779 0.0045  I  -117.704    0.802    -9.133    0.241  0.233267  0.300669 -0.1101847  -117.773    -9.189  
-21 919 59476.00 I  0.231950 0.000027  0.298946 0.000018  I-0.1097962 0.0000061 -0.3156 0.0058  I  -117.601    0.638    -9.086    0.159  0.231901  0.298971 -0.1097908  -117.690    -9.120  
-21 920 59477.00 I  0.230912 0.000020  0.297070 0.000018  I-0.1095058 0.0000060 -0.2061 0.0042  I  -117.617    0.638    -8.955    0.159  0.230860  0.297082 -0.1095369  -117.703    -8.970  
-21 921 59478.00 I  0.230449 0.000016  0.295190 0.000008  I-0.1093773 0.0000059 -0.1167 0.0042  I  -117.672    0.603    -8.737    0.052  0.230386  0.295169 -0.1093835  -117.748    -8.731  
-21 922 59479.00 I  0.230222 0.000020  0.293451 0.000034  I-0.1092491 0.0000059 -0.0973 0.0040  I  -117.733    0.601    -8.511    0.062  0.230280  0.293410 -0.1092939  -117.791    -8.533  
-21 923 59480.00 I  0.229734 0.000020  0.291962 0.000034  I-0.1091847 0.0000053 -0.0718 0.0040  I  -117.841    0.601    -8.401    0.062  0.229745  0.291932 -0.1092075  -117.893    -8.459  
-21 924 59481.00 I  0.229050 0.000020  0.290728 0.000034  I-0.1090674 0.0000055 -0.1606 0.0062  I  -118.068    0.486    -8.478    0.113  0.229059  0.290744 -0.1090710  -118.064    -8.550  
-21 925 59482.00 I  0.228149 0.000018  0.289698 0.000034  I-0.1088532 0.0000111 -0.2801 0.0047  I  -118.135    0.486    -8.618    0.113  0.228196  0.289721 -0.1088548  -118.132    -8.702  
-21 926 59483.00 I  0.226731 0.000019  0.288540 0.000035  I-0.1085067 0.0000077 -0.4009 0.0069  I  -118.049    0.658    -8.713    0.081  0.226765  0.288616 -0.1085235  -118.029    -8.801  
-21 927 59484.00 I  0.224988 0.000018  0.286871 0.000035  I-0.1080378 0.0000081 -0.5626 0.0058  I  -117.850    0.658    -8.724    0.081  0.224983  0.286909 -0.1080259  -117.816    -8.811  
-21 928 59485.00 I  0.223251 0.000014  0.285093 0.000012  I-0.1073990 0.0000086 -0.6719 0.0051  I  -117.684    0.672    -8.731    0.073  0.223233  0.285091 -0.1073996  -117.636    -8.811  
-21 929 59486.00 I  0.221734 0.000020  0.283227 0.000017  I-0.1067206 0.0000062 -0.7015 0.0053  I  -117.576    0.701    -8.818    0.105  0.221642  0.283266 -0.1067014  -117.530    -8.894  
-21 930 59487.00 I  0.220681 0.000023  0.281345 0.000017  I-0.1059828 0.0000061 -0.7706 0.0042  I  -117.354    0.701    -8.959    0.105  0.220649  0.281274 -0.1059687  -117.318    -9.028  
-2110 1 59488.00 I  0.219920 0.000025  0.279828 0.000016  I-0.1052404 0.0000057 -0.6567 0.0041  I  -116.913    0.719    -9.053    0.123  0.219900  0.279843 -0.1052566  -116.884    -9.102  
-2110 2 59489.00 I  0.219188 0.000024  0.278462 0.000015  I-0.1047003 0.0000055 -0.4501 0.0035  I  -116.349    0.719    -9.010    0.123  0.219232  0.278385 -0.1046635  -116.396    -9.043  
-2110 3 59490.00 I  0.218063 0.000026  0.277410 0.000016  I-0.1043190 0.0000040 -0.3071 0.0033  I  -116.021    0.829    -8.851    0.162  0.218114  0.277440 -0.1042262  -116.108    -8.872  
-2110 4 59491.00 I  0.216517 0.000026  0.276370 0.000017  I-0.1041097 0.0000036 -0.0933 0.0029  I  -116.030    0.829    -8.634    0.162  0.216463  0.276398 -0.1040412  -116.115    -8.648  
-2110 5 59492.00 I  0.214839 0.000020  0.275295 0.000011  I-0.1041577 0.0000043  0.1966 0.0027  I  -116.226    0.858    -8.417    0.187  0.214966  0.275265 -0.1041427  -116.245    -8.435  
-2110 6 59493.00 I  0.212841 0.000021  0.274060 0.000020  I-0.1044985 0.0000040  0.4735 0.0029  I  -116.465    0.798    -8.287    0.179  0.212886  0.274073 -0.1045130  -116.543    -8.305  
-2110 7 59494.00 I  0.210716 0.000020  0.272253 0.000020  I-0.1050403 0.0000040  0.5574 0.0029  I  -116.703    0.798    -8.338    0.179  0.210670  0.272310 -0.1050355  -116.846    -8.364  
-2110 8 59495.00 I  0.208770 0.000020  0.270362 0.000020  I-0.1055542 0.0000041  0.4641 0.0030  I  -117.077    0.199    -8.550    0.167  0.208740  0.270354 -0.1055552  -117.140    -8.593  
-2110 9 59496.00 I  0.207046 0.000016  0.268634 0.000020  I-0.1059322 0.0000046  0.2619 0.0032  I  -117.006    0.199    -8.726    0.167  0.206987  0.268630 -0.1059176  -117.149    -8.775  
-211010 59497.00 I  0.205607 0.000016  0.267108 0.000020  I-0.1060595 0.0000049  0.0043 0.0030  I  -116.877    0.199    -8.689    0.167  0.205587  0.267049 -0.1060489  -117.008    -8.734  
-211011 59498.00 I  0.204303 0.000020  0.265970 0.000022  I-0.1059633 0.0000040 -0.1856 0.0035  I  -116.735    0.498    -8.463    0.121  0.204294  0.265940 -0.1059506  -116.845    -8.499  
-211012 59499.00 I  0.202917 0.000021  0.265370 0.000015  I-0.1057105 0.0000050 -0.3088 0.0030  I  -116.620    0.672    -8.241    0.021  0.202929  0.265318 -0.1056985  -116.696    -8.264  
-211013 59500.00 I  0.201334 0.000024  0.265039 0.000020  I-0.1053754 0.0000044 -0.3430 0.0034  I  -116.510    0.669    -8.164    0.063  0.201347  0.265115 -0.1053769  -116.533    -8.163  
-211014 59501.00 I  0.199470 0.000023  0.264502 0.000021  I-0.1050543 0.0000047 -0.2879 0.0033  I  -116.349    0.669    -8.205    0.063  0.199531  0.264474 -0.1050561  -116.392    -8.233  
-211015 59502.00 I  0.197117 0.000024  0.264010 0.000021  I-0.1048184 0.0000048 -0.1764 0.0034  I  -116.078    0.664    -8.289    0.089  0.197144  0.264052 -0.1048215  -116.168    -8.339  
-211016 59503.00 I  0.194630 0.000025  0.263332 0.000021  I-0.1047176 0.0000049 -0.0165 0.0035  I  -115.831    0.664    -8.322    0.089  0.194540  0.263311 -0.1047296  -115.892    -8.371  
-211017 59504.00 I  0.192495 0.000024  0.262707 0.000033  I-0.1047826 0.0000050  0.1351 0.0035  I  -115.633    0.573    -8.293    0.073  0.192522  0.262732 -0.1047961  -115.671    -8.326  
-211018 59505.00 I  0.190391 0.000019  0.262045 0.000033  I-0.1049874 0.0000051  0.2856 0.0038  I  -115.558    0.573    -8.157    0.073  0.190330  0.262116 -0.1049797  -115.586    -8.172  
-211019 59506.00 I  0.188479 0.000015  0.261101 0.000030  I-0.1053253 0.0000056  0.3506 0.0037  I  -115.562    0.549    -7.903    0.060  0.188419  0.261094 -0.1053261  -115.599    -7.898  
-211020 59507.00 I  0.187014 0.000020  0.260354 0.000031  I-0.1056529 0.0000053  0.3085 0.0038  I  -115.538    0.576    -7.630    0.105  0.186951  0.260372 -0.1056852  -115.532    -7.637  
-211021 59508.00 I  0.185923 0.000018  0.259645 0.000031  I-0.1059410 0.0000052  0.2624 0.0037  I  -115.389    0.727    -7.595    0.167  0.185890  0.259671 -0.1059933  -115.408    -7.531  
-211022 59509.00 I  0.185078 0.000021  0.258900 0.000031  I-0.1061493 0.0000052  0.1309 0.0042  I  -115.324    0.727    -7.650    0.167  0.185109  0.258931 -0.1061695  -115.283    -7.652  
-211023 59510.00 I  0.183898 0.000020  0.258067 0.000016  I-0.1061660 0.0000066 -0.1112 0.0042  I  -115.250    0.727    -7.831    0.167  0.183997  0.258126 -0.1061599  -115.214    -7.852  
-211024 59511.00 I  0.182243 0.000023  0.256851 0.000023  I-0.1059400 0.0000065 -0.3140 0.0046  I  -115.116    0.740    -7.965    0.119  0.182170  0.256859 -0.1059532  -115.105    -7.981  
-211025 59512.00 I  0.180791 0.000022  0.255744 0.000023  I-0.1055627 0.0000064 -0.4426 0.0050  I  -114.938    0.740    -7.991    0.119  0.180765  0.255674 -0.1055673  -114.951    -7.995  
-211026 59513.00 I  0.179385 0.000022  0.255122 0.000020  I-0.1050724 0.0000077 -0.5184 0.0042  I  -114.813    0.753    -7.994    0.025  0.179443  0.255135 -0.1050710  -114.842    -7.976  
-211027 59514.00 I  0.177416 0.000023  0.254633 0.000023  I-0.1045658 0.0000053 -0.4745 0.0046  I  -114.744    0.629    -8.053    0.107  0.177475  0.254614 -0.1045560  -114.798    -8.064  
-211028 59515.00 I  0.175039 0.000020  0.254166 0.000022  I-0.1041316 0.0000052 -0.4061 0.0039  I  -114.550    0.629    -8.106    0.107  0.174986  0.254210 -0.1040921  -114.636    -8.154  
-211029 59516.00 I  0.172943 0.000019  0.253719 0.000022  I-0.1037650 0.0000058 -0.3036 0.0039  I  -114.130    0.569    -8.065    0.133  0.172883  0.253703 -0.1037503  -114.222    -8.112  
-211030 59517.00 I  0.171128 0.000016  0.253432 0.000016  I-0.1035655 0.0000058 -0.0778 0.0042  I  -113.565    0.569    -7.826    0.133  0.171153  0.253485 -0.1035881  -113.712    -7.886  
-211031 59518.00 I  0.169169 0.000018  0.253020 0.000017  I-0.1036412 0.0000060  0.2435 0.0041  I  -113.316    0.569    -7.580    0.133  0.169153  0.253030 -0.1036762  -113.489    -7.636  
-2111 1 59519.00 I  0.167192 0.000022  0.252558 0.000027  I-0.1040422 0.0000058  0.5340 0.0052  I  -113.470    0.637    -7.412    0.100  0.167161  0.252590 -0.1040619  -113.648    -7.463  
-2111 2 59520.00 I  0.165520 0.000021  0.251988 0.000024  I-0.1046895 0.0000086  0.7654 0.0036  I  -113.619    0.692    -7.244    0.053  0.165421  0.252037 -0.1047142  -113.919    -7.301  
-2111 3 59521.00 I  0.164374 0.000022  0.251144 0.000028  I-0.1055272 0.0000044  0.8592 0.0047  I  -113.957    0.495    -7.058    0.045  0.164345  0.251154 -0.1055305  -114.076    -7.098  
-2111 4 59522.00 I  0.163277 0.000023  0.250403 0.000027  I-0.1063491 0.0000038  0.7765 0.0030  I  -114.200    0.495    -6.951    0.045  0.163380  0.250407 -0.1063597  -114.274    -6.977  
-2111 5 59523.00 I  0.161443 0.000023  0.249783 0.000027  I-0.1070346 0.0000041  0.5572 0.0028  I  -114.304    0.495    -7.056    0.045  0.161527  0.249780 -0.1070350  -114.417    -7.068  
-2111 6 59524.00 I  0.158963 0.000023  0.249269 0.000027  I-0.1074215 0.0000040  0.2121 0.0029  I  -114.138    0.495    -7.251    0.045  0.158959  0.249274 -0.1074216  -114.174    -7.273  
-2111 7 59525.00 I  0.156486 0.000016  0.248733 0.000026  I-0.1074873 0.0000041 -0.0473 0.0029  I  -113.762    0.466    -7.271    0.067  0.156428  0.248766 -0.1075061  -113.720    -7.312  
-2111 8 59526.00 I  0.154401 0.000015  0.248077 0.000025  I-0.1073735 0.0000041 -0.1669 0.0052  I  -113.449    0.466    -7.081    0.067  0.154365  0.248057 -0.1073849  -113.374    -7.138  
-2111 9 59527.00 I  0.152528 0.000013  0.247543 0.000021  I-0.1071778 0.0000095 -0.2138 0.0052  I  -113.100    0.892    -6.946    0.104  0.152501  0.247567 -0.1071716  -113.247    -7.009  
-211110 59528.00 I  0.150845 0.000021  0.247118 0.000032  I-0.1069757 0.0000096 -0.1715 0.0069  I  -113.254    0.777    -7.016    0.083  0.150781  0.247125 -0.1069620  -113.363    -7.072  
-211111 59529.00 I  0.149530 0.000021  0.246768 0.000032  I-0.1068801 0.0000100  0.0066 0.0070  I  -113.306    0.777    -7.190    0.083  0.149470  0.246785 -0.1068772  -113.428    -7.227  
-211112 59530.00 I  0.148524 0.000022  0.246609 0.000032  I-0.1069917 0.0000102  0.1929 0.0076  I  -113.227    0.777    -7.246    0.083  0.148470  0.246564 -0.1069721  -113.370    -7.262  
-211113 59531.00 I  0.147731 0.000022  0.246458 0.000025  I-0.1072536 0.0000115  0.3422 0.0059  I  -113.083    0.585    -7.145    0.046  0.147692  0.246455 -0.1072523  -113.185    -7.165  
-211114 59532.00 I  0.146991 0.000029  0.246430 0.000027  I-0.1076409 0.0000060  0.3860 0.0065  I  -112.947    0.624    -6.988    0.109  0.147041  0.246459 -0.1076527  -112.994    -7.024  
-211115 59533.00 I  0.145706 0.000028  0.246293 0.000027  I-0.1079865 0.0000059  0.3125 0.0040  I  -112.888    0.624    -6.824    0.109  0.145836  0.246338 -0.1080024  -112.892    -6.878  
-211116 59534.00 I  0.143581 0.000025  0.245994 0.000013  I-0.1082688 0.0000052  0.2477 0.0034  I  -112.910    0.639    -6.648    0.131  0.143555  0.246023 -0.1082774  -112.883    -6.691  
-211117 59535.00 I  0.141479 0.000029  0.245387 0.000017  I-0.1084699 0.0000033  0.1468 0.0031  I  -112.947    0.627    -6.365    0.093  0.141392  0.245346 -0.1084806  -112.918    -6.416  
-211118 59536.00 I  0.139777 0.000028  0.245122 0.000017  I-0.1085497 0.0000032  0.0077 0.0023  I  -112.897    0.627    -6.187    0.093  0.139789  0.245077 -0.1085552  -112.878    -6.226  
-211119 59537.00 I  0.137829 0.000028  0.245224 0.000018  I-0.1084690 0.0000033 -0.1804 0.0025  I  -112.755    0.627    -6.238    0.093  0.137868  0.245245 -0.1084680  -112.755    -6.253  
-211120 59538.00 I  0.135539 0.000022  0.245332 0.000016  I-0.1081900 0.0000038 -0.3652 0.0025  I  -112.579    0.623    -6.465    0.045  0.135470  0.245267 -0.1081943  -112.586    -6.495  
-211121 59539.00 I  0.133471 0.000023  0.245952 0.000015  I-0.1077755 0.0000038 -0.4394 0.0027  I  -112.409    0.623    -6.679    0.045  0.133433  0.245936 -0.1077699  -112.425    -6.731  
-211122 59540.00 I  0.131598 0.000023  0.246876 0.000016  I-0.1073085 0.0000038 -0.5217 0.0031  I  -112.252    0.687    -6.767    0.052  0.131584  0.246933 -0.1072664  -112.282    -6.830  
-211123 59541.00 I  0.129625 0.000018  0.247268 0.000011  I-0.1067448 0.0000050 -0.5658 0.0032  I  -112.119    0.724    -6.790    0.058  0.129614  0.247350 -0.1067281  -112.157    -6.857  
-211124 59542.00 I  0.127862 0.000020  0.247300 0.000016  I-0.1062107 0.0000052 -0.5086 0.0036  I  -111.996    0.739    -6.838    0.054  0.127746  0.247246 -0.1062044  -112.031    -6.907  
-211125 59543.00 I  0.126572 0.000020  0.247702 0.000015  I-0.1057315 0.0000053 -0.4397 0.0037  I  -111.791    0.739    -6.875    0.054  0.126546  0.247694 -0.1057277  -111.742    -6.907  
-211126 59544.00 I  0.125318 0.000019  0.248375 0.000015  I-0.1053815 0.0000053 -0.2201 0.0041  I  -111.356    0.923    -6.733    0.032  0.125318  0.248339 -0.1053900  -111.268    -6.773  
-211127 59545.00 I  0.123945 0.000019  0.249129 0.000015  I-0.1053186 0.0000062  0.0815 0.0040  I  -111.042    0.923    -6.557    0.032  0.123926  0.249137 -0.1053000  -110.920    -6.580  
-211128 59546.00 I  0.122508 0.000021  0.250112 0.000018  I-0.1055093 0.0000059  0.2777 0.0043  I  -110.967    0.532    -6.419    0.140  0.122510  0.250182 -0.1054501  -110.876    -6.447  
-211129 59547.00 I  0.120992 0.000021  0.250795 0.000017  I-0.1058362 0.0000059  0.3605 0.0041  I  -111.176    0.532    -6.413    0.140  0.120935  0.250800 -0.1057693  -111.138    -6.452  
-211130 59548.00 I  0.119475 0.000020  0.251402 0.000013  I-0.1062466 0.0000058  0.4920 0.0037  I  -111.442    0.488    -6.403    0.159  0.119462  0.251409 -0.1062356  -111.496    -6.463  
-2112 1 59549.00 I  0.117975 0.000024  0.252126 0.000022  I-0.1068040 0.0000045  0.5748 0.0037  I  -111.625    0.616    -6.214    0.137  0.117908  0.252101 -0.1068219  -111.672    -6.258  
-2112 2 59550.00 I  0.116668 0.000024  0.253063 0.000022  I-0.1073454 0.0000047  0.5053 0.0033  I  -111.845    0.616    -5.940    0.137  0.116646  0.253077 -0.1073817  -111.874    -5.966  
-2112 3 59551.00 I  0.115232 0.000025  0.254113 0.000023  I-0.1077649 0.0000049  0.2867 0.0040  I  -112.117    0.616    -5.860    0.137  0.115236  0.254139 -0.1077758  -112.122    -5.874  
-2112 4 59552.00 I  0.113608 0.000021  0.254399 0.000021  I-0.1078887 0.0000064 -0.0224 0.0033  I  -112.182    0.717    -6.016    0.112  0.113528  0.254463 -0.1079062  -112.187    -6.031  
-2112 5 59553.00 I  0.112222 0.000026  0.254584 0.000027  I-0.1077618 0.0000043 -0.2066 0.0038  I  -111.890    0.699    -6.133    0.117  0.112210  0.254544 -0.1077891  -111.884    -6.154  
-2112 6 59554.00 I  0.110908 0.000027  0.255085 0.000028  I-0.1075221 0.0000042 -0.2509 0.0035  I  -111.497    0.699    -6.053    0.117  0.110933  0.255126 -0.1075299  -111.458    -6.078  
-2112 7 59555.00 I  0.109151 0.000026  0.255695 0.000023  I-0.1072763 0.0000054 -0.2462 0.0030  I  -111.339    0.657    -5.973    0.123  0.109262  0.255631 -0.1072636  -111.227    -6.002  
-2112 8 59556.00 I  0.106687 0.000029  0.256255 0.000032  I-0.1070718 0.0000044 -0.1152 0.0034  I  -111.253    0.621    -6.110    0.125  0.106686  0.256326 -0.1071092  -111.176    -6.134  
-2112 9 59557.00 I  0.104023 0.000029  0.256732 0.000032  I-0.1071018 0.0000041  0.1834 0.0028  I  -111.162    0.621    -6.317    0.125  0.103984  0.256757 -0.1071653  -111.132    -6.338  
-211210 59558.00 I  0.101398 0.000031  0.257109 0.000031  I-0.1073914 0.0000036  0.3404 0.0031  I  -111.069    0.621    -6.289    0.125  0.101414  0.257116 -0.1074002  -111.095    -6.308  
-211211 59559.00 I  0.098430 0.000026  0.257351 0.000027  I-0.1077498 0.0000046  0.3991 0.0028  I  -111.051    0.590    -5.980    0.127  0.098426  0.257383 -0.1077748  -111.085    -5.998  
-211212 59560.00 I  0.095295 0.000026  0.257386 0.000028  I-0.1081927 0.0000043  0.4672 0.0032  I  -111.088    0.716    -5.636    0.114  0.095231  0.257384 -0.1082102  -111.113    -5.653  
-211213 59561.00 I  0.092595 0.000024  0.257453 0.000027  I-0.1086342 0.0000044  0.3852 0.0034  I  -111.130    0.716    -5.456    0.114  0.092509  0.257408 -0.1086201  -111.139    -5.474  
-211214 59562.00 I  0.090276 0.000020  0.258104 0.000016  I-0.1089561 0.0000053  0.2823 0.0033  I  -111.194    0.820    -5.403    0.098  0.090306  0.258026 -0.1089586  -111.161    -5.420  
-211215 59563.00 I  0.087851 0.000033  0.258958 0.000030  I-0.1091983 0.0000050  0.1780 0.0037  I  -111.284    0.749    -5.355    0.119  0.087829  0.258992 -0.1091980  -111.310    -5.388  
-211216 59564.00 I  0.085324 0.000032  0.259733 0.000030  I-0.1093006 0.0000053  0.0391 0.0037  I  -111.510    0.486    -5.368    0.150  0.085353  0.259707 -0.1093060  -111.400    -5.371  
-211217 59565.00 I  0.082668 0.000032  0.260717 0.000030  I-0.1092647 0.0000054 -0.1352 0.0043  I  -111.309    0.486    -5.432    0.150  0.082621  0.260745 -0.1092661  -111.355    -5.475  
-211218 59566.00 I  0.080323 0.000030  0.261287 0.000028  I-0.1090409 0.0000067 -0.2772 0.0036  I  -111.058    0.486    -5.638    0.150  0.080179  0.261328 -0.1090678  -111.129    -5.691  
-211219 59567.00 I  0.078759 0.000036  0.261719 0.000033  I-0.1087409 0.0000048 -0.3273 0.0042  I  -110.867    0.696    -5.856    0.099  0.078732  0.261660 -0.1087469  -110.910    -5.904  
-211220 59568.00 I  0.077308 0.000035  0.262553 0.000034  I-0.1083881 0.0000049 -0.3721 0.0032  I  -110.735    0.696    -5.951    0.099  0.077355  0.262569 -0.1083780  -110.743    -5.989  
-211221 59569.00 I  0.075376 0.000026  0.263490 0.000026  I-0.1079985 0.0000043 -0.4117 0.0032  I  -110.577    0.698    -5.935    0.051  0.075405  0.263444 -0.1079991  -110.539    -5.957  
-211222 59570.00 I  0.073157 0.000025  0.264268 0.000026  I-0.1075939 0.0000040 -0.3638 0.0029  I  -110.343    0.698    -5.915    0.051  0.073133  0.264278 -0.1076234  -110.373    -5.927  
-211223 59571.00 I  0.070906 0.000025  0.265177 0.000026  I-0.1073204 0.0000038 -0.1674 0.0028  I  -110.040    0.698    -5.934    0.051  0.070881  0.265173 -0.1073418  -110.167    -5.926  
-211224 59572.00 I  0.068527 0.000026  0.266504 0.000028  I-0.1072576 0.0000038  0.0244 0.0029  I  -109.302    0.322    -6.229    0.160  0.068514  0.266510 -0.1072445  -109.820    -5.942  
-211225 59573.00 I  0.066137 0.000017  0.267799 0.000020  I-0.1073724 0.0000045  0.2257 0.0025  I  -109.009    0.322    -6.115    0.160  0.066054  0.267813 -0.1073681  -109.476    -5.912  
-211226 59574.00 I  0.064276 0.000024  0.268995 0.000036  I-0.1077247 0.0000031  0.4741 0.0028  I  -108.951    0.879    -6.014    0.333  0.064264  0.268977 -0.1077173  -109.284    -5.893  
-211227 59575.00 I  0.062755 0.000025  0.270350 0.000034  I-0.1082854 0.0000033  0.6168 0.0021  I  -109.120    0.879    -5.996    0.333  0.062771  0.270366 -0.1082590  -109.258    -5.955  
-211228 59576.00 I  0.061073 0.000032  0.271940 0.000046  I-0.1089206 0.0000028  0.6463 0.0022  I  -109.409    0.740    -5.972    0.320  0.061119  0.271893 -0.1089162  -109.321    -6.008  
-211229 59577.00 I  0.059246 0.000032  0.273457 0.000045  I-0.1095562 0.0000028  0.6103 0.0019  I  -109.787    0.740    -5.788    0.320  0.059184  0.273531 -0.1095688  -109.829    -5.847  
-211230 59578.00 I  0.057741 0.000032  0.274734 0.000045  I-0.1100986 0.0000027  0.4464 0.0020  I  -110.724    0.150    -5.506    0.299  0.057753  0.274728 -0.1101029  -110.666    -5.562  
-211231 59579.00 I  0.056257 0.000032  0.275941 0.000045  I-0.1104198 0.0000028  0.1948 0.0032  I  -111.345    0.150    -5.371    0.299  0.056304  0.275973 -0.1104355  -111.412    -5.426  
-22 1 1 59580.00 I  0.054645 0.000027  0.276988 0.000036  I-0.1104946 0.0000059 -0.0377 0.0030  I  -111.826    0.150    -5.524    0.299  0.054574  0.276983 -0.1105197  -111.899    -5.573  
-22 1 2 59581.00 I  0.053441 0.000029  0.277925 0.000037  I-0.1103623 0.0000052 -0.2166 0.0044  I  -111.797    0.316    -5.758    0.223  0.053381  0.277886 -0.1103891  -111.877    -5.801  
-22 1 3 59582.00 I  0.052975 0.000020  0.279046 0.000022  I-0.1101105 0.0000066 -0.2481 0.0042  I  -111.314    0.338    -5.830    0.175  0.052855  0.278999 -0.1101398  -111.401    -5.868  
-22 1 4 59583.00 I  0.053258 0.000020  0.280688 0.000023  I-0.1099154 0.0000067 -0.1315 0.0044  I  -110.721    0.338    -5.796    0.175  0.053294  0.280607 -0.1099190  -110.807    -5.829  
-22 1 5 59584.00 I  0.053466 0.000021  0.282938 0.000022  I-0.1098783 0.0000057  0.0775 0.0044  I  -110.221    0.400    -5.847    0.149  0.053559  0.282963 -0.1098692  -110.307    -5.882  
-22 1 6 59585.00 I  0.052942 0.000021  0.285051 0.000022  I-0.1100614 0.0000058  0.2596 0.0040  I  -109.851    0.400    -5.934    0.149  0.053042  0.285048 -0.1100259  -109.937    -5.974  
-22 1 7 59586.00 I  0.051786 0.000020  0.286927 0.000017  I-0.1103699 0.0000055  0.3590 0.0044  I  -109.691    0.400    -5.815    0.149  0.051849  0.286983 -0.1103610  -109.778    -5.861  
-22 1 8 59587.00 I  0.050225 0.000015  0.288664 0.000011  I-0.1107735 0.0000066  0.4405 0.0038  I  -109.807    0.474    -5.434    0.112  0.050225  0.288671 -0.1107892  -109.885    -5.484  
-22 1 9 59588.00 I  0.048620 0.000022  0.290199 0.000015  I-0.1112177 0.0000051  0.4222 0.0042  I  -110.085    0.666    -5.046    0.077  0.048602  0.290231 -0.1112277  -110.147    -5.099  
-22 110 59589.00 I  0.047147 0.000022  0.291462 0.000014  I-0.1115966 0.0000051  0.3401 0.0041  I  -110.337    0.666    -4.909    0.077  0.047155  0.291472 -0.1116091  -110.373    -4.960  
-22 111 59590.00 I  0.045618 0.000022  0.292582 0.000013  I-0.1118671 0.0000063  0.1657 0.0036  I  -110.469    0.740    -4.985    0.028  0.045595  0.292576 -0.1118697  -110.484    -5.049  
-22 112 59591.00 I  0.044275 0.000023  0.293451 0.000014  I-0.1119276 0.0000050 -0.0100 0.0041  I  -110.608    0.660    -5.145    0.053  0.044205  0.293449 -0.1119606  -110.597    -5.195  
-22 113 59592.00 I  0.043440 0.000024  0.294436 0.000014  I-0.1118568 0.0000052 -0.1566 0.0035  I  -110.612    0.660    -5.231    0.053  0.043394  0.294345 -0.1118677  -110.603    -5.273  
-22 114 59593.00 I  0.043159 0.000023  0.295887 0.000015  I-0.1115914 0.0000050 -0.3721 0.0041  I  -110.445    0.660    -5.319    0.053  0.043106  0.295839 -0.1115941  -110.438    -5.353  
-22 115 59594.00 I  0.043041 0.000020  0.297886 0.000012  I-0.1111325 0.0000064 -0.5279 0.0040  I  -110.205    0.575    -5.508    0.069  0.043114  0.297844 -0.1111643  -110.195    -5.540  
-22 116 59595.00 I  0.042499 0.000023  0.299850 0.000013  I-0.1105758 0.0000063 -0.5632 0.0040  I  -110.046    0.575    -5.758    0.069  0.042534  0.299918 -0.1106129  -110.039    -5.787  
-22 117 59596.00 I  0.041459 0.000025  0.301463 0.000014  I-0.1099959 0.0000049 -0.6290 0.0043  I  -109.983    0.501    -5.927    0.124  0.041549  0.301463 -0.1100064  -109.987    -5.955  
-22 118 59597.00 I  0.039933 0.000023  0.302935 0.000014  I-0.1093453 0.0000058 -0.6122 0.0031  I  -109.869    0.374    -5.944    0.164  0.039912  0.303016 -0.1093760  -109.902    -5.973  
-22 119 59598.00 I  0.038545 0.000025  0.303983 0.000014  I-0.1088136 0.0000037 -0.4690 0.0034  I  -109.593    0.464    -5.875    0.198  0.038420  0.303951 -0.1088179  -109.671    -5.907  
-22 120 59599.00 I  0.037865 0.000025  0.305015 0.000013  I-0.1084263 0.0000035 -0.2689 0.0023  I  -109.227    0.464    -5.821    0.198  0.037831  0.305025 -0.1084531  -109.285    -5.871  
-22 121 59600.00 I  0.037465 0.000023  0.306190 0.000012  I-0.1082832 0.0000028 -0.0467 0.0023  I  -108.950    0.464    -5.816    0.198  0.037456  0.306196 -0.1082981  -108.956    -5.893  
-22 122 59601.00 I  0.036910 0.000019  0.307343 0.000011  I-0.1083078 0.0000030  0.1003 0.0019  I  -108.860    0.464    -5.827    0.198  0.036968  0.307328 -0.1083306  -108.866    -5.897  
-22 123 59602.00 I  0.035920 0.000022  0.308663 0.000009  I-0.1084800 0.0000026  0.2360 0.0020  I  -108.910    0.396    -5.823    0.181  0.036011  0.308634 -0.1085119  -108.922    -5.877  
-22 124 59603.00 I  0.034432 0.000022  0.310115 0.000009  I-0.1087505 0.0000027  0.2840 0.0027  I  -109.027    0.396    -5.800    0.181  0.034458  0.310100 -0.1087689  -109.048    -5.839  
-22 125 59604.00 I  0.032762 0.000020  0.311545 0.000007  I-0.1090158 0.0000047  0.2355 0.0023  I  -109.178    0.269    -5.738    0.125  0.032747  0.311519 -0.1090294  -109.241    -5.759  
-22 126 59605.00 I  0.031385 0.000023  0.312797 0.000014  I-0.1092023 0.0000036  0.1293 0.0030  I  -109.365    0.421    -5.619    0.157  0.031327  0.312793 -0.1092242  -109.416    -5.652  
-22 127 59606.00 I  0.030246 0.000025  0.314129 0.000015  I-0.1092558 0.0000038 -0.0329 0.0026  I  -109.655    0.421    -5.500    0.157  0.030254  0.314102 -0.1092764  -109.698    -5.548  
-22 128 59607.00 I  0.029127 0.000025  0.315661 0.000015  I-0.1091244 0.0000037 -0.2314 0.0031  I  -109.981    0.563    -5.525    0.185  0.029060  0.315654 -0.1091370  -110.085    -5.577  
-22 129 59608.00 I  0.028298 0.000019  0.317152 0.000015  I-0.1088013 0.0000048 -0.4049 0.0025  I  -110.443    0.563    -5.741    0.185  0.028306  0.317130 -0.1088191  -110.488    -5.790  
-22 130 59609.00 I  0.027570 0.000024  0.318998 0.000019  I-0.1083404 0.0000033 -0.5010 0.0029  I  -110.599    0.461    -6.021    0.198  0.027664  0.318978 -0.1083658  -110.627    -6.064  
-22 131 59610.00 I  0.026683 0.000024  0.320951 0.000019  I-0.1078341 0.0000034 -0.4927 0.0025  I  -110.410    0.461    -6.182    0.198  0.026619  0.320963 -0.1078483  -110.424    -6.222  
-22 2 1 59611.00 I  0.026120 0.000021  0.323090 0.000015  I-0.1073939 0.0000037 -0.3676 0.0024  I  -110.025    0.395    -6.224    0.209  0.026102  0.323015 -0.1073994  -110.029    -6.256  
-22 2 2 59612.00 I  0.025848 0.000020  0.325440 0.000015  I-0.1071280 0.0000034 -0.1551 0.0026  I  -109.557    0.397    -6.236    0.225  0.025834  0.325489 -0.1071431  -109.538    -6.310  
-22 2 3 59613.00 I  0.025709 0.000021  0.327756 0.000014  I-0.1070840 0.0000037  0.0583 0.0026  I  -109.168    0.397    -6.270    0.225  0.025683  0.327751 -0.1070987  -109.116    -6.393  
-22 2 4 59614.00 I  0.025775 0.000020  0.329989 0.000014  I-0.1072185 0.0000040  0.1935 0.0037  I  -109.000    0.397    -6.201    0.225  0.025779  0.330022 -0.1072225  -108.919    -6.381  
-22 2 5 59615.00 I  0.025749 0.000015  0.332150 0.000008  I-0.1074256 0.0000065  0.1924 0.0030  I  -109.148    0.439    -5.977    0.284  0.025738  0.332211 -0.1074267  -109.063    -6.141  
-22 2 6 59616.00 I  0.025719 0.000021  0.333907 0.000008  I-0.1075777 0.0000046  0.1143 0.0040  I  -109.520    0.477    -5.750    0.130  0.025676  0.333942 -0.1076113  -109.447    -5.873  
-22 2 7 59617.00 I  0.025702 0.000021  0.335607 0.000008  I-0.1076483 0.0000047  0.0184 0.0036  I  -109.902    0.477    -5.709    0.130  0.025772  0.335603 -0.1076870  -109.853    -5.790  
-22 2 8 59618.00 I  0.025134 0.000020  0.337306 0.000007  I-0.1075833 0.0000055 -0.1713 0.0031  I  -110.126    0.484    -5.837    0.013  0.025193  0.337374 -0.1075919  -110.126    -5.888  
-22 2 9 59619.00 I  0.024112 0.000020  0.338499 0.000007  I-0.1072954 0.0000039 -0.3920 0.0033  I  -110.187    0.502    -6.026    0.021  0.024114  0.338478 -0.1072977  -110.203    -6.067  
-22 210 59620.00 I  0.022891 0.000019  0.339529 0.000007  I-0.1068102 0.0000037 -0.5800 0.0027  I  -110.037    0.502    -6.107    0.021  0.022952  0.339544 -0.1067962  -110.062    -6.157  
-22 211 59621.00 I  0.021292 0.000019  0.340652 0.000007  I-0.1061227 0.0000036 -0.8061 0.0025  I  -109.675    0.502    -6.143    0.021  0.021317  0.340636 -0.1061126  -109.706    -6.193  
-22 212 59622.00 I  0.019528 0.000014  0.341941 0.000008  I-0.1052490 0.0000035 -0.8793 0.0025  I  -109.225    0.542    -6.268    0.027  0.019510  0.341957 -0.1052912  -109.259    -6.321  
-22 213 59623.00 I  0.018053 0.000016  0.343130 0.000010  I-0.1044122 0.0000035 -0.8084 0.0024  I  -108.888    0.571    -6.506    0.097  0.017952  0.343165 -0.1044265  -108.917    -6.560  
-22 214 59624.00 I  0.017241 0.000016  0.344307 0.000010  I-0.1036357 0.0000034 -0.7272 0.0028  I  -108.746    0.571    -6.738    0.097  0.017178  0.344276 -0.1036375  -108.763    -6.785  
-22 215 59625.00 I  0.016798 0.000015  0.345873 0.000010  I-0.1029904 0.0000044 -0.5481 0.0026  I  -108.687    0.593    -6.834    0.133  0.016814  0.345848 -0.1029937  -108.690    -6.864  
-22 216 59626.00 I  0.016421 0.000022  0.347660 0.000013  I-0.1025441 0.0000039 -0.3550 0.0029  I  -108.562    0.565    -6.770    0.218  0.016373  0.347600 -0.1025279  -108.569    -6.803  
-22 217 59627.00 I  0.016159 0.000022  0.349967 0.000013  I-0.1022883 0.0000039 -0.1382 0.0028  I  -108.360    0.565    -6.659    0.218  0.016174  0.349955 -0.1022855  -108.379    -6.702  
-22 218 59628.00 I  0.015966 0.000020  0.352553 0.000012  I-0.1022741 0.0000039  0.0976 0.0031  I  -108.215    0.565    -6.612    0.218  0.015893  0.352552 -0.1022778  -108.238    -6.679  
-22 219 59629.00 I  0.016039 0.000018  0.354982 0.000013  I-0.1024662 0.0000047  0.2814 0.0029  I  -108.224    0.540    -6.649    0.274  0.016057  0.355009 -0.1024803  -108.239    -6.688  
-22 220 59630.00 I  0.016151 0.000029  0.357317 0.000016  I-0.1028123 0.0000042  0.3915 0.0031  I  -108.366    0.515    -6.713    0.218  0.016152  0.357350 -0.1028229  -108.367    -6.714  
-22 221 59631.00 I  0.016267 0.000030  0.359419 0.000016  I-0.1032028 0.0000041  0.3625 0.0033  I  -108.582    0.515    -6.731    0.218  0.016225  0.359459 -0.1032042  -108.568    -6.699  
-22 222 59632.00 I  0.016726 0.000027  0.361250 0.000014  I-0.1035161 0.0000050  0.2701 0.0027  I  -108.840    0.439    -6.683    0.064  0.016672  0.361277 -0.1035256  -108.817    -6.617  
-22 223 59633.00 I  0.017620 0.000030  0.362774 0.000014  I-0.1037175 0.0000034  0.1014 0.0031  I  -109.095    0.443    -6.615    0.146  0.017619  0.362779 -0.1037081  -109.078    -6.583  
-22 224 59634.00 I  0.018442 0.000030  0.364353 0.000015  I-0.1036983 0.0000035 -0.1292 0.0023  I  -109.261    0.443    -6.601    0.146  0.018496  0.364360 -0.1036928  -109.259    -6.613  
-22 225 59635.00 I  0.018979 0.000030  0.365795 0.000013  I-0.1034719 0.0000031 -0.3215 0.0025  I  -109.219    0.448    -6.729    0.192  0.018931  0.365807 -0.1034734  -109.270    -6.743  
-22 226 59636.00 I  0.019617 0.000020  0.367246 0.000008  I-0.1030795 0.0000035 -0.4411 0.0025  I  -109.056    0.448    -6.878    0.192  0.019607  0.367229 -0.1031018  -109.106    -6.902  
-22 227 59637.00 I  0.020237 0.000029  0.368838 0.000010  I-0.1026452 0.0000038 -0.3943 0.0026  I  -108.805    0.418    -7.028    0.155  0.020241  0.368836 -0.1026797  -108.854    -7.042  
-22 228 59638.00 I  0.020644 0.000029  0.370619 0.000011  I-0.1023227 0.0000039 -0.2523 0.0031  I  -108.575    0.418    -7.105    0.155  0.020656  0.370624 -0.1023250  -108.624    -7.107  
-22 3 1 59639.00 I  0.020988 0.000025  0.372332 0.000010  I-0.1021455 0.0000048 -0.0956 0.0029  I  -108.412    0.383    -7.117    0.104  0.020909  0.372342 -0.1021425  -108.462    -7.107  
-22 3 2 59640.00 I  0.021874 0.000028  0.374021 0.000013  I-0.1021639 0.0000043  0.1583 0.0032  I  -108.285    0.490    -7.126    0.107  0.021778  0.373951 -0.1021944  -108.199    -7.104  
-22 3 3 59641.00 I  0.023306 0.000028  0.376267 0.000013  I-0.1024453 0.0000043  0.3616 0.0030  I  -108.155    0.490    -7.153    0.107  0.023290  0.376273 -0.1024561  -107.898    -7.117  
-22 3 4 59642.00 I  0.025006 0.000028  0.378497 0.000013  I-0.1028385 0.0000043  0.4190 0.0038  I  -108.032    0.762    -7.162    0.115  0.024972  0.378479 -0.1028435  -107.637    -7.109  
-22 3 5 59643.00 I  0.026706 0.000017  0.380551 0.000010  I-0.1032447 0.0000062  0.3607 0.0029  I  -108.082    0.762    -7.127    0.115  0.026774  0.380581 -0.1032424  -107.706    -7.086  
-22 3 6 59644.00 I  0.028126 0.000021  0.382624 0.000013  I-0.1035428 0.0000038  0.2512 0.0036  I  -108.304    0.501    -7.110    0.073  0.028086  0.382600 -0.1035550  -108.027    -7.094  
-22 3 7 59645.00 I  0.029547 0.000020  0.384741 0.000013  I-0.1037273 0.0000038  0.0823 0.0025  I  -108.610    0.501    -7.183    0.073  0.029543  0.384798 -0.1037203  -108.450    -7.191  
-22 3 8 59646.00 I  0.030999 0.000016  0.386703 0.000011  I-0.1036821 0.0000034 -0.1627 0.0024  I  -108.843    0.446    -7.322    0.060  0.031018  0.386712 -0.1036844  -108.826    -7.354  
-22 3 9 59647.00 I  0.032216 0.000019  0.388513 0.000016  I-0.1034078 0.0000028 -0.3902 0.0022  I  -108.861    0.640    -7.427    0.047  0.032281  0.388541 -0.1034089  -108.866    -7.460  
-22 310 59648.00 I  0.033082 0.000019  0.390308 0.000016  I-0.1029230 0.0000027 -0.5539 0.0020  I  -108.353    0.785    -7.426    0.029  0.033104  0.390312 -0.1029383  -108.612    -7.475  
-22 311 59649.00 I  0.033672 0.000020  0.392121 0.000016  I-0.1023276 0.0000028 -0.6347 0.0022  I  -108.004    0.785    -7.446    0.029  0.033708  0.392105 -0.1023346  -108.109    -7.473  
-22 312 59650.00 I  0.034135 0.000018  0.393692 0.000015  I-0.1016713 0.0000035 -0.6624 0.0026  I  -107.521    0.785    -7.560    0.029  0.034130  0.393729 -0.1016864  -107.569    -7.581  
-22 313 59651.00 I  0.034427 0.000025  0.395170 0.000020  I-0.1010163 0.0000044 -0.6498 0.0028  I  -107.088    0.707    -7.795    0.042  0.034502  0.395152 -0.1010372  -107.117    -7.813  
-22 314 59652.00 I  0.034370 0.000025  0.396639 0.000019  I-0.1003898 0.0000043 -0.5831 0.0038  I  -106.859    0.707    -8.049    0.042  0.034354  0.396685 -0.1004104  -106.877    -8.063  
-22 315 59653.00 I  0.034234 0.000023  0.398079 0.000015  I-0.0998758 0.0000061 -0.4393 0.0032  I  -106.880    0.600    -8.182    0.052  0.034250  0.398014 -0.0998830  -106.865    -8.198  
-22 316 59654.00 I  0.033955 0.000033  0.399537 0.000017  I-0.0995328 0.0000048 -0.2306 0.0039  I  -106.947    0.617    -8.164    0.103  0.033972  0.399563 -0.0995467  -106.918    -8.181  
-22 317 59655.00 I  0.033459 0.000033  0.401249 0.000017  I-0.0994310 0.0000047  0.0273 0.0035  I  -106.984    0.617    -8.037    0.103  0.033426  0.401244 -0.0994339  -106.930    -8.064  
-22 318 59656.00 I  0.033076 0.000031  0.402918 0.000017  I-0.0995526 0.0000051  0.1808 0.0034  I  -106.956    0.617    -7.907    0.103  0.033046  0.402931 -0.0995428  -106.876    -7.950  
-22 319 59657.00 I  0.032925 0.000027  0.404429 0.000011  I-0.0997804 0.0000048  0.2976 0.0035  I  -106.959    0.659    -7.852    0.165  0.032894  0.404430 -0.0998242  -106.884    -7.889  
-22 320 59658.00 I  0.033031 0.000027  0.405970 0.000011  I-0.1001533 0.0000047  0.4307 0.0032  I  -107.117    0.659    -7.890    0.165  0.033017  0.405997 -0.1001905  -107.059    -7.919  
-22 321 59659.00 I  0.033373 0.000033  0.407434 0.000014  I-0.1005689 0.0000043  0.3449 0.0036  I  -107.450    0.572    -7.980    0.111  0.033291  0.407432 -0.1005194  -107.409    -8.005  
-22 322 59660.00 I  0.034272 0.000023  0.408886 0.000011  I-0.1007884 0.0000054  0.0948 0.0031  I  -107.861    0.530    -8.021    0.068  0.034163  0.408866 -0.1007374  -107.806    -8.084  
-22 323 59661.00 I  0.035752 0.000024  0.410767 0.000016  I-0.1007727 0.0000045 -0.1128 0.0035  I  -108.093    0.497    -8.079    0.071  0.035739  0.410677 -0.1007668  -108.069    -8.122  
-22 324 59662.00 I  0.037151 0.000025  0.412868 0.000016  I-0.1005690 0.0000044 -0.3019 0.0031  I  -108.064    0.497    -8.114    0.071  0.037184  0.412921 -0.1005632  -108.121    -8.146  
-22 325 59663.00 I  0.038266 0.000024  0.415015 0.000016  I-0.1001862 0.0000042 -0.4391 0.0031  I  -107.764    0.497    -8.165    0.071  0.038276  0.415002 -0.1001852  -107.917    -8.187  
-22 326 59664.00 I  0.039265 0.000024  0.416908 0.000016  I-0.0997291 0.0000044 -0.4614 0.0032  I  -107.290    0.497    -8.243    0.071  0.039275  0.416959 -0.0997325  -107.413    -8.263  
-22 327 59665.00 I  0.040351 0.000019  0.418580 0.000015  I-0.0993023 0.0000047 -0.3669 0.0032  I  -106.799    0.538    -8.326    0.085  0.040293  0.418593 -0.0993188  -106.847    -8.345  
-22 328 59666.00 I  0.041640 0.000019  0.420162 0.000016  I-0.0990358 0.0000047 -0.1510 0.0038  I  -106.438    0.538    -8.391    0.085  0.041691  0.420175 -0.0990554  -106.412    -8.410  
-22 329 59667.00 I  0.042745 0.000018  0.421729 0.000012  I-0.0989806 0.0000059  0.0057 0.0033  I  -106.254    0.660    -8.423    0.077  0.042792  0.421696 -0.0989777  -106.189    -8.449  
-22 330 59668.00 I  0.043409 0.000021  0.423077 0.000019  I-0.0990310 0.0000047  0.1139 0.0039  I  -106.308    0.629    -8.427    0.080  0.043491  0.423055 -0.0990426  -106.244    -8.453  
-22 331 59669.00 I  0.043548 0.000022  0.424808 0.000019  I-0.0992196 0.0000050  0.2557 0.0035  I  -106.436    0.629    -8.386    0.080  0.043570  0.424794 -0.0992346  -106.398    -8.414  
-22 4 1 59670.00 I  0.043351 0.000023  0.426970 0.000020  I-0.0995107 0.0000051  0.3023 0.0038  I  -106.519    0.629    -8.310    0.080  0.043301  0.426919 -0.0995031  -106.506    -8.343  
-22 4 2 59671.00 I  0.043555 0.000018  0.428883 0.000018  I-0.0997950 0.0000058  0.2613 0.0041  I  -106.531    0.585    -8.249    0.083  0.043471  0.428898 -0.0997958  -106.536    -8.278  
-22 4 3 59672.00 I  0.044381 0.000021  0.431006 0.000020  I-0.1000069 0.0000064  0.1413 0.0043  I  -106.561    0.574    -8.269    0.062  0.044401  0.430964 -0.1000185  -106.583    -8.291  
-22 4 4 59673.00 I  0.045130 0.000020  0.433541 0.000020  I-0.1000660 0.0000063 -0.0133 0.0052  I  -106.688    0.574    -8.380    0.062  0.045179  0.433548 -0.1000877  -106.727    -8.395  
-22 4 5 59674.00 I  0.045606 0.000016  0.436188 0.000014  I-0.0999593 0.0000081 -0.2308 0.0049  I  -106.866    0.565    -8.510    0.032  0.045558  0.436184 -0.0999601  -106.928    -8.515  
-22 4 6 59675.00 I  0.046388 0.000019  0.438250 0.000020  I-0.0996011 0.0000075 -0.4581 0.0055  I  -107.021    0.620    -8.581    0.039  0.046324  0.438296 -0.0996161  -107.011    -8.588  
-22 4 7 59676.00 I  0.047706 0.000019  0.440056 0.000020  I-0.0990861 0.0000074 -0.5566 0.0053  I  -106.894    0.620    -8.605    0.039  0.047660  0.440084 -0.0991087  -106.904    -8.610  
-22 4 8 59677.00 I  0.049433 0.000018  0.441874 0.000019  I-0.0985111 0.0000074 -0.5857 0.0053  I  -106.565    0.620    -8.665    0.039  0.049412  0.441800 -0.0985116  -106.602    -8.670  
-22 4 9 59678.00 I  0.051231 0.000015  0.443552 0.000017  I-0.0979307 0.0000077 -0.5669 0.0050  I  -106.083    0.620    -8.840    0.039  0.051279  0.443588 -0.0979207  -106.131    -8.844  
-22 410 59679.00 I  0.052565 0.000016  0.445332 0.000019  I-0.0973866 0.0000066 -0.5204 0.0051  I  -105.529    0.786    -9.102    0.045  0.052631  0.445310 -0.0973816  -105.574    -9.106  
-22 411 59680.00 I  0.053446 0.000015  0.447041 0.000018  I-0.0969113 0.0000066 -0.4098 0.0041  I  -105.062    0.786    -9.348    0.045  0.053447  0.447037 -0.0969159  -105.095    -9.347  
-22 412 59681.00 I  0.054290 0.000013  0.449062 0.000017  I-0.0965831 0.0000048 -0.2510 0.0038  I  -104.883    0.835    -9.501    0.112  0.054284  0.449011 -0.0965845  -104.884    -9.491  
-22 413 59682.00 I  0.055326 0.000011  0.451035 0.000017  I-0.0964339 0.0000039 -0.0184 0.0033  I  -105.048    0.835    -9.551    0.112  0.055292  0.451073 -0.0964523  -105.062    -9.565  
-22 414 59683.00 I  0.056533 0.000011  0.452915 0.000017  I-0.0965583 0.0000044  0.2502 0.0029  I  -105.349    0.835    -9.493    0.112  0.056547  0.452892 -0.0965557  -105.379    -9.547  
-22 415 59684.00 I  0.057880 0.000015  0.454454 0.000018  I-0.0969079 0.0000043  0.4396 0.0030  I  -105.523    0.835    -9.313    0.112  0.057823  0.454485 -0.0968994  -105.550    -9.362  
-22 416 59685.00 I  0.059422 0.000018  0.456174 0.000016  I-0.0974121 0.0000042  0.5529 0.0031  I  -105.584    0.778    -9.059    0.154  0.059424  0.456172 -0.0974129  -105.603    -9.095  
-22 417 59686.00 I  0.061286 0.000020  0.457791 0.000016  I-0.0979771 0.0000044  0.5563 0.0043  I  -105.790    0.778    -8.874    0.154  0.061164  0.457851 -0.0979865  -105.807    -8.908  
-22 418 59687.00 I  0.063721 0.000022  0.459297 0.000016  I-0.0984833 0.0000074  0.4355 0.0043  I  -106.252    0.806    -8.891    0.015  0.063734  0.459266 -0.0985020  -106.274    -8.922  
-22 419 59688.00 I  0.066169 0.000023  0.460809 0.000016  I-0.0988174 0.0000075  0.2225 0.0042  I  -106.782    0.806    -8.999    0.015  0.066192  0.460869 -0.0988272  -106.773    -9.104  
-22 420 59689.00 I  0.068331 0.000027  0.462008 0.000026  I-0.0989000 0.0000041 -0.0756 0.0043  I  -106.912    0.792    -9.262    0.084  0.068329  0.461999 -0.0988949  -106.960    -9.291  
-22 421 59690.00 I  0.070493 0.000026  0.463048 0.000026  I-0.0986843 0.0000043 -0.3196 0.0032  I  -106.641    0.792    -9.418    0.084  0.070468  0.463064 -0.0987060  -106.695    -9.434  
-22 422 59691.00 I  0.072758 0.000023  0.464119 0.000027  I-0.0983194 0.0000049 -0.3878 0.0033  I  -106.179    0.792    -9.477    0.084  0.072707  0.464098 -0.0983386  -106.211    -9.508  
-22 423 59692.00 I  0.075224 0.000022  0.465083 0.000026  I-0.0979269 0.0000049 -0.4013 0.0037  I  -105.765    0.792    -9.509    0.084  0.075204  0.465058 -0.0979051  -105.797    -9.527  
-22 424 59693.00 I  0.077856 0.000017  0.466283 0.000040  I-0.0975412 0.0000056 -0.3417 0.0037  I  -105.469    0.768    -9.550    0.101  0.077859  0.466247 -0.0975194  -105.498    -9.555  
-22 425 59694.00 I  0.080485 0.000015  0.467920 0.000040  I-0.0972766 0.0000056 -0.1828 0.0055  I  -105.250    0.768    -9.589    0.101  0.080557  0.467896 -0.0972632  -105.265    -9.590  
-22 426 59695.00 I  0.082817 0.000012  0.469862 0.000035  I-0.0971782 0.0000095 -0.0162 0.0040  I  -105.105    0.734    -9.598    0.070  0.082859  0.469891 -0.0971847  -105.109    -9.593  
-22 427 59696.00 I  0.084841 0.000019  0.471453 0.000035  I-0.0972281 0.0000058  0.1021 0.0055  I  -105.009    0.749    -9.695    0.183  0.084908  0.471486 -0.0972203  -105.096    -9.548  
-22 428 59697.00 I  0.086493 0.000020  0.472743 0.000035  I-0.0973574 0.0000055  0.1456 0.0043  I  -105.194    0.749    -9.487    0.183  0.086518  0.472819 -0.0973522  -105.258    -9.407  
-22 429 59698.00 I  0.087931 0.000020  0.473543 0.000036  I-0.0974953 0.0000063  0.1172 0.0041  I  -105.450    0.749    -9.213    0.183  0.087895  0.473595 -0.0974914  -105.480    -9.203  
-22 430 59699.00 I  0.089677 0.000019  0.474074 0.000012  I-0.0975714 0.0000060  0.0277 0.0043  I  -105.613    0.749    -8.997    0.183  0.089653  0.474104 -0.0975559  -105.614    -9.011  
-22 5 1 59700.00 I  0.091698 0.000020  0.474621 0.000014  I-0.0975428 0.0000060 -0.0854 0.0043  I  -105.650    0.749    -8.968    0.183  0.091728  0.474632 -0.0975257  -105.627    -8.987  
-22 5 2 59701.00 I  0.093634 0.000024  0.475316 0.000020  I-0.0974058 0.0000062 -0.1830 0.0046  I  -105.655    0.749    -9.133    0.116  0.093634  0.475311 -0.0974187  -105.619    -9.154  
-22 5 3 59702.00 I  0.095564 0.000018  0.476114 0.000019  I-0.0971898 0.0000071 -0.2415 0.0044  I  -105.768    0.749    -9.322    0.030  0.095563  0.476140 -0.0972185  -105.662    -9.372  
-22 5 4 59703.00 I  0.097693 0.000023  0.476934 0.000028  I-0.0969120 0.0000062 -0.3323 0.0047  I  -105.769    0.784    -9.473    0.037  0.097691  0.476906 -0.0969126  -105.734    -9.493  
-22 5 5 59704.00 I  0.099820 0.000023  0.477875 0.000028  I-0.0965122 0.0000061 -0.4620 0.0044  I  -105.743    0.784    -9.518    0.037  0.099882  0.477903 -0.0964992  -105.770    -9.526  
-22 5 6 59705.00 I  0.101675 0.000024  0.478832 0.000028  I-0.0960243 0.0000062 -0.4827 0.0043  I  -105.687    0.784    -9.589    0.037  0.101687  0.478833 -0.0960256  -105.754    -9.581  
-22 5 7 59706.00 I  0.103386 0.000024  0.479498 0.000027  I-0.0955680 0.0000062 -0.4398 0.0040  I  -105.566    0.784    -9.779    0.037  0.103404  0.479538 -0.0955546  -105.646    -9.779  
-22 5 8 59707.00 I  0.105106 0.000024  0.480063 0.000027  I-0.0951539 0.0000051 -0.3692 0.0040  I  -105.288    0.796   -10.022    0.102  0.105117  0.480078 -0.0951550  -105.347   -10.030  
-22 5 9 59708.00 I  0.106695 0.000024  0.480513 0.000027  I-0.0948662 0.0000052 -0.1889 0.0036  I  -104.882    0.796   -10.188    0.102  0.106699  0.480537 -0.0949242  -104.904   -10.197  
-22 510 59709.00 I  0.108521 0.000019  0.480972 0.000018  I-0.0947986 0.0000052  0.0589 0.0032  I  -104.620    0.772   -10.247    0.139  0.108427  0.480933 -0.0948334  -104.607   -10.261  
-22 511 59710.00 I  0.110913 0.000019  0.481771 0.000026  I-0.0949978 0.0000037  0.3482 0.0033  I  -104.755    0.770   -10.274    0.158  0.110941  0.481776 -0.0950144  -104.732   -10.281  
-22 512 59711.00 I  0.113494 0.000018  0.482666 0.000026  I-0.0954644 0.0000041  0.5456 0.0031  I  -105.181    0.770   -10.282    0.158  0.113474  0.482707 -0.0954543  -105.174   -10.290  
-22 513 59712.00 I  0.116069 0.000018  0.483382 0.000026  I-0.0960614 0.0000049  0.6602 0.0037  I  -105.540    0.770   -10.144    0.158  0.116107  0.483379 -0.0960629  -105.566   -10.162  
-22 514 59713.00 I  0.118511 0.000014  0.483943 0.000022  I-0.0967523 0.0000061  0.6771 0.0039  I  -105.727    0.768    -9.783    0.175  0.118527  0.483975 -0.0967431  -105.773    -9.799  
-22 515 59714.00 I  0.120714 0.000021  0.484477 0.000032  I-0.0973746 0.0000061  0.5708 0.0044  I  -106.021    0.850    -9.387    0.156  0.120799  0.484444 -0.0973670  -106.086    -9.399  
-22 516 59715.00 I  0.122296 0.000022  0.485288 0.000031  I-0.0978782 0.0000063  0.4175 0.0059  I  -106.570    0.850    -9.269    0.156  0.122385  0.485333 -0.0978659  -106.653    -9.281  
-22 517 59716.00 I  0.123269 0.000023  0.485820 0.000026  I-0.0981864 0.0000101  0.1947 0.0061  I  -107.056    0.996    -9.503    0.128  0.123240  0.485912 -0.0981728  -107.146    -9.513  
-22 518 59717.00 I  0.124657 0.000028  0.485658 0.000040  I-0.0982697 0.0000105 -0.0217 0.0073  I  -107.060    1.005    -9.843    0.134  0.124614  0.485666 -0.0982338  -107.148    -9.846  
-22 519 59718.00 I  0.126490 0.000027  0.485546 0.000040  I-0.0981577 0.0000105 -0.1941 0.0075  I  -106.590    1.005   -10.040    0.134  0.126492  0.485563 -0.0980742  -106.655   -10.034  
-22 520 59719.00 I  0.128445 0.000027  0.485604 0.000040  I-0.0979282 0.0000107 -0.2265 0.0081  I  -106.038    1.005   -10.084    0.134  0.128370  0.485536 -0.0979421  -106.062   -10.068  
-22 521 59720.00 I  0.130661 0.000022  0.486032 0.000033  I-0.0977464 0.0000123 -0.1338 0.0070  I  -105.740    1.028   -10.086    0.145  0.130677  0.486020 -0.0977739  -105.765   -10.071  
-22 522 59721.00 I  0.132973 0.000026  0.486744 0.000042  I-0.0976766 0.0000089  0.0069 0.0076  I  -105.718    0.874   -10.069    0.090  0.132949  0.486774 -0.0977075  -105.758   -10.059  
-22 523 59722.00 I  0.135353 0.000027  0.487369 0.000041  I-0.0977620 0.0000088  0.1529 0.0060  I  -105.790    0.874    -9.981    0.090  0.135359  0.487350 -0.0977582  -105.848    -9.982  
-22 524 59723.00 I  0.137677 0.000021  0.488142 0.000028  I-0.0979664 0.0000080  0.2508 0.0055  I  -105.807    0.828    -9.816    0.055  0.137703  0.488205 -0.0979698  -105.891    -9.829  
-22 525 59724.00 I  0.139652 0.000023  0.488534 0.000038  I-0.0982380 0.0000066  0.2718 0.0052  I  -105.793    0.868    -9.608    0.057  0.139642  0.488593 -0.0982642  -105.852    -9.614  
-22 526 59725.00 I  0.141660 0.000022  0.488494 0.000037  I-0.0984839 0.0000065  0.2145 0.0046  I  -105.887    0.868    -9.368    0.057  0.141637  0.488529 -0.0985094  -105.918    -9.361  
-22 527 59726.00 I  0.143579 0.000023  0.488465 0.000037  I-0.0986409 0.0000065  0.0790 0.0046  I  -106.147    0.868    -9.110    0.057  0.143638  0.488445 -0.0986407  -106.153    -9.084  
-22 528 59727.00 I  0.145156 0.000017  0.488364 0.000028  I-0.0986084 0.0000066 -0.1571 0.0047  I  -106.453    0.896    -8.928    0.059  0.145102  0.488400 -0.0986068  -106.467    -8.914  
-22 529 59728.00 I  0.146684 0.000016  0.488245 0.000029  I-0.0983139 0.0000067 -0.4317 0.0045  I  -106.638    0.896    -8.971    0.059  0.146706  0.488268 -0.0983314  -106.669    -8.976  
-22 530 59729.00 I  0.148142 0.000026  0.487967 0.000040  I-0.0977447 0.0000060 -0.7073 0.0048  I  -106.661    0.852    -9.278    0.044  0.148067  0.488086 -0.0977877  -106.716    -9.292  
-22 531 59730.00 I  0.149845 0.000024  0.487088 0.000030  I-0.0969122 0.0000070 -0.9442 0.0042  I  -106.606    0.791    -9.683    0.022  0.149795  0.487092 -0.0969563  -106.700    -9.703  
-22 6 1 59731.00 I  0.152003 0.000030  0.486176 0.000040  I-0.0958955 0.0000059 -1.0635 0.0047  I  -106.570    0.998    -9.951    0.041  0.151943  0.486170 -0.0959109  -106.731    -9.971  
-22 6 2 59732.00 I  0.154335 0.000030  0.485423 0.000040  I-0.0947983 0.0000062 -1.1436 0.0045  I  -106.608    0.998   -10.005    0.041  0.154357  0.485426 -0.0947757  -106.670   -10.005  
-22 6 3 59733.00 I  0.156609 0.000030  0.484774 0.000040  I-0.0936396 0.0000068 -1.1300 0.0046  I  -106.745    0.998    -9.979    0.041  0.156589  0.484781 -0.0936356  -106.660    -9.955  
-22 6 4 59734.00 I  0.158876 0.000030  0.484145 0.000039  I-0.0925763 0.0000067 -1.0026 0.0051  I  -106.915    0.998   -10.015    0.041  0.158889  0.484149 -0.0925602  -106.851    -9.984  
-22 6 5 59735.00 I  0.161158 0.000021  0.483621 0.000028  I-0.0916251 0.0000077 -0.9033 0.0047  I  -106.933    1.250   -10.088    0.057  0.161161  0.483622 -0.0916220  -106.921   -10.058  
-22 6 6 59736.00 I  0.163475 0.000027  0.483151 0.000034  I-0.0907856 0.0000065 -0.7563 0.0053  I  -106.704    1.009   -10.069    0.084  0.163382  0.483150 -0.0908246  -106.715   -10.044  
-22 6 7 59737.00 I  0.166257 0.000021  0.482841 0.000020  I-0.0901365 0.0000073 -0.5372 0.0046  I  -106.450    0.875    -9.939    0.099  0.166198  0.482812 -0.0901686  -106.474    -9.925  
-22 6 8 59738.00 I  0.169366 0.000026  0.482835 0.000040  I-0.0896850 0.0000065 -0.3968 0.0049  I  -106.534    0.903    -9.832    0.086  0.169346  0.482843 -0.0896819  -106.581    -9.834  
-22 6 9 59739.00 I  0.172337 0.000026  0.482859 0.000041  I-0.0893321 0.0000066 -0.2888 0.0046  I  -107.025    0.903    -9.819    0.086  0.172338  0.482895 -0.0893344  -107.056    -9.817  
-22 610 59740.00 I  0.175171 0.000026  0.482888 0.000041  I-0.0890948 0.0000066 -0.2185 0.0047  I  -107.638    0.903    -9.757    0.086  0.175150  0.482907 -0.0890843  -107.652    -9.745  
-22 611 59741.00 I  0.177826 0.000026  0.482630 0.000041  I-0.0888495 0.0000068 -0.2850 0.0044  I  -108.183    0.903    -9.475    0.086  0.177834  0.482720 -0.0888551  -108.201    -9.465  
-22 612 59742.00 I  0.180320 0.000022  0.481995 0.000044  I-0.0884938 0.0000057 -0.4446 0.0044  I  -108.787    0.773    -9.089    0.090  0.180290  0.482016 -0.0885165  -108.809    -9.083  
-22 613 59743.00 I  0.182802 0.000022  0.481217 0.000044  I-0.0879285 0.0000056 -0.6998 0.0041  I  -109.509    0.773    -8.953    0.090  0.182826  0.481258 -0.0879480  -109.531    -8.942  
-22 614 59744.00 I  0.185077 0.000015  0.480375 0.000026  I-0.0870865 0.0000059 -0.9782 0.0039  I  -109.999    0.690    -9.207    0.105  0.185100  0.480403 -0.0870940  -110.036    -9.188  
-22 615 59745.00 I  0.187071 0.000035  0.479276 0.000036  I-0.0859924 0.0000055 -1.1956 0.0040  I  -109.879    0.704    -9.596    0.140  0.187052  0.479331 -0.0859830  -109.873    -9.588  
-22 616 59746.00 I  0.189198 0.000035  0.478011 0.000036  I-0.0847403 0.0000055 -1.2779 0.0039  I  -109.275    0.704    -9.827    0.140  0.189149  0.478024 -0.0847332  -109.222    -9.837  
-22 617 59747.00 I  0.191615 0.000034  0.476726 0.000036  I-0.0834987 0.0000056 -1.1739 0.0049  I  -108.682    0.704    -9.900    0.140  0.191602  0.476728 -0.0834949  -108.594    -9.934  
-22 618 59748.00 I  0.194038 0.000033  0.475538 0.000027  I-0.0824295 0.0000081 -0.9590 0.0054  I  -108.441    0.837    -9.953    0.222  0.194019  0.475550 -0.0824189  -108.365    -9.983  
-22 619 59749.00 I  0.196593 0.000033  0.474522 0.000027  I-0.0815734 0.0000092 -0.7660 0.0051  I  -108.557    0.837    -9.955    0.222  0.196541  0.474534 -0.0815575  -108.509    -9.976  
-22 620 59750.00 I  0.199463 0.000034  0.473569 0.000034  I-0.0808815 0.0000062 -0.6210 0.0055  I  -108.866    0.811    -9.778    0.159  0.199454  0.473574 -0.0808812  -108.836    -9.796  
-22 621 59751.00 I  0.202394 0.000012  0.472814 0.000023  I-0.0803065 0.0000059 -0.5505 0.0039  I  -109.178    0.808    -9.449    0.137  0.202403  0.472799 -0.0803109  -109.153    -9.467  
-22 622 59752.00 I  0.205097 0.000015  0.472255 0.000027  I-0.0797506 0.0000047 -0.5695 0.0038  I  -109.380    0.719    -9.158    0.135  0.205128  0.472282 -0.0797589  -109.347    -9.174  
-22 623 59753.00 I  0.207617 0.000016  0.471607 0.000028  I-0.0791244 0.0000049 -0.7179 0.0034  I  -109.530    0.719    -9.018    0.135  0.207619  0.471645 -0.0791011  -109.587    -9.025  
-22 624 59754.00 I  0.210143 0.000016  0.470771 0.000028  I-0.0783038 0.0000050 -0.8994 0.0035  I  -109.778    0.719    -8.977    0.135  0.210148  0.470821 -0.0782976  -109.961    -8.971  
-22 625 59755.00 I  0.212734 0.000017  0.469692 0.000028  I-0.0773338 0.0000050 -1.0563 0.0034  I  -110.138    0.719    -8.983    0.135  0.212693  0.469719 -0.0773260  -110.305    -8.982  
-22 626 59756.00 I  0.215401 0.000023  0.468441 0.000029  I-0.0761717 0.0000047 -1.2717 0.0035  I  -110.451    0.782    -9.101    0.139  0.215376  0.468485 -0.0761726  -110.571    -9.112  
-22 627 59757.00 I  0.218222 0.000023  0.467029 0.000028  I-0.0748150 0.0000048 -1.4135 0.0038  I  -110.567    0.782    -9.404    0.139  0.218164  0.467038 -0.0748406  -110.659    -9.428  
-22 628 59758.00 I  0.221337 0.000021  0.465597 0.000025  I-0.0733612 0.0000059 -1.5060 0.0040  I  -110.511    0.910    -9.793    0.144  0.221330  0.465623 -0.0733645  -110.576    -9.834  
-22 629 59759.00 I  0.224404 0.000022  0.464144 0.000038  I-0.0718062 0.0000065 -1.5888 0.0046  I  -110.442    0.947   -10.029    0.126  0.224443  0.464165 -0.0718011  -110.473   -10.052  
-22 630 59760.00 I  0.227228 0.000022  0.462598 0.000037  I-0.0702106 0.0000070 -1.5905 0.0048  I  -110.497    0.947    -9.980    0.126  0.227220  0.462671 -0.0702118  -110.474    -9.975  
-22 7 1 59761.00 I  0.230018 0.000022  0.460847 0.000037  I-0.0686600 0.0000072 -1.4877 0.0066  I  -110.702    0.947    -9.762    0.126  0.230002  0.460818 -0.0686663  -110.599    -9.722  
-22 7 2 59762.00 I  0.232934 0.000011  0.459215 0.000031  I-0.0672413 0.0000112 -1.3666 0.0058  I  -110.971    1.012    -9.589    0.082  0.232881  0.459225 -0.0672447  -110.959    -9.582  
-22 7 3 59763.00 I  0.236097 0.000015  0.457823 0.000041  I-0.0659489 0.0000092 -1.1791 0.0072  I  -111.139    0.873    -9.533    0.141  0.236109  0.457809 -0.0659625  -111.150    -9.536  
-22 7 4 59764.00 I  0.239191 0.000015  0.456540 0.000041  I-0.0649152 0.0000090 -0.8952 0.0058  I  -111.087    0.873    -9.489    0.141  0.239234  0.456579 -0.0649159  -111.121    -9.498  
-22 7 5 59765.00 I  0.241894 0.000013  0.455121 0.000035  I-0.0641419 0.0000071 -0.6611 0.0055  I  -110.909    0.820    -9.377    0.171  0.241892  0.455171 -0.0641393  -110.976    -9.390  
-22 7 6 59766.00 I  0.244459 0.000013  0.453293 0.000035  I-0.0635565 0.0000062 -0.5367 0.0047  I  -110.895    0.820    -9.260    0.171  0.244450  0.453302 -0.0635337  -110.950    -9.262  
-22 7 7 59767.00 I  0.247125 0.000013  0.451608 0.000035  I-0.0630515 0.0000063 -0.4635 0.0045  I  -111.265    0.820    -9.234    0.171  0.247124  0.451582 -0.0630501  -111.305    -9.226  
-22 7 8 59768.00 I  0.249746 0.000013  0.450109 0.000035  I-0.0625980 0.0000065 -0.4849 0.0047  I  -111.936    0.820    -9.243    0.171  0.249756  0.450120 -0.0625785  -111.978    -9.228  
-22 7 9 59769.00 I  0.252293 0.000009  0.448653 0.000024  I-0.0620342 0.0000071 -0.6487 0.0038  I  -112.679    0.877    -9.148    0.179  0.252297  0.448682 -0.0620271  -112.723    -9.129  
-22 710 59770.00 I  0.254694 0.000016  0.447028 0.000025  I-0.0612804 0.0000041 -0.8730 0.0043  I  -113.384    0.803    -8.978    0.143  0.254733  0.447060 -0.0612967  -113.423    -8.960  
-22 711 59771.00 I  0.256802 0.000016  0.445401 0.000017  I-0.0602885 0.0000047 -1.0964 0.0031  I  -113.968    0.771    -8.954    0.116  0.256857  0.445395 -0.0603249  -114.007    -8.936  
-22 712 59772.00 I  0.258321 0.000016  0.443917 0.000017  I-0.0591181 0.0000047 -1.2284 0.0030  I  -114.198    0.771    -9.167    0.116  0.258411  0.443974 -0.0591324  -114.246    -9.142  
-22 713 59773.00 I  0.259223 0.000017  0.442026 0.000020  I-0.0578283 0.0000036 -1.3707 0.0030  I  -113.927    0.783    -9.408    0.153  0.259174  0.442066 -0.0577813  -113.960    -9.403  
-22 714 59774.00 I  0.260256 0.000017  0.439915 0.000020  I-0.0564435 0.0000037 -1.3125 0.0027  I  -113.400    0.783    -9.465    0.153  0.260201  0.439888 -0.0564587  -113.418    -9.484  
-22 715 59775.00 I  0.261705 0.000018  0.438129 0.000019  I-0.0552624 0.0000039 -1.0771 0.0035  I  -113.026    0.783    -9.419    0.153  0.261642  0.438122 -0.0552630  -113.037    -9.466  
-22 716 59776.00 I  0.263451 0.000013  0.436348 0.000018  I-0.0542796 0.0000060 -0.8709 0.0028  I  -112.968    0.808    -9.461    0.195  0.263441  0.436373 -0.0542876  -112.983    -9.496  
-22 717 59777.00 I  0.265296 0.000017  0.434376 0.000019  I-0.0535139 0.0000041 -0.6849 0.0036  I  -113.148    0.864    -9.533    0.136  0.265267  0.434398 -0.0535228  -113.161    -9.544  
-22 718 59778.00 I  0.267260 0.000017  0.432334 0.000019  I-0.0528829 0.0000040 -0.5796 0.0030  I  -113.506    0.864    -9.412    0.136  0.267234  0.432352 -0.0528927  -113.506    -9.398  
-22 719 59779.00 I  0.269239 0.000018  0.430284 0.000014  I-0.0523133 0.0000045 -0.5983 0.0029  I  -113.980    0.894    -9.083    0.066  0.269260  0.430298 -0.0523068  -113.947    -9.037  
-22 720 59780.00 I  0.270985 0.000025  0.428191 0.000029  I-0.0516616 0.0000041 -0.6910 0.0031  I  -114.405    0.821    -8.812    0.126  0.270974  0.428173 -0.0516628  -114.393    -8.784  
-22 721 59781.00 I  0.272566 0.000025  0.426252 0.000029  I-0.0509179 0.0000043 -0.8240 0.0030  I  -114.656    0.821    -8.809    0.126  0.272574  0.426255 -0.0508922  -114.674    -8.805  
-22 722 59782.00 I  0.274104 0.000025  0.424462 0.000030  I-0.0499879 0.0000045 -1.0342 0.0040  I  -114.827    0.821    -9.000    0.126  0.274053  0.424453 -0.0499591  -114.884    -9.018  
-22 723 59783.00 I  0.275661 0.000023  0.422673 0.000029  I-0.0488633 0.0000067 -1.2030 0.0038  I  -115.067    0.680    -9.188    0.176  0.275681  0.422673 -0.0488673  -115.096    -9.210  
-22 724 59784.00 I  0.277055 0.000023  0.420910 0.000035  I-0.0475897 0.0000060 -1.3483 0.0045  I  -115.345    0.776    -9.320    0.182  0.277006  0.420915 -0.0476028  -115.333    -9.343  
-22 725 59785.00 I  0.278485 0.000023  0.419325 0.000035  I-0.0461859 0.0000059 -1.4360 0.0050  I  -115.499    0.776    -9.490    0.182  0.278471  0.419285 -0.0462003  -115.452    -9.519  
-22 726 59786.00 I  0.279855 0.000014  0.417904 0.000025  I-0.0447445 0.0000081 -1.4434 0.0052  I  -115.482    0.870    -9.729    0.190  0.279867  0.417962 -0.0447491  -115.399    -9.768  
-22 727 59787.00 I  0.281074 0.000023  0.416119 0.000039  I-0.0433006 0.0000085 -1.4464 0.0061  I  -115.416    0.830    -9.901    0.179  0.281044  0.416126 -0.0432579  -115.379    -9.934  
-22 728 59788.00 I  0.282268 0.000023  0.414141 0.000038  I-0.0418516 0.0000092 -1.4497 0.0070  I  -115.407    0.830    -9.846    0.179  0.282267  0.414205 -0.0417953  -115.431    -9.867  
-22 729 59789.00 I  0.283372 0.000022  0.411848 0.000038  I-0.0404325 0.0000110 -1.3592 0.0099  I  -115.450    0.830    -9.591    0.179  0.283345  0.411841 -0.0404282  -115.538    -9.595  
-22 730 59790.00 I  0.284624 0.000021  0.409427 0.000032  I-0.0391818 0.0000176 -1.1231 0.0076  I  -115.480    0.671    -9.336    0.152  0.284587  0.409400 -0.0392089  -115.593    -9.353  
-22 731 59791.00 I  0.285988 0.000025  0.407284 0.000041  I-0.0381746 0.0000106 -0.9222 0.0103  I  -115.462    0.777    -9.233    0.276  0.286000  0.407286 -0.0381849  -115.593    -9.273  
-22 8 1 59792.00 I  0.287130 0.000025  0.405197 0.000041  I-0.0373422 0.0000106 -0.7071 0.0069  I  -115.386    0.777    -9.258    0.276  0.287161  0.405194 -0.0373892  -115.536    -9.320  
-22 8 2 59793.00 I  0.287887 0.000019  0.403236 0.000032  I-0.0367520 0.0000088 -0.5173 0.0067  I  -115.276    0.760    -9.287    0.277  0.287882  0.403262 -0.0367846  -115.439    -9.376  
-22 8 3 59794.00 I  0.288545 0.000019  0.400998 0.000032  I-0.0362649 0.0000083 -0.4555 0.0057  I  -115.252    0.760    -9.257    0.277  0.288468  0.401019 -0.0362792  -115.414    -9.314  
-22 8 4 59795.00 I  0.289527 0.000019  0.398720 0.000032  I-0.0358182 0.0000073 -0.4622 0.0055  I  -115.487    0.760    -9.205    0.277  0.289489  0.398709 -0.0358145  -115.635    -9.222  
-22 8 5 59796.00 I  0.290537 0.000019  0.396553 0.000032  I-0.0353212 0.0000071 -0.5267 0.0052  I  -116.042    0.760    -9.178    0.277  0.290582  0.396579 -0.0353263  -116.154    -9.192  
-22 8 6 59797.00 I  0.291094 0.000015  0.394196 0.000017  I-0.0347348 0.0000073 -0.6811 0.0044  I  -116.770    0.717    -9.180    0.251  0.291080  0.394221 -0.0347316  -116.838    -9.204  
-22 8 7 59798.00 I  0.291547 0.000021  0.391643 0.000021  I-0.0339400 0.0000051 -0.8924 0.0047  I  -117.409    0.700    -9.226    0.255  0.291487  0.391652 -0.0339451  -117.435    -9.261  
-22 8 8 59799.00 I  0.292337 0.000019  0.389021 0.000014  I-0.0329727 0.0000058 -1.0355 0.0039  I  -117.721    0.685    -9.357    0.258  0.292293  0.389056 -0.0329721  -117.715    -9.399  
-22 8 9 59800.00 I  0.293210 0.000019  0.386220 0.000014  I-0.0318941 0.0000058 -1.1033 0.0037  I  -117.606    0.685    -9.522    0.258  0.293211  0.386232 -0.0318918  -117.585    -9.565  
-22 810 59801.00 I  0.293834 0.000021  0.383251 0.000026  I-0.0308088 0.0000045 -1.0429 0.0039  I  -117.203    0.743    -9.547    0.269  0.293803  0.383250 -0.0308088  -117.149    -9.591  
-22 811 59802.00 I  0.294451 0.000021  0.380334 0.000027  I-0.0298560 0.0000051 -0.8392 0.0036  I  -116.848    0.743    -9.351    0.269  0.294459  0.380298 -0.0298577  -116.770    -9.397  
-22 812 59803.00 I  0.295060 0.000021  0.377818 0.000027  I-0.0291390 0.0000057 -0.6096 0.0043  I  -116.775    0.743    -9.119    0.269  0.295055  0.377755 -0.0291384  -116.681    -9.171  
-22 813 59804.00 I  0.295579 0.000015  0.375709 0.000025  I-0.0286243 0.0000068 -0.4175 0.0043  I  -116.899    0.780    -9.088    0.278  0.295537  0.375740 -0.0286307  -116.834    -9.134  
-22 814 59805.00 I  0.296373 0.000014  0.373568 0.000025  I-0.0282807 0.0000064 -0.2951 0.0046  I  -117.030    0.780    -9.221    0.278  0.296313  0.373591 -0.0282983  -117.006    -9.266  
-22 815 59806.00 I  0.297512 0.000015  0.371304 0.000029  I-0.0279871 0.0000063 -0.3135 0.0063  I  -117.197    0.779    -9.253    0.230  0.297500  0.371314 -0.0279699  -117.203    -9.307  
-22 816 59807.00 I  0.298550 0.000014  0.369042 0.000019  I-0.0276157 0.0000109 -0.4460 0.0065  I  -117.539    0.779    -9.067    0.125  0.298583  0.369059 -0.0276395  -117.555    -9.139  
-22 817 59808.00 I  0.299277 0.000019  0.366742 0.000030  I-0.0270844 0.0000113 -0.6108 0.0079  I  -118.002    0.760    -8.854    0.125  0.299254  0.366732 -0.0270866  -118.003    -8.949  
-22 818 59809.00 I  0.299910 0.000020  0.364400 0.000031  I-0.0263631 0.0000113 -0.8687 0.0080  I  -118.372    0.760    -8.839    0.125  0.299866  0.364425 -0.0263517  -118.274    -8.865  
-22 819 59810.00 I  0.300903 0.000020  0.362025 0.000030  I-0.0253588 0.0000113 -1.0911 0.0082  I  -118.565    0.760    -9.005    0.125  0.300823  0.362010 -0.0253455  -118.335    -8.928  
-22 820 59811.00 I  0.302125 0.000020  0.359758 0.000030  I-0.0241914 0.0000118 -1.2820 0.0072  I  -118.671    0.760    -9.157    0.125  0.302176  0.359779 -0.0241871  -118.439    -9.105  
-22 821 59812.00 I  0.303009 0.000024  0.357421 0.000041  I-0.0228181 0.0000089 -1.4029 0.0073  I  -118.741    0.614    -9.190    0.108  0.302992  0.357455 -0.0228266  -118.572    -9.196  
-22 822 59813.00 I  0.303768 0.000023  0.354930 0.000041  I-0.0214185 0.0000086 -1.4250 0.0057  I  -118.710    0.614    -9.194    0.108  0.303769  0.354926 -0.0213929  -118.632    -9.243  
-22 823 59814.00 I  0.304486 0.000019  0.352484 0.000034  I-0.0199966 0.0000072 -1.3617 0.0051  I  -118.540    0.616    -9.291    0.104  0.304513  0.352500 -0.0199836  -118.587    -9.375  
-22 824 59815.00 I  0.304888 0.000018  0.349901 0.000039  I-0.0187067 0.0000056 -1.2635 0.0046  I  -118.308    0.714    -9.444    0.131  0.304896  0.349874 -0.0186613  -118.307    -9.531  
-22 825 59816.00 I  0.305185 0.000018  0.347450 0.000039  I-0.0174471 0.0000057 -1.2329 0.0040  I  -118.108    0.714    -9.494    0.131  0.305201  0.347486 -0.0174037  -118.023    -9.577  
-22 826 59817.00 I  0.305355 0.000017  0.344923 0.000039  I-0.0162886 0.0000056 -1.0594 0.0043  I  -117.945    0.714    -9.355    0.131  0.305398  0.344912 -0.0162851  -117.767    -9.438  
-22 827 59818.00 I  0.305270 0.000010  0.342339 0.000023  I-0.0153437 0.0000064 -0.8397 0.0038  I  -117.796    0.895    -9.124    0.159  0.305290  0.342335 -0.0153482  -117.637    -9.193  
-22 828 59819.00 I  0.304966 0.000020  0.339915 0.000030  I-0.0146128 0.0000050 -0.6091 0.0040  I  -117.682    0.774    -8.979    0.178  0.304974  0.339946 -0.0146136  -117.565    -9.035  
-22 829 59820.00 I  0.304625 0.000020  0.337394 0.000030  I-0.0141179 0.0000049 -0.4011 0.0036  I  -117.644    0.774    -9.006    0.178  0.304586  0.337401 -0.0140968  -117.551    -9.055  
-22 830 59821.00 I  0.304499 0.000020  0.334986 0.000023  I-0.0137967 0.0000052 -0.2347 0.0032  I  -117.661    0.717    -9.129    0.191  0.304464  0.334971 -0.0137838  -117.601    -9.176  
-22 831 59822.00 I  0.304617 0.000022  0.332728 0.000027  I-0.0136235 0.0000040 -0.1432 0.0033  I  -117.689    0.747    -9.210    0.165  0.304595  0.332751 -0.0136099  -117.612    -9.248  
-22 9 1 59823.00 I  0.304750 0.000022  0.330386 0.000027  I-0.0134686 0.0000040 -0.1769 0.0032  I  -117.787    0.747    -9.185    0.165  0.304814  0.330440 -0.0134836  -117.693    -9.211  
-22 9 2 59824.00 I  0.304506 0.000022  0.327664 0.000027  I-0.0132464 0.0000050 -0.2806 0.0035  I  -118.070    0.747    -9.105    0.165  0.304501  0.327651 -0.0132494  -118.154    -9.102  
-22 9 3 59825.00 I  0.304210 0.000012  0.325045 0.000017  I-0.0128898 0.0000057 -0.4371 0.0043  I  -118.518    0.778    -9.071    0.133  0.304186  0.324993 -0.0128821  -118.590    -9.080  
-22 9 4 59826.00 I  0.304086 0.000015  0.322759 0.000024  I-0.0123680 0.0000070 -0.6064 0.0046  I  -118.883    0.750    -9.142    0.193  0.304085  0.322764 -0.0123741  -118.929    -9.170  
-22 9 5 59827.00 I  0.303787 0.000015  0.320457 0.000023  I-0.0117011 0.0000071 -0.7036 0.0075  I  -118.886    0.750    -9.281    0.193  0.303820  0.320481 -0.0117203  -118.916    -9.328  
-22 9 6 59828.00 I  0.303228 0.000013  0.317957 0.000019  I-0.0110127 0.0000132 -0.6450 0.0062  I  -118.480    0.719    -9.349    0.246  0.303248  0.318029 -0.0110190  -118.525    -9.426  
-22 9 7 59829.00 I  0.302620 0.000015  0.314925 0.000027  I-0.0104253 0.0000102 -0.5436 0.0082  I  -117.922    0.887    -9.201    0.188  0.302652  0.314951 -0.0103738  -117.930    -9.248  
-22 9 8 59830.00 I  0.301723 0.000016  0.311761 0.000028  I-0.0099629 0.0000096 -0.3300 0.0072  I  -117.587    0.887    -8.846    0.188  0.301793  0.311758 -0.0099952  -117.557    -8.853  
-22 9 9 59831.00 I  0.300345 0.000017  0.308693 0.000029  I-0.0097975 0.0000102 -0.0199 0.0068  I  -117.615    0.887    -8.497    0.188  0.300297  0.308670 -0.0098037  -117.537    -8.461  
-22 910 59832.00 I  0.299161 0.000014  0.305663 0.000024  I-0.0098959 0.0000095  0.2084 0.0058  I  -117.809    1.155    -8.384    0.070  0.299086  0.305665 -0.0098938  -117.785    -8.354  
-22 911 59833.00 I  0.298571 0.000024  0.302851 0.000036  I-0.0101845 0.0000057  0.3472 0.0055  I  -117.910    1.007    -8.507    0.141  0.298524  0.302843 -0.0101991  -117.949    -8.495  
-22 912 59834.00 I  0.298128 0.000024  0.300270 0.000036  I-0.0105524 0.0000057  0.3723 0.0042  I  -117.925    1.007    -8.663    0.141  0.298153  0.300265 -0.0105663  -118.003    -8.665  
-22 913 59835.00 I  0.297554 0.000024  0.297926 0.000032  I-0.0108733 0.0000061  0.2299 0.0037  I  -118.064    0.934    -8.702    0.175  0.297509  0.297897 -0.0108687  -118.179    -8.722  
-22 914 59836.00 I  0.296978 0.000025  0.295807 0.000051  I-0.0109915 0.0000048  0.0255 0.0039  I  -118.399    0.930    -8.680    0.134  0.296992  0.295809 -0.0110048  -118.515    -8.694  
-22 915 59837.00 I  0.296334 0.000024  0.293809 0.000051  I-0.0109042 0.0000048 -0.2391 0.0034  I  -118.757    0.930    -8.727    0.134  0.296326  0.293853 -0.0109071  -118.881    -8.735  
-22 916 59838.00 I  0.295609 0.000024  0.291699 0.000051  I-0.0105277 0.0000047 -0.4605 0.0038  I  -118.920    0.930    -8.843    0.134  0.295633  0.291666 -0.0105453  -119.064    -8.840  
-22 917 59839.00 I  0.294744 0.000015  0.289611 0.000043  I-0.0099915 0.0000060 -0.6569 0.0035  I  -118.830    0.926    -8.901    0.072  0.294765  0.289613 -0.0099966  -118.954    -8.905  
-22 918 59840.00 I  0.293576 0.000020  0.287789 0.000057  I-0.0092321 0.0000052 -0.7987 0.0040  I  -118.558    0.998    -8.833    0.118  0.293594  0.287789 -0.0092502  -118.640    -8.844  
-22 919 59841.00 I  0.292284 0.000020  0.285843 0.000056  I-0.0084342 0.0000052 -0.8200 0.0040  I  -118.193    0.998    -8.730    0.118  0.292235  0.285928 -0.0084134  -118.223    -8.750  
-22 920 59842.00 I  0.291356 0.000020  0.283523 0.000039  I-0.0075715 0.0000060 -0.9029 0.0034  I  -117.817    1.067    -8.733    0.149  0.291284  0.283515 -0.0075559  -117.778    -8.771  
-22 921 59843.00 I  0.290657 0.000020  0.281046 0.000041  I-0.0066827 0.0000045 -0.8228 0.0037  I  -117.525    0.969    -8.846    0.115  0.290675  0.281089 -0.0066950  -117.531    -8.864  
-22 922 59844.00 I  0.289762 0.000020  0.278371 0.000041  I-0.0059697 0.0000043 -0.6114 0.0033  I  -117.370    0.969    -8.933    0.115  0.289785  0.278400 -0.0059969  -117.441    -8.921  
-22 923 59845.00 I  0.288625 0.000019  0.275550 0.000041  I-0.0054453 0.0000048 -0.4437 0.0038  I  -117.323    0.969    -8.862    0.115  0.288673  0.275532 -0.0054471  -117.457    -8.810  
-22 924 59846.00 I  0.287260 0.000013  0.272936 0.000016  I-0.0050917 0.0000063 -0.2478 0.0036  I  -117.318    0.763    -8.654    0.022  0.287244  0.272949 -0.0051006  -117.468    -8.622  
-22 925 59847.00 I  0.285950 0.000027  0.270430 0.000037  I-0.0049465 0.0000053 -0.0616 0.0041  I  -117.333    0.723    -8.458    0.183  0.285878  0.270404 -0.0049635  -117.484    -8.457  
-22 926 59848.00 I  0.285167 0.000027  0.268165 0.000037  I-0.0049530 0.0000054  0.0782 0.0042  I  -117.383    0.723    -8.411    0.183  0.285103  0.268121 -0.0049793  -117.537    -8.441  
-22 927 59849.00 I  0.284710 0.000027  0.266423 0.000035  I-0.0050991 0.0000066  0.2068 0.0039  I  -117.467    0.699    -8.518    0.247  0.284746  0.266357 -0.0051012  -117.616    -8.597  
-22 928 59850.00 I  0.283878 0.000028  0.264922 0.000035  I-0.0053104 0.0000055  0.1669 0.0041  I  -117.563    0.627    -8.651    0.177  0.283878  0.264953 -0.0053014  -117.693    -8.702  
-22 929 59851.00 I  0.283008 0.000027  0.263304 0.000035  I-0.0053959 0.0000048  0.0160 0.0036  I  -117.662    0.627    -8.692    0.177  0.282943  0.263319 -0.0054180  -117.779    -8.707  
-22 930 59852.00 I  0.282323 0.000027  0.261509 0.000035  I-0.0053335 0.0000048 -0.1615 0.0035  I  -117.777    0.627    -8.626    0.177  0.282338  0.261528 -0.0053388  -117.905    -8.603  
-2210 1 59853.00 I  0.281362 0.000013  0.259745 0.000014  I-0.0050469 0.0000050 -0.4171 0.0034  I  -117.856    0.514    -8.539    0.036  0.281388  0.259744 -0.0049041  -117.934    -8.536  
-2210 2 59854.00 I  0.280043 0.000011  0.257883 0.000014  I-0.0045484 0.0000049 -0.5255 0.0033  I  -117.773    0.514    -8.516    0.036  0.280092  0.257931 -0.0043864  -117.763    -8.633  
-2210 3 59855.00 I  0.278450 0.000018  0.255736 0.000015  I-0.0040473 0.0000042 -0.4797 0.0038  I  -117.410    0.880    -8.559    0.121  0.278478  0.255746 -0.0040146  -117.380    -8.681  
-2210 4 59856.00 I  0.276547 0.000017  0.253520 0.000015  I-0.0035919 0.0000057 -0.4253 0.0030  I  -116.810    1.094    -8.579    0.164  0.276607  0.253527 -0.0035590  -116.777    -8.672  
-2210 5 59857.00 I  0.274395 0.000017  0.251432 0.000021  I-0.0032283 0.0000042 -0.2762 0.0037  I  -116.208    1.048    -8.477    0.140  0.274352  0.251450 -0.0032281  -116.158    -8.550  
-2210 6 59858.00 I  0.272446 0.000021  0.249225 0.000021  I-0.0030732 0.0000047 -0.0259 0.0033  I  -115.870    1.048    -8.245    0.140  0.272409  0.249284 -0.0030816  -115.892    -8.306  
-2210 7 59859.00 I  0.270893 0.000024  0.246721 0.000019  I-0.0031814 0.0000050  0.2390 0.0035  I  -115.874    1.048    -7.990    0.140  0.270869  0.246728 -0.0031810  -115.963    -8.047  
-2210 8 59860.00 I  0.269391 0.000024  0.244284 0.000019  I-0.0035376 0.0000051  0.4632 0.0038  I  -116.056    1.048    -7.831    0.140  0.269464  0.244272 -0.0035337  -116.181    -7.889  
-2210 9 59861.00 I  0.267405 0.000019  0.242149 0.000017  I-0.0040729 0.0000057  0.5828 0.0033  I  -116.188    1.007    -7.792    0.112  0.267436  0.242181 -0.0040628  -116.323    -7.852  
-221010 59862.00 I  0.265327 0.000021  0.239992 0.000019  I-0.0046627 0.0000041  0.5811 0.0038  I  -116.197    0.874    -7.809    0.088  0.265240  0.239987 -0.0046541  -116.330    -7.871  
-221011 59863.00 I  0.263669 0.000021  0.237871 0.000012  I-0.0051867 0.0000049  0.4344 0.0031  I  -116.209    0.740    -7.835    0.055  0.263701  0.237885 -0.0051692  -116.344    -7.899  
-221012 59864.00 I  0.262030 0.000020  0.235728 0.000012  I-0.0055025 0.0000047  0.2007 0.0034  I  -116.363    0.783    -7.883    0.043  0.262046  0.235701 -0.0055011  -116.517    -7.950  
-221013 59865.00 I  0.259880 0.000018  0.233780 0.000012  I-0.0055843 0.0000048 -0.0442 0.0034  I  -116.617    0.783    -7.971    0.043  0.260021  0.233734 -0.0055722  -116.707    -8.023  
-221014 59866.00 I  0.256987 0.000018  0.232088 0.000011  I-0.0054363 0.0000050 -0.2223 0.0036  I  -116.775    0.783    -8.050    0.043  0.256936  0.232102 -0.0054362  -116.793    -8.078  
-221015 59867.00 I  0.254059 0.000018  0.230367 0.000011  I-0.0051796 0.0000053 -0.2806 0.0041  I  -116.667    0.783    -8.047    0.043  0.254063  0.230356 -0.0051876  -116.700    -8.075  
-221016 59868.00 I  0.251191 0.000018  0.228842 0.000026  I-0.0048947 0.0000065 -0.2802 0.0042  I  -116.282    0.899    -7.957    0.072  0.251206  0.228893 -0.0049099  -116.365    -7.987  
-221017 59869.00 I  0.248067 0.000022  0.227228 0.000027  I-0.0046551 0.0000064 -0.1722 0.0050  I  -115.751    0.899    -7.886    0.072  0.248052  0.227286 -0.0046783  -115.804    -7.935  
-221018 59870.00 I  0.245191 0.000019  0.225137 0.000028  I-0.0045621 0.0000075 -0.0288 0.0046  I  -115.218    0.932    -7.935    0.095  0.245102  0.225158 -0.0045660  -115.200    -8.015  
-221019 59871.00 I  0.243016 0.000019  0.222944 0.000034  I-0.0045915 0.0000067  0.0966 0.0050  I  -114.761    0.988    -8.084    0.131  0.243041  0.222898 -0.0045814  -114.747    -8.164  
-221020 59872.00 I  0.240704 0.000020  0.221151 0.000034  I-0.0047741 0.0000067  0.2784 0.0047  I  -114.448    0.988    -8.189    0.131  0.240817  0.221191 -0.0047645  -114.446    -8.265  
-221021 59873.00 I  0.237719 0.000020  0.219311 0.000034  I-0.0051506 0.0000065  0.4670 0.0053  I  -114.358    0.988    -8.116    0.131  0.237688  0.219313 -0.0051434  -114.344    -8.197  
-221022 59874.00 I  0.234655 0.000019  0.217534 0.000023  I-0.0057147 0.0000081  0.6755 0.0047  I  -114.523    1.044    -7.860    0.163  0.234606  0.217522 -0.0057243  -114.532    -7.927  
-221023 59875.00 I  0.232019 0.000015  0.216033 0.000026  I-0.0065067 0.0000069  0.8992 0.0054  I  -114.840    0.896    -7.538    0.137  0.231878  0.216031 -0.0064986  -114.866    -7.589  
-221024 59876.00 I  0.230033 0.000016  0.214646 0.000026  I-0.0074623 0.0000070  0.9704 0.0050  I  -115.124    0.896    -7.299    0.137  0.230043  0.214645 -0.0074339  -115.163    -7.341  
-221025 59877.00 I  0.228137 0.000016  0.213211 0.000023  I-0.0084022 0.0000071  0.9057 0.0049  I  -115.259    0.739    -7.232    0.089  0.228137  0.213232 -0.0084121  -115.318    -7.265  
-221026 59878.00 I  0.226079 0.000016  0.211770 0.000023  I-0.0092487 0.0000070  0.7662 0.0050  I  -115.254    0.739    -7.325    0.089  0.226115  0.211747 -0.0092591  -115.297    -7.349  
-221027 59879.00 I  0.223699 0.000015  0.210386 0.000022  I-0.0098858 0.0000070  0.4804 0.0048  I  -115.193    0.739    -7.487    0.089  0.223756  0.210409 -0.0098856  -115.222    -7.492  
-221028 59880.00 I  0.220829 0.000013  0.208851 0.000022  I-0.0102115 0.0000065  0.2004 0.0053  I  -115.115    0.739    -7.601    0.089  0.220823  0.208832 -0.0102779  -115.143    -7.612  
-221029 59881.00 I  0.217712 0.000013  0.207409 0.000017  I-0.0103251 0.0000080  0.0357 0.0043  I  -114.987    0.748    -7.610    0.051  0.217709  0.207418 -0.0103958  -115.022    -7.628  
-221030 59882.00 I  0.214510 0.000016  0.206265 0.000024  I-0.0102979 0.0000056 -0.0839 0.0047  I  -114.767    0.780    -7.555    0.167  0.214473  0.206229 -0.0103095  -114.810    -7.575  
-221031 59883.00 I  0.211392 0.000016  0.205212 0.000019  I-0.0101970 0.0000049 -0.0842 0.0037  I  -114.440    0.806    -7.515    0.226  0.211345  0.205237 -0.0101927  -114.492    -7.538  
-2211 1 59884.00 I  0.208608 0.000017  0.204242 0.000021  I-0.0101874 0.0000048  0.0894 0.0033  I  -114.044    0.806    -7.507    0.226  0.208514  0.204211 -0.0101774  -114.100    -7.544  
-2211 2 59885.00 I  0.206230 0.000018  0.203468 0.000026  I-0.0104119 0.0000044  0.3714 0.0034  I  -113.657    0.829    -7.480    0.192  0.206235  0.203545 -0.0104065  -113.700    -7.501  
-2211 3 59886.00 I  0.203875 0.000019  0.202379 0.000026  I-0.0109487 0.0000047  0.7090 0.0031  I  -113.378    0.829    -7.391    0.192  0.203841  0.202359 -0.0109528  -113.392    -7.399  
-2211 4 59887.00 I  0.201541 0.000018  0.201374 0.000026  I-0.0118055 0.0000044  0.9735 0.0040  I  -113.284    0.829    -7.242    0.192  0.201477  0.201353 -0.0118134  -113.257    -7.249  
-2211 5 59888.00 I  0.199498 0.000014  0.200681 0.000019  I-0.0128218 0.0000065  1.0162 0.0032  I  -113.376    0.852    -7.059    0.145  0.199403  0.200700 -0.0128173  -113.353    -7.066  
-2211 6 59889.00 I  0.197923 0.000015  0.199801 0.000025  I-0.0138077 0.0000046  0.9682 0.0042  I  -113.545    0.736    -6.862    0.097  0.197880  0.199789 -0.0138349  -113.543    -6.869  
-2211 7 59890.00 I  0.196415 0.000015  0.199008 0.000023  I-0.0147317 0.0000053  0.8409 0.0035  I  -113.642    0.736    -6.683    0.097  0.196436  0.198985 -0.0147274  -113.659    -6.688  
-2211 8 59891.00 I  0.194600 0.000028  0.198378 0.000025  I-0.0154512 0.0000053  0.5989 0.0035  I  -113.613    0.662    -6.586    0.027  0.194574  0.198424 -0.0154466  -113.660    -6.582  
-2211 9 59892.00 I  0.192635 0.000027  0.197577 0.000025  I-0.0159477 0.0000047  0.4115 0.0035  I  -113.553    0.662    -6.628    0.027  0.192696  0.197558 -0.0159684  -113.571    -6.657  
-221110 59893.00 I  0.190360 0.000027  0.196720 0.000025  I-0.0162477 0.0000047  0.1447 0.0031  I  -113.575    0.662    -6.785    0.027  0.190367  0.196722 -0.0162302  -113.564    -6.849  
-221111 59894.00 I  0.187844 0.000027  0.195891 0.000025  I-0.0162357 0.0000041 -0.1262 0.0041  I  -113.643    0.662    -6.942    0.027  0.187822  0.195880 -0.0162520  -113.631    -7.013  
-221112 59895.00 I  0.185418 0.000027  0.195030 0.000018  I-0.0160482 0.0000067 -0.2383 0.0029  I  -113.593    0.739    -6.992    0.002  0.185361  0.195076 -0.0160839  -113.596    -7.056  
-221113 59896.00 I  0.183321 0.000028  0.193962 0.000022  I-0.0157851 0.0000040 -0.2724 0.0038  I  -113.330    0.716    -6.948    0.082  0.183217  0.193981 -0.0158151  -113.352    -6.999  
-221114 59897.00 I  0.181908 0.000014  0.192835 0.000015  I-0.0155292 0.0000034 -0.2292 0.0027  I  -112.924    0.714    -6.925    0.090  0.181786  0.192794 -0.0155444  -112.967    -6.958  
-221115 59898.00 I  0.181149 0.000015  0.192237 0.000015  I-0.0153534 0.0000035 -0.1058 0.0026  I  -112.489    0.714    -6.991    0.090  0.181089  0.192167 -0.0153549  -112.549    -7.008  
-221116 59899.00 I  0.180591 0.000016  0.192106 0.000022  I-0.0153326 0.0000039  0.0627 0.0027  I  -112.067    0.740    -7.083    0.128  0.180613  0.192084 -0.0153236  -112.120    -7.099  
-221117 59900.00 I  0.179829 0.000015  0.192248 0.000023  I-0.0154880 0.0000041  0.2587 0.0029  I  -111.705    0.740    -7.070    0.128  0.179894  0.192217 -0.0154871  -111.735    -7.093  
-221118 59901.00 I  0.178495 0.000016  0.192646 0.000023  I-0.0158574 0.0000044  0.4767 0.0041  I  -111.561    0.740    -6.901    0.128  0.178587  0.192658 -0.0158559  -111.559    -6.936  
-221119 59902.00 I  0.176650 0.000012  0.192925 0.000020  I-0.0164185 0.0000070  0.6260 0.0030  I  -111.786    0.775    -6.640    0.159  0.176631  0.192939 -0.0164100  -111.782    -6.671  
-221120 59903.00 I  0.174676 0.000012  0.192883 0.000023  I-0.0171056 0.0000042  0.7640 0.0041  I  -112.281    0.703    -6.374    0.142  0.174678  0.192941 -0.0171134  -112.283    -6.399  
-221121 59904.00 I  0.172507 0.000012  0.192690 0.000023  I-0.0179152 0.0000042  0.8080 0.0029  I  -112.743    0.703    -6.140    0.142  0.172482  0.192686 -0.0178985  -112.747    -6.164  
-221122 59905.00 I  0.170166 0.000011  0.192510 0.000017  I-0.0186674 0.0000040  0.6894 0.0038  I  -112.971    0.650    -5.974    0.128  0.170135  0.192562 -0.0186627  -112.985    -5.999  
-221123 59906.00 I  0.167914 0.000014  0.192110 0.000035  I-0.0192785 0.0000063  0.5243 0.0038  I  -113.013    0.651    -5.963    0.121  0.167864  0.192125 -0.0192839  -113.015    -5.992  
-221124 59907.00 I  0.165798 0.000014  0.191649 0.000035  I-0.0196865 0.0000064  0.2707 0.0046  I  -112.965    0.651    -6.144    0.121  0.165815  0.191634 -0.0196773  -112.960    -6.178  
-221125 59908.00 I  0.163386 0.000014  0.191406 0.000035  I-0.0198180 0.0000066  0.0114 0.0061  I  -112.800    0.651    -6.380    0.121  0.163449  0.191394 -0.0198119  -112.800    -6.422  
-221126 59909.00 I  0.160411 0.000016  0.191123 0.000034  I-0.0197339 0.0000103 -0.1741 0.0060  I  -112.499    0.651    -6.463    0.113  0.160439  0.191188 -0.0197408  -112.502    -6.504  
-221127 59910.00 I  0.156936 0.000016  0.190783 0.000034  I-0.0195087 0.0000100 -0.2429 0.0064  I  -112.172    0.651    -6.353    0.113  0.156985  0.190819 -0.0195486  -112.173    -6.392  
-221128 59911.00 I  0.153234 0.000015  0.190262 0.000036  I-0.0193014 0.0000077 -0.1518 0.0059  I  -111.943    0.736    -6.212    0.087  0.153168  0.190278 -0.0193141  -111.939    -6.246  
-221129 59912.00 I  0.149942 0.000013  0.189790 0.000016  I-0.0192279 0.0000064  0.0078 0.0047  I  -111.811    0.832    -6.175    0.051  0.149881  0.189736 -0.0192085  -111.789    -6.198  
-221130 59913.00 I  0.147025 0.000017  0.189832 0.000022  I-0.0193202 0.0000054  0.1771 0.0041  I  -111.708    0.751    -6.198    0.094  0.146998  0.189837 -0.0193120  -111.648    -6.204  
-2212 1 59914.00 I  0.144055 0.000021  0.190078 0.000022  I-0.0195934 0.0000051  0.3802 0.0037  I  -111.624    0.751    -6.171    0.094  0.144039  0.190129 -0.0196037  -111.563    -6.191  
-2212 2 59915.00 I  0.141127 0.000021  0.189960 0.000023  I-0.0200309 0.0000051  0.4342 0.0036  I  -111.587    0.751    -6.063    0.094  0.141086  0.190030 -0.0200182  -111.557    -6.103  
-2212 3 59916.00 I  0.138501 0.000021  0.189628 0.000025  I-0.0204315 0.0000051  0.3974 0.0035  I  -111.616    0.751    -5.915    0.094  0.138520  0.189588 -0.0204483  -111.593    -5.954  
-2212 4 59917.00 I  0.135670 0.000022  0.189544 0.000025  I-0.0208123 0.0000048  0.3203 0.0036  I  -111.697    0.814    -5.755    0.131  0.135739  0.189603 -0.0208072  -111.696    -5.787  
-2212 5 59918.00 I  0.132719 0.000023  0.189098 0.000025  I-0.0210315 0.0000050  0.1215 0.0035  I  -111.741    0.814    -5.594    0.131  0.132595  0.189132 -0.0210271  -111.763    -5.625  
-2212 6 59919.00 I  0.130243 0.000022  0.188804 0.000021  I-0.0210516 0.0000052 -0.0884 0.0037  I  -111.651    0.986    -5.493    0.142  0.130234  0.188807 -0.0210546  -111.664    -5.528  
-2212 7 59920.00 I  0.127862 0.000020  0.188834 0.000024  I-0.0208560 0.0000054 -0.2943 0.0038  I  -111.477    0.838    -5.541    0.113  0.127804  0.188914 -0.0208636  -111.530    -5.568  
-2212 8 59921.00 I  0.125542 0.000018  0.188710 0.000023  I-0.0204803 0.0000056 -0.4484 0.0040  I  -111.359    0.838    -5.751    0.113  0.125550  0.188683 -0.0204842  -111.431    -5.765  
-2212 9 59922.00 I  0.123013 0.000018  0.188908 0.000021  I-0.0199691 0.0000060 -0.5727 0.0048  I  -111.366    0.838    -6.004    0.113  0.123051  0.188943 -0.0199575  -111.450    -5.997  
-221210 59923.00 I  0.120044 0.000016  0.189244 0.000016  I-0.0193475 0.0000078 -0.6591 0.0045  I  -111.402    0.680    -6.147    0.074  0.120023  0.189212 -0.0193465  -111.433    -6.148  
-221211 59924.00 I  0.117118 0.000016  0.189440 0.000024  I-0.0186861 0.0000068 -0.6399 0.0052  I  -111.327    0.690    -6.155    0.158  0.117059  0.189519 -0.0187186  -111.306    -6.171  
-221212 59925.00 I  0.114540 0.000014  0.189327 0.000024  I-0.0180997 0.0000068 -0.5249 0.0043  I  -111.103    0.690    -6.137    0.158  0.114474  0.189311 -0.0181257  -111.063    -6.164  
-221213 59926.00 I  0.112258 0.000014  0.189386 0.000024  I-0.0176355 0.0000052 -0.4125 0.0042  I  -110.760    0.814    -6.171    0.193  0.112235  0.189380 -0.0176371  -110.733    -6.213  
-221214 59927.00 I  0.110085 0.000014  0.189773 0.000024  I-0.0172856 0.0000048 -0.2675 0.0033  I  -110.321    0.814    -6.189    0.193  0.110057  0.189733 -0.0172887  -110.324    -6.215  
-221215 59928.00 I  0.107805 0.000014  0.190633 0.000023  I-0.0171050 0.0000042 -0.1091 0.0032  I  -109.853    0.814    -6.075    0.193  0.107848  0.190644 -0.0170929  -109.882    -6.084  
-221216 59929.00 I  0.105273 0.000014  0.191581 0.000023  I-0.0170821 0.0000041  0.0935 0.0029  I  -109.577    0.814    -5.844    0.193  0.105276  0.191662 -0.0170407  -109.642    -5.845  
-221217 59930.00 I  0.102628 0.000011  0.192140 0.000016  I-0.0172782 0.0000040  0.2548 0.0030  I  -109.720    0.903    -5.642    0.178  0.102588  0.192217 -0.0171383  -109.796    -5.644  
-221218 59931.00 I  0.100234 0.000024  0.192465 0.000038  I-0.0175404 0.0000044  0.2622 0.0038  I  -110.233    0.796    -5.555    0.137  0.100160  0.192490 -0.0173664  -110.291    -5.561  
-221219 59932.00 I  0.098289 0.000024  0.192767 0.000037  I-0.0177852 0.0000065  0.2174 0.0031  I  -110.806    0.687    -5.485    0.080  0.098210  0.192803 -0.0177187  -110.824    -5.496  
-221220 59933.00 I  0.096780 0.000026  0.193098 0.000038  I-0.0179691 0.0000044  0.1544 0.0040  I  -111.251    0.630    -5.327    0.078  0.096711  0.193084 -0.0179634  -111.212    -5.340  
-221221 59934.00 I  0.095783 0.000025  0.193369 0.000038  I-0.0180904 0.0000046  0.0806 0.0032  I  -111.661    0.630    -5.202    0.078  0.095777  0.193348 -0.0181234  -111.654    -5.239  
-221222 59935.00 I  0.094827 0.000026  0.194012 0.000039  I-0.0181002 0.0000047 -0.0835 0.0033  I  -112.054    0.630    -5.334    0.078  0.094877  0.193950 -0.0181060  -112.105    -5.394  
-221223 59936.00 I  0.093412 0.000028  0.194949 0.000039  I-0.0179153 0.0000048 -0.2719 0.0033  I  -112.156    0.630    -5.688    0.078  0.093472  0.194922 -0.0178955  -112.150    -5.759  
-221224 59937.00 I  0.091300 0.000019  0.196101 0.000017  I-0.0176069 0.0000046 -0.3087 0.0034  I  -111.800    0.565    -5.935    0.075  0.091397  0.196126 -0.0175841  -111.706    -6.007  
-221225 59938.00 I  0.088380 0.000019  0.197002 0.000016  I-0.0173447 0.0000048 -0.2052 0.0040  I  -111.255    0.565    -5.874    0.075  0.088402  0.197099 -0.0173115  -111.094    -5.943  
-221226 59939.00 I  0.085232 0.000042  0.197368 0.000041  I-0.0172486 0.0000065  0.0544 0.0039  I  -110.921    0.578    -5.678    0.166  0.085204  0.197391 -0.0172323  -110.709    -5.742  
-221227 59940.00 I  0.081992 0.000042  0.197787 0.000041  I-0.0174695 0.0000062  0.3618 0.0043  I  -110.868    0.578    -5.599    0.166  0.082060  0.197809 -0.0174541  -110.623    -5.660  
-221228 59941.00 I  0.078272 0.000044  0.198344 0.000042  I-0.0179186 0.0000056  0.5083 0.0042  I  -110.908    0.656    -5.612    0.153  0.078253  0.198379 -0.0179243  -110.647    -5.673  
-221229 59942.00 I  0.074738 0.000043  0.198601 0.000042  I-0.0184525 0.0000057  0.5539 0.0039  I  -110.946    0.656    -5.527    0.153  0.074744  0.198584 -0.0184719  -110.694    -5.570  
-221230 59943.00 I  0.071203 0.000043  0.199206 0.000041  I-0.0190020 0.0000054  0.5263 0.0040  I  -111.033    0.656    -5.313    0.153  0.071281  0.199199 -0.0190102  -110.793    -5.341  
-221231 59944.00 I  0.067041 0.000043  0.200080 0.000041  I-0.0194826 0.0000056  0.4312 0.0044  I  -111.201    0.656    -5.126    0.153  0.067074  0.200103 -0.0194855  -110.973    -5.182  
-23 1 1 59945.00 I  0.062786 0.000019  0.200919 0.000015  I-0.0198272 0.0000070  0.2245 0.0041  I  -111.392    0.715    -5.060    0.140  0.062699  0.200944 -0.0197967  -111.162    -5.163  
-23 1 2 59946.00 I  0.059055 0.000022  0.201756 0.000023  I-0.0199244 0.0000060 -0.0038 0.0054  I  -111.512    0.573    -5.062    0.097  0.059003  0.201796 -0.0199243  -111.443    -5.114  
-23 1 3 59947.00 I  0.055737 0.000019  0.202460 0.000034  I-0.0198275 0.0000082 -0.2084 0.0052  I  -111.468    0.606    -5.076    0.132  0.055638  0.202514 -0.0198250  -111.467    -5.128  
-23 1 4 59948.00 I  0.052977 0.000019  0.203016 0.000035  I-0.0195035 0.0000086 -0.4253 0.0062  I  -111.218    0.606    -5.159    0.132  0.052933  0.202990 -0.0195007  -111.313    -5.194  
-23 1 5 59949.00 I  0.050803 0.000019  0.203873 0.000036  I-0.0190212 0.0000094 -0.5092 0.0064  I  -110.849    0.606    -5.389    0.132  0.050795  0.203830 -0.0190232  -110.822    -5.531  
-23 1 6 59950.00 I  0.048797 0.000020  0.205075 0.000036  I-0.0185021 0.0000094 -0.5419 0.0066  I  -110.558    0.606    -5.685    0.132  0.048795  0.205101 -0.0184663  -110.510    -5.834  
-23 1 7 59951.00 I  0.046882 0.000019  0.206241 0.000036  I-0.0179526 0.0000092 -0.5288 0.0068  I  -110.423    0.606    -5.868    0.132  0.046853  0.206221 -0.0179143  -110.392    -5.984  
-23 1 8 59952.00 I  0.045143 0.000016  0.207584 0.000032  I-0.0174794 0.0000097 -0.4110 0.0063  I  -110.351    0.816    -5.857    0.177  0.045146  0.207590 -0.0174487  -110.316    -5.948  
-23 1 9 59953.00 I  0.043364 0.000011  0.209053 0.000016  I-0.0171413 0.0000085 -0.2612 0.0062  I  -110.218    0.807    -5.747    0.146  0.043370  0.209111 -0.0171274  -110.159    -5.821  
-23 110 59954.00 I  0.041296 0.000010  0.210242 0.000014  I-0.0169624 0.0000077 -0.0953 0.0055  I  -109.979    0.807    -5.670    0.146  0.041325  0.210288 -0.0169671  -109.874    -5.733  
-23 111 59955.00 I  0.038966 0.000015  0.211106 0.000015  I-0.0169542 0.0000070  0.0813 0.0049  I  -109.660    0.754    -5.623    0.124  0.038979  0.211134 -0.0169747  -109.583    -5.665  
-23 112 59956.00 I  0.036561 0.000014  0.211940 0.000014  I-0.0170849 0.0000062  0.1378 0.0048  I  -109.329    0.754    -5.515    0.124  0.036547  0.211915 -0.0170559  -109.296    -5.533  
-23 113 59957.00 I  0.034182 0.000014  0.213038 0.000014  I-0.0172131 0.0000067  0.1441 0.0058  I  -109.127    0.754    -5.352    0.124  0.034173  0.213022 -0.0172046  -109.147    -5.343  
-23 114 59958.00 I  0.031794 0.000013  0.214424 0.000012  I-0.0173788 0.0000099  0.1675 0.0057  I  -109.205    0.669    -5.285    0.088  0.031810  0.214393 -0.0173877  -109.253    -5.273  
-23 115 59959.00 I  0.029348 0.000016  0.216072 0.000021  I-0.0175459 0.0000092  0.1844 0.0069  I  -109.543    0.637    -5.406    0.113  0.029351  0.216047 -0.0175710  -109.621    -5.396  
-23 116 59960.00 I  0.026873 0.000016  0.217964 0.000021  I-0.0177222 0.0000095  0.1250 0.0073  I  -109.926    0.637    -5.573    0.113  0.026882  0.217923 -0.0177110  -110.037    -5.563  
-23 117 59961.00 I  0.024332 0.000012  0.220219 0.000019  I-0.0177507 0.0000113 -0.0702 0.0069  I  -110.264    0.618    -5.570    0.129  0.024343  0.220214 -0.0177400  -110.403    -5.564  
-23 118 59962.00 I  0.021690 0.000039  0.222446 0.000019  I-0.0175804 0.0000101 -0.2696 0.0075  I  -110.745    0.676    -5.451    0.136  0.021681  0.222504 -0.0175873  -110.857    -5.445  
-23 119 59963.00 I  0.019115 0.000040  0.224215 0.000019  I-0.0172297 0.0000099 -0.4145 0.0071  I  -111.420    0.676    -5.517    0.136  0.019078  0.224261 -0.0172362  -111.474    -5.516  
-23 120 59964.00 I  0.016662 0.000040  0.225636 0.000019  I-0.0167588 0.0000100 -0.5373 0.0081  I  -111.874    0.676    -5.878    0.136  0.016715  0.225678 -0.0167521  -111.849    -5.887  
-23 121 59965.00 I  0.013978 0.000039  0.226843 0.000011  I-0.0161726 0.0000127 -0.6075 0.0061  I  -111.678    0.845    -6.222    0.148  0.014033  0.226892 -0.0161896  -111.635    -6.235  
-23 122 59966.00 I  0.010876 0.000040  0.227751 0.000014  I-0.0156157 0.0000070 -0.4620 0.0071  I  -110.999    0.550    -6.219    0.105  0.010879  0.227740 -0.0156593  -110.964    -6.230  
-23 123 59967.00 I  0.007811 0.000040  0.228860 0.000016  I-0.0152836 0.0000065 -0.2114 0.0047  I  -110.402    0.550    -5.967    0.105  0.007728  0.228830 -0.0153087  -110.393    -5.970  
-23 124 59968.00 I  0.005409 0.000019  0.230211 0.000017  I-0.0152061 0.0000062  0.0789 0.0045  I  -110.171    0.354    -5.801    0.066  0.005300  0.230244 -0.0152158  -110.223    -5.787  
-23 125 59969.00 I  0.003919 0.000023  0.231456 0.000027  I-0.0154130 0.0000062  0.2841 0.0044  I  -110.166    0.569    -5.798    0.149  0.003852  0.231401 -0.0153642  -110.193    -5.799  
-23 126 59970.00 I  0.002888 0.000024  0.233326 0.000029  I-0.0156959 0.0000062  0.2542 0.0043  I  -110.256    0.569    -5.755    0.149  0.002927  0.233231 -0.0156349  -110.268    -5.775  
-23 127 59971.00 I  0.001580 0.000024  0.235870 0.000030  I-0.0159008 0.0000061  0.1625 0.0049  I  -110.440    0.569    -5.595    0.149  0.001593  0.235918 -0.0158886  -110.468    -5.635  
-23 128 59972.00 I  0.000382 0.000022  0.238118 0.000030  I-0.0159939 0.0000076 -0.0101 0.0046  I  -110.659    0.709    -5.503    0.193  0.000279  0.238107 -0.0159862  -110.687    -5.537  
-23 129 59973.00 I -0.000272 0.000026  0.240384 0.000033  I-0.0158856 0.0000069 -0.1677 0.0051  I  -110.781    0.831    -5.636    0.183 -0.000230  0.240378 -0.0158927  -110.794    -5.657  
-23 130 59974.00 I -0.000860 0.000025  0.242657 0.000033  I-0.0156618 0.0000067 -0.3155 0.0051  I  -110.771    0.831    -5.890    0.183 -0.000925  0.242670 -0.0156444  -110.750    -5.905  
-23 131 59975.00 I -0.001399 0.000022  0.245014 0.000026  I-0.0152307 0.0000074 -0.5349 0.0045  I  -110.672    1.146    -6.069    0.163 -0.001326  0.244961 -0.0152262  -110.583    -6.080  
-23 2 1 59976.00 I -0.002309 0.000021  0.247812 0.000044  I-0.0146185 0.0000061 -0.6749 0.0048  I  -110.484    1.038    -6.147    0.176 -0.002296  0.247864 -0.0146010  -110.444    -6.163  
-23 2 2 59977.00 I -0.003561 0.000021  0.250311 0.000044  I-0.0138975 0.0000060 -0.7652 0.0044  I  -110.207    1.038    -6.241    0.176 -0.003547  0.250346 -0.0138591  -110.219    -6.262  
-23 2 3 59978.00 I -0.004904 0.000021  0.252506 0.000043  I-0.0131157 0.0000063 -0.7729 0.0046  I  -109.945    1.038    -6.397    0.176 -0.004856  0.252572 -0.0130960  -109.978    -6.426  
-23 2 4 59979.00 I -0.006471 0.000017  0.254279 0.000041  I-0.0124014 0.0000070 -0.6316 0.0041  I  -109.831    0.944    -6.502    0.187 -0.006428  0.254285 -0.0124190  -109.861    -6.529  
-23 2 5 59980.00 I -0.008209 0.000019  0.255937 0.000041  I-0.0118698 0.0000053 -0.4386 0.0044  I  -109.847    0.729    -6.431    0.154 -0.008204  0.255923 -0.0118777  -109.870    -6.457  
-23 2 6 59981.00 I -0.009960 0.000020  0.257733 0.000041  I-0.0115083 0.0000053 -0.2935 0.0037  I  -109.837    0.729    -6.223    0.154 -0.009964  0.257731 -0.0114958  -109.866    -6.252  
-23 2 7 59982.00 I -0.011916 0.000020  0.259667 0.000017  I-0.0112781 0.0000051 -0.1625 0.0032  I  -109.681    0.541    -6.036    0.116 -0.011876  0.259655 -0.0112745  -109.747    -6.070  
-23 2 8 59983.00 I -0.014092 0.000033  0.261639 0.000038  I-0.0111859 0.0000035 -0.0237 0.0030  I  -109.406    0.739    -5.952    0.086 -0.014175  0.261674 -0.0111959  -109.435    -5.978  
-23 2 9 59984.00 I -0.015723 0.000032  0.263453 0.000038  I-0.0112380 0.0000033  0.1369 0.0026  I  -109.143    0.739    -5.925    0.086 -0.015815  0.263434 -0.0112446  -109.132    -5.933  
-23 210 59985.00 I -0.016726 0.000032  0.265588 0.000038  I-0.0114602 0.0000038  0.2991 0.0030  I  -109.016    0.739    -5.905    0.086 -0.016692  0.265519 -0.0114722  -108.968    -5.888  
-23 211 59986.00 I -0.017893 0.000029  0.268005 0.000037  I-0.0117978 0.0000051  0.3462 0.0029  I  -109.087    0.911    -5.946    0.044 -0.017796  0.268043 -0.0117909  -109.040    -5.942  
-23 212 59987.00 I -0.019635 0.000029  0.270435 0.000037  I-0.0121293 0.0000044  0.3233 0.0033  I  -109.309    0.766    -6.118    0.124 -0.019580  0.270405 -0.0121316  -109.260    -6.133  
-23 213 59988.00 I -0.021943 0.000029  0.273088 0.000038  I-0.0124050 0.0000043  0.1823 0.0035  I  -109.543    0.766    -6.351    0.124 -0.021949  0.273140 -0.0123642  -109.473    -6.379  
-23 214 59989.00 I -0.024483 0.000015  0.275695 0.000018  I-0.0124666 0.0000054 -0.0406 0.0036  I  -109.724    0.669    -6.481    0.163 -0.024489  0.275701 -0.0124632  -109.625    -6.523  
-23 215 59990.00 I -0.026965 0.000028  0.278180 0.000020  I-0.0123412 0.0000058 -0.2113 0.0038  I  -109.978    0.644    -6.487    0.150 -0.026961  0.278194 -0.0123539  -109.980    -6.504  
-23 216 59991.00 I -0.029371 0.000027  0.280690 0.000021  I-0.0120580 0.0000054 -0.3399 0.0040  I  -110.405    0.644    -6.569    0.150 -0.029393  0.280732 -0.0120613  -110.553    -6.554  
-23 217 59992.00 I -0.031759 0.000027  0.282893 0.000023  I-0.0116893 0.0000054 -0.3849 0.0048  I  -110.765    0.644    -6.864    0.150 -0.031780  0.282935 -0.0116902  -111.072    -6.818  
-23 218 59993.00 I -0.033991 0.000025  0.284847 0.000023  I-0.0113596 0.0000080 -0.2157 0.0045  I  -110.671    0.401    -7.190    0.084 -0.034066  0.284869 -0.0113623  -110.935    -7.143  
-23 219 59994.00 I -0.035823 0.000032  0.286845 0.000028  I-0.0113099 0.0000071  0.1097 0.0053  I  -110.105    0.723    -7.250    0.201 -0.035884  0.286825 -0.0113117  -110.257    -7.216  
-23 220 59995.00 I -0.037241 0.000031  0.288962 0.000027  I-0.0115759 0.0000071  0.4259 0.0049  I  -109.463    0.723    -7.045    0.201 -0.037338  0.288920 -0.0115669  -109.509    -7.029  
-23 221 59996.00 I -0.038247 0.000021  0.291495 0.000025  I-0.0121535 0.0000067  0.7175 0.0045  I  -109.083    0.769    -6.850    0.230 -0.038274  0.291422 -0.0121587  -109.019    -6.868  
-23 222 59997.00 I -0.038779 0.000023  0.294616 0.000025  I-0.0129450 0.0000055  0.8115 0.0046  I  -108.997    0.742    -6.807    0.179 -0.038866  0.294588 -0.0129291  -108.925    -6.815  
-23 223 59998.00 I -0.038964 0.000025  0.298256 0.000023  I-0.0137345 0.0000062  0.7795 0.0047  I  -109.136    0.742    -6.787    0.179 -0.038960  0.298263 -0.0137066  -109.077    -6.785  
-23 224 59999.00 I -0.039165 0.000025  0.301855 0.000023  I-0.0144986 0.0000077  0.7312 0.0056  I  -109.461    0.742    -6.698    0.179 -0.039119  0.301926 -0.0145020  -109.413    -6.693  
-23 225 60000.00 I -0.039676 0.000017  0.305101 0.000012  I-0.0151484 0.0000094  0.5373 0.0058  I  -109.838    0.661    -6.676    0.065 -0.039564  0.305114 -0.0151424  -109.790    -6.690  
-23 226 60001.00 I -0.040939 0.000021  0.308169 0.000017  I-0.0155416 0.0000087  0.2486 0.0064  I  -110.068    0.721    -6.868    0.058 -0.040856  0.308232 -0.0155421  -110.020    -6.905  
-23 227 60002.00 I -0.042705 0.000021  0.310720 0.000018  I-0.0156487 0.0000088 -0.0309 0.0075  I  -110.088    0.721    -7.181    0.058 -0.042777  0.310760 -0.0156050  -110.045    -7.236  
-23 228 60003.00 I -0.044028 0.000020  0.313321 0.000018  I-0.0155141 0.0000123 -0.2074 0.0064  I  -109.978    0.881    -7.385    0.021 -0.044051  0.313293 -0.0155019  -109.938    -7.454  
-23 3 1 60004.00 I -0.045094 0.000019  0.316290 0.000019  I-0.0152968 0.0000092 -0.1953 0.0072  I  -109.760    0.860    -7.402    0.122 -0.045086  0.316379 -0.0152786  -109.729    -7.431  
-23 3 2 60005.00 I -0.046059 0.000018  0.318742 0.000019  I-0.0151071 0.0000075 -0.2323 0.0058  I  -109.391    0.860    -7.361    0.122 -0.046065  0.318766 -0.0150624  -109.433    -7.347  
-23 3 3 60006.00 I -0.046662 0.000016  0.321114 0.000019  I-0.0148441 0.0000072 -0.2336 0.0051  I  -108.939    0.860    -7.400    0.122 -0.046677  0.321138 -0.0148245  -108.998    -7.328  
-23 3 4 60007.00 I -0.046921 0.000012  0.323798 0.000016  I-0.0146894 0.0000069 -0.0865 0.0048  I  -108.601    0.815    -7.480    0.217 -0.046882  0.323792 -0.0146819  -108.638    -7.416  
-23 3 5 60008.00 I -0.046594 0.000036  0.326590 0.000019  I-0.0146895 0.0000064  0.1156 0.0045  I  -108.485    0.909    -7.454    0.104 -0.046540  0.326621 -0.0146823  -108.483    -7.439  
-23 3 6 60009.00 I -0.045655 0.000037  0.329778 0.000018  I-0.0149305 0.0000059  0.3474 0.0047  I  -108.494    0.909    -7.281    0.104 -0.045657  0.329817 -0.0149129  -108.456    -7.322  
-23 3 7 60010.00 I -0.044607 0.000036  0.333305 0.000017  I-0.0153729 0.0000068  0.5451 0.0040  I  -108.473    0.929    -7.082    0.044 -0.044599  0.333296 -0.0153659  -108.413    -7.174  
-23 3 8 60011.00 I -0.043512 0.000037  0.336633 0.000016  I-0.0160146 0.0000054  0.7245 0.0042  I  -108.402    0.795    -7.003    0.038 -0.043530  0.336616 -0.0160051  -108.388    -7.094  
-23 3 9 60012.00 I -0.042352 0.000037  0.339812 0.000016  I-0.0167933 0.0000050  0.8181 0.0036  I  -108.377    0.795    -7.071    0.038 -0.042352  0.339803 -0.0167760  -108.432    -7.140  
-23 310 60013.00 I -0.041303 0.000037  0.343079 0.000015  I-0.0176198 0.0000048  0.8186 0.0031  I  -108.451    0.795    -7.206    0.038 -0.041322  0.343084 -0.0176027  -108.573    -7.251  
-23 311 60014.00 I -0.040750 0.000013  0.346411 0.000009  I-0.0184075 0.0000038  0.7501 0.0034  I  -108.577    0.697    -7.341    0.034 -0.040776  0.346390 -0.0184047  -108.718    -7.379  
-23 312 60015.00 I -0.040529 0.000013  0.349519 0.000010  I-0.0190955 0.0000048  0.6083 0.0031  I  -108.692    0.740    -7.472    0.052 -0.040519  0.349496 -0.0190910  -108.819    -7.513  
-23 313 60016.00 I -0.040089 0.000013  0.352556 0.000010  I-0.0195981 0.0000049  0.3886 0.0039  I  -108.760    0.740    -7.613    0.052 -0.040097  0.352572 -0.0196023  -108.854    -7.660  
-23 314 60017.00 I -0.039702 0.000014  0.355962 0.000012  I-0.0199052 0.0000062  0.2663 0.0039  I  -108.752    0.812    -7.749    0.072 -0.039717  0.355976 -0.0199116  -108.796    -7.801  
-23 315 60018.00 I -0.039676 0.000014  0.359426 0.000012  I-0.0201114 0.0000060  0.0860 0.0043  I  -108.663    0.812    -7.869    0.072 -0.039696  0.359397 -0.0200604  -108.636    -7.924  
-23 316 60019.00 I -0.039798 0.000013  0.362273 0.000012  I-0.0200825 0.0000060 -0.0783 0.0042  I  -108.524    0.812    -8.014    0.072 -0.039824  0.362249 -0.0200712  -108.426    -8.068  
-23 317 60020.00 I -0.039667 0.000012  0.364618 0.000012  I-0.0200347 0.0000059 -0.0030 0.0043  I  -108.359    0.812    -8.204    0.072 -0.039666  0.364628 -0.0200376  -108.244    -8.259  
-23 318 60021.00 I -0.039055 0.000011  0.366839 0.000011  I-0.0201206 0.0000063  0.2047 0.0035  I  -108.157    0.322    -8.345    0.160 -0.039047  0.366850 -0.0201299  -108.073    -8.402  
-23 319 60022.00 I -0.038098 0.000013  0.368982 0.000012  I-0.0204822 0.0000037  0.5268 0.0036  I  -107.940    0.618    -8.310    0.078 -0.038102  0.368994 -0.0204875  -107.908    -8.371  
-23 320 60023.00 I -0.036912 0.000009  0.371252 0.000008  I-0.0211492 0.0000036  0.7737 0.0026  I  -107.779    0.618    -8.120    0.078 -0.036907  0.371284 -0.0211416  -107.809    -8.185  
-23 321 60024.00 I -0.035479 0.000009  0.373933 0.000008  I-0.0219996 0.0000036  0.9304 0.0029  I  -107.712    0.618    -7.950    0.078 -0.035480  0.373974 -0.0220007  -107.798    -8.018  
-23 322 60025.00 I -0.033921 0.000012  0.377070 0.000012  I-0.0229704 0.0000045  0.9682 0.0029  I  -107.716    0.707    -7.910    0.051 -0.033918  0.377072 -0.0229616  -107.800    -7.977  
-23 323 60026.00 I -0.032493 0.000012  0.380217 0.000013  I-0.0238905 0.0000046  0.8695 0.0033  I  -107.807    0.707    -7.941    0.051 -0.032503  0.380245 -0.0238876  -107.871    -8.006  
-23 324 60027.00 I -0.031182 0.000011  0.383297 0.000013  I-0.0246830 0.0000047  0.6915 0.0036  I  -108.031    0.707    -7.964    0.051 -0.031173  0.383274 -0.0246908  -108.068    -8.026  
-23 325 60028.00 I -0.029863 0.000009  0.386398 0.000013  I-0.0252284 0.0000056  0.3780 0.0033  I  -108.330    0.760    -8.025    0.019 -0.029863  0.386430 -0.0252241  -108.334    -8.069  
-23 326 60029.00 I -0.028394 0.000014  0.389489 0.000018  I-0.0254385 0.0000045  0.0630 0.0036  I  -108.541    0.803    -8.203    0.111 -0.028402  0.389466 -0.0254315  -108.511    -8.224  
-23 327 60030.00 I -0.026607 0.000014  0.392602 0.000018  I-0.0253934 0.0000045 -0.1349 0.0035  I  -108.574    0.803    -8.444    0.111 -0.026589  0.392633 -0.0253926  -108.515    -8.443  
-23 328 60031.00 I -0.024709 0.000013  0.395453 0.000016  I-0.0251879 0.0000053 -0.2753 0.0033  I  -108.463    0.855    -8.599    0.160 -0.024718  0.395445 -0.0251809  -108.385    -8.580  
-23 329 60032.00 I -0.023045 0.000016  0.397855 0.000020  I-0.0248767 0.0000048 -0.3142 0.0037  I  -108.233    0.748    -8.618    0.111 -0.023029  0.397858 -0.0248761  -108.184    -8.619  
-23 330 60033.00 I -0.021724 0.000019  0.400028 0.000021  I-0.0245951 0.0000052 -0.2463 0.0040  I  -107.843    0.748    -8.610    0.111 -0.021735  0.400017 -0.0245819  -107.840    -8.642  
-23 331 60034.00 I -0.020386 0.000020  0.402185 0.000021  I-0.0243993 0.0000065 -0.1327 0.0049  I  -107.336    0.748    -8.699    0.111 -0.020397  0.402194 -0.0243867  -107.382    -8.762  
-23 4 1 60035.00 I -0.018859 0.000018  0.404604 0.000018  I-0.0243386 0.0000084  0.0077 0.0051  I  -106.908    0.681    -8.855    0.021 -0.018832  0.404562 -0.0243447  -106.941    -8.931  
-23 4 2 60036.00 I -0.017328 0.000019  0.407371 0.000020  I-0.0244341 0.0000079  0.2064 0.0056  I  -106.750    0.752    -8.923    0.064                                                     
-23 4 3 60037.00 I -0.015623 0.000019  0.409983 0.000020  I-0.0247500 0.0000073  0.4008 0.0054  I  -106.855    0.752    -8.803    0.064                                                     
-23 4 4 60038.00 I -0.013827 0.000019  0.412632 0.000021  I-0.0252207 0.0000074  0.5500 0.0050  I  -107.057    0.771    -8.566    0.092                                                     
-23 4 5 60039.00 I -0.012262 0.000015  0.415451 0.000020  I-0.0258397 0.0000069  0.6681 0.0043  I  -107.233    0.771    -8.385    0.092                                                     
-23 4 6 60040.00 I -0.010696 0.000015  0.418305 0.000019  I-0.0265275 0.0000042  0.6979 0.0039  I  -107.374    0.771    -8.368    0.092                                                     
-23 4 7 60041.00 I -0.009135 0.000015  0.421176 0.000019  I-0.0272228 0.0000038  0.6896 0.0028  I  -107.513    0.771    -8.489    0.092                                                     
-23 4 8 60042.00 I -0.007829 0.000014  0.423801 0.000016  I-0.0278873 0.0000038  0.6233 0.0032  I  -107.651    0.631    -8.645    0.081                                                     
-23 4 9 60043.00 I -0.006568 0.000015  0.426292 0.000016  I-0.0284442 0.0000051  0.4816 0.0051  I  -107.765    0.631    -8.768    0.081                                                     
-23 410 60044.00 I -0.005306 0.000014  0.428799 0.000022  I-0.0288335 0.0000095  0.2890 0.0050  I  -107.835    0.807    -8.865    0.052                                                     
-23 411 60045.00 I -0.004033 0.000013  0.431389 0.000023  I-0.0290185 0.0000087  0.0855 0.0054  I  -107.809    0.807    -8.979    0.052                                                     
-23 412 60046.00 I -0.002967 0.000014  0.434147 0.000023  I-0.0290317 0.0000052 -0.0363 0.0051  I  -107.600    0.817    -9.129    0.025                                                     
-23 413 60047.00 I -0.002355 0.000016  0.436717 0.000023  I-0.0289846 0.0000052 -0.0420 0.0036  I  -107.173    0.817    -9.290    0.025                                                     
-23 414 60048.00 I -0.001837 0.000018  0.439279 0.000023  I-0.0290006 0.0000051  0.1109 0.0038  I  -106.645    0.817    -9.405    0.025                                                     
-23 415 60049.00 I -0.001123 0.000017  0.441663 0.000023  I-0.0292399 0.0000056  0.3642 0.0040  I  -106.236    0.817    -9.416    0.025                                                     
-23 416 60050.00 I  0.000178 0.000017  0.443568 0.000011  I-0.0297577 0.0000061  0.7036 0.0041  I  -106.114    0.706    -9.310    0.025                                                     
-23 417 60051.00 I  0.001667 0.000017  0.445287 0.000010  I-0.0306176 0.0000060  0.9544 0.0048  I  -106.268    0.706    -9.137    0.025                                                     
-23 418 60052.00 I  0.002963 0.000016  0.446945 0.000009  I-0.0315944 0.0000075  0.9890 0.0043  I  -106.537    0.636    -8.986    0.029                                                     
-23 419 60053.00 I  0.004293 0.000012  0.448612 0.000011  I-0.0325548 0.0000061  0.9014 0.0049  I  -106.755    0.648    -8.906    0.033                                                     
-23 420 60054.00 I  0.005752 0.000008  0.450447 0.000010  I-0.0333636 0.0000064  0.7132 0.0048  I  -106.883    0.648    -8.893    0.033                                                     
-23 421 60055.00 I  0.007427 0.000008  0.452616 0.000010  I-0.0339540 0.0000074  0.4436 0.0053  I  -106.985    0.648    -8.930    0.033                                                     
-23 422 60056.00 I  0.009104 0.000007  0.455126 0.000009  I-0.0342557 0.0000084  0.1889 0.0050  I  -107.111    0.705    -9.030    0.046                                                     
-23 423 60057.00 I  0.010719 0.000008  0.457863 0.000020  I-0.0343538 0.0000066  0.0004 0.0053  I  -107.231    0.848    -9.193    0.061                                                     
-23 424 60058.00 I  0.012629 0.000009  0.460581 0.000020  I-0.0342653 0.0000066 -0.1617 0.0053  I  -107.279    0.848    -9.355    0.061                                                     
-23 425 60059.00 I  0.014953 0.000010  0.462939 0.000019  I-0.0340606 0.0000084 -0.2332 0.0050  I  -107.218    0.870    -9.438    0.064                                                     
-23 426 60060.00 I  0.017319 0.000011  0.465022 0.000028  I-0.0338247 0.0000074 -0.2272 0.0055  I  -107.027    0.870    -9.449    0.064                                                     
-23 427 60061.00 I  0.019407 0.000011  0.467120 0.000029  I-0.0336194 0.0000072 -0.1817 0.0054  I  -106.690    0.870    -9.491    0.064                                                     
-23 428 60062.00 I  0.021468 0.000012  0.469075 0.000029  I-0.0334895 0.0000079 -0.0516 0.0062  I  -106.238    0.870    -9.638    0.064                                                     
-23 429 60063.00 I  0.023801 0.000011  0.470664 0.000023  I-0.0335369 0.0000101  0.1406 0.0069  I  -105.810    0.322    -9.835    0.160                                                     
-23 430 60064.00 I  0.025989 0.000011  0.472096 0.000023  I-0.0337777 0.0000113  0.3537 0.0072  I  -105.602    0.322    -9.927    0.160                                                     
-23 5 1 60065.00 I  0.027591 0.000011  0.473437 0.000023  I-0.0342371 0.0000102  0.5453 0.0086  I  -105.722    1.020    -9.816    0.099                                                     
-23 5 2 60066.00 I  0.028835 0.000009  0.474635 0.000008  I-0.0348282 0.0000129  0.6168 0.0070  I  -106.090    1.020    -9.558    0.099                                                     
-23 5 3 60067.00 I  0.030235 0.000008  0.475652 0.000009  I-0.0354586 0.0000097  0.6520 0.0079  I  -106.505    1.002    -9.304    0.075                                                     
-23 5 4 60068.00 I  0.031949 0.000009  0.476564 0.000008  I-0.0361380 0.0000091  0.7045 0.0067  I  -106.806    1.002    -9.179    0.075                                                     
-23 5 5 60069.00 I  0.033799 0.000009  0.477610 0.000008  I-0.0368130 0.0000093  0.5930 0.0063  I  -106.984    1.002    -9.215    0.075                                                     
-23 5 6 60070.00 I  0.035739 0.000010  0.478665 0.000009  I-0.0373242 0.0000087  0.4821 0.0065  I  -107.130    1.002    -9.371    0.075                                                     
-23 5 7 60071.00 I  0.037826 0.000011  0.479811 0.000010  I-0.0377573 0.0000090  0.3116 0.0063  I  -107.294    1.083    -9.592    0.152                                                     
-23 5 8 60072.00 I  0.039827 0.000012  0.481232 0.000012  I-0.0379487 0.0000091  0.1449 0.0073  I  -107.402    1.083    -9.822    0.152                                                     
-23 5 9 60073.00 I  0.041741 0.000012  0.482739 0.000011  I-0.0380824 0.0000114  0.0841 0.0074  I  -107.322    1.217   -10.018    0.224                                                     
-23 510 60074.00 I  0.043535 0.000011  0.484271 0.000011  I-0.0381415 0.0000117  0.0973 0.0075  P  -107.062    0.278   -10.129    0.145                                                     
-23 511 60075.00 I  0.045319 0.000012  0.485528 0.000010  I-0.0383566 0.0000097  0.3494 0.0072  P  -106.694    0.288   -10.149    0.148                                                     
-23 512 60076.00 I  0.047270 0.000078  0.486614 0.000078  I-0.0388331 0.0000083  0.5800 0.0067  P  -106.353    0.297   -10.099    0.151                                                     
-23 513 60077.00 I  0.049465 0.000078  0.487754 0.000078  I-0.0395258 0.0000092  0.8384 0.0061  P  -106.154    0.304    -9.996    0.154                                                     
-23 514 60078.00 I  0.052355 0.000085  0.489080 0.000085  I-0.0405252 0.0000090  1.1428 0.0061  P  -106.156    0.309    -9.850    0.155                                                     
-23 515 60079.00 I  0.055823 0.000091  0.490647 0.000091  I-0.0417656 0.0000079  1.3097 0.0059  P  -106.350    0.313    -9.671    0.157                                                     
-23 516 60080.00 I  0.059182 0.000091  0.492199 0.000091  I-0.0430864 0.0000075  1.3020 0.0057  P  -106.668    0.316    -9.471    0.158                                                     
-23 517 60081.00 I  0.062075 0.000091  0.493471 0.000091  I-0.0443097 0.0000083  1.1147 0.0058  P  -106.997    0.318    -9.275    0.158                                                     
-23 518 60082.00 I  0.064538 0.000091  0.494606 0.000091  I-0.0452777 0.0000088  0.8132 0.0055  P  -107.225    0.319    -9.138    0.159                                                     
-23 519 60083.00 I  0.066905 0.000091  0.495692 0.000090  I-0.0459284 0.0000073  0.4887 0.0059  P  -107.311    0.320    -9.131    0.159                                                     
-23 520 60084.00 I  0.069347 0.000091  0.496656 0.000091  I-0.0462757 0.0000078  0.2262 0.0058  P  -107.316    0.321    -9.280    0.160                                                     
-23 521 60085.00 I  0.071616 0.000091  0.497496 0.000091  I-0.0463859 0.0000089 -0.0208 0.0056  P  -107.343    0.321    -9.519    0.160                                                     
-23 522 60086.00 I  0.073729 0.000091  0.498189 0.000091  I-0.0462453 0.0000080 -0.2342 0.0059  P  -107.430    0.321    -9.717    0.160                                                     
-23 523 60087.00 I  0.076210 0.000091  0.498997 0.000091  I-0.0459641 0.0000076 -0.3077 0.0057  P  -107.527    0.321    -9.787    0.160                                                     
-23 524 60088.00 I  0.079152 0.000091  0.499991 0.000091  I-0.0456633 0.0000082 -0.2810 0.0058  P  -107.563    0.322    -9.775    0.160                                                     
-23 525 60089.00 I  0.082204 0.000090  0.501136 0.000091  I-0.0453859 0.0000087                 P  -107.495    0.322    -9.803    0.160                                                     
-23 526 60090.00 P  0.085155 0.000600  0.502166 0.000425  P-0.0451659 0.0001080                 P  -107.303    0.322    -9.923    0.160                                                     
-23 527 60091.00 P  0.088012 0.000891  0.503223 0.000700  P-0.0450616 0.0002041                 P  -107.011    0.322   -10.046    0.160                                                     
-23 528 60092.00 P  0.090860 0.001123  0.504149 0.000937  P-0.0451160 0.0003028                 P  -106.759    0.322   -10.030    0.160                                                     
-23 529 60093.00 P  0.093670 0.001323  0.504928 0.001153  P-0.0453306 0.0004021                 P  -106.781    0.322    -9.835    0.160                                                     
-23 530 60094.00 P  0.096449 0.001503  0.505583 0.001353  P-0.0456505 0.0005017                 P  -107.208    0.322    -9.554    0.160                                                     
-23 531 60095.00 P  0.099209 0.001667  0.506139 0.001543  P-0.0459875 0.0006014                 P  -107.886    0.322    -9.311    0.160                                                     
-23 6 1 60096.00 P  0.101978 0.001820  0.506625 0.001724  P-0.0462601 0.0007012                 P  -108.495    0.322    -9.154    0.160                                                     
-23 6 2 60097.00 P  0.104748 0.001964  0.507064 0.001899  P-0.0463965 0.0007500                 P  -108.875    0.322    -9.087    0.160                                                     
-23 6 3 60098.00 P  0.107500 0.002101  0.507466 0.002067  P-0.0463276 0.0005500                 P  -109.132    0.322    -9.144    0.160                                                     
-23 6 4 60099.00 P  0.110246 0.002231  0.507839 0.002229  P-0.0460431 0.0007548                 P  -109.380    0.322    -9.362    0.160                                                     
-23 6 5 60100.00 P  0.113002 0.002355  0.508160 0.002388  P-0.0455705 0.0009344                 P  -109.511    0.322    -9.664    0.160                                                     
-23 6 6 60101.00 P  0.115784 0.002475  0.508426 0.002542  P-0.0449965 0.0010994                 P  -109.358    0.322    -9.877    0.160                                                     
-23 6 7 60102.00 P  0.118582 0.002591  0.508655 0.002693  P-0.0444818 0.0012543                 P  -108.978    0.322    -9.889    0.160                                                     
-23 6 8 60103.00 P  0.121388 0.002702  0.508854 0.002841  P-0.0441560 0.0014016                 P  -108.642    0.322    -9.757    0.160                                                     
-23 6 9 60104.00 P  0.124195 0.002811  0.509021 0.002985  P-0.0441055 0.0015429                 P  -108.550    0.322    -9.609    0.160                                                     
-23 610 60105.00 P  0.126995 0.002916  0.509146 0.003127  P-0.0443337 0.0016792                 P  -108.661    0.322    -9.508    0.160                                                     
-23 611 60106.00 P  0.129785 0.003019  0.509226 0.003267  P-0.0447922 0.0018113                 P  -108.809    0.322    -9.425    0.160                                                     
-23 612 60107.00 P  0.132563 0.003119  0.509259 0.003404  P-0.0453632 0.0019399                 P  -108.920    0.322    -9.315    0.160                                                     
-23 613 60108.00 P  0.135334 0.003216  0.509241 0.003539  P-0.0458976 0.0020652                 P  -109.070    0.322    -9.157    0.160                                                     
-23 614 60109.00 P  0.138099 0.003312  0.509174 0.003672  P-0.0462685 0.0021877                 P  -109.341    0.322    -8.969    0.160                                                     
-23 615 60110.00 P  0.140863 0.003405  0.509058 0.003804  P-0.0463849 0.0023077                 P  -109.673    0.322    -8.825    0.160                                                     
-23 616 60111.00 P  0.143624 0.003496  0.508900 0.003933  P-0.0462053 0.0024255                 P  -109.909    0.322    -8.839    0.160                                                     
-23 617 60112.00 P  0.146381 0.003586  0.508700 0.004061  P-0.0457351 0.0025411                 P  -109.979    0.322    -9.074    0.160                                                     
-23 618 60113.00 P  0.149132 0.003674  0.508458 0.004187  P-0.0450274 0.0026548                 P  -109.974    0.322    -9.447    0.160                                                     
-23 619 60114.00 P  0.151877 0.003761  0.508173 0.004312  P-0.0441691 0.0027668                 P  -110.025    0.322    -9.753    0.160                                                     
-23 620 60115.00 P  0.154615 0.003846  0.507847 0.004436  P-0.0432430 0.0028772                 P  -110.165    0.322    -9.831    0.160                                                     
-23 621 60116.00 P  0.157344 0.003929  0.507479 0.004558  P-0.0423298 0.0029860                 P  -110.343    0.322    -9.712    0.160                                                     
-23 622 60117.00 P  0.160066 0.004012  0.507070 0.004679  P-0.0414937 0.0030934                 P  -110.499    0.322    -9.571    0.160                                                     
-23 623 60118.00 P  0.162777 0.004093  0.506621 0.004799  P-0.0407731 0.0031995                 P  -110.557    0.322    -9.521    0.160                                                     
-23 624 60119.00 P  0.165477 0.004173  0.506130 0.004917  P-0.0401827 0.0033043                 P  -110.442    0.322    -9.496    0.160                                                     
-23 625 60120.00 P  0.168165 0.004251  0.505599 0.005035  P-0.0397207 0.0034080                 P  -110.208    0.322    -9.370    0.160                                                     
-23 626 60121.00 P  0.170841 0.004329  0.505027 0.005151  P-0.0393635 0.0035105                 P  -110.142    0.322    -9.142    0.160                                                     
-23 627 60122.00 P  0.173503 0.004406  0.504414 0.005266  P-0.0390569 0.0036120                 P  -110.555    0.322    -8.958    0.160                                                     
-23 628 60123.00 P  0.176151 0.004481  0.503760 0.005381  P-0.0387358 0.0037124                 P  -111.413    0.322    -8.925    0.160                                                     
-23 629 60124.00 P  0.178786 0.004556  0.503066 0.005494  P-0.0383258 0.0038119                 P  -112.302    0.322    -8.980    0.160                                                     
-23 630 60125.00 P  0.181406 0.004630  0.502331 0.005607  P-0.0377456 0.0039105                 P  -112.871    0.322    -9.003    0.160                                                     
-23 7 1 60126.00 P  0.184011 0.004702  0.501557 0.005719  P-0.0369353 0.0040082                 P  -113.141    0.322    -9.026    0.160                                                     
-23 7 2 60127.00 P  0.186600 0.004774  0.500744 0.005830  P-0.0358970 0.0041051                 P  -113.269    0.322    -9.183    0.160                                                     
-23 7 3 60128.00 P  0.189172 0.004846  0.499891 0.005940  P-0.0347046 0.0042012                 P  -113.215    0.322    -9.455    0.160                                                     
-23 7 4 60129.00 P  0.191728 0.004916  0.499000 0.006049  P-0.0334883 0.0042965                 P  -112.895    0.322    -9.621    0.160                                                     
-23 7 5 60130.00 P  0.194265 0.004986  0.498071 0.006157  P-0.0323935 0.0043911                 P  -112.498    0.322    -9.531    0.160                                                     
-23 7 6 60131.00 P  0.196783 0.005055  0.497104 0.006265  P-0.0315298 0.0044849                 P  -112.373    0.322    -9.315    0.160                                                     
-23 7 7 60132.00 P  0.199283 0.005123  0.496099 0.006372  P-0.0309329 0.0045781                 P  -112.639    0.322    -9.189    0.160                                                     
-23 7 8 60133.00 P  0.201762 0.005191  0.495057 0.006479  P-0.0305522 0.0046706                 P  -113.093    0.322    -9.180    0.160                                                     
-23 7 9 60134.00 P  0.204220 0.005257  0.493978 0.006584  P-0.0302712 0.0047625                 P  -113.469    0.322    -9.160    0.160                                                     
-23 710 60135.00 P  0.206657 0.005324  0.492861 0.006689  P-0.0299560 0.0048537                 P  -113.667    0.322    -9.067    0.160                                                     
-23 711 60136.00 P  0.209073 0.005389  0.491709 0.006794  P-0.0294878 0.0049444                 P  -113.773    0.322    -8.960    0.160                                                     
-23 712 60137.00 P  0.211466 0.005454  0.490520 0.006897  P-0.0287941 0.0050344                 P  -113.944    0.322    -8.895    0.160                                                     
-23 713 60138.00 P  0.213836 0.005519  0.489296 0.007001  P-0.0278502 0.0051240                 P  -114.248    0.322    -8.882    0.160                                                     
-23 714 60139.00 P  0.216182 0.005583  0.488036 0.007103  P-0.0266720 0.0052129                 P  -114.580    0.322    -8.957    0.160                                                     
-23 715 60140.00 P  0.218504 0.005646  0.486741 0.007205  P-0.0253091 0.0053014                 P  -114.778    0.322    -9.185    0.160                                                     
-23 716 60141.00 P  0.220801 0.005709  0.485412 0.007307  P-0.0238318 0.0053893                 P  -114.805    0.322    -9.539    0.160                                                     
-23 717 60142.00 P  0.223073 0.005771  0.484049 0.007407  P-0.0223181 0.0054768                 P  -114.769    0.322    -9.835    0.160                                                     
-23 718 60143.00 P  0.225319 0.005833  0.482652 0.007508  P-0.0208438 0.0055637                 P  -114.780    0.322    -9.860    0.160                                                     
-23 719 60144.00 P  0.227539 0.005895  0.481221 0.007608  P-0.0194768 0.0056502                 P  -114.868    0.322    -9.592    0.160                                                     
-23 720 60145.00 P  0.229731 0.005955  0.479758 0.007707  P-0.0182612 0.0057362                 P  -114.997    0.322    -9.234    0.160                                                     
-23 721 60146.00 P  0.231896 0.006016  0.478263 0.007806  P-0.0172204 0.0058218                 P  -115.088    0.322    -9.000    0.160                                                     
-23 722 60147.00 P  0.234033 0.006076  0.476735 0.007904  P-0.0163450 0.0059070                 P  -115.044    0.322    -8.900    0.160                                                     
-23 723 60148.00 P  0.236141 0.006135  0.475176 0.008002  P-0.0156023 0.0059917                 P  -114.862    0.322    -8.810    0.160                                                     
-23 724 60149.00 P  0.238220 0.006194  0.473586 0.008100  P-0.0149420 0.0060760                 P  -114.767    0.322    -8.696    0.160                                                     
-23 725 60150.00 P  0.240269 0.006253  0.471965 0.008196  P-0.0142998 0.0061599                 P  -115.089    0.322    -8.689    0.160                                                     
-23 726 60151.00 P  0.242288 0.006311  0.470315 0.008293  P-0.0136072 0.0062434                 P  -115.896    0.322    -8.893    0.160                                                     
-23 727 60152.00 P  0.244276 0.006369  0.468634 0.008389  P-0.0127952 0.0063266                 P  -116.815    0.322    -9.198    0.160                                                     
-23 728 60153.00 P  0.246234 0.006426  0.466925 0.008485  P-0.0118082 0.0064093                 P  -117.397    0.322    -9.388    0.160                                                     
-23 729 60154.00 P  0.248159 0.006483  0.465186 0.008580  P-0.0106248 0.0064917                 P  -117.541    0.322    -9.415    0.160                                                     
-23 730 60155.00 P  0.250053 0.006540  0.463420 0.008675  P-0.0092847 0.0065737                 P  -117.407    0.322    -9.437    0.160                                                     
-23 731 60156.00 P  0.251914 0.006596  0.461626 0.008769  P-0.0078962 0.0066554                 P  -117.087    0.322    -9.517    0.160                                                     
-23 8 1 60157.00 P  0.253742 0.006652  0.459805 0.008863  P-0.0066047 0.0067368                 P  -116.655    0.322    -9.495    0.160                                                     
-23 8 2 60158.00 P  0.255536 0.006708  0.457957 0.008957  P-0.0055502 0.0068177                 P  -116.381    0.322    -9.271    0.160                                                     
-23 8 3 60159.00 P  0.257297 0.006763  0.456084 0.009050  P-0.0048119 0.0068984                 P  -116.529    0.322    -9.050    0.160                                                     
-23 8 4 60160.00 P  0.259023 0.006818  0.454184 0.009143  P-0.0043697 0.0069788                 P  -116.999    0.322    -9.083    0.160                                                     
-23 8 5 60161.00 P  0.260715 0.006873  0.452260 0.009236  P-0.0041135 0.0070588                 P  -117.463    0.322    -9.288    0.160                                                     
-23 8 6 60162.00 P  0.262372 0.006927  0.450311 0.009328  P-0.0038862 0.0071385                 P  -117.772    0.322    -9.368    0.160                                                     
-23 8 7 60163.00 P  0.263993 0.006981  0.448339 0.009420  P-0.0035333 0.0072179                 P  -117.998    0.322    -9.238    0.160                                                     
-23 8 8 60164.00 P  0.265578 0.007034  0.446343 0.009511  P-0.0029525 0.0072970                                                                                                             
-23 8 9 60165.00 P  0.267127 0.007088  0.444324 0.009602  P-0.0021044 0.0073758                                                                                                             
-23 810 60166.00 P  0.268640 0.007141  0.442284 0.009693  P-0.0010050 0.0074544                                                                                                             
-23 811 60167.00 P  0.270116 0.007194  0.440221 0.009784  P 0.0002908 0.0075326                                                                                                             
-23 812 60168.00 P  0.271554 0.007246  0.438138 0.009874  P 0.0017052 0.0076106                                                                                                             
-23 813 60169.00 P  0.272955 0.007298  0.436034 0.009964  P 0.0031524 0.0076883                                                                                                             
-23 814 60170.00 P  0.274318 0.007350  0.433911 0.010053  P 0.0045542 0.0077657                                                                                                             
-23 815 60171.00 P  0.275643 0.007402  0.431768 0.010142  P 0.0058435 0.0078428                                                                                                             
-23 816 60172.00 P  0.276929 0.007453  0.429606 0.010231  P 0.0069708 0.0079197                                                                                                             
-23 817 60173.00 P  0.278176 0.007504  0.427427 0.010320  P 0.0079089 0.0079964                                                                                                             
-23 818 60174.00 P  0.279385 0.007555  0.425230 0.010408  P 0.0086579 0.0080728                                                                                                             
-23 819 60175.00 P  0.280554 0.007605  0.423016 0.010496  P 0.0092455 0.0081489                                                                                                             
-23 820 60176.00 P  0.281683 0.007655  0.420786 0.010584  P 0.0097206 0.0082248                                                                                                             
-23 821 60177.00 P  0.282773 0.007706  0.418540 0.010671  P 0.0101495 0.0083005                                                                                                             
-23 822 60178.00 P  0.283822 0.007755  0.416280 0.010758  P 0.0106035 0.0083759                                                                                                             
-23 823 60179.00 P  0.284832 0.007805  0.414005 0.010845  P 0.0111499 0.0084511                                                                                                             
-23 824 60180.00 P  0.285801 0.007854  0.411717 0.010932  P 0.0118454 0.0085261                                                                                                             
-23 825 60181.00 P  0.286729 0.007903  0.409415 0.011018  P 0.0127140 0.0086008                                                                                                             
-23 826 60182.00 P  0.287616 0.007952  0.407101 0.011104  P 0.0137348 0.0086754                                                                                                             
-23 827 60183.00 P  0.288463 0.008001  0.404775 0.011190  P 0.0148302 0.0087497                                                                                                             
-23 828 60184.00 P  0.289268 0.008049  0.402438 0.011276  P 0.0158715 0.0088237                                                                                                             
-23 829 60185.00 P  0.290032 0.008097  0.400091 0.011361  P 0.0167113 0.0088976                                                                                                             
-23 830 60186.00 P  0.290754 0.008145  0.397733 0.011446  P 0.0172335 0.0089713                                                                                                             
-23 831 60187.00 P  0.291435 0.008193  0.395367 0.011531  P 0.0174028 0.0090448                                                                                                             
-23 9 1 60188.00 P  0.292074 0.008241  0.392992 0.011616  P 0.0172856 0.0091180                                                                                                             
-23 9 2 60189.00 P  0.292671 0.008288  0.390609 0.011700  P 0.0170311 0.0091911                                                                                                             
-23 9 3 60190.00 P  0.293227 0.008335  0.388218 0.011784  P 0.0168190 0.0092639                                                                                                             
-23 9 4 60191.00 P  0.293741 0.008382  0.385820 0.011868  P 0.0167994 0.0093366                                                                                                             
-23 9 5 60192.00 P  0.294212 0.008429  0.383416 0.011952  P 0.0170533 0.0094091                                                                                                             
-23 9 6 60193.00 P  0.294642 0.008475  0.381006 0.012035  P 0.0175863 0.0094814                                                                                                             
-23 9 7 60194.00 P  0.295029 0.008522  0.378592 0.012118  P 0.0183467 0.0095535                                                                                                             
-23 9 8 60195.00 P  0.295374 0.008568  0.376173 0.012201  P 0.0192522 0.0096254                                                                                                             
-23 9 9 60196.00 P  0.295677 0.008614  0.373751 0.012284  P 0.0202126 0.0096971                                                                                                             
-23 910 60197.00 P  0.295937 0.008660  0.371327 0.012367  P 0.0211439 0.0097686                                                                                                             
-23 911 60198.00 P  0.296156 0.008705  0.368900 0.012449  P 0.0219150 0.0098400                                                                                                             
-23 912 60199.00 P  0.296332 0.008751  0.366472 0.012531  P 0.0225329 0.0099112                                                                                                             
-23 913 60200.00 P  0.296466 0.008796  0.364044 0.012613  P 0.0229642 0.0099822                                                                                                             
-23 914 60201.00 P  0.296558 0.008841  0.361615 0.012695  P 0.0232020 0.0100531                                                                                                             
-23 915 60202.00 P  0.296607 0.008886  0.359187 0.012776  P 0.0232670 0.0101238                                                                                                             
-23 916 60203.00 P  0.296615 0.008931  0.356760 0.012858  P 0.0232069 0.0101943                                                                                                             
-23 917 60204.00 P  0.296580 0.008975  0.354335 0.012939  P 0.0230886 0.0102646                                                                                                             
-23 918 60205.00 P  0.296504 0.009020  0.351912 0.013020  P 0.0229880 0.0103348                                                                                                             
-23 919 60206.00 P  0.296386 0.009064  0.349493 0.013100  P 0.0229779 0.0104048                                                                                                             
-23 920 60207.00 P  0.296226 0.009108  0.347077 0.013181  P 0.0231143 0.0104747                                                                                                             
-23 921 60208.00 P  0.296024 0.009152  0.344666 0.013261  P 0.0234243 0.0105444                                                                                                             
-23 922 60209.00 P  0.295781 0.009196  0.342259 0.013341  P 0.0238951 0.0106139                                                                                                             
-23 923 60210.00 P  0.295497 0.009239  0.339859 0.013421  P 0.0244665 0.0106833                                                                                                             
-23 924 60211.00 P  0.295171 0.009283  0.337465 0.013501  P 0.0250329 0.0107526                                                                                                             
-23 925 60212.00 P  0.294805 0.009326  0.335078 0.013581  P 0.0254595 0.0108216                                                                                                             
-23 926 60213.00 P  0.294397 0.009369  0.332698 0.013660  P 0.0256189 0.0108906                                                                                                             
-23 927 60214.00 P  0.293949 0.009412  0.330327 0.013739  P 0.0254358 0.0109594                                                                                                             
-23 928 60215.00 P  0.293460 0.009455  0.327964 0.013818  P 0.0249224 0.0110280                                                                                                             
-23 929 60216.00 P  0.292931 0.009498  0.325611 0.013897  P 0.0241841 0.0110965                                                                                                             
-23 930 60217.00 P  0.292361 0.009540  0.323268 0.013976  P 0.0233906 0.0111649                                                                                                             
-2310 1 60218.00 P  0.291752 0.009583  0.320936 0.014055  P 0.0227193 0.0112331                                                                                                             
-2310 2 60219.00 P  0.291104 0.009625  0.318615 0.014133  P 0.0223008 0.0113012                                                                                                             
-2310 3 60220.00 P  0.290415 0.009667  0.316306 0.014211  P 0.0221877 0.0113691                                                                                                             
-2310 4 60221.00 P  0.289688 0.009709  0.314010 0.014289  P 0.0223548 0.0114369                                                                                                             
-2310 5 60222.00 P  0.288922 0.009751  0.311726 0.014367  P 0.0227245 0.0115046                                                                                                             
-2310 6 60223.00 P  0.288117 0.009793  0.309457 0.014445  P 0.0231989 0.0115721                                                                                                             
-2310 7 60224.00 P  0.287274 0.009834  0.307201 0.014522  P 0.0236820 0.0116395                                                                                                             
-2310 8 60225.00 P  0.286393 0.009876  0.304961 0.014600  P 0.0240932 0.0117067                                                                                                             
-2310 9 60226.00 P  0.285474 0.009917  0.302736 0.014677  P 0.0243708 0.0117739                                                                                                             
-231010 60227.00 P  0.284517 0.009958  0.300527 0.014754  P 0.0244757 0.0118409                                                                                                             
-231011 60228.00 P  0.283524 0.009999  0.298335 0.014831  P 0.0243937 0.0119077                                                                                                             
-231012 60229.00 P  0.282494 0.010040  0.296160 0.014907  P 0.0241374 0.0119745                                                                                                             
-231013 60230.00 P  0.281427 0.010081  0.294002 0.014984  P 0.0237462 0.0120411                                                                                                             
-231014 60231.00 P  0.280324 0.010122  0.291863 0.015060  P 0.0232821 0.0121076                                                                                                             
-231015 60232.00 P  0.279186 0.010162  0.289743 0.015137  P 0.0228220 0.0121740                                                                                                             
-231016 60233.00 P  0.278012 0.010203  0.287642 0.015213  P 0.0224461 0.0122402                                                                                                             
-231017 60234.00 P  0.276804 0.010243  0.285561 0.015289  P 0.0222224 0.0123063                                                                                                             
-231018 60235.00 P  0.275560 0.010283  0.283500 0.015365  P 0.0221897 0.0123723                                                                                                             
-231019 60236.00 P  0.274283 0.010323  0.281460 0.015440  P 0.0223440 0.0124382                                                                                                             
-231020 60237.00 P  0.272972 0.010363  0.279442 0.015516  P 0.0226325 0.0125040                                                                                                             
-231021 60238.00 P  0.271627 0.010403  0.277446 0.015591  P 0.0229593 0.0125696                                                                                                             
-231022 60239.00 P  0.270250 0.010443  0.275472 0.015667  P 0.0232019 0.0126352                                                                                                             
-231023 60240.00 P  0.268840 0.010482  0.273521 0.015742  P 0.0232385 0.0127006                                                                                                             
-231024 60241.00 P  0.267398 0.010522  0.271594 0.015817  P 0.0229825 0.0127659                                                                                                             
-231025 60242.00 P  0.265925 0.010561  0.269690 0.015892  P 0.0224115 0.0128311                                                                                                             
-231026 60243.00 P  0.264420 0.010601  0.267811 0.015966  P 0.0215848 0.0128962                                                                                                             
-231027 60244.00 P  0.262885 0.010640  0.265957 0.016041  P 0.0206336 0.0129612                                                                                                             
-231028 60245.00 P  0.261320 0.010679  0.264128 0.016115  P 0.0197243 0.0130260                                                                                                             
-231029 60246.00 P  0.259725 0.010718  0.262325 0.016190  P 0.0190088 0.0130908                                                                                                             
-231030 60247.00 P  0.258101 0.010757  0.260548 0.016264  P 0.0185810 0.0131554                                                                                                             
-231031 60248.00 P  0.256448 0.010796  0.258798 0.016338  P 0.0184575 0.0132199                                                                                                             
-2311 1 60249.00 P  0.254766 0.010834  0.257075 0.016412  P 0.0185871 0.0132844                                                                                                             
-2311 2 60250.00 P  0.253057 0.010873  0.255379 0.016486  P 0.0188782 0.0133487                                                                                                             
-2311 3 60251.00 P  0.251321 0.010911  0.253712 0.016559  P 0.0192290 0.0134129                                                                                                             
-2311 4 60252.00 P  0.249559 0.010950  0.252072 0.016633  P 0.0195486 0.0134770                                                                                                             
-2311 5 60253.00 P  0.247770 0.010988  0.250461 0.016706  P 0.0197656 0.0135410                                                                                                             
-2311 6 60254.00 P  0.245955 0.011026  0.248880 0.016780  P 0.0198328 0.0136050                                                                                                             
-2311 7 60255.00 P  0.244116 0.011064  0.247328 0.016853  P 0.0197287 0.0136688                                                                                                             
-2311 8 60256.00 P  0.242252 0.011102  0.245806 0.016926  P 0.0194573 0.0137325                                                                                                             
-2311 9 60257.00 P  0.240364 0.011140  0.244314 0.016999  P 0.0190488 0.0137961                                                                                                             
-231110 60258.00 P  0.238453 0.011177  0.242852 0.017071  P 0.0185552 0.0138596                                                                                                             
-231111 60259.00 P  0.236518 0.011215  0.241421 0.017144  P 0.0180464 0.0139230                                                                                                             
-231112 60260.00 P  0.234562 0.011253  0.240022 0.017217  P 0.0176014 0.0139863                                                                                                             
-231113 60261.00 P  0.232584 0.011290  0.238654 0.017289  P 0.0172966 0.0140495                                                                                                             
-231114 60262.00 P  0.230585 0.011327  0.237318 0.017361  P 0.0171866 0.0141127                                                                                                             
-231115 60263.00 P  0.228565 0.011365  0.236015 0.017434  P 0.0172852 0.0141757                                                                                                             
-231116 60264.00 P  0.226526 0.011402  0.234743 0.017506  P 0.0175533 0.0142386                                                                                                             
-231117 60265.00 P  0.224467 0.011439  0.233505 0.017578  P 0.0179020 0.0143014                                                                                                             
-231118 60266.00 P  0.222390 0.011476  0.232299 0.017649  P 0.0182108 0.0143642                                                                                                             
-231119 60267.00 P  0.220294 0.011513  0.231127 0.017721  P 0.0183597 0.0144268                                                                                                             
-231120 60268.00 P  0.218181 0.011550  0.229988 0.017793  P 0.0182614 0.0144894                                                                                                             
-231121 60269.00 P  0.216051 0.011587  0.228883 0.017864  P 0.0178862 0.0145519                                                                                                             
-231122 60270.00 P  0.213905 0.011623  0.227813 0.017936  P 0.0172734 0.0146142                                                                                                             
-231123 60271.00 P  0.211743 0.011660  0.226776 0.018007  P 0.0165245 0.0146765                                                                                                             
-231124 60272.00 P  0.209567 0.011696  0.225774 0.018078  P 0.0157798 0.0147387                                                                                                             
-231125 60273.00 P  0.207376 0.011733  0.224807 0.018149  P 0.0151820 0.0148008                                                                                                             
-231126 60274.00 P  0.205171 0.011769  0.223874 0.018220  P 0.0148385 0.0148629                                                                                                             
-231127 60275.00 P  0.202953 0.011805  0.222977 0.018291  P 0.0147954 0.0149248                                                                                                             
-231128 60276.00 P  0.200722 0.011841  0.222115 0.018362  P 0.0150318 0.0149867                                                                                                             
-231129 60277.00 P  0.198480 0.011877  0.221288 0.018433  P 0.0154745 0.0150484                                                                                                             
-231130 60278.00 P  0.196227 0.011913  0.220497 0.018503  P 0.0160240 0.0151101                                                                                                             
-2312 1 60279.00 P  0.193963 0.011949  0.219742 0.018573  P 0.0165794 0.0151717                                                                                                             
-2312 2 60280.00 P  0.191689 0.011985  0.219022 0.018644  P 0.0170566 0.0152332                                                                                                             
-2312 3 60281.00 P  0.189406 0.012021  0.218339 0.018714  P 0.0173972 0.0152946                                                                                                             
-2312 4 60282.00 P  0.187114 0.012056  0.217692 0.018784  P 0.0175724 0.0153560                                                                                                             
-2312 5 60283.00 P  0.184814 0.012092  0.217081 0.018854  P 0.0175834 0.0154172                                                                                                             
-2312 6 60284.00 P  0.182507 0.012127  0.216506 0.018924  P 0.0174586 0.0154784                                                                                                             
-2312 7 60285.00 P  0.180194 0.012163  0.215968 0.018994  P 0.0172470 0.0155395                                                                                                             
-2312 8 60286.00 P  0.177874 0.012198  0.215466 0.019064  P 0.0170104 0.0156005                                                                                                             
-2312 9 60287.00 P  0.175549 0.012233  0.215001 0.019133  P 0.0168159 0.0156614                                                                                                             
-231210 60288.00 P  0.173220 0.012269  0.214573 0.019203  P 0.0167287 0.0157223                                                                                                             
-231211 60289.00 P  0.170886 0.012304  0.214181 0.019272  P 0.0168009 0.0157831                                                                                                             
-231212 60290.00 P  0.168549 0.012339  0.213826 0.019342  P 0.0170546 0.0158438                                                                                                             
-231213 60291.00 P  0.166209 0.012374  0.213507 0.019411  P 0.0174652 0.0159044                                                                                                             
-231214 60292.00 P  0.163868 0.012409  0.213226 0.019480  P 0.0179536 0.0159649                                                                                                             
-231215 60293.00 P  0.161524 0.012443  0.212981 0.019549  P 0.0183995 0.0160254                                                                                                             
-231216 60294.00 P  0.159180 0.012478  0.212773 0.019618  P 0.0186751 0.0160858                                                                                                             
-231217 60295.00 P  0.156836 0.012513  0.212602 0.019687  P 0.0186863 0.0161461                                                                                                             
-231218 60296.00 P  0.154493 0.012547  0.212467 0.019756  P 0.0184044 0.0162063                                                                                                             
-231219 60297.00 P  0.152151 0.012582  0.212369 0.019824  P 0.0178740 0.0162665                                                                                                             
-231220 60298.00 P  0.149810 0.012616  0.212308 0.019893  P 0.0171976 0.0163265                                                                                                             
-231221 60299.00 P  0.147472 0.012651  0.212283 0.019961  P 0.0165063 0.0163866                                                                                                             
-231222 60300.00 P  0.145138 0.012685  0.212295 0.020030  P 0.0159272 0.0164465                                                                                                             
-231223 60301.00 P  0.142807 0.012719  0.212344 0.020098  P 0.0155534 0.0165063                                                                                                             
-231224 60302.00 P  0.140480 0.012753  0.212429 0.020166  P 0.0154262 0.0165661                                                                                                             
-231225 60303.00 P  0.138159 0.012787  0.212550 0.020234  P 0.0155333 0.0166258                                                                                                             
-231226 60304.00 P  0.135843 0.012821  0.212707 0.020302  P 0.0158223 0.0166855                                                                                                             
-231227 60305.00 P  0.133534 0.012855  0.212900 0.020370  P 0.0162144 0.0167451                                                                                                             
-231228 60306.00 P  0.131231 0.012889  0.213129 0.020438  P 0.0166167 0.0168046                                                                                                             
-231229 60307.00 P  0.128937 0.012923  0.213394 0.020506  P 0.0169465 0.0168640                                                                                                             
-231230 60308.00 P  0.126650 0.012957  0.213695 0.020574  P 0.0171649 0.0169233                                                                                                             
-231231 60309.00 P  0.124372 0.012991  0.214031 0.020641  P 0.0172859 0.0169826                                                                                                             
-24 1 1 60310.00 P  0.122104 0.013024  0.214403 0.020709  P 0.0173156 0.0170419                                                                                                             
-24 1 2 60311.00 P  0.119846 0.013058  0.214809 0.020776  P 0.0172388 0.0171010                                                                                                             
-24 1 3 60312.00 P  0.117599 0.013091  0.215251 0.020843  P 0.0170490 0.0171601                                                                                                             
-24 1 4 60313.00 P  0.115363 0.013125  0.215727 0.020911  P 0.0167657 0.0172191                                                                                                             
-24 1 5 60314.00 P  0.113139 0.013158  0.216238 0.020978  P 0.0164902 0.0172780                                                                                                             
-24 1 6 60315.00 P  0.110927 0.013191  0.216784 0.021045  P 0.0163037 0.0173369                                                                                                             
-24 1 7 60316.00 P  0.108729 0.013225  0.217364 0.021112  P 0.0161861 0.0173957                                                                                                             
-24 1 8 60317.00 P  0.106544 0.013258  0.217977 0.021179  P 0.0162250 0.0174545                                                                                                             
-24 1 9 60318.00 P  0.104374 0.013291  0.218624 0.021246  P 0.0164393 0.0175131                                                                                                             
-24 110 60319.00 P  0.102218 0.013324  0.219305 0.021313  P 0.0167400 0.0175718                                                                                                             
-24 111 60320.00 P  0.100078 0.013357  0.220019 0.021379  P 0.0171012 0.0176303                                                                                                             
-24 112 60321.00 P  0.097954 0.013390  0.220766 0.021446  P 0.0173851 0.0176888                                                                                                             
-24 113 60322.00 P  0.095847 0.013423  0.221545 0.021512  P 0.0173998 0.0177472                                                                                                             
-24 114 60323.00 P  0.093757 0.013456  0.222357 0.021579  P 0.0170933 0.0178055                                                                                                             
-24 115 60324.00 P  0.091684 0.013488  0.223201 0.021645  P 0.0164798 0.0178638                                                                                                             
-24 116 60325.00 P  0.089630 0.013521  0.224077 0.021711  P 0.0156854 0.0179220                                                                                                             
-24 117 60326.00 P  0.087594 0.013554  0.224984 0.021778  P 0.0149524 0.0179802                                                                                                             
-24 118 60327.00 P  0.085578 0.013586  0.225922 0.021844  P 0.0144053 0.0180383                                                                                                             
-24 119 60328.00 P  0.083582 0.013619  0.226891 0.021910  P 0.0141564 0.0180963                                                                                                             
-24 120 60329.00 P  0.081606 0.013651  0.227891 0.021976  P 0.0142418 0.0181543                                                                                                             
-24 121 60330.00 P  0.079651 0.013683  0.228921 0.022042  P 0.0145770 0.0182122                                                                                                             
-24 122 60331.00 P  0.077717 0.013716  0.229980 0.022107  P 0.0151148 0.0182700                                                                                                             
-24 123 60332.00 P  0.075806 0.013748  0.231069 0.022173  P 0.0157653 0.0183278                                                                                                             
-24 124 60333.00 P  0.073916 0.013780  0.232188 0.022239  P 0.0164975 0.0183855                                                                                                             
-24 125 60334.00 P  0.072050 0.013812  0.233335 0.022304  P 0.0172281 0.0184432                                                                                                             
-24 126 60335.00 P  0.070207 0.013845  0.234510 0.022370  P 0.0178879 0.0185008                                                                                                             
-24 127 60336.00 P  0.068388 0.013877  0.235713 0.022435  P 0.0184047 0.0185583                                                                                                             
-24 128 60337.00 P  0.066593 0.013909  0.236944 0.022501  P 0.0187388 0.0186158                                                                                                             
-24 129 60338.00 P  0.064824 0.013941  0.238202 0.022566  P 0.0188782 0.0186732                                                                                                             
-24 130 60339.00 P  0.063079 0.013972  0.239487 0.022631  P 0.0188329 0.0187306                                                                                                             
-24 131 60340.00 P  0.061360 0.014004  0.240798 0.022696  P 0.0187338 0.0187879                                                                                                             
-24 2 1 60341.00 P  0.059667 0.014036  0.242135 0.022761  P 0.0187172 0.0188451                                                                                                             
-24 2 2 60342.00 P  0.058001 0.014068  0.243497 0.022826  P 0.0187265 0.0189023                                                                                                             
-24 2 3 60343.00 P  0.056361 0.014099  0.244885 0.022891  P 0.0188416 0.0189594                                                                                                             
-24 2 4 60344.00 P  0.054749 0.014131  0.246297 0.022956  P 0.0191555 0.0190165                                                                                                             
-24 2 5 60345.00 P  0.053165 0.014163  0.247733 0.023021  P 0.0196285 0.0190735                                                                                                             
-24 2 6 60346.00 P  0.051609 0.014194  0.249193 0.023086  P 0.0203184 0.0191305                                                                                                             
-24 2 7 60347.00 P  0.050082 0.014226  0.250677 0.023150  P 0.0211126 0.0191874                                                                                                             
-24 2 8 60348.00 P  0.048583 0.014257  0.252183 0.023215  P 0.0218127 0.0192442                                                                                                             
-24 2 9 60349.00 P  0.047114 0.014288  0.253711 0.023279  P 0.0222873 0.0193010                                                                                                             
-24 210 60350.00 P  0.045675 0.014320  0.255262 0.023344  P 0.0223847 0.0193577                                                                                                             
-24 211 60351.00 P  0.044265 0.014351  0.256833 0.023408  P 0.0221236 0.0194144                                                                                                             
-24 212 60352.00 P  0.042886 0.014382  0.258426 0.023472  P 0.0216171 0.0194710                                                                                                             
-24 213 60353.00 P  0.041538 0.014413  0.260039 0.023537  P 0.0208840 0.0195276                                                                                                             
-24 214 60354.00 P  0.040221 0.014444  0.261672 0.023601  P 0.0201405 0.0195841                                                                                                             
-24 215 60355.00 P  0.038934 0.014475  0.263324 0.023665  P 0.0196365 0.0196405                                                                                                             
-24 216 60356.00 P  0.037680 0.014506  0.264995 0.023729  P 0.0193349 0.0196969                                                                                                             
-24 217 60357.00 P  0.036458 0.014537  0.266685 0.023793  P 0.0193549 0.0197532                                                                                                             
-24 218 60358.00 P  0.035267 0.014568  0.268393 0.023857  P 0.0195393 0.0198095                                                                                                             
-24 219 60359.00 P  0.034110 0.014599  0.270117 0.023921  P 0.0198757 0.0198658                                                                                                             
-24 220 60360.00 P  0.032985 0.014630  0.271859 0.023984  P 0.0202152 0.0199219                                                                                                             
-24 221 60361.00 P  0.031893 0.014661  0.273617 0.024048  P 0.0205229 0.0199781                                                                                                             
-24 222 60362.00 P  0.030834 0.014691  0.275391 0.024112  P 0.0207222 0.0200341                                                                                                             
-24 223 60363.00 P  0.029809 0.014722  0.277180 0.024175  P 0.0207513 0.0200902                                                                                                             
-24 224 60364.00 P  0.028817 0.014753  0.278984 0.024239  P 0.0205864 0.0201461                                                                                                             
-24 225 60365.00 P  0.027860 0.014783  0.280802 0.024302  P 0.0202677 0.0202021                                                                                                             
-24 226 60366.00 P  0.026937 0.014814  0.282633 0.024366  P 0.0197328 0.0202579                                                                                                             
-24 227 60367.00 P  0.026048 0.014844  0.284478 0.024429  P 0.0191359 0.0203137                                                                                                             
-24 228 60368.00 P  0.025193 0.014874  0.286335 0.024492  P 0.0185505 0.0203695                                                                                                             
-24 229 60369.00 P  0.024373 0.014905  0.288204 0.024555  P 0.0180182 0.0204252                                                                                                             
-24 3 1 60370.00 P  0.023589 0.014935  0.290085 0.024618  P 0.0176214 0.0204809                                                                                                             
-24 3 2 60371.00 P  0.022839 0.014965  0.291976 0.024681  P 0.0174195 0.0205365                                                                                                             
-24 3 3 60372.00 P  0.022124 0.014996  0.293878 0.024744  P 0.0174377 0.0205920                                                                                                             
-24 3 4 60373.00 P  0.021445 0.015026  0.295790 0.024807  P 0.0176575 0.0206475                                                                                                             
-24 3 5 60374.00 P  0.020801 0.015056  0.297711 0.024870  P 0.0180532 0.0207030                                                                                                             
-24 3 6 60375.00 P  0.020192 0.015086  0.299640 0.024933  P 0.0184609 0.0207584                                                                                                             
-24 3 7 60376.00 P  0.019620 0.015116  0.301577 0.024996  P 0.0187495 0.0208138                                                                                                             
-24 3 8 60377.00 P  0.019083 0.015146  0.303522 0.025058  P 0.0187446 0.0208691                                                                                                             
-24 3 9 60378.00 P  0.018582 0.015176  0.305474 0.025121  P 0.0183844 0.0209243                                                                                                             
-24 310 60379.00 P  0.018117 0.015206  0.307433 0.025184  P 0.0176192 0.0209795                                                                                                             
-24 311 60380.00 P  0.017687 0.015236  0.309397 0.025246  P 0.0165622 0.0210347                                                                                                             
-24 312 60381.00 P  0.017294 0.015266  0.311366 0.025309  P 0.0155738 0.0210898                                                                                                             
-24 313 60382.00 P  0.016937 0.015295  0.313340 0.025371  P 0.0147621 0.0211449                                                                                                             
-24 314 60383.00 P  0.016616 0.015325  0.315318 0.025433  P 0.0143211 0.0211999                                                                                                             
-24 315 60384.00 P  0.016331 0.015355  0.317300 0.025495  P 0.0141679 0.0212548                                                                                                             
-24 316 60385.00 P  0.016083 0.015385  0.319284 0.025558  P 0.0143408 0.0213098                                                                                                             
-24 317 60386.00 P  0.015870 0.015414  0.321271 0.025620  P 0.0146371 0.0213646                                                                                                             
-24 318 60387.00 P  0.015694 0.015444  0.323260 0.025682  P 0.0150142 0.0214195                                                                                                             
-24 319 60388.00 P  0.015553 0.015473  0.325250 0.025744  P 0.0153318 0.0214742                                                                                                             
-24 320 60389.00 P  0.015449 0.015503  0.327241 0.025806  P 0.0154823 0.0215290                                                                                                             
-24 321 60390.00 P  0.015381 0.015532  0.329231 0.025868  P 0.0154119 0.0215837                                                                                                             
-24 322 60391.00 P  0.015349 0.015561  0.331222 0.025930  P 0.0151088 0.0216383                                                                                                             
-24 323 60392.00 P  0.015352 0.015591  0.333211 0.025991  P 0.0145623 0.0216929                                                                                                             
-24 324 60393.00 P  0.015392 0.015620  0.335198 0.026053  P 0.0138748 0.0217474                                                                                                             
-24 325 60394.00 P  0.015467 0.015649  0.337184 0.026115  P 0.0131057 0.0218019                                                                                                             
-24 326 60395.00 P  0.015578 0.015679  0.339167 0.026176  P 0.0123224 0.0218564                                                                                                             
-24 327 60396.00 P  0.015725 0.015708  0.341146 0.026238  P 0.0116097 0.0219108                                                                                                             
-24 328 60397.00 P  0.015907 0.015737  0.343122 0.026299  P 0.0110313 0.0219652                                                                                                             
-24 329 60398.00 P  0.016124 0.015766  0.345093 0.026361  P 0.0105921 0.0220195                                                                                                             
-24 330 60399.00 P  0.016377 0.015795  0.347059 0.026422  P 0.0103740 0.0220738                                                                                                             
-24 331 60400.00 P  0.016665 0.015824  0.349020 0.026484  P 0.0103197 0.0221280                                                                                                             
-24 4 1 60401.00 P  0.016987 0.015853  0.350975 0.026545  P 0.0103822 0.0221822                                                                                                             
-24 4 2 60402.00 P  0.017345 0.015882  0.352923 0.026606  P 0.0104601 0.0222363                                                                                                             
-24 4 3 60403.00 P  0.017737 0.015911  0.354864 0.026667  P 0.0105190 0.0222904                                                                                                             
-24 4 4 60404.00 P  0.018163 0.015940  0.356797 0.026728  P 0.0103366 0.0223444                                                                                                             
-24 4 5 60405.00 P  0.018624 0.015969  0.358723 0.026790  P 0.0098859 0.0223985                                                                                                             
-24 4 6 60406.00 P  0.019119 0.015997  0.360639 0.026851  P 0.0090945 0.0224524                                                                                                             
-24 4 7 60407.00 P  0.019647 0.016026  0.362546 0.026912  P 0.0079451 0.0225063                                                                                                             
-24 4 8 60408.00 P  0.020209 0.016055  0.364443 0.026972  P 0.0066242 0.0225602                                                                                                             
-24 4 9 60409.00 P  0.020805 0.016084  0.366330 0.027033  P 0.0054011 0.0226140                                                                                                             
-24 410 60410.00 P  0.021433 0.016112  0.368206 0.027094  P 0.0044793 0.0226678                                                                                                             
-24 411 60411.00 P  0.022095 0.016141  0.370071 0.027155  P 0.0039168 0.0227216                                                                                                             
-24 412 60412.00 P  0.022789 0.016169  0.371924 0.027216  P 0.0037326 0.0227753                                                                                                             
-24 413 60413.00 P  0.023516 0.016198  0.373765 0.027276  P 0.0038197 0.0228290                                                                                                             
-24 414 60414.00 P  0.024274 0.016226  0.375592 0.027337  P 0.0040590 0.0228826                                                                                                             
-24 415 60415.00 P  0.025065 0.016255  0.377406 0.027397  P 0.0043839 0.0229362                                                                                                             
-24 416 60416.00 P  0.025887 0.016283  0.379207 0.027458  P 0.0046300 0.0229897                                                                                                             
-24 417 60417.00 P  0.026740 0.016312  0.380993 0.027518  P 0.0047702 0.0230432                                                                                                             
-24 418 60418.00 P  0.027624 0.016340  0.382764 0.027579  P 0.0047356 0.0230966                                                                                                             
-24 419 60419.00 P  0.028539 0.016368  0.384520 0.027639  P 0.0045312 0.0231500                                                                                                             
-24 420 60420.00 P  0.029484 0.016396  0.386260 0.027699  P 0.0041581 0.0232034                                                                                                             
-24 421 60421.00 P  0.030459 0.016425  0.387984 0.027759  P 0.0037453 0.0232567                                                                                                             
-24 422 60422.00 P  0.031463 0.016453  0.389691 0.027820  P 0.0031906 0.0233100                                                                                                             
-24 423 60423.00 P  0.032497 0.016481  0.391381 0.027880  P 0.0026789 0.0233633                                                                                                             
-24 424 60424.00 P  0.033560 0.016509  0.393053 0.027940  P 0.0023108 0.0234165                                                                                                             
-24 425 60425.00 P  0.034651 0.016537  0.394707 0.028000  P 0.0020967 0.0234697                                                                                                             
-24 426 60426.00 P  0.035770 0.016565  0.396343 0.028060  P 0.0020595 0.0235228                                                                                                             
-24 427 60427.00 P  0.036917 0.016593  0.397960 0.028120  P 0.0021795 0.0235759                                                                                                             
-24 428 60428.00 P  0.038092 0.016621  0.399557 0.028180  P 0.0024751 0.0236289                                                                                                             
-24 429 60429.00 P  0.039294 0.016649  0.401135 0.028239  P 0.0028136 0.0236819                                                                                                             
-24 430 60430.00 P  0.040522 0.016677  0.402692 0.028299  P 0.0031425 0.0237349                                                                                                             
-24 5 1 60431.00 P  0.041776 0.016705  0.404229 0.028359  P 0.0033937 0.0237878                                                                                                             
-24 5 2 60432.00 P  0.043056 0.016733  0.405745 0.028419  P 0.0034691 0.0238407                                                                                                             
-24 5 3 60433.00 P  0.044362 0.016760  0.407239 0.028478  P 0.0032130 0.0238935                                                                                                             
-24 5 4 60434.00 P  0.045692 0.016788  0.408712 0.028538  P 0.0027041 0.0239463                                                                                                             
-24 5 5 60435.00 P  0.047047 0.016816  0.410162 0.028597  P 0.0020247 0.0239991                                                                                                             
-24 5 6 60436.00 P  0.048426 0.016844  0.411590 0.028657  P 0.0013245 0.0240518                                                                                                             
-24 5 7 60437.00 P  0.049829 0.016871  0.412995 0.028716  P 0.0007864 0.0241045                                                                                                             
-24 5 8 60438.00 P  0.051255 0.016899  0.414377 0.028776  P 0.0006022 0.0241572                                                                                                             
-24 5 9 60439.00 P  0.052703 0.016926  0.415735 0.028835  P 0.0007608 0.0242098                                                                                                             
-24 510 60440.00 P  0.054174 0.016954  0.417069 0.028894  P 0.0012404 0.0242624                                                                                                             
-24 511 60441.00 P  0.055666 0.016982  0.418379 0.028954  P 0.0019716 0.0243149                                                                                                             
-24 512 60442.00 P  0.057180 0.017009  0.419664 0.029013  P 0.0027486 0.0243674                                                                                                             
-24 513 60443.00 P  0.058715 0.017036  0.420925 0.029072  P 0.0035218 0.0244199                                                                                                             
-24 514 60444.00 P  0.060269 0.017064  0.422160 0.029131  P 0.0042165 0.0244723                                                                                                             
-24 515 60445.00 P  0.061844 0.017091  0.423369 0.029190  P 0.0047941 0.0245247                                                                                                             
-24 516 60446.00 P  0.063438 0.017119  0.424553 0.029249  P 0.0052143 0.0245770                                                                                                             
-24 517 60447.00 P  0.065051 0.017146  0.425711 0.029308  P 0.0055141 0.0246293                                                                                                             
-24 518 60448.00 P  0.066682 0.017173  0.426842 0.029367  P 0.0057337 0.0246816                                                                                                             
-24 519 60449.00 P  0.068331 0.017200  0.427946 0.029426  P 0.0058762 0.0247338                                                                                                             
-24 520 60450.00 P  0.069997 0.017228  0.429024 0.029485  P 0.0059805 0.0247860                                                                                                             
-24 521 60451.00 P  0.071680 0.017255  0.430074 0.029543  P 0.0061402 0.0248382                                                                                                             
-24 522 60452.00 P  0.073379 0.017282  0.431097 0.029602  P 0.0064430 0.0248903                                                                                                             
-24 523 60453.00 P  0.075094 0.017309  0.432092 0.029661  P 0.0069648 0.0249424                                                                                                             
-24 524 60454.00 P  0.076824 0.017336  0.433060 0.029720  P 0.0077172 0.0249945                                                                                                             
-24 525 60455.00 P  0.078569 0.017363  0.433999 0.029778  P 0.0086499 0.0250465                                                                                                             
-24 526 60456.00 P  0.080328 0.017390  0.434910 0.029837  P 0.0097066 0.0250985                                                                                                             
-24 527 60457.00 P  0.082100 0.017417  0.435792 0.029895  P 0.0106961 0.0251504                                                                                                             
-24 528 60458.00 P  0.083886 0.017444  0.436645 0.029954  P 0.0115734 0.0252023                                                                                                             
-24 529 60459.00 P  0.085684 0.017471  0.437470 0.030012  P 0.0122381 0.0252542                                                                                                             
-24 530 60460.00 P  0.087494 0.017498  0.438265 0.030070  P 0.0125876 0.0253060                                                                                                             
-24 531 60461.00 P  0.089315 0.017525  0.439032 0.030129  P 0.0126809 0.0253578                                                                                                             
-24 6 1 60462.00 P  0.091147 0.017552  0.439768 0.030187  P 0.0126419 0.0254096                                                                                                             
-24 6 2 60463.00                                                                                                                                                                            
-24 6 3 60464.00                                                                                                                                                                            
-24 6 4 60465.00                                                                                                                                                                            
-24 6 5 60466.00                                                                                                                                                                            
-24 6 6 60467.00                                                                                                                                                                            
-24 6 7 60468.00                                                                                                                                                                            
-24 6 8 60469.00                                                                                                                                                                            
-24 6 9 60470.00                                                                                                                                                                            
-24 610 60471.00                                                                                                                                                                            
-24 611 60472.00                                                                                                                                                                            
-24 612 60473.00                                                                                                                                                                            
-24 613 60474.00                                                                                                                                                                            
-24 614 60475.00                                                                                                                                                                            
-24 615 60476.00                                                                                                                                                                            
-24 616 60477.00                                                                                                                                                                            
-24 617 60478.00                                                                                                                                                                            
-24 618 60479.00                                                                                                                                                                            
-24 619 60480.00                                                                                                                                                                            
-24 620 60481.00                                                                                                                                                                            
-24 621 60482.00                                                                                                                                                                            
-24 622 60483.00                                                                                                                                                                            
-24 623 60484.00                                                                                                                                                                            
-24 624 60485.00                                                                                                                                                                            
-24 625 60486.00                                                                                                                                                                            
-24 626 60487.00                                                                                                                                                                            
-24 627 60488.00                                                                                                                                                                            
-24 628 60489.00                                                                                                                                                                            
-24 629 60490.00                                                                                                                                                                            
-24 630 60491.00                                                                                                                                                                            
-24 7 1 60492.00                                                                                                                                                                            
-24 7 2 60493.00                                                                                                                                                                            
-24 7 3 60494.00                                                                                                                                                                            
-24 7 4 60495.00                                                                                                                                                                            
-24 7 5 60496.00                                                                                                                                                                            
-24 7 6 60497.00                                                                                                                                                                            
+201226 59209.00 I  0.075986 0.000025  0.297953 0.000018  I-0.1785028 0.0000076 -0.2136 0.0050  I  -110.324    0.112    -5.248    0.181  0.076029  0.297933 -0.1785155  -110.588    -5.069  
+201227 59210.00 I  0.075021 0.000043  0.298714 0.000042  I-0.1782078 0.0000059 -0.3720 0.0045  I  -110.270    0.322    -5.191    0.160  0.075042  0.298659 -0.1782196  -110.593    -4.992  
+201228 59211.00 I  0.073953 0.000045  0.299954 0.000049  I-0.1777715 0.0000050 -0.4923 0.0038  I  -110.287    0.322    -5.339    0.160  0.074002  0.299890 -0.1777873  -110.681    -5.121  
+201229 59212.00 I  0.072644 0.000047  0.301496 0.000049  I-0.1772387 0.0000049 -0.5661 0.0035  I  -110.331    0.322    -5.616    0.160  0.072652  0.301612 -0.1772435  -110.800    -5.378  
+201230 59213.00 I  0.071189 0.000048  0.302560 0.000049  I-0.1766424 0.0000049 -0.6306 0.0031  I  -110.229    0.322    -5.859    0.160  0.071166  0.302626 -0.1766471  -110.575    -5.713  
+201231 59214.00 I  0.069767 0.000053  0.303105 0.000049  I-0.1759902 0.0000037 -0.6569 0.0047  I  -109.891    0.322    -5.959    0.160  0.069727  0.303062 -0.1760031  -110.137    -5.856  
+21 1 1 59215.00 I  0.068691 0.000053  0.304048 0.000048  I-0.1753606 0.0000080 -0.5872 0.0054  I  -109.393    0.322    -6.022    0.160  0.068654  0.303977 -0.1753760  -109.613    -5.841  
+21 1 2 59216.00 I  0.067678 0.000027  0.305445 0.000021  I-0.1748408 0.0000101 -0.4424 0.0051  I  -109.009    0.322    -5.936    0.160  0.067783  0.305455 -0.1748394  -109.207    -5.801  
+21 1 3 59217.00 I  0.066045 0.000027  0.306735 0.000030  I-0.1744883 0.0000062 -0.2600 0.0059  I  -108.783    0.413    -5.883    0.064  0.066068  0.306714 -0.1744761  -108.905    -5.788  
+21 1 4 59218.00 I  0.063870 0.000023  0.307765 0.000030  I-0.1743298 0.0000062 -0.0505 0.0044  I  -108.655    0.413    -5.865    0.064  0.063906  0.307809 -0.1743246  -108.696    -5.815  
+21 1 5 59219.00 I  0.061814 0.000022  0.308629 0.000030  I-0.1743807 0.0000063  0.1391 0.0041  I  -108.589    0.413    -5.821    0.064  0.061685  0.308623 -0.1743819  -108.543    -5.819  
+21 1 6 59220.00 I  0.060433 0.000027  0.309510 0.000044  I-0.1745789 0.0000055  0.2414 0.0036  I  -108.656    0.413    -5.700    0.064  0.060391  0.309503 -0.1746023  -108.462    -5.682  
+21 1 7 59221.00 I  0.059583 0.000028  0.310269 0.000045  I-0.1748375 0.0000033  0.2657 0.0032  I  -108.937    0.413    -5.516    0.064  0.059466  0.310304 -0.1748751  -108.581    -5.464  
+21 1 8 59222.00 I  0.058950 0.000030  0.311083 0.000046  I-0.1750651 0.0000034  0.1544 0.0023  I  -109.389    0.413    -5.362    0.064  0.059005  0.311054 -0.1750757  -108.877    -5.271  
+21 1 9 59223.00 I  0.058323 0.000026  0.311977 0.000036  I-0.1751023 0.0000033 -0.0889 0.0028  I  -109.834    0.322    -5.324    0.160  0.058270  0.311975 -0.1750823  -109.379    -5.254  
+21 110 59224.00 I  0.057967 0.000030  0.313025 0.000055  I-0.1748876 0.0000044 -0.3313 0.0027  I  -110.076    0.444    -5.397    0.164  0.058057  0.313002 -0.1748654  -109.768    -5.367  
+21 111 59225.00 I  0.057559 0.000030  0.314057 0.000055  I-0.1744740 0.0000044 -0.4708 0.0032  I  -110.037    0.444    -5.486    0.164  0.057636  0.314178 -0.1744765  -109.894    -5.482  
+21 112 59226.00 I  0.056939 0.000026  0.314652 0.000045  I-0.1739718 0.0000047 -0.5330 0.0033  I  -109.788    0.444    -5.528    0.164  0.057033  0.314438 -0.1739724  -109.829    -5.535  
+21 113 59227.00 I  0.056041 0.000026  0.315411 0.000048  I-0.1734203 0.0000050 -0.5582 0.0034  I  -109.115    0.926    -5.837    0.104  0.056028  0.315487 -0.1734272  -109.447    -5.630  
+21 114 59228.00 I  0.054983 0.000023  0.316090 0.000047  I-0.1728944 0.0000050 -0.4663 0.0035  I  -108.891    0.926    -5.894    0.104  0.054873  0.316051 -0.1729081  -108.989    -5.826  
+21 115 59229.00 I  0.054316 0.000021  0.316871 0.000048  I-0.1724715 0.0000050 -0.4228 0.0039  I  -108.680    0.926    -6.020    0.104  0.054335  0.316875 -0.1724606  -108.538    -6.095  
+21 116 59230.00 I  0.053770 0.000017  0.317806 0.000024  I-0.1720571 0.0000061 -0.3544 0.0037  I  -108.544    0.926    -6.084    0.104  0.053758  0.317833 -0.1721004  -108.364    -6.182  
+21 117 59231.00 I  0.053040 0.000019  0.318728 0.000032  I-0.1717852 0.0000054 -0.2187 0.0041  I  -108.570    0.783    -5.998    0.150  0.052962  0.318726 -0.1718081  -108.435    -6.070  
+21 118 59232.00 I  0.052519 0.000020  0.319453 0.000031  I-0.1715870 0.0000054 -0.1813 0.0036  I  -108.779    0.783    -5.819    0.150  0.052474  0.319502 -0.1715790  -108.695    -5.858  
+21 119 59233.00 I  0.052578 0.000020  0.320015 0.000025  I-0.1714154 0.0000047 -0.1654 0.0036  I  -109.085    0.544    -5.684    0.191  0.052506  0.319950 -0.1714126  -109.065    -5.679  
+21 120 59234.00 I  0.052771 0.000027  0.320924 0.000042  I-0.1712499 0.0000048 -0.1682 0.0034  I  -109.356    0.568    -5.642    0.154  0.052837  0.320909 -0.1712427  -109.276    -5.677  
+21 121 59235.00 I  0.052579 0.000027  0.321983 0.000041  I-0.1710607 0.0000048 -0.2257 0.0033  I  -109.497    0.568    -5.615    0.154  0.052498  0.321943 -0.1710484  -109.337    -5.704  
+21 122 59236.00 I  0.052405 0.000027  0.323082 0.000041  I-0.1707998 0.0000046 -0.2792 0.0036  I  -109.484    0.626    -5.582    0.027  0.052370  0.323115 -0.1707975  -109.260    -5.651  
+21 123 59237.00 I  0.052364 0.000025  0.324261 0.000035  I-0.1704878 0.0000054 -0.3762 0.0042  I  -109.372    0.626    -5.426    0.027  0.052397  0.324238 -0.1704758  -109.170    -5.507  
+21 124 59238.00 I  0.051875 0.000032  0.325654 0.000049  I-0.1700259 0.0000070 -0.5378 0.0045  I  -109.268    0.616    -5.367    0.100  0.051888  0.325635 -0.1700327  -109.121    -5.441  
+21 125 59239.00 I  0.051012 0.000031  0.327161 0.000049  I-0.1694244 0.0000071 -0.6628 0.0056  I  -109.235    0.616    -5.517    0.100  0.050946  0.327158 -0.1694247  -109.156    -5.579  
+21 126 59240.00 I  0.050368 0.000025  0.328687 0.000036  I-0.1687147 0.0000087 -0.7444 0.0056  I  -109.262    0.614    -5.810    0.117  0.050305  0.328651 -0.1687165  -109.246    -5.884  
+21 127 59241.00 I  0.050035 0.000025  0.330502 0.000045  I-0.1679717 0.0000086 -0.7175 0.0061  I  -109.142    0.734    -6.182    0.094  0.050009  0.330496 -0.1680026  -109.141    -6.231  
+21 128 59242.00 I  0.049906 0.000026  0.332425 0.000045  I-0.1673316 0.0000086 -0.5348 0.0060  I  -108.860    0.734    -6.397    0.094  0.049854  0.332424 -0.1673675  -108.815    -6.433  
+21 129 59243.00 I  0.049886 0.000025  0.334338 0.000045  I-0.1669136 0.0000083 -0.3176 0.0060  I  -108.454    0.734    -6.400    0.094  0.049925  0.334359 -0.1669073  -108.303    -6.429  
+21 130 59244.00 I  0.049606 0.000016  0.336136 0.000029  I-0.1666923 0.0000083 -0.1126 0.0050  I  -108.090    0.998    -6.271    0.025  0.049593  0.336126 -0.1666565  -107.964    -6.280  
+21 131 59245.00 I  0.049361 0.000016  0.337912 0.000036  I-0.1667111 0.0000054  0.1606 0.0049  I  -107.928    0.469    -6.151    0.029  0.049315  0.337874 -0.1666887  -107.846    -6.140  
+21 2 1 59246.00 I  0.049428 0.000016  0.339852 0.000036  I-0.1670144 0.0000052  0.4366 0.0031  I  -108.028    0.469    -6.129    0.029  0.049421  0.339866 -0.1670204  -107.967    -6.108  
+21 2 2 59247.00 I  0.049459 0.000015  0.341657 0.000023  I-0.1675564 0.0000030  0.6290 0.0029  I  -108.337    0.269    -6.177    0.031  0.049490  0.341692 -0.1675614  -108.292    -6.165  
+21 2 3 59248.00 I  0.049299 0.000018  0.343145 0.000039  I-0.1682175 0.0000024  0.6567 0.0020  I  -108.735    0.288    -6.205    0.033  0.049274  0.343178 -0.1681920  -108.630    -6.177  
+21 2 4 59249.00 I  0.049231 0.000019  0.344374 0.000039  I-0.1688232 0.0000027  0.5445 0.0018  I  -109.131    0.288    -6.153    0.033  0.049231  0.344351 -0.1688000  -108.983    -6.111  
+21 2 5 59250.00 I  0.049260 0.000018  0.345639 0.000039  I-0.1692847 0.0000027  0.3667 0.0018  I  -109.235    0.504    -5.972    0.047  0.049262  0.345628 -0.1692802  -109.304    -6.001  
+21 2 6 59251.00 I  0.049170 0.000016  0.346997 0.000032  I-0.1695447 0.0000023  0.1530 0.0026  I  -109.439    0.504    -5.910    0.047  0.049156  0.346983 -0.1696139  -109.483    -5.921  
+21 2 7 59252.00 I  0.049118 0.000017  0.348390 0.000036  I-0.1695977 0.0000044 -0.0399 0.0025  I  -109.437    0.480    -5.906    0.197  0.049075  0.348358 -0.1696850  -109.454    -5.901  
+21 2 8 59253.00 I  0.049360 0.000017  0.349884 0.000036  I-0.1694906 0.0000044 -0.1559 0.0036  I  -109.223    0.480    -5.954    0.197  0.049311  0.349885 -0.1694924  -109.221    -5.926  
+21 2 9 59254.00 I  0.049920 0.000015  0.351324 0.000020  I-0.1693336 0.0000058 -0.1288 0.0042  I  -108.917    0.474    -6.005    0.220  0.049922  0.351343 -0.1693373  -108.874    -5.989  
+21 210 59255.00 I  0.050595 0.000019  0.352614 0.000032  I-0.1692534 0.0000072 -0.0405 0.0046  I  -108.558    0.636    -6.185    0.159  0.050607  0.352626 -0.1692436  -108.510    -6.178  
+21 211 59256.00 I  0.051150 0.000019  0.353811 0.000033  I-0.1692598 0.0000072  0.0693 0.0051  I  -108.331    0.636    -6.405    0.159  0.051207  0.353801 -0.1692657  -108.257    -6.433  
+21 212 59257.00 I  0.051354 0.000021  0.354907 0.000034  I-0.1694129 0.0000072  0.2417 0.0058  I  -108.232    0.636    -6.604    0.159  0.051383  0.354941 -0.1694090  -108.111    -6.679  
+21 213 59258.00 I  0.051524 0.000020  0.355727 0.000029  I-0.1697391 0.0000092  0.4019 0.0060  I  -108.195    0.783    -6.705    0.037  0.051474  0.355706 -0.1697045  -108.084    -6.767  
+21 214 59259.00 I  0.051835 0.000020  0.356786 0.000029  I-0.1701992 0.0000095  0.5097 0.0055  I  -108.199    0.783    -6.693    0.037  0.051922  0.356756 -0.1701305  -108.104    -6.728  
+21 215 59260.00 I  0.051651 0.000035  0.358119 0.000043  I-0.1707272 0.0000059  0.5236 0.0050  I  -108.285    0.735    -6.635    0.126  0.051716  0.358143 -0.1706473  -108.193    -6.652  
+21 216 59261.00 I  0.050957 0.000032  0.359271 0.000035  I-0.1712255 0.0000033  0.4746 0.0038  I  -108.517    0.707    -6.519    0.169  0.050949  0.359283 -0.1711965  -108.366    -6.610  
+21 217 59262.00 I  0.050404 0.000040  0.360288 0.000050  I-0.1716618 0.0000047  0.3816 0.0029  I  -108.657    0.664    -6.566    0.192  0.050326  0.360338 -0.1716669  -108.536    -6.606  
+21 218 59263.00 I  0.050428 0.000040  0.361156 0.000049  I-0.1719484 0.0000048  0.1676 0.0034  I  -108.681    0.664    -6.596    0.192  0.050378  0.361154 -0.1719511  -108.669    -6.586  
+21 219 59264.00 I  0.050877 0.000040  0.362008 0.000049  I-0.1720054 0.0000050 -0.0213 0.0036  I  -108.591    0.664    -6.583    0.192  0.050885  0.361987 -0.1720228  -108.704    -6.521  
+21 220 59265.00 I  0.051398 0.000040  0.363043 0.000049  I-0.1719070 0.0000053 -0.2068 0.0038  I  -108.482    0.664    -6.576    0.192  0.051501  0.363070 -0.1719007  -108.603    -6.534  
+21 221 59266.00 I  0.051364 0.000031  0.363875 0.000044  I-0.1715738 0.0000056 -0.4463 0.0038  I  -108.412    0.560    -6.654    0.153  0.051463  0.363914 -0.1715820  -108.490    -6.656  
+21 222 59267.00 I  0.050693 0.000031  0.364570 0.000044  I-0.1710543 0.0000055 -0.5660 0.0039  I  -108.357    0.560    -6.853    0.153  0.050700  0.364562 -0.1710795  -108.387    -6.899  
+21 223 59268.00 I  0.049876 0.000021  0.365237 0.000025  I-0.1704603 0.0000053 -0.6302 0.0039  I  -108.311    0.558    -7.204    0.037  0.049836  0.365309 -0.1704677  -108.274    -7.237  
+21 224 59269.00 I  0.049504 0.000022  0.365611 0.000044  I-0.1698306 0.0000055 -0.5842 0.0037  I  -108.284    0.512    -7.501    0.056  0.049396  0.365588 -0.1698548  -108.271    -7.557  
+21 225 59270.00 I  0.049816 0.000023  0.366109 0.000044  I-0.1693395 0.0000053 -0.3955 0.0037  I  -108.245    0.512    -7.737    0.056  0.049801  0.366059 -0.1693475  -108.285    -7.804  
+21 226 59271.00 I  0.050257 0.000023  0.367127 0.000044  I-0.1690595 0.0000050 -0.1473 0.0041  I  -108.047    0.512    -7.815    0.056  0.050306  0.367069 -0.1690477  -108.145    -7.894  
+21 227 59272.00 I  0.050421 0.000017  0.368560 0.000037  I-0.1690533 0.0000062  0.1259 0.0039  I  -107.624    0.400    -7.688    0.073  0.050431  0.368528 -0.1690351  -107.687    -7.757  
+21 228 59273.00 I  0.050493 0.000027  0.370230 0.000048  I-0.1693069 0.0000061  0.3859 0.0043  I  -107.191    0.498    -7.448    0.051  0.050498  0.370227 -0.1693081  -107.188    -7.498  
+21 3 1 59274.00 I  0.050627 0.000027  0.371997 0.000049  I-0.1698038 0.0000059  0.5821 0.0043  I  -107.089    0.498    -7.289    0.051  0.050616  0.371982 -0.1697877  -107.024    -7.321  
+21 3 2 59275.00 I  0.050673 0.000025  0.373718 0.000032  I-0.1704164 0.0000062  0.6141 0.0042  I  -107.399    0.554    -7.314    0.025  0.050706  0.373771 -0.1703934  -107.298    -7.344  
+21 3 3 59276.00 I  0.050672 0.000027  0.375237 0.000050  I-0.1710185 0.0000061  0.6056 0.0043  I  -107.951    0.513    -7.500    0.040  0.050584  0.375262 -0.1710261  -107.867    -7.504  
+21 3 4 59277.00 I  0.051148 0.000027  0.376535 0.000050  I-0.1715856 0.0000061  0.4710 0.0043  I  -108.369    0.513    -7.639    0.040  0.051059  0.376549 -0.1715540  -108.333    -7.617  
+21 3 5 59278.00 I  0.052209 0.000027  0.377893 0.000050  I-0.1719085 0.0000061  0.1804 0.0044  I  -108.517    0.513    -7.643    0.040  0.052201  0.377870 -0.1718838  -108.535    -7.596  
+21 3 6 59279.00 I  0.053359 0.000017  0.379382 0.000039  I-0.1719688 0.0000064 -0.0430 0.0040  I  -108.460    0.388    -7.567    0.070  0.053360  0.379379 -0.1719881  -108.484    -7.535  
+21 3 7 59280.00 I  0.054609 0.000016  0.380848 0.000046  I-0.1718500 0.0000053 -0.1840 0.0041  I  -108.297    0.520    -7.505    0.067  0.054561  0.380833 -0.1718731  -108.315    -7.503  
+21 3 8 59281.00 I  0.056160 0.000016  0.382346 0.000046  I-0.1716151 0.0000050 -0.2820 0.0036  I  -108.045    0.520    -7.514    0.067  0.056191  0.382351 -0.1716080  -108.062    -7.541  
+21 3 9 59282.00 I  0.057605 0.000013  0.383884 0.000027  I-0.1713208 0.0000048 -0.2756 0.0033  I  -107.681    0.561    -7.620    0.066  0.057662  0.383909 -0.1713243  -107.722    -7.670  
+21 310 59283.00 I  0.058708 0.000019  0.385235 0.000040  I-0.1711047 0.0000042 -0.1468 0.0032  I  -107.335    0.555    -7.796    0.113  0.058750  0.385265 -0.1710993  -107.388    -7.839  
+21 311 59284.00 I  0.059636 0.000019  0.386402 0.000040  I-0.1710279 0.0000041 -0.0158 0.0029  I  -107.123    0.555    -7.985    0.113  0.059621  0.386346 -0.1710012  -107.198    -8.012  
+21 312 59285.00 I  0.060590 0.000019  0.387760 0.000040  I-0.1710769 0.0000039  0.1268 0.0023  I  -107.103    0.555    -8.082    0.113  0.060542  0.387744 -0.1710599  -107.204    -8.099  
+21 313 59286.00 I  0.061753 0.000018  0.389365 0.000032  I-0.1712857 0.0000020  0.2821 0.0032  I  -107.174    0.547    -8.025    0.147  0.061723  0.389349 -0.1712387  -107.275    -8.029  
+21 314 59287.00 I  0.063042 0.000023  0.391005 0.000041  I-0.1716108 0.0000050  0.3464 0.0027  I  -107.210    0.700    -7.872    0.112  0.063046  0.391028 -0.1715574  -107.295    -7.866  
+21 315 59288.00 I  0.064316 0.000024  0.392543 0.000041  I-0.1719493 0.0000050  0.3232 0.0041  I  -107.195    0.700    -7.758    0.112  0.064331  0.392504 -0.1719515  -107.259    -7.749  
+21 316 59289.00 I  0.065270 0.000019  0.394203 0.000028  I-0.1722327 0.0000065  0.2265 0.0035  I  -107.186    0.796    -7.770    0.068  0.065375  0.394218 -0.1722335  -107.205    -7.755  
+21 317 59290.00 I  0.065642 0.000026  0.395929 0.000045  I-0.1723871 0.0000049  0.0841 0.0040  I  -107.188    0.689    -7.868    0.054  0.065657  0.395943 -0.1724026  -107.211    -7.870  
+21 318 59291.00 I  0.065874 0.000026  0.397445 0.000045  I-0.1724047 0.0000048 -0.0468 0.0035  I  -107.149    0.689    -7.959    0.054  0.065853  0.397460 -0.1724204  -107.178    -7.981  
+21 319 59292.00 I  0.066218 0.000027  0.398940 0.000045  I-0.1722889 0.0000050 -0.1916 0.0030  I  -107.086    0.689    -8.020    0.054  0.066235  0.398938 -0.1722871  -107.117    -8.061  
+21 320 59293.00 I  0.066657 0.000023  0.400398 0.000037  I-0.1720295 0.0000037 -0.3125 0.0031  I  -107.068    0.577    -8.112    0.038  0.066580  0.400421 -0.1720284  -107.085    -8.161  
+21 321 59294.00 I  0.067553 0.000022  0.401822 0.000037  I-0.1716901 0.0000038 -0.3549 0.0034  I  -107.066    0.577    -8.273    0.038  0.067507  0.401767 -0.1716900  -107.075    -8.325  
+21 322 59295.00 I  0.068767 0.000025  0.403491 0.000049  I-0.1713329 0.0000056 -0.3578 0.0042  I  -106.926    0.589    -8.452    0.082  0.068766  0.403525 -0.1713132  -106.939    -8.503  
+21 323 59296.00 I  0.070030 0.000018  0.405082 0.000035  I-0.1709787 0.0000074 -0.3480 0.0040  I  -106.625    0.593    -8.520    0.104  0.070017  0.405095 -0.1709575  -106.635    -8.632  
+21 324 59297.00 I  0.071466 0.000020  0.406495 0.000044  I-0.1706717 0.0000056 -0.2338 0.0046  I  -106.321    0.624    -8.689    0.073  0.071509  0.406504 -0.1706787  -106.371    -8.750  
+21 325 59298.00 I  0.072762 0.000020  0.407848 0.000044  I-0.1705336 0.0000055 -0.0520 0.0040  I  -106.229    0.624    -8.931    0.073  0.072812  0.407873 -0.1705313  -106.284    -8.978  
+21 326 59299.00 I  0.073770 0.000020  0.408995 0.000044  I-0.1705906 0.0000057  0.1984 0.0040  I  -106.181    0.651    -9.218    0.013  0.073728  0.409056 -0.1705938  -106.226    -9.237  
+21 327 59300.00 I  0.074995 0.000019  0.409612 0.000044  I-0.1709346 0.0000057  0.4615 0.0044  I  -105.829    0.651    -9.270    0.013  0.074948  0.409668 -0.1709185  -105.910    -9.285  
+21 328 59301.00 I  0.076576 0.000020  0.409846 0.000041  I-0.1714975 0.0000068  0.6763 0.0044  I  -105.352    0.696    -9.043    0.042  0.076573  0.409823 -0.1714942  -105.462    -9.044  
+21 329 59302.00 I  0.078199 0.000020  0.410129 0.000041  I-0.1722581 0.0000068  0.8039 0.0052  I  -105.225    0.696    -8.743    0.042  0.078236  0.410129 -0.1722454  -105.357    -8.732  
+21 330 59303.00 I  0.079555 0.000026  0.410483 0.000051  I-0.1730454 0.0000078  0.7517 0.0052  I  -105.650    0.957    -8.667    0.060  0.079581  0.410456 -0.1730409  -105.788    -8.649  
+21 331 59304.00 I  0.080666 0.000026  0.411078 0.000051  I-0.1737276 0.0000080  0.5978 0.0054  I  -106.271    0.957    -8.848    0.060  0.080692  0.411065 -0.1737315  -106.343    -8.857  
+21 4 1 59305.00 I  0.081551 0.000027  0.411749 0.000051  I-0.1742206 0.0000076  0.3826 0.0054  I  -106.615    0.957    -9.053    0.060  0.081597  0.411745 -0.1742201  -106.573    -9.100  
+21 4 2 59306.00 I  0.082249 0.000026  0.412533 0.000051  I-0.1744958 0.0000073  0.1764 0.0044  I  -107.388    0.322    -8.989    0.160  0.082266  0.412527 -0.1744884  -106.526    -9.134  
+21 4 3 59307.00 I  0.082889 0.000023  0.413361 0.000042  I-0.1745772 0.0000045 -0.0184 0.0043  I  -107.155    0.322    -8.933    0.160  0.082863  0.413394 -0.1745594  -106.357    -9.054  
+21 4 4 59308.00 I  0.083737 0.000023  0.413941 0.000042  I-0.1744947 0.0000046 -0.1063 0.0029  I  -106.932    0.322    -8.908    0.160  0.083694  0.413955 -0.1744710  -106.265    -8.993  
+21 4 5 59309.00 I  0.084848 0.000014  0.414539 0.000027  I-0.1744238 0.0000035 -0.0168 0.0029  I  -106.781    0.394    -8.949    0.136  0.084866  0.414476 -0.1744009  -106.290    -8.990  
+21 4 6 59310.00 I  0.085827 0.000014  0.415614 0.000027  I-0.1744684 0.0000035  0.0944 0.0024  I  -106.586    0.394    -9.030    0.136  0.085863  0.415604 -0.1744328  -106.306    -9.021  
+21 4 7 59311.00 I  0.086621 0.000017  0.416784 0.000040  I-0.1746088 0.0000032  0.1940 0.0023  I  -106.259    0.567    -9.134    0.092  0.086636  0.416842 -0.1745974  -106.207    -9.070  
+21 4 8 59312.00 I  0.087297 0.000017  0.417765 0.000040  I-0.1748729 0.0000031  0.3429 0.0023  I  -105.883    0.567    -9.222    0.092  0.087374  0.417758 -0.1748862  -105.886    -9.192  
+21 4 9 59313.00 I  0.087572 0.000016  0.418797 0.000040  I-0.1752809 0.0000033  0.4506 0.0023  I  -105.647    0.567    -9.205    0.092  0.087621  0.418801 -0.1752874  -105.640    -9.234  
+21 410 59314.00 I  0.087455 0.000015  0.419882 0.000039  I-0.1757602 0.0000033  0.5167 0.0026  I  -105.632    0.567    -9.015    0.092  0.087511  0.419908 -0.1757729  -105.648    -9.045  
+21 411 59315.00 I  0.087102 0.000024  0.420737 0.000050  I-0.1763028 0.0000041  0.5482 0.0026  I  -105.744    0.671    -8.731    0.020  0.087081  0.420785 -0.1762939  -105.773    -8.744  
+21 412 59316.00 I  0.086813 0.000027  0.421362 0.000050  I-0.1768210 0.0000041  0.4729 0.0045  I  -105.837    0.671    -8.554    0.020  0.086768  0.421358 -0.1767986  -105.846    -8.552  
+21 413 59317.00 I  0.086940 0.000026  0.421867 0.000042  I-0.1772510 0.0000080  0.4047 0.0033  I  -105.850    0.832    -8.619    0.038  0.086839  0.421892 -0.1772455  -105.810    -8.603  
+21 414 59318.00 I  0.087730 0.000029  0.422438 0.000051  I-0.1776221 0.0000051  0.3117 0.0047  I  -105.795    0.646    -8.863    0.039  0.087692  0.422398 -0.1776055  -105.761    -8.851  
+21 415 59319.00 I  0.088783 0.000030  0.423233 0.000051  I-0.1778606 0.0000050  0.1775 0.0036  I  -105.720    0.646    -9.116    0.039  0.088768  0.423267 -0.1778557  -105.691    -9.111  
+21 416 59320.00 I  0.090122 0.000030  0.423814 0.000051  I-0.1779905 0.0000050  0.0837 0.0031  I  -105.716    0.646    -9.299    0.039  0.089996  0.423845 -0.1779907  -105.670    -9.299  
+21 417 59321.00 I  0.092135 0.000022  0.424360 0.000033  I-0.1780302 0.0000038 -0.0033 0.0031  I  -105.864    0.612    -9.475    0.039  0.092158  0.424284 -0.1780250  -105.805    -9.475  
+21 418 59322.00 I  0.094197 0.000020  0.425249 0.000039  I-0.1779901 0.0000036 -0.0715 0.0026  I  -106.075    0.380    -9.693    0.060  0.094246  0.425257 -0.1779868  -106.010    -9.693  
+21 419 59323.00 I  0.095895 0.000019  0.426264 0.000038  I-0.1779059 0.0000036 -0.0835 0.0027  I  -106.085    0.380    -9.876    0.060  0.095947  0.426181 -0.1779103  -106.040    -9.876  
+21 420 59324.00 I  0.097226 0.000014  0.427566 0.000025  I-0.1778521 0.0000039 -0.0085 0.0024  I  -105.785    0.285    -9.929    0.069  0.097266  0.427588 -0.1778571  -105.762    -9.917  
+21 421 59325.00 I  0.098224 0.000019  0.428912 0.000037  I-0.1779066 0.0000032  0.1195 0.0025  I  -105.261    0.557    -9.870    0.083  0.098245  0.428908 -0.1779160  -105.268    -9.880  
+21 422 59326.00 I  0.098990 0.000019  0.430097 0.000037  I-0.1781108 0.0000032  0.3066 0.0022  I  -105.021    0.557    -9.926    0.083  0.099005  0.430149 -0.1781298  -105.013    -9.959  
+21 423 59327.00 I  0.099559 0.000019  0.431133 0.000037  I-0.1785334 0.0000031  0.5346 0.0021  I  -105.023    0.614   -10.165    0.093  0.099573  0.431096 -0.1785406  -105.001   -10.212  
+21 424 59328.00 I  0.099853 0.000017  0.432027 0.000028  I-0.1791694 0.0000028  0.7308 0.0022  I  -104.955    0.614   -10.291    0.093  0.099809  0.432023 -0.1791390  -104.985   -10.413  
+21 425 59329.00 I  0.100026 0.000018  0.432773 0.000037  I-0.1799802 0.0000031  0.8825 0.0021  I  -104.770    0.614   -10.076    0.093  0.100034  0.432771 -0.1799364  -104.882   -10.281  
+21 426 59330.00 I  0.100442 0.000017  0.433379 0.000038  I-0.1809192 0.0000031  0.9887 0.0029  I  -104.878    0.614    -9.633    0.093  0.100355  0.433380 -0.1809123  -105.064    -9.917  
+21 427 59331.00 I  0.101372 0.000010  0.433863 0.000026  I-0.1819033 0.0000050  0.9319 0.0026  I  -105.482    0.322    -9.345    0.160  0.101324  0.433851 -0.1819026  -105.732    -9.702  
+21 428 59332.00 I  0.102665 0.000017  0.434402 0.000035  I-0.1827157 0.0000041  0.6731 0.0033  I  -106.178    0.885    -9.386    0.078  0.102654  0.434414 -0.1826964  -106.366    -9.670  
+21 429 59333.00 I  0.104017 0.000017  0.434854 0.000035  I-0.1832166 0.0000043  0.3156 0.0030  I  -106.422    0.885    -9.562    0.078  0.104008  0.434868 -0.1831982  -106.503    -9.731  
+21 430 59334.00 I  0.105401 0.000017  0.435231 0.000035  I-0.1833706 0.0000044  0.0293 0.0031  I  -106.116    0.885    -9.640    0.078  0.105404  0.435218 -0.1833833  -106.086    -9.707  
+21 5 1 59335.00 I  0.106808 0.000016  0.435780 0.000025  I-0.1833154 0.0000045 -0.1363 0.0038  I  -105.690    0.885    -9.740    0.078  0.106820  0.435779 -0.1833089  -105.624    -9.755  
+21 5 2 59336.00 I  0.108215 0.000028  0.436470 0.000039  I-0.1831090 0.0000063 -0.2688 0.0039  I  -105.419    0.693    -9.915    0.063  0.108188  0.436419 -0.1830909  -105.392    -9.936  
+21 5 3 59337.00 I  0.109805 0.000029  0.437431 0.000039  I-0.1828035 0.0000063 -0.3244 0.0054  I  -105.431    0.693   -10.107    0.063  0.109767  0.437441 -0.1827909  -105.435   -10.113  
+21 5 4 59338.00 I  0.111567 0.000028  0.438463 0.000032  I-0.1825155 0.0000087 -0.2143 0.0045  I  -105.603    0.511   -10.177    0.044  0.111592  0.438462 -0.1825243  -105.659   -10.174  
+21 5 5 59339.00 I  0.113351 0.000032  0.439375 0.000037  I-0.1823930 0.0000063 -0.0500 0.0053  I  -105.693    0.506   -10.108    0.074  0.113313  0.439364 -0.1823978  -105.759   -10.107  
+21 5 6 59340.00 I  0.115275 0.000032  0.440336 0.000037  I-0.1824015 0.0000061  0.0722 0.0045  I  -105.582    0.506    -9.986    0.074  0.115279  0.440309 -0.1824200  -105.659    -9.997  
+21 5 7 59341.00 I  0.117110 0.000032  0.441483 0.000037  I-0.1825528 0.0000063  0.2406 0.0037  I  -105.418    0.506    -9.835    0.074  0.117172  0.441478 -0.1825670  -105.509    -9.864  
+21 5 8 59342.00 I  0.118705 0.000022  0.442599 0.000021  I-0.1828400 0.0000041  0.2810 0.0041  I  -105.449    0.485    -9.602    0.106  0.118681  0.442646 -0.1827886  -105.519    -9.632  
+21 5 9 59343.00 I  0.120399 0.000028  0.443443 0.000027  I-0.1830715 0.0000053  0.1917 0.0034  I  -105.726    0.478    -9.312    0.104  0.120432  0.443435 -0.1830318  -105.761    -9.338  
+21 510 59344.00 I  0.121974 0.000026  0.444237 0.000027  I-0.1832338 0.0000053  0.1337 0.0050  I  -106.057    0.478    -9.133    0.104  0.122013  0.444253 -0.1832398  -106.060    -9.161  
+21 511 59345.00 I  0.123227 0.000022  0.444887 0.000021  I-0.1833566 0.0000084  0.1290 0.0031  I  -106.262    0.473    -9.228    0.103  0.123229  0.444950 -0.1833696  -106.211    -9.260  
+21 512 59346.00 I  0.124611 0.000030  0.445069 0.000036  I-0.1834439 0.0000034 -0.0193 0.0045  I  -106.177    0.567    -9.553    0.095  0.124570  0.445119 -0.1834050  -106.142    -9.592  
+21 513 59347.00 I  0.126411 0.000030  0.444943 0.000036  I-0.1833052 0.0000031 -0.2062 0.0023  I  -105.999    0.567    -9.895    0.095  0.126398  0.444900 -0.1833166  -105.971    -9.938  
+21 514 59348.00 I  0.128373 0.000030  0.445064 0.000036  I-0.1830862 0.0000031 -0.2292 0.0017  I  -105.893    0.567   -10.094    0.095  0.128393  0.445000 -0.1831001  -105.857   -10.138  
+21 515 59349.00 I  0.130315 0.000025  0.445429 0.000032  I-0.1828412 0.0000014 -0.2690 0.0018  I  -105.967    0.603   -10.185    0.089  0.130276  0.445421 -0.1828031  -105.951   -10.226  
+21 516 59350.00 I  0.132484 0.000025  0.445801 0.000031  I-0.1825517 0.0000020 -0.2982 0.0013  I  -106.176    0.603   -10.277    0.089  0.132466  0.445767 -0.1824802  -106.179   -10.311  
+21 517 59351.00 I  0.134865 0.000026  0.446309 0.000039  I-0.1822619 0.0000023 -0.2761 0.0018  I  -106.307    0.569   -10.370    0.088  0.134899  0.446354 -0.1822601  -106.327   -10.390  
+21 518 59352.00 I  0.137091 0.000015  0.446611 0.000026  I-0.1820350 0.0000029 -0.1476 0.0019  I  -106.224    0.520   -10.362    0.087  0.137096  0.446653 -0.1820734  -106.203   -10.375  
+21 519 59353.00 I  0.139425 0.000020  0.446453 0.000032  I-0.1819779 0.0000030  0.0144 0.0021  I  -105.845    0.634   -10.279    0.175  0.139382  0.446488 -0.1819842  -105.891   -10.264  
+21 520 59354.00 I  0.142026 0.000020  0.446225 0.000032  I-0.1820965 0.0000030  0.2747 0.0021  I  -105.577    0.634   -10.250    0.175  0.142062  0.446194 -0.1821300  -105.602   -10.265  
+21 521 59355.00 I  0.144479 0.000019  0.446090 0.000032  I-0.1825095 0.0000030  0.4818 0.0021  I  -105.539    0.718   -10.417    0.233  0.144518  0.446092 -0.1825058  -105.556   -10.433  
+21 522 59356.00 I  0.146582 0.000018  0.446136 0.000032  I-0.1830317 0.0000028  0.6038 0.0023  I  -105.826    0.718   -10.483    0.233  0.146638  0.446087 -0.1830591  -105.780   -10.527  
+21 523 59357.00 I  0.148354 0.000017  0.446246 0.000021  I-0.1837196 0.0000036  0.7335 0.0018  I  -106.169    0.718   -10.301    0.233  0.148357  0.446319 -0.1837359  -106.114   -10.345  
+21 524 59358.00 I  0.150035 0.000022  0.446011 0.000028  I-0.1844372 0.0000022  0.6787 0.0020  I  -106.735    0.421    -9.901    0.173  0.150055  0.446007 -0.1844377  -106.686    -9.942  
+21 525 59359.00 I  0.151661 0.000018  0.445541 0.000021  I-0.1850360 0.0000017  0.5007 0.0017  I  -107.568    0.330    -9.591    0.114  0.151671  0.445578 -0.1850358  -107.551    -9.625  
+21 526 59360.00 I  0.153129 0.000020  0.445145 0.000031  I-0.1854191 0.0000025  0.2641 0.0015  I  -108.292    0.350    -9.566    0.125  0.153177  0.445002 -0.1854186  -108.338    -9.587  
+21 527 59361.00 I  0.154588 0.000021  0.444720 0.000032  I-0.1855527 0.0000025 -0.0069 0.0018  I  -108.453    0.350    -9.691    0.125  0.154610  0.444641 -0.1855433  -108.444    -9.735  
+21 528 59362.00 I  0.156105 0.000021  0.444058 0.000033  I-0.1854098 0.0000025 -0.2642 0.0018  I  -108.034    0.350    -9.790    0.125  0.156083  0.444149 -0.1854061  -107.950    -9.866  
+21 529 59363.00 I  0.157801 0.000023  0.443389 0.000033  I-0.1850555 0.0000025 -0.4279 0.0024  I  -107.392    0.350    -9.920    0.125  0.157787  0.443296 -0.1850586  -107.322    -9.999  
+21 530 59364.00 I  0.159439 0.000024  0.443181 0.000038  I-0.1845965 0.0000040 -0.4642 0.0024  I  -106.884    0.585   -10.186    0.168  0.159496  0.443194 -0.1846181  -106.855   -10.257  
+21 531 59365.00 I  0.160786 0.000023  0.443021 0.000038  I-0.1841715 0.0000040 -0.3672 0.0031  I  -106.703    0.585   -10.462    0.168  0.160764  0.443056 -0.1841962  -106.711   -10.524  
+21 6 1 59366.00 I  0.162207 0.000022  0.442538 0.000030  I-0.1838779 0.0000047 -0.2229 0.0028  I  -106.860    0.540   -10.506    0.174  0.162221  0.442541 -0.1838763  -106.911   -10.562  
+21 6 2 59367.00 I  0.163439 0.000024  0.442187 0.000038  I-0.1837186 0.0000039 -0.0999 0.0033  I  -106.913    0.783   -10.298    0.152  0.163505  0.442197 -0.1837088  -107.189   -10.310  
+21 6 3 59368.00 I  0.164294 0.000025  0.441786 0.000037  I-0.1836725 0.0000045  0.0064 0.0031  I  -107.152    0.783    -9.973    0.152  0.164269  0.441835 -0.1836734  -107.307    -9.973  
+21 6 4 59369.00 I  0.165288 0.000024  0.441036 0.000037  I-0.1837134 0.0000047  0.0585 0.0036  I  -107.212    0.783    -9.733    0.152  0.165264  0.441101 -0.1837182  -107.243    -9.722  
+21 6 5 59370.00 I  0.166468 0.000017  0.439943 0.000027  I-0.1837491 0.0000055 -0.0108 0.0047  I  -107.329    0.783    -9.567    0.152  0.166494  0.439959 -0.1837435  -107.338    -9.564  
+21 6 6 59371.00 I  0.167460 0.000022  0.438783 0.000036  I-0.1836759 0.0000082 -0.1278 0.0049  I  -107.690    0.682    -9.409    0.147  0.167443  0.438760 -0.1837213  -107.712    -9.420  
+21 6 7 59372.00 I  0.168518 0.000022  0.437810 0.000036  I-0.1834833 0.0000082 -0.2754 0.0057  I  -108.186    0.682    -9.312    0.147  0.168452  0.437773 -0.1835146  -108.222    -9.335  
+21 6 8 59373.00 I  0.170000 0.000019  0.437044 0.000034  I-0.1831184 0.0000078 -0.4429 0.0057  I  -108.567    0.528    -9.408    0.133  0.169988  0.437038 -0.1831307  -108.616    -9.447  
+21 6 9 59374.00 I  0.171621 0.000018  0.436495 0.000034  I-0.1825979 0.0000079 -0.6090 0.0055  I  -108.705    0.528    -9.726    0.133  0.171662  0.436466 -0.1825961  -108.746    -9.756  
+21 610 59375.00 I  0.173023 0.000017  0.436097 0.000034  I-0.1819091 0.0000078 -0.7489 0.0054  I  -108.686    0.528   -10.082    0.133  0.173060  0.436107 -0.1819126  -108.720   -10.098  
+21 611 59376.00 I  0.174263 0.000017  0.435730 0.000035  I-0.1811045 0.0000075 -0.8756 0.0047  I  -108.648    0.528   -10.270    0.133  0.174245  0.435720 -0.1810931  -108.643   -10.282  
+21 612 59377.00 I  0.175427 0.000011  0.435397 0.000024  I-0.1801830 0.0000052 -0.9268 0.0048  I  -108.690    0.500   -10.255    0.125  0.175463  0.435402 -0.1802017  -108.645   -10.266  
+21 613 59378.00 I  0.176480 0.000013  0.435064 0.000031  I-0.1792700 0.0000059 -0.9205 0.0055  I  -108.837    0.576   -10.165    0.119  0.176463  0.435076 -0.1792824  -108.763   -10.171  
+21 614 59379.00 I  0.177520 0.000011  0.434808 0.000022  I-0.1783568 0.0000097 -0.8698 0.0053  I  -109.034    0.755   -10.115    0.109  0.177561  0.434800 -0.1783898  -108.931   -10.112  
+21 615 59380.00 I  0.178428 0.000013  0.434500 0.000023  I-0.1775755 0.0000088 -0.6839 0.0056  I  -109.150    0.755   -10.108    0.109  0.178436  0.434544 -0.1776041  -109.005   -10.092  
+21 616 59381.00 I  0.179178 0.000016  0.433937 0.000029  I-0.1769789 0.0000055 -0.5285 0.0052  I  -109.098    0.588   -10.093    0.194  0.179161  0.433958 -0.1769638  -109.007   -10.090  
+21 617 59382.00 I  0.180088 0.000016  0.433090 0.000028  I-0.1765265 0.0000055 -0.3491 0.0039  I  -108.952    0.588   -10.055    0.194  0.179975  0.433150 -0.1765219  -108.937   -10.073  
+21 618 59383.00 I  0.181591 0.000016  0.432033 0.000029  I-0.1762902 0.0000054 -0.1410 0.0036  I  -108.945    0.517   -10.053    0.237  0.181538  0.431985 -0.1762920  -108.971   -10.051  
+21 619 59384.00 I  0.183453 0.000014  0.431234 0.000023  I-0.1762203 0.0000047 -0.0054 0.0037  I  -109.137    0.517    -9.929    0.237  0.183459  0.431221 -0.1762499  -109.186    -9.941  
+21 620 59385.00 I  0.185268 0.000028  0.430718 0.000032  I-0.1762492 0.0000052  0.0396 0.0035  I  -109.632    0.551    -9.707    0.195  0.185268  0.430690 -0.1762848  -109.672    -9.715  
+21 621 59386.00 I  0.186989 0.000027  0.430323 0.000032  I-0.1762222 0.0000052 -0.1475 0.0066  I  -110.372    0.551    -9.448    0.195  0.187008  0.430371 -0.1762299  -110.397    -9.446  
+21 622 59387.00 I  0.188636 0.000026  0.429670 0.000026  I-0.1759403 0.0000122 -0.3765 0.0042  I  -111.155    0.595    -9.287    0.131  0.188612  0.429729 -0.1759694  -111.169    -9.304  
+21 623 59388.00 I  0.190263 0.000027  0.428662 0.000028  I-0.1754675 0.0000066 -0.6107 0.0069  I  -111.724    0.537    -9.382    0.207  0.190249  0.428692 -0.1754577  -111.740    -9.402  
+21 624 59389.00 I  0.192021 0.000027  0.427528 0.000027  I-0.1746773 0.0000066 -0.9697 0.0046  I  -111.835    0.537    -9.530    0.207  0.191984  0.427561 -0.1746551  -111.870    -9.570  
+21 625 59390.00 I  0.193858 0.000028  0.426256 0.000027  I-0.1735840 0.0000064 -1.1609 0.0045  I  -111.566    0.537    -9.610    0.207  0.193895  0.426260 -0.1736026  -111.627    -9.678  
+21 626 59391.00 I  0.195553 0.000014  0.424979 0.000016  I-0.1723977 0.0000061 -1.2257 0.0040  I  -111.155    0.482    -9.705    0.258  0.195529  0.424979 -0.1723902  -111.223    -9.764  
+21 627 59392.00 I  0.197259 0.000017  0.423970 0.000031  I-0.1711515 0.0000047 -1.2340 0.0038  I  -110.800    0.462    -9.941    0.204  0.197249  0.423941 -0.1711520  -110.867    -9.981  
+21 628 59393.00 I  0.199043 0.000017  0.423147 0.000032  I-0.1699781 0.0000046 -1.0971 0.0030  I  -110.650    0.462   -10.213    0.204  0.199016  0.423212 -0.1700013  -110.723   -10.241  
+21 629 59394.00 I  0.201030 0.000016  0.421975 0.000032  I-0.1689857 0.0000037 -0.8750 0.0028  I  -110.826    0.456   -10.267    0.157  0.201014  0.422014 -0.1689979  -110.903   -10.285  
+21 630 59395.00 I  0.203112 0.000019  0.420660 0.000037  I-0.1681915 0.0000032 -0.7627 0.0027  I  -111.273    0.479   -10.019    0.145  0.203151  0.420682 -0.1681557  -111.326   -10.039  
+21 7 1 59396.00 I  0.205014 0.000017  0.419363 0.000039  I-0.1674334 0.0000040 -0.7313 0.0027  I  -111.789    0.517    -9.646    0.129  0.205011  0.419357 -0.1674255  -111.755    -9.689  
+21 7 2 59397.00 I  0.206927 0.000017  0.418125 0.000038  I-0.1667271 0.0000043 -0.7055 0.0036  I  -112.018    0.517    -9.432    0.129  0.206921  0.418137 -0.1667352  -112.004    -9.464  
+21 7 3 59398.00 I  0.209057 0.000016  0.416937 0.000028  I-0.1659922 0.0000059 -0.7705 0.0040  I  -112.152    0.517    -9.376    0.129  0.209024  0.416956 -0.1660067  -112.140    -9.398  
+21 7 4 59399.00 I  0.211307 0.000016  0.415846 0.000027  I-0.1651689 0.0000068 -0.8873 0.0040  I  -112.382    0.517    -9.360    0.129  0.211331  0.415811 -0.1651797  -112.363    -9.373  
+21 7 5 59400.00 I  0.213431 0.000019  0.414953 0.000033  I-0.1641902 0.0000055 -1.0863 0.0051  I  -112.723    0.633    -9.330    0.126  0.213414  0.414996 -0.1642095  -112.694    -9.336  
+21 7 6 59401.00 I  0.215664 0.000017  0.414033 0.000027  I-0.1630268 0.0000077 -1.1940 0.0039  I  -113.021    0.761    -9.374    0.123  0.215650  0.414027 -0.1630892  -112.980    -9.377  
+21 7 7 59402.00 I  0.218080 0.000019  0.413112 0.000029  I-0.1618138 0.0000054 -1.2671 0.0047  I  -113.170    0.734    -9.580    0.106  0.218140  0.413172 -0.1618291  -113.113    -9.583  
+21 7 8 59403.00 I  0.220159 0.000018  0.412100 0.000029  I-0.1604715 0.0000053 -1.4037 0.0037  I  -113.205    0.734    -9.877    0.106  0.220214  0.412138 -0.1604574  -113.230    -9.877  
+21 7 9 59404.00 I  0.221841 0.000017  0.410730 0.000029  I-0.1590303 0.0000052 -1.4686 0.0035  I  -113.198    0.734   -10.080    0.106  0.221832  0.410821 -0.1590228  -113.321   -10.078  
+21 710 59405.00 I  0.223645 0.000017  0.409105 0.000029  I-0.1575737 0.0000046 -1.4155 0.0031  I  -113.183    0.734   -10.068    0.106  0.223600  0.409097 -0.1575892  -113.323   -10.077  
+21 711 59406.00 I  0.225637 0.000014  0.407654 0.000027  I-0.1562196 0.0000032 -1.3017 0.0029  I  -113.196    0.677    -9.898    0.069  0.225666  0.407615 -0.1562169  -113.312    -9.920  
+21 712 59407.00 I  0.227531 0.000013  0.406534 0.000028  I-0.1549782 0.0000034 -1.1641 0.0024  I  -113.293    0.677    -9.734    0.069  0.227521  0.406499 -0.1549674  -113.374    -9.766  
+21 713 59408.00 I  0.229295 0.000010  0.405739 0.000022  I-0.1539054 0.0000036 -0.9844 0.0024  I  -113.458    0.678    -9.695    0.071  0.229363  0.405735 -0.1538980  -113.495    -9.729  
+21 714 59409.00 I  0.230855 0.000011  0.405107 0.000030  I-0.1530285 0.0000033 -0.7474 0.0029  I  -113.569    0.657    -9.760    0.083  0.230852  0.405177 -0.1530567  -113.617    -9.794  
+21 715 59410.00 I  0.232360 0.000010  0.404157 0.000030  I-0.1524095 0.0000045 -0.5139 0.0030  I  -113.540    0.657    -9.819    0.083  0.232364  0.404183 -0.1524225  -113.614    -9.847  
+21 716 59411.00 I  0.233956 0.000012  0.403081 0.000030  I-0.1519891 0.0000049 -0.3154 0.0046  I  -113.512    0.546    -9.778    0.102  0.233932  0.403085 -0.1520045  -113.595    -9.787  
+21 717 59412.00 I  0.235535 0.000010  0.402266 0.000025  I-0.1517526 0.0000081 -0.1953 0.0034  I  -113.674    0.546    -9.604    0.102  0.235568  0.402256 -0.1517411  -113.759    -9.608  
+21 718 59413.00 I  0.236943 0.000014  0.401495 0.000032  I-0.1515310 0.0000047 -0.2776 0.0047  I  -114.202    0.578    -9.387    0.143  0.236938  0.401571 -0.1515176  -114.276    -9.388  
+21 719 59414.00 I  0.238375 0.000015  0.400303 0.000032  I-0.1511792 0.0000048 -0.4143 0.0036  I  -114.945    0.578    -9.260    0.143  0.238366  0.400312 -0.1511975  -115.015    -9.262  
+21 720 59415.00 I  0.239932 0.000016  0.398907 0.000025  I-0.1507064 0.0000054 -0.5389 0.0032  I  -115.568    0.589    -9.306    0.161  0.239941  0.398929 -0.1507114  -115.643    -9.312  
+21 721 59416.00 I  0.241375 0.000017  0.397611 0.000031  I-0.1500907 0.0000041 -0.6957 0.0033  I  -115.815    0.637    -9.469    0.166  0.241402  0.397614 -0.1500616  -115.876    -9.476  
+21 722 59417.00 I  0.242534 0.000018  0.396308 0.000031  I-0.1493131 0.0000039 -0.8583 0.0030  I  -115.708    0.637    -9.593    0.166  0.242550  0.396349 -0.1492653  -115.745    -9.604  
+21 723 59418.00 I  0.243563 0.000018  0.394831 0.000031  I-0.1483996 0.0000044 -0.9446 0.0041  I  -115.357    0.746    -9.613    0.173  0.243559  0.394850 -0.1483896  -115.468    -9.626  
+21 724 59419.00 I  0.244415 0.000015  0.393383 0.000022  I-0.1474810 0.0000072 -0.8597 0.0033  I  -115.261    0.746    -9.596    0.173  0.244504  0.393363 -0.1475216  -115.321    -9.619  
+21 725 59420.00 I  0.244598 0.000021  0.392090 0.000037  I-0.1467112 0.0000049 -0.6819 0.0043  I  -115.215    0.536    -9.688    0.131  0.244659  0.392108 -0.1467385  -115.265    -9.715  
+21 726 59421.00 I  0.244304 0.000020  0.390790 0.000037  I-0.1460905 0.0000047 -0.5844 0.0036  I  -115.222    0.536    -9.845    0.131  0.244282  0.390818 -0.1460743  -115.280    -9.873  
+21 727 59422.00 I  0.244043 0.000019  0.389170 0.000031  I-0.1455425 0.0000053 -0.4866 0.0031  I  -115.369    0.367    -9.888    0.090  0.244021  0.389282 -0.1455380  -115.457    -9.910  
+21 728 59423.00 I  0.244010 0.000018  0.386991 0.000039  I-0.1451243 0.0000040 -0.3676 0.0032  I  -115.722    0.385    -9.730    0.090  0.243957  0.387023 -0.1451164  -115.784    -9.750  
+21 729 59424.00 I  0.244336 0.000019  0.384574 0.000039  I-0.1447658 0.0000035 -0.3729 0.0027  I  -116.266    0.414    -9.501    0.089  0.244271  0.384533 -0.1447485  -116.221    -9.509  
+21 730 59425.00 I  0.245094 0.000021  0.382522 0.000039  I-0.1443687 0.0000035 -0.4074 0.0029  I  -116.564    0.414    -9.372    0.089  0.245054  0.382456 -0.1443684  -116.596    -9.367  
+21 731 59426.00 I  0.246005 0.000016  0.381141 0.000025  I-0.1439305 0.0000047 -0.5034 0.0029  I  -116.705    0.414    -9.378    0.089  0.246021  0.381094 -0.1439172  -116.756    -9.383  
+21 8 1 59427.00 I  0.246809 0.000021  0.380133 0.000036  I-0.1433465 0.0000047 -0.6456 0.0033  I  -116.769    0.673    -9.408    0.131  0.246780  0.380162 -0.1433541  -116.809    -9.429  
+21 8 2 59428.00 I  0.247742 0.000022  0.378994 0.000035  I-0.1426499 0.0000047 -0.7559 0.0033  I  -116.858    0.673    -9.379    0.131  0.247724  0.379020 -0.1426563  -116.864    -9.419  
+21 8 3 59429.00 I  0.248638 0.000023  0.377636 0.000035  I-0.1418310 0.0000046 -0.8772 0.0035  I  -116.993    0.702    -9.353    0.118  0.248665  0.377672 -0.1418281  -116.928    -9.418  
+21 8 4 59430.00 I  0.249330 0.000022  0.376207 0.000035  I-0.1408997 0.0000053 -0.9859 0.0035  I  -117.140    0.702    -9.454    0.118  0.249247  0.376225 -0.1408819  -117.087    -9.488  
+21 8 5 59431.00 I  0.250339 0.000021  0.374735 0.000035  I-0.1398654 0.0000053 -1.0760 0.0038  I  -117.244    0.702    -9.701    0.118  0.250318  0.374716 -0.1398588  -117.212    -9.692  
+21 8 6 59432.00 I  0.251512 0.000020  0.373437 0.000035  I-0.1387840 0.0000055 -1.0573 0.0040  I  -117.343    0.322    -9.921    0.160  0.251557  0.373439 -0.1388293  -117.228    -9.944  
+21 8 7 59433.00 I  0.252320 0.000015  0.372184 0.000025  I-0.1377575 0.0000060 -1.0187 0.0040  I  -117.054    0.322    -9.990    0.160  0.252384  0.372189 -0.1377997  -117.131   -10.037  
+21 8 8 59434.00 I  0.252522 0.000014  0.370924 0.000026  I-0.1367460 0.0000059 -0.9821 0.0043  I  -116.803    0.322    -9.864    0.160  0.252618  0.370959 -0.1367543  -116.976    -9.913  
+21 8 9 59435.00 I  0.251920 0.000013  0.369466 0.000021  I-0.1358292 0.0000061 -0.8380 0.0040  I  -116.669    0.559    -9.662    0.049  0.251958  0.369547 -0.1358220  -116.861    -9.698  
+21 810 59436.00 I  0.250917 0.000013  0.367464 0.000021  I-0.1350822 0.0000054 -0.6573 0.0039  I  -116.699    0.559    -9.559    0.049  0.250843  0.367504 -0.1350686  -116.860    -9.570  
+21 811 59437.00 I  0.250234 0.000017  0.365281 0.000031  I-0.1345132 0.0000048 -0.4806 0.0036  I  -116.835    0.493    -9.626    0.126  0.250176  0.365255 -0.1345085  -116.935    -9.605  
+21 812 59438.00 I  0.249913 0.000016  0.363355 0.000031  I-0.1341184 0.0000049 -0.3115 0.0034  I  -116.985    0.493    -9.777    0.126  0.249897  0.363348 -0.1341190  -117.018    -9.784  
+21 813 59439.00 I  0.249586 0.000015  0.361520 0.000031  I-0.1338431 0.0000049 -0.2835 0.0035  I  -117.141    0.493    -9.859    0.126  0.249586  0.361519 -0.1338317  -117.129    -9.917  
+21 814 59440.00 I  0.249171 0.000014  0.359753 0.000031  I-0.1335206 0.0000050 -0.3479 0.0040  I  -117.391    0.493    -9.789    0.126  0.249168  0.359749 -0.1335458  -117.340    -9.843  
+21 815 59441.00 I  0.248745 0.000013  0.358118 0.000025  I-0.1331316 0.0000062 -0.4594 0.0032  I  -117.789    0.358    -9.622    0.178  0.248726  0.358103 -0.1331531  -117.733    -9.659  
+21 816 59442.00 I  0.248383 0.000013  0.356527 0.000031  I-0.1325653 0.0000040 -0.6803 0.0034  I  -118.229    0.487    -9.489    0.154  0.248321  0.356538 -0.1325675  -118.199    -9.514  
+21 817 59443.00 I  0.248158 0.000008  0.354900 0.000022  I-0.1317597 0.0000030 -0.9351 0.0030  I  -118.499    0.527    -9.471    0.136  0.248130  0.354895 -0.1317488  -118.520    -9.488  
+21 818 59444.00 I  0.248037 0.000012  0.353255 0.000027  I-0.1307233 0.0000045 -1.1054 0.0027  I  -118.462    0.554    -9.533    0.137  0.248008  0.353279 -0.1307185  -118.546    -9.545  
+21 819 59445.00 I  0.247965 0.000011  0.351673 0.000027  I-0.1295768 0.0000046 -1.1919 0.0033  I  -118.183    0.554    -9.578    0.137  0.247978  0.351653 -0.1295488  -118.297    -9.587  
+21 820 59446.00 I  0.247724 0.000012  0.350058 0.000027  I-0.1283665 0.0000047 -1.1973 0.0033  I  -117.888    0.628    -9.550    0.138  0.247731  0.350108 -0.1283563  -117.988    -9.566  
+21 821 59447.00 I  0.247300 0.000012  0.348292 0.000028  I-0.1272417 0.0000048 -1.0243 0.0035  I  -117.607    0.628    -9.514    0.138  0.247290  0.348276 -0.1272649  -117.743    -9.514  
+21 822 59448.00 I  0.246848 0.000013  0.346515 0.000023  I-0.1263287 0.0000051 -0.8190 0.0035  I  -117.437    0.956    -9.510    0.137  0.246822  0.346558 -0.1263384  -117.577    -9.494  
+21 823 59449.00 I  0.246375 0.000014  0.344527 0.000023  I-0.1255817 0.0000052 -0.6798 0.0032  I  -117.338    0.956    -9.514    0.137  0.246343  0.344554 -0.1255763  -117.443    -9.485  
+21 824 59450.00 I  0.246057 0.000011  0.342239 0.000017  I-0.1249651 0.0000040 -0.5526 0.0036  I  -117.334    1.067    -9.451    0.136  0.245986  0.342232 -0.1249636  -117.347    -9.416  
+21 825 59451.00 I  0.246022 0.000028  0.340127 0.000029  I-0.1244694 0.0000051 -0.4466 0.0032  I  -117.522    1.021    -9.303    0.139  0.246006  0.340077 -0.1244735  -117.579    -9.295  
+21 826 59452.00 I  0.246037 0.000028  0.338297 0.000030  I-0.1240270 0.0000050 -0.4752 0.0035  I  -117.913    1.021    -9.158    0.139  0.246029  0.338309 -0.1240162  -118.019    -9.189  
+21 827 59453.00 I  0.246058 0.000028  0.336460 0.000030  I-0.1235033 0.0000049 -0.5507 0.0048  I  -118.605    0.533    -9.099    0.157  0.246039  0.336463 -0.1235117  -118.513    -9.184  
+21 828 59454.00 I  0.246070 0.000028  0.334743 0.000029  I-0.1229011 0.0000082 -0.6995 0.0035  I  -118.811    0.533    -9.128    0.157  0.246083  0.334712 -0.1228899  -118.761    -9.205  
+21 829 59455.00 I  0.246025 0.000030  0.333204 0.000041  I-0.1221164 0.0000049 -0.8119 0.0047  I  -118.832    0.610    -9.146    0.113  0.246022  0.333214 -0.1221387  -118.783    -9.190  
+21 830 59456.00 I  0.245766 0.000030  0.331655 0.000041  I-0.1212885 0.0000047 -0.8905 0.0029  I  -118.748    0.610    -9.101    0.113  0.245834  0.331664 -0.1212791  -118.708    -9.104  
+21 831 59457.00 I  0.245078 0.000018  0.329809 0.000034  I-0.1203297 0.0000031 -0.9860 0.0030  I  -118.699    0.627    -9.004    0.101  0.245060  0.329881 -0.1203267  -118.658    -9.011  
+21 9 1 59458.00 I  0.244342 0.000025  0.327819 0.000040  I-0.1193421 0.0000037 -1.0046 0.0024  I  -118.639    0.676    -9.125    0.106  0.244291  0.327776 -0.1193071  -118.650    -9.123  
+21 9 2 59459.00 I  0.243923 0.000025  0.325945 0.000040  I-0.1182978 0.0000036 -1.0914 0.0025  I  -118.539    0.676    -9.374    0.106  0.243859  0.325972 -0.1182574  -118.581    -9.390  
+21 9 3 59460.00 I  0.243864 0.000024  0.324202 0.000039  I-0.1172249 0.0000034 -0.9815 0.0031  I  -118.345    0.676    -9.635    0.106  0.243838  0.324135 -0.1172280  -118.364    -9.679  
+21 9 4 59461.00 I  0.243828 0.000020  0.322767 0.000026  I-0.1163486 0.0000051 -0.8304 0.0033  I  -118.130    0.696    -9.752    0.110  0.243924  0.322819 -0.1162657  -118.147    -9.782  
+21 9 5 59462.00 I  0.243251 0.000021  0.321176 0.000025  I-0.1155460 0.0000057 -0.7338 0.0033  I  -118.006    0.696    -9.656    0.110  0.243284  0.321221 -0.1154565  -117.995    -9.664  
+21 9 6 59463.00 I  0.242256 0.000021  0.319261 0.000040  I-0.1149296 0.0000041 -0.4914 0.0035  I  -118.010    0.523    -9.420    0.106  0.242288  0.319291 -0.1149183  -117.966    -9.415  
+21 9 7 59464.00 I  0.241133 0.000012  0.317269 0.000034  I-0.1145640 0.0000039 -0.2467 0.0030  I  -118.422    0.137    -9.192    0.101  0.241085  0.317267 -0.1145864  -118.054    -9.194  
+21 9 8 59465.00 I  0.240207 0.000014  0.315378 0.000039  I-0.1144284 0.0000045 -0.0253 0.0029  I  -118.246    0.411    -9.142    0.099  0.240168  0.315380 -0.1144389  -118.217    -9.134  
+21 9 9 59466.00 I  0.239548 0.000016  0.313676 0.000040  I-0.1144641 0.0000044  0.0481 0.0032  I  -118.133    0.411    -9.271    0.099  0.239509  0.313682 -0.1144456  -118.199    -9.278  
+21 910 59467.00 I  0.239102 0.000017  0.311961 0.000040  I-0.1144997 0.0000045  0.0469 0.0034  I  -118.027    0.604    -9.451    0.097  0.239055  0.311944 -0.1145001  -118.196    -9.493  
+21 911 59468.00 I  0.238933 0.000017  0.310410 0.000041  I-0.1145235 0.0000052 -0.0576 0.0038  I  -118.301    0.604    -9.573    0.097  0.238903  0.310398 -0.1145067  -118.376    -9.600  
+21 912 59469.00 I  0.239046 0.000015  0.309197 0.000033  I-0.1143427 0.0000061 -0.2874 0.0040  I  -118.546    0.626    -9.528    0.118  0.239057  0.309176 -0.1143417  -118.582    -9.536  
+21 913 59470.00 I  0.238925 0.000016  0.308177 0.000032  I-0.1139356 0.0000062 -0.5566 0.0045  I  -118.689    0.626    -9.376    0.118  0.239061  0.308241 -0.1139194  -118.703    -9.367  
+21 914 59471.00 I  0.238108 0.000022  0.306824 0.000026  I-0.1132503 0.0000066 -0.7634 0.0045  I  -118.690    0.641    -9.233    0.133  0.238135  0.306840 -0.1132542  -118.709    -9.209  
+21 915 59472.00 I  0.236807 0.000025  0.305459 0.000034  I-0.1124497 0.0000064 -0.8476 0.0050  I  -118.537    0.691    -9.159    0.186  0.236855  0.305424 -0.1124265  -118.563    -9.153  
+21 916 59473.00 I  0.235248 0.000024  0.304155 0.000034  I-0.1115819 0.0000076 -0.8513 0.0053  I  -118.262    0.691    -9.140    0.186  0.235175  0.304217 -0.1115600  -118.302    -9.166  
+21 917 59474.00 I  0.234102 0.000024  0.302442 0.000033  I-0.1107914 0.0000084 -0.7222 0.0072  I  -117.948    0.691    -9.140    0.186  0.234052  0.302470 -0.1107776  -117.983    -9.205  
+21 918 59475.00 I  0.233193 0.000024  0.300660 0.000026  I-0.1101777 0.0000123 -0.4725 0.0056  I  -117.704    0.802    -9.133    0.241  0.233267  0.300669 -0.1101847  -117.773    -9.189  
+21 919 59476.00 I  0.231949 0.000026  0.298943 0.000033  I-0.1098169 0.0000075 -0.3113 0.0072  I  -117.601    0.638    -9.086    0.159  0.231901  0.298971 -0.1097908  -117.690    -9.120  
+21 920 59477.00 I  0.230910 0.000021  0.297073 0.000032  I-0.1095342 0.0000074 -0.2129 0.0054  I  -117.617    0.638    -8.955    0.159  0.230860  0.297082 -0.1095369  -117.703    -8.970  
+21 921 59478.00 I  0.230447 0.000016  0.295177 0.000022  I-0.1093892 0.0000078 -0.1203 0.0052  I  -117.672    0.603    -8.737    0.052  0.230386  0.295169 -0.1093835  -117.748    -8.731  
+21 922 59479.00 I  0.230224 0.000020  0.293453 0.000048  I-0.1092721 0.0000073 -0.0922 0.0048  I  -117.733    0.601    -8.511    0.062  0.230280  0.293410 -0.1092939  -117.791    -8.533  
+21 923 59480.00 I  0.229734 0.000021  0.291962 0.000048  I-0.1091983 0.0000055 -0.0836 0.0047  I  -117.841    0.601    -8.401    0.062  0.229745  0.291932 -0.1092075  -117.893    -8.459  
+21 924 59481.00 I  0.229047 0.000021  0.290724 0.000048  I-0.1090766 0.0000058 -0.1597 0.0065  I  -118.068    0.486    -8.478    0.113  0.229059  0.290744 -0.1090710  -118.064    -8.550  
+21 925 59482.00 I  0.228150 0.000018  0.289697 0.000045  I-0.1088675 0.0000117 -0.2698 0.0059  I  -118.135    0.486    -8.618    0.113  0.228196  0.289721 -0.1088548  -118.132    -8.702  
+21 926 59483.00 I  0.226731 0.000019  0.288535 0.000056  I-0.1085268 0.0000103 -0.4105 0.0080  I  -118.049    0.658    -8.713    0.081  0.226765  0.288616 -0.1085235  -118.029    -8.801  
+21 927 59484.00 I  0.224987 0.000018  0.286877 0.000057  I-0.1080394 0.0000110 -0.5724 0.0081  I  -117.850    0.658    -8.724    0.081  0.224983  0.286909 -0.1080259  -117.816    -8.811  
+21 928 59485.00 I  0.223250 0.000013  0.285070 0.000037  I-0.1074037 0.0000124 -0.6691 0.0067  I  -117.684    0.672    -8.731    0.073  0.223233  0.285091 -0.1073996  -117.636    -8.811  
+21 929 59486.00 I  0.221733 0.000021  0.283226 0.000042  I-0.1067197 0.0000077 -0.7102 0.0073  I  -117.576    0.701    -8.818    0.105  0.221642  0.283266 -0.1067014  -117.530    -8.894  
+21 930 59487.00 I  0.220681 0.000024  0.281350 0.000042  I-0.1059785 0.0000077 -0.7658 0.0053  I  -117.354    0.701    -8.959    0.105  0.220649  0.281274 -0.1059687  -117.318    -9.028  
+2110 1 59488.00 I  0.219922 0.000025  0.279819 0.000042  I-0.1052424 0.0000073 -0.6584 0.0051  I  -116.913    0.719    -9.053    0.123  0.219900  0.279843 -0.1052566  -116.884    -9.102  
+2110 2 59489.00 I  0.219190 0.000024  0.278466 0.000025  I-0.1046917 0.0000066 -0.4610 0.0047  I  -116.349    0.719    -9.010    0.123  0.219232  0.278385 -0.1046635  -116.396    -9.043  
+2110 3 59490.00 I  0.218064 0.000026  0.277407 0.000028  I-0.1043054 0.0000060 -0.3087 0.0043  I  -116.021    0.829    -8.851    0.162  0.218114  0.277440 -0.1042262  -116.108    -8.872  
+2110 4 59491.00 I  0.216515 0.000026  0.276371 0.000028  I-0.1040955 0.0000054 -0.0928 0.0057  I  -116.030    0.829    -8.634    0.162  0.216463  0.276398 -0.1040412  -116.115    -8.648  
+2110 5 59492.00 I  0.214841 0.000018  0.275292 0.000019  I-0.1041487 0.0000097  0.2099 0.0041  I  -116.226    0.858    -8.417    0.187  0.214966  0.275265 -0.1041427  -116.245    -8.435  
+2110 6 59493.00 I  0.212842 0.000020  0.274053 0.000032  I-0.1045040 0.0000062  0.4788 0.0057  I  -116.465    0.798    -8.287    0.179  0.212886  0.274073 -0.1045130  -116.543    -8.305  
+2110 7 59494.00 I  0.210715 0.000020  0.272257 0.000031  I-0.1050416 0.0000061  0.5538 0.0044  I  -116.703    0.798    -8.338    0.179  0.210670  0.272310 -0.1050355  -116.846    -8.364  
+2110 8 59495.00 I  0.208772 0.000020  0.270357 0.000031  I-0.1055579 0.0000062  0.4679 0.0039  I  -117.077    0.199    -8.550    0.167  0.208740  0.270354 -0.1055552  -117.140    -8.593  
+2110 9 59496.00 I  0.207046 0.000017  0.268632 0.000028  I-0.1059383 0.0000047  0.2649 0.0040  I  -117.006    0.199    -8.726    0.167  0.206987  0.268630 -0.1059176  -117.149    -8.775  
+211010 59497.00 I  0.205607 0.000017  0.267108 0.000029  I-0.1060701 0.0000050  0.0091 0.0028  I  -116.877    0.199    -8.689    0.167  0.205587  0.267049 -0.1060489  -117.008    -8.734  
+211011 59498.00 I  0.204303 0.000021  0.265972 0.000033  I-0.1059780 0.0000029 -0.1822 0.0030  I  -116.735    0.498    -8.463    0.121  0.204294  0.265940 -0.1059506  -116.845    -8.499  
+211012 59499.00 I  0.202918 0.000020  0.265374 0.000021  I-0.1057250 0.0000033 -0.3156 0.0023  I  -116.620    0.672    -8.241    0.021  0.202929  0.265318 -0.1056985  -116.696    -8.264  
+211013 59500.00 I  0.201334 0.000024  0.265023 0.000024  I-0.1053813 0.0000035 -0.3456 0.0024  I  -116.510    0.669    -8.164    0.063  0.201347  0.265115 -0.1053769  -116.533    -8.163  
+211014 59501.00 I  0.199471 0.000023  0.264508 0.000026  I-0.1050614 0.0000035 -0.2930 0.0024  I  -116.349    0.669    -8.205    0.063  0.199531  0.264474 -0.1050561  -116.392    -8.233  
+211015 59502.00 I  0.197120 0.000024  0.264001 0.000026  I-0.1048167 0.0000034 -0.1764 0.0025  I  -116.078    0.664    -8.289    0.089  0.197144  0.264052 -0.1048215  -116.168    -8.339  
+211016 59503.00 I  0.194628 0.000025  0.263335 0.000026  I-0.1047288 0.0000036  0.0008 0.0028  I  -115.831    0.664    -8.322    0.089  0.194540  0.263311 -0.1047296  -115.892    -8.371  
+211017 59504.00 I  0.192496 0.000023  0.262708 0.000042  I-0.1048035 0.0000045  0.1338 0.0029  I  -115.633    0.573    -8.293    0.073  0.192522  0.262732 -0.1047961  -115.671    -8.326  
+211018 59505.00 I  0.190391 0.000020  0.262041 0.000041  I-0.1049980 0.0000045  0.2718 0.0033  I  -115.558    0.573    -8.157    0.073  0.190330  0.262116 -0.1049797  -115.586    -8.172  
+211019 59506.00 I  0.188478 0.000016  0.261095 0.000040  I-0.1053281 0.0000047  0.3529 0.0034  I  -115.562    0.549    -7.903    0.060  0.188419  0.261094 -0.1053261  -115.599    -7.898  
+211020 59507.00 I  0.187014 0.000020  0.260352 0.000043  I-0.1056655 0.0000052  0.3190 0.0036  I  -115.538    0.576    -7.630    0.105  0.186951  0.260372 -0.1056852  -115.532    -7.637  
+211021 59508.00 I  0.185923 0.000018  0.259646 0.000043  I-0.1059571 0.0000054  0.2582 0.0038  I  -115.389    0.727    -7.595    0.167  0.185890  0.259671 -0.1059933  -115.408    -7.531  
+211022 59509.00 I  0.185080 0.000021  0.258894 0.000044  I-0.1061588 0.0000055  0.1280 0.0045  I  -115.324    0.727    -7.650    0.167  0.185109  0.258931 -0.1061695  -115.283    -7.652  
+211023 59510.00 I  0.183900 0.000019  0.258063 0.000024  I-0.1061799 0.0000071 -0.1017 0.0044  I  -115.250    0.727    -7.831    0.167  0.183997  0.258126 -0.1061599  -115.214    -7.852  
+211024 59511.00 I  0.182242 0.000023  0.256852 0.000033  I-0.1059622 0.0000068 -0.3110 0.0049  I  -115.116    0.740    -7.965    0.119  0.182170  0.256859 -0.1059532  -115.105    -7.981  
+211025 59512.00 I  0.180791 0.000022  0.255749 0.000033  I-0.1055795 0.0000068 -0.4557 0.0052  I  -114.938    0.740    -7.991    0.119  0.180765  0.255674 -0.1055673  -114.951    -7.995  
+211026 59513.00 I  0.179385 0.000022  0.255109 0.000026  I-0.1050768 0.0000080 -0.5226 0.0042  I  -114.813    0.753    -7.994    0.025  0.179443  0.255135 -0.1050710  -114.842    -7.976  
+211027 59514.00 I  0.177417 0.000024  0.254633 0.000036  I-0.1045726 0.0000049 -0.4747 0.0045  I  -114.744    0.629    -8.053    0.107  0.177475  0.254614 -0.1045560  -114.798    -8.064  
+211028 59515.00 I  0.175038 0.000021  0.254166 0.000035  I-0.1041327 0.0000042 -0.4109 0.0033  I  -114.550    0.629    -8.106    0.107  0.174986  0.254210 -0.1040921  -114.636    -8.154  
+211029 59516.00 I  0.172943 0.000020  0.253715 0.000035  I-0.1037682 0.0000045 -0.2949 0.0030  I  -114.130    0.569    -8.065    0.133  0.172883  0.253703 -0.1037503  -114.222    -8.112  
+211030 59517.00 I  0.171130 0.000016  0.253429 0.000028  I-0.1035808 0.0000044 -0.0653 0.0032  I  -113.565    0.569    -7.826    0.133  0.171153  0.253485 -0.1035881  -113.712    -7.886  
+211031 59518.00 I  0.169169 0.000018  0.253021 0.000028  I-0.1036639 0.0000045  0.2430 0.0033  I  -113.316    0.569    -7.580    0.133  0.169153  0.253030 -0.1036762  -113.489    -7.636  
+2111 1 59519.00 I  0.167192 0.000021  0.252558 0.000040  I-0.1040585 0.0000049  0.5263 0.0049  I  -113.470    0.637    -7.412    0.100  0.167161  0.252590 -0.1040619  -113.648    -7.463  
+2111 2 59520.00 I  0.165519 0.000019  0.251986 0.000031  I-0.1046989 0.0000087  0.7568 0.0033  I  -113.619    0.692    -7.244    0.053  0.165421  0.252037 -0.1047142  -113.919    -7.301  
+2111 3 59521.00 I  0.164374 0.000020  0.251134 0.000038  I-0.1055290 0.0000045  0.8579 0.0048  I  -113.957    0.495    -7.058    0.045  0.164345  0.251154 -0.1055305  -114.076    -7.098  
+2111 4 59522.00 I  0.163278 0.000021  0.250404 0.000038  I-0.1063546 0.0000041  0.7786 0.0030  I  -114.200    0.495    -6.951    0.045  0.163380  0.250407 -0.1063597  -114.274    -6.977  
+2111 5 59523.00 I  0.161445 0.000021  0.249774 0.000037  I-0.1070385 0.0000040  0.5563 0.0028  I  -114.304    0.495    -7.056    0.045  0.161527  0.249780 -0.1070350  -114.417    -7.068  
+2111 6 59524.00 I  0.158962 0.000021  0.249269 0.000037  I-0.1074313 0.0000037  0.2263 0.0024  I  -114.138    0.495    -7.251    0.045  0.158959  0.249274 -0.1074216  -114.174    -7.273  
+2111 7 59525.00 I  0.156485 0.000018  0.248731 0.000037  I-0.1075120 0.0000027 -0.0411 0.0023  I  -113.762    0.466    -7.271    0.067  0.156428  0.248766 -0.1075061  -113.720    -7.312  
+2111 8 59526.00 I  0.154402 0.000017  0.248080 0.000037  I-0.1073922 0.0000026 -0.1793 0.0024  I  -113.449    0.466    -7.081    0.067  0.154365  0.248057 -0.1073849  -113.374    -7.138  
+2111 9 59527.00 I  0.152526 0.000016  0.247529 0.000029  I-0.1071865 0.0000040 -0.2184 0.0029  I  -113.100    0.892    -6.946    0.104  0.152501  0.247567 -0.1071716  -113.247    -7.009  
+211110 59528.00 I  0.150844 0.000023  0.247116 0.000035  I-0.1069843 0.0000052 -0.1710 0.0034  I  -113.254    0.777    -7.016    0.083  0.150781  0.247125 -0.1069620  -113.363    -7.072  
+211111 59529.00 I  0.149530 0.000023  0.246777 0.000035  I-0.1068851 0.0000054 -0.0019 0.0038  I  -113.306    0.777    -7.190    0.083  0.149470  0.246785 -0.1068772  -113.428    -7.227  
+211112 59530.00 I  0.148524 0.000024  0.246575 0.000035  I-0.1069909 0.0000055  0.1985 0.0048  I  -113.227    0.777    -7.246    0.083  0.148470  0.246564 -0.1069721  -113.370    -7.262  
+211113 59531.00 I  0.147730 0.000021  0.246473 0.000021  I-0.1072628 0.0000079  0.3409 0.0036  I  -113.083    0.585    -7.145    0.046  0.147692  0.246455 -0.1072523  -113.185    -7.165  
+211114 59532.00 I  0.146991 0.000027  0.246425 0.000024  I-0.1076479 0.0000045  0.4089 0.0045  I  -112.947    0.624    -6.988    0.109  0.147041  0.246459 -0.1076527  -112.994    -7.024  
+211115 59533.00 I  0.145708 0.000027  0.246299 0.000026  I-0.1080248 0.0000043  0.3094 0.0029  I  -112.888    0.624    -6.824    0.109  0.145836  0.246338 -0.1080024  -112.892    -6.878  
+211116 59534.00 I  0.143583 0.000023  0.245970 0.000019  I-0.1082685 0.0000037  0.2154 0.0025  I  -112.910    0.639    -6.648    0.131  0.143555  0.246023 -0.1082774  -112.883    -6.691  
+211117 59535.00 I  0.141477 0.000025  0.245395 0.000028  I-0.1084696 0.0000026  0.1635 0.0023  I  -112.947    0.627    -6.365    0.093  0.141392  0.245346 -0.1084806  -112.918    -6.416  
+211118 59536.00 I  0.139777 0.000024  0.245127 0.000028  I-0.1085597 0.0000027  0.0041 0.0018  I  -112.897    0.627    -6.187    0.093  0.139789  0.245077 -0.1085552  -112.878    -6.226  
+211119 59537.00 I  0.137833 0.000024  0.245206 0.000028  I-0.1084680 0.0000025 -0.1848 0.0019  I  -112.755    0.627    -6.238    0.093  0.137868  0.245245 -0.1084680  -112.755    -6.253  
+211120 59538.00 I  0.135539 0.000018  0.245339 0.000026  I-0.1081988 0.0000026 -0.3475 0.0018  I  -112.579    0.623    -6.465    0.045  0.135470  0.245267 -0.1081943  -112.586    -6.495  
+211121 59539.00 I  0.133470 0.000019  0.245958 0.000025  I-0.1077913 0.0000027 -0.4552 0.0017  I  -112.409    0.623    -6.679    0.045  0.133433  0.245936 -0.1077699  -112.425    -6.731  
+211122 59540.00 I  0.131599 0.000019  0.246865 0.000028  I-0.1073005 0.0000021 -0.5268 0.0019  I  -112.252    0.687    -6.767    0.052  0.131584  0.246933 -0.1072664  -112.282    -6.830  
+211123 59541.00 I  0.129625 0.000017  0.247267 0.000020  I-0.1067521 0.0000026 -0.5554 0.0019  I  -112.119    0.724    -6.790    0.058  0.129614  0.247350 -0.1067281  -112.157    -6.857  
+211124 59542.00 I  0.127862 0.000021  0.247289 0.000022  I-0.1062149 0.0000032 -0.5085 0.0021  I  -111.996    0.739    -6.838    0.054  0.127746  0.247246 -0.1062044  -112.031    -6.907  
+211125 59543.00 I  0.126572 0.000021  0.247710 0.000022  I-0.1057449 0.0000034 -0.4323 0.0025  I  -111.791    0.739    -6.875    0.054  0.126546  0.247694 -0.1057277  -111.742    -6.907  
+211126 59544.00 I  0.125316 0.000021  0.248348 0.000021  I-0.1053930 0.0000038 -0.2279 0.0031  I  -111.356    0.923    -6.733    0.032  0.125318  0.248339 -0.1053900  -111.268    -6.773  
+211127 59545.00 I  0.123944 0.000020  0.249146 0.000021  I-0.1053216 0.0000051  0.0741 0.0044  I  -111.042    0.923    -6.557    0.032  0.123926  0.249137 -0.1053000  -110.920    -6.580  
+211128 59546.00 I  0.122508 0.000023  0.250102 0.000027  I-0.1055073 0.0000079  0.2745 0.0047  I  -110.967    0.532    -6.419    0.140  0.122510  0.250182 -0.1054501  -110.876    -6.447  
+211129 59547.00 I  0.120992 0.000023  0.250797 0.000027  I-0.1058347 0.0000080  0.3671 0.0056  I  -111.176    0.532    -6.413    0.140  0.120935  0.250800 -0.1057693  -111.138    -6.452  
+211130 59548.00 I  0.119475 0.000020  0.251394 0.000025  I-0.1062537 0.0000080  0.4963 0.0052  I  -111.442    0.488    -6.403    0.159  0.119462  0.251409 -0.1062356  -111.496    -6.463  
+2112 1 59549.00 I  0.117974 0.000021  0.252124 0.000029  I-0.1068110 0.0000066  0.5767 0.0052  I  -111.625    0.616    -6.214    0.137  0.117908  0.252101 -0.1068219  -111.672    -6.258  
+2112 2 59550.00 I  0.116669 0.000021  0.253079 0.000030  I-0.1073553 0.0000067  0.5019 0.0047  I  -111.845    0.616    -5.940    0.137  0.116646  0.253077 -0.1073817  -111.874    -5.966  
+2112 3 59551.00 I  0.115236 0.000022  0.254064 0.000030  I-0.1077674 0.0000067  0.2850 0.0052  I  -112.117    0.616    -5.860    0.137  0.115236  0.254139 -0.1077758  -112.122    -5.874  
+2112 4 59552.00 I  0.113608 0.000016  0.254414 0.000021  I-0.1078987 0.0000080 -0.0118 0.0041  I  -112.182    0.717    -6.016    0.112  0.113528  0.254463 -0.1079062  -112.187    -6.031  
+2112 5 59553.00 I  0.112222 0.000019  0.254586 0.000023  I-0.1077731 0.0000047 -0.2208 0.0047  I  -111.890    0.699    -6.133    0.117  0.112210  0.254544 -0.1077891  -111.884    -6.154  
+2112 6 59554.00 I  0.110908 0.000021  0.255092 0.000025  I-0.1075124 0.0000048 -0.2640 0.0035  I  -111.497    0.699    -6.053    0.117  0.110933  0.255126 -0.1075299  -111.458    -6.078  
+2112 7 59555.00 I  0.109156 0.000022  0.255657 0.000022  I-0.1072705 0.0000051 -0.2311 0.0033  I  -111.339    0.657    -5.973    0.123  0.109262  0.255631 -0.1072636  -111.227    -6.002  
+2112 8 59556.00 I  0.106687 0.000025  0.256268 0.000029  I-0.1070812 0.0000044 -0.1051 0.0033  I  -111.253    0.621    -6.110    0.125  0.106686  0.256326 -0.1071092  -111.176    -6.134  
+2112 9 59557.00 I  0.104022 0.000025  0.256732 0.000029  I-0.1071108 0.0000042  0.1723 0.0028  I  -111.162    0.621    -6.317    0.125  0.103984  0.256757 -0.1071653  -111.132    -6.338  
+211210 59558.00 I  0.101400 0.000026  0.257088 0.000028  I-0.1073893 0.0000035  0.3401 0.0032  I  -111.069    0.621    -6.289    0.125  0.101414  0.257116 -0.1074002  -111.095    -6.308  
+211211 59559.00 I  0.098431 0.000024  0.257355 0.000027  I-0.1077608 0.0000047  0.4174 0.0024  I  -111.051    0.590    -5.980    0.127  0.098426  0.257383 -0.1077748  -111.085    -5.998  
+211212 59560.00 I  0.095295 0.000022  0.257381 0.000030  I-0.1082100 0.0000032  0.4526 0.0028  I  -111.088    0.716    -5.636    0.114  0.095231  0.257384 -0.1082102  -111.113    -5.653  
+211213 59561.00 I  0.092594 0.000021  0.257467 0.000029  I-0.1086269 0.0000032  0.3705 0.0022  I  -111.130    0.716    -5.456    0.114  0.092509  0.257408 -0.1086201  -111.139    -5.474  
+211214 59562.00 I  0.090280 0.000019  0.258071 0.000021  I-0.1089523 0.0000030  0.2922 0.0024  I  -111.194    0.820    -5.403    0.098  0.090306  0.258026 -0.1089586  -111.161    -5.420  
+211215 59563.00 I  0.087851 0.000028  0.258957 0.000030  I-0.1092029 0.0000036  0.1888 0.0025  I  -111.284    0.749    -5.355    0.119  0.087829  0.258992 -0.1091980  -111.310    -5.388  
+211216 59564.00 I  0.085324 0.000028  0.259746 0.000031  I-0.1093137 0.0000039  0.0370 0.0027  I  -111.510    0.486    -5.368    0.150  0.085353  0.259707 -0.1093060  -111.400    -5.371  
+211217 59565.00 I  0.082673 0.000028  0.260685 0.000030  I-0.1092674 0.0000039 -0.1431 0.0034  I  -111.309    0.486    -5.432    0.150  0.082621  0.260745 -0.1092661  -111.355    -5.475  
+211218 59566.00 I  0.080323 0.000027  0.261293 0.000026  I-0.1090445 0.0000056 -0.2721 0.0031  I  -111.058    0.486    -5.638    0.150  0.080179  0.261328 -0.1090678  -111.129    -5.691  
+211219 59567.00 I  0.078759 0.000028  0.261727 0.000030  I-0.1087445 0.0000047 -0.3372 0.0036  I  -110.867    0.696    -5.856    0.099  0.078732  0.261660 -0.1087469  -110.910    -5.904  
+211220 59568.00 I  0.077307 0.000028  0.262558 0.000030  I-0.1083780 0.0000046 -0.3787 0.0029  I  -110.735    0.696    -5.951    0.099  0.077355  0.262569 -0.1083780  -110.743    -5.989  
+211221 59569.00 I  0.075382 0.000020  0.263451 0.000032  I-0.1079939 0.0000034 -0.3999 0.0027  I  -110.577    0.698    -5.935    0.051  0.075405  0.263444 -0.1079991  -110.539    -5.957  
+211222 59570.00 I  0.073157 0.000019  0.264273 0.000032  I-0.1075984 0.0000030 -0.3604 0.0022  I  -110.343    0.698    -5.915    0.051  0.073133  0.264278 -0.1076234  -110.373    -5.927  
+211223 59571.00 I  0.070906 0.000019  0.265198 0.000032  I-0.1073220 0.0000029 -0.1742 0.0021  I  -110.040    0.698    -5.934    0.051  0.070881  0.265173 -0.1073418  -110.167    -5.926  
+211224 59572.00 I  0.068527 0.000019  0.266491 0.000034  I-0.1072533 0.0000030  0.0219 0.0021  I  -109.302    0.322    -6.229    0.160  0.068514  0.266510 -0.1072445  -109.820    -5.942  
+211225 59573.00 I  0.066137 0.000017  0.267798 0.000030  I-0.1073673 0.0000029  0.2226 0.0019  I  -109.009    0.322    -6.115    0.160  0.066054  0.267813 -0.1073681  -109.476    -5.912  
+211226 59574.00 I  0.064276 0.000023  0.268997 0.000037  I-0.1077126 0.0000023  0.4655 0.0020  I  -108.951    0.879    -6.014    0.333  0.064264  0.268977 -0.1077173  -109.284    -5.893  
+211227 59575.00 I  0.062755 0.000023  0.270355 0.000028  I-0.1082711 0.0000027  0.6268 0.0016  I  -109.120    0.879    -5.996    0.333  0.062771  0.270366 -0.1082590  -109.258    -5.955  
+211228 59576.00 I  0.061075 0.000031  0.271920 0.000036  I-0.1089221 0.0000022  0.6559 0.0017  I  -109.409    0.740    -5.972    0.320  0.061119  0.271893 -0.1089162  -109.321    -6.008  
+211229 59577.00 I  0.059245 0.000030  0.273459 0.000036  I-0.1095581 0.0000022  0.6105 0.0015  I  -109.787    0.740    -5.788    0.320  0.059184  0.273531 -0.1095688  -109.829    -5.847  
+211230 59578.00 I  0.057738 0.000030  0.274728 0.000036  I-0.1101027 0.0000021  0.4441 0.0015  I  -110.724    0.150    -5.506    0.299  0.057753  0.274728 -0.1101029  -110.666    -5.562  
+211231 59579.00 I  0.056257 0.000030  0.275943 0.000035  I-0.1104179 0.0000019  0.1927 0.0016  I  -111.345    0.150    -5.371    0.299  0.056304  0.275973 -0.1104355  -111.412    -5.426  
+22 1 1 59580.00 I  0.054644 0.000026  0.276986 0.000032  I-0.1104988 0.0000023 -0.0267 0.0022  I  -111.826    0.150    -5.524    0.299  0.054574  0.276983 -0.1105197  -111.899    -5.573  
+22 1 2 59581.00 I  0.053441 0.000030  0.277925 0.000033  I-0.1103729 0.0000040 -0.2209 0.0029  I  -111.797    0.316    -5.758    0.223  0.053381  0.277886 -0.1103891  -111.877    -5.801  
+22 1 3 59582.00 I  0.052973 0.000021  0.279047 0.000025  I-0.1101047 0.0000054 -0.2719 0.0034  I  -111.314    0.338    -5.830    0.175  0.052855  0.278999 -0.1101398  -111.401    -5.868  
+22 1 4 59583.00 I  0.053260 0.000022  0.280694 0.000025  I-0.1099008 0.0000056 -0.1079 0.0039  I  -110.721    0.338    -5.796    0.175  0.053294  0.280607 -0.1099190  -110.807    -5.829  
+22 1 5 59584.00 I  0.053468 0.000024  0.282930 0.000027  I-0.1099040 0.0000055  0.1013 0.0040  I  -110.221    0.400    -5.847    0.149  0.053559  0.282963 -0.1098692  -110.307    -5.882  
+22 1 6 59585.00 I  0.052941 0.000023  0.285050 0.000027  I-0.1100781 0.0000056  0.2346 0.0040  I  -109.851    0.400    -5.934    0.149  0.053042  0.285048 -0.1100259  -109.937    -5.974  
+22 1 7 59586.00 I  0.051789 0.000022  0.286929 0.000023  I-0.1103701 0.0000059  0.3586 0.0044  I  -109.691    0.400    -5.815    0.149  0.051849  0.286983 -0.1103610  -109.778    -5.861  
+22 1 8 59587.00 I  0.050226 0.000015  0.288661 0.000019  I-0.1107840 0.0000069  0.4488 0.0044  I  -109.807    0.474    -5.434    0.112  0.050225  0.288671 -0.1107892  -109.885    -5.484  
+22 1 9 59588.00 I  0.048620 0.000018  0.290196 0.000022  I-0.1112265 0.0000066  0.4156 0.0048  I  -110.085    0.666    -5.046    0.077  0.048602  0.290231 -0.1112277  -110.147    -5.099  
+22 110 59589.00 I  0.047147 0.000019  0.291470 0.000022  I-0.1115956 0.0000066  0.3238 0.0051  I  -110.337    0.666    -4.909    0.077  0.047155  0.291472 -0.1116091  -110.373    -4.960  
+22 111 59590.00 I  0.045621 0.000018  0.292556 0.000016  I-0.1118561 0.0000079  0.1781 0.0044  I  -110.469    0.740    -4.985    0.028  0.045595  0.292576 -0.1118697  -110.484    -5.049  
+22 112 59591.00 I  0.044275 0.000018  0.293459 0.000023  I-0.1119402 0.0000058 -0.0025 0.0050  I  -110.608    0.660    -5.145    0.053  0.044205  0.293449 -0.1119606  -110.597    -5.195  
+22 113 59592.00 I  0.043440 0.000019  0.294438 0.000024  I-0.1118519 0.0000060 -0.1806 0.0041  I  -110.612    0.660    -5.231    0.053  0.043394  0.294345 -0.1118677  -110.603    -5.273  
+22 114 59593.00 I  0.043161 0.000019  0.295889 0.000024  I-0.1115808 0.0000058 -0.3533 0.0040  I  -110.445    0.660    -5.319    0.053  0.043106  0.295839 -0.1115941  -110.438    -5.353  
+22 115 59594.00 I  0.043042 0.000019  0.297881 0.000021  I-0.1111492 0.0000054 -0.5142 0.0040  I  -110.205    0.575    -5.508    0.069  0.043114  0.297844 -0.1111643  -110.195    -5.540  
+22 116 59595.00 I  0.042499 0.000022  0.299844 0.000022  I-0.1105848 0.0000054 -0.5777 0.0034  I  -110.046    0.575    -5.758    0.069  0.042534  0.299918 -0.1106129  -110.039    -5.787  
+22 117 59596.00 I  0.041460 0.000022  0.301471 0.000027  I-0.1100033 0.0000042 -0.6126 0.0034  I  -109.983    0.501    -5.927    0.124  0.041549  0.301463 -0.1100064  -109.987    -5.955  
+22 118 59597.00 I  0.039933 0.000021  0.302929 0.000022  I-0.1093690 0.0000040 -0.6192 0.0030  I  -109.869    0.374    -5.944    0.164  0.039912  0.303016 -0.1093760  -109.902    -5.973  
+22 119 59598.00 I  0.038548 0.000022  0.303977 0.000025  I-0.1088123 0.0000043 -0.4835 0.0029  I  -109.593    0.464    -5.875    0.198  0.038420  0.303951 -0.1088179  -109.671    -5.907  
+22 120 59599.00 I  0.037866 0.000022  0.305019 0.000024  I-0.1084318 0.0000042 -0.2584 0.0029  I  -109.227    0.464    -5.821    0.198  0.037831  0.305025 -0.1084531  -109.285    -5.871  
+22 121 59600.00 I  0.037467 0.000019  0.306187 0.000024  I-0.1082918 0.0000040 -0.0442 0.0029  I  -108.950    0.464    -5.816    0.198  0.037456  0.306196 -0.1082981  -108.956    -5.893  
+22 122 59601.00 I  0.036910 0.000015  0.307343 0.000023  I-0.1083222 0.0000041  0.1065 0.0030  I  -108.860    0.464    -5.827    0.198  0.036968  0.307328 -0.1083306  -108.866    -5.897  
+22 123 59602.00 I  0.035920 0.000018  0.308664 0.000018  I-0.1084942 0.0000044  0.2253 0.0031  I  -108.910    0.396    -5.823    0.181  0.036011  0.308634 -0.1085119  -108.922    -5.877  
+22 124 59603.00 I  0.034432 0.000018  0.310118 0.000017  I-0.1087496 0.0000046  0.2746 0.0033  I  -109.027    0.396    -5.800    0.181  0.034458  0.310100 -0.1087689  -109.048    -5.839  
+22 125 59604.00 I  0.032765 0.000017  0.311527 0.000010  I-0.1090171 0.0000049  0.2451 0.0029  I  -109.178    0.269    -5.738    0.125  0.032747  0.311519 -0.1090294  -109.241    -5.759  
+22 126 59605.00 I  0.031386 0.000023  0.312803 0.000014  I-0.1092155 0.0000034  0.1429 0.0030  I  -109.365    0.421    -5.619    0.157  0.031327  0.312793 -0.1092242  -109.416    -5.652  
+22 127 59606.00 I  0.030246 0.000024  0.314138 0.000015  I-0.1092761 0.0000036 -0.0395 0.0024  I  -109.655    0.421    -5.500    0.157  0.030254  0.314102 -0.1092764  -109.698    -5.548  
+22 128 59607.00 I  0.029130 0.000024  0.315630 0.000017  I-0.1091307 0.0000034 -0.2394 0.0027  I  -109.981    0.563    -5.525    0.185  0.029060  0.315654 -0.1091370  -110.085    -5.577  
+22 129 59608.00 I  0.028298 0.000021  0.317168 0.000016  I-0.1088120 0.0000041 -0.3953 0.0027  I  -110.443    0.563    -5.741    0.185  0.028306  0.317130 -0.1088191  -110.488    -5.790  
+22 130 59609.00 I  0.027570 0.000024  0.318991 0.000021  I-0.1083554 0.0000043 -0.5052 0.0030  I  -110.599    0.461    -6.021    0.198  0.027664  0.318978 -0.1083658  -110.627    -6.064  
+22 131 59610.00 I  0.026683 0.000024  0.320958 0.000021  I-0.1078395 0.0000043 -0.5013 0.0035  I  -110.410    0.461    -6.182    0.198  0.026619  0.320963 -0.1078483  -110.424    -6.222  
+22 2 1 59611.00 I  0.026123 0.000018  0.323070 0.000019  I-0.1073953 0.0000055 -0.3700 0.0035  I  -110.025    0.395    -6.224    0.209  0.026102  0.323015 -0.1073994  -110.029    -6.256  
+22 2 2 59612.00 I  0.025848 0.000026  0.325448 0.000020  I-0.1071299 0.0000055 -0.1474 0.0040  I  -109.557    0.397    -6.236    0.225  0.025834  0.325489 -0.1071431  -109.538    -6.310  
+22 2 3 59613.00 I  0.025709 0.000027  0.327754 0.000020  I-0.1070988 0.0000059  0.0701 0.0041  I  -109.168    0.397    -6.270    0.225  0.025683  0.327751 -0.1070987  -109.116    -6.393  
+22 2 4 59614.00 I  0.025771 0.000026  0.329988 0.000020  I-0.1072359 0.0000062  0.1850 0.0067  I  -109.000    0.397    -6.201    0.225  0.025779  0.330022 -0.1072225  -108.919    -6.381  
+22 2 5 59615.00 I  0.025748 0.000025  0.332144 0.000014  I-0.1074324 0.0000121  0.1907 0.0043  I  -109.148    0.439    -5.977    0.284  0.025738  0.332211 -0.1074267  -109.063    -6.141  
+22 2 6 59616.00 I  0.025719 0.000027  0.333909 0.000017  I-0.1075893 0.0000061  0.1123 0.0068  I  -109.520    0.477    -5.750    0.130  0.025676  0.333942 -0.1076113  -109.447    -5.873  
+22 2 7 59617.00 I  0.025701 0.000027  0.335614 0.000018  I-0.1076479 0.0000061  0.0064 0.0044  I  -109.902    0.477    -5.709    0.130  0.025772  0.335603 -0.1076870  -109.853    -5.790  
+22 2 8 59618.00 I  0.025135 0.000017  0.337291 0.000015  I-0.1075786 0.0000064 -0.1701 0.0042  I  -110.126    0.484    -5.837    0.013  0.025193  0.337374 -0.1075919  -110.126    -5.888  
+22 2 9 59619.00 I  0.024113 0.000018  0.338501 0.000021  I-0.1072942 0.0000058 -0.3872 0.0043  I  -110.187    0.502    -6.026    0.021  0.024114  0.338478 -0.1072977  -110.203    -6.067  
+22 210 59620.00 I  0.022890 0.000018  0.339530 0.000021  I-0.1068126 0.0000056 -0.5793 0.0040  I  -110.037    0.502    -6.107    0.021  0.022952  0.339544 -0.1067962  -110.062    -6.157  
+22 211 59621.00 I  0.021291 0.000017  0.340652 0.000022  I-0.1061234 0.0000056 -0.8081 0.0043  I  -109.675    0.502    -6.143    0.021  0.021317  0.340636 -0.1061126  -109.706    -6.193  
+22 212 59622.00 I  0.019528 0.000015  0.341934 0.000020  I-0.1052494 0.0000064 -0.8781 0.0037  I  -109.225    0.542    -6.268    0.027  0.019510  0.341957 -0.1052912  -109.259    -6.321  
+22 213 59623.00 I  0.018054 0.000016  0.343126 0.000024  I-0.1044131 0.0000049 -0.8105 0.0040  I  -108.888    0.571    -6.506    0.097  0.017952  0.343165 -0.1044265  -108.917    -6.560  
+22 214 59624.00 I  0.017241 0.000015  0.344317 0.000024  I-0.1036308 0.0000049 -0.7357 0.0035  I  -108.746    0.571    -6.738    0.097  0.017178  0.344276 -0.1036375  -108.763    -6.785  
+22 215 59625.00 I  0.016801 0.000013  0.345841 0.000019  I-0.1029828 0.0000049 -0.5377 0.0032  I  -108.687    0.593    -6.834    0.133  0.016814  0.345848 -0.1029937  -108.690    -6.864  
+22 216 59626.00 I  0.016422 0.000016  0.347670 0.000019  I-0.1025493 0.0000040 -0.3581 0.0031  I  -108.562    0.565    -6.770    0.218  0.016373  0.347600 -0.1025279  -108.569    -6.803  
+22 217 59627.00 I  0.016159 0.000016  0.349971 0.000018  I-0.1022728 0.0000039 -0.1600 0.0028  I  -108.360    0.565    -6.659    0.218  0.016174  0.349955 -0.1022855  -108.379    -6.702  
+22 218 59628.00 I  0.015973 0.000015  0.352529 0.000018  I-0.1022552 0.0000038  0.1158 0.0028  I  -108.215    0.565    -6.612    0.218  0.015893  0.352552 -0.1022778  -108.238    -6.679  
+22 219 59629.00 I  0.016039 0.000014  0.354991 0.000013  I-0.1024744 0.0000039  0.3015 0.0027  I  -108.224    0.540    -6.649    0.274  0.016057  0.355009 -0.1024803  -108.239    -6.688  
+22 220 59630.00 I  0.016150 0.000022  0.357313 0.000017  I-0.1028227 0.0000038  0.3805 0.0026  I  -108.366    0.515    -6.713    0.218  0.016152  0.357350 -0.1028229  -108.367    -6.714  
+22 221 59631.00 I  0.016267 0.000024  0.359423 0.000016  I-0.1032029 0.0000034  0.3620 0.0028  I  -108.582    0.515    -6.731    0.218  0.016225  0.359459 -0.1032042  -108.568    -6.699  
+22 222 59632.00 I  0.016729 0.000022  0.361222 0.000016  I-0.1035198 0.0000041  0.2629 0.0027  I  -108.840    0.439    -6.683    0.064  0.016672  0.361277 -0.1035256  -108.817    -6.617  
+22 223 59633.00 I  0.017620 0.000025  0.362789 0.000020  I-0.1037067 0.0000042  0.0976 0.0029  I  -109.095    0.443    -6.615    0.146  0.017619  0.362779 -0.1037081  -109.078    -6.583  
+22 224 59634.00 I  0.018441 0.000025  0.364347 0.000020  I-0.1036979 0.0000042 -0.1192 0.0030  I  -109.261    0.443    -6.601    0.146  0.018496  0.364360 -0.1036928  -109.259    -6.613  
+22 225 59635.00 I  0.018982 0.000024  0.365793 0.000019  I-0.1034735 0.0000043 -0.3204 0.0033  I  -109.219    0.448    -6.729    0.192  0.018931  0.365807 -0.1034734  -109.270    -6.743  
+22 226 59636.00 I  0.019617 0.000018  0.367245 0.000017  I-0.1030872 0.0000050 -0.4312 0.0027  I  -109.056    0.448    -6.878    0.192  0.019607  0.367229 -0.1031018  -109.106    -6.902  
+22 227 59637.00 I  0.020237 0.000021  0.368842 0.000020  I-0.1026591 0.0000031 -0.3981 0.0029  I  -108.805    0.418    -7.028    0.155  0.020241  0.368836 -0.1026797  -108.854    -7.042  
+22 228 59638.00 I  0.020643 0.000022  0.370620 0.000020  I-0.1023234 0.0000031 -0.2680 0.0020  I  -108.575    0.418    -7.105    0.155  0.020656  0.370624 -0.1023250  -108.624    -7.107  
+22 3 1 59639.00 I  0.020995 0.000019  0.372307 0.000017  I-0.1021399 0.0000025 -0.0876 0.0025  I  -108.412    0.383    -7.117    0.104  0.020909  0.372342 -0.1021425  -108.462    -7.107  
+22 3 2 59640.00 I  0.021875 0.000022  0.374044 0.000021  I-0.1021706 0.0000039  0.1600 0.0023  I  -108.285    0.490    -7.126    0.107  0.021778  0.373951 -0.1021944  -108.199    -7.104  
+22 3 3 59641.00 I  0.023305 0.000022  0.376260 0.000020  I-0.1024422 0.0000039  0.3544 0.0027  I  -108.155    0.490    -7.153    0.107  0.023290  0.376273 -0.1024561  -107.898    -7.117  
+22 3 4 59642.00 I  0.025009 0.000023  0.378484 0.000019  I-0.1028386 0.0000038  0.4263 0.0036  I  -108.032    0.762    -7.162    0.115  0.024972  0.378479 -0.1028435  -107.637    -7.109  
+22 3 5 59643.00 I  0.026706 0.000017  0.380550 0.000016  I-0.1032508 0.0000061  0.3660 0.0031  I  -108.082    0.762    -7.127    0.115  0.026774  0.380581 -0.1032424  -107.706    -7.086  
+22 3 6 59644.00 I  0.028127 0.000017  0.382627 0.000022  I-0.1035497 0.0000049  0.2429 0.0039  I  -108.304    0.501    -7.110    0.073  0.028086  0.382600 -0.1035550  -108.027    -7.094  
+22 3 7 59645.00 I  0.029547 0.000016  0.384742 0.000021  I-0.1037253 0.0000048  0.0860 0.0032  I  -108.610    0.501    -7.183    0.073  0.029543  0.384798 -0.1037203  -108.450    -7.191  
+22 3 8 59646.00 I  0.031002 0.000010  0.386679 0.000018  I-0.1036867 0.0000041 -0.1760 0.0029  I  -108.843    0.446    -7.322    0.060  0.031018  0.386712 -0.1036844  -108.826    -7.354  
+22 3 9 59647.00 I  0.032216 0.000012  0.388518 0.000020  I-0.1033883 0.0000031 -0.3931 0.0026  I  -108.861    0.640    -7.427    0.047  0.032281  0.388541 -0.1034089  -108.866    -7.460  
+22 310 59648.00 I  0.033082 0.000010  0.390315 0.000021  I-0.1029238 0.0000031 -0.5404 0.0022  I  -108.353    0.785    -7.426    0.029  0.033104  0.390312 -0.1029383  -108.612    -7.475  
+22 311 59649.00 I  0.033674 0.000013  0.392091 0.000021  I-0.1023234 0.0000032 -0.6398 0.0021  I  -108.004    0.785    -7.446    0.029  0.033708  0.392105 -0.1023346  -108.109    -7.473  
+22 312 59650.00 I  0.034135 0.000016  0.393701 0.000015  I-0.1016717 0.0000029 -0.6565 0.0021  I  -107.521    0.785    -7.560    0.029  0.034130  0.393729 -0.1016864  -107.569    -7.581  
+22 313 59651.00 I  0.034426 0.000022  0.395168 0.000018  I-0.1010181 0.0000027 -0.6501 0.0020  I  -107.088    0.707    -7.795    0.042  0.034502  0.395152 -0.1010372  -107.117    -7.813  
+22 314 59652.00 I  0.034370 0.000023  0.396646 0.000017  I-0.1003917 0.0000027 -0.5830 0.0024  I  -106.859    0.707    -8.049    0.042  0.034354  0.396685 -0.1004104  -106.877    -8.063  
+22 315 59653.00 I  0.034236 0.000023  0.398032 0.000014  I-0.0998809 0.0000039 -0.4295 0.0023  I  -106.880    0.600    -8.182    0.052  0.034250  0.398014 -0.0998830  -106.865    -8.198  
+22 316 59654.00 I  0.033954 0.000033  0.399557 0.000016  I-0.0995535 0.0000038 -0.2135 0.0027  I  -106.947    0.617    -8.164    0.103  0.033972  0.399563 -0.0995467  -106.918    -8.181  
+22 317 59655.00 I  0.033459 0.000032  0.401248 0.000016  I-0.0994564 0.0000036  0.0100 0.0027  I  -106.984    0.617    -8.037    0.103  0.033426  0.401244 -0.0994339  -106.930    -8.064  
+22 318 59656.00 I  0.033078 0.000030  0.402896 0.000016  I-0.0995545 0.0000039  0.1765 0.0032  I  -106.956    0.617    -7.907    0.103  0.033046  0.402931 -0.0995428  -106.876    -7.950  
+22 319 59657.00 I  0.032925 0.000026  0.404440 0.000013  I-0.0998023 0.0000052  0.3217 0.0032  I  -106.959    0.659    -7.852    0.165  0.032894  0.404430 -0.0998242  -106.884    -7.889  
+22 320 59658.00 I  0.033030 0.000026  0.405969 0.000013  I-0.1001813 0.0000050  0.4171 0.0032  I  -107.117    0.659    -7.890    0.165  0.033017  0.405997 -0.1001905  -107.059    -7.919  
+22 321 59659.00 I  0.033374 0.000032  0.407427 0.000017  I-0.1005703 0.0000036  0.3138 0.0031  I  -107.450    0.572    -7.980    0.111  0.033291  0.407432 -0.1005194  -107.409    -8.005  
+22 322 59660.00 I  0.034273 0.000022  0.408901 0.000014  I-0.1007722 0.0000035  0.1005 0.0032  I  -107.861    0.530    -8.021    0.068  0.034163  0.408866 -0.1007374  -107.806    -8.084  
+22 323 59661.00 I  0.035750 0.000024  0.410730 0.000014  I-0.1007766 0.0000052 -0.0967 0.0031  I  -108.093    0.497    -8.079    0.071  0.035739  0.410677 -0.1007668  -108.069    -8.122  
+22 324 59662.00 I  0.037151 0.000024  0.412884 0.000014  I-0.1005739 0.0000052 -0.3084 0.0035  I  -108.064    0.497    -8.114    0.071  0.037184  0.412921 -0.1005632  -108.121    -8.146  
+22 325 59663.00 I  0.038266 0.000024  0.414992 0.000015  I-0.1001880 0.0000048 -0.4355 0.0036  I  -107.764    0.497    -8.165    0.071  0.038276  0.415002 -0.1001852  -107.917    -8.187  
+22 326 59664.00 I  0.039265 0.000023  0.416914 0.000015  I-0.0997422 0.0000050 -0.4445 0.0037  I  -107.290    0.497    -8.243    0.071  0.039275  0.416959 -0.0997325  -107.413    -8.263  
+22 327 59665.00 I  0.040352 0.000018  0.418581 0.000012  I-0.0993293 0.0000057 -0.3624 0.0038  I  -106.799    0.538    -8.326    0.085  0.040293  0.418593 -0.0993188  -106.847    -8.345  
+22 328 59666.00 I  0.041639 0.000017  0.420174 0.000013  I-0.0990507 0.0000058 -0.1803 0.0037  I  -106.438    0.538    -8.391    0.085  0.041691  0.420175 -0.0990554  -106.412    -8.410  
+22 329 59667.00 I  0.042747 0.000016  0.421684 0.000013  I-0.0989745 0.0000048  0.0193 0.0035  I  -106.254    0.660    -8.423    0.077  0.042792  0.421696 -0.0989777  -106.189    -8.449  
+22 330 59668.00 I  0.043408 0.000019  0.423095 0.000018  I-0.0990621 0.0000040  0.1372 0.0032  I  -106.308    0.629    -8.427    0.080  0.043491  0.423055 -0.0990426  -106.244    -8.453  
+22 331 59669.00 I  0.043544 0.000020  0.424826 0.000018  I-0.0992408 0.0000041  0.2308 0.0028  I  -106.436    0.629    -8.386    0.080  0.043570  0.424794 -0.0992346  -106.398    -8.414  
+22 4 1 59670.00 I  0.043355 0.000022  0.426902 0.000018  I-0.0995152 0.0000038  0.2990 0.0029  I  -106.519    0.629    -8.310    0.080  0.043301  0.426919 -0.0995031  -106.506    -8.343  
+22 4 2 59671.00 I  0.043560 0.000019  0.428907 0.000017  I-0.0998077 0.0000042  0.2738 0.0025  I  -106.531    0.585    -8.249    0.083  0.043471  0.428898 -0.0997958  -106.536    -8.278  
+22 4 3 59672.00 I  0.044378 0.000020  0.431006 0.000019  I-0.1000285 0.0000033  0.1456 0.0026  I  -106.561    0.574    -8.269    0.062  0.044401  0.430964 -0.1000185  -106.583    -8.291  
+22 4 4 59673.00 I  0.045126 0.000020  0.433556 0.000019  I-0.1000837 0.0000031 -0.0282 0.0023  I  -106.688    0.574    -8.380    0.062  0.045179  0.433548 -0.1000877  -106.727    -8.395  
+22 4 5 59674.00 I  0.045609 0.000017  0.436132 0.000015  I-0.0999612 0.0000031 -0.2346 0.0023  I  -106.866    0.565    -8.510    0.032  0.045558  0.436184 -0.0999601  -106.928    -8.515  
+22 4 6 59675.00 I  0.046389 0.000018  0.438265 0.000014  I-0.0996137 0.0000035 -0.4435 0.0025  I  -107.021    0.620    -8.581    0.039  0.046324  0.438296 -0.0996161  -107.011    -8.588  
+22 4 7 59676.00 I  0.047706 0.000017  0.440068 0.000014  I-0.0991024 0.0000038 -0.5678 0.0026  I  -106.894    0.620    -8.605    0.039  0.047660  0.440084 -0.0991087  -106.904    -8.610  
+22 4 8 59677.00 I  0.049437 0.000016  0.441810 0.000014  I-0.0985133 0.0000038 -0.5866 0.0029  I  -106.565    0.620    -8.665    0.039  0.049412  0.441800 -0.0985116  -106.602    -8.670  
+22 4 9 59678.00 I  0.051228 0.000014  0.443582 0.000010  I-0.0979471 0.0000044 -0.5516 0.0025  I  -106.083    0.620    -8.840    0.039  0.051279  0.443588 -0.0979207  -106.131    -8.844  
+22 410 59679.00 I  0.052563 0.000014  0.445318 0.000015  I-0.0974066 0.0000031 -0.5269 0.0027  I  -105.529    0.786    -9.102    0.045  0.052631  0.445310 -0.0973816  -105.574    -9.106  
+22 411 59680.00 I  0.053447 0.000013  0.447060 0.000014  I-0.0969204 0.0000031 -0.4207 0.0022  I  -105.062    0.786    -9.348    0.045  0.053447  0.447037 -0.0969159  -105.095    -9.347  
+22 412 59681.00 I  0.054292 0.000012  0.449012 0.000017  I-0.0965844 0.0000031 -0.2569 0.0021  I  -104.883    0.835    -9.501    0.112  0.054284  0.449011 -0.0965845  -104.884    -9.491  
+22 413 59682.00 I  0.055326 0.000010  0.451054 0.000017  I-0.0964330 0.0000029 -0.0138 0.0022  I  -105.048    0.835    -9.551    0.112  0.055292  0.451073 -0.0964523  -105.062    -9.565  
+22 414 59683.00 I  0.056532 0.000010  0.452863 0.000017  I-0.0965616 0.0000030  0.2438 0.0020  I  -105.349    0.835    -9.493    0.112  0.056547  0.452892 -0.0965557  -105.379    -9.547  
+22 415 59684.00 I  0.057880 0.000015  0.454480 0.000018  I-0.0969019 0.0000028  0.4452 0.0026  I  -105.523    0.835    -9.313    0.112  0.057823  0.454485 -0.0968994  -105.550    -9.362  
+22 416 59685.00 I  0.059421 0.000020  0.456167 0.000015  I-0.0974266 0.0000042  0.5705 0.0026  I  -105.584    0.778    -9.059    0.154  0.059424  0.456172 -0.0974129  -105.603    -9.095  
+22 417 59686.00 I  0.061289 0.000021  0.457792 0.000015  I-0.0979911 0.0000043  0.5403 0.0033  I  -105.790    0.778    -8.874    0.154  0.061164  0.457851 -0.0979865  -105.807    -8.908  
+22 418 59687.00 I  0.063720 0.000026  0.459301 0.000013  I-0.0984761 0.0000050  0.4168 0.0033  I  -106.252    0.806    -8.891    0.015  0.063734  0.459266 -0.0985020  -106.274    -8.922  
+22 419 59688.00 I  0.066167 0.000028  0.460813 0.000014  I-0.0988025 0.0000050  0.2265 0.0031  I  -106.782    0.806    -8.999    0.015  0.066192  0.460869 -0.0988272  -106.773    -9.104  
+22 420 59689.00 I  0.068332 0.000029  0.461998 0.000015  I-0.0988976 0.0000036 -0.0585 0.0031  I  -106.912    0.792    -9.262    0.084  0.068329  0.461999 -0.0988949  -106.960    -9.291  
+22 421 59690.00 I  0.070492 0.000027  0.463054 0.000015  I-0.0986939 0.0000036 -0.3182 0.0025  I  -106.641    0.792    -9.418    0.084  0.070468  0.463064 -0.0987060  -106.695    -9.434  
+22 422 59691.00 I  0.072758 0.000023  0.464105 0.000016  I-0.0983227 0.0000036 -0.3933 0.0025  I  -106.179    0.792    -9.477    0.084  0.072707  0.464098 -0.0983386  -106.211    -9.508  
+22 423 59692.00 I  0.075224 0.000022  0.465086 0.000015  I-0.0979347 0.0000036 -0.3862 0.0031  I  -105.765    0.792    -9.509    0.084  0.075204  0.465058 -0.0979051  -105.797    -9.527  
+22 424 59693.00 I  0.077857 0.000017  0.466283 0.000026  I-0.0975643 0.0000050 -0.3372 0.0031  I  -105.469    0.768    -9.550    0.101  0.077859  0.466247 -0.0975194  -105.498    -9.555  
+22 425 59694.00 I  0.080484 0.000015  0.467927 0.000025  I-0.0972900 0.0000050 -0.1990 0.0052  I  -105.250    0.768    -9.589    0.101  0.080557  0.467896 -0.0972632  -105.265    -9.590  
+22 426 59695.00 I  0.082817 0.000013  0.469839 0.000025  I-0.0971796 0.0000092 -0.0210 0.0040  I  -105.105    0.734    -9.598    0.070  0.082859  0.469891 -0.0971847  -105.109    -9.593  
+22 427 59696.00 I  0.084840 0.000019  0.471459 0.000028  I-0.0972299 0.0000063  0.1028 0.0055  I  -105.009    0.749    -9.695    0.183  0.084908  0.471486 -0.0972203  -105.096    -9.548  
+22 428 59697.00 I  0.086491 0.000020  0.472740 0.000027  I-0.0973576 0.0000062  0.1438 0.0044  I  -105.194    0.749    -9.487    0.183  0.086518  0.472819 -0.0973522  -105.258    -9.407  
+22 429 59698.00 I  0.087933 0.000020  0.473537 0.000028  I-0.0974959 0.0000061  0.1200 0.0040  I  -105.450    0.749    -9.213    0.183  0.087895  0.473595 -0.0974914  -105.480    -9.203  
+22 430 59699.00 I  0.089678 0.000019  0.474076 0.000017  I-0.0975807 0.0000050  0.0453 0.0039  I  -105.613    0.749    -8.997    0.183  0.089653  0.474104 -0.0975559  -105.614    -9.011  
+22 5 1 59700.00 I  0.091696 0.000020  0.474622 0.000018  I-0.0975681 0.0000050 -0.0848 0.0037  I  -105.650    0.749    -8.968    0.183  0.091728  0.474632 -0.0975257  -105.627    -8.987  
+22 5 2 59701.00 I  0.093634 0.000023  0.475315 0.000019  I-0.0974149 0.0000054 -0.2037 0.0038  I  -105.655    0.749    -9.133    0.116  0.093634  0.475311 -0.0974187  -105.619    -9.154  
+22 5 3 59702.00 I  0.095566 0.000018  0.476114 0.000014  I-0.0971873 0.0000058 -0.2429 0.0038  I  -105.768    0.749    -9.322    0.030  0.095563  0.476140 -0.0972185  -105.662    -9.372  
+22 5 4 59703.00 I  0.097693 0.000021  0.476924 0.000016  I-0.0969128 0.0000054 -0.3309 0.0040  I  -105.769    0.784    -9.473    0.037  0.097691  0.476906 -0.0969126  -105.734    -9.493  
+22 5 5 59704.00 I  0.099819 0.000021  0.477880 0.000016  I-0.0965103 0.0000054 -0.4643 0.0038  I  -105.743    0.784    -9.518    0.037  0.099882  0.477903 -0.0964992  -105.770    -9.526  
+22 5 6 59705.00 I  0.101674 0.000022  0.478819 0.000015  I-0.0960238 0.0000054 -0.4787 0.0038  I  -105.687    0.784    -9.589    0.037  0.101687  0.478833 -0.0960256  -105.754    -9.581  
+22 5 7 59706.00 I  0.103388 0.000023  0.479502 0.000013  I-0.0955768 0.0000054 -0.4214 0.0037  I  -105.566    0.784    -9.779    0.037  0.103404  0.479538 -0.0955546  -105.646    -9.779  
+22 5 8 59707.00 I  0.105104 0.000022  0.480062 0.000013  I-0.0951795 0.0000050 -0.3687 0.0037  I  -105.288    0.796   -10.022    0.102  0.105117  0.480078 -0.0951550  -105.347   -10.030  
+22 5 9 59708.00 I  0.106695 0.000023  0.480513 0.000014  I-0.0948755 0.0000052 -0.2078 0.0037  I  -104.882    0.796   -10.188    0.102  0.106699  0.480537 -0.0949242  -104.904   -10.197  
+22 510 59709.00 I  0.108523 0.000019  0.480966 0.000012  I-0.0947980 0.0000055  0.0552 0.0035  I  -104.620    0.772   -10.247    0.139  0.108427  0.480933 -0.0948334  -104.607   -10.261  
+22 511 59710.00 I  0.110912 0.000019  0.481772 0.000014  I-0.0949959 0.0000046  0.3481 0.0036  I  -104.755    0.770   -10.274    0.158  0.110941  0.481776 -0.0950144  -104.732   -10.281  
+22 512 59711.00 I  0.113494 0.000017  0.482666 0.000014  I-0.0954625 0.0000045  0.5460 0.0032  I  -105.181    0.770   -10.282    0.158  0.113474  0.482707 -0.0954543  -105.174   -10.290  
+22 513 59712.00 I  0.116069 0.000018  0.483374 0.000015  I-0.0960613 0.0000044  0.6640 0.0029  I  -105.551    0.768   -10.148    0.175  0.116107  0.483379 -0.0960629  -105.566   -10.162  
+22 514 59713.00 I  0.118512 0.000016  0.483943 0.000016  I-0.0967616 0.0000035  0.6953 0.0030  I  -105.716    0.768    -9.777    0.175  0.118527  0.483975 -0.0967431  -105.773    -9.799  
+22 515 59714.00 I  0.120713 0.000024  0.484482 0.000019  I-0.0974001 0.0000040  0.5713 0.0027  I  -106.001    0.850    -9.378    0.156  0.120799  0.484444 -0.0973670  -106.086    -9.399  
+22 516 59715.00 I  0.122292 0.000025  0.485289 0.000018  I-0.0978880 0.0000042  0.3987 0.0039  I  -106.551    0.850    -9.261    0.156  0.122385  0.485333 -0.0978659  -106.653    -9.281  
+22 517 59716.00 I  0.123273 0.000026  0.485803 0.000018  I-0.0981858 0.0000066  0.1911 0.0048  I  -107.041    0.996    -9.497    0.128  0.123240  0.485912 -0.0981728  -107.146    -9.513  
+22 518 59717.00 I  0.124658 0.000029  0.485665 0.000026  I-0.0982687 0.0000086 -0.0210 0.0057  I  -107.050    1.005    -9.840    0.134  0.124614  0.485666 -0.0982338  -107.148    -9.846  
+22 519 59718.00 I  0.126488 0.000028  0.485546 0.000027  I-0.0981576 0.0000092 -0.1917 0.0062  I  -106.584    1.005   -10.039    0.134  0.126492  0.485563 -0.0980742  -106.655   -10.034  
+22 520 59719.00 I  0.128445 0.000027  0.485595 0.000026  I-0.0979316 0.0000089 -0.2234 0.0068  I  -106.007    1.028   -10.111    0.145  0.128370  0.485536 -0.0979421  -106.062   -10.068  
+22 521 59720.00 I  0.130660 0.000021  0.486037 0.000024  I-0.0977566 0.0000101 -0.1175 0.0057  I  -105.734    1.028   -10.101    0.145  0.130677  0.486020 -0.0977739  -105.765   -10.071  
+22 522 59721.00 I  0.132973 0.000024  0.486739 0.000027  I-0.0977032 0.0000071  0.0083 0.0061  I  -105.723    0.874   -10.077    0.090  0.132949  0.486774 -0.0977075  -105.758   -10.059  
+22 523 59722.00 I  0.135354 0.000025  0.487376 0.000026  I-0.0977735 0.0000070  0.1352 0.0048  I  -105.799    0.874    -9.985    0.090  0.135359  0.487350 -0.0977582  -105.848    -9.982  
+22 524 59723.00 I  0.137673 0.000022  0.488128 0.000018  I-0.0979683 0.0000064  0.2463 0.0045  I  -105.815    0.828    -9.816    0.055  0.137703  0.488205 -0.0979698  -105.891    -9.829  
+22 525 59724.00 I  0.139655 0.000023  0.488533 0.000021  I-0.0982372 0.0000056  0.2707 0.0042  I  -105.798    0.868    -9.607    0.057  0.139642  0.488593 -0.0982642  -105.852    -9.614  
+22 526 59725.00 I  0.141661 0.000022  0.488499 0.000021  I-0.0984824 0.0000054  0.2130 0.0038  I  -105.849    0.896    -9.320    0.059  0.141637  0.488529 -0.0985094  -105.918    -9.361  
+22 527 59726.00 I  0.143575 0.000023  0.488453 0.000021  I-0.0986396 0.0000052  0.0844 0.0038  I  -106.128    0.896    -9.089    0.059  0.143638  0.488445 -0.0986407  -106.153    -9.084  
+22 528 59727.00 I  0.145158 0.000019  0.488367 0.000018  I-0.0986187 0.0000054 -0.1416 0.0039  I  -106.450    0.896    -8.926    0.059  0.145102  0.488400 -0.0986068  -106.467    -8.914  
+22 529 59728.00 I  0.146682 0.000016  0.488247 0.000019  I-0.0983361 0.0000057 -0.4286 0.0037  I  -106.643    0.896    -8.978    0.059  0.146706  0.488268 -0.0983314  -106.669    -8.976  
+22 530 59729.00 I  0.148142 0.000024  0.487960 0.000024  I-0.0977616 0.0000050 -0.7154 0.0040  I  -106.668    0.852    -9.288    0.044  0.148067  0.488086 -0.0977877  -106.716    -9.292  
+22 531 59730.00 I  0.149847 0.000023  0.487093 0.000020  I-0.0969215 0.0000057 -0.9538 0.0036  I  -106.715    0.791    -9.681    0.022  0.149795  0.487092 -0.0969563  -106.700    -9.703  
+22 6 1 59731.00 I  0.152001 0.000028  0.486164 0.000024  I-0.0958951 0.0000051 -1.0690 0.0040  I  -106.614    0.998    -9.952    0.041  0.151943  0.486170 -0.0959109  -106.731    -9.971  
+22 6 2 59732.00 I  0.154335 0.000028  0.485428 0.000024  I-0.0947972 0.0000056 -1.1430 0.0039  I  -106.609    0.998   -10.008    0.041  0.154357  0.485426 -0.0947757  -106.670   -10.005  
+22 6 3 59733.00 I  0.156608 0.000027  0.484762 0.000023  I-0.0936390 0.0000060 -1.1272 0.0041  I  -106.726    0.998    -9.982    0.041  0.156589  0.484781 -0.0936356  -106.660    -9.955  
+22 6 4 59734.00 I  0.158876 0.000028  0.484148 0.000022  I-0.0925843 0.0000059 -0.9870 0.0046  I  -106.890    0.998   -10.018    0.041  0.158889  0.484149 -0.0925602  -106.851    -9.984  
+22 6 5 59735.00 I  0.161156 0.000020  0.483620 0.000017  I-0.0916470 0.0000069 -0.9007 0.0040  I  -106.908    1.250   -10.090    0.057  0.161161  0.483622 -0.0916220  -106.921   -10.058  
+22 6 6 59736.00 I  0.163478 0.000025  0.483151 0.000018  I-0.0907993 0.0000053 -0.7650 0.0046  I  -106.684    1.009   -10.071    0.084  0.163382  0.483150 -0.0908246  -106.715   -10.044  
+22 6 7 59737.00 I  0.166258 0.000020  0.482845 0.000012  I-0.0901458 0.0000062 -0.5429 0.0040  I  -106.522    0.897    -9.941    0.091  0.166198  0.482812 -0.0901686  -106.474    -9.925  
+22 6 8 59738.00 I  0.169362 0.000023  0.482824 0.000024  I-0.0896892 0.0000061 -0.3938 0.0043  I  -106.543    0.925    -9.820    0.077  0.169346  0.482843 -0.0896819  -106.581    -9.834  
+22 6 9 59739.00 I  0.172338 0.000023  0.482864 0.000024  I-0.0893428 0.0000059 -0.2909 0.0041  I  -106.992    0.925    -9.798    0.077  0.172338  0.482895 -0.0893344  -107.056    -9.817  
+22 610 59740.00 I  0.175170 0.000023  0.482876 0.000025  I-0.0890964 0.0000056 -0.2208 0.0041  I  -107.587    0.925    -9.733    0.077  0.175150  0.482907 -0.0890843  -107.652    -9.745  
+22 611 59741.00 I  0.177825 0.000023  0.482631 0.000024  I-0.0888622 0.0000057 -0.2676 0.0040  I  -108.127    0.925    -9.449    0.077  0.177834  0.482720 -0.0888551  -108.201    -9.465  
+22 612 59742.00 I  0.180322 0.000019  0.481995 0.000026  I-0.0885178 0.0000058 -0.4445 0.0040  I  -108.733    0.794    -9.064    0.079  0.180290  0.482016 -0.0885165  -108.809    -9.083  
+22 613 59743.00 I  0.182802 0.000019  0.481220 0.000025  I-0.0879416 0.0000056 -0.7161 0.0039  I  -109.461    0.794    -8.930    0.079  0.182826  0.481258 -0.0879480  -109.531    -8.942  
+22 614 59744.00 I  0.185074 0.000013  0.480362 0.000015  I-0.0870864 0.0000052 -0.9852 0.0039  I  -109.960    0.711    -9.187    0.095  0.185100  0.480403 -0.0870940  -110.036    -9.188  
+22 615 59745.00 I  0.187072 0.000032  0.479278 0.000021  I-0.0859913 0.0000053 -1.1941 0.0037  I  -109.847    0.724    -9.581    0.132  0.187052  0.479331 -0.0859830  -109.873    -9.588  
+22 616 59746.00 I  0.189200 0.000032  0.478013 0.000021  I-0.0847395 0.0000054 -1.2791 0.0037  I  -109.249    0.724    -9.815    0.132  0.189149  0.478024 -0.0847332  -109.222    -9.837  
+22 617 59747.00 I  0.191612 0.000031  0.476718 0.000021  I-0.0834976 0.0000053 -1.1708 0.0043  I  -108.660    0.724    -9.891    0.132  0.191602  0.476728 -0.0834949  -108.594    -9.934  
+22 618 59748.00 I  0.194038 0.000030  0.475540 0.000018  I-0.0824386 0.0000066 -0.9405 0.0048  I  -108.422    0.856    -9.944    0.218  0.194019  0.475550 -0.0824189  -108.365    -9.983  
+22 619 59749.00 I  0.196595 0.000030  0.474520 0.000019  I-0.0815999 0.0000080 -0.7601 0.0042  I  -108.537    0.856    -9.945    0.218  0.196541  0.474534 -0.0815575  -108.509    -9.976  
+22 620 59750.00 I  0.199463 0.000031  0.473569 0.000021  I-0.0808990 0.0000053 -0.6377 0.0047  I  -108.844    0.832    -9.765    0.152  0.199454  0.473574 -0.0808812  -108.836    -9.796  
+22 621 59751.00 I  0.202393 0.000010  0.472817 0.000015  I-0.0803101 0.0000049 -0.5585 0.0034  I  -109.154    0.829    -9.434    0.128  0.202403  0.472799 -0.0803109  -109.153    -9.467  
+22 622 59752.00 I  0.205095 0.000015  0.472245 0.000016  I-0.0797518 0.0000041 -0.5700 0.0032  I  -109.352    0.740    -9.141    0.127  0.205128  0.472282 -0.0797589  -109.347    -9.174  
+22 623 59753.00 I  0.207617 0.000015  0.471609 0.000018  I-0.0791238 0.0000041 -0.7203 0.0030  I  -109.499    0.740    -8.999    0.127  0.207619  0.471645 -0.0791011  -109.587    -9.025  
+22 624 59754.00 I  0.210143 0.000016  0.470762 0.000018  I-0.0783037 0.0000044 -0.8931 0.0030  I  -109.743    0.740    -8.958    0.127  0.210148  0.470821 -0.0782976  -109.961    -8.971  
+22 625 59755.00 I  0.212733 0.000017  0.469694 0.000017  I-0.0773458 0.0000045 -1.0413 0.0028  I  -110.102    0.740    -8.965    0.127  0.212693  0.469719 -0.0773260  -110.305    -8.982  
+22 626 59756.00 I  0.215401 0.000023  0.468440 0.000016  I-0.0761929 0.0000036 -1.2742 0.0029  I  -110.417    0.803    -9.084    0.131  0.215376  0.468485 -0.0761726  -110.571    -9.112  
+22 627 59757.00 I  0.218224 0.000023  0.467032 0.000016  I-0.0748245 0.0000038 -1.4257 0.0031  I  -110.536    0.803    -9.388    0.131  0.218164  0.467038 -0.0748406  -110.659    -9.428  
+22 628 59758.00 I  0.221335 0.000020  0.465586 0.000015  I-0.0733636 0.0000050 -1.5110 0.0032  I  -110.481    0.931    -9.777    0.135  0.221330  0.465623 -0.0733645  -110.576    -9.834  
+22 629 59759.00 I  0.224409 0.000019  0.464145 0.000019  I-0.0718046 0.0000052 -1.5901 0.0036  I  -110.414    0.968   -10.013    0.117  0.224443  0.464165 -0.0718011  -110.473   -10.052  
+22 630 59760.00 I  0.227232 0.000019  0.462593 0.000019  I-0.0702097 0.0000051 -1.5905 0.0036  I  -110.471    0.968    -9.963    0.117  0.227220  0.462671 -0.0702118  -110.474    -9.975  
+22 7 1 59761.00 I  0.230021 0.000019  0.460837 0.000019  I-0.0686589 0.0000050 -1.4850 0.0048  I  -110.676    0.968    -9.743    0.117  0.230002  0.460818 -0.0686663  -110.599    -9.722  
+22 7 2 59762.00 I  0.232938 0.000010  0.459216 0.000018  I-0.0672487 0.0000081 -1.3523 0.0043  I  -110.944    1.033    -9.570    0.071  0.232881  0.459225 -0.0672447  -110.959    -9.582  
+22 7 3 59763.00 I  0.236102 0.000012  0.457821 0.000023  I-0.0659704 0.0000069 -1.1712 0.0052  I  -111.110    0.893    -9.514    0.133  0.236109  0.457809 -0.0659625  -111.150    -9.536  
+22 7 4 59764.00 I  0.239196 0.000012  0.456540 0.000023  I-0.0649346 0.0000066 -0.9052 0.0047  I  -111.057    0.893    -9.471    0.133  0.239234  0.456579 -0.0649159  -111.121    -9.498  
+22 7 5 59765.00 I  0.241897 0.000011  0.455099 0.000019  I-0.0641485 0.0000065 -0.6739 0.0046  I  -110.879    0.840    -9.359    0.162  0.241892  0.455171 -0.0641393  -110.976    -9.390  
+22 7 6 59766.00 I  0.244464 0.000011  0.453300 0.000019  I-0.0635553 0.0000063 -0.5373 0.0045  I  -110.867    0.840    -9.242    0.162  0.244450  0.453302 -0.0635337  -110.950    -9.262  
+22 7 7 59767.00 I  0.247128 0.000010  0.451596 0.000019  I-0.0630527 0.0000061 -0.4643 0.0043  I  -111.239    0.840    -9.217    0.162  0.247124  0.451582 -0.0630501  -111.305    -9.226  
+22 7 8 59768.00 I  0.249750 0.000010  0.450110 0.000019  I-0.0625956 0.0000060 -0.4845 0.0047  I  -111.911    0.840    -9.226    0.162  0.249756  0.450120 -0.0625785  -111.978    -9.228  
+22 7 9 59769.00 I  0.252297 0.000008  0.448647 0.000014  I-0.0620425 0.0000071 -0.6282 0.0039  I  -112.654    0.896    -9.130    0.166  0.252297  0.448682 -0.0620271  -112.723    -9.129  
+22 710 59770.00 I  0.254699 0.000013  0.447025 0.000018  I-0.0613058 0.0000050 -0.8721 0.0042  I  -113.359    0.822    -8.960    0.134  0.254733  0.447060 -0.0612967  -113.423    -8.960  
+22 711 59771.00 I  0.256806 0.000013  0.445406 0.000017  I-0.0602981 0.0000045 -1.1165 0.0034  I  -113.942    0.790    -8.936    0.109  0.256857  0.445395 -0.0603249  -114.007    -8.936  
+22 712 59772.00 I  0.258325 0.000013  0.443901 0.000017  I-0.0591165 0.0000045 -1.2296 0.0034  I  -114.171    0.790    -9.148    0.109  0.258411  0.443974 -0.0591324  -114.246    -9.142  
+22 713 59773.00 I  0.259228 0.000014  0.442021 0.000021  I-0.0578293 0.0000052 -1.3713 0.0034  I  -113.900    0.803    -9.391    0.145  0.259174  0.442066 -0.0577813  -113.960    -9.403  
+22 714 59774.00 I  0.260261 0.000014  0.439922 0.000020  I-0.0564411 0.0000052 -1.3114 0.0036  I  -113.373    0.803    -9.448    0.145  0.260201  0.439888 -0.0564587  -113.418    -9.484  
+22 715 59775.00 I  0.261708 0.000015  0.438116 0.000020  I-0.0552656 0.0000051 -1.0742 0.0041  I  -113.000    0.803    -9.403    0.145  0.261642  0.438122 -0.0552630  -113.037    -9.466  
+22 716 59776.00 I  0.263456 0.000012  0.436344 0.000016  I-0.0542863 0.0000063 -0.8561 0.0033  I  -112.943    0.827    -9.444    0.186  0.263441  0.436373 -0.0542876  -112.983    -9.496  
+22 717 59777.00 I  0.265301 0.000014  0.434374 0.000019  I-0.0535385 0.0000043 -0.6827 0.0038  I  -113.125    0.883    -9.516    0.127  0.265267  0.434398 -0.0535228  -113.161    -9.544  
+22 718 59778.00 I  0.267264 0.000014  0.432333 0.000019  I-0.0528913 0.0000043 -0.5983 0.0027  I  -113.482    0.883    -9.395    0.127  0.267234  0.432352 -0.0528927  -113.506    -9.398  
+22 719 59779.00 I  0.269243 0.000014  0.430273 0.000014  I-0.0523130 0.0000033 -0.6007 0.0027  I  -113.956    0.912    -9.065    0.054  0.269260  0.430298 -0.0523068  -113.947    -9.037  
+22 720 59780.00 I  0.270990 0.000021  0.428191 0.000018  I-0.0516609 0.0000033 -0.6901 0.0025  I  -114.380    0.840    -8.794    0.118  0.270974  0.428173 -0.0516628  -114.393    -8.784  
+22 721 59781.00 I  0.272571 0.000021  0.426252 0.000018  I-0.0509183 0.0000038 -0.8231 0.0026  I  -114.630    0.840    -8.792    0.118  0.272574  0.426255 -0.0508922  -114.674    -8.805  
+22 722 59782.00 I  0.274107 0.000021  0.424447 0.000020  I-0.0499892 0.0000040 -1.0327 0.0035  I  -114.800    0.840    -8.983    0.118  0.274053  0.424453 -0.0499591  -114.884    -9.018  
+22 723 59783.00 I  0.275666 0.000020  0.422672 0.000017  I-0.0488704 0.0000059 -1.1897 0.0032  I  -115.041    0.700    -9.172    0.168  0.275681  0.422673 -0.0488673  -115.096    -9.210  
+22 724 59784.00 I  0.277059 0.000021  0.420908 0.000019  I-0.0476108 0.0000051 -1.3437 0.0039  I  -115.320    0.796    -9.305    0.174  0.277006  0.420915 -0.0476028  -115.333    -9.343  
+22 725 59785.00 I  0.278490 0.000021  0.419330 0.000020  I-0.0461984 0.0000050 -1.4516 0.0046  I  -115.476    0.796    -9.475    0.174  0.278471  0.419285 -0.0462003  -115.452    -9.519  
+22 726 59786.00 I  0.279859 0.000014  0.417883 0.000018  I-0.0447451 0.0000076 -1.4469 0.0059  I  -115.461    0.890    -9.715    0.183  0.279867  0.417962 -0.0447491  -115.399    -9.768  
+22 727 59787.00 I  0.281078 0.000026  0.416122 0.000028  I-0.0433061 0.0000106 -1.4375 0.0066  I  -115.394    0.849    -9.887    0.173  0.281044  0.416126 -0.0432579  -115.379    -9.934  
+22 728 59788.00 I  0.282272 0.000025  0.414137 0.000027  I-0.0418627 0.0000107 -1.4503 0.0075  I  -115.385    0.849    -9.833    0.173  0.282267  0.414205 -0.0417953  -115.431    -9.867  
+22 729 59789.00 I  0.283375 0.000024  0.411830 0.000026  I-0.0404400 0.0000107 -1.3596 0.0100  I  -115.427    0.849    -9.579    0.173  0.283345  0.411841 -0.0404282  -115.538    -9.595  
+22 730 59790.00 I  0.284628 0.000023  0.409435 0.000025  I-0.0391963 0.0000169 -1.1107 0.0072  I  -115.457    0.690    -9.324    0.148  0.284587  0.409400 -0.0392089  -115.593    -9.353  
+22 731 59791.00 I  0.285992 0.000026  0.407276 0.000028  I-0.0381992 0.0000096 -0.9202 0.0097  I  -115.440    0.794    -9.221    0.270  0.286000  0.407286 -0.0381849  -115.593    -9.273  
+22 8 1 59792.00 I  0.287135 0.000027  0.405203 0.000027  I-0.0373594 0.0000097 -0.7192 0.0059  I  -115.364    0.794    -9.245    0.270  0.287161  0.405194 -0.0373892  -115.536    -9.320  
+22 8 2 59793.00 I  0.287890 0.000020  0.403213 0.000017  I-0.0367585 0.0000070 -0.5250 0.0059  I  -115.255    0.777    -9.273    0.270  0.287882  0.403262 -0.0367846  -115.439    -9.376  
+22 8 3 59794.00 I  0.288549 0.000020  0.401001 0.000017  I-0.0362692 0.0000067 -0.4514 0.0047  I  -115.232    0.777    -9.242    0.270  0.288468  0.401019 -0.0362792  -115.414    -9.314  
+22 8 4 59795.00 I  0.289531 0.000020  0.398714 0.000017  I-0.0358253 0.0000064 -0.4689 0.0046  I  -115.467    0.777    -9.189    0.270  0.289489  0.398709 -0.0358145  -115.635    -9.222  
+22 8 5 59796.00 I  0.290542 0.000020  0.396548 0.000017  I-0.0353196 0.0000062 -0.5217 0.0050  I  -116.021    0.777    -9.161    0.270  0.290582  0.396579 -0.0353263  -116.154    -9.192  
+22 8 6 59797.00 I  0.291098 0.000016  0.394193 0.000009  I-0.0347527 0.0000077 -0.6623 0.0040  I  -116.749    0.733    -9.162    0.243  0.291080  0.394221 -0.0347316  -116.838    -9.204  
+22 8 7 59798.00 I  0.291552 0.000019  0.391644 0.000010  I-0.0339656 0.0000050 -0.8913 0.0046  I  -117.388    0.717    -9.208    0.248  0.291487  0.391652 -0.0339451  -117.435    -9.261  
+22 8 8 59799.00 I  0.292342 0.000016  0.389019 0.000009  I-0.0329945 0.0000049 -1.0470 0.0035  I  -117.700    0.702    -9.340    0.252  0.292293  0.389056 -0.0329721  -117.715    -9.399  
+22 8 9 59800.00 I  0.293213 0.000016  0.386208 0.000009  I-0.0319006 0.0000050 -1.1158 0.0033  I  -117.585    0.702    -9.505    0.252  0.293211  0.386232 -0.0318918  -117.585    -9.565  
+22 810 59801.00 I  0.293839 0.000016  0.383248 0.000011  I-0.0308127 0.0000045 -1.0353 0.0033  I  -117.182    0.761    -9.530    0.262  0.293803  0.383250 -0.0308088  -117.149    -9.591  
+22 811 59802.00 I  0.294456 0.000016  0.380335 0.000012  I-0.0298665 0.0000044 -0.8452 0.0032  I  -116.828    0.761    -9.336    0.262  0.294459  0.380298 -0.0298577  -116.770    -9.397  
+22 812 59803.00 I  0.295064 0.000016  0.377810 0.000012  I-0.0291372 0.0000045 -0.6102 0.0036  I  -116.757    0.761    -9.104    0.262  0.295055  0.377755 -0.0291384  -116.681    -9.171  
+22 813 59804.00 I  0.295584 0.000012  0.375705 0.000012  I-0.0286394 0.0000057 -0.3952 0.0035  I  -116.881    0.797    -9.073    0.271  0.295537  0.375740 -0.0286307  -116.834    -9.134  
+22 814 59805.00 I  0.296377 0.000010  0.373564 0.000012  I-0.0283070 0.0000053 -0.2996 0.0036  I  -117.013    0.797    -9.207    0.271  0.296313  0.373591 -0.0282983  -117.006    -9.266  
+22 815 59806.00 I  0.297516 0.000012  0.371303 0.000013  I-0.0279976 0.0000045 -0.3317 0.0040  I  -117.181    0.796    -9.239    0.223  0.297500  0.371314 -0.0279699  -117.203    -9.307  
+22 816 59807.00 I  0.298555 0.000013  0.369040 0.000011  I-0.0276144 0.0000061 -0.4514 0.0044  I  -117.524    0.793    -9.053    0.117  0.298583  0.369059 -0.0276395  -117.555    -9.139  
+22 817 59808.00 I  0.299280 0.000016  0.366732 0.000016  I-0.0270829 0.0000075 -0.6069 0.0048  I  -117.986    0.774    -8.840    0.120  0.299254  0.366732 -0.0270866  -118.003    -8.949  
+22 818 59809.00 I  0.299914 0.000017  0.364397 0.000018  I-0.0263646 0.0000074 -0.8704 0.0052  I  -118.355    0.774    -8.825    0.120  0.299866  0.364425 -0.0263517  -118.274    -8.865  
+22 819 59810.00 I  0.300906 0.000017  0.362019 0.000017  I-0.0253590 0.0000073 -1.0832 0.0054  I  -118.546    0.774    -8.990    0.120  0.300823  0.362010 -0.0253455  -118.335    -8.928  
+22 820 59811.00 I  0.302130 0.000017  0.359755 0.000017  I-0.0242070 0.0000078 -1.2698 0.0051  I  -118.649    0.774    -9.143    0.120  0.302176  0.359779 -0.0241871  -118.439    -9.105  
+22 821 59812.00 I  0.303014 0.000019  0.357415 0.000023  I-0.0228341 0.0000072 -1.4125 0.0052  I  -118.719    0.629    -9.176    0.108  0.302992  0.357455 -0.0228266  -118.572    -9.196  
+22 822 59813.00 I  0.303772 0.000018  0.354935 0.000023  I-0.0214226 0.0000069 -1.4335 0.0048  I  -118.688    0.629    -9.181    0.108  0.303769  0.354926 -0.0213929  -118.632    -9.243  
+22 823 59814.00 I  0.304490 0.000016  0.352461 0.000021  I-0.0199983 0.0000062 -1.3608 0.0046  I  -118.519    0.630    -9.278    0.105  0.304513  0.352500 -0.0199836  -118.587    -9.375  
+22 824 59815.00 I  0.304892 0.000016  0.349908 0.000022  I-0.0187092 0.0000061 -1.2635 0.0043  I  -118.290    0.729    -9.431    0.129  0.304896  0.349874 -0.0186613  -118.307    -9.531  
+22 825 59816.00 I  0.305189 0.000015  0.347446 0.000022  I-0.0174493 0.0000060 -1.2324 0.0042  I  -118.094    0.729    -9.481    0.129  0.305201  0.347486 -0.0174037  -118.023    -9.577  
+22 826 59817.00 I  0.305358 0.000015  0.344908 0.000022  I-0.0162919 0.0000058 -1.0590 0.0046  I  -117.933    0.729    -9.342    0.129  0.305398  0.344912 -0.0162851  -117.767    -9.438  
+22 827 59818.00 I  0.305274 0.000009  0.342344 0.000015  I-0.0153533 0.0000071 -0.8196 0.0040  I  -117.784    0.910    -9.110    0.154  0.305290  0.342335 -0.0153482  -117.637    -9.193  
+22 828 59819.00 I  0.304971 0.000017  0.339907 0.000018  I-0.0146448 0.0000054 -0.6038 0.0044  I  -117.668    0.791    -8.966    0.172  0.304974  0.339946 -0.0146136  -117.565    -9.035  
+22 829 59820.00 I  0.304629 0.000017  0.337395 0.000017  I-0.0141332 0.0000053 -0.4255 0.0037  I  -117.628    0.791    -8.993    0.172  0.304586  0.337401 -0.0140968  -117.551    -9.055  
+22 830 59821.00 I  0.304501 0.000017  0.334972 0.000014  I-0.0137961 0.0000051 -0.2404 0.0034  I  -117.644    0.734    -9.116    0.185  0.304464  0.334971 -0.0137838  -117.601    -9.176  
+22 831 59822.00 I  0.304621 0.000019  0.332730 0.000016  I-0.0136234 0.0000044 -0.1423 0.0033  I  -117.672    0.763    -9.197    0.158  0.304595  0.332751 -0.0136099  -117.612    -9.248  
+22 9 1 59823.00 I  0.304755 0.000019  0.330377 0.000017  I-0.0134673 0.0000043 -0.1770 0.0031  I  -117.772    0.763    -9.171    0.158  0.304814  0.330440 -0.0134836  -117.693    -9.211  
+22 9 2 59824.00 I  0.304509 0.000019  0.327657 0.000016  I-0.0132476 0.0000044 -0.2773 0.0031  I  -118.057    0.763    -9.090    0.158  0.304501  0.327651 -0.0132494  -118.154    -9.102  
+22 9 3 59825.00 I  0.304214 0.000012  0.325048 0.000012  I-0.0128977 0.0000045 -0.4225 0.0043  I  -118.505    0.793    -9.056    0.126  0.304186  0.324993 -0.0128821  -118.590    -9.080  
+22 9 4 59826.00 I  0.304090 0.000015  0.322753 0.000019  I-0.0123927 0.0000075 -0.5974 0.0044  I  -118.869    0.767    -9.128    0.186  0.304085  0.322764 -0.0123741  -118.929    -9.170  
+22 9 5 59827.00 I  0.303791 0.000015  0.320459 0.000019  I-0.0117197 0.0000076 -0.7219 0.0070  I  -118.870    0.767    -9.268    0.186  0.303820  0.320481 -0.0117203  -118.916    -9.328  
+22 9 6 59828.00 I  0.303230 0.000013  0.317934 0.000017  I-0.0110135 0.0000119 -0.6525 0.0063  I  -118.464    0.736    -9.336    0.239  0.303248  0.318029 -0.0110190  -118.525    -9.426  
+22 9 7 59829.00 I  0.302624 0.000016  0.314928 0.000017  I-0.0104287 0.0000101 -0.5412 0.0079  I  -117.909    0.902    -9.187    0.182  0.302652  0.314951 -0.0103738  -117.930    -9.248  
+22 9 8 59830.00 I  0.301728 0.000017  0.311763 0.000017  I-0.0099631 0.0000103 -0.3339 0.0071  I  -117.578    0.902    -8.831    0.182  0.301793  0.311758 -0.0099952  -117.557    -8.853  
+22 9 9 59831.00 I  0.300348 0.000018  0.308679 0.000019  I-0.0097985 0.0000100 -0.0136 0.0060  I  -117.609    0.902    -8.482    0.182  0.300297  0.308670 -0.0098037  -117.537    -8.461  
+22 910 59832.00 I  0.299165 0.000015  0.305664 0.000012  I-0.0099088 0.0000063  0.2256 0.0054  I  -117.803    1.169    -8.368    0.061  0.299086  0.305665 -0.0098938  -117.785    -8.354  
+22 911 59833.00 I  0.298576 0.000021  0.302848 0.000016  I-0.0102096 0.0000042  0.3446 0.0038  I  -117.903    1.020    -8.492    0.134  0.298524  0.302843 -0.0101991  -117.949    -8.495  
+22 912 59834.00 I  0.298133 0.000021  0.300269 0.000016  I-0.0105617 0.0000042  0.3547 0.0031  I  -117.916    1.020    -8.649    0.134  0.298153  0.300265 -0.0105663  -118.003    -8.665  
+22 913 59835.00 I  0.297557 0.000020  0.297911 0.000018  I-0.0108727 0.0000046  0.2258 0.0028  I  -118.053    0.948    -8.689    0.168  0.297509  0.297897 -0.0108687  -118.179    -8.722  
+22 914 59836.00 I  0.296983 0.000019  0.295809 0.000030  I-0.0109906 0.0000037  0.0287 0.0029  I  -118.387    0.944    -8.666    0.128  0.296992  0.295809 -0.0110048  -118.515    -8.694  
+22 915 59837.00 I  0.296339 0.000019  0.293806 0.000030  I-0.0109060 0.0000036 -0.2408 0.0025  I  -118.744    0.944    -8.713    0.128  0.296326  0.293853 -0.0109071  -118.881    -8.735  
+22 916 59838.00 I  0.295612 0.000019  0.291683 0.000030  I-0.0105264 0.0000035 -0.4582 0.0026  I  -118.909    0.944    -8.829    0.128  0.295633  0.291666 -0.0105453  -119.064    -8.840  
+22 917 59839.00 I  0.294748 0.000012  0.289618 0.000028  I-0.0100028 0.0000038 -0.6360 0.0023  I  -118.821    0.940    -8.887    0.066  0.294765  0.289613 -0.0099966  -118.954    -8.905  
+22 918 59840.00 I  0.293581 0.000016  0.287785 0.000035  I-0.0092599 0.0000030 -0.7974 0.0024  I  -118.549    1.013    -8.820    0.112  0.293594  0.287789 -0.0092502  -118.640    -8.844  
+22 919 59841.00 I  0.292289 0.000016  0.285838 0.000035  I-0.0084479 0.0000030 -0.8392 0.0023  I  -118.184    1.013    -8.718    0.112  0.292235  0.285928 -0.0084134  -118.223    -8.750  
+22 920 59842.00 I  0.291359 0.000016  0.283510 0.000025  I-0.0075723 0.0000034 -0.9086 0.0025  I  -117.809    1.083    -8.720    0.142  0.291284  0.283515 -0.0075559  -117.778    -8.771  
+22 921 59843.00 I  0.290662 0.000017  0.281046 0.000026  I-0.0066831 0.0000039 -0.8208 0.0025  I  -117.517    0.985    -8.832    0.110  0.290675  0.281089 -0.0066950  -117.531    -8.864  
+22 922 59844.00 I  0.289766 0.000017  0.278366 0.000026  I-0.0059712 0.0000038 -0.6115 0.0027  I  -117.360    0.985    -8.918    0.110  0.289785  0.278400 -0.0059969  -117.441    -8.921  
+22 923 59845.00 I  0.288628 0.000016  0.275546 0.000025  I-0.0054467 0.0000037 -0.4424 0.0034  I  -117.313    0.985    -8.846    0.110  0.288673  0.275532 -0.0054471  -117.457    -8.810  
+22 924 59846.00 I  0.287265 0.000013  0.272931 0.000013  I-0.0051007 0.0000057 -0.2305 0.0032  I  -117.309    0.778    -8.639    0.031  0.287244  0.272949 -0.0051006  -117.468    -8.622  
+22 925 59847.00 I  0.285955 0.000024  0.270425 0.000021  I-0.0049719 0.0000052 -0.0601 0.0039  I  -117.325    0.735    -8.445    0.179  0.285878  0.270404 -0.0049635  -117.484    -8.457  
+22 926 59848.00 I  0.285171 0.000025  0.268170 0.000021  I-0.0049632 0.0000052  0.0585 0.0039  I  -117.377    0.735    -8.400    0.179  0.285103  0.268121 -0.0049793  -117.537    -8.441  
+22 927 59849.00 I  0.284714 0.000024  0.266406 0.000019  I-0.0050980 0.0000058  0.2045 0.0036  I  -117.461    0.709    -8.507    0.241  0.284746  0.266357 -0.0051012  -117.616    -8.597  
+22 928 59850.00 I  0.283882 0.000024  0.264921 0.000024  I-0.0053121 0.0000051  0.1702 0.0039  I  -117.555    0.637    -8.640    0.172  0.283878  0.264953 -0.0053014  -117.693    -8.702  
+22 929 59851.00 I  0.283012 0.000024  0.263300 0.000024  I-0.0053977 0.0000052  0.0136 0.0037  I  -117.653    0.637    -8.679    0.172  0.282943  0.263319 -0.0054180  -117.779    -8.707  
+22 930 59852.00 I  0.282326 0.000024  0.261505 0.000024  I-0.0053345 0.0000053 -0.1576 0.0039  I  -117.766    0.637    -8.611    0.172  0.282338  0.261528 -0.0053388  -117.905    -8.603  
+2210 1 59853.00 I  0.281366 0.000013  0.259742 0.000019  I-0.0050587 0.0000058 -0.4002 0.0039  I  -117.845    0.521    -8.523    0.032  0.281388  0.259744 -0.0049041  -117.934    -8.536  
+2210 2 59854.00 I  0.280048 0.000010  0.257878 0.000019  I-0.0045731 0.0000058 -0.5259 0.0042  I  -117.762    0.521    -8.501    0.032  0.280092  0.257931 -0.0043864  -117.763    -8.633  
+2210 3 59855.00 I  0.278455 0.000015  0.255734 0.000023  I-0.0040579 0.0000060 -0.4984 0.0049  I  -117.401    0.890    -8.545    0.116  0.278478  0.255746 -0.0040146  -117.380    -8.681  
+2210 4 59856.00 I  0.276552 0.000014  0.253523 0.000019  I-0.0035908 0.0000079 -0.4272 0.0044  I  -116.804    1.107    -8.566    0.160  0.276607  0.253527 -0.0035590  -116.777    -8.672  
+2210 5 59857.00 I  0.274397 0.000015  0.251421 0.000021  I-0.0032304 0.0000065 -0.2754 0.0051  I  -116.203    1.059    -8.465    0.135  0.274352  0.251450 -0.0032281  -116.158    -8.550  
+2210 6 59858.00 I  0.272450 0.000019  0.249219 0.000021  I-0.0030723 0.0000065 -0.0268 0.0047  I  -115.867    1.059    -8.233    0.135  0.272409  0.249284 -0.0030816  -115.892    -8.306  
+2210 7 59859.00 I  0.270895 0.000021  0.246711 0.000019  I-0.0031837 0.0000067  0.2425 0.0047  I  -115.870    1.059    -7.977    0.135  0.270869  0.246728 -0.0031810  -115.963    -8.047  
+2210 8 59860.00 I  0.269396 0.000021  0.244287 0.000019  I-0.0035469 0.0000068  0.4805 0.0047  I  -116.052    1.059    -7.818    0.135  0.269464  0.244272 -0.0035337  -116.181    -7.889  
+2210 9 59861.00 I  0.267409 0.000018  0.242142 0.000015  I-0.0041015 0.0000067  0.5889 0.0044  I  -116.183    1.018    -7.779    0.108  0.267436  0.242181 -0.0040628  -116.323    -7.852  
+221010 59862.00 I  0.265331 0.000019  0.239992 0.000020  I-0.0046811 0.0000055  0.5667 0.0043  I  -116.191    0.884    -7.797    0.085  0.265240  0.239987 -0.0046541  -116.330    -7.871  
+221011 59863.00 I  0.263673 0.000019  0.237866 0.000019  I-0.0051948 0.0000053  0.4244 0.0036  I  -116.203    0.749    -7.823    0.053  0.263701  0.237885 -0.0051692  -116.344    -7.899  
+221012 59864.00 I  0.262033 0.000019  0.235719 0.000023  I-0.0055021 0.0000046  0.1986 0.0035  I  -116.357    0.792    -7.871    0.042  0.262046  0.235701 -0.0055011  -116.517    -7.950  
+221013 59865.00 I  0.259885 0.000017  0.233783 0.000024  I-0.0055864 0.0000047 -0.0441 0.0035  I  -116.612    0.792    -7.958    0.042  0.260021  0.233734 -0.0055722  -116.707    -8.023  
+221014 59866.00 I  0.256989 0.000016  0.232073 0.000024  I-0.0054360 0.0000052 -0.2206 0.0035  I  -116.772    0.792    -8.038    0.042  0.256936  0.232102 -0.0054362  -116.793    -8.078  
+221015 59867.00 I  0.254063 0.000016  0.230370 0.000023  I-0.0051908 0.0000053 -0.2602 0.0043  I  -116.664    0.792    -8.034    0.042  0.254063  0.230356 -0.0051876  -116.700    -8.075  
+221016 59868.00 I  0.251196 0.000020  0.228841 0.000020  I-0.0049213 0.0000068 -0.2828 0.0043  I  -116.279    0.908    -7.944    0.068  0.251206  0.228893 -0.0049099  -116.365    -7.987  
+221017 59869.00 I  0.248071 0.000023  0.227220 0.000020  I-0.0046630 0.0000067 -0.1922 0.0054  I  -115.749    0.908    -7.873    0.068  0.248052  0.227286 -0.0046783  -115.804    -7.935  
+221018 59870.00 I  0.245193 0.000020  0.225121 0.000017  I-0.0045608 0.0000083 -0.0300 0.0049  I  -115.215    0.940    -7.924    0.089  0.245102  0.225158 -0.0045660  -115.200    -8.015  
+221019 59871.00 I  0.243020 0.000021  0.222953 0.000022  I-0.0045919 0.0000071  0.0990 0.0053  I  -114.759    0.998    -8.073    0.125  0.243041  0.222898 -0.0045814  -114.747    -8.164  
+221020 59872.00 I  0.240709 0.000021  0.221142 0.000022  I-0.0047752 0.0000067  0.2771 0.0048  I  -114.447    0.998    -8.178    0.125  0.240817  0.221191 -0.0047645  -114.446    -8.265  
+221021 59873.00 I  0.237722 0.000022  0.219301 0.000023  I-0.0051504 0.0000065  0.4679 0.0047  I  -114.358    0.998    -8.106    0.125  0.237688  0.219313 -0.0051434  -114.344    -8.197  
+221022 59874.00 I  0.234659 0.000019  0.217534 0.000022  I-0.0057184 0.0000065  0.6809 0.0040  I  -114.523    1.057    -7.850    0.157  0.234606  0.217522 -0.0057243  -114.532    -7.927  
+221023 59875.00 I  0.232023 0.000015  0.216031 0.000026  I-0.0065133 0.0000047  0.8972 0.0040  I  -114.839    0.908    -7.528    0.131  0.231878  0.216031 -0.0064986  -114.866    -7.589  
+221024 59876.00 I  0.230037 0.000016  0.214643 0.000025  I-0.0074632 0.0000048  0.9646 0.0032  I  -115.122    0.908    -7.289    0.131  0.230043  0.214645 -0.0074339  -115.163    -7.341  
+221025 59877.00 I  0.228140 0.000015  0.213201 0.000020  I-0.0084004 0.0000044  0.9057 0.0032  I  -115.256    0.751    -7.220    0.082  0.228137  0.213232 -0.0084121  -115.318    -7.265  
+221026 59878.00 I  0.226083 0.000014  0.211771 0.000020  I-0.0092475 0.0000043  0.7656 0.0030  I  -115.253    0.751    -7.313    0.082  0.226115  0.211747 -0.0092591  -115.297    -7.349  
+221027 59879.00 I  0.223702 0.000014  0.210371 0.000020  I-0.0098839 0.0000042  0.4825 0.0028  I  -115.193    0.751    -7.474    0.082  0.223756  0.210409 -0.0098856  -115.222    -7.492  
+221028 59880.00 I  0.220833 0.000011  0.208850 0.000019  I-0.0102145 0.0000035  0.2054 0.0034  I  -115.115    0.751    -7.589    0.082  0.220823  0.208832 -0.0102779  -115.143    -7.612  
+221029 59881.00 I  0.217717 0.000012  0.207410 0.000013  I-0.0103324 0.0000054  0.0415 0.0032  I  -114.988    0.760    -7.598    0.042  0.217709  0.207418 -0.0103958  -115.022    -7.628  
+221030 59882.00 I  0.214515 0.000016  0.206260 0.000019  I-0.0103082 0.0000054 -0.0904 0.0042  I  -114.767    0.791    -7.544    0.161  0.214473  0.206229 -0.0103095  -114.810    -7.575  
+221031 59883.00 I  0.211397 0.000015  0.205208 0.000020  I-0.0101956 0.0000065 -0.0902 0.0043  I  -114.441    0.816    -7.504    0.220  0.211345  0.205237 -0.0101927  -114.492    -7.538  
+2211 1 59884.00 I  0.208610 0.000016  0.204241 0.000022  I-0.0101886 0.0000066  0.0923 0.0044  I  -114.046    0.816    -7.497    0.220  0.208514  0.204211 -0.0101774  -114.100    -7.544  
+2211 2 59885.00 I  0.206235 0.000019  0.203455 0.000026  I-0.0104116 0.0000060  0.3690 0.0045  I  -113.659    0.841    -7.471    0.185  0.206235  0.203545 -0.0104065  -113.700    -7.501  
+2211 3 59886.00 I  0.203880 0.000020  0.202379 0.000026  I-0.0109480 0.0000061  0.7100 0.0042  I  -113.381    0.841    -7.381    0.185  0.203841  0.202359 -0.0109528  -113.392    -7.399  
+2211 4 59887.00 I  0.201543 0.000020  0.201375 0.000026  I-0.0118061 0.0000060  0.9745 0.0047  I  -113.287    0.841    -7.231    0.185  0.201477  0.201353 -0.0118134  -113.257    -7.249  
+2211 5 59888.00 I  0.199502 0.000016  0.200669 0.000022  I-0.0128248 0.0000072  1.0224 0.0045  I  -113.379    0.866    -7.048    0.136  0.199403  0.200700 -0.0128173  -113.353    -7.066  
+2211 6 59889.00 I  0.197927 0.000017  0.199802 0.000022  I-0.0138160 0.0000066  0.9655 0.0050  I  -113.548    0.748    -6.852    0.090  0.197880  0.199789 -0.0138349  -113.543    -6.869  
+2211 7 59890.00 I  0.196420 0.000018  0.199011 0.000020  I-0.0147308 0.0000070  0.8336 0.0050  I  -113.644    0.748    -6.672    0.090  0.196436  0.198985 -0.0147274  -113.659    -6.688  
+2211 8 59891.00 I  0.194602 0.000024  0.198362 0.000021  I-0.0154493 0.0000076  0.6001 0.0051  I  -113.614    0.673    -6.575    0.019  0.194574  0.198424 -0.0154466  -113.660    -6.582  
+2211 9 59892.00 I  0.192640 0.000023  0.197576 0.000021  I-0.0159464 0.0000073  0.4127 0.0052  I  -113.553    0.673    -6.618    0.019  0.192696  0.197558 -0.0159684  -113.571    -6.657  
+221110 59893.00 I  0.190363 0.000023  0.196714 0.000021  I-0.0162480 0.0000072  0.1452 0.0050  I  -113.574    0.673    -6.776    0.019  0.190367  0.196722 -0.0162302  -113.564    -6.849  
+221111 59894.00 I  0.187848 0.000023  0.195889 0.000021  I-0.0162361 0.0000068 -0.1242 0.0055  I  -113.642    0.673    -6.934    0.019  0.187822  0.195880 -0.0162520  -113.631    -7.013  
+221112 59895.00 I  0.185423 0.000022  0.195026 0.000020  I-0.0160519 0.0000083 -0.2366 0.0041  I  -113.592    0.758    -6.983    0.004  0.185361  0.195076 -0.0160839  -113.596    -7.056  
+221113 59896.00 I  0.183325 0.000021  0.193955 0.000021  I-0.0157871 0.0000047 -0.2765 0.0045  I  -113.331    0.727    -6.939    0.076  0.183217  0.193981 -0.0158151  -113.352    -6.999  
+221114 59897.00 I  0.181912 0.000009  0.192840 0.000013  I-0.0155279 0.0000035 -0.2294 0.0030  I  -112.927    0.725    -6.915    0.083  0.181786  0.192794 -0.0155444  -112.967    -6.958  
+221115 59898.00 I  0.181152 0.000010  0.192227 0.000013  I-0.0153542 0.0000037 -0.1046 0.0028  I  -112.493    0.725    -6.982    0.083  0.181089  0.192167 -0.0153549  -112.549    -7.008  
+221116 59899.00 I  0.180595 0.000012  0.192102 0.000014  I-0.0153305 0.0000043  0.0556 0.0029  I  -112.072    0.751    -7.073    0.121  0.180613  0.192084 -0.0153236  -112.120    -7.099  
+221117 59900.00 I  0.179834 0.000012  0.192250 0.000015  I-0.0154805 0.0000045  0.2612 0.0032  I  -111.711    0.751    -7.060    0.121  0.179894  0.192217 -0.0154871  -111.735    -7.093  
+221118 59901.00 I  0.178497 0.000012  0.192634 0.000014  I-0.0158586 0.0000047  0.4840 0.0042  I  -111.567    0.751    -6.891    0.121  0.178587  0.192658 -0.0158559  -111.559    -6.936  
+221119 59902.00 I  0.176654 0.000011  0.192919 0.000011  I-0.0164176 0.0000071  0.6141 0.0033  I  -111.790    0.786    -6.630    0.153  0.176631  0.192939 -0.0164100  -111.782    -6.671  
+221120 59903.00 I  0.174680 0.000013  0.192880 0.000014  I-0.0170916 0.0000045  0.7587 0.0042  I  -112.284    0.712    -6.365    0.137  0.174678  0.192941 -0.0171134  -112.283    -6.399  
+221121 59904.00 I  0.172511 0.000013  0.192693 0.000015  I-0.0179071 0.0000045  0.8197 0.0030  I  -112.743    0.712    -6.131    0.137  0.172482  0.192686 -0.0178985  -112.747    -6.164  
+221122 59905.00 I  0.170168 0.000012  0.192494 0.000013  I-0.0186682 0.0000041  0.6922 0.0037  I  -112.971    0.659    -5.965    0.123  0.170135  0.192562 -0.0186627  -112.985    -5.999  
+221123 59906.00 I  0.167918 0.000019  0.192107 0.000019  I-0.0192774 0.0000058  0.5225 0.0036  I  -113.014    0.659    -5.954    0.115  0.167864  0.192125 -0.0192839  -113.015    -5.992  
+221124 59907.00 I  0.165803 0.000019  0.191654 0.000019  I-0.0196856 0.0000059  0.2701 0.0042  I  -112.967    0.659    -6.135    0.115  0.165815  0.191634 -0.0196773  -112.960    -6.178  
+221125 59908.00 I  0.163389 0.000019  0.191387 0.000019  I-0.0198163 0.0000060  0.0137 0.0054  I  -112.806    0.659    -6.371    0.115  0.163449  0.191394 -0.0198119  -112.800    -6.422  
+221126 59909.00 I  0.160415 0.000019  0.191126 0.000017  I-0.0197375 0.0000090 -0.1691 0.0053  I  -112.507    0.658    -6.453    0.106  0.160439  0.191188 -0.0197408  -112.502    -6.504  
+221127 59910.00 I  0.156941 0.000019  0.190778 0.000017  I-0.0195128 0.0000087 -0.2476 0.0058  I  -112.182    0.658    -6.343    0.106  0.156985  0.190819 -0.0195486  -112.173    -6.392  
+221128 59911.00 I  0.153238 0.000019  0.190257 0.000019  I-0.0192988 0.0000073 -0.1564 0.0055  I  -111.955    0.742    -6.202    0.081  0.153168  0.190278 -0.0193141  -111.939    -6.246  
+221129 59912.00 I  0.149946 0.000013  0.189796 0.000013  I-0.0192254 0.0000067  0.0111 0.0045  I  -111.824    0.839    -6.164    0.046  0.149881  0.189736 -0.0192085  -111.789    -6.198  
+221130 59913.00 I  0.147027 0.000018  0.189823 0.000015  I-0.0193201 0.0000051  0.1759 0.0041  I  -111.720    0.764    -6.188    0.089  0.146998  0.189837 -0.0193120  -111.648    -6.204  
+2212 1 59914.00 I  0.144060 0.000022  0.190071 0.000017  I-0.0195901 0.0000048  0.3794 0.0035  I  -111.632    0.764    -6.161    0.089  0.144039  0.190129 -0.0196037  -111.563    -6.191  
+2212 2 59915.00 I  0.141129 0.000022  0.189946 0.000024  I-0.0200305 0.0000048  0.4376 0.0034  I  -111.593    0.764    -6.054    0.089  0.141086  0.190030 -0.0200182  -111.557    -6.103  
+2212 3 59916.00 I  0.138505 0.000022  0.189639 0.000031  I-0.0204348 0.0000048  0.4041 0.0030  I  -111.622    0.764    -5.907    0.089  0.138520  0.189588 -0.0204483  -111.593    -5.954  
+2212 4 59917.00 I  0.135675 0.000023  0.189528 0.000036  I-0.0208205 0.0000036  0.3160 0.0031  I  -111.706    0.830    -5.747    0.126  0.135739  0.189603 -0.0208072  -111.696    -5.787  
+2212 5 59918.00 I  0.132723 0.000024  0.189100 0.000036  I-0.0210293 0.0000038  0.1156 0.0025  I  -111.753    0.830    -5.586    0.126  0.132595  0.189132 -0.0210271  -111.763    -5.625  
+2212 6 59919.00 I  0.130246 0.000022  0.188802 0.000035  I-0.0210510 0.0000036 -0.0867 0.0028  I  -111.665    1.001    -5.485    0.137  0.130234  0.188807 -0.0210546  -111.664    -5.528  
+2212 7 59920.00 I  0.127866 0.000020  0.188820 0.000035  I-0.0208534 0.0000042 -0.2963 0.0028  I  -111.490    0.851    -5.532    0.107  0.127804  0.188914 -0.0208636  -111.530    -5.568  
+2212 8 59921.00 I  0.125547 0.000018  0.188717 0.000030  I-0.0204783 0.0000043 -0.4460 0.0031  I  -111.370    0.851    -5.742    0.107  0.125550  0.188683 -0.0204842  -111.431    -5.765  
+2212 9 59922.00 I  0.123016 0.000018  0.188896 0.000023  I-0.0199702 0.0000045 -0.5693 0.0037  I  -111.374    0.851    -5.994    0.107  0.123051  0.188943 -0.0199575  -111.450    -5.997  
+221210 59923.00 I  0.120048 0.000017  0.189242 0.000012  I-0.0193536 0.0000061 -0.6509 0.0036  I  -111.408    0.691    -6.137    0.065  0.120023  0.189212 -0.0193465  -111.433    -6.148  
+221211 59924.00 I  0.117122 0.000020  0.189431 0.000013  I-0.0186972 0.0000056 -0.6462 0.0041  I  -111.334    0.700    -6.146    0.153  0.117059  0.189519 -0.0187186  -111.306    -6.171  
+221212 59925.00 I  0.114545 0.000019  0.189330 0.000015  I-0.0180980 0.0000056 -0.5311 0.0036  I  -111.110    0.700    -6.128    0.153  0.114474  0.189311 -0.0181257  -111.063    -6.164  
+221213 59926.00 I  0.112260 0.000018  0.189372 0.000017  I-0.0176364 0.0000045 -0.4120 0.0036  I  -110.769    0.821    -6.163    0.188  0.112235  0.189380 -0.0176371  -110.733    -6.213  
+221214 59927.00 I  0.110090 0.000018  0.189777 0.000016  I-0.0172825 0.0000044 -0.2676 0.0031  I  -110.332    0.821    -6.182    0.188  0.110057  0.189733 -0.0172887  -110.324    -6.215  
+221215 59928.00 I  0.107807 0.000018  0.190623 0.000016  I-0.0171064 0.0000042 -0.1076 0.0030  I  -109.866    0.821    -6.067    0.188  0.107848  0.190644 -0.0170929  -109.882    -6.084  
+221216 59929.00 I  0.105278 0.000018  0.191573 0.000016  I-0.0170801 0.0000041  0.0907 0.0029  I  -109.592    0.821    -5.836    0.188  0.105276  0.191662 -0.0170407  -109.642    -5.845  
+221217 59930.00 I  0.102632 0.000012  0.192138 0.000015  I-0.0172767 0.0000040  0.2556 0.0032  I  -109.736    0.910    -5.634    0.172  0.102588  0.192217 -0.0171383  -109.796    -5.644  
+221218 59931.00 I  0.100238 0.000028  0.192464 0.000024  I-0.0175381 0.0000048  0.2609 0.0041  I  -110.249    0.802    -5.547    0.131  0.100160  0.192490 -0.0173664  -110.291    -5.561  
+221219 59932.00 I  0.098294 0.000028  0.192770 0.000022  I-0.0177833 0.0000071  0.2204 0.0034  I  -110.821    0.693    -5.477    0.073  0.098210  0.192803 -0.0177187  -110.824    -5.496  
+221220 59933.00 I  0.096782 0.000031  0.193071 0.000029  I-0.0179703 0.0000047  0.1539 0.0043  I  -111.265    0.637    -5.319    0.073  0.096711  0.193084 -0.0179634  -111.212    -5.340  
+221221 59934.00 I  0.095788 0.000031  0.193378 0.000029  I-0.0180885 0.0000048  0.0796 0.0034  I  -111.675    0.637    -5.193    0.073  0.095777  0.193348 -0.0181234  -111.654    -5.239  
+221222 59935.00 I  0.094829 0.000031  0.193998 0.000030  I-0.0181001 0.0000049 -0.0828 0.0034  I  -112.065    0.637    -5.326    0.073  0.094877  0.193950 -0.0181060  -112.105    -5.394  
+221223 59936.00 I  0.093417 0.000033  0.194952 0.000030  I-0.0179130 0.0000049 -0.2750 0.0033  I  -112.165    0.637    -5.680    0.073  0.093472  0.194922 -0.0178955  -112.150    -5.759  
+221224 59937.00 I  0.091304 0.000021  0.196098 0.000024  I-0.0176036 0.0000044 -0.3066 0.0033  I  -111.806    0.574    -5.928    0.072  0.091397  0.196126 -0.0175841  -111.706    -6.007  
+221225 59938.00 I  0.088384 0.000021  0.196991 0.000024  I-0.0173441 0.0000044 -0.2052 0.0038  I  -111.258    0.574    -5.868    0.072  0.088402  0.197099 -0.0173115  -111.094    -5.943  
+221226 59939.00 I  0.085236 0.000045  0.197370 0.000026  I-0.0172451 0.0000062  0.0518 0.0036  I  -110.921    0.616    -5.672    0.165  0.085204  0.197391 -0.0172323  -110.709    -5.742  
+221227 59940.00 I  0.081997 0.000046  0.197794 0.000026  I-0.0174667 0.0000058  0.3659 0.0040  I  -110.868    0.616    -5.594    0.165  0.082060  0.197809 -0.0174541  -110.623    -5.660  
+221228 59941.00 I  0.078274 0.000047  0.198310 0.000031  I-0.0179197 0.0000049  0.5084 0.0038  I  -110.911    0.679    -5.607    0.150  0.078253  0.198379 -0.0179243  -110.647    -5.673  
+221229 59942.00 I  0.074743 0.000046  0.198612 0.000031  I-0.0184506 0.0000050  0.5522 0.0034  I  -110.953    0.679    -5.521    0.150  0.074744  0.198584 -0.0184719  -110.694    -5.570  
+221230 59943.00 I  0.071206 0.000046  0.199199 0.000030  I-0.0190011 0.0000047  0.5270 0.0035  I  -111.047    0.679    -5.307    0.150  0.071281  0.199199 -0.0190102  -110.793    -5.341  
+221231 59944.00 I  0.067045 0.000045  0.200073 0.000030  I-0.0194826 0.0000050  0.4357 0.0039  I  -111.221    0.679    -5.118    0.150  0.067074  0.200103 -0.0194855  -110.973    -5.182  
+23 1 1 59945.00 I  0.062790 0.000016  0.200920 0.000022  I-0.0198320 0.0000062  0.2228 0.0036  I  -111.413    0.728    -5.052    0.134  0.062699  0.200944 -0.0197967  -111.162    -5.163  
+23 1 2 59946.00 I  0.059059 0.000021  0.201753 0.000025  I-0.0199222 0.0000053 -0.0082 0.0047  I  -111.532    0.587    -5.053    0.096  0.059003  0.201796 -0.0199243  -111.443    -5.114  
+23 1 3 59947.00 I  0.055741 0.000024  0.202454 0.000019  I-0.0198272 0.0000070 -0.2045 0.0045  I  -111.483    0.624    -5.067    0.133  0.055638  0.202514 -0.0198250  -111.467    -5.128  
+23 1 4 59948.00 I  0.052978 0.000024  0.203007 0.000019  I-0.0195052 0.0000073 -0.4246 0.0054  I  -111.224    0.624    -5.152    0.133  0.052933  0.202990 -0.0195007  -111.313    -5.194  
+23 1 5 59949.00 I  0.050805 0.000024  0.203865 0.000020  I-0.0190225 0.0000083 -0.5110 0.0055  I  -110.844    0.624    -5.386    0.133  0.050795  0.203830 -0.0190232  -110.822    -5.531  
+23 1 6 59950.00 I  0.048801 0.000024  0.205068 0.000019  I-0.0185027 0.0000082 -0.5390 0.0058  I  -110.541    0.624    -5.685    0.133  0.048795  0.205101 -0.0184663  -110.510    -5.834  
+23 1 7 59951.00 I  0.046886 0.000023  0.206242 0.000019  I-0.0179589 0.0000081 -0.5238 0.0059  I  -110.398    0.624    -5.870    0.133  0.046853  0.206221 -0.0179143  -110.392    -5.984  
+23 1 8 59952.00 I  0.045148 0.000019  0.207585 0.000015  I-0.0174852 0.0000086 -0.4185 0.0058  I  -110.319    0.839    -5.859    0.175  0.045146  0.207590 -0.0174487  -110.316    -5.948  
+23 1 9 59953.00 I  0.043369 0.000010  0.209048 0.000012  I-0.0171385 0.0000083 -0.2636 0.0057  I  -110.182    0.829    -5.749    0.144  0.043370  0.209111 -0.0171274  -110.159    -5.821  
+23 110 59954.00 I  0.041301 0.000009  0.210234 0.000012  I-0.0169629 0.0000076 -0.0940 0.0052  I  -109.939    0.829    -5.672    0.144  0.041325  0.210288 -0.0169671  -109.874    -5.733  
+23 111 59955.00 I  0.038971 0.000020  0.211105 0.000039  I-0.0169516 0.0000061  0.0791 0.0046  I  -109.618    0.777    -5.624    0.122  0.038979  0.211134 -0.0169747  -109.583    -5.665  
+23 112 59956.00 I  0.036566 0.000019  0.211939 0.000038  I-0.0170835 0.0000051  0.1395 0.0041  I  -109.289    0.777    -5.515    0.122  0.036547  0.211915 -0.0170559  -109.296    -5.533  
+23 113 59957.00 I  0.034184 0.000019  0.213044 0.000038  I-0.0172129 0.0000056  0.1469 0.0048  I  -109.092    0.777    -5.351    0.122  0.034173  0.213022 -0.0172046  -109.147    -5.343  
+23 114 59958.00 I  0.031799 0.000018  0.214423 0.000039  I-0.0173830 0.0000082  0.1714 0.0047  I  -109.182    0.693    -5.283    0.086  0.031810  0.214393 -0.0173877  -109.253    -5.273  
+23 115 59959.00 I  0.029352 0.000019  0.216067 0.000040  I-0.0175499 0.0000076  0.1786 0.0057  I  -109.534    0.649    -5.403    0.109  0.029351  0.216047 -0.0175710  -109.621    -5.396  
+23 116 59960.00 I  0.026878 0.000020  0.217969 0.000039  I-0.0177195 0.0000080  0.1238 0.0064  I  -109.930    0.649    -5.568    0.109  0.026882  0.217923 -0.0177110  -110.037    -5.563  
+23 117 59961.00 I  0.024334 0.000011  0.220204 0.000013  I-0.0177515 0.0000103 -0.0689 0.0060  I  -110.275    0.624    -5.566    0.123  0.024343  0.220214 -0.0177400  -110.403    -5.564  
+23 118 59962.00 I  0.021695 0.000015  0.222441 0.000038  I-0.0175755 0.0000089 -0.2803 0.0068  I  -110.753    0.688    -5.447    0.131  0.021681  0.222504 -0.0175873  -110.857    -5.445  
+23 119 59963.00 I  0.019118 0.000016  0.224211 0.000039  I-0.0172178 0.0000088 -0.4111 0.0062  I  -111.418    0.688    -5.514    0.131  0.019078  0.224261 -0.0172362  -111.474    -5.516  
+23 120 59964.00 I  0.016678 0.000017  0.225648 0.000039  I-0.0167579 0.0000087 -0.5282 0.0073  I  -111.858    0.688    -5.877    0.131  0.016715  0.225678 -0.0167521  -111.849    -5.887  
+23 121 59965.00 I  0.013983 0.000017  0.226834 0.000038  I-0.0161754 0.0000116 -0.6031 0.0055  I  -111.650    0.870    -6.222    0.146  0.014033  0.226892 -0.0161896  -111.635    -6.235  
+23 122 59966.00 I  0.010880 0.000019  0.227753 0.000039  I-0.0156229 0.0000066 -0.4642 0.0066  I  -110.962    0.572    -6.219    0.103  0.010879  0.227740 -0.0156593  -110.964    -6.230  
+23 123 59967.00 I  0.007815 0.000019  0.228863 0.000041  I-0.0152830 0.0000063 -0.2174 0.0046  I  -110.363    0.572    -5.966    0.103  0.007728  0.228830 -0.0153087  -110.393    -5.970  
+23 124 59968.00 I  0.005413 0.000021  0.230194 0.000019  I-0.0152050 0.0000064  0.0802 0.0047  I  -110.135    0.377    -5.799    0.065  0.005300  0.230244 -0.0152158  -110.223    -5.787  
+23 125 59969.00 I  0.003923 0.000025  0.231461 0.000022  I-0.0154122 0.0000070  0.2844 0.0047  I  -110.144    0.585    -5.796    0.146  0.003852  0.231401 -0.0153642  -110.193    -5.799  
+23 126 59970.00 I  0.002893 0.000025  0.233335 0.000025  I-0.0156946 0.0000070  0.2510 0.0049  I  -110.250    0.585    -5.753    0.146  0.002927  0.233231 -0.0156349  -110.268    -5.775  
+23 127 59971.00 I  0.001582 0.000024  0.235845 0.000028  I-0.0158965 0.0000069  0.1646 0.0055  I  -110.448    0.585    -5.591    0.146  0.001593  0.235918 -0.0158886  -110.468    -5.635  
+23 128 59972.00 I  0.000385 0.000023  0.238121 0.000029  I-0.0159968 0.0000086 -0.0026 0.0052  I  -110.671    0.722    -5.500    0.189  0.000279  0.238107 -0.0159862  -110.687    -5.537  
+23 129 59973.00 I -0.000267 0.000026  0.240381 0.000031  I-0.0158906 0.0000078 -0.1717 0.0057  I  -110.790    0.848    -5.633    0.180 -0.000230  0.240378 -0.0158927  -110.794    -5.657  
+23 130 59974.00 I -0.000856 0.000024  0.242650 0.000031  I-0.0156606 0.0000076 -0.3192 0.0050  I  -110.771    0.848    -5.887    0.180 -0.000925  0.242670 -0.0156444  -110.750    -5.905  
+23 131 59975.00 I -0.001394 0.000020  0.245027 0.000029  I-0.0152305 0.0000062 -0.5319 0.0045  I  -110.661    1.172    -6.068    0.161 -0.001326  0.244961 -0.0152262  -110.583    -6.080  
+23 2 1 59976.00 I -0.002305 0.000020  0.247799 0.000031  I-0.0146201 0.0000047 -0.6747 0.0039  I  -110.463    1.063    -6.146    0.174 -0.002296  0.247864 -0.0146010  -110.444    -6.163  
+23 2 2 59977.00 I -0.003556 0.000020  0.250314 0.000028  I-0.0138984 0.0000047 -0.7656 0.0034  I  -110.177    1.063    -6.241    0.174 -0.003547  0.250346 -0.0138591  -110.219    -6.262  
+23 2 3 59978.00 I -0.004901 0.000020  0.252484 0.000026  I-0.0131162 0.0000048 -0.7745 0.0034  I  -109.909    1.063    -6.398    0.174 -0.004856  0.252572 -0.0130960  -109.978    -6.426  
+23 2 4 59979.00 I -0.006467 0.000017  0.254281 0.000021  I-0.0124005 0.0000050 -0.6302 0.0033  I  -109.790    0.968    -6.503    0.185 -0.006428  0.254285 -0.0124190  -109.861    -6.529  
+23 2 5 59980.00 I -0.008205 0.000019  0.255936 0.000021  I-0.0118712 0.0000044 -0.4397 0.0033  I  -109.803    0.753    -6.432    0.152 -0.008204  0.255923 -0.0118777  -109.870    -6.457  
+23 2 6 59981.00 I -0.009956 0.000021  0.257732 0.000021  I-0.0115058 0.0000044 -0.2951 0.0034  I  -109.791    0.753    -6.225    0.152 -0.009964  0.257731 -0.0114958  -109.866    -6.252  
+23 2 7 59982.00 I -0.011912 0.000019  0.259664 0.000014  I-0.0112778 0.0000051 -0.1601 0.0031  I  -109.635    0.566    -6.037    0.115 -0.011876  0.259655 -0.0112745  -109.747    -6.070  
+23 2 8 59983.00 I -0.014087 0.000038  0.261630 0.000020  I-0.0111850 0.0000044 -0.0269 0.0034  I  -109.362    0.762    -5.953    0.085 -0.014175  0.261674 -0.0111959  -109.435    -5.978  
+23 2 9 59984.00 I -0.015718 0.000037  0.263458 0.000019  I-0.0112342 0.0000044  0.1368 0.0031  I  -109.103    0.762    -5.925    0.085 -0.015815  0.263434 -0.0112446  -109.132    -5.933  
+23 210 59985.00 I -0.016724 0.000037  0.265574 0.000020  I-0.0114595 0.0000045  0.3032 0.0036  I  -108.978    0.762    -5.904    0.085 -0.016692  0.265519 -0.0114722  -108.968    -5.888  
+23 211 59986.00 I -0.017888 0.000035  0.267999 0.000020  I-0.0118001 0.0000056  0.3481 0.0031  I  -109.050    0.934    -5.946    0.042 -0.017796  0.268043 -0.0117909  -109.040    -5.942  
+23 212 59987.00 I -0.019631 0.000035  0.270438 0.000020  I-0.0121312 0.0000043  0.3194 0.0035  I  -109.271    0.788    -6.118    0.123 -0.019580  0.270405 -0.0121316  -109.260    -6.133  
+23 213 59988.00 I -0.021939 0.000035  0.273084 0.000020  I-0.0124025 0.0000043  0.1814 0.0030  I  -109.504    0.788    -6.351    0.123 -0.021949  0.273140 -0.0123642  -109.473    -6.379  
+23 214 59989.00 I -0.024479 0.000013  0.275687 0.000014  I-0.0124664 0.0000043 -0.0394 0.0030  I  -109.686    0.691    -6.481    0.161 -0.024489  0.275701 -0.0124632  -109.625    -6.523  
+23 215 59990.00 I -0.026960 0.000033  0.278184 0.000021  I-0.0123394 0.0000043 -0.2133 0.0030  I  -109.943    0.668    -6.487    0.149 -0.026961  0.278194 -0.0123539  -109.980    -6.504  
+23 216 59991.00 I -0.029366 0.000033  0.280685 0.000021  I-0.0120560 0.0000042 -0.3388 0.0029  I  -110.376    0.668    -6.568    0.149 -0.029393  0.280732 -0.0120613  -110.553    -6.554  
+23 217 59992.00 I -0.031757 0.000033  0.282880 0.000021  I-0.0116878 0.0000039 -0.3865 0.0036  I  -110.746    0.668    -6.863    0.149 -0.031780  0.282935 -0.0116902  -111.072    -6.818  
+23 218 59993.00 I -0.033987 0.000032  0.284847 0.000021  I-0.0113576 0.0000059 -0.2104 0.0035  I  -110.663    0.435    -7.188    0.087 -0.034066  0.284869 -0.0113623  -110.935    -7.143  
+23 219 59994.00 I -0.035819 0.000041  0.286840 0.000022  I-0.0113152 0.0000057  0.1102 0.0041  I  -110.108    0.737    -7.248    0.198 -0.035884  0.286825 -0.0113117  -110.257    -7.216  
+23 220 59995.00 I -0.037237 0.000041  0.288963 0.000021  I-0.0115748 0.0000057  0.4210 0.0041  I  -109.475    0.737    -7.043    0.198 -0.037338  0.288920 -0.0115669  -109.509    -7.029  
+23 221 59996.00 I -0.038245 0.000028  0.291480 0.000015  I-0.0121537 0.0000059  0.7213 0.0039  I  -109.099    0.781    -6.849    0.225 -0.038274  0.291422 -0.0121587  -109.019    -6.868  
+23 222 59997.00 I -0.038775 0.000028  0.294620 0.000016  I-0.0129461 0.0000052  0.8077 0.0040  I  -109.008    0.759    -6.805    0.176 -0.038866  0.294588 -0.0129291  -108.925    -6.815  
+23 223 59998.00 I -0.038959 0.000030  0.298252 0.000015  I-0.0137306 0.0000055  0.7785 0.0041  I  -109.138    0.759    -6.786    0.176 -0.038960  0.298263 -0.0137066  -109.077    -6.785  
+23 224 59999.00 I -0.039161 0.000030  0.301845 0.000018  I-0.0144983 0.0000063  0.7348 0.0047  I  -109.451    0.759    -6.697    0.176 -0.039119  0.301926 -0.0145020  -109.413    -6.693  
+23 225 60000.00 I -0.039671 0.000016  0.305107 0.000019  I-0.0151507 0.0000076  0.5424 0.0046  I  -109.818    0.693    -6.675    0.064 -0.039564  0.305114 -0.0151424  -109.790    -6.690  
+23 226 60001.00 I -0.040934 0.000018  0.308157 0.000030  I-0.0155484 0.0000067  0.2457 0.0051  I  -110.041    0.756    -6.867    0.058 -0.040856  0.308232 -0.0155421  -110.020    -6.905  
+23 227 60002.00 I -0.042701 0.000018  0.310720 0.000030  I-0.0156470 0.0000067 -0.0364 0.0056  I  -110.056    0.756    -7.179    0.058 -0.042777  0.310760 -0.0156050  -110.045    -7.236  
+23 228 60003.00 I -0.044026 0.000016  0.313325 0.000031  I-0.0155124 0.0000090 -0.2082 0.0048  I  -109.943    0.925    -7.384    0.025 -0.044051  0.313293 -0.0155019  -109.938    -7.454  
+23 3 1 60004.00 I -0.045089 0.000015  0.316272 0.000031  I-0.0152925 0.0000070 -0.1944 0.0055  I  -109.724    0.896    -7.400    0.125 -0.045086  0.316379 -0.0152786  -109.729    -7.431  
+23 3 2 60005.00 I -0.046055 0.000014  0.318742 0.000029  I-0.0151082 0.0000063 -0.2268 0.0051  I  -109.354    0.896    -7.359    0.125 -0.046065  0.318766 -0.0150624  -109.433    -7.347  
+23 3 3 60006.00 I -0.046658 0.000012  0.321115 0.000027  I-0.0148464 0.0000073 -0.2367 0.0054  I  -108.903    0.896    -7.397    0.125 -0.046677  0.321138 -0.0148245  -108.998    -7.328  
+23 3 4 60007.00 I -0.046916 0.000010  0.323790 0.000015  I-0.0146882 0.0000088 -0.0865 0.0049  I  -108.565    0.833    -7.477    0.222 -0.046882  0.323792 -0.0146819  -108.638    -7.416  
+23 3 5 60008.00 I -0.046590 0.000010  0.326591 0.000018  I-0.0146905 0.0000065  0.1150 0.0054  I  -108.449    0.942    -7.452    0.107 -0.046540  0.326621 -0.0146823  -108.483    -7.439  
+23 3 6 60009.00 I -0.045652 0.000011  0.329782 0.000015  I-0.0149283 0.0000061  0.3469 0.0048  I  -108.458    0.942    -7.280    0.107 -0.045657  0.329817 -0.0149129  -108.456    -7.322  
+23 3 7 60010.00 I -0.044591 0.000009  0.333285 0.000015  I-0.0153734 0.0000071  0.5460 0.0041  I  -108.436    0.965    -7.082    0.046 -0.044599  0.333296 -0.0153659  -108.413    -7.174  
+23 3 8 60011.00 I -0.043508 0.000011  0.336631 0.000016  I-0.0160118 0.0000056  0.7194 0.0039  I  -108.364    0.828    -7.004    0.039 -0.043530  0.336616 -0.0160051  -108.388    -7.094  
+23 3 9 60012.00 I -0.042348 0.000012  0.339812 0.000015  I-0.0167882 0.0000032  0.8208 0.0031  I  -108.338    0.828    -7.072    0.039 -0.042352  0.339803 -0.0167760  -108.432    -7.140  
+23 310 60013.00 I -0.041298 0.000013  0.343080 0.000016  I-0.0176199 0.0000026  0.8217 0.0022  I  -108.411    0.828    -7.207    0.039 -0.041322  0.343084 -0.0176027  -108.573    -7.251  
+23 311 60014.00 I -0.040745 0.000013  0.346404 0.000011  I-0.0184074 0.0000031  0.7502 0.0025  I  -108.537    0.727    -7.341    0.034 -0.040776  0.346390 -0.0184047  -108.718    -7.379  
+23 312 60015.00 I -0.040525 0.000013  0.349513 0.000012  I-0.0190968 0.0000043  0.6083 0.0027  I  -108.652    0.773    -7.472    0.052 -0.040519  0.349496 -0.0190910  -108.819    -7.513  
+23 313 60016.00 I -0.040085 0.000012  0.352561 0.000014  I-0.0195976 0.0000044  0.3870 0.0035  I  -108.720    0.773    -7.614    0.052 -0.040097  0.352572 -0.0196023  -108.854    -7.660  
+23 314 60017.00 I -0.039698 0.000014  0.355960 0.000016  I-0.0199049 0.0000055  0.2678 0.0035  I  -108.713    0.850    -7.749    0.072 -0.039717  0.355976 -0.0199116  -108.796    -7.801  
+23 315 60018.00 I -0.039671 0.000014  0.359417 0.000015  I-0.0201122 0.0000055  0.0857 0.0043  I  -108.623    0.850    -7.870    0.072 -0.039696  0.359397 -0.0200604  -108.636    -7.924  
+23 316 60019.00 I -0.039793 0.000012  0.362266 0.000015  I-0.0200814 0.0000066 -0.0811 0.0044  I  -108.484    0.850    -8.015    0.072 -0.039824  0.362249 -0.0200712  -108.426    -8.068  
+23 317 60020.00 I -0.039663 0.000012  0.364620 0.000014  I-0.0200318 0.0000069 -0.0024 0.0054  I  -108.319    0.850    -8.204    0.072 -0.039666  0.364628 -0.0200376  -108.244    -8.259  
+23 318 60021.00 I -0.039050 0.000011  0.366835 0.000013  I-0.0201210 0.0000085  0.2096 0.0042  I  -108.116    0.322    -8.346    0.160 -0.039047  0.366850 -0.0201299  -108.073    -8.402  
+23 319 60022.00 I -0.038093 0.000013  0.368979 0.000012  I-0.0204860 0.0000049  0.5265 0.0049  I  -107.898    0.645    -8.311    0.077 -0.038102  0.368994 -0.0204875  -107.908    -8.371  
+23 320 60023.00 I -0.036908 0.000008  0.371251 0.000010  I-0.0211499 0.0000050  0.7712 0.0035  I  -107.738    0.645    -8.122    0.077 -0.036907  0.371284 -0.0211416  -107.809    -8.185  
+23 321 60024.00 I -0.035475 0.000008  0.373935 0.000009  I-0.0220000 0.0000049  0.9306 0.0036  I  -107.671    0.645    -7.951    0.077 -0.035480  0.373974 -0.0220007  -107.798    -8.018  
+23 322 60025.00 I -0.033917 0.000010  0.377063 0.000013  I-0.0229696 0.0000051  0.9654 0.0035  I  -107.675    0.734    -7.911    0.051 -0.033918  0.377072 -0.0229616  -107.800    -7.977  
+23 323 60026.00 I -0.032489 0.000010  0.380214 0.000016  I-0.0238872 0.0000051  0.8693 0.0037  I  -107.767    0.734    -7.942    0.051 -0.032503  0.380245 -0.0238876  -107.871    -8.006  
+23 324 60027.00 I -0.031177 0.000010  0.383293 0.000017  I-0.0246819 0.0000053  0.6943 0.0041  I  -107.993    0.734    -7.965    0.051 -0.031173  0.383274 -0.0246908  -108.068    -8.026  
+23 325 60028.00 I -0.029858 0.000008  0.386395 0.000016  I-0.0252289 0.0000065  0.3786 0.0037  I  -108.292    0.787    -8.025    0.022 -0.029863  0.386430 -0.0252241  -108.334    -8.069  
+23 326 60029.00 I -0.028389 0.000012  0.389489 0.000018  I-0.0254399 0.0000053  0.0653 0.0044  I  -108.504    0.831    -8.202    0.113 -0.028402  0.389466 -0.0254315  -108.511    -8.224  
+23 327 60030.00 I -0.026603 0.000012  0.392600 0.000018  I-0.0253981 0.0000059 -0.1324 0.0042  I  -108.537    0.831    -8.443    0.113 -0.026589  0.392633 -0.0253926  -108.515    -8.443  
+23 328 60031.00 I -0.024705 0.000011  0.395442 0.000016  I-0.0251914 0.0000064 -0.2814 0.0039  I  -108.426    0.883    -8.598    0.162 -0.024718  0.395445 -0.0251809  -108.385    -8.580  
+23 329 60032.00 I -0.023041 0.000013  0.397855 0.000018  I-0.0248750 0.0000050 -0.3114 0.0040  I  -108.194    0.774    -8.617    0.113 -0.023029  0.397858 -0.0248761  -108.184    -8.619  
+23 330 60033.00 I -0.021719 0.000016  0.400025 0.000017  I-0.0246014 0.0000048 -0.2431 0.0034  I  -107.803    0.774    -8.610    0.113 -0.021735  0.400017 -0.0245819  -107.840    -8.642  
+23 331 60034.00 I -0.020382 0.000017  0.402179 0.000019  I-0.0244035 0.0000047 -0.1308 0.0038  I  -107.295    0.774    -8.700    0.113 -0.020397  0.402194 -0.0243867  -107.382    -8.762  
+23 4 1 60035.00 I -0.018854 0.000014  0.404610 0.000019  I-0.0243539 0.0000059  0.0237 0.0034  I  -106.867    0.704    -8.857    0.022 -0.018832  0.404562 -0.0243447  -106.941    -8.931  
+23 4 2 60036.00 I -0.017323 0.000016  0.407361 0.000021  I-0.0244603 0.0000049  0.2065 0.0038  I  -106.710    0.777    -8.925    0.064 -0.017339  0.407431 -0.0244585  -106.744    -9.003  
+23 4 3 60037.00 I -0.015619 0.000016  0.409982 0.000022  I-0.0247653 0.0000048  0.3844 0.0038  I  -106.816    0.777    -8.805    0.064 -0.015648  0.409984 -0.0247405  -106.816    -8.883  
+23 4 4 60038.00 I -0.013823 0.000018  0.412629 0.000022  I-0.0252235 0.0000057  0.5455 0.0038  I  -107.020    0.799    -8.568    0.090 -0.013789  0.412618 -0.0252154  -107.008    -8.648  
+23 4 5 60039.00 I -0.012258 0.000016  0.415448 0.000022  I-0.0258436 0.0000058  0.6684 0.0040  I  -107.195    0.799    -8.386    0.090 -0.012263  0.415517 -0.0258359  -107.244    -8.468  
+23 4 6 60040.00 I -0.010692 0.000015  0.418301 0.000020  I-0.0265287 0.0000056  0.6966 0.0040  I  -107.336    0.799    -8.368    0.090 -0.010755  0.418256 -0.0265377  -107.466    -8.452  
+23 4 7 60041.00 I -0.009130 0.000016  0.421171 0.000017  I-0.0272264 0.0000055  0.6937 0.0040  I  -107.475    0.799    -8.488    0.090 -0.009065  0.421259 -0.0272490  -107.657    -8.560  
+23 4 8 60042.00 I -0.007825 0.000016  0.423798 0.000015  I-0.0278940 0.0000057  0.6246 0.0039  I  -107.615    0.659    -8.642    0.078 -0.007878  0.423780 -0.0279197  -107.816    -8.694  
+23 4 9 60043.00 I -0.006563 0.000017  0.426291 0.000014  I-0.0284512 0.0000056  0.4824 0.0047  I  -107.732    0.659    -8.763    0.078 -0.006541  0.426318 -0.0284814  -107.930    -8.792  
+23 410 60044.00 I -0.005302 0.000017  0.428795 0.000025  I-0.0288425 0.0000075  0.2913 0.0053  I  -107.805    0.801    -8.859    0.054 -0.005307  0.428835 -0.0288476  -107.977    -8.867  
+23 411 60045.00 I -0.004030 0.000017  0.431393 0.000026  I-0.0290273 0.0000090  0.0807 0.0045  I  -107.782    0.801    -8.972    0.054 -0.004073  0.431351 -0.0290184  -107.906    -8.967  
+23 412 60046.00 I -0.002958 0.000017  0.434128 0.000026  I-0.0290340 0.0000050 -0.0396 0.0052  I  -107.575    0.809    -9.123    0.034 -0.002903  0.434183 -0.0290346  -107.627    -9.117  
+23 413 60047.00 I -0.002350 0.000019  0.436721 0.000026  I-0.0289870 0.0000054 -0.0432 0.0037  I  -107.150    0.809    -9.284    0.034 -0.002436  0.436715 -0.0289857  -107.084    -9.311  
+23 414 60048.00 I -0.001832 0.000020  0.439275 0.000026  I-0.0290011 0.0000054  0.1138 0.0038  I  -106.621    0.809    -9.400    0.034 -0.001750  0.439264 -0.0290056  -106.448    -9.462  
+23 415 60049.00 I -0.001119 0.000020  0.441655 0.000026  I-0.0292460 0.0000054  0.3652 0.0043  I  -106.211    0.809    -9.413    0.034 -0.001196  0.441724 -0.0292618  -106.033    -9.492  
+23 416 60050.00 I  0.000182 0.000018  0.443568 0.000013  I-0.0297620 0.0000067  0.7082 0.0042  I  -106.086    0.711    -9.307    0.023  0.000214  0.443555 -0.0298215  -105.983    -9.387  
+23 417 60051.00 I  0.001671 0.000018  0.445285 0.000011  I-0.0306300 0.0000064  0.9541 0.0053  I  -106.237    0.711    -9.135    0.023  0.001716  0.445308 -0.0306441  -106.240    -9.208  
+23 418 60052.00 I  0.002967 0.000017  0.446940 0.000009  I-0.0315994 0.0000081  0.9876 0.0046  I  -106.503    0.663    -8.983    0.027  0.002942  0.446930 -0.0316096  -106.615    -9.044  
+23 419 60053.00 I  0.004298 0.000014  0.448610 0.000017  I-0.0325675 0.0000065  0.9080 0.0053  I  -106.720    0.680    -8.902    0.031  0.004306  0.448627 -0.0325371  -106.853    -8.950  
+23 420 60054.00 I  0.005756 0.000011  0.450445 0.000018  I-0.0333737 0.0000067  0.7034 0.0046  I  -106.846    0.680    -8.886    0.031  0.005723  0.450456 -0.0333578  -106.967    -8.923  
+23 421 60055.00 I  0.007433 0.000010  0.452618 0.000018  I-0.0339555 0.0000065  0.4426 0.0041  I  -106.947    0.680    -8.921    0.031  0.007430  0.452633 -0.0339749  -107.047    -8.949  
+23 422 60056.00 I  0.009109 0.000007  0.455125 0.000017  I-0.0342690 0.0000047  0.2121 0.0039  I  -107.071    0.755    -9.023    0.045  0.009155  0.455143 -0.0342997  -107.160    -9.039  
+23 423 60057.00 I  0.010723 0.000008  0.457862 0.000024  I-0.0343868 0.0000042  0.0028 0.0033  I  -107.186    0.878    -9.191    0.063  0.010695  0.457843 -0.0343744  -107.269    -9.198  
+23 424 60058.00 I  0.012633 0.000009  0.460575 0.000024  I-0.0342825 0.0000045 -0.1830 0.0036  I  -107.228    0.878    -9.364    0.063  0.012615  0.460612 -0.0342760  -107.304    -9.366  
+23 425 60059.00 I  0.014957 0.000009  0.462930 0.000020  I-0.0340635 0.0000059 -0.2407 0.0034  I  -107.154    0.898    -9.465    0.066  0.014950  0.462927 -0.0340746  -107.224    -9.466  
+23 426 60060.00 I  0.017324 0.000014  0.465026 0.000042  I-0.0338249 0.0000052 -0.2268 0.0040  I  -106.947    0.961    -9.504    0.127  0.017333  0.465001 -0.0338446  -106.721    -9.586  
+23 427 60061.00 I  0.019411 0.000014  0.467119 0.000042  I-0.0336200 0.0000055 -0.1824 0.0038  I  -106.593    0.961    -9.576    0.127  0.019395  0.467135 -0.0336272  -106.199    -9.723  
+23 428 60062.00 I  0.021475 0.000014  0.469070 0.000042  I-0.0334909 0.0000055 -0.0455 0.0042  I  -106.127    0.961    -9.748    0.127  0.021422  0.469079 -0.0335007  -105.977    -9.882  
+23 429 60063.00 I  0.023806 0.000014  0.470667 0.000038  I-0.0335520 0.0000064  0.1604 0.0043  I  -105.694    1.150    -9.952    0.218  0.023823  0.470667 -0.0335561  -106.132    -9.986  
+23 430 60064.00 I  0.025994 0.000013  0.472094 0.000038  I-0.0338086 0.0000067  0.3571 0.0044  I  -105.491    1.150   -10.037    0.218  0.025987  0.472089 -0.0338124  -105.944   -10.067  
+23 5 1 60065.00 I  0.027595 0.000017  0.473435 0.000038  I-0.0342612 0.0000060  0.5390 0.0049  I  -105.623    1.120    -9.910    0.143  0.027605  0.473468 -0.0342084  -106.095    -9.946  
+23 5 2 60066.00 I  0.028839 0.000013  0.474632 0.000010  I-0.0348477 0.0000072  0.6042 0.0041  I  -106.010    1.107    -9.628    0.079                                                     
+23 5 3 60067.00 I  0.030244 0.000013  0.475649 0.000014  I-0.0354618 0.0000055  0.6459 0.0048  I  -106.449    1.020    -9.349    0.067                                                     
+23 5 4 60068.00 I  0.031953 0.000013  0.476566 0.000015  I-0.0361456 0.0000064  0.7057 0.0042  I  -106.776    1.020    -9.204    0.067                                                     
+23 5 5 60069.00 I  0.033805 0.000013  0.477607 0.000016  I-0.0368161 0.0000064  0.5940 0.0045  I  -106.979    1.020    -9.224    0.067                                                     
+23 5 6 60070.00 I  0.035744 0.000014  0.478661 0.000016  I-0.0373423 0.0000064  0.5083 0.0046  I  -107.146    1.020    -9.373    0.067                                                     
+23 5 7 60071.00 I  0.037830 0.000026  0.479812 0.000019  I-0.0377966 0.0000067  0.3141 0.0050  I  -107.325    0.976    -9.589    0.157                                                     
+23 5 8 60072.00 I  0.039832 0.000026  0.481227 0.000019  I-0.0379705 0.0000077  0.1197 0.0060  I  -107.446    0.976    -9.815    0.157                                                     
+23 5 9 60073.00 I  0.041738 0.000026  0.482743 0.000017  I-0.0380860 0.0000100  0.0754 0.0054  I  -107.381    1.054   -10.001    0.222                                                     
+23 510 60074.00 I  0.043539 0.000027  0.484264 0.000016  I-0.0381473 0.0000076  0.1093 0.0061  I  -107.082    1.051   -10.119    0.187                                                     
+23 511 60075.00 I  0.045323 0.000027  0.485525 0.000016  I-0.0383715 0.0000070  0.3440 0.0050  I  -106.628    1.051   -10.167    0.187                                                     
+23 512 60076.00 I  0.047277 0.000027  0.486614 0.000017  I-0.0388336 0.0000064  0.5736 0.0048  I  -106.171    1.051   -10.155    0.187                                                     
+23 513 60077.00 I  0.049470 0.000011  0.487752 0.000013  I-0.0395318 0.0000066  0.8424 0.0039  I  -105.853    1.047   -10.087    0.129                                                     
+23 514 60078.00 I  0.052358 0.000015  0.489083 0.000015  I-0.0405278 0.0000046  1.1394 0.0040  I  -105.756    1.124    -9.970    0.167                                                     
+23 515 60079.00 I  0.055845 0.000015  0.490650 0.000017  I-0.0417715 0.0000044  1.3190 0.0034  I  -105.883    1.124    -9.813    0.167                                                     
+23 516 60080.00 I  0.059205 0.000015  0.492207 0.000019  I-0.0431001 0.0000051  1.3014 0.0030  I  -106.171    1.183    -9.631    0.188                                                     
+23 517 60081.00 I  0.062097 0.000021  0.493463 0.000024  I-0.0443153 0.0000042  1.1068 0.0035  I  -106.505    1.183    -9.447    0.188                                                     
+23 518 60082.00 I  0.064541 0.000022  0.494603 0.000025  I-0.0452852 0.0000048  0.8267 0.0032  I  -106.763    1.183    -9.317    0.188                                                     
+23 519 60083.00 I  0.066915 0.000021  0.495696 0.000025  I-0.0459479 0.0000048  0.4842 0.0043  I  -106.892    1.183    -9.310    0.188                                                     
+23 520 60084.00 I  0.069374 0.000020  0.496673 0.000024  I-0.0462776 0.0000072  0.2135 0.0044  I  -106.946    0.322    -9.455    0.160                                                     
+23 521 60085.00 I  0.071638 0.000022  0.497520 0.000022  I-0.0463878 0.0000074 -0.0186 0.0052  I  -107.019    0.775    -9.686    0.041                                                     
+23 522 60086.00 I  0.073704 0.000022  0.498172 0.000021  I-0.0462467 0.0000074 -0.2316 0.0062  I  -107.146    0.775    -9.875    0.041                                                     
+23 523 60087.00 I  0.076189 0.000018  0.498969 0.000014  I-0.0459742 0.0000099 -0.2956 0.0051  I  -107.272    0.775    -9.935    0.041                                                     
+23 524 60088.00 I  0.079176 0.000018  0.499962 0.000016  I-0.0456699 0.0000070 -0.3164 0.0061  I  -107.323    1.003    -9.914    0.030                                                     
+23 525 60089.00 I  0.082214 0.000018  0.501055 0.000015  I-0.0453518 0.0000072 -0.3058 0.0050  I  -107.258    1.003    -9.934    0.030                                                     
+23 526 60090.00 I  0.084803 0.000016  0.502435 0.000014  I-0.0450857 0.0000072 -0.2128 0.0050  I  -107.062    1.003   -10.049    0.030                                                     
+23 527 60091.00 I  0.086793 0.000012  0.503644 0.000015  I-0.0449524 0.0000068 -0.0413 0.0050  I  -106.762    1.042   -10.172    0.026                                                     
+23 528 60092.00 I  0.088633 0.000012  0.504458 0.000015  I-0.0450008 0.0000070  0.1233 0.0043  I  -106.498    1.042   -10.160    0.026                                                     
+23 529 60093.00 I  0.090318 0.000018  0.505219 0.000014  I-0.0451802 0.0000054  0.2315 0.0045  I  -106.510    1.114    -9.970    0.072                                                     
+23 530 60094.00 I  0.091893 0.000017  0.506039 0.000011  I-0.0454548 0.0000057  0.3127 0.0041  I  -106.929    1.193    -9.696    0.110                                                     
+23 531 60095.00 I  0.093805 0.000017  0.506927 0.000011  I-0.0457726 0.0000061  0.2949 0.0045  I  -107.603    1.193    -9.460    0.110                                                     
+23 6 1 60096.00 I  0.096352 0.000017  0.507808 0.000012  I-0.0460254 0.0000070  0.2194 0.0048  I  -108.215    1.193    -9.310    0.110                                                     
+23 6 2 60097.00 I  0.099268 0.000017  0.508635 0.000012  I-0.0461917 0.0000073  0.0849 0.0053  I  -108.604    1.193    -9.249    0.110                                                     
+23 6 3 60098.00 I  0.102228 0.000019  0.509370 0.000014  I-0.0461740 0.0000080 -0.1131 0.0051  I  -108.874    1.193    -9.314    0.110                                                     
+23 6 4 60099.00 I  0.105153 0.000016  0.509997 0.000015  I-0.0459452 0.0000072 -0.3719 0.0060  I  -109.135    0.939    -9.539    0.123                                                     
+23 6 5 60100.00 I  0.108081 0.000016  0.510390 0.000014  I-0.0454554 0.0000090 -0.5550 0.0058  I  -109.279    0.785    -9.850    0.147                                                     
+23 6 6 60101.00 I  0.111224 0.000016  0.510816 0.000015  I-0.0449064 0.0000091 -0.5246 0.0065  I  -109.135    0.785   -10.074    0.147                                                     
+23 6 7 60102.00 I  0.114140 0.000021  0.511283 0.000020  I-0.0444226 0.0000095 -0.4449 0.0064  I  -108.760    0.785   -10.100    0.147                                                     
+23 6 8 60103.00 I  0.116588 0.000021  0.511546 0.000019  I-0.0440532 0.0000091 -0.2553 0.0065  I  -108.425    0.785    -9.982    0.147                                                     
+23 6 9 60104.00 I  0.119151 0.000021  0.511808 0.000020  I-0.0439290 0.0000090 -0.0148 0.0085  I  -108.332    0.785    -9.852    0.147                                                     
+23 610 60105.00 I  0.121672 0.000019  0.512145 0.000020  I-0.0440222 0.0000144  0.2215 0.0069  I  -108.440    0.322    -9.769    0.160                                                     
+23 611 60106.00 I  0.123883 0.000024  0.512550 0.000024  I-0.0443196 0.0000105  0.3007 0.0087  I  -108.586    0.963    -9.705    0.258                                                     
+23 612 60107.00 I  0.126138 0.000027  0.512892 0.000028  I-0.0445772 0.0000097  0.2406 0.0071  I  -108.697    0.963    -9.615    0.258                                                     
+23 613 60108.00 I  0.128649 0.000023  0.513071 0.000026  I-0.0447853 0.0000097  0.1341 0.0068  I  -108.850    0.963    -9.477    0.258                                                     
+23 614 60109.00 I  0.131251 0.000029  0.513140 0.000032  I-0.0448186 0.0000096 -0.0527 0.0067  P  -109.139    0.278    -9.286    0.145                                                     
+23 615 60110.00 I  0.133808 0.000027  0.513048 0.000033  I-0.0446706 0.0000092 -0.2673 0.0062  P  -109.503    0.288    -9.112    0.148                                                     
+23 616 60111.00 I  0.136539 0.000091  0.512921 0.000091  I-0.0442559 0.0000080 -0.5663 0.0064  P  -109.778    0.297    -9.085    0.151                                                     
+23 617 60112.00 I  0.139484 0.000091  0.512884 0.000091  I-0.0435767 0.0000088 -0.7492 0.0050  P  -109.884    0.304    -9.283    0.154                                                     
+23 618 60113.00 I  0.142526 0.000090  0.512748 0.000091  I-0.0428000 0.0000061 -0.8047 0.0058  P  -109.909    0.309    -9.626    0.155                                                     
+23 619 60114.00 I  0.145630 0.000090  0.512525 0.000090  I-0.0419754 0.0000077 -0.8360 0.0096  P  -109.982    0.313    -9.906    0.157                                                     
+23 620 60115.00 I  0.148749 0.000090  0.512312 0.000091  I-0.0411429 0.0000183 -0.8226 0.0103  P  -110.135    0.316    -9.961    0.158                                                     
+23 621 60116.00 I  0.152072 0.000090  0.511976 0.000090  I-0.0403414 0.0000191 -0.7757 0.0132  P  -110.321    0.318    -9.822    0.158                                                     
+23 622 60117.00 I  0.155396 0.000090  0.511562 0.000091  I-0.0395959 0.0000191 -0.7156 0.0162  P  -110.480    0.319    -9.663    0.159                                                     
+23 623 60118.00 I  0.158430 0.000091  0.511172 0.000091  I-0.0389353 0.0000262 -0.5803 0.0176  P  -110.540    0.320    -9.596    0.159                                                     
+23 624 60119.00 I  0.161373 0.000091  0.510865 0.000091  I-0.0384348 0.0000296 -0.4465 0.0190  P  -110.426    0.321    -9.559    0.160                                                     
+23 625 60120.00 I  0.164257 0.000091  0.510651 0.000091  I-0.0380216 0.0000275 -0.3749 0.0193  P  -110.195    0.321    -9.422    0.160                                                     
+23 626 60121.00 I  0.167207 0.000091  0.510335 0.000091  I-0.0377012 0.0000248 -0.2547 0.0178  P  -110.131    0.321    -9.185    0.160                                                     
+23 627 60122.00 I  0.170481 0.000091  0.510040 0.000091  I-0.0374829 0.0000225 -0.2224 0.0160  P  -110.546    0.321    -8.993    0.160                                                     
+23 628 60123.00 I  0.173866 0.000091  0.509898 0.000091  I-0.0372276 0.0000202 -0.2766 0.0298  P  -111.406    0.322    -8.954    0.160                                                     
+23 629 60124.00 I  0.177042 0.000091  0.509708 0.000090  I-0.0368832 0.0000552                 P  -112.298    0.322    -9.004    0.160                                                     
+23 630 60125.00 P  0.180068 0.000602  0.509331 0.000400  P-0.0365085 0.0001080                 P  -112.867    0.322    -9.024    0.160                                                     
+23 7 1 60126.00 P  0.182926 0.000894  0.508797 0.000659  P-0.0359376 0.0002041                 P  -113.138    0.322    -9.043    0.160                                                     
+23 7 2 60127.00 P  0.185697 0.001127  0.508160 0.000882  P-0.0351192 0.0003028                 P  -113.267    0.322    -9.197    0.160                                                     
+23 7 3 60128.00 P  0.188414 0.001328  0.507394 0.001085  P-0.0341237 0.0004021                 P  -113.214    0.322    -9.467    0.160                                                     
+23 7 4 60129.00 P  0.191115 0.001508  0.506515 0.001274  P-0.0330774 0.0005017                 P  -112.894    0.322    -9.630    0.160                                                     
+23 7 5 60130.00 P  0.193792 0.001673  0.505592 0.001453  P-0.0321200 0.0006014                 P  -112.497    0.322    -9.539    0.160                                                     
+23 7 6 60131.00 P  0.196430 0.001826  0.504652 0.001624  P-0.0313628 0.0007012                 P  -112.372    0.322    -9.322    0.160                                                     
+23 7 7 60132.00 P  0.199045 0.001971  0.503710 0.001788  P-0.0308674 0.0007500                 P  -112.639    0.322    -9.195    0.160                                                     
+23 7 8 60133.00 P  0.201624 0.002108  0.502762 0.001946  P-0.0306057 0.0005500                 P  -113.093    0.322    -9.184    0.160                                                     
+23 7 9 60134.00 P  0.204160 0.002238  0.501763 0.002099  P-0.0305020 0.0007548                 P  -113.469    0.322    -9.163    0.160                                                     
+23 710 60135.00 P  0.206651 0.002363  0.500719 0.002248  P-0.0304256 0.0009344                 P  -113.667    0.322    -9.070    0.160                                                     
+23 711 60136.00 P  0.209095 0.002483  0.499647 0.002394  P-0.0302454 0.0010994                 P  -113.773    0.322    -8.962    0.160                                                     
+23 712 60137.00 P  0.211513 0.002599  0.498517 0.002536  P-0.0298228 0.0012543                 P  -113.944    0.322    -8.897    0.160                                                     
+23 713 60138.00 P  0.213893 0.002711  0.497335 0.002675  P-0.0291342 0.0014016                 P  -114.248    0.322    -8.884    0.160                                                     
+23 714 60139.00 P  0.216221 0.002820  0.496114 0.002811  P-0.0282058 0.0015429                 P  -114.580    0.322    -8.959    0.160                                                     
+23 715 60140.00 P  0.218520 0.002926  0.494859 0.002945  P-0.0271054 0.0016792                 P  -114.778    0.322    -9.186    0.160                                                     
+23 716 60141.00 P  0.220797 0.003028  0.493567 0.003076  P-0.0259170 0.0018113                 P  -114.805    0.322    -9.540    0.160                                                     
+23 717 60142.00 P  0.223042 0.003129  0.492226 0.003205  P-0.0247088 0.0019399                 P  -114.769    0.322    -9.836    0.160                                                     
+23 718 60143.00 P  0.225266 0.003227  0.490829 0.003332  P-0.0235326 0.0020652                 P  -114.780    0.322    -9.860    0.160                                                     
+23 719 60144.00 P  0.227470 0.003322  0.489382 0.003458  P-0.0224540 0.0021877                 P  -114.868    0.322    -9.592    0.160                                                     
+23 720 60145.00 P  0.229643 0.003416  0.487891 0.003581  P-0.0215182 0.0023077                 P  -114.997    0.322    -9.235    0.160                                                     
+23 721 60146.00 P  0.231783 0.003508  0.486359 0.003703  P-0.0207600 0.0024255                 P  -115.088    0.322    -9.000    0.160                                                     
+23 722 60147.00 P  0.233900 0.003598  0.484794 0.003824  P-0.0201755 0.0025411                 P  -115.044    0.322    -8.900    0.160                                                     
+23 723 60148.00 P  0.235996 0.003686  0.483209 0.003943  P-0.0197344 0.0026548                 P  -114.862    0.322    -8.810    0.160                                                     
+23 724 60149.00 P  0.238067 0.003773  0.481605 0.004060  P-0.0193798 0.0027668                 P  -114.767    0.322    -8.697    0.160                                                     
+23 725 60150.00 P  0.240111 0.003858  0.479979 0.004177  P-0.0190484 0.0028772                 P  -115.089    0.322    -8.689    0.160                                                     
+23 726 60151.00 P  0.242127 0.003942  0.478337 0.004292  P-0.0186649 0.0029860                 P  -115.896    0.322    -8.893    0.160                                                     
+23 727 60152.00 P  0.244113 0.004025  0.476673 0.004406  P-0.0181615 0.0030934                 P  -116.815    0.322    -9.198    0.160                                                     
+23 728 60153.00 P  0.246072 0.004106  0.474985 0.004518  P-0.0174851 0.0031995                 P  -117.397    0.322    -9.388    0.160                                                     
+23 729 60154.00 P  0.248004 0.004186  0.473270 0.004630  P-0.0166197 0.0033043                 P  -117.541    0.322    -9.416    0.160                                                     
+23 730 60155.00 P  0.249908 0.004265  0.471522 0.004741  P-0.0156152 0.0034080                 P  -117.407    0.322    -9.437    0.160                                                     
+23 731 60156.00 P  0.251782 0.004343  0.469743 0.004850  P-0.0145812 0.0035105                 P  -117.087    0.322    -9.517    0.160                                                     
+23 8 1 60157.00 P  0.253629 0.004420  0.467937 0.004959  P-0.0136673 0.0036120                 P  -116.655    0.322    -9.495    0.160                                                     
+23 8 2 60158.00 P  0.255448 0.004496  0.466103 0.005067  P-0.0130191 0.0037124                 P  -116.381    0.322    -9.271    0.160                                                     
+23 8 3 60159.00 P  0.257237 0.004571  0.464242 0.005174  P-0.0127195 0.0038119                 P  -116.529    0.322    -9.050    0.160                                                     
+23 8 4 60160.00 P  0.258995 0.004645  0.462357 0.005280  P-0.0127435 0.0039105                 P  -116.999    0.322    -9.083    0.160                                                     
+23 8 5 60161.00 P  0.260722 0.004718  0.460449 0.005385  P-0.0129752 0.0040082                 P  -117.463    0.322    -9.288    0.160                                                     
+23 8 6 60162.00 P  0.262418 0.004790  0.458519 0.005489  P-0.0132455 0.0041051                 P  -117.772    0.322    -9.368    0.160                                                     
+23 8 7 60163.00 P  0.264081 0.004862  0.456567 0.005593  P-0.0133923 0.0042012                 P  -117.998    0.322    -9.238    0.160                                                     
+23 8 8 60164.00 P  0.265710 0.004932  0.454593 0.005696  P-0.0133017 0.0042965                 P  -118.189    0.322    -9.107    0.160                                                     
+23 8 9 60165.00 P  0.267305 0.005002  0.452599 0.005798  P-0.0129261 0.0043911                 P  -118.336    0.322    -9.151    0.160                                                     
+23 810 60166.00 P  0.268864 0.005071  0.450584 0.005899  P-0.0122835 0.0044849                 P  -118.483    0.322    -9.309    0.160                                                     
+23 811 60167.00 P  0.270386 0.005140  0.448549 0.006000  P-0.0114310 0.0045781                 P  -118.670    0.322    -9.444    0.160                                                     
+23 812 60168.00 P  0.271872 0.005208  0.446494 0.006100  P-0.0104413 0.0046706                 P  -118.810    0.322    -9.551    0.160                                                     
+23 813 60169.00 P  0.273321 0.005275  0.444419 0.006200  P-0.0093956 0.0047625                 P  -118.785    0.322    -9.694    0.160                                                     
+23 814 60170.00 P  0.274733 0.005341  0.442323 0.006299  P-0.0083703 0.0048537                 P  -118.613    0.322    -9.822    0.160                                                     
+23 815 60171.00 P  0.276107 0.005407  0.440205 0.006397  P-0.0074318 0.0049444                 P  -118.421    0.322    -9.764    0.160                                                     
+23 816 60172.00 P  0.277445 0.005472  0.438068 0.006495  P-0.0066326 0.0050344                 P  -118.299    0.322    -9.437    0.160                                                     
+23 817 60173.00 P  0.278746 0.005537  0.435910 0.006592  P-0.0060063 0.0051240                 P  -118.243    0.322    -8.999    0.160                                                     
+23 818 60174.00 P  0.280009 0.005601  0.433733 0.006688  P-0.0055537 0.0052129                 P  -118.200    0.322    -8.706    0.160                                                     
+23 819 60175.00 P  0.281234 0.005665  0.431537 0.006784  P-0.0052468 0.0053014                 P  -118.126    0.322    -8.652    0.160                                                     
+23 820 60176.00 P  0.282421 0.005728  0.429322 0.006880  P-0.0050382 0.0053893                 P  -118.013    0.322    -8.729    0.160                                                     
+23 821 60177.00 P  0.283568 0.005790  0.427091 0.006975  P-0.0048644 0.0054768                 P  -117.956    0.322    -8.815    0.160                                                     
+23 822 60178.00 P  0.284676 0.005852  0.424844 0.007069  P-0.0046507 0.0055637                 P  -118.139    0.322    -8.938    0.160                                                     
+23 823 60179.00 P  0.285744 0.005914  0.422582 0.007163  P-0.0043280 0.0056502                 P  -118.649    0.322    -9.184    0.160                                                     
+23 824 60180.00 P  0.286772 0.005975  0.420305 0.007257  P-0.0038453 0.0057362                 P  -119.291    0.322    -9.504    0.160                                                     
+23 825 60181.00 P  0.287759 0.006036  0.418013 0.007350  P-0.0031803 0.0058218                 P  -119.711    0.322    -9.722    0.160                                                     
+23 826 60182.00 P  0.288705 0.006096  0.415708 0.007443  P-0.0023539 0.0059070                 P  -119.728    0.322    -9.744    0.160                                                     
+23 827 60183.00 P  0.289610 0.006155  0.413390 0.007535  P-0.0014413 0.0059917                 P  -119.421    0.322    -9.656    0.160                                                     
+23 828 60184.00 P  0.290475 0.006215  0.411058 0.007627  P-0.0005707 0.0060760                 P  -118.959    0.322    -9.533    0.160                                                     
+23 829 60185.00 P  0.291299 0.006273  0.408715 0.007718  P 0.0001081 0.0061599                 P  -118.548    0.322    -9.298    0.160                                                     
+23 830 60186.00 P  0.292082 0.006332  0.406359 0.007809  P 0.0004783 0.0062434                 P  -118.464    0.322    -8.934    0.160                                                     
+23 831 60187.00 P  0.292824 0.006390  0.403993 0.007899  P 0.0005019 0.0063266                 P  -118.808    0.322    -8.690    0.160                                                     
+23 9 1 60188.00 P  0.293524 0.006448  0.401616 0.007989  P 0.0002418 0.0064093                 P  -119.285    0.322    -8.824    0.160                                                     
+23 9 2 60189.00 P  0.294184 0.006505  0.399230 0.008079  P-0.0001537 0.0064917                 P  -119.514    0.322    -9.197    0.160                                                     
+23 9 3 60190.00 P  0.294803 0.006562  0.396835 0.008168  P-0.0005089 0.0065737                 P  -119.528    0.322    -9.394    0.160                                                     
+23 9 4 60191.00 P  0.295380 0.006618  0.394431 0.008257  P-0.0006711 0.0066554                 P  -119.648    0.322    -9.260    0.160                                                     
+23 9 5 60192.00 P  0.295915 0.006674  0.392020 0.008346  P-0.0005573 0.0067368                 P  -119.952    0.322    -9.070    0.160                                                     
+23 9 6 60193.00 P  0.296409 0.006730  0.389603 0.008434  P-0.0001615 0.0068177                 P  -120.204    0.322    -9.117    0.160                                                     
+23 9 7 60194.00 P  0.296862 0.006785  0.387179 0.008522  P 0.0004650 0.0068984                 P  -120.255    0.322    -9.344    0.160                                                     
+23 9 8 60195.00 P  0.297272 0.006840  0.384750 0.008609  P 0.0012411 0.0069788                 P  -120.191    0.322    -9.496    0.160                                                     
+23 9 9 60196.00 P  0.297640 0.006895  0.382317 0.008696  P 0.0020768 0.0070588                 P  -120.089    0.322    -9.474    0.160                                                     
+23 910 60197.00 P  0.297967 0.006950  0.379879 0.008783  P 0.0028884 0.0071385                 P  -119.892    0.322    -9.392    0.160                                                     
+23 911 60198.00 P  0.298251 0.007004  0.377438 0.008870  P 0.0036041 0.0072179                 P  -119.579    0.322    -9.347    0.160                                                     
+23 912 60199.00 P  0.298494 0.007058  0.374995 0.008956  P 0.0041679 0.0072970                                                                                                             
+23 913 60200.00 P  0.298694 0.007111  0.372549 0.009042  P 0.0045494 0.0073758                                                                                                             
+23 914 60201.00 P  0.298853 0.007164  0.370102 0.009127  P 0.0047410 0.0074544                                                                                                             
+23 915 60202.00 P  0.298970 0.007217  0.367654 0.009212  P 0.0047646 0.0075326                                                                                                             
+23 916 60203.00 P  0.299045 0.007270  0.365205 0.009297  P 0.0046674 0.0076106                                                                                                             
+23 917 60204.00 P  0.299079 0.007322  0.362758 0.009382  P 0.0045153 0.0076883                                                                                                             
+23 918 60205.00 P  0.299071 0.007374  0.360311 0.009466  P 0.0043835 0.0077657                                                                                                             
+23 919 60206.00 P  0.299022 0.007426  0.357867 0.009550  P 0.0043461 0.0078428                                                                                                             
+23 920 60207.00 P  0.298931 0.007477  0.355425 0.009634  P 0.0044616 0.0079197                                                                                                             
+23 921 60208.00 P  0.298798 0.007529  0.352986 0.009717  P 0.0047547 0.0079964                                                                                                             
+23 922 60209.00 P  0.298625 0.007579  0.350551 0.009800  P 0.0052115 0.0080728                                                                                                             
+23 923 60210.00 P  0.298410 0.007630  0.348120 0.009883  P 0.0057732 0.0081489                                                                                                             
+23 924 60211.00 P  0.298154 0.007681  0.345694 0.009966  P 0.0063330 0.0082248                                                                                                             
+23 925 60212.00 P  0.297857 0.007731  0.343274 0.010048  P 0.0067570 0.0083005                                                                                                             
+23 926 60213.00 P  0.297519 0.007781  0.340861 0.010130  P 0.0069201 0.0083759                                                                                                             
+23 927 60214.00 P  0.297140 0.007830  0.338454 0.010212  P 0.0067459 0.0084511                                                                                                             
+23 928 60215.00 P  0.296721 0.007880  0.336055 0.010294  P 0.0062456 0.0085261                                                                                                             
+23 929 60216.00 P  0.296261 0.007929  0.333664 0.010375  P 0.0055232 0.0086008                                                                                                             
+23 930 60217.00 P  0.295761 0.007978  0.331281 0.010456  P 0.0047444 0.0086754                                                                                                             
+2310 1 60218.00 P  0.295222 0.008027  0.328908 0.010537  P 0.0040874 0.0087497                                                                                                             
+2310 2 60219.00 P  0.294643 0.008076  0.326546 0.010618  P 0.0036833 0.0088237                                                                                                             
+2310 3 60220.00 P  0.294024 0.008124  0.324193 0.010698  P 0.0035839 0.0088976                                                                                                             
+2310 4 60221.00 P  0.293366 0.008172  0.321852 0.010778  P 0.0037602 0.0089713                                                                                                             
+2310 5 60222.00 P  0.292669 0.008220  0.319523 0.010858  P 0.0041336 0.0090448                                                                                                             
+2310 6 60223.00 P  0.291933 0.008268  0.317206 0.010938  P 0.0046068 0.0091180                                                                                                             
+2310 7 60224.00 P  0.291159 0.008315  0.314902 0.011017  P 0.0050860 0.0091911                                                                                                             
+2310 8 60225.00 P  0.290346 0.008362  0.312612 0.011096  P 0.0054916 0.0092639                                                                                                             
+2310 9 60226.00 P  0.289496 0.008410  0.310335 0.011175  P 0.0057620 0.0093366                                                                                                             
+231010 60227.00 P  0.288608 0.008456  0.308074 0.011254  P 0.0058574 0.0094091                                                                                                             
+231011 60228.00 P  0.287683 0.008503  0.305828 0.011333  P 0.0057626 0.0094814                                                                                                             
+231012 60229.00 P  0.286721 0.008550  0.303597 0.011411  P 0.0054890 0.0095535                                                                                                             
+231013 60230.00 P  0.285722 0.008596  0.301383 0.011489  P 0.0050772 0.0096254                                                                                                             
+231014 60231.00 P  0.284686 0.008642  0.299187 0.011567  P 0.0045894 0.0096971                                                                                                             
+231015 60232.00 P  0.283615 0.008688  0.297007 0.011645  P 0.0041055 0.0097686                                                                                                             
+231016 60233.00 P  0.282507 0.008734  0.294846 0.011722  P 0.0036217 0.0098400                                                                                                             
+231017 60234.00 P  0.281365 0.008779  0.292703 0.011800  P 0.0032905 0.0099112                                                                                                             
+231018 60235.00 P  0.280187 0.008825  0.290580 0.011877  P 0.0031503 0.0099822                                                                                                             
+231019 60236.00 P  0.278975 0.008870  0.288476 0.011954  P 0.0031976 0.0100531                                                                                                             
+231020 60237.00 P  0.277728 0.008915  0.286393 0.012030  P 0.0033798 0.0101238                                                                                                             
+231021 60238.00 P  0.276448 0.008960  0.284330 0.012107  P 0.0036015 0.0101943                                                                                                             
+231022 60239.00 P  0.275134 0.009005  0.282289 0.012183  P 0.0037406 0.0102646                                                                                                             
+231023 60240.00 P  0.273787 0.009049  0.280269 0.012259  P 0.0036761 0.0103348                                                                                                             
+231024 60241.00 P  0.272408 0.009094  0.278271 0.012335  P 0.0033205 0.0104048                                                                                                             
+231025 60242.00 P  0.270996 0.009138  0.276297 0.012411  P 0.0026511 0.0104747                                                                                                             
+231026 60243.00 P  0.269553 0.009182  0.274345 0.012487  P 0.0017268 0.0105444                                                                                                             
+231027 60244.00 P  0.268078 0.009226  0.272418 0.012562  P 0.0006786 0.0106139                                                                                                             
+231028 60245.00 P  0.266572 0.009270  0.270514 0.012638  P-0.0003271 0.0106833                                                                                                             
+231029 60246.00 P  0.265036 0.009313  0.268635 0.012713  P-0.0011385 0.0107526                                                                                                             
+231030 60247.00 P  0.263470 0.009357  0.266782 0.012788  P-0.0016613 0.0108216                                                                                                             
+231031 60248.00 P  0.261874 0.009400  0.264954 0.012863  P-0.0018790 0.0108906                                                                                                             
+2311 1 60249.00 P  0.260250 0.009443  0.263152 0.012937  P-0.0018423 0.0109594                                                                                                             
+2311 2 60250.00 P  0.258597 0.009486  0.261376 0.013012  P-0.0016430 0.0110280                                                                                                             
+2311 3 60251.00 P  0.256916 0.009529  0.259627 0.013086  P-0.0013825 0.0110965                                                                                                             
+2311 4 60252.00 P  0.255207 0.009571  0.257906 0.013160  P-0.0011525 0.0111649                                                                                                             
+2311 5 60253.00 P  0.253472 0.009614  0.256212 0.013234  P-0.0010240 0.0112331                                                                                                             
+2311 6 60254.00 P  0.251710 0.009656  0.254547 0.013308  P-0.0010443 0.0113012                                                                                                             
+2311 7 60255.00 P  0.249922 0.009699  0.252910 0.013381  P-0.0012350 0.0113691                                                                                                             
+2311 8 60256.00 P  0.248109 0.009741  0.251301 0.013455  P-0.0015917 0.0114369                                                                                                             
+2311 9 60257.00 P  0.246270 0.009783  0.249722 0.013528  P-0.0020851 0.0115046                                                                                                             
+231110 60258.00 P  0.244408 0.009825  0.248173 0.013601  P-0.0026629 0.0115721                                                                                                             
+231111 60259.00 P  0.242521 0.009866  0.246654 0.013674  P-0.0032552 0.0116395                                                                                                             
+231112 60260.00 P  0.240612 0.009908  0.245165 0.013747  P-0.0037822 0.0117067                                                                                                             
+231113 60261.00 P  0.238679 0.009949  0.243707 0.013820  P-0.0041682 0.0117739                                                                                                             
+231114 60262.00 P  0.236725 0.009991  0.242280 0.013892  P-0.0043580 0.0118409                                                                                                             
+231115 60263.00 P  0.234749 0.010032  0.240884 0.013965  P-0.0043382 0.0119077                                                                                                             
+231116 60264.00 P  0.232752 0.010073  0.239520 0.014037  P-0.0041476 0.0119745                                                                                                             
+231117 60265.00 P  0.230734 0.010114  0.238187 0.014109  P-0.0038757 0.0120411                                                                                                             
+231118 60266.00 P  0.228697 0.010155  0.236888 0.014181  P-0.0036434 0.0121076                                                                                                             
+231119 60267.00 P  0.226641 0.010196  0.235620 0.014253  P-0.0035710 0.0121740                                                                                                             
+231120 60268.00 P  0.224566 0.010236  0.234386 0.014325  P-0.0037470 0.0122402                                                                                                             
+231121 60269.00 P  0.222472 0.010277  0.233184 0.014396  P-0.0042018 0.0123063                                                                                                             
+231122 60270.00 P  0.220362 0.010317  0.232016 0.014468  P-0.0048977 0.0123723                                                                                                             
+231123 60271.00 P  0.218234 0.010357  0.230882 0.014539  P-0.0057341 0.0124382                                                                                                             
+231124 60272.00 P  0.216091 0.010397  0.229782 0.014610  P-0.0065730 0.0125040                                                                                                             
+231125 60273.00 P  0.213931 0.010437  0.228715 0.014681  P-0.0072728 0.0125696                                                                                                             
+231126 60274.00 P  0.211757 0.010477  0.227683 0.014752  P-0.0077273 0.0126352                                                                                                             
+231127 60275.00 P  0.209568 0.010517  0.226686 0.014823  P-0.0078914 0.0127006                                                                                                             
+231128 60276.00 P  0.207366 0.010557  0.225723 0.014893  P-0.0077856 0.0127659                                                                                                             
+231129 60277.00 P  0.205150 0.010596  0.224795 0.014964  P-0.0074820 0.0128311                                                                                                             
+231130 60278.00 P  0.202922 0.010635  0.223902 0.015034  P-0.0070771 0.0128962                                                                                                             
+2312 1 60279.00 P  0.200682 0.010675  0.223045 0.015104  P-0.0066670 0.0129612                                                                                                             
+2312 2 60280.00 P  0.198431 0.010714  0.222223 0.015174  P-0.0063308 0.0130260                                                                                                             
+2312 3 60281.00 P  0.196169 0.010753  0.221436 0.015244  P-0.0061232 0.0130908                                                                                                             
+2312 4 60282.00 P  0.193898 0.010792  0.220685 0.015314  P-0.0060723 0.0131554                                                                                                             
+2312 5 60283.00 P  0.191616 0.010831  0.219971 0.015384  P-0.0061798 0.0132199                                                                                                             
+2312 6 60284.00 P  0.189326 0.010870  0.219292 0.015454  P-0.0064224 0.0132844                                                                                                             
+2312 7 60285.00 P  0.187029 0.010908  0.218649 0.015523  P-0.0067556 0.0133487                                                                                                             
+2312 8 60286.00 P  0.184723 0.010947  0.218043 0.015592  P-0.0071190 0.0134129                                                                                                             
+2312 9 60287.00 P  0.182411 0.010985  0.217472 0.015662  P-0.0074421 0.0134770                                                                                                             
+231210 60288.00 P  0.180093 0.011024  0.216939 0.015731  P-0.0076518 0.0135410                                                                                                             
+231211 60289.00 P  0.177769 0.011062  0.216441 0.015800  P-0.0076856 0.0136050                                                                                                             
+231212 60290.00 P  0.175440 0.011100  0.215981 0.015869  P-0.0075110 0.0136688                                                                                                             
+231213 60291.00 P  0.173108 0.011138  0.215556 0.015937  P-0.0071447 0.0137325                                                                                                             
+231214 60292.00 P  0.170771 0.011176  0.215169 0.016006  P-0.0066621 0.0137961                                                                                                             
+231215 60293.00 P  0.168432 0.011214  0.214818 0.016075  P-0.0061830 0.0138596                                                                                                             
+231216 60294.00 P  0.166090 0.011252  0.214503 0.016143  P-0.0058395 0.0139230                                                                                                             
+231217 60295.00 P  0.163747 0.011290  0.214226 0.016211  P-0.0057332 0.0139863                                                                                                             
+231218 60296.00 P  0.161403 0.011327  0.213985 0.016280  P-0.0059030 0.0140495                                                                                                             
+231219 60297.00 P  0.159059 0.011365  0.213781 0.016348  P-0.0063129 0.0141127                                                                                                             
+231220 60298.00 P  0.156714 0.011402  0.213613 0.016416  P-0.0068648 0.0141757                                                                                                             
+231221 60299.00 P  0.154371 0.011439  0.213482 0.016483  P-0.0074266 0.0142386                                                                                                             
+231222 60300.00 P  0.152029 0.011477  0.213388 0.016551  P-0.0078668 0.0143014                                                                                                             
+231223 60301.00 P  0.149690 0.011514  0.213330 0.016619  P-0.0080843 0.0143642                                                                                                             
+231224 60302.00 P  0.147353 0.011551  0.213309 0.016686  P-0.0080287 0.0144268                                                                                                             
+231225 60303.00 P  0.145020 0.011588  0.213324 0.016754  P-0.0077055 0.0144894                                                                                                             
+231226 60304.00 P  0.142691 0.011625  0.213375 0.016821  P-0.0071688 0.0145519                                                                                                             
+231227 60305.00 P  0.140367 0.011661  0.213463 0.016888  P-0.0065030 0.0146142                                                                                                             
+231228 60306.00 P  0.138048 0.011698  0.213587 0.016956  P-0.0058014 0.0146765                                                                                                             
+231229 60307.00 P  0.135736 0.011735  0.213747 0.017023  P-0.0051474 0.0147387                                                                                                             
+231230 60308.00 P  0.133429 0.011771  0.213943 0.017090  P-0.0046025 0.0148008                                                                                                             
+231231 60309.00 P  0.131130 0.011808  0.214174 0.017156  P-0.0042009 0.0148629                                                                                                             
+24 1 1 60310.00 P  0.128839 0.011844  0.214441 0.017223  P-0.0039485 0.0149248                                                                                                             
+24 1 2 60311.00 P  0.126557 0.011880  0.214744 0.017290  P-0.0038257 0.0149867                                                                                                             
+24 1 3 60312.00 P  0.124283 0.011916  0.215082 0.017356  P-0.0037920 0.0150484                                                                                                             
+24 1 4 60313.00 P  0.122020 0.011952  0.215456 0.017423  P-0.0037940 0.0151101                                                                                                             
+24 1 5 60314.00 P  0.119766 0.011988  0.215864 0.017489  P-0.0037716 0.0151717                                                                                                             
+24 1 6 60315.00 P  0.117524 0.012024  0.216308 0.017555  P-0.0036647 0.0152332                                                                                                             
+24 1 7 60316.00 P  0.115293 0.012060  0.216785 0.017621  P-0.0034202 0.0152946                                                                                                             
+24 1 8 60317.00 P  0.113074 0.012096  0.217298 0.017687  P-0.0030044 0.0153560                                                                                                             
+24 1 9 60318.00 P  0.110867 0.012132  0.217844 0.017753  P-0.0024217 0.0154172                                                                                                             
+24 110 60319.00 P  0.108674 0.012167  0.218425 0.017819  P-0.0017310 0.0154784                                                                                                             
+24 111 60320.00 P  0.106495 0.012203  0.219039 0.017885  P-0.0010472 0.0155395                                                                                                             
+24 112 60321.00 P  0.104330 0.012238  0.219687 0.017951  P-0.0005165 0.0156005                                                                                                             
+24 113 60322.00 P  0.102180 0.012274  0.220368 0.018016  P-0.0002705 0.0156614                                                                                                             
+24 114 60323.00 P  0.100046 0.012309  0.221082 0.018082  P-0.0003770 0.0157223                                                                                                             
+24 115 60324.00 P  0.097928 0.012344  0.221829 0.018147  P-0.0008118 0.0157831                                                                                                             
+24 116 60325.00 P  0.095826 0.012379  0.222609 0.018212  P-0.0014639 0.0158438                                                                                                             
+24 117 60326.00 P  0.093742 0.012414  0.223421 0.018277  P-0.0021729 0.0159044                                                                                                             
+24 118 60327.00 P  0.091676 0.012449  0.224264 0.018343  P-0.0027782 0.0159649                                                                                                             
+24 119 60328.00 P  0.089627 0.012484  0.225140 0.018408  P-0.0031608 0.0160254                                                                                                             
+24 120 60329.00 P  0.087598 0.012519  0.226046 0.018472  P-0.0032632 0.0160858                                                                                                             
+24 121 60330.00 P  0.085587 0.012554  0.226984 0.018537  P-0.0030878 0.0161461                                                                                                             
+24 122 60331.00 P  0.083597 0.012588  0.227952 0.018602  P-0.0026809 0.0162063                                                                                                             
+24 123 60332.00 P  0.081627 0.012623  0.228951 0.018667  P-0.0021151 0.0162665                                                                                                             
+24 124 60333.00 P  0.079678 0.012658  0.229979 0.018731  P-0.0014733 0.0163265                                                                                                             
+24 125 60334.00 P  0.077750 0.012692  0.231037 0.018796  P-0.0008383 0.0163866                                                                                                             
+24 126 60335.00 P  0.075844 0.012727  0.232125 0.018860  P-0.0002840 0.0164465                                                                                                             
+24 127 60336.00 P  0.073960 0.012761  0.233241 0.018924  P 0.0001320 0.0165063                                                                                                             
+24 128 60337.00 P  0.072099 0.012795  0.234387 0.018989  P 0.0003786 0.0165661                                                                                                             
+24 129 60338.00 P  0.070262 0.012829  0.235560 0.019053  P 0.0004582 0.0166258                                                                                                             
+24 130 60339.00 P  0.068448 0.012864  0.236761 0.019117  P 0.0004032 0.0166855                                                                                                             
+24 131 60340.00 P  0.066658 0.012898  0.237989 0.019181  P 0.0002685 0.0167451                                                                                                             
+24 2 1 60341.00 P  0.064893 0.012932  0.239245 0.019245  P 0.0001236 0.0168046                                                                                                             
+24 2 2 60342.00 P  0.063153 0.012966  0.240527 0.019309  P 0.0000344 0.0168640                                                                                                             
+24 2 3 60343.00 P  0.061438 0.012999  0.241835 0.019372  P 0.0000600 0.0169233                                                                                                             
+24 2 4 60344.00 P  0.059749 0.013033  0.243170 0.019436  P 0.0002578 0.0169826                                                                                                             
+24 2 5 60345.00 P  0.058087 0.013067  0.244529 0.019500  P 0.0006525 0.0170419                                                                                                             
+24 2 6 60346.00 P  0.056451 0.013101  0.245914 0.019563  P 0.0012055 0.0171010                                                                                                             
+24 2 7 60347.00 P  0.054843 0.013134  0.247323 0.019626  P 0.0018305 0.0171601                                                                                                             
+24 2 8 60348.00 P  0.053262 0.013168  0.248756 0.019690  P 0.0023744 0.0172191                                                                                                             
+24 2 9 60349.00 P  0.051709 0.013201  0.250212 0.019753  P 0.0027402 0.0172780                                                                                                             
+24 210 60350.00 P  0.050184 0.013235  0.251692 0.019816  P 0.0027198 0.0173369                                                                                                             
+24 211 60351.00 P  0.048688 0.013268  0.253194 0.019879  P 0.0023815 0.0173957                                                                                                             
+24 212 60352.00 P  0.047220 0.013301  0.254719 0.019942  P 0.0017373 0.0174545                                                                                                             
+24 213 60353.00 P  0.045783 0.013334  0.256266 0.020005  P 0.0009154 0.0175131                                                                                                             
+24 214 60354.00 P  0.044374 0.013368  0.257833 0.020068  P 0.0001188 0.0175718                                                                                                             
+24 215 60355.00 P  0.042996 0.013401  0.259422 0.020131  P-0.0005232 0.0176303                                                                                                             
+24 216 60356.00 P  0.041648 0.013434  0.261031 0.020194  P-0.0009496 0.0176888                                                                                                             
+24 217 60357.00 P  0.040331 0.013467  0.262659 0.020256  P-0.0011021 0.0177472                                                                                                             
+24 218 60358.00 P  0.039045 0.013500  0.264307 0.020319  P-0.0010470 0.0178055                                                                                                             
+24 219 60359.00 P  0.037790 0.013533  0.265974 0.020381  P-0.0008161 0.0178638                                                                                                             
+24 220 60360.00 P  0.036566 0.013565  0.267659 0.020444  P-0.0005409 0.0179220                                                                                                             
+24 221 60361.00 P  0.035374 0.013598  0.269362 0.020506  P-0.0003259 0.0179802                                                                                                             
+24 222 60362.00 P  0.034215 0.013631  0.271083 0.020568  P-0.0001535 0.0180383                                                                                                             
+24 223 60363.00 P  0.033087 0.013663  0.272820 0.020630  P-0.0001755 0.0180963                                                                                                             
+24 224 60364.00 P  0.031992 0.013696  0.274573 0.020693  P-0.0003885 0.0181543                                                                                                             
+24 225 60365.00 P  0.030930 0.013728  0.276342 0.020755  P-0.0007466 0.0182122                                                                                                             
+24 226 60366.00 P  0.029901 0.013761  0.278126 0.020817  P-0.0012520 0.0182700                                                                                                             
+24 227 60367.00 P  0.028905 0.013793  0.279925 0.020878  P-0.0018323 0.0183278                                                                                                             
+24 228 60368.00 P  0.027943 0.013826  0.281738 0.020940  P-0.0024246 0.0183855                                                                                                             
+24 229 60369.00 P  0.027014 0.013858  0.283565 0.021002  P-0.0029667 0.0184432                                                                                                             
+24 3 1 60370.00 P  0.026119 0.013890  0.285405 0.021064  P-0.0034069 0.0185008                                                                                                             
+24 3 2 60371.00 P  0.025258 0.013922  0.287257 0.021125  P-0.0037211 0.0185583                                                                                                             
+24 3 3 60372.00 P  0.024431 0.013954  0.289122 0.021187  P-0.0039762 0.0186158                                                                                                             
+24 3 4 60373.00 P  0.023639 0.013986  0.290997 0.021248  P-0.0040419 0.0186732                                                                                                             
+24 3 5 60374.00 P  0.022881 0.014018  0.292884 0.021310  P-0.0040144 0.0187306                                                                                                             
+24 3 6 60375.00 P  0.022157 0.014050  0.294781 0.021371  P-0.0040288 0.0187879                                                                                                             
+24 3 7 60376.00 P  0.021469 0.014082  0.296688 0.021432  P-0.0041950 0.0188451                                                                                                             
+24 3 8 60377.00 P  0.020815 0.014114  0.298604 0.021494  P-0.0047087 0.0189023                                                                                                             
+24 3 9 60378.00 P  0.020196 0.014146  0.300529 0.021555  P-0.0055651 0.0189594                                                                                                             
+24 310 60379.00 P  0.019612 0.014177  0.302461 0.021616  P-0.0066588 0.0190165                                                                                                             
+24 311 60380.00 P  0.019063 0.014209  0.304402 0.021677  P-0.0078993 0.0190735                                                                                                             
+24 312 60381.00 P  0.018549 0.014241  0.306349 0.021738  P-0.0091442 0.0191305                                                                                                             
+24 313 60382.00 P  0.018071 0.014272  0.308303 0.021799  P-0.0102350 0.0191874                                                                                                             
+24 314 60383.00 P  0.017628 0.014304  0.310263 0.021859  P-0.0111080 0.0192442                                                                                                             
+24 315 60384.00 P  0.017220 0.014335  0.312228 0.021920  P-0.0116511 0.0193010                                                                                                             
+24 316 60385.00 P  0.016848 0.014367  0.314198 0.021981  P-0.0118926 0.0193577                                                                                                             
+24 317 60386.00 P  0.016511 0.014398  0.316172 0.022041  P-0.0120014 0.0194144                                                                                                             
+24 318 60387.00 P  0.016210 0.014429  0.318150 0.022102  P-0.0120441 0.0194710                                                                                                             
+24 319 60388.00 P  0.015944 0.014461  0.320131 0.022162  P-0.0121014 0.0195276                                                                                                             
+24 320 60389.00 P  0.015714 0.014492  0.322114 0.022223  P-0.0122907 0.0195841                                                                                                             
+24 321 60390.00 P  0.015518 0.014523  0.324099 0.022283  P-0.0125971 0.0196405                                                                                                             
+24 322 60391.00 P  0.015359 0.014554  0.326086 0.022343  P-0.0130399 0.0196969                                                                                                             
+24 323 60392.00 P  0.015235 0.014585  0.328073 0.022404  P-0.0136785 0.0197532                                                                                                             
+24 324 60393.00 P  0.015146 0.014616  0.330061 0.022464  P-0.0144782 0.0198095                                                                                                             
+24 325 60394.00 P  0.015092 0.014647  0.332049 0.022524  P-0.0153933 0.0198658                                                                                                             
+24 326 60395.00 P  0.015073 0.014678  0.334035 0.022584  P-0.0163203 0.0199219                                                                                                             
+24 327 60396.00 P  0.015090 0.014709  0.336021 0.022644  P-0.0170935 0.0199781                                                                                                             
+24 328 60397.00 P  0.015142 0.014740  0.338004 0.022704  P-0.0177137 0.0200341                                                                                                             
+24 329 60398.00 P  0.015228 0.014770  0.339985 0.022764  P-0.0180902 0.0200902                                                                                                             
+24 330 60399.00 P  0.015350 0.014801  0.341963 0.022823  P-0.0182043 0.0201461                                                                                                             
+24 331 60400.00 P  0.015506 0.014832  0.343937 0.022883  P-0.0181614 0.0202021                                                                                                             
+24 4 1 60401.00 P  0.015697 0.014862  0.345907 0.022943  P-0.0179874 0.0202579                                                                                                             
+24 4 2 60402.00 P  0.015922 0.014893  0.347872 0.023002  P-0.0177880 0.0203137                                                                                                             
+24 4 3 60403.00 P  0.016181 0.014923  0.349832 0.023062  P-0.0176253 0.0203695                                                                                                             
+24 4 4 60404.00 P  0.016475 0.014954  0.351787 0.023121  P-0.0176564 0.0204252                                                                                                             
+24 4 5 60405.00 P  0.016803 0.014984  0.353735 0.023181  P-0.0179428 0.0204809                                                                                                             
+24 4 6 60406.00 P  0.017164 0.015015  0.355676 0.023240  P-0.0185541 0.0205365                                                                                                             
+24 4 7 60407.00 P  0.017560 0.015045  0.357610 0.023300  P-0.0194494 0.0205920                                                                                                             
+24 4 8 60408.00 P  0.017988 0.015075  0.359536 0.023359  P-0.0205158 0.0206475                                                                                                             
+24 4 9 60409.00 P  0.018450 0.015105  0.361453 0.023418  P-0.0215665 0.0207030                                                                                                             
+24 410 60410.00 P  0.018945 0.015136  0.363362 0.023477  P-0.0223658 0.0207584                                                                                                             
+24 411 60411.00 P  0.019473 0.015166  0.365261 0.023536  P-0.0227716 0.0208138                                                                                                             
+24 412 60412.00 P  0.020034 0.015196  0.367150 0.023595  P-0.0228705 0.0208691                                                                                                             
+24 413 60413.00 P  0.020626 0.015226  0.369028 0.023654  P-0.0227029 0.0209243                                                                                                             
+24 414 60414.00 P  0.021251 0.015256  0.370896 0.023713  P-0.0223427 0.0209795                                                                                                             
+24 415 60415.00 P  0.021908 0.015286  0.372752 0.023772  P-0.0219602 0.0210347                                                                                                             
+24 416 60416.00 P  0.022597 0.015316  0.374597 0.023831  P-0.0215444 0.0210898                                                                                                             
+24 417 60417.00 P  0.023316 0.015346  0.376428 0.023889  P-0.0211981 0.0211449                                                                                                             
+24 418 60418.00 P  0.024067 0.015375  0.378247 0.023948  P-0.0210587 0.0211999                                                                                                             
+24 419 60419.00 P  0.024849 0.015405  0.380052 0.024007  P-0.0210795 0.0212548                                                                                                             
+24 420 60420.00 P  0.025661 0.015435  0.381844 0.024065  P-0.0212858 0.0213098                                                                                                             
+24 421 60421.00 P  0.026503 0.015465  0.383621 0.024124  P-0.0215999 0.0213646                                                                                                             
+24 422 60422.00 P  0.027375 0.015494  0.385383 0.024182  P-0.0219208 0.0214195                                                                                                             
+24 423 60423.00 P  0.028277 0.015524  0.387130 0.024241  P-0.0223019 0.0214742                                                                                                             
+24 424 60424.00 P  0.029208 0.015554  0.388861 0.024299  P-0.0226479 0.0215290                                                                                                             
+24 425 60425.00 P  0.030167 0.015583  0.390576 0.024357  P-0.0228311 0.0215837                                                                                                             
+24 426 60426.00 P  0.031156 0.015613  0.392274 0.024416  P-0.0229005 0.0216383                                                                                                             
+24 427 60427.00 P  0.032172 0.015642  0.393955 0.024474  P-0.0227289 0.0216929                                                                                                             
+24 428 60428.00 P  0.033216 0.015671  0.395618 0.024532  P-0.0224796 0.0217474                                                                                                             
+24 429 60429.00 P  0.034288 0.015701  0.397264 0.024590  P-0.0221471 0.0218019                                                                                                             
+24 430 60430.00 P  0.035387 0.015730  0.398891 0.024648  P-0.0218847 0.0218564                                                                                                             
+24 5 1 60431.00 P  0.036513 0.015759  0.400499 0.024706  P-0.0217604 0.0219108                                                                                                             
+24 5 2 60432.00 P  0.037664 0.015789  0.402088 0.024764  P-0.0219139 0.0219652                                                                                                             
+24 5 3 60433.00 P  0.038842 0.015818  0.403657 0.024822  P-0.0223827 0.0220195                                                                                                             
+24 5 4 60434.00 P  0.040045 0.015847  0.405207 0.024880  P-0.0231367 0.0220738                                                                                                             
+24 5 5 60435.00 P  0.041274 0.015876  0.406736 0.024937  P-0.0240471 0.0221280                                                                                                             
+24 5 6 60436.00 P  0.042527 0.015905  0.408244 0.024995  P-0.0250577 0.0221822                                                                                                             
+24 5 7 60437.00 P  0.043804 0.015934  0.409731 0.025053  P-0.0258676 0.0222363                                                                                                             
+24 5 8 60438.00 P  0.045105 0.015963  0.411196 0.025110  P-0.0263687 0.0222904                                                                                                             
+24 5 9 60439.00 P  0.046430 0.015992  0.412639 0.025168  P-0.0265455 0.0223444                                                                                                             
+24 510 60440.00 P  0.047778 0.016021  0.414061 0.025225  P-0.0263766 0.0223985                                                                                                             
+24 511 60441.00 P  0.049148 0.016050  0.415459 0.025283  P-0.0259482 0.0224524                                                                                                             
+24 512 60442.00 P  0.050540 0.016079  0.416835 0.025340  P-0.0253742 0.0225063                                                                                                             
+24 513 60443.00 P  0.051954 0.016108  0.418187 0.025398  P-0.0247707 0.0225602                                                                                                             
+24 514 60444.00 P  0.053389 0.016136  0.419516 0.025455  P-0.0241617 0.0226140                                                                                                             
+24 515 60445.00 P  0.054845 0.016165  0.420820 0.025512  P-0.0236615 0.0226678                                                                                                             
+24 516 60446.00 P  0.056321 0.016194  0.422101 0.025569  P-0.0233136 0.0227216                                                                                                             
+24 517 60447.00 P  0.057817 0.016222  0.423357 0.025626  P-0.0230901 0.0227753                                                                                                             
+24 518 60448.00 P  0.059332 0.016251  0.424588 0.025684  P-0.0229512 0.0228290                                                                                                             
+24 519 60449.00 P  0.060866 0.016280  0.425794 0.025741  P-0.0229156 0.0228826                                                                                                             
+24 520 60450.00 P  0.062418 0.016308  0.426974 0.025798  P-0.0229285 0.0229362                                                                                                             
+24 521 60451.00 P  0.063988 0.016337  0.428129 0.025855  P-0.0227426 0.0229897                                                                                                             
+24 522 60452.00 P  0.065575 0.016365  0.429258 0.025911  P-0.0223712 0.0230432                                                                                                             
+24 523 60453.00 P  0.067179 0.016394  0.430360 0.025968  P-0.0217314 0.0230966                                                                                                             
+24 524 60454.00 P  0.068799 0.016422  0.431437 0.026025  P-0.0209410 0.0231500                                                                                                             
+24 525 60455.00 P  0.070436 0.016450  0.432486 0.026082  P-0.0199205 0.0232034                                                                                                             
+24 526 60456.00 P  0.072087 0.016479  0.433508 0.026139  P-0.0188750 0.0232567                                                                                                             
+24 527 60457.00 P  0.073753 0.016507  0.434504 0.026195  P-0.0178365 0.0233100                                                                                                             
+24 528 60458.00 P  0.075434 0.016535  0.435472 0.026252  P-0.0169537 0.0233633                                                                                                             
+24 529 60459.00 P  0.077128 0.016563  0.436412 0.026308  P-0.0163617 0.0234165                                                                                                             
+24 530 60460.00 P  0.078835 0.016591  0.437325 0.026365  P-0.0161455 0.0234697                                                                                                             
+24 531 60461.00 P  0.080555 0.016620  0.438209 0.026421  P-0.0162581 0.0235228                                                                                                             
+24 6 1 60462.00 P  0.082287 0.016648  0.439066 0.026478  P-0.0165977 0.0235759                                                                                                             
+24 6 2 60463.00 P  0.084031 0.016676  0.439894 0.026534  P-0.0170058 0.0236289                                                                                                             
+24 6 3 60464.00 P  0.085786 0.016704  0.440694 0.026591  P-0.0172917 0.0236819                                                                                                             
+24 6 4 60465.00 P  0.087551 0.016732  0.441465 0.026647  P-0.0173163 0.0237349                                                                                                             
+24 6 5 60466.00 P  0.089326 0.016760  0.442207 0.026703  P-0.0170135 0.0237878                                                                                                             
+24 6 6 60467.00 P  0.091111 0.016788  0.442920 0.026759  P-0.0163848 0.0238407                                                                                                             
+24 6 7 60468.00 P  0.092905 0.016815  0.443605 0.026815  P-0.0155439 0.0238935                                                                                                             
+24 6 8 60469.00 P  0.094707 0.016843  0.444260 0.026871  P-0.0145027 0.0239463                                                                                                             
+24 6 9 60470.00 P  0.096517 0.016871  0.444886 0.026928  P-0.0134644 0.0239991                                                                                                             
+24 610 60471.00 P  0.098334 0.016899  0.445482 0.026984  P-0.0125040 0.0240518                                                                                                             
+24 611 60472.00 P  0.100158 0.016927  0.446049 0.027040  P-0.0116879 0.0241045                                                                                                             
+24 612 60473.00 P  0.101987 0.016954  0.446586 0.027095  P-0.0109619 0.0241572                                                                                                             
+24 613 60474.00 P  0.103823 0.016982  0.447094 0.027151  P-0.0104223 0.0242098                                                                                                             
+24 614 60475.00 P  0.105664 0.017010  0.447572 0.027207  P-0.0099404 0.0242624                                                                                                             
+24 615 60476.00 P  0.107509 0.017037  0.448020 0.027263  P-0.0094981 0.0243149                                                                                                             
+24 616 60477.00 P  0.109358 0.017065  0.448439 0.027319  P-0.0091346 0.0243674                                                                                                             
+24 617 60478.00 P  0.111210 0.017092  0.448827 0.027374  P-0.0087392 0.0244199                                                                                                             
+24 618 60479.00 P  0.113065 0.017120  0.449186 0.027430  P-0.0081597 0.0244723                                                                                                             
+24 619 60480.00 P  0.114923 0.017147  0.449515 0.027486  P-0.0073387 0.0245247                                                                                                             
+24 620 60481.00 P  0.116782 0.017175  0.449814 0.027541  P-0.0063143 0.0245770                                                                                                             
+24 621 60482.00 P  0.118643 0.017202  0.450083 0.027597  P-0.0050560 0.0246293                                                                                                             
+24 622 60483.00 P  0.120504 0.017230  0.450322 0.027652  P-0.0036612 0.0246816                                                                                                             
+24 623 60484.00 P  0.122365 0.017257  0.450531 0.027708  P-0.0022432 0.0247338                                                                                                             
+24 624 60485.00 P  0.124226 0.017284  0.450710 0.027763  P-0.0008760 0.0247860                                                                                                             
+24 625 60486.00 P  0.126086 0.017311  0.450859 0.027818  P 0.0002637 0.0248382                                                                                                             
+24 626 60487.00 P  0.127944 0.017339  0.450979 0.027874  P 0.0011461 0.0248903                                                                                                             
+24 627 60488.00 P  0.129800 0.017366  0.451068 0.027929  P 0.0016995 0.0249424                                                                                                             
+24 628 60489.00 P  0.131654 0.017393  0.451128 0.027984  P 0.0020595 0.0249945                                                                                                             
+24 629 60490.00 P  0.133504 0.017420  0.451159 0.028039  P 0.0023180 0.0250465                                                                                                             
+24 630 60491.00 P  0.135351 0.017447  0.451159 0.028095  P 0.0027166 0.0250985                                                                                                             
+24 7 1 60492.00 P  0.137193 0.017474  0.451131 0.028150  P 0.0032031 0.0251504                                                                                                             
+24 7 2 60493.00 P  0.139031 0.017501  0.451073 0.028205  P 0.0039895 0.0252023                                                                                                             
+24 7 3 60494.00 P  0.140863 0.017529  0.450985 0.028260  P 0.0051112 0.0252542                                                                                                             
+24 7 4 60495.00 P  0.142690 0.017556  0.450868 0.028315  P 0.0064348 0.0253060                                                                                                             
+24 7 5 60496.00 P  0.144510 0.017582  0.450723 0.028370  P 0.0078953 0.0253578                                                                                                             
+24 7 6 60497.00 P  0.146323 0.017609  0.450548 0.028424  P 0.0093703 0.0254096                                                                                                             
 24 7 7 60498.00                                                                                                                                                                            
 24 7 8 60499.00                                                                                                                                                                            
 24 7 9 60500.00                                                                                                                                                                            
 24 710 60501.00                                                                                                                                                                            
 24 711 60502.00                                                                                                                                                                            
 24 712 60503.00                                                                                                                                                                            
 24 713 60504.00                                                                                                                                                                            
@@ -18823,7 +18823,42 @@
 24 715 60506.00                                                                                                                                                                            
 24 716 60507.00                                                                                                                                                                            
 24 717 60508.00                                                                                                                                                                            
 24 718 60509.00                                                                                                                                                                            
 24 719 60510.00                                                                                                                                                                            
 24 720 60511.00                                                                                                                                                                            
 24 721 60512.00                                                                                                                                                                            
+24 722 60513.00                                                                                                                                                                            
+24 723 60514.00                                                                                                                                                                            
+24 724 60515.00                                                                                                                                                                            
+24 725 60516.00                                                                                                                                                                            
+24 726 60517.00                                                                                                                                                                            
+24 727 60518.00                                                                                                                                                                            
+24 728 60519.00                                                                                                                                                                            
+24 729 60520.00                                                                                                                                                                            
+24 730 60521.00                                                                                                                                                                            
+24 731 60522.00                                                                                                                                                                            
+24 8 1 60523.00                                                                                                                                                                            
+24 8 2 60524.00                                                                                                                                                                            
+24 8 3 60525.00                                                                                                                                                                            
+24 8 4 60526.00                                                                                                                                                                            
+24 8 5 60527.00                                                                                                                                                                            
+24 8 6 60528.00                                                                                                                                                                            
+24 8 7 60529.00                                                                                                                                                                            
+24 8 8 60530.00                                                                                                                                                                            
+24 8 9 60531.00                                                                                                                                                                            
+24 810 60532.00                                                                                                                                                                            
+24 811 60533.00                                                                                                                                                                            
+24 812 60534.00                                                                                                                                                                            
+24 813 60535.00                                                                                                                                                                            
+24 814 60536.00                                                                                                                                                                            
+24 815 60537.00                                                                                                                                                                            
+24 816 60538.00                                                                                                                                                                            
+24 817 60539.00                                                                                                                                                                            
+24 818 60540.00                                                                                                                                                                            
+24 819 60541.00                                                                                                                                                                            
+24 820 60542.00                                                                                                                                                                            
+24 821 60543.00                                                                                                                                                                            
+24 822 60544.00                                                                                                                                                                            
+24 823 60545.00                                                                                                                                                                            
+24 824 60546.00                                                                                                                                                                            
+24 825 60547.00
```

### Comparing `pyTMD-2.0.5/pyTMD/data/historic_deltat.data` & `pyTMD-2.0.6/pyTMD/data/historic_deltat.data`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/data/iers_deltat.data` & `pyTMD-2.0.6/pyTMD/data/iers_deltat.data`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/data/leap-seconds.list` & `pyTMD-2.0.6/pyTMD/data/leap-seconds.list`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/data/mean-pole.tab` & `pyTMD-2.0.6/pyTMD/data/mean-pole.tab`

 * *Files 1% similar despite different names*

```diff
@@ -2109,359 +2109,361 @@
 2005.40   0.0583695   0.3448657
 2005.45   0.0585648   0.3449049
 2005.50   0.0587615   0.3449429
 2005.55   0.0589594   0.3449797
 2005.60   0.0591588   0.3450154
 2005.65   0.0593595   0.3450499
 2005.70   0.0595615   0.3450833
-2005.75   0.0597648   0.3451154
+2005.75   0.0597648   0.3451155
 2005.80   0.0599695   0.3451465
 2005.85   0.0601755   0.3451764
 2005.90   0.0603828   0.3452051
 2005.95   0.0605915   0.3452327
 2006.00   0.0608014   0.3452592
 2006.05   0.0610127   0.3452846
-2006.10   0.0612252   0.3453088
+2006.10   0.0612252   0.3453089
 2006.15   0.0614390   0.3453320
 2006.20   0.0616541   0.3453541
 2006.25   0.0618705   0.3453751
 2006.30   0.0620881   0.3453950
 2006.35   0.0623070   0.3454139
 2006.40   0.0625270   0.3454317
 2006.45   0.0627483   0.3454485
 2006.50   0.0629709   0.3454644
 2006.55   0.0631946   0.3454792
-2006.60   0.0634194   0.3454930
-2006.65   0.0636455   0.3455059
+2006.60   0.0634194   0.3454931
+2006.65   0.0636455   0.3455060
 2006.70   0.0638726   0.3455179
 2006.75   0.0641010   0.3455290
 2006.80   0.0643304   0.3455391
 2006.85   0.0645609   0.3455484
-2006.90   0.0647925   0.3455568
-2006.95   0.0650252   0.3455644
+2006.90   0.0647925   0.3455569
+2006.95   0.0650252   0.3455645
 2007.00   0.0652589   0.3455712
-2007.05   0.0654936   0.3455772
+2007.05   0.0654936   0.3455773
 2007.10   0.0657294   0.3455825
 2007.15   0.0659661   0.3455870
 2007.20   0.0662038   0.3455908
-2007.25   0.0664424   0.3455939
+2007.25   0.0664424   0.3455940
 2007.30   0.0666819   0.3455964
-2007.35   0.0669224   0.3455982
+2007.35   0.0669224   0.3455983
 2007.40   0.0671637   0.3455995
-2007.45   0.0674059   0.3456001
+2007.45   0.0674059   0.3456002
 2007.50   0.0676489   0.3456003
 2007.55   0.0678927   0.3455999
 2007.60   0.0681374   0.3455990
-2007.65   0.0683827   0.3455976
-2007.70   0.0686288   0.3455959
+2007.65   0.0683827   0.3455977
+2007.70   0.0686289   0.3455959
 2007.75   0.0688757   0.3455937
 2007.80   0.0691232   0.3455912
-2007.85   0.0693714   0.3455883
-2007.90   0.0696202   0.3455851
-2007.95   0.0698697   0.3455817
+2007.85   0.0693714   0.3455884
+2007.90   0.0696202   0.3455852
+2007.95   0.0698697   0.3455818
 2008.00   0.0701197   0.3455781
 2008.05   0.0703703   0.3455742
-2008.10   0.0706214   0.3455701
+2008.10   0.0706214   0.3455702
 2008.15   0.0708731   0.3455660
-2008.20   0.0711252   0.3455617
-2008.25   0.0713778   0.3455573
+2008.20   0.0711252   0.3455618
+2008.25   0.0713778   0.3455574
 2008.30   0.0716309   0.3455530
 2008.35   0.0718843   0.3455486
-2008.40   0.0721382   0.3455442
-2008.45   0.0723924   0.3455399
-2008.50   0.0726469   0.3455357
-2008.55   0.0729018   0.3455316
-2008.60   0.0731569   0.3455277
-2008.65   0.0734123   0.3455240
-2008.70   0.0736679   0.3455205
-2008.75   0.0739238   0.3455173
-2008.80   0.0741798   0.3455143
-2008.85   0.0744359   0.3455118
-2008.90   0.0746923   0.3455095
-2008.95   0.0749487   0.3455077
-2009.00   0.0752052   0.3455063
-2009.05   0.0754617   0.3455053
-2009.10   0.0757183   0.3455048
-2009.15   0.0759750   0.3455049
-2009.20   0.0762316   0.3455055
-2009.25   0.0764882   0.3455067
-2009.30   0.0767447   0.3455085
-2009.35   0.0770011   0.3455109
-2009.40   0.0772575   0.3455140
-2009.45   0.0775137   0.3455178
-2009.50   0.0777698   0.3455223
-2009.55   0.0780258   0.3455276
-2009.60   0.0782815   0.3455337
-2009.65   0.0785371   0.3455406
-2009.70   0.0787924   0.3455483
-2009.75   0.0790476   0.3455568
-2009.80   0.0793024   0.3455663
-2009.85   0.0795570   0.3455766
-2009.90   0.0798113   0.3455879
-2009.95   0.0800653   0.3456001
-2010.00   0.0803190   0.3456133
-2010.05   0.0805723   0.3456274
-2010.10   0.0808253   0.3456426
-2010.15   0.0810779   0.3456588
-2010.20   0.0813301   0.3456761
-2010.25   0.0815820   0.3456944
-2010.30   0.0818334   0.3457138
-2010.35   0.0820844   0.3457343
-2010.40   0.0823350   0.3457560
-2010.45   0.0825851   0.3457787
-2010.50   0.0828348   0.3458026
-2010.55   0.0830840   0.3458276
-2010.60   0.0833328   0.3458538
-2010.65   0.0835810   0.3458811
-2010.70   0.0838288   0.3459097
-2010.75   0.0840761   0.3459394
-2010.80   0.0843228   0.3459703
-2010.85   0.0845691   0.3460024
-2010.90   0.0848148   0.3460357
-2010.95   0.0850600   0.3460702
-2011.00   0.0853047   0.3461060
-2011.05   0.0855488   0.3461429
-2011.10   0.0857924   0.3461811
-2011.15   0.0860354   0.3462204
-2011.20   0.0862779   0.3462610
-2011.25   0.0865199   0.3463028
-2011.30   0.0867613   0.3463458
-2011.35   0.0870021   0.3463900
-2011.40   0.0872424   0.3464354
-2011.45   0.0874821   0.3464820
-2011.50   0.0877212   0.3465298
-2011.55   0.0879598   0.3465788
-2011.60   0.0881979   0.3466289
-2011.65   0.0884353   0.3466802
-2011.70   0.0886723   0.3467327
-2011.75   0.0889086   0.3467862
-2011.80   0.0891444   0.3468409
-2011.85   0.0893797   0.3468967
-2011.90   0.0896144   0.3469536
-2011.95   0.0898486   0.3470116
-2012.00   0.0900822   0.3470706
-2012.05   0.0903153   0.3471307
-2012.10   0.0905478   0.3471918
-2012.15   0.0907798   0.3472540
-2012.20   0.0910113   0.3473171
-2012.25   0.0912422   0.3473811
-2012.30   0.0914727   0.3474461
-2012.35   0.0917026   0.3475121
-2012.40   0.0919320   0.3475789
-2012.45   0.0921610   0.3476466
-2012.50   0.0923894   0.3477152
-2012.55   0.0926173   0.3477846
-2012.60   0.0928448   0.3478547
-2012.65   0.0930717   0.3479257
-2012.70   0.0932982   0.3479974
-2012.75   0.0935242   0.3480698
-2012.80   0.0937498   0.3481429
-2012.85   0.0939749   0.3482167
-2012.90   0.0941996   0.3482911
-2012.95   0.0944238   0.3483661
-2013.00   0.0946476   0.3484416
-2013.05   0.0948709   0.3485177
-2013.10   0.0950939   0.3485943
-2013.15   0.0953164   0.3486714
-2013.20   0.0955385   0.3487489
-2013.25   0.0957602   0.3488269
-2013.30   0.0959815   0.3489052
-2013.35   0.0962024   0.3489838
-2013.40   0.0964229   0.3490628
-2013.45   0.0966431   0.3491420
-2013.50   0.0968628   0.3492215
-2013.55   0.0970822   0.3493012
-2013.60   0.0973012   0.3493810
-2013.65   0.0975199   0.3494610
-2013.70   0.0977382   0.3495412
-2013.75   0.0979562   0.3496213
-2013.80   0.0981738   0.3497015
-2013.85   0.0983911   0.3497818
-2013.90   0.0986080   0.3498619
-2013.95   0.0988246   0.3499420
-2014.00   0.0990409   0.3500221
-2014.05   0.0992569   0.3501019
-2014.10   0.0994725   0.3501816
-2014.15   0.0996878   0.3502611
-2014.20   0.0999028   0.3503404
-2014.25   0.1001174   0.3504194
-2014.30   0.1003318   0.3504980
-2014.35   0.1005458   0.3505764
-2014.40   0.1007595   0.3506543
-2014.45   0.1009729   0.3507319
-2014.50   0.1011860   0.3508090
-2014.55   0.1013988   0.3508857
-2014.60   0.1016112   0.3509618
-2014.65   0.1018234   0.3510374
-2014.70   0.1020352   0.3511125
-2014.75   0.1022467   0.3511869
-2014.80   0.1024579   0.3512607
-2014.85   0.1026688   0.3513339
-2014.90   0.1028794   0.3514064
-2014.95   0.1030896   0.3514782
-2015.00   0.1032995   0.3515492
-2015.05   0.1035090   0.3516195
-2015.10   0.1037183   0.3516889
-2015.15   0.1039272   0.3517576
-2015.20   0.1041357   0.3518254
-2015.25   0.1043439   0.3518923
-2015.30   0.1045517   0.3519583
-2015.35   0.1047592   0.3520234
-2015.40   0.1049663   0.3520876
-2015.45   0.1051730   0.3521508
-2015.50   0.1053794   0.3522129
-2015.55   0.1055853   0.3522741
-2015.60   0.1057909   0.3523343
-2015.65   0.1059960   0.3523934
-2015.70   0.1062008   0.3524514
-2015.75   0.1064051   0.3525083
-2015.80   0.1066090   0.3525641
-2015.85   0.1068124   0.3526188
-2015.90   0.1070154   0.3526724
-2015.95   0.1072180   0.3527247
-2016.00   0.1074201   0.3527759
-2016.05   0.1076216   0.3528259
-2016.10   0.1078228   0.3528747
-2016.15   0.1080234   0.3529223
-2016.20   0.1082235   0.3529687
-2016.25   0.1084230   0.3530138
-2016.30   0.1086221   0.3530576
-2016.35   0.1088206   0.3531002
-2016.40   0.1090185   0.3531415
-2016.45   0.1092159   0.3531816
-2016.50   0.1094127   0.3532203
-2016.55   0.1096089   0.3532577
-2016.60   0.1098045   0.3532938
-2016.65   0.1099994   0.3533286
-2016.70   0.1101938   0.3533621
-2016.75   0.1103875   0.3533943
-2016.80   0.1105805   0.3534251
-2016.85   0.1107729   0.3534546
-2016.90   0.1109645   0.3534827
-2016.95   0.1111555   0.3535095
-2017.00   0.1113458   0.3535350
-2017.05   0.1115353   0.3535591
-2017.10   0.1117241   0.3535819
-2017.15   0.1119122   0.3536033
-2017.20   0.1120995   0.3536233
-2017.25   0.1122860   0.3536421
-2017.30   0.1124717   0.3536594
-2017.35   0.1126566   0.3536755
-2017.40   0.1128407   0.3536902
-2017.45   0.1130239   0.3537035
-2017.50   0.1132063   0.3537155
-2017.55   0.1133878   0.3537262
-2017.60   0.1135685   0.3537355
-2017.65   0.1137482   0.3537436
-2017.70   0.1139271   0.3537503
-2017.75   0.1141050   0.3537556
-2017.80   0.1142821   0.3537597
-2017.85   0.1144581   0.3537625
-2017.90   0.1146332   0.3537640
-2017.95   0.1148074   0.3537641
-2018.00   0.1149805   0.3537630
-2018.05   0.1151527   0.3537607
-2018.10   0.1153238   0.3537570
-2018.15   0.1154940   0.3537521
-2018.20   0.1156631   0.3537460
-2018.25   0.1158311   0.3537386
-2018.30   0.1159981   0.3537299
-2018.35   0.1161641   0.3537201
-2018.40   0.1163289   0.3537090
-2018.45   0.1164927   0.3536967
-2018.50   0.1166553   0.3536833
-2018.55   0.1168169   0.3536686
-2018.60   0.1169773   0.3536528
-2018.65   0.1171366   0.3536358
-2018.70   0.1172947   0.3536176
-2018.75   0.1174517   0.3535983
-2018.80   0.1176075   0.3535779
-2018.85   0.1177622   0.3535563
-2018.90   0.1179157   0.3535336
-2018.95   0.1180679   0.3535099
-2019.00   0.1182190   0.3534850
-2019.05   0.1183688   0.3534590
-2019.10   0.1185175   0.3534320
-2019.15   0.1186649   0.3534040
-2019.20   0.1188111   0.3533749
-2019.25   0.1189560   0.3533447
-2019.30   0.1190997   0.3533136
-2019.35   0.1192421   0.3532814
-2019.40   0.1193833   0.3532482
-2019.45   0.1195232   0.3532141
-2019.50   0.1196618   0.3531790
-2019.55   0.1197991   0.3531429
-2019.60   0.1199352   0.3531058
-2019.65   0.1200699   0.3530679
-2019.70   0.1202034   0.3530289
-2019.75   0.1203355   0.3529891
-2019.80   0.1204664   0.3529484
-2019.85   0.1205959   0.3529068
-2019.90   0.1207241   0.3528643
-2019.95   0.1208510   0.3528209
-2020.00   0.1209766   0.3527767
-2020.05   0.1211008   0.3527316
-2020.10   0.1212237   0.3526857
-2020.15   0.1213453   0.3526390
-2020.20   0.1214655   0.3525915
-2020.25   0.1215844   0.3525431
-2020.30   0.1217019   0.3524940
-2020.35   0.1218181   0.3524441
-2020.40   0.1219330   0.3523934
-2020.45   0.1220465   0.3523420
-2020.50   0.1221587   0.3522898
-2020.55   0.1222695   0.3522368
-2020.60   0.1223790   0.3521832
-2020.65   0.1224871   0.3521288
-2020.70   0.1225939   0.3520738
-2020.75   0.1226993   0.3520180
-2020.80   0.1228034   0.3519615
-2020.85   0.1229061   0.3519044
-2020.90   0.1230075   0.3518466
-2020.95   0.1231075   0.3517882
-2021.00   0.1232062   0.3517291
-2021.05   0.1233035   0.3516693
-2021.10   0.1233995   0.3516090
-2021.15   0.1234941   0.3515480
-2021.20   0.1235874   0.3514864
-2021.25   0.1236794   0.3514243
-2021.30   0.1237700   0.3513615
-2021.35   0.1238593   0.3512981
-2021.40   0.1239473   0.3512342
-2021.45   0.1240339   0.3511697
-2021.50   0.1241192   0.3511047
-2021.55   0.1242032   0.3510391
-2021.60   0.1242858   0.3509730
-2021.65   0.1243672   0.3509063
-2021.70   0.1244472   0.3508392
-2021.75   0.1245259   0.3507715
-2021.80   0.1246033   0.3507033
-2021.85   0.1246794   0.3506346
-2021.90   0.1247542   0.3505654
-2021.95   0.1248277   0.3504958
-2022.00   0.1248999   0.3504256
-2022.05   0.1249709   0.3503550
-2022.10   0.1250405   0.3502840
-2022.15   0.1251089   0.3502125
-2022.20   0.1251760   0.3501405
-2022.25   0.1252418   0.3500682
-2022.30   0.1253064   0.3499953
-2022.35   0.1253697   0.3499221
-2022.40   0.1254317   0.3498485
-2022.45   0.1254925   0.3497744
-2022.50   0.1255521   0.3496999
-2022.55   0.1256104   0.3496251
-2022.60   0.1256675   0.3495498
-2022.65   0.1257234   0.3494742
-2022.70   0.1257780   0.3493982
-2022.75   0.1258314   0.3493218
-2022.80   0.1258837   0.3492451
-2022.85   0.1259347   0.3491680
-2022.90   0.1259845   0.3490906
-2022.95   0.1260331   0.3490128
-2023.00   0.1260805   0.3489347
-2023.05   0.1261268   0.3488562
-2023.10   0.1261719   0.3487775
-2023.15   0.1262158   0.3486984
-2023.20   0.1262585   0.3486190
-2023.25   0.1263001   0.3485392
-2023.30   0.1263405   0.3484592
+2008.40   0.0721382   0.3455443
+2008.45   0.0723924   0.3455400
+2008.50   0.0726469   0.3455358
+2008.55   0.0729018   0.3455317
+2008.60   0.0731569   0.3455278
+2008.65   0.0734123   0.3455241
+2008.70   0.0736679   0.3455206
+2008.75   0.0739238   0.3455174
+2008.80   0.0741798   0.3455145
+2008.85   0.0744360   0.3455119
+2008.90   0.0746923   0.3455097
+2008.95   0.0749487   0.3455079
+2009.00   0.0752052   0.3455065
+2009.05   0.0754617   0.3455055
+2009.10   0.0757184   0.3455051
+2009.15   0.0759750   0.3455051
+2009.20   0.0762316   0.3455058
+2009.25   0.0764882   0.3455070
+2009.30   0.0767447   0.3455088
+2009.35   0.0770011   0.3455112
+2009.40   0.0772575   0.3455143
+2009.45   0.0775137   0.3455182
+2009.50   0.0777698   0.3455227
+2009.55   0.0780258   0.3455280
+2009.60   0.0782815   0.3455341
+2009.65   0.0785371   0.3455410
+2009.70   0.0787925   0.3455487
+2009.75   0.0790476   0.3455573
+2009.80   0.0793024   0.3455668
+2009.85   0.0795570   0.3455772
+2009.90   0.0798113   0.3455885
+2009.95   0.0800653   0.3456007
+2010.00   0.0803190   0.3456139
+2010.05   0.0805723   0.3456282
+2010.10   0.0808253   0.3456434
+2010.15   0.0810779   0.3456597
+2010.20   0.0813301   0.3456770
+2010.25   0.0815820   0.3456953
+2010.30   0.0818334   0.3457148
+2010.35   0.0820844   0.3457354
+2010.40   0.0823350   0.3457570
+2010.45   0.0825851   0.3457798
+2010.50   0.0828348   0.3458038
+2010.55   0.0830840   0.3458289
+2010.60   0.0833328   0.3458551
+2010.65   0.0835810   0.3458826
+2010.70   0.0838288   0.3459112
+2010.75   0.0840760   0.3459410
+2010.80   0.0843228   0.3459720
+2010.85   0.0845690   0.3460042
+2010.90   0.0848148   0.3460376
+2010.95   0.0850600   0.3460722
+2011.00   0.0853046   0.3461080
+2011.05   0.0855487   0.3461451
+2011.10   0.0857923   0.3461834
+2011.15   0.0860354   0.3462229
+2011.20   0.0862778   0.3462636
+2011.25   0.0865198   0.3463055
+2011.30   0.0867611   0.3463487
+2011.35   0.0870020   0.3463930
+2011.40   0.0872422   0.3464386
+2011.45   0.0874819   0.3464854
+2011.50   0.0877211   0.3465333
+2011.55   0.0879596   0.3465825
+2011.60   0.0881976   0.3466328
+2011.65   0.0884351   0.3466843
+2011.70   0.0886720   0.3467369
+2011.75   0.0889083   0.3467907
+2011.80   0.0891441   0.3468457
+2011.85   0.0893794   0.3469017
+2011.90   0.0896140   0.3469589
+2011.95   0.0898482   0.3470171
+2012.00   0.0900818   0.3470764
+2012.05   0.0903148   0.3471368
+2012.10   0.0905473   0.3471982
+2012.15   0.0907793   0.3472606
+2012.20   0.0910107   0.3473241
+2012.25   0.0912417   0.3473885
+2012.30   0.0914721   0.3474538
+2012.35   0.0917020   0.3475202
+2012.40   0.0919313   0.3475874
+2012.45   0.0921602   0.3476555
+2012.50   0.0923886   0.3477245
+2012.55   0.0926164   0.3477943
+2012.60   0.0928438   0.3478649
+2012.65   0.0930707   0.3479364
+2012.70   0.0932972   0.3480086
+2012.75   0.0935231   0.3480815
+2012.80   0.0937486   0.3481552
+2012.85   0.0939736   0.3482295
+2012.90   0.0941982   0.3483045
+2012.95   0.0944223   0.3483801
+2013.00   0.0946460   0.3484563
+2013.05   0.0948693   0.3485330
+2013.10   0.0950921   0.3486103
+2013.15   0.0953145   0.3486881
+2013.20   0.0955365   0.3487664
+2013.25   0.0957581   0.3488451
+2013.30   0.0959793   0.3489242
+2013.35   0.0962001   0.3490037
+2013.40   0.0964204   0.3490835
+2013.45   0.0966404   0.3491637
+2013.50   0.0968601   0.3492441
+2013.55   0.0970793   0.3493247
+2013.60   0.0972981   0.3494056
+2013.65   0.0975166   0.3494866
+2013.70   0.0977348   0.3495678
+2013.75   0.0979525   0.3496491
+2013.80   0.0981700   0.3497305
+2013.85   0.0983870   0.3498119
+2013.90   0.0986037   0.3498934
+2013.95   0.0988201   0.3499748
+2014.00   0.0990361   0.3500561
+2014.05   0.0992518   0.3501374
+2014.10   0.0994672   0.3502185
+2014.15   0.0996822   0.3502995
+2014.20   0.0998969   0.3503803
+2014.25   0.1001113   0.3504609
+2014.30   0.1003253   0.3505412
+2014.35   0.1005390   0.3506212
+2014.40   0.1007523   0.3507010
+2014.45   0.1009654   0.3507803
+2014.50   0.1011781   0.3508593
+2014.55   0.1013905   0.3509379
+2014.60   0.1016025   0.3510161
+2014.65   0.1018142   0.3510938
+2014.70   0.1020256   0.3511709
+2014.75   0.1022367   0.3512476
+2014.80   0.1024474   0.3513237
+2014.85   0.1026578   0.3513992
+2014.90   0.1028678   0.3514741
+2014.95   0.1030775   0.3515484
+2015.00   0.1032868   0.3516220
+2015.05   0.1034958   0.3516949
+2015.10   0.1037044   0.3517671
+2015.15   0.1039126   0.3518386
+2015.20   0.1041205   0.3519093
+2015.25   0.1043280   0.3519792
+2015.30   0.1045351   0.3520483
+2015.35   0.1047418   0.3521166
+2015.40   0.1049482   0.3521840
+2015.45   0.1051541   0.3522506
+2015.50   0.1053596   0.3523162
+2015.55   0.1055647   0.3523810
+2015.60   0.1057694   0.3524448
+2015.65   0.1059736   0.3525076
+2015.70   0.1061774   0.3525695
+2015.75   0.1063807   0.3526304
+2015.80   0.1065836   0.3526903
+2015.85   0.1067859   0.3527492
+2015.90   0.1069878   0.3528071
+2015.95   0.1071893   0.3528639
+2016.00   0.1073902   0.3529196
+2016.05   0.1075905   0.3529743
+2016.10   0.1077904   0.3530279
+2016.15   0.1079897   0.3530804
+2016.20   0.1081885   0.3531318
+2016.25   0.1083866   0.3531821
+2016.30   0.1085843   0.3532312
+2016.35   0.1087813   0.3532792
+2016.40   0.1089777   0.3533261
+2016.45   0.1091735   0.3533719
+2016.50   0.1093687   0.3534164
+2016.55   0.1095632   0.3534599
+2016.60   0.1097571   0.3535021
+2016.65   0.1099503   0.3535432
+2016.70   0.1101428   0.3535831
+2016.75   0.1103346   0.3536219
+2016.80   0.1105257   0.3536594
+2016.85   0.1107161   0.3536958
+2016.90   0.1109057   0.3537310
+2016.95   0.1110946   0.3537650
+2017.00   0.1112827   0.3537979
+2017.05   0.1114700   0.3538295
+2017.10   0.1116565   0.3538600
+2017.15   0.1118422   0.3538893
+2017.20   0.1120271   0.3539175
+2017.25   0.1122111   0.3539444
+2017.30   0.1123943   0.3539702
+2017.35   0.1125766   0.3539948
+2017.40   0.1127580   0.3540183
+2017.45   0.1129385   0.3540406
+2017.50   0.1131181   0.3540617
+2017.55   0.1132967   0.3540817
+2017.60   0.1134744   0.3541006
+2017.65   0.1136511   0.3541183
+2017.70   0.1138269   0.3541349
+2017.75   0.1140016   0.3541504
+2017.80   0.1141754   0.3541648
+2017.85   0.1143481   0.3541780
+2017.90   0.1145198   0.3541902
+2017.95   0.1146904   0.3542013
+2018.00   0.1148600   0.3542113
+2018.05   0.1150285   0.3542203
+2018.10   0.1151959   0.3542281
+2018.15   0.1153623   0.3542350
+2018.20   0.1155275   0.3542408
+2018.25   0.1156915   0.3542455
+2018.30   0.1158544   0.3542493
+2018.35   0.1160162   0.3542520
+2018.40   0.1161768   0.3542538
+2018.45   0.1163362   0.3542545
+2018.50   0.1164945   0.3542543
+2018.55   0.1166515   0.3542531
+2018.60   0.1168073   0.3542510
+2018.65   0.1169619   0.3542480
+2018.70   0.1171153   0.3542440
+2018.75   0.1172674   0.3542391
+2018.80   0.1174182   0.3542333
+2018.85   0.1175678   0.3542266
+2018.90   0.1177161   0.3542190
+2018.95   0.1178631   0.3542106
+2019.00   0.1180088   0.3542013
+2019.05   0.1181532   0.3541912
+2019.10   0.1182963   0.3541802
+2019.15   0.1184381   0.3541685
+2019.20   0.1185785   0.3541559
+2019.25   0.1187176   0.3541425
+2019.30   0.1188554   0.3541284
+2019.35   0.1189918   0.3541135
+2019.40   0.1191268   0.3540979
+2019.45   0.1192604   0.3540815
+2019.50   0.1193927   0.3540644
+2019.55   0.1195236   0.3540466
+2019.60   0.1196531   0.3540281
+2019.65   0.1197813   0.3540088
+2019.70   0.1199080   0.3539890
+2019.75   0.1200333   0.3539684
+2019.80   0.1201572   0.3539472
+2019.85   0.1202797   0.3539254
+2019.90   0.1204008   0.3539029
+2019.95   0.1205204   0.3538798
+2020.00   0.1206387   0.3538561
+2020.05   0.1207555   0.3538319
+2020.10   0.1208708   0.3538070
+2020.15   0.1209848   0.3537816
+2020.20   0.1210972   0.3537556
+2020.25   0.1212083   0.3537291
+2020.30   0.1213179   0.3537020
+2020.35   0.1214261   0.3536745
+2020.40   0.1215328   0.3536464
+2020.45   0.1216381   0.3536178
+2020.50   0.1217419   0.3535887
+2020.55   0.1218443   0.3535591
+2020.60   0.1219452   0.3535291
+2020.65   0.1220447   0.3534986
+2020.70   0.1221427   0.3534677
+2020.75   0.1222393   0.3534363
+2020.80   0.1223345   0.3534045
+2020.85   0.1224282   0.3533723
+2020.90   0.1225204   0.3533397
+2020.95   0.1226112   0.3533067
+2021.00   0.1227006   0.3532733
+2021.05   0.1227885   0.3532395
+2021.10   0.1228750   0.3532053
+2021.15   0.1229600   0.3531708
+2021.20   0.1230436   0.3531359
+2021.25   0.1231258   0.3531007
+2021.30   0.1232066   0.3530651
+2021.35   0.1232859   0.3530292
+2021.40   0.1233638   0.3529930
+2021.45   0.1234403   0.3529565
+2021.50   0.1235154   0.3529197
+2021.55   0.1235890   0.3528826
+2021.60   0.1236613   0.3528452
+2021.65   0.1237321   0.3528076
+2021.70   0.1238015   0.3527696
+2021.75   0.1238696   0.3527314
+2021.80   0.1239362   0.3526930
+2021.85   0.1240015   0.3526543
+2021.90   0.1240654   0.3526153
+2021.95   0.1241279   0.3525761
+2022.00   0.1241890   0.3525367
+2022.05   0.1242488   0.3524971
+2022.10   0.1243072   0.3524573
+2022.15   0.1243643   0.3524172
+2022.20   0.1244200   0.3523770
+2022.25   0.1244743   0.3523365
+2022.30   0.1245274   0.3522959
+2022.35   0.1245791   0.3522551
+2022.40   0.1246294   0.3522141
+2022.45   0.1246785   0.3521729
+2022.50   0.1247262   0.3521316
+2022.55   0.1247726   0.3520901
+2022.60   0.1248177   0.3520485
+2022.65   0.1248616   0.3520067
+2022.70   0.1249041   0.3519648
+2022.75   0.1249453   0.3519228
+2022.80   0.1249853   0.3518806
+2022.85   0.1250240   0.3518383
+2022.90   0.1250615   0.3517959
+2022.95   0.1250977   0.3517533
+2023.00   0.1251326   0.3517107
+2023.05   0.1251664   0.3516679
+2023.10   0.1251988   0.3516251
+2023.15   0.1252301   0.3515821
+2023.20   0.1252601   0.3515391
+2023.25   0.1252889   0.3514959
+2023.30   0.1253166   0.3514527
+2023.35   0.1253430   0.3514094
+2023.40   0.1253682   0.3513661
```

### Comparing `pyTMD-2.0.5/pyTMD/data/merged_deltat.data` & `pyTMD-2.0.6/pyTMD/data/merged_deltat.data`

 * *Files 1% similar despite different names*

```diff
@@ -7735,7 +7735,56 @@
  2023  6  2 69.2302
  2023  6  3 69.2302
  2023  6  4 69.2299
  2023  6  5 69.2294
  2023  6  6 69.2289
  2023  6  7 69.2284
  2023  6  8 69.2281
+ 2023  6  9 69.2279
+ 2023  6 10 69.2280
+ 2023  6 11 69.2283
+ 2023  6 12 69.2286
+ 2023  6 13 69.2288
+ 2023  6 14 69.2288
+ 2023  6 15 69.2287
+ 2023  6 16 69.2283
+ 2023  6 17 69.2276
+ 2023  6 18 69.2268
+ 2023  6 19 69.2260
+ 2023  6 20 69.2251
+ 2023  6 21 69.2243
+ 2023  6 22 69.2236
+ 2023  6 23 69.2229
+ 2023  6 24 69.2224
+ 2023  6 25 69.2220
+ 2023  6 26 69.2217
+ 2023  6 27 69.2215
+ 2023  6 28 69.2212
+ 2023  6 29 69.2209
+ 2023  6 30 69.2206
+ 2023  7  1 69.2201
+ 2023  7  2 69.2194
+ 2023  7  3 69.2185
+ 2023  7  4 69.2175
+ 2023  7  5 69.2166
+ 2023  7  6 69.2159
+ 2023  7  7 69.2154
+ 2023  7  8 69.2152
+ 2023  7  9 69.2150
+ 2023  7 10 69.2147
+ 2023  7 11 69.2143
+ 2023  7 12 69.2138
+ 2023  7 13 69.2133
+ 2023  7 14 69.2118
+ 2023  7 15 69.2106
+ 2023  7 16 69.2094
+ 2023  7 17 69.2081
+ 2023  7 18 69.2068
+ 2023  7 19 69.2058
+ 2023  7 20 69.2050
+ 2023  7 21 69.2044
+ 2023  7 22 69.2040
+ 2023  7 23 69.2038
+ 2023  7 24 69.2036
+ 2023  7 25 69.2034
+ 2023  7 26 69.2031
+ 2023  7 27 69.2027
```

### Comparing `pyTMD-2.0.5/pyTMD/data/opoleloadcoefcmcor.txt.gz` & `pyTMD-2.0.6/pyTMD/data/opoleloadcoefcmcor.txt.gz`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/data/ser7.dat` & `pyTMD-2.0.6/pyTMD/data/ser7.dat`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
                                                                                
       **********************************************************************   
       *                                                                    *   
       *                   I E R S   B U L L E T I N - A                    *   
       *                                                                    *   
       *           Rapid Service/Prediction of Earth Orientation            *   
       **********************************************************************   
-      8 June 2023                                         Vol. XXXVI No. 023   
+      27 July 2023                                        Vol. XXXVI No. 030   
       ______________________________________________________________________   
       GENERAL INFORMATION:                                                     
          MJD = Julian Date - 2 400 000.5 days                                  
          UT2-UT1 = 0.022 sin(2*pi*T) - 0.012 cos(2*pi*T)                       
                                      - 0.006 sin(4*pi*T) + 0.007 cos(4*pi*T)   
             where pi = 3.14159265... and T is the date in Besselian years.     
          TT = TAI + 32.184 seconds                                             
          DUT1= (UT1-UTC) transmitted with time signals                         
              =  0.0 seconds beginning 28 July 2022 at 0000 UTC                 
          Beginning 1 January 2017:                                             
             TAI-UTC = 37.000 000 seconds                                       
      ***********************************************************************
      * ANNOUNCEMENTS:                                                      *
      *                                                                     *
-     * NO leap second will be introduced at the end of June 2023.          *
+     * NO leap second will be introduced at the end of December 2023.      *
      *                                                                     *
      * The primary source for IERS Rapid Service/Prediction Center (RS/PC) *
      * data products is the official IERS RS/PC website:                   *
      *   https://maia.usno.navy.mil                                        *
      *                                                                     *
      * IERS RS/PC products are also available from:                        *
      *   NASA CDDIS: https://cddis.nasa.gov/archive/products/iers/         *
@@ -49,528 +49,425 @@
      ________________________________________________________________________  
                                                                                
       COMBINED EARTH ORIENTATION PARAMETERS:                                   
                                                                                
                               IERS Rapid Service                               
               MJD      x    error     y    error   UT1-UTC   error             
                        "      "       "      "        s        s               
-   23  6  2  60097 0.09927 .00009 0.50865 .00009 -0.046186 0.000010          
-   23  6  3  60098 0.10222 .00009 0.50940 .00009 -0.046162 0.000012          
-   23  6  4  60099 0.10514 .00009 0.51001 .00009 -0.045918 0.000016          
-   23  6  5  60100 0.10809 .00009 0.51040 .00009 -0.045448 0.000019          
-   23  6  6  60101 0.11119 .00009 0.51082 .00009 -0.044903 0.000020          
-   23  6  7  60102 0.11409 .00009 0.51127 .00009 -0.044423 0.000022          
-   23  6  8  60103 0.11660 .00009 0.51165 .00009 -0.044092 0.000028          
-                                                                               
-                              IERS Final Values                                
-                               MJD        x        y      UT1-UTC              
-                                          "        "         s                 
-           23  4  2           60036   -0.0173   0.4074  -0.02446       
-           23  4  3           60037   -0.0156   0.4100  -0.02474       
-           23  4  4           60038   -0.0138   0.4126  -0.02522       
-           23  4  5           60039   -0.0123   0.4155  -0.02584       
-           23  4  6           60040   -0.0108   0.4183  -0.02654       
-           23  4  7           60041   -0.0091   0.4213  -0.02725       
-           23  4  8           60042   -0.0079   0.4238  -0.02792       
-           23  4  9           60043   -0.0065   0.4263  -0.02848       
-           23  4 10           60044   -0.0053   0.4288  -0.02885       
-           23  4 11           60045   -0.0041   0.4314  -0.02902       
-           23  4 12           60046   -0.0029   0.4342  -0.02903       
-           23  4 13           60047   -0.0024   0.4367  -0.02899       
-           23  4 14           60048   -0.0018   0.4393  -0.02901       
-           23  4 15           60049   -0.0012   0.4417  -0.02926       
-           23  4 16           60050    0.0002   0.4436  -0.02982       
-           23  4 17           60051    0.0017   0.4453  -0.03064       
-           23  4 18           60052    0.0029   0.4469  -0.03161       
-           23  4 19           60053    0.0043   0.4486  -0.03254       
-           23  4 20           60054    0.0057   0.4505  -0.03336       
-           23  4 21           60055    0.0074   0.4526  -0.03397       
-           23  4 22           60056    0.0092   0.4551  -0.03430       
-           23  4 23           60057    0.0107   0.4578  -0.03437       
-           23  4 24           60058    0.0126   0.4606  -0.03428       
-           23  4 25           60059    0.0149   0.4629  -0.03407       
-           23  4 26           60060    0.0173   0.4650  -0.03384       
-           23  4 27           60061    0.0194   0.4671  -0.03363       
-           23  4 28           60062    0.0214   0.4691  -0.03350       
-           23  4 29           60063    0.0238   0.4707  -0.03356       
-           23  4 30           60064    0.0260   0.4721  -0.03381       
-           23  5  1           60065    0.0276   0.4735  -0.03421       
+   23  7 21  60146 0.23587 .00009 0.49114 .00009 -0.020431 0.000012          
+   23  7 22  60147 0.23822 .00009 0.48995 .00009 -0.020029 0.000013          
+   23  7 23  60148 0.24043 .00009 0.48862 .00009 -0.019782 0.000012          
+   23  7 24  60149 0.24268 .00009 0.48712 .00009 -0.019599 0.000012          
+   23  7 25  60150 0.24499 .00009 0.48553 .00009 -0.019359 0.000012          
+   23  7 26  60151 0.24738 .00009 0.48396 .00009 -0.019103 0.000013          
+   23  7 27  60152 0.24985 .00009 0.48239 .00009 -0.018731 0.000014          
                                                                                
       _______________________________________________________________________  
                                                                                
       PREDICTIONS:                                                             
       The following formulas will not reproduce the predictions given below,   
       but may be used to extend the predictions beyond the end of this table.  
                                                                                
-      x =  0.1312 - 0.0139 cos A + 0.1174 sin A - 0.0006 cos C + 0.0595 sin C  
-      y =  0.3421 + 0.1071 cos A + 0.0149 sin A + 0.0595 cos C + 0.0006 sin C  
-         UT1-UTC = -0.0247 + 0.00014 (MJD - 60111) - (UT2-UT1)                 
+      x =  0.1405 + 0.0694 cos A + 0.0786 sin A + 0.0399 cos C + 0.0585 sin C  
+      y =  0.3512 + 0.0746 cos A - 0.0624 sin A + 0.0585 cos C - 0.0399 sin C  
+         UT1-UTC = -0.0390 + 0.00010 (MJD - 60160) - (UT2-UT1)                 
                                                                                
-      where A = 2*pi*(MJD-60103)/365.25 and C = 2*pi*(MJD-60103)/435.          
+      where A = 2*pi*(MJD-60152)/365.25 and C = 2*pi*(MJD-60152)/435.          
                                                                                
-         TAI-UTC(MJD 60104) = 37.0                                             
+         TAI-UTC(MJD 60153) = 37.0                                             
       The accuracy may be estimated from the expressions:                      
-      S x,y = 0.00068 (MJD-60103)**0.80   S t = 0.00025 (MJD-60103)**0.75      
+      S x,y = 0.00068 (MJD-60152)**0.80   S t = 0.00025 (MJD-60152)**0.75      
       Estimated accuracies are:  Predictions     10 d   20 d   30 d   40 d     
                                  Polar coord's  0.004  0.007  0.010  0.013     
                                  UT1-UTC        0.0014 0.0024 0.0032 0.0040    
                                                                                
                     MJD      x(arcsec)   y(arcsec)   UT1-UTC(sec)              
-       2023  6  9  60104       0.1191      0.5119     -0.04401         
-       2023  6 10  60105       0.1215      0.5121     -0.04415         
-       2023  6 11  60106       0.1239      0.5123     -0.04445         
-       2023  6 12  60107       0.1264      0.5124     -0.04479         
-       2023  6 13  60108       0.1290      0.5124     -0.04506         
-       2023  6 14  60109       0.1317      0.5124     -0.04517         
-       2023  6 15  60110       0.1345      0.5124     -0.04504         
-       2023  6 16  60111       0.1372      0.5123     -0.04467         
-       2023  6 17  60112       0.1400      0.5122     -0.04404         
-       2023  6 18  60113       0.1428      0.5121     -0.04321         
-       2023  6 19  60114       0.1455      0.5119     -0.04229         
-       2023  6 20  60115       0.1483      0.5117     -0.04135         
-       2023  6 21  60116       0.1510      0.5114     -0.04047         
-       2023  6 22  60117       0.1537      0.5111     -0.03970         
-       2023  6 23  60118       0.1564      0.5107     -0.03907         
-       2023  6 24  60119       0.1591      0.5103     -0.03858         
-       2023  6 25  60120       0.1617      0.5099     -0.03824         
-       2023  6 26  60121       0.1644      0.5094     -0.03801         
-       2023  6 27  60122       0.1671      0.5088     -0.03784         
-       2023  6 28  60123       0.1697      0.5083     -0.03768         
-       2023  6 29  60124       0.1724      0.5076     -0.03746         
-       2023  6 30  60125       0.1750      0.5070     -0.03711         
-       2023  7  1  60126       0.1777      0.5063     -0.03658         
-       2023  7  2  60127       0.1803      0.5056     -0.03587         
-       2023  7  3  60128       0.1829      0.5048     -0.03505         
-       2023  7  4  60129       0.1855      0.5040     -0.03424         
-       2023  7  5  60130       0.1880      0.5031     -0.03357         
-       2023  7  6  60131       0.1906      0.5022     -0.03315         
-       2023  7  7  60132       0.1931      0.5013     -0.03298         
-       2023  7  8  60133       0.1956      0.5004     -0.03302         
-       2023  7  9  60134       0.1981      0.4994     -0.03314         
-       2023  7 10  60135       0.2006      0.4983     -0.03320         
-       2023  7 11  60136       0.2031      0.4972     -0.03309         
-       2023  7 12  60137       0.2055      0.4961     -0.03273         
-       2023  7 13  60138       0.2079      0.4950     -0.03210         
-       2023  7 14  60139       0.2103      0.4938     -0.03119         
-       2023  7 15  60140       0.2127      0.4926     -0.03008         
-       2023  7 16  60141       0.2150      0.4913     -0.02882         
-       2023  7 17  60142       0.2173      0.4900     -0.02751         
-       2023  7 18  60143       0.2196      0.4887     -0.02622         
-       2023  7 19  60144       0.2219      0.4873     -0.02503         
-       2023  7 20  60145       0.2241      0.4859     -0.02398         
-       2023  7 21  60146       0.2263      0.4845     -0.02310         
-       2023  7 22  60147       0.2285      0.4830     -0.02237         
-       2023  7 23  60148       0.2307      0.4815     -0.02176         
-       2023  7 24  60149       0.2328      0.4800     -0.02122         
-       2023  7 25  60150       0.2349      0.4784     -0.02070         
-       2023  7 26  60151       0.2370      0.4769     -0.02011         
-       2023  7 27  60152       0.2390      0.4752     -0.01940         
-       2023  7 28  60153       0.2411      0.4736     -0.01849         
-       2023  7 29  60154       0.2431      0.4719     -0.01738         
-       2023  7 30  60155       0.2450      0.4702     -0.01612         
-       2023  7 31  60156       0.2469      0.4685     -0.01480         
-       2023  8  1  60157       0.2488      0.4667     -0.01358         
-       2023  8  2  60158       0.2507      0.4649     -0.01260         
-       2023  8  3  60159       0.2525      0.4631     -0.01195         
-       2023  8  4  60160       0.2543      0.4612     -0.01160         
-       2023  8  5  60161       0.2561      0.4594     -0.01145         
-       2023  8  6  60162       0.2578      0.4575     -0.01134         
-       2023  8  7  60163       0.2595      0.4555     -0.01112         
-       2023  8  8  60164       0.2611      0.4536     -0.01066         
-       2023  8  9  60165       0.2628      0.4516     -0.00994         
-       2023  8 10  60166       0.2643      0.4496     -0.00896         
-       2023  8 11  60167       0.2659      0.4476     -0.00779         
-       2023  8 12  60168       0.2674      0.4456     -0.00649         
-       2023  8 13  60169       0.2689      0.4435     -0.00515         
-       2023  8 14  60170       0.2703      0.4414     -0.00385         
-       2023  8 15  60171       0.2717      0.4393     -0.00264         
-       2023  8 16  60172       0.2731      0.4372     -0.00160         
-       2023  8 17  60173       0.2744      0.4351     -0.00073         
-       2023  8 18  60174       0.2757      0.4329     -0.00005         
-       2023  8 19  60175       0.2769      0.4307      0.00048         
-       2023  8 20  60176       0.2782      0.4285      0.00091         
-       2023  8 21  60177       0.2793      0.4263      0.00130         
-       2023  8 22  60178       0.2805      0.4241      0.00173         
-       2023  8 23  60179       0.2815      0.4218      0.00225         
-       2023  8 24  60180       0.2826      0.4196      0.00293         
-       2023  8 25  60181       0.2836      0.4173      0.00379         
-       2023  8 26  60182       0.2846      0.4150      0.00481         
-       2023  8 27  60183       0.2855      0.4127      0.00590         
-       2023  8 28  60184       0.2864      0.4104      0.00695         
-       2023  8 29  60185       0.2873      0.4080      0.00780         
-       2023  8 30  60186       0.2881      0.4057      0.00833         
-       2023  8 31  60187       0.2888      0.4034      0.00850         
-       2023  9  1  60188       0.2896      0.4010      0.00839         
-       2023  9  2  60189       0.2902      0.3986      0.00813         
-       2023  9  3  60190       0.2909      0.3963      0.00791         
-       2023  9  4  60191       0.2915      0.3939      0.00788         
-       2023  9  5  60192       0.2921      0.3915      0.00812         
-       2023  9  6  60193       0.2926      0.3891      0.00865         
-       2023  9  7  60194       0.2930      0.3867      0.00940         
-       2023  9  8  60195       0.2935      0.3843      0.01029         
-       2023  9  9  60196       0.2939      0.3818      0.01124         
-       2023  9 10  60197       0.2942      0.3794      0.01216         
-       2023  9 11  60198       0.2945      0.3770      0.01298         
-       2023  9 12  60199       0.2948      0.3746      0.01364         
-       2023  9 13  60200       0.2950      0.3722      0.01411         
-       2023  9 14  60201       0.2952      0.3697      0.01439         
-       2023  9 15  60202       0.2954      0.3673      0.01450         
-       2023  9 16  60203       0.2955      0.3649      0.01449         
-       2023  9 17  60204       0.2955      0.3624      0.01442         
-       2023  9 18  60205       0.2955      0.3600      0.01437         
-       2023  9 19  60206       0.2955      0.3576      0.01441         
-       2023  9 20  60207       0.2954      0.3551      0.01459         
-       2023  9 21  60208       0.2953      0.3527      0.01496         
-       2023  9 22  60209       0.2952      0.3503      0.01548         
-       2023  9 23  60210       0.2950      0.3479      0.01611         
-       2023  9 24  60211       0.2948      0.3455      0.01673         
-       2023  9 25  60212       0.2945      0.3431      0.01712         
-       2023  9 26  60213       0.2942      0.3407      0.01725         
-       2023  9 27  60214       0.2938      0.3383      0.01703         
-       2023  9 28  60215       0.2934      0.3359      0.01648         
-       2023  9 29  60216       0.2930      0.3335      0.01570         
-       2023  9 30  60217       0.2925      0.3312      0.01487         
-       2023 10  1  60218       0.2920      0.3288      0.01415         
-       2023 10  2  60219       0.2914      0.3264      0.01369         
-       2023 10  3  60220       0.2909      0.3241      0.01353         
-       2023 10  4  60221       0.2902      0.3218      0.01366         
-       2023 10  5  60222       0.2895      0.3195      0.01398         
-       2023 10  6  60223       0.2888      0.3172      0.01441         
-       2023 10  7  60224       0.2881      0.3149      0.01485         
-       2023 10  8  60225       0.2873      0.3126      0.01522         
-       2023 10  9  60226       0.2865      0.3103      0.01546         
-       2023 10 10  60227       0.2856      0.3081      0.01552         
-       2023 10 11  60228       0.2847      0.3059      0.01540         
-       2023 10 12  60229       0.2838      0.3036      0.01510         
-       2023 10 13  60230       0.2828      0.3014      0.01467         
-       2023 10 14  60231       0.2818      0.2993      0.01416         
-       2023 10 15  60232       0.2807      0.2971      0.01366         
-       2023 10 16  60233       0.2796      0.2949      0.01324         
-       2023 10 17  60234       0.2785      0.2928      0.01297         
-       2023 10 18  60235       0.2773      0.2907      0.01289         
-       2023 10 19  60236       0.2762      0.2886      0.01300         
-       2023 10 20  60237       0.2749      0.2865      0.01325         
-       2023 10 21  60238       0.2737      0.2845      0.01353         
-       2023 10 22  60239       0.2724      0.2825      0.01373         
-       2023 10 23  60240       0.2711      0.2805      0.01373         
-       2023 10 24  60241       0.2697      0.2785      0.01344         
-       2023 10 25  60242       0.2683      0.2765      0.01283         
-       2023 10 26  60243       0.2669      0.2746      0.01197         
-       2023 10 27  60244       0.2654      0.2727      0.01099         
-       2023 10 28  60245       0.2639      0.2708      0.01005         
-       2023 10 29  60246       0.2624      0.2689      0.00931         
-       2023 10 30  60247       0.2609      0.2671      0.00885         
-       2023 10 31  60248       0.2593      0.2653      0.00870         
-       2023 11  1  60249       0.2577      0.2635      0.00880         
-       2023 11  2  60250       0.2561      0.2617      0.00906         
-       2023 11  3  60251       0.2544      0.2600      0.00939         
-       2023 11  4  60252       0.2527      0.2583      0.00968         
-       2023 11  5  60253       0.2510      0.2566      0.00986         
-       2023 11  6  60254       0.2493      0.2549      0.00990         
-       2023 11  7  60255       0.2475      0.2533      0.00976         
-       2023 11  8  60256       0.2457      0.2517      0.00946         
-       2023 11  9  60257       0.2439      0.2502      0.00903         
-       2023 11 10  60258       0.2420      0.2486      0.00851         
-       2023 11 11  60259       0.2402      0.2471      0.00797         
-       2023 11 12  60260       0.2383      0.2456      0.00750         
-       2023 11 13  60261       0.2364      0.2442      0.00717         
-       2023 11 14  60262       0.2344      0.2428      0.00704         
-       2023 11 15  60263       0.2325      0.2414      0.00712         
-       2023 11 16  60264       0.2305      0.2401      0.00737         
-       2023 11 17  60265       0.2285      0.2387      0.00770         
-       2023 11 18  60266       0.2265      0.2374      0.00799         
-       2023 11 19  60267       0.2245      0.2362      0.00812         
-       2023 11 20  60268       0.2224      0.2350      0.00800         
-       2023 11 21  60269       0.2203      0.2338      0.00760         
-       2023 11 22  60270       0.2183      0.2326      0.00696         
-       2023 11 23  60271       0.2161      0.2315      0.00618         
-       2023 11 24  60272       0.2140      0.2304      0.00540         
-       2023 11 25  60273       0.2119      0.2294      0.00477         
-       2023 11 26  60274       0.2097      0.2283      0.00437         
-       2023 11 27  60275       0.2076      0.2274      0.00427         
-       2023 11 28  60276       0.2054      0.2264      0.00445         
-       2023 11 29  60277       0.2032      0.2255      0.00482         
-       2023 11 30  60278       0.2010      0.2246      0.00530         
-       2023 12  1  60279       0.1988      0.2238      0.00578         
-       2023 12  2  60280       0.1965      0.2230      0.00620         
-       2023 12  3  60281       0.1943      0.2222      0.00648         
-       2023 12  4  60282       0.1920      0.2214      0.00661         
-       2023 12  5  60283       0.1898      0.2207      0.00659         
-       2023 12  6  60284       0.1875      0.2201      0.00643         
-       2023 12  7  60285       0.1852      0.2194      0.00619         
-       2023 12  8  60286       0.1830      0.2189      0.00592         
-       2023 12  9  60287       0.1807      0.2183      0.00569         
-       2023 12 10  60288       0.1784      0.2178      0.00559         
-       2023 12 11  60289       0.1761      0.2173      0.00568         
-       2023 12 12  60290       0.1738      0.2168      0.00599         
-       2023 12 13  60291       0.1714      0.2164      0.00650         
-       2023 12 14  60292       0.1691      0.2160      0.00715         
-       2023 12 15  60293       0.1668      0.2157      0.00779         
-       2023 12 16  60294       0.1645      0.2154      0.00830         
-       2023 12 17  60295       0.1622      0.2151      0.00857         
-       2023 12 18  60296       0.1599      0.2149      0.00853         
-       2023 12 19  60297       0.1575      0.2147      0.00823         
-       2023 12 20  60298       0.1552      0.2146      0.00775         
-       2023 12 21  60299       0.1529      0.2144      0.00723         
-       2023 12 22  60300       0.1506      0.2143      0.00681         
-       2023 12 23  60301       0.1483      0.2143      0.00661         
-       2023 12 24  60302       0.1459      0.2143      0.00669         
-       2023 12 25  60303       0.1436      0.2143      0.00705         
-       2023 12 26  60304       0.1413      0.2144      0.00763         
-       2023 12 27  60305       0.1390      0.2145      0.00836         
-       2023 12 28  60306       0.1367      0.2146      0.00912         
-       2023 12 29  60307       0.1344      0.2148      0.00983         
-       2023 12 30  60308       0.1322      0.2150      0.01041         
-       2023 12 31  60309       0.1299      0.2152      0.01082         
-       2024  1  1  60310       0.1276      0.2155      0.01106         
-       2024  1  2  60311       0.1254      0.2158      0.01113         
-       2024  1  3  60312       0.1231      0.2161      0.01107         
-       2024  1  4  60313       0.1209      0.2165      0.01092         
-       2024  1  5  60314       0.1187      0.2169      0.01075         
-       2024  1  6  60315       0.1164      0.2174      0.01061         
-       2024  1  7  60316       0.1142      0.2179      0.01057         
-       2024  1  8  60317       0.1120      0.2184      0.01069         
-       2024  1  9  60318       0.1099      0.2189      0.01098         
-       2024  1 10  60319       0.1077      0.2195      0.01141         
-       2024  1 11  60320       0.1055      0.2201      0.01188         
-       2024  1 12  60321       0.1034      0.2208      0.01224         
-       2024  1 13  60322       0.1013      0.2215      0.01235         
-       2024  1 14  60323       0.0992      0.2222      0.01217         
-       2024  1 15  60324       0.0971      0.2229      0.01170         
-       2024  1 16  60325       0.0950      0.2237      0.01105         
-       2024  1 17  60326       0.0929      0.2245      0.01036         
-       2024  1 18  60327       0.0909      0.2254      0.00979         
-       2024  1 19  60328       0.0889      0.2263      0.00943         
-       2024  1 20  60329       0.0869      0.2272      0.00931         
-       2024  1 21  60330       0.0849      0.2281      0.00934         
-       2024  1 22  60331       0.0829      0.2291      0.00962         
-       2024  1 23  60332       0.0810      0.2301      0.01002         
-       2024  1 24  60333       0.0791      0.2311      0.01042         
-       2024  1 25  60334       0.0772      0.2322      0.01078         
-       2024  1 26  60335       0.0753      0.2333      0.01096         
-       2024  1 27  60336       0.0734      0.2344      0.01099         
-       2024  1 28  60337       0.0716      0.2355      0.01096         
-       2024  1 29  60338       0.0698      0.2367      0.01083         
-       2024  1 30  60339       0.0680      0.2379      0.01062         
-       2024  1 31  60340       0.0663      0.2391      0.01032         
-       2024  2  1  60341       0.0645      0.2404      0.00996         
-       2024  2  2  60342       0.0628      0.2416      0.00967         
-       2024  2  3  60343       0.0611      0.2430      0.00950         
-       2024  2  4  60344       0.0595      0.2443      0.00941         
-       2024  2  5  60345       0.0578      0.2456      0.00948         
-       2024  2  6  60346       0.0562      0.2470      0.00968         
-       2024  2  7  60347       0.0546      0.2484      0.00989         
-       2024  2  8  60348       0.0531      0.2498      0.01006         
-       2024  2  9  60349       0.0516      0.2513      0.01006         
-       2024  2 10  60350       0.0501      0.2528      0.00970         
-       2024  2 11  60351       0.0486      0.2543      0.00898         
-       2024  2 12  60352       0.0472      0.2558      0.00797         
-       2024  2 13  60353       0.0458      0.2573      0.00685         
-       2024  2 14  60354       0.0444      0.2589      0.00588         
-       2024  2 15  60355       0.0430      0.2605      0.00521         
-       2024  2 16  60356       0.0417      0.2621      0.00491         
-       2024  2 17  60357       0.0404      0.2637      0.00496         
-       2024  2 18  60358       0.0392      0.2653      0.00524         
-       2024  2 19  60359       0.0380      0.2670      0.00566         
-       2024  2 20  60360       0.0368      0.2687      0.00612         
-       2024  2 21  60361       0.0356      0.2703      0.00659         
-       2024  2 22  60362       0.0345      0.2720      0.00699         
-       2024  2 23  60363       0.0334      0.2738      0.00729         
-       2024  2 24  60364       0.0323      0.2755      0.00743         
-       2024  2 25  60365       0.0313      0.2773      0.00739         
-       2024  2 26  60366       0.0303      0.2790      0.00717         
-       2024  2 27  60367       0.0293      0.2808      0.00681         
-       2024  2 28  60368       0.0284      0.2826      0.00644         
-       2024  2 29  60369       0.0275      0.2844      0.00621         
-       2024  3  1  60370       0.0266      0.2863      0.00605         
-       2024  3  2  60371       0.0258      0.2881      0.00604         
-       2024  3  3  60372       0.0250      0.2899      0.00624         
-       2024  3  4  60373       0.0243      0.2918      0.00658         
-       2024  3  5  60374       0.0235      0.2937      0.00709         
-       2024  3  6  60375       0.0228      0.2955      0.00762         
-       2024  3  7  60376       0.0222      0.2974      0.00798         
-       2024  3  8  60377       0.0216      0.2993      0.00804         
-       2024  3  9  60378       0.0210      0.3012      0.00768         
-       2024  3 10  60379       0.0204      0.3031      0.00697         
-       2024  3 11  60380       0.0199      0.3051      0.00607         
-       2024  3 12  60381       0.0194      0.3070      0.00502         
-       2024  3 13  60382       0.0190      0.3089      0.00406         
-       2024  3 14  60383       0.0186      0.3109      0.00341         
-       2024  3 15  60384       0.0182      0.3128      0.00301         
-       2024  3 16  60385       0.0179      0.3147      0.00293         
-       2024  3 17  60386       0.0176      0.3167      0.00297         
-       2024  3 18  60387       0.0173      0.3186      0.00311         
-       2024  3 19  60388       0.0171      0.3206      0.00319         
-       2024  3 20  60389       0.0169      0.3226      0.00320         
-       2024  3 21  60390       0.0167      0.3245      0.00306         
-       2024  3 22  60391       0.0166      0.3265      0.00274         
-       2024  3 23  60392       0.0165      0.3284      0.00223         
-       2024  3 24  60393       0.0164      0.3304      0.00161         
-       2024  3 25  60394       0.0164      0.3324      0.00081         
-       2024  3 26  60395       0.0164      0.3343      0.00000         
-       2024  3 27  60396       0.0165      0.3363     -0.00073         
-       2024  3 28  60397       0.0165      0.3382     -0.00135         
-       2024  3 29  60398       0.0167      0.3402     -0.00179         
-       2024  3 30  60399       0.0168      0.3421     -0.00200         
-       2024  3 31  60400       0.0170      0.3441     -0.00198         
-       2024  4  1  60401       0.0172      0.3460     -0.00179         
-       2024  4  2  60402       0.0175      0.3479     -0.00149         
-       2024  4  3  60403       0.0178      0.3499     -0.00124         
-       2024  4  4  60404       0.0181      0.3518     -0.00117         
-       2024  4  5  60405       0.0185      0.3537     -0.00142         
-       2024  4  6  60406       0.0188      0.3556     -0.00202         
-       2024  4  7  60407       0.0193      0.3575     -0.00295         
-       2024  4  8  60408       0.0197      0.3594     -0.00410         
-       2024  4  9  60409       0.0202      0.3613     -0.00508         
-       2024  4 10  60410       0.0207      0.3631     -0.00580         
-       2024  4 11  60411       0.0213      0.3650     -0.00610         
-       2024  4 12  60412       0.0219      0.3668     -0.00611         
-       2024  4 13  60413       0.0225      0.3687     -0.00582         
-       2024  4 14  60414       0.0232      0.3705     -0.00545         
-       2024  4 15  60415       0.0239      0.3723     -0.00505         
-       2024  4 16  60416       0.0246      0.3741     -0.00476         
-       2024  4 17  60417       0.0253      0.3759     -0.00467         
-       2024  4 18  60418       0.0261      0.3777     -0.00481         
-       2024  4 19  60419       0.0269      0.3795     -0.00516         
-       2024  4 20  60420       0.0278      0.3812     -0.00573         
-       2024  4 21  60421       0.0286      0.3830     -0.00639         
-       2024  4 22  60422       0.0295      0.3847     -0.00707         
-       2024  4 23  60423       0.0305      0.3864     -0.00770         
-       2024  4 24  60424       0.0314      0.3881     -0.00820         
-       2024  4 25  60425       0.0324      0.3897     -0.00851         
-       2024  4 26  60426       0.0334      0.3914     -0.00865         
-       2024  4 27  60427       0.0345      0.3930     -0.00855         
-       2024  4 28  60428       0.0355      0.3946     -0.00830         
-       2024  4 29  60429       0.0366      0.3962     -0.00799         
-       2024  4 30  60430       0.0377      0.3978     -0.00773         
-       2024  5  1  60431       0.0389      0.3994     -0.00755         
-       2024  5  2  60432       0.0401      0.4009     -0.00765         
-       2024  5  3  60433       0.0413      0.4024     -0.00801         
-       2024  5  4  60434       0.0425      0.4039     -0.00864         
-       2024  5  5  60435       0.0438      0.4054     -0.00953         
-       2024  5  6  60436       0.0450      0.4069     -0.01048         
-       2024  5  7  60437       0.0463      0.4083     -0.01124         
-       2024  5  8  60438       0.0477      0.4097     -0.01163         
-       2024  5  9  60439       0.0490      0.4111     -0.01166         
-       2024  5 10  60440       0.0504      0.4125     -0.01134         
-       2024  5 11  60441       0.0518      0.4138     -0.01080         
-       2024  5 12  60442       0.0532      0.4152     -0.01017         
-       2024  5 13  60443       0.0546      0.4165     -0.00951         
-       2024  5 14  60444       0.0561      0.4177     -0.00896         
-       2024  5 15  60445       0.0575      0.4190     -0.00854         
-       2024  5 16  60446       0.0590      0.4202     -0.00829         
-       2024  5 17  60447       0.0606      0.4214     -0.00819         
-       2024  5 18  60448       0.0621      0.4226     -0.00821         
-       2024  5 19  60449       0.0636      0.4237     -0.00822         
-       2024  5 20  60450       0.0652      0.4249     -0.00831         
-       2024  5 21  60451       0.0668      0.4260     -0.00830         
-       2024  5 22  60452       0.0684      0.4270     -0.00810         
-       2024  5 23  60453       0.0700      0.4281     -0.00772         
-       2024  5 24  60454       0.0717      0.4291     -0.00714         
-       2024  5 25  60455       0.0733      0.4301     -0.00643         
-       2024  5 26  60456       0.0750      0.4311     -0.00558         
-       2024  5 27  60457       0.0767      0.4320     -0.00478         
-       2024  5 28  60458       0.0784      0.4329     -0.00406         
-       2024  5 29  60459       0.0801      0.4338     -0.00349         
-       2024  5 30  60460       0.0818      0.4346     -0.00312         
-       2024  5 31  60461       0.0835      0.4355     -0.00303         
-       2024  6  1  60462       0.0853      0.4363     -0.00309         
-       2024  6  2  60463       0.0870      0.4370     -0.00320         
-       2024  6  3  60464       0.0888      0.4378     -0.00321         
-       2024  6  4  60465       0.0906      0.4385     -0.00299         
-       2024  6  5  60466       0.0923      0.4392     -0.00238         
-       2024  6  6  60467       0.0941      0.4398     -0.00147         
-       2024  6  7  60468       0.0959      0.4404     -0.00030         
+       2023  7 28  60153       0.2522      0.4808     -0.01819         
+       2023  7 29  60154       0.2545      0.4792     -0.01744         
+       2023  7 30  60155       0.2566      0.4776     -0.01656         
+       2023  7 31  60156       0.2587      0.4759     -0.01561         
+       2023  8  1  60157       0.2606      0.4741     -0.01473         
+       2023  8  2  60158       0.2625      0.4723     -0.01406         
+       2023  8  3  60159       0.2644      0.4704     -0.01369         
+       2023  8  4  60160       0.2662      0.4684     -0.01361         
+       2023  8  5  60161       0.2679      0.4665     -0.01372         
+       2023  8  6  60162       0.2697      0.4645     -0.01391         
+       2023  8  7  60163       0.2714      0.4625     -0.01401         
+       2023  8  8  60164       0.2731      0.4604     -0.01391         
+       2023  8  9  60165       0.2747      0.4583     -0.01356         
+       2023  8 10  60166       0.2763      0.4562     -0.01295         
+       2023  8 11  60167       0.2779      0.4541     -0.01218         
+       2023  8 12  60168       0.2794      0.4520     -0.01129         
+       2023  8 13  60169       0.2809      0.4498     -0.01035         
+       2023  8 14  60170       0.2823      0.4476     -0.00940         
+       2023  8 15  60171       0.2837      0.4454     -0.00853         
+       2023  8 16  60172       0.2850      0.4432     -0.00778         
+       2023  8 17  60173       0.2863      0.4410     -0.00718         
+       2023  8 18  60174       0.2876      0.4387     -0.00674         
+       2023  8 19  60175       0.2888      0.4364     -0.00644         
+       2023  8 20  60176       0.2900      0.4341     -0.00626         
+       2023  8 21  60177       0.2912      0.4318     -0.00612         
+       2023  8 22  60178       0.2923      0.4294     -0.00598         
+       2023  8 23  60179       0.2934      0.4270     -0.00574         
+       2023  8 24  60180       0.2944      0.4247     -0.00535         
+       2023  8 25  60181       0.2954      0.4223     -0.00479         
+       2023  8 26  60182       0.2964      0.4199     -0.00409         
+       2023  8 27  60183       0.2973      0.4175     -0.00333         
+       2023  8 28  60184       0.2981      0.4150     -0.00263         
+       2023  8 29  60185       0.2990      0.4126     -0.00214         
+       2023  8 30  60186       0.2998      0.4101     -0.00196         
+       2023  8 31  60187       0.3005      0.4077     -0.00213         
+       2023  9  1  60188       0.3012      0.4052     -0.00259         
+       2023  9  2  60189       0.3019      0.4027     -0.00320         
+       2023  9  3  60190       0.3025      0.4002     -0.00377         
+       2023  9  4  60191       0.3030      0.3977     -0.00415         
+       2023  9  5  60192       0.3036      0.3952     -0.00425         
+       2023  9  6  60193       0.3041      0.3927     -0.00407         
+       2023  9  7  60194       0.3045      0.3902     -0.00365         
+       2023  9  8  60195       0.3049      0.3877     -0.00309         
+       2023  9  9  60196       0.3053      0.3851     -0.00247         
+       2023  9 10  60197       0.3056      0.3826     -0.00189         
+       2023  9 11  60198       0.3058      0.3801     -0.00141         
+       2023  9 12  60199       0.3061      0.3775     -0.00110         
+       2023  9 13  60200       0.3063      0.3750     -0.00099         
+       2023  9 14  60201       0.3064      0.3724     -0.00110         
+       2023  9 15  60202       0.3065      0.3699     -0.00139         
+       2023  9 16  60203       0.3065      0.3674     -0.00182         
+       2023  9 17  60204       0.3065      0.3648     -0.00231         
+       2023  9 18  60205       0.3065      0.3623     -0.00279         
+       2023  9 19  60206       0.3064      0.3597     -0.00316         
+       2023  9 20  60207       0.3063      0.3572     -0.00338         
+       2023  9 21  60208       0.3061      0.3547     -0.00342         
+       2023  9 22  60209       0.3059      0.3521     -0.00328         
+       2023  9 23  60210       0.3057      0.3496     -0.00304         
+       2023  9 24  60211       0.3054      0.3471     -0.00279         
+       2023  9 25  60212       0.3051      0.3446     -0.00268         
+       2023  9 26  60213       0.3047      0.3421     -0.00281         
+       2023  9 27  60214       0.3043      0.3396     -0.00328         
+       2023  9 28  60215       0.3038      0.3371     -0.00407         
+       2023  9 29  60216       0.3033      0.3346     -0.00507         
+       2023  9 30  60217       0.3028      0.3321     -0.00613         
+       2023 10  1  60218       0.3022      0.3297     -0.00705         
+       2023 10  2  60219       0.3015      0.3272     -0.00773         
+       2023 10  3  60220       0.3009      0.3248     -0.00808         
+       2023 10  4  60221       0.3002      0.3224     -0.00815         
+       2023 10  5  60222       0.2994      0.3199     -0.00800         
+       2023 10  6  60223       0.2986      0.3175     -0.00775         
+       2023 10  7  60224       0.2978      0.3152     -0.00747         
+       2023 10  8  60225       0.2969      0.3128     -0.00725         
+       2023 10  9  60226       0.2960      0.3104     -0.00715         
+       2023 10 10  60227       0.2951      0.3081     -0.00722         
+       2023 10 11  60228       0.2941      0.3058     -0.00747         
+       2023 10 12  60229       0.2931      0.3034     -0.00788         
+       2023 10 13  60230       0.2920      0.3011     -0.00843         
+       2023 10 14  60231       0.2909      0.2989     -0.00904         
+       2023 10 15  60232       0.2898      0.2966     -0.00965         
+       2023 10 16  60233       0.2886      0.2944     -0.01017         
+       2023 10 17  60234       0.2874      0.2922     -0.01055         
+       2023 10 18  60235       0.2861      0.2900     -0.01073         
+       2023 10 19  60236       0.2849      0.2878     -0.01072         
+       2023 10 20  60237       0.2835      0.2856     -0.01059         
+       2023 10 21  60238       0.2822      0.2835     -0.01041         
+       2023 10 22  60239       0.2808      0.2814     -0.01031         
+       2023 10 23  60240       0.2794      0.2793     -0.01042         
+       2023 10 24  60241       0.2779      0.2772     -0.01081         
+       2023 10 25  60242       0.2764      0.2752     -0.01152         
+       2023 10 26  60243       0.2749      0.2732     -0.01248         
+       2023 10 27  60244       0.2733      0.2712     -0.01356         
+       2023 10 28  60245       0.2718      0.2692     -0.01460         
+       2023 10 29  60246       0.2701      0.2673     -0.01543         
+       2023 10 30  60247       0.2685      0.2654     -0.01598         
+       2023 10 31  60248       0.2668      0.2635     -0.01622         
+       2023 11  1  60249       0.2651      0.2616     -0.01621         
+       2023 11  2  60250       0.2634      0.2598     -0.01602         
+       2023 11  3  60251       0.2616      0.2580     -0.01578         
+       2023 11  4  60252       0.2598      0.2562     -0.01556         
+       2023 11  5  60253       0.2580      0.2544     -0.01544         
+       2023 11  6  60254       0.2561      0.2527     -0.01547         
+       2023 11  7  60255       0.2543      0.2510     -0.01566         
+       2023 11  8  60256       0.2524      0.2494     -0.01600         
+       2023 11  9  60257       0.2504      0.2478     -0.01648         
+       2023 11 10  60258       0.2485      0.2462     -0.01704         
+       2023 11 11  60259       0.2465      0.2446     -0.01761         
+       2023 11 12  60260       0.2445      0.2431     -0.01811         
+       2023 11 13  60261       0.2425      0.2416     -0.01859         
+       2023 11 14  60262       0.2404      0.2401     -0.01887         
+       2023 11 15  60263       0.2383      0.2387     -0.01894         
+       2023 11 16  60264       0.2363      0.2373     -0.01883         
+       2023 11 17  60265       0.2341      0.2359     -0.01865         
+       2023 11 18  60266       0.2320      0.2346     -0.01850         
+       2023 11 19  60267       0.2299      0.2333     -0.01852         
+       2023 11 20  60268       0.2277      0.2320     -0.01878         
+       2023 11 21  60269       0.2255      0.2308     -0.01932         
+       2023 11 22  60270       0.2233      0.2296     -0.02010         
+       2023 11 23  60271       0.2211      0.2284     -0.02102         
+       2023 11 24  60272       0.2188      0.2273     -0.02194         
+       2023 11 25  60273       0.2166      0.2262     -0.02272         
+       2023 11 26  60274       0.2143      0.2251     -0.02326         
+       2023 11 27  60275       0.2120      0.2241     -0.02350         
+       2023 11 28  60276       0.2097      0.2231     -0.02347         
+       2023 11 29  60277       0.2074      0.2222     -0.02324         
+       2023 11 30  60278       0.2050      0.2213     -0.02291         
+       2023 12  1  60279       0.2027      0.2204     -0.02258         
+       2023 12  2  60280       0.2004      0.2196     -0.02232         
+       2023 12  3  60281       0.1980      0.2188     -0.02219         
+       2023 12  4  60282       0.1956      0.2180     -0.02222         
+       2023 12  5  60283       0.1932      0.2173     -0.02241         
+       2023 12  6  60284       0.1909      0.2166     -0.02274         
+       2023 12  7  60285       0.1885      0.2160     -0.02317         
+       2023 12  8  60286       0.1860      0.2153     -0.02362         
+       2023 12  9  60287       0.1836      0.2148     -0.02404         
+       2023 12 10  60288       0.1812      0.2142     -0.02435         
+       2023 12 11  60289       0.1788      0.2137     -0.02448         
+       2023 12 12  60290       0.1764      0.2133     -0.02441         
+       2023 12 13  60291       0.1739      0.2129     -0.02414         
+       2023 12 14  60292       0.1715      0.2125     -0.02376         
+       2023 12 15  60293       0.1691      0.2121     -0.02338         
+       2023 12 16  60294       0.1666      0.2118     -0.02313         
+       2023 12 17  60295       0.1642      0.2116     -0.02312         
+       2023 12 18  60296       0.1617      0.2113     -0.02339         
+       2023 12 19  60297       0.1593      0.2112     -0.02390         
+       2023 12 20  60298       0.1568      0.2110     -0.02454         
+       2023 12 21  60299       0.1544      0.2109     -0.02521         
+       2023 12 22  60300       0.1520      0.2108     -0.02575         
+       2023 12 23  60301       0.1495      0.2108     -0.02607         
+       2023 12 24  60302       0.1471      0.2108     -0.02612         
+       2023 12 25  60303       0.1447      0.2108     -0.02591         
+       2023 12 26  60304       0.1422      0.2109     -0.02549         
+       2023 12 27  60305       0.1398      0.2110     -0.02495         
+       2023 12 28  60306       0.1374      0.2112     -0.02438         
+       2023 12 29  60307       0.1350      0.2114     -0.02387         
+       2023 12 30  60308       0.1326      0.2116     -0.02347         
+       2023 12 31  60309       0.1302      0.2119     -0.02324         
+       2024  1  1  60310       0.1278      0.2122     -0.02317         
+       2024  1  2  60311       0.1255      0.2125     -0.02324         
+       2024  1  3  60312       0.1231      0.2129     -0.02342         
+       2024  1  4  60313       0.1207      0.2133     -0.02366         
+       2024  1  5  60314       0.1184      0.2137     -0.02387         
+       2024  1  6  60315       0.1161      0.2142     -0.02401         
+       2024  1  7  60316       0.1137      0.2147     -0.02401         
+       2024  1  8  60317       0.1114      0.2153     -0.02383         
+       2024  1  9  60318       0.1091      0.2159     -0.02346         
+       2024  1 10  60319       0.1069      0.2165     -0.02295         
+       2024  1 11  60320       0.1046      0.2172     -0.02241         
+       2024  1 12  60321       0.1024      0.2179     -0.02199         
+       2024  1 13  60322       0.1001      0.2186     -0.02180         
+       2024  1 14  60323       0.0979      0.2194     -0.02193         
+       2024  1 15  60324       0.0957      0.2202     -0.02234         
+       2024  1 16  60325       0.0935      0.2210     -0.02294         
+       2024  1 17  60326       0.0914      0.2219     -0.02358         
+       2024  1 18  60327       0.0892      0.2228     -0.02411         
+       2024  1 19  60328       0.0871      0.2238     -0.02443         
+       2024  1 20  60329       0.0850      0.2247     -0.02447         
+       2024  1 21  60330       0.0829      0.2257     -0.02426         
+       2024  1 22  60331       0.0808      0.2268     -0.02383         
+       2024  1 23  60332       0.0788      0.2278     -0.02328         
+       2024  1 24  60333       0.0768      0.2289     -0.02268         
+       2024  1 25  60334       0.0748      0.2301     -0.02213         
+       2024  1 26  60335       0.0728      0.2312     -0.02170         
+       2024  1 27  60336       0.0709      0.2324     -0.02141         
+       2024  1 28  60337       0.0689      0.2336     -0.02130         
+       2024  1 29  60338       0.0670      0.2349     -0.02133         
+       2024  1 30  60339       0.0652      0.2362     -0.02148         
+       2024  1 31  60340       0.0633      0.2375     -0.02167         
+       2024  2  1  60341       0.0615      0.2388     -0.02186         
+       2024  2  2  60342       0.0597      0.2402     -0.02198         
+       2024  2  3  60343       0.0579      0.2416     -0.02197         
+       2024  2  4  60344       0.0562      0.2430     -0.02179         
+       2024  2  5  60345       0.0544      0.2444     -0.02143         
+       2024  2  6  60346       0.0527      0.2459     -0.02091         
+       2024  2  7  60347       0.0511      0.2474     -0.02032         
+       2024  2  8  60348       0.0495      0.2489     -0.01978         
+       2024  2  9  60349       0.0478      0.2505     -0.01942         
+       2024  2 10  60350       0.0463      0.2520     -0.01936         
+       2024  2 11  60351       0.0447      0.2536     -0.01964         
+       2024  2 12  60352       0.0432      0.2552     -0.02017         
+       2024  2 13  60353       0.0417      0.2569     -0.02081         
+       2024  2 14  60354       0.0403      0.2585     -0.02139         
+       2024  2 15  60355       0.0389      0.2602     -0.02175         
+       2024  2 16  60356       0.0375      0.2619     -0.02183         
+       2024  2 17  60357       0.0361      0.2637     -0.02163         
+       2024  2 18  60358       0.0348      0.2654     -0.02121         
+       2024  2 19  60359       0.0335      0.2672     -0.02068         
+       2024  2 20  60360       0.0323      0.2690     -0.02013         
+       2024  2 21  60361       0.0310      0.2708     -0.01965         
+       2024  2 22  60362       0.0298      0.2726     -0.01932         
+       2024  2 23  60363       0.0287      0.2744     -0.01918         
+       2024  2 24  60364       0.0276      0.2763     -0.01925         
+       2024  2 25  60365       0.0265      0.2781     -0.01955         
+       2024  2 26  60366       0.0254      0.2800     -0.02005         
+       2024  2 27  60367       0.0244      0.2819     -0.02069         
+       2024  2 28  60368       0.0234      0.2839     -0.02136         
+       2024  2 29  60369       0.0225      0.2858     -0.02198         
+       2024  3  1  60370       0.0216      0.2877     -0.02247         
+       2024  3  2  60371       0.0207      0.2897     -0.02278         
+       2024  3  3  60372       0.0198      0.2917     -0.02288         
+       2024  3  4  60373       0.0190      0.2937     -0.02281         
+       2024  3  5  60374       0.0183      0.2956     -0.02266         
+       2024  3  6  60375       0.0175      0.2977     -0.02249         
+       2024  3  7  60376       0.0168      0.2997     -0.02254         
+       2024  3  8  60377       0.0162      0.3017     -0.02285         
+       2024  3  9  60378       0.0155      0.3037     -0.02352         
+       2024  3 10  60379       0.0150      0.3058     -0.02458         
+       2024  3 11  60380       0.0144      0.3078     -0.02594         
+       2024  3 12  60381       0.0139      0.3099     -0.02734         
+       2024  3 13  60382       0.0134      0.3120     -0.02850         
+       2024  3 14  60383       0.0130      0.3140     -0.02940         
+       2024  3 15  60384       0.0126      0.3161     -0.02994         
+       2024  3 16  60385       0.0122      0.3182     -0.03019         
+       2024  3 17  60386       0.0119      0.3203     -0.03023         
+       2024  3 18  60387       0.0116      0.3224     -0.03004         
+       2024  3 19  60388       0.0113      0.3245     -0.02975         
+       2024  3 20  60389       0.0111      0.3266     -0.02952         
+       2024  3 21  60390       0.0109      0.3287     -0.02947         
+       2024  3 22  60391       0.0108      0.3308     -0.02963         
+       2024  3 23  60392       0.0107      0.3329     -0.02988         
+       2024  3 24  60393       0.0106      0.3350     -0.03032         
+       2024  3 25  60394       0.0106      0.3371     -0.03085         
+       2024  3 26  60395       0.0106      0.3392     -0.03147         
+       2024  3 27  60396       0.0106      0.3413     -0.03202         
+       2024  3 28  60397       0.0107      0.3434     -0.03245         
+       2024  3 29  60398       0.0108      0.3455     -0.03275         
+       2024  3 30  60399       0.0110      0.3475     -0.03287         
+       2024  3 31  60400       0.0112      0.3496     -0.03279         
+       2024  4  1  60401       0.0114      0.3517     -0.03256         
+       2024  4  2  60402       0.0117      0.3538     -0.03227         
+       2024  4  3  60403       0.0120      0.3559     -0.03206         
+       2024  4  4  60404       0.0123      0.3579     -0.03209         
+       2024  4  5  60405       0.0127      0.3600     -0.03238         
+       2024  4  6  60406       0.0131      0.3621     -0.03309         
+       2024  4  7  60407       0.0135      0.3641     -0.03405         
+       2024  4  8  60408       0.0140      0.3661     -0.03518         
+       2024  4  9  60409       0.0145      0.3682     -0.03631         
+       2024  4 10  60410       0.0150      0.3702     -0.03723         
+       2024  4 11  60411       0.0156      0.3722     -0.03788         
+       2024  4 12  60412       0.0162      0.3742     -0.03826         
+       2024  4 13  60413       0.0169      0.3762     -0.03840         
+       2024  4 14  60414       0.0175      0.3782     -0.03841         
+       2024  4 15  60415       0.0182      0.3801     -0.03836         
+       2024  4 16  60416       0.0190      0.3821     -0.03837         
+       2024  4 17  60417       0.0198      0.3840     -0.03854         
+       2024  4 18  60418       0.0206      0.3859     -0.03874         
+       2024  4 19  60419       0.0214      0.3879     -0.03917         
+       2024  4 20  60420       0.0223      0.3897     -0.03975         
+       2024  4 21  60421       0.0232      0.3916     -0.04038         
+       2024  4 22  60422       0.0241      0.3935     -0.04106         
+       2024  4 23  60423       0.0251      0.3953     -0.04170         
+       2024  4 24  60424       0.0261      0.3972     -0.04223         
+       2024  4 25  60425       0.0271      0.3990     -0.04259         
+       2024  4 26  60426       0.0282      0.4008     -0.04276         
+       2024  4 27  60427       0.0293      0.4026     -0.04276         
+       2024  4 28  60428       0.0304      0.4043     -0.04272         
+       2024  4 29  60429       0.0316      0.4061     -0.04256         
+       2024  4 30  60430       0.0327      0.4078     -0.04244         
+       2024  5  1  60431       0.0339      0.4095     -0.04250         
+       2024  5  2  60432       0.0352      0.4112     -0.04281         
+       2024  5  3  60433       0.0364      0.4129     -0.04348         
+       2024  5  4  60434       0.0377      0.4145     -0.04441         
+       2024  5  5  60435       0.0390      0.4161     -0.04541         
+       2024  5  6  60436       0.0404      0.4177     -0.04637         
+       2024  5  7  60437       0.0417      0.4193     -0.04714         
+       2024  5  8  60438       0.0431      0.4209     -0.04761         
+       2024  5  9  60439       0.0445      0.4224     -0.04782         
+       2024  5 10  60440       0.0460      0.4239     -0.04771         
+       2024  5 11  60441       0.0474      0.4254     -0.04738         
+       2024  5 12  60442       0.0489      0.4268     -0.04703         
+       2024  5 13  60443       0.0504      0.4283     -0.04671         
+       2024  5 14  60444       0.0519      0.4297     -0.04649         
+       2024  5 15  60445       0.0535      0.4311     -0.04646         
+       2024  5 16  60446       0.0551      0.4324     -0.04655         
+       2024  5 17  60447       0.0567      0.4338     -0.04673         
+       2024  5 18  60448       0.0583      0.4351     -0.04704         
+       2024  5 19  60449       0.0599      0.4364     -0.04741         
+       2024  5 20  60450       0.0616      0.4376     -0.04778         
+       2024  5 21  60451       0.0632      0.4389     -0.04805         
+       2024  5 22  60452       0.0649      0.4401     -0.04803         
+       2024  5 23  60453       0.0666      0.4412     -0.04778         
+       2024  5 24  60454       0.0683      0.4424     -0.04724         
+       2024  5 25  60455       0.0701      0.4435     -0.04643         
+       2024  5 26  60456       0.0718      0.4446     -0.04555         
+       2024  5 27  60457       0.0736      0.4456     -0.04465         
+       2024  5 28  60458       0.0754      0.4467     -0.04388         
+       2024  5 29  60459       0.0772      0.4477     -0.04329         
+       2024  5 30  60460       0.0790      0.4487     -0.04294         
+       2024  5 31  60461       0.0809      0.4496     -0.04279         
+       2024  6  1  60462       0.0827      0.4505     -0.04280         
+       2024  6  2  60463       0.0845      0.4514     -0.04286         
+       2024  6  3  60464       0.0864      0.4523     -0.04287         
+       2024  6  4  60465       0.0883      0.4531     -0.04269         
+       2024  6  5  60466       0.0902      0.4539     -0.04218         
+       2024  6  6  60467       0.0921      0.4546     -0.04129         
+       2024  6  7  60468       0.0940      0.4554     -0.04020         
+       2024  6  8  60469       0.0959      0.4561     -0.03896         
+       2024  6  9  60470       0.0978      0.4567     -0.03767         
+       2024  6 10  60471       0.0998      0.4574     -0.03647         
+       2024  6 11  60472       0.1017      0.4580     -0.03531         
+       2024  6 12  60473       0.1036      0.4586     -0.03426         
+       2024  6 13  60474       0.1056      0.4591     -0.03341         
+       2024  6 14  60475       0.1075      0.4596     -0.03266         
+       2024  6 15  60476       0.1095      0.4601     -0.03202         
+       2024  6 16  60477       0.1115      0.4606     -0.03139         
+       2024  6 17  60478       0.1134      0.4610     -0.03066         
+       2024  6 18  60479       0.1154      0.4614     -0.02990         
+       2024  6 19  60480       0.1174      0.4617     -0.02902         
+       2024  6 20  60481       0.1194      0.4621     -0.02794         
+       2024  6 21  60482       0.1214      0.4624     -0.02677         
+       2024  6 22  60483       0.1233      0.4626     -0.02542         
+       2024  6 23  60484       0.1253      0.4629     -0.02413         
+       2024  6 24  60485       0.1273      0.4631     -0.02292         
+       2024  6 25  60486       0.1293      0.4632     -0.02198         
+       2024  6 26  60487       0.1313      0.4634     -0.02129         
+       2024  6 27  60488       0.1332      0.4635     -0.02090         
+       2024  6 28  60489       0.1352      0.4635     -0.02071         
+       2024  6 29  60490       0.1372      0.4636     -0.02060         
+       2024  6 30  60491       0.1391      0.4636     -0.02038         
+       2024  7  1  60492       0.1411      0.4636     -0.02006         
+       2024  7  2  60493       0.1431      0.4635     -0.01941         
+       2024  7  3  60494       0.1450      0.4634     -0.01845         
+       2024  7  4  60495       0.1469      0.4633     -0.01727         
+       2024  7  5  60496       0.1489      0.4632     -0.01589         
+       2024  7  6  60497       0.1508      0.4630     -0.01443         
+       2024  7  7  60498       0.1527      0.4628     -0.01298         
+       2024  7  8  60499       0.1547      0.4626     -0.01162         
+       2024  7  9  60500       0.1566      0.4623     -0.01032         
+       2024  7 10  60501       0.1585      0.4620     -0.00916         
+       2024  7 11  60502       0.1604      0.4617     -0.00814         
+       2024  7 12  60503       0.1622      0.4613     -0.00719         
+       2024  7 13  60504       0.1641      0.4609     -0.00625         
+       2024  7 14  60505       0.1660      0.4605     -0.00533         
+       2024  7 15  60506       0.1678      0.4601     -0.00438         
+       2024  7 16  60507       0.1696      0.4596     -0.00319         
+       2024  7 17  60508       0.1715      0.4591     -0.00178         
+       2024  7 18  60509       0.1733      0.4586     -0.00009         
+       2024  7 19  60510       0.1751      0.4580      0.00164         
+       2024  7 20  60511       0.1768      0.4574      0.00348         
+       2024  7 21  60512       0.1786      0.4568      0.00515         
+       2024  7 22  60513       0.1803      0.4562      0.00661         
+       2024  7 23  60514       0.1821      0.4555      0.00774         
+       2024  7 24  60515       0.1838      0.4548      0.00846         
+       2024  7 25  60516       0.1855      0.4541      0.00883         
+       2024  7 26  60517       0.1872      0.4533      0.00902         
       These predictions are based on all announced leap seconds.               
                                                                                
       CELESTIAL POLE OFFSET SERIES:                                            
                            NEOS Celestial Pole Offset Series                   
                        MJD      dpsi    error     deps    error                
                                         (msec. of arc)                         
-                      60084  -106.87    0.32   -9.47    0.16   
-                      60085  -106.93    0.32   -9.70    0.16   
-                      60086  -107.04    0.32   -9.90    0.16   
-                      60087  -107.17    0.32   -9.96    0.16   
-                      60088  -107.24    1.03   -9.93    0.02   
-                      60089  -107.20    1.03   -9.94    0.02   
-                      60090  -107.04    1.03  -10.04    0.02   
-                                                                               
-                     IERS Celestial Pole Offset Final Series                   
-                           MJD          dpsi      deps                         
-                                        (msec. of arc)                         
-                          60036      -106.7      -9.0                      
-                          60037      -106.8      -8.9                      
-                          60038      -107.0      -8.6                      
-                          60039      -107.2      -8.5                      
-                          60040      -107.5      -8.5                      
-                          60041      -107.7      -8.6                      
-                          60042      -107.8      -8.7                      
-                          60043      -107.9      -8.8                      
-                          60044      -108.0      -8.9                      
-                          60045      -107.9      -9.0                      
-                          60046      -107.6      -9.1                      
-                          60047      -107.1      -9.3                      
-                          60048      -106.4      -9.5                      
-                          60049      -106.0      -9.5                      
-                          60050      -106.0      -9.4                      
-                          60051      -106.2      -9.2                      
-                          60052      -106.6      -9.0                      
-                          60053      -106.9      -8.9                      
-                          60054      -107.0      -8.9                      
-                          60055      -107.0      -8.9                      
-                          60056      -107.2      -9.0                      
-                          60057      -107.3      -9.2                      
-                          60058      -107.3      -9.4                      
-                          60059      -107.2      -9.5                      
-                          60060      -106.7      -9.6                      
-                          60061      -106.2      -9.7                      
-                          60062      -106.0      -9.9                      
-                          60063      -106.1     -10.0                      
-                          60064      -105.9     -10.1                      
-                          60065      -106.1      -9.9                      
+                      60130  -112.31    0.87   -9.78    0.29   
+                      60131  -112.19    0.87   -9.55    0.29   
+                      60132  -112.47    0.87   -9.42    0.29   
+                      60133  -112.93    0.78   -9.39    0.31   
+                      60134  -113.31    0.91   -9.34    0.21   
+                      60135  -113.51    0.91   -9.22    0.21   
+                      60136  -113.62    0.97   -9.09    0.10   
                                                             
                      IAU2000A Celestial Pole Offset Series  
                       MJD      dX     error     dY     error
                                     (msec. of arc)          
-                      60084    0.455  0.128   -0.113   0.160          
-                      60085    0.451  0.128   -0.099   0.160          
-                      60086    0.446  0.128   -0.085   0.160          
-                      60087    0.440  0.128   -0.069   0.160          
-                      60088    0.434  0.412   -0.053   0.022          
-                      60089    0.426  0.412   -0.036   0.022          
-                      60090    0.419  0.412   -0.019   0.022          
-                                                                               
-                                                                               
-                 IAU2000A Celestial Pole Offset Final Series 
-                             MJD     dX         dY           
-                             (msec. of arc)          
-                           60036     0.29      -0.09
-                           60037     0.31      -0.11
-                           60038     0.32      -0.12
-                           60039     0.29      -0.12
-                           60040     0.25      -0.11
-                           60041     0.23      -0.09
-                           60042     0.22      -0.06
-                           60043     0.22      -0.02
-                           60044     0.23       0.01
-                           60045     0.24       0.04
-                           60046     0.27       0.04
-                           60047     0.32       0.01
-                           60048     0.35      -0.03
-                           60049     0.35      -0.05
-                           60050     0.32      -0.05
-                           60051     0.27      -0.04
-                           60052     0.23      -0.03
-                           60053     0.23      -0.01
-                           60054     0.24       0.02
-                           60055     0.26       0.04
-                           60056     0.28       0.06
-                           60057     0.30       0.08
-                           60058     0.32       0.08
-                           60059     0.34       0.07
-                           60060     0.47      -0.05
-                           60061     0.56      -0.15
-                           60062     0.47      -0.17
-                           60063     0.25      -0.09
-                           60064     0.25      -0.09
-                           60065     0.24      -0.10
+                      60130    0.384  0.347   -0.270   0.287          
+                      60131    0.377  0.347   -0.260   0.287          
+                      60132    0.372  0.347   -0.245   0.287          
+                      60133    0.369  0.311   -0.224   0.306          
+                      60134    0.368  0.364   -0.196   0.205          
+                      60135    0.369  0.364   -0.165   0.205          
+                      60136    0.370  0.385   -0.131   0.100
```

### Comparing `pyTMD-2.0.5/pyTMD/data/tab5.2e.txt` & `pyTMD-2.0.6/pyTMD/data/tab5.2e.txt`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/data/tab5.3a.txt` & `pyTMD-2.0.6/pyTMD/data/tab5.3a.txt`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/data/tab5.3b.txt` & `pyTMD-2.0.6/pyTMD/data/tab5.3b.txt`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/eop.py` & `pyTMD-2.0.6/pyTMD/eop.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/interpolate.py` & `pyTMD-2.0.6/pyTMD/interpolate.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/io/ATLAS.py` & `pyTMD-2.0.6/pyTMD/io/ATLAS.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,18 +103,15 @@
 import pyTMD.io.constituents
 import pyTMD.interpolate
 
 # attempt imports
 try:
     import netCDF4
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("netCDF4 not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.critical("netCDF4 not available")
 
 # PURPOSE: extract harmonic constants from tide models at coordinates
 def extract_constants(
         ilon: np.ndarray, ilat: np.ndarray,
         grid_file: str | pathlib.Path | None = None,
         model_files: str | list | pathlib.Path | None = None,
         **kwargs
```

### Comparing `pyTMD-2.0.5/pyTMD/io/FES.py` & `pyTMD-2.0.6/pyTMD/io/FES.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,18 +103,15 @@
 import pyTMD.interpolate
 import pyTMD.io.constituents
 
 # attempt imports
 try:
     import netCDF4
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("netCDF4 not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.critical("netCDF4 not available")
 
 # PURPOSE: extract harmonic constants from tide models at coordinates
 def extract_constants(
         ilon: np.ndarray,
         ilat: np.ndarray,
         model_files: str | list | pathlib.Path | None = None,
         **kwargs
```

### Comparing `pyTMD-2.0.5/pyTMD/io/GOT.py` & `pyTMD-2.0.6/pyTMD/io/GOT.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,18 +94,15 @@
 import pyTMD.interpolate
 import pyTMD.io.constituents
 
 # attempt imports
 try:
     import netCDF4
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("netCDF4 not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.debug("netCDF4 not available")
 
 # PURPOSE: extract harmonic constants from tide models at coordinates
 def extract_constants(
         ilon: np.ndarray,
         ilat: np.ndarray,
         model_files: str | pathlib.Path | list | None = None,
         **kwargs
```

### Comparing `pyTMD-2.0.5/pyTMD/io/OTIS.py` & `pyTMD-2.0.6/pyTMD/io/OTIS.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,30 +108,28 @@
     Updated 07/2018: added different interpolation methods
     Updated 09/2017: Adapted for Python
 """
 from __future__ import division, annotations
 
 import copy
 import struct
+import logging
 import pathlib
 import warnings
 import numpy as np
 import scipy.interpolate
 import pyTMD.interpolate
 import pyTMD.io.constituents
 from pyTMD.convert_crs import convert_crs
 
 # attempt imports
 try:
     import netCDF4
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("netCDF4 not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.debug("netCDF4 not available")
 
 # PURPOSE: extract harmonic constants from tide models at coordinates
 def extract_constants(
         ilon: np.ndarray,
         ilat: np.ndarray,
         grid_file: str | pathlib.Path | None = None,
         model_file: str | pathlib.Path | list | None = None,
```

### Comparing `pyTMD-2.0.5/pyTMD/io/constituents.py` & `pyTMD-2.0.6/pyTMD/io/constituents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #!/usr/bin/env python
 u"""
 constituents.py
-Written by Tyler Sutterley (03/2023)
+Written by Tyler Sutterley (07/2023)
 Basic tide model constituent class
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
 
 UPDATE HISTORY:
+    Updated 07/2023: output constituent from get and pop as copy
     Updated 03/2023: add basic variable typing to function inputs
     Written 12/2022
 """
 from __future__ import division, annotations
 
+import copy
 import numpy as np
 
 class constituents:
     """
     Class for tide model constituents
 
     Attributes
@@ -60,15 +62,16 @@
             Tide model constituent name
 
         Returns
         -------
         constituent: np.ndarray
             Tide model constituent (complex form)
         """
-        return getattr(self, field)
+        constituent = getattr(self, field)
+        return copy.copy(constituent)
 
     def pop(self, field: str):
         """
         Retrieve a tide model constituent and remove from list
 
         Parameters
         ----------
@@ -79,15 +82,15 @@
         -------
         constituent: np.ndarray
             Tide model constituent (complex form)
         """
         self.fields.remove(field)
         constituent = getattr(self, field)
         delattr(self, field)
-        return constituent
+        return copy.copy(constituent)
 
     def update(self, field: str, constituent: np.ndarray):
         """
         Update a tide model constituent
 
         Parameters
         ----------
```

### Comparing `pyTMD-2.0.5/pyTMD/io/model.py` & `pyTMD-2.0.6/pyTMD/io/model.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/io/ocean_pole_tide.py` & `pyTMD-2.0.6/pyTMD/io/ocean_pole_tide.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/load_constituent.py` & `pyTMD-2.0.6/pyTMD/load_constituent.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/load_nodal_corrections.py` & `pyTMD-2.0.6/pyTMD/load_nodal_corrections.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/predict.py` & `pyTMD-2.0.6/pyTMD/predict.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/spatial.py` & `pyTMD-2.0.6/pyTMD/spatial.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         try to get grid mapping attributes from netCDF4 and HDF5
     Updated 10/2021: add pole case in stereographic area scale calculation
         using python logging for handling verbose output
     Updated 09/2021: can calculate height differences between ellipsoids
     Updated 07/2021: added function for determining input variable type
     Updated 03/2021: added polar stereographic area scale calculation
         add routines for converting to and from cartesian coordinates
-        eplaced numpy bool/int to prevent deprecation warnings
+        replaced numpy bool/int to prevent deprecation warnings
     Updated 01/2021: add streaming from bytes for ascii, netCDF4, HDF5, geotiff
         set default time for geotiff files to 0
     Updated 12/2020: added module for converting ellipsoids
     Updated 11/2020: output data as masked arrays if containing fill values
         add functions to read from and write to geotiff image formats
     Written 09/2020
 """
@@ -69,37 +69,31 @@
 import copy
 import gzip
 import uuid
 import yaml
 import logging
 import pathlib
 import datetime
-import warnings
 import numpy as np
 import pyTMD.time
 from pyTMD.constants import constants
 import pyTMD.version
 # attempt imports
 try:
     import osgeo.gdal, osgeo.osr, osgeo.gdalconst
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("GDAL not available", ImportWarning)
+    logging.debug("GDAL not available")
 try:
     import h5py
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("h5py not available", ImportWarning)
+    logging.debug("h5py not available")
 try:
     import netCDF4
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("netCDF4 not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.debug("netCDF4 not available")
 
 def case_insensitive_filename(filename: str | pathlib.Path):
     """
     Searches a directory for a filename without case dependence
 
     Parameters
     ----------
@@ -1600,16 +1594,16 @@
         lat[ind] = np.arctan2(zi, ((1.0 - e12)*wi))/dtr
         h[ind] = np.sign(t-1.0+l)*np.sqrt((w-wi)**2.0 + (z[ind]-zi)**2.0)
     # return latitude, longitude and height
     return (lon, lat, h)
 
 def scale_areas(
         lat: np.ndarray,
-        flat: float=_wgs84.flat,
-        ref: float=70.0
+        flat: float = _wgs84.flat,
+        ref: float = 70.0
     ):
     """
     Calculates area scaling factors for a polar stereographic projection
     including special case of at the exact pole [1]_ [2]_
 
     Parameters
     ----------
```

### Comparing `pyTMD-2.0.5/pyTMD/tidal_ellipse.py` & `pyTMD-2.0.6/pyTMD/tidal_ellipse.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/time.py` & `pyTMD-2.0.6/pyTMD/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 u"""
 time.py
-Written by Tyler Sutterley (05/2023)
+Written by Tyler Sutterley (06/2023)
 Utilities for calculating time operations
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
     dateutil: powerful extensions to datetime
         https://dateutil.readthedocs.io/en/stable/
     lxml: processing XML and HTML in Python
         https://pypi.python.org/pypi/lxml
 
 PROGRAM DEPENDENCIES:
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
+    Updated 06/2023: improve conversion of timescale to datetime arrays
     Updated 05/2023: add timescale class for converting between time scales
         added timescale to_datetime function to create datetime arrays
         allow epoch arguments to be numpy datetime64 variables or strings
         function to convert a string with time zone information to datetime
     Updated 04/2023: using pathlib to define and expand paths
     Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: added interpolation for delta time (TT - UT1)
@@ -131,15 +132,15 @@
         epoch = parse(date_string)
     except ValueError:
         pass
     else:
         # return the epoch (as list)
         return (datetime_to_list(epoch), 0.0)
     # split the date string into units and epoch
-    units,epoch = split_date_string(date_string)
+    units, epoch = split_date_string(date_string)
     if units not in _to_sec.keys():
         raise ValueError(f'Invalid units: {units}')
     # return the epoch (as list) and the time unit conversion factors
     return (datetime_to_list(epoch), _to_sec[units])
 
 # PURPOSE: split a date string into units and epoch
 def split_date_string(date_string: str):
@@ -189,15 +190,15 @@
     Parameters
     ----------
     year: int, float or np.ndarray
         calendar year
 
     Returns
     -------
-    dpm: list
+    dpm: np.ndarray
         number of days for each month
     """
     # Rules in the Gregorian calendar for a year to be a leap year:
     # divisible by 4, but not by 100 unless divisible by 400
     # True length of the year is about 365.2422 days
     # Adding a leap day every four years ==> average 365.25
     # Subtracting a leap year every 100 years ==> average 365.24
@@ -251,17 +252,17 @@
     """
     Convert delta time from seconds since ``epoch1`` to time since ``epoch2``
 
     Parameters
     ----------
     delta_time: np.ndarray
         seconds since epoch1
-    epoch1: tuple or NoneType, default None
+    epoch1: str, tuple, list or NoneType, default None
         epoch for input ``delta_time``
-    epoch2: tuple or NoneType, default None
+    epoch2: str, tuple, list or NoneType, default None
         epoch for output ``delta_time``
     scale: float, default 1.0
         scaling factor for converting time to output units
     """
     # convert epochs to datetime variables
     if isinstance(epoch1, (tuple, list)):
         epoch1 = np.datetime64(datetime.datetime(*epoch1))
@@ -285,15 +286,15 @@
         hour: np.ndarray | float = 0.0,
         minute: np.ndarray | float = 0.0,
         second: np.ndarray | float = 0.0,
         epoch: tuple | list | np.datetime64 = _tide_epoch,
         scale: float = 1.0
     ) -> np.ndarray:
     """
-    Calculate the time in time units since ``epoch`` from calendar dates
+    Calculate the time in units since ``epoch`` from calendar dates
 
     Parameters
     ----------
     year: np.ndarray
         calendar year
     month: np.ndarray
         month of the year
@@ -755,15 +756,15 @@
             ``numpy.datetime64`` array
         """
         # convert Modified Julian Day epoch to datetime variable
         epoch = np.datetime64(datetime.datetime(*_mjd_epoch))
         # use nanoseconds to keep as much precision as possible
         delta_time = np.atleast_1d(self.MJD*self.day*1e9).astype(np.int64)
         # return the datetime array
-        return np.array([epoch + np.timedelta64(s, 'ns') for s in delta_time])
+        return np.array(epoch + delta_time.astype('timedelta64[ns]'))
 
     # PURPOSE: calculate the sum of a polynomial function of time
     def polynomial_sum(self, coefficients: list | np.ndarray, t: np.ndarray):
         """
         Calculates the sum of a polynomial function of time
 
         Parameters
```

### Comparing `pyTMD-2.0.5/pyTMD/tools.py` & `pyTMD-2.0.6/pyTMD/tools.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD/utilities.py` & `pyTMD-2.0.6/pyTMD/utilities.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/pyTMD.egg-info/PKG-INFO` & `pyTMD-2.0.6/pyTMD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTMD
-Version: 2.0.5
+Version: 2.0.6
 Summary: Tide Model Driver to read OTIS, GOT and FES formatted tidal solutions and make tidal predictions
 Home-page: https://github.com/tsutterley/pyTMD
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: Ocean Tides,Load Tides,Pole Tides,Tidal Prediction,OTIS,GOT,FES
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyTMD-2.0.5/pyTMD.egg-info/SOURCES.txt` & `pyTMD-2.0.6/pyTMD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/scripts/arcticdata_tides.py` & `pyTMD-2.0.6/scripts/arcticdata_tides.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/scripts/aviso_fes_tides.py` & `pyTMD-2.0.6/scripts/aviso_fes_tides.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/scripts/compute_LPET_elevations.py` & `pyTMD-2.0.6/scripts/compute_LPET_elevations.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,27 +84,23 @@
     Written 09/2020
 """
 from __future__ import print_function
 
 import sys
 import logging
 import pathlib
-import warnings
 import argparse
 import numpy as np
 import pyTMD
 
 # attempt imports
 try:
     import pyproj
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("pyproj not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.critical("pyproj not available")
 
 # PURPOSE: try to get the projection information for the input file
 def get_projection(attributes, PROJECTION):
     # coordinate reference system string from file
     try:
         crs = pyproj.CRS.from_string(attributes['projection'])
     except (ValueError,KeyError,pyproj.exceptions.CRSError):
```

### Comparing `pyTMD-2.0.5/scripts/compute_LPT_displacements.py` & `pyTMD-2.0.6/scripts/compute_LPT_displacements.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,27 +102,23 @@
     Written 10/2017 for public release
 """
 from __future__ import print_function
 
 import sys
 import logging
 import pathlib
-import warnings
 import argparse
 import numpy as np
 import pyTMD
 
 # attempt imports
 try:
     import pyproj
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("pyproj not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.critical("pyproj not available")
 
 # PURPOSE: try to get the projection information for the input file
 def get_projection(attributes, PROJECTION):
     # coordinate reference system string from file
     try:
         crs = pyproj.CRS.from_string(attributes['projection'])
     except (ValueError,KeyError,pyproj.exceptions.CRSError):
```

### Comparing `pyTMD-2.0.5/scripts/compute_OPT_displacements.py` & `pyTMD-2.0.6/scripts/compute_OPT_displacements.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,28 +118,24 @@
     Written 10/2017 for public release
 """
 from __future__ import print_function
 
 import sys
 import logging
 import pathlib
-import warnings
 import argparse
 import numpy as np
 import scipy.interpolate
 import pyTMD
 
 # attempt imports
 try:
     import pyproj
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("pyproj not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.critical("pyproj not available")
 
 # PURPOSE: try to get the projection information for the input file
 def get_projection(attributes, PROJECTION):
     # coordinate reference system string from file
     try:
         crs = pyproj.CRS.from_string(attributes['projection'])
     except (ValueError,KeyError,pyproj.exceptions.CRSError):
```

### Comparing `pyTMD-2.0.5/scripts/compute_SET_displacements.py` & `pyTMD-2.0.6/scripts/compute_SET_displacements.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,27 +97,23 @@
     Written 04/2023
 """
 from __future__ import print_function
 
 import sys
 import logging
 import pathlib
-import warnings
 import argparse
 import numpy as np
 import pyTMD
 
 # attempt imports
 try:
     import pyproj
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("pyproj not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.critical("pyproj not available")
 
 # PURPOSE: try to get the projection information for the input file
 def get_projection(attributes, PROJECTION):
     # coordinate reference system string from file
     try:
         crs = pyproj.CRS.from_string(attributes['projection'])
     except (ValueError,KeyError,pyproj.exceptions.CRSError):
```

### Comparing `pyTMD-2.0.5/scripts/compute_tidal_currents.py` & `pyTMD-2.0.6/scripts/compute_tidal_currents.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,27 +133,23 @@
     Written 10/2017 for public release
 """
 from __future__ import print_function
 
 import sys
 import logging
 import pathlib
-import warnings
 import argparse
 import numpy as np
 import pyTMD
 
 # attempt imports
 try:
     import pyproj
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("pyproj not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.critical("pyproj not available")
 
 # PURPOSE: try to get the projection information for the input file
 def get_projection(attributes, PROJECTION):
     # coordinate reference system string from file
     try:
         crs = pyproj.CRS.from_string(attributes['projection'])
     except (ValueError,KeyError,pyproj.exceptions.CRSError):
```

### Comparing `pyTMD-2.0.5/scripts/compute_tidal_elevations.py` & `pyTMD-2.0.6/scripts/compute_tidal_elevations.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,27 +138,23 @@
     Written 10/2017 for public release
 """
 from __future__ import print_function
 
 import sys
 import logging
 import pathlib
-import warnings
 import argparse
 import numpy as np
 import pyTMD
 
 # attempt imports
 try:
     import pyproj
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("pyproj not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.critical("pyproj not available")
 
 # PURPOSE: try to get the projection information for the input file
 def get_projection(attributes, PROJECTION):
     # coordinate reference system string from file
     try:
         crs = pyproj.CRS.from_string(attributes['projection'])
     except (ValueError,KeyError,pyproj.exceptions.CRSError):
```

### Comparing `pyTMD-2.0.5/scripts/reduce_OTIS_files.py` & `pyTMD-2.0.6/scripts/reduce_OTIS_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,30 +46,27 @@
         Program Data Center http://www.usap-dc.org/view/dataset/601235
     Updated 11/2019: added AOTIM-5-2018 tide model (2018 update to 2004 model)
     Written 08/2018
 """
 from __future__ import print_function
 
 import sys
+import logging
 import pathlib
-import warnings
 import argparse
 import numpy as np
 import pyTMD.io
 import pyTMD.utilities
 from pyTMD.convert_crs import convert_crs
 
 # attempt imports
 try:
     import pyproj
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("pyproj not available", ImportWarning)
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.critical("pyproj not available")
 
 # PURPOSE: try to get the projection information for the input file
 def get_projection(PROJECTION):
     # EPSG projection code
     try:
         crs = pyproj.CRS.from_epsg(int(PROJECTION))
     except (ValueError,pyproj.exceptions.CRSError):
```

### Comparing `pyTMD-2.0.5/scripts/usap_cats_tides.py` & `pyTMD-2.0.6/scripts/usap_cats_tides.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/scripts/verify_box_tpxo.py` & `pyTMD-2.0.6/scripts/verify_box_tpxo.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.5/setup.py` & `pyTMD-2.0.6/setup.py`

 * *Files identical despite different names*

