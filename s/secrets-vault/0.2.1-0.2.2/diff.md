# Comparing `tmp/secrets-vault-0.2.1.tar.gz` & `tmp/secrets-vault-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.2.1.tar", last modified: Thu Jul 27 12:18:48 2023, max compression
+gzip compressed data, was "secrets-vault-0.2.2.tar", last modified: Thu Jul 27 12:36:19 2023, max compression
```

## Comparing `secrets-vault-0.2.1.tar` & `secrets-vault-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:18:48.814110 secrets-vault-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-27 12:18:48.814110 secrets-vault-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:18:48.814110 secrets-vault-0.2.1/secrets_vault/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/secrets_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/secrets_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/secrets_vault/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/secrets_vault/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/secrets_vault/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/secrets_vault/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/secrets_vault/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:18:48.814110 secrets-vault-0.2.1/secrets_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-27 12:18:48.000000 secrets-vault-0.2.1/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-27 12:18:48.000000 secrets-vault-0.2.1/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:18:48.000000 secrets-vault-0.2.1/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 12:18:48.000000 secrets-vault-0.2.1/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 12:18:48.000000 secrets-vault-0.2.1/secrets_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 12:18:48.000000 secrets-vault-0.2.1/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:18:48.814110 secrets-vault-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:18:48.814110 secrets-vault-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/tests/test_backwards_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-07-27 12:18:27.000000 secrets-vault-0.2.1/tests/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:36:19.569603 secrets-vault-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-27 12:36:19.569603 secrets-vault-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:36:19.569603 secrets-vault-0.2.2/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/secrets_vault/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/secrets_vault/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/secrets_vault/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/secrets_vault/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:36:19.569603 secrets-vault-0.2.2/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-27 12:36:19.000000 secrets-vault-0.2.2/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-27 12:36:19.000000 secrets-vault-0.2.2/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:36:19.000000 secrets-vault-0.2.2/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 12:36:19.000000 secrets-vault-0.2.2/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 12:36:19.000000 secrets-vault-0.2.2/secrets_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 12:36:19.000000 secrets-vault-0.2.2/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:36:19.569603 secrets-vault-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:36:19.569603 secrets-vault-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/tests/test_backwards_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-27 12:35:49.000000 secrets-vault-0.2.2/tests/test_vault.py
```

### Comparing `secrets-vault-0.2.1/LICENSE` & `secrets-vault-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.1/PKG-INFO` & `secrets-vault-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: secrets-vault
-Version: 0.2.1
-Summary: Simple encrypted secrets for Python
-Home-page: https://github.com/anthonynsimon/secrets-vault
-Author: Anthony N. Simon
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # secrets-vault
 
 Keep your app secrets encrypted in-repo, automatically decrypt on local dev or deploy.
 
 Inspired by Rails credentials - it pairs nicely with [mrsk](https://mrsk.dev). But it can be used as a standalone CLI tool or as a library. 
 
 The vault is YAML encoded and encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
@@ -39,34 +24,34 @@
 3. Edit secrets:
 ```bash
 $ secrets edit
 
 >> Opening secrets file in editor...
 
 # Add your secrets below, comments are supported too.
-# django:
-#     secret_key: abc
+# dev:
+#     secret-key: abc123
 #
-# database_url: supersecret
+# database-url: postgres://user:pass@localhost:5432/dev
 ```
 
 4. Read secrets:
 
 ```bash
 # Via CLI
-$ secrets get database_url
-> supersecret
+$ secrets get database-url
+> postgres://user:pass@localhost:5432/dev
 ```
 
 ```python
 # In Python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault()
-foo = vault.get('database_url')
+foo = vault.get('database-url')
 ```
 
 **Important:** You should keep the `master.key` secret, do NOT commit it. Ignore it in your `.gitignore` file. The `secrets.yml.enc` file is encrypted and can be committed.
 
 ## CLI usage
 
 You can view the help anytime by running `secrets --help`:
@@ -102,56 +87,56 @@
 
 List all secrets:
 
 ```bash
 $ secrets get
 
 # Add your secrets below, comments are supported too.
-# django:
-#     secret_key: abc
+# dev:
+#     secret-key: abc123
 #
-# database_url: supersecret
+# database-url: postgres://user:pass@localhost:5432/dev
 ```
 
 Get a secret:
 
 ```bash
-$ secrets get database_url
-> supersecret
+$ secrets get database-url
+> postgres://user:pass@localhost:5432/dev
 ```
 
 Traverse nested objects:
 
 ```bash
 $ secrets get
 
-django:
- secret_key: abc
+dev:
+ secret-key: abc123
  admins: [zero, one, two three]
 
-database_url: supersecret
+database-url: postgres://user:pass@localhost:5432/dev
 ```
 
 ```bash
-$ secrets get django.admins.2
+$ secrets get dev.admins.2
 
 > two
 ```
 
 
 ### In Python
 
 Simply call `get` with the key. Note that if the secret is missing it will return `None`
 
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault()
 
-admins = vault.get('django.admins')
+admins = vault.get('dev.admins')
 ```
 
 
 ## Editing secrets
 
 ### CLI command
 
@@ -167,18 +152,18 @@
 
 ```bash
 $ secrets edit
 
 >> Opening secrets file in editor...
 
 # Add your secrets below, comments are supported too.
-# django:
-#     secret_key: abc
+# dev:
+#     secret-key: abc123
 #
-# database_url: supersecret
+# database-url: postgres://user:pass@localhost:5432/dev
 ```
 
 Any saved changes will be encrypted and saved to the file on disk when you close the editor.
 
 ### In Python
 
 You can also edit secrets from code:
@@ -220,40 +205,44 @@
 
 ```bash
 $ secrets edit
 
 aws-credentials:
     aws-access-key-id: abc123
     aws-secret-access-key: abc456
+    
+database-url: postgres://user:pass@localhost:5432/dev
 ```
 
-Get will print the secrets as-is:
+Envify will print the secrets ready for consumption as environment variables:
 
 ```bash
-$ secrets get aws-credentials
+$ secrets envify aws-credentials
 
-aws-access-key-id: abc123
-aws-secret-access-key: abc456
+AWS_ACCESS_KEY_ID=abc123
+AWS_SECRET_ACCESS_KEY=abc456
 ```
 
-Envify will print the secrets ready for consumption as environment variables:
+You can also print the entire vault as environment variables:
 
 ```bash
-$ secrets envify aws-credentials
+$ secrets envify
 
-AWS_ACCESS_KEY_ID=abc123
-AWS_SECRET_ACCESS_KEY=abc456
+AWS_CREDENTIALS={"aws-access-key-id": "abc123", "aws-secret-access-key": "abc456"}
+DATABASE_URL=postgres://user:pass@localhost:5432/dev
 ```
 
-A few conventions are applied:
+The following conventions are applied:
 - The key is uppercased
 - Dashes are replaced with underscores
 - Values are serialized as plain-text (eg. strings and numbers) 
 - Objects are JSON encoded (eg. lists and dicts) 
 
+### Consuming the output of envify
+
 You can then use it in your shell like this:
 
 ```bash
 $ $(secrets envify --export aws-credentials)
 $ echo $AWS_ACCESS_KEY_ID
 
 abc123
@@ -338,9 +327,7 @@
 
 Please check for any existing issues before openning a new Issue. If you'd like to work on something, please open a new Issue describing what you'd like to do before submitting a Pull Request.
 
 
 ## License
 
 See [LICENSE](https://github.com/anthonynsimon/secrets-vault/blob/master/LICENSE).
-
-
```

### Comparing `secrets-vault-0.2.1/README.md` & `secrets-vault-0.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: secrets-vault
+Version: 0.2.2
+Summary: Simple encrypted secrets for Python
+Home-page: https://github.com/anthonynsimon/secrets-vault
+Author: Anthony N. Simon
+License: MIT
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # secrets-vault
 
 Keep your app secrets encrypted in-repo, automatically decrypt on local dev or deploy.
 
 Inspired by Rails credentials - it pairs nicely with [mrsk](https://mrsk.dev). But it can be used as a standalone CLI tool or as a library. 
 
 The vault is YAML encoded and encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
@@ -24,34 +39,34 @@
 3. Edit secrets:
 ```bash
 $ secrets edit
 
 >> Opening secrets file in editor...
 
 # Add your secrets below, comments are supported too.
-# django:
-#     secret_key: abc
+# dev:
+#     secret-key: abc123
 #
-# database_url: supersecret
+# database-url: postgres://user:pass@localhost:5432/dev
 ```
 
 4. Read secrets:
 
 ```bash
 # Via CLI
-$ secrets get database_url
-> supersecret
+$ secrets get database-url
+> postgres://user:pass@localhost:5432/dev
 ```
 
 ```python
 # In Python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault()
-foo = vault.get('database_url')
+foo = vault.get('database-url')
 ```
 
 **Important:** You should keep the `master.key` secret, do NOT commit it. Ignore it in your `.gitignore` file. The `secrets.yml.enc` file is encrypted and can be committed.
 
 ## CLI usage
 
 You can view the help anytime by running `secrets --help`:
@@ -87,56 +102,56 @@
 
 List all secrets:
 
 ```bash
 $ secrets get
 
 # Add your secrets below, comments are supported too.
-# django:
-#     secret_key: abc
+# dev:
+#     secret-key: abc123
 #
-# database_url: supersecret
+# database-url: postgres://user:pass@localhost:5432/dev
 ```
 
 Get a secret:
 
 ```bash
-$ secrets get database_url
-> supersecret
+$ secrets get database-url
+> postgres://user:pass@localhost:5432/dev
 ```
 
 Traverse nested objects:
 
 ```bash
 $ secrets get
 
-django:
- secret_key: abc
+dev:
+ secret-key: abc123
  admins: [zero, one, two three]
 
-database_url: supersecret
+database-url: postgres://user:pass@localhost:5432/dev
 ```
 
 ```bash
-$ secrets get django.admins.2
+$ secrets get dev.admins.2
 
 > two
 ```
 
 
 ### In Python
 
 Simply call `get` with the key. Note that if the secret is missing it will return `None`
 
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault()
 
-admins = vault.get('django.admins')
+admins = vault.get('dev.admins')
 ```
 
 
 ## Editing secrets
 
 ### CLI command
 
@@ -152,18 +167,18 @@
 
 ```bash
 $ secrets edit
 
 >> Opening secrets file in editor...
 
 # Add your secrets below, comments are supported too.
-# django:
-#     secret_key: abc
+# dev:
+#     secret-key: abc123
 #
-# database_url: supersecret
+# database-url: postgres://user:pass@localhost:5432/dev
 ```
 
 Any saved changes will be encrypted and saved to the file on disk when you close the editor.
 
 ### In Python
 
 You can also edit secrets from code:
@@ -205,40 +220,44 @@
 
 ```bash
 $ secrets edit
 
 aws-credentials:
     aws-access-key-id: abc123
     aws-secret-access-key: abc456
+    
+database-url: postgres://user:pass@localhost:5432/dev
 ```
 
-Get will print the secrets as-is:
+Envify will print the secrets ready for consumption as environment variables:
 
 ```bash
-$ secrets get aws-credentials
+$ secrets envify aws-credentials
 
-aws-access-key-id: abc123
-aws-secret-access-key: abc456
+AWS_ACCESS_KEY_ID=abc123
+AWS_SECRET_ACCESS_KEY=abc456
 ```
 
-Envify will print the secrets ready for consumption as environment variables:
+You can also print the entire vault as environment variables:
 
 ```bash
-$ secrets envify aws-credentials
+$ secrets envify
 
-AWS_ACCESS_KEY_ID=abc123
-AWS_SECRET_ACCESS_KEY=abc456
+AWS_CREDENTIALS={"aws-access-key-id": "abc123", "aws-secret-access-key": "abc456"}
+DATABASE_URL=postgres://user:pass@localhost:5432/dev
 ```
 
-A few conventions are applied:
+The following conventions are applied:
 - The key is uppercased
 - Dashes are replaced with underscores
 - Values are serialized as plain-text (eg. strings and numbers) 
 - Objects are JSON encoded (eg. lists and dicts) 
 
+### Consuming the output of envify
+
 You can then use it in your shell like this:
 
 ```bash
 $ $(secrets envify --export aws-credentials)
 $ echo $AWS_ACCESS_KEY_ID
 
 abc123
@@ -323,7 +342,9 @@
 
 Please check for any existing issues before openning a new Issue. If you'd like to work on something, please open a new Issue describing what you'd like to do before submitting a Pull Request.
 
 
 ## License
 
 See [LICENSE](https://github.com/anthonynsimon/secrets-vault/blob/master/LICENSE).
+
+
```

### Comparing `secrets-vault-0.2.1/secrets_vault/__main__.py` & `secrets-vault-0.2.2/secrets_vault/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         exceptions.MasterKeyInvalid,
         exceptions.MalformedSecretsFile,
     ) as e:
         click.echo(str(e))
         exit(1)
 
 
-@cli.command(help="Get a secret value. If none are specified, all secrets are printed (eg. `secrets get`).")
+@cli.command(help="Get a secret value. If no specific key is provided, all secrets are printed.")
 @click.argument("key", required=False)
 @click.pass_context
 def get(ctx, key):
     fformat = ctx.obj["format"]
 
     def handler(vault):
         if key:
@@ -125,31 +125,35 @@
 
         click.echo(serialize(result, fformat))
 
     with_vault(ctx, handler)
 
 
 @cli.command(
-    help="Prints a provided secret key as one or more env variables. In case the value is a nested object, it will flatten the key=value pairs."
+    help="Prints a secret as an environment variable (eg. KEY=value). If no specific key is provided, all secrets are printed."
 )
-@click.argument("key")
+@click.argument("key", required=False)
 @click.option("--export", is_flag=True, help="Include the export modified for each environment variable.")
 @click.pass_context
 def envify(ctx, key, export):
     puts = lambda k, v: click.echo(
         f"{'export ' if export else ''}{k.upper().replace('-', '_')}={serialize(v, 'dotenv')}"
     )
 
     def handler(vault):
-        value = vault.get(key)
-        if isinstance(value, dict):
-            for k, v in value.items():
-                puts(k, v)
+        if key:
+            value = vault.get(key)
+            if isinstance(value, dict):
+                for k, v in value.items():
+                    puts(k, v)
+            else:
+                puts(key, value)
         else:
-            puts(key, value)
+            for k, v in vault.secrets.items():
+                puts(k, v)
 
     with_vault(ctx, handler)
 
 
 @cli.command(
     help="Store a secret. If the secret already exists, it will be overwritten. For example: `secrets set foo bar`"
 )
```

### Comparing `secrets-vault-0.2.1/secrets_vault/backends.py` & `secrets-vault-0.2.2/secrets_vault/backends.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.1/secrets_vault/vault.py` & `secrets-vault-0.2.2/secrets_vault/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,19 +176,19 @@
         Path(secrets_filepath).touch()
 
     @classmethod
     def _get_example(cls, file_format):
         if file_format == "json":
             return json.dumps(
                 {
-                    "django": {"secret_key": "abc"},
-                    "database_url": "supersecret",
+                    "app": {"secret-key": "abc123"},
+                    "database-url": "postgres://user:pass@localhost:5432/dev",
                 }
             )
         elif file_format == "yaml":
             return """
 # Add your secrets below, comments are supported too.
-# django:
-#     secret_key: abc
+# app:
+#     secret-key: abc123
 
-database_url: supersecret
+database-url: postgres://user:pass@localhost:5432/dev
 """.strip()
```

### Comparing `secrets-vault-0.2.1/secrets_vault.egg-info/PKG-INFO` & `secrets-vault-0.2.2/secrets_vault.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -39,34 +39,34 @@
 3. Edit secrets:
 ```bash
 $ secrets edit
 
 >> Opening secrets file in editor...
 
 # Add your secrets below, comments are supported too.
-# django:
-#     secret_key: abc
+# dev:
+#     secret-key: abc123
 #
-# database_url: supersecret
+# database-url: postgres://user:pass@localhost:5432/dev
 ```
 
 4. Read secrets:
 
 ```bash
 # Via CLI
-$ secrets get database_url
-> supersecret
+$ secrets get database-url
+> postgres://user:pass@localhost:5432/dev
 ```
 
 ```python
 # In Python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault()
-foo = vault.get('database_url')
+foo = vault.get('database-url')
 ```
 
 **Important:** You should keep the `master.key` secret, do NOT commit it. Ignore it in your `.gitignore` file. The `secrets.yml.enc` file is encrypted and can be committed.
 
 ## CLI usage
 
 You can view the help anytime by running `secrets --help`:
@@ -102,56 +102,56 @@
 
 List all secrets:
 
 ```bash
 $ secrets get
 
 # Add your secrets below, comments are supported too.
-# django:
-#     secret_key: abc
+# dev:
+#     secret-key: abc123
 #
-# database_url: supersecret
+# database-url: postgres://user:pass@localhost:5432/dev
 ```
 
 Get a secret:
 
 ```bash
-$ secrets get database_url
-> supersecret
+$ secrets get database-url
+> postgres://user:pass@localhost:5432/dev
 ```
 
 Traverse nested objects:
 
 ```bash
 $ secrets get
 
-django:
- secret_key: abc
+dev:
+ secret-key: abc123
  admins: [zero, one, two three]
 
-database_url: supersecret
+database-url: postgres://user:pass@localhost:5432/dev
 ```
 
 ```bash
-$ secrets get django.admins.2
+$ secrets get dev.admins.2
 
 > two
 ```
 
 
 ### In Python
 
 Simply call `get` with the key. Note that if the secret is missing it will return `None`
 
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault()
 
-admins = vault.get('django.admins')
+admins = vault.get('dev.admins')
 ```
 
 
 ## Editing secrets
 
 ### CLI command
 
@@ -167,18 +167,18 @@
 
 ```bash
 $ secrets edit
 
 >> Opening secrets file in editor...
 
 # Add your secrets below, comments are supported too.
-# django:
-#     secret_key: abc
+# dev:
+#     secret-key: abc123
 #
-# database_url: supersecret
+# database-url: postgres://user:pass@localhost:5432/dev
 ```
 
 Any saved changes will be encrypted and saved to the file on disk when you close the editor.
 
 ### In Python
 
 You can also edit secrets from code:
@@ -220,40 +220,44 @@
 
 ```bash
 $ secrets edit
 
 aws-credentials:
     aws-access-key-id: abc123
     aws-secret-access-key: abc456
+    
+database-url: postgres://user:pass@localhost:5432/dev
 ```
 
-Get will print the secrets as-is:
+Envify will print the secrets ready for consumption as environment variables:
 
 ```bash
-$ secrets get aws-credentials
+$ secrets envify aws-credentials
 
-aws-access-key-id: abc123
-aws-secret-access-key: abc456
+AWS_ACCESS_KEY_ID=abc123
+AWS_SECRET_ACCESS_KEY=abc456
 ```
 
-Envify will print the secrets ready for consumption as environment variables:
+You can also print the entire vault as environment variables:
 
 ```bash
-$ secrets envify aws-credentials
+$ secrets envify
 
-AWS_ACCESS_KEY_ID=abc123
-AWS_SECRET_ACCESS_KEY=abc456
+AWS_CREDENTIALS={"aws-access-key-id": "abc123", "aws-secret-access-key": "abc456"}
+DATABASE_URL=postgres://user:pass@localhost:5432/dev
 ```
 
-A few conventions are applied:
+The following conventions are applied:
 - The key is uppercased
 - Dashes are replaced with underscores
 - Values are serialized as plain-text (eg. strings and numbers) 
 - Objects are JSON encoded (eg. lists and dicts) 
 
+### Consuming the output of envify
+
 You can then use it in your shell like this:
 
 ```bash
 $ $(secrets envify --export aws-credentials)
 $ echo $AWS_ACCESS_KEY_ID
 
 abc123
```

### Comparing `secrets-vault-0.2.1/setup.py` & `secrets-vault-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.1/tests/test_backends.py` & `secrets-vault-0.2.2/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.1/tests/test_backwards_compat.py` & `secrets-vault-0.2.2/tests/test_backwards_compat.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.1/tests/test_vault.py` & `secrets-vault-0.2.2/tests/test_vault.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     with open(TEST_DATA_DIR / "master-1.key", "rb") as fin:
         assert fin.read().decode() == master_key
 
     vault = SecretsVault(
         secrets_filepath=TEST_DATA_DIR / "secrets-1.yml.enc",
         master_key_filepath=TEST_DATA_DIR / "master-1.key",
     )
-    assert vault.get("database_url") == "supersecret"
+    assert vault.get("database-url") == "postgres://user:pass@localhost:5432/dev"
 
 
 def test_requires_master_key():
     SecretsVault.create(
         secrets_filepath=TEST_DATA_DIR / "secrets-2.yml.enc",
         master_key_filepath=TEST_DATA_DIR / "master-2.key",
     )
@@ -52,15 +52,15 @@
         master_key = fin.read().decode()
         os.environ["MASTER_KEY"] = master_key
 
     vault = SecretsVault(
         secrets_filepath=TEST_DATA_DIR / "secrets-2a.yml.enc",
         master_key_filepath=None,
     )
-    assert vault.get("database_url") == "supersecret"
+    assert vault.get("database-url") == "postgres://user:pass@localhost:5432/dev"
 
     # Cleanup to not affect other tests
     del os.environ["MASTER_KEY"]
 
 
 def test_requires_secrets_file():
     SecretsVault.create(
@@ -85,15 +85,15 @@
     )
 
     vault = SecretsVault(
         secrets_filepath=TEST_DATA_DIR / "secrets-4.yml.enc",
         master_key_filepath=TEST_DATA_DIR / "master-4.key",
     )
 
-    assert vault.get("database_url") == "supersecret"
+    assert vault.get("database-url") == "postgres://user:pass@localhost:5432/dev"
     assert vault.get("hello") is None
     assert vault.get("nested") is None
 
     vault.set("hello", "world")
     vault.set("nested", {"object": "value"})
     vault.save()
 
@@ -108,42 +108,42 @@
         master_key_filepath=TEST_DATA_DIR / "master-4f.key",
     )
 
     # check wrote yaml
     with open(TEST_DATA_DIR / "secrets-4f.yml.enc", "rb") as fin:
         contents = vault.backend.decrypt(fin.read()).decode()
     assert "# Add your secrets below, comments are supported too." in contents
-    assert "database_url: supersecret" in contents
+    assert "database-url: postgres://user:pass@localhost:5432/dev" in contents
 
     # saving preserves format
     vault.set("hello", "world")
     vault.save()
     with open(TEST_DATA_DIR / "secrets-4f.yml.enc", "rb") as fin:
         contents = vault.backend.decrypt(fin.read()).decode()
         assert "# Add your secrets below, comments are supported too." in contents
-        assert "database_url: supersecret" in contents
+        assert "database-url: postgres://user:pass@localhost:5432/dev" in contents
         assert "hello: world" in contents
 
     # can change format
     vault.file_format = "json"
     vault.save()
 
     with open(TEST_DATA_DIR / "secrets-4f.yml.enc", "rb") as fin:
         contents = vault.backend.decrypt(fin.read()).decode()
         assert "# Add your secrets below, comments are supported too." not in contents
-        assert '"database_url": "supersecret"' in contents
+        assert '"database-url": "postgres://user:pass@localhost:5432/dev"' in contents
         assert '"hello": "world"' in contents
 
     # and can read back in new format
     vault = SecretsVault(
         secrets_filepath=TEST_DATA_DIR / "secrets-4f.yml.enc",
         master_key_filepath=TEST_DATA_DIR / "master-4f.key",
         file_format="json",
     )
-    assert vault.get("database_url") == "supersecret"
+    assert vault.get("database-url") == "postgres://user:pass@localhost:5432/dev"
 
 
 def test_large_secrets_file():
     SecretsVault.create(
         secrets_filepath=TEST_DATA_DIR / "secrets-5.yml.enc",
         master_key_filepath=TEST_DATA_DIR / "master-5.key",
     )
```

