# Comparing `tmp/masterpass-0.2.2.tar.gz` & `tmp/masterpass-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masterpass-0.2.2.tar", last modified: Sun Jul 16 16:47:25 2023, max compression
+gzip compressed data, was "masterpass-0.2.3.tar", last modified: Thu Jul 27 01:25:16 2023, max compression
```

## Comparing `masterpass-0.2.2.tar` & `masterpass-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-16 16:47:25.103395 masterpass-0.2.2/
--rw-r--r--   0 pedro      (503) staff       (20)     1076 2023-07-16 16:43:11.000000 masterpass-0.2.2/LICENSE
--rw-r--r--   0 pedro      (503) staff       (20)     2749 2023-07-16 16:47:25.097844 masterpass-0.2.2/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)     2109 2023-07-16 16:31:39.000000 masterpass-0.2.2/README.md
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-16 16:47:25.096711 masterpass-0.2.2/master/
--rw-r--r--   0 pedro      (503) staff       (20)       18 2023-07-16 16:28:05.000000 masterpass-0.2.2/master/__init__.py
--rwxr-xr-x   0 pedro      (503) staff       (20)     3604 2023-07-16 16:28:35.000000 masterpass-0.2.2/master/cli.py
--rw-r--r--   0 pedro      (503) staff       (20)      953 2023-07-16 16:09:16.000000 masterpass-0.2.2/master/logger.py
--rw-r--r--   0 pedro      (503) staff       (20)     2179 2023-07-16 16:09:38.000000 masterpass-0.2.2/master/master.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-16 16:47:25.097628 masterpass-0.2.2/masterpass.egg-info/
--rw-r--r--   0 pedro      (503) staff       (20)     2749 2023-07-16 16:47:25.000000 masterpass-0.2.2/masterpass.egg-info/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      266 2023-07-16 16:47:25.000000 masterpass-0.2.2/masterpass.egg-info/SOURCES.txt
--rw-r--r--   0 pedro      (503) staff       (20)        1 2023-07-16 16:47:25.000000 masterpass-0.2.2/masterpass.egg-info/dependency_links.txt
--rw-r--r--   0 pedro      (503) staff       (20)       43 2023-07-16 16:47:25.000000 masterpass-0.2.2/masterpass.egg-info/entry_points.txt
--rw-r--r--   0 pedro      (503) staff       (20)        7 2023-07-16 16:47:25.000000 masterpass-0.2.2/masterpass.egg-info/top_level.txt
--rw-r--r--   0 pedro      (503) staff       (20)       38 2023-07-16 16:47:25.103451 masterpass-0.2.2/setup.cfg
--rw-r--r--   0 pedro      (503) staff       (20)      946 2023-07-16 16:19:44.000000 masterpass-0.2.2/setup.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-27 01:25:16.148211 masterpass-0.2.3/
+-rw-r--r--   0 pedro      (503) staff       (20)     1076 2023-07-16 16:43:11.000000 masterpass-0.2.3/LICENSE
+-rw-r--r--   0 pedro      (503) staff       (20)     3009 2023-07-27 01:25:16.148096 masterpass-0.2.3/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)     2369 2023-07-16 22:39:05.000000 masterpass-0.2.3/README.md
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-27 01:25:16.147238 masterpass-0.2.3/master/
+-rw-r--r--   0 pedro      (503) staff       (20)       18 2023-07-27 01:24:42.000000 masterpass-0.2.3/master/__init__.py
+-rwxr-xr-x   0 pedro      (503) staff       (20)     3737 2023-07-27 01:24:36.000000 masterpass-0.2.3/master/cli.py
+-rw-r--r--   0 pedro      (503) staff       (20)      953 2023-07-16 16:09:16.000000 masterpass-0.2.3/master/logger.py
+-rw-r--r--   0 pedro      (503) staff       (20)     2179 2023-07-16 16:09:38.000000 masterpass-0.2.3/master/master.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-27 01:25:16.147900 masterpass-0.2.3/masterpass.egg-info/
+-rw-r--r--   0 pedro      (503) staff       (20)     3009 2023-07-27 01:25:16.000000 masterpass-0.2.3/masterpass.egg-info/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      266 2023-07-27 01:25:16.000000 masterpass-0.2.3/masterpass.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        1 2023-07-27 01:25:16.000000 masterpass-0.2.3/masterpass.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       43 2023-07-27 01:25:16.000000 masterpass-0.2.3/masterpass.egg-info/entry_points.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        7 2023-07-27 01:25:16.000000 masterpass-0.2.3/masterpass.egg-info/top_level.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       38 2023-07-27 01:25:16.148252 masterpass-0.2.3/setup.cfg
+-rw-r--r--   0 pedro      (503) staff       (20)      946 2023-07-16 16:19:44.000000 masterpass-0.2.3/setup.py
```

### Comparing `masterpass-0.2.2/LICENSE` & `masterpass-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `masterpass-0.2.2/PKG-INFO` & `masterpass-0.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterpass
-Version: 0.2.2
+Version: 0.2.3
 Summary: Deterministic password generator
 Home-page: https://github.com/jpedro/master
 Download-URL: https://github.com/jpedro/master/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
 Keywords: deterministic password generator
@@ -19,28 +19,33 @@
 
 # Master
 
 [![Deploy pages](https://github.com/jpedro/master/actions/workflows/pages.yaml/badge.svg)](https://github.com/jpedro/master/actions/workflows/pages.yaml)
 
 Generates deterministic passwords
 
-Inspired by [spectre.app](https://spectre.app/) but simpler.
 
-
-![Pictutre](https://raw.githubusercontent.com/jpedro/master/master/docs/strong.jpg)
+<!-- ![Pictutre](https://raw.githubusercontent.com/jpedro/master/master/docs/strong.jpg) -->
 <!-- ![Strong password](https://raw.githubusercontent.com/jpedro/master/master/docs/blink.gif) -->
 
+This is inspired by [spectre.app](https://spectre.app/) but simpler.
 This uses a sha256 hashed combination of `username + password + service`
 to generate the same password, thus eliminating the need to store,
 maintain and back up other generated passwords.
 
+[jpedro.github.io/master](https://jpedro.github.io/master/) has the
+browser experience.
+
 The used service name list is kept under the file
 `~/.config/master/list.txt` (or whatever `MASTER_LIST` points to)
 *purely for autocompletion*, which will be added later.
 
+Eventually, the idea is to create a simple browser extension that uses
+the URL domain name as the service.
+
 
 ## Install
 
     pip install masterpass
 
 Yes, yes. The package is called `masterpass` but the binary is called
 `master`. To be fixed after [#2582](https://github.com/pypi/support/issues/2582)
@@ -72,15 +77,14 @@
 | `MASTER_LIST`       | `~/.config/master/list.txt`   |
 | `MASTER_USERNAME`   | (None) [1]                    |
 | `MASTER_PASSWORD`   | (None) [1]                    |
 | `MASTER_SEPARATOR`  | `-`                           |
 | `MASTER_LENGTH`     | `6`                           |
 | `MASTER_CHUNKS`     | `6`                           |
 
-**Note [1]:** If you don't set the `MASTER_USERNAME` or the
-`MASTER_PASSWORD` you will be prompted for them.
-
-
-## Online
-
-[jpedro.github.io/master](https://jpedro.github.io/master/) has the
-browser experience.
+Using these default settings, it will generate a password that's 41
+characters long. 6 chunks of 6 character long with 5 separators in
+between.
+
+> *Note*
+> [1] If you don't set the `MASTER_USERNAME` or the `MASTER_PASSWORD` you
+> will be prompted for them.
```

