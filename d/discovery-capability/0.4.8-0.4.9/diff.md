# Comparing `tmp/discovery-capability-0.4.8.tar.gz` & `tmp/discovery-capability-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-capability-0.4.8.tar", last modified: Tue Jul 25 13:19:27 2023, max compression
+gzip compressed data, was "discovery-capability-0.4.9.tar", last modified: Thu Jul 27 16:17:51 2023, max compression
```

## Comparing `discovery-capability-0.4.8.tar` & `discovery-capability-0.4.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.751383 discovery-capability-0.4.8/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.4.8/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.4.8/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-25 13:19:27.751701 discovery-capability-0.4.8/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.4.8/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.601534 discovery-capability-0.4.8/discovery_capability.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-25 13:19:27.000000 discovery-capability-0.4.8/discovery_capability.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     2313 2023-07-25 13:19:27.000000 discovery-capability-0.4.8/discovery_capability.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-25 13:19:27.000000 discovery-capability-0.4.8/discovery_capability.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-07-25 13:19:27.000000 discovery-capability-0.4.8/discovery_capability.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-07-25 13:19:27.000000 discovery-capability-0.4.8/discovery_capability.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.602381 discovery-capability-0.4.8/ds_capability/
--rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-24 23:05:27.000000 discovery-capability-0.4.8/ds_capability/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.606983 discovery-capability-0.4.8/ds_capability/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.4.8/ds_capability/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13503 2023-07-24 23:04:05.000000 discovery-capability-0.4.8/ds_capability/components/abstract_common_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3135 2023-07-24 22:34:35.000000 discovery-capability-0.4.8/ds_capability/components/commons.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5246 2023-07-24 22:53:50.000000 discovery-capability-0.4.8/ds_capability/components/discovery.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.4.8/ds_capability/components/feature_build.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.608039 discovery-capability-0.4.8/ds_capability/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.4.8/ds_capability/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.613149 discovery-capability-0.4.8/ds_capability/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.4.8/ds_capability/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.4.8/ds_capability/intent/abstract_feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.4.8/ds_capability/intent/common_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7128 2023-07-03 22:57:08.000000 discovery-capability-0.4.8/ds_capability/intent/feature_build_correlate_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    66414 2023-07-25 13:15:36.000000 discovery-capability-0.4.8/ds_capability/intent/feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15830 2023-07-21 22:27:17.000000 discovery-capability-0.4.8/ds_capability/intent/feature_build_model_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.618163 discovery-capability-0.4.8/ds_capability/managers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.4.8/ds_capability/managers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.4.8/ds_capability/managers/controller_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.4.8/ds_capability/managers/feature_build_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.4.8/ds_capability/managers/feature_select_property_manager.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.740487 discovery-capability-0.4.8/ds_capability/sample/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/lookup_complaints.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/lookup_professions.py
--rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/lookup_uk_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/lookup_uk_postcode_district.py
--rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/lookup_us_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/lookup_us_street_names.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/lookup_us_street_suffix.py
--rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_companies_fortune1000.py
--rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_companies_inc5000.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_uk_postcodes_primary.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_age_salary.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_city_area_code.csv
--rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_city_zipcodes_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_forename_mf.py
--rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_forename_unisex.py
--rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_full_address.py
--rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_healthcare_organisations.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_phone_code.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_profession_detail_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.4.8/ds_capability/sample/map_us_surname_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.4.8/ds_capability/sample/sample_data.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-07-25 13:19:27.752799 discovery-capability-0.4.8/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.4.8/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.744904 discovery-capability-0.4.8/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.4.8/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.746289 discovery-capability-0.4.8/test/component/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.4.8/test/component/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2086 2023-07-24 22:07:08.000000 discovery-capability-0.4.8/test/component/discovery_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.4.8/test/component/synthetic_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.747314 discovery-capability-0.4.8/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.4.8/test/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-25 13:19:27.750591 discovery-capability-0.4.8/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.4.8/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.4.8/test/intent/fb_analysis_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.4.8/test/intent/fb_diff_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-25 13:17:32.000000 discovery-capability-0.4.8/test/intent/fb_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.4.8/test/intent/fb_model_intent_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:51.101684 discovery-capability-0.4.9/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.4.9/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.4.9/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-27 16:17:51.102237 discovery-capability-0.4.9/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.4.9/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:50.935577 discovery-capability-0.4.9/discovery_capability.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-27 16:17:50.000000 discovery-capability-0.4.9/discovery_capability.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     2313 2023-07-27 16:17:50.000000 discovery-capability-0.4.9/discovery_capability.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-27 16:17:50.000000 discovery-capability-0.4.9/discovery_capability.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-07-27 16:17:50.000000 discovery-capability-0.4.9/discovery_capability.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-07-27 16:17:50.000000 discovery-capability-0.4.9/discovery_capability.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:50.935911 discovery-capability-0.4.9/ds_capability/
+-rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-25 13:20:19.000000 discovery-capability-0.4.9/ds_capability/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:50.937942 discovery-capability-0.4.9/ds_capability/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.4.9/ds_capability/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13503 2023-07-24 23:04:05.000000 discovery-capability-0.4.9/ds_capability/components/abstract_common_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3007 2023-07-27 15:44:19.000000 discovery-capability-0.4.9/ds_capability/components/commons.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    10395 2023-07-27 16:16:38.000000 discovery-capability-0.4.9/ds_capability/components/discovery.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.4.9/ds_capability/components/feature_build.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:50.938697 discovery-capability-0.4.9/ds_capability/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.4.9/ds_capability/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:50.942852 discovery-capability-0.4.9/ds_capability/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.4.9/ds_capability/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.4.9/ds_capability/intent/abstract_feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.4.9/ds_capability/intent/common_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7128 2023-07-03 22:57:08.000000 discovery-capability-0.4.9/ds_capability/intent/feature_build_correlate_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    66414 2023-07-25 13:15:36.000000 discovery-capability-0.4.9/ds_capability/intent/feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15830 2023-07-21 22:27:17.000000 discovery-capability-0.4.9/ds_capability/intent/feature_build_model_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:50.946194 discovery-capability-0.4.9/ds_capability/managers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.4.9/ds_capability/managers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.4.9/ds_capability/managers/controller_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.4.9/ds_capability/managers/feature_build_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.4.9/ds_capability/managers/feature_select_property_manager.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:51.090894 discovery-capability-0.4.9/ds_capability/sample/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/lookup_complaints.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/lookup_professions.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/lookup_uk_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/lookup_uk_postcode_district.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/lookup_us_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/lookup_us_street_names.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/lookup_us_street_suffix.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_companies_fortune1000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_companies_inc5000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_uk_postcodes_primary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_age_salary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_city_area_code.csv
+-rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_city_zipcodes_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_forename_mf.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_forename_unisex.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_full_address.py
+-rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_healthcare_organisations.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_phone_code.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_profession_detail_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.4.9/ds_capability/sample/map_us_surname_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.4.9/ds_capability/sample/sample_data.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-07-27 16:17:51.103386 discovery-capability-0.4.9/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.4.9/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:51.092007 discovery-capability-0.4.9/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.4.9/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:51.093723 discovery-capability-0.4.9/test/component/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.4.9/test/component/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2954 2023-07-27 16:12:25.000000 discovery-capability-0.4.9/test/component/discovery_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.4.9/test/component/synthetic_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:51.095254 discovery-capability-0.4.9/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.4.9/test/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 16:17:51.100101 discovery-capability-0.4.9/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.4.9/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.4.9/test/intent/fb_analysis_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.4.9/test/intent/fb_diff_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-25 13:17:32.000000 discovery-capability-0.4.9/test/intent/fb_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.4.9/test/intent/fb_model_intent_test.py
```

### Comparing `discovery-capability-0.4.8/LICENSE.txt` & `discovery-capability-0.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/PKG-INFO` & `discovery-capability-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.4.8
+Version: 0.4.9
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.4.8/README.rst` & `discovery-capability-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/discovery_capability.egg-info/PKG-INFO` & `discovery-capability-0.4.9/discovery_capability.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.4.8
+Version: 0.4.9
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.4.8/discovery_capability.egg-info/SOURCES.txt` & `discovery-capability-0.4.9/discovery_capability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/components/abstract_common_component.py` & `discovery-capability-0.4.9/ds_capability/components/abstract_common_component.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/components/commons.py` & `discovery-capability-0.4.9/ds_capability/components/commons.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,16 +50,14 @@
         for header in index_header:
             prev = ''
             for idx in range(len(canonical[header])):
                 if canonical[header].iloc[idx] == prev:
                     canonical[header].iloc[idx] = ''
                 else:
                     prev = canonical[header].iloc[idx]
