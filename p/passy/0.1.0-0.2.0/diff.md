# Comparing `tmp/passy-0.1.0.tar.gz` & `tmp/passy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passy-0.1.0.tar", last modified: Thu Jul 27 15:55:48 2023, max compression
+gzip compressed data, was "passy-0.2.0.tar", last modified: Thu Jul 27 16:04:25 2023, max compression
```

## Comparing `passy-0.1.0.tar` & `passy-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3078 2023-04-15 14:30:30.500826 passy-0.1.0/.gitignore
--rw-r--r--   0        0        0    18090 2023-05-15 13:04:52.553780 passy-0.1.0/LICENSE
--rw-r--r--   0        0        0      214 2023-05-15 12:44:31.225932 passy-0.1.0/README.md
--rw-r--r--   0        0        0       44 2023-07-27 14:11:19.271144 passy-0.1.0/passy/__init__.py
--rw-r--r--   0        0        0     1511 2023-07-27 14:09:48.204792 passy-0.1.0/passy/otp.py
--rw-r--r--   0        0        0     1611 2023-07-27 15:29:27.537453 passy-0.1.0/passy/passy.py
--rw-r--r--   0        0        0      904 2023-07-27 15:55:22.393150 passy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      208 2023-05-16 21:48:12.866622 passy-0.1.0/test.py
--rw-r--r--   0        0        0      175 2023-07-27 15:15:56.940391 passy-0.1.0/tests/test_2fa.py
--rw-r--r--   0        0        0      575 2023-07-27 15:21:04.634404 passy-0.1.0/tests/test_auth.py
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 passy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-04-15 14:30:30.500826 passy-0.2.0/.gitignore
+-rw-r--r--   0        0        0    18090 2023-05-15 13:04:52.553780 passy-0.2.0/LICENSE
+-rw-r--r--   0        0        0      214 2023-05-15 12:44:31.225932 passy-0.2.0/README.md
+-rw-r--r--   0        0        0       44 2023-07-27 14:11:19.271144 passy-0.2.0/passy/__init__.py
+-rw-r--r--   0        0        0     1511 2023-07-27 14:09:48.204792 passy-0.2.0/passy/otp.py
+-rw-r--r--   0        0        0     1627 2023-07-27 16:02:33.751941 passy-0.2.0/passy/passy.py
+-rw-r--r--   0        0        0      904 2023-07-27 16:03:07.544783 passy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      208 2023-05-16 21:48:12.866622 passy-0.2.0/test.py
+-rw-r--r--   0        0        0      175 2023-07-27 15:15:56.940391 passy-0.2.0/tests/test_2fa.py
+-rw-r--r--   0        0        0      575 2023-07-27 15:21:04.634404 passy-0.2.0/tests/test_auth.py
+-rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 passy-0.2.0/PKG-INFO
```

### Comparing `passy-0.1.0/.gitignore` & `passy-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `passy-0.1.0/LICENSE` & `passy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `passy-0.1.0/passy/otp.py` & `passy-0.2.0/passy/otp.py`

 * *Files identical despite different names*

### Comparing `passy-0.1.0/passy/passy.py` & `passy-0.2.0/passy/passy.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,16 @@
         success = argon2.verify(password, self._password_hash)
         if self._otp is None:
             raise OTPNeeded()
 
         return success
 
 
-    def loads(self, data: str) -> Self:
+    @classmethod
+    def loads(cls, data: str) -> Self:
         decoded = json.loads(b64decode(data))
         password_hash = decoded['password_hash']
         if "otp" in decoded:
             otp = OTP.loads(decoded["otp"])
         else:
             otp = None
```

### Comparing `passy-0.1.0/pyproject.toml` & `passy-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.8.0,<4"]
 
 [project]
 name = "passy"
-version = "0.1.0"
+version = "0.2.0"
 description = "Logins made simple"
 license = {file = "LICENSE"}
 authors = [
     {name = "Ben Brady", email = "benbradybusiness@gmail.com"},
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `passy-0.1.0/tests/test_auth.py` & `passy-0.2.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `passy-0.1.0/PKG-INFO` & `passy-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passy
-Version: 0.1.0
+Version: 0.2.0
 Summary: Logins made simple
 Author-email: Ben Brady <benbradybusiness@gmail.com>
 Requires-Python: >=3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

