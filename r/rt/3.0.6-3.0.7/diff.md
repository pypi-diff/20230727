# Comparing `tmp/rt-3.0.6.tar.gz` & `tmp/rt-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rt-3.0.6.tar", last modified: Wed Jun 21 15:49:00 2023, max compression
+gzip compressed data, was "rt-3.0.7.tar", last modified: Thu Jul 27 21:39:13 2023, max compression
```

## Comparing `rt-3.0.6.tar` & `rt-3.0.7.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:00.058401 rt-3.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-21 15:48:45.000000 rt-3.0.6/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-21 15:48:45.000000 rt-3.0.6/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-06-21 15:48:45.000000 rt-3.0.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-21 15:48:45.000000 rt-3.0.6/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-06-21 15:48:45.000000 rt-3.0.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-21 15:48:45.000000 rt-3.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-21 15:48:45.000000 rt-3.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-06-21 15:49:00.058401 rt-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-06-21 15:48:45.000000 rt-3.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:00.054401 rt-3.0.6/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-06-21 15:48:45.000000 rt-3.0.6/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-21 15:48:45.000000 rt-3.0.6/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-06-21 15:48:45.000000 rt-3.0.6/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-21 15:48:45.000000 rt-3.0.6/doc/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-21 15:48:45.000000 rt-3.0.6/doc/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-21 15:48:45.000000 rt-3.0.6/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 15:48:45.000000 rt-3.0.6/doc/rest1.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 15:48:45.000000 rt-3.0.6/doc/rest2.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-06-21 15:48:45.000000 rt-3.0.6/doc/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-21 15:48:45.000000 rt-3.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:00.054401 rt-3.0.6/rt/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-21 15:48:45.000000 rt-3.0.6/rt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-21 15:48:45.000000 rt-3.0.6/rt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:48:45.000000 rt-3.0.6/rt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64987 2023-06-21 15:48:45.000000 rt-3.0.6/rt/rest1.py
--rw-r--r--   0 runner    (1001) docker     (123)    60728 2023-06-21 15:48:45.000000 rt-3.0.6/rt/rest2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:00.058401 rt-3.0.6/rt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-06-21 15:49:00.000000 rt-3.0.6/rt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-21 15:49:00.000000 rt-3.0.6/rt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:49:00.000000 rt-3.0.6/rt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-21 15:49:00.000000 rt-3.0.6/rt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-21 15:49:00.000000 rt-3.0.6/rt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:49:00.058401 rt-3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 15:48:45.000000 rt-3.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:00.058401 rt-3.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-21 15:48:45.000000 rt-3.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-21 15:48:45.000000 rt-3.0.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-06-21 15:48:45.000000 rt-3.0.6/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-06-21 15:48:45.000000 rt-3.0.6/tests/test_rest1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-21 15:48:45.000000 rt-3.0.6/tests/test_tickets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:13.090179 rt-3.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 21:38:56.000000 rt-3.0.7/.codespell_ignore
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-27 21:38:56.000000 rt-3.0.7/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-27 21:38:56.000000 rt-3.0.7/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-07-27 21:38:56.000000 rt-3.0.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-27 21:38:56.000000 rt-3.0.7/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-27 21:38:56.000000 rt-3.0.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-27 21:38:56.000000 rt-3.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-27 21:38:56.000000 rt-3.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-27 21:39:13.090179 rt-3.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-07-27 21:38:56.000000 rt-3.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:13.086179 rt-3.0.7/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-27 21:38:56.000000 rt-3.0.7/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-27 21:38:56.000000 rt-3.0.7/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-07-27 21:38:56.000000 rt-3.0.7/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-27 21:38:56.000000 rt-3.0.7/doc/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-27 21:38:56.000000 rt-3.0.7/doc/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-27 21:38:56.000000 rt-3.0.7/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-27 21:38:56.000000 rt-3.0.7/doc/rest1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-27 21:38:56.000000 rt-3.0.7/doc/rest2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-07-27 21:38:56.000000 rt-3.0.7/doc/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-27 21:38:56.000000 rt-3.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:13.086179 rt-3.0.7/rt/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-27 21:38:56.000000 rt-3.0.7/rt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 21:38:56.000000 rt-3.0.7/rt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:38:56.000000 rt-3.0.7/rt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64987 2023-07-27 21:38:56.000000 rt-3.0.7/rt/rest1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60883 2023-07-27 21:38:56.000000 rt-3.0.7/rt/rest2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:13.086179 rt-3.0.7/rt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-27 21:39:13.000000 rt-3.0.7/rt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-27 21:39:13.000000 rt-3.0.7/rt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:39:13.000000 rt-3.0.7/rt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-27 21:39:13.000000 rt-3.0.7/rt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-27 21:39:13.000000 rt-3.0.7/rt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:39:13.090179 rt-3.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-27 21:38:56.000000 rt-3.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:39:13.090179 rt-3.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-27 21:38:56.000000 rt-3.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-27 21:38:56.000000 rt-3.0.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-07-27 21:38:56.000000 rt-3.0.7/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-07-27 21:38:56.000000 rt-3.0.7/tests/test_rest1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-27 21:38:56.000000 rt-3.0.7/tests/test_tickets.py
```

### Comparing `rt-3.0.6/.pylintrc` & `rt-3.0.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `rt-3.0.6/CHANGELOG.md` & `rt-3.0.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [v3.0.7], 2023-07-27
+### Fixes
+- Fix sorting when using search() method (#90)
+
 ## [v3.0.6], 2023-06-21
-### Added
+### Fixes
 - Fixed bug in rest1 (#86)
 
 ## [v3.0.5], 2023-02-02
 ### Added
 - Added support for specifying custom fields on user creation/edit (#82).
 
 ## [v3.0.4], 2022-11-08
```

