# Comparing `tmp/secrets-vault-0.2.0.tar.gz` & `tmp/secrets-vault-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.2.0.tar", last modified: Thu Jul 27 11:32:16 2023, max compression
+gzip compressed data, was "secrets-vault-0.2.1.tar", last modified: Thu Jul 27 12:18:48 2023, max compression
```

## Comparing `secrets-vault-0.2.0.tar` & `secrets-vault-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:32:16.589991 secrets-vault-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-07-27 11:32:16.589991 secrets-vault-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:32:16.589991 secrets-vault-0.2.0/secrets_vault/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/secrets_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/secrets_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/secrets_vault/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/secrets_vault/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/secrets_vault/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/secrets_vault/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/secrets_vault/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:32:16.589991 secrets-vault-0.2.0/secrets_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-07-27 11:32:16.000000 secrets-vault-0.2.0/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-27 11:32:16.000000 secrets-vault-0.2.0/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:32:16.000000 secrets-vault-0.2.0/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 11:32:16.000000 secrets-vault-0.2.0/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 11:32:16.000000 secrets-vault-0.2.0/secrets_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 11:32:16.000000 secrets-vault-0.2.0/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:32:16.589991 secrets-vault-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:32:16.589991 secrets-vault-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/tests/test_backwards_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/tests/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:18:48.814110 secrets-vault-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-27 12:18:48.814110 secrets-vault-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:18:48.814110 secrets-vault-0.2.1/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/secrets_vault/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/secrets_vault/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/secrets_vault/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/secrets_vault/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:18:48.814110 secrets-vault-0.2.1/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-27 12:18:48.000000 secrets-vault-0.2.1/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-27 12:18:48.000000 secrets-vault-0.2.1/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:18:48.000000 secrets-vault-0.2.1/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 12:18:48.000000 secrets-vault-0.2.1/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 12:18:48.000000 secrets-vault-0.2.1/secrets_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 12:18:48.000000 secrets-vault-0.2.1/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:18:48.814110 secrets-vault-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:18:48.814110 secrets-vault-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/tests/test_backwards_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/tests/test_vault.py
```

### Comparing `secrets-vault-0.2.0/LICENSE` & `secrets-vault-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.0/PKG-INFO` & `secrets-vault-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -217,34 +217,57 @@
 ## Printing secrets as environment variables
 
 Sometimes you may want to print a secret as environment variables. It will also apply if you have nested objects. You can do so by running:
 
 ```bash
 $ secrets edit
 
-dev:
-  aws-credentials:
-    AWS_ACCESS_KEY_ID: ..."
-    AWS_SECRET_ACCESS_KEY: ...
+aws-credentials:
+    aws-access-key-id: abc123
+    aws-secret-access-key: abc456
 ```
 
 Get will print the secrets as-is:
 
 ```bash
-$ secrets get dev.aws-credentials
-AWS_ACCESS_KEY_ID: ..."
-AWS_SECRET_ACCESS_KEY: ...
+$ secrets get aws-credentials
+
+aws-access-key-id: abc123
+aws-secret-access-key: abc456
 ```
 
 Envify will print the secrets ready for consumption as environment variables:
 
 ```bash
-$ secrets envify --export dev.aws-credentials
-> export AWS_ACCESS_KEY_ID=...
-> export AWS_SECRET_ACCESS_KEY=...
+$ secrets envify aws-credentials
+
+AWS_ACCESS_KEY_ID=abc123
+AWS_SECRET_ACCESS_KEY=abc456
+```
+
+A few conventions are applied:
+- The key is uppercased
+- Dashes are replaced with underscores
+- Values are serialized as plain-text (eg. strings and numbers) 
+- Objects are JSON encoded (eg. lists and dicts) 
+
+You can then use it in your shell like this:
+
+```bash
+$ $(secrets envify --export aws-credentials)
+$ echo $AWS_ACCESS_KEY_ID
+
+abc123
+```
+
+Or dump multiple secrets to a dotenv file:
+
+```bash
+$ secrets envify aws-credentials >> .env
+$ secrets envify database-url >> .env
 ```
 
 ## Providing the master.key file
 
 ### File on disk
 By default, the vault will look for the master key in a file located at `./master.key`.
