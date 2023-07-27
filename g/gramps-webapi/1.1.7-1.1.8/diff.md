# Comparing `tmp/gramps-webapi-1.1.7.tar.gz` & `tmp/gramps-webapi-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gramps-webapi-1.1.7.tar", last modified: Fri Jul 21 19:02:46 2023, max compression
+gzip compressed data, was "gramps-webapi-1.1.8.tar", last modified: Thu Jul 27 09:06:31 2023, max compression
```

## Comparing `gramps-webapi-1.1.7.tar` & `gramps-webapi-1.1.8.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:02:46.733732 gramps-webapi-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-21 19:02:46.733732 gramps-webapi-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:02:46.713732 gramps-webapi-1.1.7/gramps_webapi/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:02:46.717732 gramps-webapi-1.1.7/gramps_webapi/api/
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    12817 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:02:46.721732 gramps-webapi-1.1.7/gramps_webapi/api/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/citations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/export_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/face_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/facts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/families.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/import_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/importers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/living.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/match.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/name_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/name_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/notes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/people.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/places.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    32597 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/trees.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    20058 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    46112 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/resources/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13165 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/api/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:02:46.721732 gramps-webapi-1.1.7/gramps_webapi/auth/
--rw-r--r--   0 runner    (1001) docker     (123)    14659 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/auth/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/auth/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/auth/sql_guid.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:02:46.725732 gramps-webapi-1.1.7/gramps_webapi/data/
--rw-r--r--   0 runner    (1001) docker     (123)   350862 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/data/apispec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/data/empty_gramps_auth.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/data/example_gramps_auth.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   930127 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/data/haarcascade_frontalface_default.xml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/data/test_auth.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/dbloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/dbmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:02:46.725732 gramps-webapi-1.1.7/gramps_webapi/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:02:46.725732 gramps-webapi-1.1.7/gramps_webapi/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/templates/confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/templates/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/templates/reset_password_base.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/templates/reset_password_error.html
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:02:46.725732 gramps-webapi-1.1.7/gramps_webapi/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/util/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/gramps_webapi/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:02:46.713732 gramps-webapi-1.1.7/gramps_webapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-21 19:02:46.000000 gramps-webapi-1.1.7/gramps_webapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-21 19:02:46.000000 gramps-webapi-1.1.7/gramps_webapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:02:46.000000 gramps-webapi-1.1.7/gramps_webapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:02:46.000000 gramps-webapi-1.1.7/gramps_webapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-21 19:02:46.000000 gramps-webapi-1.1.7/gramps_webapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 19:02:46.000000 gramps-webapi-1.1.7/gramps_webapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-21 19:02:46.733732 gramps-webapi-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:02:46.729732 gramps-webapi-1.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:02:46.733732 gramps-webapi-1.1.7/tests/test_endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)    23353 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_citations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    36600 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    20530 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_facts.py
--rw-r--r--   0 runner    (1001) docker     (123)    48295 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_families.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_import_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_importers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_living.py
--rw-r--r--   0 runner    (1001) docker     (123)    22991 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_media_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_name_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_name_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    21252 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)    67014 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_people.py
--rw-r--r--   0 runner    (1001) docker     (123)    24741 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_places.py
--rw-r--r--   0 runner    (1001) docker     (123)    28473 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    23669 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    23885 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_timelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_trees.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    38607 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_endpoints/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_sqlauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-21 19:02:41.000000 gramps-webapi-1.1.7/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:06:31.722872 gramps-webapi-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-27 09:06:31.722872 gramps-webapi-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:06:31.690870 gramps-webapi-1.1.8/gramps_webapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:06:31.694870 gramps-webapi-1.1.8/gramps_webapi/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12817 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:06:31.706871 gramps-webapi-1.1.8/gramps_webapi/api/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/citations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/export_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/face_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/families.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/import_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/importers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/living.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/name_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/name_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/people.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/places.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32597 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20058 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46804 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/resources/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13165 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/api/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:06:31.706871 gramps-webapi-1.1.8/gramps_webapi/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)    14659 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/auth/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/auth/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/auth/sql_guid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:06:31.710871 gramps-webapi-1.1.8/gramps_webapi/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   350862 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/data/apispec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/data/empty_gramps_auth.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/data/example_gramps_auth.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   930127 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/data/haarcascade_frontalface_default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/data/test_auth.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/dbloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/dbmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:06:31.710871 gramps-webapi-1.1.8/gramps_webapi/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:06:31.710871 gramps-webapi-1.1.8/gramps_webapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/templates/confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/templates/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/templates/reset_password_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/templates/reset_password_error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:06:31.710871 gramps-webapi-1.1.8/gramps_webapi/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/util/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/gramps_webapi/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:06:31.690870 gramps-webapi-1.1.8/gramps_webapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-27 09:06:31.000000 gramps-webapi-1.1.8/gramps_webapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-27 09:06:31.000000 gramps-webapi-1.1.8/gramps_webapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 09:06:31.000000 gramps-webapi-1.1.8/gramps_webapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 09:06:31.000000 gramps-webapi-1.1.8/gramps_webapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-27 09:06:31.000000 gramps-webapi-1.1.8/gramps_webapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 09:06:31.000000 gramps-webapi-1.1.8/gramps_webapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 09:06:31.722872 gramps-webapi-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:06:31.714871 gramps-webapi-1.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:06:31.718871 gramps-webapi-1.1.8/tests/test_endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23353 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_citations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36600 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20530 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48295 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_families.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_import_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_importers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_living.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22991 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_media_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_name_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_name_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21252 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67014 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_people.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24741 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_places.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28473 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23669 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23885 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_timelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38607 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_endpoints/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_sqlauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-27 09:06:26.000000 gramps-webapi-1.1.8/tests/test_version.py
```

### Comparing `gramps-webapi-1.1.7/LICENSE` & `gramps-webapi-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/PKG-INFO` & `gramps-webapi-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramps-webapi
-Version: 1.1.7
+Version: 1.1.8
 Summary: A RESTful web API for the Gramps genealogical database.
 Home-page: https://github.com/gramps-project/web-api
 Author: Gramps Development Team
 License: AGPL v3 or greater
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gramps-webapi-1.1.7/README.md` & `gramps-webapi-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/__init__.py` & `gramps-webapi-1.1.8/gramps_webapi/__init__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/__main__.py` & `gramps-webapi-1.1.8/gramps_webapi/__main__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/_version.py` & `gramps-webapi-1.1.8/gramps_webapi/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 #
 
 # make sure to match this version with the one in apispec.yaml
