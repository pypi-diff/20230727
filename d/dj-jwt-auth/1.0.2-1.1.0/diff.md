# Comparing `tmp/dj-jwt-auth-1.0.2.tar.gz` & `tmp/dj-jwt-auth-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-jwt-auth-1.0.2.tar", last modified: Tue Jul  4 08:45:57 2023, max compression
+gzip compressed data, was "dj-jwt-auth-1.1.0.tar", last modified: Thu Jul 27 11:33:33 2023, max compression
```

## Comparing `dj-jwt-auth-1.0.2.tar` & `dj-jwt-auth-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-07-04 08:45:57.008318 dj-jwt-auth-1.0.2/
--rw-r--r--   0 seleznevk (984925890) 1002642239     2720 2023-07-04 08:45:57.008480 dj-jwt-auth-1.0.2/PKG-INFO
--rw-r--r--   0 seleznevk (984925890) 1002642239     1779 2023-06-16 14:04:30.000000 dj-jwt-auth-1.0.2/README.md
-drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-07-04 08:45:57.001358 dj-jwt-auth-1.0.2/dj_jwt_auth.egg-info/
--rw-r--r--   0 seleznevk (984925890) 1002642239     2720 2023-07-04 08:45:56.000000 dj-jwt-auth-1.0.2/dj_jwt_auth.egg-info/PKG-INFO
--rw-r--r--   0 seleznevk (984925890) 1002642239      409 2023-07-04 08:45:56.000000 dj-jwt-auth-1.0.2/dj_jwt_auth.egg-info/SOURCES.txt
--rw-r--r--   0 seleznevk (984925890) 1002642239        1 2023-07-04 08:45:56.000000 dj-jwt-auth-1.0.2/dj_jwt_auth.egg-info/dependency_links.txt
--rw-r--r--   0 seleznevk (984925890) 1002642239       63 2023-07-04 08:45:56.000000 dj-jwt-auth-1.0.2/dj_jwt_auth.egg-info/requires.txt
--rw-r--r--   0 seleznevk (984925890) 1002642239       17 2023-07-04 08:45:56.000000 dj-jwt-auth-1.0.2/dj_jwt_auth.egg-info/top_level.txt
-drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-07-04 08:45:57.005023 dj-jwt-auth-1.0.2/django_jwt/
--rw-r--r--   0 seleznevk (984925890) 1002642239        0 2022-10-13 11:25:09.000000 dj-jwt-auth-1.0.2/django_jwt/__init__.py
--rw-r--r--   0 seleznevk (984925890) 1002642239     1092 2023-06-19 08:56:53.000000 dj-jwt-auth-1.0.2/django_jwt/middleware.py
--rw-r--r--   0 seleznevk (984925890) 1002642239      981 2023-06-19 09:22:31.000000 dj-jwt-auth-1.0.2/django_jwt/settings.py
--rw-r--r--   0 seleznevk (984925890) 1002642239     3508 2023-07-04 08:33:47.000000 dj-jwt-auth-1.0.2/django_jwt/user.py
--rw-r--r--   0 seleznevk (984925890) 1002642239     1482 2023-06-19 08:56:53.000000 dj-jwt-auth-1.0.2/django_jwt/utils.py
--rw-r--r--   0 seleznevk (984925890) 1002642239      200 2022-12-07 14:39:32.000000 dj-jwt-auth-1.0.2/django_jwt/views.py
--rw-r--r--   0 seleznevk (984925890) 1002642239      221 2022-10-24 09:36:12.000000 dj-jwt-auth-1.0.2/pyproject.toml
--rw-r--r--   0 seleznevk (984925890) 1002642239      991 2023-07-04 08:45:57.009206 dj-jwt-auth-1.0.2/setup.cfg
--rw-r--r--   0 seleznevk (984925890) 1002642239       90 2022-10-24 09:36:32.000000 dj-jwt-auth-1.0.2/setup.py
-drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-07-04 08:45:57.007496 dj-jwt-auth-1.0.2/tests/
--rw-r--r--   0 seleznevk (984925890) 1002642239        0 2022-10-13 13:02:24.000000 dj-jwt-auth-1.0.2/tests/__init__.py
--rw-r--r--   0 seleznevk (984925890) 1002642239      251 2023-06-19 08:33:20.000000 dj-jwt-auth-1.0.2/tests/models.py
--rw-r--r--   0 seleznevk (984925890) 1002642239     5123 2023-06-23 16:01:33.000000 dj-jwt-auth-1.0.2/tests/test.py
--rw-r--r--   0 seleznevk (984925890) 1002642239      212 2022-10-14 10:04:40.000000 dj-jwt-auth-1.0.2/tests/urls.py
+drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2023-07-27 11:33:33.051848 dj-jwt-auth-1.1.0/
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     3044 2023-07-27 11:33:33.052090 dj-jwt-auth-1.1.0/PKG-INFO
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     2103 2023-07-26 13:49:02.000000 dj-jwt-auth-1.1.0/README.md
+drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2023-07-27 11:33:33.044595 dj-jwt-auth-1.1.0/dj_jwt_auth.egg-info/
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     3044 2023-07-27 11:33:33.000000 dj-jwt-auth-1.1.0/dj_jwt_auth.egg-info/PKG-INFO
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      409 2023-07-27 11:33:33.000000 dj-jwt-auth-1.1.0/dj_jwt_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        1 2023-07-27 11:33:33.000000 dj-jwt-auth-1.1.0/dj_jwt_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)       63 2023-07-27 11:33:33.000000 dj-jwt-auth-1.1.0/dj_jwt_auth.egg-info/requires.txt
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)       17 2023-07-27 11:33:33.000000 dj-jwt-auth-1.1.0/dj_jwt_auth.egg-info/top_level.txt
+drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2023-07-27 11:33:33.048187 dj-jwt-auth-1.1.0/django_jwt/
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2022-10-13 11:25:09.000000 dj-jwt-auth-1.1.0/django_jwt/__init__.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     1075 2023-07-27 10:46:52.000000 dj-jwt-auth-1.1.0/django_jwt/middleware.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     1049 2023-07-26 13:56:02.000000 dj-jwt-auth-1.1.0/django_jwt/settings.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     3508 2023-07-04 08:33:47.000000 dj-jwt-auth-1.1.0/django_jwt/user.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     1829 2023-07-27 11:15:14.000000 dj-jwt-auth-1.1.0/django_jwt/utils.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      200 2022-12-07 14:39:32.000000 dj-jwt-auth-1.1.0/django_jwt/views.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      221 2022-10-24 09:36:12.000000 dj-jwt-auth-1.1.0/pyproject.toml
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      991 2023-07-27 11:33:33.053076 dj-jwt-auth-1.1.0/setup.cfg
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)       90 2022-10-24 09:36:32.000000 dj-jwt-auth-1.1.0/setup.py
+drwxr-xr-x   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2023-07-27 11:33:33.051094 dj-jwt-auth-1.1.0/tests/
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)        0 2022-10-13 13:02:24.000000 dj-jwt-auth-1.1.0/tests/__init__.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      251 2023-06-19 08:33:20.000000 dj-jwt-auth-1.1.0/tests/models.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)     5123 2023-07-27 10:39:36.000000 dj-jwt-auth-1.1.0/tests/test.py
+-rw-r--r--   0 seleznevk (984925890) SCIENCE\Domain Users (1002642239)      212 2022-10-14 10:04:40.000000 dj-jwt-auth-1.1.0/tests/urls.py
```

### Comparing `dj-jwt-auth-1.0.2/PKG-INFO` & `dj-jwt-auth-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-jwt-auth
-Version: 1.0.2
+Version: 1.1.0
 Summary: A Django package for JSON Web Token validation and verification. Using PyJWT.
 Home-page: https://www.example.com/
 Author: Konstantin Seleznev
 Author-email: k.seleznev@elsevier.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -72,11 +72,18 @@
 ```
 
 - OIDC_USER_ON_CREATE and OIDC_USER_ON_UPDATE - functions to be called on user creation and update, by default:
 ```
     OIDC_USER_ON_CREATE = None
     OIDC_USER_ON_UPDATE = None
 ```
+- OIDC_CONFIG_ROUTES - dict of 'algorithm': 'config_url', by default is empty. If filled will be used instead of OIDC_CERTS_URL
+```
+   OIDC_CONFIG_ROUTES = {
+       'RS256': 'https://keyCloak/realms/h/.well-known/openid-configuration',
+       'HS256': 'https://keyCloak/realms/h/.well-known/openid-configuration',
+   } 
+```
 These functions should accept two arguments: user and request.
 
 ### Testing:
 Run command `python runtests.py` to run tests.
```

