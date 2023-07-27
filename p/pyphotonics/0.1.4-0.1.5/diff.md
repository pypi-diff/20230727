# Comparing `tmp/pyphotonics-0.1.4.tar.gz` & `tmp/pyphotonics-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyphotonics-0.1.4.tar", last modified: Tue Aug  3 01:29:47 2021, max compression
+gzip compressed data, was "pyphotonics-0.1.5.tar", last modified: Thu Jul 27 07:12:08 2023, max compression
```

## Comparing `pyphotonics-0.1.4.tar` & `pyphotonics-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,17 @@
-drwxrwxrwx   0 sherif    (1000) sherif    (1000)        0 2021-08-03 01:29:47.532078 pyphotonics-0.1.4/
--rwxrwxrwx   0 sherif    (1000) sherif    (1000)      551 2021-08-03 01:29:47.533075 pyphotonics-0.1.4/PKG-INFO
-drwxrwxrwx   0 sherif    (1000) sherif    (1000)        0 2021-08-03 01:29:47.531080 pyphotonics-0.1.4/pyphotonics/
--rwxrwxrwx   0 sherif    (1000) sherif    (1000)       22 2021-08-03 01:29:40.310906 pyphotonics-0.1.4/pyphotonics/__init__.py
--rwxrwxrwx   0 sherif    (1000) sherif    (1000)     3088 2021-08-02 04:01:57.101000 pyphotonics-0.1.4/pyphotonics/configuration_coordinate.py
--rwxrwxrwx   0 sherif    (1000) sherif    (1000)       66 2021-08-02 04:01:57.242000 pyphotonics-0.1.4/pyphotonics/constants.py
--rwxrwxrwx   0 sherif    (1000) sherif    (1000)     6978 2021-08-03 01:28:51.448150 pyphotonics-0.1.4/pyphotonics/photoluminescence.py
--rwxrwxrwx   0 sherif    (1000) sherif    (1000)     2064 2021-08-02 04:02:12.848000 pyphotonics-0.1.4/pyphotonics/schrodinger.py
--rwxrwxrwx   0 sherif    (1000) sherif    (1000)      553 2021-08-03 00:27:27.588000 pyphotonics-0.1.4/pyphotonics/xyz.py
--rwxrwxrwx   0 sherif    (1000) sherif    (1000)        0 2021-08-02 03:52:28.422969 pyphotonics-0.1.4/setup.cfg
--rwxrwxrwx   0 sherif    (1000) sherif    (1000)      747 2021-08-03 01:29:16.979673 pyphotonics-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:12:08.023450 pyphotonics-0.1.5/
+-rw-rw-rw-   0        0        0        0 2023-05-25 04:36:44.000000 pyphotonics-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      548 2023-07-27 07:12:08.023450 pyphotonics-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3073 2023-05-25 04:36:44.000000 pyphotonics-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 07:12:08.011450 pyphotonics-0.1.5/pyphotonics/
+-rw-rw-rw-   0        0        0       23 2023-07-27 05:42:52.000000 pyphotonics-0.1.5/pyphotonics/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-27 05:47:04.000000 pyphotonics-0.1.5/pyphotonics/__main__.py
+-rw-rw-rw-   0        0        0       68 2023-05-25 04:36:44.000000 pyphotonics-0.1.5/pyphotonics/constants.py
+-rw-rw-rw-   0        0        0     7057 2023-07-27 07:07:49.000000 pyphotonics-0.1.5/pyphotonics/photoluminescence.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:12:08.021450 pyphotonics-0.1.5/pyphotonics.egg-info/
+-rw-rw-rw-   0        0        0      548 2023-07-27 07:12:07.000000 pyphotonics-0.1.5/pyphotonics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-27 07:12:07.000000 pyphotonics-0.1.5/pyphotonics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 07:12:07.000000 pyphotonics-0.1.5/pyphotonics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-27 07:12:07.000000 pyphotonics-0.1.5/pyphotonics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-27 07:12:07.000000 pyphotonics-0.1.5/pyphotonics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 07:12:08.024450 pyphotonics-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      762 2023-07-27 07:11:38.000000 pyphotonics-0.1.5/setup.py
```

### Comparing `pyphotonics-0.1.4/PKG-INFO` & `pyphotonics-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 1.0
-Name: pyphotonics
-Version: 0.1.4
-Summary: The PyPhotonics python code is a post-processing code written entirely in python which takes as input the output files of the VASP and phonopy codes for a defect system, and calculates the Huang-Rhys factor and the PL lineshapes for that system.
-Home-page: https://github.com/sheriftawfikabbas/pyphotonics
-Author: Sherif Abdulkader Tawfik
-Author-email: sherif.tawfic@gmail.com
-License: gpl-3.0
-Description: UNKNOWN
-Keywords: DFT,Material science,Photoluminescence,VASP
-Platform: UNKNOWN
+Metadata-Version: 2.1
+Name: pyphotonics
+Version: 0.1.5
+Summary: The PyPhotonics python code is a post-processing code written entirely in python which takes as input the output files of the VASP and phonopy codes for a defect system, and calculates the Huang-Rhys factor and the PL lineshapes for that system.
+Home-page: https://github.com/sheriftawfikabbas/pyphotonics
+Author: Sherif Abdulkader Tawfik
+Author-email: sherif.tawfic@gmail.com
+License: gpl-3.0
+Keywords: DFT,Material science,Photoluminescence,VASP
+License-File: LICENSE.txt
```

