# Comparing `tmp/solo_epd_loader-0.3.4.tar.gz` & `tmp/solo_epd_loader-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-kdtqsuqj/solo_epd_loader-0.3.4.tar", last modified: Mon Jul 24 13:34:24 2023, max compression
+gzip compressed data, was "solo_epd_loader-0.3.5.tar", last modified: Thu Jul 27 14:11:26 2023, max compression
```

## Comparing `solo_epd_loader-0.3.4.tar` & `solo_epd_loader-0.3.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.894011 solo_epd_loader-0.3.4/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.4/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.4/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16742 2023-07-24 13:34:24.898011 solo_epd_loader-0.3.4/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15894 2023-07-20 13:53:21.000000 solo_epd_loader-0.3.4/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.3.4/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.882011 solo_epd_loader-0.3.4/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.4/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.4/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.3.4/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.4/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.886011 solo_epd_loader-0.3.4/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.3.4/examples/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.3.4/examples/ws2021_fig_2d.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.3.4/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.3.4/gh2021_fig_2a.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.886011 solo_epd_loader-0.3.4/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.4/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2023-07-05 12:35:18.000000 solo_epd_loader-0.3.4/licenses/SUNPY_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.4/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.4/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       89 2023-07-24 13:24:35.000000 solo_epd_loader-0.3.4/requirements.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2209 2023-07-24 13:34:24.898011 solo_epd_loader-0.3.4/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.4/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.890011 solo_epd_loader-0.3.4/solo_epd_loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    83025 2023-07-24 12:55:49.000000 solo_epd_loader-0.3.4/solo_epd_loader/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.874011 solo_epd_loader-0.3.4/solo_epd_loader/data/
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.874011 solo_epd_loader-0.3.4/solo_epd_loader/data/test/
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.874011 solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.874011 solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.894011 solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/ept/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   104579 2022-06-20 13:33:16.000000 solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-asun-rates_20200603_V02.cdf
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   107761 2022-06-20 13:33:23.000000 solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-north-rates_20200603_V02.cdf
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   104907 2022-06-20 13:33:32.000000 solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-south-rates_20200603_V02.cdf
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   103697 2022-06-20 13:33:39.000000 solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-sun-rates_20200603_V02.cdf
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.894011 solo_epd_loader-0.3.4/solo_epd_loader/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.4/solo_epd_loader/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     9850 2023-07-24 13:16:47.000000 solo_epd_loader-0.3.4/solo_epd_loader/tests/tests.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-07-24 13:34:24.000000 solo_epd_loader-0.3.4/solo_epd_loader/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-24 13:34:24.890011 solo_epd_loader-0.3.4/solo_epd_loader.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16742 2023-07-24 13:34:24.000000 solo_epd_loader-0.3.4/solo_epd_loader.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1011 2023-07-24 13:34:24.000000 solo_epd_loader-0.3.4/solo_epd_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-07-24 13:34:24.000000 solo_epd_loader-0.3.4/solo_epd_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.3.4/solo_epd_loader.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      175 2023-07-24 13:34:24.000000 solo_epd_loader-0.3.4/solo_epd_loader.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-07-24 13:34:24.000000 solo_epd_loader-0.3.4/solo_epd_loader.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.3.4/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-27 14:11:26.318010 solo_epd_loader-0.3.5/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.5/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.5/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    17027 2023-07-27 14:11:26.318010 solo_epd_loader-0.3.5/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16179 2023-07-27 14:07:51.000000 solo_epd_loader-0.3.5/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.3.5/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-27 14:11:26.310010 solo_epd_loader-0.3.5/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.5/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.5/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.3.5/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.5/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-27 14:11:26.314010 solo_epd_loader-0.3.5/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.3.5/examples/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.3.5/examples/ws2021_fig_2d.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.3.5/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.3.5/gh2021_fig_2a.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-27 14:11:26.314010 solo_epd_loader-0.3.5/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.5/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2023-07-05 12:35:18.000000 solo_epd_loader-0.3.5/licenses/SUNPY_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.5/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.5/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       89 2023-07-24 13:24:35.000000 solo_epd_loader-0.3.5/requirements.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2036 2023-07-27 14:11:26.322010 solo_epd_loader-0.3.5/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.5/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-27 14:11:26.314010 solo_epd_loader-0.3.5/solo_epd_loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    83194 2023-07-27 14:06:05.000000 solo_epd_loader-0.3.5/solo_epd_loader/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-27 14:11:26.298010 solo_epd_loader-0.3.5/solo_epd_loader/data/
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-27 14:11:26.298010 solo_epd_loader-0.3.5/solo_epd_loader/data/test/
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-27 14:11:26.298010 solo_epd_loader-0.3.5/solo_epd_loader/data/test/l2/
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-27 14:11:26.298010 solo_epd_loader-0.3.5/solo_epd_loader/data/test/l2/epd/
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-27 14:11:26.318010 solo_epd_loader-0.3.5/solo_epd_loader/data/test/l2/epd/ept/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   104579 2022-06-20 13:33:16.000000 solo_epd_loader-0.3.5/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-asun-rates_20200603_V02.cdf
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   107761 2022-06-20 13:33:23.000000 solo_epd_loader-0.3.5/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-north-rates_20200603_V02.cdf
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   104907 2022-06-20 13:33:32.000000 solo_epd_loader-0.3.5/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-south-rates_20200603_V02.cdf
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   103697 2022-06-20 13:33:39.000000 solo_epd_loader-0.3.5/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-sun-rates_20200603_V02.cdf
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-27 14:11:26.318010 solo_epd_loader-0.3.5/solo_epd_loader/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.5/solo_epd_loader/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     9850 2023-07-24 13:16:47.000000 solo_epd_loader-0.3.5/solo_epd_loader/tests/tests.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-07-27 14:11:26.000000 solo_epd_loader-0.3.5/solo_epd_loader/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-27 14:11:26.314010 solo_epd_loader-0.3.5/solo_epd_loader.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    17027 2023-07-27 14:11:26.000000 solo_epd_loader-0.3.5/solo_epd_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1011 2023-07-27 14:11:26.000000 solo_epd_loader-0.3.5/solo_epd_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-07-27 14:11:26.000000 solo_epd_loader-0.3.5/solo_epd_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.3.5/solo_epd_loader.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      175 2023-07-27 14:11:26.000000 solo_epd_loader-0.3.5/solo_epd_loader.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-07-27 14:11:26.000000 solo_epd_loader-0.3.5/solo_epd_loader.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.3.5/tox.ini
```

### Comparing `solo_epd_loader-0.3.4/LICENSE.rst` & `solo_epd_loader-0.3.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/PKG-INFO` & `solo_epd_loader-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo_epd_loader
-Version: 0.3.4
+Version: 0.3.5
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -20,25 +20,28 @@
 Provides-Extra: test
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
 solo-epd-loader
 ===============
 
