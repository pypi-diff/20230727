# Comparing `tmp/greynoiselabs-0.1.1.tar.gz` & `tmp/greynoiselabs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greynoiselabs-0.1.1.tar", last modified: Thu Jul 27 03:51:51 2023, max compression
+gzip compressed data, was "greynoiselabs-0.1.7.tar", last modified: Thu Jul 27 18:38:35 2023, max compression
```

## Comparing `greynoiselabs-0.1.1.tar` & `greynoiselabs-0.1.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:51:51.593615 greynoiselabs-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-27 03:51:51.593615 greynoiselabs-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-27 03:51:51.593615 greynoiselabs-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-27 03:51:41.000000 greynoiselabs-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:51:51.589615 greynoiselabs-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:51:51.589615 greynoiselabs-0.1.1/src/greynoiselabs/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-27 03:51:41.000000 greynoiselabs-0.1.1/src/greynoiselabs/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:51:51.593615 greynoiselabs-0.1.1/src/greynoiselabs/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/async_base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/generate_g_n_q_l.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/get_c2s.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/get_i_ps.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/get_knocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/get_noise_ranks.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/get_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/input_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/noise_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/scalars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/top_h_t_t_p_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/top_knocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/api/top_popular_i_ps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:51:51.593615 greynoiselabs-0.1.1/src/greynoiselabs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5763 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-07-27 03:51:21.000000 greynoiselabs-0.1.1/src/greynoiselabs/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:51:51.589615 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-27 03:51:51.000000 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-27 03:51:51.000000 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:51:51.000000 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 03:51:51.000000 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:51:51.000000 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-27 03:51:51.000000 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 03:51:51.000000 greynoiselabs-0.1.1/src/greynoiselabs.egg-info/top_level.txt
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.736639 greynoiselabs-0.1.7/
+-rw-r--r--   0 matt       (502) staff       (20)     1079 2023-06-16 04:21:17.000000 greynoiselabs-0.1.7/LICENSE
+-rw-r--r--   0 matt       (502) staff       (20)     2005 2023-07-27 18:38:35.736729 greynoiselabs-0.1.7/PKG-INFO
+-rw-r--r--   0 matt       (502) staff       (20)      960 2023-07-27 16:38:11.000000 greynoiselabs-0.1.7/README.rst
+-rw-r--r--   0 matt       (502) staff       (20)      281 2023-07-27 18:38:35.737016 greynoiselabs-0.1.7/setup.cfg
+-rw-r--r--   0 matt       (502) staff       (20)     1698 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/setup.py
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.729256 greynoiselabs-0.1.7/src/
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.730993 greynoiselabs-0.1.7/src/greynoiselabs/
+-rw-r--r--   0 matt       (502) staff       (20)        0 2023-07-27 04:05:43.000000 greynoiselabs-0.1.7/src/greynoiselabs/__init__.py
+-rw-r--r--   0 matt       (502) staff       (20)      254 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/__version__.py
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.736050 greynoiselabs-0.1.7/src/greynoiselabs/api/
+-rw-r--r--   0 matt       (502) staff       (20)     1611 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/__init__.py
+-rw-r--r--   0 matt       (502) staff       (20)     7371 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/async_base_client.py
+-rw-r--r--   0 matt       (502) staff       (20)     1951 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/base_model.py
+-rw-r--r--   0 matt       (502) staff       (20)     4181 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/client.py
+-rw-r--r--   0 matt       (502) staff       (20)       84 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/enums.py
+-rw-r--r--   0 matt       (502) staff       (20)     2366 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/exceptions.py
+-rw-r--r--   0 matt       (502) staff       (20)      461 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/generate_g_n_q_l.py
+-rw-r--r--   0 matt       (502) staff       (20)      593 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/get_c2s.py
+-rw-r--r--   0 matt       (502) staff       (20)      614 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/get_i_ps.py
+-rw-r--r--   0 matt       (502) staff       (20)      775 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/get_knocks.py
+-rw-r--r--   0 matt       (502) staff       (20)      689 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/get_noise_ranks.py
+-rw-r--r--   0 matt       (502) staff       (20)      755 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/get_requests.py
+-rw-r--r--   0 matt       (502) staff       (20)      221 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/input_types.py
+-rw-r--r--   0 matt       (502) staff       (20)      942 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/noise_rank.py
+-rw-r--r--   0 matt       (502) staff       (20)      220 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/scalars.py
+-rw-r--r--   0 matt       (502) staff       (20)     1138 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/top_h_t_t_p_requests.py
+-rw-r--r--   0 matt       (502) staff       (20)     1060 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/top_knocks.py
+-rw-r--r--   0 matt       (502) staff       (20)      993 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/top_popular_i_ps.py
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.736481 greynoiselabs-0.1.7/src/greynoiselabs/cli/
+-rw-r--r--   0 matt       (502) staff       (20)        0 2023-07-27 03:55:22.000000 greynoiselabs-0.1.7/src/greynoiselabs/cli/__init__.py
+-rwxr-xr-x   0 matt       (502) staff       (20)     5763 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/cli/auth.py
+-rw-r--r--   0 matt       (502) staff       (20)     4985 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/cli/main.py
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.732309 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/
+-rw-r--r--   0 matt       (502) staff       (20)     2005 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (502) staff       (20)     1148 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (502) staff       (20)        1 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (502) staff       (20)       61 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/entry_points.txt
+-rw-r--r--   0 matt       (502) staff       (20)        1 2023-07-27 03:56:32.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/not-zip-safe
+-rw-r--r--   0 matt       (502) staff       (20)      246 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/requires.txt
+-rw-r--r--   0 matt       (502) staff       (20)       14 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/top_level.txt
```

### Comparing `greynoiselabs-0.1.1/LICENSE` & `greynoiselabs-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `greynoiselabs-0.1.1/PKG-INFO` & `greynoiselabs-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: greynoiselabs
-Version: 0.1.1
+Version: 0.1.7
 Summary: Abstraction to interact with GreyNoise Labs GraphQL API.
 Home-page: https://api.labs.greynoise.io/
+Download-URL: https://github.com/GreyNoise-Intelligence/greynoiselabs
 Author: GreyNoise Intelligence
 Author-email: labs@greynoise.io
 License: MIT
-Download-URL: https://github.com/GreyNoise-Intelligence/greynoiselabs
 Keywords: internet,scanning,threat intelligence,security
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -58,17 +57,7 @@
     client = Client("https://api.labs.greynoise.io/1/query",
                     {"Authorization": f"Bearer {os.environ['AUTH_TOKEN']}"})
 
     response = asyncio.run(client.top_knocks(ip="221.144.229.187"))
     print(response)
 
 
-=========
-Changelog
-=========
-
-Version `0.1.1`_
-================
-**Date**: July 27, 2023
-
-.. _`0.1.1`: https://github.com/GreyNoise-Intelligence/greynoiselabs/compare/v0.1.0...0.1.1
-
```