### Comparing `masterpass-0.2.2/README.md` & `masterpass-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # Master
 
 [![Deploy pages](https://github.com/jpedro/master/actions/workflows/pages.yaml/badge.svg)](https://github.com/jpedro/master/actions/workflows/pages.yaml)
 
 Generates deterministic passwords
 
-Inspired by [spectre.app](https://spectre.app/) but simpler.
 
-
-![Pictutre](https://raw.githubusercontent.com/jpedro/master/master/docs/strong.jpg)
+<!-- ![Pictutre](https://raw.githubusercontent.com/jpedro/master/master/docs/strong.jpg) -->
 <!-- ![Strong password](https://raw.githubusercontent.com/jpedro/master/master/docs/blink.gif) -->
 
+This is inspired by [spectre.app](https://spectre.app/) but simpler.
 This uses a sha256 hashed combination of `username + password + service`
 to generate the same password, thus eliminating the need to store,
 maintain and back up other generated passwords.
 
+[jpedro.github.io/master](https://jpedro.github.io/master/) has the
+browser experience.
+
 The used service name list is kept under the file
 `~/.config/master/list.txt` (or whatever `MASTER_LIST` points to)
 *purely for autocompletion*, which will be added later.
 
+Eventually, the idea is to create a simple browser extension that uses
+the URL domain name as the service.
+
 
 ## Install
 
     pip install masterpass
 
 Yes, yes. The package is called `masterpass` but the binary is called
 `master`. To be fixed after [#2582](https://github.com/pypi/support/issues/2582)
@@ -53,15 +58,14 @@
 | `MASTER_LIST`       | `~/.config/master/list.txt`   |
 | `MASTER_USERNAME`   | (None) [1]                    |
 | `MASTER_PASSWORD`   | (None) [1]                    |
 | `MASTER_SEPARATOR`  | `-`                           |
 | `MASTER_LENGTH`     | `6`                           |
 | `MASTER_CHUNKS`     | `6`                           |
 
-**Note [1]:** If you don't set the `MASTER_USERNAME` or the
-`MASTER_PASSWORD` you will be prompted for them.
-
-
-## Online
-
-[jpedro.github.io/master](https://jpedro.github.io/master/) has the
-browser experience.
+Using these default settings, it will generate a password that's 41
+characters long. 6 chunks of 6 character long with 5 separators in
+between.
+
+> *Note*
+> [1] If you don't set the `MASTER_USERNAME` or the `MASTER_PASSWORD` you
+> will be prompted for them.
```

### Comparing `masterpass-0.2.2/master/cli.py` & `masterpass-0.2.3/master/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,22 +20,29 @@
 from .logger import Logger
 
 
 USER_HOME        = os.path.expanduser("~")
 MASTER_LIST      = f"{USER_HOME}/.config/master/list.txt"
 MASTER_LIST      = os.environ.get("MASTER_LIST", MASTER_LIST)
 MASTER_DEBUG     = bool(os.environ.get("MASTER_DEBUG"))
-MASTER_USERNAME  = os.environ.get("MASTER_USERNAME")
-MASTER_PASSWORD  = os.environ.get("MASTER_PASSWORD")
+MASTER_USERNAME  = os.environ.get("MASTER_USERNAME", "")
+MASTER_PASSWORD  = os.environ.get("MASTER_PASSWORD", "")
 MASTER_SEPARATOR = os.environ.get("MASTER_SEPARATOR", "-")
 MASTER_LENGTH    = int(os.environ.get("MASTER_LENGTH", "6"))
 MASTER_CHUNKS    = int(os.environ.get("MASTER_CHUNKS", "6"))
 
 class Cli:
 
+    def __init__(self):
+        self.master = Master(MASTER_LIST)
+        self.master.chunks = MASTER_CHUNKS
+        self.master.length = MASTER_LENGTH
+        self.master.separator = MASTER_SEPARATOR
+
+
     def ask(self) -> (str, str):
         if len(MASTER_USERNAME) > 0:
             username = MASTER_USERNAME
         else:
             prompt = "Enter your master username: "
             username = getpass.getpass(prompt=prompt)
 
@@ -50,59 +57,55 @@
 
 
     @Logger.trace()
     def get(self, service: str, counter: int = 0):
         """Gets the deterministic password for SERVICE."""
         username, password = self.ask()
 
-        master = Master(MASTER_LIST)
-        master.add(service)
-        master.save()
-
-        master.username = username
-        master.password = password
-        random = master.generate(service, counter)
+        self.master.add(service)
+        self.master.save()
+
+        self.master.username = username
+        self.master.password = password
+        random = self.master.generate(service, counter)
         print(random)
 
     @Logger.trace()
     def start(self):
         """Asks input for a new SERVICE."""
         username, password = self.ask()
         service = input("Enter your service name: ")
 
-        master = Master(MASTER_LIST)
-        master.add(service)
-        master.save()
-
-        master.username = username
-        master.password = password
-        random = master.generate(service)
+        self.master.add(service)
+        self.master.save()
+
+        self.master.username = username
+        self.master.password = password
+        random = self.master.generate(service)
         print(random)
 
     @Logger.trace()
     def ls(self):
         """Lists all stored services."""
-        master = Master(MASTER_LIST)
-        master.load()
-        for service in master.services:
+        self.master.load()
+        for service in self.master.services:
             print(service)
 
 
     @Logger.trace()
     def version(self):
         """Prints the version."""
         print(f"v{VERSION}")
 
 
     @Logger.trace()
     def remove(self, service: str):
         """Removes SERVICE from the stored list."""
-        master = Master(MASTER_LIST)
-        master.remove(service)
-        master.save()
+        self.master.remove(service)
+        self.master.save()
 
 
 def main():
     cli = Cli()
     cmd = sys.argv[1] if len(sys.argv) > 1 else None
     args = sys.argv[1:]
```

### Comparing `masterpass-0.2.2/master/logger.py` & `masterpass-0.2.3/master/logger.py`

 * *Files identical despite different names*

### Comparing `masterpass-0.2.2/master/master.py` & `masterpass-0.2.3/master/master.py`

 * *Files identical despite different names*

### Comparing `masterpass-0.2.2/masterpass.egg-info/PKG-INFO` & `masterpass-0.2.3/masterpass.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masterpass
-Version: 0.2.2
+Version: 0.2.3
 Summary: Deterministic password generator
 Home-page: https://github.com/jpedro/master
 Download-URL: https://github.com/jpedro/master/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
 Keywords: deterministic password generator
@@ -19,28 +19,33 @@
 
 # Master
 
 [![Deploy pages](https://github.com/jpedro/master/actions/workflows/pages.yaml/badge.svg)](https://github.com/jpedro/master/actions/workflows/pages.yaml)
 
 Generates deterministic passwords
 
-Inspired by [spectre.app](https://spectre.app/) but simpler.
 
-
-![Pictutre](https://raw.githubusercontent.com/jpedro/master/master/docs/strong.jpg)
+<!-- ![Pictutre](https://raw.githubusercontent.com/jpedro/master/master/docs/strong.jpg) -->
 <!-- ![Strong password](https://raw.githubusercontent.com/jpedro/master/master/docs/blink.gif) -->
 
+This is inspired by [spectre.app](https://spectre.app/) but simpler.
 This uses a sha256 hashed combination of `username + password + service`
 to generate the same password, thus eliminating the need to store,
 maintain and back up other generated passwords.
 
+[jpedro.github.io/master](https://jpedro.github.io/master/) has the
+browser experience.
+
 The used service name list is kept under the file
 `~/.config/master/list.txt` (or whatever `MASTER_LIST` points to)
 *purely for autocompletion*, which will be added later.
 
+Eventually, the idea is to create a simple browser extension that uses
+the URL domain name as the service.
+
 
 ## Install
 
     pip install masterpass
 
 Yes, yes. The package is called `masterpass` but the binary is called
 `master`. To be fixed after [#2582](https://github.com/pypi/support/issues/2582)
@@ -72,15 +77,14 @@
 | `MASTER_LIST`       | `~/.config/master/list.txt`   |
 | `MASTER_USERNAME`   | (None) [1]                    |
 | `MASTER_PASSWORD`   | (None) [1]                    |
 | `MASTER_SEPARATOR`  | `-`                           |
 | `MASTER_LENGTH`     | `6`                           |
 | `MASTER_CHUNKS`     | `6`                           |
 
-**Note [1]:** If you don't set the `MASTER_USERNAME` or the
-`MASTER_PASSWORD` you will be prompted for them.
-
-
-## Online
-
-[jpedro.github.io/master](https://jpedro.github.io/master/) has the
-browser experience.
+Using these default settings, it will generate a password that's 41
+characters long. 6 chunks of 6 character long with 5 separators in
+between.
+
+> *Note*
+> [1] If you don't set the `MASTER_USERNAME` or the `MASTER_PASSWORD` you
+> will be prompted for them.
```

### Comparing `masterpass-0.2.2/setup.py` & `masterpass-0.2.3/setup.py`

 * *Files identical despite different names*

