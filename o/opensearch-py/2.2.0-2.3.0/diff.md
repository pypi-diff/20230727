# Comparing `tmp/opensearch-py-2.2.0.tar.gz` & `tmp/opensearch-py-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensearch-py-2.2.0.tar", last modified: Wed Mar  1 22:34:49 2023, max compression
+gzip compressed data, was "opensearch-py-2.3.0.tar", last modified: Thu Jul 27 19:07:42 2023, max compression
```

## Comparing `opensearch-py-2.2.0.tar` & `opensearch-py-2.3.0.tar`

### file list

```diff
@@ -1,167 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:34:49.516153 opensearch-py-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-03-01 22:34:49.516153 opensearch-py-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:34:49.492153 opensearch-py-2.2.0/opensearch_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-03-01 22:34:49.000000 opensearch-py-2.2.0/opensearch_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-03-01 22:34:49.000000 opensearch-py-2.2.0/opensearch_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 22:34:49.000000 opensearch-py-2.2.0/opensearch_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 22:34:49.000000 opensearch-py-2.2.0/opensearch_py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-01 22:34:49.000000 opensearch-py-2.2.0/opensearch_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-01 22:34:49.000000 opensearch-py-2.2.0/opensearch_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:34:49.492153 opensearch-py-2.2.0/opensearchpy/
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:34:49.496153 opensearch-py-2.2.0/opensearchpy/_async/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/_extra_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:34:49.496153 opensearch-py-2.2.0/opensearchpy/_async/client/
--rw-r--r--   0 runner    (1001) docker     (123)    85442 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46274 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29940 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/cat.py
--rw-r--r--   0 runner    (1001) docker     (123)    22836 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/cat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17123 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/cluster.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/dangling_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/dangling_indices.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/features.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    70997 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/indices.py
--rw-r--r--   0 runner    (1001) docker     (123)    53603 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/indices.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/ingest.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/plugins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/remote.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/snapshot.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/tasks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/client/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17645 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/helpers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/http_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/http_aiohttp.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:34:49.500153 opensearch-py-2.2.0/opensearchpy/_async/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/plugins/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/plugins/alerting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/plugins/alerting.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18066 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_async/transport.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:34:49.504153 opensearch-py-2.2.0/opensearchpy/client/
--rw-r--r--   0 runner    (1001) docker     (123)    84926 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45958 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29568 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/cat.py
--rw-r--r--   0 runner    (1001) docker     (123)    22704 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/cat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16943 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/cluster.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/dangling_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/dangling_indices.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/features.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    71619 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/indices.py
--rw-r--r--   0 runner    (1001) docker     (123)    53267 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/indices.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/ingest.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/plugins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/remote.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/snapshot.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/tasks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/client/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/compat.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:34:49.504153 opensearch-py-2.2.0/opensearchpy/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection/connections.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection/http_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection/http_async.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection/http_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection/http_requests.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection/http_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection/http_urllib3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection/pooling.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/connection_pool.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/exceptions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:34:49.512153 opensearch-py-2.2.0/opensearchpy/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24406 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/actions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/aggs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/aggs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/analysis.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/asyncsigner.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/asyncsigner.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/document.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13797 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/faceted_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/faceted_search.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14196 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/field.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/function.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/index.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/mapping.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12591 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:34:49.516153 opensearch-py-2.2.0/opensearchpy/helpers/response/
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/response/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/response/aggs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/response/aggs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/response/hit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/response/hit.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25586 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/search.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/test.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/update_by_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/update_by_query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19065 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/helpers/wrappers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:34:49.516153 opensearch-py-2.2.0/opensearchpy/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/plugins/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/plugins/alerting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/plugins/alerting.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18470 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/opensearchpy/transport.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-01 22:34:49.516153 opensearch-py-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-03-01 22:34:40.000000 opensearch-py-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:07:42.350440 opensearch-py-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-07-27 19:07:42.350440 opensearch-py-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:07:42.322440 opensearch-py-2.3.0/opensearch_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-07-27 19:07:42.000000 opensearch-py-2.3.0/opensearch_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-07-27 19:07:42.000000 opensearch-py-2.3.0/opensearch_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:07:42.000000 opensearch-py-2.3.0/opensearch_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:07:42.000000 opensearch-py-2.3.0/opensearch_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-27 19:07:42.000000 opensearch-py-2.3.0/opensearch_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-27 19:07:42.000000 opensearch-py-2.3.0/opensearch_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:07:42.326439 opensearch-py-2.3.0/opensearchpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:07:42.326439 opensearch-py-2.3.0/opensearchpy/_async/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/_extra_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:07:42.330440 opensearch-py-2.3.0/opensearchpy/_async/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    85525 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47084 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29940 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22836 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/cat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17123 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/cluster.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/dangling_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/dangling_indices.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    70997 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53603 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/indices.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/ingest.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/plugins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/remote.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23129 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/security.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/snapshot.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/tasks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/client/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:07:42.334440 opensearch-py-2.3.0/opensearchpy/_async/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17605 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/actions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16308 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/document.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/faceted_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/faceted_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23606 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/index.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/mapping.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17058 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/search.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/update_by_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/helpers/update_by_query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14193 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/http_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/http_aiohttp.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:07:42.334440 opensearch-py-2.3.0/opensearchpy/_async/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/plugins/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/plugins/alerting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/plugins/alerting.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/plugins/index_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/plugins/index_management.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18066 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_async/transport.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:07:42.338440 opensearch-py-2.3.0/opensearchpy/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    85008 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46762 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29568 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22704 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/cat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16943 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/cluster.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/dangling_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/dangling_indices.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    71619 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53267 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/indices.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/ingest.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/plugins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/remote.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22549 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/security.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/snapshot.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/tasks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/client/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:07:42.342440 opensearch-py-2.3.0/opensearchpy/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/async_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/async_connections.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/connections.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/http_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/http_async.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/http_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/http_requests.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/http_urllib3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/http_urllib3.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection/pooling.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/connection_pool.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/exceptions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:07:42.346440 opensearch-py-2.3.0/opensearchpy/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24406 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/actions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/aggs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/aggs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/analysis.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/asyncsigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/asyncsigner.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/document.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13797 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/faceted_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/faceted_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14196 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/field.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/function.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/index.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/mapping.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12591 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:07:42.346440 opensearch-py-2.3.0/opensearchpy/helpers/response/
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/response/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/response/aggs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/response/aggs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/response/hit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/response/hit.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26468 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/search.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/update_by_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/update_by_query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19065 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/helpers/wrappers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:07:42.350440 opensearch-py-2.3.0/opensearchpy/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/plugins/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/plugins/alerting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/plugins/alerting.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/plugins/index_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/plugins/index_management.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18470 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/opensearchpy/transport.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-27 19:07:42.350440 opensearch-py-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-27 17:18:30.000000 opensearch-py-2.3.0/setup.py
```

### Comparing `opensearch-py-2.2.0/CONTRIBUTING.md` & `opensearch-py-2.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/LICENSE.txt` & `opensearch-py-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/PKG-INFO` & `opensearch-py-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-py
-Version: 2.2.0
+Version: 2.3.0
 Summary: Python client for OpenSearch
 Home-page: https://github.com/opensearch-project/opensearch-py
 Author: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Author-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 Maintainer: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Maintainer-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 License: Apache-2.0
