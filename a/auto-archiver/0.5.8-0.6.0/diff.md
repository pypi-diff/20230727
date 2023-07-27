# Comparing `tmp/auto_archiver-0.5.8.tar.gz` & `tmp/auto_archiver-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_archiver-0.5.8.tar", last modified: Tue May  2 13:32:57 2023, max compression
+gzip compressed data, was "auto_archiver-0.6.0.tar", last modified: Thu Jul 27 14:46:00 2023, max compression
```

## Comparing `auto_archiver-0.5.8.tar` & `auto_archiver-0.6.0.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-02 13:32:57.396901 auto_archiver-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.380901 auto_archiver-0.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.384901 auto_archiver-0.5.8/src/auto_archiver/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.388901 auto_archiver-0.5.8/src/auto_archiver/archivers/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/instagram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/instagram_tbot_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/telegram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/telethon_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/tiktok_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/twitter_api_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/twitter_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/vk_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/archivers/youtubedl_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/auto_auto_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.388901 auto_archiver-0.5.8/src/auto_archiver/core/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/core/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/core/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.388901 auto_archiver-0.5.8/src/auto_archiver/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/databases/console_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/databases/csv_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/databases/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/databases/gsheet_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/src/auto_archiver/enrichers/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/hash_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/screenshot_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/thumbnail_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/wacz_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/wayback_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/enrichers/whisper_enricher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/src/auto_archiver/feeders/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/feeders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/feeders/cli_feeder.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/feeders/feeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/feeders/gsheet_feeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/src/auto_archiver/formatters/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/formatters/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/formatters/html_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/formatters/mute_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/src/auto_archiver/formatters/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/formatters/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/formatters/templates/html_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/formatters/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/src/auto_archiver/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/storages/gd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/storages/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/storages/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/storages/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.392901 auto_archiver-0.5.8/src/auto_archiver/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/utils/gsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/utils/gworksheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/utils/webdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-02 13:31:36.000000 auto_archiver-0.5.8/src/auto_archiver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:32:57.384901 auto_archiver-0.5.8/src/auto_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-05-02 13:32:57.000000 auto_archiver-0.5.8/src/auto_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-02 13:32:57.000000 auto_archiver-0.5.8/src/auto_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:32:57.000000 auto_archiver-0.5.8/src/auto_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-02 13:32:57.000000 auto_archiver-0.5.8/src/auto_archiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:32:57.000000 auto_archiver-0.5.8/src/auto_archiver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-02 13:32:57.000000 auto_archiver-0.5.8/src/auto_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 13:32:57.000000 auto_archiver-0.5.8/src/auto_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.840499 auto_archiver-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-07-27 14:46:00.840499 auto_archiver-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-27 14:46:00.840499 auto_archiver-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.820499 auto_archiver-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.828498 auto_archiver-0.6.0/src/auto_archiver/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.832499 auto_archiver-0.6.0/src/auto_archiver/archivers/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/instagram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/instagram_tbot_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/telegram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/telethon_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/tiktok_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/twitter_api_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/twitter_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/vk_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/youtubedl_archiver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.832499 auto_archiver-0.6.0/src/auto_archiver/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/core/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/core/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.832499 auto_archiver-0.6.0/src/auto_archiver/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/databases/api_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/databases/console_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/databases/csv_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/databases/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/databases/gsheet_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.836499 auto_archiver-0.6.0/src/auto_archiver/enrichers/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/hash_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/pdq_hash_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/screenshot_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/thumbnail_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/wacz_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/wayback_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/whisper_enricher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.836499 auto_archiver-0.6.0/src/auto_archiver/feeders/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/feeders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/feeders/cli_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/feeders/feeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/feeders/gsheet_feeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.836499 auto_archiver-0.6.0/src/auto_archiver/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/formatters/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/formatters/html_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/formatters/mute_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.836499 auto_archiver-0.6.0/src/auto_archiver/formatters/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/formatters/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/formatters/templates/html_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/formatters/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.840499 auto_archiver-0.6.0/src/auto_archiver/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/storages/gd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/storages/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/storages/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/storages/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.840499 auto_archiver-0.6.0/src/auto_archiver/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/utils/gsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/utils/gworksheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/utils/webdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.832499 auto_archiver-0.6.0/src/auto_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-07-27 14:46:00.000000 auto_archiver-0.6.0/src/auto_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-27 14:46:00.000000 auto_archiver-0.6.0/src/auto_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:46:00.000000 auto_archiver-0.6.0/src/auto_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 14:46:00.000000 auto_archiver-0.6.0/src/auto_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:46:00.000000 auto_archiver-0.6.0/src/auto_archiver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-27 14:46:00.000000 auto_archiver-0.6.0/src/auto_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 14:46:00.000000 auto_archiver-0.6.0/src/auto_archiver.egg-info/top_level.txt
```

### Comparing `auto_archiver-0.5.8/LICENSE` & `auto_archiver-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/PKG-INFO` & `auto_archiver-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_archiver
-Version: 0.5.8
+Version: 0.6.0
 Summary: Easily archive online media content
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
 Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
 Project-URL: Bellingcat, https://www.bellingcat.com
