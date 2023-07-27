# Comparing `tmp/nuclia-1.1.5.tar.gz` & `tmp/nuclia-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclia-1.1.5.tar", last modified: Wed Jul 26 11:51:07 2023, max compression
+gzip compressed data, was "nuclia-1.1.6.tar", last modified: Thu Jul 27 18:21:12 2023, max compression
```

## Comparing `nuclia-1.1.5.tar` & `nuclia-1.1.6.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.515290 nuclia-1.1.5/
--rw-r--r--   0 ebr        (501) staff       (20)       43 2023-07-26 11:51:06.000000 nuclia-1.1.5/.gitignore
--rw-r--r--   0 ebr        (501) staff       (20)       10 2023-07-26 11:51:06.000000 nuclia-1.1.5/.python-version
--rw-r--r--   0 ebr        (501) staff       (20)     1002 2023-07-26 11:51:06.000000 nuclia-1.1.5/CHANGELOG.md
--rw-r--r--   0 ebr        (501) staff       (20)     1063 2023-07-26 11:51:06.000000 nuclia-1.1.5/LICENSE
--rw-r--r--   0 ebr        (501) staff       (20)       83 2023-07-26 11:51:06.000000 nuclia-1.1.5/MANIFEST.in
--rw-r--r--   0 ebr        (501) staff       (20)      236 2023-07-26 11:51:06.000000 nuclia-1.1.5/Makefile
--rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-26 11:51:07.515452 nuclia-1.1.5/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)      955 2023-07-26 11:51:06.000000 nuclia-1.1.5/README.md
--rw-r--r--   0 ebr        (501) staff       (20)        6 2023-07-26 11:51:06.000000 nuclia-1.1.5/VERSION
--rw-r--r--   0 ebr        (501) staff       (20)       24 2023-07-26 11:51:06.000000 nuclia-1.1.5/code-requirements.txt
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.501650 nuclia-1.1.5/docs/
--rw-r--r--   0 ebr        (501) staff       (20)      941 2023-07-26 11:51:06.000000 nuclia-1.1.5/docs/AUTH.md
--rw-r--r--   0 ebr        (501) staff       (20)     1225 2023-07-26 11:51:06.000000 nuclia-1.1.5/docs/CONVERSATION.md
--rw-r--r--   0 ebr        (501) staff       (20)      892 2023-07-26 11:51:06.000000 nuclia-1.1.5/docs/DEFAULT.md
--rw-r--r--   0 ebr        (501) staff       (20)     1106 2023-07-26 11:51:06.000000 nuclia-1.1.5/docs/EXTRACT.md
--rw-r--r--   0 ebr        (501) staff       (20)      715 2023-07-26 11:51:06.000000 nuclia-1.1.5/docs/README.md
--rw-r--r--   0 ebr        (501) staff       (20)     1277 2023-07-26 11:51:06.000000 nuclia-1.1.5/docs/SEARCH.md
--rw-r--r--   0 ebr        (501) staff       (20)     2202 2023-07-26 11:51:06.000000 nuclia-1.1.5/docs/UPLOAD.md
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.503769 nuclia-1.1.5/nuclia/
--rw-r--r--   0 ebr        (501) staff       (20)      339 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.506920 nuclia-1.1.5/nuclia/cli/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/cli/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)     1353 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/cli/run.py
--rw-r--r--   0 ebr        (501) staff       (20)     1223 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/cli/utils.py
--rw-r--r--   0 ebr        (501) staff       (20)     6734 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/config.py
--rw-r--r--   0 ebr        (501) staff       (20)      739 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/data.py
--rw-r--r--   0 ebr        (501) staff       (20)     3473 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/decorators.py
--rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/exceptions.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.508817 nuclia-1.1.5/nuclia/lib/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/lib/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      153 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/lib/conversations.py
--rw-r--r--   0 ebr        (501) staff       (20)     5507 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/lib/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)      868 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/lib/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)      123 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/lib/nua_responses.py
--rw-r--r--   0 ebr        (501) staff       (20)      472 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/lib/utils.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.513106 nuclia-1.1.5/nuclia/sdk/
--rw-r--r--   0 ebr        (501) staff       (20)      388 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      647 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/accounts.py
--rw-r--r--   0 ebr        (501) staff       (20)     8210 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/auth.py
--rw-r--r--   0 ebr        (501) staff       (20)     2091 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)     3223 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/kbs.py
--rw-r--r--   0 ebr        (501) staff       (20)       57 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/logger.py
--rw-r--r--   0 ebr        (501) staff       (20)      311 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)     1092 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/nuas.py
--rw-r--r--   0 ebr        (501) staff       (20)      469 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/predict.py
--rw-r--r--   0 ebr        (501) staff       (20)      190 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/process.py
--rw-r--r--   0 ebr        (501) staff       (20)     3570 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/resource.py
--rw-r--r--   0 ebr        (501) staff       (20)     2974 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/search.py
--rw-r--r--   0 ebr        (501) staff       (20)      188 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/train.py
--rw-r--r--   0 ebr        (501) staff       (20)     9248 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/upload.py
--rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/zones.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.514796 nuclia-1.1.5/nuclia/tests/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.515042 nuclia-1.1.5/nuclia/tests/assets/
--rw-r--r--   0 ebr        (501) staff       (20)      348 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/assets/conversation.json
--rw-r--r--   0 ebr        (501) staff       (20)       50 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/conftest.py
--rw-r--r--   0 ebr        (501) staff       (20)     1200 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/fixtures.py
--rw-r--r--   0 ebr        (501) staff       (20)      492 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/test_auth.py
--rw-r--r--   0 ebr        (501) staff       (20)      738 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/test_conversation.py
--rw-r--r--   0 ebr        (501) staff       (20)      247 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/test_predict.py
--rw-r--r--   0 ebr        (501) staff       (20)      894 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/test_resource.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.506113 nuclia-1.1.5/nuclia.egg-info/
--rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-26 11:51:07.000000 nuclia-1.1.5/nuclia.egg-info/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)     1311 2023-07-26 11:51:07.000000 nuclia-1.1.5/nuclia.egg-info/SOURCES.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-26 11:51:07.000000 nuclia-1.1.5/nuclia.egg-info/dependency_links.txt
--rw-r--r--   0 ebr        (501) staff       (20)       47 2023-07-26 11:51:07.000000 nuclia-1.1.5/nuclia.egg-info/entry_points.txt
--rw-r--r--   0 ebr        (501) staff       (20)      105 2023-07-26 11:51:07.000000 nuclia-1.1.5/nuclia.egg-info/requires.txt
--rw-r--r--   0 ebr        (501) staff       (20)        7 2023-07-26 11:51:07.000000 nuclia-1.1.5/nuclia.egg-info/top_level.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-26 11:51:07.000000 nuclia-1.1.5/nuclia.egg-info/zip-safe
--rw-r--r--   0 ebr        (501) staff       (20)      104 2023-07-26 11:51:06.000000 nuclia-1.1.5/requirements.txt
--rw-r--r--   0 ebr        (501) staff       (20)      204 2023-07-26 11:51:07.515964 nuclia-1.1.5/setup.cfg
--rw-r--r--   0 ebr        (501) staff       (20)     1946 2023-07-26 11:51:06.000000 nuclia-1.1.5/setup.py
--rw-r--r--   0 ebr        (501) staff       (20)       45 2023-07-26 11:51:06.000000 nuclia-1.1.5/test-requirements.txt
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-07-27 18:21:12.946040 nuclia-1.1.6/
+-rw-r--r--   0 ramon      (501) staff       (20)       43 2023-07-27 18:21:12.000000 nuclia-1.1.6/.gitignore
+-rw-r--r--   0 ramon      (501) staff       (20)       10 2023-07-27 18:21:12.000000 nuclia-1.1.6/.python-version
+-rw-r--r--   0 ramon      (501) staff       (20)     1065 2023-07-27 18:21:12.000000 nuclia-1.1.6/CHANGELOG.md
+-rw-r--r--   0 ramon      (501) staff       (20)     1063 2023-07-27 18:21:12.000000 nuclia-1.1.6/LICENSE
+-rw-r--r--   0 ramon      (501) staff       (20)       83 2023-07-27 18:21:12.000000 nuclia-1.1.6/MANIFEST.in
+-rw-r--r--   0 ramon      (501) staff       (20)      236 2023-07-27 18:21:12.000000 nuclia-1.1.6/Makefile
+-rw-r--r--   0 ramon      (501) staff       (20)     1740 2023-07-27 18:21:12.946113 nuclia-1.1.6/PKG-INFO
+-rw-r--r--   0 ramon      (501) staff       (20)      955 2023-07-27 18:21:12.000000 nuclia-1.1.6/README.md
+-rw-r--r--   0 ramon      (501) staff       (20)        6 2023-07-27 18:21:12.000000 nuclia-1.1.6/VERSION
+-rw-r--r--   0 ramon      (501) staff       (20)       24 2023-07-27 18:21:12.000000 nuclia-1.1.6/code-requirements.txt
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-07-27 18:21:12.938055 nuclia-1.1.6/docs/
+-rw-r--r--   0 ramon      (501) staff       (20)      941 2023-07-27 18:21:12.000000 nuclia-1.1.6/docs/AUTH.md
+-rw-r--r--   0 ramon      (501) staff       (20)     1225 2023-07-27 18:21:12.000000 nuclia-1.1.6/docs/CONVERSATION.md
+-rw-r--r--   0 ramon      (501) staff       (20)      892 2023-07-27 18:21:12.000000 nuclia-1.1.6/docs/DEFAULT.md
+-rw-r--r--   0 ramon      (501) staff       (20)     1106 2023-07-27 18:21:12.000000 nuclia-1.1.6/docs/EXTRACT.md
+-rw-r--r--   0 ramon      (501) staff       (20)      715 2023-07-27 18:21:12.000000 nuclia-1.1.6/docs/README.md
+-rw-r--r--   0 ramon      (501) staff       (20)     1277 2023-07-27 18:21:12.000000 nuclia-1.1.6/docs/SEARCH.md
+-rw-r--r--   0 ramon      (501) staff       (20)     2202 2023-07-27 18:21:12.000000 nuclia-1.1.6/docs/UPLOAD.md
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-07-27 18:21:12.938887 nuclia-1.1.6/nuclia/
+-rw-r--r--   0 ramon      (501) staff       (20)      339 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/__init__.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-07-27 18:21:12.940801 nuclia-1.1.6/nuclia/cli/
+-rw-r--r--   0 ramon      (501) staff       (20)        0 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/cli/__init__.py
+-rw-r--r--   0 ramon      (501) staff       (20)     1353 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/cli/run.py
+-rw-r--r--   0 ramon      (501) staff       (20)     1223 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/cli/utils.py
+-rw-r--r--   0 ramon      (501) staff       (20)     6734 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/config.py
+-rw-r--r--   0 ramon      (501) staff       (20)      739 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/data.py
+-rw-r--r--   0 ramon      (501) staff       (20)     3473 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/decorators.py
+-rw-r--r--   0 ramon      (501) staff       (20)      223 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/exceptions.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-07-27 18:21:12.941836 nuclia-1.1.6/nuclia/lib/
+-rw-r--r--   0 ramon      (501) staff       (20)        0 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/lib/__init__.py
+-rw-r--r--   0 ramon      (501) staff       (20)      153 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/lib/conversations.py
+-rw-r--r--   0 ramon      (501) staff       (20)     5507 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/lib/kb.py
+-rw-r--r--   0 ramon      (501) staff       (20)      868 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/lib/nua.py
+-rw-r--r--   0 ramon      (501) staff       (20)      123 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/lib/nua_responses.py
+-rw-r--r--   0 ramon      (501) staff       (20)      472 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/lib/utils.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-07-27 18:21:12.944397 nuclia-1.1.6/nuclia/sdk/
+-rw-r--r--   0 ramon      (501) staff       (20)      388 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/sdk/__init__.py
+-rw-r--r--   0 ramon      (501) staff       (20)      647 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/sdk/accounts.py
+-rw-r--r--   0 ramon      (501) staff       (20)     8420 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/sdk/auth.py
+-rw-r--r--   0 ramon      (501) staff       (20)     4698 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/sdk/kb.py
+-rw-r--r--   0 ramon      (501) staff       (20)     3209 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/sdk/kbs.py
+-rw-r--r--   0 ramon      (501) staff       (20)       57 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/sdk/logger.py
+-rw-r--r--   0 ramon      (501) staff       (20)      287 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/sdk/nua.py
+-rw-r--r--   0 ramon      (501) staff       (20)     1092 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/sdk/nuas.py
+-rw-r--r--   0 ramon      (501) staff       (20)      469 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/sdk/predict.py
+-rw-r--r--   0 ramon      (501) staff       (20)      190 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/sdk/process.py
+-rw-r--r--   0 ramon      (501) staff       (20)     3570 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/sdk/resource.py
+-rw-r--r--   0 ramon      (501) staff       (20)     2974 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/sdk/search.py
+-rw-r--r--   0 ramon      (501) staff       (20)      188 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/sdk/train.py
+-rw-r--r--   0 ramon      (501) staff       (20)     9248 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/sdk/upload.py
+-rw-r--r--   0 ramon      (501) staff       (20)      223 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/sdk/zones.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-07-27 18:21:12.945707 nuclia-1.1.6/nuclia/tests/
+-rw-r--r--   0 ramon      (501) staff       (20)        0 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/tests/__init__.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-07-27 18:21:12.945877 nuclia-1.1.6/nuclia/tests/assets/
+-rw-r--r--   0 ramon      (501) staff       (20)      348 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/tests/assets/conversation.json
+-rw-r--r--   0 ramon      (501) staff       (20)       50 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/tests/conftest.py
+-rw-r--r--   0 ramon      (501) staff       (20)     1200 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/tests/fixtures.py
+-rw-r--r--   0 ramon      (501) staff       (20)      492 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/tests/test_auth.py
+-rw-r--r--   0 ramon      (501) staff       (20)      738 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/tests/test_conversation.py
+-rw-r--r--   0 ramon      (501) staff       (20)      879 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/tests/test_labels.py
+-rw-r--r--   0 ramon      (501) staff       (20)      247 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/tests/test_predict.py
+-rw-r--r--   0 ramon      (501) staff       (20)      894 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia/tests/test_resource.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-07-27 18:21:12.940265 nuclia-1.1.6/nuclia.egg-info/
+-rw-r--r--   0 ramon      (501) staff       (20)     1740 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia.egg-info/PKG-INFO
+-rw-r--r--   0 ramon      (501) staff       (20)     1339 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia.egg-info/SOURCES.txt
+-rw-r--r--   0 ramon      (501) staff       (20)        1 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia.egg-info/dependency_links.txt
+-rw-r--r--   0 ramon      (501) staff       (20)       47 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia.egg-info/entry_points.txt
+-rw-r--r--   0 ramon      (501) staff       (20)      105 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia.egg-info/requires.txt
+-rw-r--r--   0 ramon      (501) staff       (20)        7 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia.egg-info/top_level.txt
+-rw-r--r--   0 ramon      (501) staff       (20)        1 2023-07-27 18:21:12.000000 nuclia-1.1.6/nuclia.egg-info/zip-safe
+-rw-r--r--   0 ramon      (501) staff       (20)      104 2023-07-27 18:21:12.000000 nuclia-1.1.6/requirements.txt
+-rw-r--r--   0 ramon      (501) staff       (20)      204 2023-07-27 18:21:12.946527 nuclia-1.1.6/setup.cfg
+-rw-r--r--   0 ramon      (501) staff       (20)     1946 2023-07-27 18:21:12.000000 nuclia-1.1.6/setup.py
+-rw-r--r--   0 ramon      (501) staff       (20)       45 2023-07-27 18:21:12.000000 nuclia-1.1.6/test-requirements.txt
```

### Comparing `nuclia-1.1.5/CHANGELOG.md` & `nuclia-1.1.6/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## 1.1.6 (2023-07-27)
+
+
+- Adding labels and labelset support
+
+
 ## 1.1.5 (2023-07-26)
 
 - Support summary as resource attribute
 - Allow to create kb
 - Allow to set default account
 
 ## 1.1.4 (2023-07-21)