```

### Comparing `opensearch-py-2.2.0/README.md` & `opensearch-py-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearch_py.egg-info/PKG-INFO` & `opensearch-py-2.3.0/opensearch_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-py
-Version: 2.2.0
+Version: 2.3.0
 Summary: Python client for OpenSearch
 Home-page: https://github.com/opensearch-project/opensearch-py
 Author: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Author-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 Maintainer: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Maintainer-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 License: Apache-2.0
```

### Comparing `opensearch-py-2.2.0/opensearch_py.egg-info/SOURCES.txt` & `opensearch-py-2.3.0/opensearch_py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 opensearchpy/serializer.pyi
 opensearchpy/transport.py
 opensearchpy/transport.pyi
 opensearchpy/_async/__init__.py
 opensearchpy/_async/_extra_imports.py
 opensearchpy/_async/compat.py
 opensearchpy/_async/compat.pyi
-opensearchpy/_async/helpers.py
-opensearchpy/_async/helpers.pyi
 opensearchpy/_async/http_aiohttp.py
 opensearchpy/_async/http_aiohttp.pyi
 opensearchpy/_async/transport.py
 opensearchpy/_async/transport.pyi
 opensearchpy/_async/client/__init__.py
 opensearchpy/_async/client/__init__.pyi
 opensearchpy/_async/client/cat.py
@@ -52,24 +50,45 @@
 opensearchpy/_async/client/ingest.pyi
 opensearchpy/_async/client/nodes.py
 opensearchpy/_async/client/nodes.pyi
 opensearchpy/_async/client/plugins.py
 opensearchpy/_async/client/plugins.pyi
 opensearchpy/_async/client/remote.py
 opensearchpy/_async/client/remote.pyi
+opensearchpy/_async/client/security.py
+opensearchpy/_async/client/security.pyi
 opensearchpy/_async/client/snapshot.py
 opensearchpy/_async/client/snapshot.pyi
 opensearchpy/_async/client/tasks.py
 opensearchpy/_async/client/tasks.pyi
 opensearchpy/_async/client/utils.py
 opensearchpy/_async/client/utils.pyi
+opensearchpy/_async/helpers/__init__.py
+opensearchpy/_async/helpers/actions.py
+opensearchpy/_async/helpers/actions.pyi
+opensearchpy/_async/helpers/document.py
+opensearchpy/_async/helpers/document.pyi
+opensearchpy/_async/helpers/faceted_search.py
+opensearchpy/_async/helpers/faceted_search.pyi
+opensearchpy/_async/helpers/index.py
+opensearchpy/_async/helpers/index.pyi
+opensearchpy/_async/helpers/mapping.py
+opensearchpy/_async/helpers/mapping.pyi
+opensearchpy/_async/helpers/search.py
+opensearchpy/_async/helpers/search.pyi
+opensearchpy/_async/helpers/test.py
+opensearchpy/_async/helpers/test.pyi
+opensearchpy/_async/helpers/update_by_query.py
+opensearchpy/_async/helpers/update_by_query.pyi
 opensearchpy/_async/plugins/__init__.py
 opensearchpy/_async/plugins/__init__.pyi
 opensearchpy/_async/plugins/alerting.py
 opensearchpy/_async/plugins/alerting.pyi
+opensearchpy/_async/plugins/index_management.py
+opensearchpy/_async/plugins/index_management.pyi
 opensearchpy/client/__init__.py
 opensearchpy/client/__init__.pyi
 opensearchpy/client/cat.py
 opensearchpy/client/cat.pyi
 opensearchpy/client/cluster.py
 opensearchpy/client/cluster.pyi
 opensearchpy/client/dangling_indices.py
@@ -82,22 +101,26 @@
 opensearchpy/client/ingest.pyi
 opensearchpy/client/nodes.py
 opensearchpy/client/nodes.pyi
 opensearchpy/client/plugins.py
 opensearchpy/client/plugins.pyi
 opensearchpy/client/remote.py
 opensearchpy/client/remote.pyi
+opensearchpy/client/security.py
+opensearchpy/client/security.pyi
 opensearchpy/client/snapshot.py
 opensearchpy/client/snapshot.pyi
 opensearchpy/client/tasks.py
 opensearchpy/client/tasks.pyi
 opensearchpy/client/utils.py
 opensearchpy/client/utils.pyi
 opensearchpy/connection/__init__.py
 opensearchpy/connection/__init__.pyi
+opensearchpy/connection/async_connections.py
+opensearchpy/connection/async_connections.pyi
 opensearchpy/connection/base.py
 opensearchpy/connection/base.pyi
 opensearchpy/connection/connections.py
 opensearchpy/connection/connections.pyi
 opensearchpy/connection/http_async.py
 opensearchpy/connection/http_async.pyi
 opensearchpy/connection/http_requests.py
@@ -148,8 +171,10 @@
 opensearchpy/helpers/response/aggs.py
 opensearchpy/helpers/response/aggs.pyi
 opensearchpy/helpers/response/hit.py
 opensearchpy/helpers/response/hit.pyi
 opensearchpy/plugins/__init__.py
 opensearchpy/plugins/__init__.pyi
 opensearchpy/plugins/alerting.py