-__version__ = "1.1.7"
+__version__ = "1.1.8"
```

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/__init__.py` & `gramps-webapi-1.1.8/gramps_webapi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/auth.py` & `gramps-webapi-1.1.8/gramps_webapi/api/auth.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/emails.py` & `gramps-webapi-1.1.8/gramps_webapi/api/emails.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/export.py` & `gramps-webapi-1.1.8/gramps_webapi/api/export.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/file.py` & `gramps-webapi-1.1.8/gramps_webapi/api/file.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/html.py` & `gramps-webapi-1.1.8/gramps_webapi/api/html.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/image.py` & `gramps-webapi-1.1.8/gramps_webapi/api/image.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/media.py` & `gramps-webapi-1.1.8/gramps_webapi/api/media.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/report.py` & `gramps-webapi-1.1.8/gramps_webapi/api/report.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/__init__.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/base.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/base.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/bookmarks.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/bookmarks.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/citations.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/citations.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/config.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/config.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/delete.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/delete.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/emit.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/emit.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/events.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/events.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/export_media.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/export_media.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/exporters.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/exporters.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     get_buffer_for_file,
     get_db_handle,
     get_tree_from_jwt,
     use_args,
 )
 from . import ProtectedResource
 from .emit import GrampsJSONEncoder
+from .util import check_fix_default_person
 
 
 class ExportersResource(ProtectedResource, GrampsJSONEncoder):
     """Exporters resource."""
 
     @use_args({}, location="query")
     def get(self, args: Dict) -> Response:
@@ -114,14 +115,16 @@
     )
     def post(self, args: Dict, extension: str) -> Response:
         """Create the export."""
         get_db_handle()  # to load plugins
         exporters = get_exporters(extension)
         if not exporters:
             abort(404)
+        if has_permissions({PERM_EDIT_OBJ}):
+            check_fix_default_person(get_db_handle(readonly=False))
         tree = get_tree_from_jwt()
         # remove JWT from args
         options = {k: v for k, v in args.items() if k != "jwt"}
         task = run_task(
             export_db,
             tree=tree,
             extension=extension.lower(),
```

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/face_detection.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/face_detection.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/facts.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/facts.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/families.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/families.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/file.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/file.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/filters.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/filters.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/holidays.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/holidays.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/import_media.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/import_media.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/importers.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/importers.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/living.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/living.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/match.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/match.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/media.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/media.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/metadata.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/metadata.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/name_formats.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/name_formats.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/name_groups.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/name_groups.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/notes.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/notes.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/objects.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/objects.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/people.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/people.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/places.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/places.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/relations.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/relations.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/reports.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/reports.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,45 +25,50 @@
 import re
 import time
 from typing import Dict
 
 from flask import Response, abort, current_app, jsonify, send_file
 from webargs import fields, validate
 
