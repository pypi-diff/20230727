# Comparing `tmp/spd_eda-0.1.2.tar.gz` & `tmp/spd_eda-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spd_eda-0.1.2.tar", last modified: Fri Jul 21 13:41:40 2023, max compression
+gzip compressed data, was "spd_eda-0.1.3.tar", last modified: Thu Jul 27 14:25:12 2023, max compression
```

## Comparing `spd_eda-0.1.2.tar` & `spd_eda-0.1.3.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:40.011090 spd_eda-0.1.2/
--rw-rw-rw-   0        0        0        0 2022-09-08 20:28:11.000000 spd_eda-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       60 2023-07-21 13:41:10.000000 spd_eda-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     9679 2023-07-21 13:41:40.009455 spd_eda-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     9316 2022-10-20 20:56:07.000000 spd_eda-0.1.2/README.md
--rw-rw-rw-   0        0        0      661 2023-07-21 13:41:20.000000 spd_eda-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-21 13:41:40.011677 spd_eda-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:39.822182 spd_eda-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:39.843975 spd_eda-0.1.2/src/spd_eda/
--rw-rw-rw-   0        0        0      931 2023-07-19 19:06:53.000000 spd_eda-0.1.2/src/spd_eda/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:39.870860 spd_eda-0.1.2/src/spd_eda/athena_tools/
--rw-rw-rw-   0        0        0        0 2022-09-12 18:57:01.000000 spd_eda-0.1.2/src/spd_eda/athena_tools/__init__.py
--rw-rw-rw-   0        0        0     6643 2022-09-12 19:03:47.000000 spd_eda-0.1.2/src/spd_eda/athena_tools/athena_column.py
--rw-rw-rw-   0        0        0     9407 2022-09-13 16:49:56.000000 spd_eda-0.1.2/src/spd_eda/athena_tools/athena_table.py
--rw-rw-rw-   0        0        0      380 2022-09-12 19:03:47.000000 spd_eda-0.1.2/src/spd_eda/athena_tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:39.876231 spd_eda-0.1.2/src/spd_eda/dataframe_structure/
--rw-rw-rw-   0        0        0        0 2023-07-19 14:01:10.000000 spd_eda-0.1.2/src/spd_eda/dataframe_structure/__init__.py
--rw-rw-rw-   0        0        0      891 2023-07-19 14:05:46.000000 spd_eda-0.1.2/src/spd_eda/dataframe_structure/dataframe_structure.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:39.881183 spd_eda-0.1.2/src/spd_eda/eda_tools/
--rw-rw-rw-   0        0        0        0 2022-09-08 18:55:20.000000 spd_eda-0.1.2/src/spd_eda/eda_tools/__init__.py
--rw-rw-rw-   0        0        0     9394 2023-02-01 17:37:20.000000 spd_eda-0.1.2/src/spd_eda/eda_tools/eda.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:39.887186 spd_eda-0.1.2/src/spd_eda/excel_tools/
--rw-rw-rw-   0        0        0        0 2022-09-08 19:22:51.000000 spd_eda-0.1.2/src/spd_eda/excel_tools/__init__.py
--rw-rw-rw-   0        0        0     7411 2022-10-24 16:58:22.000000 spd_eda-0.1.2/src/spd_eda/excel_tools/excel_output.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:39.901004 spd_eda-0.1.2/src/spd_eda/hh_batch/
--rw-rw-rw-   0        0        0      124 2023-07-19 19:10:06.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/__init__.py
--rw-rw-rw-   0        0        0     6894 2023-07-19 19:11:26.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/api_batch.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:39.923429 spd_eda-0.1.2/src/spd_eda/hh_batch/config/
--rw-rw-rw-   0        0        0        0 2023-05-09 14:29:38.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/config/__init__.py
--rw-rw-rw-   0        0        0     6287 2023-06-12 21:00:40.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/config/base_report_config.csv
--rw-rw-rw-   0        0        0    73110 2023-04-20 18:39:58.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/config/batch_column_config.csv
--rw-rw-rw-   0        0        0    35195 2023-06-12 21:03:11.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/config/batch_data_dictionary.csv
--rw-rw-rw-   0        0        0    18723 2023-07-05 16:34:04.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/config/config.py
--rw-rw-rw-   0        0        0     9320 2023-07-19 19:13:44.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/portfolio_analysis.py
--rw-rw-rw-   0        0        0    13934 2023-07-21 13:34:31.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/report.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:39.929432 spd_eda-0.1.2/src/spd_eda/hh_batch/tests/
--rw-rw-rw-   0        0        0        0 2023-06-12 21:21:53.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/tests/__init__.py
--rw-rw-rw-   0        0        0      424 2023-06-12 21:25:27.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/tests/scratch.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:39.947597 spd_eda-0.1.2/src/spd_eda/hh_batch/utils/
--rw-rw-rw-   0        0        0        0 2023-04-28 18:01:54.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/utils/__init__.py
--rw-rw-rw-   0        0        0     2139 2023-05-04 14:43:39.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/utils/binning_utils.py
--rw-rw-rw-   0        0        0      473 2023-05-01 18:44:46.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/utils/chart_utils.py
--rw-rw-rw-   0        0        0     7692 2023-05-31 18:42:16.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/utils/excel_utils.py
--rw-rw-rw-   0        0        0      591 2023-05-01 18:03:50.000000 spd_eda-0.1.2/src/spd_eda/hh_batch/utils/stat_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:39.951313 spd_eda-0.1.2/src/spd_eda/modeling/
--rw-rw-rw-   0        0        0       69 2023-07-19 17:24:49.000000 spd_eda-0.1.2/src/spd_eda/modeling/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:39.956324 spd_eda-0.1.2/src/spd_eda/modeling/utils/
--rw-rw-rw-   0        0        0        0 2023-06-20 19:12:15.000000 spd_eda-0.1.2/src/spd_eda/modeling/utils/__init__.py
--rw-rw-rw-   0        0        0     1915 2023-07-19 17:24:49.000000 spd_eda-0.1.2/src/spd_eda/modeling/utils/binning_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:39.991110 spd_eda-0.1.2/src/spd_eda/pa/
--rw-rw-rw-   0        0        0        0 2022-09-09 17:04:23.000000 spd_eda-0.1.2/src/spd_eda/pa/__init__.py
--rw-rw-rw-   0        0        0    38969 2022-09-15 14:49:00.000000 spd_eda-0.1.2/src/spd_eda/pa/analysis.py
--rw-rw-rw-   0        0        0     1993 2022-09-26 15:12:59.000000 spd_eda-0.1.2/src/spd_eda/pa/analysis_summary.py
--rw-rw-rw-   0        0        0     1218 2022-09-15 14:49:00.000000 spd_eda-0.1.2/src/spd_eda/pa/config.py
--rw-rw-rw-   0        0        0      241 2022-09-09 17:05:24.000000 spd_eda-0.1.2/src/spd_eda/pa/connection.py
--rw-rw-rw-   0        0        0     5615 2022-09-09 17:34:27.000000 spd_eda-0.1.2/src/spd_eda/pa/datasource.py
--rw-rw-rw-   0        0        0     3225 2022-09-09 17:34:27.000000 spd_eda-0.1.2/src/spd_eda/pa/dataview.py
--rw-rw-rw-   0        0        0    18925 2022-09-13 14:22:51.000000 spd_eda-0.1.2/src/spd_eda/pa/dataview_eda.py
--rw-rw-rw-   0        0        0    17580 2022-09-15 14:49:00.000000 spd_eda-0.1.2/src/spd_eda/pa/pa_stats.py
--rw-rw-rw-   0        0        0     5041 2022-09-14 15:46:48.000000 spd_eda-0.1.2/src/spd_eda/pa/plinko.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:40.005111 spd_eda-0.1.2/src/spd_eda/sql_tools/
--rw-rw-rw-   0        0        0        0 2022-09-12 19:35:04.000000 spd_eda-0.1.2/src/spd_eda/sql_tools/__init__.py
--rw-rw-rw-   0        0        0      241 2022-09-12 19:47:52.000000 spd_eda-0.1.2/src/spd_eda/sql_tools/connection.py
--rw-rw-rw-   0        0        0     4858 2022-09-12 20:38:00.000000 spd_eda-0.1.2/src/spd_eda/sql_tools/sql_table.py
--rw-rw-rw-   0        0        0      253 2022-09-12 19:53:22.000000 spd_eda-0.1.2/src/spd_eda/sql_tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:41:39.858595 spd_eda-0.1.2/src/spd_eda.egg-info/
--rw-rw-rw-   0        0        0     9679 2023-07-21 13:41:39.000000 spd_eda-0.1.2/src/spd_eda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1829 2023-07-21 13:41:39.000000 spd_eda-0.1.2/src/spd_eda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 13:41:39.000000 spd_eda-0.1.2/src/spd_eda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2023-07-21 13:41:39.000000 spd_eda-0.1.2/src/spd_eda.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-21 13:41:39.000000 spd_eda-0.1.2/src/spd_eda.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.647568 spd_eda-0.1.3/
+-rw-rw-rw-   0        0        0        0 2022-09-08 20:28:11.000000 spd_eda-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      104 2023-07-27 14:24:52.000000 spd_eda-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     9679 2023-07-27 14:25:12.645568 spd_eda-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9316 2022-10-20 20:56:07.000000 spd_eda-0.1.3/README.md
+-rw-rw-rw-   0        0        0      661 2023-07-27 14:24:52.000000 spd_eda-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 14:25:12.648569 spd_eda-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.438547 spd_eda-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.461548 spd_eda-0.1.3/src/spd_eda/
+-rw-rw-rw-   0        0        0      931 2023-07-19 19:06:53.000000 spd_eda-0.1.3/src/spd_eda/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.494552 spd_eda-0.1.3/src/spd_eda/athena_tools/
+-rw-rw-rw-   0        0        0        0 2022-09-12 18:57:01.000000 spd_eda-0.1.3/src/spd_eda/athena_tools/__init__.py
+-rw-rw-rw-   0        0        0     6643 2022-09-12 19:03:47.000000 spd_eda-0.1.3/src/spd_eda/athena_tools/athena_column.py
+-rw-rw-rw-   0        0        0     9407 2022-09-13 16:49:56.000000 spd_eda-0.1.3/src/spd_eda/athena_tools/athena_table.py
+-rw-rw-rw-   0        0        0      380 2022-09-12 19:03:47.000000 spd_eda-0.1.3/src/spd_eda/athena_tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.500553 spd_eda-0.1.3/src/spd_eda/dataframe_structure/
+-rw-rw-rw-   0        0        0        0 2023-07-19 14:01:10.000000 spd_eda-0.1.3/src/spd_eda/dataframe_structure/__init__.py
+-rw-rw-rw-   0        0        0      891 2023-07-19 14:05:46.000000 spd_eda-0.1.3/src/spd_eda/dataframe_structure/dataframe_structure.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.506549 spd_eda-0.1.3/src/spd_eda/eda_tools/
+-rw-rw-rw-   0        0        0        0 2022-09-08 18:55:20.000000 spd_eda-0.1.3/src/spd_eda/eda_tools/__init__.py
+-rw-rw-rw-   0        0        0     9394 2023-02-01 17:37:20.000000 spd_eda-0.1.3/src/spd_eda/eda_tools/eda.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.513547 spd_eda-0.1.3/src/spd_eda/excel_tools/
+-rw-rw-rw-   0        0        0        0 2022-09-08 19:22:51.000000 spd_eda-0.1.3/src/spd_eda/excel_tools/__init__.py
+-rw-rw-rw-   0        0        0     7411 2022-10-24 16:58:22.000000 spd_eda-0.1.3/src/spd_eda/excel_tools/excel_output.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.528551 spd_eda-0.1.3/src/spd_eda/hh_batch/
+-rw-rw-rw-   0        0        0      124 2023-07-19 19:10:06.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/__init__.py
+-rw-rw-rw-   0        0        0     6894 2023-07-19 19:11:26.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/api_batch.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.555552 spd_eda-0.1.3/src/spd_eda/hh_batch/config/
+-rw-rw-rw-   0        0        0        0 2023-05-09 14:29:38.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/config/__init__.py
+-rw-rw-rw-   0        0        0     6287 2023-06-12 21:00:40.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/config/base_report_config.csv
+-rw-rw-rw-   0        0        0    73110 2023-04-20 18:39:58.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/config/batch_column_config.csv
+-rw-rw-rw-   0        0        0    35195 2023-06-12 21:03:11.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/config/batch_data_dictionary.csv
+-rw-rw-rw-   0        0        0    18723 2023-07-05 16:34:04.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/config/config.py
+-rw-rw-rw-   0        0        0    12764 2023-06-12 21:05:37.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/config/report_translation_tables.xlsx
+-rw-rw-rw-   0        0        0     9320 2023-07-19 19:13:44.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/portfolio_analysis.py
+-rw-rw-rw-   0        0        0    13934 2023-07-21 13:34:31.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/report.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.561554 spd_eda-0.1.3/src/spd_eda/hh_batch/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-12 21:21:53.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/tests/__init__.py
+-rw-rw-rw-   0        0        0      424 2023-06-12 21:25:27.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/tests/scratch.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.579567 spd_eda-0.1.3/src/spd_eda/hh_batch/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-28 18:01:54.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/utils/__init__.py
+-rw-rw-rw-   0        0        0     2139 2023-05-04 14:43:39.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/utils/binning_utils.py
+-rw-rw-rw-   0        0        0      473 2023-05-01 18:44:46.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/utils/chart_utils.py
+-rw-rw-rw-   0        0        0     7692 2023-05-31 18:42:16.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/utils/excel_utils.py
+-rw-rw-rw-   0        0        0      591 2023-05-01 18:03:50.000000 spd_eda-0.1.3/src/spd_eda/hh_batch/utils/stat_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.583564 spd_eda-0.1.3/src/spd_eda/modeling/
+-rw-rw-rw-   0        0        0       69 2023-07-19 17:24:49.000000 spd_eda-0.1.3/src/spd_eda/modeling/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.588565 spd_eda-0.1.3/src/spd_eda/modeling/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-20 19:12:15.000000 spd_eda-0.1.3/src/spd_eda/modeling/utils/__init__.py
+-rw-rw-rw-   0        0        0     1915 2023-07-19 17:24:49.000000 spd_eda-0.1.3/src/spd_eda/modeling/utils/binning_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.628568 spd_eda-0.1.3/src/spd_eda/pa/
+-rw-rw-rw-   0        0        0        0 2022-09-09 17:04:23.000000 spd_eda-0.1.3/src/spd_eda/pa/__init__.py
+-rw-rw-rw-   0        0        0    38969 2022-09-15 14:49:00.000000 spd_eda-0.1.3/src/spd_eda/pa/analysis.py
+-rw-rw-rw-   0        0        0     1993 2022-09-26 15:12:59.000000 spd_eda-0.1.3/src/spd_eda/pa/analysis_summary.py
+-rw-rw-rw-   0        0        0     1218 2022-09-15 14:49:00.000000 spd_eda-0.1.3/src/spd_eda/pa/config.py
+-rw-rw-rw-   0        0        0      241 2022-09-09 17:05:24.000000 spd_eda-0.1.3/src/spd_eda/pa/connection.py
+-rw-rw-rw-   0        0        0     5615 2022-09-09 17:34:27.000000 spd_eda-0.1.3/src/spd_eda/pa/datasource.py
+-rw-rw-rw-   0        0        0     3225 2022-09-09 17:34:27.000000 spd_eda-0.1.3/src/spd_eda/pa/dataview.py
+-rw-rw-rw-   0        0        0    18925 2022-09-13 14:22:51.000000 spd_eda-0.1.3/src/spd_eda/pa/dataview_eda.py
+-rw-rw-rw-   0        0        0    17580 2022-09-15 14:49:00.000000 spd_eda-0.1.3/src/spd_eda/pa/pa_stats.py
+-rw-rw-rw-   0        0        0     5041 2022-09-14 15:46:48.000000 spd_eda-0.1.3/src/spd_eda/pa/plinko.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.642563 spd_eda-0.1.3/src/spd_eda/sql_tools/
+-rw-rw-rw-   0        0        0        0 2022-09-12 19:35:04.000000 spd_eda-0.1.3/src/spd_eda/sql_tools/__init__.py
+-rw-rw-rw-   0        0        0      241 2022-09-12 19:47:52.000000 spd_eda-0.1.3/src/spd_eda/sql_tools/connection.py
+-rw-rw-rw-   0        0        0     4858 2022-09-12 20:38:00.000000 spd_eda-0.1.3/src/spd_eda/sql_tools/sql_table.py
+-rw-rw-rw-   0        0        0      253 2022-09-12 19:53:22.000000 spd_eda-0.1.3/src/spd_eda/sql_tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:25:12.479547 spd_eda-0.1.3/src/spd_eda.egg-info/
+-rw-rw-rw-   0        0        0     9679 2023-07-27 14:25:12.000000 spd_eda-0.1.3/src/spd_eda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1888 2023-07-27 14:25:12.000000 spd_eda-0.1.3/src/spd_eda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 14:25:12.000000 spd_eda-0.1.3/src/spd_eda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2023-07-27 14:25:12.000000 spd_eda-0.1.3/src/spd_eda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-27 14:25:12.000000 spd_eda-0.1.3/src/spd_eda.egg-info/top_level.txt
```

### Comparing `spd_eda-0.1.2/PKG-INFO` & `spd_eda-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spd_eda
-Version: 0.1.2
+Version: 0.1.3
 Summary: initial testing
 Author-email: sdooley <author@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `spd_eda-0.1.2/README.md` & `spd_eda-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/pyproject.toml` & `spd_eda-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2273 7064 5f65 6461 220d 0a76 6572  = "spd_eda"..ver
-00000020: 7369 6f6e 203d 2022 302e 312e 3222 0d0a  sion = "0.1.2"..
+00000020: 7369 6f6e 203d 2022 302e 312e 3322 0d0a  sion = "0.1.3"..
 00000030: 6175 7468 6f72 7320 3d20 5b0d 0a20 207b  authors = [..  {
 00000040: 206e 616d 653d 2273 646f 6f6c 6579 222c   name="sdooley",
 00000050: 2065 6d61 696c 3d22 6175 7468 6f72 4065   email="author@e
 00000060: 7861 6d70 6c65 2e63 6f6d 2220 7d2c 0d0a  xample.com" },..
 00000070: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
 00000080: 2022 696e 6974 6961 6c20 7465 7374 696e   "initial testin
 00000090: 6722 0d0a 7265 6164 6d65 203d 2022 5245  g"..readme = "RE
```