-|pypi Version| |conda version| |license| |python version| |zenodo doi|
+|pypi Version| |conda version| |python version| |pytest| |codecov| |license| |zenodo doi|
 
 .. |pypi Version| image:: https://img.shields.io/pypi/v/solo-epd-loader?style=flat&logo=pypi
    :target: https://pypi.org/project/solo-epd-loader/
 .. |conda version| image:: https://img.shields.io/conda/vn/conda-forge/solo-epd-loader?style=flat&logo=anaconda
    :target: https://anaconda.org/conda-forge/solo-epd-loader/
 .. |license| image:: https://img.shields.io/conda/l/conda-forge/solo-epd-loader?style=flat
    :target: https://github.com/jgieseler/solo-epd-loader/blob/main/LICENSE.rst
 .. |python version| image:: https://img.shields.io/pypi/pyversions/solo-epd-loader?style=flat&logo=python
 .. |zenodo doi| image:: https://zenodo.org/badge/446889843.svg
    :target: https://zenodo.org/badge/latestdoi/446889843
+.. |pytest| image:: https://github.com/jgieseler/solo-epd-loader/workflows/pytest/badge.svg
+.. |codecov| image:: https://codecov.io/gh/jgieseler/solo-epd-loader/branch/main/graph/badge.svg?token=Z8dueEWqKS
+   :target: https://codecov.io/gh/jgieseler/solo-epd-loader
 
 Python data loader for Solar Orbiter's (SolO) `Energetic Particle Detector (EPD) <http://espada.uah.es/epd/>`_. At the moment provides level 2 (l2) and low latency (ll) data (`more details on data levels here <http://espada.uah.es/epd/EPD_data_overview.php>`_) obtained through CDF files from ESA's `Solar Orbiter Archive (SOAR) <http://soar.esac.esa.int/soar>`_ for the following sensors:
 
 - Electron Proton Telescope (EPT)
 - High Energy Telescope (HET)
 - SupraThermal Electrons and Protons (STEP)
