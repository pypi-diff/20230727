# Comparing `tmp/greynoiselabs-0.1.0.tar.gz` & `tmp/greynoiselabs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greynoiselabs-0.1.0.tar", last modified: Fri Jun 16 04:37:42 2023, max compression
+gzip compressed data, was "greynoiselabs-0.1.1.tar", last modified: Thu Jul 27 03:51:51 2023, max compression
```

## Comparing `greynoiselabs-0.1.0.tar` & `greynoiselabs-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:37:42.956658 greynoiselabs-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-16 04:37:42.956658 greynoiselabs-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-16 04:37:42.956658 greynoiselabs-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:37:42.952658 greynoiselabs-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:37:42.956658 greynoiselabs-0.1.0/src/greynoiselabs/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/src/greynoiselabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/src/greynoiselabs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/src/greynoiselabs/async_base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/src/greynoiselabs/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/src/greynoiselabs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/src/greynoiselabs/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/src/greynoiselabs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/src/greynoiselabs/get_c2s.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/src/greynoiselabs/input_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/src/greynoiselabs/noise_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/src/greynoiselabs/scalars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/src/greynoiselabs/top_h_t_t_p_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/src/greynoiselabs/top_knocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-16 04:37:39.000000 greynoiselabs-0.1.0/src/greynoiselabs/top_popular_i_ps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:37:42.956658 greynoiselabs-0.1.0/src/greynoiselabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-16 04:37:42.000000 greynoiselabs-0.1.0/src/greynoiselabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-16 04:37:42.000000 greynoiselabs-0.1.0/src/greynoiselabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 04:37:42.000000 greynoiselabs-0.1.0/src/greynoiselabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 04:37:42.000000 greynoiselabs-0.1.0/src/greynoiselabs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 04:37:42.000000 greynoiselabs-0.1.0/src/greynoiselabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 04:37:42.000000 greynoiselabs-0.1.0/src/greynoiselabs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:51:51.593615 greynoiselabs-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-27 03:51:51.593615 greynoiselabs-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-27 03:51:51.593615 greynoiselabs-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-27 03:51:41.000000 greynoiselabs-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:51:51.589615 greynoiselabs-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:51:51.589615 greynoiselabs-0.1.1/src/greynoiselabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-27 03:51:41.000000 greynoiselabs-0.1.1/src/greynoiselabs/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:51:51.593615 greynoiselabs-0.1.1/src/greynoiselabs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/async_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/generate_g_n_q_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/get_c2s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/get_i_ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/get_knocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/get_noise_ranks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/get_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/input_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/noise_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/scalars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/top_h_t_t_p_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/top_knocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/top_popular_i_ps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:51:51.593615 greynoiselabs-0.1.1/src/greynoiselabs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5763 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:51:51.589615 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-27 03:51:51.000000 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-27 03:51:51.000000 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:51:51.000000 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 03:51:51.000000 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:51:51.000000 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-27 03:51:51.000000 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 03:51:51.000000 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/top_level.txt
```

### Comparing `greynoiselabs-0.1.0/LICENSE` & `greynoiselabs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `greynoiselabs-0.1.0/PKG-INFO` & `greynoiselabs-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greynoiselabs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Abstraction to interact with GreyNoise Labs GraphQL API.
 Home-page: https://api.labs.greynoise.io/
 Author: GreyNoise Intelligence
 Author-email: labs@greynoise.io
 License: MIT
 Download-URL: https://github.com/GreyNoise-Intelligence/greynoiselabs
 Keywords: internet,scanning,threat intelligence,security
@@ -41,15 +41,15 @@
 
 .. _Documentation: https://api.labs.greynoise.io/1/docs/
 
 Quick Start
 ===========
 **Install the library**:
 
-``pip install labs-graphql-client`` or ``python setup.py install``
+``pip install greynoiselabs`` or ``python setup.py install``
 
 Example Code
 
 ..  code-block:: python
 
     import os
     import asyncio
@@ -62,13 +62,13 @@
     print(response)
 
 
 =========
 Changelog
 =========
 
-Version `dev`_
+Version `0.1.1`_
 ================
-**Date**: unreleased
+**Date**: July 27, 2023
 
-.. _`dev`: https://github.com/GreyNoise-Intelligence/labs-graphql-client/compare/v0.1.0...HEAD
+.. _`0.1.1`: https://github.com/GreyNoise-Intelligence/greynoiselabs/compare/v0.1.0...0.1.1
```

