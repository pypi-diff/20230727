# Comparing `tmp/sweetrpg-catalog-objects-0.0.6.tar.gz` & `tmp/sweetrpg-catalog-objects-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweetrpg-catalog-objects-0.0.6.tar", last modified: Thu Jul 27 15:20:12 2023, max compression
+gzip compressed data, was "sweetrpg-catalog-objects-0.0.7.tar", last modified: Thu Jul 27 15:23:55 2023, max compression
```

## Comparing `sweetrpg-catalog-objects-0.0.6.tar` & `sweetrpg-catalog-objects-0.0.7.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.076628 sweetrpg-catalog-objects-0.0.6/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      663 2023-07-27 15:20:12.076628 sweetrpg-catalog-objects-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/README.md
--rw-r--r--   0 root         (0) root         (0)      188 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)     1199 2023-07-27 15:20:12.076628 sweetrpg-catalog-objects-0.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.064627 sweetrpg-catalog-objects-0.0.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.064627 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/
--rwxr-xr-x   0 root         (0) root         (0)      381 2023-07-27 15:20:07.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.068628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/
--rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.068628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/contribution/
--rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/contribution/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1069 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/contribution/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.068628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/license/
--rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/license/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      984 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/license/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.068628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/person/
--rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/person/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1045 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/person/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.068628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/publisher/
--rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/publisher/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      796 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/publisher/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.068628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/review/
--rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/review/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1081 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/review/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.068628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/studio/
--rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/studio/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      775 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/studio/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.068628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/system/
--rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/system/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      745 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/system/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.068628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/volume/
--rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/volume/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1221 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/volume/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.068628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/
--rwxr-xr-x   0 root         (0) root         (0)       99 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.068628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/contribution/
--rwxr-xr-x   0 root         (0) root         (0)      116 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/contribution/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1323 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/contribution/document.py
--rwxr-xr-x   0 root         (0) root         (0)      474 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/contribution/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.068628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/embedded/
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/embedded/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.068628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/embedded/property/
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/embedded/property/__init__.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/embedded/property/document.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/embedded/property/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.072628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/embedded/tag/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/embedded/tag/__init__.py
--rw-r--r--   0 root         (0) root         (0)      412 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/embedded/tag/document.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/embedded/tag/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.072628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/license/
--rwxr-xr-x   0 root         (0) root         (0)      117 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/license/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1486 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/license/document.py
--rwxr-xr-x   0 root         (0) root         (0)      756 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/license/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.072628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/person/
--rwxr-xr-x   0 root         (0) root         (0)      116 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/person/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1312 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/person/document.py
--rwxr-xr-x   0 root         (0) root         (0)      542 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/person/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.072628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/publisher/
--rwxr-xr-x   0 root         (0) root         (0)      119 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/publisher/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1211 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/publisher/document.py
--rwxr-xr-x   0 root         (0) root         (0)      554 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/publisher/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.072628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/review/
--rwxr-xr-x   0 root         (0) root         (0)      116 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/review/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1325 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/review/document.py
--rwxr-xr-x   0 root         (0) root         (0)      598 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/review/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.072628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/studio/
--rwxr-xr-x   0 root         (0) root         (0)      116 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/studio/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1357 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/studio/document.py
--rwxr-xr-x   0 root         (0) root         (0)      542 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/studio/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.072628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/system/
--rwxr-xr-x   0 root         (0) root         (0)      121 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/system/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1258 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/system/document.py
--rwxr-xr-x   0 root         (0) root         (0)      512 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/system/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.072628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/volume/
--rwxr-xr-x   0 root         (0) root         (0)      117 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/volume/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1661 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/volume/document.py
--rwxr-xr-x   0 root         (0) root         (0)      896 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/volume/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.076628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/
--rwxr-xr-x   0 root         (0) root         (0)       95 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      780 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/contribution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.076628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/embedded/
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/embedded/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      533 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/embedded/property.py
--rwxr-xr-x   0 root         (0) root         (0)      621 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/embedded/tag.py
--rwxr-xr-x   0 root         (0) root         (0)      688 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/license.py
--rwxr-xr-x   0 root         (0) root         (0)      638 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/person.py
--rwxr-xr-x   0 root         (0) root         (0)      607 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/publisher.py
--rwxr-xr-x   0 root         (0) root         (0)      871 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/review.py
--rwxr-xr-x   0 root         (0) root         (0)      595 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/studio.py
--rwxr-xr-x   0 root         (0) root         (0)      610 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/system.py
--rwxr-xr-x   0 root         (0) root         (0)      826 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/volume.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.076628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/utils/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/utils/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     3078 2023-07-27 15:20:06.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/utils/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:20:12.068628 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects.egg-info/
--rw-r--r--   0 root         (0) root         (0)      663 2023-07-27 15:20:12.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3645 2023-07-27 15:20:12.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 15:20:12.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-27 15:20:12.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-07-27 15:20:12.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-27 15:20:12.000000 sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.499094 sweetrpg-catalog-objects-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      663 2023-07-27 15:23:55.499094 sweetrpg-catalog-objects-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      188 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)     1199 2023-07-27 15:23:55.499094 sweetrpg-catalog-objects-0.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.483094 sweetrpg-catalog-objects-0.0.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.487094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/
+-rwxr-xr-x   0 root         (0) root         (0)      381 2023-07-27 15:23:53.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.491094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.491094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/contribution/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/contribution/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1069 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/contribution/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.491094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/license/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/license/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      984 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/license/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.491094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/person/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/person/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1045 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/person/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.491094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/publisher/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/publisher/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      796 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/publisher/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.491094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/review/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/review/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1081 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/review/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.491094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/studio/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/studio/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      775 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/studio/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.491094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/system/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/system/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      745 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/system/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.491094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/volume/
+-rwxr-xr-x   0 root         (0) root         (0)       81 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/volume/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1221 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/volume/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.491094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/
+-rwxr-xr-x   0 root         (0) root         (0)       99 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.491094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/contribution/
+-rwxr-xr-x   0 root         (0) root         (0)      116 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/contribution/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1323 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/contribution/document.py
+-rwxr-xr-x   0 root         (0) root         (0)      474 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/contribution/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.491094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/embedded/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/embedded/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.495094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/embedded/property/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/embedded/property/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/embedded/property/document.py
+-rw-r--r--   0 root         (0) root         (0)      510 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/embedded/property/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.495094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/embedded/tag/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/embedded/tag/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      412 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/embedded/tag/document.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/embedded/tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.495094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/license/
+-rwxr-xr-x   0 root         (0) root         (0)      117 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/license/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1486 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/license/document.py
+-rwxr-xr-x   0 root         (0) root         (0)      756 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/license/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.495094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/person/
+-rwxr-xr-x   0 root         (0) root         (0)      116 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/person/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1312 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/person/document.py
+-rwxr-xr-x   0 root         (0) root         (0)      542 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/person/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.495094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/publisher/
+-rwxr-xr-x   0 root         (0) root         (0)      119 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/publisher/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1211 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/publisher/document.py
+-rwxr-xr-x   0 root         (0) root         (0)      554 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/publisher/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.495094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/review/
+-rwxr-xr-x   0 root         (0) root         (0)      116 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/review/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1325 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/review/document.py
+-rwxr-xr-x   0 root         (0) root         (0)      598 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/review/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.495094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/studio/
+-rwxr-xr-x   0 root         (0) root         (0)      116 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/studio/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1357 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/studio/document.py
+-rwxr-xr-x   0 root         (0) root         (0)      542 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/studio/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.495094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/system/
+-rwxr-xr-x   0 root         (0) root         (0)      121 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/system/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1258 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/system/document.py
+-rwxr-xr-x   0 root         (0) root         (0)      512 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/system/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.499094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/volume/
+-rwxr-xr-x   0 root         (0) root         (0)      117 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/volume/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1661 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/volume/document.py
+-rwxr-xr-x   0 root         (0) root         (0)      896 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/volume/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.499094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/
+-rwxr-xr-x   0 root         (0) root         (0)       95 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      780 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/contribution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.499094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/embedded/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/embedded/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      533 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/embedded/property.py
+-rwxr-xr-x   0 root         (0) root         (0)      621 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/embedded/tag.py
+-rwxr-xr-x   0 root         (0) root         (0)      688 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/license.py
+-rwxr-xr-x   0 root         (0) root         (0)      638 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/person.py
+-rwxr-xr-x   0 root         (0) root         (0)      607 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/publisher.py
+-rwxr-xr-x   0 root         (0) root         (0)      871 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/review.py
+-rwxr-xr-x   0 root         (0) root         (0)      595 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/studio.py
+-rwxr-xr-x   0 root         (0) root         (0)      610 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/system.py
+-rwxr-xr-x   0 root         (0) root         (0)      826 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/volume.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.499094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/utils/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/utils/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3078 2023-07-27 15:23:52.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/utils/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:23:55.487094 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      663 2023-07-27 15:23:55.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3645 2023-07-27 15:23:55.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 15:23:55.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-27 15:23:55.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-07-27 15:23:55.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-27 15:23:55.000000 sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects.egg-info/top_level.txt
```

### Comparing `sweetrpg-catalog-objects-0.0.6/LICENSE` & `sweetrpg-catalog-objects-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/PKG-INFO` & `sweetrpg-catalog-objects-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweetrpg-catalog-objects
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://sweetrpg.com
 Author: Paul Schifferer
 Author-email: dm@sweetrpg.com
 License: MIT
 Project-URL: Documentation, https://sweetrpg.github.io/catalog-objects
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `sweetrpg-catalog-objects-0.0.6/setup.cfg` & `sweetrpg-catalog-objects-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/contribution/schema.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/contribution/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/license/schema.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/license/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/person/schema.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/person/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/publisher/schema.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/publisher/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/review/schema.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/review/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/studio/schema.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/studio/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/system/schema.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/system/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/api/volume/schema.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/api/volume/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/contribution/document.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/contribution/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/license/document.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/license/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/license/schema.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/license/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/person/document.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/person/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/person/schema.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/person/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/publisher/document.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/publisher/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/publisher/schema.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/publisher/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/review/document.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/review/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/review/schema.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/review/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/studio/document.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/studio/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/studio/schema.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/studio/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/system/document.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/system/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/system/schema.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/system/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/volume/document.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/volume/document.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/db/volume/schema.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/db/volume/schema.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/contribution.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/contribution.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/embedded/property.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/embedded/property.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/embedded/tag.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/embedded/tag.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/license.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/license.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/person.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/person.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/publisher.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/publisher.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/review.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/review.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/studio.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/studio.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/system.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/system.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/model/volume.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/model/volume.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects/utils/user.py` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects/utils/user.py`

 * *Files identical despite different names*

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects.egg-info/PKG-INFO` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweetrpg-catalog-objects
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://sweetrpg.com
 Author: Paul Schifferer
 Author-email: dm@sweetrpg.com
 License: MIT
 Project-URL: Documentation, https://sweetrpg.github.io/catalog-objects
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `sweetrpg-catalog-objects-0.0.6/src/sweetrpg_catalog_objects.egg-info/SOURCES.txt` & `sweetrpg-catalog-objects-0.0.7/src/sweetrpg_catalog_objects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