-from ...auth.const import PERM_VIEW_PRIVATE
+from ...auth.const import PERM_EDIT_OBJ, PERM_VIEW_PRIVATE
 from ...const import MIME_TYPES
 from ..auth import has_permissions
 from ..report import check_report_id_exists, get_reports, run_report
 from ..tasks import AsyncResult, generate_report, make_task_response, run_task
 from ..util import (
     get_buffer_for_file,
     get_db_handle,
     get_tree_from_jwt,
     use_args,
 )
 from . import ProtectedResource
 from .emit import GrampsJSONEncoder
+from .util import check_fix_default_person
 
 
 class ReportsResource(ProtectedResource, GrampsJSONEncoder):
     """Reports resource."""
 
     @use_args({}, location="query")
     def get(self, args: Dict) -> Response:
         """Get all available report attributes."""
+        if has_permissions({PERM_EDIT_OBJ}):
+            check_fix_default_person(get_db_handle(readonly=False))
         reports = get_reports(get_db_handle())
         return self.response(200, reports)
 
 
 class ReportResource(ProtectedResource, GrampsJSONEncoder):
     """Report resource."""
 
     @use_args({}, location="query")
     def get(self, args: Dict, report_id: str) -> Response:
         """Get specific report attributes."""
+        if has_permissions({PERM_EDIT_OBJ}):
+            check_fix_default_person(get_db_handle(readonly=False))
         reports = get_reports(get_db_handle(), report_id=report_id)
         if not reports:
             abort(404)
         return self.response(200, reports[0])
 
 
 class ReportFileResource(ProtectedResource, GrampsJSONEncoder):
@@ -86,14 +91,17 @@
             try:
                 report_options = json.loads(args["options"])
             except json.JSONDecodeError:
                 abort(400)
         if "of" in report_options:
             abort(422)
 
+        if has_permissions({PERM_EDIT_OBJ}):
+            check_fix_default_person(get_db_handle(readonly=False))
+
         file_name, file_type = run_report(
             db_handle=get_db_handle(),
             report_id=report_id,
             report_options=report_options,
             language=args["locale"],
         )
         report_path = current_app.config.get("REPORT_DIR")
@@ -117,14 +125,16 @@
         if "options" in args:
             try:
                 report_options = json.loads(args["options"])
             except json.JSONDecodeError:
                 abort(400)
         if "of" in report_options:
             abort(422)