```

### Comparing `solo_epd_loader-0.3.4/README.rst` & `solo_epd_loader-0.3.5/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 solo-epd-loader
 ===============
 
-|pypi Version| |conda version| |license| |python version| |zenodo doi|
+|pypi Version| |conda version| |python version| |pytest| |codecov| |license| |zenodo doi|
 
 .. |pypi Version| image:: https://img.shields.io/pypi/v/solo-epd-loader?style=flat&logo=pypi
    :target: https://pypi.org/project/solo-epd-loader/
 .. |conda version| image:: https://img.shields.io/conda/vn/conda-forge/solo-epd-loader?style=flat&logo=anaconda
    :target: https://anaconda.org/conda-forge/solo-epd-loader/
 .. |license| image:: https://img.shields.io/conda/l/conda-forge/solo-epd-loader?style=flat
    :target: https://github.com/jgieseler/solo-epd-loader/blob/main/LICENSE.rst
 .. |python version| image:: https://img.shields.io/pypi/pyversions/solo-epd-loader?style=flat&logo=python
 .. |zenodo doi| image:: https://zenodo.org/badge/446889843.svg
    :target: https://zenodo.org/badge/latestdoi/446889843
+.. |pytest| image:: https://github.com/jgieseler/solo-epd-loader/workflows/pytest/badge.svg
+.. |codecov| image:: https://codecov.io/gh/jgieseler/solo-epd-loader/branch/main/graph/badge.svg?token=Z8dueEWqKS
+   :target: https://codecov.io/gh/jgieseler/solo-epd-loader
 
 Python data loader for Solar Orbiter's (SolO) `Energetic Particle Detector (EPD) <http://espada.uah.es/epd/>`_. At the moment provides level 2 (l2) and low latency (ll) data (`more details on data levels here <http://espada.uah.es/epd/EPD_data_overview.php>`_) obtained through CDF files from ESA's `Solar Orbiter Archive (SOAR) <http://soar.esac.esa.int/soar>`_ for the following sensors:
 
 - Electron Proton Telescope (EPT)
 - High Energy Telescope (HET)
 - SupraThermal Electrons and Protons (STEP)
```

### Comparing `solo_epd_loader-0.3.4/code_of_conduct.md` & `solo_epd_loader-0.3.5/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/docs/Makefile` & `solo_epd_loader-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/docs/conf.py` & `solo_epd_loader-0.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/docs/make.bat` & `solo_epd_loader-0.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/examples/gh2021_fig_2.png` & `solo_epd_loader-0.3.5/examples/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/examples/ws2021_fig_2d.png` & `solo_epd_loader-0.3.5/examples/ws2021_fig_2d.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/gh2021_fig_2.png` & `solo_epd_loader-0.3.5/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/gh2021_fig_2a.png` & `solo_epd_loader-0.3.5/gh2021_fig_2a.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/licenses/LICENSE.rst` & `solo_epd_loader-0.3.5/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/licenses/SUNPY_LICENSE.rst` & `solo_epd_loader-0.3.5/licenses/SUNPY_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/licenses/TEMPLATE_LICENSE.rst` & `solo_epd_loader-0.3.5/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/setup.py` & `solo_epd_loader-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/solo_epd_loader/__init__.py` & `solo_epd_loader-0.3.5/solo_epd_loader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1029,15 +1029,20 @@
         # if not only_averages:
         for i in range(1, 16):
             Electron_Flux_Mult['Electron_'+str(i).rjust(2, '0')+'_Flux_Mult'] = cdf['Electron_'+str(i).rjust(2, '0')+'_Flux_Mult']
         # df_Electron_Flux_Mult = pd.DataFrame(Electron_Flux_Mult)  # get dataframe from dict - not needed atm.
 
         meta['Electron_Flux_Mult'] = Electron_Flux_Mult
 