### Comparing `greynoiselabs-0.1.1/README.rst` & `greynoiselabs-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `greynoiselabs-0.1.1/setup.py` & `greynoiselabs-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 
 
 def read(fname):
     """Read file and return its contents."""
     with open(os.path.join(os.path.dirname(__file__), fname)) as input_file:
         return input_file.read()
 
+
 setup(
     name="greynoiselabs",
-    version="0.1.1",
+    version="0.1.7",
     description="Abstraction to interact with GreyNoise Labs GraphQL API.",
     url="https://api.labs.greynoise.io/",
     author="GreyNoise Intelligence",
     author_email="labs@greynoise.io",
     license="MIT",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     install_requires=read("requirements/common.txt").split("\n"),
-    long_description=read("README.rst") + "\n\n" + read("CHANGELOG.rst"),
+    long_description=read("README.rst") + "\n\n" + read("CHANGELOG.md"),
     python_requires=">=3.0, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python",
```

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/__init__.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-26 20:32
+# Generated by ariadne-codegen on 2023-07-27 18:00
 
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel
 from .client import Client
 from .exceptions import (
     GraphQLClientError,
     GraphQLClientGraphQLError,
```

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/api/async_base_client.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-28 15:55
+# Generated by ariadne-codegen on 2023-07-27 18:00
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/api/base_model.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-28 15:55
+# Generated by ariadne-codegen on 2023-07-27 18:00
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/api/client.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-28 15:55
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from .async_base_client import AsyncBaseClient
 from .generate_g_n_q_l import GenerateGNQL
 from .get_c2s import GetC2s
 from .get_i_ps import GetIPs
 from .get_knocks import GetKnocks
```

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/api/exceptions.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-28 15:55
+# Generated by ariadne-codegen on 2023-07-27 18:00
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/api/get_c2s.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/get_c2s.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-28 15:55
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/api/get_i_ps.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/get_i_ps.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-28 15:55
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/api/get_knocks.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/get_knocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-28 15:55
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from typing import Any, List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/api/get_noise_ranks.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/get_noise_ranks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-28 15:55
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/api/get_requests.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/get_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-28 15:55
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/api/noise_rank.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/noise_rank.py`

 * *Files identical despite different names*

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/api/top_h_t_t_p_requests.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/top_h_t_t_p_requests.py`

 * *Files identical despite different names*

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/api/top_knocks.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/top_knocks.py`

 * *Files identical despite different names*

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/api/top_popular_i_ps.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/top_popular_i_ps.py`

 * *Files identical despite different names*

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/cli/auth.py` & `greynoiselabs-0.1.7/src/greynoiselabs/cli/auth.py`

 * *Files identical despite different names*

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs/cli/main.py` & `greynoiselabs-0.1.7/src/greynoiselabs/cli/main.py`

 * *Files identical despite different names*

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs.egg-info/PKG-INFO` & `greynoiselabs-0.1.7/src/greynoiselabs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: greynoiselabs
-Version: 0.1.1
+Version: 0.1.7
 Summary: Abstraction to interact with GreyNoise Labs GraphQL API.
 Home-page: https://api.labs.greynoise.io/
+Download-URL: https://github.com/GreyNoise-Intelligence/greynoiselabs
 Author: GreyNoise Intelligence
 Author-email: labs@greynoise.io
 License: MIT
-Download-URL: https://github.com/GreyNoise-Intelligence/greynoiselabs
 Keywords: internet,scanning,threat intelligence,security
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -58,17 +57,7 @@
     client = Client("https://api.labs.greynoise.io/1/query",
                     {"Authorization": f"Bearer {os.environ['AUTH_TOKEN']}"})
 
     response = asyncio.run(client.top_knocks(ip="221.144.229.187"))
     print(response)
 
 
-=========
-Changelog
-=========
-
-Version `0.1.1`_
-================
-**Date**: July 27, 2023
-
-.. _`0.1.1`: https://github.com/GreyNoise-Intelligence/greynoiselabs/compare/v0.1.0...0.1.1
-
```

### Comparing `greynoiselabs-0.1.1/src/greynoiselabs.egg-info/SOURCES.txt` & `greynoiselabs-0.1.7/src/greynoiselabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