### Comparing `dj-jwt-auth-1.0.2/README.md` & `dj-jwt-auth-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -48,11 +48,18 @@
 ```
 
 - OIDC_USER_ON_CREATE and OIDC_USER_ON_UPDATE - functions to be called on user creation and update, by default:
 ```
     OIDC_USER_ON_CREATE = None
     OIDC_USER_ON_UPDATE = None
 ```
+- OIDC_CONFIG_ROUTES - dict of 'algorithm': 'config_url', by default is empty. If filled will be used instead of OIDC_CERTS_URL
+```
+   OIDC_CONFIG_ROUTES = {
+       'RS256': 'https://keyCloak/realms/h/.well-known/openid-configuration',
+       'HS256': 'https://keyCloak/realms/h/.well-known/openid-configuration',
+   } 
+```
 These functions should accept two arguments: user and request.
 
 ### Testing:
 Run command `python runtests.py` to run tests.
```

### Comparing `dj-jwt-auth-1.0.2/dj_jwt_auth.egg-info/PKG-INFO` & `dj-jwt-auth-1.1.0/dj_jwt_auth.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-jwt-auth
-Version: 1.0.2
+Version: 1.1.0
 Summary: A Django package for JSON Web Token validation and verification. Using PyJWT.
 Home-page: https://www.example.com/
 Author: Konstantin Seleznev
 Author-email: k.seleznev@elsevier.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -72,11 +72,18 @@
 ```
 
 - OIDC_USER_ON_CREATE and OIDC_USER_ON_UPDATE - functions to be called on user creation and update, by default:
 ```
     OIDC_USER_ON_CREATE = None
     OIDC_USER_ON_UPDATE = None
 ```
+- OIDC_CONFIG_ROUTES - dict of 'algorithm': 'config_url', by default is empty. If filled will be used instead of OIDC_CERTS_URL
+```
+   OIDC_CONFIG_ROUTES = {
+       'RS256': 'https://keyCloak/realms/h/.well-known/openid-configuration',
+       'HS256': 'https://keyCloak/realms/h/.well-known/openid-configuration',
+   } 
+```
 These functions should accept two arguments: user and request.
 
 ### Testing:
 Run command `python runtests.py` to run tests.
```

