# Comparing `tmp/lti-consumer-xblock-9.5.5.tar.gz` & `tmp/lti-consumer-xblock-9.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lti-consumer-xblock-9.5.5.tar", last modified: Fri Jul 14 13:13:09 2023, max compression
+gzip compressed data, was "lti-consumer-xblock-9.5.7.tar", last modified: Thu Jul 27 19:30:34 2023, max compression
```

## Comparing `lti-consumer-xblock-9.5.5.tar` & `lti-consumer-xblock-9.5.7.tar`

### file list

```diff
@@ -1,246 +1,246 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.837741 lti-consumer-xblock-9.5.5/
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-07-14 13:13:09.837741 lti-consumer-xblock-9.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13672 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.817741 lti-consumer-xblock-9.5.5/lti_consumer/
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      672 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     6551 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.817741 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15317 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.817741 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/contrib/django.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.817741 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/contrib/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/contrib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/contrib/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.817741 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14154 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/tests/test_oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.821741 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/ags.py
--rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    35328 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.821741 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.821741 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      388 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      554 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10557 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/nprs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.821741 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.821741 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.821741 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     9875 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/test_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    45009 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/test_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/test_key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/test_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    73194 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/lti_xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.825741 lti-consumer-xblock-9.5.5/lti_consumer/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0002_ltiagslineitem.py
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0003_ltiagsscore.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0005_migrate_keyset_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0007_ltidlcontentitem.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0008_fix_uuid_backfill.py
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0013_auto_20210712_1352.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0014_adds_external_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0015_add_additional_1p3_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/outcomes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.825741 lti-consumer-xblock-9.5.5/lti_consumer/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11574 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/plugin/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    35805 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.809741 lti-consumer-xblock-9.5.5/lti_consumer/public/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.809741 lti-consumer-xblock-9.5.5/lti_consumer/public/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.809741 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.825741 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/ar/
--rw-r--r--   0 runner    (1001) docker     (122)    22730 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/ar/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.825741 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/en/
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/en/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.825741 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/es_419/
--rw-r--r--   0 runner    (1001) docker     (122)    23422 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/es_419/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.825741 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/fr/
--rw-r--r--   0 runner    (1001) docker     (122)    21751 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/fr/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.825741 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/he/
--rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/he/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.825741 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/hi/
--rw-r--r--   0 runner    (1001) docker     (122)     3735 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/hi/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.825741 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/it/
--rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/it/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.825741 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/ja/
--rw-r--r--   0 runner    (1001) docker     (122)    16711 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/ja/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.825741 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/ko/
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/ko/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.825741 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/pt_BR/
--rw-r--r--   0 runner    (1001) docker     (122)     4601 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/pt_BR/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.825741 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/pt_PT/
--rw-r--r--   0 runner    (1001) docker     (122)    27017 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/pt_PT/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.825741 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/ru/
--rw-r--r--   0 runner    (1001) docker     (122)     3772 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/ru/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.825741 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/zh_CN/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.829741 lti-consumer-xblock-9.5.5/lti_consumer/signals/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.813741 lti-consumer-xblock-9.5.5/lti_consumer/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.829741 lti-consumer-xblock-9.5.5/lti_consumer/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/static/css/student.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.829741 lti-consumer-xblock-9.5.5/lti_consumer/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)    12186 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/static/js/xblock_lti_consumer.js
--rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/static/js/xblock_studio_view.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.829741 lti-consumer-xblock-9.5.5/lti_consumer/static/sass/
--rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/static/sass/student.scss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.813741 lti-consumer-xblock-9.5.5/lti_consumer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.829741 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.829741 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti-dl/
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti-dl/dl_response_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti-dl/dl_response_saved.html
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti-dl/render_dl_content.html
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti-dl/render_html.html
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti-dl/render_image.html
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti-dl/render_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti_1p3_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti_1p3_permission_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti_1p3_studio.html
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti_iframe.html
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti_launch_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti_proctoring_start_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti_start_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/html/student.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.829741 lti-consumer-xblock-9.5.5/lti_consumer/templates/xml/
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templates/xml/outcome_service_response.xml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.829741 lti-consumer-xblock-9.5.5/lti_consumer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templatetags/get_dl_lti_launch_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/templatetags/lti_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.829741 lti-consumer-xblock-9.5.5/lti_consumer/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.833741 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.833741 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11960 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/plugin/test_proctoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/plugin/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    85408 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/test_lti_xblock.py
--rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/test_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/track.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.833741 lti-consumer-xblock-9.5.5/lti_consumer/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.813741 lti-consumer-xblock-9.5.5/lti_consumer/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.833741 lti-consumer-xblock-9.5.5/lti_consumer/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10252 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/ar/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)      512 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.813741 lti-consumer-xblock-9.5.5/lti_consumer/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.833741 lti-consumer-xblock-9.5.5/lti_consumer/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/en/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.813741 lti-consumer-xblock-9.5.5/lti_consumer/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.833741 lti-consumer-xblock-9.5.5/lti_consumer/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    20799 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26467 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.813741 lti-consumer-xblock-9.5.5/lti_consumer/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.833741 lti-consumer-xblock-9.5.5/lti_consumer/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    18761 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/fr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25340 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/fr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.813741 lti-consumer-xblock-9.5.5/lti_consumer/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.833741 lti-consumer-xblock-9.5.5/lti_consumer/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.813741 lti-consumer-xblock-9.5.5/lti_consumer/translations/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.833741 lti-consumer-xblock-9.5.5/lti_consumer/translations/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9608 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/he/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/he/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.813741 lti-consumer-xblock-9.5.5/lti_consumer/translations/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.837741 lti-consumer-xblock-9.5.5/lti_consumer/translations/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/hi/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16407 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/hi/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.813741 lti-consumer-xblock-9.5.5/lti_consumer/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.837741 lti-consumer-xblock-9.5.5/lti_consumer/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9323 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21266 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.813741 lti-consumer-xblock-9.5.5/lti_consumer/translations/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.837741 lti-consumer-xblock-9.5.5/lti_consumer/translations/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.813741 lti-consumer-xblock-9.5.5/lti_consumer/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.837741 lti-consumer-xblock-9.5.5/lti_consumer/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16884 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.813741 lti-consumer-xblock-9.5.5/lti_consumer/translations/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.837741 lti-consumer-xblock-9.5.5/lti_consumer/translations/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    23772 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27799 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.813741 lti-consumer-xblock-9.5.5/lti_consumer/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.837741 lti-consumer-xblock-9.5.5/lti_consumer/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/ru/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16547 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/ru/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.813741 lti-consumer-xblock-9.5.5/lti_consumer/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.837741 lti-consumer-xblock-9.5.5/lti_consumer/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16458 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/lti_consumer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.837741 lti-consumer-xblock-9.5.5/lti_consumer_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-07-14 13:13:09.000000 lti-consumer-xblock-9.5.5/lti_consumer_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7644 2023-07-14 13:13:09.000000 lti-consumer-xblock-9.5.5/lti_consumer_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-14 13:13:09.000000 lti-consumer-xblock-9.5.5/lti_consumer_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-07-14 13:13:09.000000 lti-consumer-xblock-9.5.5/lti_consumer_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-07-14 13:13:09.000000 lti-consumer-xblock-9.5.5/lti_consumer_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-14 13:13:09.000000 lti-consumer-xblock-9.5.5/lti_consumer_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:09.837741 lti-consumer-xblock-9.5.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-07-14 13:13:09.837741 lti-consumer-xblock-9.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-07-14 13:13:05.000000 lti-consumer-xblock-9.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.938440 lti-consumer-xblock-9.5.7/
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)    14574 2023-07-27 19:30:34.938440 lti-consumer-xblock-9.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13790 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.922440 lti-consumer-xblock-9.5.7/lti_consumer/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6551 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.922440 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15317 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.922440 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/contrib/django.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.922440 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/contrib/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/contrib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/contrib/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.922440 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14154 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/tests/test_oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.922440 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3053 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35328 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.922440 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.926440 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      388 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      554 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10557 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/nprs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.926440 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.926440 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.926440 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9875 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/test_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45009 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/test_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/test_key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/test_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    73332 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/lti_xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.926440 lti-consumer-xblock-9.5.7/lti_consumer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0002_ltiagslineitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0003_ltiagsscore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0005_migrate_keyset_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0007_ltidlcontentitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0008_fix_uuid_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0013_auto_20210712_1352.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0014_adds_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0015_add_additional_1p3_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/outcomes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.926440 lti-consumer-xblock-9.5.7/lti_consumer/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11574 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/plugin/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36822 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.914440 lti-consumer-xblock-9.5.7/lti_consumer/public/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.914440 lti-consumer-xblock-9.5.7/lti_consumer/public/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.914440 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.926440 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/ar/
+-rw-r--r--   0 runner    (1001) docker     (122)    22730 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/ar/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.926440 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/en/
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/en/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/es_419/
+-rw-r--r--   0 runner    (1001) docker     (122)    23422 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/es_419/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/fr/
+-rw-r--r--   0 runner    (1001) docker     (122)    21751 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/fr/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/he/
+-rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/he/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/hi/
+-rw-r--r--   0 runner    (1001) docker     (122)     3735 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/hi/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/it/
+-rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/it/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/ja/
+-rw-r--r--   0 runner    (1001) docker     (122)    16711 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/ja/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/ko/
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/ko/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/pt_BR/
+-rw-r--r--   0 runner    (1001) docker     (122)     4601 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/pt_BR/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/pt_PT/
+-rw-r--r--   0 runner    (1001) docker     (122)    27017 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/pt_PT/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/ru/
+-rw-r--r--   0 runner    (1001) docker     (122)     3772 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/ru/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/zh_CN/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/signals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.914440 lti-consumer-xblock-9.5.7/lti_consumer/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/static/css/student.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    12186 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/static/js/xblock_lti_consumer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/static/js/xblock_studio_view.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/static/sass/
+-rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/static/sass/student.scss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.918440 lti-consumer-xblock-9.5.7/lti_consumer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti-dl/
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti-dl/dl_response_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti-dl/dl_response_saved.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti-dl/render_dl_content.html
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti-dl/render_html.html
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti-dl/render_image.html
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti-dl/render_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti_1p3_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti_1p3_permission_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti_1p3_studio.html
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti_iframe.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      481 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti_launch_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti_proctoring_start_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti_start_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/html/student.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.930440 lti-consumer-xblock-9.5.7/lti_consumer/templates/xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templates/xml/outcome_service_response.xml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.934440 lti-consumer-xblock-9.5.7/lti_consumer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templatetags/get_dl_lti_launch_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/templatetags/lti_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.934440 lti-consumer-xblock-9.5.7/lti_consumer/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.934440 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.934440 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11960 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/plugin/test_proctoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27971 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/plugin/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    85409 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/test_lti_xblock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/test_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/track.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.934440 lti-consumer-xblock-9.5.7/lti_consumer/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.918440 lti-consumer-xblock-9.5.7/lti_consumer/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.934440 lti-consumer-xblock-9.5.7/lti_consumer/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10252 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/ar/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/ar/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)      512 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.918440 lti-consumer-xblock-9.5.7/lti_consumer/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.934440 lti-consumer-xblock-9.5.7/lti_consumer/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/en/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/en/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.918440 lti-consumer-xblock-9.5.7/lti_consumer/translations/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.934440 lti-consumer-xblock-9.5.7/lti_consumer/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    20799 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26467 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/es_419/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.918440 lti-consumer-xblock-9.5.7/lti_consumer/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.934440 lti-consumer-xblock-9.5.7/lti_consumer/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    18761 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/fr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25340 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/fr/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.918440 lti-consumer-xblock-9.5.7/lti_consumer/translations/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.934440 lti-consumer-xblock-9.5.7/lti_consumer/translations/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.918440 lti-consumer-xblock-9.5.7/lti_consumer/translations/he/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.938440 lti-consumer-xblock-9.5.7/lti_consumer/translations/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9608 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/he/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/he/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.918440 lti-consumer-xblock-9.5.7/lti_consumer/translations/hi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.938440 lti-consumer-xblock-9.5.7/lti_consumer/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/hi/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16407 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/hi/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.918440 lti-consumer-xblock-9.5.7/lti_consumer/translations/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.938440 lti-consumer-xblock-9.5.7/lti_consumer/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9323 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21266 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.918440 lti-consumer-xblock-9.5.7/lti_consumer/translations/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.938440 lti-consumer-xblock-9.5.7/lti_consumer/translations/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.918440 lti-consumer-xblock-9.5.7/lti_consumer/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.938440 lti-consumer-xblock-9.5.7/lti_consumer/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16884 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.918440 lti-consumer-xblock-9.5.7/lti_consumer/translations/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.938440 lti-consumer-xblock-9.5.7/lti_consumer/translations/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    23772 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27799 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.918440 lti-consumer-xblock-9.5.7/lti_consumer/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.938440 lti-consumer-xblock-9.5.7/lti_consumer/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/ru/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16547 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/ru/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.918440 lti-consumer-xblock-9.5.7/lti_consumer/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.938440 lti-consumer-xblock-9.5.7/lti_consumer/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16458 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/lti_consumer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.938440 lti-consumer-xblock-9.5.7/lti_consumer_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14574 2023-07-27 19:30:34.000000 lti-consumer-xblock-9.5.7/lti_consumer_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7644 2023-07-27 19:30:34.000000 lti-consumer-xblock-9.5.7/lti_consumer_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-27 19:30:34.000000 lti-consumer-xblock-9.5.7/lti_consumer_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-07-27 19:30:34.000000 lti-consumer-xblock-9.5.7/lti_consumer_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-07-27 19:30:34.000000 lti-consumer-xblock-9.5.7/lti_consumer_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-27 19:30:34.000000 lti-consumer-xblock-9.5.7/lti_consumer_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 19:30:34.938440 lti-consumer-xblock-9.5.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-07-27 19:30:34.938440 lti-consumer-xblock-9.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-07-27 19:30:30.000000 lti-consumer-xblock-9.5.7/setup.py
```

### Comparing `lti-consumer-xblock-9.5.5/LICENSE` & `lti-consumer-xblock-9.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/NOTICE` & `lti-consumer-xblock-9.5.7/NOTICE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/PKG-INFO` & `lti-consumer-xblock-9.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.5.5
+Version: 9.5.7
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
@@ -168,14 +168,15 @@
 
 Unit Testing
 ============
 
 * To run all of the unit tests at once, run `make test`
 * To run tests on individual files in development, run `python ./test.py -k=[name of test file without .py]`
 * For example, if you want to run the tests in test_permissions.py, run `python ./test.py -k=test_permissions`