```

### Comparing `nuclia-1.1.5/LICENSE` & `nuclia-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/PKG-INFO` & `nuclia-1.1.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.1.5
+Version: 1.1.6
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
-Description: # Nuclia Python Client
-        
-        In order to install
-        
-        ```bash
-        pip install nuclia
-        ```
-        
-        ## Authentication
-        
-        ### Nuclia
-        
-        You can login with your Nuclia user [How to sign-up](https://nuclia.cloud/user/signup) via
-        
-        ```bash
-        nuclia auth login
-        ```
-        
-        
-        ### Nuclia Knowledgebox
-        
-        You can login to a specific knowledgebox if you have a Service Token (How to get a Service Token) or your NucliaDB is [deployed on-premise](https://docs.nuclia.dev/docs/nucliadb/deploy)
-        
-        ```bash
-        nuclia auth kb --url KB_URL --token SERVICE_TOKEN
-        ```
-        
-        KB_URL its the url of the Knowledge Box. On the cloud service you can retrieve it on the dashboard. On the on-premise/community deployment its the url mapped to it.
-        
-        
-        ### Nuclia Understanding API
-        
-        You can login with a Nuclia Understanding API key to process files, predict and train using our system
-        
-        ```bash
-        nuclia auth nua --key ZZZZ
-        ```
-        
-        ## Documentation
-        
-        You can find the documentation [here](https://github.com/nuclia/nuclia.py/tree/main/docs)
 Keywords: search,semantic,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Nuclia Python Client
+
+In order to install
+
+```bash
+pip install nuclia
+```
+
+## Authentication
+
+### Nuclia
+
+You can login with your Nuclia user [How to sign-up](https://nuclia.cloud/user/signup) via
+
+```bash
+nuclia auth login
+```
+
+
+### Nuclia Knowledgebox
+
+You can login to a specific knowledgebox if you have a Service Token (How to get a Service Token) or your NucliaDB is [deployed on-premise](https://docs.nuclia.dev/docs/nucliadb/deploy)
+
+```bash
+nuclia auth kb --url KB_URL --token SERVICE_TOKEN
+```
+
+KB_URL its the url of the Knowledge Box. On the cloud service you can retrieve it on the dashboard. On the on-premise/community deployment its the url mapped to it.
+
+
+### Nuclia Understanding API
+
+You can login with a Nuclia Understanding API key to process files, predict and train using our system
+
+```bash
+nuclia auth nua --key ZZZZ
+```
+
+## Documentation
+
+You can find the documentation [here](https://github.com/nuclia/nuclia.py/tree/main/docs)
+
```

### Comparing `nuclia-1.1.5/README.md` & `nuclia-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/docs/AUTH.md` & `nuclia-1.1.6/docs/AUTH.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/docs/CONVERSATION.md` & `nuclia-1.1.6/docs/CONVERSATION.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/docs/DEFAULT.md` & `nuclia-1.1.6/docs/DEFAULT.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/docs/EXTRACT.md` & `nuclia-1.1.6/docs/EXTRACT.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/docs/README.md` & `nuclia-1.1.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/docs/SEARCH.md` & `nuclia-1.1.6/docs/SEARCH.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/docs/UPLOAD.md` & `nuclia-1.1.6/docs/UPLOAD.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia/cli/run.py` & `nuclia-1.1.6/nuclia/cli/run.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia/cli/utils.py` & `nuclia-1.1.6/nuclia/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia/config.py` & `nuclia-1.1.6/nuclia/config.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia/data.py` & `nuclia-1.1.6/nuclia/data.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia/decorators.py` & `nuclia-1.1.6/nuclia/decorators.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia/lib/kb.py` & `nuclia-1.1.6/nuclia/lib/kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia/lib/nua.py` & `nuclia-1.1.6/nuclia/lib/nua.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia/sdk/accounts.py` & `nuclia-1.1.6/nuclia/sdk/accounts.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia/sdk/auth.py` & `nuclia-1.1.6/nuclia/sdk/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -187,34 +187,41 @@
         else:
             return False
 
     def post_login(self):
         self.accounts()
         self.zones()
 
-    def _request(self, method: str, path: str, data: Optional[Any] = None):
+    def _request(
+        self, method: str, path: str, data: Optional[Any] = None, remove_null=True
+    ):
         if not self._config.token:
             raise NeedUserToken()
-        kwargs = {"headers": {"Authorization": f"Bearer {self._config.token}"}}
+        kwargs: Dict[str, Any] = {
+            "headers": {"Authorization": f"Bearer {self._config.token}"}
+        }
         if data is not None:
-            non_null_values = {k: v for k, v in data.items() if v is not None}
-            kwargs["data"] = json.dumps(non_null_values)
+            if remove_null:
+                data = {k: v for k, v in data.items() if v is not None}
+            kwargs["data"] = json.dumps(data)
         resp = requests.request(
             method,
             path,
             **kwargs,
         )
         if resp.status_code == 204:
             return None
         elif resp.status_code >= 200 and resp.status_code < 300:
             return resp.json()
+        elif resp.status_code >= 300 and resp.status_code < 400:
+            return None
         elif resp.status_code == 403:
             raise UserTokenExpired()
         else:
-            raise Exception(resp.text)
+            raise Exception({"status": resp.status_code, "message": resp.text})
 
     def accounts(self) -> List[Account]:
         accounts = self._request("GET", ACCOUNTS)
         result = []
         self._config.accounts = []
         for account in accounts:
             account_obj = Account.parse_obj(account)
```

### Comparing `nuclia-1.1.5/nuclia/sdk/kbs.py` & `nuclia-1.1.6/nuclia/sdk/kbs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Optional
 
 from nuclia import BASE
-from nuclia.config import KnowledgeBox, retrieve
+from nuclia.config import retrieve
 from nuclia.data import get_auth
 from nuclia.decorators import account, accounts
 from nuclia.sdk.auth import NucliaAuth
 
 KBS_ENDPOINT = BASE + "/api/v1/account/{account}/kbs"
 KB_ENDPOINT = BASE + "/api/v1/account/{account}/kb/{slug}"
```

### Comparing `nuclia-1.1.5/nuclia/sdk/nuas.py` & `nuclia-1.1.6/nuclia/sdk/nuas.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia/sdk/resource.py` & `nuclia-1.1.6/nuclia/sdk/resource.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia/sdk/search.py` & `nuclia-1.1.6/nuclia/sdk/search.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia/sdk/upload.py` & `nuclia-1.1.6/nuclia/sdk/upload.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia/tests/fixtures.py` & `nuclia-1.1.6/nuclia/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia/tests/test_conversation.py` & `nuclia-1.1.6/nuclia/tests/test_conversation.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia/tests/test_resource.py` & `nuclia-1.1.6/nuclia/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.5/nuclia.egg-info/PKG-INFO` & `nuclia-1.1.6/nuclia.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.1.5
+Version: 1.1.6
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
-Description: # Nuclia Python Client
-        
-        In order to install
-        
-        ```bash
-        pip install nuclia
-        ```
-        
-        ## Authentication
-        
-        ### Nuclia
-        
-        You can login with your Nuclia user [How to sign-up](https://nuclia.cloud/user/signup) via
-        
-        ```bash
-        nuclia auth login
-        ```
-        
-        
-        ### Nuclia Knowledgebox
-        
-        You can login to a specific knowledgebox if you have a Service Token (How to get a Service Token) or your NucliaDB is [deployed on-premise](https://docs.nuclia.dev/docs/nucliadb/deploy)
-        
-        ```bash
-        nuclia auth kb --url KB_URL --token SERVICE_TOKEN
-        ```
-        
-        KB_URL its the url of the Knowledge Box. On the cloud service you can retrieve it on the dashboard. On the on-premise/community deployment its the url mapped to it.
-        
-        
-        ### Nuclia Understanding API
-        
-        You can login with a Nuclia Understanding API key to process files, predict and train using our system
-        
-        ```bash
-        nuclia auth nua --key ZZZZ
-        ```
-        
-        ## Documentation
-        
-        You can find the documentation [here](https://github.com/nuclia/nuclia.py/tree/main/docs)
 Keywords: search,semantic,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Nuclia Python Client
+
+In order to install
+
+```bash
+pip install nuclia
+```
+
+## Authentication
+
+### Nuclia
+
+You can login with your Nuclia user [How to sign-up](https://nuclia.cloud/user/signup) via
+
+```bash
+nuclia auth login
+```
+
+
+### Nuclia Knowledgebox
+
+You can login to a specific knowledgebox if you have a Service Token (How to get a Service Token) or your NucliaDB is [deployed on-premise](https://docs.nuclia.dev/docs/nucliadb/deploy)
+
+```bash
+nuclia auth kb --url KB_URL --token SERVICE_TOKEN
+```
+
+KB_URL its the url of the Knowledge Box. On the cloud service you can retrieve it on the dashboard. On the on-premise/community deployment its the url mapped to it.
+
+
+### Nuclia Understanding API
+
+You can login with a Nuclia Understanding API key to process files, predict and train using our system
+
+```bash
+nuclia auth nua --key ZZZZ
+```
+
+## Documentation
+
+You can find the documentation [here](https://github.com/nuclia/nuclia.py/tree/main/docs)
+
```

### Comparing `nuclia-1.1.5/nuclia.egg-info/SOURCES.txt` & `nuclia-1.1.6/nuclia.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -55,10 +55,11 @@
 nuclia/sdk/upload.py
 nuclia/sdk/zones.py
 nuclia/tests/__init__.py
 nuclia/tests/conftest.py
 nuclia/tests/fixtures.py
 nuclia/tests/test_auth.py
 nuclia/tests/test_conversation.py
+nuclia/tests/test_labels.py
 nuclia/tests/test_predict.py
 nuclia/tests/test_resource.py
 nuclia/tests/assets/conversation.json
```

### Comparing `nuclia-1.1.5/setup.py` & `nuclia-1.1.6/setup.py`

 * *Files identical despite different names*

