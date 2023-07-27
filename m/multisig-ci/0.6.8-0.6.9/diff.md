# Comparing `tmp/multisig_ci-0.6.8.tar.gz` & `tmp/multisig_ci-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multisig_ci-0.6.8.tar", max compression
+gzip compressed data, was "multisig_ci-0.6.9.tar", max compression
```

## Comparing `multisig_ci-0.6.8.tar` & `multisig_ci-0.6.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-07-27 05:38:48.369910 multisig_ci-0.6.8/LICENSE
--rw-r--r--   0        0        0        0 2023-07-27 05:38:48.369910 multisig_ci-0.6.8/multisig_ci/__init__.py
--rw-r--r--   0        0        0      570 2023-07-27 05:38:48.369910 multisig_ci-0.6.8/multisig_ci/__main__.py
--rw-r--r--   0        0        0     4315 2023-07-27 05:38:48.369910 multisig_ci-0.6.8/multisig_ci/ci_override.py
--rw-r--r--   0        0        0     5811 2023-07-27 05:38:48.369910 multisig_ci-0.6.8/multisig_ci/hydrate_ci_cache.py
--rw-r--r--   0        0        0     2033 2023-07-27 05:38:48.369910 multisig_ci-0.6.8/multisig_ci/run_brownie.py
--rw-r--r--   0        0        0      811 2023-07-27 05:38:48.369910 multisig_ci-0.6.8/multisig_ci/safes.py
--rw-r--r--   0        0        0     1580 2023-07-27 05:38:48.369910 multisig_ci-0.6.8/multisig_ci/sign.py
--rw-r--r--   0        0        0     1913 2023-07-27 05:38:48.369910 multisig_ci-0.6.8/multisig_ci/telegram.py
--rwxr-xr-x   0        0        0      651 2023-07-27 05:38:48.369910 multisig_ci-0.6.8/multisig_ci/test_telegram.sh
--rw-r--r--   0        0        0      506 2023-07-27 05:38:48.369910 multisig_ci-0.6.8/pyproject.toml
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 multisig_ci-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-27 06:42:39.204615 multisig_ci-0.6.9/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-27 06:42:39.204615 multisig_ci-0.6.9/multisig_ci/__init__.py
+-rw-r--r--   0        0        0      570 2023-07-27 06:42:39.204615 multisig_ci-0.6.9/multisig_ci/__main__.py
+-rw-r--r--   0        0        0     5826 2023-07-27 06:42:39.204615 multisig_ci-0.6.9/multisig_ci/ci_override.py
+-rw-r--r--   0        0        0     5811 2023-07-27 06:42:39.204615 multisig_ci-0.6.9/multisig_ci/hydrate_ci_cache.py
+-rw-r--r--   0        0        0     2033 2023-07-27 06:42:39.204615 multisig_ci-0.6.9/multisig_ci/run_brownie.py
+-rw-r--r--   0        0        0      811 2023-07-27 06:42:39.204615 multisig_ci-0.6.9/multisig_ci/safes.py
+-rw-r--r--   0        0        0     1580 2023-07-27 06:42:39.204615 multisig_ci-0.6.9/multisig_ci/sign.py
+-rw-r--r--   0        0        0     1913 2023-07-27 06:42:39.204615 multisig_ci-0.6.9/multisig_ci/telegram.py
+-rwxr-xr-x   0        0        0      651 2023-07-27 06:42:39.204615 multisig_ci-0.6.9/multisig_ci/test_telegram.sh
+-rw-r--r--   0        0        0      506 2023-07-27 06:42:39.204615 multisig_ci-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 multisig_ci-0.6.9/PKG-INFO
```

### Comparing `multisig_ci-0.6.8/LICENSE` & `multisig_ci-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.8/multisig_ci/__main__.py` & `multisig_ci-0.6.9/multisig_ci/__main__.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.8/multisig_ci/hydrate_ci_cache.py` & `multisig_ci-0.6.9/multisig_ci/hydrate_ci_cache.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.8/multisig_ci/run_brownie.py` & `multisig_ci-0.6.9/multisig_ci/run_brownie.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.8/multisig_ci/safes.py` & `multisig_ci-0.6.9/multisig_ci/safes.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.8/multisig_ci/sign.py` & `multisig_ci-0.6.9/multisig_ci/sign.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.8/multisig_ci/telegram.py` & `multisig_ci-0.6.9/multisig_ci/telegram.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.8/multisig_ci/test_telegram.sh` & `multisig_ci-0.6.9/multisig_ci/test_telegram.sh`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.8/PKG-INFO` & `multisig_ci-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multisig-ci
-Version: 0.6.8
+Version: 0.6.9
 Summary: Gnosis safe ci scripts.
 License: AGPLv3
 Author: kx9x
 Author-email: kx9x@protonmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

