# Comparing `tmp/djangocms-frontend-1.1.5.tar.gz` & `tmp/djangocms-frontend-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-frontend-1.1.5.tar", last modified: Fri Jul 14 14:00:41 2023, max compression
+gzip compressed data, was "djangocms-frontend-1.1.6.tar", last modified: Thu Jul 27 11:52:13 2023, max compression
```

## Comparing `djangocms-frontend-1.1.5.tar` & `djangocms-frontend-1.1.6.tar`

### file list

```diff
@@ -1,687 +1,700 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.591064 djangocms-frontend-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-07-14 14:00:41.591064 djangocms-frontend-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.495063 djangocms-frontend-1.1.5/djangocms_frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/cms_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.499063 djangocms-frontend-1.1.5/djangocms_frontend/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/common/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/common/background.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.499063 djangocms-frontend-1.1.5/djangocms_frontend/common/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/common/bootstrap5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/common/bootstrap5/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/common/bootstrap5/responsive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/common/bootstrap5/sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/common/responsive.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/common/sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/common/spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/common/title.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.499063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.499063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.499063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.499063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.479063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.479063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.499063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion.html
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.499063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.499063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.499063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.479063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.479063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.499063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.499063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.499063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.503063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.503063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.503063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.479063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.503063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.503063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/badge.html
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/templates/djangocms_frontend/badge.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.503063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.503063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.503063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.503063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card.html
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.503063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.503063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.503063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.507063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.507063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/carousel.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.507063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.507063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.507063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.507063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.507063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/collapse.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.507063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-container.html
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.507063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.507063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.511063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.511063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/figure.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.511063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/code.html
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/figure.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.511063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.511063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.511063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.511063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.511063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/grid_row.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.515063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.515063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.515063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.515063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/ckeditor.icons.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.527063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   277297 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    59388 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    63664 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   123564 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   516494 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   123376 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   123452 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    54568 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   150535 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    56976 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    32020 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   643290 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   127824 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   103304 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   105448 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot
--rw-r--r--   0 runner    (1001) docker     (123)   304476 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg
--rw-r--r--   0 runner    (1001) docker     (123)   105284 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105360 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28196 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot
--rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf
--rw-r--r--   0 runner    (1001) docker     (123)    54789 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   729984 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)  2883039 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   729800 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   386256 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   282928 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    99774 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   184969 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)    99564 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    56468 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    44720 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    45816 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot
--rw-r--r--   0 runner    (1001) docker     (123)   132305 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45648 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    45724 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.543063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/
--rw-r--r--   0 runner    (1001) docker     (123)    48146 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)    30533 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json
--rw-r--r--   0 runner    (1001) docker     (123)    35481 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    18498 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json
--rw-r--r--   0 runner    (1001) docker     (123)    15099 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json
--rw-r--r--   0 runner    (1001) docker     (123)    23027 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json
--rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    35227 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.543063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.543063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.543063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.547063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)    30045 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    28165 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   137737 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)   115209 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    20997 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    18213 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    27048 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css
--rw-r--r--   0 runner    (1001) docker     (123)    20593 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    77647 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    65062 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    32569 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    26765 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.483063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.547063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.551063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/icon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.551063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/add_css.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.551063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/templatetags/icon_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.551063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.551063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.551063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.551063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/image.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.551063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.551063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.551063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.555064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.555064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/jumbotron.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.555064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/jumbotron.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.555064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.555064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.555064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.555064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.555064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.555064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.559064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.559064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.559064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.559064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.487063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.559064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/list-group.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.559064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.559064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.559064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.563063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/media.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.563063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/media.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.563063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.563063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.563063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.563063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/nav_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navlink.html
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.567063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.567063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.567063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.567063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.567063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.571064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/tabs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.571064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.571064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.571064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.571064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.571064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.571064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/no_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/spacing.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.571064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/toc.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.571064 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/templatetags/fe_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.571064 djangocms-frontend-1.1.5/djangocms_frontend/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.575064 djangocms-frontend-1.1.5/djangocms_frontend/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    26790 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    44731 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.575064 djangocms-frontend-1.1.5/djangocms_frontend/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    34046 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.575064 djangocms-frontend-1.1.5/djangocms_frontend/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.575064 djangocms-frontend-1.1.5/djangocms_frontend/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15741 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    39659 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.575064 djangocms-frontend-1.1.5/djangocms_frontend/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/management/bootstrap4_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.575064 djangocms-frontend-1.1.5/djangocms_frontend/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/management/commands/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.575064 djangocms-frontend-1.1.5/djangocms_frontend/management/commands/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/management/commands/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/management/commands/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/management/commands/subcommands/frequency_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/management/commands/subcommands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/management/commands/subcommands/stale_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/management/commands/subcommands/sync_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/management/icon_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/management/styled_link_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.579064 djangocms-frontend-1.1.5/djangocms_frontend/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.491063 djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.579064 djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/css/
--rw-r--r--   0 runner    (1001) docker     (123)    78932 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/css/base.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/css/button_group.css
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/css/div_select.css
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/css/select2.css
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/css/select2.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.579064 djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/js/auto_input.js
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js
--rw-r--r--   0 runner    (1001) docker     (123)    95562 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/js/django_select2.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.579064 djangocms-frontend-1.1.5/djangocms_frontend/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.579064 djangocms-frontend-1.1.5/djangocms_frontend/templates/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templates/bootstrap5/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templates/bootstrap5/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templates/bootstrap5/menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.579064 djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.583063 djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/base-collapse.html
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.583063 djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.583063 djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/html_container.html
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.583063 djangocms-frontend-1.1.5/djangocms_frontend/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/djangocms_frontend/templatetags/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.499063 djangocms-frontend-1.1.5/djangocms_frontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-07-14 14:00:41.000000 djangocms-frontend-1.1.5/djangocms_frontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33060 2023-07-14 14:00:41.000000 djangocms-frontend-1.1.5/djangocms_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:00:41.000000 djangocms-frontend-1.1.5/djangocms_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:00:41.000000 djangocms-frontend-1.1.5/djangocms_frontend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-14 14:00:41.000000 djangocms-frontend-1.1.5/djangocms_frontend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 14:00:41.000000 djangocms-frontend-1.1.5/djangocms_frontend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-14 14:00:41.591064 djangocms-frontend-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.583063 djangocms-frontend-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.587064 djangocms-frontend-1.1.5/tests/accordion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/accordion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/accordion/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/accordion/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.587064 djangocms-frontend-1.1.5/tests/alert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/alert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/alert/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/alert/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.587064 djangocms-frontend-1.1.5/tests/badge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/badge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/badge/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/badge/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.587064 djangocms-frontend-1.1.5/tests/card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/card/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/card/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.587064 djangocms-frontend-1.1.5/tests/carousel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/carousel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/carousel/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/carousel/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.587064 djangocms-frontend-1.1.5/tests/collapse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/collapse/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/collapse/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.587064 djangocms-frontend-1.1.5/tests/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/content/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/content/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.587064 djangocms-frontend-1.1.5/tests/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/grid/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/grid/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.587064 djangocms-frontend-1.1.5/tests/icon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/icon/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/icon/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.587064 djangocms-frontend-1.1.5/tests/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/image/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/image/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.587064 djangocms-frontend-1.1.5/tests/jumbotron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/jumbotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/jumbotron/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/jumbotron/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.587064 djangocms-frontend-1.1.5/tests/link/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/link/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/link/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/link/test_urlconf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.591064 djangocms-frontend-1.1.5/tests/listgroup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/listgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/listgroup/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/listgroup/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.591064 djangocms-frontend-1.1.5/tests/media/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/media/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/media/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.591064 djangocms-frontend-1.1.5/tests/navigation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/navigation/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/navigation/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.591064 djangocms-frontend-1.1.5/tests/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/tabs/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/tabs/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:41.591064 djangocms-frontend-1.1.5/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/utilities/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-14 14:00:32.000000 djangocms-frontend-1.1.5/tests/utilities/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.444592 djangocms-frontend-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-07-27 11:52:13.444592 djangocms-frontend-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/cms_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/background.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/responsive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/responsive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/title.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.348593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.348593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.352593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.352593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.352593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/badge.html
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/templates/djangocms_frontend/badge.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.356593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.356593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card.html
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.356593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.356593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/carousel.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.356593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.356593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.360592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.360592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/collapse.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.360592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.360592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/figure.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/code.html
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/figure.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/grid_row.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/ckeditor.icons.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.404592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   277297 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    59388 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    63664 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   123564 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   516494 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   123376 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   123452 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    54568 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   150535 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    56976 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32020 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   643290 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   127824 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   103304 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   105448 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   304476 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   105284 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105360 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28196 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    54789 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   729984 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)  2883039 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   729800 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   386256 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   282928 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    99774 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   184969 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    99564 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    56468 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    44720 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    45816 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   132305 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45648 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    45724 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.408592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/
+-rw-r--r--   0 runner    (1001) docker     (123)    48146 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30533 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35481 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18498 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15099 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23027 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35227 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.408592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.408592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.408592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.412593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)    30045 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28165 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   137737 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   115209 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20997 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18213 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    27048 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20593 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    77647 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    65062 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32569 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    26765 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.412593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.412593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/icon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.412593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/add_css.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.412593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templatetags/icon_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.412593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.412593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/image.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/jumbotron.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/jumbotron.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/list-group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/media.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/media.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/nav_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navlink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/tabs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/no_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/spacing.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/toc.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templatetags/fe_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.372593 djangocms-frontend-1.1.6/djangocms_frontend/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    35898 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    28086 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    44731 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    34046 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    28086 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    44731 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.372593 djangocms-frontend-1.1.6/djangocms_frontend/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    29617 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.372593 djangocms-frontend-1.1.6/djangocms_frontend/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37743 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.372593 djangocms-frontend-1.1.6/djangocms_frontend/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    24671 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    43925 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17985 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/bootstrap4_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.432592 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/frequency_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/stale_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/sync_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/icon_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/styled_link_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.432592 djangocms-frontend-1.1.6/djangocms_frontend/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.372593 djangocms-frontend-1.1.6/djangocms_frontend/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.372593 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.432592 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    78932 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/base.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/button_group.css
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/div_select.css
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/select2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/select2.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/auto_input.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95562 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/django_select2.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/templates/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/bootstrap5/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/bootstrap5/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/bootstrap5/menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/base-collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/html_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templatetags/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-07-27 11:52:13.000000 djangocms-frontend-1.1.6/djangocms_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33417 2023-07-27 11:52:13.000000 djangocms-frontend-1.1.6/djangocms_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:52:13.000000 djangocms-frontend-1.1.6/djangocms_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:52:13.000000 djangocms-frontend-1.1.6/djangocms_frontend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-27 11:52:13.000000 djangocms-frontend-1.1.6/djangocms_frontend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 11:52:13.000000 djangocms-frontend-1.1.6/djangocms_frontend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-27 11:52:13.444592 djangocms-frontend-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/tests/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/accordion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/accordion/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/accordion/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/tests/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/alert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/alert/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/alert/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/badge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/badge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/badge/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/badge/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/card/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/card/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/carousel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/carousel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/carousel/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/carousel/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/collapse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/collapse/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/collapse/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/content/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/content/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/grid/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/grid/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/icon/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/icon/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/image/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/image/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/jumbotron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/jumbotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/jumbotron/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/jumbotron/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/link/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/link/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/link/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/link/test_urlconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/listgroup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/listgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/listgroup/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/listgroup/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/media/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/media/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/media/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/navigation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/navigation/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/navigation/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.444592 djangocms-frontend-1.1.6/tests/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/tabs/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/tabs/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.444592 djangocms-frontend-1.1.6/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/utilities/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/utilities/test_plugins.py
```

### Comparing `djangocms-frontend-1.1.5/LICENSE` & `djangocms-frontend-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/PKG-INFO` & `djangocms-frontend-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-frontend
-Version: 1.1.5
+Version: 1.1.6
 Summary: Adds abstract User Interface items as plugins to django CMS.
 Home-page: https://github.com/django-cms/djangocms-frontend
 Author: fsbraun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-frontend-1.1.5/README.rst` & `djangocms-frontend-1.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/__init__.py` & `djangocms-frontend-1.1.6/djangocms_frontend/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
  9. git push
 10. Assure that all tests pass on https://github.com/django-cms/djangocms-frontend/actions
 11. Create a new release on https://github.com/django-cms/djangocms-frontend/releases/new
 12. Publish the release when ready
 13. Github actions will publish the new package to pypi
 """
 
-__version__ = "1.1.5"
+__version__ = "1.1.6"
```

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/common/attributes.py` & `djangocms-frontend-1.1.6/djangocms_frontend/common/attributes.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/common/bootstrap5/background.py` & `djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/background.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/common/bootstrap5/responsive.py` & `djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/responsive.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/common/bootstrap5/sizing.py` & `djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/sizing.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/common/spacing.py` & `djangocms-frontend-1.1.6/djangocms_frontend/common/spacing.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/common/title.py` & `djangocms-frontend-1.1.6/djangocms_frontend/common/title.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/models.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/badge/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/constants.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/frameworks/foundation6.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/frameworks/foundation6.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/models.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/constants.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/models.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/models.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/models.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from django.utils.translation import gettext_lazy as _
 
 from ...models import FrontendUIItem
+from .constants import CODE_TYPE_CHOICES
 
 
 class CodeBlock(FrontendUIItem):
     """
     Content > "Code" Plugin
     https://getbootstrap.com/docs/5.0/content/code/
     """
 
     class Meta:
         proxy = True
         verbose_name = _("Code block")
 
     def get_short_description(self):
-        return f"<{self.code_type}>"
+        return f'<{self.config.get("code_type", CODE_TYPE_CHOICES[0][0])}>'
 
 
 class Blockquote(FrontendUIItem):
     """
     Content > "Blockquote" Plugin
     https://getbootstrap.com/docs/5.0/content/typography/#blockquotes
     """
```

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/constants.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/frameworks/foundation6.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/frameworks/foundation6.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/models.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/conf.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/conf.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/fields.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/icon/templatetags/icon_tags.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templatetags/icon_tags.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/models.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/constants.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/helpers.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/models.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/link/views.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/listgroup/models.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/media/models.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/models.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/constants.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/models.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/cms_plugins.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/forms.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/models.py` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html` & `djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/fields.py` & `djangocms-frontend-1.1.6/djangocms_frontend/fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.6/djangocms_frontend/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/helpers.py` & `djangocms-frontend-1.1.6/djangocms_frontend/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/locale/de/LC_MESSAGES/django.mo` & `djangocms-frontend-1.1.6/djangocms_frontend/locale/de/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2022-05-05 19:13+0000\n"
-"Last-Translator: Fabian Braun <fsbraun@gmx.de>, 2022\n"
-"Language-Team: German (https://www.transifex.com/divio/teams/58664/de/)\n"
+"PO-Revision-Date: 2023-01-20 15:48+0000\n"
+"Last-Translator: Fabian Braun <fsbraun@gmx.de>, 2023\n"
+"Language-Team: German (https://app.transifex.com/divio/teams/58664/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
@@ -164,14 +164,17 @@
 msgstr ""
 "Attribute werden auf die auf die Liste für jede Einrückungstiefe im "
 "Inhaltesverzeichnis angewendet."
 
 msgid "Auto"
 msgstr "Auto"
 
+msgid "Auto start"
+msgstr "Autostart"
+
 msgid "Automatic scaling"
 msgstr "Automatische Skalierung"
 
 msgid ""
 "Autoplays the carousel after the user manually cycles the first item. If "
 "\"carousel\", autoplays the carousel on load."
 msgstr "Startet das Karussell direkt nach dem Laden."
@@ -247,14 +250,20 @@
 
 msgid "Center"
 msgstr "Mitte"
 
 msgid "Choices"
 msgstr "Optionen"
 
+msgid "Circular icon"
+msgstr "Kreisförmiges Icon"
+
+msgid "Click to add icon"
+msgstr "Klicken zum Hinzufügen"
+
 msgid "Close"
 msgstr "Schliessen"
 
 msgid "Code"
 msgstr "Code"
 
 msgid "Code block"
@@ -323,14 +332,17 @@
 msgid "Create lists of content in a card with a flush list group."
 msgstr ""
 "Erstellt eine Listengruppe, die in einer Karte eingebettet werden kann."
 
 msgid "Crop image"
 msgstr "Bild beschneiden"
 
+msgid "Cropping"
+msgstr "Beschneiden"
+
 msgid ""
 "Crops the image according to the thumbnail settings provided in the template."
 msgstr "Schneidet das Bild gemäß der Vorschau-Einstellungen in der Vorlage zu."
 
 msgid "Danger"
 msgstr "Gefahr"
 
@@ -346,23 +358,29 @@
 msgid ""
 "Defines if the grid should use fixed width, fluid width or the container "
 "should fill the full width without margins or padding."
 msgstr ""
 "Legt fest, ob das Raster feste Breiten, variable Breiten nutzt oder der "
 "Container die volle Breite ohne Rand einnehmen soll."
 
+msgid "Defines the whole template set for this navigation."
+msgstr "Legt die Vorlagen für die Navigation fest."
+
 msgid "Delegate to parent"
 msgstr "An Elternelement delegieren"
 
 msgid "Delegate to top"
 msgstr "An oberstes Element delegieren"
 
 msgid "Design"
 msgstr "Design"
 
+msgid "Determines if slides change by sliding or fading."
+msgstr "Legt fest, ob Karussell-Bild herein gleitet oder übergeblendet wird."
+
 msgid ""
 "Determines width and height of the image according to the selected ratio."
 msgstr ""
 "Bestimmt die Höhe und Breite der Bilder anhand des ausgewählten "
 "Seitenverhältnises."
 
 msgid "Device"
@@ -407,15 +425,15 @@
 msgid "Extra small"
 msgstr "Sehr klein"
 
 msgid "Extra-extra large"
 msgstr "XXL"
 
 msgid "Fade"
-msgstr "Fading"
+msgstr "Überblenden"
 
 msgid "Figure"
 msgstr "Abbildung"
 
 msgid "File link"
 msgstr "Datei-Link"
 
@@ -433,14 +451,17 @@
 
 msgid "Fluid container"
 msgstr "Container mit voller Breite"
 
 msgid "Footer"
 msgstr "Footer"
 
+msgid "Foreground context"
+msgstr "Kontext für Vordergrund"
+
 msgid "Format"
 msgstr "Format"
 
 msgid "Frontend"
 msgstr "Frontend"
 
 msgid "Full container"
@@ -508,20 +529,26 @@
 
 msgid "Horizontal size"
 msgstr "Horizontale Größe"
 
 msgid "ID"
 msgstr "ID"
 
+msgid "Icon"
+msgstr "Icon"
+
 msgid "Icon left"
 msgstr "Icon links"
 
 msgid "Icon right"
 msgstr "Icon rechts"
 
+msgid "Icon size"
+msgstr "Icon-Größe"
+
 msgid "Identifier to connect trigger with container."
 msgstr "Kennung, welche den Auslöser mit dem Collapse-Kontainer verbindet."
 
 msgid ""
 "If checked cards in one row will automatically extend to the full row height."
 msgstr "Wenn angewählt, erhalten alle Cards in einer Reihe die volle Höhe."
 
@@ -713,14 +740,17 @@
 
 msgid "Navigation container"
 msgstr "Navigationscontainer"
 
 msgid "Navigation link"
 msgstr "Navigationsverweis"
 
+msgid "Never"
+msgstr "Nie"
+
 msgid "Next"
 msgstr "Weiter"
 
 msgid "No"
 msgstr "Nein"
 
 msgid "Number of accordion items to create when saving."
@@ -729,17 +759,23 @@
 
 msgid "Number of cards to create when saving."
 msgstr "Anzahl der Karten, die beim Speichern erstellt werden soll."
 
 msgid "Number of columns to create when saving."
 msgstr "Anzahl der Spalten, die beim Speichern erstellt werden soll."
 
+msgid "Offcanvas"
+msgstr "Off-Canvas"
+
 msgid "Offset"
 msgstr "Versatz"
 
+msgid "On hover"
+msgstr "Mit Maus"
+
 msgid "One line content"
 msgstr "Inhalt (eine Zeile)"
 
 msgid "Only one of {0} or {1} may be given."
 msgstr "Nur einer aus {0} oder {1} können ausgewählt werden."
 
 msgid "Opacity of card background color (only if no outline selected)"
@@ -811,15 +847,15 @@
 
 msgid "Pills style"
 msgstr "Pillen-Stil"
 
 msgid "Please add a title if you want to publish it."
 msgstr "Bitte Titel-Attribut hinzufügen, wenn es öffentlich sein soll."
 
-msgid "Please chose a side to which the spacing should be applied."
+msgid "Please choose a side to which the spacing should be applied."
 msgstr "Bitte Seite auswählen, auf die der Abstand angewendet werden soll."
 
 msgid ""
 "Please enter at least one choice. Use the <code>+</code> symbol to add a "
 "choice."
 msgstr ""
 "Mindestens eine Option angeben. <code>+</code>-Symbol nutzen, um eine Option "
@@ -849,14 +885,17 @@
 msgid "Quote"
 msgstr "Quote"
 
 msgid ""
 "Read more in the <a href=\"{link}\" target=\"_blank\">documentation</a>."
 msgstr "Mehr in der <a href=\"{link}\" target=\"_blank\">Dokumentation</a>."
 
+msgid "Regular"
+msgstr "Schriftgröße"
+
 msgid "Removes the coloring from a button and keeps the outline."
 msgstr "Beschränkt die Färbung auf den Umriß der Schaltfläche."
 
 msgid ""
 "Removes the default background-color, some borders, and some rounded corners "
 "to render accordions edge-to-edge with their parent container "
 msgstr ""
@@ -956,23 +995,35 @@
 
 msgid "Site"
 msgstr "Website"
 
 msgid "Size"
 msgstr "Größe"
 
+msgid "Slide"
+msgstr "Gleiten"
+
 msgid "Slide image"
 msgstr "Karussell-Bild"
 
 msgid "Small"
 msgstr "Klein"
 
+msgid "Source"
+msgstr "Quelle"
+
 msgid "Spacing"
 msgstr "Abstand"
 
+msgid "Start level"
+msgstr "Start-Ebene"
+
+msgid "Start level of this page tree (0: root, 1: level below root, etc.)"
+msgstr "Start-Ebene dieser Seite (0: Wurzel, 1: erste Ebene, ...)"
+
 msgid "State"
 msgstr "Zustand"
 
 msgid "Stretch link"
 msgstr "Link ausdehnen"
 
 msgid ""
@@ -1054,14 +1105,17 @@
 
 msgid "To remove all spaces between rows set gutters to 0."
 msgstr "Um den Abstand zwischen den Spalten zu entfernen hier 0 eintragen."
 
 msgid "Top"
 msgstr "Oben"
 
+msgid "Transition"
+msgstr "Übergang"
+
 msgid "Transparent"
 msgstr "Transparent"
 
 msgid "Type"
 msgstr "Typ"
 
 msgid "UI item"
@@ -1168,7 +1222,28 @@
 
 msgid "You need to add either an image, or a URL linking to an external image."
 msgstr "Entweder ein Bild oder eine URL für ein externed Bild angeben."
 
 msgctxt "shadow"
 msgid "None"
 msgstr "Keiner"
+
+msgid "undefined"
+msgstr "undefiniert"
+
+msgid "x 12"
+msgstr "x 12"
+
+msgid "x 2"
+msgstr "x 2"
+
+msgid "x 3"
+msgstr "x 3"
+
+msgid "x 4"
+msgstr "x 4"
+
+msgid "x 5"
+msgstr "x 5"
+
+msgid "x 8"
+msgstr "x 8"
```

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/locale/de/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.6/djangocms_frontend/locale/de/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-03-11 17:20+0100\n"
 "PO-Revision-Date: 2023-01-20 15:48+0000\n"
 "Last-Translator: Fabian Braun <fsbraun@gmx.de>, 2023\n"
-"Language-Team: German (https://www.transifex.com/divio/teams/58664/de/)\n"
+"Language-Team: German (https://app.transifex.com/divio/teams/58664/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: common/attributes.py:9
```

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/locale/en/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.6/djangocms_frontend/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/locale/fr/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.6/djangocms_frontend/locale/fr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-03-11 17:20+0100\n"
 "PO-Revision-Date: 2023-01-20 15:48+0000\n"
 "Last-Translator: Adrien Delhorme, 2023\n"
-"Language-Team: French (https://www.transifex.com/divio/teams/58664/fr/)\n"
+"Language-Team: French (https://app.transifex.com/divio/teams/58664/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: common/attributes.py:9
```

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/locale/sq/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.6/djangocms_frontend/locale/sq/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# 
 # Translators:
+# Mark Walker <theshow@gmail.com>, 2023
 # Besnik Bleta <besnik@programeshqip.org>, 2023
-#
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-03-11 17:20+0100\n"
-"PO-Revision-Date: 2022-05-05 19:13+0000\n"
+"PO-Revision-Date: 2023-01-20 15:48+0000\n"
 "Last-Translator: Besnik Bleta <besnik@programeshqip.org>, 2023\n"
-"Language-Team: Albanian (https://www.transifex.com/divio/teams/58664/sq/)\n"
-"Language: sq\n"
+"Language-Team: Albanian (https://app.transifex.com/divio/teams/58664/sq/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: sq\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: common/attributes.py:9
 msgid ""
 "Advanced settings lets you add html attributes to render this element. Use "
 "them wisely and rarely."
 msgstr ""
+"Rregullimet e mëtejshme ju lejojnë të shtoni atribute HTML për shfaqjen e "
+"këtij elementi. Përdoreni me mend dhe rrallë."
 
 #: common/attributes.py:26 contrib/accordion/cms_plugins.py:91
 msgid "Advanced settings"
 msgstr "Rregullime të mëtejshme"
 
 #: common/bootstrap5/background.py:20
 msgid "Background"
@@ -47,34 +50,37 @@
 #: common/bootstrap5/background.py:57
 msgid "Background opacity"
 msgstr "Patejdukshmëri sfondi"
 
 #: common/bootstrap5/background.py:62
 msgid "Opacity of card background color (only if no outline selected)"
 msgstr ""
+"Patejdukshmëri e ngjyrës së sfondit të kartës (nëse s’është përzgjedhur "
+"përvijim)"
 
-#: common/bootstrap5/background.py:66 contrib/alert/frameworks/bootstrap5.py:42
+#: common/bootstrap5/background.py:66
+#: contrib/alert/frameworks/bootstrap5.py:42
 msgid "Shadow"
 msgstr "Hije"
 
 #: common/bootstrap5/background.py:71
 msgid "Use shadows to optically lift cards from the background."
-msgstr ""
+msgstr "Përdorni hije për t’i dalluar nga ana pamore kartat nga sfondi."
 
 #: common/bootstrap5/responsive.py:35
 msgid "Visibility"
 msgstr "Dukshmëri"
 
 #: common/bootstrap5/responsive.py:58
 msgid "Show element on device"
 msgstr "Shfaq elementin në pajisje"
 
 #: common/bootstrap5/responsive.py:60
 msgid "Select only devices on which this element should be shown."
-msgstr ""
+msgstr "Përzgjidhni vetëm pajisjet te të cilat ky element duhet shfaqur."
 
 #: common/bootstrap5/sizing.py:8 common/spacing.py:11
 #: contrib/utilities/forms.py:51 frameworks/bootstrap5.py:90
 #: frameworks/bootstrap5.py:103
 msgid "Auto"
 msgstr "Auto"
 
@@ -83,27 +89,32 @@
 msgstr "Madhësi horizontale"
 
 #: common/bootstrap5/sizing.py:50
 msgid ""
 "Sets the horizontal size relative to the surrounding container or the "
 "viewport."
 msgstr ""
+"Cakton madhësinë horizontale, relative ndaj kontejnerit ose pjesës së "
+"ekranit që e rrethon."
 
 #: common/bootstrap5/sizing.py:54
 msgid "Vertical size"
 msgstr "Madhësi vertikale"
 
 #: common/bootstrap5/sizing.py:60
 msgid ""
-"Sets the vertical size relative to the surrounding container or the viewport."
+"Sets the vertical size relative to the surrounding container or the "
+"viewport."
 msgstr ""
+"Cakton madhësinë vertikale, relative ndaj kontejnerit ose pjesës së ekranit "
+"që e rrethon."
 
 #: common/spacing.py:84
 msgid "Please choose a side to which the spacing should be applied."
-msgstr ""
+msgstr "Ju lutemi, zgjidhni një anë mbi të cilën duhet aplikuar hapësira."
 
 #: common/spacing.py:113
 msgid "Margin"
 msgstr "Mënjanë"
 
 #: common/spacing.py:139 common/spacing.py:147
 msgid "Padding"
@@ -127,14 +138,17 @@
 msgstr "Apliko mënjanë te pajisja"
 
 #: common/spacing.py:204
 msgid ""
 "Select only devices on which the margin should be applied. On other devices "
 "larger than the first selected device the margin will be set to zero."
 msgstr ""
+"Përgjidhni një anë mbi të cilën duhet aplikuar hapësira. Select only devices"
+" on which the margin should be applied. On other devices larger than the "
+"first selected device the margin will be set to zero."
 
 #: common/spacing.py:221
 msgid "Horizontal padding"
 msgstr "Mbushje horizontale"
 
 #: common/spacing.py:227
 msgid "Vertical padding"
@@ -142,31 +156,36 @@
 
 #: common/spacing.py:233
 msgid "Apply padding on device"
 msgstr "Apliko mbushje te pajisja"
 
 #: common/spacing.py:236
 msgid ""
-"Select only devices on which the padding should be applied. On other devices "
-"larger than the first selected device the padding will be set to zero."
+"Select only devices on which the padding should be applied. On other devices"
+" larger than the first selected device the padding will be set to zero."
 msgstr ""
+"Përzgjidhni vetëm pajisjet mbi të cilat duhet aplikuar mbushja. Në pajisje "
+"të tjera, më të mëdha se pajisja e parë e përzgjedhur, mbushja do të "
+"caktohet si zero."
 
 #: common/title.py:40
 msgid "Please add a title if you want to publish it."
 msgstr "Ju lutemi, shtoni një titull, nëse doni të botohet."
 
 #: common/title.py:64
 msgid "Title"
 msgstr "Titull"
 
 #: common/title.py:67
 msgid ""
-"Optional title of the plugin for easier identification. Its <code>title</"
-"code> attribute will only be set if the checkbox is selected."
+"Optional title of the plugin for easier identification. Its "
+"<code>title</code> attribute will only be set if the checkbox is selected."
 msgstr ""
+"Titull i shtojcës, në daçi, për identifikim më të kollajtë. Atributi "
+"<code>title</code> për të do të ujdiset vetëm nëse përzgjidhet kutiza."
 
 #: contrib/accordion/cms_plugins.py:21 contrib/accordion/models.py:14
 msgid "Accordion"
 msgstr "Fizarmonikë"
 
 #: contrib/accordion/cms_plugins.py:22 contrib/accordion/cms_plugins.py:72
 #: contrib/alert/cms_plugins.py:25 contrib/badge/cms_plugins.py:21
@@ -188,53 +207,56 @@
 #: contrib/utilities/cms_plugins.py:50 contrib/utilities/cms_plugins.py:62
 #: contrib/utilities/cms_plugins.py:123
 msgid "Frontend"
 msgstr "Pjesa e dukshme"
 
 #: contrib/accordion/cms_plugins.py:57
 msgid "Item {}"
-msgstr "Objket {}"
+msgstr "Objekt {}"
 
 #: contrib/accordion/cms_plugins.py:71 contrib/accordion/models.py:33
 msgid "Accordion item"
 msgstr "Objekt fizarmonike"
 
 #: contrib/accordion/forms.py:34
 msgid "Create accordion items"
 msgstr "Krijoni objekte fizarmonikë"
 
 #: contrib/accordion/forms.py:35
 msgid "Number of accordion items to create when saving."
-msgstr ""
+msgstr "Numër objektesh fizarmonikë për t’u krijuar, kur ruhet."
 
 #: contrib/accordion/forms.py:42
 msgid "Header type"
 msgstr "Lloj kryesh"
 
 #: contrib/accordion/forms.py:48
 msgid "Integrate into parent"
 msgstr "Integroje te mëma"
 
 #: contrib/accordion/forms.py:52
 msgid ""
-"Removes the default background-color, some borders, and some rounded corners "
-"to render accordions edge-to-edge with their parent container "
+"Removes the default background-color, some borders, and some rounded corners"
+" to render accordions edge-to-edge with their parent container "
 msgstr ""
+"Bën heqjen e ngjyrës parazgjedhje për sfondin, disa anë dhe disa cepa të "
+"rrumbullakosur, për t’i shfaqur fizarmonikat nga skaji në skaj, me "
+"kontejnerin e tyre mëmë "
 
 #: contrib/accordion/forms.py:78 contrib/card/constants.py:16
 msgid "Header"
 msgstr "Krye"
 
 #: contrib/accordion/forms.py:82
 msgid "Item open"
 msgstr ""
 
 #: contrib/accordion/forms.py:85
 msgid "Initially shows this accordion item on page load."
-msgstr ""
+msgstr "E shfaq fillimisht këtë objekt fizarmonikë gjatë ngarkimit të faqes."
 
 #: contrib/accordion/models.py:20
 msgid "({} entries)"
 msgstr "({} zëra)"
 
 #: contrib/accordion/models.py:29
 msgid "AccordionItem"
@@ -251,15 +273,15 @@
 
 #: contrib/alert/forms.py:47
 msgid "Dismissible"
 msgstr "Që mund të hidhet tej"
 
 #: contrib/alert/forms.py:50
 msgid "Allows the alert to be closed."
-msgstr ""
+msgstr "Lejon mbylljen e sinjalizimit."
 
 #: contrib/alert/frameworks/bootstrap5.py:47
 msgid "Use shadows to optically lift alerts from the background."
 msgstr "Përdorni hije për t’i dalluar nga ana pamore sinjalizimet nga sfondi."
 
 #: contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html:4
 msgid "Close"
@@ -279,32 +301,32 @@
 
 #: contrib/badge/forms.py:46
 msgid "Activates the pills style."
 msgstr "Aktivizon stilin e sumbullave."
 
 #: contrib/card/cms_plugins.py:24 contrib/card/models.py:20
 msgid "Card layout"
-msgstr ""
+msgstr "Skemë karte"
 
 #: contrib/card/cms_plugins.py:47 contrib/grid/cms_plugins.py:93
 #: contrib/grid/cms_plugins.py:173
 msgid "Responsive settings"
 msgstr "Rregullime reaguese"
 
 #: contrib/card/cms_plugins.py:85 contrib/card/models.py:35
 msgid "Card"
-msgstr ""
+msgstr "Kartë"
 
 #: contrib/card/cms_plugins.py:145 contrib/card/models.py:57
 msgid "Card inner"
 msgstr ""
 
 #: contrib/card/constants.py:4
 msgid "Card group"
-msgstr ""
+msgstr "Grup karte"
 
 #: contrib/card/constants.py:5
 msgid "Grid cards"
 msgstr ""
 
 #: contrib/card/constants.py:9 contrib/utilities/forms.py:108
 #: frameworks/bootstrap5.py:59 settings.py:47
@@ -334,31 +356,31 @@
 
 #: contrib/card/forms.py:35 contrib/card/models.py:9
 msgid "White"
 msgstr "E bardhë"
 
 #: contrib/card/forms.py:61
 msgid "Create cards"
-msgstr ""
+msgstr "Krijoni karta"
 
 #: contrib/card/forms.py:62
 msgid "Number of cards to create when saving."
-msgstr ""
+msgstr "Numër kartash për t’u krijuar, kur ruhet."
 
 #: contrib/card/forms.py:68
 msgid "Card type"
 msgstr "Lloj karte"
 
 #: contrib/card/forms.py:122
 msgid "Card outline context"
 msgstr ""
 
 #: contrib/card/forms.py:126
 msgid "Uses the border to indicate context."
-msgstr "Përdor anën për të treguar kontekstin"
+msgstr "Përdor anën për të treguar kontekstin."
 
 #: contrib/card/forms.py:132 contrib/content/forms.py:99
 #: contrib/content/forms.py:137 contrib/grid/cms_plugins.py:99
 #: contrib/image/forms.py:147 contrib/tabs/forms.py:57
 #: contrib/utilities/forms.py:139
 msgid "Alignment"
 msgstr "Drejtim"
@@ -369,16 +391,19 @@
 
 #: contrib/card/forms.py:148
 msgid "Full height"
 msgstr "Lartësi e plotë"
 
 #: contrib/card/forms.py:152
 msgid ""
-"If checked cards in one row will automatically extend to the full row height."
+"If checked cards in one row will automatically extend to the full row "
+"height."
 msgstr ""
+"Në iu vëntë shenjë, kartat e një rreshti do të zgjerohen vetvetiu sa "
+"lartësia e plotë e rreshtit."
 
 #: contrib/card/forms.py:186
 msgid "Inner type"
 msgstr "Lloj i Brendshëm"
 
 #: contrib/card/forms.py:189
 msgid "Define the structure of the plugin."
@@ -439,35 +464,35 @@
 
 #: contrib/carousel/forms.py:64 contrib/carousel/models.py:24
 msgid "Interval"
 msgstr "Interval"
 
 #: contrib/carousel/forms.py:67
 msgid ""
-"The amount of time to delay between automatically cycling an item. If false, "
-"carousel will not automatically cycle."
+"The amount of time to delay between automatically cycling an item. If false,"
+" carousel will not automatically cycle."
 msgstr ""
 "Sasia e kohës në sekonda për vonim zërash te kalimi automatikisht në ta. Në "
 "u vëntë 0, rrotullamja s’do të kalojë automatikisht nëpër ta."
 
 #: contrib/carousel/forms.py:72 contrib/carousel/models.py:25
 msgid "Controls"
 msgstr "Kontrolle"
 
 #: contrib/carousel/forms.py:75
 msgid "Adding in the previous and next controls."
-msgstr "Po shtohet te kontrollet “i mëparshmi” dhe “pasuesi”."
+msgstr "Po shtohen kontrollet “i mëparshmi” dhe “pasuesi”."
 
 #: contrib/carousel/forms.py:78 contrib/carousel/models.py:26
 msgid "Indicators"
 msgstr "Tregues"
 
 #: contrib/carousel/forms.py:81
 msgid "Adding in the indicators to the carousel."
-msgstr "Po shtohet te treguesit te rrotullamja."
+msgstr "Po shtohen treguesit te rrotullamja."
 
 #: contrib/carousel/forms.py:84 contrib/carousel/models.py:27
 msgid "Keyboard"
 msgstr "Tastierë"
 
 #: contrib/carousel/forms.py:87
 msgid "Whether the carousel should react to keyboard events."
@@ -479,49 +504,55 @@
 
 #: contrib/carousel/forms.py:94
 msgid ""
 "If set to \"hover\", pauses the cycling of the carousel on \"mouseenter\" "
 "and resumes the cycling of the carousel on \"mouseleave\". If set to "
 "\"false\", hovering over the carousel won't pause it."
 msgstr ""
+"Në u vëntë si “hover”, e ndal rrotullimin e rrotullames pas një akti "
+"“mouseenter” dhe e rifillon rrotullimin e rrotullames pas një akti "
+"“mouseleave”. Në u vëntë si “false”, kalimi i kursorit mbi rrotullamen s’do "
+"ta ndalë atë."
 
 #: contrib/carousel/forms.py:102
 msgid "Auto start"
 msgstr ""
 
 #: contrib/carousel/forms.py:106
 msgid ""
 "Autoplays the carousel after the user manually cycles the first item. If "
 "\"carousel\", autoplays the carousel on load."
 msgstr ""
 "Vetëluhet rrotullamja, pasi përdoruesi vë në punë dorazi kuadrin e parë. Në "
-"u vëntë “carousel”, vetëluhet automatikisht rrotullamja, kur ngarkohet faqja."
+"u vëntë “carousel”, vetëluhet automatikisht rrotullamja, kur ngarkohet "
+"faqja."
 
 #: contrib/carousel/forms.py:111 contrib/carousel/models.py:30
 msgid "Wrap"
 msgstr ""
 
 #: contrib/carousel/forms.py:115
 msgid "Whether the carousel should cycle continuously or have hard stops."
 msgstr ""
+"Nëse rrotullamja duhet të rrotullohet vazhdimisht, apo të ketë ndalesa."
 
 #: contrib/carousel/forms.py:119
 msgid "Aspect ratio"
-msgstr "Përpjestim"
+msgstr "Përpjesëtim"
 
 #: contrib/carousel/forms.py:124
 msgid ""
 "Determines width and height of the image according to the selected ratio."
 msgstr ""
+"Përcakton gjerësinë dhe lartësinë e fizarmonikës së figurave sa përpjesëtimi"
+" i përzgjedhur."
 
 #: contrib/carousel/forms.py:129
-#, fuzzy
-#| msgid "Navigation"
 msgid "Transition"
-msgstr "Lëvizje"
+msgstr ""
 
 #: contrib/carousel/forms.py:133
 msgid "Determines if slides change by sliding or fading."
 msgstr ""
 
 #: contrib/carousel/forms.py:177
 msgid "Slide image"
@@ -529,15 +560,15 @@
 
 #: contrib/carousel/forms.py:181
 msgid "Content"
 msgstr "Lëndë"
 
 #: contrib/carousel/forms.py:184
 msgid "Content may also be added using child plugins."
-msgstr ""
+msgstr "Lëndë mund të shtohet edhe duke përdorur shtojca pjellë."
 
 #: contrib/carousel/models.py:29
 msgid "Ride"
 msgstr ""
 
 #: contrib/carousel/models.py:51 contrib/image/models.py:154
 msgid "<file is missing>"
@@ -623,15 +654,15 @@
 
 #: contrib/content/forms.py:90
 msgid "Quote"
 msgstr "Citim"
 
 #: contrib/content/forms.py:95
 msgid "Source"
-msgstr ""
+msgstr "Burim"
 
 #: contrib/content/forms.py:132
 msgid "Caption"
 msgstr "Titull"
 
 #: contrib/grid/cms_plugins.py:36 contrib/grid/constants.py:19
 #: contrib/grid/models.py:28 contrib/navigation/forms.py:48
@@ -708,14 +739,16 @@
 msgstr "Lloj kontejneri"
 
 #: contrib/grid/forms.py:65
 msgid ""
 "Defines if the grid should use fixed width, fluid width or the container "
 "should fill the full width without margins or padding."
 msgstr ""
+"Përcakton nëse rrjeta duhet të përdorë gjerësi të fiksuar, të ndryshueshme "
+"apo kontejneri duhet të mbushë gjerësinë e plotë, pa mënjana apo mbushje."
 
 #: contrib/grid/forms.py:97
 msgid "Create columns"
 msgstr "Krijoni shtylla"
 
 #: contrib/grid/forms.py:98
 msgid "Number of columns to create when saving."
@@ -742,14 +775,16 @@
 msgstr "Drejtim shtylle"
 
 #: contrib/grid/forms.py:195
 #, python-format
 msgid ""
 "Column size needs to be empty, \"auto\", or a number between 1 and %(cols)d"
 msgstr ""
+"Madhësia e shtyllës lypset të jetë e zbrazët, “auto”, ose një numër mes 1 "
+"dhe %(cols)d"
 
 #: contrib/grid/models.py:29
 msgid "GridContainer"
 msgstr ""
 
 #: contrib/grid/models.py:56
 msgid "GridRow"
@@ -788,18 +823,16 @@
 
 #: contrib/grid/templates/djangocms_frontend/admin/grid_column.html:21
 msgid "Reset"
 msgstr "Riktheje te parazgjedhje"
 
 #: contrib/icon/apps.py:7 contrib/icon/cms_plugins.py:29
 #: contrib/icon/models.py:14
-#, fuzzy
-#| msgid "Icon left"
 msgid "Icon"
-msgstr "Ikonë majtas"
+msgstr ""
 
 #: contrib/icon/conf.py:52
 msgid "Regular"
 msgstr ""
 
 #: contrib/icon/conf.py:53
 msgid "x 2"
@@ -822,34 +855,28 @@
 msgstr ""
 
 #: contrib/icon/conf.py:58
 msgid "x 12"
 msgstr ""
 
 #: contrib/icon/forms.py:43
-#, fuzzy
-#| msgid "Button size"
 msgid "Icon size"
-msgstr "Madhësi butoni"
+msgstr ""
 
 #: contrib/icon/forms.py:49
-#, fuzzy
-#| msgid "Background context"
 msgid "Foreground context"
-msgstr "Kontekst sfondi"
+msgstr ""
 
 #: contrib/icon/forms.py:56
 msgid "Circular icon"
 msgstr ""
 
 #: contrib/icon/models.py:17
-#, fuzzy
-#| msgid "Rounded"
 msgid "undefined"
-msgstr "Rrumbullake"
+msgstr ""
 
 #: contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html:5
 msgid "Click to add icon"
 msgstr ""
 
 #: contrib/image/cms_plugins.py:30
 msgid "Picture / Image"
@@ -857,15 +884,15 @@
 
 #: contrib/image/cms_plugins.py:56
 msgid "Format"
 msgstr "Formatoje"
 
 #: contrib/image/cms_plugins.py:67
 msgid "Cropping"
-msgstr ""
+msgstr "Qethje"
 
 #: contrib/image/forms.py:25
 msgid "Align left"
 msgstr "Vëre majtas"
 
 #: contrib/image/forms.py:26
 msgid "Align right"
@@ -912,56 +939,58 @@
 msgstr "Figurë e jashtme"
 
 #: contrib/image/forms.py:118
 msgid ""
 "If provided, overrides the embedded image. Certain options such as cropping "
 "are not applicable to external images."
 msgstr ""
-"Nëse jepet, anashkalon figurën e trupëzuar. Disa mundësi, bie fjala, qethja, "
-"s’janë të zbatueshme mbi figura të jashtme."
+"Nëse jepet, anashkalon figurën e trupëzuar. Disa mundësi, bie fjala, qethja,"
+" s’janë të zbatueshme mbi figura të jashtme."
 
 #: contrib/image/forms.py:123
 msgid "Load lazily"
-msgstr ""
+msgstr "Ngarkim dembel"
 
 #: contrib/image/forms.py:126
 msgid ""
 "Use for images below the fold. This will load images only if user scrolls "
 "them into view. "
 msgstr ""
+"Përdoreni për figura nën palosjen. Kjo do të ngarkojë figurat vetëm nëse "
+"përdoruesi rrëshqet në faqe dhe ato vijnë në pamje. "
 
 #: contrib/image/forms.py:131
 msgid "Width"
 msgstr "Gjerësi"
 
 #: contrib/image/forms.py:135
-msgid ""
-"The image width as number in pixels. Example: \"720\" and not \"720px\"."
-msgstr "Gjerësia e figurës si numër pikselash. Shembull: “720” dhe jo “720px”."
+msgid "The image width as number in pixels. Example: \"720\" and not \"720px\"."
+msgstr ""
+"Gjerësia e figurës si numër pikselash. Shembull: “720” dhe jo “720px”."
 
 #: contrib/image/forms.py:139
 msgid "Height"
 msgstr "Lartësi"
 
 #: contrib/image/forms.py:143
-msgid ""
-"The image height as number in pixels. Example: \"720\" and not \"720px\"."
-msgstr "Lartësia e figurës si numër pikselash. Shembull: “720” dhe jo “720px”."
+msgid "The image height as number in pixels. Example: \"720\" and not \"720px\"."
+msgstr ""
+"Lartësia e figurës si numër pikselash. Shembull: “720” dhe jo “720px”."
 
 #: contrib/image/forms.py:150
 msgid "Aligns the image according to the selected option."
 msgstr "E drejton figurën sipas mundësisë së përzgjedhur."
 
 #: contrib/image/forms.py:153 contrib/utilities/forms.py:167
 msgid "Link attributes"
 msgstr "Atribute lidhjeje"
 
 #: contrib/image/forms.py:154
 msgid "Attributes apply to the <b>link</b>."
-msgstr ""
+msgstr "Atribute që aplikohen mbi <b>lidhjen</b>."
 
 #: contrib/image/forms.py:160
 msgid "Automatic scaling"
 msgstr "Përshkallëzim automatik"
 
 #: contrib/image/forms.py:163
 msgid "Uses the placeholder dimensions to automatically calculate the size."
@@ -978,15 +1007,16 @@
 
 #: contrib/image/forms.py:176
 msgid "Crop image"
 msgstr "Qetheni figurën"
 
 #: contrib/image/forms.py:179
 msgid ""
-"Crops the image according to the thumbnail settings provided in the template."
+"Crops the image according to the thumbnail settings provided in the "
+"template."
 msgstr "E qeth figurën sipas rregullimeve miniaturash të dhëna te gjedhja."
 
 #: contrib/image/forms.py:183
 msgid "Upscale image"
 msgstr ""
 
 #: contrib/image/forms.py:186
@@ -996,18 +1026,21 @@
 
 #: contrib/image/forms.py:190
 msgid "Use responsive image"
 msgstr "Përdor figurë reaguese"
 
 #: contrib/image/forms.py:194
 msgid ""
-"Uses responsive image technique to choose better image to display based upon "
-"screen viewport. This configuration only applies to uploaded images "
+"Uses responsive image technique to choose better image to display based upon"
+" screen viewport. This configuration only applies to uploaded images "
 "(external pictures will not be affected). "
 msgstr ""
+"Përdor teknikën e figurave reaguese për të zgjedhur figurë më të mirë për "
+"shfaqje, bazuar në ekranin e parjes. Ky formësim zbatohet vetëm mbi figurat "
+"e ngarkuara (fotot e jashtme nuk do të preken prej kësaj). "
 
 #: contrib/image/forms.py:203
 msgid "Thumbnail options"
 msgstr "Mundësi miniaturash"
 
 #: contrib/image/forms.py:206
 msgid ""
@@ -1019,40 +1052,43 @@
 
 #: contrib/image/forms.py:210
 msgid "Responsive"
 msgstr "Reaguese"
 
 #: contrib/image/forms.py:213
 msgid "Adds the .img-fluid class to make the image responsive."
-msgstr ""
+msgstr "Shton klasën .img-fluid për ta bërë figurën reaguese."
 
 #: contrib/image/forms.py:216
 msgid "Rounded"
 msgstr "Rrumbullake"
 
 #: contrib/image/forms.py:219
 msgid "Adds the .rounded class for round corners."
-msgstr ""
+msgstr "Shton klasën .rounded për cepa të rrumbullakët."
 
 #: contrib/image/forms.py:222
 msgid "Thumbnail"
 msgstr "Miniaturë"
 
 #: contrib/image/forms.py:225
 msgid "Adds the .img-thumbnail class."
 msgstr "Shton .img-thumbnail class."
 
 #: contrib/image/forms.py:246
 msgid ""
 "You have given more than one external, internal, or file link target. Only "
 "one option is allowed."
 msgstr ""
+"Keni dhënë më shumë se një objektiv të jashtëm, të brendshëm, ose lidhje për"
+" te kartelë. Lejohet vetëm një mundësi."
 
 #: contrib/image/forms.py:255
-msgid "You need to add either an image, or a URL linking to an external image."
+msgid ""
+"You need to add either an image, or a URL linking to an external image."
 msgstr ""
 "Lypset të shtoni ose një figurë, ose një URL që shpie te një figurë e "
 "jashtme."
 
 #: contrib/image/forms.py:281
 #, python-brace-format
 msgid ""
@@ -1069,14 +1105,15 @@
 #: contrib/jumbotron/forms.py:49 contrib/jumbotron/models.py:19
 msgid "Fluid"
 msgstr ""
 
 #: contrib/jumbotron/forms.py:53
 msgid "Makes the jumbotron fill the full width of the container or window."
 msgstr ""
+"E bën jumbotron-in të mbushë krejt gjerësinë e kontejnerit ose dritares."
 
 #: contrib/link/apps.py:11 contrib/link/constants.py:5
 #: contrib/link/models.py:11 contrib/link/models.py:114
 msgid "Link"
 msgstr "Lidhje"
 
 #: contrib/link/cms_plugins.py:97
@@ -1194,14 +1231,16 @@
 msgstr "Shformoje lidhjen"
 
 #: contrib/link/forms.py:329
 msgid ""
 "Stretches the active link area to the containing block (with position: "
 "relative)."
 msgstr ""
+"E tendos fushën e lidhjes aktive sa blloku që e përmban (me pozicionin: "
+"relative)."
 
 #: contrib/link/forms.py:333 contrib/tabs/forms.py:51
 msgid "Type"
 msgstr "Lloj"
 
 #: contrib/link/forms.py:337
 msgid "Adds either a text link or a button which links to the target."
@@ -1221,15 +1260,15 @@
 
 #: contrib/link/forms.py:362
 msgid "Block"
 msgstr ""
 
 #: contrib/link/forms.py:365
 msgid "Extends the button to the width of its container."
-msgstr ""
+msgstr "E zgjeron butonin sa gjerësia e kontejnerit përkatës."
 
 #: contrib/link/forms.py:368
 msgid "Icon left"
 msgstr "Ikonë majtas"
 
 #: contrib/link/forms.py:373
 msgid "Icon right"
@@ -1310,35 +1349,37 @@
 
 #: contrib/navigation/cms_plugins.py:164
 msgid "Navigation link"
 msgstr "Lidhje lëvizjeje"
 
 #: contrib/navigation/forms.py:45
 msgid "Defines the whole template set for this navigation."
-msgstr ""
+msgstr "Përcakton krejt grupin e gjedheve për këtë menu lëvizjesh."
 
 #: contrib/navigation/forms.py:53
 msgid "Design"
 msgstr ""
 
 #: contrib/navigation/forms.py:60
 msgid "Expand on device (and larger)"
-msgstr ""
+msgstr "Zgjeroje në pajisje (dhe më të mëdha)"
 
 #: contrib/navigation/forms.py:81
 msgid "Start level"
-msgstr ""
+msgstr "Nivel fillimi"
 
 #: contrib/navigation/forms.py:84
 msgid "Start level of this page tree (0: root, 1: level below root, etc.)"
 msgstr ""
+"Nivel fillimi për këtë pemë faqesh (0: rrënjë, 1: niveli nën rrënjë, etj.)"
 
 #: contrib/navigation/forms.py:106
 msgid "Enter brand name or add child plugins for brand icon or image"
-msgstr "Jepni emër marke, ose shtoni shtojca pjellë për ikonë ose figurë marke"
+msgstr ""
+"Jepni emër marke, ose shtoni shtojca pjellë për ikonë ose figurë marke"
 
 #: contrib/navigation/models.py:30
 msgid "Navigation Link"
 msgstr "Lidhje Lëvizjeje"
 
 #: contrib/tabs/cms_plugins.py:24 contrib/tabs/constants.py:5
 msgid "Tabs"
@@ -1354,15 +1395,15 @@
 
 #: contrib/tabs/constants.py:10
 msgid "Fill"
 msgstr "Mbushje"
 
 #: contrib/tabs/constants.py:11
 msgid "Justified"
-msgstr ""
+msgstr "Përligjur"
 
 #: contrib/tabs/constants.py:12
 msgid "Justify start"
 msgstr ""
 
 #: contrib/tabs/constants.py:13
 msgid "Justify center"
@@ -1375,14 +1416,15 @@
 #: contrib/tabs/forms.py:64
 msgid "Index"
 msgstr "Tregues"
 
 #: contrib/tabs/forms.py:67
 msgid "Index of element to open on page load starting at 1."
 msgstr ""
+"Tregues elementësh për t’u hapur në ngarkim faqeje, duke filluar me 1."
 
 #: contrib/tabs/forms.py:70
 msgid "Animation effect"
 msgstr "Efekt animacioni"
 
 #: contrib/tabs/forms.py:96
 msgid "Tab title"
@@ -1430,20 +1472,24 @@
 msgstr "Pajisje"
 
 #: contrib/utilities/forms.py:74
 msgid ""
 "Padding does not have an auto spacing. Either switch to margin or a defined "
 "size."
 msgstr ""
+"Mbushja s’ka aplikim vetvetiu hapësire. Ose kaloni te mënjanë, ose te një "
+"madhësi e përcaktuar."
 
 #: contrib/utilities/forms.py:78
 msgid ""
 "Padding does not have an auto spacing. Either switch to a defined size or "
 "change the spacing property."
 msgstr ""
+"Mbushja s’ka aplikim vetvetiu hapësire. Ose kaloni te një madhësi e "
+"përcaktuar, ose ndryshoni vetinë për hapësira."
 
 #: contrib/utilities/forms.py:101 settings.py:38
 msgid "Heading 1"
 msgstr "Krye 1"
 
 #: contrib/utilities/forms.py:102 settings.py:39
 msgid "Heading 2"
@@ -1467,45 +1513,48 @@
 
 #: contrib/utilities/forms.py:125
 msgid "ID"
 msgstr "ID"
 
 #: contrib/utilities/forms.py:128
 msgid ""
-"Fill in unique ID for table of contents. If empty heading will not appear in "
-"table of contents."
+"Fill in unique ID for table of contents. If empty heading will not appear in"
+" table of contents."
 msgstr ""
+"Plotësoni ID unike për tryezë lënde. Në u lëntë e zbrazët, kryet s’do të "
+"duken te tryezë e lëndës."
 
 #: contrib/utilities/forms.py:132
 msgid "Heading context"
 msgstr "Kontekst kryesh"
 
 #: contrib/utilities/forms.py:160
 msgid "List attributes"
-msgstr ""
+msgstr "Atribute liste"
 
 #: contrib/utilities/forms.py:162
 msgid ""
 "Attributes apply to the <b>list</b> for each level in the table of contents."
-msgstr ""
+msgstr "Atribute aplikohen te <b>lista</b> për çdo nivel te tryeza e lëndës."
 
 #: contrib/utilities/forms.py:169
 msgid ""
 "Attributes apply to the <b>link</b> for each entry in the table of contents."
-msgstr ""
+msgstr "Atribute aplikohen te <b>lidhja</b> për çdo nivel te tryeza e lëndës."
 
 #: contrib/utilities/forms.py:173
 msgid "Item attributes"
 msgstr "Atribute objekti"
 
 #: contrib/utilities/forms.py:175
 msgid ""
 "Attributes apply to the <b>list items</b> for each entry in the table of "
 "contents."
 msgstr ""
+"Atribute aplikohen te <b>zëra liste</b> për çdo zë te tryeza e lëndës."
 
 #: fields.py:94
 msgid "Please select at least one device size"
 msgstr "Ju lutemi, përzgjidhni të paktën një madhësi pajisjeje"
 
 #: fields.py:102 fields.py:110
 msgid "Attributes"
@@ -1516,14 +1565,16 @@
 msgstr "Zgjedhje"
 
 #: fields.py:142
 msgid ""
 "Please enter at least one choice. Use the <code>+</code> symbol to add a "
 "choice."
 msgstr ""
+"Ju lutemi, jepni të paktën një zgjedhje. Që të shtoni një zgjedhje, përdorni"
+" simbolin <code>+</code>."
 
 #: fields.py:161 fields.py:175
 msgid "Tag type"
 msgstr "Lloj etikete"
 
 #: fields.py:169
 msgid "Select the HTML tag to be used."
@@ -1600,23 +1651,22 @@
 
 #: frameworks/bootstrap5.py:137
 msgid "XX large"
 msgstr ""
 
 #: helpers.py:112
 #, python-brace-format
-msgid ""
-"Read more in the <a href=\"{link}\" target=\"_blank\">documentation</a>."
-msgstr ""
-"Lexoni më tepër, te <a href=\"{link}\" target=\"_blank\">dokumentimi</a>."
+msgid "Read more in the <a href=\"{link}\" target=\"_blank\">documentation</a>."
+msgstr "Lexoni më tepër, te <a href=\"{link}\" target=\"_blank\">dokumentimi</a>."
 
 #: models.py:24
 msgid "UI item"
 msgstr "Element UI"
 
 #: settings.py:14
 msgid "There are no further settings for this plugin. Please press save."
-msgstr "S’ka rregullime të tjera për këtë shtojcë. Ju lutemi, shtypni “Ruaje”."
+msgstr ""
+"S’ka rregullime të tjera për këtë shtojcë. Ju lutemi, shtypni “Ruaje”."
 
 #: settings.py:73
 msgid "Offcanvas"
 msgstr ""
```

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/management/bootstrap4_migration.py` & `djangocms-frontend-1.1.6/djangocms_frontend/management/bootstrap4_migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,19 @@
             elif prop == "mr":
                 lst.append(f"{size}_mr -> {size}_me")
             else:
                 lst.append(f"{size}_{prop}")
     return lst
 
 
+plugin_names = {
+    "CodeBlock": "CodePlugin",
+}
+
+
 plugin_migrations = {
     "bootstrap4_alerts.Bootstrap4Alerts -> alert.Alert": [
         "alert_context",
         "alert_dismissable -> alert_dismissible",
         "tag_type",
         "attributes",
         "P001",  # additional data migration, see below
@@ -87,14 +92,15 @@
         "M001-m",  # SpacingMixin
         "M001-p",  # SpacingMixin
         "M002",  # ResponsiveMixin
         "M003",  # BackgroundMixin
     ],
     "bootstrap4_content.Bootstrap4Code -> content.CodeBlock": [
         "code_content",
+        "tag_type -> code_type",
         "attributes",
         "P001",
         "M001-m",  # SpacingMixin
         "M001-p",  # SpacingMixin
         "M002",  # ResponsiveMixin
         "M003",  # BackgroundMixin
     ],
```

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/management/commands/frontend.py` & `djangocms-frontend-1.1.6/djangocms_frontend/management/commands/frontend.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/management/commands/subcommands/base.py` & `djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/management/commands/subcommands/frequency_analysis.py` & `djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/frequency_analysis.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/management/commands/subcommands/migrate.py` & `djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/migrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # Bootstrap 4
 if "djangocms_bootstrap4" in apps.all_models:
     from djangocms_frontend.management import bootstrap4_migration
 
     plugin_migrations.update(bootstrap4_migration.plugin_migrations)
     data_migration.update(bootstrap4_migration.data_migration)
     plugin_prefixes.append(bootstrap4_migration.plugin_prefix)
+    plugin_names.update(bootstrap4_migration.plugin_names)
 # Styled link
 if "djangocms_styledlink" in apps.all_models:
     from djangocms_frontend.management import styled_link_migration
 
     plugin_migrations.update(styled_link_migration.plugin_migrations)
     data_migration.update(styled_link_migration.data_migration)
     plugin_prefixes.append(styled_link_migration.plugin_prefix)
@@ -44,14 +45,16 @@
 
     for migration_module_path in additional_migrations:
         try:
             migration_module = importlib.import_module(migration_module_path)
             plugin_migrations.update(migration_module.plugin_migrations)
             data_migration.update(migration_module.data_migration)
             plugin_prefixes.append(migration_module.plugin_prefix)
+            if hasattr(migration_module, "plugin_names"):
+                plugin_names.update(migration_module.plugin_names)
         except ModuleNotFoundError:
             print(f"Warning: can not import migration module: {migration_module_path}.")
 
 
 def migrate_to_djangocms_frontend(apps, schema_editor):
     cnt = 0
     for plugin_model, fields in plugin_migrations.items():
```

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/management/commands/subcommands/stale_references.py` & `djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/stale_references.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/management/commands/subcommands/sync_permissions.py` & `djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/sync_permissions.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/management/icon_migration.py` & `djangocms-frontend-1.1.6/djangocms_frontend/management/icon_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/management/styled_link_migration.py` & `djangocms-frontend-1.1.6/djangocms_frontend/management/styled_link_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/migrations/0001_initial.py` & `djangocms-frontend-1.1.6/djangocms_frontend/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/models.py` & `djangocms-frontend-1.1.6/djangocms_frontend/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/settings.py` & `djangocms-frontend-1.1.6/djangocms_frontend/settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/css/base.css` & `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/base.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/css/base.css.map` & `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/base.css.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/css/button_group.css` & `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/button_group.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map` & `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/css/select2.css` & `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/select2.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/js/auto_input.js` & `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/auto_input.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js` & `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js` & `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js` & `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/static/djangocms_frontend/js/django_select2.js` & `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/django_select2.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/templates/bootstrap5/base.html` & `djangocms-frontend-1.1.6/djangocms_frontend/templates/bootstrap5/base.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/templates/bootstrap5/menu.html` & `djangocms-frontend-1.1.6/djangocms_frontend/templates/bootstrap5/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html` & `djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html` & `djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html` & `djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html` & `djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html` & `djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html` & `djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/templates/djangocms_frontend.html` & `djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend/templatetags/frontend.py` & `djangocms-frontend-1.1.6/djangocms_frontend/templatetags/frontend.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend.egg-info/PKG-INFO` & `djangocms-frontend-1.1.6/djangocms_frontend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-frontend
-Version: 1.1.5
+Version: 1.1.6
 Summary: Adds abstract User Interface items as plugins to django CMS.
 Home-page: https://github.com/django-cms/djangocms-frontend
 Author: fsbraun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-frontend-1.1.5/djangocms_frontend.egg-info/SOURCES.txt` & `djangocms-frontend-1.1.6/djangocms_frontend.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -370,19 +370,26 @@
 djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/no_form.html
 djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/spacing.html
 djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html
 djangocms_frontend/contrib/utilities/templatetags/__init__.py
 djangocms_frontend/contrib/utilities/templatetags/fe_utilities.py
 djangocms_frontend/frameworks/__init__.py
 djangocms_frontend/frameworks/bootstrap5.py
+djangocms_frontend/locale/ar/LC_MESSAGES/django.mo
+djangocms_frontend/locale/ar/LC_MESSAGES/django.po
 djangocms_frontend/locale/de/LC_MESSAGES/django.mo
 djangocms_frontend/locale/de/LC_MESSAGES/django.po
 djangocms_frontend/locale/en/LC_MESSAGES/django.mo
 djangocms_frontend/locale/en/LC_MESSAGES/django.po
+djangocms_frontend/locale/es/LC_MESSAGES/django.mo
+djangocms_frontend/locale/es/LC_MESSAGES/django.po
+djangocms_frontend/locale/fr/LC_MESSAGES/django.mo
 djangocms_frontend/locale/fr/LC_MESSAGES/django.po
+djangocms_frontend/locale/nl/LC_MESSAGES/django.mo
+djangocms_frontend/locale/nl/LC_MESSAGES/django.po
 djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
 djangocms_frontend/locale/sq/LC_MESSAGES/django.po
 djangocms_frontend/management/__init__.py
 djangocms_frontend/management/bootstrap4_migration.py
 djangocms_frontend/management/icon_migration.py
 djangocms_frontend/management/styled_link_migration.py
 djangocms_frontend/management/commands/__init__.py
```

### Comparing `djangocms-frontend-1.1.5/pyproject.toml` & `djangocms-frontend-1.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/setup.py` & `djangocms-frontend-1.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/accordion/test_models.py` & `djangocms-frontend-1.1.6/tests/accordion/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/accordion/test_plugins.py` & `djangocms-frontend-1.1.6/tests/accordion/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/alert/test_plugins.py` & `djangocms-frontend-1.1.6/tests/alert/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/badge/test_plugins.py` & `djangocms-frontend-1.1.6/tests/badge/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/card/test_models.py` & `djangocms-frontend-1.1.6/tests/card/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/card/test_plugins.py` & `djangocms-frontend-1.1.6/tests/card/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/carousel/test_models.py` & `djangocms-frontend-1.1.6/tests/carousel/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/carousel/test_plugins.py` & `djangocms-frontend-1.1.6/tests/carousel/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/collapse/test_models.py` & `djangocms-frontend-1.1.6/tests/collapse/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/collapse/test_plugins.py` & `djangocms-frontend-1.1.6/tests/collapse/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/content/test_models.py` & `djangocms-frontend-1.1.6/tests/content/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/content/test_plugins.py` & `djangocms-frontend-1.1.6/tests/content/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/fixtures.py` & `djangocms-frontend-1.1.6/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/grid/test_models.py` & `djangocms-frontend-1.1.6/tests/grid/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/grid/test_plugins.py` & `djangocms-frontend-1.1.6/tests/grid/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/helpers.py` & `djangocms-frontend-1.1.6/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/icon/test_models.py` & `djangocms-frontend-1.1.6/tests/icon/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/icon/test_plugins.py` & `djangocms-frontend-1.1.6/tests/icon/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/image/test_plugins.py` & `djangocms-frontend-1.1.6/tests/image/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/jumbotron/test_plugins.py` & `djangocms-frontend-1.1.6/tests/jumbotron/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/link/test_plugins.py` & `djangocms-frontend-1.1.6/tests/link/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/link/test_urlconf.py` & `djangocms-frontend-1.1.6/tests/link/test_urlconf.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/listgroup/test_models.py` & `djangocms-frontend-1.1.6/tests/listgroup/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/listgroup/test_plugins.py` & `djangocms-frontend-1.1.6/tests/listgroup/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/media/test_models.py` & `djangocms-frontend-1.1.6/tests/media/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/media/test_plugins.py` & `djangocms-frontend-1.1.6/tests/media/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/navigation/test_models.py` & `djangocms-frontend-1.1.6/tests/navigation/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/navigation/test_plugins.py` & `djangocms-frontend-1.1.6/tests/navigation/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/tabs/test_models.py` & `djangocms-frontend-1.1.6/tests/tabs/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/tabs/test_plugins.py` & `djangocms-frontend-1.1.6/tests/tabs/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/test_constants.py` & `djangocms-frontend-1.1.6/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/test_fields.py` & `djangocms-frontend-1.1.6/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/test_helpers.py` & `djangocms-frontend-1.1.6/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/test_migrations.py` & `djangocms-frontend-1.1.6/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/test_settings.py` & `djangocms-frontend-1.1.6/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/utilities/test_models.py` & `djangocms-frontend-1.1.6/tests/utilities/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.5/tests/utilities/test_plugins.py` & `djangocms-frontend-1.1.6/tests/utilities/test_plugins.py`

 * *Files identical despite different names*