@@ -17,15 +17,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">Auto Archiver</h1>
 
 [![PyPI version](https://badge.fury.io/py/auto-archiver.svg)](https://badge.fury.io/py/auto-archiver)
-[![Docker Image Version (latest by date)](https://img.shields.io/docker/v/bellingcat/auto-archiver?label=version&logo=docker)](https://pypi.org/project/auto-archiver/)
+[![Docker Image Version (latest by date)](https://img.shields.io/docker/v/bellingcat/auto-archiver?label=version&logo=docker)](https://hub.docker.com/r/bellingcat/auto-archiver)
 <!-- ![Docker Pulls](https://img.shields.io/docker/pulls/bellingcat/auto-archiver) -->
 <!-- [![PyPI download month](https://img.shields.io/pypi/dm/auto-archiver.svg)](https://pypi.python.org/pypi/auto-archiver/) -->
 <!-- [![Documentation Status](https://readthedocs.org/projects/vk-url-scraper/badge/?version=latest)](https://vk-url-scraper.readthedocs.io/en/latest/?badge=latest) -->
 
 
 Read the [article about Auto Archiver on bellingcat.com](https://www.bellingcat.com/resources/2022/09/22/preserve-vital-online-content-with-bellingcats-auto-archiver-tool/).
 
@@ -36,64 +36,61 @@
 1. (easiest installation) via docker
 2. (local python install) `pip install auto-archiver`
 3. (legacy/development) clone and manually install from repo (see legacy [tutorial video](https://youtu.be/VfAhcuV2tLQ))
 
 But **you always need a configuration/orchestration file**, which is where you'll configure where/what/how to archive. Make sure you read [orchestration](#orchestration).
 
 
-## How to run the auto-archiver
+## How to install and run the auto-archiver
 
 ### Option 1 - docker
 
-<details><summary><code>Docker instructions</code></summary>
-
 [![dockeri.co](https://dockerico.blankenship.io/image/bellingcat/auto-archiver)](https://hub.docker.com/r/bellingcat/auto-archiver)
 
 Docker works like a virtual machine running inside your computer, it isolates everything and makes installation simple. Since it is an isolated environment when you need to pass it your orchestration file or get downloaded media out of docker you will need to connect folders on your machine with folders inside docker with the `-v` volume flag.
 
 
 1. install [docker](https://docs.docker.com/get-docker/)
 2. pull the auto-archiver docker [image](https://hub.docker.com/r/bellingcat/auto-archiver) with `docker pull bellingcat/auto-archiver`
-3. run the docker image locally in a container: `docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver -m auto_archiver  --config secrets/orchestration.yaml` breaking this command down:
+3. run the docker image locally in a container: `docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver --config secrets/orchestration.yaml` breaking this command down:
    1. `docker run` tells docker to start a new container (an instance of the image)
    2. `--rm` makes sure this container is removed after execution (less garbage locally)
    3. `-v $PWD/secrets:/app/secrets` - your secrets folder
       1. `-v` is a volume flag which means a folder that you have on your computer will be connected to a folder inside the docker container
       2. `$PWD/secrets` points to a `secrets/` folder in your current working directory (where your console points to), we use this folder as a best practice to hold all the secrets/tokens/passwords/... you use
       3. `/app/secrets` points to the path the docker container where this image can be found
    4.  `-v $PWD/local_archive:/app/local_archive` - (optional) if you use local_storage
        1.  `-v` same as above, this is a volume instruction
        2.  `$PWD/local_archive` is a folder `local_archive/` in case you want to archive locally and have the files accessible outside docker
        3.  `/app/local_archive` is a folder inside docker that you can reference in your orchestration.yml file 
 
-</details>
-
 ### Option 2 - python package
 
 <details><summary><code>Python package instructions</code></summary>
 
 1. make sure you have python 3.8 or higher installed
 2. install the package `pip/pipenv/conda install auto-archiver`
 3. test it's installed with `auto-archiver --help`
-4. run it with your orchestration file and pass any flags you want in the command line `auto-archiver --config secrets/orchestration.yaml`
-   1. if your orchestration file is inside a `secrets/` which we advise
+4. run it with your orchestration file and pass any flags you want in the command line `auto-archiver --config secrets/orchestration.yaml` if your orchestration file is inside a `secrets/`, which we advise
+   
+You will also need [ffmpeg](https://www.ffmpeg.org/), [firefox](https://www.mozilla.org/en-US/firefox/new/) and [geckodriver](https://github.com/mozilla/geckodriver/releases), and optionally [fonts-noto](https://fonts.google.com/noto). Similar to the local installation. 
 
 </details>
 
 
 ### Option 3 - local installation
 This can also be used for development.
 
 <details><summary><code>Legacy instructions, only use if docker/package is not an option</code></summary>
 
 
 Install the following locally:
 1. [ffmpeg](https://www.ffmpeg.org/) must also be installed locally for this tool to work. 
 2. [firefox](https://www.mozilla.org/en-US/firefox/new/) and [geckodriver](https://github.com/mozilla/geckodriver/releases) on a path folder like `/usr/local/bin`. 
-3. [fonts-noto](https://fonts.google.com/noto) to deal with multiple unicode characters during selenium/geckodriver's screenshots: `sudo apt install fonts-noto -y`. 
+3. (optional) [fonts-noto](https://fonts.google.com/noto) to deal with multiple unicode characters during selenium/geckodriver's screenshots: `sudo apt install fonts-noto -y`. 
 
 Clone and run:
 1. `git clone https://github.com/bellingcat/auto-archiver`
 2. `pipenv install`
 3. `pipenv run python -m src.auto_archiver --config secrets/orchestration.yaml`
 
 
@@ -103,19 +100,17 @@
 The archiver work is orchestrated by the following workflow (we call each a **step**): 
 1. **Feeder** gets the links (from a spreadsheet, from the console, ...)
 2. **Archiver** tries to archive the link (twitter, youtube, ...)
 3. **Enricher** adds more info to the content (hashes, thumbnails, ...)
 4. **Formatter** creates a report from all the archived content (HTML, PDF, ...)
 5. **Database** knows what's been archived and also stores the archive result (spreadsheet, CSV, or just the console)
 
-To check all available steps (which archivers, storages, databses, ...) exist check the [example.orchestration.yaml](example.orchestration.yaml).
+To setup an auto-archiver instance create an `orchestration.yaml` which contains the workflow you would like. We advise you put this file into a `secrets/` folder and do not share it with others because it will contain passwords and other secrets. 
 
-The great thing is you configure all the workflow in your `orchestration.yaml` file which we advise you put into a `secrets/` folder and don't share it with others because it will contain passwords and other secrets. 
-
-The structure of orchestration file is split into 2 parts: `steps` (what **steps** to use) and `configs` (how those steps should behave), here's a simplification:
+The structure of orchestration file is split into 2 parts: `steps` (what **steps** to use) and `configurations` (how those steps should behave), here's a simplification:
 ```yaml
 # orchestration.yaml content
 steps:
   feeder: gsheet_feeder
   archivers: # order matters
     - youtubedl_archiver
   enrichers:
@@ -129,18 +124,20 @@
 configurations:
   gsheet_feeder:
     sheet: "your google sheet name"
     header: 2 # row with header for your sheet
   # ... configurations for the other steps here ...
 ```
 
+To see all available `steps` (which archivers, storages, databses, ...) exist check the [example.orchestration.yaml](example.orchestration.yaml).
+
 All the `configurations` in the `orchestration.yaml` file (you can name it differently but need to pass it in the `--config FILENAME` argument) can be seen in the console by using the `--help` flag. They can also be overwritten, for example if you are using the `cli_feeder` to archive from the command line and want to provide the URLs you should do:
 
 ```bash
-auto-archiver --config orchestration.yaml --cli_feeder.urls="url1,url2,url3"
+auto-archiver --config secrets/orchestration.yaml --cli_feeder.urls="url1,url2,url3"
 ```
 
 Here's the complete workflow that the auto-archiver goes through:
 ```mermaid
 graph TD
     s((start)) --> F(fa:fa-table Feeder)
     F -->|get and clean URL| D1{fa:fa-database Database}
@@ -163,61 +160,100 @@
     * if you use private channels you need to add `channel_invites` and set `join_channels=true` at least once
   * [ ] (optional for VK) a `vk_config.v2.json`
   * [ ] (optional for using GoogleDrive storage) `gd-token.json` (see [help script](scripts/create_update_gdrive_oauth_token.py))
   * [ ] (optional for instagram) `instaloader.session` file which appears after the 1st run and login in instagram
   * [ ] (optional for browsertrix) `profile.tar.gz` file
 
 #### Example invocations
-These assume you've installed with pipenv, see docker section above for how to run through docker
+The recommended way to run the auto-archiver is through Docker. The invocations below will run the auto-archiver Docker image using a configuration file that you have specified
+
+```bash
+# all the configurations come from ./secrets/orchestration.yaml
+docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver --config secrets/orchestration.yaml
+# uses the same configurations but for another google docs sheet 
+# with a header on row 2 and with some different column names
+# notice that columns is a dictionary so you need to pass it as JSON and it will override only the values provided
+docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver --config secrets/orchestration.yaml --gsheet_feeder.sheet="use it on another sheets doc" --gsheet_feeder.header=2 --gsheet_feeder.columns='{"url": "link"}'
+# all the configurations come from orchestration.yaml and specifies that s3 files should be private
+docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver --config secrets/orchestration.yaml --s3_storage.private=1
+```
+
+The auto-archiver can also be run locally, if pre-requisites are correctly configured. Equivalent invocations are below.
 
 ```bash
-# all the configurations come from ./orchestration.yaml
-auto-archiver
 # all the configurations come from ./secrets/orchestration.yaml
 auto-archiver --config secrets/orchestration.yaml
 # uses the same configurations but for another google docs sheet 
 # with a header on row 2 and with some different column names
 # notice that columns is a dictionary so you need to pass it as JSON and it will override only the values provided
-auto-archiver --config orchestration.yaml --gsheet_feeder.sheet="use it on another sheets doc" --gsheet_feeder.header=2 --gsheet_feeder.columns='{"url": "link"}'
+auto-archiver --config secrets/orchestration.yaml --gsheet_feeder.sheet="use it on another sheets doc" --gsheet_feeder.header=2 --gsheet_feeder.columns='{"url": "link"}'
 # all the configurations come from orchestration.yaml and specifies that s3 files should be private
-auto-archiver --s3_storage.private=1
+auto-archiver --config secrets/orchestration.yaml --s3_storage.private=1
 ```
 
 ### Extra notes on configuration
 #### Google Drive
 To use Google Drive storage you need the id of the shared folder in the `config.yaml` file which must be shared with the service account eg `autoarchiverservice@auto-archiver-111111.iam.gserviceaccount.com` and then you can use `--storage=gd`
 
 #### Telethon + Instagram with telegram bot
 The first time you run, you will be prompted to do a authentication with the phone number associated, alternatively you can put your `anon.session` in the root.
 
 
 ## Running on Google Sheets Feeder (gsheet_feeder)
 The `--gseets_feeder.sheet` property is the name of the Google Sheet to check for URLs. 
 This sheet must have been shared with the Google Service account used by `gspread`. 
-This sheet must also have specific columns (case-insensitive) in the `header` row - see [Gsheet.configs](src/auto_archiver/utils/gsheet.py) for all their names.
+This sheet must also have specific columns (case-insensitive) in the `header` as specified in [Gsheet.configs](src/auto_archiver/utils/gsheet.py). The default names of these columns and their purpose is:
+
+Inputs:
+
+* **Link** *(required)*: the URL of the post to archive
+* **Destination folder**: custom folder for archived file (regardless of storage)
+
+Outputs:
+* **Archive status** *(required)*: Status of archive operation
+* **Archive location**: URL of archived post
+* **Archive date**: Date archived
+* **Thumbnail**: Embeds a thumbnail for the post in the spreadsheet
+* **Timestamp**: Timestamp of original post
+* **Title**: Post title
+* **Text**: Post text
+* **Screenshot**: Link to screenshot of post
+* **Hash**: Hash of archived HTML file (which contains hashes of post media) - for checksums/verification
+* **Perceptual Hash**: Perceptual hashes of found images - these can be used for de-duplication of content
+* **WACZ**: Link to a WACZ web archive of post
+* **ReplayWebpage**: Link to a ReplayWebpage viewer of the WACZ archive
+
+For example, this is a spreadsheet configured with all of the columns for the auto archiver and a few URLs to archive. (Note that the column names are not case sensitive.)
 
-For example, for use with this spreadsheet:
+![A screenshot of a Google Spreadsheet with column headers defined as above, and several Youtube and Twitter URLs in the "Link" column](docs/demo-before.png)
 
-![A screenshot of a Google Spreadsheet with column headers defined as above, and several Youtube and Twitter URLs in the "Media URL" column](docs/demo-before.png)
+Now the auto archiver can be invoked, with this command in this example: `docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver:dockerize --config secrets/orchestration-global.yaml --gsheet_feeder.sheet "Auto archive test 2023-2"`. Note that the sheet name has been overridden/specified in the command line invocation.
 
 When the auto archiver starts running, it updates the "Archive status" column.
-![A screenshot of a Google Spreadsheet with column headers defined as above, and several Youtube and Twitter URLs in the "Media URL" column. The auto archiver has added "archive in progress" to one of the status columns.](docs/demo-progress.png)
+
+![A screenshot of a Google Spreadsheet with column headers defined as above, and several Youtube and Twitter URLs in the "Link" column. The auto archiver has added "archive in progress" to one of the status columns.](docs/demo-progress.png)
+
 The links are downloaded and archived, and the spreadsheet is updated to the following:
+
 ![A screenshot of a Google Spreadsheet with videos archived and metadata added per the description of the columns above.](docs/demo-after.png)
+
 Note that the first row is skipped, as it is assumed to be a header row (`--gsheet_feeder.header=1` and you can change it if you use more rows above). Rows with an empty URL column, or a non-empty archive column are also skipped. All sheets in the document will be checked.
 
+The "archive location" link contains the path of the archived file, in local storage, S3, or in Google Drive.
+
+![The archive result for a link in the demo sheet.](docs/demo-archive.png)
 
 ---
 ## Development
 Use `python -m src.auto_archiver --config secrets/orchestration.yaml` to run from the local development environment.
 
 #### Docker development
 working with docker locally:
   * `docker build . -t auto-archiver` to build a local image
-  * `docker run --rm -v $PWD/secrets:/app/secrets aa --config secrets/config.yaml`
+  * `docker run --rm -v $PWD/secrets:/app/secrets auto-archiver  --config secrets/orchestration.yaml`
     * to use local archive, also create a volume `-v` for it by adding `-v $PWD/local_archive:/app/local_archive`
 
 
 release to docker hub
   * `docker image tag auto-archiver bellingcat/auto-archiver:latest`
   * `docker push bellingcat/auto-archiver`
```

### Comparing `auto_archiver-0.5.8/README.md` & `auto_archiver-0.6.0/src/auto_archiver.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,31 @@
+Metadata-Version: 2.1
+Name: auto-archiver
+Version: 0.6.0
+Summary: Easily archive online media content
+Author: Bellingcat
+Author-email: tech@bellingcat.com
+License: MIT
+Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
+Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
+Project-URL: Bellingcat, https://www.bellingcat.com
+Keywords: archive,oosi,osint,scraping
+Platform: any
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h1 align="center">Auto Archiver</h1>
 
 [![PyPI version](https://badge.fury.io/py/auto-archiver.svg)](https://badge.fury.io/py/auto-archiver)
-[![Docker Image Version (latest by date)](https://img.shields.io/docker/v/bellingcat/auto-archiver?label=version&logo=docker)](https://pypi.org/project/auto-archiver/)
+[![Docker Image Version (latest by date)](https://img.shields.io/docker/v/bellingcat/auto-archiver?label=version&logo=docker)](https://hub.docker.com/r/bellingcat/auto-archiver)
 <!-- ![Docker Pulls](https://img.shields.io/docker/pulls/bellingcat/auto-archiver) -->
 <!-- [![PyPI download month](https://img.shields.io/pypi/dm/auto-archiver.svg)](https://pypi.python.org/pypi/auto-archiver/) -->
 <!-- [![Documentation Status](https://readthedocs.org/projects/vk-url-scraper/badge/?version=latest)](https://vk-url-scraper.readthedocs.io/en/latest/?badge=latest) -->
 
 
 Read the [article about Auto Archiver on bellingcat.com](https://www.bellingcat.com/resources/2022/09/22/preserve-vital-online-content-with-bellingcats-auto-archiver-tool/).
 
@@ -16,64 +36,61 @@
 1. (easiest installation) via docker
 2. (local python install) `pip install auto-archiver`
 3. (legacy/development) clone and manually install from repo (see legacy [tutorial video](https://youtu.be/VfAhcuV2tLQ))
 
 But **you always need a configuration/orchestration file**, which is where you'll configure where/what/how to archive. Make sure you read [orchestration](#orchestration).
 
 
-## How to run the auto-archiver
+## How to install and run the auto-archiver
 
 ### Option 1 - docker
 
-<details><summary><code>Docker instructions</code></summary>
-
 [![dockeri.co](https://dockerico.blankenship.io/image/bellingcat/auto-archiver)](https://hub.docker.com/r/bellingcat/auto-archiver)
 
 Docker works like a virtual machine running inside your computer, it isolates everything and makes installation simple. Since it is an isolated environment when you need to pass it your orchestration file or get downloaded media out of docker you will need to connect folders on your machine with folders inside docker with the `-v` volume flag.
 
 
 1. install [docker](https://docs.docker.com/get-docker/)
 2. pull the auto-archiver docker [image](https://hub.docker.com/r/bellingcat/auto-archiver) with `docker pull bellingcat/auto-archiver`
-3. run the docker image locally in a container: `docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver -m auto_archiver  --config secrets/orchestration.yaml` breaking this command down:
+3. run the docker image locally in a container: `docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver --config secrets/orchestration.yaml` breaking this command down:
    1. `docker run` tells docker to start a new container (an instance of the image)
    2. `--rm` makes sure this container is removed after execution (less garbage locally)
    3. `-v $PWD/secrets:/app/secrets` - your secrets folder
       1. `-v` is a volume flag which means a folder that you have on your computer will be connected to a folder inside the docker container
       2. `$PWD/secrets` points to a `secrets/` folder in your current working directory (where your console points to), we use this folder as a best practice to hold all the secrets/tokens/passwords/... you use
       3. `/app/secrets` points to the path the docker container where this image can be found
    4.  `-v $PWD/local_archive:/app/local_archive` - (optional) if you use local_storage
        1.  `-v` same as above, this is a volume instruction
        2.  `$PWD/local_archive` is a folder `local_archive/` in case you want to archive locally and have the files accessible outside docker
        3.  `/app/local_archive` is a folder inside docker that you can reference in your orchestration.yml file 
 
-</details>
-
 ### Option 2 - python package
 
 <details><summary><code>Python package instructions</code></summary>
 
 1. make sure you have python 3.8 or higher installed
 2. install the package `pip/pipenv/conda install auto-archiver`
 3. test it's installed with `auto-archiver --help`
-4. run it with your orchestration file and pass any flags you want in the command line `auto-archiver --config secrets/orchestration.yaml`
-   1. if your orchestration file is inside a `secrets/` which we advise
+4. run it with your orchestration file and pass any flags you want in the command line `auto-archiver --config secrets/orchestration.yaml` if your orchestration file is inside a `secrets/`, which we advise
+   
+You will also need [ffmpeg](https://www.ffmpeg.org/), [firefox](https://www.mozilla.org/en-US/firefox/new/) and [geckodriver](https://github.com/mozilla/geckodriver/releases), and optionally [fonts-noto](https://fonts.google.com/noto). Similar to the local installation. 
 
 </details>
 
 
 ### Option 3 - local installation
 This can also be used for development.
 
 <details><summary><code>Legacy instructions, only use if docker/package is not an option</code></summary>
 
 
 Install the following locally:
 1. [ffmpeg](https://www.ffmpeg.org/) must also be installed locally for this tool to work. 
 2. [firefox](https://www.mozilla.org/en-US/firefox/new/) and [geckodriver](https://github.com/mozilla/geckodriver/releases) on a path folder like `/usr/local/bin`. 
-3. [fonts-noto](https://fonts.google.com/noto) to deal with multiple unicode characters during selenium/geckodriver's screenshots: `sudo apt install fonts-noto -y`. 
+3. (optional) [fonts-noto](https://fonts.google.com/noto) to deal with multiple unicode characters during selenium/geckodriver's screenshots: `sudo apt install fonts-noto -y`. 
 
 Clone and run:
 1. `git clone https://github.com/bellingcat/auto-archiver`
 2. `pipenv install`
 3. `pipenv run python -m src.auto_archiver --config secrets/orchestration.yaml`
 
 
@@ -83,19 +100,17 @@
 The archiver work is orchestrated by the following workflow (we call each a **step**): 
 1. **Feeder** gets the links (from a spreadsheet, from the console, ...)
 2. **Archiver** tries to archive the link (twitter, youtube, ...)
 3. **Enricher** adds more info to the content (hashes, thumbnails, ...)
 4. **Formatter** creates a report from all the archived content (HTML, PDF, ...)
 5. **Database** knows what's been archived and also stores the archive result (spreadsheet, CSV, or just the console)
 
-To check all available steps (which archivers, storages, databses, ...) exist check the [example.orchestration.yaml](example.orchestration.yaml).
-
-The great thing is you configure all the workflow in your `orchestration.yaml` file which we advise you put into a `secrets/` folder and don't share it with others because it will contain passwords and other secrets. 
+To setup an auto-archiver instance create an `orchestration.yaml` which contains the workflow you would like. We advise you put this file into a `secrets/` folder and do not share it with others because it will contain passwords and other secrets. 
 
-The structure of orchestration file is split into 2 parts: `steps` (what **steps** to use) and `configs` (how those steps should behave), here's a simplification:
+The structure of orchestration file is split into 2 parts: `steps` (what **steps** to use) and `configurations` (how those steps should behave), here's a simplification:
 ```yaml
 # orchestration.yaml content
 steps:
   feeder: gsheet_feeder
   archivers: # order matters
     - youtubedl_archiver
   enrichers:
@@ -109,18 +124,20 @@
 configurations:
   gsheet_feeder:
     sheet: "your google sheet name"
     header: 2 # row with header for your sheet
   # ... configurations for the other steps here ...
 ```
 
+To see all available `steps` (which archivers, storages, databses, ...) exist check the [example.orchestration.yaml](example.orchestration.yaml).
+
 All the `configurations` in the `orchestration.yaml` file (you can name it differently but need to pass it in the `--config FILENAME` argument) can be seen in the console by using the `--help` flag. They can also be overwritten, for example if you are using the `cli_feeder` to archive from the command line and want to provide the URLs you should do:
 
 ```bash
-auto-archiver --config orchestration.yaml --cli_feeder.urls="url1,url2,url3"
+auto-archiver --config secrets/orchestration.yaml --cli_feeder.urls="url1,url2,url3"
 ```
 
 Here's the complete workflow that the auto-archiver goes through:
 ```mermaid
 graph TD
     s((start)) --> F(fa:fa-table Feeder)
     F -->|get and clean URL| D1{fa:fa-database Database}
@@ -143,66 +160,105 @@
     * if you use private channels you need to add `channel_invites` and set `join_channels=true` at least once
   * [ ] (optional for VK) a `vk_config.v2.json`
   * [ ] (optional for using GoogleDrive storage) `gd-token.json` (see [help script](scripts/create_update_gdrive_oauth_token.py))
   * [ ] (optional for instagram) `instaloader.session` file which appears after the 1st run and login in instagram
   * [ ] (optional for browsertrix) `profile.tar.gz` file
 
 #### Example invocations
-These assume you've installed with pipenv, see docker section above for how to run through docker
+The recommended way to run the auto-archiver is through Docker. The invocations below will run the auto-archiver Docker image using a configuration file that you have specified
+
+```bash
+# all the configurations come from ./secrets/orchestration.yaml
+docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver --config secrets/orchestration.yaml
+# uses the same configurations but for another google docs sheet 
+# with a header on row 2 and with some different column names
+# notice that columns is a dictionary so you need to pass it as JSON and it will override only the values provided
+docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver --config secrets/orchestration.yaml --gsheet_feeder.sheet="use it on another sheets doc" --gsheet_feeder.header=2 --gsheet_feeder.columns='{"url": "link"}'
+# all the configurations come from orchestration.yaml and specifies that s3 files should be private
+docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver --config secrets/orchestration.yaml --s3_storage.private=1
+```
+
+The auto-archiver can also be run locally, if pre-requisites are correctly configured. Equivalent invocations are below.
 
 ```bash
-# all the configurations come from ./orchestration.yaml
-auto-archiver
 # all the configurations come from ./secrets/orchestration.yaml
 auto-archiver --config secrets/orchestration.yaml
 # uses the same configurations but for another google docs sheet 
 # with a header on row 2 and with some different column names
 # notice that columns is a dictionary so you need to pass it as JSON and it will override only the values provided
-auto-archiver --config orchestration.yaml --gsheet_feeder.sheet="use it on another sheets doc" --gsheet_feeder.header=2 --gsheet_feeder.columns='{"url": "link"}'
+auto-archiver --config secrets/orchestration.yaml --gsheet_feeder.sheet="use it on another sheets doc" --gsheet_feeder.header=2 --gsheet_feeder.columns='{"url": "link"}'
 # all the configurations come from orchestration.yaml and specifies that s3 files should be private
-auto-archiver --s3_storage.private=1
+auto-archiver --config secrets/orchestration.yaml --s3_storage.private=1
 ```
 
 ### Extra notes on configuration
 #### Google Drive
 To use Google Drive storage you need the id of the shared folder in the `config.yaml` file which must be shared with the service account eg `autoarchiverservice@auto-archiver-111111.iam.gserviceaccount.com` and then you can use `--storage=gd`
 
 #### Telethon + Instagram with telegram bot
 The first time you run, you will be prompted to do a authentication with the phone number associated, alternatively you can put your `anon.session` in the root.
 
 
 ## Running on Google Sheets Feeder (gsheet_feeder)
 The `--gseets_feeder.sheet` property is the name of the Google Sheet to check for URLs. 
 This sheet must have been shared with the Google Service account used by `gspread`. 
-This sheet must also have specific columns (case-insensitive) in the `header` row - see [Gsheet.configs](src/auto_archiver/utils/gsheet.py) for all their names.
+This sheet must also have specific columns (case-insensitive) in the `header` as specified in [Gsheet.configs](src/auto_archiver/utils/gsheet.py). The default names of these columns and their purpose is:
+
+Inputs:
+
+* **Link** *(required)*: the URL of the post to archive
+* **Destination folder**: custom folder for archived file (regardless of storage)
+
+Outputs:
+* **Archive status** *(required)*: Status of archive operation
+* **Archive location**: URL of archived post
+* **Archive date**: Date archived
+* **Thumbnail**: Embeds a thumbnail for the post in the spreadsheet
+* **Timestamp**: Timestamp of original post
+* **Title**: Post title
+* **Text**: Post text
+* **Screenshot**: Link to screenshot of post
+* **Hash**: Hash of archived HTML file (which contains hashes of post media) - for checksums/verification
+* **Perceptual Hash**: Perceptual hashes of found images - these can be used for de-duplication of content
+* **WACZ**: Link to a WACZ web archive of post
+* **ReplayWebpage**: Link to a ReplayWebpage viewer of the WACZ archive
 
-For example, for use with this spreadsheet:
+For example, this is a spreadsheet configured with all of the columns for the auto archiver and a few URLs to archive. (Note that the column names are not case sensitive.)
 
-![A screenshot of a Google Spreadsheet with column headers defined as above, and several Youtube and Twitter URLs in the "Media URL" column](docs/demo-before.png)
+![A screenshot of a Google Spreadsheet with column headers defined as above, and several Youtube and Twitter URLs in the "Link" column](docs/demo-before.png)
+
+Now the auto archiver can be invoked, with this command in this example: `docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver:dockerize --config secrets/orchestration-global.yaml --gsheet_feeder.sheet "Auto archive test 2023-2"`. Note that the sheet name has been overridden/specified in the command line invocation.
 
 When the auto archiver starts running, it updates the "Archive status" column.
-![A screenshot of a Google Spreadsheet with column headers defined as above, and several Youtube and Twitter URLs in the "Media URL" column. The auto archiver has added "archive in progress" to one of the status columns.](docs/demo-progress.png)
+
+![A screenshot of a Google Spreadsheet with column headers defined as above, and several Youtube and Twitter URLs in the "Link" column. The auto archiver has added "archive in progress" to one of the status columns.](docs/demo-progress.png)
+
 The links are downloaded and archived, and the spreadsheet is updated to the following:
+
 ![A screenshot of a Google Spreadsheet with videos archived and metadata added per the description of the columns above.](docs/demo-after.png)
+
 Note that the first row is skipped, as it is assumed to be a header row (`--gsheet_feeder.header=1` and you can change it if you use more rows above). Rows with an empty URL column, or a non-empty archive column are also skipped. All sheets in the document will be checked.
 
+The "archive location" link contains the path of the archived file, in local storage, S3, or in Google Drive.
+
+![The archive result for a link in the demo sheet.](docs/demo-archive.png)
 
 ---
 ## Development
 Use `python -m src.auto_archiver --config secrets/orchestration.yaml` to run from the local development environment.
 
 #### Docker development
 working with docker locally:
   * `docker build . -t auto-archiver` to build a local image
-  * `docker run --rm -v $PWD/secrets:/app/secrets aa --config secrets/config.yaml`
+  * `docker run --rm -v $PWD/secrets:/app/secrets auto-archiver  --config secrets/orchestration.yaml`
     * to use local archive, also create a volume `-v` for it by adding `-v $PWD/local_archive:/app/local_archive`
 
 
 release to docker hub
   * `docker image tag auto-archiver bellingcat/auto-archiver:latest`
   * `docker push bellingcat/auto-archiver`
 
 #### RELEASE
 * update version in [version.py](src/auto_archiver/version.py)
 * run `bash ./scripts/release.sh` and confirm
 * package is automatically updated in pypi
-* docker image is automatically pushed to dockerhup
+* docker image is automatically pushed to dockerhup
```

### Comparing `auto_archiver-0.5.8/setup.cfg` & `auto_archiver-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/archivers/archiver.py` & `auto_archiver-0.6.0/src/auto_archiver/archivers/archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/archivers/instagram_archiver.py` & `auto_archiver-0.6.0/src/auto_archiver/archivers/instagram_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/archivers/instagram_tbot_archiver.py` & `auto_archiver-0.6.0/src/auto_archiver/archivers/instagram_tbot_archiver.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     @staticmethod
     def configs() -> dict:
         return {
             "api_id": {"default": None, "help": "telegram API_ID value, go to https://my.telegram.org/apps"},
             "api_hash": {"default": None, "help": "telegram API_HASH value, go to https://my.telegram.org/apps"},
             "session_file": {"default": "secrets/anon-insta", "help": "optional, records the telegram login session for future usage, '.session' will be appended to the provided value."},
-            "timeout": {"default": 15, "help": "timeout to fetch the instagram content in seconds."},
+            "timeout": {"default": 45, "help": "timeout to fetch the instagram content in seconds."},
         }
 
     def setup(self) -> None:
         logger.info(f"SETUP {self.name} checking login...")
         with self.client.start():
             logger.success(f"SETUP {self.name} login works.")
 
@@ -48,17 +48,17 @@
         with self.client.start():
             chat = self.client.get_entity("instagram_load_bot")
             since_id = self.client.send_message(entity=chat, message=url).id
 
             attempts = 0
             seen_media = []
             message = ""
-            time.sleep(4)
+            time.sleep(3)
             # media is added before text by the bot so it can be used as a stop-logic mechanism
-            while attempts < self.timeout and (not message or not len(seen_media)):
+            while attempts < (self.timeout - 3) and (not message or not len(seen_media)):
                 attempts += 1
                 time.sleep(1)
                 for post in self.client.iter_messages(chat, min_id=since_id):
                     since_id = max(since_id, post.id)
                     if post.media and post.id not in seen_media:
                         filename_dest = os.path.join(tmp_dir, f'{chat.id}_{post.id}')
                         media = self.client.download_media(post.media, filename_dest)
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/archivers/telegram_archiver.py` & `auto_archiver-0.6.0/src/auto_archiver/archivers/telegram_archiver.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         result.set_content(html.escape(str(t.content)))
         if (timestamp := (s.find_all('time') or [{}])[0].get('datetime')):
             result.set_timestamp(timestamp)
 
         video = s.find("video")
         if video is None:
             logger.warning("could not find video")
-            image_tags = s.find_all(class_="js-message_photo")
+            image_tags = s.find_all(class_="tgme_widget_message_photo_wrap")
 
             image_urls = []
             for im in image_tags:
                 urls = [u.replace("'", "") for u in re.findall(r'url\((.*?)\)', im['style'])]
                 image_urls += urls
 
             if not len(image_urls): return False
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/archivers/telethon_archiver.py` & `auto_archiver-0.6.0/src/auto_archiver/archivers/telethon_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/archivers/tiktok_archiver.py` & `auto_archiver-0.6.0/src/auto_archiver/archivers/tiktok_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/archivers/twitter_api_archiver.py` & `auto_archiver-0.6.0/src/auto_archiver/archivers/twitter_api_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/archivers/twitter_archiver.py` & `auto_archiver-0.6.0/src/auto_archiver/archivers/twitter_archiver.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from datetime import datetime
 from loguru import logger
 from snscrape.modules.twitter import TwitterTweetScraper, Video, Gif, Photo
 from slugify import slugify
 
 from . import Archiver
 from ..core import Metadata, Media
+from ..utils import UrlUtil
 
 
 class TwitterArchiver(Archiver):
     """
     This Twitter Archiver uses unofficial scraping methods.
     """
 
@@ -73,58 +74,64 @@
                 media.set("src", variant.url).set("duration", tweet_media.duration)
                 mimetype = variant.contentType
             elif type(tweet_media) == Gif:
                 variant = tweet_media.variants[0]
                 media.set("src", variant.url)
                 mimetype = variant.contentType
             elif type(tweet_media) == Photo:
-                media.set("src", tweet_media.fullUrl.replace('name=large', 'name=orig'))
+                media.set("src", tweet_media.fullUrl.replace('name=large', 'name=orig').replace('name=small', 'name=orig'))
                 mimetype = "image/jpeg"
             else:
                 logger.warning(f"Could not get media URL of {tweet_media}")
                 continue
             ext = mimetypes.guess_extension(mimetype)
             media.filename = self.download_from_url(media.get("src"), f'{slugify(url)}_{i}{ext}', item)
             result.add_media(media)
 
         return result.success("twitter-snscrape")
 
     def download_alternative(self, item: Metadata, url: str, tweet_id: str) -> Metadata:
         """
-        CURRENTLY STOPPED WORKING
+        Hack alternative working again.
+        https://stackoverflow.com/a/71867055/6196010 (OUTDATED URL)
+        https://github.com/JustAnotherArchivist/snscrape/issues/996#issuecomment-1615937362
+        next to test: https://cdn.embedly.com/widgets/media.html?&schema=twitter&url=https://twitter.com/bellingcat/status/1674700676612386816
         """
-        return False
-        # https://stackoverflow.com/a/71867055/6196010
+
         logger.debug(f"Trying twitter hack for {url=}")
         result = Metadata()
 
-        hack_url = f"https://cdn.syndication.twimg.com/tweet?id={tweet_id}"
+        hack_url = f"https://cdn.syndication.twimg.com/tweet-result?id={tweet_id}"
         r = requests.get(hack_url)
         if r.status_code != 200: return False
         tweet = r.json()
 
         urls = []
-        for p in tweet["photos"]:
+        for p in tweet.get("photos", []):
             urls.append(p["url"])
 
         # 1 tweet has 1 video max
         if "video" in tweet:
             v = tweet["video"]
             urls.append(self.choose_variant(v.get("variants", [])))
 
         logger.debug(f"Twitter hack got {urls=}")
 
-        for u in urls:
-            media = Media()
+        for i, u in enumerate(urls):
+            media = Media(filename="")
             media.set("src", u)
-            media.filename = self.download_from_url(u, f'{slugify(url)}_{i}', item)
+            ext = ""
+            if (mtype := mimetypes.guess_type(UrlUtil.remove_get_parameters(u))[0]):
+                ext = mimetypes.guess_extension(mtype)
+
+            media.filename = self.download_from_url(u, f'{slugify(url)}_{i}{ext}', item)
             result.add_media(media)
 
-        result.set_content(json.dumps(tweet, ensure_ascii=False)).set_timestamp(datetime.strptime(tweet["created_at"], "%Y-%m-%dT%H:%M:%S.%fZ"))
-        return result
+        result.set_title(tweet.get("text")).set_content(json.dumps(tweet, ensure_ascii=False)).set_timestamp(datetime.strptime(tweet["created_at"], "%Y-%m-%dT%H:%M:%S.%fZ"))
+        return result.success("twitter-hack")
 
     def get_username_tweet_id(self, url):
         # detect URLs that we definitely cannot handle
         matches = self.link_pattern.findall(url)
         if not len(matches): return False, False
 
         username, tweet_id = matches[0]  # only one URL supported
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/archivers/vk_archiver.py` & `auto_archiver-0.6.0/src/auto_archiver/archivers/vk_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/archivers/youtubedl_archiver.py` & `auto_archiver-0.6.0/src/auto_archiver/archivers/youtubedl_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/core/config.py` & `auto_archiver-0.6.0/src/auto_archiver/core/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from ..archivers import Archiver
 from ..feeders import Feeder
 from ..databases import Database
 from ..formatters import Formatter
 from ..storages import Storage
 from ..enrichers import Enricher
 from . import Step
+from ..utils import update_nested_dict
 
 
 @dataclass
 class Config:
     configurable_parents = [
         Feeder,
         Enricher,
@@ -34,18 +35,19 @@
     databases: List[Database] = field(default_factory=[])
 
     def __init__(self) -> None:
         self.defaults = {}
         self.cli_ops = {}
         self.config = {}
 
-    def parse(self, use_cli=True, yaml_config_filename: str = None):
+    def parse(self, use_cli=True, yaml_config_filename: str = None, overwrite_configs: str = {}):
         """
         if yaml_config_filename is provided, the --config argument is ignored, 
         useful for library usage when the config values are preloaded
+        overwrite_configs is a dict that overwrites the yaml file contents
         """
         # 1. parse CLI values
         if use_cli:
             parser = argparse.ArgumentParser(
                 # prog = "auto-archiver",
                 description="Auto Archiver is a CLI tool to archive media/metadata from online URLs; it can read URLs from many sources (Google Sheets, Command Line, ...); and write results to many destinations too (CSV, Google Sheets, MongoDB, ...)!",
                 epilog="Check the code at https://github.com/bellingcat/auto-archiver"
@@ -76,14 +78,15 @@
         if use_cli:
             args = parser.parse_args()
             yaml_config_filename = yaml_config_filename or getattr(args, "config")
         else: args = {}
 
         # 2. read YAML config file (or use provided value)
         self.yaml_config = self.read_yaml(yaml_config_filename)
+        update_nested_dict(self.yaml_config, overwrite_configs)
 
         # 3. CONFIGS: decide value with priority: CLI >> config.yaml >> default
         self.config = defaultdict(dict)
         for config_path, default in self.defaults.items():
             child, config = tuple(config_path.split("."))
             val = getattr(args, config_path, None)
             if val is not None and config_path in self.cli_ops:
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/core/context.py` & `auto_archiver-0.6.0/src/auto_archiver/core/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     def get_instance():
         if ArchivingContext._instance is None:
             ArchivingContext._instance = ArchivingContext()
         return ArchivingContext._instance
 
     @staticmethod
     def set(key, value, keep_on_reset: bool = False):
-        logger.error(f"SET [{key}]={value}")
         ac = ArchivingContext.get_instance()
         ac.configs[key] = value
         if keep_on_reset: ac.keep_on_reset.add(key)
 
     @staticmethod
     def get(key: str, default=None):
         return ArchivingContext.get_instance().configs.get(key, default)
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/core/media.py` & `auto_archiver-0.6.0/src/auto_archiver/core/media.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 
 from __future__ import annotations
-from ast import List
-from typing import Any
+from typing import Any, List
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 import mimetypes
 
 from .context import ArchivingContext
 
 from loguru import logger
@@ -15,38 +14,42 @@
 @dataclass
 class Media:
     filename: str
     key: str = None
     urls: List[str] = field(default_factory=list)
     properties: dict = field(default_factory=dict)
     _mimetype: str = None  # eg: image/jpeg
-    _stored: bool = field(default=False, repr=False, metadata=config(exclude=lambda _: True)) # always exclude
+    _stored: bool = field(default=False, repr=False, metadata=config(exclude=lambda _: True))  # always exclude
 
     def store(self: Media, override_storages: List = None, url: str = "url-not-available"):
         # stores the media into the provided/available storages [Storage]
         # repeats the process for its properties, in case they have inner media themselves
         # for now it only goes down 1 level but it's easy to make it recursive if needed
         storages = override_storages or ArchivingContext.get("storages")
         if not len(storages):
             logger.warning(f"No storages found in local context or provided directly for {self.filename}.")
             return
 
         for s in storages:
-            s.store(self, url)
-            # Media can be inside media properties, examples include transformations on original media
-            for prop in self.properties.values():
-                if isinstance(prop, Media):
-                    s.store(prop, url)
-                if isinstance(prop, list):
-                    for prop_media in prop:
-                        if isinstance(prop_media, Media):
-                            s.store(prop_media, url)
+            for any_media in self.all_inner_media(include_self=True):
+                s.store(any_media, url)
+
+    def all_inner_media(self, include_self=False):
+        """ Media can be inside media properties, examples include transformations on original media.
+        This function returns a generator for all the inner media.        
+        """
+        if include_self: yield self
+        for prop in self.properties.values():
+            if isinstance(prop, Media): yield prop
+            if isinstance(prop, list):
+                for prop_media in prop:
+                    if isinstance(prop_media, Media): yield prop_media
 
     def is_stored(self) -> bool:
-        return len(self.urls) > 0
+        return len(self.urls) > 0 and len(self.urls) == len(ArchivingContext.get("storages"))
 
     def set(self, key: str, value: Any) -> Media:
         self.properties[key] = value
         return self
 
     def get(self, key: str, default: Any = None) -> Any:
         return self.properties.get(key, default)
@@ -67,7 +70,10 @@
         self._mimetype = v
 
     def is_video(self) -> bool:
         return self.mimetype.startswith("video")
 
     def is_audio(self) -> bool:
         return self.mimetype.startswith("audio")
+    
+    def is_image(self) -> bool:
+        return self.mimetype.startswith("image")
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/core/metadata.py` & `auto_archiver-0.6.0/src/auto_archiver/core/metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 
 from __future__ import annotations
-from ast import List, Set
-from typing import Any, Union, Dict
+from typing import Any, List, Union, Dict
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 import datetime
 from urllib.parse import urlparse
 from dateutil.parser import parse as parse_dt
 from .media import Media
 from .context import ArchivingContext
@@ -85,15 +84,16 @@
     def get_url(self) -> str:
         url = self.get("url")
         assert type(url) is str and len(url) > 0, "invalid URL"
         return url
 
     def set_content(self, content: str) -> Metadata:
         # a dump with all the relevant content
-        return self.set("content", content)
+        append_content = (self.get("content", "") + content + "\n").strip()
+        return self.set("content", append_content)
 
     def set_title(self, title: str) -> Metadata:
         return self.set("title", title)
 
     def get_title(self) -> str:
         return self.get("title")
 
@@ -132,10 +132,14 @@
     def set_final_media(self, final: Media) -> Metadata:
         """final media is a special type of media: if you can show only 1 this is it, it's useful for some DBs like GsheetDb"""
         self.add_media(final, "_final_media")
 
     def get_final_media(self) -> Media:
         _default = self.media[0] if len(self.media) else None
         return self.get_media_by_id("_final_media", _default)
+    
+    def get_all_media(self) -> List[Media]:
+        # returns a list with all the media and inner media
+        return [inner for m in self.media for inner in m.all_inner_media(True)]
 
     def __str__(self) -> str:
         return self.__repr__()
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/core/orchestrator.py` & `auto_archiver-0.6.0/src/auto_archiver/core/orchestrator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from __future__ import annotations
-from ast import List
-from typing import Union
+from typing import Generator, Union, List
 
 from .context import ArchivingContext
 
 from ..archivers import Archiver
 from ..feeders import Feeder
 from ..formatters import Formatter
 from ..storages import Storage
 from ..enrichers import Enricher
 from ..databases import Database
-from .media import Media
 from .metadata import Metadata
 
 import tempfile, traceback
 from loguru import logger
 
 
 class ArchivingOrchestrator:
@@ -25,17 +23,17 @@
         self.archivers: List[Archiver] = config.archivers
         self.databases: List[Database] = config.databases
         self.storages: List[Storage] = config.storages
         ArchivingContext.set("storages", self.storages, keep_on_reset=True)
 
         for a in self.archivers: a.setup()
 
-    def feed(self) -> None:
+    def feed(self) -> Generator[Metadata]:
         for item in self.feeder:
-            self.feed_item(item)
+            yield self.feed_item(item)
 
     def feed_item(self, item: Metadata) -> Metadata:
         try:
             ArchivingContext.reset()
             with tempfile.TemporaryDirectory(dir="./") as tmp_dir:
                 ArchivingContext.set_tmp_dir(tmp_dir)
                 return self.archive(item)
@@ -89,32 +87,34 @@
         # 3 - call archivers until one succeeds
         for a in self.archivers:
             logger.info(f"Trying archiver {a.name} for {url}")
             try:
                 # Q: should this be refactored so it's just a.download(result)?
                 result.merge(a.download(result))
                 if result.is_success(): break
-            except Exception as e: logger.error(f"Unexpected error with archiver {a.name}: {e}")
+            except Exception as e: logger.error(f"Unexpected error with archiver {a.name}: {e}: {traceback.format_exc()}")
 
         # what if an archiver returns multiple entries and one is to be part of HTMLgenerator?
         # should it call the HTMLgenerator as if it's not an enrichment?
         # eg: if it is enable: generates an HTML with all the returned media, should it include enrichers? yes
         # then how to execute it last? should there also be post-processors? are there other examples?
         # maybe as a PDF? or a Markdown file
 
         # 4 - call enrichers: have access to archived content, can generate metadata and Media
         # eg: screenshot, wacz, webarchive, thumbnails
         for e in self.enrichers:
             try: e.enrich(result)
-            except Exception as exc: logger.error(f"Unexpected error with enricher {e.name}: {exc}")
+            except Exception as exc: logger.error(f"Unexpected error with enricher {e.name}: {exc}: {traceback.format_exc()}")
 
         # 5 - store media
         # looks for Media in result.media and also result.media[x].properties (as list or dict values)
         result.store()
 
+        #TODO: remove any duplicate media, if hash is available
+
         # 6 - format and store formatted if needed
         # enrichers typically need access to already stored URLs etc
         if (final_media := self.formatter.format(result)):
             final_media.store(url=url)
             result.set_final_media(final_media)
 
         if result.is_empty():
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/core/step.py` & `auto_archiver-0.6.0/src/auto_archiver/core/step.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             self.__setattr__(k, v)
 
     @staticmethod
     def configs() -> dict: return {}
 
     def init(name: str, config: dict, child: Type[Step]) -> Step:
         """
-        looks into direct subclasses of child for name and returns such ab object
+        looks into direct subclasses of child for name and returns such an object
         TODO: cannot find subclasses of child.subclasses
         """
         for sub in child.__subclasses__():
             if sub.name == name:
                 return sub(config)
         raise ClassFoundException(f"Unable to initialize STEP with {name=}, check your configuration file/step names, and make sure you made the step discoverable by putting it into __init__.py")
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/databases/console_db.py` & `auto_archiver-0.6.0/src/auto_archiver/databases/console_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/databases/csv_db.py` & `auto_archiver-0.6.0/src/auto_archiver/databases/csv_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/databases/database.py` & `auto_archiver-0.6.0/src/auto_archiver/databases/database.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/databases/gsheet_db.py` & `auto_archiver-0.6.0/src/auto_archiver/databases/gsheet_db.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,26 +48,40 @@
         # self._safe_status_update(item, 'done')
 
         cell_updates = []
         row_values = gw.get_row(row)
 
         def batch_if_valid(col, val, final_value=None):
             final_value = final_value or val
-            if val and gw.col_exists(col) and gw.get_cell(row_values, col) == '':
-                cell_updates.append((row, col, final_value))
+            try:
+                if val and gw.col_exists(col) and gw.get_cell(row_values, col) == '':
+                    cell_updates.append((row, col, final_value))
+            except Exception as e:
+                logger.error(f"Unable to batch {col}={final_value} due to {e}")
 
         cell_updates.append((row, 'status', item.status))
 
         media: Media = item.get_final_media()
         if hasattr(media, "urls"):
             batch_if_valid('archive', "\n".join(media.urls))
         batch_if_valid('date', True, datetime.datetime.utcnow().replace(tzinfo=datetime.timezone.utc).isoformat())
         batch_if_valid('title', item.get_title())
-        batch_if_valid('text', item.get("content", "")[:500])
+        batch_if_valid('text', item.get("content", ""))
         batch_if_valid('timestamp', item.get_timestamp())
+        if media: batch_if_valid('hash', media.get("hash", "not-calculated"))
+
+        # merge all pdq hashes into a single string, if present
+        pdq_hashes = []
+        all_media = item.get_all_media()
+        for m in all_media:
+            if pdq := m.get("pdq_hash"):
+                pdq_hashes.append(pdq)
+        if len(pdq_hashes):
+            batch_if_valid('pdq_hash', ",".join(pdq_hashes))
+
         if (screenshot := item.get_media_by_id("screenshot")) and hasattr(screenshot, "urls"):
             batch_if_valid('screenshot', "\n".join(screenshot.urls))
 
         if (thumbnail := item.get_first_image("thumbnail")):
             if hasattr(thumbnail, "urls"):
                 batch_if_valid('thumbnail', f'=IMAGE("{thumbnail.urls[0]}")')
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/enrichers/enricher.py` & `auto_archiver-0.6.0/src/auto_archiver/enrichers/enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/enrichers/hash_enricher.py` & `auto_archiver-0.6.0/src/auto_archiver/enrichers/hash_enricher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import hashlib
 from loguru import logger
 
 from . import Enricher
-from ..core import Metadata
+from ..core import Metadata, ArchivingContext
 
 
 class HashEnricher(Enricher):
     """
     Calculates hashes for Media instances
     """
     name = "hash_enricher"
 
     def __init__(self, config: dict) -> None:
         # without this STEP.__init__ is not called
         super().__init__(config)
         algo_choices = self.configs()["algorithm"]["choices"]
         assert self.algorithm in algo_choices, f"Invalid hash algorithm selected, must be one of {algo_choices} (you selected {self.algorithm})."
         self.chunksize = int(self.chunksize)
+        ArchivingContext.set("hash_enricher.algorithm", self.algorithm, keep_on_reset=True)
 
     @staticmethod
     def configs() -> dict:
         return {
             "algorithm": {"default": "SHA-256", "help": "hash algorithm to use", "choices": ["SHA-256", "SHA3-512"]},
             "chunksize": {"default": 1.6e7, "help": "number of bytes to use when reading files in chunks (if this value is too large you will run out of RAM), default is 16MB"},
         }
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/enrichers/screenshot_enricher.py` & `auto_archiver-0.6.0/src/auto_archiver/enrichers/screenshot_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/enrichers/thumbnail_enricher.py` & `auto_archiver-0.6.0/src/auto_archiver/enrichers/thumbnail_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/enrichers/wayback_enricher.py` & `auto_archiver-0.6.0/src/auto_archiver/enrichers/wayback_enricher.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         return {
             "timeout": {"default": 15, "help": "seconds to wait for successful archive confirmation from wayback, if more than this passes the result contains the job_id so the status can later be checked manually."},
             "key": {"default": None, "help": "wayback API key. to get credentials visit https://archive.org/account/s3.php"},
             "secret": {"default": None, "help": "wayback API secret. to get credentials visit https://archive.org/account/s3.php"}
         }
 
     def download(self, item: Metadata) -> Metadata:
+        # this new Metadata object is required to avoid duplication
         result = Metadata()
         result.merge(item)
         if self.enrich(result):
             return result.success("wayback")
 
     def enrich(self, to_enrich: Metadata) -> bool:
         url = to_enrich.get_url()
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/enrichers/whisper_enricher.py` & `auto_archiver-0.6.0/src/auto_archiver/enrichers/whisper_enricher.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         self.timeout = int(self.timeout)
 
     @staticmethod
     def configs() -> dict:
         return {
             "api_endpoint": {"default": "https://whisper.spoettel.dev/api/v1", "help": "WhisperApi api endpoint"},
             "api_key": {"default": None, "help": "WhisperApi api key for authentication"},
+            "include_srt": {"default": False, "help": "Whether to include a subtitle SRT (SubRip Subtitle file) for the video (can be used in video players)."},
             "timeout": {"default": 90, "help": "How many seconds to wait at most for a successful job completion."},
             "action": {"default": "translation", "help": "which Whisper operation to execute", "choices": ["transcript", "translation", "language_detection"]},
 
         }
 
     def enrich(self, to_enrich: Metadata) -> None:
         if not self._get_s3_storage():
@@ -54,16 +55,21 @@
         job_results = self.check_jobs(job_results)
 
         for i, m in enumerate(to_enrich.media):
             if m.is_video() or m.is_audio():
                 job_id = to_enrich.media[i].get("whisper_model")["job_id"]
                 to_enrich.media[i].set("whisper_model", {
                     "job_id": job_id,
-                    **job_results[job_id]
+                    **(job_results[job_id] if job_results[job_id] else {"result": "incomplete or failed job"})
                 })
+                # append the extracted text to the content of the post so it gets written to the DBs like gsheets text column
+                if job_results[job_id]:
+                    for k,v in job_results[job_id].items():
+                        if "_text" in k and len(v):
+                            to_enrich.set_content(f"\n[automatic video transcript]: {v}")
 
     def submit_job(self, media: Media):
         s3 = self._get_s3_storage()
         s3_url = s3.get_cdn_url(media)
         assert s3_url in media.urls, f"Could not find S3 url ({s3_url}) in list of stored media urls "
         payload = {
             "url": s3_url,
@@ -77,15 +83,15 @@
 
     def check_jobs(self, job_results: dict):
         start_time = time.time()
         all_completed = False
         while not all_completed and (time.time() - start_time) <= self.timeout:
             all_completed = True
             for job_id in job_results:
-                if job_results[job_id]: continue
+                if job_results[job_id] != False: continue
                 all_completed = False  # at least one not ready
                 try: job_results[job_id] = self.check_job(job_id)
                 except Exception as e:
                     logger.error(f"Failed to check {job_id=} with error {e}\n{traceback.format_exc()}")
             if not all_completed: time.sleep(3)
         return job_results
 
@@ -104,16 +110,19 @@
             for art_id, artifact in enumerate(r_res.json()):
                 subtitle = []
                 full_text = []
                 for i, d in enumerate(artifact.get("data")):
                     subtitle.append(f"{i+1}\n{d.get('start')} --> {d.get('end')}\n{d.get('text').strip()}")
                     full_text.append(d.get('text').strip())
                 if not len(subtitle): continue
-                result[f"artifact_{art_id}_subtitle"] = "\n".join(subtitle)
+                if self.include_srt: result[f"artifact_{art_id}_subtitle"] = "\n".join(subtitle)
                 result[f"artifact_{art_id}_text"] = "\n".join(full_text)
+            # call /delete endpoint on timely success
+            r_del = requests.delete(f'{self.api_endpoint}/jobs/{job_id}', headers={'Authorization': f'Bearer {self.api_key}'})
+            logger.debug(f"DELETE whisper {job_id=} result: {r_del.status_code}")
             return result
         return False
 
     def _get_s3_storage(self) -> S3Storage:
         try:
             return next(s for s in ArchivingContext.get("storages") if s.__class__ == S3Storage)
         except:
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/feeders/cli_feeder.py` & `auto_archiver-0.6.0/src/auto_archiver/feeders/cli_feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/feeders/feeder.py` & `auto_archiver-0.6.0/src/auto_archiver/feeders/feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/feeders/gsheet_feeder.py` & `auto_archiver-0.6.0/src/auto_archiver/feeders/gsheet_feeder.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 "use_sheet_names_in_stored_paths": {
                     "default": True,
                     "help": "if True the stored files path will include 'workbook_name/worksheet_name/...'",
                 }
             })
 
     def __iter__(self) -> Metadata:
-        sh = self.gsheets_client.open(self.sheet)
+        sh = self.open_sheet()
         for ii, wks in enumerate(sh.worksheets()):
             if not self.should_process_sheet(wks.title):
                 logger.debug(f"SKIPPED worksheet '{wks.title}' due to allow/block rules")
                 continue
 
             logger.info(f'Opening worksheet {ii=}: {wks.title=} header={self.header}')
             gw = GWorksheet(wks, header_row=self.header, columns=self.columns)
@@ -60,16 +60,24 @@
                 status = gw.get_cell(row, 'status', fresh=original_status in ['', None])
                 # TODO: custom status parser(?) aka should_retry_from_status
                 if status not in ['', None]: continue
 
                 # All checks done - archival process starts here
                 m = Metadata().set_url(url)
                 ArchivingContext.set("gsheet", {"row": row, "worksheet": gw}, keep_on_reset=True)
-                if self.use_sheet_names_in_stored_paths:
-                    ArchivingContext.set("folder", os.path.join(slugify(self.sheet), slugify(wks.title)), True)
+                if gw.get_cell_or_default(row, 'folder', "") is None:
+                    folder = ''
+                else:
+                    folder = slugify(gw.get_cell_or_default(row, 'folder', "").strip())
+                if len(folder):
+                    if self.use_sheet_names_in_stored_paths:
+                        ArchivingContext.set("folder", os.path.join(folder, slugify(self.sheet), slugify(wks.title)), True)
+                    else:
+                        ArchivingContext.set("folder", folder, True)
+
                 yield m
 
             logger.success(f'Finished worksheet {wks.title}')
 
     def should_process_sheet(self, sheet_name: str) -> bool:
         if len(self.allow_worksheets) and sheet_name not in self.allow_worksheets:
             # ALLOW rules exist AND sheet name not explicitly allowed
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/formatters/formatter.py` & `auto_archiver-0.6.0/src/auto_archiver/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/formatters/html_formatter.py` & `auto_archiver-0.6.0/src/auto_archiver/formatters/html_formatter.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from jinja2 import Environment, FileSystemLoader
 from urllib.parse import quote
 from loguru import logger
 
 from ..version import __version__
 from ..core import Metadata, Media, ArchivingContext
 from . import Formatter
+from ..enrichers import HashEnricher
 
 
 @dataclass
 class HtmlFormatter(Formatter):
     name = "html_formatter"
 
     def __init__(self, config: dict) -> None:
@@ -42,19 +43,24 @@
             media=item.media,
             metadata=item.metadata,
             version=__version__
         )
         html_path = os.path.join(ArchivingContext.get_tmp_dir(), f"formatted{str(uuid.uuid4())}.html")
         with open(html_path, mode="w", encoding="utf-8") as outf:
             outf.write(content)
-        return Media(filename=html_path)
+        final_media = Media(filename=html_path)
 
+        he = HashEnricher({"hash_enricher": {"algorithm": ArchivingContext.get("hash_enricher.algorithm"), "chunksize": 1.6e7}})
+        if len(hd := he.calculate_hash(final_media.filename)):
+            final_media.set("hash", f"{he.algorithm}:{hd}")
+
+        return final_media
 
-# JINJA helper filters
 
+# JINJA helper filters
 class JinjaHelpers:
     @staticmethod
     def is_list(v) -> bool:
         return isinstance(v, list)
 
     @staticmethod
     def is_video(s: str) -> bool:
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/formatters/templates/html_template.html` & `auto_archiver-0.6.0/src/auto_archiver/formatters/templates/html_template.html`

 * *Files 4% similar despite different names*

```diff
@@ -121,15 +121,22 @@
                     <p></p>
                     <div>
                         <b class="collapsible" title="expand">{{ prop }}:</b>
                         <p></p>
                         <div class="collapsible-content">
                             {% for subprop in m.properties[prop] %}
                             {% if subprop | is_media %}
-                            {{ macros.display_media(subprop, false, url) }}
+                            {{ macros.display_media(subprop, true, url) }}
+
+                            <ul>
+                                {% for subprop_prop in subprop.properties %}
+                                <li><b>{{ subprop_prop }}:</b> {{ macros.copy_urlize(subprop.properties[subprop_prop]) }}</li>
+                                {% endfor %}
+                            </ul>
+
                             {% else %}
                             {{ subprop }}
                             {% endif %}
                             {% endfor %}
                         </div>
                     </div>
                     <p></p>
@@ -158,15 +165,16 @@
             <td>
                 {{ macros.copy_urlize(metadata[key]) }}
             </td>
         </tr>
         {% endfor %}
     </table>
 
-    <p style="text-align:center;">Made with <a href="https://github.com/bellingcat/auto-archiver">bellingcat/auto-archiver</a> v{{ version }}</p>
+    <p style="text-align:center;">Made with <a
+            href="https://github.com/bellingcat/auto-archiver">bellingcat/auto-archiver</a> v{{ version }}</p>
 </body>
 <script defer>
     // notification logic
     const notification = document.getElementById("notification");
 
     function showNotification(message, miliseconds) {
         notification.style.display = "block";
@@ -197,15 +205,15 @@
     })
 
     // collapsibles
     let coll = document.getElementsByClassName("collapsible");
     let i;
 
     for (i = 0; i < coll.length; i++) {
-        coll[i].addEventListener("click", function() {
+        coll[i].addEventListener("click", function () {
             this.classList.toggle("active");
             // let content = this.nextElementSibling;
             let content = this.parentElement.querySelector(".collapsible-content");
             if (content.style.display === "block") {
                 content.style.display = "none";
             } else {
                 content.style.display = "block";
```

#### html2text {}

```diff
@@ -8,19 +8,26 @@
     * type: {{ m.mimetype }}
     * {% for prop in m.properties %} {%
       if m.properties[prop] | is_list
       %}
       {{ prop }}:
       {% for subprop in m.properties
       [prop] %} {% if subprop |
-      is_media %} {                     {{ macros.display_media(m, true, url)
-      { macros.display_media(subprop,   }}
-      false, url) }} {% else %} {
-      { subprop }} {% endif %} {%
-      endfor %}
+      is_media %} {
+      { macros.display_media(subprop,
+      true, url) }}
+          o {% for subprop_prop in      {{ macros.display_media(m, true, url)
+            subprop.properties %}       }}
+          o {{ subprop_prop }}: {
+            { macros.copy_urlize
+            (subprop.properties
+            [subprop_prop]) }}
+          o {% endfor %}
+      {% else %} {{ subprop }} {% endif
+      %} {% endfor %}
     * {% elif m.properties[prop] |
       string | length > 1 %}
     * {{ prop }}: {{ macros.copy_urlize
       (m.properties[prop]) }}
     * {% endif %} {% endfor %}
 ***** metadata *****
 key       value
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/formatters/templates/macros.html` & `auto_archiver-0.6.0/src/auto_archiver/formatters/templates/macros.html`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/storages/gd.py` & `auto_archiver-0.6.0/src/auto_archiver/storages/gd.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/storages/local.py` & `auto_archiver-0.6.0/src/auto_archiver/storages/local.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/storages/s3.py` & `auto_archiver-0.6.0/src/auto_archiver/storages/s3.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver/storages/storage.py` & `auto_archiver-0.6.0/src/auto_archiver/storages/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     def init(name: str, config: dict) -> Storage:
         # only for typing...
         return Step.init(name, config, Storage)
 
     def store(self, media: Media, url: str) -> None:
         if media.is_stored(): 
-            logger.debug(f"{self.key} already stored, skipping")
+            logger.debug(f"{media.key} already stored, skipping")
             return
         self.set_key(media, url)
         self.upload(media)
         media.add_url(self.get_cdn_url(media))
 
     @abstractmethod
     def get_cdn_url(self, media: Media) -> str: pass
@@ -73,12 +73,12 @@
         elif self.path_generator == "url": path = slugify(url)
         elif self.path_generator == "random":
             path = ArchivingContext.get("random_path", str(uuid.uuid4())[:16], True)
 
         # filename_generator logic
         if self.filename_generator == "random": filename = str(uuid.uuid4())[:16]
         elif self.filename_generator == "static":
-            he = HashEnricher({"hash_enricher": {"algorithm": "SHA-256", "chunksize": 1.6e7}})
+            he = HashEnricher({"hash_enricher": {"algorithm": ArchivingContext.get("hash_enricher.algorithm"), "chunksize": 1.6e7}})
             hd = he.calculate_hash(media.filename)
             filename = hd[:24]
 
         media.key = os.path.join(folder, path, f"{filename}{ext}")
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/utils/gsheet.py` & `auto_archiver-0.6.0/src/auto_archiver/utils/gsheet.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,41 +6,47 @@
 class Gsheets(Step):
     name = "gsheets"
 
     def __init__(self, config: dict) -> None:
         # without this STEP.__init__ is not called
         super().__init__(config)
         self.gsheets_client = gspread.service_account(filename=self.service_account)
-        #TODO: config should be responsible for conversions
+        # TODO: config should be responsible for conversions
         try: self.header = int(self.header)
         except: pass
         assert type(self.header) == int, f"header ({self.header}) value must be an integer not {type(self.header)}"
-        assert self.sheet is not None, "You need to define a sheet name in your orchestration file when using gsheets."
+        assert self.sheet is not None or self.sheet_id is not None, "You need to define either a 'sheet' name or a 'sheet_id' in your orchestration file when using gsheets."
 
     @staticmethod
     def configs() -> dict:
         return {
             "sheet": {"default": None, "help": "name of the sheet to archive"},
+            "sheet_id": {"default": None, "help": "(alternative to sheet name) the id of the sheet to archive"},
             "header": {"default": 1, "help": "index of the header row (starts at 1)"},
             "service_account": {"default": "secrets/service_account.json", "help": "service account JSON file path"},
             "columns": {
                 "default": {
                     'url': 'link',
                     'status': 'archive status',
                     'folder': 'destination folder',
                     'archive': 'archive location',
                     'date': 'archive date',
                     'thumbnail': 'thumbnail',
-                    'thumbnail_index': 'thumbnail index',
                     'timestamp': 'upload timestamp',
                     'title': 'upload title',
                     'text': 'text content',
-                    'duration': 'duration',
                     'screenshot': 'screenshot',
                     'hash': 'hash',
+                    'pdq_hash': 'perceptual hashes',
                     'wacz': 'wacz',
                     'replaywebpage': 'replaywebpage',
                 },
                 "help": "names of columns in the google sheet (stringified JSON object)",
                 "cli_set": lambda cli_val, cur_val: dict(cur_val, **json.loads(cli_val))
             },
-        }
+        }
+
+    def open_sheet(self):
+        if self.sheet:
+            return self.gsheets_client.open(self.sheet)
+        else:  # self.sheet_id
+            return self.gsheets_client.open_by_key(self.sheet_id)
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/utils/gworksheet.py` & `auto_archiver-0.6.0/src/auto_archiver/utils/gworksheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,19 @@
     COLUMN_NAMES = {
         'url': 'link',
         'status': 'archive status',
         'folder': 'destination folder',
         'archive': 'archive location',
         'date': 'archive date',
         'thumbnail': 'thumbnail',
-        'thumbnail_index': 'thumbnail index',
         'timestamp': 'upload timestamp',
         'title': 'upload title',
-        'duration': 'duration',
         'screenshot': 'screenshot',
         'hash': 'hash',
+        'pdq_hash': 'perceptual hashes',
         'wacz': 'wacz',
         'replaywebpage': 'replaywebpage',
     }
 
     def __init__(self, worksheet, columns=COLUMN_NAMES, header_row=1):
         self.wks = worksheet
         self.columns = columns
@@ -94,15 +93,15 @@
     def batch_set_cell(self, cell_updates):
         """
         receives a list of [(row:int, col:str, val)] and batch updates it, the parameters are the same as in the self.set_cell() method
         """
         cell_updates = [
             {
                 'range': self.to_a1(row, col),
-                'values': [[val]]
+                'values': [[str(val)[0:49999]]]
             }
             for row, col, val in cell_updates
         ]
         self.wks.batch_update(cell_updates, value_input_option='USER_ENTERED')
 
     def to_a1(self, row: int, col: str):
         # row is 1-based
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver/utils/webdriver.py` & `auto_archiver-0.6.0/src/auto_archiver/utils/webdriver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.8/src/auto_archiver.egg-info/PKG-INFO` & `auto_archiver-0.6.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,11 @@
-Metadata-Version: 2.1
-Name: auto-archiver
-Version: 0.5.8
-Summary: Easily archive online media content
-Author: Bellingcat
-Author-email: tech@bellingcat.com
-License: MIT
-Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
-Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
-Project-URL: Bellingcat, https://www.bellingcat.com
-Keywords: archive,oosi,osint,scraping
-Platform: any
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">Auto Archiver</h1>
 
 [![PyPI version](https://badge.fury.io/py/auto-archiver.svg)](https://badge.fury.io/py/auto-archiver)
-[![Docker Image Version (latest by date)](https://img.shields.io/docker/v/bellingcat/auto-archiver?label=version&logo=docker)](https://pypi.org/project/auto-archiver/)
+[![Docker Image Version (latest by date)](https://img.shields.io/docker/v/bellingcat/auto-archiver?label=version&logo=docker)](https://hub.docker.com/r/bellingcat/auto-archiver)
 <!-- ![Docker Pulls](https://img.shields.io/docker/pulls/bellingcat/auto-archiver) -->
 <!-- [![PyPI download month](https://img.shields.io/pypi/dm/auto-archiver.svg)](https://pypi.python.org/pypi/auto-archiver/) -->
 <!-- [![Documentation Status](https://readthedocs.org/projects/vk-url-scraper/badge/?version=latest)](https://vk-url-scraper.readthedocs.io/en/latest/?badge=latest) -->
 
 
 Read the [article about Auto Archiver on bellingcat.com](https://www.bellingcat.com/resources/2022/09/22/preserve-vital-online-content-with-bellingcats-auto-archiver-tool/).
 
@@ -36,64 +16,61 @@
 1. (easiest installation) via docker
 2. (local python install) `pip install auto-archiver`
 3. (legacy/development) clone and manually install from repo (see legacy [tutorial video](https://youtu.be/VfAhcuV2tLQ))
 
 But **you always need a configuration/orchestration file**, which is where you'll configure where/what/how to archive. Make sure you read [orchestration](#orchestration).
 
 
-## How to run the auto-archiver
+## How to install and run the auto-archiver
 
 ### Option 1 - docker
 
-<details><summary><code>Docker instructions</code></summary>
-
 [![dockeri.co](https://dockerico.blankenship.io/image/bellingcat/auto-archiver)](https://hub.docker.com/r/bellingcat/auto-archiver)
 
 Docker works like a virtual machine running inside your computer, it isolates everything and makes installation simple. Since it is an isolated environment when you need to pass it your orchestration file or get downloaded media out of docker you will need to connect folders on your machine with folders inside docker with the `-v` volume flag.
 
 
 1. install [docker](https://docs.docker.com/get-docker/)
 2. pull the auto-archiver docker [image](https://hub.docker.com/r/bellingcat/auto-archiver) with `docker pull bellingcat/auto-archiver`
-3. run the docker image locally in a container: `docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver -m auto_archiver  --config secrets/orchestration.yaml` breaking this command down:
+3. run the docker image locally in a container: `docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver --config secrets/orchestration.yaml` breaking this command down:
    1. `docker run` tells docker to start a new container (an instance of the image)
    2. `--rm` makes sure this container is removed after execution (less garbage locally)
    3. `-v $PWD/secrets:/app/secrets` - your secrets folder
       1. `-v` is a volume flag which means a folder that you have on your computer will be connected to a folder inside the docker container
       2. `$PWD/secrets` points to a `secrets/` folder in your current working directory (where your console points to), we use this folder as a best practice to hold all the secrets/tokens/passwords/... you use
       3. `/app/secrets` points to the path the docker container where this image can be found
    4.  `-v $PWD/local_archive:/app/local_archive` - (optional) if you use local_storage
        1.  `-v` same as above, this is a volume instruction
        2.  `$PWD/local_archive` is a folder `local_archive/` in case you want to archive locally and have the files accessible outside docker
        3.  `/app/local_archive` is a folder inside docker that you can reference in your orchestration.yml file 
 
-</details>
-
 ### Option 2 - python package
 
 <details><summary><code>Python package instructions</code></summary>
 
 1. make sure you have python 3.8 or higher installed
 2. install the package `pip/pipenv/conda install auto-archiver`
 3. test it's installed with `auto-archiver --help`
-4. run it with your orchestration file and pass any flags you want in the command line `auto-archiver --config secrets/orchestration.yaml`
-   1. if your orchestration file is inside a `secrets/` which we advise
+4. run it with your orchestration file and pass any flags you want in the command line `auto-archiver --config secrets/orchestration.yaml` if your orchestration file is inside a `secrets/`, which we advise
+   
+You will also need [ffmpeg](https://www.ffmpeg.org/), [firefox](https://www.mozilla.org/en-US/firefox/new/) and [geckodriver](https://github.com/mozilla/geckodriver/releases), and optionally [fonts-noto](https://fonts.google.com/noto). Similar to the local installation. 
 
 </details>
 
 
 ### Option 3 - local installation
 This can also be used for development.
 
 <details><summary><code>Legacy instructions, only use if docker/package is not an option</code></summary>
 
 
 Install the following locally:
 1. [ffmpeg](https://www.ffmpeg.org/) must also be installed locally for this tool to work. 
 2. [firefox](https://www.mozilla.org/en-US/firefox/new/) and [geckodriver](https://github.com/mozilla/geckodriver/releases) on a path folder like `/usr/local/bin`. 
-3. [fonts-noto](https://fonts.google.com/noto) to deal with multiple unicode characters during selenium/geckodriver's screenshots: `sudo apt install fonts-noto -y`. 
+3. (optional) [fonts-noto](https://fonts.google.com/noto) to deal with multiple unicode characters during selenium/geckodriver's screenshots: `sudo apt install fonts-noto -y`. 
 
 Clone and run:
 1. `git clone https://github.com/bellingcat/auto-archiver`
 2. `pipenv install`
 3. `pipenv run python -m src.auto_archiver --config secrets/orchestration.yaml`
 
 
@@ -103,19 +80,17 @@
 The archiver work is orchestrated by the following workflow (we call each a **step**): 
 1. **Feeder** gets the links (from a spreadsheet, from the console, ...)
 2. **Archiver** tries to archive the link (twitter, youtube, ...)
 3. **Enricher** adds more info to the content (hashes, thumbnails, ...)
 4. **Formatter** creates a report from all the archived content (HTML, PDF, ...)
 5. **Database** knows what's been archived and also stores the archive result (spreadsheet, CSV, or just the console)
 
-To check all available steps (which archivers, storages, databses, ...) exist check the [example.orchestration.yaml](example.orchestration.yaml).
-
-The great thing is you configure all the workflow in your `orchestration.yaml` file which we advise you put into a `secrets/` folder and don't share it with others because it will contain passwords and other secrets. 
+To setup an auto-archiver instance create an `orchestration.yaml` which contains the workflow you would like. We advise you put this file into a `secrets/` folder and do not share it with others because it will contain passwords and other secrets. 
 
-The structure of orchestration file is split into 2 parts: `steps` (what **steps** to use) and `configs` (how those steps should behave), here's a simplification:
+The structure of orchestration file is split into 2 parts: `steps` (what **steps** to use) and `configurations` (how those steps should behave), here's a simplification:
 ```yaml
 # orchestration.yaml content
 steps:
   feeder: gsheet_feeder
   archivers: # order matters
     - youtubedl_archiver
   enrichers:
@@ -129,18 +104,20 @@
 configurations:
   gsheet_feeder:
     sheet: "your google sheet name"
     header: 2 # row with header for your sheet
   # ... configurations for the other steps here ...
 ```
 
+To see all available `steps` (which archivers, storages, databses, ...) exist check the [example.orchestration.yaml](example.orchestration.yaml).
+
 All the `configurations` in the `orchestration.yaml` file (you can name it differently but need to pass it in the `--config FILENAME` argument) can be seen in the console by using the `--help` flag. They can also be overwritten, for example if you are using the `cli_feeder` to archive from the command line and want to provide the URLs you should do:
 
 ```bash
-auto-archiver --config orchestration.yaml --cli_feeder.urls="url1,url2,url3"
+auto-archiver --config secrets/orchestration.yaml --cli_feeder.urls="url1,url2,url3"
 ```
 
 Here's the complete workflow that the auto-archiver goes through:
 ```mermaid
 graph TD
     s((start)) --> F(fa:fa-table Feeder)
     F -->|get and clean URL| D1{fa:fa-database Database}
@@ -163,61 +140,100 @@
     * if you use private channels you need to add `channel_invites` and set `join_channels=true` at least once
   * [ ] (optional for VK) a `vk_config.v2.json`
   * [ ] (optional for using GoogleDrive storage) `gd-token.json` (see [help script](scripts/create_update_gdrive_oauth_token.py))
   * [ ] (optional for instagram) `instaloader.session` file which appears after the 1st run and login in instagram
   * [ ] (optional for browsertrix) `profile.tar.gz` file
 
 #### Example invocations
-These assume you've installed with pipenv, see docker section above for how to run through docker
+The recommended way to run the auto-archiver is through Docker. The invocations below will run the auto-archiver Docker image using a configuration file that you have specified
+
+```bash
+# all the configurations come from ./secrets/orchestration.yaml
+docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver --config secrets/orchestration.yaml
+# uses the same configurations but for another google docs sheet 
+# with a header on row 2 and with some different column names
+# notice that columns is a dictionary so you need to pass it as JSON and it will override only the values provided
+docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver --config secrets/orchestration.yaml --gsheet_feeder.sheet="use it on another sheets doc" --gsheet_feeder.header=2 --gsheet_feeder.columns='{"url": "link"}'
+# all the configurations come from orchestration.yaml and specifies that s3 files should be private
+docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver --config secrets/orchestration.yaml --s3_storage.private=1
+```
+
+The auto-archiver can also be run locally, if pre-requisites are correctly configured. Equivalent invocations are below.
 
 ```bash
-# all the configurations come from ./orchestration.yaml
-auto-archiver
 # all the configurations come from ./secrets/orchestration.yaml
 auto-archiver --config secrets/orchestration.yaml
 # uses the same configurations but for another google docs sheet 
 # with a header on row 2 and with some different column names
 # notice that columns is a dictionary so you need to pass it as JSON and it will override only the values provided
-auto-archiver --config orchestration.yaml --gsheet_feeder.sheet="use it on another sheets doc" --gsheet_feeder.header=2 --gsheet_feeder.columns='{"url": "link"}'
+auto-archiver --config secrets/orchestration.yaml --gsheet_feeder.sheet="use it on another sheets doc" --gsheet_feeder.header=2 --gsheet_feeder.columns='{"url": "link"}'
 # all the configurations come from orchestration.yaml and specifies that s3 files should be private
-auto-archiver --s3_storage.private=1
+auto-archiver --config secrets/orchestration.yaml --s3_storage.private=1
 ```
 
 ### Extra notes on configuration
 #### Google Drive
 To use Google Drive storage you need the id of the shared folder in the `config.yaml` file which must be shared with the service account eg `autoarchiverservice@auto-archiver-111111.iam.gserviceaccount.com` and then you can use `--storage=gd`
 
 #### Telethon + Instagram with telegram bot
 The first time you run, you will be prompted to do a authentication with the phone number associated, alternatively you can put your `anon.session` in the root.
 
 
 ## Running on Google Sheets Feeder (gsheet_feeder)
 The `--gseets_feeder.sheet` property is the name of the Google Sheet to check for URLs. 
 This sheet must have been shared with the Google Service account used by `gspread`. 
-This sheet must also have specific columns (case-insensitive) in the `header` row - see [Gsheet.configs](src/auto_archiver/utils/gsheet.py) for all their names.
+This sheet must also have specific columns (case-insensitive) in the `header` as specified in [Gsheet.configs](src/auto_archiver/utils/gsheet.py). The default names of these columns and their purpose is:
+
+Inputs:
+
+* **Link** *(required)*: the URL of the post to archive
+* **Destination folder**: custom folder for archived file (regardless of storage)
+
+Outputs:
+* **Archive status** *(required)*: Status of archive operation
+* **Archive location**: URL of archived post
+* **Archive date**: Date archived
+* **Thumbnail**: Embeds a thumbnail for the post in the spreadsheet
+* **Timestamp**: Timestamp of original post
+* **Title**: Post title
+* **Text**: Post text
+* **Screenshot**: Link to screenshot of post
+* **Hash**: Hash of archived HTML file (which contains hashes of post media) - for checksums/verification
+* **Perceptual Hash**: Perceptual hashes of found images - these can be used for de-duplication of content
+* **WACZ**: Link to a WACZ web archive of post
+* **ReplayWebpage**: Link to a ReplayWebpage viewer of the WACZ archive
 
-For example, for use with this spreadsheet:
+For example, this is a spreadsheet configured with all of the columns for the auto archiver and a few URLs to archive. (Note that the column names are not case sensitive.)
 
-![A screenshot of a Google Spreadsheet with column headers defined as above, and several Youtube and Twitter URLs in the "Media URL" column](docs/demo-before.png)
+![A screenshot of a Google Spreadsheet with column headers defined as above, and several Youtube and Twitter URLs in the "Link" column](docs/demo-before.png)
+
+Now the auto archiver can be invoked, with this command in this example: `docker run --rm -v $PWD/secrets:/app/secrets -v $PWD/local_archive:/app/local_archive bellingcat/auto-archiver:dockerize --config secrets/orchestration-global.yaml --gsheet_feeder.sheet "Auto archive test 2023-2"`. Note that the sheet name has been overridden/specified in the command line invocation.
 
 When the auto archiver starts running, it updates the "Archive status" column.
-![A screenshot of a Google Spreadsheet with column headers defined as above, and several Youtube and Twitter URLs in the "Media URL" column. The auto archiver has added "archive in progress" to one of the status columns.](docs/demo-progress.png)
+
+![A screenshot of a Google Spreadsheet with column headers defined as above, and several Youtube and Twitter URLs in the "Link" column. The auto archiver has added "archive in progress" to one of the status columns.](docs/demo-progress.png)
+
 The links are downloaded and archived, and the spreadsheet is updated to the following:
+
 ![A screenshot of a Google Spreadsheet with videos archived and metadata added per the description of the columns above.](docs/demo-after.png)
+
 Note that the first row is skipped, as it is assumed to be a header row (`--gsheet_feeder.header=1` and you can change it if you use more rows above). Rows with an empty URL column, or a non-empty archive column are also skipped. All sheets in the document will be checked.
 
+The "archive location" link contains the path of the archived file, in local storage, S3, or in Google Drive.
+
+![The archive result for a link in the demo sheet.](docs/demo-archive.png)
 
 ---
 ## Development
 Use `python -m src.auto_archiver --config secrets/orchestration.yaml` to run from the local development environment.
 
 #### Docker development
 working with docker locally:
   * `docker build . -t auto-archiver` to build a local image
-  * `docker run --rm -v $PWD/secrets:/app/secrets aa --config secrets/config.yaml`
+  * `docker run --rm -v $PWD/secrets:/app/secrets auto-archiver  --config secrets/orchestration.yaml`
     * to use local archive, also create a volume `-v` for it by adding `-v $PWD/local_archive:/app/local_archive`
 
 
 release to docker hub
   * `docker image tag auto-archiver bellingcat/auto-archiver:latest`
   * `docker push bellingcat/auto-archiver`
```

### Comparing `auto_archiver-0.5.8/src/auto_archiver.egg-info/SOURCES.txt` & `auto_archiver-0.6.0/src/auto_archiver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/auto_archiver/__init__.py
 src/auto_archiver/__main__.py
-src/auto_archiver/auto_auto_archive.py
 src/auto_archiver/version.py
 src/auto_archiver.egg-info/PKG-INFO
 src/auto_archiver.egg-info/SOURCES.txt
 src/auto_archiver.egg-info/dependency_links.txt
 src/auto_archiver.egg-info/entry_points.txt
 src/auto_archiver.egg-info/not-zip-safe
 src/auto_archiver.egg-info/requires.txt
@@ -29,21 +28,23 @@
 src/auto_archiver/core/config.py
 src/auto_archiver/core/context.py
 src/auto_archiver/core/media.py
 src/auto_archiver/core/metadata.py
 src/auto_archiver/core/orchestrator.py
 src/auto_archiver/core/step.py
 src/auto_archiver/databases/__init__.py
+src/auto_archiver/databases/api_db.py
 src/auto_archiver/databases/console_db.py
 src/auto_archiver/databases/csv_db.py
 src/auto_archiver/databases/database.py
 src/auto_archiver/databases/gsheet_db.py
 src/auto_archiver/enrichers/__init__.py
 src/auto_archiver/enrichers/enricher.py
 src/auto_archiver/enrichers/hash_enricher.py
+src/auto_archiver/enrichers/pdq_hash_enricher.py
 src/auto_archiver/enrichers/screenshot_enricher.py
 src/auto_archiver/enrichers/thumbnail_enricher.py
 src/auto_archiver/enrichers/wacz_enricher.py
 src/auto_archiver/enrichers/wayback_enricher.py
 src/auto_archiver/enrichers/whisper_enricher.py
 src/auto_archiver/feeders/__init__.py
 src/auto_archiver/feeders/cli_feeder.py
```

