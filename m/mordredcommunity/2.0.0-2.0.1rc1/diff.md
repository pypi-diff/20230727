# Comparing `tmp/mordredcommunity-2.0.0.tar.gz` & `tmp/mordredcommunity-2.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mordredcommunity-2.0.0.tar", last modified: Fri Jul 21 16:38:58 2023, max compression
+gzip compressed data, was "mordredcommunity-2.0.1rc1.tar", last modified: Thu Jul 27 21:07:14 2023, max compression
```

## Comparing `mordredcommunity-2.0.0.tar` & `mordredcommunity-2.0.1rc1.tar`

### file list

```diff
@@ -1,107 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.311249 mordredcommunity-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-21 16:38:58.311249 mordredcommunity-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.299249 mordredcommunity-2.0.0/mordred/
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/ABCIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/AcidBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/AdjacencyMatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Aromatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/AtomCount.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/BCUT.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/BalabanJ.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/BaryszMatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/BertzCT.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/BondCount.py
--rw-r--r--   0 runner    (1001) docker     (123)     9304 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/CPSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/CarbonTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Chi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Constitutional.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/DetourMatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/DistanceMatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/EState.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/EccentricConnectivityIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)    20747 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/ExtendedTopochemicalAtom.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/FragmentComplexity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/GeometricalIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/GravitationalIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/HydrogenBond.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/InformationContent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/KappaShapeIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Lipinski.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/LogS.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/McGowanVolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/MoRSE.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/MoeType.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/MolecularDistanceEdge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/MolecularId.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/MomentOfInertia.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/PBF.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/PathCount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Polarizability.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/RingCount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/RotatableBond.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/SLogP.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/TopoPSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/TopologicalCharge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/TopologicalIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/VdwVolumeABC.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/VertexAdjacencyInformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/WalkCount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Weight.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/WienerIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/ZagrebIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_atomic_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.299249 mordredcommunity-2.0.0/mordred/_base/
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/pandas_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/result.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_graph_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_matrix_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.299249 mordredcommunity-2.0.0/mordred/descriptors/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/descriptors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.303249 mordredcommunity-2.0.0/mordred/error/
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.303249 mordredcommunity-2.0.0/mordred/surface_area/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/surface_area/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/surface_area/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/surface_area/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/surface_area/_sasa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.307249 mordredcommunity-2.0.0/mordred/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/Dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_ABCIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_ETA.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_SASA.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_SLogP.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_VEA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_atomic_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_by_references.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_compose_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_import_all_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_mordred_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_result_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.311249 mordredcommunity-2.0.0/mordredcommunity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-21 16:38:58.000000 mordredcommunity-2.0.0/mordredcommunity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-21 16:38:58.000000 mordredcommunity-2.0.0/mordredcommunity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:38:58.000000 mordredcommunity-2.0.0/mordredcommunity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-21 16:38:58.000000 mordredcommunity-2.0.0/mordredcommunity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 16:38:58.000000 mordredcommunity-2.0.0/mordredcommunity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 16:38:58.311249 mordredcommunity-2.0.0/setup.cfg
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.207553 mordredcommunity-2.0.1rc1/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1493 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/LICENSE
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)     5756 2023-07-27 21:07:14.207553 mordredcommunity-2.0.1rc1/PKG-INFO
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     5144 2023-07-21 16:14:04.000000 mordredcommunity-2.0.1rc1/README.md
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.183553 mordredcommunity-2.0.1rc1/mordred/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1954 2023-07-21 14:50:39.000000 mordredcommunity-2.0.1rc1/mordred/ABCIndex.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1810 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/AcidBase.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1394 2023-07-21 16:05:36.000000 mordredcommunity-2.0.1rc1/mordred/AdjacencyMatrix.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      947 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Aromatic.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2949 2023-07-21 14:53:32.000000 mordredcommunity-2.0.1rc1/mordred/AtomCount.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     7796 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Autocorrelation.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     3003 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/BCUT.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      733 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/BalabanJ.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2410 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/BaryszMatrix.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      711 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/BertzCT.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2711 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/BondCount.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     9304 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/CPSA.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     3502 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/CarbonTypes.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     6216 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Chi.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1882 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Constitutional.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     5927 2023-07-21 14:55:24.000000 mordredcommunity-2.0.1rc1/mordred/DetourMatrix.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1273 2023-07-21 14:53:32.000000 mordredcommunity-2.0.1rc1/mordred/DistanceMatrix.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     3679 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/EState.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      957 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/EccentricConnectivityIndex.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)    20747 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/ExtendedTopochemicalAtom.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      978 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/FragmentComplexity.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1873 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Framework.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2504 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/GeometricalIndex.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1459 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/GravitationalIndex.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1041 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/HydrogenBond.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     7355 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/InformationContent.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2177 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/KappaShapeIndex.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1448 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Lipinski.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1540 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/LogS.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      667 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/McGowanVolume.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2224 2023-07-21 15:02:23.000000 mordredcommunity-2.0.1rc1/mordred/MoRSE.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2718 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/MoeType.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2728 2023-07-21 15:07:03.000000 mordredcommunity-2.0.1rc1/mordred/MolecularDistanceEdge.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     4271 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/MolecularId.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1655 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/MomentOfInertia.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      543 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/PBF.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     4030 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/PathCount.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1565 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Polarizability.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     4512 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/RingCount.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1368 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/RotatableBond.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      990 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/SLogP.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     3438 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/TopoPSA.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2607 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/TopologicalCharge.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2414 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/TopologicalIndex.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1602 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/VdwVolumeABC.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      943 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/VertexAdjacencyInformation.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2156 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/WalkCount.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1141 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Weight.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      995 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/WienerIndex.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2111 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/ZagrebIndex.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      268 2023-07-21 15:05:05.000000 mordredcommunity-2.0.1rc1/mordred/__init__.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     6462 2023-07-21 16:05:30.000000 mordredcommunity-2.0.1rc1/mordred/__main__.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     8724 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_atomic_property.py
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.187553 mordredcommunity-2.0.1rc1/mordred/_base/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2193 2023-07-21 15:06:36.000000 mordredcommunity-2.0.1rc1/mordred/_base/__init__.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)    12279 2023-07-21 16:05:54.000000 mordredcommunity-2.0.1rc1/mordred/_base/calculator.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2430 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_base/context.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     9681 2023-07-21 14:52:55.000000 mordredcommunity-2.0.1rc1/mordred/_base/descriptor.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      400 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_base/pandas_module.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2169 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_base/parallel.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     4323 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_base/result.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      435 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_base/util.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     3336 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_graph_matrix.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     6191 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_matrix_attributes.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2230 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_util.py
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.187553 mordredcommunity-2.0.1rc1/mordred/data/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1291 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/allred_rocow_electron_negativity.txt
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2220 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/ionization_potential.txt
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2553 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/mass.txt
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1602 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/mc_gowan_volume.txt
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1612 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/pauling_electron_negativity.txt
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2046 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/polarizalibity78.txt
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2510 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/polarizalibity94.txt
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1472 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/sanderson_electron_negativity.txt
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1569 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/van_der_waals_radii.txt
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.187553 mordredcommunity-2.0.1rc1/mordred/descriptors/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1044 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/descriptors/__init__.py
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.187553 mordredcommunity-2.0.1rc1/mordred/error/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2045 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/error/__init__.py
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.187553 mordredcommunity-2.0.1rc1/mordred/surface_area/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      519 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/surface_area/__init__.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1422 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/surface_area/__main__.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2392 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/surface_area/_mesh.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     3433 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/surface_area/_sasa.py
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.191553 mordredcommunity-2.0.1rc1/mordred/tests/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      633 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/Dummy.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)       28 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/__init__.py
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.199553 mordredcommunity-2.0.1rc1/mordred/tests/references/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      349 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Aromatic.yaml
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.199553 mordredcommunity-2.0.1rc1/mordred/tests/references/Atom/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      884 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Atom/AtomCount.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      948 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Atom/CarbonTypes.yaml
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.203553 mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     9836 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/AATS.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)    10241 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/AATSC.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     9554 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/ATS.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)    10102 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/ATSC.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     8768 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/GATS.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     9170 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/MATS.yaml
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.203553 mordredcommunity-2.0.1rc1/mordred/tests/references/Bond/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1062 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Bond/BondTypes.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      345 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Bond/HBond.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      577 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Bond/Rotatable.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1525 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/CPSA.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     8654 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Chi.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2049 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Constitutional.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1546 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/DistanceEdge.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      318 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/EState.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)    10580 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/ExtendedTopochemicalAtom.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      296 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/FragmentComplexity.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      310 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Framework.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1356 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/GeometricalIndex.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2177 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/GravitationalIndex.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2546 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Indices.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     4713 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/InformationContent.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      416 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Lipinski.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      861 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/LogS.yaml
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.203553 mordredcommunity-2.0.1rc1/mordred/tests/references/Matrix/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      544 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Matrix/BCUT.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1346 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Matrix/barysz.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1072 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Matrix/detour.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1725 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Matrix/distance.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      518 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/MoRSE.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      926 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/MolecularId.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1802 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/MomentOfInertia.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     3549 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/PathCount.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      532 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Polarizability.yaml
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.203553 mordredcommunity-2.0.1rc1/mordred/tests/references/Property/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      311 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Property/McGowanVolume.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      380 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Property/Vabc.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      556 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Property/Weight.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      508 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Ring.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      507 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Smarts.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      922 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/TopoPSA.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     3340 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/TopologicalCharge.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      601 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/VAdjMat.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     3663 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Walk.yaml
+-rw-r--r--   0 jackson   (1000) jackson   (1000)    64187 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/structures.sdf
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1262 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/structures.smi
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      605 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_ABCIndex.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     4227 2023-07-21 14:44:01.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_ETA.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1554 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_SASA.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      444 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_SLogP.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     4732 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_VEA.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     3171 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_atomic_property.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      811 2023-07-21 16:08:22.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_attributes.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2024 2023-07-21 15:24:13.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_by_references.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      615 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_compose_descriptor.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      587 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_exceptions.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      346 2023-07-21 15:07:33.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_import_all_descriptors.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      243 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_json.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     4905 2023-07-21 16:06:00.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_mordred_main.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      565 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_pandas.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      842 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_parallel.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1013 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_pickle.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     2326 2023-07-21 16:12:42.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_result_type.py
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.207553 mordredcommunity-2.0.1rc1/mordredcommunity.egg-info/
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)     5756 2023-07-27 21:07:14.000000 mordredcommunity-2.0.1rc1/mordredcommunity.egg-info/PKG-INFO
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)     4880 2023-07-27 21:07:14.000000 mordredcommunity-2.0.1rc1/mordredcommunity.egg-info/SOURCES.txt
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)        1 2023-07-27 21:07:14.000000 mordredcommunity-2.0.1rc1/mordredcommunity.egg-info/dependency_links.txt
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)       98 2023-07-27 21:07:14.000000 mordredcommunity-2.0.1rc1/mordredcommunity.egg-info/requires.txt
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)        8 2023-07-27 21:07:14.000000 mordredcommunity-2.0.1rc1/mordredcommunity.egg-info/top_level.txt
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1168 2023-07-27 21:06:38.000000 mordredcommunity-2.0.1rc1/pyproject.toml
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)       38 2023-07-27 21:07:14.207553 mordredcommunity-2.0.1rc1/setup.cfg
```

### Comparing `mordredcommunity-2.0.0/LICENSE` & `mordredcommunity-2.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/PKG-INFO` & `mordredcommunity-2.0.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mordredcommunity
-Version: 2.0.0
+Version: 2.0.1rc1
 Summary: Community-Maintained Version of mordred
 Author-email: Jackson Burns <jwburns@mit.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/JacksonBurns/mordred-community
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mordredcommunity-2.0.0/README.md` & `mordredcommunity-2.0.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/ABCIndex.py` & `mordredcommunity-2.0.1rc1/mordred/ABCIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/AcidBase.py` & `mordredcommunity-2.0.1rc1/mordred/AcidBase.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/AdjacencyMatrix.py` & `mordredcommunity-2.0.1rc1/mordred/AdjacencyMatrix.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/Aromatic.py` & `mordredcommunity-2.0.1rc1/mordred/Aromatic.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/AtomCount.py` & `mordredcommunity-2.0.1rc1/mordred/AtomCount.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/Autocorrelation.py` & `mordredcommunity-2.0.1rc1/mordred/Autocorrelation.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/BCUT.py` & `mordredcommunity-2.0.1rc1/mordred/BCUT.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/BalabanJ.py` & `mordredcommunity-2.0.1rc1/mordred/BalabanJ.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/BaryszMatrix.py` & `mordredcommunity-2.0.1rc1/mordred/BaryszMatrix.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/BertzCT.py` & `mordredcommunity-2.0.1rc1/mordred/BertzCT.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/BondCount.py` & `mordredcommunity-2.0.1rc1/mordred/BondCount.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/CPSA.py` & `mordredcommunity-2.0.1rc1/mordred/CPSA.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/CarbonTypes.py` & `mordredcommunity-2.0.1rc1/mordred/CarbonTypes.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/Chi.py` & `mordredcommunity-2.0.1rc1/mordred/Chi.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/Constitutional.py` & `mordredcommunity-2.0.1rc1/mordred/Constitutional.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/DetourMatrix.py` & `mordredcommunity-2.0.1rc1/mordred/DetourMatrix.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/DistanceMatrix.py` & `mordredcommunity-2.0.1rc1/mordred/DistanceMatrix.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/EState.py` & `mordredcommunity-2.0.1rc1/mordred/EState.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/EccentricConnectivityIndex.py` & `mordredcommunity-2.0.1rc1/mordred/EccentricConnectivityIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/ExtendedTopochemicalAtom.py` & `mordredcommunity-2.0.1rc1/mordred/ExtendedTopochemicalAtom.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/FragmentComplexity.py` & `mordredcommunity-2.0.1rc1/mordred/FragmentComplexity.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/Framework.py` & `mordredcommunity-2.0.1rc1/mordred/Framework.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/GeometricalIndex.py` & `mordredcommunity-2.0.1rc1/mordred/GeometricalIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/GravitationalIndex.py` & `mordredcommunity-2.0.1rc1/mordred/GravitationalIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/HydrogenBond.py` & `mordredcommunity-2.0.1rc1/mordred/HydrogenBond.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/InformationContent.py` & `mordredcommunity-2.0.1rc1/mordred/InformationContent.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/KappaShapeIndex.py` & `mordredcommunity-2.0.1rc1/mordred/KappaShapeIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/Lipinski.py` & `mordredcommunity-2.0.1rc1/mordred/Lipinski.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/LogS.py` & `mordredcommunity-2.0.1rc1/mordred/LogS.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/McGowanVolume.py` & `mordredcommunity-2.0.1rc1/mordred/McGowanVolume.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/MoRSE.py` & `mordredcommunity-2.0.1rc1/mordred/MoRSE.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/MoeType.py` & `mordredcommunity-2.0.1rc1/mordred/MoeType.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/MolecularDistanceEdge.py` & `mordredcommunity-2.0.1rc1/mordred/MolecularDistanceEdge.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/MolecularId.py` & `mordredcommunity-2.0.1rc1/mordred/MolecularId.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/MomentOfInertia.py` & `mordredcommunity-2.0.1rc1/mordred/MomentOfInertia.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/PBF.py` & `mordredcommunity-2.0.1rc1/mordred/PBF.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/PathCount.py` & `mordredcommunity-2.0.1rc1/mordred/PathCount.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/Polarizability.py` & `mordredcommunity-2.0.1rc1/mordred/Polarizability.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/RingCount.py` & `mordredcommunity-2.0.1rc1/mordred/RingCount.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/RotatableBond.py` & `mordredcommunity-2.0.1rc1/mordred/RotatableBond.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/SLogP.py` & `mordredcommunity-2.0.1rc1/mordred/SLogP.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/TopoPSA.py` & `mordredcommunity-2.0.1rc1/mordred/TopoPSA.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/TopologicalCharge.py` & `mordredcommunity-2.0.1rc1/mordred/TopologicalCharge.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/TopologicalIndex.py` & `mordredcommunity-2.0.1rc1/mordred/TopologicalIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/VdwVolumeABC.py` & `mordredcommunity-2.0.1rc1/mordred/VdwVolumeABC.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/VertexAdjacencyInformation.py` & `mordredcommunity-2.0.1rc1/mordred/VertexAdjacencyInformation.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/WalkCount.py` & `mordredcommunity-2.0.1rc1/mordred/WalkCount.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/Weight.py` & `mordredcommunity-2.0.1rc1/mordred/Weight.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/WienerIndex.py` & `mordredcommunity-2.0.1rc1/mordred/WienerIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/ZagrebIndex.py` & `mordredcommunity-2.0.1rc1/mordred/ZagrebIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/__main__.py` & `mordredcommunity-2.0.1rc1/mordred/__main__.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/_atomic_property.py` & `mordredcommunity-2.0.1rc1/mordred/_atomic_property.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/_base/__init__.py` & `mordredcommunity-2.0.1rc1/mordred/_base/__init__.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/_base/calculator.py` & `mordredcommunity-2.0.1rc1/mordred/_base/calculator.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/_base/context.py` & `mordredcommunity-2.0.1rc1/mordred/_base/context.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/_base/descriptor.py` & `mordredcommunity-2.0.1rc1/mordred/_base/descriptor.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/_base/parallel.py` & `mordredcommunity-2.0.1rc1/mordred/_base/parallel.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/_base/result.py` & `mordredcommunity-2.0.1rc1/mordred/_base/result.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/_graph_matrix.py` & `mordredcommunity-2.0.1rc1/mordred/_graph_matrix.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/_matrix_attributes.py` & `mordredcommunity-2.0.1rc1/mordred/_matrix_attributes.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/_util.py` & `mordredcommunity-2.0.1rc1/mordred/_util.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/descriptors/__init__.py` & `mordredcommunity-2.0.1rc1/mordred/descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/error/__init__.py` & `mordredcommunity-2.0.1rc1/mordred/error/__init__.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/surface_area/__init__.py` & `mordredcommunity-2.0.1rc1/mordred/surface_area/__init__.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/surface_area/__main__.py` & `mordredcommunity-2.0.1rc1/mordred/surface_area/__main__.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/surface_area/_mesh.py` & `mordredcommunity-2.0.1rc1/mordred/surface_area/_mesh.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/surface_area/_sasa.py` & `mordredcommunity-2.0.1rc1/mordred/surface_area/_sasa.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/tests/Dummy.py` & `mordredcommunity-2.0.1rc1/mordred/tests/Dummy.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/tests/test_ABCIndex.py` & `mordredcommunity-2.0.1rc1/mordred/tests/test_ABCIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/tests/test_ETA.py` & `mordredcommunity-2.0.1rc1/mordred/tests/test_ETA.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/tests/test_SASA.py` & `mordredcommunity-2.0.1rc1/mordred/tests/test_SASA.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/tests/test_VEA.py` & `mordredcommunity-2.0.1rc1/mordred/tests/test_VEA.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/tests/test_atomic_property.py` & `mordredcommunity-2.0.1rc1/mordred/tests/test_atomic_property.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/tests/test_attributes.py` & `mordredcommunity-2.0.1rc1/mordred/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/tests/test_by_references.py` & `mordredcommunity-2.0.1rc1/mordred/tests/test_by_references.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/tests/test_compose_descriptor.py` & `mordredcommunity-2.0.1rc1/mordred/tests/test_compose_descriptor.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/tests/test_exceptions.py` & `mordredcommunity-2.0.1rc1/mordred/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/tests/test_mordred_main.py` & `mordredcommunity-2.0.1rc1/mordred/tests/test_mordred_main.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/tests/test_pandas.py` & `mordredcommunity-2.0.1rc1/mordred/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/tests/test_parallel.py` & `mordredcommunity-2.0.1rc1/mordred/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/tests/test_pickle.py` & `mordredcommunity-2.0.1rc1/mordred/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordred/tests/test_result_type.py` & `mordredcommunity-2.0.1rc1/mordred/tests/test_result_type.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.0/mordredcommunity.egg-info/PKG-INFO` & `mordredcommunity-2.0.1rc1/mordredcommunity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mordredcommunity
-Version: 2.0.0
+Version: 2.0.1rc1
 Summary: Community-Maintained Version of mordred
 Author-email: Jackson Burns <jwburns@mit.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/JacksonBurns/mordred-community
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mordredcommunity-2.0.0/pyproject.toml` & `mordredcommunity-2.0.1rc1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mordredcommunity"
-version = "2.0.0"
+version = "2.0.1rc1"
 authors = [{ name = "Jackson Burns", email = "jwburns@mit.edu" }]
 license = { text = "BSD-3-Clause" }
 description = "Community-Maintained Version of mordred"
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -34,11 +34,14 @@
 
 [tool.isort]
 profile = "black"
 
 [tool.setuptools]
 include-package-data = true
 
+[tool.setuptools.package-data]
+mordred = ["data/*.txt", "tests/references/**"]
+
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["mordred*"]
 exclude = ["docs*", "examples*"]
```

