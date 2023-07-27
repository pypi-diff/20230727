# Comparing `tmp/pyspex-1.3.9.tar.gz` & `tmp/pyspex-1.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspex-1.3.9.tar", last modified: Wed Mar 29 15:22:14 2023, max compression
+gzip compressed data, was "pyspex-1.4.0rc1.tar", last modified: Thu Jul 27 11:11:09 2023, max compression
```

## Comparing `pyspex-1.3.9.tar` & `pyspex-1.4.0rc1.tar`

### file list

```diff
@@ -1,88 +1,96 @@
-drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.695713 pyspex-1.3.9/
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      188 2023-03-27 13:44:41.000000 pyspex-1.3.9/.gitignore
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      175 2023-03-27 13:44:41.000000 pyspex-1.3.9/.readthedocs.yaml
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      490 2023-03-27 13:44:41.000000 pyspex-1.3.9/CITATION.cff
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      915 2023-03-27 13:44:41.000000 pyspex-1.3.9/ChangeLog.md
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     1730 2023-03-27 13:44:41.000000 pyspex-1.3.9/INSTALL.md
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     1550 2023-03-27 13:44:41.000000 pyspex-1.3.9/LICENSE
--rw-rw-r--   0 richardh  (1000) richardh  (1000)        0 2023-03-27 13:44:41.000000 pyspex-1.3.9/MANIFEST.in
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     2683 2023-03-29 15:22:14.695713 pyspex-1.3.9/PKG-INFO
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     1609 2023-03-27 13:44:41.000000 pyspex-1.3.9/README.md
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      732 2023-03-27 13:44:41.000000 pyspex-1.3.9/ToDo.md
-drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.683713 pyspex-1.3.9/docs/
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      634 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/Makefile
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     1725 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/build.rst
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     1230 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/conf.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     1427 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/index.rst
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      800 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/make.bat
--rw-rw-r--   0 richardh  (1000) richardh  (1000)       49 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/modules.rst
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      335 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/pyspex.gen_l1a.rst
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     1058 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/pyspex.lib.rst
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     2846 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/pyspex.rst
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      426 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/quick.rst
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     7194 2023-03-27 13:44:41.000000 pyspex-1.3.9/docs/tools.rst
-drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.679713 pyspex-1.3.9/examples/
-drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.687713 pyspex-1.3.9/examples/l1agen_spex/
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    14960 2023-03-27 13:44:41.000000 pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE.20240324T143103.L1A.cdl
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    12158 2023-03-27 13:44:41.000000 pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE_CAL.20230105T143532.L1A.cdl
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    12158 2023-03-27 13:44:41.000000 pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE_DARK.20230105T143356.L1A.cdl
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    11929 2023-03-27 13:44:41.000000 pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE_OCAL.20240324T114855.L1A.cdl
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     3270 2023-03-27 13:44:41.000000 pyspex-1.3.9/examples/l1agen_spex/README.rst
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      670 2023-03-27 13:44:41.000000 pyspex-1.3.9/examples/l1agen_spex/run_393-398+hkt.yaml
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      356 2023-03-27 13:44:41.000000 pyspex-1.3.9/examples/l1agen_spex/run_429-432.yaml
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     1483 2023-03-29 15:20:38.000000 pyspex-1.3.9/pyproject.toml
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      375 2023-03-27 13:44:41.000000 pyspex-1.3.9/requirement.txt
-drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.687713 pyspex-1.3.9/scripts/
--rwxrwxr-x   0 richardh  (1000) richardh  (1000)      678 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/l1agen_spex.py
--rwxrwxr-x   0 richardh  (1000) richardh  (1000)     1823 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_add_egse2l1a.py
--rwxrwxr-x   0 richardh  (1000) richardh  (1000)     5382 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_add_ogse2l1a.py
--rwxrwxr-x   0 richardh  (1000) richardh  (1000)     9914 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_ccsds2l1a.py
--rwxrwxr-x   0 richardh  (1000) richardh  (1000)    15175 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_ckd_report.py
--rwxrwxr-x   0 richardh  (1000) richardh  (1000)     3168 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_csv2bin_tbl.py
--rwxrwxr-x   0 richardh  (1000) richardh  (1000)     8743 2023-03-29 10:24:36.000000 pyspex-1.3.9/scripts/spx1_dem2l1a.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     6312 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_l1a_select.py
--rwxrwxr-x   0 richardh  (1000) richardh  (1000)     4958 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_quicklook_lite.py
--rwxrwxr-x   0 richardh  (1000) richardh  (1000)    10216 2023-03-27 13:44:41.000000 pyspex-1.3.9/scripts/spx1_tif2l1a.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      434 2023-03-29 15:22:14.695713 pyspex-1.3.9/setup.cfg
-drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.679713 pyspex-1.3.9/src/
-drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.691713 pyspex-1.3.9/src/pyspex/
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      444 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/__init__.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     8700 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/binning_tables.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    20549 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/ccsds_io.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     8942 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/ckd_io.py
-drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.691713 pyspex-1.3.9/src/pyspex/data/
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     3321 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/data/tai-utc.dat
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    15467 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/dem_io.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    12901 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/egse_db.py
-drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.691713 pyspex-1.3.9/src/pyspex/gen_l1a/
--rw-rw-r--   0 richardh  (1000) richardh  (1000)        0 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/gen_l1a/__init__.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     2356 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/gen_l1a/cli.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     7325 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/hkt_io.py
-drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.695713 pyspex-1.3.9/src/pyspex/lib/
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      201 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lib/__init__.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     3507 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lib/attrs_def.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     8413 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lib/l1a_def.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    11384 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lib/l1b_def.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    15027 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lib/l1c_def.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     1617 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lib/leap_sec.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    26986 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lib/tmtc_def.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    24127 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lv0_io.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    10098 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lv1_args.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    10514 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lv1_gse.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    35163 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/lv1_io.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    13316 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/ogse_db.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     2318 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/ogse_dolp.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     5868 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/ogse_grande.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)    24872 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/ogse_helios.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     2984 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/ogse_laser.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     1459 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/spx_product.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     5373 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/tif_io.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     6786 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/tm_science.py
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      596 2023-03-27 13:44:41.000000 pyspex-1.3.9/src/pyspex/version.py
-drwxrwxr-x   0 richardh  (1000) richardh  (1000)        0 2023-03-29 15:22:14.691713 pyspex-1.3.9/src/pyspex.egg-info/
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     2683 2023-03-29 15:22:14.000000 pyspex-1.3.9/src/pyspex.egg-info/PKG-INFO
--rw-rw-r--   0 richardh  (1000) richardh  (1000)     1890 2023-03-29 15:22:14.000000 pyspex-1.3.9/src/pyspex.egg-info/SOURCES.txt
--rw-rw-r--   0 richardh  (1000) richardh  (1000)        1 2023-03-29 15:22:14.000000 pyspex-1.3.9/src/pyspex.egg-info/dependency_links.txt
--rw-rw-r--   0 richardh  (1000) richardh  (1000)       58 2023-03-29 15:22:14.000000 pyspex-1.3.9/src/pyspex.egg-info/entry_points.txt
--rw-rw-r--   0 richardh  (1000) richardh  (1000)      162 2023-03-29 15:22:14.000000 pyspex-1.3.9/src/pyspex.egg-info/requires.txt
--rw-rw-r--   0 richardh  (1000) richardh  (1000)        7 2023-03-29 15:22:14.000000 pyspex-1.3.9/src/pyspex.egg-info/top_level.txt
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-07-27 11:11:09.048174 pyspex-1.4.0rc1/
+-rw-r--r--   0 richardh  (1304) earth     (3300)      189 2023-07-07 14:08:26.000000 pyspex-1.4.0rc1/.gitignore
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-07-27 11:11:09.044174 pyspex-1.4.0rc1/.idea/
+-rw-r--r--   0 richardh  (1304) earth     (3300)       47 2023-03-29 18:38:01.000000 pyspex-1.4.0rc1/.idea/.gitignore
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-07-27 11:11:09.044174 pyspex-1.4.0rc1/.idea/inspectionProfiles/
+-rw-r--r--   0 richardh  (1304) earth     (3300)      911 2023-03-29 18:38:01.000000 pyspex-1.4.0rc1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      174 2023-03-29 18:38:01.000000 pyspex-1.4.0rc1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      311 2023-07-19 12:18:04.000000 pyspex-1.4.0rc1/.idea/misc.xml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      264 2023-03-29 18:38:01.000000 pyspex-1.4.0rc1/.idea/modules.xml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      509 2023-03-29 18:38:01.000000 pyspex-1.4.0rc1/.idea/pyspex.iml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      167 2023-03-29 18:38:01.000000 pyspex-1.4.0rc1/.idea/vcs.xml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      175 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/.readthedocs.yaml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      490 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/CITATION.cff
+-rw-r--r--   0 richardh  (1304) earth     (3300)      915 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/ChangeLog.md
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1730 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/INSTALL.md
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1550 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/LICENSE
+-rw-r--r--   0 richardh  (1304) earth     (3300)        0 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/MANIFEST.in
+-rw-r--r--   0 richardh  (1304) earth     (3300)     2686 2023-07-27 11:11:09.048174 pyspex-1.4.0rc1/PKG-INFO
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1609 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/README.md
+-rw-r--r--   0 richardh  (1304) earth     (3300)       73 2023-07-27 10:11:04.000000 pyspex-1.4.0rc1/ToDo.md
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-07-27 11:11:09.048174 pyspex-1.4.0rc1/docs/
+-rw-r--r--   0 richardh  (1304) earth     (3300)      634 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/docs/Makefile
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1725 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/docs/build.rst
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1230 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/docs/conf.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1427 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/docs/index.rst
+-rw-r--r--   0 richardh  (1304) earth     (3300)      800 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/docs/make.bat
+-rw-r--r--   0 richardh  (1304) earth     (3300)       55 2023-07-27 10:11:04.000000 pyspex-1.4.0rc1/docs/modules.rst
+-rw-r--r--   0 richardh  (1304) earth     (3300)      335 2023-07-27 10:04:52.000000 pyspex-1.4.0rc1/docs/pyspex.gen_l1a.rst
+-rw-r--r--   0 richardh  (1304) earth     (3300)      919 2023-07-27 10:11:04.000000 pyspex-1.4.0rc1/docs/pyspex.lib.rst
+-rw-r--r--   0 richardh  (1304) earth     (3300)     2678 2023-07-27 10:11:04.000000 pyspex-1.4.0rc1/docs/pyspex.rst
+-rw-r--r--   0 richardh  (1304) earth     (3300)      426 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/docs/quick.rst
+-rw-r--r--   0 richardh  (1304) earth     (3300)     7194 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/docs/tools.rst
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-07-27 11:11:09.048174 pyspex-1.4.0rc1/examples/
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-07-27 11:11:09.048174 pyspex-1.4.0rc1/examples/l1agen_spex/
+-rw-r--r--   0 richardh  (1304) earth     (3300)    14960 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/examples/l1agen_spex/PACE_SPEXONE.20240324T143103.L1A.cdl
+-rw-r--r--   0 richardh  (1304) earth     (3300)    12158 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/examples/l1agen_spex/PACE_SPEXONE_CAL.20230105T143532.L1A.cdl
+-rw-r--r--   0 richardh  (1304) earth     (3300)    12158 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/examples/l1agen_spex/PACE_SPEXONE_DARK.20230105T143356.L1A.cdl
+-rw-r--r--   0 richardh  (1304) earth     (3300)    11929 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/examples/l1agen_spex/PACE_SPEXONE_OCAL.20240324T114855.L1A.cdl
+-rw-r--r--   0 richardh  (1304) earth     (3300)     3286 2023-07-27 10:11:04.000000 pyspex-1.4.0rc1/examples/l1agen_spex/README.rst
+-rw-r--r--   0 richardh  (1304) earth     (3300)      670 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/examples/l1agen_spex/run_393-398+hkt.yaml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      356 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/examples/l1agen_spex/run_429-432.yaml
+-rw-r--r--   0 richardh  (1304) earth     (3300)     2004 2023-07-27 11:08:37.000000 pyspex-1.4.0rc1/examples/run_20230615.yaml
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1483 2023-03-29 18:33:17.000000 pyspex-1.4.0rc1/pyproject.toml
+-rw-r--r--   0 richardh  (1304) earth     (3300)      418 2023-07-27 11:08:37.000000 pyspex-1.4.0rc1/requirements.txt
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-07-27 11:11:09.048174 pyspex-1.4.0rc1/scripts/
+-rwxr-xr-x   0 richardh  (1304) earth     (3300)      678 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/scripts/l1agen_spex.py
+-rwxr-xr-x   0 richardh  (1304) earth     (3300)     1823 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/scripts/spx1_add_egse2l1a.py
+-rwxr-xr-x   0 richardh  (1304) earth     (3300)     5306 2023-03-29 18:38:01.000000 pyspex-1.4.0rc1/scripts/spx1_add_ogse2l1a.py
+-rwxr-xr-x   0 richardh  (1304) earth     (3300)    11001 2023-07-27 10:11:04.000000 pyspex-1.4.0rc1/scripts/spx1_ccsds2l1a.py
+-rwxr-xr-x   0 richardh  (1304) earth     (3300)    15175 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/scripts/spx1_ckd_report.py
+-rwxr-xr-x   0 richardh  (1304) earth     (3300)     3168 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/scripts/spx1_csv2bin_tbl.py
+-rwxr-xr-x   0 richardh  (1304) earth     (3300)     9776 2023-07-27 10:11:04.000000 pyspex-1.4.0rc1/scripts/spx1_dem2l1a.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     6317 2023-03-29 18:38:01.000000 pyspex-1.4.0rc1/scripts/spx1_l1a_select.py
+-rwxr-xr-x   0 richardh  (1304) earth     (3300)     5005 2023-03-30 10:01:34.000000 pyspex-1.4.0rc1/scripts/spx1_quicklook_lite.py
+-rwxr-xr-x   0 richardh  (1304) earth     (3300)    11454 2023-07-27 10:11:04.000000 pyspex-1.4.0rc1/scripts/spx1_tif2l1a.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)      434 2023-07-27 11:11:09.052174 pyspex-1.4.0rc1/setup.cfg
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-07-27 11:11:09.044174 pyspex-1.4.0rc1/src/
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-07-27 11:11:09.048174 pyspex-1.4.0rc1/src/pyspex/
+-rw-r--r--   0 richardh  (1304) earth     (3300)      489 2023-07-27 10:11:04.000000 pyspex-1.4.0rc1/src/pyspex/__init__.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     8866 2023-07-27 10:11:04.000000 pyspex-1.4.0rc1/src/pyspex/binning_tables.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    20543 2023-07-07 14:08:26.000000 pyspex-1.4.0rc1/src/pyspex/ccsds_io.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     7865 2023-07-27 11:08:37.000000 pyspex-1.4.0rc1/src/pyspex/ckd_io.py
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-07-27 11:11:09.048174 pyspex-1.4.0rc1/src/pyspex/data/
+-rw-r--r--   0 richardh  (1304) earth     (3300)     3321 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/src/pyspex/data/tai-utc.dat
+-rw-r--r--   0 richardh  (1304) earth     (3300)    15502 2023-03-29 18:38:01.000000 pyspex-1.4.0rc1/src/pyspex/dem_io.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    12931 2023-07-27 10:11:04.000000 pyspex-1.4.0rc1/src/pyspex/egse_db.py
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-07-27 11:11:09.048174 pyspex-1.4.0rc1/src/pyspex/gen_l1a/
+-rw-r--r--   0 richardh  (1304) earth     (3300)        0 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/src/pyspex/gen_l1a/__init__.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     2196 2023-07-27 11:08:37.000000 pyspex-1.4.0rc1/src/pyspex/gen_l1a/cli.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    13443 2023-07-27 11:08:37.000000 pyspex-1.4.0rc1/src/pyspex/hkt_io.py
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-07-27 11:11:09.048174 pyspex-1.4.0rc1/src/pyspex/lib/
+-rw-r--r--   0 richardh  (1304) earth     (3300)      201 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/src/pyspex/lib/__init__.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     3514 2023-07-27 10:11:04.000000 pyspex-1.4.0rc1/src/pyspex/lib/attrs_def.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     9799 2023-07-27 11:08:37.000000 pyspex-1.4.0rc1/src/pyspex/lib/l1a_def.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     1656 2023-07-11 08:16:08.000000 pyspex-1.4.0rc1/src/pyspex/lib/leap_sec.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     9524 2023-07-13 13:53:11.000000 pyspex-1.4.0rc1/src/pyspex/lib/tlm_utils.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    27034 2023-07-11 08:16:08.000000 pyspex-1.4.0rc1/src/pyspex/lib/tmtc_def.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    17973 2023-07-27 11:08:37.000000 pyspex-1.4.0rc1/src/pyspex/lv0_io.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    10500 2023-07-27 10:11:04.000000 pyspex-1.4.0rc1/src/pyspex/lv1_args.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    10552 2023-07-27 10:11:04.000000 pyspex-1.4.0rc1/src/pyspex/lv1_gse.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    19433 2023-07-27 11:08:37.000000 pyspex-1.4.0rc1/src/pyspex/lv1_io.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    13318 2023-07-27 11:08:37.000000 pyspex-1.4.0rc1/src/pyspex/ogse_db.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     2318 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/src/pyspex/ogse_dolp.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     5868 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/src/pyspex/ogse_grande.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    24872 2023-03-28 14:35:04.000000 pyspex-1.4.0rc1/src/pyspex/ogse_helios.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     3020 2023-07-27 11:08:37.000000 pyspex-1.4.0rc1/src/pyspex/ogse_laser.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)     5493 2023-07-27 11:08:37.000000 pyspex-1.4.0rc1/src/pyspex/tif_io.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)    26187 2023-07-27 11:08:37.000000 pyspex-1.4.0rc1/src/pyspex/tlm.py
+-rw-r--r--   0 richardh  (1304) earth     (3300)      719 2023-07-07 14:08:26.000000 pyspex-1.4.0rc1/src/pyspex/version.py
+drwxr-xr-x   0 richardh  (1304) earth     (3300)        0 2023-07-27 11:11:09.048174 pyspex-1.4.0rc1/src/pyspex.egg-info/
+-rw-r--r--   0 richardh  (1304) earth     (3300)     2686 2023-07-27 11:11:09.000000 pyspex-1.4.0rc1/src/pyspex.egg-info/PKG-INFO
+-rw-r--r--   0 richardh  (1304) earth     (3300)     2034 2023-07-27 11:11:09.000000 pyspex-1.4.0rc1/src/pyspex.egg-info/SOURCES.txt
+-rw-r--r--   0 richardh  (1304) earth     (3300)        1 2023-07-27 11:11:09.000000 pyspex-1.4.0rc1/src/pyspex.egg-info/dependency_links.txt
+-rw-r--r--   0 richardh  (1304) earth     (3300)       58 2023-07-27 11:11:09.000000 pyspex-1.4.0rc1/src/pyspex.egg-info/entry_points.txt
+-rw-r--r--   0 richardh  (1304) earth     (3300)      162 2023-07-27 11:11:09.000000 pyspex-1.4.0rc1/src/pyspex.egg-info/requires.txt
+-rw-r--r--   0 richardh  (1304) earth     (3300)        7 2023-07-27 11:11:09.000000 pyspex-1.4.0rc1/src/pyspex.egg-info/top_level.txt
```

### Comparing `pyspex-1.3.9/ChangeLog.md` & `pyspex-1.4.0rc1/ChangeLog.md`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/INSTALL.md` & `pyspex-1.4.0rc1/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/LICENSE` & `pyspex-1.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/PKG-INFO` & `pyspex-1.4.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspex
-Version: 1.3.9
+Version: 1.4.0rc1
 Summary: Software package to handle SPEXone Level-0 and Level-1 data
 Author-email: Richard van Hees <r.m.van.hees@sron.nl>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/rmvanhees/pyspex
 Project-URL: documentation, https://pyspex.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/rmvanhees/pyspex/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyspex-1.3.9/README.md` & `pyspex-1.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/docs/Makefile` & `pyspex-1.4.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/docs/build.rst` & `pyspex-1.4.0rc1/docs/build.rst`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/docs/conf.py` & `pyspex-1.4.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/docs/index.rst` & `pyspex-1.4.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/docs/make.bat` & `pyspex-1.4.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/docs/pyspex.lib.rst` & `pyspex-1.4.0rc1/docs/pyspex.lib.rst`

 * *Files 20% similar despite different names*

```diff
@@ -16,34 +16,26 @@
 --------------------------
 
 .. automodule:: pyspex.lib.l1a_def
    :members:
    :undoc-members:
    :show-inheritance:
 
