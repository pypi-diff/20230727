# Comparing `tmp/biobb_flexserv-4.0.2.tar.gz` & `tmp/biobb_flexserv-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_flexserv-4.0.2.tar", last modified: Wed May 31 10:41:43 2023, max compression
+gzip compressed data, was "dist/biobb_flexserv-4.0.3.tar", last modified: Thu Jul 27 11:29:17 2023, max compression
```

## Comparing `biobb_flexserv-4.0.2.tar` & `biobb_flexserv-4.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.2/LICENSE
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1082 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5896 2023-05-31 10:41:05.000000 biobb_flexserv-4.0.2/README.md
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       81 2023-05-31 10:40:45.000000 biobb_flexserv-4.0.2/biobb_flexserv/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv/flexserv/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       61 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.2/biobb_flexserv/flexserv/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7209 2023-04-13 07:06:13.000000 biobb_flexserv-4.0.2/biobb_flexserv/flexserv/bd_run.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7677 2023-04-13 07:06:13.000000 biobb_flexserv-4.0.2/biobb_flexserv/flexserv/dmd_run.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7628 2023-05-31 10:38:32.000000 biobb_flexserv-4.0.2/biobb_flexserv/flexserv/nma_run.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      194 2023-04-13 07:06:13.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7497 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_animate.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9623 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_bfactor.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8126 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_collectivity.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8444 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_evecs.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12583 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_hinges.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9331 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_info.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8036 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_lindemann.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    18293 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_similarity.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8807 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_stiffness.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7450 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_unzip.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8897 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_zip.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv.egg-info/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1082 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      888 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      762 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       15 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2429 2023-05-31 10:40:40.000000 biobb_flexserv-4.0.2/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-07-27 11:29:17.000000 biobb_flexserv-4.0.3/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573    11357 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.3/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1082 2023-07-27 11:29:17.000000 biobb_flexserv-4.0.3/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     5896 2023-07-27 11:27:44.000000 biobb_flexserv-4.0.3/README.md
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-07-27 11:29:17.000000 biobb_flexserv-4.0.3/biobb_flexserv/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       81 2023-07-27 11:27:29.000000 biobb_flexserv-4.0.3/biobb_flexserv/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-07-27 11:29:17.000000 biobb_flexserv-4.0.3/biobb_flexserv/flexserv/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       61 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.3/biobb_flexserv/flexserv/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7209 2023-04-13 07:06:13.000000 biobb_flexserv-4.0.3/biobb_flexserv/flexserv/bd_run.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7677 2023-04-13 07:06:13.000000 biobb_flexserv-4.0.3/biobb_flexserv/flexserv/dmd_run.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7628 2023-05-31 10:38:32.000000 biobb_flexserv-4.0.3/biobb_flexserv/flexserv/nma_run.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-07-27 11:29:17.000000 biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      194 2023-04-13 07:06:13.000000 biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7497 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_animate.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9623 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_bfactor.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8126 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_collectivity.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8444 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_evecs.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12583 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_hinges.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9331 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_info.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8036 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_lindemann.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    23047 2023-07-27 11:20:19.000000 biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_similarity.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8807 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_stiffness.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7450 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_unzip.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8897 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_zip.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-07-27 11:29:17.000000 biobb_flexserv-4.0.3/biobb_flexserv.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1082 2023-07-27 11:29:17.000000 biobb_flexserv-4.0.3/biobb_flexserv.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      888 2023-07-27 11:29:17.000000 biobb_flexserv-4.0.3/biobb_flexserv.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2023-07-27 11:29:17.000000 biobb_flexserv-4.0.3/biobb_flexserv.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      762 2023-07-27 11:29:17.000000 biobb_flexserv-4.0.3/biobb_flexserv.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2023-07-27 11:29:17.000000 biobb_flexserv-4.0.3/biobb_flexserv.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       15 2023-07-27 11:29:17.000000 biobb_flexserv-4.0.3/biobb_flexserv.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2023-07-27 11:29:17.000000 biobb_flexserv-4.0.3/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2429 2023-07-27 11:27:19.000000 biobb_flexserv-4.0.3/setup.py
```

### Comparing `biobb_flexserv-4.0.2/LICENSE` & `biobb_flexserv-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/PKG-INFO` & `biobb_flexserv-4.0.3/biobb_flexserv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: biobb_flexserv
-Version: 4.0.2
+Name: biobb-flexserv
+Version: 4.0.3
 Summary: biobb_flexserv is a BioBB category for biomolecular flexibility studies on protein 3D structures.
 Home-page: https://github.com/bioexcel/biobb_flexserv
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_flexserv.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
```

### Comparing `biobb_flexserv-4.0.2/README.md` & `biobb_flexserv-4.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_flexserv?label=Version)](https://GitHub.com/bioexcel/biobb_flexserv/tags/)
 [![](https://img.shields.io/pypi/v/biobb-flexserv.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-flexserv/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_flexserv?label=Conda)](https://anaconda.org/bioconda/biobb_flexserv)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_flexserv?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_flexserv)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_flexserv?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_flexserv:4.0.2--pypl5321hdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_flexserv:4.0.3--pypl5321hdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_flexserv)
 [![](https://img.shields.io/pypi/pyversions/biobb-flexserv.svg?label=Python%20Versions)](https://pypi.org/project/biobb-flexserv/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_flexserv)
 
 [![](https://readthedocs.org/projects/biobb-flexserv/badge/?version=latest&label=Docs)](https://biobb-flexserv.readthedocs.io/en/latest/?badge=latest)
@@ -31,60 +31,60 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_flexserv.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.2 2023.1
+v4.0.3 2023.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_flexserv>=4.0.2"
+        pip install "biobb_flexserv>=4.0.3"
 
 
 * Usage: [Python API documentation](https://biobb-flexserv.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_flexserv>=4.0.2"
+        conda install -c bioconda "biobb_flexserv>=4.0.3"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-flexserv.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-flexserv.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_flexserv:4.0.2--pypl5321hdfd78af_0
+        docker pull quay.io/biocontainers/biobb_flexserv:4.0.3--pypl5321hdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_flexserv:4.0.2--pypl5321hdfd78af_0
+        docker run quay.io/biocontainers/biobb_flexserv:4.0.3--pypl5321hdfd78af_0
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_flexserv.sif https://depot.galaxyproject.org/singularity/biobb_flexserv:4.0.2--pypl5321hdfd78af_0
+        singularity pull --name biobb_flexserv.sif https://depot.galaxyproject.org/singularity/biobb_flexserv:4.0.3--pypl5321hdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_flexserv.sif <command>
```

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv/flexserv/bd_run.py` & `biobb_flexserv-4.0.3/biobb_flexserv/flexserv/bd_run.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv/flexserv/dmd_run.py` & `biobb_flexserv-4.0.3/biobb_flexserv/flexserv/dmd_run.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv/flexserv/nma_run.py` & `biobb_flexserv-4.0.3/biobb_flexserv/flexserv/nma_run.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_animate.py` & `biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_animate.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_bfactor.py` & `biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_bfactor.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_collectivity.py` & `biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_collectivity.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_evecs.py` & `biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_evecs.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_hinges.py` & `biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_hinges.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_info.py` & `biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_info.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_lindemann.py` & `biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_lindemann.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_similarity.py` & `biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_similarity.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     | Wrapper of the pczdump tool from the PCAsuite FlexServ module.
 
     Args:
         input_pcz_path1 (str): Input compressed trajectory file 1. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/data/pcasuite/pcazip.pcz>`_. Accepted formats: pcz (edam:format_3874).
         input_pcz_path2 (str): Input compressed trajectory file 2. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/data/pcasuite/pcazip.pcz>`_. Accepted formats: pcz (edam:format_3874).
         output_json_path (str): Output json file with PCA Similarity results. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/pcasuite/pcz_similarity.json>`_. Accepted formats: json (edam:format_3464).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
+            * **amplifying_factor** (*float*) - ("0.0") common displacement (dx) along the different eigenvectors. If 0, the result is the absolute similarity index (dot product).
             * **binary_path** (*str*) - ("pczdump") pczdump binary path to be used.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
@@ -62,14 +63,15 @@
             'in': {'input_pcz_path1': input_pcz_path1,
                    'input_pcz_path2': input_pcz_path2},
             'out': {'output_json_path': output_json_path}
         }
 
         # Properties specific for BB
         self.properties = properties
+        self.amplifying_factor = properties.get('amplifying_factor')
         self.binary_path = properties.get('binary_path', 'pczdump')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     # Check two eigenvectors to be compatible for dot product
@@ -80,23 +82,24 @@
             print('WARNING: Number of eigenvectors does not match')
             return False
         if len(eigenvectors_1[0]) != len(eigenvectors_2[0]):
             print('WARNING: Number of values in eigenvectors does not match')
             return False
         return True
 
+    # Weighted Cross Product (WCP).
     # Get the weighted cross product between eigenvectors
     # This is meant to compare PCA results for molecular dynamics structural conformations
     # The number of eigenvectors to be compared may be specified. All (0) by default
     # DISCLAIMER: This code has been translated from a perl script signed by Alberto Perez (13/09/04)
+    # Exploring the Essential Dynamics of B-DNA; Alberto Perez, Jose Ramon Blas, Manuel Rueda,
+    # Jose Maria Lopez-Bes, Xavier de la Cruz and Modesto Orozco. J. Chem. Theory Comput.2005,1.
     def get_similarity_index(self,
                              eigenvalues_1, eigenvectors_1,
-                             eigenvalues_2, eigenvectors_2):
-
-        amplifying_factor = 0
+                             eigenvalues_2, eigenvectors_2, dx=None):
 
         # Check the number of eigenvectors and the number of values in both eigenvectors to match
         if not self.are_compatible(eigenvectors_1, eigenvectors_2):
             raise SystemExit('Eigenvectors are not compatible')
 
         # Find out the total number of eigenvectors
         # Set the number of eigenvectors to be analyzed in case it is not set or it exceeds the total
@@ -104,15 +107,29 @@
 
         # Find out the number of atoms in the structure
         # Eigenvectors are atom coordinates and each atom has 3 coordinates (x, y, z)
         if len(eigenvectors_1[0]) % 3 != 0:
             raise SystemExit('Something is wrong with eigenvectors since number of values is not divisor of 3')
         atom_number = int(len(eigenvectors_1[0]) / 3)
 
+        # Amplifying factor: if it is 0 the algorithm is the same as a simple dot product.
+        # The value of the ~10th eigenvalue is usually taken.
+        if dx is not None:
+            amplifying_factor = dx
+        else:
+            amplifying_factor = eigenvalues_1[eigenvectors_number-1]
+
         # Get the denominator
+        # Find new denominator
+        # for ($i=0;$i<$nvec;$i++){
+        #     $cte1+=exp(-1/$val_1[$i]*$ampf);
+        #     $cte2+=exp(-1/$val_2[$i]*$ampf);
+        #     $part1+=exp(-2/$val_1[$i]*$ampf)*exp(-2/$val_1[$i]*$ampf);
+        #     $part2+=exp(-2/$val_2[$i]*$ampf)*exp(-2/$val_2[$i]*$ampf);
+        # }
         cte1 = part1 = cte2 = part2 = 0
         for eigenvalue in eigenvalues_1:
             cte1 += exp(-1 / eigenvalue * amplifying_factor)
             part1 += exp(-2 / eigenvalue * amplifying_factor) ** 2
         for eigenvalue in eigenvalues_2:
             cte2 += exp(-1 / eigenvalue * amplifying_factor)
             part2 += exp(-2 / eigenvalue * amplifying_factor) ** 2
@@ -143,49 +160,135 @@
                 add = add * exp(-1 / eigenvalues_1[i] * amplifying_factor - 1 / eigenvalues_2[j] * amplifying_factor)
                 add2 = add ** 2
                 total_summatory += add2
 
         similarity_index = total_summatory * 2 / denominator
         return similarity_index
 
+    # Weighted Cross Product (WCP).
+    # DF implementation of Alberto's formula
+    # Exploring the Essential Dynamics of B-DNA; Alberto Perez, Jose Ramon Blas, Manuel Rueda,
+    # Jose Maria Lopez-Bes, Xavier de la Cruz and Modesto Orozco. J. Chem. Theory Comput.2005,1.
+    def eigenmsip(self, eigenvalues_1, eigenvectors_1,
+                  eigenvalues_2, eigenvectors_2,
+                  dx=None):
+
+        evals1 = np.array(eigenvalues_1)
+        evals2 = np.array(eigenvalues_2)
+
+        evecs1 = np.array(eigenvectors_1)
+        evecs2 = np.array(eigenvectors_2)
+
+        n_components = len(eigenvectors_1)
+
+        # Amplifying factor: if it is 0 the algorithm is the same as a simple dot product.
+        # The value of the ~10th eigenvalue is usually taken.
+        if dx is not None:
+            amplifying_factor = dx
+        else:
+            amplifying_factor = evals1[n_components-1]
+
+        e1 = np.exp(-(amplifying_factor)**2/evals1)
+        e2 = np.exp(-(amplifying_factor)**2/evals2)
+
+        e1_2 = np.exp(-2*(amplifying_factor)**2/evals1)
+        e2_2 = np.exp(-2*(amplifying_factor)**2/evals2)
+        sume1 = np.sum(e1)
+        sume2 = np.sum(e2)
+
+        denominator = np.sum((e1_2/sume1**2)**2)+np.sum((e2_2/sume2**2)**2)
+
+        # numerator_df = np.square(np.dot(evecs1, evecs2)*np.outer(e1, e2)/(sume1*sume2))
+        # numerator_df = 2 * np.sum(numerator_df)
+
+        val_tmp = 0
+        accum_a = 0
+        c = sume1*sume2
+        for pc in range(0, n_components):
+            for pc2 in range(0, n_components):
+                eve1 = evecs1[pc]
+                eve2 = evecs2[pc2]
+                eva1 = evals1[pc]
+                eva2 = evals2[pc2]
+                a = np.dot(eve1, eve2)
+                b = np.exp(-(amplifying_factor)**2/eva1 - (amplifying_factor)**2/eva2)
+                val_tmp = val_tmp + ((a * b)/c)**2
+                accum_a = accum_a + a
+
+        numerator = 2 * val_tmp
+
+        return numerator/(denominator)
+
     # Get the dot product matrix of two eigenvectors
     def dot_product(self, eigenvectors_1, eigenvectors_2):
         # Check the number of eigenvectors and the number of values in both eigenvectors to match
         if not self.are_compatible(eigenvectors_1, eigenvectors_2):
             raise SystemExit('Eigenvectors are not compatible')
         # Get the dot product
         dpm = np.dot(eigenvectors_1, np.transpose(eigenvectors_2))
         return dpm
 
+    # Get the dot product matrix of two eigenvectors (squared and normalized).
+    # Absolute Similarity Index (Hess 2000, 2002)
+    def dot_product_accum(self, eigenvectors_1, eigenvectors_2):
+        n_components = len(eigenvectors_1)
+        # Get the dot product
+        dpm = self.dot_product(eigenvectors_1, eigenvectors_2)
+
+        sso = (dpm * dpm).sum() / n_components
+        # sso = (dpm * dpm).sum() / n_components
+        return sso
+
     # Get the subspace overlap
-    # DANI: Es como el similarity index pero sin utilizar los eigenvalues y sin toda la parte de los weights, creo
+    # Same as before, but with a square root
     def get_subspace_overlap(self, eigenvectors_1, eigenvectors_2):
         # Get the number of eigenvectors
         n_components = len(eigenvectors_1)
         # Get the dot product
         dpm = self.dot_product(eigenvectors_1, eigenvectors_2)
-        print(dpm)
+
         sso = np.sqrt((dpm * dpm).sum() / n_components)
         # sso = (dpm * dpm).sum() / n_components
         return sso
 
+    # Classic RMSip (Root Mean Square Inner Product), gives the same results as the previous function get_subspace_overlap
+    def get_rmsip(self, eigenvectors_1, eigenvectors_2):
+
+        # Get the number of eigenvectors
+        n_components = len(eigenvectors_1)
+
+        accum = 0
+        for pc in range(0, n_components):
+            for pc2 in range(0, n_components):
+                dpm = np.dot(eigenvectors_1[pc], eigenvectors_2[pc2])
+                val = dpm * dpm
+                accum = accum + val
+
+        sso = np.sqrt(accum / n_components)
+        # sso = (dpm * dpm).sum() / n_components
+        return sso
+
+    # RWSIP, Root Weighted Square Inner Product. Same as before, but weighted using the eigen values.
+    # See Edvin Fuglebakk and others, Measuring and comparing structural fluctuation patterns in large protein datasets,
+    # Bioinformatics, Volume 28, Issue 19, October 2012, Pages 2431–2440, https://doi.org/10.1093/bioinformatics/bts445
     def get_rwsip(self,
                   eigenvalues_1, eigenvectors_1,
                   eigenvalues_2, eigenvectors_2):
 
         # Get the number of eigenvectors
         n_components = len(eigenvectors_1)
 
         accum = 0
         norm = 0
         for pc in range(0, n_components):
-            dpm = np.dot(eigenvectors_1[pc], np.transpose(eigenvectors_2[pc]))
-            val = dpm * dpm * eigenvalues_1[pc] * eigenvalues_2[pc]
+            for pc2 in range(0, n_components):
+                dpm = np.dot(eigenvectors_1[pc], eigenvectors_2[pc2])
+                val = dpm * dpm * eigenvalues_1[pc] * eigenvalues_2[pc2]
+                accum = accum + val
             norm = norm + eigenvalues_1[pc] * eigenvalues_2[pc]
-            accum = accum + val
 
         sso = np.sqrt(accum / norm)
         # sso = (dpm * dpm).sum() / n_components
         return sso
 
     @launchlogger
     def launch(self):
@@ -330,34 +433,35 @@
                     info = line.strip().split(' ')
                     for nums in info:
                         if nums:
                             list_evecs.append(float(nums))
                 info_dict['evecs_2'][pc_id] = list_evecs
                 eigenvectors_2.append(list_evecs)
 
-        simIndex = self.get_similarity_index(info_dict['evals_1'], eigenvectors_1, info_dict['evals_2'], eigenvectors_2)
-        info_dict['similarityIndex'] = float("{:.3f}".format(simIndex))
-        dotProduct = self.get_subspace_overlap(eigenvectors_1, eigenvectors_2)
-        # info_dict['similarityIndex_dotProduct'] = float("{:.3f}".format(dotProduct))
-        info_dict['similarityIndex_rmsip'] = float("{:.3f}".format(dotProduct))
+        # simIndex = self.get_similarity_index(info_dict['evals_1'], eigenvectors_1, info_dict['evals_2'], eigenvectors_2, self.amplifying_factor)
+        # info_dict['similarityIndex_WCP2'] = float("{:.3f}".format(simIndex))
+        # dotProduct = self.get_subspace_overlap(eigenvectors_1, eigenvectors_2)
+        # info_dict['similarityIndex_rmsip2'] = float("{:.3f}".format(dotProduct))
+        eigenmsip = self.eigenmsip(info_dict['evals_1'], eigenvectors_1, info_dict['evals_2'], eigenvectors_2, self.amplifying_factor)
+        info_dict['similarityIndex_WCP'] = float("{:.3f}".format(eigenmsip))
+        rmsip = self.get_rmsip(eigenvectors_1, eigenvectors_2)
+        info_dict['similarityIndex_rmsip'] = float("{:.3f}".format(rmsip))
         rwsip = self.get_rwsip(info_dict['evals_1'], eigenvectors_1, info_dict['evals_2'], eigenvectors_2)
         info_dict['similarityIndex_rwsip'] = float("{:.3f}".format(rwsip))
+        dotp = self.dot_product_accum(eigenvectors_1, eigenvectors_2)
+        info_dict['similarityIndex_dotp'] = float("{:.3f}".format(dotp))
 
         with open(PurePath(self.tmp_folder).joinpath(temp_json), 'w') as out_file:
             out_file.write(json.dumps(info_dict, indent=4))
 
         # Copy outputs from temporary folder to output path
         shutil.copy2(PurePath(self.tmp_folder).joinpath(temp_json), PurePath(self.io_dict["out"]["output_json_path"]))
 
-        # Copy files to host
-        # self.copy_to_host()
-
         # remove temporary folder(s)
         self.tmp_files.extend([
-            # self.stage_io_dict.get("unique_dir"),
             self.tmp_folder
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_stiffness.py` & `biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_stiffness.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_unzip.py` & `biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_unzip.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_zip.py` & `biobb_flexserv-4.0.3/biobb_flexserv/pcasuite/pcz_zip.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv.egg-info/PKG-INFO` & `biobb_flexserv-4.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: biobb-flexserv
-Version: 4.0.2
+Name: biobb_flexserv
+Version: 4.0.3
 Summary: biobb_flexserv is a BioBB category for biomolecular flexibility studies on protein 3D structures.
 Home-page: https://github.com/bioexcel/biobb_flexserv
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_flexserv.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
```

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv.egg-info/SOURCES.txt` & `biobb_flexserv-4.0.3/biobb_flexserv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/biobb_flexserv.egg-info/entry_points.txt` & `biobb_flexserv-4.0.3/biobb_flexserv.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.2/setup.py` & `biobb_flexserv-4.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_flexserv",
-    version="4.0.2",
+    version="4.0.3",
     author="Biobb developers",
     author_email="adam.hospital@irbbarcelona.org",
     description="biobb_flexserv is a BioBB category for biomolecular flexibility studies on protein 3D structures.",
     long_description="biobb_flexserv allows the generation of protein conformational ensembles from 3D structures and the analysis of its molecular flexibility.",
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure",
     url="https://github.com/bioexcel/biobb_flexserv",
```

