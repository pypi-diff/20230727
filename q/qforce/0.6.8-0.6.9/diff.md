# Comparing `tmp/qforce-0.6.8.tar.gz` & `tmp/qforce-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qforce-0.6.8.tar", last modified: Wed Nov 30 19:43:10 2022, max compression
+gzip compressed data, was "qforce-0.6.9.tar", last modified: Sun Dec 11 20:52:48 2022, max compression
```

## Comparing `qforce-0.6.8.tar` & `qforce-0.6.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 ssami      (501) staff       (20)        0 2022-11-30 19:43:10.137226 qforce-0.6.8/
--rw-r--r--   0 ssami      (501) staff       (20)    11528 2022-11-30 19:29:24.000000 qforce-0.6.8/LICENCE
--rw-r--r--   0 ssami      (501) staff       (20)     1606 2022-11-30 19:43:10.137311 qforce-0.6.8/PKG-INFO
--rw-r--r--   0 ssami      (501) staff       (20)      865 2022-11-30 19:29:24.000000 qforce-0.6.8/README.md
-drwxr-xr-x   0 ssami      (501) staff       (20)        0 2022-11-30 19:43:10.129675 qforce-0.6.8/qforce/
--rw-r--r--   0 ssami      (501) staff       (20)      125 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/__init__.py
--rw-r--r--   0 ssami      (501) staff       (20)     1039 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/calculator.py
-drwxr-xr-x   0 ssami      (501) staff       (20)        0 2022-11-30 19:43:10.132895 qforce-0.6.8/qforce/data/
--rw-r--r--   0 ssami      (501) staff       (20)  2679956 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/data/charmm36.itp
--rw-r--r--   0 ssami      (501) staff       (20)     1848 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/data/default.mdp
--rwxr-xr-x   0 ssami      (501) staff       (20)     6820 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/data/gaff.itp
--rw-r--r--   0 ssami      (501) staff       (20)     7738 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/data/gaff2.itp
--rw-r--r--   0 ssami      (501) staff       (20)   219093 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/data/gromos.itp
--rw-r--r--   0 ssami      (501) staff       (20)    62929 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/data/opls.itp
--rw-r--r--   0 ssami      (501) staff       (20)    20001 2022-11-30 19:37:45.000000 qforce-0.6.8/qforce/dihedral_scan.py
--rw-r--r--   0 ssami      (501) staff       (20)     3259 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/elements.py
--rw-r--r--   0 ssami      (501) staff       (20)    20848 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/forcefield.py
--rw-r--r--   0 ssami      (501) staff       (20)     8283 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/forces.py
--rw-r--r--   0 ssami      (501) staff       (20)    18194 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/fragment.py
--rw-r--r--   0 ssami      (501) staff       (20)     4352 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/frequencies.py
--rw-r--r--   0 ssami      (501) staff       (20)     3826 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/hessian.py
--rw-r--r--   0 ssami      (501) staff       (20)     5620 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/initialize.py
--rwxr-xr-x   0 ssami      (501) staff       (20)     2875 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/main.py
--rwxr-xr-x   0 ssami      (501) staff       (20)     1007 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/misc.py
-drwxr-xr-x   0 ssami      (501) staff       (20)        0 2022-11-30 19:43:10.134761 qforce-0.6.8/qforce/molecule/
--rw-r--r--   0 ssami      (501) staff       (20)      146 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/molecule/__init__.py
--rw-r--r--   0 ssami      (501) staff       (20)     4659 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/molecule/base.py
--rw-r--r--   0 ssami      (501) staff       (20)     2732 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/molecule/baseterms.py
--rw-r--r--   0 ssami      (501) staff       (20)    10184 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/molecule/dihedral_terms.py
--rw-r--r--   0 ssami      (501) staff       (20)      613 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/molecule/molecule.py
--rw-r--r--   0 ssami      (501) staff       (20)    27859 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/molecule/non_bonded.py
--rw-r--r--   0 ssami      (501) staff       (20)     1658 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/molecule/non_bonded_terms.py
--rw-r--r--   0 ssami      (501) staff       (20)     4231 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/molecule/non_dihedral_terms.py
--rw-r--r--   0 ssami      (501) staff       (20)     2900 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/molecule/storage.py
--rw-r--r--   0 ssami      (501) staff       (20)     5762 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/molecule/terms.py
--rw-r--r--   0 ssami      (501) staff       (20)     6246 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/molecule/topology.py
--rw-r--r--   0 ssami      (501) staff       (20)     4052 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/polarize.py
-drwxr-xr-x   0 ssami      (501) staff       (20)        0 2022-11-30 19:43:10.136004 qforce-0.6.8/qforce/qm/
--rw-r--r--   0 ssami      (501) staff       (20)        0 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/qm/__init__.py
--rwxr-xr-x   0 ssami      (501) staff       (20)     6731 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/qm/gaussian.py
--rw-r--r--   0 ssami      (501) staff       (20)    21062 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/qm/orca.py
--rwxr-xr-x   0 ssami      (501) staff       (20)     8704 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/qm/qchem.py
--rw-r--r--   0 ssami      (501) staff       (20)     8121 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/qm/qm.py
--rwxr-xr-x   0 ssami      (501) staff       (20)     8129 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/qm/qm_base.py
--rw-r--r--   0 ssami      (501) staff       (20)     3926 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/qm/torsiondrive_xtb.py
--rw-r--r--   0 ssami      (501) staff       (20)    13465 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/qm/xtb.py
-drwxr-xr-x   0 ssami      (501) staff       (20)        0 2022-11-30 19:43:10.137069 qforce-0.6.8/qforce/tests/
--rw-r--r--   0 ssami      (501) staff       (20)        0 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/tests/__init__.py
--rw-r--r--   0 ssami      (501) staff       (20)     1566 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/tests/test_fragments.py
--rw-r--r--   0 ssami      (501) staff       (20)     4496 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/tests/test_qm_gaussian.py
--rw-r--r--   0 ssami      (501) staff       (20)     4220 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/tests/test_qm_orca.py
--rw-r--r--   0 ssami      (501) staff       (20)     4431 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/tests/test_qm_xtb.py
--rw-r--r--   0 ssami      (501) staff       (20)     3986 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/tests/test_run_xtb.py
--rw-r--r--   0 ssami      (501) staff       (20)     1642 2022-11-30 19:29:24.000000 qforce-0.6.8/qforce/tests/test_torsiondrive_xtb.py
-drwxr-xr-x   0 ssami      (501) staff       (20)        0 2022-11-30 19:43:10.130361 qforce-0.6.8/qforce.egg-info/
--rw-r--r--   0 ssami      (501) staff       (20)     1606 2022-11-30 19:43:10.000000 qforce-0.6.8/qforce.egg-info/PKG-INFO
--rw-r--r--   0 ssami      (501) staff       (20)     1309 2022-11-30 19:43:10.000000 qforce-0.6.8/qforce.egg-info/SOURCES.txt
--rw-r--r--   0 ssami      (501) staff       (20)        1 2022-11-30 19:43:10.000000 qforce-0.6.8/qforce.egg-info/dependency_links.txt
--rw-r--r--   0 ssami      (501) staff       (20)       44 2022-11-30 19:43:10.000000 qforce-0.6.8/qforce.egg-info/entry_points.txt
--rw-r--r--   0 ssami      (501) staff       (20)       79 2022-11-30 19:43:10.000000 qforce-0.6.8/qforce.egg-info/requires.txt
--rw-r--r--   0 ssami      (501) staff       (20)        7 2022-11-30 19:43:10.000000 qforce-0.6.8/qforce.egg-info/top_level.txt
--rw-r--r--   0 ssami      (501) staff       (20)      851 2022-11-30 19:43:10.137599 qforce-0.6.8/setup.cfg
--rw-r--r--   0 ssami      (501) staff       (20)      223 2022-11-30 19:29:24.000000 qforce-0.6.8/setup.py
+drwxr-xr-x   0 ssami      (501) staff       (20)        0 2022-12-11 20:52:48.840050 qforce-0.6.9/
+-rw-r--r--   0 ssami      (501) staff       (20)    11528 2022-11-30 19:29:24.000000 qforce-0.6.9/LICENCE
+-rw-r--r--   0 ssami      (501) staff       (20)     1606 2022-12-11 20:52:48.840118 qforce-0.6.9/PKG-INFO
+-rw-r--r--   0 ssami      (501) staff       (20)      865 2022-11-30 19:29:24.000000 qforce-0.6.9/README.md
+drwxr-xr-x   0 ssami      (501) staff       (20)        0 2022-12-11 20:52:48.829797 qforce-0.6.9/qforce/
+-rw-r--r--   0 ssami      (501) staff       (20)      125 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/__init__.py
+-rw-r--r--   0 ssami      (501) staff       (20)     1039 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/calculator.py
+drwxr-xr-x   0 ssami      (501) staff       (20)        0 2022-12-11 20:52:48.835943 qforce-0.6.9/qforce/data/
+-rw-r--r--   0 ssami      (501) staff       (20)  2679956 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/data/charmm36.itp
+-rw-r--r--   0 ssami      (501) staff       (20)     1848 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/data/default.mdp
+-rwxr-xr-x   0 ssami      (501) staff       (20)     6820 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/data/gaff.itp
+-rw-r--r--   0 ssami      (501) staff       (20)     7738 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/data/gaff2.itp
+-rw-r--r--   0 ssami      (501) staff       (20)   219093 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/data/gromos.itp
+-rw-r--r--   0 ssami      (501) staff       (20)    62929 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/data/opls.itp
+-rw-r--r--   0 ssami      (501) staff       (20)    20001 2022-11-30 19:37:45.000000 qforce-0.6.9/qforce/dihedral_scan.py
+-rw-r--r--   0 ssami      (501) staff       (20)     3259 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/elements.py
+-rw-r--r--   0 ssami      (501) staff       (20)    20848 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/forcefield.py
+-rw-r--r--   0 ssami      (501) staff       (20)     8283 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/forces.py
+-rw-r--r--   0 ssami      (501) staff       (20)    18194 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/fragment.py
+-rw-r--r--   0 ssami      (501) staff       (20)     4352 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/frequencies.py
+-rw-r--r--   0 ssami      (501) staff       (20)     3826 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/hessian.py
+-rw-r--r--   0 ssami      (501) staff       (20)     5620 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/initialize.py
+-rwxr-xr-x   0 ssami      (501) staff       (20)     2875 2022-12-11 20:47:54.000000 qforce-0.6.9/qforce/main.py
+-rwxr-xr-x   0 ssami      (501) staff       (20)     1007 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/misc.py
+drwxr-xr-x   0 ssami      (501) staff       (20)        0 2022-12-11 20:52:48.837650 qforce-0.6.9/qforce/molecule/
+-rw-r--r--   0 ssami      (501) staff       (20)      146 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/molecule/__init__.py
+-rw-r--r--   0 ssami      (501) staff       (20)     4659 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/molecule/base.py
+-rw-r--r--   0 ssami      (501) staff       (20)     2732 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/molecule/baseterms.py
+-rw-r--r--   0 ssami      (501) staff       (20)    10184 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/molecule/dihedral_terms.py
+-rw-r--r--   0 ssami      (501) staff       (20)      613 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/molecule/molecule.py
+-rw-r--r--   0 ssami      (501) staff       (20)    27859 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/molecule/non_bonded.py
+-rw-r--r--   0 ssami      (501) staff       (20)     1658 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/molecule/non_bonded_terms.py
+-rw-r--r--   0 ssami      (501) staff       (20)     4231 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/molecule/non_dihedral_terms.py
+-rw-r--r--   0 ssami      (501) staff       (20)     2900 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/molecule/storage.py
+-rw-r--r--   0 ssami      (501) staff       (20)     5762 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/molecule/terms.py
+-rw-r--r--   0 ssami      (501) staff       (20)     6246 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/molecule/topology.py
+-rw-r--r--   0 ssami      (501) staff       (20)     4052 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/polarize.py
+drwxr-xr-x   0 ssami      (501) staff       (20)        0 2022-12-11 20:52:48.838990 qforce-0.6.9/qforce/qm/
+-rw-r--r--   0 ssami      (501) staff       (20)        0 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/qm/__init__.py
+-rwxr-xr-x   0 ssami      (501) staff       (20)     6731 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/qm/gaussian.py
+-rw-r--r--   0 ssami      (501) staff       (20)    21133 2022-12-11 20:51:25.000000 qforce-0.6.9/qforce/qm/orca.py
+-rwxr-xr-x   0 ssami      (501) staff       (20)     8704 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/qm/qchem.py
+-rw-r--r--   0 ssami      (501) staff       (20)     8121 2022-12-11 20:47:51.000000 qforce-0.6.9/qforce/qm/qm.py
+-rwxr-xr-x   0 ssami      (501) staff       (20)     8129 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/qm/qm_base.py
+-rw-r--r--   0 ssami      (501) staff       (20)     3926 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/qm/torsiondrive_xtb.py
+-rw-r--r--   0 ssami      (501) staff       (20)    13465 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/qm/xtb.py
+drwxr-xr-x   0 ssami      (501) staff       (20)        0 2022-12-11 20:52:48.839910 qforce-0.6.9/qforce/tests/
+-rw-r--r--   0 ssami      (501) staff       (20)        0 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/tests/__init__.py
+-rw-r--r--   0 ssami      (501) staff       (20)     1566 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/tests/test_fragments.py
+-rw-r--r--   0 ssami      (501) staff       (20)     4496 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/tests/test_qm_gaussian.py
+-rw-r--r--   0 ssami      (501) staff       (20)     4220 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/tests/test_qm_orca.py
+-rw-r--r--   0 ssami      (501) staff       (20)     4431 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/tests/test_qm_xtb.py
+-rw-r--r--   0 ssami      (501) staff       (20)     3986 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/tests/test_run_xtb.py
+-rw-r--r--   0 ssami      (501) staff       (20)     1642 2022-11-30 19:29:24.000000 qforce-0.6.9/qforce/tests/test_torsiondrive_xtb.py
+drwxr-xr-x   0 ssami      (501) staff       (20)        0 2022-12-11 20:52:48.830502 qforce-0.6.9/qforce.egg-info/
+-rw-r--r--   0 ssami      (501) staff       (20)     1606 2022-12-11 20:52:48.000000 qforce-0.6.9/qforce.egg-info/PKG-INFO
+-rw-r--r--   0 ssami      (501) staff       (20)     1309 2022-12-11 20:52:48.000000 qforce-0.6.9/qforce.egg-info/SOURCES.txt
+-rw-r--r--   0 ssami      (501) staff       (20)        1 2022-12-11 20:52:48.000000 qforce-0.6.9/qforce.egg-info/dependency_links.txt
+-rw-r--r--   0 ssami      (501) staff       (20)       44 2022-12-11 20:52:48.000000 qforce-0.6.9/qforce.egg-info/entry_points.txt
+-rw-r--r--   0 ssami      (501) staff       (20)       79 2022-12-11 20:52:48.000000 qforce-0.6.9/qforce.egg-info/requires.txt
+-rw-r--r--   0 ssami      (501) staff       (20)        7 2022-12-11 20:52:48.000000 qforce-0.6.9/qforce.egg-info/top_level.txt
+-rw-r--r--   0 ssami      (501) staff       (20)      851 2022-12-11 20:52:48.840391 qforce-0.6.9/setup.cfg
+-rw-r--r--   0 ssami      (501) staff       (20)      223 2022-11-30 19:29:24.000000 qforce-0.6.9/setup.py
```

### Comparing `qforce-0.6.8/LICENCE` & `qforce-0.6.9/LICENCE`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/PKG-INFO` & `qforce-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qforce
-Version: 0.6.8
+Version: 0.6.9
 Summary: Q-Force: Quantum mechanically augmented molecular force fields
 Home-page: https://github.com/selimsami/qforce
 Author: Selim Sami
 Author-email: s.sami@rug.nl
 License: UNKNOWN
 Keywords: qm forcefield md
 Platform: UNKNOWN
```