-opensearchpy/plugins/alerting.pyi
+opensearchpy/plugins/alerting.pyi
+opensearchpy/plugins/index_management.py
+opensearchpy/plugins/index_management.pyi
```

### Comparing `opensearch-py-2.2.0/opensearchpy/__init__.py` & `opensearch-py-2.3.0/opensearchpy/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/__init__.pyi` & `opensearch-py-2.3.0/opensearchpy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/__init__.py` & `opensearch-py-2.3.0/opensearchpy/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/_extra_imports.py` & `opensearch-py-2.3.0/opensearchpy/_async/_extra_imports.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/__init__.py` & `opensearch-py-2.3.0/opensearchpy/_async/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from .dangling_indices import DanglingIndicesClient
 from .features import FeaturesClient
 from .indices import IndicesClient
 from .ingest import IngestClient
 from .nodes import NodesClient
 from .plugins import PluginsClient
 from .remote import RemoteClient
+from .security import SecurityClient
 from .snapshot import SnapshotClient
 from .tasks import TasksClient
 from .utils import SKIP_IN_PATH, _bulk_body, _make_path, _normalize_hosts, query_params
 
 logger = logging.getLogger("opensearch")
 
 
@@ -192,20 +193,22 @@
         self.cat = CatClient(self)
         self.cluster = ClusterClient(self)
         self.dangling_indices = DanglingIndicesClient(self)
         self.indices = IndicesClient(self)
         self.ingest = IngestClient(self)
         self.nodes = NodesClient(self)
         self.remote = RemoteClient(self)
+        self.security = SecurityClient(self)
         self.snapshot = SnapshotClient(self)
         self.tasks = TasksClient(self)
-        self.plugins = PluginsClient(self)
 
         self.features = FeaturesClient(self)
 
+        self.plugins = PluginsClient(self)
+
     def __repr__(self):
         try:
             # get a list of all connections
             cons = self.transport.hosts
             # truncate to 5 if there are too many
             if len(cons) > 5:
                 cons = cons[:5] + ["..."]
```

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/__init__.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/client/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from .cluster import ClusterClient
 from .dangling_indices import DanglingIndicesClient
 from .features import FeaturesClient
 from .indices import IndicesClient
 from .ingest import IngestClient
 from .nodes import NodesClient
 from .remote import RemoteClient
+from .security import SecurityClient
 from .snapshot import SnapshotClient
 from .tasks import TasksClient
 
 logger: logging.Logger
 
 class AsyncOpenSearch(object):
     transport: AsyncTransport
@@ -50,14 +51,15 @@
     cat: CatClient
     cluster: ClusterClient
     features: FeaturesClient
     indices: IndicesClient
     ingest: IngestClient
     nodes: NodesClient
     remote: RemoteClient
+    security: SecurityClient
     snapshot: SnapshotClient
     tasks: TasksClient
     def __init__(
         self,
         hosts: Any = ...,
         transport_class: Type[AsyncTransport] = ...,
         **kwargs: Any,
@@ -1051,32 +1053,49 @@
         ignore: Optional[Union[int, Collection[int]]] = ...,
         opaque_id: Optional[str] = ...,
         http_auth: Optional[Union[str, Tuple[str, str]]] = ...,
         api_key: Optional[Union[str, Tuple[str, str]]] = ...,
         params: Optional[MutableMapping[str, Any]] = ...,
         headers: Optional[MutableMapping[str, str]] = ...,
     ) -> Any: ...
-    async def close_point_in_time(
+    async def list_all_point_in_time(
+        self,
+        *,
+        pretty: Optional[bool] = ...,
+        human: Optional[bool] = ...,
+        error_trace: Optional[bool] = ...,
+        format: Optional[str] = ...,
+        filter_path: Optional[Union[str, Collection[str]]] = ...,
+        request_timeout: Optional[Union[int, float]] = ...,
+        ignore: Optional[Union[int, Collection[int]]] = ...,
+        opaque_id: Optional[str] = ...,
+        http_auth: Optional[Union[str, Tuple[str, str]]] = ...,
+        api_key: Optional[Union[str, Tuple[str, str]]] = ...,
+        params: Optional[MutableMapping[str, Any]] = ...,
+        headers: Optional[MutableMapping[str, str]] = ...,
+    ) -> Any: ...
+    async def delete_point_in_time(
         self,
         *,
         body: Optional[Any] = ...,
+        all: Optional[bool] = ...,
         pretty: Optional[bool] = ...,
         human: Optional[bool] = ...,
         error_trace: Optional[bool] = ...,
         format: Optional[str] = ...,
         filter_path: Optional[Union[str, Collection[str]]] = ...,
         request_timeout: Optional[Union[int, float]] = ...,
         ignore: Optional[Union[int, Collection[int]]] = ...,
         opaque_id: Optional[str] = ...,
         http_auth: Optional[Union[str, Tuple[str, str]]] = ...,
         api_key: Optional[Union[str, Tuple[str, str]]] = ...,
         params: Optional[MutableMapping[str, Any]] = ...,
         headers: Optional[MutableMapping[str, str]] = ...,
     ) -> Any: ...
-    async def open_point_in_time(
+    async def create_point_in_time(
         self,
         *,
         index: Optional[Any] = ...,
         expand_wildcards: Optional[Any] = ...,
         ignore_unavailable: Optional[Any] = ...,
         keep_alive: Optional[Any] = ...,
         preference: Optional[Any] = ...,
```

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/cat.py` & `opensearch-py-2.3.0/opensearchpy/_async/client/cat.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/cat.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/client/cat.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/cluster.py` & `opensearch-py-2.3.0/opensearchpy/_async/client/cluster.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/cluster.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/client/cluster.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/dangling_indices.py` & `opensearch-py-2.3.0/opensearchpy/_async/client/dangling_indices.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/dangling_indices.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/client/dangling_indices.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/features.py` & `opensearch-py-2.3.0/opensearchpy/_async/client/features.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/features.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/client/features.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/indices.py` & `opensearch-py-2.3.0/opensearchpy/_async/client/indices.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/indices.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/client/indices.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/ingest.py` & `opensearch-py-2.3.0/opensearchpy/_async/client/ingest.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/ingest.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/client/ingest.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/nodes.py` & `opensearch-py-2.3.0/opensearchpy/_async/client/nodes.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/nodes.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/client/nodes.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/plugins.py` & `opensearch-py-2.3.0/opensearchpy/_async/client/plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,43 +6,42 @@
 #
 # Modifications Copyright OpenSearch Contributors. See
 # GitHub history for details.
 
 import warnings
 
 from ..plugins.alerting import AlertingClient
