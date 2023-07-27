# Comparing `tmp/fastapi_login-1.9.0.tar.gz` & `tmp/fastapi_login-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_login-1.9.0.tar", max compression
+gzip compressed data, was "fastapi_login-1.9.1.tar", max compression
```

## Comparing `fastapi_login-1.9.0.tar` & `fastapi_login-1.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2023-03-27 14:39:21.546024 fastapi_login-1.9.0/LICENSE
--rw-r--r--   0        0        0     4958 2023-03-27 14:39:21.546024 fastapi_login-1.9.0/README.md
--rw-r--r--   0        0        0       68 2023-03-27 14:39:21.550025 fastapi_login-1.9.0/fastapi_login/__init__.py
--rw-r--r--   0        0        0      249 2023-03-27 14:39:21.550025 fastapi_login-1.9.0/fastapi_login/exceptions.py
--rw-r--r--   0        0        0    17000 2023-03-27 14:39:21.550025 fastapi_login-1.9.0/fastapi_login/fastapi_login.py
--rw-r--r--   0        0        0        0 2023-03-27 14:39:21.550025 fastapi_login-1.9.0/fastapi_login/py.typed
--rw-r--r--   0        0        0     2628 2023-03-27 14:39:21.550025 fastapi_login-1.9.0/fastapi_login/secrets.py
--rw-r--r--   0        0        0      642 2023-03-27 14:39:21.550025 fastapi_login-1.9.0/fastapi_login/utils.py
--rw-r--r--   0        0        0     1254 2023-03-27 14:39:21.550025 fastapi_login-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     6002 1970-01-01 00:00:00.000000 fastapi_login-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-27 11:44:06.104906 fastapi_login-1.9.1/LICENSE
+-rw-r--r--   0        0        0     4958 2023-07-27 11:44:06.108906 fastapi_login-1.9.1/README.md
+-rw-r--r--   0        0        0       68 2023-07-27 11:44:06.108906 fastapi_login-1.9.1/fastapi_login/__init__.py
+-rw-r--r--   0        0        0      249 2023-07-27 11:44:06.108906 fastapi_login-1.9.1/fastapi_login/exceptions.py
+-rw-r--r--   0        0        0    17103 2023-07-27 11:44:06.108906 fastapi_login-1.9.1/fastapi_login/fastapi_login.py
+-rw-r--r--   0        0        0        0 2023-07-27 11:44:06.108906 fastapi_login-1.9.1/fastapi_login/py.typed
+-rw-r--r--   0        0        0     2628 2023-07-27 11:44:06.108906 fastapi_login-1.9.1/fastapi_login/secrets.py
+-rw-r--r--   0        0        0      642 2023-07-27 11:44:06.108906 fastapi_login-1.9.1/fastapi_login/utils.py
+-rw-r--r--   0        0        0     1462 2023-07-27 11:44:06.108906 fastapi_login-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5954 1970-01-01 00:00:00.000000 fastapi_login-1.9.1/PKG-INFO
```

### Comparing `fastapi_login-1.9.0/LICENSE` & `fastapi_login-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_login-1.9.0/README.md` & `fastapi_login-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_login-1.9.0/fastapi_login/fastapi_login.py` & `fastapi_login-1.9.1/fastapi_login/fastapi_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 
         """
         if use_cookie is False and use_header is False:
             # TODO: change this to AttributeError
             raise Exception(
                 "use_cookie and use_header are both False one of them needs to be True"
             )
+        if isinstance(secret, str):
+            secret = secret.encode()
 
         self.secret = parse_obj_as(Secret, {"algorithms": algorithm, "secret": secret})
         self._user_callback = None
         self.algorithm = algorithm
         self.pwd_context = CryptContext(schemes=["bcrypt"])
         self.tokenUrl = token_url
         self.oauth_scheme = None
@@ -115,15 +117,15 @@
             PendingDeprecationWarning(
                 "Setting a custom exception this way will be deprecated in future releases. "
                 "Have a look at https://fastapi-login.readthedocs.io/advanced_usage/#exception-handling"
                 "for the updated way."
             )
         )
 
-    def user_loader(self, *args, **kwargs) -> Union[Callable, Awaitable]:
+    def user_loader(self, *args, **kwargs) -> Union[Callable, Callable[..., Awaitable]]:
         """
         This sets the callback to retrieve the user.
         The function should take an unique identifier like an email
         and return the user object or None.
 
         Basic usage:
 
@@ -146,15 +148,15 @@
             args: Positional arguments to pass on to the decorated method
             kwargs: Keyword arguments to pass on to the decorated method
 
         Returns:
             The callback
         """
 
-        def decorator(callback: Union[Callable, Awaitable]):
+        def decorator(callback: Union[Callable, Callable[..., Awaitable]]):
             """
             The actual setter of the load_user callback
             Args:
                 callback (Callable or Awaitable): The callback which returns the user
 
             Returns:
                 Partial of the callback with given args and keyword arguments already set
```

### Comparing `fastapi_login-1.9.0/fastapi_login/secrets.py` & `fastapi_login-1.9.1/fastapi_login/secrets.py`

 * *Files identical despite different names*

### Comparing `fastapi_login-1.9.0/fastapi_login/utils.py` & `fastapi_login-1.9.1/fastapi_login/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_login-1.9.0/PKG-INFO` & `fastapi_login-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: fastapi-login
-Version: 1.9.0
+Version: 1.9.1
 Summary: Flask-Login like package for FastAPI
 Home-page: https://github.com/MushroomMaula/fastapi_login
 License: MIT
 Author: Max Rausch-Dupont
 Author-email: maxrd79@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Provides-Extra: asymmetric
 Requires-Dist: anyio[trio] (>=3.6.2,<4.0.0)
-Requires-Dist: cryptography (>=39.0.1,<40.0.0) ; extra == "asymmetric"
+Requires-Dist: cryptography (>=39.0.1,<42.0.0) ; extra == "asymmetric"
 Requires-Dist: fastapi
 Requires-Dist: passlib[bcrypt]
 Requires-Dist: pyjwt (>=2.4,<3.0)
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
 Project-URL: Documentation, https://fastapi-login.readthedocs.io/
 Description-Content-Type: text/markdown
```