### Comparing `rt-3.0.6/LICENSE` & `rt-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rt-3.0.6/PKG-INFO` & `rt-3.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rt
-Version: 3.0.6
+Version: 3.0.7
 Summary: Python interface to Request Tracker API
 Author-email: Georges Toth <georges.toth@govcert.etat.lu>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/python-rt/python-rt
 Project-URL: Documentation, https://python-rt.readthedocs.io/
 Project-URL: Source, https://github.com/python-rt/python-rt
 Project-URL: Tracker, https://github.com/python-rt/python-rt/issues
```

### Comparing `rt-3.0.6/README.rst` & `rt-3.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `rt-3.0.6/doc/Makefile` & `rt-3.0.7/doc/Makefile`

 * *Files identical despite different names*

### Comparing `rt-3.0.6/doc/changelog.rst` & `rt-3.0.7/doc/changelog.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,28 @@
 Change Log
 ==========
 
+Version 3.0.7 (2023-07-27)
+----------------------------
+Fixes
+^^^^^
+- Fix sorting when using search() method (#90)
+
+Version 3.0.6 (2023-06-21)
+----------------------------
+Fixes
+^^^^^
+- Fixed bug in rest1 (#86)
+
+Version 3.0.5 (2023-02-02)
+----------------------------
+Fixes
+^^^^^
+- Added support for specifying custom fields on user creation/edit (#82).
+
 Version 3.0.4 (2022-11-08)
 ----------------------------
 Fixes
 ^^^^^
 - Workaround for parsing issues with tickets with only 1 attachment (#80), due to probably an upstream bug.
 
 Version 3.0.3 (2022-06-16)
```

### Comparing `rt-3.0.6/doc/conf.py` & `rt-3.0.7/doc/conf.py`

 * *Files identical despite different names*

### Comparing `rt-3.0.6/doc/index.rst` & `rt-3.0.7/doc/index.rst`

 * *Files identical despite different names*

### Comparing `rt-3.0.6/doc/usage.rst` & `rt-3.0.7/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `rt-3.0.6/pyproject.toml` & `rt-3.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rt-3.0.6/rt/exceptions.py` & `rt-3.0.7/rt/exceptions.py`

 * *Files identical despite different names*

### Comparing `rt-3.0.6/rt/rest1.py` & `rt-3.0.7/rt/rest1.py`

 * *Files identical despite different names*

### Comparing `rt-3.0.6/rt/rest2.py` & `rt-3.0.7/rt/rest2.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,15 +510,19 @@
                     query.append(f'{key}{op}\'{value}\'')
                 else:
                     query.append(f'''CF.{{{key[3:]}}}'{op}'{value}\'''')
         else:
             query.append(raw_query)
         get_params['query'] = ' AND '.join('(' + part + ')' for part in query)
         if order:
-            get_params['orderby'] = order
+            if order.startswith("-"):
+                get_params['orderby'] = order[1:]
+                get_params['order'] = "DESC"
+            else:
+                get_params['orderby'] = order
 
         if query_format == 'l':
             get_params['fields'] = 'Owner,Status,Created,Subject,Queue,CustomFields,Requestor,Cc,AdminCc,Started,Created,TimeEstimated,Due,Type,InitialPriority,Priority,TimeLeft,LastUpdated'
             get_params['fields[Queue]'] = 'Name'
         elif query_format == 's':
             get_params['fields'] = 'Subject'
```

### Comparing `rt-3.0.6/rt.egg-info/PKG-INFO` & `rt-3.0.7/rt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rt
-Version: 3.0.6
+Version: 3.0.7
 Summary: Python interface to Request Tracker API
 Author-email: Georges Toth <georges.toth@govcert.etat.lu>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/python-rt/python-rt
 Project-URL: Documentation, https://python-rt.readthedocs.io/
 Project-URL: Source, https://github.com/python-rt/python-rt
 Project-URL: Tracker, https://github.com/python-rt/python-rt/issues
```

### Comparing `rt-3.0.6/rt.egg-info/SOURCES.txt` & `rt-3.0.7/rt.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.codespell_ignore
 .editorconfig
 .flake8
 .pylintrc
 AUTHORS
 CHANGELOG.md
 LICENSE
 MANIFEST.in
```

### Comparing `rt-3.0.6/tests/test_basic.py` & `rt-3.0.7/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `rt-3.0.6/tests/test_rest1.py` & `rt-3.0.7/tests/test_rest1.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     '"Jiri Machalek" <jiri.machalek@nic.cz>'
 ]
 
 import random
 import string
 import unittest
 
+import requests.utils
+
 import rt.rest1
 
 
 class RtTestCase(unittest.TestCase):
     rt.DEBUG_MODE = True
     RT_VALID_CREDENTIALS = {
         'RT4.4 stable': {
@@ -72,23 +74,36 @@
             'default_password': 'idonthavepassword',
         },
     }
 
     def _have_creds(*creds_seq):
         return all(creds[name].get('url') for creds in creds_seq for name in creds)
 
+    @staticmethod
+    def _fix_unsecure_cookie(tracker: rt.rest1.Rt) -> None:
+        """As of RT 5.0.4, cookies returned by the REST API are marked as secure by default.
+
+        This breaks tests though as we are connecting via HTTP. This method fixes these cookies
+        for the tests to work.
+        """
+        cookies = requests.utils.dict_from_cookiejar(tracker.session.cookies)
+        tracker.session.cookies.clear()
+        tracker.session.cookies.update(cookies)
+
     @unittest.skipUnless(_have_creds(RT_VALID_CREDENTIALS,
                                      RT_INVALID_CREDENTIALS,
                                      RT_MISSING_CREDENTIALS,
                                      RT_BAD_URL),
                          "missing credentials required to run test")
     def test_login_and_logout(self):
         for name in self.RT_VALID_CREDENTIALS:
             tracker = rt.rest1.Rt(self.RT_VALID_CREDENTIALS[name]['url'], **self.RT_VALID_CREDENTIALS[name]['support'])
             self.assertTrue(tracker.login(), 'Invalid login to RT demo site ' + name)
+            # unsecure cookie
+            self._fix_unsecure_cookie(tracker)
             self.assertTrue(tracker.logout(), 'Invalid logout from RT demo site ' + name)
         for name, params in self.RT_INVALID_CREDENTIALS.items():
             tracker = rt.rest1.Rt(**params)
             self.assertFalse(tracker.login(), 'Login to RT demo site ' + name + ' should fail but did not')
             self.assertRaises(rt.exceptions.AuthorizationError, lambda: tracker.search())
         for name, params in self.RT_MISSING_CREDENTIALS.items():
             tracker = rt.rest1.Rt(**params)
@@ -104,14 +119,16 @@
         ticket_text = 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.'
         for name in ('RT4.4 stable',):
             url = self.RT_VALID_CREDENTIALS[name]['url']
             default_login = self.RT_VALID_CREDENTIALS[name]['support']['default_login']
             default_password = self.RT_VALID_CREDENTIALS[name]['support']['default_password']
             tracker = rt.rest1.Rt(url, default_login=default_login, default_password=default_password)
             self.assertTrue(tracker.login(), 'Invalid login to RT demo site ' + name)
+            # unsecure cookie
+            self._fix_unsecure_cookie(tracker)
             # empty search result
             search_result = tracker.search(Subject=ticket_subject)
             self.assertEqual(search_result, [], 'Search for ticket with random subject returned non empty list.')
             # create
             ticket_id = tracker.create_ticket(Subject=ticket_subject, Text=ticket_text)
             self.assertTrue(ticket_id > -1, 'Creating ticket failed.')
             # search
@@ -194,14 +211,17 @@
         for name in ('RT4.4 stable',):
             url = self.RT_VALID_CREDENTIALS[name]['url']
             default_login = self.RT_VALID_CREDENTIALS[name]['support']['default_login']
             default_password = self.RT_VALID_CREDENTIALS[name]['support']['default_password']
             tracker = rt.rest1.Rt(url, default_login=default_login, default_password=default_password)
             self.assertTrue(tracker.login(), 'Invalid login to RT demo site ' + name)
 
+            # unsecure cookie
+            self._fix_unsecure_cookie(tracker)
+
             ticket_id = tracker.create_ticket(Subject=ticket_subject, Text=ticket_text)
             self.assertTrue(ticket_id > -1, 'Creating ticket failed.')
 
             # make sure Requestors, AdminCc and Cc are present and an empty list, as would be expected
             ticket = tracker.get_ticket(ticket_id)
             self.assertTrue(len(ticket['Requestors']) >= 0)
             self.assertTrue(len(ticket['AdminCc']) >= 0)
```

### Comparing `rt-3.0.6/tests/test_tickets.py` & `rt-3.0.7/tests/test_tickets.py`

 * *Files identical despite different names*