+from ..plugins.index_management import IndexManagementClient
 from .utils import NamespacedClient
 
 
 class PluginsClient(NamespacedClient):
     def __init__(self, client):
         super(PluginsClient, self).__init__(client)
         # self.query_workbench = QueryWorkbenchClient(client)
         # self.reporting = ReportingClient(client)
         # self.notebooks = NotebooksClient(client)
         self.alerting = AlertingClient(client)
         # self.anomaly_detection = AnomalyDetectionClient(client)
         # self.trace_analytics = TraceAnalyticsClient(client)
-        # self.index_management = IndexManagementClient(client)
-        # self.security = SecurityClient(client)
+        self.index_management = IndexManagementClient(client)
 
         self._dynamic_lookup(client)
 
     def _dynamic_lookup(self, client):
         # Issue : https://github.com/opensearch-project/opensearch-py/issues/90#issuecomment-1003396742
 
         plugins = [
             # "query_workbench",
             # "reporting",
             # "notebooks",
             "alerting",
             # "anomaly_detection",
             # "trace_analytics",
-            # "index_management",
-            # "security"
+            "index_management",
         ]
         for plugin in plugins:
             if not hasattr(client, plugin):
                 setattr(client, plugin, getattr(self, plugin))
             else:
                 warnings.warn(
                     f"Cannot load `{plugin}` directly to AsyncOpenSearch. `{plugin}` already exists in AsyncOpenSearch. Please use `AsyncOpenSearch.plugin.{plugin}` instead.",
```

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/plugins.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/client/plugins.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 
 from ..client import AsyncOpenSearch
 from ..plugins.alerting import AlertingClient as AlertingClient
 from .utils import NamespacedClient as NamespacedClient
 
 class PluginsClient(NamespacedClient):
     alerting: Any
+    index_management: Any
     def __init__(self, client: AsyncOpenSearch) -> None: ...
```

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/remote.py` & `opensearch-py-2.3.0/opensearchpy/_async/client/remote.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/remote.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/client/remote.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/snapshot.py` & `opensearch-py-2.3.0/opensearchpy/_async/client/snapshot.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/snapshot.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/client/snapshot.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/tasks.py` & `opensearch-py-2.3.0/opensearchpy/_async/client/tasks.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/tasks.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/client/tasks.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/utils.py` & `opensearch-py-2.3.0/opensearchpy/_async/client/utils.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/client/utils.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/client/utils.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/compat.py` & `opensearch-py-2.3.0/opensearchpy/_async/compat.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/compat.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/compat.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/helpers.py` & `opensearch-py-2.3.0/opensearchpy/_async/helpers/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,24 +28,23 @@
 # Licensed to Elasticsearch B.V.under one or more agreements.
 # Elasticsearch B.V.licenses this file to you under the Apache 2.0 License.
 # See the LICENSE file in the project root for more information
 
 import asyncio
 import logging
 
-from ..compat import map
-from ..exceptions import TransportError
-from ..helpers.actions import (
+from ...compat import map
+from ...exceptions import TransportError
+from ...helpers.actions import (
     _ActionChunker,
     _process_bulk_chunk_error,
     _process_bulk_chunk_success,
     expand_action,
 )
-from ..helpers.errors import ScanError
-from .client import AsyncOpenSearch  # noqa
+from ...helpers.errors import ScanError
 
 logger = logging.getLogger("opensearchpy.helpers")
 
 
 async def _chunk_actions(actions, chunk_size, max_chunk_bytes, serializer):
     """
     Split actions into chunks by number or size, serialize them into strings in
```

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/helpers.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/helpers/actions.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -37,16 +37,16 @@
     Mapping,
     Optional,
     Tuple,
     TypeVar,
     Union,
 )
 
-from ..serializer import Serializer
-from .client import AsyncOpenSearch
+from ...serializer import Serializer
+from ..client import AsyncOpenSearch
 
 logger: logging.Logger
 
 T = TypeVar("T")
 
 def _chunk_actions(
     actions: Any, chunk_size: int, max_chunk_bytes: int, serializer: Serializer
```

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/http_aiohttp.py` & `opensearch-py-2.3.0/opensearchpy/_async/http_aiohttp.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         ssl_assert_fingerprint=None,
         maxsize=10,
         headers=None,
         ssl_context=None,
         http_compress=None,
         opaque_id=None,
         loop=None,
+        trust_env=False,
         **kwargs
     ):
         """
         Default connection class for ``AsyncOpenSearch`` using the `aiohttp` library and the http protocol.
 
         :arg host: hostname of the node (default: localhost)
         :arg port: port to use (integer, default: 9200)
@@ -215,14 +216,15 @@
         self.loop = loop
         self.session = None
 
         # Parameters for creating an aiohttp.ClientSession later.
         self._limit = maxsize
         self._http_auth = http_auth
         self._ssl_context = ssl_context
+        self._trust_env = trust_env
 
     async def perform_request(
         self, method, url, params=None, body=None, timeout=None, ignore=(), headers=None
     ):
         if self.session is None:
             await self._create_aiohttp_session()
         assert self.session is not None
@@ -327,15 +329,19 @@
                 str(url),
                 url_path,
                 orig_body,
                 duration,
                 status_code=response.status,
                 response=raw_data,
             )
-            self._raise_error(response.status, raw_data)
+            self._raise_error(
+                response.status,
+                raw_data,
+                response.headers.get("content-type"),
+            )
 
         self.log_request_success(
             method, str(url), url_path, orig_body, response.status, raw_data, duration
         )
 
         return response.status, response.headers, raw_data
 
@@ -359,14 +365,15 @@
             auto_decompress=True,
             loop=self.loop,
             cookie_jar=aiohttp.DummyCookieJar(),
             response_class=OpenSearchClientResponse,
             connector=aiohttp.TCPConnector(
                 limit=self._limit, use_dns_cache=True, ssl=self._ssl_context
             ),
+            trust_env=self._trust_env,
         )
 
 
 class OpenSearchClientResponse(aiohttp.ClientResponse):
     async def text(self, encoding=None, errors="strict"):
         if self._body is None:
             await self.read()