### Comparing `spd_eda-0.1.2/src/spd_eda/__init__.py` & `spd_eda-0.1.3/src/spd_eda/__init__.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/athena_tools/athena_column.py` & `spd_eda-0.1.3/src/spd_eda/athena_tools/athena_column.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/athena_tools/athena_table.py` & `spd_eda-0.1.3/src/spd_eda/athena_tools/athena_table.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/dataframe_structure/dataframe_structure.py` & `spd_eda-0.1.3/src/spd_eda/dataframe_structure/dataframe_structure.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/eda_tools/eda.py` & `spd_eda-0.1.3/src/spd_eda/eda_tools/eda.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/excel_tools/excel_output.py` & `spd_eda-0.1.3/src/spd_eda/excel_tools/excel_output.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/hh_batch/api_batch.py` & `spd_eda-0.1.3/src/spd_eda/hh_batch/api_batch.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/hh_batch/config/base_report_config.csv` & `spd_eda-0.1.3/src/spd_eda/hh_batch/config/base_report_config.csv`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/hh_batch/config/batch_column_config.csv` & `spd_eda-0.1.3/src/spd_eda/hh_batch/config/batch_column_config.csv`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/hh_batch/config/batch_data_dictionary.csv` & `spd_eda-0.1.3/src/spd_eda/hh_batch/config/batch_data_dictionary.csv`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/hh_batch/config/config.py` & `spd_eda-0.1.3/src/spd_eda/hh_batch/config/config.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/hh_batch/portfolio_analysis.py` & `spd_eda-0.1.3/src/spd_eda/hh_batch/portfolio_analysis.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/hh_batch/report.py` & `spd_eda-0.1.3/src/spd_eda/hh_batch/report.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/hh_batch/utils/binning_utils.py` & `spd_eda-0.1.3/src/spd_eda/hh_batch/utils/binning_utils.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/hh_batch/utils/excel_utils.py` & `spd_eda-0.1.3/src/spd_eda/hh_batch/utils/excel_utils.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/hh_batch/utils/stat_utils.py` & `spd_eda-0.1.3/src/spd_eda/hh_batch/utils/stat_utils.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/modeling/utils/binning_utils.py` & `spd_eda-0.1.3/src/spd_eda/modeling/utils/binning_utils.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/pa/analysis.py` & `spd_eda-0.1.3/src/spd_eda/pa/analysis.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/pa/analysis_summary.py` & `spd_eda-0.1.3/src/spd_eda/pa/analysis_summary.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/pa/config.py` & `spd_eda-0.1.3/src/spd_eda/pa/config.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/pa/datasource.py` & `spd_eda-0.1.3/src/spd_eda/pa/datasource.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/pa/dataview.py` & `spd_eda-0.1.3/src/spd_eda/pa/dataview.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/pa/dataview_eda.py` & `spd_eda-0.1.3/src/spd_eda/pa/dataview_eda.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/pa/pa_stats.py` & `spd_eda-0.1.3/src/spd_eda/pa/pa_stats.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/pa/plinko.py` & `spd_eda-0.1.3/src/spd_eda/pa/plinko.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda/sql_tools/sql_table.py` & `spd_eda-0.1.3/src/spd_eda/sql_tools/sql_table.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.1.2/src/spd_eda.egg-info/PKG-INFO` & `spd_eda-0.1.3/src/spd_eda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spd-eda
-Version: 0.1.2
+Version: 0.1.3
 Summary: initial testing
 Author-email: sdooley <author@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `spd_eda-0.1.2/src/spd_eda.egg-info/SOURCES.txt` & `spd_eda-0.1.3/src/spd_eda.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 src/spd_eda/hh_batch/portfolio_analysis.py
 src/spd_eda/hh_batch/report.py
 src/spd_eda/hh_batch/config/__init__.py
 src/spd_eda/hh_batch/config/base_report_config.csv
 src/spd_eda/hh_batch/config/batch_column_config.csv
 src/spd_eda/hh_batch/config/batch_data_dictionary.csv
 src/spd_eda/hh_batch/config/config.py
+src/spd_eda/hh_batch/config/report_translation_tables.xlsx
 src/spd_eda/hh_batch/tests/__init__.py
 src/spd_eda/hh_batch/tests/scratch.py
 src/spd_eda/hh_batch/utils/__init__.py
 src/spd_eda/hh_batch/utils/binning_utils.py
 src/spd_eda/hh_batch/utils/chart_utils.py
 src/spd_eda/hh_batch/utils/excel_utils.py
 src/spd_eda/hh_batch/utils/stat_utils.py
```

