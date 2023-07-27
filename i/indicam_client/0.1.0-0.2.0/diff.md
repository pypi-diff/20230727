# Comparing `tmp/indicam_client-0.1.0.tar.gz` & `tmp/indicam_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indicam_client-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indicam_client-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indicam_client-0.1.0.tar` & `indicam_client-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      292 2023-07-13 19:20:46.669162 indicam_client-0.1.0/.editorconfig
--rw-r--r--   0        0        0      325 2023-07-13 19:20:46.693162 indicam_client-0.1.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0     1204 2023-07-13 19:20:46.661162 indicam_client-0.1.0/.gitignore
--rw-r--r--   0        0        0      290 2023-07-13 19:20:46.645162 indicam_client-0.1.0/.travis.yml
--rw-r--r--   0        0        0      154 2023-07-13 19:20:46.669162 indicam_client-0.1.0/AUTHORS.rst
--rw-r--r--   0        0        0     3611 2023-07-13 19:20:46.661162 indicam_client-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0       89 2023-07-13 19:20:46.669162 indicam_client-0.1.0/HISTORY.rst
--rw-r--r--   0        0        0     1071 2023-07-13 19:20:46.649162 indicam_client-0.1.0/LICENSE
--rw-r--r--   0        0        0      262 2023-07-13 19:20:46.661162 indicam_client-0.1.0/MANIFEST.in
--rw-r--r--   0        0        0     2323 2023-07-13 19:20:46.653162 indicam_client-0.1.0/Makefile
--rw-r--r--   0        0        0      658 2023-07-14 20:15:23.503574 indicam_client-0.1.0/README.rst
--rw-r--r--   0        0        0      615 2023-07-13 19:20:46.685162 indicam_client-0.1.0/docs/Makefile
--rw-r--r--   0        0        0       28 2023-07-13 19:20:46.685162 indicam_client-0.1.0/docs/authors.rst
--rwxr-xr-x   0        0        0     4869 2023-07-13 19:20:46.693162 indicam_client-0.1.0/docs/conf.py
--rw-r--r--   0        0        0       33 2023-07-13 19:20:46.685162 indicam_client-0.1.0/docs/contributing.rst
--rw-r--r--   0        0        0       28 2023-07-13 19:20:46.689162 indicam_client-0.1.0/docs/history.rst
--rw-r--r--   0        0        0      311 2023-07-13 19:20:46.685162 indicam_client-0.1.0/docs/index.rst
--rw-r--r--   0        0        0     1174 2023-07-13 19:20:46.681162 indicam_client-0.1.0/docs/installation.rst
--rw-r--r--   0        0        0      812 2023-07-13 19:20:46.689162 indicam_client-0.1.0/docs/make.bat
--rw-r--r--   0        0        0       27 2023-07-13 19:20:46.685162 indicam_client-0.1.0/docs/readme.rst
--rw-r--r--   0        0        0       83 2023-07-13 19:20:46.681162 indicam_client-0.1.0/docs/usage.rst
--rw-r--r--   0        0        0       68 2023-07-20 18:49:11.457350 indicam_client-0.1.0/indicam_client/__init__.py
--rw-r--r--   0        0        0     5483 2023-07-14 20:52:28.286784 indicam_client-0.1.0/indicam_client/indicam_client.py
--rw-r--r--   0        0        0      509 2023-07-20 18:49:11.413350 indicam_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       18 2023-07-14 21:20:15.496566 indicam_client-0.1.0/requirements.txt
--rw-r--r--   0        0        0      107 2023-07-20 18:41:34.753873 indicam_client-0.1.0/requirements_dev.txt
--rw-r--r--   0        0        0      347 2023-07-13 19:20:46.661162 indicam_client-0.1.0/setup.cfg
--rw-r--r--   0        0        0     1348 2023-07-13 19:20:46.665162 indicam_client-0.1.0/setup.py
--rw-r--r--   0        0        0       44 2023-07-13 19:20:46.677162 indicam_client-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     6160 2023-07-20 18:34:45.544929 indicam_client-0.1.0/tests/test_indicam_client.py
--rw-r--r--   0        0        0      275 2023-07-13 19:20:46.661162 indicam_client-0.1.0/tox.ini
--rw-r--r--   0        0        0     1051 1970-01-01 00:00:00.000000 indicam_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      292 2023-07-13 19:20:46.669162 indicam_client-0.2.0/.editorconfig
+-rw-r--r--   0        0        0      325 2023-07-13 19:20:46.693162 indicam_client-0.2.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0     1204 2023-07-13 19:20:46.661162 indicam_client-0.2.0/.gitignore
+-rw-r--r--   0        0        0      290 2023-07-13 19:20:46.645162 indicam_client-0.2.0/.travis.yml
+-rw-r--r--   0        0        0      154 2023-07-13 19:20:46.669162 indicam_client-0.2.0/AUTHORS.rst
+-rw-r--r--   0        0        0     3611 2023-07-13 19:20:46.661162 indicam_client-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      310 2023-07-27 19:55:42.859196 indicam_client-0.2.0/HISTORY.rst
+-rw-r--r--   0        0        0     1071 2023-07-13 19:20:46.649162 indicam_client-0.2.0/LICENSE
+-rw-r--r--   0        0        0      262 2023-07-13 19:20:46.661162 indicam_client-0.2.0/MANIFEST.in
+-rw-r--r--   0        0        0     2323 2023-07-13 19:20:46.653162 indicam_client-0.2.0/Makefile
+-rw-r--r--   0        0        0      498 2023-07-27 19:52:20.726633 indicam_client-0.2.0/README.rst
+-rw-r--r--   0        0        0      615 2023-07-13 19:20:46.685162 indicam_client-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0       28 2023-07-13 19:20:46.685162 indicam_client-0.2.0/docs/authors.rst
+-rwxr-xr-x   0        0        0     4869 2023-07-13 19:20:46.693162 indicam_client-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0       33 2023-07-13 19:20:46.685162 indicam_client-0.2.0/docs/contributing.rst
+-rw-r--r--   0        0        0       28 2023-07-13 19:20:46.689162 indicam_client-0.2.0/docs/history.rst
+-rw-r--r--   0        0        0      311 2023-07-13 19:20:46.685162 indicam_client-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0     1174 2023-07-13 19:20:46.681162 indicam_client-0.2.0/docs/installation.rst
+-rw-r--r--   0        0        0      812 2023-07-13 19:20:46.689162 indicam_client-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0       27 2023-07-13 19:20:46.685162 indicam_client-0.2.0/docs/readme.rst
+-rw-r--r--   0        0        0       83 2023-07-13 19:20:46.681162 indicam_client-0.2.0/docs/usage.rst
+-rw-r--r--   0        0        0       68 2023-07-27 19:53:18.382802 indicam_client-0.2.0/indicam_client/__init__.py
+-rw-r--r--   0        0        0     6117 2023-07-27 19:48:54.041949 indicam_client-0.2.0/indicam_client/indicam_client.py
+-rw-r--r--   0        0        0      509 2023-07-20 18:49:11.413350 indicam_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-07-14 21:20:15.496566 indicam_client-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      107 2023-07-20 18:41:34.753873 indicam_client-0.2.0/requirements_dev.txt
+-rw-r--r--   0        0        0      347 2023-07-27 19:56:25.811305 indicam_client-0.2.0/setup.cfg
+-rw-r--r--   0        0        0     1348 2023-07-13 19:20:46.665162 indicam_client-0.2.0/setup.py
+-rw-r--r--   0        0        0       44 2023-07-13 19:20:46.677162 indicam_client-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     6160 2023-07-20 18:34:45.544929 indicam_client-0.2.0/tests/test_indicam_client.py
+-rw-r--r--   0        0        0      275 2023-07-13 19:20:46.661162 indicam_client-0.2.0/tox.ini
+-rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 indicam_client-0.2.0/PKG-INFO
```

### Comparing `indicam_client-0.1.0/.gitignore` & `indicam_client-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `indicam_client-0.1.0/CONTRIBUTING.rst` & `indicam_client-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `indicam_client-0.1.0/LICENSE` & `indicam_client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `indicam_client-0.1.0/Makefile` & `indicam_client-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `indicam_client-0.1.0/docs/Makefile` & `indicam_client-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `indicam_client-0.1.0/docs/conf.py` & `indicam_client-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `indicam_client-0.1.0/docs/installation.rst` & `indicam_client-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `indicam_client-0.1.0/docs/make.bat` & `indicam_client-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `indicam_client-0.1.0/indicam_client/indicam_client.py` & `indicam_client-0.2.0/indicam_client/indicam_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from __future__ import annotations
 
 import io
 from dataclasses import dataclass
 import logging