-            # index = canonical[canonical[header].duplicated()].index.to_list()
-            # canonical.loc[index, header] = ''
         canonical = canonical.reset_index(drop=True)
         df_style = canonical.style.set_table_styles(style)
         _ = df_style.set_properties(**{'text-align': 'left'})
         if len(bold) > 0:
             _ = df_style.set_properties(subset=bold, **{'font-weight': 'bold'})
         if len(large_font) > 0:
             _ = df_style.set_properties(subset=large_font, **{'font-size': "120%"})
```

### Comparing `discovery-capability-0.4.8/ds_capability/components/feature_build.py` & `discovery-capability-0.4.9/ds_capability/components/feature_build.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/intent/abstract_feature_build_intent.py` & `discovery-capability-0.4.9/ds_capability/intent/abstract_feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/intent/common_intent.py` & `discovery-capability-0.4.9/ds_capability/intent/common_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/intent/feature_build_correlate_intent.py` & `discovery-capability-0.4.9/ds_capability/intent/feature_build_correlate_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/intent/feature_build_intent.py` & `discovery-capability-0.4.9/ds_capability/intent/feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/intent/feature_build_model_intent.py` & `discovery-capability-0.4.9/ds_capability/intent/feature_build_model_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/managers/controller_property_manager.py` & `discovery-capability-0.4.9/ds_capability/managers/controller_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/managers/feature_build_property_manager.py` & `discovery-capability-0.4.9/ds_capability/managers/feature_build_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/managers/feature_select_property_manager.py` & `discovery-capability-0.4.9/ds_capability/managers/feature_select_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/lookup_complaints.py` & `discovery-capability-0.4.9/ds_capability/sample/lookup_complaints.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/lookup_professions.py` & `discovery-capability-0.4.9/ds_capability/sample/lookup_professions.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/lookup_uk_city.py` & `discovery-capability-0.4.9/ds_capability/sample/lookup_uk_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/lookup_uk_postcode_district.py` & `discovery-capability-0.4.9/ds_capability/sample/lookup_uk_postcode_district.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/lookup_us_city.py` & `discovery-capability-0.4.9/ds_capability/sample/lookup_us_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/lookup_us_street_names.py` & `discovery-capability-0.4.9/ds_capability/sample/lookup_us_street_names.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/lookup_us_street_suffix.py` & `discovery-capability-0.4.9/ds_capability/sample/lookup_us_street_suffix.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/map_companies_fortune1000.py` & `discovery-capability-0.4.9/ds_capability/sample/map_companies_fortune1000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/map_companies_inc5000.py` & `discovery-capability-0.4.9/ds_capability/sample/map_companies_inc5000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/map_uk_postcodes_primary.py` & `discovery-capability-0.4.9/ds_capability/sample/map_uk_postcodes_primary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/map_us_age_salary.py` & `discovery-capability-0.4.9/ds_capability/sample/map_us_age_salary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/map_us_city_area_code.csv` & `discovery-capability-0.4.9/ds_capability/sample/map_us_city_area_code.csv`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/map_us_city_zipcodes_rank.py` & `discovery-capability-0.4.9/ds_capability/sample/map_us_city_zipcodes_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/map_us_forename_mf.py` & `discovery-capability-0.4.9/ds_capability/sample/map_us_forename_mf.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/map_us_forename_unisex.py` & `discovery-capability-0.4.9/ds_capability/sample/map_us_forename_unisex.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/map_us_full_address.py` & `discovery-capability-0.4.9/ds_capability/sample/map_us_full_address.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/map_us_healthcare_organisations.py` & `discovery-capability-0.4.9/ds_capability/sample/map_us_healthcare_organisations.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/map_us_phone_code.py` & `discovery-capability-0.4.9/ds_capability/sample/map_us_phone_code.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/map_us_profession_detail_rank.py` & `discovery-capability-0.4.9/ds_capability/sample/map_us_profession_detail_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/map_us_surname_rank.py` & `discovery-capability-0.4.9/ds_capability/sample/map_us_surname_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/ds_capability/sample/sample_data.py` & `discovery-capability-0.4.9/ds_capability/sample/sample_data.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/setup.py` & `discovery-capability-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/test/component/discovery_test.py` & `discovery-capability-0.4.9/test/component/discovery_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,28 +44,52 @@
             os.makedirs(os.environ['HADRON_PM_PATH'])
         except OSError:
             pass
         try:
             os.makedirs(os.environ['HADRON_DEFAULT_PATH'])
         except OSError:
             pass
+        try:
+            shutil.copytree('../_test_data', os.path.join(os.environ['PWD'], 'working/source'))
+        except OSError:
+            pass
         PropertyManager._remove_all()
 
     def tearDown(self):
         try:
             shutil.rmtree('working')
         except OSError:
             pass
 
     def test_for_smoke(self):
         sb = FeatureBuild.from_memory()
         tools: FeatureBuildIntentModel = sb.tools
-        tbl = tools.get_synthetic_data_types(1_000)
-        result = DataDiscovery.data_dictionary(tbl, stylise=True)
-        pprint(result)
+        tbl = tools.get_synthetic_data_types(1_000, inc_nulls=True)
+        self.assertEqual(1_000, tbl.num_rows)
+        self.assertEqual(17, tbl.num_columns)
+
+    def test_data_dictionary(self):
+        sb = FeatureBuild.from_memory()
+        tools: FeatureBuildIntentModel = sb.tools
+        tbl = tools.get_synthetic_data_types(1000)
+        result = DataDiscovery.data_dictionary(tbl)
+        print(result.column_names)
+
+    def test_data_quality(self):
+        sb = FeatureBuild.from_memory()
+        tools: FeatureBuildIntentModel = sb.tools
+        tbl = tools.get_synthetic_data_types(1000)
+        result = DataDiscovery.data_quality(tbl)
+        print(result.column_names)
+        # c = result.column('summary').combine_chunks()
+        # print(c)
+        result = DataDiscovery.data_quality(tbl, stylise=True)
+        pprint(result.to_string())
+
+
 
     def test_raise(self):
         with self.assertRaises(KeyError) as context:
             env = os.environ['NoEnvValueTest']
         self.assertTrue("'NoEnvValueTest'" in str(context.exception))
```

### Comparing `discovery-capability-0.4.8/test/component/synthetic_test.py` & `discovery-capability-0.4.9/test/component/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/test/intent/fb_analysis_intent_test.py` & `discovery-capability-0.4.9/test/intent/fb_analysis_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/test/intent/fb_diff_intent_test.py` & `discovery-capability-0.4.9/test/intent/fb_diff_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/test/intent/fb_intent_test.py` & `discovery-capability-0.4.9/test/intent/fb_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.4.8/test/intent/fb_model_intent_test.py` & `discovery-capability-0.4.9/test/intent/fb_model_intent_test.py`

 * *Files identical despite different names*

