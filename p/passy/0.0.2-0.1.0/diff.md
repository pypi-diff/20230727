# Comparing `tmp/passy-0.0.2.tar.gz` & `tmp/passy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passy-0.0.2.tar", last modified: Sat Apr 15 14:36:39 2023, max compression
+gzip compressed data, was "passy-0.1.0.tar", last modified: Thu Jul 27 15:55:48 2023, max compression
```

## Comparing `passy-0.0.2.tar` & `passy-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-04-15 14:30:49.061192 passy-0.0.2/LICENSE
--rw-r--r--   0        0        0       57 2023-04-15 14:30:16.196544 passy-0.0.2/passy/__init__.py
--rw-r--r--   0        0        0      814 2023-04-15 14:36:38.692068 passy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 passy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-04-15 14:30:30.500826 passy-0.1.0/.gitignore
+-rw-r--r--   0        0        0    18090 2023-05-15 13:04:52.553780 passy-0.1.0/LICENSE
+-rw-r--r--   0        0        0      214 2023-05-15 12:44:31.225932 passy-0.1.0/README.md
+-rw-r--r--   0        0        0       44 2023-07-27 14:11:19.271144 passy-0.1.0/passy/__init__.py
+-rw-r--r--   0        0        0     1511 2023-07-27 14:09:48.204792 passy-0.1.0/passy/otp.py
+-rw-r--r--   0        0        0     1611 2023-07-27 15:29:27.537453 passy-0.1.0/passy/passy.py
+-rw-r--r--   0        0        0      904 2023-07-27 15:55:22.393150 passy-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      208 2023-05-16 21:48:12.866622 passy-0.1.0/test.py
+-rw-r--r--   0        0        0      175 2023-07-27 15:15:56.940391 passy-0.1.0/tests/test_2fa.py
+-rw-r--r--   0        0        0      575 2023-07-27 15:21:04.634404 passy-0.1.0/tests/test_auth.py
+-rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 passy-0.1.0/PKG-INFO
```

### Comparing `passy-0.0.2/PKG-INFO` & `passy-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: passy
-Version: 0.0.2
-Summary: Login and Password Handler for python
+Version: 0.1.0
+Summary: Logins made simple
 Author-email: Ben Brady <benbradybusiness@gmail.com>
 Requires-Python: >=3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
+Requires-Dist: passlib[argon2]~=1.7.4
+Requires-Dist: pyotp~=2.8.0
+Requires-Dist: typing_extensions>=4.5.0
 Project-URL: Source, https://github.com/Ben-Brady/passy
```