### Comparing `qforce-0.6.8/README.md` & `qforce-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/calculator.py` & `qforce-0.6.9/qforce/calculator.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/data/charmm36.itp` & `qforce-0.6.9/qforce/data/charmm36.itp`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/data/default.mdp` & `qforce-0.6.9/qforce/data/default.mdp`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/data/gaff.itp` & `qforce-0.6.9/qforce/data/gaff.itp`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/data/gaff2.itp` & `qforce-0.6.9/qforce/data/gaff2.itp`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/data/gromos.itp` & `qforce-0.6.9/qforce/data/gromos.itp`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/data/opls.itp` & `qforce-0.6.9/qforce/data/opls.itp`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/dihedral_scan.py` & `qforce-0.6.9/qforce/dihedral_scan.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/elements.py` & `qforce-0.6.9/qforce/elements.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/forcefield.py` & `qforce-0.6.9/qforce/forcefield.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/forces.py` & `qforce-0.6.9/qforce/forces.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/fragment.py` & `qforce-0.6.9/qforce/fragment.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/frequencies.py` & `qforce-0.6.9/qforce/frequencies.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/hessian.py` & `qforce-0.6.9/qforce/hessian.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/initialize.py` & `qforce-0.6.9/qforce/initialize.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/main.py` & `qforce-0.6.9/qforce/main.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/misc.py` & `qforce-0.6.9/qforce/misc.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/molecule/base.py` & `qforce-0.6.9/qforce/molecule/base.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/molecule/baseterms.py` & `qforce-0.6.9/qforce/molecule/baseterms.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/molecule/dihedral_terms.py` & `qforce-0.6.9/qforce/molecule/dihedral_terms.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/molecule/molecule.py` & `qforce-0.6.9/qforce/molecule/molecule.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/molecule/non_bonded.py` & `qforce-0.6.9/qforce/molecule/non_bonded.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/molecule/non_bonded_terms.py` & `qforce-0.6.9/qforce/molecule/non_bonded_terms.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/molecule/non_dihedral_terms.py` & `qforce-0.6.9/qforce/molecule/non_dihedral_terms.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/molecule/storage.py` & `qforce-0.6.9/qforce/molecule/storage.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/molecule/terms.py` & `qforce-0.6.9/qforce/molecule/terms.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/molecule/topology.py` & `qforce-0.6.9/qforce/molecule/topology.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/polarize.py` & `qforce-0.6.9/qforce/polarize.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/qm/gaussian.py` & `qforce-0.6.9/qforce/qm/gaussian.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/qm/orca.py` & `qforce-0.6.9/qforce/qm/orca.py`

 * *Files 1% similar despite different names*