+        if has_permissions({PERM_EDIT_OBJ}):
+            check_fix_default_person(get_db_handle(readonly=False))
         tree = get_tree_from_jwt()
         task = run_task(
             generate_report,
             tree=tree,
             report_id=report_id.lower(),
             options=report_options,
             view_private=has_permissions({PERM_VIEW_PRIVATE}),
```

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/repositories.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/repositories.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/search.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/search.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/sort.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/sort.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/sources.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/sources.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/tags.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/tags.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/tasks.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/tasks.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/timeline.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/timeline.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/token.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/token.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/transactions.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/transactions.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,14 +86,19 @@
                     if not self.old_unchanged(db_handle, class_name, handle, old_data):
                         abort_with_message(409, "Object has changed")
                     new_data = item["new"]
                     if new_data:
                         new_obj = from_json(json.dumps(new_data))
                     if trans_type == "delete":
                         self.handle_delete(trans, class_name, handle)
+                        if (
+                            class_name == "Person"
+                            and handle == db_handle.get_default_handle()
+                        ):
+                            db_handle.set_default_person_handle(None)
                     elif trans_type == "add":
                         self.handle_add(trans, class_name, new_obj)
                     elif trans_type == "update":
                         self.handle_commit(trans, class_name, new_obj)
                     else:
                         abort_with_message(400, "Unexpected transaction type")
                 except (KeyError, UnicodeDecodeError, json.JSONDecodeError, TypeError):
```

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/translations.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/translations.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/trees.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/trees.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/types.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/types.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/user.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/user.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/resources/util.py` & `gramps-webapi-1.1.8/gramps_webapi/api/resources/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1299,7 +1299,28 @@
     set_tree_usage(tree, usage_media=usage_media)
 
     return {
         "missing": len(checksums_handles),
         "uploaded": len(to_upload) - num_failures,
         "failures": num_failures,
     }
+
+
+def check_fix_default_person(db_handle: Union[DbReadBase, DbWriteBase]) -> None:
+    """If the db is writable, check if the default person still exists.
+
+    If it doesn't exist, set the default person to None.
+    """
+    if not isinstance(db_handle, DbWriteBase):
+        # not writable
+        return None
+    handle = db_handle.get_default_handle()
+    if not handle:
+        # default person is already empty
+        return None
+    if db_handle.has_person_handle(handle):
+        # default person exists
+        return None
+    # OK, we have a problem - default person is not empty but does not exist
+    # - set to empty
+    db_handle.set_default_person_handle(None)
+    return None
```

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/s3.py` & `gramps-webapi-1.1.8/gramps_webapi/api/s3.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/search.py` & `gramps-webapi-1.1.8/gramps_webapi/api/search.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/tasks.py` & `gramps-webapi-1.1.8/gramps_webapi/api/tasks.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/api/util.py` & `gramps-webapi-1.1.8/gramps_webapi/api/util.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/app.py` & `gramps-webapi-1.1.8/gramps_webapi/app.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/auth/__init__.py` & `gramps-webapi-1.1.8/gramps_webapi/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/auth/const.py` & `gramps-webapi-1.1.8/gramps_webapi/auth/const.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/auth/passwords.py` & `gramps-webapi-1.1.8/gramps_webapi/auth/passwords.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/auth/sql_guid.py` & `gramps-webapi-1.1.8/gramps_webapi/auth/sql_guid.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/config.py` & `gramps-webapi-1.1.8/gramps_webapi/config.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/const.py` & `gramps-webapi-1.1.8/gramps_webapi/const.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/data/apispec.yaml` & `gramps-webapi-1.1.8/gramps_webapi/data/apispec.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 00000170: 6d70 7320 616e 6420 7468 6520 6e75 6d65  mps and the nume
 00000180: 726f 7573 2066 6561 7475 7265 7320 6974  rous features it
 00000190: 2070 726f 7669 6465 7320 666f 7220 6765   provides for ge
 000001a0: 6e65 616c 6f67 6973 7473 2063 616e 2062  nealogists can b
 000001b0: 6520 666f 756e 6420 6174 2068 7474 7073  e found at https
 000001c0: 3a2f 2f67 7261 6d70 732d 7072 6f6a 6563  ://gramps-projec
 000001d0: 742e 6f72 670a 2020 7665 7273 696f 6e3a  t.org.  version:
-000001e0: 2022 312e 312e 3722 2020 2320 6d61 6b65   "1.1.7"  # make
+000001e0: 2022 312e 312e 3822 2020 2320 6d61 6b65   "1.1.8"  # make
 000001f0: 2073 7572 6520 746f 206d 6174 6368 2074   sure to match t
 00000200: 6869 7320 7665 7273 696f 6e20 7769 7468  his version with
 00000210: 2074 6865 206f 6e65 2069 6e20 5f76 6572   the one in _ver
 00000220: 7369 6f6e 2e70 790a 2020 6c69 6365 6e73  sion.py.  licens
 00000230: 653a 0a20 2020 206e 616d 653a 2022 474e  e:.    name: "GN
 00000240: 5520 4166 6665 726f 2047 656e 6572 616c  U Affero General
 00000250: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License
```

### Comparing `gramps-webapi-1.1.7/gramps_webapi/data/haarcascade_frontalface_default.xml` & `gramps-webapi-1.1.8/gramps_webapi/data/haarcascade_frontalface_default.xml`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/dbloader.py` & `gramps-webapi-1.1.8/gramps_webapi/dbloader.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/dbmanager.py` & `gramps-webapi-1.1.8/gramps_webapi/dbmanager.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/templates/confirmation.html` & `gramps-webapi-1.1.8/gramps_webapi/templates/confirmation.html`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/templates/reset_password.html` & `gramps-webapi-1.1.8/gramps_webapi/templates/reset_password.html`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/templates/reset_password_base.html` & `gramps-webapi-1.1.8/gramps_webapi/templates/reset_password_base.html`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/types.py` & `gramps-webapi-1.1.8/gramps_webapi/types.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/util/__init__.py` & `gramps-webapi-1.1.8/gramps_webapi/util/__init__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/util/celery.py` & `gramps-webapi-1.1.8/gramps_webapi/util/celery.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi/wsgi.py` & `gramps-webapi-1.1.8/gramps_webapi/wsgi.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/gramps_webapi.egg-info/PKG-INFO` & `gramps-webapi-1.1.8/gramps_webapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramps-webapi
-Version: 1.1.7
+Version: 1.1.8
 Summary: A RESTful web API for the Gramps genealogical database.
 Home-page: https://github.com/gramps-project/web-api
 Author: Gramps Development Team
 License: AGPL v3 or greater
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gramps-webapi-1.1.7/gramps_webapi.egg-info/SOURCES.txt` & `gramps-webapi-1.1.8/gramps_webapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/setup.py` & `gramps-webapi-1.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/__init__.py` & `gramps-webapi-1.1.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_cli.py` & `gramps-webapi-1.1.8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_db.py` & `gramps-webapi-1.1.8/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/__init__.py` & `gramps-webapi-1.1.8/tests/test_endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/checks.py` & `gramps-webapi-1.1.8/tests/test_endpoints/checks.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_bookmarks.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_bookmarks.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_citations.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_citations.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_config.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_config.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_delete.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_delete.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_events.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_events.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_exporters.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_exporters.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_facts.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_facts.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_families.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_families.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_file.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_file.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_filters.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_filters.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_holidays.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_holidays.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_import_media.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_import_media.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_importers.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_importers.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_living.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_living.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_media.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_media.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_media_archive.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_media_archive.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_metadata.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_metadata.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_name_formats.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_name_formats.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_name_groups.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_name_groups.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_notes.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_notes.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_people.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_people.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_places.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_places.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_post.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_post.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_put.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_put.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_relations.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_relations.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_reports.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_reports.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_repositories.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_repositories.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_s3.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_s3.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_search.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_search.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_sources.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_sources.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_tags.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_tags.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_tasks.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_tasks.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_timelines.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_timelines.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_token.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_token.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_transactions.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_transactions.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_translations.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_translations.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_trees.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_trees.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_types.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_types.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_upload.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_upload.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/test_user.py` & `gramps-webapi-1.1.8/tests/test_endpoints/test_user.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_endpoints/util.py` & `gramps-webapi-1.1.8/tests/test_endpoints/util.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_init.py` & `gramps-webapi-1.1.8/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_jwt.py` & `gramps-webapi-1.1.8/tests/test_jwt.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_limiter.py` & `gramps-webapi-1.1.8/tests/test_limiter.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_password.py` & `gramps-webapi-1.1.8/tests/test_password.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_s3.py` & `gramps-webapi-1.1.8/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_schema.py` & `gramps-webapi-1.1.8/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_sqlauth.py` & `gramps-webapi-1.1.8/tests/test_sqlauth.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.7/tests/test_version.py` & `gramps-webapi-1.1.8/tests/test_version.py`

 * *Files identical despite different names*