### Comparing `greynoiselabs-0.1.0/README.rst` & `greynoiselabs-0.1.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 .. _Documentation: https://api.labs.greynoise.io/1/docs/
 
 Quick Start
 ===========
 **Install the library**:
 
-``pip install labs-graphql-client`` or ``python setup.py install``
+``pip install greynoiselabs`` or ``python setup.py install``
 
 Example Code
 
 ..  code-block:: python
 
     import os
     import asyncio
```

### Comparing `greynoiselabs-0.1.0/setup.py` & `greynoiselabs-0.1.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,32 +6,25 @@
 
 
 def read(fname):
     """Read file and return its contents."""
     with open(os.path.join(os.path.dirname(__file__), fname)) as input_file:
         return input_file.read()
 
-
-INSTALL_REQUIRES = [
-    "pydantic",
-    "httpx",
-    "websockets",
-]
-
 setup(
     name="greynoiselabs",
-    version="0.1.0",
+    version="0.1.1",
     description="Abstraction to interact with GreyNoise Labs GraphQL API.",
     url="https://api.labs.greynoise.io/",
     author="GreyNoise Intelligence",
     author_email="labs@greynoise.io",
     license="MIT",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
-    install_requires=INSTALL_REQUIRES,
+    install_requires=read("requirements/common.txt").split("\n"),
     long_description=read("README.rst") + "\n\n" + read("CHANGELOG.rst"),
     python_requires=">=3.0, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -40,11 +33,12 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Topic :: Software Development :: Libraries",
     ],
+    entry_points={"console_scripts": ["greynoiselabs = greynoiselabs.cli.main:app"]},
     zip_safe=False,
     keywords=["internet", "scanning", "threat intelligence", "security"],
     download_url="https://github.com/GreyNoise-Intelligence/greynoiselabs",
 )
```

### Comparing `greynoiselabs-0.1.0/src/greynoiselabs/__init__.py` & `greynoiselabs-0.1.1/src/greynoiselabs/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,56 @@
-# Generated by ariadne-codegen on 2023-06-15 23:53
+# Generated by ariadne-codegen on 2023-07-26 20:32
 
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel
 from .client import Client
 from .exceptions import (
     GraphQLClientError,
     GraphQLClientGraphQLError,
     GraphQLClientGraphQLMultiError,
     GraphQLClientHttpError,
     GraphQlClientInvalidResponseError,
 )