### Comparing `dj-jwt-auth-1.0.2/django_jwt/middleware.py` & `dj-jwt-auth-1.1.0/django_jwt/middleware.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,13 @@
         if not auth_header.startswith("Bearer "):
             return
 
         # auth part
         raw_token = auth_header[7:]
         try:
             info = oidc_handler.decode_token(raw_token)
+            request.user = request._cached_user = UserHandler(info, request, raw_token).get_user()
         except ExpiredSignatureError:
             return JsonResponse(status=HTTPStatus.UNAUTHORIZED.value, data={"detail": "expired token"})
         except Exception as exc:
             log.error("Unexpected error", exc)
             return
-
-        # user part
-        request.user = request._cached_user = UserHandler(info, request, raw_token).get_user()
```

### Comparing `dj-jwt-auth-1.0.2/django_jwt/settings.py` & `dj-jwt-auth-1.1.0/django_jwt/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,7 +30,9 @@
     None,
 )
 OIDC_USER_ON_UPDATE = getattr(
     settings,
     "OIDC_USER_ON_UPDATE",
     None,
 )
+
+OIDC_CONFIG_ROUTES = getattr(settings, "OIDC_CONFIG_ROUTES", None)
```

### Comparing `dj-jwt-auth-1.0.2/django_jwt/user.py` & `dj-jwt-auth-1.1.0/django_jwt/user.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.0.2/setup.cfg` & `dj-jwt-auth-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj-jwt-auth
-version = 1.0.2
+version = 1.1.0
 description = A Django package for JSON Web Token validation and verification. Using PyJWT.
 long_description = file: README.md
 url = https://www.example.com/
 author = Konstantin Seleznev
 author_email = k.seleznev@elsevier.com
 license = MIT
 classifiers =
```

### Comparing `dj-jwt-auth-1.0.2/tests/test.py` & `dj-jwt-auth-1.1.0/tests/test.py`

 * *Files identical despite different names*

