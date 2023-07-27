# Comparing `tmp/secrets-vault-0.1.9.tar.gz` & `tmp/secrets-vault-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.1.9.tar", last modified: Fri Jul 21 14:45:22 2023, max compression
+gzip compressed data, was "secrets-vault-0.2.0.tar", last modified: Thu Jul 27 11:32:16 2023, max compression
```

## Comparing `secrets-vault-0.1.9.tar` & `secrets-vault-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:45:22.294222 secrets-vault-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-07-21 14:45:22.294222 secrets-vault-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:45:22.294222 secrets-vault-0.1.9/secrets_vault/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/secrets_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/secrets_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/secrets_vault/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/secrets_vault/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/secrets_vault/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/secrets_vault/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/secrets_vault/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:45:22.294222 secrets-vault-0.1.9/secrets_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-07-21 14:45:22.000000 secrets-vault-0.1.9/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-21 14:45:22.000000 secrets-vault-0.1.9/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:45:22.000000 secrets-vault-0.1.9/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-21 14:45:22.000000 secrets-vault-0.1.9/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 14:45:22.000000 secrets-vault-0.1.9/secrets_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 14:45:22.000000 secrets-vault-0.1.9/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 14:45:22.294222 secrets-vault-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:45:22.294222 secrets-vault-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/tests/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:32:16.589991 secrets-vault-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-07-27 11:32:16.589991 secrets-vault-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:32:16.589991 secrets-vault-0.2.0/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/secrets_vault/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/secrets_vault/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/secrets_vault/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/secrets_vault/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:32:16.589991 secrets-vault-0.2.0/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-07-27 11:32:16.000000 secrets-vault-0.2.0/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-27 11:32:16.000000 secrets-vault-0.2.0/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:32:16.000000 secrets-vault-0.2.0/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 11:32:16.000000 secrets-vault-0.2.0/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 11:32:16.000000 secrets-vault-0.2.0/secrets_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 11:32:16.000000 secrets-vault-0.2.0/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:32:16.589991 secrets-vault-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:32:16.589991 secrets-vault-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/tests/test_backwards_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-07-27 11:31:51.000000 secrets-vault-0.2.0/tests/test_vault.py
```

### Comparing `secrets-vault-0.1.9/LICENSE` & `secrets-vault-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.9/PKG-INFO` & `secrets-vault-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,114 +1,142 @@
-Metadata-Version: 2.1
-Name: secrets-vault
-Version: 0.1.9
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
 
-Simple encrypted secrets for Python.
+Keep your app secrets encrypted in-repo, automatically decrypt on local dev or deploy.
 