```diff
@@ -589,11 +589,12 @@
             point_charges["cm5"] = charges
         if config.charge_method == "esp":
             n_atoms, charges = self._read_orca_esp(
                 '{}_charge.pc_chelpg'.format(base))
             point_charges["esp"] = charges
         n_atoms, elements, coords = self._read_orca_allxyz(
             '{}_scan.allxyz'.format(base))
-        angles, _ = self._read_orca_dat('{}_scan.relaxscanact.dat'.format(base))
-        _, energies = self._read_orca_dat('{}_sp.xyzact.dat'.format(base))
+        angles, energies = self._read_orca_dat('{}_scan.relaxscanact.dat'.format(base))
+        if os.path.isfile('{}_sp.xyzact.dat'.format(base)):
+            _, energies = self._read_orca_dat('{}_sp.xyzact.dat'.format(base))
         energies = np.array(energies) * Hartree * mol / kJ
         return n_atoms, coords, angles, energies, point_charges
```

### Comparing `qforce-0.6.8/qforce/qm/qchem.py` & `qforce-0.6.9/qforce/qm/qchem.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/qm/qm.py` & `qforce-0.6.9/qforce/qm/qm.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/qm/qm_base.py` & `qforce-0.6.9/qforce/qm/qm_base.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/qm/torsiondrive_xtb.py` & `qforce-0.6.9/qforce/qm/torsiondrive_xtb.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/qm/xtb.py` & `qforce-0.6.9/qforce/qm/xtb.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/tests/test_fragments.py` & `qforce-0.6.9/qforce/tests/test_fragments.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/tests/test_qm_gaussian.py` & `qforce-0.6.9/qforce/tests/test_qm_gaussian.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/tests/test_qm_orca.py` & `qforce-0.6.9/qforce/tests/test_qm_orca.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/tests/test_qm_xtb.py` & `qforce-0.6.9/qforce/tests/test_qm_xtb.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/tests/test_run_xtb.py` & `qforce-0.6.9/qforce/tests/test_run_xtb.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce/tests/test_torsiondrive_xtb.py` & `qforce-0.6.9/qforce/tests/test_torsiondrive_xtb.py`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/qforce.egg-info/PKG-INFO` & `qforce-0.6.9/qforce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qforce
-Version: 0.6.8
+Version: 0.6.9
 Summary: Q-Force: Quantum mechanically augmented molecular force fields
 Home-page: https://github.com/selimsami/qforce
 Author: Selim Sami
 Author-email: s.sami@rug.nl
 License: UNKNOWN
 Keywords: qm forcefield md
 Platform: UNKNOWN
```

### Comparing `qforce-0.6.8/qforce.egg-info/SOURCES.txt` & `qforce-0.6.9/qforce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qforce-0.6.8/setup.cfg` & `qforce-0.6.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qforce
-version = 0.6.8
+version = 0.6.9
 description = Q-Force: Quantum mechanically augmented molecular force fields
 long_description = file: README.md
 long_description_content_type = text/markdown
 licence = Apache 2.0
 author = Selim Sami
 author_email = s.sami@rug.nl
 url = https://github.com/selimsami/qforce
```