+from typing import Any, Optional
 
 import requests as req
 
 # Camera config items
 CAMCONFIG_MAX_KEY = 'full_perc_from_top'
 CAMCONFIG_MIN_KEY = 'empty_perc_from_bottom'
 # Timeout for service requests
@@ -60,14 +61,31 @@
                 "Failed to find the indicam - handle=%s, status=%d",
                 name,
                 response.status_code
             )
             return None
         return response.json()[0]['id']
 
+    def list_indicams(self) -> Optional[dict[str, Any]]:
+        """Return a list of all the indicams belonging to the user. Might be empty. Returns "None" if an error
+        occurred.
+        """
+        response = req.get(
+            f'{self._url}/indicams/',
+            timeout=HTTP_TIMEOUT,
+            headers=self._req_header
+        )
+        if response.status_code != 200:
+            _LOGGER.error(
+                "Failed to return a list of indicams, even if empty - status=%d",
+                response.status_code
+            )
+            return None
+        return response.json()
+
     def get_camconfig(self, indicam_id: int) -> CamConfig | None:
         """ Get the service's version of the camera configuration. """
         response = req.get(
             f'{self._url}/indicams/{indicam_id}/camconfig_current/',
             timeout=HTTP_TIMEOUT,
             headers=self._req_header
         )
```

### Comparing `indicam_client-0.1.0/setup.py` & `indicam_client-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `indicam_client-0.1.0/tests/test_indicam_client.py` & `indicam_client-0.2.0/tests/test_indicam_client.py`

 * *Files identical despite different names*