+* To run a specific test in a file, run something like `python ./test.py -k=test_permissions.TestClass.test_function`
 
 Testing Against an LTI Provider
 ===============================
 
 LTI 1.1
 -------
```

### Comparing `lti-consumer-xblock-9.5.5/README.rst` & `lti-consumer-xblock-9.5.7/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -147,14 +147,15 @@
 
 Unit Testing
 ============
 
 * To run all of the unit tests at once, run `make test`
 * To run tests on individual files in development, run `python ./test.py -k=[name of test file without .py]`
 * For example, if you want to run the tests in test_permissions.py, run `python ./test.py -k=test_permissions`
+* To run a specific test in a file, run something like `python ./test.py -k=test_permissions.TestClass.test_function`
 
 Testing Against an LTI Provider
 ===============================
 
 LTI 1.1
 -------
```

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/admin.py` & `lti-consumer-xblock-9.5.7/lti_consumer/admin.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/api.py` & `lti-consumer-xblock-9.5.7/lti_consumer/api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/apps.py` & `lti-consumer-xblock-9.5.7/lti_consumer/apps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/data.py` & `lti-consumer-xblock-9.5.7/lti_consumer/data.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/filters.py` & `lti-consumer-xblock-9.5.7/lti_consumer/filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/forms.py` & `lti-consumer-xblock-9.5.7/lti_consumer/forms.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/consumer.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/contrib/django.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/contrib/django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/contrib/tests/test_django.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/contrib/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/oauth.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/tests/test_consumer.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p1/tests/test_oauth.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p1/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/ags.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/constants.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,13 +92,13 @@
     'session_data',
     'start_assessment_url',
     'assessment_control_url',
     'assessment_control_actions'
 ]
 
 LTI_PROCTORING_ASSESSMENT_CONTROL_ACTIONS = [
-    'pauseRequest',
-    'resumeRequest',
-    'terminateRequest',
+    'pause',
+    'resume',
+    'terminate',
     'update',
-    'flagRequest',
+    'flag',
 ]
```

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/consumer.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/deep_linking.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/exceptions.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/exceptions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/extensions/rest_framework/utils.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/extensions/rest_framework/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/key_handlers.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/nprs.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/nprs.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/test_ags.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/test_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/test_consumer.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/test_deep_linking.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/test_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/test_key_handlers.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/test_key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_1p3/tests/test_nrps.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_1p3/tests/test_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/lti_xblock.py` & `lti-consumer-xblock-9.5.7/lti_consumer/lti_xblock.py`

 * *Files 0% similar despite different names*

```diff
@@ -1231,17 +1231,19 @@
             user_id = self.get_lti_1p1_user_id()
             role = self.role
 
             # Convert the LMS role into an LTI 1.1 role.
             role = LTI_1P1_ROLE_MAP.get(role, 'Student,Learner')
 
             result_sourcedid = self.lis_result_sourcedid
