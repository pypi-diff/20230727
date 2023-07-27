# Comparing `tmp/multisig_ci-0.6.3.tar.gz` & `tmp/multisig_ci-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multisig_ci-0.6.3.tar", max compression
+gzip compressed data, was "multisig_ci-0.6.4.tar", max compression
```

## Comparing `multisig_ci-0.6.3.tar` & `multisig_ci-0.6.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/LICENSE
--rw-r--r--   0        0        0        0 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/__init__.py
--rw-r--r--   0        0        0      570 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/__main__.py
--rw-r--r--   0        0        0     7435 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/ci_override.py
--rw-r--r--   0        0        0     5811 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/hydrate_ci_cache.py
--rw-r--r--   0        0        0     2033 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/run_brownie.py
--rw-r--r--   0        0        0      811 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/safes.py
--rw-r--r--   0        0        0     1580 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/sign.py
--rw-r--r--   0        0        0     1913 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/telegram.py
--rwxr-xr-x   0        0        0      651 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/test_telegram.sh
--rw-r--r--   0        0        0      508 2023-07-27 03:14:43.874093 multisig_ci-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 multisig_ci-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/__init__.py
+-rw-r--r--   0        0        0      570 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/__main__.py
+-rw-r--r--   0        0        0     7414 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/ci_override.py
+-rw-r--r--   0        0        0     5811 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/hydrate_ci_cache.py
+-rw-r--r--   0        0        0     2033 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/run_brownie.py
+-rw-r--r--   0        0        0      811 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/safes.py
+-rw-r--r--   0        0        0     1580 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/sign.py
+-rw-r--r--   0        0        0     1913 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/telegram.py
+-rwxr-xr-x   0        0        0      651 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/test_telegram.sh
+-rw-r--r--   0        0        0      508 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 multisig_ci-0.6.4/PKG-INFO
```

### Comparing `multisig_ci-0.6.3/LICENSE` & `multisig_ci-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.3/multisig_ci/__main__.py` & `multisig_ci-0.6.4/multisig_ci/__main__.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.3/multisig_ci/ci_override.py` & `multisig_ci-0.6.4/multisig_ci/ci_override.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from copy import copy
 from brownie_safe import BrownieSafe as ApeSafe
-from brownie_safe import transaction_service, multisends
+from brownie_safe import multisends
 from brownie import accounts, network, chain, Contract
 from gnosis.safe.safe_tx import SafeTx
 from eth_abi import encode_abi
 from typing import Optional, Union
 from brownie.network.account import LocalAccount
 from brownie._config import CONFIG
```

### Comparing `multisig_ci-0.6.3/multisig_ci/hydrate_ci_cache.py` & `multisig_ci-0.6.4/multisig_ci/hydrate_ci_cache.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.3/multisig_ci/run_brownie.py` & `multisig_ci-0.6.4/multisig_ci/run_brownie.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.3/multisig_ci/safes.py` & `multisig_ci-0.6.4/multisig_ci/safes.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.3/multisig_ci/sign.py` & `multisig_ci-0.6.4/multisig_ci/sign.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.3/multisig_ci/telegram.py` & `multisig_ci-0.6.4/multisig_ci/telegram.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.3/multisig_ci/test_telegram.sh` & `multisig_ci-0.6.4/multisig_ci/test_telegram.sh`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.3/PKG-INFO` & `multisig_ci-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multisig-ci
-Version: 0.6.3
+Version: 0.6.4
 Summary: Gnosis safe ci scripts.
 License: AGPLv3
 Author: kx9x
 Author-email: kx9x@protonmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

