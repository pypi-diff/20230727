# Comparing `tmp/fsl-pipe-0.7.0.tar.gz` & `tmp/fsl-pipe-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsl-pipe-0.7.0.tar", last modified: Fri Jul  7 15:40:22 2023, max compression
+gzip compressed data, was "fsl-pipe-1.0.0.tar", last modified: Thu Jul 27 14:04:27 2023, max compression
```

## Comparing `fsl-pipe-0.7.0.tar` & `fsl-pipe-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:40:22.092599 fsl-pipe-0.7.0/
--rw-rw-rw-   0 root         (0) root         (0)     1094 2023-03-28 12:35:56.000000 fsl-pipe-0.7.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-03-29 09:39:12.000000 fsl-pipe-0.7.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2796 2023-07-07 15:40:22.092599 fsl-pipe-0.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2280 2023-04-17 12:08:35.000000 fsl-pipe-0.7.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-03-28 12:35:56.000000 fsl-pipe-0.7.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1003 2023-07-07 15:40:22.093599 fsl-pipe-0.7.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:40:22.089599 fsl-pipe-0.7.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:40:22.091600 fsl-pipe-0.7.0/src/fsl_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-07 13:58:51.000000 fsl-pipe-0.7.0/src/fsl_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1233 2023-03-28 12:35:56.000000 fsl-pipe-0.7.0/src/fsl_pipe/datalad.py
--rw-rw-rw-   0 root         (0) root         (0)    33496 2023-07-07 12:21:17.000000 fsl-pipe-0.7.0/src/fsl_pipe/job.py
--rw-rw-rw-   0 root         (0) root         (0)    37846 2023-07-07 13:57:09.000000 fsl-pipe-0.7.0/src/fsl_pipe/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      162 2023-03-28 12:35:56.000000 fsl-pipe-0.7.0/src/fsl_pipe/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:40:22.092599 fsl-pipe-0.7.0/src/fsl_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2796 2023-07-07 15:40:22.000000 fsl-pipe-0.7.0/src/fsl_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-07 15:40:22.000000 fsl-pipe-0.7.0/src/fsl_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:40:22.000000 fsl-pipe-0.7.0/src/fsl_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-07-07 15:40:22.000000 fsl-pipe-0.7.0/src/fsl_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-07 15:40:22.000000 fsl-pipe-0.7.0/src/fsl_pipe.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:04:27.056511 fsl-pipe-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2023-03-28 12:35:56.000000 fsl-pipe-1.0.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-03-29 09:39:12.000000 fsl-pipe-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3617 2023-07-27 14:04:27.056511 fsl-pipe-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2023-07-27 13:39:54.000000 fsl-pipe-1.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-03-28 12:35:56.000000 fsl-pipe-1.0.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2023-07-27 14:04:27.057511 fsl-pipe-1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:04:27.054511 fsl-pipe-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:04:27.055511 fsl-pipe-1.0.0/src/fsl_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-27 13:57:26.000000 fsl-pipe-1.0.0/src/fsl_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-03-28 12:35:56.000000 fsl-pipe-1.0.0/src/fsl_pipe/datalad.py
+-rw-rw-rw-   0 root         (0) root         (0)    33496 2023-07-07 12:21:17.000000 fsl-pipe-1.0.0/src/fsl_pipe/job.py
+-rw-rw-rw-   0 root         (0) root         (0)    37846 2023-07-07 13:57:09.000000 fsl-pipe-1.0.0/src/fsl_pipe/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-03-28 12:35:56.000000 fsl-pipe-1.0.0/src/fsl_pipe/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:04:27.056511 fsl-pipe-1.0.0/src/fsl_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3617 2023-07-27 14:04:27.000000 fsl-pipe-1.0.0/src/fsl_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-27 14:04:27.000000 fsl-pipe-1.0.0/src/fsl_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 14:04:27.000000 fsl-pipe-1.0.0/src/fsl_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-27 14:04:27.000000 fsl-pipe-1.0.0/src/fsl_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-27 14:04:27.000000 fsl-pipe-1.0.0/src/fsl_pipe.egg-info/top_level.txt
```

### Comparing `fsl-pipe-0.7.0/LICENSE` & `fsl-pipe-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fsl-pipe-0.7.0/PKG-INFO` & `fsl-pipe-1.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,20 @@
-Metadata-Version: 2.1
-Name: fsl-pipe
-Version: 0.7.0
-Summary: Declative pipelines based on Filetrees
-Home-page: https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe
-Author: Michiel Cottaar
-Author-email: michiel.cottaar@ndcn.ox.ac.uk
-Project-URL: Bug Tracker, https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/-/issues
-Project-URL: Documentation, https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Documentation](https://img.shields.io/badge/Documentation-fsl--pipe-blue)](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe)
 [![File-tree Documentation](https://img.shields.io/badge/Documentation-file--tree-blue)](https://open.win.ox.ac.uk/pages/ndcn0236/file-tree)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6577069.svg)](https://doi.org/10.5281/zenodo.6577069)
 [![Pipeline status](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/badges/main/pipeline.svg)](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/-/pipelines/latest)
 [![Coverage report](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/badges/main/coverage.svg)](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe/htmlcov)
 
-Declative pipelines based on Filetrees
+Declative pipelines based on Filetrees. A pipeline is defined by:
+- A file-tree, which defines the directory structure of the inputs and outputs of the pipeline. A tutorial on these file-trees is available [here](https://open.win.ox.ac.uk/pages/ndcn0236/file-tree).
+- A set of recipes describing how all the pipeline outputs are produced. A tutorial on writing these recipes is available [here](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe).
+Fsl-pipe will stitch these recipes together to produce any user-selected output files.
+Resulting jobs will either run locally, run distributed using [dask](https://www.dask.org), or be submitted to a cluster using [fsl-sub](https://git.fmrib.ox.ac.uk/fsl/fsl_sub).
+
+An example diffusion MRI pipeline using fsl-pipe with detailed comments is available [here](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe-example).
 
 # Installation
 ```shell
 pip install fsl-pipe
 ```
 
 Any bug reports and feature requests are very welcome (see [issue tracker](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/-/issues)).
```

### Comparing `fsl-pipe-0.7.0/setup.cfg` & `fsl-pipe-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.7.0
+current_version = 1.0.0
 commit = True
 tag = True
 
 [bumpversion:file:src/fsl_pipe/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
```

### Comparing `fsl-pipe-0.7.0/src/fsl_pipe/datalad.py` & `fsl-pipe-1.0.0/src/fsl_pipe/datalad.py`

 * *Files identical despite different names*

### Comparing `fsl-pipe-0.7.0/src/fsl_pipe/job.py` & `fsl-pipe-1.0.0/src/fsl_pipe/job.py`

 * *Files identical despite different names*

### Comparing `fsl-pipe-0.7.0/src/fsl_pipe/pipeline.py` & `fsl-pipe-1.0.0/src/fsl_pipe/pipeline.py`

 * *Files identical despite different names*

### Comparing `fsl-pipe-0.7.0/src/fsl_pipe.egg-info/PKG-INFO` & `fsl-pipe-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsl-pipe
-Version: 0.7.0
+Version: 1.0.0
 Summary: Declative pipelines based on Filetrees
 Home-page: https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe
 Author: Michiel Cottaar
 Author-email: michiel.cottaar@ndcn.ox.ac.uk
 Project-URL: Bug Tracker, https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/-/issues
 Project-URL: Documentation, https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,21 @@
 
 [![Documentation](https://img.shields.io/badge/Documentation-fsl--pipe-blue)](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe)
 [![File-tree Documentation](https://img.shields.io/badge/Documentation-file--tree-blue)](https://open.win.ox.ac.uk/pages/ndcn0236/file-tree)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6577069.svg)](https://doi.org/10.5281/zenodo.6577069)
 [![Pipeline status](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/badges/main/pipeline.svg)](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/-/pipelines/latest)
 [![Coverage report](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/badges/main/coverage.svg)](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe/htmlcov)
 
-Declative pipelines based on Filetrees
+Declative pipelines based on Filetrees. A pipeline is defined by:
+- A file-tree, which defines the directory structure of the inputs and outputs of the pipeline. A tutorial on these file-trees is available [here](https://open.win.ox.ac.uk/pages/ndcn0236/file-tree).
+- A set of recipes describing how all the pipeline outputs are produced. A tutorial on writing these recipes is available [here](https://open.win.ox.ac.uk/pages/ndcn0236/fsl-pipe).
+Fsl-pipe will stitch these recipes together to produce any user-selected output files.
+Resulting jobs will either run locally, run distributed using [dask](https://www.dask.org), or be submitted to a cluster using [fsl-sub](https://git.fmrib.ox.ac.uk/fsl/fsl_sub).
+
+An example diffusion MRI pipeline using fsl-pipe with detailed comments is available [here](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe-example).
 
 # Installation
 ```shell
 pip install fsl-pipe
 ```
 
 Any bug reports and feature requests are very welcome (see [issue tracker](https://git.fmrib.ox.ac.uk/ndcn0236/fsl-pipe/-/issues)).
```

