# Comparing `tmp/beehiiv-0.1b0.tar.gz` & `tmp/beehiiv-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beehiiv-0.1b0.tar", last modified: Thu Jul 27 01:24:36 2023, max compression
+gzip compressed data, was "beehiiv-0.2.tar", last modified: Thu Jul 27 10:21:49 2023, max compression
```

## Comparing `beehiiv-0.1b0.tar` & `beehiiv-0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 bojan     (1000) bojan     (1000)        0 2023-07-27 01:24:36.686013 beehiiv-0.1b0/
--rw-rw-r--   0 bojan     (1000) bojan     (1000)     1065 2023-07-26 00:33:59.000000 beehiiv-0.1b0/LICENSE
--rw-rw-r--   0 bojan     (1000) bojan     (1000)      658 2023-07-27 01:24:36.686013 beehiiv-0.1b0/PKG-INFO
--rw-rw-r--   0 bojan     (1000) bojan     (1000)       41 2023-07-26 23:44:06.000000 beehiiv-0.1b0/README.md
-drwxrwxr-x   0 bojan     (1000) bojan     (1000)        0 2023-07-27 01:24:36.686013 beehiiv-0.1b0/beehiiv/
--rw-rw-r--   0 bojan     (1000) bojan     (1000)      713 2023-07-27 00:51:00.000000 beehiiv-0.1b0/beehiiv/__init__.py
--rw-rw-r--   0 bojan     (1000) bojan     (1000)       22 2023-07-27 01:05:44.000000 beehiiv-0.1b0/beehiiv/__version__.py
--rw-rw-r--   0 bojan     (1000) bojan     (1000)     1445 2023-07-27 00:38:15.000000 beehiiv-0.1b0/beehiiv/email_blasts.py
--rw-rw-r--   0 bojan     (1000) bojan     (1000)      999 2023-07-27 00:35:47.000000 beehiiv-0.1b0/beehiiv/endpoint.py
--rw-rw-r--   0 bojan     (1000) bojan     (1000)     1270 2023-07-27 00:43:02.000000 beehiiv-0.1b0/beehiiv/posts.py
--rw-rw-r--   0 bojan     (1000) bojan     (1000)      715 2023-07-27 00:46:49.000000 beehiiv-0.1b0/beehiiv/publications.py
--rw-rw-r--   0 bojan     (1000) bojan     (1000)      531 2023-07-27 00:50:16.000000 beehiiv-0.1b0/beehiiv/referral_program.py
--rw-rw-r--   0 bojan     (1000) bojan     (1000)     1327 2023-07-27 00:53:26.000000 beehiiv-0.1b0/beehiiv/segments.py
--rw-rw-r--   0 bojan     (1000) bojan     (1000)     2412 2023-07-27 00:40:33.000000 beehiiv-0.1b0/beehiiv/subscriptions.py
-drwxrwxr-x   0 bojan     (1000) bojan     (1000)        0 2023-07-27 01:24:36.686013 beehiiv-0.1b0/beehiiv.egg-info/
--rw-rw-r--   0 bojan     (1000) bojan     (1000)      658 2023-07-27 01:24:36.000000 beehiiv-0.1b0/beehiiv.egg-info/PKG-INFO
--rw-rw-r--   0 bojan     (1000) bojan     (1000)      391 2023-07-27 01:24:36.000000 beehiiv-0.1b0/beehiiv.egg-info/SOURCES.txt
--rw-rw-r--   0 bojan     (1000) bojan     (1000)        1 2023-07-27 01:24:36.000000 beehiiv-0.1b0/beehiiv.egg-info/dependency_links.txt
--rw-rw-r--   0 bojan     (1000) bojan     (1000)        9 2023-07-27 01:24:36.000000 beehiiv-0.1b0/beehiiv.egg-info/requires.txt
--rw-rw-r--   0 bojan     (1000) bojan     (1000)        8 2023-07-27 01:24:36.000000 beehiiv-0.1b0/beehiiv.egg-info/top_level.txt
--rw-rw-r--   0 bojan     (1000) bojan     (1000)      161 2023-07-27 01:24:36.686013 beehiiv-0.1b0/setup.cfg
--rw-rw-r--   0 bojan     (1000) bojan     (1000)      912 2023-07-27 01:23:50.000000 beehiiv-0.1b0/setup.py
+drwxrwxr-x   0 bojan     (1000) bojan     (1000)        0 2023-07-27 10:21:49.967983 beehiiv-0.2/
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)     1065 2023-07-26 00:33:59.000000 beehiiv-0.2/LICENSE
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)     2327 2023-07-27 10:21:49.967983 beehiiv-0.2/PKG-INFO
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)     1713 2023-07-27 10:19:02.000000 beehiiv-0.2/README.md
+drwxrwxr-x   0 bojan     (1000) bojan     (1000)        0 2023-07-27 10:21:49.963983 beehiiv-0.2/beehiiv/
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)      713 2023-07-27 00:51:00.000000 beehiiv-0.2/beehiiv/__init__.py
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)       21 2023-07-27 10:19:17.000000 beehiiv-0.2/beehiiv/__version__.py
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)     2533 2023-07-27 10:05:42.000000 beehiiv-0.2/beehiiv/email_blasts.py
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)     1417 2023-07-27 09:30:27.000000 beehiiv-0.2/beehiiv/endpoint.py
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)     5255 2023-07-27 10:06:30.000000 beehiiv-0.2/beehiiv/posts.py
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)     1882 2023-07-27 10:06:55.000000 beehiiv-0.2/beehiiv/publications.py
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)     1207 2023-07-27 10:07:11.000000 beehiiv-0.2/beehiiv/referral_program.py
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)     3505 2023-07-27 10:08:05.000000 beehiiv-0.2/beehiiv/segments.py
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)     7433 2023-07-27 10:09:20.000000 beehiiv-0.2/beehiiv/subscriptions.py
+drwxrwxr-x   0 bojan     (1000) bojan     (1000)        0 2023-07-27 10:21:49.967983 beehiiv-0.2/beehiiv.egg-info/
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)     2327 2023-07-27 10:21:49.000000 beehiiv-0.2/beehiiv.egg-info/PKG-INFO
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)      391 2023-07-27 10:21:49.000000 beehiiv-0.2/beehiiv.egg-info/SOURCES.txt
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)        1 2023-07-27 10:21:49.000000 beehiiv-0.2/beehiiv.egg-info/dependency_links.txt
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)        9 2023-07-27 10:21:49.000000 beehiiv-0.2/beehiiv.egg-info/requires.txt
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)        8 2023-07-27 10:21:49.000000 beehiiv-0.2/beehiiv.egg-info/top_level.txt
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)      161 2023-07-27 10:21:49.967983 beehiiv-0.2/setup.cfg
+-rw-rw-r--   0 bojan     (1000) bojan     (1000)      911 2023-07-27 10:20:52.000000 beehiiv-0.2/setup.py
```

### Comparing `beehiiv-0.1b0/LICENSE` & `beehiiv-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beehiiv-0.1b0/beehiiv/__init__.py` & `beehiiv-0.2/beehiiv/__init__.py`

 * *Files identical despite different names*

### Comparing `beehiiv-0.1b0/beehiiv/subscriptions.py` & `beehiiv-0.2/beehiiv/publications.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,54 @@
 from beehiiv.endpoint import Endpoint
 
 