-    if 'RTN' in cdf.cdf_info().zVariables:
+    if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+        zvars = cdf.cdf_info().zVariables
+    else:
+        zvars = cdf.cdf_info()['zVariables']
+
+    if 'RTN' in zvars:
         meta['df_rtn_desc'] = cdf.varattsget('RTN')['CATDESC']
 
     del cdf
 
     df = pd.DataFrame()
     df_rtn = pd.DataFrame()
     df_hci = pd.DataFrame()
```

### Comparing `solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-asun-rates_20200603_V02.cdf` & `solo_epd_loader-0.3.5/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-asun-rates_20200603_V02.cdf`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-north-rates_20200603_V02.cdf` & `solo_epd_loader-0.3.5/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-north-rates_20200603_V02.cdf`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-south-rates_20200603_V02.cdf` & `solo_epd_loader-0.3.5/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-south-rates_20200603_V02.cdf`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-sun-rates_20200603_V02.cdf` & `solo_epd_loader-0.3.5/solo_epd_loader/data/test/l2/epd/ept/solo_L2_epd-ept-sun-rates_20200603_V02.cdf`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/solo_epd_loader/tests/tests.py` & `solo_epd_loader-0.3.5/solo_epd_loader/tests/tests.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/solo_epd_loader.egg-info/PKG-INFO` & `solo_epd_loader-0.3.5/solo_epd_loader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo-epd-loader
-Version: 0.3.4
+Version: 0.3.5
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -20,25 +20,28 @@
 Provides-Extra: test
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
 solo-epd-loader
 ===============
 
-|pypi Version| |conda version| |license| |python version| |zenodo doi|
+|pypi Version| |conda version| |python version| |pytest| |codecov| |license| |zenodo doi|
 
 .. |pypi Version| image:: https://img.shields.io/pypi/v/solo-epd-loader?style=flat&logo=pypi
    :target: https://pypi.org/project/solo-epd-loader/
 .. |conda version| image:: https://img.shields.io/conda/vn/conda-forge/solo-epd-loader?style=flat&logo=anaconda
    :target: https://anaconda.org/conda-forge/solo-epd-loader/
 .. |license| image:: https://img.shields.io/conda/l/conda-forge/solo-epd-loader?style=flat
    :target: https://github.com/jgieseler/solo-epd-loader/blob/main/LICENSE.rst
 .. |python version| image:: https://img.shields.io/pypi/pyversions/solo-epd-loader?style=flat&logo=python
 .. |zenodo doi| image:: https://zenodo.org/badge/446889843.svg
    :target: https://zenodo.org/badge/latestdoi/446889843
+.. |pytest| image:: https://github.com/jgieseler/solo-epd-loader/workflows/pytest/badge.svg
+.. |codecov| image:: https://codecov.io/gh/jgieseler/solo-epd-loader/branch/main/graph/badge.svg?token=Z8dueEWqKS
+   :target: https://codecov.io/gh/jgieseler/solo-epd-loader
 
 Python data loader for Solar Orbiter's (SolO) `Energetic Particle Detector (EPD) <http://espada.uah.es/epd/>`_. At the moment provides level 2 (l2) and low latency (ll) data (`more details on data levels here <http://espada.uah.es/epd/EPD_data_overview.php>`_) obtained through CDF files from ESA's `Solar Orbiter Archive (SOAR) <http://soar.esac.esa.int/soar>`_ for the following sensors:
 
 - Electron Proton Telescope (EPT)
 - High Energy Telescope (HET)
 - SupraThermal Electrons and Protons (STEP)
```

### Comparing `solo_epd_loader-0.3.4/solo_epd_loader.egg-info/SOURCES.txt` & `solo_epd_loader-0.3.5/solo_epd_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.3.4/tox.ini` & `solo_epd_loader-0.3.5/tox.ini`

 * *Files identical despite different names*