-from .get_c2s import GetC2s, GetC2sTopC2s, GetC2sTopC2sC2s, GetC2sTopC2sQueryInfo
-from .input_types import SpectaQLOption
-from .noise_rank import (
-    NoiseRank,
-    NoiseRankNoiseRank,
-    NoiseRankNoiseRankIps,
-    NoiseRankNoiseRankQueryInfo,
-)
-from .top_h_t_t_p_requests import (
-    TopHTTPRequests,
-    TopHTTPRequestsTopHTTPRequests,
-    TopHTTPRequestsTopHTTPRequestsHttpRequests,
-    TopHTTPRequestsTopHTTPRequestsQueryInfo,
+from .generate_g_n_q_l import GenerateGNQL, GenerateGNQLGenerateGNQL
+from .get_c2s import GetC2s, GetC2sTopC2s, GetC2sTopC2sC2s
+from .get_i_ps import GetIPs, GetIPsTopPopularIPs, GetIPsTopPopularIPsPopularIPs
+from .get_knocks import GetKnocks, GetKnocksTopKnocks, GetKnocksTopKnocksKnock
+from .get_noise_ranks import (
+    GetNoiseRanks,
+    GetNoiseRanksNoiseRank,
+    GetNoiseRanksNoiseRankIps,
 )
-from .top_knocks import (
-    TopKnocks,
-    TopKnocksTopKnocks,
-    TopKnocksTopKnocksKnock,
-    TopKnocksTopKnocksQueryInfo,
-)
-from .top_popular_i_ps import (
-    TopPopularIPs,
-    TopPopularIPsTopPopularIPs,
-    TopPopularIPsTopPopularIPsPopularIPs,
-    TopPopularIPsTopPopularIPsQueryInfo,
+from .get_requests import (
+    GetRequests,
+    GetRequestsTopHTTPRequests,
+    GetRequestsTopHTTPRequestsHttpRequests,
 )
+from .input_types import SpectaQLOption
 
 __all__ = [
     "AsyncBaseClient",
     "BaseModel",
     "Client",
+    "GenerateGNQL",
+    "GenerateGNQLGenerateGNQL",
     "GetC2s",
     "GetC2sTopC2s",
     "GetC2sTopC2sC2s",
-    "GetC2sTopC2sQueryInfo",
+    "GetIPs",
+    "GetIPsTopPopularIPs",
+    "GetIPsTopPopularIPsPopularIPs",
+    "GetKnocks",
+    "GetKnocksTopKnocks",
+    "GetKnocksTopKnocksKnock",
+    "GetNoiseRanks",
+    "GetNoiseRanksNoiseRank",
+    "GetNoiseRanksNoiseRankIps",
+    "GetRequests",
+    "GetRequestsTopHTTPRequests",
+    "GetRequestsTopHTTPRequestsHttpRequests",
     "GraphQLClientError",
     "GraphQLClientGraphQLError",
     "GraphQLClientGraphQLMultiError",
     "GraphQLClientHttpError",
     "GraphQlClientInvalidResponseError",
-    "NoiseRank",
-    "NoiseRankNoiseRank",
-    "NoiseRankNoiseRankIps",
-    "NoiseRankNoiseRankQueryInfo",
     "SpectaQLOption",
-    "TopHTTPRequests",
-    "TopHTTPRequestsTopHTTPRequests",
-    "TopHTTPRequestsTopHTTPRequestsHttpRequests",
-    "TopHTTPRequestsTopHTTPRequestsQueryInfo",
-    "TopKnocks",
-    "TopKnocksTopKnocks",
-    "TopKnocksTopKnocksKnock",
-    "TopKnocksTopKnocksQueryInfo",
-    "TopPopularIPs",
-    "TopPopularIPsTopPopularIPs",
-    "TopPopularIPsTopPopularIPsPopularIPs",
-    "TopPopularIPsTopPopularIPsQueryInfo",
 ]
```

### Comparing `greynoiselabs-0.1.0/src/greynoiselabs/async_base_client.py` & `greynoiselabs-0.1.1/src/greynoiselabs/api/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-15 23:53
+# Generated by ariadne-codegen on 2023-06-28 15:55
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `greynoiselabs-0.1.0/src/greynoiselabs/base_model.py` & `greynoiselabs-0.1.1/src/greynoiselabs/api/base_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-15 23:53
+# Generated by ariadne-codegen on 2023-06-28 15:55
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `greynoiselabs-0.1.0/src/greynoiselabs/client.py` & `greynoiselabs-0.1.1/src/greynoiselabs/api/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,151 +1,147 @@
-# Generated by ariadne-codegen on 2023-06-15 23:53
+# Generated by ariadne-codegen on 2023-06-28 15:55
 # Source: queries
 
 from .async_base_client import AsyncBaseClient
+from .generate_g_n_q_l import GenerateGNQL
 from .get_c2s import GetC2s
-from .noise_rank import NoiseRank
-from .top_h_t_t_p_requests import TopHTTPRequests
-from .top_knocks import TopKnocks
-from .top_popular_i_ps import TopPopularIPs
+from .get_i_ps import GetIPs
+from .get_knocks import GetKnocks
+from .get_noise_ranks import GetNoiseRanks
+from .get_requests import GetRequests
 
 
 def gql(q: str) -> str:
     return q
 
 
 class Client(AsyncBaseClient):
     async def get_c2s(self) -> GetC2s:
         query = gql(
             """
             query getC2s {
               topC2s {
-                queryInfo {
-                  resultsAvailable
-                  resultsLimit
-                }
                 c2s {
-                  c2_domains
-                  c2_ips
+                  source_ip
                   hits
-                  payload
                   pervasiveness
-                  source_ip
+                  c2_ips
+                  c2_domains
+                  payload
                 }
               }
             }
             """
         )
         variables: dict[str, object] = {}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetC2s.parse_obj(data)
 
-    async def top_h_t_t_p_requests(self) -> TopHTTPRequests:
+    async def get_requests(self) -> GetRequests:
         query = gql(
             """
-            query TopHTTPRequests {
+            query getRequests {
               topHTTPRequests {
-                queryInfo {
-                  resultsAvailable
-                  resultsLimit
-                }
                 httpRequests {
-                  method
                   path
-                  pervasiveness
                   request_count
-                  request_headers
                   source_ip_count
+                  request_headers
+                  pervasiveness
                 }
               }
             }
             """
         )
         variables: dict[str, object] = {}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
-        return TopHTTPRequests.parse_obj(data)
+        return GetRequests.parse_obj(data)
 
-    async def top_knocks(self, ip: str) -> TopKnocks:
+    async def get_knocks(self, ip: str) -> GetKnocks:
         query = gql(
             """
-            query TopKnocks($ip: String!) {
+            query getKnocks($ip: String!) {
               topKnocks(ip: $ip) {
-                queryInfo {
-                  resultsAvailable
-                  resultsLimit
-                }
                 knock {
-                  tor_exit
-                  title
                   source_ip
-                  links
-                  last_seen
-                  last_crawled
-                  knock_port
-                  jarm
-                  ips
                   headers
-                  favicon_mmh3_32
-                  favicon_mmh3_128
-                  emails
                   apps
+                  emails
+                  favicon_mmh3_128
+                  favicon_mmh3_32
+                  ips
+                  knock_port
+                  jarm
+                  last_seen
+                  last_crawled
+                  links
+                  title
+                  tor_exit
                 }
               }
             }
             """
         )
         variables: dict[str, object] = {"ip": ip}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
-        return TopKnocks.parse_obj(data)
+        return GetKnocks.parse_obj(data)
 
-    async def noise_rank(self, ip: str) -> NoiseRank:
+    async def generate_g_n_q_l(self, input: str) -> GenerateGNQL:
         query = gql(
             """
-            query NoiseRank($ip: String!) {
+            query generateGNQL($input: String!) {
+              generateGNQL(input: $input) {
+                input_text
+                queries
+              }
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return GenerateGNQL.parse_obj(data)
+
+    async def get_noise_ranks(self, ip: str) -> GetNoiseRanks:
+        query = gql(
+            """
+            query getNoiseRanks($ip: String!) {
               noiseRank(ip: $ip) {
-                queryInfo {
-                  resultsAvailable
-                  resultsLimit
-                }
                 ips {
-                  country_pervasiveness
                   ip
                   noise_score
+                  country_pervasiveness
                   payload_diversity
                   port_diversity
                   request_rate
                   sensor_pervasiveness
                 }
               }
             }
             """
         )
         variables: dict[str, object] = {"ip": ip}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
-        return NoiseRank.parse_obj(data)
+        return GetNoiseRanks.parse_obj(data)
 
-    async def top_popular_i_ps(self) -> TopPopularIPs:
+    async def get_i_ps(self) -> GetIPs:
         query = gql(
             """
-            query TopPopularIPs {
+            query getIPs {
               topPopularIPs {
-                queryInfo {
-                  resultsAvailable
-                  resultsLimit
-                }
                 popularIPs {
                   ip
                   request_count
                   users_count
                 }
               }
             }
             """
         )
         variables: dict[str, object] = {}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
-        return TopPopularIPs.parse_obj(data)
+        return GetIPs.parse_obj(data)
```

### Comparing `greynoiselabs-0.1.0/src/greynoiselabs/exceptions.py` & `greynoiselabs-0.1.1/src/greynoiselabs/api/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-15 23:53
+# Generated by ariadne-codegen on 2023-06-28 15:55
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `greynoiselabs-0.1.0/src/greynoiselabs/noise_rank.py` & `greynoiselabs-0.1.1/src/greynoiselabs/api/noise_rank.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-15 23:53
+# Generated by ariadne-codegen on 2023-06-16 04:37
 # Source: queries
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.0/src/greynoiselabs/top_h_t_t_p_requests.py` & `greynoiselabs-0.1.1/src/greynoiselabs/api/top_h_t_t_p_requests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-15 23:53
+# Generated by ariadne-codegen on 2023-06-16 04:37
 # Source: queries
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.0/src/greynoiselabs/top_knocks.py` & `greynoiselabs-0.1.1/src/greynoiselabs/api/top_knocks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-15 23:53
+# Generated by ariadne-codegen on 2023-06-16 04:37
 # Source: queries
 
 from typing import Any, List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.0/src/greynoiselabs/top_popular_i_ps.py` & `greynoiselabs-0.1.1/src/greynoiselabs/api/top_popular_i_ps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-15 23:53
+# Generated by ariadne-codegen on 2023-06-16 04:37
 # Source: queries
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.0/src/greynoiselabs.egg-info/PKG-INFO` & `greynoiselabs-0.1.1/src/greynoiselabs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greynoiselabs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Abstraction to interact with GreyNoise Labs GraphQL API.
 Home-page: https://api.labs.greynoise.io/
 Author: GreyNoise Intelligence
 Author-email: labs@greynoise.io
 License: MIT
 Download-URL: https://github.com/GreyNoise-Intelligence/greynoiselabs
 Keywords: internet,scanning,threat intelligence,security
@@ -41,15 +41,15 @@
 
 .. _Documentation: https://api.labs.greynoise.io/1/docs/
 
 Quick Start
 ===========
 **Install the library**:
 
-``pip install labs-graphql-client`` or ``python setup.py install``
+``pip install greynoiselabs`` or ``python setup.py install``
 
 Example Code
 
 ..  code-block:: python
 
     import os
     import asyncio
@@ -62,13 +62,13 @@
     print(response)
 
 
 =========
 Changelog
 =========
 
-Version `dev`_
+Version `0.1.1`_
 ================
-**Date**: unreleased
+**Date**: July 27, 2023
 
-.. _`dev`: https://github.com/GreyNoise-Intelligence/labs-graphql-client/compare/v0.1.0...HEAD
+.. _`0.1.1`: https://github.com/GreyNoise-Intelligence/greynoiselabs/compare/v0.1.0...0.1.1
```

### Comparing `greynoiselabs-0.1.0/src/greynoiselabs.egg-info/SOURCES.txt` & `greynoiselabs-0.1.1/src/greynoiselabs.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 LICENSE
 README.rst
 setup.cfg
 setup.py
 src/greynoiselabs/__init__.py
 src/greynoiselabs/__version__.py
-src/greynoiselabs/async_base_client.py
-src/greynoiselabs/base_model.py
-src/greynoiselabs/client.py
-src/greynoiselabs/enums.py
-src/greynoiselabs/exceptions.py
-src/greynoiselabs/get_c2s.py
-src/greynoiselabs/input_types.py
-src/greynoiselabs/noise_rank.py
-src/greynoiselabs/scalars.py
-src/greynoiselabs/top_h_t_t_p_requests.py
-src/greynoiselabs/top_knocks.py
-src/greynoiselabs/top_popular_i_ps.py
 src/greynoiselabs.egg-info/PKG-INFO
 src/greynoiselabs.egg-info/SOURCES.txt
 src/greynoiselabs.egg-info/dependency_links.txt
+src/greynoiselabs.egg-info/entry_points.txt
 src/greynoiselabs.egg-info/not-zip-safe
 src/greynoiselabs.egg-info/requires.txt
-src/greynoiselabs.egg-info/top_level.txt
+src/greynoiselabs.egg-info/top_level.txt
+src/greynoiselabs/api/__init__.py
+src/greynoiselabs/api/async_base_client.py
+src/greynoiselabs/api/base_model.py
+src/greynoiselabs/api/client.py
+src/greynoiselabs/api/enums.py
+src/greynoiselabs/api/exceptions.py
+src/greynoiselabs/api/generate_g_n_q_l.py
+src/greynoiselabs/api/get_c2s.py
+src/greynoiselabs/api/get_i_ps.py
+src/greynoiselabs/api/get_knocks.py
+src/greynoiselabs/api/get_noise_ranks.py
+src/greynoiselabs/api/get_requests.py
+src/greynoiselabs/api/input_types.py
+src/greynoiselabs/api/noise_rank.py
+src/greynoiselabs/api/scalars.py
+src/greynoiselabs/api/top_h_t_t_p_requests.py
+src/greynoiselabs/api/top_knocks.py
+src/greynoiselabs/api/top_popular_i_ps.py
+src/greynoiselabs/cli/__init__.py
+src/greynoiselabs/cli/auth.py
+src/greynoiselabs/cli/main.py
```