-pyspex.lib.l1b\_def module
---------------------------
-
-.. automodule:: pyspex.lib.l1b_def
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-pyspex.lib.l1c\_def module
---------------------------
+pyspex.lib.leap\_sec module
+---------------------------
 
-.. automodule:: pyspex.lib.l1c_def
+.. automodule:: pyspex.lib.leap_sec
    :members:
    :undoc-members:
    :show-inheritance:
 
-pyspex.lib.leap\_sec module
----------------------------
+pyspex.lib.tlm\_utils module
+----------------------------
 
-.. automodule:: pyspex.lib.leap_sec
+.. automodule:: pyspex.lib.tlm_utils
    :members:
    :undoc-members:
    :show-inheritance:
 
 pyspex.lib.tmtc\_def module
 ---------------------------
```

### Comparing `pyspex-1.3.9/docs/pyspex.rst` & `pyspex-1.4.0rc1/docs/pyspex.rst`

 * *Files 2% similar despite different names*

```diff
@@ -129,34 +129,26 @@
 -------------------------
 
 .. automodule:: pyspex.ogse_laser
    :members:
    :undoc-members:
    :show-inheritance:
 
-pyspex.spx\_product module
---------------------------
-
-.. automodule:: pyspex.spx_product
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
 pyspex.tif\_io module
 ---------------------
 
 .. automodule:: pyspex.tif_io
    :members:
    :undoc-members:
    :show-inheritance:
 
-pyspex.tm\_science module
--------------------------
+pyspex.tlm module
+-----------------
 
-.. automodule:: pyspex.tm_science
+.. automodule:: pyspex.tlm
    :members:
    :undoc-members:
    :show-inheritance:
 
 pyspex.version module
 ---------------------
```

### Comparing `pyspex-1.3.9/docs/tools.rst` & `pyspex-1.4.0rc1/docs/tools.rst`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE.20240324T143103.L1A.cdl` & `pyspex-1.4.0rc1/examples/l1agen_spex/PACE_SPEXONE.20240324T143103.L1A.cdl`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE_CAL.20230105T143532.L1A.cdl` & `pyspex-1.4.0rc1/examples/l1agen_spex/PACE_SPEXONE_CAL.20230105T143532.L1A.cdl`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE_DARK.20230105T143356.L1A.cdl` & `pyspex-1.4.0rc1/examples/l1agen_spex/PACE_SPEXONE_DARK.20230105T143356.L1A.cdl`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/examples/l1agen_spex/PACE_SPEXONE_OCAL.20240324T114855.L1A.cdl` & `pyspex-1.4.0rc1/examples/l1agen_spex/PACE_SPEXONE_OCAL.20240324T114855.L1A.cdl`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/examples/l1agen_spex/README.rst` & `pyspex-1.4.0rc1/examples/l1agen_spex/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
    This command produces no L1A product. If you are interested in the content of the file
    then you can use the option `--dump`, which dumps the L0 data packages in ASCII.
    The output can be found in `SPX000000436.dump` and `SPX000000436_hk.dump`.
 
 Tests using YAML configuration
 ------------------------------
 Operational processing requires multiple file input, including SPEXone L0
-products and HKT products. The latter contain the navigation data, necessary to
-calculate the geolocation information in the L1B products.
+products and HKT products. The latter contain PACE navigation data, necessary
+for the determination of geo-location information by the L1A->L1B processor.
 
 #. This example uses as input multiple files, which contain a subset of the measurements
    we will perform inflight during eclipse. The measurements are performed in *diagnostic
    mode* (full frame) which are stored in the file:
    
     `PACE_SPEXONE_CAL.20230105T143532.L1A.nc`
    and *science mode* measurements stored in the file:
```

### Comparing `pyspex-1.3.9/examples/l1agen_spex/run_393-398+hkt.yaml` & `pyspex-1.4.0rc1/examples/l1agen_spex/run_393-398+hkt.yaml`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/pyproject.toml` & `pyspex-1.4.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/scripts/l1agen_spex.py` & `pyspex-1.4.0rc1/scripts/l1agen_spex.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/scripts/spx1_add_egse2l1a.py` & `pyspex-1.4.0rc1/scripts/spx1_add_egse2l1a.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/scripts/spx1_add_ogse2l1a.py` & `pyspex-1.4.0rc1/scripts/spx1_add_ogse2l1a.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,33 +64,33 @@
         add_ogse_ref_diode(args.ogse_dir / DB_REF_DIODE, args.l1a_file)
 
     if args.avantes:
         add_ogse_wav_mon(args.ogse_dir / DB_WAV_MON, args.l1a_file)
 
     if args.helios:
         xds = helios_spectrum()