-        except LtiError:
+        # Fails if extract_real_user_data() fails
+        except LtiError as err:
             loader = ResourceLoader(__name__)
-            template = loader.render_django_template('/templates/html/lti_launch_error.html')
+            template = loader.render_django_template('/templates/html/lti_launch_error.html',
+                                                     context={"error_msg": err})
             return Response(template, status=400, content_type='text/html')
 
         username = None
         full_name = None
         email = None
 
         # Send PII fields only if this XBlock is configured to allow the sending PII.
```

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0001_initial.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0002_ltiagslineitem.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0002_ltiagslineitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0003_ltiagsscore.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0003_ltiagsscore.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0004_keyset_mgmt_to_model.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0004_keyset_mgmt_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0005_migrate_keyset_to_model.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0005_migrate_keyset_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0007_ltidlcontentitem.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0007_ltidlcontentitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0008_fix_uuid_backfill.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0008_fix_uuid_backfill.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0009_backfill-empty-string-config-id.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0009_backfill-empty-string-config-id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0013_auto_20210712_1352.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0013_auto_20210712_1352.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0014_adds_external_id.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0014_adds_external_id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0015_add_additional_1p3_fields.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0015_add_additional_1p3_fields.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py` & `lti-consumer-xblock-9.5.7/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/models.py` & `lti-consumer-xblock-9.5.7/lti_consumer/models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/outcomes.py` & `lti-consumer-xblock-9.5.7/lti_consumer/outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/plugin/compat.py` & `lti-consumer-xblock-9.5.7/lti_consumer/plugin/compat.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/plugin/urls.py` & `lti-consumer-xblock-9.5.7/lti_consumer/plugin/urls.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/plugin/views.py` & `lti-consumer-xblock-9.5.7/lti_consumer/plugin/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,51 +135,77 @@
     * login_hint (REQUIRED): an identifier for the user that initiated the launch; it is stable and unique to the issuer
     """
     # pylint: disable=too-many-statements
     request_params = request.GET if request.method == 'GET' else request.POST
 
     lti_message_hint = request_params.get('lti_message_hint')
     if not lti_message_hint:
-        log.info('The lti_message_hint query param in the request is missing or empty.')
-        return render(request, 'html/lti_launch_error.html', status=HTTP_400_BAD_REQUEST)
+        error_msg = 'The lti_message_hint is missing or empty.'
+        log.info(error_msg)
+        return render(
+            request,
+            'html/lti_launch_error.html',
+            context={"error_msg": error_msg},
+            status=HTTP_400_BAD_REQUEST
+        )
 
     login_hint = request_params.get('login_hint')
     if not login_hint:
-        log.info('The login_hint query param in the request is missing or empty.')
-        return render(request, 'html/lti_launch_error.html', status=HTTP_400_BAD_REQUEST)
+        error_msg = 'The login_hint is missing or empty.'
+        log.info(error_msg)
+        return render(
+            request,
+            'html/lti_launch_error.html',
+            context={"error_msg": error_msg},
+            status=HTTP_400_BAD_REQUEST
+        )
 
     launch_data = get_data_from_cache(lti_message_hint)
     if not launch_data:
-        log.warning(
-            f'There was a cache miss trying to fetch the launch data during an LTI 1.3 launch when using the cache'
-            f' key {lti_message_hint}. The login hint is {login_hint}.'
+        error_msg = (
+            f'Unable to find record of an OIDC launch for the provided lti_message_hint: {lti_message_hint}'
+        )
+        log.warning(error_msg)
+        return render(
+            request,
+            'html/lti_launch_error.html',
+            context={"error_msg": error_msg},
+            status=HTTP_400_BAD_REQUEST
         )
-        return render(request, 'html/lti_launch_error.html', status=HTTP_400_BAD_REQUEST)
 
-    # Validate the Lti1p3LaunchData.
     is_valid, validation_messages = validate_lti_1p3_launch_data(launch_data)
     if not is_valid:
         validation_message = " ".join(validation_messages)
-        log.error(
-            f"The Lti1p3LaunchData is not valid. {validation_message}"
+        error_msg = f"The Lti1p3LaunchData is not valid. {validation_message}"
+        log.error(error_msg)
+        return render(
+            request,
+            'html/lti_launch_error.html',
+            context={"error_msg": error_msg},
+            status=HTTP_400_BAD_REQUEST
         )
-        return render(request, 'html/lti_launch_error.html', status=HTTP_400_BAD_REQUEST)
 
     config_id = launch_data.config_id
     try:
         lti_config = LtiConfiguration.objects.get(
             config_id=config_id
         )
     except (LtiConfiguration.DoesNotExist, ValidationError) as exc:
         log.error("Invalid config_id '%s' for LTI 1.3 Launch callback", config_id)
         raise Http404 from exc
 
     if lti_config.version != LtiConfiguration.LTI_1P3:
-        log.error("The LTI Version of configuration %s is not LTI 1.3", lti_config)
-        return render(request, 'html/lti_launch_error.html', status=HTTP_404_NOT_FOUND)
+        error_msg = f"The LTI Version of the following configuration is not LTI 1.3: {lti_config}"
+        log.error(error_msg)
+        return render(
+            request,
+            'html/lti_launch_error.html',
+            context={"error_msg": error_msg},
+            status=HTTP_404_NOT_FOUND
+        )
 
     context = {}
 
     try:
         lti_consumer = lti_config.get_lti_consumer()
 
         # Set sub and roles claims.
@@ -206,19 +232,25 @@
         context_type = launch_data.context_type
         context_types_claim = None
 
         if context_type:
             try:
                 context_types_claim = get_lti_1p3_context_types_claim(context_type)
             except ValueError:
-                log.error(
-                    "The context_type key %s in the launch data does not represent a valid context_type.",
-                    context_type
+                error_msg = (
+                    f"The context_type key {context_type} in the launch "
+                    f"data does not represent a valid context_type."
+                )
+                log.error(error_msg)
+                return render(
+                    request,
+                    'html/lti_launch_error.html',
+                    context={"error_msg": error_msg},
+                    status=HTTP_400_BAD_REQUEST
                 )
-                return render(request, 'html/lti_launch_error.html', status=HTTP_400_BAD_REQUEST)
 
         lti_consumer.set_context_claim(
             launch_data.context_id,
             context_types_claim,
             launch_data.context_title,
             launch_data.context_label,
         )
@@ -298,20 +330,22 @@
             'launch_url': context['launch_url']
         }
         track_event('xblock.launch_request', event)
 
         return render(request, 'html/lti_1p3_launch.html', context)
     except Lti1p3Exception as exc:
         resource_link_id = launch_data.resource_link_id
+        error_msg = f"Error preparing LTI 1.3 launch for resource with resource_link_id {resource_link_id}: {exc}"
         log.warning(
             "Error preparing LTI 1.3 launch for resource with resource_link_id %r: %s",
             resource_link_id,
             exc,
             exc_info=True
         )
+        context.update({"error_msg": error_msg})
         return render(request, 'html/lti_launch_error.html', context, status=HTTP_400_BAD_REQUEST)
     except AssertionError as exc:
         resource_link_id = launch_data.resource_link_id
         log.warning(
             "Permission on resource with resource_link_id %r denied for user %r: %s",
             resource_link_id,
             user_id,
@@ -481,21 +515,33 @@
 @xframe_options_sameorigin
 def deep_linking_content_endpoint(request, lti_config_id):
     """
     Deep Linking endpoint for rendering Deep Linking Content Items.
     """
     launch_data_key = request.GET.get("launch_data_key")
     if not launch_data_key:
-        log.info('The launch_data_key query param in the request is missing or empty.')
-        return render(request, 'html/lti_launch_error.html', status=HTTP_400_BAD_REQUEST)
+        error_msg = 'The launch_data_key query param in the request is missing or empty.'
+        log.info(error_msg)
+        return render(
+            request,
+            'html/lti_launch_error.html',
+            context={"error_msg": error_msg},
+            status=HTTP_400_BAD_REQUEST
+        )
 
     launch_data = get_data_from_cache(launch_data_key)
     if not launch_data:
-        log.warning(f'There was a cache miss during an LTI 1.3 launch when using the cache_key {launch_data_key}.')
-        return render(request, 'html/lti_launch_error.html', status=HTTP_400_BAD_REQUEST)
+        error_msg = f'There was a cache miss during an LTI 1.3 launch when using the cache_key {launch_data_key}.'
+        log.warning(error_msg)
+        return render(
+            request,
+            'html/lti_launch_error.html',
+            context={"error_msg": error_msg},
+            status=HTTP_400_BAD_REQUEST
+        )
     try:
         # Get LTI Configuration
         lti_config = LtiConfiguration.objects.get(id=lti_config_id)
     except LtiConfiguration.DoesNotExist as exc:
         log.info("LtiConfiguration %r does not exist: %s", lti_config_id, exc)
         raise Http404 from exc
```

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/ar/text.js` & `lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/ar/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/en/text.js` & `lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/en/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/es_419/text.js` & `lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/es_419/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/fr/text.js` & `lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/fr/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/he/text.js` & `lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/he/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/hi/text.js` & `lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/hi/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/it/text.js` & `lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/it/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/ja/text.js` & `lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/ja/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/ko/text.js` & `lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/ko/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/pt_BR/text.js` & `lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/pt_BR/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/pt_PT/text.js` & `lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/pt_PT/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/ru/text.js` & `lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/ru/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/public/js/translations/zh_CN/text.js` & `lti-consumer-xblock-9.5.7/lti_consumer/public/js/translations/zh_CN/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/signals/signals.py` & `lti-consumer-xblock-9.5.7/lti_consumer/signals/signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/static/css/student.css` & `lti-consumer-xblock-9.5.7/lti_consumer/static/css/student.css`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/static/js/xblock_lti_consumer.js` & `lti-consumer-xblock-9.5.7/lti_consumer/static/js/xblock_lti_consumer.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/static/js/xblock_studio_view.js` & `lti-consumer-xblock-9.5.7/lti_consumer/static/js/xblock_studio_view.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/static/sass/student.scss` & `lti-consumer-xblock-9.5.7/lti_consumer/static/sass/student.scss`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti-dl/render_dl_content.html` & `lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti-dl/render_dl_content.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti-dl/render_image.html` & `lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti-dl/render_image.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti-dl/render_link.html` & `lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti-dl/render_link.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti_1p3_launch.html` & `lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti_1p3_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti_1p3_studio.html` & `lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti_1p3_studio.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/templates/html/lti_launch.html` & `lti-consumer-xblock-9.5.7/lti_consumer/templates/html/lti_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/templates/html/student.html` & `lti-consumer-xblock-9.5.7/lti_consumer/templates/html/student.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/templates/xml/outcome_service_response.xml` & `lti-consumer-xblock-9.5.7/lti_consumer/templates/xml/outcome_service_response.xml`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/templatetags/get_dl_lti_launch_url.py` & `lti-consumer-xblock-9.5.7/lti_consumer/templatetags/get_dl_lti_launch_url.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/templatetags/lti_sanitize.py` & `lti-consumer-xblock-9.5.7/lti_consumer/templatetags/lti_sanitize.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/tests/test_utils.py` & `lti-consumer-xblock-9.5.7/lti_consumer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/plugin/test_proctoring.py` & `lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/plugin/test_proctoring.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/plugin/test_views.py` & `lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/plugin/test_views.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from lti_consumer.utils import cache_lti_1p3_launch_data
 
 
 class TestLti1p3KeysetEndpoint(TestCase):
     """
     Test `public_keyset_endpoint` method.
     """
+
     def setUp(self):
         super().setUp()
 
         self.location = 'block-v1:course+test+2020+type@problem+block@test'
         self.url = f'/lti_consumer/v1/public_keysets/{self.location}'
 
         # Set up LTI Configuration
@@ -103,14 +104,15 @@
 
 
 @ddt.ddt
 class TestLti1p3LaunchGateEndpoint(TestCase):
     """
     Tests for the `launch_gate_endpoint` method.
     """
+
     def setUp(self):
         super().setUp()
 
         self.location = 'block-v1:course+test+2020+type@problem+block@test'
         self.url = '/lti_consumer/v1/launch/'
         self.config = LtiConfiguration(
             version=LtiConfiguration.LTI_1P3,
@@ -183,63 +185,116 @@
                 "lti_message_hint": self.launch_data_key
             }
         )
         self.assertEqual(response.status_code, 404)
 
     def test_missing_required_lti_message_hint_param(self):
         """
-        Check that a 400 error is returned when required lti_message_hint query parameter is not provided.
+        Check for the expected error message when required lti_message_hint query parameter is not provided.
         """
         response = self.client.post(self.url, {"login_hint": "login_hint"})
         self.assertEqual(response.status_code, 400)
+        self.assertIn(
+            'The lti_message_hint is missing or empty.',
+            str(response.content)
+        )
 
     def test_missing_required_login_hint_param(self):
         """
-        Check that a 400 error is returned when required login_hint query parameter is not provided.
+        Check for the expected error message when required login_hint query parameter is not provided.
         """
         response = self.client.post(self.url, {"lti_message_hint": "lti_message_hint"})
         self.assertEqual(response.status_code, 400)
 
-    def test_missing_launch_data(self):
+        # Assert expected error msg in the HttpResponse
+        self.assertIn(
+            'The login_hint is missing or empty.',
+            str(response.content)
+        )
+
+    @patch('lti_consumer.plugin.views.get_data_from_cache')
+    def test_missing_launch_data(self, mock_get_data_from_cache):
         """
-        Check that a 400 error is returned when required lti_message_hint query parameter is not associated with
-        launch_data in the cache.
+        Check that the expected error message returned when required lti_message_hint query parameter
+        is not associated with launch_data in the cache.
         """
+        # Mock getting the launch_data from the cache.
+        mock_get_data_from_cache.return_value = None
         response = self.client.post(self.url, {"lti_message_hint": "lti_message_hint", "login_hint": "login_hint"})
         self.assertEqual(response.status_code, 400)
 
-    @patch('lti_consumer.api.validate_lti_1p3_launch_data')
-    @patch('lti_consumer.utils.get_data_from_cache')
+        # Assert expected error msg in the HttpResponse
+        self.assertIn(
+            'Unable to find record of an OIDC launch for the provided lti_message_hint:',
+            str(response.content)
+        )
+
+    @patch('lti_consumer.plugin.views.validate_lti_1p3_launch_data')
+    @patch('lti_consumer.plugin.views.get_data_from_cache')
     def test_invalid_launch_data(self, mock_get_data_from_cache, mock_validate_launch_data):
         """
         Check that a 400 error is returned when the launch_data stored in the cache is not valid.
         """
         # Mock getting the launch_data from the cache.
-        mock_get_data_from_cache.return_value = {}
+        mock_get_data_from_cache.return_value = {"context_type": "invalid_context_type"}
 
         # Mock checking the launch_data for validity.
-        mock_validate_launch_data.return_value = (False, [])
+        mock_validate_launch_data.return_value = (False, [
+            'The context_id attribute is required in the launch data if any optional context properties are provided.',
+        ])
 
         response = self.client.post(self.url, {"lti_message_hint": "lti_message_hint", "login_hint": "login_hint"})
         self.assertEqual(response.status_code, 400)
 
-    @patch('lti_consumer.api.validate_lti_1p3_launch_data')
-    @patch('lti_consumer.utils.get_data_from_cache')
+        # Assert expected error msg in the HttpResponse
+        self.assertIn(
+            'The context_id attribute is required in the launch data if any optional context properties are provided.',
+            str(response.content)
+        )
+
+    @patch('lti_consumer.plugin.views.validate_lti_1p3_launch_data')
+    @patch('lti_consumer.plugin.views.get_data_from_cache')
     def test_invalid_context_type(self, mock_get_data_from_cache, mock_validate_launch_data):
         # Mock getting the launch_data from the cache.
-        mock_launch_data = Mock()
-        mock_launch_data.context_type = "invalid_context_type"
-        mock_get_data_from_cache.return_value = mock_launch_data
+        mock_get_data_from_cache.return_value = Lti1p3LaunchData(
+            user_id=3,
+            user_role='instructor',
+            config_id=self.config.config_id,
+            resource_link_id=(
+                'block-v1:edX+LTI-xblock+consumer+'
+                'type@lti_consumer+block@7f9f07d76ce440f39d892f7f0d312cf2'
+            ),
+            preferred_username=None,
+            name=None,
+            email=None,
+            external_user_id='cd6fafb6-2bf7-4196-9b23-a1361c1bf0ef',
+            launch_presentation_document_target='iframe',
+            launch_presentation_return_url=None,
+            message_type='LtiStartProctoring',  # 'LtiResourceLinkRequest',
+            # context_id='course-v1:edX+LTI-xblock+consumer',
+            context_type=['invalid_context_type'],  # ['course_offering'],
+            context_title='edx-LTI-xblock-thing - edX',
+            context_label='course-v1:edX+LTI-xblock+consumer',
+            deep_linking_content_item_id=None,
+            proctoring_launch_data=Lti1p3ProctoringLaunchData(attempt_number=1)  # None
+        )
 
         # Mock checking the launch_data for validity.
         mock_validate_launch_data.return_value = (True, [])
 
         response = self.client.post(self.url, {"lti_message_hint": "lti_message_hint", "login_hint": "login_hint"})
         self.assertEqual(response.status_code, 400)
 
+        # Assert expected error msg in the HttpResponse
+        self.assertIn(
+            # The error message in the HttpResponse contains a messy formatted string, so only test for part it.
+            'the launch data does not represent a valid context_type.',
+            str(response.content)
+        )
+
     def test_lti_launch_response(self):
         """
         Check that the right launch response is generated
         """
         params = {
             "nonce": "nonce-value",
             "state": "hello-world",
@@ -262,15 +317,15 @@
         # Make a fake invalid preflight request, with empty parameters
         response = self.client.get(self.url)
 
         # Check response and assert that state was inserted
         self.assertEqual(response.status_code, 400)
 
         response_body = response.content.decode('utf-8')
-        self.assertIn("There was an error while launching the LTI tool.", response_body)
+        self.assertIn("There was an error while launching the LTI tool: ", response_body)
         self.assertNotIn("% trans", response_body)
 
         with patch(
             "lti_consumer.models.LtiAdvantageConsumer.generate_launch_request",
             side_effect=PreflightRequestValidationFailure()
         ):
             params = {
@@ -525,14 +580,15 @@
         self.assertEqual(response.status_code, 200)
 
 
 class TestLti1p3AccessTokenEndpoint(TestCase):
     """
     Test `access_token_endpoint` method.
     """
+
     def setUp(self):
         super().setUp()
 
         location = 'block-v1:course+test+2020+type@problem+block@test'
         self.config = LtiConfiguration(version=LtiConfiguration.LTI_1P3, location=location)
         self.config.save()
         self.url = reverse('lti_consumer:lti_consumer.access_token', args=[str(self.config.config_id)])
```

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/plugin/test_views_lti_ags.py` & `lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/plugin/test_views_lti_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py` & `lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py` & `lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/test_api.py` & `lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/test_filters.py` & `lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/test_lti_xblock.py` & `lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/test_lti_xblock.py`

 * *Files 0% similar despite different names*

```diff
@@ -915,15 +915,15 @@
         request = make_request('', 'GET')
         response = self.xblock.lti_launch_handler(request)
 
         self.assertEqual(response.status_code, 400)
         self.assertEqual(response.content_type, 'text/html')
 
         response_body = response.body.decode('utf-8')
