# Comparing `tmp/discovery-capability-0.4.9.tar.gz` & `tmp/discovery-capability-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-capability-0.4.9.tar", last modified: Thu Jul 27 16:17:51 2023, max compression
+gzip compressed data, was "discovery-capability-0.5.0.tar", last modified: Thu Jul 27 20:10:14 2023, max compression
```

## Comparing `discovery-capability-0.4.9.tar` & `discovery-capability-0.5.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:51.101684 discovery-capability-0.4.9/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.4.9/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.4.9/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-27 16:17:51.102237 discovery-capability-0.4.9/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.4.9/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:50.935577 discovery-capability-0.4.9/discovery_capability.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-27 16:17:50.000000 discovery-capability-0.4.9/discovery_capability.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     2313 2023-07-27 16:17:50.000000 discovery-capability-0.4.9/discovery_capability.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-27 16:17:50.000000 discovery-capability-0.4.9/discovery_capability.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-07-27 16:17:50.000000 discovery-capability-0.4.9/discovery_capability.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-07-27 16:17:50.000000 discovery-capability-0.4.9/discovery_capability.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:50.935911 discovery-capability-0.4.9/ds_capability/
--rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-25 13:20:19.000000 discovery-capability-0.4.9/ds_capability/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:50.937942 discovery-capability-0.4.9/ds_capability/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.4.9/ds_capability/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13503 2023-07-24 23:04:05.000000 discovery-capability-0.4.9/ds_capability/components/abstract_common_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3007 2023-07-27 15:44:19.000000 discovery-capability-0.4.9/ds_capability/components/commons.py
--rw-r--r--   0 doatridge   (503) staff       (20)    10395 2023-07-27 16:16:38.000000 discovery-capability-0.4.9/ds_capability/components/discovery.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.4.9/ds_capability/components/feature_build.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:50.938697 discovery-capability-0.4.9/ds_capability/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.4.9/ds_capability/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:50.942852 discovery-capability-0.4.9/ds_capability/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.4.9/ds_capability/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.4.9/ds_capability/intent/abstract_feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.4.9/ds_capability/intent/common_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7128 2023-07-03 22:57:08.000000 discovery-capability-0.4.9/ds_capability/intent/feature_build_correlate_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    66414 2023-07-25 13:15:36.000000 discovery-capability-0.4.9/ds_capability/intent/feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15830 2023-07-21 22:27:17.000000 discovery-capability-0.4.9/ds_capability/intent/feature_build_model_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:50.946194 discovery-capability-0.4.9/ds_capability/managers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.4.9/ds_capability/managers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.4.9/ds_capability/managers/controller_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.4.9/ds_capability/managers/feature_build_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.4.9/ds_capability/managers/feature_select_property_manager.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:51.090894 discovery-capability-0.4.9/ds_capability/sample/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/lookup_complaints.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/lookup_professions.py
--rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/lookup_uk_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/lookup_uk_postcode_district.py
--rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/lookup_us_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/lookup_us_street_names.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/lookup_us_street_suffix.py
--rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_companies_fortune1000.py
--rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_companies_inc5000.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_uk_postcodes_primary.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_age_salary.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_city_area_code.csv
--rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_city_zipcodes_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_forename_mf.py
--rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_forename_unisex.py
--rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_full_address.py
--rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_healthcare_organisations.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_phone_code.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_profession_detail_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_surname_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.4.9/ds_capability/sample/sample_data.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-07-27 16:17:51.103386 discovery-capability-0.4.9/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.4.9/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:51.092007 discovery-capability-0.4.9/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.4.9/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:51.093723 discovery-capability-0.4.9/test/component/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.4.9/test/component/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2954 2023-07-27 16:12:25.000000 discovery-capability-0.4.9/test/component/discovery_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.4.9/test/component/synthetic_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:51.095254 discovery-capability-0.4.9/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.4.9/test/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:51.100101 discovery-capability-0.4.9/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.4.9/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.4.9/test/intent/fb_analysis_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.4.9/test/intent/fb_diff_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-25 13:17:32.000000 discovery-capability-0.4.9/test/intent/fb_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.4.9/test/intent/fb_model_intent_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:14.089218 discovery-capability-0.5.0/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.5.0/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.5.0/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-27 20:10:14.089477 discovery-capability-0.5.0/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.5.0/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:13.914532 discovery-capability-0.5.0/discovery_capability.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-27 20:10:13.000000 discovery-capability-0.5.0/discovery_capability.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     2313 2023-07-27 20:10:13.000000 discovery-capability-0.5.0/discovery_capability.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-27 20:10:13.000000 discovery-capability-0.5.0/discovery_capability.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-07-27 20:10:13.000000 discovery-capability-0.5.0/discovery_capability.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-07-27 20:10:13.000000 discovery-capability-0.5.0/discovery_capability.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:13.914960 discovery-capability-0.5.0/ds_capability/
+-rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-27 16:53:34.000000 discovery-capability-0.5.0/ds_capability/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:13.918783 discovery-capability-0.5.0/ds_capability/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.5.0/ds_capability/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14475 2023-07-27 16:49:58.000000 discovery-capability-0.5.0/ds_capability/components/abstract_common_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3007 2023-07-27 15:44:19.000000 discovery-capability-0.5.0/ds_capability/components/commons.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    10419 2023-07-27 18:38:24.000000 discovery-capability-0.5.0/ds_capability/components/discovery.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.5.0/ds_capability/components/feature_build.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:13.919791 discovery-capability-0.5.0/ds_capability/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.5.0/ds_capability/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:13.923784 discovery-capability-0.5.0/ds_capability/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.5.0/ds_capability/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.5.0/ds_capability/intent/abstract_feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.5.0/ds_capability/intent/common_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7128 2023-07-03 22:57:08.000000 discovery-capability-0.5.0/ds_capability/intent/feature_build_correlate_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    67984 2023-07-27 20:04:19.000000 discovery-capability-0.5.0/ds_capability/intent/feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15830 2023-07-21 22:27:17.000000 discovery-capability-0.5.0/ds_capability/intent/feature_build_model_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:13.927507 discovery-capability-0.5.0/ds_capability/managers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.5.0/ds_capability/managers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.5.0/ds_capability/managers/controller_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.5.0/ds_capability/managers/feature_build_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.5.0/ds_capability/managers/feature_select_property_manager.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:14.081872 discovery-capability-0.5.0/ds_capability/sample/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/lookup_complaints.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/lookup_professions.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/lookup_uk_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/lookup_uk_postcode_district.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/lookup_us_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/lookup_us_street_names.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/lookup_us_street_suffix.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_companies_fortune1000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_companies_inc5000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_uk_postcodes_primary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_age_salary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_city_area_code.csv
+-rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_city_zipcodes_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_forename_mf.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_forename_unisex.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_full_address.py
+-rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_healthcare_organisations.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_phone_code.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_profession_detail_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_surname_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.5.0/ds_capability/sample/sample_data.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-07-27 20:10:14.090286 discovery-capability-0.5.0/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.5.0/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:14.082897 discovery-capability-0.5.0/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.5.0/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:14.084371 discovery-capability-0.5.0/test/component/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.5.0/test/component/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2986 2023-07-27 16:26:58.000000 discovery-capability-0.5.0/test/component/discovery_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.5.0/test/component/synthetic_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:14.085205 discovery-capability-0.5.0/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.5.0/test/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:14.088155 discovery-capability-0.5.0/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.5.0/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.5.0/test/intent/fb_analysis_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.5.0/test/intent/fb_diff_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-27 20:05:03.000000 discovery-capability-0.5.0/test/intent/fb_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.5.0/test/intent/fb_model_intent_test.py
```

### Comparing `discovery-capability-0.4.9/LICENSE.txt` & `discovery-capability-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/PKG-INFO` & `discovery-capability-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.4.9
+Version: 0.5.0
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.4.9/README.rst` & `discovery-capability-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/discovery_capability.egg-info/PKG-INFO` & `discovery-capability-0.5.0/discovery_capability.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.4.9
+Version: 0.5.0
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.4.9/discovery_capability.egg-info/SOURCES.txt` & `discovery-capability-0.5.0/discovery_capability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/components/abstract_common_component.py` & `discovery-capability-0.5.0/ds_capability/components/abstract_common_component.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,21 +90,36 @@
         return
 
     @staticmethod
     def canonical_report(canonical: pa.Table, stylise: bool=None, display_width: int=None):
         """The Canonical Report is a data dictionary of the canonical providing a reference view of the dataset's
         attribute properties
 
-        :param canonical: the DataFrame to view
-        :param stylise: if True present the report stylised.
+        :param canonical: the table to view
+        :param stylise: (optional) if True present the report stylised.
         :param display_width: (optional) the width of the observational display
         """
         stylise = stylise if isinstance(stylise, bool) else True
         return DataDiscovery.data_dictionary(canonical=canonical, stylise=stylise, display_width=display_width)
 
