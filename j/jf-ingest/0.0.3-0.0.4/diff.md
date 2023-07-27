# Comparing `tmp/jf_ingest-0.0.3.tar.gz` & `tmp/jf_ingest-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jf_ingest-0.0.3.tar", last modified: Wed Jul 26 15:55:55 2023, max compression
+gzip compressed data, was "jf_ingest-0.0.4.tar", last modified: Thu Jul 27 15:04:54 2023, max compression
```

## Comparing `jf_ingest-0.0.3.tar` & `jf_ingest-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-07-19 15:50:56.382404 jf_ingest-0.0.3/LICENSE
--rw-r--r--   0        0        0       19 2023-07-21 18:28:01.314703 jf_ingest-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-07-26 15:55:41.201986 jf_ingest-0.0.3/jf_ingest/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 18:28:01.314868 jf_ingest-0.0.3/jf_ingest/jf_jira/__init__.py
--rw-r--r--   0        0        0     1692 2023-07-21 18:28:01.315993 jf_ingest-0.0.3/jf_ingest/jf_jira/downloaders.py
--rw-r--r--   0        0        0      679 2023-07-26 15:55:55.443279 jf_ingest-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 18:28:01.319487 jf_ingest-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 15:55:41.203566 jf_ingest-0.0.3/tests/jf_jira/__init__.py
--rw-r--r--   0        0        0     1837 2023-07-26 15:55:41.204174 jf_ingest-0.0.3/tests/jf_jira/fixtures/jira_fields_response.json
--rw-r--r--   0        0        0     3162 2023-07-26 15:55:41.204525 jf_ingest-0.0.3/tests/jf_jira/test_jira_downloaders.py
--rw-r--r--   0        0        0      377 1970-01-01 00:00:00.000000 jf_ingest-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-19 15:50:56.382404 jf_ingest-0.0.4/LICENSE
+-rw-r--r--   0        0        0       19 2023-07-21 18:28:01.314703 jf_ingest-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 15:55:41.201986 jf_ingest-0.0.4/jf_ingest/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 18:28:01.314868 jf_ingest-0.0.4/jf_ingest/jf_jira/__init__.py
+-rw-r--r--   0        0        0     1863 2023-07-27 15:04:45.351692 jf_ingest-0.0.4/jf_ingest/jf_jira/downloaders.py
+-rw-r--r--   0        0        0      679 2023-07-27 15:04:54.282612 jf_ingest-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 18:28:01.319487 jf_ingest-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:55:41.203566 jf_ingest-0.0.4/tests/jf_jira/__init__.py
+-rw-r--r--   0        0        0     1837 2023-07-26 15:55:41.204174 jf_ingest-0.0.4/tests/jf_jira/fixtures/jira_fields_response.json
+-rw-r--r--   0        0        0     3121 2023-07-27 15:04:45.353600 jf_ingest-0.0.4/tests/jf_jira/test_jira_downloaders.py
+-rw-r--r--   0        0        0      377 1970-01-01 00:00:00.000000 jf_ingest-0.0.4/PKG-INFO
```

### Comparing `jf_ingest-0.0.3/LICENSE` & `jf_ingest-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jf_ingest-0.0.3/jf_ingest/jf_jira/downloaders.py` & `jf_ingest-0.0.4/jf_ingest/jf_jira/downloaders.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from jira import JIRA
-from jira.resources import AgileResource
+# jira renamed this between api versions for some reason
+try:
+    from jira.resources import AgileResource as AGILE_BASE_REST_PATH
+except ImportError:
+    from jira.resources import GreenHopperResource as AGILE_BASE_REST_PATH
 
 
 def get_jira_connection(config, creds, max_retries=3):
     kwargs = {
         'server': config.jira_url,
         'max_retries': max_retries,
         'options': {
-            'agile_rest_path': AgileResource.AGILE_BASE_REST_PATH,
+            'agile_rest_path': AGILE_BASE_REST_PATH,
             'verify': not config.skip_ssl_verification,
         },
     }
 
     if creds.jira_username and creds.jira_password:
         kwargs['basic_auth'] = (creds.jira_username, creds.jira_password)
     elif creds.jira_bearer_token:
```

### Comparing `jf_ingest-0.0.3/pyproject.toml` & `jf_ingest-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jf_ingest"
-version = "0.0.3"
+version = "0.0.4"
 readme = "README.md"
 description = "library used for ingesting jira data"
 authors = [
     { name = "jellyfish-oss", email = "oss@jellyfish.co" },
 ]
 dependencies = [
     "jira >= 2.0.0, < 2.1",
```

### Comparing `jf_ingest-0.0.3/tests/jf_jira/fixtures/jira_fields_response.json` & `jf_ingest-0.0.4/tests/jf_jira/fixtures/jira_fields_response.json`

 * *Files identical despite different names*

### Comparing `jf_ingest-0.0.3/tests/jf_jira/test_jira_downloaders.py` & `jf_ingest-0.0.4/tests/jf_jira/test_jira_downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 
 import requests_mock
 from unittest import TestCase
 
-from jf_ingest.jf_jira.downloaders import get_jira_connection
-from jf_ingest.jf_jira.downloaders import download_fields
+from jf_ingest.jf_jira.downloaders import get_jira_connection, download_fields
 
 MOCK_SERVER_INFO_RESP = '{"baseUrl":"https://test-co.atlassian.net","version":"1001.0.0-SNAPSHOT",' \
                         '"versionNumbers":[1001,0,0],"deploymentType":"Cloud","buildNumber":100218,' \
                         '"buildDate":"2023-03-16T08:21:48.000-0400","serverTime":"2023-03-17T16:32:45.255-0400",' \
                         '"scmInfo":"9999999999999999999999999999999999999999","serverTitle":"JIRA",' \
                         '"defaultLocale":{"locale":"en_US"}} '
```