-        xds.to_netcdf(args.l1a_file, mode='r+', format='NETCDF4',
+        xds.to_netcdf(args.l1a_file, mode='a',
                       group='/gse_data/ReferenceSpectrum')
 
     if args.grande:
         xds = gsfc_polarizer()
-        xds.to_netcdf(args.l1a_file, mode='r+', format='NETCDF4',
+        xds.to_netcdf(args.l1a_file, mode='a',
                       group='/gse_data/SpectralDolP')
         for n_lamps in (1, 2, 3, 5, 9):
             if args.l1a_file.name.find(f'-L{n_lamps:1d}_') > 0:
                 xds = grande_spectrum(n_lamps)
-                xds.to_netcdf(args.l1a_file, mode='r+', format='NETCDF4',
+                xds.to_netcdf(args.l1a_file, mode='a',
                               group='/gse_data/ReferenceSpectrum')
                 break
 
     if args.opo_laser:
         target_cwl = args.l1a_file.stem.split('_')[2].split('-')[-1]
         xds = read_gse_excel(args.ogse_dir, target_cwl)
         if xds is not None:
-            xds.to_netcdf(args.l1a_file, mode='r+', format='NETCDF4',
+            xds.to_netcdf(args.l1a_file, mode='a',
                           group='/gse_data/OPO_laser')
 
 
 # - main function ----------------------------------
 def main():
     """Main function."""
     # parse command-line parameters
```

### Comparing `pyspex-1.3.9/scripts/spx1_ccsds2l1a.py` & `pyspex-1.4.0rc1/scripts/spx1_ccsds2l1a.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,20 +18,43 @@
 
 import numpy as np
 
 from pyspex.ccsds_io import CCSDSio
 from pyspex.lib.tmtc_def import tmtc_dtype
 from pyspex.lv0_io import hk_sec_of_day, img_sec_of_day
 from pyspex.lv1_io import L1Aio
-from pyspex.spx_product import get_l1a_name
+from pyspex.version import pyspex_version
 
 # - global parameters ------------------------------
 EPOCH = datetime(1970, 1, 1, tzinfo=timezone.utc)
 
 
+# - local functions --------------------------------
+def get_l1a_name(msm_id: str) -> str:
+    """
+    Return name of SPEXone product for OCAL measurements (@SRON).
+
+    Parameters
+    ----------
+    msm_id : string, optional
+       Provide identifier for measurement, OCAL only
+
+    Notes
+    -----
+    L1A file name format:
+       SPX1_OCAL_<msm_id>[_YYYYMMDDTHHMMSS]_L1A_vvvvvvv.nc
+    where
+       msm_id is the measurement identifier
+       YYYYMMDDTHHMMSS is time stamp of the first image in the file
+       vvvvvvv is the git-hash string of the pyspex repository
+    """
+    # define string of sensing start as yyyymmddThhmmss
+    return f'SPX1_OCAL_{msm_id}_L1A_{pyspex_version(githash=True)}.nc'
+
+
 # - main function ----------------------------------
 def main():
     """
     main function
 
     Examples
     --------
@@ -69,15 +92,14 @@
                               ' msmt_id+"_hk" (also without extension).'))
     args = parser.parse_args()
     if args.verbose:
         print(args)
 
     # Read Science packages
     data_dir = args.msmt_id.parent
-    sci_files = []
     if not args.pdump:
         sci_files = sorted(data_dir.glob(args.msmt_id.name + '.[0-9]')) \
             + sorted(data_dir.glob(args.msmt_id.name + '.?[0-9]'))
     else:
         sci_files = [args.msmt_id]
 
     packets = ()
@@ -192,15 +214,15 @@
         us100 = np.round(10000 * img_subsec.astype(float) / 65536)
         buff = us100 + img_sec - 10000
         us100 = buff.astype('u8') % 10000
         img_subsec = ((us100 << 16) // 10000).astype('u2')
 
     ref_date, img_time = img_sec_of_day(img_sec, img_subsec, img_hk)
 
-    # extract timestaps and telemetry of NomHK data
+    # extract timestamps and telemetry of NomHK data
     if nomhk_tm:
         nomhk_sec = np.empty(len(nomhk_tm), dtype='u4')
         nomhk_subsec = np.empty(len(nomhk_tm), dtype='u2')
         nomhk_data = np.empty(len(nomhk_tm), dtype=tmtc_dtype(0x320))
         for ii, packet in enumerate(nomhk_tm):
             nomhk_sec[ii] = packet['packet_header']['tai_sec']
             nomhk_subsec[ii] = packet['packet_header']['sub_sec']
@@ -227,15 +249,15 @@
     try:
         new_date = datetime.strptime(
             msm_id[-22:], '%y-%j-%H:%M:%S.%f').strftime('%Y%m%dT%H%M%S.%f')
     except ValueError:
         pass
     else:
         msm_id = msm_id[:-22] + new_date
-    prod_name = get_l1a_name(msm_id, None)
+    prod_name = get_l1a_name(msm_id)
 
     # pylint: disable=unsubscriptable-object
     n_frame = 1 if img_data.ndim == 1 else img_data.shape[0]
     n_sample = img_data.size if img_data.ndim == 1 else img_data.shape[1]
     if args.verbose:
         print(f'[INFO]: dimension of images [{n_frame},{n_sample}]')
     dims = {'number_of_images': n_frame,
@@ -244,26 +266,33 @@
             'SC_records': None}
 
     # Generate L1A product
     with L1Aio(args.datapath / prod_name, dims=dims,
                ref_date=ref_date.date()) as l1a:
         # write image data, detector telemetry and image attributes
         l1a.fill_science(img_data, img_hk, img_id)
+
         l1a.set_dset('/image_attributes/icu_time_sec', img_sec)
+        l1a.set_attr('valid_min', np.uint32(1577800000),
+                     ds_name='/image_attributes/icu_time_sec')
+        l1a.set_attr('valid_max', np.uint32(1735700000),
+                     ds_name='/image_attributes/icu_time_sec')
+        l1a.set_attr('units', "seconds since 1970-01-01 00:00:00",
+                     ds_name='/image_attributes/icu_time_sec')
         l1a.set_dset('/image_attributes/icu_time_subsec', img_subsec)
         l1a.set_dset('/image_attributes/image_time', img_time)
 
         # write engineering data
         if nomhk_tm:
             l1a.fill_nomhk(nomhk_data)
             hk_time = hk_sec_of_day(nomhk_sec, nomhk_subsec, ref_date)
             l1a.set_dset('/engineering_data/HK_tlm_time', hk_time)
 
         if demhk_tm:
-            l1a.fill_demhk(demhk_data)
+            l1a.set_dset('/engineering_data/DemHK_telemetry', demhk_data)
 
         # write global attributes
         l1a.fill_global_attrs(inflight=False)
         l1a.set_attr('input_files', [Path(x).name for x in sci_files])
 
 
 # --------------------------------------------------
```

### Comparing `pyspex-1.3.9/scripts/spx1_ckd_report.py` & `pyspex-1.4.0rc1/scripts/spx1_ckd_report.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/scripts/spx1_csv2bin_tbl.py` & `pyspex-1.4.0rc1/scripts/spx1_csv2bin_tbl.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/scripts/spx1_dem2l1a.py` & `pyspex-1.4.0rc1/scripts/spx1_dem2l1a.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,38 +13,63 @@
 The DEM measurements are performed at SRON between 17-10-2019 and 13-12-2019.
 
 References
 ----------
 * SRON-SPEX-TN-2020-001_0_5_SPEXone_Detector_Characterization.pdf
 """
 import argparse
-from datetime import datetime, timezone
+from datetime import datetime, timedelta, timezone
 from pathlib import Path
 
 import h5py
 import numpy as np
 
 from pyspex.dem_io import DEMio
 from pyspex.lib.tmtc_def import tmtc_dtype
 from pyspex.lv0_io import img_sec_of_day
 from pyspex.lv1_gse import LV1gse
 from pyspex.lv1_io import L1Aio
-from pyspex.spx_product import get_l1a_name
+from pyspex.version import pyspex_version
 
 # - global parameters ------------------------------
 EPOCH = datetime(1970, 1, 1, tzinfo=timezone.utc)
 
 
 # - local functions --------------------------------
+def get_l1a_name(msm_id: str, utc_sensing_start: datetime) -> str:
+    """
+    Return name of SPEXone product for DEM measurements.
+
+    Parameters
+    ----------
+    msm_id : string, optional
+       Provide identifier for measurement, OCAL only
+    utc_sensing_start: datetime
+       Provide sensing start of first measurement in L1A product
+
+    Notes
+    -----
+    L1A file name format:
+       SPX1_OCAL_<msm_id>[_YYYYMMDDTHHMMSS]_L1A_vvvvvvv.nc
+    where
+       msm_id is the measurement identifier
+       YYYYMMDDTHHMMSS is time stamp of the first image in the file
+       vvvvvvv is the git-hash string of the pyspex repository
+    """
+    # define string of sensing start as yyyymmddThhmmss
+    sensing_start = utc_sensing_start.strftime("%Y%m%dT%H%M%S")
+
+    return (f'SPX1_OCAL_{msm_id}_{sensing_start}'
+            f'_L1A_{pyspex_version(githash=True)}.nc')
 
 
 # - main function ----------------------------------
 def main():
     """
-    main program to illustate the creation of a L1A calibration product
+    main program to illustrate the creation of a L1A calibration product
     """
     parser = argparse.ArgumentParser(
         description='create SPEXone L1A product from DEM measurement(s)')
     parser.add_argument('--verbose', default=False, action='store_true',
                         help='be verbose, default be silent')
     parser.add_argument('--reference', default=None,
                         help='reference detector data (for non-linearity)')
@@ -62,27 +87,21 @@
 
     # sort file on timestamp in filename (problem: midnight...)
     buff = [name for name in args.file_list if name.endswith('.bin')]
     args.file_list = sorted(buff, key=lambda name: name.split('_')[-2])
 
     # obtain DEM_ID (can be specified on command-line)
     # and list of measurements used to generate the L1A product
-    list_dem_id = []
-    for file in args.file_list:
-        parts = Path(file).parts
-        if len(parts) > 2:
-            list_dem_id.append(parts[-2].split('_')[1])
-
     if args.dem_id is None:
         dem_id_list = []
         for file in args.file_list:
             parts = Path(file).parts
             if len(parts) == 1:
                 continue
-            for dem_id in ('D35', 'D39'):
+            for dem_id in ('D35', 'D39', 'D84'):
                 if parts[-2].find(dem_id) != -1:
                     dem_id_list.append(dem_id)
 
         if not dem_id_list:
             raise KeyError(
                 'Can not determine DEM_ID, please specify --dem_id')
         dem_id_list = set(dem_id_list)
@@ -186,28 +205,35 @@
     dims = {'number_of_images': n_images,
             'samples_per_image': n_samples,
             'hk_packets': 0}
 
     # generate L1A product
     with L1Aio(prod_name, dims=dims, ref_date=ref_date.date()) as l1a:
         # write image data, detector telemetry and image attributes
-        l1a.fill_science(images.reshape(n_images, n_samples), img_hk,
-                         np.arange(n_images))
+        l1a.fill_science(images.reshape(n_images, n_samples),
+                         img_hk, np.arange(n_images))
+
         l1a.set_dset('/image_attributes/icu_time_sec', img_sec)
         l1a.set_attr('valid_min', np.uint32(1577800000),
                      ds_name='/image_attributes/icu_time_sec')
         l1a.set_attr('valid_max', np.uint32(1735700000),
                      ds_name='/image_attributes/icu_time_sec')
         l1a.set_attr('units', "seconds since 1970-01-01 00:00:00",
                      ds_name='/image_attributes/icu_time_sec')
         l1a.set_dset('/image_attributes/icu_time_subsec', img_subsec)
         l1a.set_dset('/image_attributes/image_time', img_time)
 
         # Global attributes
         l1a.fill_global_attrs(inflight=False)
+        if len(tstamp) == 1:
+            tstamp.append(tstamp[0] + timedelta(seconds=t_frm[0]))
+        l1a.set_attr('time_coverage_start',
+                     tstamp[0].isoformat(timespec='milliseconds'))
+        l1a.set_attr('time_coverage_end',
+                     tstamp[-1].isoformat(timespec='milliseconds'))
         l1a.set_attr('input_files', [Path(x).name for x in args.file_list])
 
     # Add OGSE and EGSE parameters
     # - Light source
     # - DoLP
     # - AoLP
     # - FOV_begin
```

### Comparing `pyspex-1.3.9/scripts/spx1_l1a_select.py` & `pyspex-1.4.0rc1/scripts/spx1_l1a_select.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     # ----- now we can update the name of the output product -----
     # - because the production time has changed
     # - and when coverage time is changed
     if l1a_filename.is_file() and l1a_product.samefile(l1a_filename):
         raise OSError('Output will overwrite original product')
 
     # ----- write new output product with selected data -----
-    with L1Aio(l1a_filename, reference_day.date(), dims=dims) as l1a:
+    with L1Aio(str(l1a_filename), reference_day.date(), dims=dims) as l1a:
         # write image data, detector telemetry and image attributes
         l1a.fill_science(img_data, img_hk, img_id)
         l1a.set_dset('/image_attributes/icu_time_sec', img_sec)
         l1a.set_dset('/image_attributes/icu_time_subsec', img_subsec)
         l1a.set_dset('/image_attributes/image_time', img_time)
 
         # write engineering data
```

### Comparing `pyspex-1.3.9/scripts/spx1_quicklook_lite.py` & `pyspex-1.4.0rc1/scripts/spx1_quicklook_lite.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     Main function of this module
     """
     parser = argparse.ArgumentParser(
         description='create Quick-Look from SPEXone L1A product')
     parser.add_argument('--verbose', default=False, action='store_true',
                         help='be verbose, default be silent')
     parser.add_argument('--show_images', type=str, default=None,
-                        help='comma seperated list, default use --max_images')
+                        help='comma separated list, default use --max_images')
     parser.add_argument('--max_images', type=int, default=20,
                         help='maximum number of images in quick-look (20)')
     parser.add_argument('file_list', nargs='*',
                         help='provide name of L1A product')
     args = parser.parse_args()
     if args.verbose:
         print(args)
@@ -73,14 +73,15 @@
             sci_hk = fid['/science_data/detector_telemetry'][:]
             dset = fid['/science_data/detector_images']
             # pylint: disable=no-member
             images = dset.astype(float)[:]
         try:
             coverage_start = coverage_start.decode()
         except (UnicodeDecodeError, AttributeError):
+            date_start = "1970-01-01T00:00:00"
             pass
         else:
             date_start = coverage_start.split('.')[0]
 
         data_dir = flname.parent / 'QuickLook'
         if not data_dir.is_dir():
             data_dir.mkdir(mode=0o755)
```

### Comparing `pyspex-1.3.9/scripts/spx1_tif2l1a.py` & `pyspex-1.4.0rc1/scripts/spx1_tif2l1a.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,30 +10,29 @@
 # License:  BSD-3-Clause
 """
 Python implementation SPEXone instrument simulator output to L1A.
 
 Environment::
 
    CKD_DIR:  directory with SPEXone CKD, default is CWD.
-
 """
 import argparse
 from datetime import datetime, timezone
 from os import environ
 from pathlib import Path
 
 import h5py
 import numpy as np
 import xarray as xr
 
 from pyspex.lib.tmtc_def import tmtc_dtype
 from pyspex.lv1_gse import LV1gse
 from pyspex.lv1_io import L1Aio
-from pyspex.spx_product import get_l1a_name
 from pyspex.tif_io import TIFio
+from pyspex.version import pyspex_version
 
 # - global parameters ------------------------------
 EPOCH = datetime(1970, 1, 1, tzinfo=timezone.utc)
 
 
 # - local functions --------------------------------
 def get_table_id(ckd_dir, bin_table_name):
@@ -82,14 +81,41 @@
                            coords=[ds_dict['Wavelength (nm)']],
                            attrs={'long_name': 'signal of stimulus',
                                   'units': 'W.m-2.sr-1.um-1'})
 
     return xr.Dataset({'wavelength': xr_wv, 'signal': xr_sign})
 
 
+def get_l1a_name(msm_id: str, utc_sensing_start: datetime) -> str:
+    """
+    Return name of SPEXone product for DEM measurements.
+
+    Parameters
+    ----------
+    msm_id : string, optional
+       Provide identifier for measurement, OCAL only
+    utc_sensing_start: datetime
+       Provide sensing start of first measurement in L1A product
+
+    Notes
+    -----
+    L1A file name format:
+       SPX1_OCAL_<msm_id>[_YYYYMMDDTHHMMSS]_L1A_vvvvvvv.nc
+    where
+       msm_id is the measurement identifier
+       YYYYMMDDTHHMMSS is time stamp of the first image in the file
+       vvvvvvv is the git-hash string of the pyspex repository
+    """
+    # define string of sensing start as yyyymmddThhmmss
+    sensing_start = utc_sensing_start.strftime("%Y%m%dT%H%M%S")
+
+    return (f'SPX1_OCAL_{msm_id}_{sensing_start}'
+            f'_L1A_{pyspex_version(githash=True)}.nc')
+
+
 # - main function ----------------------------------
 def main():
     """
     main program to illustate the creation of a L1A calibration product
 
     Environment
     -----------
@@ -209,17 +235,24 @@
     sci_hk['DET_EXPTIME'] = \
         int(1e7 * float(hdr['Exposure time (s)']) / 129 - 0.43 * 20)
     sci_hk['REG_NCOADDFRAMES'] = int(hdr['Co-additions'])
 
     # Generate L1A product
     with L1Aio(prod_name, dims=dims, ref_date=utc_start.date()) as l1a:
         # write image data, detector telemetry and image attributes
-        l1a.fill_science(images.reshape(n_images, -1), sci_hk,
-                         np.arange(n_images))
+        l1a.fill_science(images.reshape(n_images, -1),
+                         sci_hk, np.arange(n_images))
+
         l1a.set_dset('/image_attributes/icu_time_sec', img_sec)
+        l1a.set_attr('valid_min', np.uint32(1577800000),
+                     ds_name='/image_attributes/icu_time_sec')
+        l1a.set_attr('valid_max', np.uint32(1735700000),
+                     ds_name='/image_attributes/icu_time_sec')
+        l1a.set_attr('units', "seconds since 1970-01-01 00:00:00",
+                     ds_name='/image_attributes/icu_time_sec')
         l1a.set_dset('/image_attributes/icu_time_subsec', img_subsec)
         l1a.set_dset('/image_attributes/image_time', img_time)
 
         # Engineering data
         l1a.fill_nomhk(nom_hk)
         l1a.set_dset('/engineering_data/HK_tlm_time', img_time)
```

### Comparing `pyspex-1.3.9/src/pyspex/binning_tables.py` & `pyspex-1.4.0rc1/src/pyspex/binning_tables.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 #    All Rights Reserved
 #
 # License:  BSD-3-Clause
 """
 This module contains the class `BinningTables` to deal with SPEXone
 binning-tables or to generate a file with binning-table definitions.
 """
+from __future__ import annotations
 __all__ = ['BinningTables']
 
 from datetime import datetime, timezone
 from os import environ
 from pathlib import Path
 
-import netCDF4 as nc4
 import numpy as np
+# pylint: disable=no-name-in-module
+from netCDF4 import Dataset
 
 from .version import pyspex_version
 
 # - global parameters ------------------------------
 FILL_VALUE = 0xFFFFFFFF  # 0X7FFFFFFF
 
 
@@ -49,15 +51,15 @@
     where yyyymmddTHHMMSS defines the validity start (UTC) and NNN the
     release number of the file format.
 
     The binning tables as defined on-ground are supposed to be available
     during the whole mission at the same on-board memory location.
     Because these original binning tables are necessary for re-processing
     and may facilitate instrument performance monitoring.
-    Therefore, it is prefered that a new binning table is added to the
+    Therefore, it is preferred that a new binning table is added to the
     current set, without changing the validity start string.
     However, new binning-table file should be released in case any of the
     binning tables are overwritten.
 
     Examples
     --------
     # create new file with binning-table definitions::
@@ -75,29 +77,29 @@
 
     # use binning-table '130' to unbin SPEXone detector data::
 
     > bin_tbl BinningTables()
     > bin_tbl.search(coverage_start)
     > img = bin_tbl.unbin(130, img_binned)
     """
-    def __init__(self, ckd_dir=None) -> None:
+    def __init__(self, ckd_dir: str | None = None) -> None:
         """Initialize class attributes.
         """
         if ckd_dir is None:
             self.ckd_dir = Path('/nfs/SPEXone/share/ckd')
             if not self.ckd_dir.is_dir():
                 self.ckd_dir = Path(environ.get('CKD_DIR', '.'))
         else:
             self.ckd_dir = Path(ckd_dir)
         if not self.ckd_dir.is_dir():
             raise FileNotFoundError('directory with SPEXone CKD does not exist')
 
         self.ckd_file = None
 
-    def create_if_needed(self, validity_start: str, release=1) -> None:
+    def create_if_needed(self, validity_start: str, release: int = 1) -> None:
         """Initialize CKD file for binning tables if not exist.
 
         Parameters
         ----------
         validity_start: str
            Validity start of the CKD data, as ``yyyymmddTHHMMSS``
         release :  int, default=1
@@ -105,30 +107,30 @@
         """
         self.ckd_file = f'SPX1_CKD_BIN_TBL_{validity_start}_{release:03d}.nc'
 
         if (self.ckd_dir / self.ckd_file).is_file():
             return
 
         # initialize netCDF file with binning tables
-        with nc4.Dataset(self.ckd_dir / self.ckd_file, 'w') as fid:
+        with Dataset(self.ckd_dir / self.ckd_file, 'w') as fid:
             fid.title = 'SPEXone Level-1 binning-tables'
-            fid.Convensions = 'CF-1.6'
+            fid.Conventions = 'CF-1.6'
             fid.project = 'PACE Project'
             fid.instrument = 'SPEXone'
             fid.institution = 'SRON Netherlands Institute for Space Research'
             fid.processing_version = pyspex_version()
             fid.validity_start = validity_start + '+00:00'
             fid.release_number = np.uint16(release)
             fid.date_created = datetime.now(timezone.utc).isoformat(
                 timespec='seconds')
 
             fid.createDimension('row', 1024)
             fid.createDimension('column', 1024)
 
-    def search(self, coverage_start=None) -> None:
+    def search(self, coverage_start: str | None = None) -> None:
         """Search CKD file with binning tables.
 
         Parameters
         ----------
         coverage_start : str, default=None
            time_coverage_start or start of the measurement (UTC)
 
@@ -154,30 +156,31 @@
                                               '%Y%m%dT%H%M%S%z')
             if validity_date < coverage_date:
                 self.ckd_file = ckd_fl
                 break
         else:
             raise FileNotFoundError('No valid CKD with binning tables found')
 
-    def add_table(self, table_id: int, lineskip_arr, binning_table) -> None:
+    def add_table(self, table_id: int, lineskip_arr: np.ndarray,
+                  binning_table: np.ndarray) -> None:
         """Add a binning table definition to existing file.
 
         Parameters
         ----------
         table_id :  int
            Table identifier (integer between 1 and 255)
         lineskip_arr :  ndarray
            Lineskip array definition
         binning_table :  ndarray
            Binning table definition
         """
         index, count = np.unique(binning_table[lineskip_arr == 1, :],
                                  return_counts=True)
 
-        with nc4.Dataset(self.ckd_dir / self.ckd_file, 'r+') as fid:
+        with Dataset(self.ckd_dir / self.ckd_file, 'r+') as fid:
             gid = fid.createGroup(f'/Table_{table_id:03d}')
             gid.tabel_id = table_id
             gid.REG_BINNING_TABLE_START = hex(0x80000000
                                               + 0x400000 * (table_id - 1))
             gid.enabled_lines = np.uint16(lineskip_arr.sum())
             gid.flex_binned_pixels = np.uint32(index.max()+1)
             gid.date_created = datetime.now(timezone.utc).isoformat(
@@ -203,30 +206,30 @@
             dset = gid.createVariable('count_table', 'u2', ('bins',),
                                       zlib=True, complevel=1, shuffle=True)
             dset.long_name = 'number of aggregated pixel readings'
             dset.valid_min = np.uint16(0)
             dset.valid_max = np.uint16(count.max())
             dset[:] = count.astype('u2')
 
-    def unbin(self, table_id: int, img_binned):
+    def unbin(self, table_id: int, img_binned: np.ndarray) -> np.ndarray:
         """Return unbinned detector data.
 
         Parameters
         ----------
         table_id :  int
            Table identifier (integer between 1 and 255)
         img_binned : np.ndarray
            Binned image data (1D array)
 
         Returns
         -------
-        numpy.ndarray
+        np.ndarray
            Unbinned image data (no interpolation).
         """
-        with nc4.Dataset(self.ckd_dir / self.ckd_file, 'r') as fid:
+        with Dataset(self.ckd_dir / self.ckd_file, 'r') as fid:
             if f'Table_{table_id:03d}' not in fid.groups:
                 raise KeyError(f'Table_{table_id:03d} not defined')
             gid = fid[f'Table_{table_id:03d}']
             binning_table = gid.variables['binning_table'][:]
             lineskip_arr = gid.variables['lineskip_arr'][:]
             count_table = gid.variables['count_table'][:]
```

### Comparing `pyspex-1.3.9/src/pyspex/ccsds_io.py` & `pyspex-1.4.0rc1/src/pyspex/ccsds_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from .lib.tmtc_def import tmtc_dtype
 
 # - global parameters ------------------------------
 # Define parameters of Primary header
 #  - Packet type     (3 bits): Version No.
 #                              Indicates this is a CCSDS version 1 packet
 #                     (1 bit): Type indicator
-#                              Indicates this is a telemetery packet
+#                              Indicates this is a telemetry packet
 #                     (1 bit): Secondary flag
 #                              Indicate presence of Secondary header
 #                   (11 bits): ApID
 #                              SPEXone ApID [0x320 - 0x351] or 2047
 #
 #  - Packet Sequence (2 bits): Grouping flag
 #                              00 continuation packet-data segment
@@ -57,16 +57,16 @@
 
 SCIHK_DTYPE = tmtc_dtype(0x350)
 
 # - Error messages ------------------------
 MSG_SKIP_FRAME = "[WARNING]: rejected a frame because it's incomplete"
 MSG_INVALID_APID = \
     '[WARNING]: found one or more telemetry packages with an invalid APID'
-MSG_CORRUPT_APID = 'corrupted segements - detected APID 1 after <> 2'
-MSG_CORRUPT_FRAME = 'corrupted segements - previous frame not closed'
+MSG_CORRUPT_APID = 'corrupted segments - detected APID 1 after <> 2'
+MSG_CORRUPT_FRAME = 'corrupted segments - previous frame not closed'
 
 
 # - class CCSDSio -------------------------
 class CCSDSio:
     """Read SPEXone telemetry packets.
 
     Parameters
@@ -317,15 +317,15 @@
         packet = np.empty(1, dtype=np.dtype([
             ('packet_header', HDR_DTYPE),
             ('science_hk', SCIHK_DTYPE),
             ('icu_time', TIME_DTYPE),
             ('image_data', 'O')]))
         packet['packet_header'] = hdr
 
-        # first segement or unsegmented data packet provides Science_HK
+        # first segment or unsegmented data packet provides Science_HK
         if self.grouping_flag in (1, 3):
             packet['science_hk'] = self.fix_sci_hk24(
                 np.fromfile(self.fp, count=1, dtype=SCIHK_DTYPE))
             num_bytes -= SCIHK_DTYPE.itemsize
             packet['icu_time'] = np.fromfile(self.fp, count=1,
                                              dtype=TIME_DTYPE)
             num_bytes -= TIME_DTYPE.itemsize
@@ -528,15 +528,15 @@
            unsegmented Science telemetry packages
         """
         # reject non-Science telemetry packages
         packets = self.select_tm(packets_in, 0x350)
         if not packets:
             return ()
 
-        # check if grouping_flag of first segement equals 1
+        # check if grouping_flag of first segment equals 1
         #   else reject all segments with grouping_flag != 1
         self.__hdr = packets[0]['packet_header']
         if self.grouping_flag != 1:
             ii = 0
             for packet in packets:
                 self.__hdr = packet['packet_header']
                 if self.grouping_flag == 1:
@@ -544,15 +544,15 @@
                 ii += 1
 
             print(f'[WARNING]: first frame incomplete - skipped {ii} segments')
             packets = packets[ii:]
             if not packets:
                 return ()
 
-        # check if grouping_flag of last segement equals 2
+        # check if grouping_flag of last segment equals 2
         #   else reject all segments after the last segment
         #   with grouping_flag == 2
         self.__hdr = packets[-1]['packet_header']
         if self.grouping_flag != 2:
             ii = 0
             for packet in packets:
                 self.__hdr = packet['packet_header']
```

### Comparing `pyspex-1.3.9/src/pyspex/ckd_io.py` & `pyspex-1.4.0rc1/src/pyspex/ckd_io.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 """
 Contains the class CKDio to read SPEXone CKD.
 
 References
 ----------
 * https://spexone-cal-doc.readthedocs.io/en/latest/
 """
+from __future__ import annotations
 __all__ = ['CKDio']
 
 from datetime import datetime, timezone
 from pathlib import Path
 
 import h5py
 import xarray as xr
@@ -73,15 +74,15 @@
         """Make sure that we close all resources.
         """
         if self.fid is not None:
             self.fid.close()
 
     @property
     def processor_version(self) -> str:
-        """Return the version of the spexone_cal program.
+        """Return the version of the `spexone_cal` program.
         """
         # pylint: disable=no-member
         return self.fid.attrs['processor_version'].decode()
 
     def date_created(self, compact=False) -> str:
         """Return creation date of the CKD product.
 
@@ -96,15 +97,15 @@
         if compact:
             return date_t.astimezone(tz=timezone.utc).strftime("%Y%m%d%H%M%S")
 
         return date_t.astimezone(tz=timezone.utc).isoformat()[:-6]
 
     @property
     def git_commit(self) -> str:
-        """Return git hash of repository spexone_cal, used to generate the CKD.
+        """Return git hash of repository `spexone_cal`, used to generate the CKD.
         """
         # pylint: disable=no-member
         return self.fid.attrs['git_commit'].decode()
 
     def dark(self) -> xr.Dataset | None:
         """Read Dark CKD.
 
@@ -263,44 +264,7 @@
         except KeyError:
             return None
         res = ()
         res += (h5_to_xr(gid['pol_m_q']),)
         res += (h5_to_xr(gid['pol_m_u']),)
         res += (h5_to_xr(gid['pol_m_t']),)
         return xr.merge(res, combine_attrs='drop_conflicts')
-
-
-# - main function ----------------------------------
-def __test():
-    """Small function to test this module.
-    """
-    ckd_dir = Path('/data/richardh/SPEXone/CKD')
-    if not ckd_dir.is_dir():
-        ckd_dir = Path('/data/richardh/SPEXone/share/ckd')
-    ckd_file = ckd_dir / 'CKD_reference_20220916_174632.nc'
-    if not ckd_file.is_file():
-        raise FileNotFoundError(f'{ckd_file} does not exist')
-
-    with CKDio(ckd_file) as ckd:
-        print(ckd.processor_version)
-        print(ckd.date_created())
-        print('# --- dark ---')
-        print(ckd.dark())
-        print('# --- noise ---')
-        print(ckd.noise())
-        print('# --- nlin ---')
-        print(ckd.nlin())
-        print('# --- prnu ---')
-        print(ckd.prnu())
-        print('# --- fov ---')
-        print(ckd.fov())
-        print('# --- wavelength ---')
-        print(ckd.wavelength())
-        print('# --- radiometric ---')
-        print(ckd.radiometric())
-        print('# --- polarimetric ---')
-        print(ckd.polarimetric())
-
-
-# --------------------------------------------------
-if __name__ == '__main__':
-    __test()
```

### Comparing `pyspex-1.3.9/src/pyspex/data/tai-utc.dat` & `pyspex-1.4.0rc1/src/pyspex/data/tai-utc.dat`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/src/pyspex/dem_io.py` & `pyspex-1.4.0rc1/src/pyspex/dem_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Copyright (c) 2019-2023 SRON - Netherlands Institute for Space Research
 #    All Rights Reserved
 #
 # License:  BSD-3-Clause
 """
 Contains the class `DEMio` to read SPEXone CMV4000 detector data.
 """
+from __future__ import annotations
 __all__ = ['DEMio']
 
 from pathlib import Path
 
 import numpy as np
 
 from .lib.tmtc_def import tmtc_dtype
```

### Comparing `pyspex-1.3.9/src/pyspex/egse_db.py` & `pyspex-1.4.0rc1/src/pyspex/egse_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 """
 __all__ = ['create_egse_db', 'add_egse_data']
 
 from datetime import datetime, timedelta, timezone
 from pathlib import Path
 
 import h5py
-import netCDF4 as nc4
 import numpy as np
+# pylint: disable=no-name-in-module
+from netCDF4 import Dataset
 
 # - global parameters ------------------------------
 DB_EGSE = 'egse_db_itos.nc'
 
 # enumerate source status
 LDLS_DICT = {b'UNPLUGGED': 0, b'Controller Fault': 1, b'Idle': 2,
              b'Laser ON': 3, b'Lamp ON': 4, b'MISSING': 255}
@@ -228,15 +229,15 @@
         try:
             res = read_egse(egse_file, verbose=args.verbose)
         except RuntimeError:
             return
 
         egse = res[0] if egse is None else np.concatenate((egse, res[0]))
 
-    with nc4.Dataset(args.egse_dir / DB_EGSE, 'w', format='NETCDF4') as fid:
+    with Dataset(args.egse_dir / DB_EGSE, 'w', format='NETCDF4') as fid:
         fid.input_files = [Path(x).name for x in args.file_list]
         fid.creation_date = \
             datetime.now(timezone.utc).isoformat(timespec='seconds')
 
         _ = fid.createEnumType('u1', 'ldls_t',
                                {k.replace(b' ', b'_').upper(): v
                                 for k, v in LDLS_DICT.items()})
@@ -290,28 +291,28 @@
     msmt_start = msmt_start.replace(microsecond=0)
     msmt_stop = msmt_start + timedelta(seconds=int(duration))
     if args.verbose:
         print('Corrected time-coverage:',
               msmt_start.timestamp(), msmt_stop.timestamp())
 
     # open EGSE database
-    with nc4.Dataset(args.egse_dir / DB_EGSE, 'r') as fid:
+    with Dataset(args.egse_dir / DB_EGSE, 'r') as fid:
         egse_time = fid['time'][:].data
         if args.verbose:
             print('EGSE time-coverage:', egse_time.min(), egse_time.max())
         mask = ((egse_time >= msmt_start.timestamp())
                 & (egse_time <= msmt_stop.timestamp()))
         if mask.sum() == 0:
             raise RuntimeError('no EGSE data found')
 
         egse_time = egse_time[mask]
         egse_data = fid['egse'][mask]
 
     # update Level-1A product with EGSE information
-    with nc4.Dataset(args.l1a_file, 'r+') as fid:
+    with Dataset(args.l1a_file, 'r+') as fid:
         if fid.groups.get('/gse_data'):
             gid = fid['/gse_data']
         else:
             gid = init_gse_data(fid)
         _ = gid.createEnumType('u1', 'ldls_t',
                                {k.replace(b' ', b'_').upper(): v
                                 for k, v in LDLS_DICT.items()})
```

### Comparing `pyspex-1.3.9/src/pyspex/lib/attrs_def.py` & `pyspex-1.4.0rc1/src/pyspex/lib/attrs_def.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,30 +6,32 @@
 # Copyright (c) 2019-2023 SRON - Netherlands Institute for Space Research
 #    All Rights Reserved
 #
 # License:  BSD-3-Clause
 """
 Provides the common global-attributes for SPEXone Level-1 products.
 """
+from __future__ import annotations
 __all__ = ['attrs_def']
 
 from datetime import datetime, timezone
 
 from ..version import pyspex_version
 
 
 # - main functions --------------------------------
-def attrs_def(level: str, inflight=True, origin=None) -> dict:
+def attrs_def(level: str, inflight: bool = True,
+              origin: str | None = None) -> dict:
     """
     Defines all global attributes for SPEXone Level-1 products.
 
     Parameters
     ----------
     level : str
-       Product processing level 'L1A', 'L1B' or 'L1C'
+       Product processing level 'L1A'
     inflight : bool
        Flag for in-flight or on-ground products
     origin : str
        Product origin: 'SRON' or 'NASA'
 
     Returns
     -------
@@ -37,47 +39,46 @@
        Global attributes for a Level-1A product
     """
     if origin is None:
         origin = 'NASA' if inflight else 'SRON'
 
     res = {
         "title": f"PACE SPEX Level-{level[1:]} data",
+        "project": "PACE Project",
+        "platform": "PACE",
         "instrument": "SPEX",
+        "product_name": None,
         "processing_version": "V1.0",
-        "conventions": "CF-1.6",
+        "processing_level": level,
         "institution": ("NASA Goddard Space Flight Center,"
                         " Ocean Biology Processing Group"),
         "license": ("http://science.nasa.gov/earth-science/"
                     "earth-science-data/data-information-policy/"),
+        "conventions": "CF-1.8 ACDD-1.3",
         "naming_authority": "gov.nasa.gsfc.sci.oceancolor",
         "keyword_vocabulary": ("NASA Global Change Master Directory (GCMD)"
                                " Science Keywords"),
-        "stdname_vocabulary": ("NetCDF Climate and Forecast (CF)"
-                               " Metadata Convention"),
-        "creator_name": "NASA/GSFC",
+        "standard_name_vocabulary": "CF Standard Name Table v79",
+        "creator_name": "NASA/GSFC/OBPG",
         "creator_email": "data@oceancolor.gsfc.nasa.gov",
         "creator_url": "http://oceancolor.gsfc.nasa.gov",
-        "project": "PACE Project",
-        "publisher_name": "NASA/GSFC",
+        "publisher_name": "NASA/GSFC/OB.DAAC",
         "publisher_email": "data@oceancolor.gsfc.nasa.gov",
         "publisher_url": "http://oceancolor.gsfc.nasa.gov",
-        "processing_level": level,
         "CDM_data_type": "swath" if inflight else "on-ground calibration",
-        "orbit_number": -1,
-        "history": None,
-        "CDL_version_date": "2020-02-20",
-        "product_name": None,
         "start_direction": "Ascending" if inflight else None,
         "end_direction": "Ascending" if inflight else None,
         "time_coverage_start": "yyyy-mm-ddTHH:MM:DD",
         "time_coverage_end": "yyyy-mm-ddTHH:MM:DD",
-        "date_created": datetime.now(timezone.utc).isoformat(
-            timespec='milliseconds'),
+        "orbit_number": -1,
         "software_name": 'https://github.com/rmvanhees/pyspex',
         "software_version": pyspex_version(),
+        "history": None,
+        "date_created": datetime.now(timezone.utc).isoformat(
+            timespec='milliseconds'),
         "sun_earth_distance": None,
         "terrain_data_source": None,
         "spectral_response_function": None,
         "systematic_uncertainty_model": None,
         "nadir_bin": None,
         "bin_size_at_nadir": None
     }
```

### Comparing `pyspex-1.3.9/src/pyspex/lib/l1a_def.py` & `pyspex-1.4.0rc1/src/pyspex/lib/l1a_def.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,45 +10,46 @@
 """
 Defines the format of a SPEXone Level-1A product.
 """
 __all__ = ['init_l1a']
 
 import datetime
 
-import netCDF4 as nc4
+# pylint: disable=no-name-in-module
+from netCDF4 import Dataset, Variable
 import numpy as np
 
 from .tmtc_def import tmtc_dtype
 
 # - global parameters ------------------------------
 ORBIT_DURATION = 5904  # seconds
 
 
 # - local functions --------------------------------
-def attrs_sec_per_day(dset, ref_date: datetime.date) -> None:
+def attrs_sec_per_day(dset: Variable, ref_date: datetime.date) -> None:
     """
     Add CF attributes to a dataset holding 'seconds of day'
 
     Parameters
     ----------
-    dset : nc4.Variable
-       Variable containing a timestamp as seconds since referencce date
+    dset : Variable
+       Variable containing a timestamp as seconds since reference date
     ref_date : datetime.date
        Reference date
 
     Examples
     --------
-    Update the attributes of variable 'time':
+    Update the attributes of variable 'time'::
 
-    >>> ref_date = datetime.date(2022, 3, 21)
-    >>> dset = sgrp.createVariable('image_time', 'f8', ('number_of_images',),
-    >>>                            fill_value=-32767)
-    >>> dset.long_name = "image time"
-    >>> dset.description = "Integration start time in seconds of day."
-    >>> attrs_sec_per_day(dset, ref_date)
+    >> ref_date = datetime.date(2022, 3, 21)
+    >> dset = sgrp.createVariable('image_time', 'f8', ('number_of_images',),
+    >>                            fill_value=-32767)
+    >> dset.long_name = "image time"
+    >> dset.description = "Integration start time in seconds of day."
+    >> attrs_sec_per_day(dset, ref_date)
 
     In CDL the variable `time` will be defined as::
 
        double time(number_of_scans) ;
           time:_FillValue = -32767. ;
           time:long_name = "time" ;
           time:units = "seconds since 2022-03-21 00:00:00" ;
@@ -66,65 +67,17 @@
     dset.year = f"{ref_date.year}"
     dset.month = f"{ref_date.month}"
     dset.day = f"{ref_date.day}"
     dset.valid_min = 0
     dset.valid_max = 86400 + ORBIT_DURATION
 
 
-# - main function ----------------------------------
-# pylint: disable=too-many-statements
-def init_l1a(l1a_flname: str, ref_date: datetime.date, dims: dict,
-             compression=False) -> nc4.Dataset:
-    """
-    Create an empty SPEXone Level-1A product (on-ground or in-flight)
-
-    Parameters
-    ----------
-    l1a_flname : str
-       Name of L1A product
-    ref_date :  datetime.date
-       Date of the first detector image
-    dims :  dict
-       Provide length of the Level-1A dimensions. Default values::
-
-          number_of_images : None     # number of image frames
-          samples_per_image : None    # depends on binning table
-          hk_packets : None           # number of HK tlm-packets (1 Hz)
-
-    compression : bool, default=False
-       Use compression on dataset /science_data/detector_images.
-
-    Notes
-    -----
-    The optional groups '/gse_data' and '/navigation_data' are not created
-    by this script.
-
-    Original CDL definition is from F. S. Patt (GSFC), 08-Feb-2019
+def image_attributes(rootgrp: Dataset, ref_date: datetime.date):
+    """Define group /image_attributes and its datasets.
     """
-    # check function parameters
-    if not isinstance(dims, dict):
-        raise TypeError("dims should be a dictionary")
-
-    # initialize dimensions
-    number_img = dims.get('number_of_images', None)
-    img_samples = dims.get('samples_per_image', None)
-    hk_packets = dims.get('hk_packets', None)
-
-    # create/overwrite netCDF4 product
-    try:
-        rootgrp = nc4.Dataset(l1a_flname, 'w')
-    except Exception as exc:
-        raise Exception(f'Failed to create netCDF4 file {l1a_flname}') from exc
-
-    # - define global dimensions
-    _ = rootgrp.createDimension('number_of_images', number_img)
-    _ = rootgrp.createDimension('samples_per_image', img_samples)
-    _ = rootgrp.createDimension('hk_packets', hk_packets)
-
-    # - define group /image_attributs and its datasets
     sgrp = rootgrp.createGroup('/image_attributes')
     dset = sgrp.createVariable('icu_time_sec', 'u4', ('number_of_images',))
     dset.long_name = "ICU time stamp (seconds)"
     dset.description = "Science TM parameter ICU_TIME_SEC."
     dset.valid_min = np.uint32(1956528000)  # year 2020
     dset.valid_max = np.uint32(2493072000)  # year 2037
     dset.units = "seconds since 1958-01-01 00:00:00 TAI"
@@ -157,20 +110,39 @@
     dset.valid_min = np.int32(1)
     dset.units = "1"
     dset = sgrp.createVariable('exposure_time', 'f8', ('number_of_images',),
                                fill_value=0)
     dset.long_name = "exposure time"
     dset.units = "s"
 
-    # - define group /science_data and its datasets
+
+def get_chunksizes(ydim: int, compression: bool) -> tuple[int, int]:
+    """Obtain chunksizes for dataset: /science_data/science_data.
+    """
+    # I did some extensive testing.
+    # - Without compression (chunked vs contiguous):
+    #   * Writing to a contiguous dataset is faster (10-20%)
+    #   * Reading one image is about as fast for chunked and contiguous storage
+    #   * Reading a pixel image is much faster for chunked storage (2-8x)
+    # - With compression (always chunked):
+    #   * Writing takes 3x as long compared to without compression,
+    #     but saves about > 40% on disk storage
+    #   * Reading of compressed data is much slower than uncompressed data
+    #   * The performance when reading one detector image is acceptable,
+    #     however reading one pixel image is really slow (specially full-frame).
+    # Therefore, these are the best choices for the variable `chunksizes`.
+    return (20, ydim) if ydim < 1048576 \
+        else (1, min(512 * 1024, ydim)) if compression else (1, ydim)
+
+
+def science_data(rootgrp: Dataset, compression: bool,
+                 chunksizes: tuple[int, int]):
+    """Define group /science_data and its datasets.
+    """
     sgrp = rootgrp.createGroup('/science_data')
-    chunksizes = (64, img_samples) if img_samples < 1048576 \
-        else (4, img_samples)
-    if not compression and number_img is not None:
-        chunksizes = None
     dset = sgrp.createVariable('detector_images', 'u2',
                                ('number_of_images', 'samples_per_image'),
                                compression='zlib' if compression else None,
                                complevel=1, chunksizes=chunksizes,
                                fill_value=0xFFFF)
     dset.long_name = "detector pixel values"
     dset.valid_min = np.uint16(0)
@@ -178,15 +150,18 @@
     dset.units = "counts"
     hk_dtype = rootgrp.createCompoundType(tmtc_dtype(0x350), 'science_dtype')
     dset = sgrp.createVariable('detector_telemetry', hk_dtype,
                                dimensions=('number_of_images',))
     dset.long_name = "SPEX science telemetry"
     dset.comment = "A subset of MPS and housekeeping parameters."
 
-    # - define group /engineering_data and its datasets
+
+def engineering_data(rootgrp: Dataset, ref_date: datetime.date):
+    """ Define group /engineering_data and its datasets.
+    """
     sgrp = rootgrp.createGroup('/engineering_data')
     dset = sgrp.createVariable('HK_tlm_time', 'f8', ('hk_packets',),
                                fill_value=-32767)
     dset.long_name = "HK telemetry packet time"
     dset.description = "Packaging time in seconds of day."
     attrs_sec_per_day(dset, ref_date)
     hk_dtype = rootgrp.createCompoundType(tmtc_dtype(0x320), 'nomhk_dtype')
@@ -212,8 +187,64 @@
     dset.valid_max = 300
     dset.units = "K"
     # hk_dtype = rootgrp.createCompoundType(tmtc_dtype(0x322)), 'demhk_dtype')
     # dset = sgrp.createVariable('DemHK_telemetry', hk_dtype, ('hk_packets',))
     # dset.long_name = "SPEX detector-HK telemetry"
     # dset.comment = "DEM housekeeping parameters."
 
+
+# - main function ----------------------------------
+def init_l1a(l1a_flname: str, ref_date: datetime.date, dims: dict,
+             compression: bool = False) -> Dataset:
+    """
+    Create an empty SPEXone Level-1A product (on-ground or in-flight)
+
+    Parameters
+    ----------
+    l1a_flname : str
+       Name of L1A product
+    ref_date :  datetime.date
+       Date of the first detector image
+    dims :  dict
+       Provide length of the Level-1A dimensions. Default values::
+
+          number_of_images : None     # number of image frames
+          samples_per_image : None    # depends on binning table
+          hk_packets : None           # number of HK tlm-packets (1 Hz)
+
+    compression : bool, default=False
+       Use compression on dataset /science_data/detector_images.
+
+    Notes
+    -----
+    The optional groups '/gse_data' and '/navigation_data' are not created
+    by this script.
+
+    Original CDL definition is from F. S. Patt (GSFC), 08-Feb-2019
+    """
+    # check function parameters
+    if not isinstance(dims, dict):
+        raise TypeError("dims should be a dictionary")
+
+    # initialize dimensions
+    number_img = dims.get('number_of_images', None)
+    img_samples = dims.get('samples_per_image', None)
+    hk_packets = dims.get('hk_packets', None)
+
+    # create/overwrite netCDF4 product
+    try:
+        rootgrp = Dataset(l1a_flname, 'w')
+    except Exception as exc:
+        raise Exception(f'Failed to create netCDF4 file {l1a_flname}') from exc
+
+    # - define global dimensions
+    _ = rootgrp.createDimension('number_of_images', number_img)
+    _ = rootgrp.createDimension('samples_per_image', img_samples)
+    _ = rootgrp.createDimension('hk_packets', hk_packets)
+
+    # - define the various HDF54/netCDF4 groups and their datasets
+    image_attributes(rootgrp, ref_date)
+    chunksizes = get_chunksizes(img_samples, compression)
+    science_data(rootgrp, compression, chunksizes)
+    engineering_data(rootgrp, ref_date)
+
     return rootgrp
```

### Comparing `pyspex-1.3.9/src/pyspex/lib/leap_sec.py` & `pyspex-1.4.0rc1/src/pyspex/lib/leap_sec.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 """
 Python script to determine the number of leap seconds for given timestamp.
 
 The source for the latest version of tai-utc.dat is the US Naval Observatory:
 
    https://maia.usno.navy.mil/ser7/tai-utc.dat
 """
+__all__ = ['get_leap_seconds']
+
 from datetime import datetime, timezone
 
 try:
     from importlib.resources import files
 except ImportError:
     from importlib_resources import files
 
@@ -39,15 +41,15 @@
         taiutc = files('pyspex.data').joinpath('tai-utc.dat')
     else:
         taiutc = Path(ocvarroot) / 'common' / 'tai-utc.dat'
 
     epochsecs = (datetime(epochyear, 1, 1, tzinfo=timezone.utc)
                  - datetime(1970, 1, 1, tzinfo=timezone.utc)).total_seconds()
     taidt = datetime.utcfromtimestamp(taitime + epochsecs)
-    leapsec = 0
+    leapsec: float = 0
     with taiutc.open("r", encoding='ascii') as fp:
         for line in fp:
             rec = line.rstrip().split(None, 7)
             if julian.from_jd(float(rec[4])) < taidt:
                 leapsec = float(rec[6])
 
     return leapsec
```

### Comparing `pyspex-1.3.9/src/pyspex/lib/tmtc_def.py` & `pyspex-1.4.0rc1/src/pyspex/lib/tmtc_def.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 * SPX1-TN-005 Telemetry and Telecommand Handbook, issue 14, date 15-Mar-2021
 """
 __all__ = ['tmtc_dtype']
 
 import numpy as np
 
 
-def __tmtc_def(apid) -> list:
+def __tmtc_def(apid: int) -> list:
     """Returns SPEXone telemetry packet structure as a list of tuples.
 
     Parameters
     ----------
     apid : int
        SPEXone telemetry APID.
        Implemented APIDs: 0x350 (Science), 0x320 (NomHK) and 0x322 (DemHK).
@@ -47,22 +47,22 @@
             ('ICU_5V_T', '>i2'),                # 28    0x0028
             ('ICU_4V_T', '>i2'),                # 30    0x002a
             ('ICU_HG1_T', '>i2'),               # 32    0x002c
             ('ICU_HG2_T', '>i2'),               # 34    0x002e
             ('ICU_MID_T', '>i2'),               # 36    0x0030
             ('ICU_MCU_T', '>i2'),               # 38    0x0032
             ('ICU_DIGV_T', '>i2'),              # 40    0x0034
-            ('ICU_4p0V_V', '>u2'),              # 42    0x0036
-            ('ICU_3p3V_V', '>u2'),              # 44    0x0038
-            ('ICU_1p2V_V', '>u2'),              # 46    0x003a
-            ('ICU_4p0V_I', '>u2'),              # 48    0x003c
-            ('ICU_3p3V_I', '>u2'),              # 50    0x003e
-            ('ICU_1p2V_I', '>u2'),              # 52    0x0040
-            ('ICU_5p0V_V', '>u2'),              # 54    0x0042
-            ('ICU_5p0V_I', '>u2'),              # 56    0x0044
+            ('ICU_4P0V_V', '>u2'),              # 42    0x0036
+            ('ICU_3P3V_V', '>u2'),              # 44    0x0038
+            ('ICU_1P2V_V', '>u2'),              # 46    0x003a
+            ('ICU_4P0V_I', '>u2'),              # 48    0x003c
+            ('ICU_3P3V_I', '>u2'),              # 50    0x003e
+            ('ICU_1P2V_I', '>u2'),              # 52    0x0040
+            ('ICU_5P0V_V', '>u2'),              # 54    0x0042
+            ('ICU_5P0V_I', '>u2'),              # 56    0x0044
             ('DEM_V', '>u2'),                   # 58    0x0046
             ('DEM_I', '>u2'),                   # 60    0x0048
             ('LED1_ANODE_V', '>u4'),            # 62    0x004a
             ('LED1_CATH_V', '>u4'),             # 66    0x004e
             ('LED1_I', '>u4'),                  # 70    0x0052
             ('LED2_ANODE_V', '>u4'),            # 74    0x0056
             ('LED2_CATH_V', '>u4'),             # 78    0x005a
@@ -455,15 +455,15 @@
             ('DET_REG124', 'u1'),               # 186   0x00c6
             ('DET_REG125', 'u1')                # 187   0x00c7
         ]                                       # 188
 
     raise ValueError('Telemetry APID not implemented')
 
 
-def tmtc_dtype(apid):
+def tmtc_dtype(apid: int) -> np.dtype:
     """Obtain SPEXone telemetry packet definition.
 
     Parameters
     ----------
     apid : int
        SPEXone telemetry APID.
        Implemented APIDs: 0x350 (Science), 0x320 (NomHK) and 0x322 (DemHK).
@@ -471,12 +471,13 @@
     Returns
     -------
     numpy.dtype
        Definition of Spexone telemetry packet.
 
     Examples
     --------
+    Usage of `tmtc_dtype`::
 
-    >>> from pyspex.lib.tmtc_def import tmtc_dtype
-    >>> mps_dtype = tmtc_dtype(0x350)
+    >> from pyspex.lib.tmtc_def import tmtc_dtype
+    >> mps_dtype = tmtc_dtype(0x350)
     """
     return np.dtype(__tmtc_def(apid))
```

### Comparing `pyspex-1.3.9/src/pyspex/lv0_io.py` & `pyspex-1.4.0rc1/src/pyspex/lv0_io.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,58 +6,156 @@
 # Copyright (c) 2019-2023 SRON - Netherlands Institute for Space Research
 #    All Rights Reserved
 #
 # License:  BSD-3-Clause
 """
 Contains a collection of routines to read and write SPEXone CCSDS data:
 
-   `dtype_packet_hdr`, `dtype_tmtc`, `dump_lv0_data`,
-   `read_lv0_data`, 'select_nomhk', `select_science`
+   `dtype_tmtc`, `read_lv0_data`, `dump_numhk`, `dump_science`
 
 And handy routines to convert CCSDS parameters:
 
-   `ap_id`, `coverage_time`, `fix_sub_sec`, `grouping_flag`,
-   `hk_sec_of_day`, `img_sec_of_day`, `nomhk_timestamps`,
-   `packet_length`, `science_timestamps`, `sequence`
+   `ap_id`, `grouping_flag`, `packet_length`, `sequence`,
+   `hk_sec_of_day`, `img_sec_of_day`
 """
 from __future__ import annotations
 
-__all__ = ['ap_id', 'coverage_time', 'fix_sub_sec', 'grouping_flag',
-           'hk_sec_of_day', 'img_sec_of_day', 'nomhk_timestamps',
-           'packet_length', 'science_timestamps', 'sequence',
-           'dtype_packet_hdr', 'dtype_tmtc', 'dump_lv0_data',
-           'read_lv0_data', 'select_nomhk', 'select_science', 'DTYPE_CFE']
+__all__ = ['ap_id', 'dtype_tmtc', 'dump_numhk', 'dump_science',
+           'grouping_flag', 'hk_sec_of_day', 'img_sec_of_day',
+           'packet_length', 'read_lv0_data', 'sequence']
 
 from datetime import datetime, timedelta, timezone
 from pathlib import Path
 from typing import Any
 
 import numpy as np
 
 from .lib.leap_sec import get_leap_seconds
 from .lib.tmtc_def import tmtc_dtype
-from .tm_science import TMscience
 
 # - global parameters ------------------------------
 FULLFRAME_BYTES = 2 * 2048 * 2048
 
-# define numpy data-type to read the cFE file-header
-DTYPE_CFE = np.dtype([
-    ('ContentType', 'S4'),
-    ('SubType', 'S4'),
-    ('FileHeaderLength', '>u4'),
-    ('SpacecraftID', 'S4'),
-    ('ProcessorID', '>u4'),
-    ('InstrumentID', 'S4'),
-    ('TimeSec', '>u4'),
-    ('TimeSubSec', '>u4'),
-    ('Filename', 'S32')])
-
 
 # - local functions --------------------------------
+def _cfe_header_(flname: Path, verbose: bool = False) -> np.ndarray:
+    """Read cFE file header (only for file_format='dsb').
+    """
+    # define numpy data-type to read the cFE file-header
+    dtype_cfe = np.dtype([
+        ('ContentType', 'S4'),
+        ('SubType', 'S4'),
+        ('FileHeaderLength', '>u4'),
+        ('SpacecraftID', 'S4'),
+        ('ProcessorID', '>u4'),
+        ('InstrumentID', 'S4'),
+        ('TimeSec', '>u4'),
+        ('TimeSubSec', '>u4'),
+        ('Filename', 'S32')])
+
+    cfe_hdr = np.fromfile(flname, count=1, dtype=dtype_cfe)[0]
+    if verbose:
+        print(f'[INFO]: content of cFE header "{cfe_hdr}"')
+    return cfe_hdr
+
+
+def _dtype_packet_(file_format: str) -> np.dtype | None:
+    """
+    Return definition of the CCSDS packet headers (primary and secondary)
+
+    Parameters
+    ----------
+    file_format : {'raw', 'dsb' or 'st3'}
+        File format of level 0 products
+
+    Returns
+    -------
+    np.dtype
+        numpy dtype of the packet headers or None if file format is unknown
+
+    Notes
+    -----
+
+    'raw': data has no file header and standard CCSDS packet headers
+
+    'st3': data has no file header and ITOS + spacewire + CCSDS packet headers
+
+    'dsb': data has a cFE file-header and spacewire + CCSDS packet headers
+
+    """
+    if file_format == 'raw':
+        return np.dtype([('type', '>u2'),
+                         ('sequence', '>u2'),
+                         ('length', '>u2'),
+                         ('tai_sec', '>u4'),
+                         ('sub_sec', '>u2')])
+
+    if file_format == 'dsb':
+        return np.dtype([('spacewire', 'u1', (2,)),
+                         ('type', '>u2'),
+                         ('sequence', '>u2'),
+                         ('length', '>u2'),
+                         ('tai_sec', '>u4'),
+                         ('sub_sec', '>u2')])
+
+    if file_format == 'st3':
+        return np.dtype([('itos_hdr', '>u2', (8,)),
+                         ('spacewire', 'u1', (2,)),
+                         ('type', '>u2'),
+                         ('sequence', '>u2'),
+                         ('length', '>u2'),
+                         ('tai_sec', '>u4'),
+                         ('sub_sec', '>u2')])
+
+    return None
+
+
+def _fix_hk24_(sci_hk: np.ndarray):
+    """
+    Correct 32-bit integers in the Science HK which originate from
+    24-bit integers in the detector register values
+
+    In addition:
+
+    - copy the first 4 bytes of 'DET_CHENA' to 'DET_ILVDS'
+    - parameter 'REG_BINNING_TABLE_START' was writen in little-endian
+
+    """
+    res = sci_hk.copy()
+    if sci_hk['ICUSWVER'] < 0x129:
+        res['REG_BINNING_TABLE_START'] = \
+            sci_hk['REG_BINNING_TABLE_START'].byteswap()
+
+    res['DET_ILVDS'] = sci_hk['DET_CHENA'] & 0xf
+    for key in ['TS1_DEM_N_T', 'TS2_HOUSING_N_T', 'TS3_RADIATOR_N_T',
+                'TS4_DEM_R_T', 'TS5_HOUSING_R_T', 'TS6_RADIATOR_R_T',
+                'LED1_ANODE_V', 'LED1_CATH_V', 'LED1_I',
+                'LED2_ANODE_V', 'LED2_CATH_V', 'LED2_I',
+                'ADC1_VCC', 'ADC1_REF', 'ADC1_T',
+                'ADC2_VCC', 'ADC2_REF', 'ADC2_T',
+                'DET_EXPTIME', 'DET_EXPSTEP', 'DET_KP1',
+                'DET_KP2', 'DET_EXPTIME2', 'DET_EXPSTEP2',
+                'DET_CHENA']:
+        res[key] = sci_hk[key] >> 8
+
+    return res
+
+
+def _get_epoch_(timestamp: int) -> datetime:
+    """
+    Determine year of epoch, 1970 (UTC) or 1958 (TAI).
+    """
+    if timestamp < 1956528000:
+        return datetime(1970, 1, 1, tzinfo=timezone.utc)
+
+    return (datetime(1958, 1, 1, tzinfo=timezone.utc)
+            - timedelta(seconds=get_leap_seconds(timestamp)))
+
+
+# - helper functions to read Level-0 data ----------
 def ap_id(hdr: np.ndarray) -> int:
     """
     Returns Telemetry APID, the range 0x320 to 0x351 is available to SPEXone
 
     Parameters
     ----------
     hdr :  np.ndarray
@@ -147,65 +245,14 @@
     -----
     We always read the primary header and secondary header at once.
     Value range: 7 - 16375
     """
     return hdr['length']
 
 
-def dtype_packet_hdr(file_format: str) -> np.dtype | None:
-    """
-    Return definition of the CCSDS packet headers (primary and secondary)
-
-    Parameters
-    ----------
-    file_format : {'raw', 'dsb' or 'st3'}
-        File format of level 0 products
-
-    Returns
-    -------
-    np.dtype
-        numpy dtype of the packet headers or None if file format is unknown
-
-    Notes
-    -----
-
-    'raw': data has no file header and standard CCSDS packet headers
-
-    'st3': data has no file header and ITOS + spacewire + CCSDS packet headers
-
-    'dsb': data has a cFE file-header and spacewire + CCSDS packet headers
-
-    """
-    if file_format == 'raw':
-        return np.dtype([('type', '>u2'),
-                         ('sequence', '>u2'),
-                         ('length', '>u2'),
-                         ('tai_sec', '>u4'),
-                         ('sub_sec', '>u2')])
-
-    if file_format == 'dsb':
-        return np.dtype([('spacewire', 'u1', (2,)),
-                         ('type', '>u2'),
-                         ('sequence', '>u2'),
-                         ('length', '>u2'),
-                         ('tai_sec', '>u4'),
-                         ('sub_sec', '>u2')])
-
-    if file_format == 'st3':
-        return np.dtype([('itos_hdr', '>u2', (8,)),
-                         ('spacewire', 'u1', (2,)),
-                         ('type', '>u2'),
-                         ('sequence', '>u2'),
-                         ('length', '>u2'),
-                         ('tai_sec', '>u4'),
-                         ('sub_sec', '>u2')])
-
-    return None
-
-
 def dtype_tmtc(hdr: np.ndarray) -> np.dtype:
     """
     Return definition of a CCSDS TmTc package (given APID)
 
     Parameters
     ----------
     hdr :  np.ndarray
@@ -236,49 +283,19 @@
                              ('TcPacketId', '>u2'),
                              ('TcSeqControl', '>u2'),
                              ('TcErrorCode', '>u2'),
                              ('FailParameter1', '>u2'),
                              ('FailParameter2', '>u2')])}.get(ap_id(hdr), None)
 
 
-def _fix_hk24_(sci_hk):
-    """
-    Correct 32-bit integers in the Science HK which originate from
-    24-bit integers in the detector register values
-
-    In addition:
-
-    - copy the first 4 bytes of 'DET_CHENA' to 'DET_ILVDS'
-    - parameter 'REG_BINNING_TABLE_START' was writen in little-endian
-
-    """
-    res = sci_hk.copy()
-    if sci_hk['ICUSWVER'] < 0x129:
-        res['REG_BINNING_TABLE_START'] = \
-            sci_hk['REG_BINNING_TABLE_START'].byteswap()
-
-    res['DET_ILVDS'] = sci_hk['DET_CHENA'] & 0xf
-    for key in ['TS1_DEM_N_T', 'TS2_HOUSING_N_T', 'TS3_RADIATOR_N_T',
-                'TS4_DEM_R_T', 'TS5_HOUSING_R_T', 'TS6_RADIATOR_R_T',
-                'LED1_ANODE_V', 'LED1_CATH_V', 'LED1_I',
-                'LED2_ANODE_V', 'LED2_CATH_V', 'LED2_I',
-                'ADC1_VCC', 'ADC1_REF', 'ADC1_T',
-                'ADC2_VCC', 'ADC2_REF', 'ADC2_T',
-                'DET_EXPTIME', 'DET_EXPSTEP', 'DET_KP1',
-                'DET_KP2', 'DET_EXPTIME2', 'DET_EXPSTEP2',
-                'DET_CHENA']:
-        res[key] = sci_hk[key] >> 8
-
-    return res
-
-
-def read_lv0_data(file_list: list, file_format: str, debug=False,
-                  verbose=False) -> tuple[tuple, tuple]:
-    """
-    Read level 0 data and return Science and telemetry data
+def read_lv0_data(file_list: list[Path, ...],
+                  file_format: str, *,
+                  debug: bool = False,
+                  verbose: bool = False) -> tuple[tuple, tuple]:
+    """Read level 0 data and return Science and telemetry data.
 
     Parameters
     ----------
     file_list : list of Path
        list of CCSDS files
     file_format : {'raw', 'st3', 'dsb'}
        type of CCSDS data
@@ -289,58 +306,54 @@
 
     Returns
     -------
     tuple
          Contains all Science and TmTc CCSDS packages as numpy arrays,
          or None if called with debug is True
     """
-    hdr_dtype = dtype_packet_hdr(file_format)
+    hdr_dtype = _dtype_packet_(file_format)
     scihk_dtype = tmtc_dtype(0x350)
     icutm_dtype = np.dtype([('tai_sec', '>u4'),
                             ('sub_sec', '>u2')])
 
     # read level 0 headers and CCSDS data of Science and TmTc data
     ccsds_sci = ()
     ccsds_hk = ()
     for flname in file_list:
+        offs = 0
+        if file_format == 'dsb':
+            cfe_hdr = _cfe_header_(flname, verbose)
+            offs += cfe_hdr['FileHeaderLength']
+
         buff_sci = ()          # Use chunking to speed-up memory allocation
         buff_hk = ()
         with open(flname, 'rb') as fp:
             if verbose:
                 print(f'[INFO]: processing file "{flname}"')
-            ccsds_data = fp.read()
-
-            offs = 0
-            if file_format == 'dsb':
-                # read cFE file-header from buffer
-                cfe_hdr = np.frombuffer(ccsds_data, count=1, offset=0,
-                                        dtype=DTYPE_CFE)[0]
-                if verbose:
-                    print(f'[INFO]: content of cFE header "{cfe_hdr}"')
-                if cfe_hdr['FileHeaderLength'] != DTYPE_CFE.itemsize:
-                    print('[WARNING]: size of cFE header is'
-                          f' {cfe_hdr["FileHeaderLength"]} bytes, expected'
-                          f' {DTYPE_CFE.itemsize} bytes')
-                offs += cfe_hdr['FileHeaderLength']
 
             # read CCSDS header and user data
+            ccsds_data = fp.read()
             while offs < len(ccsds_data):
                 try:
                     hdr = np.frombuffer(ccsds_data, count=1, offset=offs,
                                         dtype=hdr_dtype)[0]
                 except ValueError as exc:
                     print(f'[WARNING]: header reading error with "{exc}"')
                     break
 
-                # copy the full CCSDS package
                 if debug:
                     print(ap_id(hdr), grouping_flag(hdr),
                           hdr_dtype.itemsize, hdr['length'], offs)
+                    if hdr['length'] == 0 or not 0x320 <= ap_id(hdr) < 0x351:
+                        raise ValueError('corrupted CCSDS header detected')
                     offs += hdr_dtype.itemsize + hdr['length'] - 5
-                elif ap_id(hdr) == 0x350:                   # Science APID
+                    continue
+
+                # copy the full CCSDS package
+                if ap_id(hdr) == 0x350:                   # Science APID
                     nbytes = hdr['length'] - 5
                     if grouping_flag(hdr) == 1:
                         buff = np.empty(1, dtype=np.dtype([
                             ('hdr', hdr_dtype),
                             ('hk', scihk_dtype),
                             ('icu_tm', icutm_dtype),
                             ('frame', 'O')]))
@@ -362,363 +375,150 @@
                             ('frame', 'O')]))
                         buff['hdr'] = hdr
                         offs += hdr_dtype.itemsize
 
                     buff['frame'][0] = np.frombuffer(ccsds_data,
                                                      count=nbytes // 2,
                                                      offset=offs, dtype='>u2')