```

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/http_aiohttp.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/http_aiohttp.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -62,9 +62,10 @@
         ssl_assert_fingerprint: Optional[Any] = ...,
         maxsize: int = ...,
         headers: Optional[Mapping[str, str]] = ...,
         ssl_context: Optional[Any] = ...,
         http_compress: Optional[bool] = ...,
         opaque_id: Optional[str] = ...,
         loop: Any = ...,
+        trust_env: bool = ...,
         **kwargs: Any
     ) -> None: ...
```

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/plugins/alerting.py` & `opensearch-py-2.3.0/opensearchpy/_async/plugins/alerting.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/plugins/alerting.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/plugins/alerting.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/transport.py` & `opensearch-py-2.3.0/opensearchpy/_async/transport.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_async/transport.pyi` & `opensearch-py-2.3.0/opensearchpy/_async/transport.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/_version.py` & `opensearch-py-2.3.0/opensearchpy/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-__versionstr__ = "2.2.0"
+__versionstr__ = "2.3.0"
```

### Comparing `opensearch-py-2.2.0/opensearchpy/client/__init__.py` & `opensearch-py-2.3.0/opensearchpy/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from .dangling_indices import DanglingIndicesClient
 from .features import FeaturesClient
 from .indices import IndicesClient
 from .ingest import IngestClient
 from .nodes import NodesClient
 from .plugins import PluginsClient
 from .remote import RemoteClient
+from .security import SecurityClient
 from .snapshot import SnapshotClient
 from .tasks import TasksClient
 from .utils import SKIP_IN_PATH, _bulk_body, _make_path, _normalize_hosts, query_params
 
 logger = logging.getLogger("opensearch")
 
 
@@ -193,14 +194,15 @@
         self.cat = CatClient(self)
         self.cluster = ClusterClient(self)
         self.dangling_indices = DanglingIndicesClient(self)
         self.indices = IndicesClient(self)
         self.ingest = IngestClient(self)
         self.nodes = NodesClient(self)
         self.remote = RemoteClient(self)
+        self.security = SecurityClient(self)
         self.snapshot = SnapshotClient(self)
         self.tasks = TasksClient(self)
 
         self.features = FeaturesClient(self)
 
         self.plugins = PluginsClient(self)
```

### Comparing `opensearch-py-2.2.0/opensearchpy/client/__init__.pyi` & `opensearch-py-2.3.0/opensearchpy/client/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from .cluster import ClusterClient
 from .dangling_indices import DanglingIndicesClient
 from .features import FeaturesClient
 from .indices import IndicesClient
 from .ingest import IngestClient
 from .nodes import NodesClient
 from .remote import RemoteClient
+from .security import SecurityClient
 from .snapshot import SnapshotClient
 from .tasks import TasksClient
 
 logger: logging.Logger
 
 class OpenSearch(object):
     transport: Transport
@@ -50,14 +51,15 @@
     cat: CatClient
     cluster: ClusterClient
     features: FeaturesClient
     indices: IndicesClient
     ingest: IngestClient
     nodes: NodesClient
     remote: RemoteClient
+    security: SecurityClient
     snapshot: SnapshotClient
     tasks: TasksClient
     def __init__(
         self, hosts: Any = ..., transport_class: Type[Transport] = ..., **kwargs: Any
     ) -> None: ...
     def __repr__(self) -> str: ...
     def __enter__(self) -> "OpenSearch": ...
@@ -1048,32 +1050,49 @@
         ignore: Optional[Union[int, Collection[int]]] = ...,
         opaque_id: Optional[str] = ...,
         http_auth: Optional[Union[str, Tuple[str, str]]] = ...,
         api_key: Optional[Union[str, Tuple[str, str]]] = ...,
         params: Optional[MutableMapping[str, Any]] = ...,
         headers: Optional[MutableMapping[str, str]] = ...,
     ) -> Any: ...