+    @staticmethod
+    def quality_report(canonical: pa.Table, nulls_threshold: float=None, dom_threshold: float=None,
+                     cat_threshold: int=None, stylise: bool=None):
+        """ Analyses a dataset, passed as a DataFrame and returns a quality summary
+
+        :param canonical: The table to view.
+        :param cat_threshold: (optional) The threshold for the max number of unique categories. Default is 60
+        :param dom_threshold: (optional) The threshold limit of a dominant value. Default 0.98
+        :param nulls_threshold: (optional) The threshold limit of a nulls value. Default 0.9
+        :param stylise: (optional) if the output is stylised
+        """
+        stylise = stylise if isinstance(stylise, bool) else True
+        return DataDiscovery.data_quality(canonical=canonical, nulls_threshold=nulls_threshold,
+                                          dom_threshold=dom_threshold, cat_threshold=cat_threshold, stylise=stylise)
+
     def report_canonical_schema(self, schema: [str, dict]=None, roots: [str, list]=None,
                                 sections: [str, list]=None, elements: [str, list]=None, stylise: bool=True):
         """ presents the current canonical schema
 
         :param schema: (optional) the name of the schema
         :param roots: (optional) one or more tree roots
         :param sections: (optional) the section under the root
```

### Comparing `discovery-capability-0.4.9/ds_capability/components/commons.py` & `discovery-capability-0.5.0/ds_capability/components/commons.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/components/discovery.py` & `discovery-capability-0.5.0/ds_capability/components/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         _key_columns = 0
         for n in tbl.column_names:
             c = tbl.column(n).combine_chunks()
             if pa.types.is_nested(c.type):
                 _nest_columns += 1
                 continue
             if not pa.types.is_dictionary(c.type):
-                if c.null_count/pc.count(c).as_py() > nulls_threshold:
+                if pc.count(c).as_py() == 0 or c.null_count/pc.count(c).as_py() > nulls_threshold:
                     _null_columns += 1
                 elif pc.count_distinct(c.drop_null()).as_py() == pc.count(c).as_py():
                     _key_columns += 1
                 elif 1-(pc.count_distinct(c.drop_null()).as_py()/pc.count(c).as_py()) > dom_threshold:
                     _dom_columns += 1
                 elif pc.count_distinct(c.drop_null()).as_py() == pc.count(c).as_py():
                     _key_columns += 1
@@ -117,19 +117,19 @@
         labels = [f'Attributes', 'DataType', 'Nulls', 'Dominate', 'Valid', 'Unique', 'Observations']
         # attempt cast
         if isinstance(table_cast, bool) and table_cast:
             canonical = Commons.table_cast(canonical)
         for c in canonical.column_names:
             column = canonical.column(c).combine_chunks()
             if pa.types.is_nested(column.type):
-                record.append([c,'Nested','','','','',''])
+                record.append([c,'nested',0,0,0,0,''])
                 continue
             # data type
             line = [c,
-                    'Category' if pc.starts_with(str(column.type), 'dict').as_py() else str(column.type),
+                    'category' if pc.starts_with(str(column.type), 'dict').as_py() else str(column.type),
                     # null percentage
                     round(column.null_count / canonical.num_rows, 3)]
             # dominant percentage
             arr_vc = column.value_counts()
             value = arr_vc.filter(pc.equal(arr_vc.field(1), pc.max(arr_vc.field(1)))).field(1)[0].as_py()
             line.append(round(value / canonical.num_rows, 3))
             # valid
```

### Comparing `discovery-capability-0.4.9/ds_capability/components/feature_build.py` & `discovery-capability-0.5.0/ds_capability/components/feature_build.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/intent/abstract_feature_build_intent.py` & `discovery-capability-0.5.0/ds_capability/intent/abstract_feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/intent/common_intent.py` & `discovery-capability-0.5.0/ds_capability/intent/common_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/intent/feature_build_correlate_intent.py` & `discovery-capability-0.5.0/ds_capability/intent/feature_build_correlate_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/intent/feature_build_intent.py` & `discovery-capability-0.5.0/ds_capability/intent/feature_build_intent.py`

 * *Files 8% similar despite different names*

```diff
@@ -956,15 +956,33 @@
             canonical = Commons.table_append(canonical, _)
             # nulls_str
             _ = pa.table([pa.array(pa.nulls(size), pa.string())], names=['nulls_str'])
             canonical = Commons.table_append(canonical, _)
             # nulls
             _ = pa.table([pa.nulls(size)], names=['nulls'])
             canonical = Commons.table_append(canonical, _)
-
+            # list array
+            _ = pa.array(list(zip(canonical.column('num').to_pylist(), canonical.column('num_null').to_pylist())))
+            _ = pa.table([_], names=['nest_list'])
+            canonical = Commons.table_append(canonical, _)
+            # struct array
+            shuffle_int = pa.Array.from_pandas(canonical.column('int').to_pandas().sample(frac=1))
+            shuffle_num = pa.Array.from_pandas(canonical.column('num').to_pandas().sample(frac=1))
+            n_tbl = pa.table([canonical.column('int')], names=['_id'])
+            n_tbl = Commons.table_append(n_tbl, pa.table([canonical.column('string')], names=['doc_name']))
+            n_tbl = Commons.table_append(n_tbl, pa.table([canonical.column('date')], names=['date.prod']))
+            n_tbl = Commons.table_append(n_tbl, pa.table([canonical.column('date_null')], names=['date.last']))
+            n_tbl = Commons.table_append(n_tbl, pa.table([shuffle_int], names=['metrics.nest_list_0._id']))
+            n_tbl = Commons.table_append(n_tbl, pa.table([shuffle_num], names=['metrics.nest_list_0.value']))
+            n_tbl = Commons.table_append(n_tbl,
+                                         pa.table([canonical.column('int_null')], names=['metrics.nest_list_1._id']))
+            n_tbl = Commons.table_append(n_tbl,
+                                         pa.table([canonical.column('num_null')], names=['metrics.nest_list_1.value']))
+            _ = Commons.table_nest(n_tbl)
+            canonical = Commons.table_append(canonical, pa.table([pa.array(_)], names=['nest_struct']))
 
         return canonical
 
     def get_noise(self, size: int, num_columns: int, seed: int = None, name_prefix: str=None,
                   save_intent: bool = None, column_name: [int, str] = None, intent_order: int = None,
                   replace_intent: bool = None, remove_duplicates: bool = None) -> pd.DataFrame:
         """ Generates multiple columns of noise in your dataset
