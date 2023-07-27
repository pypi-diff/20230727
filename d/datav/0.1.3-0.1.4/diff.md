# Comparing `tmp/datav-0.1.3.tar.gz` & `tmp/datav-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datav-0.1.3.tar", last modified: Wed Mar 30 10:17:03 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `datav-0.1.3.tar` & `datav-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 tcztzy    (1000) tcztzy    (1000)        0 2022-03-30 10:17:03.482940 datav-0.1.3/
--rw-r--r--   0 tcztzy    (1000) tcztzy    (1000)     7650 2022-03-18 14:54:26.000000 datav-0.1.3/LICENSE
--rw-r--r--   0 tcztzy    (1000) tcztzy    (1000)    13142 2022-03-30 10:17:03.482940 datav-0.1.3/PKG-INFO
--rw-r--r--   0 tcztzy    (1000) tcztzy    (1000)     3357 2022-03-18 07:04:10.000000 datav-0.1.3/README.md
-drwxr-xr-x   0 tcztzy    (1000) tcztzy    (1000)        0 2022-03-30 10:17:03.482940 datav-0.1.3/datav.egg-info/
--rw-r--r--   0 tcztzy    (1000) tcztzy    (1000)    13142 2022-03-30 10:17:02.000000 datav-0.1.3/datav.egg-info/PKG-INFO
--rw-r--r--   0 tcztzy    (1000) tcztzy    (1000)      185 2022-03-30 10:17:03.000000 datav-0.1.3/datav.egg-info/SOURCES.txt
--rw-r--r--   0 tcztzy    (1000) tcztzy    (1000)        1 2022-03-30 10:17:03.000000 datav-0.1.3/datav.egg-info/dependency_links.txt
--rw-r--r--   0 tcztzy    (1000) tcztzy    (1000)       36 2022-03-30 10:17:03.000000 datav-0.1.3/datav.egg-info/requires.txt
--rw-r--r--   0 tcztzy    (1000) tcztzy    (1000)        6 2022-03-30 10:17:03.000000 datav-0.1.3/datav.egg-info/top_level.txt
--rwxr-xr-x   0 tcztzy    (1000) tcztzy    (1000)     5212 2022-03-18 07:05:25.000000 datav-0.1.3/datav.py
--rw-r--r--   0 tcztzy    (1000) tcztzy    (1000)     1014 2022-03-30 10:06:26.000000 datav-0.1.3/pyproject.toml
--rw-r--r--   0 tcztzy    (1000) tcztzy    (1000)       38 2022-03-30 10:17:03.482940 datav-0.1.3/setup.cfg
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 datav-0.1.4/CHANGELOG
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 datav-0.1.4/requirements-dev.lock
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 datav-0.1.4/requirements.lock
+-rw-r--r--   0        0        0  1126690 2020-02-02 00:00:00.000000 datav-0.1.4/research_site.png
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 datav-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 datav-0.1.4/.github/workflows/qa.yml
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 datav-0.1.4/examples/alaer.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 datav-0.1.4/src/datav/__init__.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 datav-0.1.4/src/datav/downloader.py
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 datav-0.1.4/src/datav/feature.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 datav-0.1.4/.gitignore
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 datav-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 datav-0.1.4/README.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 datav-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 datav-0.1.4/PKG-INFO
```

### Comparing `datav-0.1.3/LICENSE` & `datav-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datav-0.1.3/PKG-INFO` & `datav-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: datav
-Version: 0.1.3
-Summary: This is an unofficial solution to draw map using Aliyun's DataV.GeoAtlas.
+Version: 0.1.4
+Summary: Data visualization tools for Python.
 Author-email: Tang Ziya <tcztzy@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -164,39 +164,50 @@
         General Public License ever published by the Free Software Foundation.
         
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
-Platform: UNKNOWN
+License-File: LICENSE
 Classifier: Framework :: Matplotlib
-Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free For Educational Use
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Requires-Dist: cartopy>=0.21.1
+Requires-Dist: geopandas>=0.13.2
+Requires-Dist: numba>=0.57.1
+Requires-Dist: spatialpandas>=0.4.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 DataV
 -----
+![PyPI](https://img.shields.io/pypi/v/datav)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/datav)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/datav)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/datav)
+![License](https://img.shields.io/github/license/tcztzy/datav)
 
 This is an unofficial solution to draw map using Aliyun's DataV.GeoAtlas.
 
 这是一个非官方的使用阿里云 DataV.GeoAtlas 绘制地图的解决方案。
 
 
 ## Examples
 
+See [examples](examples) for more.
+
 ```python
 import cartopy.crs as ccrs
 import cartopy.feature as cfeature
 import matplotlib.pyplot as plt
 import numpy as np
 from cartopy.mpl.gridliner import LATITUDE_FORMATTER, LONGITUDE_FORMATTER
 from matplotlib.transforms import offset_copy
@@ -287,9 +298,7 @@
 2. Chinese name alias for adcode
 
    使用中文名替代 adcode 查询
 
 3. More features such as line
 
    从 GeoJSON 中提取更多可定制的 feature。
-
-
```

### Comparing `datav-0.1.3/README.md` & `datav-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 DataV
 -----
+![PyPI](https://img.shields.io/pypi/v/datav)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/datav)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/datav)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/datav)
+![License](https://img.shields.io/github/license/tcztzy/datav)
 
 This is an unofficial solution to draw map using Aliyun's DataV.GeoAtlas.
 
 这是一个非官方的使用阿里云 DataV.GeoAtlas 绘制地图的解决方案。
 
 
 ## Examples
 
+See [examples](examples) for more.
+
 ```python
 import cartopy.crs as ccrs
 import cartopy.feature as cfeature
 import matplotlib.pyplot as plt
 import numpy as np
 from cartopy.mpl.gridliner import LATITUDE_FORMATTER, LONGITUDE_FORMATTER
 from matplotlib.transforms import offset_copy
```