-class Subscriptions(Endpoint):
+class Publications(Endpoint):
 
-    def __init__(self, api_key, publicationId):
-        super().__init__(api_key)
-        self.endpoint = "/publications/{}/subscriptions"
-        self.publicationId = publicationId
+    def __init__(self, api_key):
+        '''init
 
-    def create(self, email, reactivate_existing=None, send_welcome_email=None,
-               utm_source=None, utm_medium=None, utm_campaign=None,
-               referring_site=None, referral_code=None, custom_fields=[]):
-        '''create'''
-        return self._make_call(
-            [self.publicationId],
-            data={
-                "email": email,
-                "reactivate_existing": reactivate_existing,
-                "send_welcome_email": send_welcome_email,
-                "utm_source": utm_source,
-                "utm_medium": utm_medium,
-                "utm_campaign": utm_campaign,
-                "referring_site": referring_site,
-                "referral_code": referral_code,
-                "custom_fields": custom_fields,
-            },
-            method="POST",
-        ).json()
+        :param str api_key: BeeHiiv API KEY
+        '''
+        super().__init__(api_key)
+        self.endpoint = "/publications"
 
-    def index(self, email=None, expand=[], limit=None, page=None, status=None,
-              tier=None):
-        '''index'''
+    def index(self, expand=[], limit=None, page=None):
+        '''index
+        Retrieve all publications associated with your API key.
+
+        https://developers.beehiiv.com/docs/v2/f2cc85aaf19cd-index
+
+        :param list expand: Optional list of expandable objects.
+                            Allowed value: [stats]
+                            stats - Returns statistics about the publication(s)
+        :param int limit: A limit on the number of objects to be returned. The limit can range between 1 and 100, and the default is 10.
+                          Default: 10
+        :param int page: Pagination returns the results in pages. Each page contains the number of results specified by the limit (default: 10).
+                         Default: 1
+        '''  # noqa E501
         return self._make_call(
-            [self.publicationId],
+            None,
             params={
-                "email": email,
                 "expand[]": expand,
                 "limit": limit,
                 "page": page,
-                "status": status,
-                "tier": tier,
             },
         ).json()
 
-    def show(self, subscriptionId, expand=[]):
-        '''show'''
+    def show(self, publicationId, expand=[]):
+        '''show
+        Retrieve a single publication
+
+        https://developers.beehiiv.com/docs/v2/d664af2e46883-show
+
+        :param str publicationId: The prefixed ID of the publication object
+        :param list expand: Optional list of expandable objects.
+                            Allowed value: [stats]
+                            stats - Returns statistics about the publication(s)
+        '''
         return self._make_call(
-            [self.publicationId, subscriptionId],
+            [publicationId],
             endpoint=self.endpoint + "/{}",
             params={
                 "expand[]": expand,
             },
         ).json()
-
-    def update(self, subscriptionId, unsubscribe=None, custom_fields=[]):
-        '''update'''
-        return self._make_call(
-            [self.publicationId, subscriptionId],
-            endpoint=self.endpoint + "/{}",
-            data={
-                "unsubscribe": unsubscribe,
-                "custom_fields": custom_fields,
-            },
-            method="PUT",
-        ).json()
-
-    def delete(self, subscriptionId):
-        '''delete'''
-        return self._make_call(
-            [self.publicationId, subscriptionId],
-            endpoint=self.endpoint + "/{}",
-            method="DELETE",
-        ).json()
```

### Comparing `beehiiv-0.1b0/setup.py` & `beehiiv-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description_content_type="text/markdown",
     long_description=readme,
     license='MIT',
     author='abrihter',
     author_email='',
     description='Python wrapper for the BeeHiiv API',
     keywords=['BEEHIIV', 'API', 'WRAPPER'],
-    download_url='https://github.com/abrihter/beehiiv/archive/refs/tags/v0.1b.tar.gz',  # noqa E501
+    download_url='https://github.com/abrihter/beehiiv/archive/refs/tags/v0.2.tar.gz',  # noqa E501
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
```