```

### Comparing `discovery-capability-0.4.9/ds_capability/intent/feature_build_model_intent.py` & `discovery-capability-0.5.0/ds_capability/intent/feature_build_model_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/managers/controller_property_manager.py` & `discovery-capability-0.5.0/ds_capability/managers/controller_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/managers/feature_build_property_manager.py` & `discovery-capability-0.5.0/ds_capability/managers/feature_build_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/managers/feature_select_property_manager.py` & `discovery-capability-0.5.0/ds_capability/managers/feature_select_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/lookup_complaints.py` & `discovery-capability-0.5.0/ds_capability/sample/lookup_complaints.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/lookup_professions.py` & `discovery-capability-0.5.0/ds_capability/sample/lookup_professions.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/lookup_uk_city.py` & `discovery-capability-0.5.0/ds_capability/sample/lookup_uk_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/lookup_uk_postcode_district.py` & `discovery-capability-0.5.0/ds_capability/sample/lookup_uk_postcode_district.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/lookup_us_city.py` & `discovery-capability-0.5.0/ds_capability/sample/lookup_us_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/lookup_us_street_names.py` & `discovery-capability-0.5.0/ds_capability/sample/lookup_us_street_names.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/lookup_us_street_suffix.py` & `discovery-capability-0.5.0/ds_capability/sample/lookup_us_street_suffix.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/map_companies_fortune1000.py` & `discovery-capability-0.5.0/ds_capability/sample/map_companies_fortune1000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/map_companies_inc5000.py` & `discovery-capability-0.5.0/ds_capability/sample/map_companies_inc5000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/map_uk_postcodes_primary.py` & `discovery-capability-0.5.0/ds_capability/sample/map_uk_postcodes_primary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/map_us_age_salary.py` & `discovery-capability-0.5.0/ds_capability/sample/map_us_age_salary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/map_us_city_area_code.csv` & `discovery-capability-0.5.0/ds_capability/sample/map_us_city_area_code.csv`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/map_us_city_zipcodes_rank.py` & `discovery-capability-0.5.0/ds_capability/sample/map_us_city_zipcodes_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/map_us_forename_mf.py` & `discovery-capability-0.5.0/ds_capability/sample/map_us_forename_mf.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/map_us_forename_unisex.py` & `discovery-capability-0.5.0/ds_capability/sample/map_us_forename_unisex.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/map_us_full_address.py` & `discovery-capability-0.5.0/ds_capability/sample/map_us_full_address.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/map_us_healthcare_organisations.py` & `discovery-capability-0.5.0/ds_capability/sample/map_us_healthcare_organisations.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/map_us_phone_code.py` & `discovery-capability-0.5.0/ds_capability/sample/map_us_phone_code.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/map_us_profession_detail_rank.py` & `discovery-capability-0.5.0/ds_capability/sample/map_us_profession_detail_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/map_us_surname_rank.py` & `discovery-capability-0.5.0/ds_capability/sample/map_us_surname_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/ds_capability/sample/sample_data.py` & `discovery-capability-0.5.0/ds_capability/sample/sample_data.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/setup.py` & `discovery-capability-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/test/component/discovery_test.py` & `discovery-capability-0.5.0/test/component/discovery_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,22 +66,22 @@
         tbl = tools.get_synthetic_data_types(1_000, inc_nulls=True)
         self.assertEqual(1_000, tbl.num_rows)
         self.assertEqual(17, tbl.num_columns)
 
     def test_data_dictionary(self):
         sb = FeatureBuild.from_memory()
         tools: FeatureBuildIntentModel = sb.tools
-        tbl = tools.get_synthetic_data_types(1000)
+        tbl = tools.get_synthetic_data_types(1000, inc_nulls=True)
         result = DataDiscovery.data_dictionary(tbl)
         print(result.column_names)
 
     def test_data_quality(self):
         sb = FeatureBuild.from_memory()
         tools: FeatureBuildIntentModel = sb.tools
-        tbl = tools.get_synthetic_data_types(1000)
+        tbl = tools.get_synthetic_data_types(1000, inc_nulls=True)
         result = DataDiscovery.data_quality(tbl)
         print(result.column_names)
         # c = result.column('summary').combine_chunks()
         # print(c)
         result = DataDiscovery.data_quality(tbl, stylise=True)
         pprint(result.to_string())
```

