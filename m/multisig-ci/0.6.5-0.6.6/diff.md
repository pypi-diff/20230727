# Comparing `tmp/multisig_ci-0.6.5.tar.gz` & `tmp/multisig_ci-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multisig_ci-0.6.5.tar", max compression
+gzip compressed data, was "multisig_ci-0.6.6.tar", max compression
```

## Comparing `multisig_ci-0.6.5.tar` & `multisig_ci-0.6.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-07-27 04:05:44.597463 multisig_ci-0.6.5/LICENSE
--rw-r--r--   0        0        0        0 2023-07-27 04:05:44.597463 multisig_ci-0.6.5/multisig_ci/__init__.py
--rw-r--r--   0        0        0      570 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/__main__.py
--rw-r--r--   0        0        0     5967 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/ci_override.py
--rw-r--r--   0        0        0     5811 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/hydrate_ci_cache.py
--rw-r--r--   0        0        0     2033 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/run_brownie.py
--rw-r--r--   0        0        0      811 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/safes.py
--rw-r--r--   0        0        0     1580 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/sign.py
--rw-r--r--   0        0        0     1913 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/telegram.py
--rwxr-xr-x   0        0        0      651 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/test_telegram.sh
--rw-r--r--   0        0        0      508 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 multisig_ci-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-27 04:19:13.176348 multisig_ci-0.6.6/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-27 04:19:13.176348 multisig_ci-0.6.6/multisig_ci/__init__.py
+-rw-r--r--   0        0        0      570 2023-07-27 04:19:13.176348 multisig_ci-0.6.6/multisig_ci/__main__.py
+-rw-r--r--   0        0        0     5962 2023-07-27 04:19:13.176348 multisig_ci-0.6.6/multisig_ci/ci_override.py
+-rw-r--r--   0        0        0     5811 2023-07-27 04:19:13.176348 multisig_ci-0.6.6/multisig_ci/hydrate_ci_cache.py
+-rw-r--r--   0        0        0     2033 2023-07-27 04:19:13.176348 multisig_ci-0.6.6/multisig_ci/run_brownie.py
+-rw-r--r--   0        0        0      811 2023-07-27 04:19:13.176348 multisig_ci-0.6.6/multisig_ci/safes.py
+-rw-r--r--   0        0        0     1580 2023-07-27 04:19:13.176348 multisig_ci-0.6.6/multisig_ci/sign.py
+-rw-r--r--   0        0        0     1913 2023-07-27 04:19:13.176348 multisig_ci-0.6.6/multisig_ci/telegram.py
+-rwxr-xr-x   0        0        0      651 2023-07-27 04:19:13.176348 multisig_ci-0.6.6/multisig_ci/test_telegram.sh
+-rw-r--r--   0        0        0      508 2023-07-27 04:19:13.176348 multisig_ci-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 multisig_ci-0.6.6/PKG-INFO
```

### Comparing `multisig_ci-0.6.5/LICENSE` & `multisig_ci-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.5/multisig_ci/__main__.py` & `multisig_ci-0.6.6/multisig_ci/__main__.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.5/multisig_ci/ci_override.py` & `multisig_ci-0.6.6/multisig_ci/ci_override.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         multisends[10] = "0x998739BFdAAdde7C933B942a68053933098f9EDa"
 
         if network.chain.id in gnosis_frontend_urls:
             self.frontend_url = gnosis_frontend_urls[network.chain.id]
         else:
             self.frontend_url = gnosis_frontend_urls[1]
 
-        super().__init__(address, base_url=self.base_url, multisend=multisend)
+        super().__init__(address, base_url=base_url, multisend=multisend)
 
     @property
     def is_ci(self):
         return os.environ.get("CI", "").lower() == "true"
 
     @property
     def is_send(self):
```

### Comparing `multisig_ci-0.6.5/multisig_ci/hydrate_ci_cache.py` & `multisig_ci-0.6.6/multisig_ci/hydrate_ci_cache.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.5/multisig_ci/run_brownie.py` & `multisig_ci-0.6.6/multisig_ci/run_brownie.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.5/multisig_ci/safes.py` & `multisig_ci-0.6.6/multisig_ci/safes.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.5/multisig_ci/sign.py` & `multisig_ci-0.6.6/multisig_ci/sign.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.5/multisig_ci/telegram.py` & `multisig_ci-0.6.6/multisig_ci/telegram.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.5/multisig_ci/test_telegram.sh` & `multisig_ci-0.6.6/multisig_ci/test_telegram.sh`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.5/PKG-INFO` & `multisig_ci-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multisig-ci
-Version: 0.6.5
+Version: 0.6.6
 Summary: Gnosis safe ci scripts.
 License: AGPLv3
 Author: kx9x
 Author-email: kx9x@protonmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

