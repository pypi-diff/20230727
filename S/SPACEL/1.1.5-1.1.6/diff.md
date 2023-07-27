# Comparing `tmp/SPACEL-1.1.5.tar.gz` & `tmp/SPACEL-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPACEL-1.1.5.tar", last modified: Wed Jul 26 13:43:28 2023, max compression
+gzip compressed data, was "SPACEL-1.1.6.tar", last modified: Thu Jul 27 12:45:42 2023, max compression
```

## Comparing `SPACEL-1.1.5.tar` & `SPACEL-1.1.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-26 13:43:28.489902 SPACEL-1.1.5/
--rw-r--r--   0 xuhao      (501) staff       (20)     5069 2023-07-26 13:43:28.489531 SPACEL-1.1.5/PKG-INFO
--rw-r--r--   0 xuhao      (501) staff       (20)     4768 2023-07-26 13:34:25.000000 SPACEL-1.1.5/README.md
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-26 13:43:28.314942 SPACEL-1.1.5/SPACEL/
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-26 13:43:28.408151 SPACEL-1.1.5/SPACEL/Scube/
--rw-r--r--   0 xuhao      (501) staff       (20)      151 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Scube/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)    13309 2023-07-11 12:14:50.000000 SPACEL-1.1.5/SPACEL/Scube/alignment.py
--rw-r--r--   0 xuhao      (501) staff       (20)    16402 2023-07-13 00:51:58.000000 SPACEL-1.1.5/SPACEL/Scube/gpr.py
--rw-r-----   0 xuhao      (501) staff       (20)     6191 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Scube/plot.py
--rw-r--r--   0 xuhao      (501) staff       (20)     6635 2023-07-12 13:05:31.000000 SPACEL-1.1.5/SPACEL/Scube/utils_3d.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-26 13:43:28.482003 SPACEL-1.1.5/SPACEL/Splane/
--rw-r--r--   0 xuhao      (501) staff       (20)      149 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Splane/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)    14649 2023-07-26 13:07:52.000000 SPACEL-1.1.5/SPACEL/Splane/base_model.py
--rw-r--r--   0 xuhao      (501) staff       (20)     1627 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Splane/graph.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-26 13:43:28.483791 SPACEL-1.1.5/SPACEL/Splane/kegra/
--rw-r--r--   0 xuhao      (501) staff       (20)        0 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Splane/kegra/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4662 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Splane/kegra/gnn.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4658 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Splane/kegra/gnn_utils.py
--rw-r--r--   0 xuhao      (501) staff       (20)     3688 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Splane/model.py
--rw-r--r--   0 xuhao      (501) staff       (20)     2050 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Splane/pygcn_utils.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4269 2023-07-13 01:47:26.000000 SPACEL-1.1.5/SPACEL/Splane/utils.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-26 13:43:28.488694 SPACEL-1.1.5/SPACEL/Spoint/
--rw-r--r--   0 xuhao      (501) staff       (20)      138 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Spoint/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)    27194 2023-07-11 09:03:42.000000 SPACEL-1.1.5/SPACEL/Spoint/base_model.py
--rw-r--r--   0 xuhao      (501) staff       (20)     1332 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Spoint/data_augmentation.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4007 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Spoint/data_downsample.py
--rw-r--r--   0 xuhao      (501) staff       (20)     6788 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Spoint/data_utils.py
--rw-r--r--   0 xuhao      (501) staff       (20)     1017 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Spoint/metrics.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4998 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Spoint/model.py
--rw-r--r--   0 xuhao      (501) staff       (20)    20829 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/Spoint/spatial_simulation.py
--rw-r--r--   0 xuhao      (501) staff       (20)      226 2023-07-12 13:29:08.000000 SPACEL-1.1.5/SPACEL/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)       32 2023-07-26 13:42:03.000000 SPACEL-1.1.5/SPACEL/_version.py
--rw-r--r--   0 xuhao      (501) staff       (20)      719 2023-07-11 08:15:35.000000 SPACEL-1.1.5/SPACEL/setting.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-26 13:43:28.316779 SPACEL-1.1.5/SPACEL.egg-info/
--rw-r--r--   0 xuhao      (501) staff       (20)     5069 2023-07-26 13:43:28.000000 SPACEL-1.1.5/SPACEL.egg-info/PKG-INFO
--rw-r--r--   0 xuhao      (501) staff       (20)      818 2023-07-26 13:43:28.000000 SPACEL-1.1.5/SPACEL.egg-info/SOURCES.txt
--rw-r--r--   0 xuhao      (501) staff       (20)        1 2023-07-26 13:43:28.000000 SPACEL-1.1.5/SPACEL.egg-info/dependency_links.txt
--rw-r--r--   0 xuhao      (501) staff       (20)       82 2023-07-26 13:43:28.000000 SPACEL-1.1.5/SPACEL.egg-info/requires.txt
--rw-r--r--   0 xuhao      (501) staff       (20)        7 2023-07-26 13:43:28.000000 SPACEL-1.1.5/SPACEL.egg-info/top_level.txt
--rw-r--r--   0 xuhao      (501) staff       (20)       38 2023-07-26 13:43:28.489997 SPACEL-1.1.5/setup.cfg
--rw-r--r--   0 xuhao      (501) staff       (20)      815 2023-07-14 02:56:55.000000 SPACEL-1.1.5/setup.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-27 12:45:42.115898 SPACEL-1.1.6/
+-rw-r--r--   0 xuhao      (501) staff       (20)     4844 2023-07-27 12:45:42.115530 SPACEL-1.1.6/PKG-INFO
+-rw-r--r--   0 xuhao      (501) staff       (20)     4543 2023-07-27 12:44:07.000000 SPACEL-1.1.6/README.md
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-27 12:45:42.103496 SPACEL-1.1.6/SPACEL/
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-27 12:45:42.107942 SPACEL-1.1.6/SPACEL/Scube/
+-rw-r--r--   0 xuhao      (501) staff       (20)      151 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Scube/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    13309 2023-07-11 12:14:50.000000 SPACEL-1.1.6/SPACEL/Scube/alignment.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    16402 2023-07-13 00:51:58.000000 SPACEL-1.1.6/SPACEL/Scube/gpr.py
+-rw-r-----   0 xuhao      (501) staff       (20)     6191 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Scube/plot.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     6635 2023-07-12 13:05:31.000000 SPACEL-1.1.6/SPACEL/Scube/utils_3d.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-27 12:45:42.110746 SPACEL-1.1.6/SPACEL/Splane/
+-rw-r--r--   0 xuhao      (501) staff       (20)      149 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Splane/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    14756 2023-07-27 12:44:07.000000 SPACEL-1.1.6/SPACEL/Splane/base_model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     1627 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Splane/graph.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-27 12:45:42.111783 SPACEL-1.1.6/SPACEL/Splane/kegra/
+-rw-r--r--   0 xuhao      (501) staff       (20)        0 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Splane/kegra/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4662 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Splane/kegra/gnn.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4658 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Splane/kegra/gnn_utils.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     3688 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Splane/model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     2050 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Splane/pygcn_utils.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4269 2023-07-13 01:47:26.000000 SPACEL-1.1.6/SPACEL/Splane/utils.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-27 12:45:42.115032 SPACEL-1.1.6/SPACEL/Spoint/
+-rw-r--r--   0 xuhao      (501) staff       (20)      138 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Spoint/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    27194 2023-07-11 09:03:42.000000 SPACEL-1.1.6/SPACEL/Spoint/base_model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     1332 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Spoint/data_augmentation.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4007 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Spoint/data_downsample.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     6788 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Spoint/data_utils.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     1017 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Spoint/metrics.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4998 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Spoint/model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    20829 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/Spoint/spatial_simulation.py
+-rw-r--r--   0 xuhao      (501) staff       (20)      226 2023-07-12 13:29:08.000000 SPACEL-1.1.6/SPACEL/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)       32 2023-07-27 12:44:07.000000 SPACEL-1.1.6/SPACEL/_version.py
+-rw-r--r--   0 xuhao      (501) staff       (20)      719 2023-07-11 08:15:35.000000 SPACEL-1.1.6/SPACEL/setting.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-27 12:45:42.105279 SPACEL-1.1.6/SPACEL.egg-info/
+-rw-r--r--   0 xuhao      (501) staff       (20)     4844 2023-07-27 12:45:42.000000 SPACEL-1.1.6/SPACEL.egg-info/PKG-INFO
+-rw-r--r--   0 xuhao      (501) staff       (20)      818 2023-07-27 12:45:42.000000 SPACEL-1.1.6/SPACEL.egg-info/SOURCES.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)        1 2023-07-27 12:45:42.000000 SPACEL-1.1.6/SPACEL.egg-info/dependency_links.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)       82 2023-07-27 12:45:42.000000 SPACEL-1.1.6/SPACEL.egg-info/requires.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)        7 2023-07-27 12:45:42.000000 SPACEL-1.1.6/SPACEL.egg-info/top_level.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)       38 2023-07-27 12:45:42.115992 SPACEL-1.1.6/setup.cfg
+-rw-r--r--   0 xuhao      (501) staff       (20)      815 2023-07-14 02:56:55.000000 SPACEL-1.1.6/setup.py
```

### Comparing `SPACEL-1.1.5/PKG-INFO` & `SPACEL-1.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPACEL
-Version: 1.1.5
+Version: 1.1.6
 Summary: SPACEL: characterizing spatial transcriptome architectures by deep-learning
 Home-page: https://github.com/QuKunLab/SPACEL
 Author: Hao Xu
 Author-email: xuhaoustc@mail.ustc.edu.cn
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -32,32 +32,30 @@
     * [SPACEL workflow (1/3): Deconvolution by Spoint on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Spoint.ipynb)
     * [SPACEL workflow (2/3): Identification of spatial domain by Splane on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Splane.ipynb)
     * [SPACEL workflow (3/3): Alignment 3D tissue by Scube on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Scube.ipynb)
 
 Read the [documentation](https://spacel.readthedocs.io) for more information.
 
 ## Latest updates
+### Version 1.1.6 2023-07-27
+#### Fixed Bugs
+- Fixed a bug regarding the similarity loss weight hyperparameter `simi_l`, which in the previous version did not affect the loss value.
+
 ### Version 1.1.5 2023-07-26
 #### Fixed Bugs
 - Fixed a bug in the similarity loss of Splane, where it minimized the cosine similarity of the latent vectors of spots with their neighbors.
 #### Features
 - Optimized the time and memory consumption of the Splane training process for large datasets.
 
 ### Version 1.1.2 2023-07-12
 #### Fixed Bugs
 - Removed `rpy2` from the pypi dependency of SPACEL. It now needs to be pre-installed when creating the environment through conda.
 - Fixed a bug in Scube where the `best_model_state` was not referenced before being used.
 #### Features
 - Added function documentations for Scube related to the GPR model.
-
-### Version 1.1.1 2023-07-11
-#### Features
-* All code based on `Tensorflow` have been mirated to `PyTorch`, it does not have `Tensorflow` as dependency anymore.
-* The `Splane.utils.add_cell_type_composition` function has been implemented to facilitate the cell type composition predicted by deconvolution methods into Splane.
-* Spoint and Splane now support tqdm type output for improved progress tracking.
     
 ## Requirements
 **Note**: The current version of SPACEL only supports Linux and MacOS, not Windows platform. 
 
 To install `SPACEL`, you need to install [PyTorch](https://pytorch.org) with GPU support first. If you don't need GPU acceleration, you can just skip the installation for `cudnn` and `cudatoolkit`.
 * Create conda environment for `SPACEL`:
 ```
```

### Comparing `SPACEL-1.1.5/README.md` & `SPACEL-1.1.6/SPACEL.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: SPACEL
+Version: 1.1.6
+Summary: SPACEL: characterizing spatial transcriptome architectures by deep-learning
+Home-page: https://github.com/QuKunLab/SPACEL
+Author: Hao Xu
+Author-email: xuhaoustc@mail.ustc.edu.cn
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 [![Documentation Status](https://readthedocs.org/projects/spacel/badge/?version=latest)](https://spacel.readthedocs.io/en/latest/?badge=latest)
 ![PyPI](https://img.shields.io/pypi/v/SPACEL)
 
 # SPACEL: characterizing spatial transcriptome architectures by deep-learning
 
 ![](docs/_static/img/figure1.png "Overview")
 SPACEL (**SP**atial **A**rchitecture **C**haracterization by d**E**ep **L**earning) is a Python package of deep-learning-based methods for ST data analysis. SPACEL consists of three modules: 
@@ -22,32 +32,30 @@
     * [SPACEL workflow (1/3): Deconvolution by Spoint on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Spoint.ipynb)
     * [SPACEL workflow (2/3): Identification of spatial domain by Splane on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Splane.ipynb)
     * [SPACEL workflow (3/3): Alignment 3D tissue by Scube on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Scube.ipynb)
 
 Read the [documentation](https://spacel.readthedocs.io) for more information.
 
 ## Latest updates
+### Version 1.1.6 2023-07-27
+#### Fixed Bugs
+- Fixed a bug regarding the similarity loss weight hyperparameter `simi_l`, which in the previous version did not affect the loss value.
+
 ### Version 1.1.5 2023-07-26
 #### Fixed Bugs
 - Fixed a bug in the similarity loss of Splane, where it minimized the cosine similarity of the latent vectors of spots with their neighbors.
 #### Features
 - Optimized the time and memory consumption of the Splane training process for large datasets.
 
 ### Version 1.1.2 2023-07-12
 #### Fixed Bugs
 - Removed `rpy2` from the pypi dependency of SPACEL. It now needs to be pre-installed when creating the environment through conda.
 - Fixed a bug in Scube where the `best_model_state` was not referenced before being used.
 #### Features
 - Added function documentations for Scube related to the GPR model.
-
-### Version 1.1.1 2023-07-11
-#### Features
-* All code based on `Tensorflow` have been mirated to `PyTorch`, it does not have `Tensorflow` as dependency anymore.
-* The `Splane.utils.add_cell_type_composition` function has been implemented to facilitate the cell type composition predicted by deconvolution methods into Splane.
-* Spoint and Splane now support tqdm type output for improved progress tracking.
     
 ## Requirements
 **Note**: The current version of SPACEL only supports Linux and MacOS, not Windows platform. 
 
 To install `SPACEL`, you need to install [PyTorch](https://pytorch.org) with GPU support first. If you don't need GPU acceleration, you can just skip the installation for `cudnn` and `cudatoolkit`.
 * Create conda environment for `SPACEL`:
 ```
```

### Comparing `SPACEL-1.1.5/SPACEL/Scube/alignment.py` & `SPACEL-1.1.6/SPACEL/Scube/alignment.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Scube/gpr.py` & `SPACEL-1.1.6/SPACEL/Scube/gpr.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Scube/plot.py` & `SPACEL-1.1.6/SPACEL/Scube/plot.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Scube/utils_3d.py` & `SPACEL-1.1.6/SPACEL/Scube/utils_3d.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Splane/base_model.py` & `SPACEL-1.1.6/SPACEL/Splane/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,17 @@
 
         Returns:
             ``None``
         """
         best_loss = np.inf
         best_db_loss = np.inf
         best_simi_loss = np.inf
-        simi_l = 1/np.mean(self.morans_mean)
+        if simi_l is None:
+            simi_l = 1/np.mean(self.morans_mean)
+            print(f'Setting the weight of similarity loss to {simi_l:.3f}')
         
         if save_path is None:
             save_path = os.path.join(tempfile.gettempdir() ,'Splane_models_'+strftime("%Y%m%d%H%M%S",localtime()))
         if not os.path.exists(save_path):
             os.makedirs(save_path)
         early_stop_count = 0
         pbar = tqdm(range(max_epochs))
```

### Comparing `SPACEL-1.1.5/SPACEL/Splane/graph.py` & `SPACEL-1.1.6/SPACEL/Splane/graph.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Splane/kegra/gnn.py` & `SPACEL-1.1.6/SPACEL/Splane/kegra/gnn.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Splane/kegra/gnn_utils.py` & `SPACEL-1.1.6/SPACEL/Splane/kegra/gnn_utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Splane/model.py` & `SPACEL-1.1.6/SPACEL/Splane/model.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Splane/pygcn_utils.py` & `SPACEL-1.1.6/SPACEL/Splane/pygcn_utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Splane/utils.py` & `SPACEL-1.1.6/SPACEL/Splane/utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Spoint/base_model.py` & `SPACEL-1.1.6/SPACEL/Spoint/base_model.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Spoint/data_augmentation.py` & `SPACEL-1.1.6/SPACEL/Spoint/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Spoint/data_downsample.py` & `SPACEL-1.1.6/SPACEL/Spoint/data_downsample.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Spoint/data_utils.py` & `SPACEL-1.1.6/SPACEL/Spoint/data_utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Spoint/metrics.py` & `SPACEL-1.1.6/SPACEL/Spoint/metrics.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Spoint/model.py` & `SPACEL-1.1.6/SPACEL/Spoint/model.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/Spoint/spatial_simulation.py` & `SPACEL-1.1.6/SPACEL/Spoint/spatial_simulation.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL/setting.py` & `SPACEL-1.1.6/SPACEL/setting.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/SPACEL.egg-info/PKG-INFO` & `SPACEL-1.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: SPACEL
-Version: 1.1.5
-Summary: SPACEL: characterizing spatial transcriptome architectures by deep-learning
-Home-page: https://github.com/QuKunLab/SPACEL
-Author: Hao Xu
-Author-email: xuhaoustc@mail.ustc.edu.cn
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 [![Documentation Status](https://readthedocs.org/projects/spacel/badge/?version=latest)](https://spacel.readthedocs.io/en/latest/?badge=latest)
 ![PyPI](https://img.shields.io/pypi/v/SPACEL)
 
 # SPACEL: characterizing spatial transcriptome architectures by deep-learning
 
 ![](docs/_static/img/figure1.png "Overview")
 SPACEL (**SP**atial **A**rchitecture **C**haracterization by d**E**ep **L**earning) is a Python package of deep-learning-based methods for ST data analysis. SPACEL consists of three modules: 
@@ -32,32 +22,30 @@
     * [SPACEL workflow (1/3): Deconvolution by Spoint on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Spoint.ipynb)
     * [SPACEL workflow (2/3): Identification of spatial domain by Splane on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Splane.ipynb)
     * [SPACEL workflow (3/3): Alignment 3D tissue by Scube on mouse brain ST dataset](docs/tutorials/ST_mouse_brain_Scube.ipynb)
 
 Read the [documentation](https://spacel.readthedocs.io) for more information.
 
 ## Latest updates
+### Version 1.1.6 2023-07-27
+#### Fixed Bugs
+- Fixed a bug regarding the similarity loss weight hyperparameter `simi_l`, which in the previous version did not affect the loss value.
+
 ### Version 1.1.5 2023-07-26
 #### Fixed Bugs
 - Fixed a bug in the similarity loss of Splane, where it minimized the cosine similarity of the latent vectors of spots with their neighbors.
 #### Features
 - Optimized the time and memory consumption of the Splane training process for large datasets.
 
 ### Version 1.1.2 2023-07-12
 #### Fixed Bugs
 - Removed `rpy2` from the pypi dependency of SPACEL. It now needs to be pre-installed when creating the environment through conda.
 - Fixed a bug in Scube where the `best_model_state` was not referenced before being used.
 #### Features
 - Added function documentations for Scube related to the GPR model.
-
-### Version 1.1.1 2023-07-11
-#### Features
-* All code based on `Tensorflow` have been mirated to `PyTorch`, it does not have `Tensorflow` as dependency anymore.
-* The `Splane.utils.add_cell_type_composition` function has been implemented to facilitate the cell type composition predicted by deconvolution methods into Splane.
-* Spoint and Splane now support tqdm type output for improved progress tracking.
     
 ## Requirements
 **Note**: The current version of SPACEL only supports Linux and MacOS, not Windows platform. 
 
 To install `SPACEL`, you need to install [PyTorch](https://pytorch.org) with GPU support first. If you don't need GPU acceleration, you can just skip the installation for `cudnn` and `cudatoolkit`.
 * Create conda environment for `SPACEL`:
 ```
```

### Comparing `SPACEL-1.1.5/SPACEL.egg-info/SOURCES.txt` & `SPACEL-1.1.6/SPACEL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.5/setup.py` & `SPACEL-1.1.6/setup.py`

 * *Files identical despite different names*