### Comparing `discovery-capability-0.4.9/test/component/synthetic_test.py` & `discovery-capability-0.5.0/test/component/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/test/intent/fb_analysis_intent_test.py` & `discovery-capability-0.5.0/test/intent/fb_analysis_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/test/intent/fb_diff_intent_test.py` & `discovery-capability-0.5.0/test/intent/fb_diff_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.9/test/intent/fb_intent_test.py` & `discovery-capability-0.5.0/test/intent/fb_intent_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,24 +55,24 @@
 
     def test_for_smoke(self):
         fb = FeatureBuild.from_memory()
         tools: FeatureBuildIntentModel = fb.tools
         tbl = tools.get_synthetic_data_types(100)
         self.assertEqual((100, 7), tbl.shape)
         tbl = tools.get_synthetic_data_types(100, inc_nulls=True, prob_nulls=0.03)
-        self.assertEqual((100, 17), tbl.shape)
+        self.assertEqual((100, 19), tbl.shape)
 
     def test_run_component_pipeline(self):
         fb = FeatureBuild.from_env('test', has_contract=False)
         tools: FeatureBuildIntentModel = fb.tools
         # reload the properties
         fb = FeatureBuild.from_env('test')
         _ = tools.get_synthetic_data_types(10, inc_nulls=True, column_name='d_types')
         result = fb.tools.run_intent_pipeline(size=20)
-        self.assertEqual((20, 17), result.shape)
+        self.assertEqual((20, 19), result.shape)
 
     def test_model_noise(self):
         fb = FeatureBuild.from_memory()
         tools: FeatureBuildIntentModel = fb.tools
         tbl = tools.get_noise(10, num_columns=3)
         self.assertEqual((10, 3), tbl.shape)
         self.assertEqual(['A', 'B', 'C'], tbl.column_names)
```

### Comparing `discovery-capability-0.4.9/test/intent/fb_model_intent_test.py` & `discovery-capability-0.5.0/test/intent/fb_model_intent_test.py`

 * *Files identical despite different names*