-        self.assertIn("There was an error while launching the LTI tool.", response_body)
+        self.assertIn("There was an error while launching the LTI tool: ", response_body)
 
     @patch('lti_consumer.lti_xblock.LtiConsumerXBlock.course')
     @patch('lti_consumer.lti_xblock.LtiConsumerXBlock.anonymous_user_id', PropertyMock(return_value=FAKE_USER_ID))
     def test_publish_tracking_event(self, mock_course):
         """
         Test a tracking event is emitted when generating a launch request
         """
```

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/test_models.py` & `lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/test_outcomes.py` & `lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/test_signals.py` & `lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/test_signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/tests/unit/test_utils.py` & `lti-consumer-xblock-9.5.7/lti_consumer/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/ar/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/ar/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/ar/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/ar/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/config.yaml` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/config.yaml`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/en/LC_MESSAGES/django.po` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/en/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/en/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/es_419/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/es_419/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/es_419/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/es_419/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/fr/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/fr/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/fr/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/fr/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/he/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/he/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/he/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/he/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/hi/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/hi/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/ru/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/ru/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/ru/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/ru/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/settings.py` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/settings.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.7/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer/utils.py` & `lti-consumer-xblock-9.5.7/lti_consumer/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer_xblock.egg-info/PKG-INFO` & `lti-consumer-xblock-9.5.7/lti_consumer_xblock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.5.5
+Version: 9.5.7
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
@@ -168,14 +168,15 @@
 
 Unit Testing
 ============
 
 * To run all of the unit tests at once, run `make test`
 * To run tests on individual files in development, run `python ./test.py -k=[name of test file without .py]`
 * For example, if you want to run the tests in test_permissions.py, run `python ./test.py -k=test_permissions`
+* To run a specific test in a file, run something like `python ./test.py -k=test_permissions.TestClass.test_function`
 
 Testing Against an LTI Provider
 ===============================
 
 LTI 1.1
 -------
```

### Comparing `lti-consumer-xblock-9.5.5/lti_consumer_xblock.egg-info/SOURCES.txt` & `lti-consumer-xblock-9.5.7/lti_consumer_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/requirements/constraints.txt` & `lti-consumer-xblock-9.5.7/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.5/setup.py` & `lti-consumer-xblock-9.5.7/setup.py`

 * *Files identical despite different names*