```

### Comparing `secrets-vault-0.2.0/README.md` & `secrets-vault-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -202,34 +202,57 @@
 ## Printing secrets as environment variables
 
 Sometimes you may want to print a secret as environment variables. It will also apply if you have nested objects. You can do so by running:
 
 ```bash
 $ secrets edit
 
-dev:
-  aws-credentials:
-    AWS_ACCESS_KEY_ID: ..."
-    AWS_SECRET_ACCESS_KEY: ...
+aws-credentials:
+    aws-access-key-id: abc123
+    aws-secret-access-key: abc456
 ```
 
 Get will print the secrets as-is:
 
 ```bash
-$ secrets get dev.aws-credentials
-AWS_ACCESS_KEY_ID: ..."
-AWS_SECRET_ACCESS_KEY: ...
+$ secrets get aws-credentials
+
+aws-access-key-id: abc123
+aws-secret-access-key: abc456
 ```
 
 Envify will print the secrets ready for consumption as environment variables:
 
 ```bash
-$ secrets envify --export dev.aws-credentials
-> export AWS_ACCESS_KEY_ID=...
-> export AWS_SECRET_ACCESS_KEY=...
+$ secrets envify aws-credentials
+
+AWS_ACCESS_KEY_ID=abc123
+AWS_SECRET_ACCESS_KEY=abc456
+```
+
+A few conventions are applied:
+- The key is uppercased
+- Dashes are replaced with underscores
+- Values are serialized as plain-text (eg. strings and numbers) 
+- Objects are JSON encoded (eg. lists and dicts) 
+
+You can then use it in your shell like this:
+
+```bash
+$ $(secrets envify --export aws-credentials)
+$ echo $AWS_ACCESS_KEY_ID
+
+abc123
+```
+
+Or dump multiple secrets to a dotenv file:
+
+```bash
+$ secrets envify aws-credentials >> .env
+$ secrets envify database-url >> .env
 ```
 
 ## Providing the master.key file
 
 ### File on disk
 By default, the vault will look for the master key in a file located at `./master.key`.
```

### Comparing `secrets-vault-0.2.0/secrets_vault/__main__.py` & `secrets-vault-0.2.1/secrets_vault/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,17 @@
 @cli.command(
     help="Prints a provided secret key as one or more env variables. In case the value is a nested object, it will flatten the key=value pairs."
 )
 @click.argument("key")
 @click.option("--export", is_flag=True, help="Include the export modified for each environment variable.")
 @click.pass_context
 def envify(ctx, key, export):
-    puts = lambda k, v: click.echo(f"{'export ' if export else ''}{k.upper()}={serialize(v, 'dotenv')}")
+    puts = lambda k, v: click.echo(
+        f"{'export ' if export else ''}{k.upper().replace('-', '_')}={serialize(v, 'dotenv')}"
+    )
 
     def handler(vault):
         value = vault.get(key)
         if isinstance(value, dict):
             for k, v in value.items():
                 puts(k, v)
         else:
```

### Comparing `secrets-vault-0.2.0/secrets_vault/backends.py` & `secrets-vault-0.2.1/secrets_vault/backends.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.0/secrets_vault/vault.py` & `secrets-vault-0.2.1/secrets_vault/vault.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.0/secrets_vault.egg-info/PKG-INFO` & `secrets-vault-0.2.1/secrets_vault.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -217,34 +217,57 @@
 ## Printing secrets as environment variables
 
 Sometimes you may want to print a secret as environment variables. It will also apply if you have nested objects. You can do so by running:
 
 ```bash
 $ secrets edit
 
-dev:
-  aws-credentials:
-    AWS_ACCESS_KEY_ID: ..."
-    AWS_SECRET_ACCESS_KEY: ...
+aws-credentials:
+    aws-access-key-id: abc123
+    aws-secret-access-key: abc456
 ```
 
 Get will print the secrets as-is:
 
 ```bash
-$ secrets get dev.aws-credentials
-AWS_ACCESS_KEY_ID: ..."
-AWS_SECRET_ACCESS_KEY: ...
+$ secrets get aws-credentials
+
+aws-access-key-id: abc123
+aws-secret-access-key: abc456
 ```
 
 Envify will print the secrets ready for consumption as environment variables:
 
 ```bash
-$ secrets envify --export dev.aws-credentials
-> export AWS_ACCESS_KEY_ID=...
-> export AWS_SECRET_ACCESS_KEY=...
+$ secrets envify aws-credentials
+
+AWS_ACCESS_KEY_ID=abc123
+AWS_SECRET_ACCESS_KEY=abc456
+```
+
+A few conventions are applied:
+- The key is uppercased
+- Dashes are replaced with underscores
+- Values are serialized as plain-text (eg. strings and numbers) 
+- Objects are JSON encoded (eg. lists and dicts) 
+
+You can then use it in your shell like this:
+
+```bash
+$ $(secrets envify --export aws-credentials)
+$ echo $AWS_ACCESS_KEY_ID
+
+abc123
+```
+
+Or dump multiple secrets to a dotenv file:
+
+```bash
+$ secrets envify aws-credentials >> .env
+$ secrets envify database-url >> .env
 ```
 
 ## Providing the master.key file
 
 ### File on disk
 By default, the vault will look for the master key in a file located at `./master.key`.
```

### Comparing `secrets-vault-0.2.0/setup.py` & `secrets-vault-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.0/tests/test_backends.py` & `secrets-vault-0.2.1/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.0/tests/test_backwards_compat.py` & `secrets-vault-0.2.1/tests/test_backwards_compat.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.0/tests/test_vault.py` & `secrets-vault-0.2.1/tests/test_vault.py`

 * *Files identical despite different names*

