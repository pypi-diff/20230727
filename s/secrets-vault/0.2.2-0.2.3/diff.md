# Comparing `tmp/secrets-vault-0.2.2.tar.gz` & `tmp/secrets-vault-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.2.2.tar", last modified: Thu Jul 27 12:36:19 2023, max compression
+gzip compressed data, was "secrets-vault-0.2.3.tar", last modified: Thu Jul 27 14:25:14 2023, max compression
```

## Comparing `secrets-vault-0.2.2.tar` & `secrets-vault-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:36:19.569603 secrets-vault-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-27 12:36:19.569603 secrets-vault-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:36:19.569603 secrets-vault-0.2.2/secrets_vault/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/secrets_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/secrets_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/secrets_vault/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/secrets_vault/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/secrets_vault/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/secrets_vault/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/secrets_vault/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:36:19.569603 secrets-vault-0.2.2/secrets_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-27 12:36:19.000000 secrets-vault-0.2.2/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-27 12:36:19.000000 secrets-vault-0.2.2/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:36:19.000000 secrets-vault-0.2.2/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 12:36:19.000000 secrets-vault-0.2.2/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 12:36:19.000000 secrets-vault-0.2.2/secrets_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 12:36:19.000000 secrets-vault-0.2.2/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:36:19.569603 secrets-vault-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:36:19.569603 secrets-vault-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/tests/test_backwards_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/tests/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:25:14.695639 secrets-vault-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-27 14:25:14.695639 secrets-vault-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:25:14.691639 secrets-vault-0.2.3/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/secrets_vault/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/secrets_vault/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/secrets_vault/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/secrets_vault/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:25:14.691639 secrets-vault-0.2.3/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-27 14:25:14.000000 secrets-vault-0.2.3/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-27 14:25:14.000000 secrets-vault-0.2.3/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:25:14.000000 secrets-vault-0.2.3/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:25:14.000000 secrets-vault-0.2.3/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 14:25:14.000000 secrets-vault-0.2.3/secrets_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 14:25:14.000000 secrets-vault-0.2.3/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:25:14.695639 secrets-vault-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:25:14.695639 secrets-vault-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/tests/test_backwards_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-27 14:24:48.000000 secrets-vault-0.2.3/tests/test_vault.py
```

### Comparing `secrets-vault-0.2.2/LICENSE` & `secrets-vault-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.2/PKG-INFO` & `secrets-vault-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `secrets-vault-0.2.2/README.md` & `secrets-vault-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.2/secrets_vault/__main__.py` & `secrets-vault-0.2.3/secrets_vault/__main__.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.2/secrets_vault/backends.py` & `secrets-vault-0.2.3/secrets_vault/backends.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.2/secrets_vault/vault.py` & `secrets-vault-0.2.3/secrets_vault/vault.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,41 +2,30 @@
 import logging
 import os
 import subprocess
 import tempfile
 from io import BytesIO
 from pathlib import Path
 
-from ruamel.yaml import YAML
 import pydash
-from secrets_vault.backends import AES256GCMBackend
-from secrets_vault.constants import (
-    DEFAULT_MASTER_KEY_FILEPATH,
-    DEFAULT_SECRETS_FILEPATH,
-    DEFAULT_FILE_FORMAT,
-    UNSET,
-)
-from secrets_vault.exceptions import (
-    MasterKeyNotFound,
-    SecretsFileNotFound,
-    SecretsFileAlreadyExists,
-    MalformedSecretsFile,
-)
+from ruamel.yaml import YAML
+
+from secrets_vault import exceptions, constants
 
 log = logging.getLogger(__name__)
 
 
 class SecretsVault:
     def __init__(
         self,
         master_key=None,
-        secrets_filepath=DEFAULT_SECRETS_FILEPATH,
-        master_key_filepath=DEFAULT_MASTER_KEY_FILEPATH,
-        backend=AES256GCMBackend,
-        file_format=DEFAULT_FILE_FORMAT,
+        secrets_filepath=constants.DEFAULT_SECRETS_FILEPATH,
+        master_key_filepath=constants.DEFAULT_MASTER_KEY_FILEPATH,
+        backend=constants.DEFAULT_BACKEND,
+        file_format=constants.DEFAULT_FILE_FORMAT,
     ):
         assert file_format in {"yaml", "json"}, "Format must be either 'yaml' or 'json'"
         self.file_format = file_format
 
         if master_key is None:
             self.master_key = self._load_master_key(master_key_filepath)
         else:
@@ -45,18 +34,18 @@
         self.backend = backend(self.master_key)
         self.secrets = dict()
         self.load()
 
     @classmethod
     def create(
         cls,
-        secrets_filepath=DEFAULT_SECRETS_FILEPATH,
-        master_key_filepath=DEFAULT_MASTER_KEY_FILEPATH,
-        backend=AES256GCMBackend,
-        file_format=DEFAULT_FILE_FORMAT,
+        secrets_filepath=constants.DEFAULT_SECRETS_FILEPATH,
+        master_key_filepath=constants.DEFAULT_MASTER_KEY_FILEPATH,
+        backend=constants.AES256GCMBackend,
+        file_format=constants.DEFAULT_FILE_FORMAT,
     ):
         """
         Create a new secrets file and returns the master key - keep it safe!
         """
         cls._prepare_dirs(master_key_filepath, secrets_filepath)
 
         master_key = backend.generate_master_key()
@@ -69,16 +58,16 @@
 
         vault.secrets = vault._deserialize(example.encode())
         vault.save()
 
         return vault, master_key
 
     def require(self, key):
-        value = self.get(key, default=UNSET)
-        if value == UNSET:
+        value = self.get(key, default=constants.UNSET)
+        if value == constants.UNSET:
             raise KeyError(f"Secret {key} not found in secrets vault")
         return value
 
     def get(self, key, default=None):
         return pydash.get(self.secrets, key, default)
 
     def set(self, key, value):
@@ -106,45 +95,49 @@
             if status != 0:
                 raise RuntimeError("Editor returned non-zero status code")
 
             with open(filename, "rb") as fin:
                 try:
                     newsecrets = self._deserialize(fin.read())
                 except Exception as e:
-                    raise MalformedSecretsFile(f"Could not parse secrets file: {e}")
+                    raise exceptions.MalformedSecretsFile(f"Could not parse secrets file: {e}")
+
+            if self._serialize(newsecrets) == self._serialize(self.secrets):
+                log.info("No changes detected")
+                return
 
             self.secrets = newsecrets
             self.save()
         finally:
             os.remove(filename)
 
     def save(self):
         with open(self.secrets_filename, "wb") as fout:
             fout.write(self.backend.encrypt(self._serialize(self.secrets)))
         log.info(f"Wrote encrypted secrets to {self.secrets_filename}")
 
     def load(self):
         log.info(f"Loading encrypted secrets from {self.secrets_filename}")
         if not os.path.exists(self.secrets_filename):
-            raise SecretsFileNotFound(f"Could not find secrets file {self.secrets_filename}")
+            raise exceptions.SecretsFileNotFound(f"Could not find secrets file {self.secrets_filename}")
         with open(self.secrets_filename, "rb") as fin:
             contents = fin.read()
             if contents:
                 self.secrets = self._deserialize(self.backend.decrypt(contents))
             else:
                 self.secrets = dict()
 
     @staticmethod
     def _load_master_key(master_key_filepath=None) -> str:
         master_key = os.environ.get("MASTER_KEY")
         if not master_key and master_key_filepath and os.path.exists(master_key_filepath):
             with open(Path(master_key_filepath).absolute(), "r") as fin:
                 master_key = fin.read().strip()
         if not master_key:
-            raise MasterKeyNotFound(
+            raise exceptions.MasterKeyNotFound(
                 "Could not find encryption master key. "
                 f"Set it as an environment variable 'MASTER_KEY', or in a file '{master_key_filepath}'"
             )
         return master_key
 
     def _deserialize(self, data: bytes) -> dict:
         if self.file_format in {"yaml", "json"}:
@@ -165,30 +158,19 @@
             return result
 
         raise NotImplementedError(f"Unknown file_format {self.file_format}")
 
     @classmethod
     def _prepare_dirs(cls, master_key_filepath, secrets_filepath):
         if Path(secrets_filepath).exists():
-            raise SecretsFileAlreadyExists(f"Secrets file {secrets_filepath} already exists")
+            raise exceptions.SecretsFileAlreadyExists(f"Secrets file {secrets_filepath} already exists")
         log.info(f"Creating new secrets file {secrets_filepath}")
         Path(master_key_filepath).parent.mkdir(parents=True, exist_ok=True)
         Path(secrets_filepath).parent.mkdir(parents=True, exist_ok=True)
         Path(secrets_filepath).touch()
 
     @classmethod
     def _get_example(cls, file_format):
         if file_format == "json":
-            return json.dumps(
-                {
-                    "app": {"secret-key": "abc123"},
-                    "database-url": "postgres://user:pass@localhost:5432/dev",
-                }
-            )
+            return constants.EXAMPLE_SECRETS_JSON
         elif file_format == "yaml":
-            return """
-# Add your secrets below, comments are supported too.
-# app:
-#     secret-key: abc123
-
-database-url: postgres://user:pass@localhost:5432/dev
-""".strip()
+            return constants.EXAMPLE_SECRETS_YAML
```

### Comparing `secrets-vault-0.2.2/secrets_vault.egg-info/PKG-INFO` & `secrets-vault-0.2.3/secrets_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `secrets-vault-0.2.2/setup.py` & `secrets-vault-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.2/tests/test_backends.py` & `secrets-vault-0.2.3/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.2/tests/test_backwards_compat.py` & `secrets-vault-0.2.3/tests/test_backwards_compat.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.2/tests/test_vault.py` & `secrets-vault-0.2.3/tests/test_vault.py`

 * *Files identical despite different names*

