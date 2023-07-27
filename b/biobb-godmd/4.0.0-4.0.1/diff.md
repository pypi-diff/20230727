# Comparing `tmp/biobb_godmd-4.0.0.tar.gz` & `tmp/biobb_godmd-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_godmd-4.0.0.tar", last modified: Wed Apr 12 10:57:24 2023, max compression
+gzip compressed data, was "dist/biobb_godmd-4.0.1.tar", last modified: Thu Jul 27 11:11:51 2023, max compression
```

## Comparing `biobb_godmd-4.0.0.tar` & `biobb_godmd-4.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2023-04-11 11:37:10.000000 biobb_godmd-4.0.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      912 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5295 2023-04-12 10:52:11.000000 biobb_godmd-4.0.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       63 2023-04-12 10:50:04.000000 biobb_godmd-4.0.0/biobb_godmd/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd/godmd/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       53 2023-04-11 11:37:10.000000 biobb_godmd-4.0.0/biobb_godmd/godmd/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2246 2023-04-12 10:26:31.000000 biobb_godmd-4.0.0/biobb_godmd/godmd/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    16873 2023-04-12 10:26:31.000000 biobb_godmd-4.0.0/biobb_godmd/godmd/godmd_prep.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15081 2023-04-12 10:27:51.000000 biobb_godmd-4.0.0/biobb_godmd/godmd/godmd_run.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd.egg-info/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      912 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      383 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      110 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       12 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/biobb_godmd.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-04-12 10:57:24.000000 biobb_godmd-4.0.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1398 2023-04-12 10:49:40.000000 biobb_godmd-4.0.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573    11357 2023-04-11 11:37:10.000000 biobb_godmd-4.0.1/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1011 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     5295 2023-07-27 11:10:07.000000 biobb_godmd-4.0.1/README.md
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       63 2023-07-27 11:09:06.000000 biobb_godmd-4.0.1/biobb_godmd/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd/godmd/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       53 2023-04-11 11:37:10.000000 biobb_godmd-4.0.1/biobb_godmd/godmd/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2281 2023-07-27 10:53:24.000000 biobb_godmd-4.0.1/biobb_godmd/godmd/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16873 2023-04-12 10:26:31.000000 biobb_godmd-4.0.1/biobb_godmd/godmd/godmd_prep.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16069 2023-07-27 10:53:24.000000 biobb_godmd-4.0.1/biobb_godmd/godmd/godmd_run.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1011 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      383 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      110 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       12 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1495 2023-07-27 11:08:46.000000 biobb_godmd-4.0.1/setup.py
```

### Comparing `biobb_godmd-4.0.0/LICENSE` & `biobb_godmd-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_godmd-4.0.0/PKG-INFO` & `biobb_godmd-4.0.1/biobb_godmd.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
-Name: biobb_godmd
-Version: 4.0.0
+Name: biobb-godmd
+Version: 4.0.1
 Summary: Biobb_godmd is a BioBB category for GOdMD tool (protein conformational transitions).
 Home-page: https://github.com/bioexcel/biobb_godmd
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_godmd.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Ensemble Protein Transitions GOdMD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
-Requires-Python: >=3.7,<=3.10
+Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Biobb_godmd allows the calculation of protein conformational transitions using the GOdMD tool.
```

### Comparing `biobb_godmd-4.0.0/README.md` & `biobb_godmd-4.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_godmd?label=Version)](https://GitHub.com/bioexcel/biobb_godmd/tags/)
 [![](https://img.shields.io/pypi/v/biobb-godmd.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-godmd/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_godmd?label=Conda)](https://anaconda.org/bioconda/biobb_godmd)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_godmd?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_godmd)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_godmd?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_godmd:4.0.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_godmd:4.0.1--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_godmd)
 [![](https://img.shields.io/pypi/pyversions/biobb-godmd.svg?label=Python%20Versions)](https://pypi.org/project/biobb-godmd/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_godmd)
 
 [![](https://readthedocs.org/projects/biobb-godmd/badge/?version=latest&label=Docs)](https://biobb-godmd.readthedocs.io/en/latest/?badge=latest)
@@ -30,61 +30,61 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_godmd.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.0 2022.3
+v4.0.1 2023.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_godmd>=4.0.0"
+        pip install "biobb_godmd>=4.0.1"
 
 
 * Usage: [Python API documentation](https://biobb-godmd.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_godmd>=4.0.0"
+        conda install -c bioconda "biobb_godmd>=4.0.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-godmd.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-godmd.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_godmd:4.0.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_godmd:4.0.1--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_godmd:4.0.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_godmd:4.0.1--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_godmd.sif https://depot.galaxyproject.org/singularity/biobb_godmd:4.0.0--pyhdfd78af_0
+        singularity pull --name biobb_godmd.sif https://depot.galaxyproject.org/singularity/biobb_godmd:4.0.1--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_godmd.sif <command>
```

### Comparing `biobb_godmd-4.0.0/biobb_godmd/godmd/common.py` & `biobb_godmd-4.0.1/biobb_godmd/godmd/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,9 +42,10 @@
         'input_aln_target_path': ['aln', 'txt'],
         'input_config_path': ['in', 'txt'],
         'output_aln_orig_path': ['aln', 'txt'],
         'output_aln_target_path': ['aln', 'txt'],
         'output_log_path': ['log', 'out', 'txt'],
         'output_ene_path': ['log', 'out', 'txt'],
         'output_trj_path': ['x', 'trj', 'crd', 'mdcrd'],
+        'output_pdb_path': ['pdb']
     }
     return ext in formats[argument]
```

### Comparing `biobb_godmd-4.0.0/biobb_godmd/godmd/godmd_prep.py` & `biobb_godmd-4.0.1/biobb_godmd/godmd/godmd_prep.py`

 * *Files identical despite different names*

### Comparing `biobb_godmd-4.0.0/biobb_godmd/godmd/godmd_run.py` & `biobb_godmd-4.0.1/biobb_godmd/godmd/godmd_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 
 """Module containing the GOdMDRun class and the command line interface."""
 import argparse
+import shutil
 from pathlib import Path
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 from biobb_godmd.godmd.common import check_input_path, check_output_path
 
 
@@ -21,14 +23,15 @@
         input_pdb_target_path (str): Input PDB file to be used as target in the conformational transition. File type: input. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/data/godmd/4ake_A.pdb>`_. Accepted formats: pdb (edam:format_1476).
         input_aln_orig_path (str): Input GOdMD alignment file corresponding to the origin structure of the conformational transition. File type: input. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/data/godmd/1ake_A.aln>`_. Accepted formats: aln (edam:format_2330), txt (edam:format_2330).
         input_aln_target_path (str): Input GOdMD alignment file corresponding to the target structure of the conformational transition. File type: input. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/data/godmd/4ake_A.aln>`_. Accepted formats: aln (edam:format_2330), txt (edam:format_2330).
         input_config_path (str) (Optional): Input GOdMD configuration file. File type: input. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/data/godmd/params.in>`_. Accepted formats: in (edam:format_2330), txt (edam:format_2330).
         output_log_path (str): Output log file. File type: output. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/reference/godmd/godmd.log>`_. Accepted formats: log (edam:format_2330), out (edam:format_2330), txt (edam:format_2330), o (edam:format_2330).
         output_ene_path (str): Output energy file. File type: output. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/reference/godmd/godmd_ene.out>`_. Accepted formats: log (edam:format_2330), out (edam:format_2330), txt (edam:format_2330), o (edam:format_2330).
         output_trj_path (str): Output trajectory file. File type: output. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/reference/godmd/godmd_trj.mdcrd>`_. Accepted formats: trj (edam:format_3878), crd (edam:format_3878), mdcrd (edam:format_3878), x (edam:format_3878).
+        output_pdb_path (str): Output structure file. File type: output. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/reference/godmd/godmd_pdb.pdb>`_. Accepted formats: pdb (edam:format_1476).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **godmdin** (*dict*) - ({}) GOdMD options specification.
             * **binary_path** (*str*) - ("discrete") Binary path.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
@@ -41,29 +44,30 @@
             godmd_run(   input_pdb_orig_path='/path/to/pdb_orig.pdb',
                          input_pdb_target_path='/path/to/pdb_target.pdb',
                          input_aln_orig_path='/path/to/aln_orig.aln',
                          input_aln_target_path='/path/to/aln_target.aln',
                          output_log_path='/path/to/godmd_log.log',
                          output_ene_path='/path/to/godmd_ene.txt',
                          output_trj_path='/path/to/godmd_trj.mdcrd',
+                         output_pdb_path='/path/to/godmd_pdb.pdb',
                          properties=prop)
 
     Info:
         * wrapped_software:
             * name: GOdMD
             * version: >=1.0
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
     def __init__(self, input_pdb_orig_path: str, input_pdb_target_path: str,
                  input_aln_orig_path: str, input_aln_target_path: str, input_config_path: str,
-                 output_log_path: str, output_ene_path: str, output_trj_path: str,
+                 output_log_path: str, output_ene_path: str, output_trj_path: str, output_pdb_path: str,
                  properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
@@ -73,15 +77,16 @@
             'in': {'input_pdb_orig_path': input_pdb_orig_path,
                    'input_pdb_target_path': input_pdb_target_path,
                    'input_aln_orig_path': input_aln_orig_path,
                    'input_aln_target_path': input_aln_target_path,
                    'input_config_path': input_config_path},
             'out': {'output_log_path': output_log_path,
                     'output_ene_path': output_ene_path,
-                    'output_trj_path': output_trj_path}
+                    'output_trj_path': output_trj_path,
+                    'output_pdb_path': output_pdb_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.godmdin = {k: str(v) for k, v in properties.get('godmdin', dict()).items()}
         self.binary_path = properties.get('binary_path', "discrete")
 
@@ -99,14 +104,15 @@
         self.io_dict["in"]["input_aln_target_path"] = check_input_path(self.io_dict["in"]["input_aln_target_path"], "input_aln_target_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_config_path"] = check_input_path(self.io_dict["in"]["input_config_path"], "input_config_path", True, out_log, self.__class__.__name__)
 
         # Check output(s)
         self.io_dict["out"]["output_log_path"] = check_output_path(self.io_dict["out"]["output_log_path"], "output_log_path", False, out_log, self.__class__.__name__)
         self.io_dict["out"]["output_ene_path"] = check_output_path(self.io_dict["out"]["output_ene_path"], "output_ene_path", False, out_log, self.__class__.__name__)
         self.io_dict["out"]["output_trj_path"] = check_output_path(self.io_dict["out"]["output_trj_path"], "output_trj_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"], "output_pdb_path", False, out_log, self.__class__.__name__)
 
     def create_godmdin(self, path: str = None) -> str:
         """Creates a GOdMD configuration file (godmdin) using the properties file settings"""
         godmdin_list = []
 
         self.output_godmdin_path = path
 
@@ -183,14 +189,17 @@
                     '-ener', self.io_dict["out"]["output_ene_path"],
                     '-trj', self.io_dict["out"]["output_trj_path"]
                     ]
 
         # Run Biobb block
         self.run_biobb()
 
+        # Copy outputs from temporary folder to output path
+        shutil.copy2("reference.pdb", PurePath(self.io_dict["out"]["output_pdb_path"]).name)
+
         # Copy files to host
         self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
             self.stage_io_dict.get("unique_dir"),
             self.tmp_folder
@@ -200,27 +209,28 @@
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
 
 def godmd_run(input_pdb_orig_path: str, input_pdb_target_path: str,
               input_aln_orig_path: str, input_aln_target_path: str,
-              output_log_path: str, output_ene_path: str, output_trj_path: str,
+              output_log_path: str, output_ene_path: str, output_trj_path: str, output_pdb_path: str,
               input_config_path: str = None, properties: dict = None, **kwargs) -> int:
     """Create :class:`GOdMDRun <godmd.godmd_run.GOdMDRun>`godmd.godmd_run.GOdMDRun class and
     execute :meth:`launch() <godmd.godmd_run.GOdMDRun.launch>` method"""
 
     return GOdMDRun(input_pdb_orig_path=input_pdb_orig_path,
                     input_pdb_target_path=input_pdb_target_path,
                     input_aln_orig_path=input_aln_orig_path,
                     input_aln_target_path=input_aln_target_path,
                     input_config_path=input_config_path,
                     output_log_path=output_log_path,
                     output_ene_path=output_ene_path,
                     output_trj_path=output_trj_path,
+                    output_pdb_path=output_pdb_path,
                     properties=properties).launch()
 
 
 def main():
     parser = argparse.ArgumentParser(description='Computing conformational transition trajectories for proteins using GOdMD tool.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
@@ -230,14 +240,15 @@
     required_args.add_argument('--input_pdb_target_path', required=True, help='Input PDB file to be used as target in the conformational transition. Accepted formats: pdb.')
     required_args.add_argument('--input_aln_orig_path', required=True, help='Input GOdMD alignment file corresponding to the origin structure of the conformational transition. Accepted formats: aln, txt.')
     required_args.add_argument('--input_aln_target_path', required=True, help='Input GOdMD alignment file corresponding to the target structure of the conformational transition. Accepted formats: aln, txt.')
     required_args.add_argument('--input_config_path', required=False, help='Input configuration file (GOdMD run options). Accepted formats: in, txt.')
     required_args.add_argument('--output_log_path', required=True, help='Output log file. Accepted formats: log, out, txt.')
     required_args.add_argument('--output_ene_path', required=True, help='Output energy file. Accepted formats: log, out, txt.')
     required_args.add_argument('--output_trj_path', required=True, help='Output trajectory file. Accepted formats: mdcrd.')
+    required_args.add_argument('--output_pdb_path', required=True, help='Output structure file. Accepted formats: pdb.')
 
     args = parser.parse_args()
     # config = args.config if args.config else None
     args.config = args.config or "{}"
     # properties = settings.ConfReader(config=config).get_prop_dic()
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
@@ -246,12 +257,13 @@
               input_pdb_target_path=args.input_pdb_target_path,
               input_aln_orig_path=args.input_aln_orig_path,
               input_aln_target_path=args.input_aln_target_path,
               input_config_path=args.input_config_path,
               output_log_path=args.output_log_path,
               output_ene_path=args.output_ene_path,
               output_trj_path=args.output_trj_path,
+              output_pdb_path=args.output_pdb_path,
               properties=properties)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_godmd-4.0.0/biobb_godmd.egg-info/PKG-INFO` & `biobb_godmd-4.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
-Name: biobb-godmd
-Version: 4.0.0
+Name: biobb_godmd
+Version: 4.0.1
 Summary: Biobb_godmd is a BioBB category for GOdMD tool (protein conformational transitions).
 Home-page: https://github.com/bioexcel/biobb_godmd
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_godmd.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Ensemble Protein Transitions GOdMD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
-Requires-Python: >=3.7,<=3.10
+Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Biobb_godmd allows the calculation of protein conformational transitions using the GOdMD tool.
```

### Comparing `biobb_godmd-4.0.0/setup.py` & `biobb_godmd-4.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_godmd",
-    version="4.0.0",
+    version="4.0.1",
     author="Biobb developers",
     author_email="adam.hospital@irbbarcelona.org",
     description="Biobb_godmd is a BioBB category for GOdMD tool (protein conformational transitions).",
     long_description="Biobb_godmd allows the calculation of protein conformational transitions using the GOdMD tool.",
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility Ensemble Protein Transitions GOdMD",
     url="https://github.com/bioexcel/biobb_godmd",
     project_urls={
         "Documentation": "http://biobb_godmd.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
     install_requires=['biobb_common==4.0.0'],
-    python_requires='>=3.7,<=3.10',
+    python_requires='>=3.7,<3.10',
     entry_points={
         "console_scripts": [
             "godmd_prep = biobb_godmd.godmd.godmd_prep:main",
             "godmd_run = biobb_godmd.godmd.godmd_run:main"
         ]
     },
     classifiers=(
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
     ),
 )
```