-    def close_point_in_time(
+    def list_all_point_in_time(
+        self,
+        *,
+        pretty: Optional[bool] = ...,
+        human: Optional[bool] = ...,
+        error_trace: Optional[bool] = ...,
+        format: Optional[str] = ...,
+        filter_path: Optional[Union[str, Collection[str]]] = ...,
+        request_timeout: Optional[Union[int, float]] = ...,
+        ignore: Optional[Union[int, Collection[int]]] = ...,
+        opaque_id: Optional[str] = ...,
+        http_auth: Optional[Union[str, Tuple[str, str]]] = ...,
+        api_key: Optional[Union[str, Tuple[str, str]]] = ...,
+        params: Optional[MutableMapping[str, Any]] = ...,
+        headers: Optional[MutableMapping[str, str]] = ...,
+    ) -> Any: ...
+    def delete_point_in_time(
         self,
         *,
         body: Optional[Any] = ...,
+        all: Optional[bool] = ...,
         pretty: Optional[bool] = ...,
         human: Optional[bool] = ...,
         error_trace: Optional[bool] = ...,
         format: Optional[str] = ...,
         filter_path: Optional[Union[str, Collection[str]]] = ...,
         request_timeout: Optional[Union[int, float]] = ...,
         ignore: Optional[Union[int, Collection[int]]] = ...,
         opaque_id: Optional[str] = ...,
         http_auth: Optional[Union[str, Tuple[str, str]]] = ...,
         api_key: Optional[Union[str, Tuple[str, str]]] = ...,
         params: Optional[MutableMapping[str, Any]] = ...,
         headers: Optional[MutableMapping[str, str]] = ...,
     ) -> Any: ...
-    def open_point_in_time(
+    def create_point_in_time(
         self,
         *,
         index: Optional[Any] = ...,
         expand_wildcards: Optional[Any] = ...,
         ignore_unavailable: Optional[Any] = ...,
         keep_alive: Optional[Any] = ...,
         preference: Optional[Any] = ...,
```

### Comparing `opensearch-py-2.2.0/opensearchpy/client/cat.py` & `opensearch-py-2.3.0/opensearchpy/client/cat.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/cat.pyi` & `opensearch-py-2.3.0/opensearchpy/client/cat.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/cluster.py` & `opensearch-py-2.3.0/opensearchpy/client/cluster.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/cluster.pyi` & `opensearch-py-2.3.0/opensearchpy/client/cluster.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/dangling_indices.py` & `opensearch-py-2.3.0/opensearchpy/client/dangling_indices.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/dangling_indices.pyi` & `opensearch-py-2.3.0/opensearchpy/client/dangling_indices.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/features.py` & `opensearch-py-2.3.0/opensearchpy/client/features.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/features.pyi` & `opensearch-py-2.3.0/opensearchpy/client/features.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/indices.py` & `opensearch-py-2.3.0/opensearchpy/client/indices.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/indices.pyi` & `opensearch-py-2.3.0/opensearchpy/client/indices.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/ingest.py` & `opensearch-py-2.3.0/opensearchpy/client/ingest.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/ingest.pyi` & `opensearch-py-2.3.0/opensearchpy/client/ingest.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/nodes.py` & `opensearch-py-2.3.0/opensearchpy/client/nodes.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/nodes.pyi` & `opensearch-py-2.3.0/opensearchpy/client/nodes.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/plugins.py` & `opensearch-py-2.3.0/opensearchpy/client/plugins.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,43 +7,42 @@
 # Modifications Copyright OpenSearch Contributors. See
 # GitHub history for details.
 
 
 import warnings
 
 from ..plugins.alerting import AlertingClient
+from ..plugins.index_management import IndexManagementClient
 from .utils import NamespacedClient
 
 
 class PluginsClient(NamespacedClient):
     def __init__(self, client):
         super(PluginsClient, self).__init__(client)
         # self.query_workbench = QueryWorkbenchClient(client)
         # self.reporting = ReportingClient(client)
         # self.notebooks = NotebooksClient(client)
         self.alerting = AlertingClient(client)
         # self.anomaly_detection = AnomalyDetectionClient(client)
         # self.trace_analytics = TraceAnalyticsClient(client)
-        # self.index_management = IndexManagementClient(client)
-        # self.security = SecurityClient(client)
+        self.index_management = IndexManagementClient(client)
 
         self._dynamic_lookup(client)
 
     def _dynamic_lookup(self, client):
         # Issue : https://github.com/opensearch-project/opensearch-py/issues/90#issuecomment-1003396742
 
         plugins = [
             # "query_workbench",
             # "reporting",
             # "notebooks",
             "alerting",
             # "anomaly_detection",
             # "trace_analytics",
-            # "index_management",
-            # "security"
+            "index_management",
         ]
         for plugin in plugins:
             if not hasattr(client, plugin):
                 setattr(client, plugin, getattr(self, plugin))
             else:
                 warnings.warn(
                     "Cannot load `{plugin}` directly to OpenSearch. `{plugin}` already exists in OpenSearch. Please use `OpenSearch.plugin.{plugin}` instead.".format(
```

### Comparing `opensearch-py-2.2.0/opensearchpy/client/plugins.pyi` & `opensearch-py-2.3.0/opensearchpy/client/plugins.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 
 from ..client import OpenSearch
 from ..plugins.alerting import AlertingClient as AlertingClient
 from .utils import NamespacedClient as NamespacedClient
 
 class PluginsClient(NamespacedClient):
     alerting: Any
+    index_management: Any
     def __init__(self, client: OpenSearch) -> None: ...
```

### Comparing `opensearch-py-2.2.0/opensearchpy/client/remote.py` & `opensearch-py-2.3.0/opensearchpy/client/remote.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/remote.pyi` & `opensearch-py-2.3.0/opensearchpy/client/remote.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/snapshot.py` & `opensearch-py-2.3.0/opensearchpy/client/snapshot.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/snapshot.pyi` & `opensearch-py-2.3.0/opensearchpy/client/snapshot.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/tasks.py` & `opensearch-py-2.3.0/opensearchpy/client/tasks.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/tasks.pyi` & `opensearch-py-2.3.0/opensearchpy/client/tasks.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/client/utils.py` & `opensearch-py-2.3.0/opensearchpy/client/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,24 +161,25 @@
             elif http_auth is not None:
                 headers["authorization"] = "Basic %s" % (
                     _base64_auth_header(http_auth),
                 )
             elif api_key is not None:
                 headers["authorization"] = "ApiKey %s" % (_base64_auth_header(api_key),)
 
+            # don't escape ignore, request_timeout, or timeout
+            for p in ("ignore", "request_timeout", "timeout"):
+                if p in kwargs:
+                    params[p] = kwargs.pop(p)
+
             for p in opensearch_query_params + GLOBAL_PARAMS:
                 if p in kwargs:
                     v = kwargs.pop(p)
                     if v is not None:
                         params[p] = _escape(v)
 
-            # don't treat ignore, request_timeout, and opaque_id as other params to avoid escaping
-            for p in ("ignore", "request_timeout"):
-                if p in kwargs:
-                    params[p] = kwargs.pop(p)
             return func(*args, params=params, headers=headers, **kwargs)
 
         return _wrapped
 
     return _wrapper
```

### Comparing `opensearch-py-2.2.0/opensearchpy/client/utils.pyi` & `opensearch-py-2.3.0/opensearchpy/client/utils.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/compat.py` & `opensearch-py-2.3.0/opensearchpy/compat.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/compat.pyi` & `opensearch-py-2.3.0/opensearchpy/compat.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/connection/__init__.py` & `opensearch-py-2.3.0/opensearchpy/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/connection/__init__.pyi` & `opensearch-py-2.3.0/opensearchpy/connection/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/connection/base.py` & `opensearch-py-2.3.0/opensearchpy/connection/base.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/connection/base.pyi` & `opensearch-py-2.3.0/opensearchpy/connection/base.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/connection/connections.py` & `opensearch-py-2.3.0/opensearchpy/connection/connections.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/connection/connections.pyi` & `opensearch-py-2.3.0/opensearchpy/connection/connections.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/connection/http_async.py` & `opensearch-py-2.3.0/opensearchpy/connection/http_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,17 +61,18 @@
             http_compress=http_compress,
             opaque_id=opaque_id,
             **kwargs
         )
 
         if http_auth is not None:
             if isinstance(http_auth, (tuple, list)):
-                http_auth = ":".join(http_auth)
+                http_auth = aiohttp.BasicAuth(login=http_auth[0], password=http_auth[1])
             elif isinstance(http_auth, string_types):
-                http_auth = tuple(http_auth.split(":", 1))
+                login, password = http_auth.split(":", 1)
+                http_auth = aiohttp.BasicAuth(login=login, password=password)
 
         # if providing an SSL context, raise error if any other SSL related flag is used
         if ssl_context and (
             (verify_certs is not VERIFY_CERTS_DEFAULT)
             or (ssl_show_warn is not SSL_SHOW_WARN_DEFAULT)
             or ca_certs
             or client_cert
@@ -186,25 +187,30 @@
         if headers:
             req_headers.update(headers)
 
         if self.http_compress and body:
             body = self._gzip_compress(body)
             req_headers["content-encoding"] = "gzip"
 
-        req_headers = {
-            **req_headers,
-            **self._http_auth(method, url, query_string, body),
-        }
+        auth = (
+            self._http_auth if isinstance(self._http_auth, aiohttp.BasicAuth) else None
+        )
+        if callable(self._http_auth):
+            req_headers = {
+                **req_headers,
+                **self._http_auth(method, url, query_string, body),
+            }
 
         start = self.loop.time()
         try:
             async with self.session.request(
                 method,
                 url,
                 data=body,
+                auth=auth,
                 headers=req_headers,
                 timeout=timeout,
                 fingerprint=self.ssl_assert_fingerprint,
             ) as response:
                 if is_head:  # We actually called 'GET' so throw away the data.
                     await response.release()
                     raw_data = ""
```

### Comparing `opensearch-py-2.2.0/opensearchpy/connection/http_async.pyi` & `opensearch-py-2.3.0/opensearchpy/connection/http_async.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/connection/http_requests.py` & `opensearch-py-2.3.0/opensearchpy/connection/http_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,23 @@
         if self.use_ssl and not verify_certs and ssl_show_warn:
             warnings.warn(
                 "Connecting to %s using SSL with verify_certs=False is insecure."
                 % self.host
             )
 
     def perform_request(
-        self, method, url, params=None, body=None, timeout=None, ignore=(), headers=None
+        self,
+        method,
+        url,
+        params=None,
+        body=None,
+        timeout=None,
+        allow_redirects=True,
+        ignore=(),
+        headers=None,
     ):
         url = self.base_url + url
         headers = headers or {}
         if params:
             url = "%s?%s" % (url, urlencode(params or {}))
 
         orig_body = body
@@ -169,15 +177,18 @@
 
         start = time.time()
         request = requests.Request(method=method, headers=headers, url=url, data=body)
         prepared_request = self.session.prepare_request(request)
         settings = self.session.merge_environment_settings(
             prepared_request.url, {}, None, None, None
         )
-        send_kwargs = {"timeout": timeout or self.timeout}
+        send_kwargs = {
+            "timeout": timeout or self.timeout,
+            "allow_redirects": allow_redirects,
+        }
         send_kwargs.update(settings)
         try:
             response = self.session.send(prepared_request, **send_kwargs)
             duration = time.time() - start
             raw_data = response.content.decode("utf-8", "surrogatepass")
         except reraise_exceptions:
             raise
```

### Comparing `opensearch-py-2.2.0/opensearchpy/connection/http_requests.pyi` & `opensearch-py-2.3.0/opensearchpy/connection/http_requests.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/connection/http_urllib3.py` & `opensearch-py-2.3.0/opensearchpy/connection/http_urllib3.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/connection/http_urllib3.pyi` & `opensearch-py-2.3.0/opensearchpy/connection/http_urllib3.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/connection/pooling.py` & `opensearch-py-2.3.0/opensearchpy/connection/pooling.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/connection/pooling.pyi` & `opensearch-py-2.3.0/opensearchpy/connection/pooling.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/connection_pool.py` & `opensearch-py-2.3.0/opensearchpy/connection_pool.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/connection_pool.pyi` & `opensearch-py-2.3.0/opensearchpy/connection_pool.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/exceptions.py` & `opensearch-py-2.3.0/opensearchpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/exceptions.pyi` & `opensearch-py-2.3.0/opensearchpy/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/__init__.py` & `opensearch-py-2.3.0/opensearchpy/helpers/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,22 +53,17 @@
     "_chunk_actions",
     "_process_bulk_chunk",
     "AWSV4SignerAuth",
     "AWSV4SignerAsyncAuth",
 ]
 
 
-try:
-    # Asyncio only supported on Python 3.6+
-    if sys.version_info < (3, 6):
-        raise ImportError
-
-    from .._async.helpers import (
+# Asyncio only supported on Python 3.6+
+if sys.version_info >= (3, 6):
+    from .._async.helpers.actions import (
         async_bulk,
         async_reindex,
         async_scan,
         async_streaming_bulk,
     )
 
     __all__ += ["async_scan", "async_bulk", "async_reindex", "async_streaming_bulk"]
-except (ImportError, SyntaxError):
-    pass
```

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/__init__.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/__init__.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from .errors import ScanError as ScanError
 
 try:
     # Asyncio only supported on Python 3.6+
     if sys.version_info < (3, 6):
         raise ImportError
 
-    from .._async.helpers import async_bulk as async_bulk
-    from .._async.helpers import async_reindex as async_reindex
-    from .._async.helpers import async_scan as async_scan
-    from .._async.helpers import async_streaming_bulk as async_streaming_bulk
+    from .._async.helpers.actions import async_bulk as async_bulk
+    from .._async.helpers.actions import async_reindex as async_reindex
+    from .._async.helpers.actions import async_scan as async_scan
+    from .._async.helpers.actions import async_streaming_bulk as async_streaming_bulk
     from .asyncsigner import AWSV4SignerAsyncAuth as AWSV4SignerAsyncAuth
     from .signer import AWSV4SignerAuth as AWSV4SignerAuth
 except (ImportError, SyntaxError):
     pass
```

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/actions.py` & `opensearch-py-2.3.0/opensearchpy/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/actions.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/actions.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/aggs.py` & `opensearch-py-2.3.0/opensearchpy/helpers/aggs.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/aggs.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/aggs.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/analysis.py` & `opensearch-py-2.3.0/opensearchpy/helpers/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
 import six
 
 from opensearchpy.connection.connections import get_connection
-
-from .utils import AttrDict, DslBase, merge
+from opensearchpy.helpers.utils import AttrDict, DslBase, merge
 
 __all__ = ["tokenizer", "analyzer", "char_filter", "token_filter", "normalizer"]
 
 
 class AnalysisBase(object):
     @classmethod
     def _type_shortcut(cls, name_or_instance, type=None, **kwargs):
```

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/analysis.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/analysis.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/asyncsigner.py` & `opensearch-py-2.3.0/opensearchpy/helpers/asyncsigner.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/asyncsigner.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/asyncsigner.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/document.py` & `opensearch-py-2.3.0/opensearchpy/helpers/document.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/document.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/document.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/errors.py` & `opensearch-py-2.3.0/opensearchpy/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/errors.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/errors.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/faceted_search.py` & `opensearch-py-2.3.0/opensearchpy/helpers/faceted_search.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/faceted_search.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/faceted_search.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/field.py` & `opensearch-py-2.3.0/opensearchpy/helpers/field.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/field.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/field.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/function.py` & `opensearch-py-2.3.0/opensearchpy/helpers/function.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/function.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/function.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/index.py` & `opensearch-py-2.3.0/opensearchpy/helpers/index.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/index.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/index.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/mapping.py` & `opensearch-py-2.3.0/opensearchpy/helpers/mapping.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/mapping.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/mapping.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/query.py` & `opensearch-py-2.3.0/opensearchpy/helpers/query.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/query.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/query.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/response/__init__.py` & `opensearch-py-2.3.0/opensearchpy/helpers/response/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/response/__init__.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/response/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/response/aggs.py` & `opensearch-py-2.3.0/opensearchpy/helpers/response/aggs.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/response/aggs.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/response/aggs.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/response/hit.py` & `opensearch-py-2.3.0/opensearchpy/helpers/response/hit.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/response/hit.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/response/hit.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/search.py` & `opensearch-py-2.3.0/opensearchpy/helpers/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,14 +327,15 @@
         All the parameters supplied (or omitted) at creation type can be later
         overridden by methods (`using`, `index` and `doc_type` respectively).
         """
         super(Search, self).__init__(**kwargs)
 
         self.aggs = AggsProxy(self)
         self._sort = []
+        self._collapse = {}
         self._source = None
         self._highlight = {}
         self._highlight_opts = {}
         self._suggest = {}
         self._script_fields = {}
         self._response_class = Response
 
@@ -575,14 +576,37 @@
             if isinstance(k, string_types) and k.startswith("-"):
                 if k[1:] == "_score":
                     raise IllegalOperation("Sorting by `-_score` is not allowed.")
                 k = {k[1:]: {"order": "desc"}}
             s._sort.append(k)
         return s
 
+    def collapse(self, field=None, inner_hits=None, max_concurrent_group_searches=None):
+        """
+        Add collapsing information to the search request.
+
+        If called without providing ``field``, it will remove all collapse
+        requirements, otherwise it will replace them with the provided
+        arguments.
+
+        The API returns a copy of the Search object and can thus be chained.
+        """
+        s = self._clone()
+        s._collapse = {}
+
+        if field is None:
+            return s
+
+        s._collapse["field"] = field
+        if inner_hits:
+            s._collapse["inner_hits"] = inner_hits
+        if max_concurrent_group_searches:
+            s._collapse["max_concurrent_group_searches"] = max_concurrent_group_searches
+        return s
+
     def highlight_options(self, **kwargs):
         """
         Update the global highlighting options used for this request. For
         example::
 
             s = Search()
             s = s.highlight_options(order='score')
@@ -670,14 +694,17 @@
 
             if self.aggs.aggs:
                 d.update(self.aggs.to_dict())
 
             if self._sort:
                 d["sort"] = self._sort
 
+            if self._collapse:
+                d["collapse"] = self._collapse
+
             d.update(recursive_to_dict(self._extra))
 
             if self._source not in (None, {}):
                 d["_source"] = self._source
 
             if self._highlight:
                 d["highlight"] = {"fields": self._highlight}
```

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/search.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/search.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/signer.py` & `opensearch-py-2.3.0/opensearchpy/helpers/signer.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/test.py` & `opensearch-py-2.3.0/opensearchpy/helpers/test.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/test.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/test.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/update_by_query.py` & `opensearch-py-2.3.0/opensearchpy/helpers/update_by_query.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/update_by_query.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/update_by_query.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/utils.py` & `opensearch-py-2.3.0/opensearchpy/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/utils.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/utils.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/wrappers.py` & `opensearch-py-2.3.0/opensearchpy/helpers/wrappers.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/helpers/wrappers.pyi` & `opensearch-py-2.3.0/opensearchpy/helpers/wrappers.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/plugins/alerting.py` & `opensearch-py-2.3.0/opensearchpy/plugins/alerting.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/plugins/alerting.pyi` & `opensearch-py-2.3.0/opensearchpy/plugins/alerting.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/serializer.py` & `opensearch-py-2.3.0/opensearchpy/serializer.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/serializer.pyi` & `opensearch-py-2.3.0/opensearchpy/serializer.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/transport.py` & `opensearch-py-2.3.0/opensearchpy/transport.py`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/opensearchpy/transport.pyi` & `opensearch-py-2.3.0/opensearchpy/transport.pyi`

 * *Files identical despite different names*

### Comparing `opensearch-py-2.2.0/setup.py` & `opensearch-py-2.3.0/setup.py`

 * *Files identical despite different names*

