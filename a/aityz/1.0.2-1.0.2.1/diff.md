# Comparing `tmp/aityz-1.0.2.tar.gz` & `tmp/aityz-1.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aityz-1.0.2.tar", last modified: Wed Jul 26 11:08:44 2023, max compression
+gzip compressed data, was "aityz-1.0.2.1.tar", last modified: Thu Jul 27 08:24:06 2023, max compression
```

## Comparing `aityz-1.0.2.tar` & `aityz-1.0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 11:08:44.607725 aityz-1.0.2/
--rw-rw-rw-   0        0        0    35821 2023-07-26 03:38:00.000000 aityz-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      447 2023-07-26 11:08:44.605421 aityz-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-26 11:03:01.000000 aityz-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 11:08:44.578122 aityz-1.0.2/aityz/
--rw-rw-rw-   0        0        0        0 2023-07-26 11:07:26.000000 aityz-1.0.2/aityz/__init__.py
--rw-rw-rw-   0        0        0     4078 2023-07-26 11:07:49.000000 aityz-1.0.2/aityz/encryption.py
--rw-rw-rw-   0        0        0      440 2023-07-26 11:05:19.000000 aityz-1.0.2/aityz/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:08:44.600516 aityz-1.0.2/aityz.egg-info/
--rw-rw-rw-   0        0        0      447 2023-07-26 11:08:44.000000 aityz-1.0.2/aityz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-26 11:08:44.000000 aityz-1.0.2/aityz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 11:08:44.000000 aityz-1.0.2/aityz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-26 11:08:44.000000 aityz-1.0.2/aityz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-26 11:08:44.000000 aityz-1.0.2/aityz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      625 2023-07-26 03:53:16.000000 aityz-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 11:08:44.607725 aityz-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      579 2023-07-26 11:08:20.000000 aityz-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:24:06.972301 aityz-1.0.2.1/
+-rw-rw-rw-   0        0        0    35821 2023-07-26 03:38:00.000000 aityz-1.0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      449 2023-07-27 08:24:06.970011 aityz-1.0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-26 11:03:01.000000 aityz-1.0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 08:24:06.930048 aityz-1.0.2.1/aityz/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:07:26.000000 aityz-1.0.2.1/aityz/__init__.py
+-rw-rw-rw-   0        0        0     5781 2023-07-27 08:22:26.000000 aityz-1.0.2.1/aityz/encryption.py
+-rw-rw-rw-   0        0        0      440 2023-07-26 11:05:19.000000 aityz-1.0.2.1/aityz/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:24:06.962069 aityz-1.0.2.1/aityz.egg-info/
+-rw-rw-rw-   0        0        0      449 2023-07-27 08:24:06.000000 aityz-1.0.2.1/aityz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-27 08:24:06.000000 aityz-1.0.2.1/aityz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 08:24:06.000000 aityz-1.0.2.1/aityz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-27 08:24:06.000000 aityz-1.0.2.1/aityz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-27 08:24:06.000000 aityz-1.0.2.1/aityz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      625 2023-07-26 03:53:16.000000 aityz-1.0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 08:24:06.972301 aityz-1.0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      606 2023-07-27 08:24:02.000000 aityz-1.0.2.1/setup.py
```

### Comparing `aityz-1.0.2/LICENSE` & `aityz-1.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aityz-1.0.2/aityz/encryption.py` & `aityz-1.0.2.1/aityz/encryption.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from aityz import exceptions
 import rsa
+from Crypto.Cipher import AES
+import base64
+
 
 def pad(pad, length=16):
     """
     Pad a given string `pad` with spaces to a specified `length`.
 
     :param pad: The string to be padded.
     :param length: The desired length of the padded string. Default is 16.
@@ -97,7 +100,54 @@
             f.close()
         Data = rsa.decrypt(data, self.Pri)
         if outputFile is not None:
             with open(outputFile, 'wb') as f:
                 f.write(Data)
         else:
             return Data
+
+
+class AES256:
+    def __init__(self, password, nonce=None):
+        super().__init__()
+        self.key = password
+        if len(password) % 16 != 0:
+            password = pad(password)
+        if nonce is None:
+            self.cipher = AES.new(password.encode('utf8'), AES.MODE_EAX)
+        else:
+            self.cipher = AES.new(password.encode('utf8'), AES.MODE_EAX, nonce=nonce)
+        self.nonce = self.cipher.nonce
+
+    def encrypt(self, content):
+        enc, tag = self.cipher.encrypt_and_digest(content.encode('utf-8'))
+        return enc, tag, self.cipher.nonce
+
+    def getNonce(self):
+        return self.cipher.nonce
+
+    def decrypt(self, content):
+        return self.cipher.decrypt(content)
+
+    def encryptFile(self, fileName, saveLoc=None):
+        with open(fileName, 'r') as f:
+            data = f.read()
+        if saveLoc is not None:
+            with open(saveLoc, 'w') as f:
+                f.write(str(self.cipher.encrypt(data.encode('utf-8'))))
+        else:
+            return str(self.cipher.encrypt(data.encode('utf-8')))
+
+    def decryptFile(self, fileName, saveLoc=None):
+        with open(fileName, 'r') as f:
+            data = f.read()
+        if saveLoc is not None:
+            with open(saveLoc, 'w') as f:
+                f.write(str(self.cipher.decrypt(data.encode('utf-8'))))
+        else:
+            return str(self.cipher.decrypt(data.encode('utf-8')))
+
+    def update(self, nonce=None):
+        if nonce is None:
+            self.cipher = AES.new(self.key, AES.MODE_EAX)
+        else:
+            self.cipher = AES.new(self.key, AES.MODE_EAX, nonce=nonce)
```

### Comparing `aityz-1.0.2/pyproject.toml` & `aityz-1.0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aityz-1.0.2/setup.py` & `aityz-1.0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aityz',
-    version='1.0.2',
+    version='1.0.2.1',
     packages=find_packages(),
     install_requires=[
-        'rsa'
+        'rsa',
+        'pycryptodome'
     ],
     author='Aityz',
     author_email='itzaityz@gmail.com',
     description='The multipurpose package, built for programmers',
     long_description='Aityz Library is a multipurpose library made for many different use cases for Python. From '
                      'Machine Learning to Encryption, it has simplified many different ways of using Python.',
     url='https://github.com/Aityz/Library',
```

