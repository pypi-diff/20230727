# Comparing `tmp/OpenFisca-France-Data-1.3.1.tar.gz` & `tmp/OpenFisca-France-Data-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-France-Data-1.3.1.tar", last modified: Fri Jul 21 13:51:25 2023, max compression
+gzip compressed data, was "OpenFisca-France-Data-2.0.0.tar", last modified: Thu Jul 27 07:48:19 2023, max compression
```

## Comparing `OpenFisca-France-Data-1.3.1.tar` & `OpenFisca-France-Data-2.0.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.024824 OpenFisca-France-Data-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.016824 OpenFisca-France-Data-1.3.1/OpenFisca_France_Data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11506 2023-07-21 13:51:24.000000 OpenFisca-France-Data-1.3.1/OpenFisca_France_Data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4229 2023-07-21 13:51:25.000000 OpenFisca-France-Data-1.3.1/OpenFisca_France_Data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 13:51:24.000000 OpenFisca-France-Data-1.3.1/OpenFisca_France_Data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-07-21 13:51:24.000000 OpenFisca-France-Data-1.3.1/OpenFisca_France_Data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      373 2023-07-21 13:51:24.000000 OpenFisca-France-Data-1.3.1/OpenFisca_France_Data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-07-21 13:51:24.000000 OpenFisca-France-Data-1.3.1/OpenFisca_France_Data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11506 2023-07-21 13:51:25.024824 OpenFisca-France-Data-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10702 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.016824 OpenFisca-France-Data-1.3.1/openfisca_france_data/
--rw-r--r--   0 runner    (1001) docker     (122)     7682 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4356 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/aggregates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.016824 OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.012823 OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/aggregats/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.016824 OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/aggregats/ines/
--rw-r--r--   0 runner    (1001) docker     (122)     4940 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/aggregats/ines/ines_2019.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.016824 OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/aggregats/taxipp/
--rw-r--r--   0 runner    (1001) docker     (122)    12991 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.016824 OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/zone_apl_data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/zone_apl_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/zone_apl_data/codeAplReader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.016824 OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/zone_apl_data/zone_apl/
--rw-r--r--   0 runner    (1001) docker     (122)      502 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/zone_apl_data/zone_apl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/base_survey.py
--rw-r--r--   0 runner    (1001) docker     (122)    21046 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/common.py
--rw-r--r--   0 runner    (1001) docker     (122)    24951 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/comparator.py
--rw-r--r--   0 runner    (1001) docker     (122)      996 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.012823 OpenFisca-France-Data-1.3.1/openfisca_france_data/dads/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.016824 OpenFisca-France-Data-1.3.1/openfisca_france_data/dads/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/dads/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.016824 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/
--rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.020824 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2637 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/run_all.py
--rw-r--r--   0 runner    (1001) docker     (122)     8932 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py
--rw-r--r--   0 runner    (1001) docker     (122)    21783 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11919 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_03_fip.py
--rw-r--r--   0 runner    (1001) docker     (122)    26165 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_04_famille.py
--rw-r--r--   0 runner    (1001) docker     (122)    13995 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py
--rw-r--r--   0 runner    (1001) docker     (122)    36615 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py
--rw-r--r--   0 runner    (1001) docker     (122)     8399 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py
--rw-r--r--   0 runner    (1001) docker     (122)    13216 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_08_final.py
--rw-r--r--   0 runner    (1001) docker     (122)     1536 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.020824 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/old/
--rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/old/aggregates.py
--rw-r--r--   0 runner    (1001) docker     (122)    19211 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/old/datatable.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.020824 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4805 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/comparison.py
--rw-r--r--   0 runner    (1001) docker     (122)     7108 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/get_survey_scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.020824 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)     6660 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15394 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (122)    25444 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
--rw-r--r--   0 runner    (1001) docker     (122)    45059 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
--rw-r--r--   0 runner    (1001) docker     (122)    35127 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
--rw-r--r--   0 runner    (1001) docker     (122)    10755 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
--rw-r--r--   0 runner    (1001) docker     (122)     2286 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     5791 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/test_case_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.012823 OpenFisca-France-Data-1.3.1/openfisca_france_data/felin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.020824 OpenFisca-France-Data-1.3.1/openfisca_france_data/felin/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/felin/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1869 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.020824 OpenFisca-France-Data-1.3.1/openfisca_france_data/model/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      541 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/model/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     8882 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/model/calage.py
--rw-r--r--   0 runner    (1001) docker     (122)    11373 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/model/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/model/id_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/model/survey_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.020824 OpenFisca-France-Data-1.3.1/openfisca_france_data/reforms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12440 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/reforms/inversion_directe_salaires.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.020824 OpenFisca-France-Data-1.3.1/openfisca_france_data/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/scripts/build_input_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6701 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/smic.py
--rw-r--r--   0 runner    (1001) docker     (122)     7052 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)    15060 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/openfisca_france_data/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-07-21 13:51:25.024824 OpenFisca-France-Data-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2425 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.024824 OpenFisca-France-Data-1.3.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.012823 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.024824 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/
--rw-r--r--   0 runner    (1001) docker     (122)     2466 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_af.py
--rw-r--r--   0 runner    (1001) docker     (122)     8456 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_al.py
--rw-r--r--   0 runner    (1001) docker     (122)    10685 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_create_salaire_de_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_impot_revenu.py
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_inflation.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_input_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_pivot_table.py
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_rebuild_input_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_rsa.py
--rw-r--r--   0 runner    (1001) docker     (122)     1532 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_salaire_imposable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:51:25.024824 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/unit/
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/unit/test_get_survey_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/erfs_fpr/unit/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/test_fake_survey_simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/test_get_baremes_salarie.py
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-07-21 13:50:59.000000 OpenFisca-France-Data-1.3.1/tests/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.343474 OpenFisca-France-Data-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11392 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.335474 OpenFisca-France-Data-2.0.0/OpenFisca_France_Data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11608 2023-07-27 07:48:19.000000 OpenFisca-France-Data-2.0.0/OpenFisca_France_Data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4229 2023-07-27 07:48:19.000000 OpenFisca-France-Data-2.0.0/OpenFisca_France_Data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 07:48:19.000000 OpenFisca-France-Data-2.0.0/OpenFisca_France_Data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-07-27 07:48:19.000000 OpenFisca-France-Data-2.0.0/OpenFisca_France_Data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-07-27 07:48:19.000000 OpenFisca-France-Data-2.0.0/OpenFisca_France_Data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-07-27 07:48:19.000000 OpenFisca-France-Data-2.0.0/OpenFisca_France_Data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    11608 2023-07-27 07:48:19.343474 OpenFisca-France-Data-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10702 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.335474 OpenFisca-France-Data-2.0.0/openfisca_france_data/
+-rw-r--r--   0 runner    (1001) docker     (122)     7682 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4356 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/aggregates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.335474 OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.331474 OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/aggregats/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.335474 OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/aggregats/ines/
+-rw-r--r--   0 runner    (1001) docker     (122)     4940 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/aggregats/ines/ines_2019.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.335474 OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/aggregats/taxipp/
+-rw-r--r--   0 runner    (1001) docker     (122)    12991 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.335474 OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/zone_apl_data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/zone_apl_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/zone_apl_data/codeAplReader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.335474 OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/zone_apl_data/zone_apl/
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/zone_apl_data/zone_apl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/base_survey.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21046 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24951 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      996 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.331474 OpenFisca-France-Data-2.0.0/openfisca_france_data/dads/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.335474 OpenFisca-France-Data-2.0.0/openfisca_france_data/dads/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/dads/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.339474 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.339474 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2637 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8932 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21783 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11919 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26165 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13995 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36615 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8399 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13216 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1536 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.339474 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/old/
+-rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/old/aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19211 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/old/datatable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.339474 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4805 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7108 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.339474 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)     6660 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15394 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25444 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45059 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35127 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10755 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2286 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5791 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/test_case_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.331474 OpenFisca-France-Data-2.0.0/openfisca_france_data/felin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.339474 OpenFisca-France-Data-2.0.0/openfisca_france_data/felin/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/felin/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1869 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.343474 OpenFisca-France-Data-2.0.0/openfisca_france_data/model/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      541 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8882 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/model/calage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11373 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/model/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/model/id_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/model/survey_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.343474 OpenFisca-France-Data-2.0.0/openfisca_france_data/reforms/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12440 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/reforms/inversion_directe_salaires.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.343474 OpenFisca-France-Data-2.0.0/openfisca_france_data/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/scripts/build_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6701 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/smic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7052 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15060 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/openfisca_france_data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-07-27 07:48:19.343474 OpenFisca-France-Data-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2525 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.343474 OpenFisca-France-Data-2.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.335474 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.343474 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)     2466 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_af.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8456 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_al.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10685 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_impot_revenu.py
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_input_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_pivot_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_rebuild_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1532 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_salaire_imposable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:48:19.343474 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/unit/test_get_survey_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/erfs_fpr/unit/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/test_fake_survey_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/test_get_baremes_salarie.py
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-07-27 07:47:53.000000 OpenFisca-France-Data-2.0.0/tests/test_misc.py
```

### Comparing `OpenFisca-France-Data-1.3.1/CHANGELOG.md` & `OpenFisca-France-Data-2.0.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 
+# 2.0.0 [#229](https://github.com/openfisca/openfisca-france-data/pull/229)
+* Technical changes
+- Met à jour Python dans le setup pour compatibilité conda
+
 # 1.3.1 [#228](https://github.com/openfisca/openfisca-france-data/pull/228)
 * Technical changes