-Inspired by Rails encrypted secrets. It can be used as a standalone CLI tool or as a library. 
+Inspired by Rails credentials - it pairs nicely with [mrsk](https://mrsk.dev). But it can be used as a standalone CLI tool or as a library. 
 
-The vault is JSON encoded and encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
+The vault is YAML encoded and encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
 
 ## Quick start
 
-> **Important:** You should keep the `master.key` secret. Ignore it in your `.gitignore` file. The `secrets.json.enc` file is safe to commit.
+1. Install it:
+```bash
+$ pip install secrets-vault
+```
 
-1. Install `pip install secrets-vault`.
-2. Run init:
-    ```bash
-    $ secrets init
-    Generated new secrets vault at ./secrets.json.enc
-    Generated new master key at ./master.key - keep it safe!
-    ``` 
-3. You can now edit your secrets:
-   ```bash
-    $ secrets edit
-   
-    >> Opening secrets file in editor...
-    {
-      "foo": "bar"
-    }
-    ```
+2. Create a new vault:
+ ```bash
+$ secrets init
 
+Generated new secrets vault at ./secrets.yml.enc
+Generated new master key at ./master.key - keep it safe!
+ ``` 
+
+3. Edit secrets:
+```bash
+$ secrets edit
+
+>> Opening secrets file in editor...
+
+# Add your secrets below, comments are supported too.
+# django:
+#     secret_key: abc
+#
+# database_url: supersecret
+```
+
+4. Read secrets:
+
+```bash
+# Via CLI
+$ secrets get database_url
+> supersecret
+```
+
+```python
+# In Python
+from secrets_vault import SecretsVault
+
+vault = SecretsVault()
+foo = vault.get('database_url')
+```
+
+**Important:** You should keep the `master.key` secret, do NOT commit it. Ignore it in your `.gitignore` file. The `secrets.yml.enc` file is encrypted and can be committed.
 
 ## CLI usage
 
 You can view the help anytime by running `secrets --help`:
 
 ```
 Usage: secrets [OPTIONS] COMMAND [ARGS]...
 
   Manage a local secrets vault.
 
 Options:
   -s, --secrets-filepath TEXT     Path to the encrypted secrets vault.
-  -m, --master-key-filepath TEXT  Path to the master.key file.
+                                  [default: ./secrets.yml.enc]
+  -m, --master-key-filepath TEXT  Path to the master.key file.  [default:
+                                  ./master.key]
+  -f, --format [yaml|json]        Format to use for the secrets vault.
+                                  [default: yaml]
+  -v, --verbose                   Enable verbose output.
   --help                          Show this message and exit.
 
 Commands:
   del      Delete a secret.
   edit     Open the secrets vault in your configured $EDITOR.
   envify   Prints a provided secret key as one or more env variables.
-  get      Get one or more secret values.
+  get      Get a secret value.
   init     Generate a new secrets vault and master.key pair.
   set      Store a secret.
   version  Show the package version.
 ```
 
 ## Reading secrets
 
 ### CLI commands
 
 List all secrets:
 
 ```bash
 $ secrets get
-> my-user: foo
-> my-password: supersecret
+
+# Add your secrets below, comments are supported too.
+# django:
+#     secret_key: abc
+#
+# database_url: supersecret
 ```
 
-Get one secret:
+Get a secret:
 
 ```bash
-$ secrets get my-password
+$ secrets get database_url
 > supersecret
 ```
 
-Get multiple secrets:
+Traverse nested objects:
+
+```bash
+$ secrets get
+
+django:
+ secret_key: abc
+ admins: [zero, one, two three]
+
+database_url: supersecret
+```
 
 ```bash
-$ secrets get my-user my-password
-> my-user: foo
-> my-password: supersecret
+$ secrets get django.admins.2
+
+> two
 ```
 
 
 ### In Python
 
 Simply call `get` with the key. Note that if the secret is missing it will return `None`
 
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault()
 
-password = vault.get('my-password')
+admins = vault.get('django.admins')
 ```
 
 
 ## Editing secrets
 
 ### CLI command
 
@@ -122,17 +150,20 @@
 
 To edit secrets, run `secrets edit`, the file will be decrypted and your editor will open.
 
 ```bash
 $ secrets edit
 
 >> Opening secrets file in editor...
-{
-  "foo": "bar"
-}
+
+# Add your secrets below, comments are supported too.
+# django:
+#     secret_key: abc
+#
+# database_url: supersecret
 ```
 
 Any saved changes will be encrypted and saved to the file on disk when you close the editor.
 
 ### In Python
 
 You can also edit secrets from code:
@@ -171,35 +202,34 @@
 ## Printing secrets as environment variables
 
 Sometimes you may want to print a secret as environment variables. It will also apply if you have nested objects. You can do so by running:
 
 ```bash
 $ secrets edit
 
-{
-  "aws-credentials": {
-    "AWS_ACCESS_KEY_ID": "...",
-    "AWS_SECRET_ACCESS_KEY": "..."
-  }
-}
+dev:
+  aws-credentials:
+    AWS_ACCESS_KEY_ID: ..."
+    AWS_SECRET_ACCESS_KEY: ...
 ```
 
 Get will print the secrets as-is:
 
 ```bash
-$ secrets get aws-credentials
-> {"AWS_ACCESS_KEY_ID": "...", "AWS_SECRET_ACCESS_KEY": "..."}
+$ secrets get dev.aws-credentials
+AWS_ACCESS_KEY_ID: ..."
+AWS_SECRET_ACCESS_KEY: ...
 ```
 
 Envify will print the secrets ready for consumption as environment variables:
 
 ```bash
-$ secrets envify aws-credentials
-> AWS_ACCESS_KEY_ID=...
-> AWS_SECRET_ACCESS_KEY=...
+$ secrets envify --export dev.aws-credentials
+> export AWS_ACCESS_KEY_ID=...
+> export AWS_SECRET_ACCESS_KEY=...
 ```
 
 ## Providing the master.key file
 
 ### File on disk
 By default, the vault will look for the master key in a file located at `./master.key`.
 
@@ -236,23 +266,23 @@
 ### CLI command
 
 You can also provide them as a CLI arguments before the command:
 
 ```bash
 $ secrets \
   --master-key-filepath ./prod/master.key \
-  --secrets-filepath ./prod/secrets.json.enc \
+  --secrets-filepath ./prod/secrets.yml.enc \
   init
 ```
 
 This can be used to separate your secrets by environments such as `prod`, `staging`, `dev`, each having with their own key.
 
 ### In Python
 
-You can also configure the filepaths at which your `secrets.json.enc` and `master.key` files are located.
+You can also configure the filepaths at which your `secrets.yml.enc` and `master.key` files are located.
 
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
@@ -270,9 +300,7 @@
 
 Please check for any existing issues before openning a new Issue. If you'd like to work on something, please open a new Issue describing what you'd like to do before submitting a Pull Request.
 
 
 ## License
 
 See [LICENSE](https://github.com/anthonynsimon/secrets-vault/blob/master/LICENSE).
-
-
```

### Comparing `secrets-vault-0.1.9/README.md` & `secrets-vault-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,99 +1,157 @@
+Metadata-Version: 2.1
+Name: secrets-vault
+Version: 0.2.0
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
 
-Simple encrypted secrets for Python.
+Keep your app secrets encrypted in-repo, automatically decrypt on local dev or deploy.
 
-Inspired by Rails encrypted secrets. It can be used as a standalone CLI tool or as a library. 
+Inspired by Rails credentials - it pairs nicely with [mrsk](https://mrsk.dev). But it can be used as a standalone CLI tool or as a library. 
 
-The vault is JSON encoded and encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
+The vault is YAML encoded and encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
 
 ## Quick start
 
-> **Important:** You should keep the `master.key` secret. Ignore it in your `.gitignore` file. The `secrets.json.enc` file is safe to commit.
+1. Install it:
+```bash
+$ pip install secrets-vault
+```
 
-1. Install `pip install secrets-vault`.
-2. Run init:
-    ```bash
-    $ secrets init
-    Generated new secrets vault at ./secrets.json.enc
-    Generated new master key at ./master.key - keep it safe!
-    ``` 
-3. You can now edit your secrets:
-   ```bash
-    $ secrets edit
-   
-    >> Opening secrets file in editor...
-    {
-      "foo": "bar"
-    }
-    ```
+2. Create a new vault:
+ ```bash
+$ secrets init
 
+Generated new secrets vault at ./secrets.yml.enc
+Generated new master key at ./master.key - keep it safe!
+ ``` 
+
+3. Edit secrets:
+```bash
+$ secrets edit
+
+>> Opening secrets file in editor...
+
+# Add your secrets below, comments are supported too.
+# django:
+#     secret_key: abc
+#
+# database_url: supersecret
+```
+
+4. Read secrets:
+
+```bash
+# Via CLI
+$ secrets get database_url
+> supersecret
+```
+
+```python
+# In Python
+from secrets_vault import SecretsVault
+
+vault = SecretsVault()
+foo = vault.get('database_url')
+```
+
+**Important:** You should keep the `master.key` secret, do NOT commit it. Ignore it in your `.gitignore` file. The `secrets.yml.enc` file is encrypted and can be committed.
 
 ## CLI usage
 
 You can view the help anytime by running `secrets --help`:
 
 ```
 Usage: secrets [OPTIONS] COMMAND [ARGS]...
 
   Manage a local secrets vault.
 
 Options:
   -s, --secrets-filepath TEXT     Path to the encrypted secrets vault.
-  -m, --master-key-filepath TEXT  Path to the master.key file.
+                                  [default: ./secrets.yml.enc]
+  -m, --master-key-filepath TEXT  Path to the master.key file.  [default:
+                                  ./master.key]
+  -f, --format [yaml|json]        Format to use for the secrets vault.
+                                  [default: yaml]
+  -v, --verbose                   Enable verbose output.
   --help                          Show this message and exit.
 
 Commands:
   del      Delete a secret.
   edit     Open the secrets vault in your configured $EDITOR.
   envify   Prints a provided secret key as one or more env variables.
-  get      Get one or more secret values.
+  get      Get a secret value.
   init     Generate a new secrets vault and master.key pair.
   set      Store a secret.
   version  Show the package version.
 ```
 
 ## Reading secrets
 
 ### CLI commands
 
 List all secrets:
 
 ```bash
 $ secrets get
-> my-user: foo
-> my-password: supersecret
+
+# Add your secrets below, comments are supported too.
+# django:
+#     secret_key: abc
+#
+# database_url: supersecret
 ```
 
-Get one secret:
+Get a secret:
 
 ```bash
-$ secrets get my-password
+$ secrets get database_url
 > supersecret
 ```
 
-Get multiple secrets:
+Traverse nested objects:
+
+```bash
+$ secrets get
+
+django:
+ secret_key: abc
+ admins: [zero, one, two three]
+
+database_url: supersecret
+```
 
 ```bash
-$ secrets get my-user my-password
-> my-user: foo
-> my-password: supersecret
+$ secrets get django.admins.2
+
+> two
 ```
 
 
 ### In Python
 
 Simply call `get` with the key. Note that if the secret is missing it will return `None`
 
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault()
 
-password = vault.get('my-password')
+admins = vault.get('django.admins')
 ```
 
 
 ## Editing secrets
 
 ### CLI command
 
@@ -107,17 +165,20 @@
 
 To edit secrets, run `secrets edit`, the file will be decrypted and your editor will open.
 
 ```bash
 $ secrets edit
 
 >> Opening secrets file in editor...
-{
-  "foo": "bar"
-}
+
+# Add your secrets below, comments are supported too.
+# django:
+#     secret_key: abc
+#
+# database_url: supersecret
 ```
 
 Any saved changes will be encrypted and saved to the file on disk when you close the editor.
 
 ### In Python
 
 You can also edit secrets from code:
@@ -156,35 +217,34 @@
 ## Printing secrets as environment variables
 
 Sometimes you may want to print a secret as environment variables. It will also apply if you have nested objects. You can do so by running:
 
 ```bash
 $ secrets edit
 
-{
-  "aws-credentials": {
-    "AWS_ACCESS_KEY_ID": "...",
-    "AWS_SECRET_ACCESS_KEY": "..."
-  }
-}
+dev:
+  aws-credentials:
+    AWS_ACCESS_KEY_ID: ..."
+    AWS_SECRET_ACCESS_KEY: ...
 ```
 
 Get will print the secrets as-is:
 
 ```bash
-$ secrets get aws-credentials
-> {"AWS_ACCESS_KEY_ID": "...", "AWS_SECRET_ACCESS_KEY": "..."}
+$ secrets get dev.aws-credentials
+AWS_ACCESS_KEY_ID: ..."
+AWS_SECRET_ACCESS_KEY: ...
 ```
 
 Envify will print the secrets ready for consumption as environment variables:
 
 ```bash
-$ secrets envify aws-credentials
-> AWS_ACCESS_KEY_ID=...
-> AWS_SECRET_ACCESS_KEY=...
+$ secrets envify --export dev.aws-credentials
+> export AWS_ACCESS_KEY_ID=...
+> export AWS_SECRET_ACCESS_KEY=...
 ```
 
 ## Providing the master.key file
 
 ### File on disk
 By default, the vault will look for the master key in a file located at `./master.key`.
 
@@ -221,23 +281,23 @@
 ### CLI command
 
 You can also provide them as a CLI arguments before the command:
 
 ```bash
 $ secrets \
   --master-key-filepath ./prod/master.key \
-  --secrets-filepath ./prod/secrets.json.enc \
+  --secrets-filepath ./prod/secrets.yml.enc \
   init
 ```
 
 This can be used to separate your secrets by environments such as `prod`, `staging`, `dev`, each having with their own key.
 
 ### In Python
 
-You can also configure the filepaths at which your `secrets.json.enc` and `master.key` files are located.
+You can also configure the filepaths at which your `secrets.yml.enc` and `master.key` files are located.
 
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
@@ -255,7 +315,9 @@
 
 Please check for any existing issues before openning a new Issue. If you'd like to work on something, please open a new Issue describing what you'd like to do before submitting a Pull Request.
 
 
 ## License
 
 See [LICENSE](https://github.com/anthonynsimon/secrets-vault/blob/master/LICENSE).
+
+
```

### Comparing `secrets-vault-0.1.9/secrets_vault/__main__.py` & `secrets-vault-0.2.0/secrets_vault/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,41 @@
 import json
+import logging
+from io import BytesIO
 
 import click
+from ruamel.yaml import YAML
 
 from secrets_vault import SecretsVault, exceptions, constants, __version__
 
 
-def serialize(v):
+def serialize(v, format="yaml"):
+    assert format in {"yaml", "json", "dotenv"}
+
     if not v:
         return ""
     if isinstance(v, str):
         return v
     if isinstance(v, int):
         return str(v)
     if isinstance(v, float):
         return str(v)
-    return json.dumps(v, default=str, sort_keys=False)
+    if format == "json":
+        return json.dumps(v, indent=2, default=str, sort_keys=False)
+    if format == "dotenv":
+        # encode non-value objects as json for use in env vars
+        return json.dumps(v, default=str, sort_keys=False)
+    if format == "yaml":
+        fout = BytesIO()
+        yaml = YAML(typ="rt")
+        yaml.dump(v, fout)
+        result = fout.getvalue().decode()
+        fout.close()
+        return result.strip()
+    raise NotImplementedError(f"Unsupported format: {format}")
 
 
 @click.group(help="Manage a local secrets vault.")
 @click.option(
     "-s",
     "--secrets-filepath",
     default=constants.DEFAULT_SECRETS_FILEPATH,
@@ -28,17 +45,32 @@
 @click.option(
     "-m",
     "--master-key-filepath",
     default=constants.DEFAULT_MASTER_KEY_FILEPATH,
     help="Path to the master.key file.",
     show_default=True,
 )
+@click.option(
+    "-f",
+    "--format",
+    default=constants.DEFAULT_FILE_FORMAT,
+    help="Format to use for the secrets vault.",
+    type=click.Choice(["yaml", "json"]),
+    show_default=True,
+)
+@click.option(
+    "-v",
+    "--verbose",
+    is_flag=True,
+    help="Enable verbose output.",
+)
 @click.pass_context
 def cli(ctx, **kwargs):
     ctx.obj = kwargs
+    logging.basicConfig(level=logging.INFO if kwargs["verbose"] else logging.ERROR)
 
 
 @cli.command(help="Show the package version.")
 @click.pass_context
 def version(ctx):
     click.echo(f"secrets-vault v{__version__}")
 
@@ -46,68 +78,76 @@
 @cli.command(
     help="Generate a new secrets vault and master.key pair. If a secrets vault already exists, this will abort."
 )
 @click.pass_context
 def init(ctx):
     try:
         SecretsVault.create(
-            secrets_filepath=ctx.obj["secrets_filepath"], master_key_filepath=ctx.obj["master_key_filepath"]
+            secrets_filepath=ctx.obj["secrets_filepath"],
+            master_key_filepath=ctx.obj["master_key_filepath"],
+            file_format=ctx.obj["format"],
         )
         click.echo(f"Generated new secrets vault at {ctx.obj['secrets_filepath']}")
         click.echo(f"Generated new master key at {ctx.obj['master_key_filepath']} - keep it safe!")
     except exceptions.SecretsFileAlreadyExists:
         print("Secrets file already exists, aborting...")
         exit(1)
 
 
 def with_vault(ctx, func):
     try:
         vault = SecretsVault(
-            secrets_filepath=ctx.obj["secrets_filepath"], master_key_filepath=ctx.obj["master_key_filepath"]
+            secrets_filepath=ctx.obj["secrets_filepath"],
+            master_key_filepath=ctx.obj["master_key_filepath"],
+            file_format=ctx.obj["format"],
         )
         func(vault)
-    except (exceptions.MasterKeyNotFound, exceptions.SecretsFileNotFound, exceptions.MasterKeyInvalid) as e:
+    except (
+        exceptions.MasterKeyNotFound,
+        exceptions.SecretsFileNotFound,
+        exceptions.MasterKeyInvalid,
+        exceptions.MalformedSecretsFile,
+    ) as e:
         click.echo(str(e))
         exit(1)
 
 
-@cli.command(
-    help="Get one or more secret values. If none are specified, all secrets are printed (eg. `secrets get`). You can also provide multiple keys to retrive more than one secret at a time (eg. secrets get foo1 foo2 foo3)."
-)
-@click.argument("key", required=False, nargs=-1)
+@cli.command(help="Get a secret value. If none are specified, all secrets are printed (eg. `secrets get`).")
+@click.argument("key", required=False)
 @click.pass_context
 def get(ctx, key):
+    fformat = ctx.obj["format"]
+
     def handler(vault):
         if key:
-            if len(key) == 1:
-                click.echo(serialize(vault.get(key[0])))
-            else:
-                for k in key:
-                    click.echo(f"{k}: {serialize(vault.get(k))}")
+            result = vault.get(key, default="")
         else:
-            for k, v in vault.secrets.items():
-                click.echo(f"{k}: {serialize(v)}")
+            result = vault.secrets
+
+        click.echo(serialize(result, fformat))
 
     with_vault(ctx, handler)
 
 
 @cli.command(
     help="Prints a provided secret key as one or more env variables. In case the value is a nested object, it will flatten the key=value pairs."
 )
 @click.argument("key")
 @click.option("--export", is_flag=True, help="Include the export modified for each environment variable.")
 @click.pass_context
 def envify(ctx, key, export):
+    puts = lambda k, v: click.echo(f"{'export ' if export else ''}{k.upper()}={serialize(v, 'dotenv')}")
+
     def handler(vault):
         value = vault.get(key)
         if isinstance(value, dict):
             for k, v in value.items():
-                click.echo(f"{'export ' if export else ''}{k}={serialize(v)}")
+                puts(k, v)
         else:
-            click.echo(f"{'export ' if export else ''}{key}={serialize(value)}")
+            puts(key, value)
 
     with_vault(ctx, handler)
 
 
 @cli.command(
     help="Store a secret. If the secret already exists, it will be overwritten. For example: `secrets set foo bar`"
 )
```

### Comparing `secrets-vault-0.1.9/secrets_vault/backends.py` & `secrets-vault-0.2.0/secrets_vault/backends.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.9/secrets_vault.egg-info/PKG-INFO` & `secrets-vault-0.2.0/secrets_vault.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,157 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.1.9
+Version: 0.2.0
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # secrets-vault
 
-Simple encrypted secrets for Python.
+Keep your app secrets encrypted in-repo, automatically decrypt on local dev or deploy.
 
-Inspired by Rails encrypted secrets. It can be used as a standalone CLI tool or as a library. 
+Inspired by Rails credentials - it pairs nicely with [mrsk](https://mrsk.dev). But it can be used as a standalone CLI tool or as a library. 
 
-The vault is JSON encoded and encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
+The vault is YAML encoded and encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
 
 ## Quick start
 
-> **Important:** You should keep the `master.key` secret. Ignore it in your `.gitignore` file. The `secrets.json.enc` file is safe to commit.
+1. Install it:
+```bash
+$ pip install secrets-vault
+```
+
+2. Create a new vault:
+ ```bash
+$ secrets init
+
+Generated new secrets vault at ./secrets.yml.enc
+Generated new master key at ./master.key - keep it safe!
+ ``` 
+
+3. Edit secrets:
+```bash
+$ secrets edit
+
+>> Opening secrets file in editor...
+
+# Add your secrets below, comments are supported too.
+# django:
+#     secret_key: abc
+#
+# database_url: supersecret
+```
+
+4. Read secrets:
+
+```bash
+# Via CLI
+$ secrets get database_url
+> supersecret
+```
+
+```python
+# In Python
+from secrets_vault import SecretsVault
 
-1. Install `pip install secrets-vault`.
-2. Run init:
-    ```bash
-    $ secrets init
-    Generated new secrets vault at ./secrets.json.enc
-    Generated new master key at ./master.key - keep it safe!
-    ``` 
-3. You can now edit your secrets:
-   ```bash
-    $ secrets edit
-   
-    >> Opening secrets file in editor...
-    {
-      "foo": "bar"
-    }
-    ```
+vault = SecretsVault()
+foo = vault.get('database_url')
+```
 
+**Important:** You should keep the `master.key` secret, do NOT commit it. Ignore it in your `.gitignore` file. The `secrets.yml.enc` file is encrypted and can be committed.
 
 ## CLI usage
 
 You can view the help anytime by running `secrets --help`:
 
 ```
 Usage: secrets [OPTIONS] COMMAND [ARGS]...
 
   Manage a local secrets vault.
 
 Options:
   -s, --secrets-filepath TEXT     Path to the encrypted secrets vault.
-  -m, --master-key-filepath TEXT  Path to the master.key file.
+                                  [default: ./secrets.yml.enc]
+  -m, --master-key-filepath TEXT  Path to the master.key file.  [default:
+                                  ./master.key]
+  -f, --format [yaml|json]        Format to use for the secrets vault.
+                                  [default: yaml]
+  -v, --verbose                   Enable verbose output.
   --help                          Show this message and exit.
 
 Commands:
   del      Delete a secret.
   edit     Open the secrets vault in your configured $EDITOR.
   envify   Prints a provided secret key as one or more env variables.
-  get      Get one or more secret values.
+  get      Get a secret value.
   init     Generate a new secrets vault and master.key pair.
   set      Store a secret.
   version  Show the package version.
 ```
 
 ## Reading secrets
 
 ### CLI commands
 
 List all secrets:
 
 ```bash
 $ secrets get
-> my-user: foo
-> my-password: supersecret
+
+# Add your secrets below, comments are supported too.
+# django:
+#     secret_key: abc
+#
+# database_url: supersecret
 ```
 
-Get one secret:
+Get a secret:
 
 ```bash
-$ secrets get my-password
+$ secrets get database_url
 > supersecret
 ```
 
-Get multiple secrets:
+Traverse nested objects:
 
 ```bash
-$ secrets get my-user my-password
-> my-user: foo
-> my-password: supersecret
+$ secrets get
+
+django:
+ secret_key: abc
+ admins: [zero, one, two three]
+
+database_url: supersecret
+```
+
+```bash
+$ secrets get django.admins.2
+
+> two
 ```
 
 
 ### In Python
 
 Simply call `get` with the key. Note that if the secret is missing it will return `None`
 
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault()
 
-password = vault.get('my-password')
+admins = vault.get('django.admins')
 ```
 
 
 ## Editing secrets
 
 ### CLI command
 
@@ -122,17 +165,20 @@
 
 To edit secrets, run `secrets edit`, the file will be decrypted and your editor will open.
 
 ```bash
 $ secrets edit
 
 >> Opening secrets file in editor...
-{
-  "foo": "bar"
-}
+
+# Add your secrets below, comments are supported too.
+# django:
+#     secret_key: abc
+#
+# database_url: supersecret
 ```
 
 Any saved changes will be encrypted and saved to the file on disk when you close the editor.
 
 ### In Python
 
 You can also edit secrets from code:
@@ -171,35 +217,34 @@
 ## Printing secrets as environment variables
 
 Sometimes you may want to print a secret as environment variables. It will also apply if you have nested objects. You can do so by running:
 
 ```bash
 $ secrets edit
 
-{
-  "aws-credentials": {
-    "AWS_ACCESS_KEY_ID": "...",
-    "AWS_SECRET_ACCESS_KEY": "..."
-  }
-}
+dev:
+  aws-credentials:
+    AWS_ACCESS_KEY_ID: ..."
+    AWS_SECRET_ACCESS_KEY: ...
 ```
 
 Get will print the secrets as-is:
 
 ```bash
-$ secrets get aws-credentials
-> {"AWS_ACCESS_KEY_ID": "...", "AWS_SECRET_ACCESS_KEY": "..."}
+$ secrets get dev.aws-credentials
+AWS_ACCESS_KEY_ID: ..."
+AWS_SECRET_ACCESS_KEY: ...
 ```
 
 Envify will print the secrets ready for consumption as environment variables:
 
 ```bash
-$ secrets envify aws-credentials
-> AWS_ACCESS_KEY_ID=...
-> AWS_SECRET_ACCESS_KEY=...
+$ secrets envify --export dev.aws-credentials
+> export AWS_ACCESS_KEY_ID=...
+> export AWS_SECRET_ACCESS_KEY=...
 ```
 
 ## Providing the master.key file
 
 ### File on disk
 By default, the vault will look for the master key in a file located at `./master.key`.
 
@@ -236,23 +281,23 @@
 ### CLI command
 
 You can also provide them as a CLI arguments before the command:
 
 ```bash
 $ secrets \
   --master-key-filepath ./prod/master.key \
-  --secrets-filepath ./prod/secrets.json.enc \
+  --secrets-filepath ./prod/secrets.yml.enc \
   init
 ```
 
 This can be used to separate your secrets by environments such as `prod`, `staging`, `dev`, each having with their own key.
 
 ### In Python
 
-You can also configure the filepaths at which your `secrets.json.enc` and `master.key` files are located.
+You can also configure the filepaths at which your `secrets.yml.enc` and `master.key` files are located.
 
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
```

### Comparing `secrets-vault-0.1.9/setup.py` & `secrets-vault-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.9/tests/test_backends.py` & `secrets-vault-0.2.0/tests/test_backends.py`

 * *Files identical despite different names*