-                    buff_sci += ({'hdr': hdr, 'data': buff.copy()},)
+                    buff_sci += (buff.copy(),)
                     offs += nbytes
                 elif 0x320 <= ap_id(hdr) < 0x335:           # other valid APIDs
                     buff = np.frombuffer(ccsds_data, count=1, offset=offs,
-                                         dtype=dtype_tmtc(hdr))[0]
-                    buff_hk += ({'hdr': hdr, 'data': buff},)
+                                         dtype=dtype_tmtc(hdr))
+                    buff_hk += (buff,)
                     offs += dtype_tmtc(hdr).itemsize
                 else:
+                    if hdr['length'] == 0:
+                        raise ValueError('corrupted CCSDS header detected')
                     offs += hdr_dtype.itemsize + hdr['length'] - 5
         ccsds_sci += buff_sci
         ccsds_hk += buff_hk
         del ccsds_data
 
     if verbose:
         print(f'[INFO]: number of Science packages {len(ccsds_sci)}')
         print(f'[INFO]: number of Engineering packages {len(ccsds_hk)}')
 
     return ccsds_sci, ccsds_hk
 
 
-def dump_lv0_data(file_list: list, datapath: Path, ccsds_sci: tuple,
-                  ccsds_hk: tuple) -> None:
-    """
-    Perform an ASCII dump of level 0 data
-
-    Parameters
-    ----------
-    file_list :  list of Path
-       list of CCSDS files as concrete paths
-    datapath :  Path
-       concrete path to the directory to write the dump-file
-    ccsds_sci :  tuple of np.ndarray
-       tuple of Science packages
-    ccsds_hk :  tuple of np.ndarray
-       tuple of nomHK packages
-    """
-    # dump header information of the Science packages
-    flname = datapath / (file_list[0].stem + '.dump')
-    with flname.open('w', encoding='ascii') as fp:
-        fp.write('APID Grouping Counter Length'
-                 ' ICUSWVER MPS_ID  IMRLEN     ICU_SEC ICU_SUBSEC\n')
-        for segment in ccsds_sci:
-            hdr = segment['hdr']
-            data = segment['data'][0]
-            if grouping_flag(hdr) == 1:
-                fp.write(f"{ap_id(hdr):4x} {grouping_flag(hdr):8d}"
-                         f" {sequence(hdr):7d} {packet_length(hdr):6d}"
-                         f" {data['hk']['ICUSWVER']:8x}"
-                         f" {data['hk']['MPS_ID']:6d}"
-                         f" {data['hk']['IMRLEN']:7d}"
-                         f" {data['icu_tm']['tai_sec']:11d}"
-                         f" {data['icu_tm']['sub_sec']:10d}\n")
-            else:
-                fp.write(f'{ap_id(hdr):4x} {grouping_flag(hdr):8d}'
-                         f' {sequence(hdr):7d} {packet_length(hdr):6d}\n')
-
-    # dump header information of the nominal house-keeping packages
-    flname = datapath / (file_list[0].stem + '_hk.dump')
-    with flname.open('w', encoding='ascii') as fp:
-        fp.write('APID Grouping Counter Length     TAI_SEC    SUB_SEC'
-                 ' ICUSWVER MPS_ID TcSeqControl TcErrorCode\n')
-        for segment in ccsds_hk:
-            hdr = segment['hdr']
-            data = segment['data']
-            msg = (f"{ap_id(hdr):4x} {grouping_flag(hdr):8d}"
-                   f" {sequence(hdr):7d} {packet_length(hdr):6d}"
-                   f" {hdr['tai_sec']:11d} {hdr['sub_sec']:10d}")
-
-            if ap_id(hdr) == 0x320:
-                msg += (f" {data['hk']['ICUSWVER']:8x}"
-                        f" {data['hk']['MPS_ID']:6d}")
-            elif ap_id(hdr) in (0x331, 0x332, 0x333, 0x334):
-                msg += f" {-1:8x} {-1:6d} {data['TcSeqControl']:12d}"
-                if ap_id(hdr) == 0x332:
-                    msg += (f" {bin(data['TcErrorCode'])}"
-                            f" {data['RejectParameter1']}"
-                            f" {data['RejectParameter2']}")
-                if ap_id(hdr) == 0x334:
-                    msg += (f" {bin(data['TcErrorCode'])}"
-                            f" {data['FailParameter1']}"
-                            f" {data['FailParameter2']}")
-            fp.write(msg + "\n")
-
-
-def fix_sub_sec(tai_sec, sub_sec) -> tuple:
-    """
-    In ICU S/W version 0x123 a bug was introduced which corrupted the
-    read of the sub-sec parameter. Therefore, all ambient measurements
-    performed between 2020-12-02T09:34 and 2021-01-04T16:23 have to be
-    adjusted.
-    """
-    us100 = np.round(10000 * sub_sec.astype(float) / 65536)
-    buff = us100 + tai_sec - 10000
-    us100 = buff.astype('u8') % 10000
-    sub_sec = ((us100 << 16) // 10000).astype('u2')
-
-    return tai_sec, sub_sec
-
-
-def science_timestamps(science: np.ndarray) -> tuple[np.ndarray, np.ndarray]:
-    """
-    Return timestamps of the Science packets
-
-    Parameters
-    ----------
-    science :  np.ndarray
-
-    Returns
-    -------
-    tuple of ndarray
-        Tuple with timestamps and sub-seconds
-    """
-    # The parameters ICU_TIME_SEC and ICU_TIME_SUBSEC contain zeros until
-    # ICU S/W version 0x125, which was first used at 2021-01-04T16:23.
-    # Note version 0x124 was not used for any OCAL measurement.
-    if science['hk']['ICUSWVER'][0] > 0x123:
-        img_sec = science['icu_tm']['tai_sec']
-        img_subsec = science['icu_tm']['sub_sec']
-        return img_sec, img_subsec
-
-    # Use the inaccurate packaging timing stored in the secondary header
-    img_sec = science['hdr']['tai_sec']
-    img_subsec = science['hdr']['sub_sec']
-    if science['hk']['ICUSWVER'][0] == 0x123:
-        # fix bug parameter sub-sec
-        return fix_sub_sec(img_sec, img_subsec)
-
-    return img_sec, img_subsec
-
-
-def nomhk_timestamps(nomhk: np.ndarray) -> tuple[np.ndarray, np.ndarray]:
-    """
-    Return timestamps of the telemetry packets
-
-    Parameters
-    ----------
-    nomhk:  np.ndarray
-
-    Returns
-    -------
-    tuple of ndarray
-        Tuple with timestamps and sub-seconds
-    """
-    nomhk_sec = nomhk['hdr']['tai_sec']
-    nomhk_subsec = nomhk['hdr']['sub_sec']
-    if nomhk['hk']['ICUSWVER'][0] == 0x123:
-        # fix bug parameter sub-sec
-        return fix_sub_sec(nomhk_sec, nomhk_subsec)
-
-    return nomhk_sec, nomhk_subsec
-
-
-def which_epoch(timestamp: int) -> datetime:
-    """
-    Determine year of epoch, 1970 (UTC) or 1958 (TAI).
-    """
-    if timestamp < 1956528000:
-        return datetime(1970, 1, 1, tzinfo=timezone.utc)
-
-    return (datetime(1958, 1, 1, tzinfo=timezone.utc)
-            - timedelta(seconds=get_leap_seconds(timestamp)))
-
-
-def img_sec_of_day(img_sec, img_subsec, img_hk) -> tuple[datetime, float | Any]:
+def img_sec_of_day(img_sec: np.ndarray, img_subsec: np.ndarray,
+                   img_hk: np.ndarray) -> tuple[datetime, float | Any]:
     """
     Convert Image CCSDS timestamp to seconds after midnight
 
     Parameters
     ----------
     img_sec : numpy array (dtype='u4')
         Seconds since 1970-01-01 (or 1958-01-01)
     img_subsec : numpy array (dtype='u2')
         Sub-seconds as (1 / 2**16) seconds
     img_hk :  numpy array
+        DemHK telemetry packages
 
     Returns
     -------
     tuple
         reference day: float, sec_of_day: numpy.ndarray
     """
     # determine for the first timestamp the offset with last midnight [seconds]
-    epoch = which_epoch(img_sec[0])
+    epoch = _get_epoch_(img_sec[0])
     tstamp0 = epoch + timedelta(seconds=int(img_sec[0]))
     ref_day = datetime(year=tstamp0.year,
                        month=tstamp0.month,
                        day=tstamp0.day, tzinfo=timezone.utc)
     # seconds since midnight
     offs_sec = (ref_day - epoch).total_seconds()
 
     # Determine offset wrt start-of-integration (IMRO + 1)
     # Where the default is defined as IMRO:
     #  [full-frame] COADDD + 2  (no typo, this is valid for the later MPS's)
     #  [binned] 2 * COADD + 1   (always valid)
     offs_msec = 0
     if img_hk['ICUSWVER'][0] > 0x123:
-        mps = TMscience(img_hk)
-        if np.bincount(mps.binning_table).argmax() == 0:
-            imro = mps.get('REG_NCOADDFRAMES') + 2
-        else:
-            imro = 2 * mps.get('REG_NCOADDFRAMES') + 1
-        offs_msec = mps.get('FTI') * (imro + 1) / 10
+        imro = np.empty(img_hk.size, dtype=float)
+        _mm = img_hk['IMRLEN'] == FULLFRAME_BYTES
+        imro[_mm] = img_hk['REG_NCOADDFRAMES'][_mm] + 2
+        imro[~_mm] = 2 * img_hk['REG_NCOADDFRAMES'][~_mm] + 1
+        offs_msec = img_hk['FTI'] * (imro + 1) / 10
 
     # return seconds since midnight
     return ref_day, img_sec - offs_sec + img_subsec / 65536 - offs_msec / 1000
 
 
-def hk_sec_of_day(ccsds_sec, ccsds_subsec, ref_day=None) -> np.ndarray:
+def hk_sec_of_day(ccsds_sec: np.ndarray, ccsds_subsec: np.ndarray,
+                  ref_day: datetime | None = None) -> np.ndarray:
     """
     Convert CCSDS timestamp to seconds after midnight
 
     Parameters
     ----------
     ccsds_sec : numpy array (dtype='u4')
         Seconds since 1970-01-01 (or 1958-01-01)
     ccsds_subsec : numpy array (dtype='u2')
         Sub-seconds as (1 / 2**16) seconds
-    ref_day : datetime.datetime
+    ref_day : datetime.datetime, optional
 
     Returns
     -------
     numpy.ndarray with sec_of_day
     """
     # determine for the first timestamp the offset with last midnight [seconds]
-    epoch = which_epoch(ccsds_sec[0])
+    epoch = _get_epoch_(ccsds_sec[0])
     if ref_day is None:
         tstamp0 = epoch + timedelta(seconds=int(ccsds_sec[0]))
         ref_day = datetime(year=tstamp0.year,
                            month=tstamp0.month,
                            day=tstamp0.day, tzinfo=timezone.utc)
     offs_sec = (ref_day - epoch).total_seconds()
 
     # return seconds since midnight
     return ccsds_sec - offs_sec + ccsds_subsec / 65536
 
 
-def coverage_time(science) -> tuple:
-    """
-    Return coverage time start and end of the Science data
-    """
-    img_sec, img_subsec = science_timestamps(science)
-    ref_date, img_time = img_sec_of_day(img_sec, img_subsec, science['hk'])
-    frame_period = 1e-7 * TMscience(science['hk'][-1]).frame_period
-    return (ref_date + timedelta(seconds=img_time[0]),
-            ref_date + timedelta(seconds=img_time[-1] + frame_period))
-
-
-def select_nomhk(ccsds_hk: tuple[np.ndarray],
-                 mps_list: list[int]) -> np.ndarray:
-    """
-    Select nominal housekeeping telemetry packages on MPS-IDs.
-
-    Parameters
-    ----------
-    ccsds_hk :  tuple of np.ndarray
-        All non-Science telementry packages
-    mps_list :  list of integers
-        Select telementry packages on MPS-IDs
-
-    Returns
-    -------
-    np.ndarray
-         Selected nominal housekeeping telemetry packages as numpy array
-    """
-    if not ccsds_hk:
-        return np.array(())
-
-    return np.concatenate(
-        [(x['data'],) for x in ccsds_hk if ap_id(x['hdr']) == 0x320
-         and x['data']['hk']['MPS_ID'] in mps_list])
-
-
-def select_science(ccsds_sci: tuple[np.ndarray],
-                   mode='all') -> tuple[np.ndarray, np.ndarray]:
-    """
-    Select Science telemetry packages and combine image data to contain one
-    detector readout.
+def dump_numhk(flname: str, ccsds_hk: tuple[np.ndarray]):
+    """Dump telemetry header info (NomHk)."""
+    with Path(flname).open('w', encoding='ascii') as fp:
+        fp.write('APID Grouping Counter Length     TAI_SEC    SUB_SEC'
+                 ' ICUSWVER MPS_ID TcSeqControl TcErrorCode\n')
+        for buf in ccsds_hk:
+            hdr = buf['hdr'][0]
+            msg = (f"{ap_id(hdr):4x} {grouping_flag(hdr):8d}"
+                   f" {sequence(hdr):7d} {packet_length(hdr):6d}"
+                   f" {hdr['tai_sec']:11d} {hdr['sub_sec']:10d}")
 
-    Parameters
-    ----------
-    ccsds_sci :  tuple of np.ndarray
-        Science TM packages (ApID: 0x350)
-    mode :  {'all', 'full', 'binned'}, default='all'
-        Select Science packages with full-frame image or binned images
+            if ap_id(hdr) == 0x320:
+                _hk = buf['hk'][0]
+                msg += f" {_hk['ICUSWVER']:8x} {_hk['MPS_ID']:6d}"
+            elif ap_id(hdr) in (0x331, 0x332, 0x333, 0x334):
+                msg += f" {-1:8x} {-1:6d} {buf['TcSeqControl'][0]:12d}"
+                if ap_id(hdr) == 0x332:
+                    msg += (f" {bin(buf['TcErrorCode'][0])}"
+                            f" {buf['RejectParameter1'][0]}"
+                            f" {buf['RejectParameter2'][0]}")
+                if ap_id(hdr) == 0x334:
+                    msg += (f" {bin(buf['TcErrorCode'][0])}"
+                            f" {buf['FailParameter1'][0]}"
+                            f" {buf['FailParameter2'][0]}")
+            fp.write(msg + "\n")
 
-    Returns
-    -------
-    tuple of np.ndarray
-         Contains Science telemetry per full detector readout. The detector
-         readouts are stored in a seperate 2-D array
-    """
-    sci = iter(ccsds_sci)
-
-    images = ()
-    science = ()
-    stop_iter = False
-    while True:
-        while True:
-            try:
-                segment = next(sci)
-            except StopIteration:
-                stop_iter = True
-                break
-
-            if grouping_flag(segment['hdr']) == 1:
-                break
-
-        if stop_iter:
-            break
-
-        # found start of detector read-out
-        buff = segment['data'].copy()
-        buff['frame'][0] = np.array(())
-
-        read_frame = False
-        frame = ()
-        if (mode == 'all'
-            or (mode == 'full'
-                and buff['hk']['IMRLEN'][0] == FULLFRAME_BYTES)
-            or (mode == 'binned'
-                and buff['hk']['IMRLEN'][0] < FULLFRAME_BYTES)):
-            read_frame = True
-            frame = (segment['data']['frame'][0],)
-
-        # perform loop over all detector segments of this frame
-        while True:
-            try:
-                segment = next(sci)
-            except StopIteration:
-                stop_iter = True
-                break
-
-            if stop_iter:
-                break
-
-            if read_frame:
-                frame += (segment['data']['frame'][0],)
-            if grouping_flag(segment['hdr']) == 2:
-                if read_frame:
-                    science += (buff,)
-                    images += (np.concatenate(frame),)
-                break
-
-    # return empty arrays when no measurement data found
-    if not science:
-        return np.array(()), np.array(())
-
-    img_dims = [frame.size for frame in images]
-    if len(np.unique(img_dims)) == 1:
-        return np.concatenate(science), np.vstack(images)
-
-    # fill image data to the dimension of the largest read-out
-    img_data = np.empty((len(img_dims), np.max(img_dims)), dtype='u2')
-    for ii, data in enumerate(images):
-        img_data[ii, :data.size] = data
 
-    return np.concatenate(science), img_data
+def dump_science(flname: str, ccsds_sci: tuple[np.ndarray]):
+    """Dump telemetry header info (Science)."""
+    with Path(flname).open('w', encoding='ascii') as fp:
+        fp.write('APID Grouping Counter Length'
+                 ' ICUSWVER MPS_ID  IMRLEN     ICU_SEC ICU_SUBSEC\n')
+        for segment in ccsds_sci:
+            hdr = segment['hdr'][0]
+            if grouping_flag(hdr) == 1:
+                nom_hk = segment['hk']
+                icu_tm = segment['icu_tm']
+                fp.write(f"{ap_id(hdr):4x} {grouping_flag(hdr):8d}"
+                         f" {sequence(hdr):7d} {packet_length(hdr):6d}"
+                         f" {nom_hk['ICUSWVER'][0]:8x}"
+                         f" {nom_hk['MPS_ID'][0]:6d}"
+                         f" {nom_hk['IMRLEN'][0]:7d}"
+                         f" {icu_tm['tai_sec'][0]:11d}"
+                         f" {icu_tm['sub_sec'][0]:10d}\n")
+            else:
+                fp.write(f'{ap_id(hdr):4x} {grouping_flag(hdr):8d}'
+                         f' {sequence(hdr):7d} {packet_length(hdr):6d}\n')
```

### Comparing `pyspex-1.3.9/src/pyspex/lv1_args.py` & `pyspex-1.4.0rc1/src/pyspex/lv1_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 #
 # License:  BSD-3-Clause
 """
 Handle command-line parameters and settings from the YAML file
 for L1A generation.
 """
 from __future__ import annotations
-
 __all__ = ['get_l1a_settings']
 
 import argparse
+import sys
 from dataclasses import dataclass, field
 from pathlib import Path
 
 import yaml
 
 from .version import pyspex_version
 
@@ -31,15 +31,15 @@
        matching.
 - st3: CCSDS packages with ITOS and spacewire headers -- provide name
        of one file with extension '.ST3'.
 - dsb: CCSDS packages with PACE headers -- provide list of filenames
        with extension '.spx'.
 """
 
-ARG_YAML_HELP = """provide settings file in YAML format (inflight example):
+ARG_YAML_HELP = """provide settings file in YAML format (in-flight example):
 
 # define output directory, default is current working directory
 outdir: .
 # define name of output file, will be generated automatically when empty
 outfile: ''
 # compress the dataset /science_data/detector_images
 compression: True
@@ -54,61 +54,63 @@
 - <PATH>/SPX022000010.spx
 - <PATH>/SPX022000011.spx
 - <PATH>/SPX022000012.spx
 - <PATH>/SPX022000013.spx
 
 """
 
-EPILOG_HELP = """Usage:
+_prog_name_ = Path(sys.argv[0]).name
+EPILOG_HELP = f"""Usage:
   Generate L1A from OCAL level-0 data directly from the SPEXone instrument:
 
-    spx1_level01a <Path>/NomSciCal1_20220123T121801.676167.H
+    {_prog_name_} <Path>/NomSciCal1_20220123T121801.676167.H
 
     Note that OCAL science & telemetry data is read from the files:
       <Path>/NomSciCal1_20220123T121801.676167.?
       <Path>/NomSciCal1_20220123T121801.676167.??
       <Path>/NomSciCal1_20220123T121801.676167_hk.?
 
   Generate L1A from OCAL level-0 data via ITOS from the PACE platform:
 
-    spx1_level01a <Path>/DIAG_20220124_175458_073.ST3
+    {_prog_name_} <Path>/DIAG_20220124_175458_073.ST3
 
-  Generate L1A from inflight level-0 data, store product in directory L1A:
+  Generate L1A from in-flight level-0 data, store product in directory L1A:
 
-    spx1_level01a --outdir L1A <Path>/SPX*.spx
+    {_prog_name_} --outdir L1A <Path>/SPX*.spx
 
-  Generate L1A from inflight level-0 data read settings from a YAML file:
+  Generate L1A from in-flight level-0 data read settings from a YAML file:
 
-    spx1_level01a --yaml config_l1a_gen.yaml
+    {_prog_name_} --yaml config_l1a_gen.yaml
 
     An example YAML file:
        outdir: L1A
        outfile: ''
        file_version: 1
-       compresion: False
+       compression: False
        eclipse: False
        hkt_list: HKT/PACE.20220617T011*.HKT.nc
        l0_list: <PATH>/SPX0220000??.spx
 
   Dry-run, be extra verbose without generating data:
 
-    spx1_level01a --debug <Path>/NomSciCal1_20220123T121801.676167.H
+    {_prog_name_} --debug <Path>/NomSciCal1_20220123T121801.676167.H
 
   Read level-0 data and dump CCSDS packet headers in ASCII:
 
-    spx1_level01a --dump <Path>/NomSciCal1_20220123T121801.676167.H
+    {_prog_name_} --dump <Path>/NomSciCal1_20220123T121801.676167.H
 
 Return codes:
   2      Failed to parse command-line parameters.
-  100    Input file does not exist or failed to read from input file.
-  101    Input file not recognized as a SPEXone level-0 product.
-  110    Corrupted SPEXone level-0 data.
-  120    SPEXone level-0 data does not contain Science data, no L1A generated.
-  130    Failed to generate output file due to permission error.
+  110    One (or more) SPEXone level-0 files not found.
+  115    Failed to generate output directry due to permission error.
+  121    Input file not recognized as a SPEXone level-0 product.
+  122    Corrupted SPEXone level-0 data.
   131    Failed to generate output file due to netCDF4 library issues.
+  132    Incomplete set of navigation data detected
+  135    Failed to generate output file due to permission error.
 
 Environment:
    'OCVARROOT'
        The number of leap seconds for the TAI to UTC conversion are determined
        using the file 'tai-utc.dat'. A copy of this file is included in the
        package `pyspex`. The latest version can be obtained from
          `https://maia.usno.navy.mil/ser7/tai-utc.dat`.
@@ -124,15 +126,15 @@
     debug: bool = False
     dump: bool = False
     verbose: bool = False
     compression: bool = False
     outdir: Path = Path('.').resolve()
     outfile: str = ''
     file_version: int = 1
-    eclipse: bool = None
+    eclipse: bool | None = None
     yaml_fl: Path = None
     hkt_list: list[Path] = field(default_factory=list)
     l0_format: str = ''
     l0_list: list[Path] = field(default_factory=list)
 
 
 def __commandline_settings():
@@ -144,44 +146,48 @@
     parser.add_argument('-v', '--version', action='version',
                         version='%(prog)s v' + pyspex_version())
     parser.add_argument('--debug', action='store_true',
                         help="be extra verbose, no output files generated")
     parser.add_argument('--dump', action='store_true',
                         help="dump CCSDS packet headers in ASCII")
     parser.add_argument('--verbose', action='store_true', help="be verbose")
+    group = parser.add_mutually_exclusive_group(required=False)
+    group.add_argument('--eclipse', action='store_true', default=None)
+    group.add_argument('--no_eclipse', dest='eclipse', action='store_false')
     parser.add_argument('--outdir', type=Path, default=None,
                         help=("directory to store the generated"
                               " level-1A product(s)"))
     # group = parser.add_mutually_exclusive_group(required=True)
     parser.add_argument('--yaml', type=Path, default=None, help=ARG_YAML_HELP)
     parser.add_argument('lv0_list', nargs='*', help=ARG_INPUT_HELP)
     args = parser.parse_args()
-    print(args)
 
     config = Config()
     if args.debug:
         config.debug = True
     if args.dump:
         config.dump = True
     if args.verbose:
         config.verbose = True
+    if args.eclipse is not None:
+        config.eclipse = args.eclipse
     if args.outdir is not None:
         config.outdir = args.outdir
     if args.yaml:
         config.yaml_fl = args.yaml
     elif args.lv0_list:
         config.l0_list = [Path(x) for x in args.lv0_list]
     else:
         parser.error('You should provide a YAML file or names of L0 products')
 
     return config
 
 
 # pylint: disable=too-many-branches
-def __yaml_settings(config):
+def __yaml_settings(config: dataclass) -> dataclass:
     """Read YAML configuration file."""
     with open(config.yaml_fl, encoding='ascii') as fid:
         config_yaml = yaml.safe_load(fid)
 
     if 'outdir' in config_yaml and config_yaml['outdir'] is not None:
         config.outdir = Path(config_yaml['outdir'])
     if 'outfile' in config_yaml and config_yaml['outfile']:
@@ -210,15 +216,15 @@
                 config.l0_list = sorted(Path(mypath).glob('*'))
             else:
                 config.l0_list = sorted(Path(mypath.parent).glob(mypath.name))
 
     return config
 
 
-def check_input_files(config):
+def check_input_files(config: dataclass) -> dataclass:
     """
     Check level-0 files on existence and format
 
     Parameters
     ----------
     config :  dataclass
```

### Comparing `pyspex-1.3.9/src/pyspex/lv1_gse.py` & `pyspex-1.4.0rc1/src/pyspex/lv1_gse.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,31 +9,32 @@
 # License:  BSD-3-Clause
 """
 Contains the class `LV1gse` which checks EGSE/OGSE data and/or writes it to
 a SPEXone Level-1A product.
 """
 __all__ = ['LV1gse']
 
-import netCDF4 as nc4
 import numpy as np
+# pylint: disable=no-name-in-module
+from netCDF4 import Dataset
 
 
 # --------------------------------------------------
 class LV1gse:
     """Adds EGSE/OGSE data to a SPEXone Level-1A product.
 
     Parameters
     ----------
     l1a_file: str
         Name of the Level-1A product
     """
     def __init__(self, l1a_file: str) -> None:
         """Initialize netCDF4 group 'gse_data' in a SPEXone Level-1 product.
         """
-        self.fid = nc4.Dataset(l1a_file, 'r+')
+        self.fid = Dataset(l1a_file, 'r+')
 
         if self.fid.groups.get("gse_data"):
             return
 
         # investigate filename
         parts = l1a_file.split('_')
         if len(parts) > 2 and parts[0] == 'SPX1':
```

### Comparing `pyspex-1.3.9/src/pyspex/ogse_db.py` & `pyspex-1.4.0rc1/src/pyspex/ogse_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         """
         Helper function for numpy.loadtxt()
         convert byte-string to timestamp (UTC)
 
         Parameters
         ----------
         str_date : byte
-            isoformated date-time string with timezone CET
+            date-time string in ISO format with timezone CET
 
         Returns
         -------
         timestamp :  float
             Unix timestamp in UTC
         """
         buff = str_date.strip().decode('ascii') + '+01:00'
```

### Comparing `pyspex-1.3.9/src/pyspex/ogse_dolp.py` & `pyspex-1.4.0rc1/src/pyspex/ogse_dolp.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/src/pyspex/ogse_grande.py` & `pyspex-1.4.0rc1/src/pyspex/ogse_grande.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/src/pyspex/ogse_helios.py` & `pyspex-1.4.0rc1/src/pyspex/ogse_helios.py`

 * *Files identical despite different names*

### Comparing `pyspex-1.3.9/src/pyspex/ogse_laser.py` & `pyspex-1.4.0rc1/src/pyspex/ogse_laser.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 #
 # Copyright (c) 2019-2023 SRON - Netherlands Institute for Space Research
 #    All Rights Reserved
 #
 # License:  BSD-3-Clause
 """
 Read characteristics of the OPO laser used at NASA GSFC for the ISRF and
-Straylight measurements.
+Stray-light measurements.
 """
+from __future__ import annotations
 __all__ = ['read_gse_excel']
 
 from pathlib import Path
 
 import numpy as np
 import xarray as xr
 from openpyxl import load_workbook
```

### Comparing `pyspex-1.3.9/src/pyspex/tif_io.py` & `pyspex-1.4.0rc1/src/pyspex/tif_io.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 # Copyright (c) 2019-2023 SRON - Netherlands Institute for Space Research
 #    All Rights Reserved
 #
 # License:  BSD-3-Clause
 """
 Contains the class `TIFio` to read simulated SPEXone measurements.
 """
+from __future__ import annotations
+
 __all__ = ['TIFio']
 
 from pathlib import Path
 
 import numpy as np
 
 try:
@@ -39,22 +41,23 @@
         ----------
         hdr_file : str
         inp_tif : bool
         lineskip : bool
 
         Examples
         --------
+        Read a SPEXone TIFF file::
 
-        >>>  tif = TIFio(filename)
-        >>>  print(tif.header())
-        >>>  print(tif.tags()[0])
-        >>>  print(tif.images().shape)
-
+        >>  tif = TIFio(filename)
+        >>  print(tif.header())
+        >>  print(tif.tags()[0])
+        >>  print(tif.images().shape)
         """
-        def __init__(self, hdr_file: str, inp_tif=False, lineskip=False):
+        def __init__(self, hdr_file: str, inp_tif: bool = False,
+                     lineskip: bool = False):
             """Initialize TIFio object
             """
             if not Path(hdr_file).is_file():
                 raise FileNotFoundError(f'file {hdr_file} not found')
 
             # initialize class-attributes
             self.filename = Path(hdr_file)
@@ -117,21 +120,21 @@
                 tif_path = self.dir_name / f'{self.__stem}_{num}.tif'
                 with pytiff.Tiff(str(tif_path)) as handle:
                     res.append(handle.read_tags())
 
             return res
 
         # --------------------------------------------------
-        def images(self, n_frame=None):
+        def images(self, n_frame: int | None = None):
             """Return TIFF data as numpy array.
 
             Parameters
             ----------
             n_frame :  int, optional
-            Distribute coadded signal (32-bit) over n_frame images (16-bit)
+               Distribute coadded signal (32-bit) over n_frame images (16-bit)
             """
             if self.__header is None:
                 self.header()
 
             if self.inp_tif:
                 tif_path = self.dir_name / f'{self.__stem}_inp.tif'
                 with pytiff.Tiff(str(tif_path)) as handle:
```

### Comparing `pyspex-1.3.9/src/pyspex/version.py` & `pyspex-1.4.0rc1/src/pyspex/version.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,10 +18,14 @@
 def pyspex_version(full=False, githash=False):
     """Returns software version as obtained from git.
     """
     if full:
         return __version__
 
     if githash:
-        return __version__.split('+g')[1].split('.')[0]
+        res = __version__.split('+g')
+        if len(res) > 1:
+            return res[1].split('.')[0]
+
+        return 'v' + ''.join([f"{int(x):02d}" for x in res[0].split('.')])
 
     return __version__.split('+')[0]
```

### Comparing `pyspex-1.3.9/src/pyspex.egg-info/PKG-INFO` & `pyspex-1.4.0rc1/src/pyspex.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspex
-Version: 1.3.9
+Version: 1.4.0rc1
 Summary: Software package to handle SPEXone Level-0 and Level-1 data
 Author-email: Richard van Hees <r.m.van.hees@sron.nl>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/rmvanhees/pyspex
 Project-URL: documentation, https://pyspex.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/rmvanhees/pyspex/issues
 Classifier: Development Status :: 5 - Production/Stable
```