-- Ajoute de deux jeux de données utilisées pour les tests au paquet : 
-    -  'assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx' 
+- Ajout de deux jeux de données utilisées pour les tests au paquet :
+    -  'assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx'
     - `'assets/aggregats/ines/ines_2019.json'
 
 # 1.3.0 [#227](https://github.com/openfisca/openfisca-france-data/pull/227)
 * Technical changes
 - Adapte le comparator pour effectuer plus de tests en distribution
 - Permet l'utilisation d'un SurveyScenario facilement personnalisable
```

### Comparing `OpenFisca-France-Data-1.3.1/CONTRIBUTING.md` & `OpenFisca-France-Data-2.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/LICENSE` & `OpenFisca-France-Data-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/OpenFisca_France_Data.egg-info/PKG-INFO` & `OpenFisca-France-Data-2.0.0/OpenFisca_France_Data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: OpenFisca-France-Data
-Version: 1.3.1
+Version: 2.0.0
 Summary: OpenFisca-France-Data module to work with French survey data
 Home-page: https://github.com/openfisca/openfisca-france-data
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit social survey data microsimulation
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >= 3.7
+Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # OpenFisca France Data
 
 [![Newsletter](https://img.shields.io/badge/newsletter-subscribe!-informational.svg?style=flat)](mailto:contact%40openfisca.org?subject=Subscribe%20to%20your%20newsletter%20%7C%20S'inscrire%20%C3%A0%20votre%20newsletter&body=%5BEnglish%20version%20below%5D%0A%0ABonjour%2C%0A%0AVotre%C2%A0pr%C3%A9sence%C2%A0ici%C2%A0nous%C2%A0ravit%C2%A0!%20%F0%9F%98%83%0A%0AEnvoyez-nous%20cet%20email%20pour%20que%20l'on%20puisse%20vous%20inscrire%20%C3%A0%20la%20newsletter.%20%0A%0AAh%C2%A0!%20Et%20si%20vous%20pouviez%20remplir%20ce%20petit%20questionnaire%2C%20%C3%A7a%20serait%20encore%20mieux%C2%A0!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2F45M0VR1TYKD1RGzX2%0A%0AAmiti%C3%A9%2C%0AL%E2%80%99%C3%A9quipe%20OpenFisca%0A%0A%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%20ENGLISH%20VERSION%20%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%0A%0AHi%2C%20%0A%0AWe're%20glad%20to%20see%20you%20here!%20%F0%9F%98%83%0A%0APlease%20send%20us%20this%20email%2C%20so%20we%20can%20subscribe%20you%20to%20the%20newsletter.%0A%0AAlso%2C%20if%20you%20can%20fill%20out%20this%20short%20survey%2C%20even%20better!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2FsOg8K1abhhm441LG2%0A%0ACheers%2C%0AThe%20OpenFisca%20Team)
```

### Comparing `OpenFisca-France-Data-1.3.1/OpenFisca_France_Data.egg-info/SOURCES.txt` & `OpenFisca-France-Data-2.0.0/OpenFisca_France_Data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/PKG-INFO` & `OpenFisca-France-Data-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: OpenFisca-France-Data
-Version: 1.3.1
+Version: 2.0.0
 Summary: OpenFisca-France-Data module to work with French survey data
 Home-page: https://github.com/openfisca/openfisca-france-data
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit social survey data microsimulation
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >= 3.7
+Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # OpenFisca France Data
 
 [![Newsletter](https://img.shields.io/badge/newsletter-subscribe!-informational.svg?style=flat)](mailto:contact%40openfisca.org?subject=Subscribe%20to%20your%20newsletter%20%7C%20S'inscrire%20%C3%A0%20votre%20newsletter&body=%5BEnglish%20version%20below%5D%0A%0ABonjour%2C%0A%0AVotre%C2%A0pr%C3%A9sence%C2%A0ici%C2%A0nous%C2%A0ravit%C2%A0!%20%F0%9F%98%83%0A%0AEnvoyez-nous%20cet%20email%20pour%20que%20l'on%20puisse%20vous%20inscrire%20%C3%A0%20la%20newsletter.%20%0A%0AAh%C2%A0!%20Et%20si%20vous%20pouviez%20remplir%20ce%20petit%20questionnaire%2C%20%C3%A7a%20serait%20encore%20mieux%C2%A0!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2F45M0VR1TYKD1RGzX2%0A%0AAmiti%C3%A9%2C%0AL%E2%80%99%C3%A9quipe%20OpenFisca%0A%0A%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%20ENGLISH%20VERSION%20%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%0A%0AHi%2C%20%0A%0AWe're%20glad%20to%20see%20you%20here!%20%F0%9F%98%83%0A%0APlease%20send%20us%20this%20email%2C%20so%20we%20can%20subscribe%20you%20to%20the%20newsletter.%0A%0AAlso%2C%20if%20you%20can%20fill%20out%20this%20short%20survey%2C%20even%20better!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2FsOg8K1abhhm441LG2%0A%0ACheers%2C%0AThe%20OpenFisca%20Team)
```

### Comparing `OpenFisca-France-Data-1.3.1/README.md` & `OpenFisca-France-Data-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/__init__.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/aggregates.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/aggregats/ines/ines_2019.json` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/aggregats/ines/ines_2019.json`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/base_survey.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/base_survey.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/common.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/common.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/comparator.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/comparator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/config.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/config.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/__init__.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/__init__.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/base.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/base.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/run_all.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/run_all.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_03_fip.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_04_famille.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_08_final.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/old/aggregates.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/old/aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/old/datatable.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/old/datatable.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs/scenario.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs/scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/comparison.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/comparison.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/get_survey_scenario.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/scenario.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/erfs_fpr/test_case_creation.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/erfs_fpr/test_case_creation.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/model/base.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/model/base.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/model/calage.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/model/calage.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/model/common.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/model/common.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/model/id_variables.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/model/id_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/model/survey_variables.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/model/survey_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/reforms/inversion_directe_salaires.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/reforms/inversion_directe_salaires.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/scripts/build_input_data.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/scripts/build_input_data.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/smic.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/smic.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/surveys.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/openfisca_france_data/utils.py` & `OpenFisca-France-Data-2.0.0/openfisca_france_data/utils.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/setup.cfg` & `OpenFisca-France-Data-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/setup.py` & `OpenFisca-France-Data-2.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,48 +2,50 @@
 
 
 with open('README.md') as file:
     long_description = file.read()
 
 setup(
     name = "OpenFisca-France-Data",
-    version = "1.3.1",
+    version = "2.0.0",
     description = "OpenFisca-France-Data module to work with French survey data",
     long_description = long_description,
     long_description_content_type="text/markdown",
     author = "OpenFisca Team",
     author_email = "contact@openfisca.fr",
     url = "https://github.com/openfisca/openfisca-france-data",
     license = "http://www.fsf.org/licensing/licenses/agpl-3.0.html",
     keywords = "tax benefit social survey data microsimulation",
     classifiers = [
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Information Analysis",
         ],
     package_data = {
         'openfisca_france_data': ['assets/aggregats/taxipp/agregats_tests_taxipp_2_0.xlsx',
                                   'assets/aggregats/ines/ines_2019.json'],
         },
     entry_points = {
         'console_scripts': [
             'build-erfs-fpr=openfisca_france_data.erfs_fpr.input_data_builder:main',
             'compare-erfs-fpr-input=openfisca_france_data.erfs_fpr.comparison:compare',
             'create-test-erfs-fpr=openfisca_france_data.erfs_fpr.test_case_creation:create_test',
             ],
         },
-    python_requires = ">= 3.7",
+    python_requires = ">= 3.9",
     install_requires = [
         "click >= 8.0.0, < 9.0.0",
         "matplotlib >= 3.1.1, < 4.0.0",
         "multipledispatch >= 0.6.0, < 1.0.0",
-        "openFisca-france >= 149.0.0, < 150.0.0",
+        "openFisca-france >= 150.0.0, < 151.0.0",
         "openFisca-survey-manager >= 1, < 2.0.0",
         "wquantiles >= 0.3.0, < 1.0.0",  # To compute weighted quantiles
         ],
     extras_require = {
         "test": [
             "autopep8 >= 1.4.0, < 1.5.0",
             "bumpver >= 2022.1120",
```

### Comparing `OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_af.py` & `OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_af.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_aggregates.py` & `OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_al.py` & `OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_al.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_create_salaire_de_base.py` & `OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_impot_revenu.py` & `OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_impot_revenu.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_inflation.py` & `OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_inflation.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_input_variables.py` & `OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_input_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_pivot_table.py` & `OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_pivot_table.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_rebuild_input_data.py` & `OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_rebuild_input_data.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_rsa.py` & `OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_rsa.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/erfs_fpr/integration/test_salaire_imposable.py` & `OpenFisca-France-Data-2.0.0/tests/erfs_fpr/integration/test_salaire_imposable.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/erfs_fpr/unit/test_get_survey_scenario.py` & `OpenFisca-France-Data-2.0.0/tests/erfs_fpr/unit/test_get_survey_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/test_aggregate.py` & `OpenFisca-France-Data-2.0.0/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/test_calibration.py` & `OpenFisca-France-Data-2.0.0/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/test_fake_survey_simulation.py` & `OpenFisca-France-Data-2.0.0/tests/test_fake_survey_simulation.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/test_get_baremes_salarie.py` & `OpenFisca-France-Data-2.0.0/tests/test_get_baremes_salarie.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.3.1/tests/test_misc.py` & `OpenFisca-France-Data-2.0.0/tests/test_misc.py`

 * *Files identical despite different names*

