# Comparing `tmp/py_tgb-0.7.0.tar.gz` & `tmp/py_tgb-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_tgb-0.7.0.tar", max compression
+gzip compressed data, was "py_tgb-0.7.5.tar", max compression
```

## Comparing `py_tgb-0.7.0.tar` & `py_tgb-0.7.5.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     4351 2023-07-21 15:22:18.659359 py_tgb-0.7.0/README.md
--rw-r--r--   0        0        0      748 2023-07-21 15:22:18.663359 py_tgb-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      177 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/MAG/mag.py
--rw-r--r--   0        0        0      820 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/MAG/old/plot_stats.py
--rw-r--r--   0        0        0     4740 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-coin.py
--rw-r--r--   0        0        0     2497 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-coin_neg_generator.py
--rw-r--r--   0        0        0     6912 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-comment.py
--rw-r--r--   0        0        0     2499 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-comment_neg_generator.py
--rw-r--r--   0        0        0     7781 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-flight.py
--rw-r--r--   0        0        0     2499 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-flight_neg_generator.py
--rw-r--r--   0        0        0     4777 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-review.py
--rw-r--r--   0        0        0     2503 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-review_neg_generator.py
--rw-r--r--   0        0        0     2543 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-wiki_neg_generator.py
--rw-r--r--   0        0        0    19780 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbn-genre.py
--rw-r--r--   0        0        0    11859 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbn-reddit.py
--rw-r--r--   0        0        0     5927 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbn-trade.py
--rw-r--r--   0        0        0      539 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/datasets/tgbn-arxiv/process_arxiv.py
--rw-r--r--   0        0        0    13895 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/linkproppred/dataset.py
--rw-r--r--   0        0        0     7532 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/linkproppred/dataset_pyg.py
--rw-r--r--   0        0        0     5869 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/linkproppred/evaluate.py
--rw-r--r--   0        0        0    14146 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/linkproppred/negative_generator.py
--rw-r--r--   0        0        0     5123 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/linkproppred/negative_sampler.py
--rw-r--r--   0        0        0    16293 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/nodeproppred/dataset.py
--rw-r--r--   0        0        0     7205 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/nodeproppred/dataset_pyg.py
--rw-r--r--   0        0        0     5336 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/nodeproppred/evaluate.py
--rw-r--r--   0        0        0     8691 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/utils/dataset_stats.py
--rw-r--r--   0        0        0     1827 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/utils/info.py
--rw-r--r--   0        0        0    27787 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/utils/pre_process.py
--rw-r--r--   0        0        0     2747 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/utils/stats.py
--rw-r--r--   0        0        0     2974 2023-07-21 15:22:18.663359 py_tgb-0.7.0/tgb/utils/utils.py
--rw-r--r--   0        0        0     5035 1970-01-01 00:00:00.000000 py_tgb-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     4653 2023-07-27 18:19:30.184342 py_tgb-0.7.5/README.md
+-rw-r--r--   0        0        0      748 2023-07-27 18:19:30.184342 py_tgb-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/MAG/mag.py
+-rw-r--r--   0        0        0      820 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/MAG/old/plot_stats.py
+-rw-r--r--   0        0        0     4740 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-coin.py
+-rw-r--r--   0        0        0     2497 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-coin_neg_generator.py
+-rw-r--r--   0        0        0     6912 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-comment.py
+-rw-r--r--   0        0        0     2499 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-comment_neg_generator.py
+-rw-r--r--   0        0        0     7781 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-flight.py
+-rw-r--r--   0        0        0     2499 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-flight_neg_generator.py
+-rw-r--r--   0        0        0     4777 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-review.py
+-rw-r--r--   0        0        0     2503 2023-07-27 18:19:30.184342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-review_neg_generator.py
+-rw-r--r--   0        0        0     2543 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-wiki_neg_generator.py
+-rw-r--r--   0        0        0    19780 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbn-genre.py
+-rw-r--r--   0        0        0    11859 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbn-reddit.py
+-rw-r--r--   0        0        0     5927 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbn-trade.py
+-rw-r--r--   0        0        0      539 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/datasets/tgbn-arxiv/process_arxiv.py
+-rw-r--r--   0        0        0     5290 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/datasets/token_network/token.py
+-rw-r--r--   0        0        0    15644 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/linkproppred/dataset.py
+-rw-r--r--   0        0        0     7532 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/linkproppred/dataset_pyg.py
+-rw-r--r--   0        0        0     5869 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/linkproppred/evaluate.py
+-rw-r--r--   0        0        0    14146 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/linkproppred/negative_generator.py
+-rw-r--r--   0        0        0     5123 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/linkproppred/negative_sampler.py
+-rw-r--r--   0        0        0    17517 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/nodeproppred/dataset.py
+-rw-r--r--   0        0        0     7205 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/nodeproppred/dataset_pyg.py
+-rw-r--r--   0        0        0     5336 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/nodeproppred/evaluate.py
+-rw-r--r--   0        0        0     8691 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/utils/dataset_stats.py
+-rw-r--r--   0        0        0     2185 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/utils/info.py
+-rw-r--r--   0        0        0    27787 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/utils/pre_process.py
+-rw-r--r--   0        0        0     2747 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/utils/stats.py
+-rw-r--r--   0        0        0     2974 2023-07-27 18:19:30.188342 py_tgb-0.7.5/tgb/utils/utils.py
+-rw-r--r--   0        0        0     5337 1970-01-01 00:00:00.000000 py_tgb-0.7.5/PKG-INFO
```

### Comparing `py_tgb-0.7.0/README.md` & `py_tgb-0.7.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,33 @@
-# TGB
+<!-- # TGB -->
+![TGB logo](imgs/logo.png)
+
 <h4>
 	<a href="https://arxiv.org/abs/2307.01026"><img src="https://img.shields.io/badge/arXiv-pdf-yellowgreen"></a>
 	<a href="https://pypi.org/project/py-tgb/"><img src="https://img.shields.io/pypi/v/py-tgb.svg?color=brightgreen"></a>
 	<a href="https://tgb.complexdatalab.com/"><img src="https://img.shields.io/badge/website-blue"></a>
 	<a href="https://docs.tgb.complexdatalab.com/"><img src="https://img.shields.io/badge/docs-orange"></a>
 </h4>
 Temporal Graph Benchmark for Machine Learning on Temporal Graphs 
 
-![TGB dataloading and evaluation pipeline](imgs/pipeline.png)
 
 Overview of the Temporal Graph Benchmark (TGB) pipeline:
 - TGB includes large-scale and realistic datasets from five different domains with both dynamic link prediction and node property prediction tasks
 - TGB automatically downloads datasets and processes them into `numpy`, `PyTorch` and `PyG compatible TemporalData` formats. 
 - Novel TG models can be easily evaluated on TGB datasets via reproducible and realistic evaluation protocols. 
 - TGB provides public and online leaderboards to track recent developments in temporal graph learning domain
 
+![TGB dataloading and evaluation pipeline](imgs/pipeline.png)
+
+### Annoucements
+
+**Please update to version `0.7.5`**
+
+the negative samples for the `tgbl-wiki` and `tgbl-review` dataset has been updated and redownload of the dataset would be needed (will be prompted automatically in this version when you use the dataloader)
+
 
 ### Pip Install
 
 You can install TGB via [pip](https://pypi.org/project/py-tgb/)
 ```
 pip install py-tgb
 ```
```

#### html2text {}

```diff
@@ -1,56 +1,59 @@
-# TGB
+ ![TGB logo](imgs/logo.png)
 *** [https://img.shields.io/badge/arXiv-pdf-yellowgreen] [https://
 img.shields.io/pypi/v/py-tgb.svg?color=brightgreen] [https://img.shields.io/
 badge/website-blue] [https://img.shields.io/badge/docs-orange] ***
-Temporal Graph Benchmark for Machine Learning on Temporal Graphs ![TGB
-dataloading and evaluation pipeline](imgs/pipeline.png) Overview of the
-Temporal Graph Benchmark (TGB) pipeline: - TGB includes large-scale and
+Temporal Graph Benchmark for Machine Learning on Temporal Graphs Overview of
+the Temporal Graph Benchmark (TGB) pipeline: - TGB includes large-scale and
 realistic datasets from five different domains with both dynamic link
 prediction and node property prediction tasks - TGB automatically downloads
 datasets and processes them into `numpy`, `PyTorch` and `PyG compatible
 TemporalData` formats. - Novel TG models can be easily evaluated on TGB
 datasets via reproducible and realistic evaluation protocols. - TGB provides
 public and online leaderboards to track recent developments in temporal graph
-learning domain ### Pip Install You can install TGB via [pip](https://pypi.org/
-project/py-tgb/) ``` pip install py-tgb ``` ### Links and Datasets The project
-website can be found [here](https://tgb.complexdatalab.com/). The API
-documentations can be found [here](https://shenyanghuang.github.io/TGB/). all
-dataset download links can be found at [info.py](https://github.com/
-shenyangHuang/TGB/blob/main/tgb/utils/info.py) TGB dataloader will also
-automatically download the dataset as well as the negative samples for the link
-property prediction datasets. ### Running Example Methods - For the dynamic
-link property prediction task, see the [`examples/linkproppred`](https://
-github.com/shenyangHuang/TGB/tree/main/examples/linkproppred) folder for
-example scripts to run TGN, DyRep and EdgeBank on TGB datasets. - For the
-dynamic node property prediction task, see the [`examples/nodeproppred`](https:
-//github.com/shenyangHuang/TGB/tree/main/examples/nodeproppred) folder for
-example scripts to run TGN, DyRep and EdgeBank on TGB datasets. - For all other
-baselines, please see the [TGB_Baselines](https://github.com/fpour/
-TGB_Baselines) repo. ### Install dependency Our implementation works with
-python >= 3.9 and can be installed as follows 1. set up virtual environment
-(conda should work as well) ``` python -m venv ~/tgb_env/ source ~/tgb_env/bin/
-activate ``` 2. install external packages ``` pip install pandas==1.5.3 pip
-install matplotlib==3.7.1 pip install clint==0.5.1 ``` install Pytorch and PyG
-dependencies (needed to run the examples) ``` pip install torch==2.0.0 --index-
-url https://download.pytorch.org/whl/cu117 pip install torch_geometric==2.3.0
-pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv
--f https://data.pyg.org/whl/torch-2.0.0+cu117.html ``` 3. install local
-dependencies under root directory `/TGB` ``` pip install -e . ``` ###
-Instruction for tracking new documentation and running mkdocs locally 1. first
-run the mkdocs server locally in your terminal ``` mkdocs serve ``` 2. go to
-the local hosted web address similar to ``` [14:18:13] Browser connected: http:
-//127.0.0.1:8000/ ``` Example: to track documentation of a new hi.py file in
-tgb/edgeregression/hi.py 3. create docs/api/tgb.hi.md and add the following ```
-# `tgb.edgeregression` ::: tgb.edgeregression.hi ``` 4. edit mkdocs.yml ```
-nav: - Overview: index.md - About: about.md - API: other *.md files -
-tgb.edgeregression: api/tgb.hi.md ``` ### Creating new branch ### ``` git fetch
-origin git checkout -b test origin/test ``` ### dependencies for mkdocs
-(documentation) ``` pip install mkdocs pip install mkdocs-material pip install
-mkdocstrings-python pip install mkdocs-jupyter pip install notebook ``` ###
-full dependency list Our implementation works with python >= 3.9 and has the
-following dependencies ``` pytorch == 2.0.0 torch-geometric == 2.3.0 torch-
-scatter==2.1.1 torch-sparse==0.6.17 torch-spline-conv==1.2.2 pandas==1.5.3
-clint==0.5.1 ``` ### Acknowledgments We thank the [OGB](https://
-ogb.stanford.edu/) team for their support throughout this project and sharing
-their website code for the construction of [TGB website](https://
-tgb.complexdatalab.com/).
+learning domain ![TGB dataloading and evaluation pipeline](imgs/pipeline.png)
+### Annoucements **Please update to version `0.7.5`** the negative samples for
+the `tgbl-wiki` and `tgbl-review` dataset has been updated and redownload of
+the dataset would be needed (will be prompted automatically in this version
+when you use the dataloader) ### Pip Install You can install TGB via [pip]
+(https://pypi.org/project/py-tgb/) ``` pip install py-tgb ``` ### Links and
+Datasets The project website can be found [here](https://
+tgb.complexdatalab.com/). The API documentations can be found [here](https://
+shenyanghuang.github.io/TGB/). all dataset download links can be found at
+[info.py](https://github.com/shenyangHuang/TGB/blob/main/tgb/utils/info.py) TGB
+dataloader will also automatically download the dataset as well as the negative
+samples for the link property prediction datasets. ### Running Example Methods
+- For the dynamic link property prediction task, see the [`examples/
+linkproppred`](https://github.com/shenyangHuang/TGB/tree/main/examples/
+linkproppred) folder for example scripts to run TGN, DyRep and EdgeBank on TGB
+datasets. - For the dynamic node property prediction task, see the [`examples/
+nodeproppred`](https://github.com/shenyangHuang/TGB/tree/main/examples/
+nodeproppred) folder for example scripts to run TGN, DyRep and EdgeBank on TGB
+datasets. - For all other baselines, please see the [TGB_Baselines](https://
+github.com/fpour/TGB_Baselines) repo. ### Install dependency Our implementation
+works with python >= 3.9 and can be installed as follows 1. set up virtual
+environment (conda should work as well) ``` python -m venv ~/tgb_env/ source ~/
+tgb_env/bin/activate ``` 2. install external packages ``` pip install
+pandas==1.5.3 pip install matplotlib==3.7.1 pip install clint==0.5.1 ```
+install Pytorch and PyG dependencies (needed to run the examples) ``` pip
+install torch==2.0.0 --index-url https://download.pytorch.org/whl/cu117 pip
+install torch_geometric==2.3.0 pip install pyg_lib torch_scatter torch_sparse
+torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-
+2.0.0+cu117.html ``` 3. install local dependencies under root directory `/TGB`
+``` pip install -e . ``` ### Instruction for tracking new documentation and
+running mkdocs locally 1. first run the mkdocs server locally in your terminal
+``` mkdocs serve ``` 2. go to the local hosted web address similar to ``` [14:
+18:13] Browser connected: http://127.0.0.1:8000/ ``` Example: to track
+documentation of a new hi.py file in tgb/edgeregression/hi.py 3. create docs/
+api/tgb.hi.md and add the following ``` # `tgb.edgeregression` :::
+tgb.edgeregression.hi ``` 4. edit mkdocs.yml ``` nav: - Overview: index.md -
+About: about.md - API: other *.md files - tgb.edgeregression: api/tgb.hi.md ```
+### Creating new branch ### ``` git fetch origin git checkout -b test origin/
+test ``` ### dependencies for mkdocs (documentation) ``` pip install mkdocs pip
+install mkdocs-material pip install mkdocstrings-python pip install mkdocs-
+jupyter pip install notebook ``` ### full dependency list Our implementation
+works with python >= 3.9 and has the following dependencies ``` pytorch ==
+2.0.0 torch-geometric == 2.3.0 torch-scatter==2.1.1 torch-sparse==0.6.17 torch-
+spline-conv==1.2.2 pandas==1.5.3 clint==0.5.1 ``` ### Acknowledgments We thank
+the [OGB](https://ogb.stanford.edu/) team for their support throughout this
+project and sharing their website code for the construction of [TGB website]
+(https://tgb.complexdatalab.com/).
```

### Comparing `py_tgb-0.7.0/pyproject.toml` & `py_tgb-0.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-tgb"
-version = "0.7.0"
+version = "0.7.5"
 description = "Temporal Graph Benchmark project repo"
 authors = ["shenyang Huang <shenyang.huang@mail.mcgill.ca>", "Farimah Poursafaei", "Emanuele Rossi <emanuele.rossi1909@gmail.com>", "Jacob Danovitch <jacob.danovitch@mila.quebec>"]
 readme = "README.md"
 packages = [{include = "tgb"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `py_tgb-0.7.0/tgb/datasets/dataset_scripts/MAG/old/plot_stats.py` & `py_tgb-0.7.5/tgb/datasets/dataset_scripts/MAG/old/plot_stats.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-coin.py` & `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-coin.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-coin_neg_generator.py` & `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-coin_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-comment.py` & `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-comment.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-comment_neg_generator.py` & `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-comment_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-flight.py` & `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-flight.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-flight_neg_generator.py` & `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-flight_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-review.py` & `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-review.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-review_neg_generator.py` & `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-review_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbl-wiki_neg_generator.py` & `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbl-wiki_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbn-genre.py` & `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbn-genre.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbn-reddit.py` & `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbn-reddit.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/datasets/dataset_scripts/tgbn-trade.py` & `py_tgb-0.7.5/tgb/datasets/dataset_scripts/tgbn-trade.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/datasets/tgbn-arxiv/process_arxiv.py` & `py_tgb-0.7.5/tgb/datasets/tgbn-arxiv/process_arxiv.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/linkproppred/dataset.py` & `py_tgb-0.7.5/tgb/linkproppred/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 import numpy as np
 import pandas as pd
 import zipfile
 import requests
 from clint.textui import progress
 
 from tgb.linkproppred.negative_sampler import NegativeEdgeSampler
-from tgb.utils.info import PROJ_DIR, DATA_URL_DICT, DATA_EVAL_METRIC_DICT, BColors
+from tgb.utils.info import (
+    PROJ_DIR, 
+    DATA_URL_DICT, 
+    DATA_VERSION_DICT, 
+    DATA_EVAL_METRIC_DICT, 
+    BColors
+)
 from tgb.utils.pre_process import (
     csv_to_pd_data,
     process_node_feat,
     csv_to_pd_data_sc,
     csv_to_pd_data_rc,
     load_edgelist_wiki,
 )
@@ -63,17 +69,23 @@
             self.dir_name = meta_dict["dir_name"]
         self.root = osp.join(root, self.dir_name)
         self.meta_dict = meta_dict
         if "fname" not in self.meta_dict:
             self.meta_dict["fname"] = self.root + "/" + self.name + "_edgelist.csv"
             self.meta_dict["nodefile"] = None
 
-        # TODO update the logic here to load the filenames from info.py
         if name == "tgbl-flight":
             self.meta_dict["nodefile"] = self.root + "/" + "airport_node_feat.csv"
+        
+        self.meta_dict["val_ns"] = self.root + "/" + self.name + "_val_ns.pkl"
+        self.meta_dict["test_ns"] = self.root + "/" + self.name + "_test_ns.pkl"
+
+        #! version check
+        self.version_passed = True
+        self._version_check()
 
         # initialize
         self._node_feat = None
         self._edge_feat = None
         self._full_data = None
         self._train_data = None
         self._val_data = None
@@ -90,14 +102,42 @@
         if preprocess:
             self.pre_process()
 
         self.ns_sampler = NegativeEdgeSampler(
             dataset_name=self.name, strategy="hist_rnd"
         )
 
+    def _version_check(self) -> None:
+        r"""Implement Version checks for dataset files
+        updates the file names based on the current version number
+        prompt the user to download the new version via self.version_passed variable
+        """
+        if (self.name in DATA_VERSION_DICT):
+            version = DATA_VERSION_DICT[self.name]
+        else:
+            print(f"Dataset {self.name} version number not found.")
+            self.version_passed = False
+            return None
+        
+        if (version > 1):
+            #* check if current version is outdated
+            self.meta_dict["fname"] = self.root + "/" + self.name + "_edgelist_v" + str(int(version)) + ".csv"
+            self.meta_dict["nodefile"] = None
+            if self.name == "tgbl-flight":
+                self.meta_dict["nodefile"] = self.root + "/" + "airport_node_feat_v" + str(int(version)) + ".csv"
+            self.meta_dict["val_ns"] = self.root + "/" + self.name + "_val_ns_v" + str(int(version)) + ".pkl"
+            self.meta_dict["test_ns"] = self.root + "/" + self.name + "_test_ns_v" + str(int(version)) + ".pkl"
+            
+            if (not osp.exists(self.meta_dict["fname"])):
+                print(f"Dataset {self.name} version {int(version)} not found.")
+                print(f"Please download the latest version of the dataset.")
+                self.version_passed = False
+                return None
+        
+
     def download(self):
         """
         downloads this dataset from url
         check if files are already downloaded
         """
         # check if the file already exists
         if osp.exists(self.meta_dict["fname"]):
@@ -134,14 +174,15 @@
                         if chunk:
                             f.write(chunk)
                             f.flush()
                 # for unzipping the file
                 with zipfile.ZipFile(path_download, "r") as zip_ref:
                     zip_ref.extractall(self.root)
                 print(f"{BColors.OKGREEN}Download completed {BColors.ENDC}")
+                self.version_passed = True
         else:
             raise Exception(
                 BColors.FAIL + "Data not found error, download " + self.name + " failed"
             )
 
     def generate_processed_files(self) -> pd.DataFrame:
         r"""
@@ -159,15 +200,15 @@
                     f"File not found at {self.meta_dict['nodefile']}"
                 )
         OUT_DF = self.root + "/" + "ml_{}.pkl".format(self.name)
         OUT_EDGE_FEAT = self.root + "/" + "ml_{}.pkl".format(self.name + "_edge")
         if self.meta_dict["nodefile"] is not None:
             OUT_NODE_FEAT = self.root + "/" + "ml_{}.pkl".format(self.name + "_node")
 
-        if osp.exists(OUT_DF):
+        if (osp.exists(OUT_DF)) and (self.version_passed is True):
             print("loading processed file")
             df = pd.read_pickle(OUT_DF)
             edge_feat = load_pkl(OUT_EDGE_FEAT)
             if self.meta_dict["nodefile"] is not None:
                 node_feat = load_pkl(OUT_NODE_FEAT)
 
         else:
@@ -277,23 +318,23 @@
         return self.ns_sampler
 
     def load_val_ns(self) -> None:
         r"""
         load the negative samples for the validation set
         """
         self.ns_sampler.load_eval_set(
-            fname=self.root + "/" + self.name + "_val_ns.pkl", split_mode="val"
+            fname=self.meta_dict["val_ns"], split_mode="val"
         )
 
     def load_test_ns(self) -> None:
         r"""
         load the negative samples for the test set
         """
         self.ns_sampler.load_eval_set(
-            fname=self.root + "/" + self.name + "_test_ns.pkl", split_mode="test"
+            fname=self.meta_dict["test_ns"], split_mode="test"
         )
 
     @property
     def node_feat(self) -> Optional[np.ndarray]:
         r"""
         Returns the node features of the dataset with dim [N, feat_dim]
         Returns:
```

### Comparing `py_tgb-0.7.0/tgb/linkproppred/dataset_pyg.py` & `py_tgb-0.7.5/tgb/linkproppred/dataset_pyg.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/linkproppred/evaluate.py` & `py_tgb-0.7.5/tgb/linkproppred/evaluate.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/linkproppred/negative_generator.py` & `py_tgb-0.7.5/tgb/linkproppred/negative_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/linkproppred/negative_sampler.py` & `py_tgb-0.7.5/tgb/linkproppred/negative_sampler.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/nodeproppred/dataset.py` & `py_tgb-0.7.5/tgb/nodeproppred/dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import requests
 from clint.textui import progress
 
 from tgb.utils.info import (
     PROJ_DIR,
     DATA_URL_DICT,
     DATA_NUM_CLASSES,
+    DATA_VERSION_DICT,
     DATA_EVAL_METRIC_DICT,
     BColors,
 )
 from tgb.utils.utils import save_pkl, load_pkl
 from tgb.utils.pre_process import (
     load_label_dict,
     load_edgelist_sr,
@@ -71,17 +72,19 @@
             meta_dict = {"dir_name": self.dir_name}
         else:
             self.dir_name = meta_dict["dir_name"]
         self.root = osp.join(root, self.dir_name)
         self.meta_dict = meta_dict
         if "fname" not in self.meta_dict:
             self.meta_dict["fname"] = self.root + "/" + self.name + "_edgelist.csv"
-            self.meta_dict["nodefile"] = (
-                self.root + "/" + self.name + "_node_labels.csv"
-            )
+            self.meta_dict["nodefile"] = self.root + "/" + self.name + "_node_labels.csv"
+
+         #! version check
+        self.version_passed = True
+        self._version_check()
 
         self._num_classes = DATA_NUM_CLASSES[self.name]
 
         # initialize
         self._node_feat = None
         self._edge_feat = None
         self._full_data = None
@@ -93,14 +96,37 @@
             raise FileNotFoundError(f"Directory not found at {self.root}")
 
         if preprocess:
             self.pre_process()
 
         self.label_ts_idx = 0  # index for which node lables to return now
 
+    def _version_check(self) -> None:
+        r"""Implement Version checks for dataset files
+        updates the file names based on the current version number
+        prompt the user to download the new version via self.version_passed variable
+        """
+        if (self.name in DATA_VERSION_DICT):
+            version = DATA_VERSION_DICT[self.name]
+        else:
+            print(f"Dataset {self.name} version number not found.")
+            self.version_passed = False
+            return None
+        
+        if (version > 1):
+            #* check if current version is outdated
+            self.meta_dict["fname"] = self.root + "/" + self.name + "_edgelist_v" + str(int(version)) + ".csv"
+            self.meta_dict["nodefile"] = self.root + "/" + self.name + "_node_labels_v" + str(int(version)) + ".csv"
+            
+            if (not osp.exists(self.meta_dict["fname"])):
+                print(f"Dataset {self.name} version {int(version)} not found.")
+                print(f"Please download the latest version of the dataset.")
+                self.version_passed = False
+                return None
+
     def download(self) -> None:
         r"""
         downloads this dataset from url
         check if files are already downloaded
         Returns:
             None
         """
```

### Comparing `py_tgb-0.7.0/tgb/nodeproppred/dataset_pyg.py` & `py_tgb-0.7.5/tgb/nodeproppred/dataset_pyg.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/nodeproppred/evaluate.py` & `py_tgb-0.7.5/tgb/nodeproppred/evaluate.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/utils/dataset_stats.py` & `py_tgb-0.7.5/tgb/utils/dataset_stats.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/utils/info.py` & `py_tgb-0.7.5/tgb/utils/info.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,24 +19,35 @@
     WARNING = "\033[93m"
     FAIL = "\033[91m"
     ENDC = "\033[0m"
     BOLD = "\033[1m"
     UNDERLINE = "\033[4m"
 
 DATA_URL_DICT = {
-    "tgbl-wiki": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-wiki.zip",
-    "tgbl-review": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-review.zip",
+    "tgbl-wiki":"https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-wiki-v2.zip", #"https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-wiki.zip", #v1
+    "tgbl-review": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-review-v2.zip", #"https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-review.zip", #v1
     "tgbl-coin": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-coin.zip",
     "tgbl-flight": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-flight.zip",
     "tgbl-comment": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbl-comment.zip",
     "tgbn-trade": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbn-trade.zip",
     "tgbn-genre": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbn-genre.zip",
     "tgbn-reddit": "https://object-arbutus.cloud.computecanada.ca/tgb/tgbn-reddit.zip",
 }
 
+DATA_VERSION_DICT = {
+    "tgbl-wiki": 2,
+    "tgbl-review": 2,
+    "tgbl-coin": 1,
+    "tgbl-comment": 1,
+    "tgbl-flight": 1,
+    "tgbn-trade": 1,
+    "tgbn-genre": 1,
+    "tgbn-reddit": 1,
+}
+
 #"https://object-arbutus.cloud.computecanada.ca/tgb/wiki_neg.zip" #for all negative samples of the wiki dataset
 #"https://object-arbutus.cloud.computecanada.ca/tgb/review_ns100.zip" #for 100 ns samples in review
 
 DATA_EVAL_METRIC_DICT = {
     "tgbl-wiki": "mrr",
     "tgbl-review": "mrr",
     "tgbl-coin": "mrr",
```

### Comparing `py_tgb-0.7.0/tgb/utils/pre_process.py` & `py_tgb-0.7.5/tgb/utils/pre_process.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/utils/stats.py` & `py_tgb-0.7.5/tgb/utils/stats.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/tgb/utils/utils.py` & `py_tgb-0.7.5/tgb/utils/utils.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.7.0/PKG-INFO` & `py_tgb-0.7.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-tgb
-Version: 0.7.0
+Version: 0.7.5
 Summary: Temporal Graph Benchmark project repo
 Author: shenyang Huang
 Author-email: shenyang.huang@mail.mcgill.ca
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,31 +13,40 @@
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: torch-geometric (>=2.3.0,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
-# TGB
+<!-- # TGB -->
+![TGB logo](imgs/logo.png)
+
 <h4>
 	<a href="https://arxiv.org/abs/2307.01026"><img src="https://img.shields.io/badge/arXiv-pdf-yellowgreen"></a>
 	<a href="https://pypi.org/project/py-tgb/"><img src="https://img.shields.io/pypi/v/py-tgb.svg?color=brightgreen"></a>
 	<a href="https://tgb.complexdatalab.com/"><img src="https://img.shields.io/badge/website-blue"></a>
 	<a href="https://docs.tgb.complexdatalab.com/"><img src="https://img.shields.io/badge/docs-orange"></a>
 </h4>
 Temporal Graph Benchmark for Machine Learning on Temporal Graphs 
 
-![TGB dataloading and evaluation pipeline](imgs/pipeline.png)
 
 Overview of the Temporal Graph Benchmark (TGB) pipeline:
 - TGB includes large-scale and realistic datasets from five different domains with both dynamic link prediction and node property prediction tasks
 - TGB automatically downloads datasets and processes them into `numpy`, `PyTorch` and `PyG compatible TemporalData` formats. 
 - Novel TG models can be easily evaluated on TGB datasets via reproducible and realistic evaluation protocols. 
 - TGB provides public and online leaderboards to track recent developments in temporal graph learning domain
 
+![TGB dataloading and evaluation pipeline](imgs/pipeline.png)
+
+### Annoucements
+
+**Please update to version `0.7.5`**
+
+the negative samples for the `tgbl-wiki` and `tgbl-review` dataset has been updated and redownload of the dataset would be needed (will be prompted automatically in this version when you use the dataloader)
+
 
 ### Pip Install
 
 You can install TGB via [pip](https://pypi.org/project/py-tgb/)
 ```
 pip install py-tgb
 ```
```

#### html2text {}

```diff
@@ -1,65 +1,68 @@
-Metadata-Version: 2.1 Name: py-tgb Version: 0.7.0 Summary: Temporal Graph
+Metadata-Version: 2.1 Name: py-tgb Version: 0.7.5 Summary: Temporal Graph
 Benchmark project repo Author: shenyang Huang Author-email:
 shenyang.huang@mail.mcgill.ca Requires-Python: >=3.9,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: clint (>=0.5.1,<0.6.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist: requests
 (>=2.28.2,<3.0.0) Requires-Dist: scikit-learn (>=1.2.2,<2.0.0) Requires-Dist:
 torch-geometric (>=2.3.0,<3.0.0) Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Description-Content-Type: text/markdown # TGB
+Description-Content-Type: text/markdown  ![TGB logo](imgs/logo.png)
 *** [https://img.shields.io/badge/arXiv-pdf-yellowgreen] [https://
 img.shields.io/pypi/v/py-tgb.svg?color=brightgreen] [https://img.shields.io/
 badge/website-blue] [https://img.shields.io/badge/docs-orange] ***
-Temporal Graph Benchmark for Machine Learning on Temporal Graphs ![TGB
-dataloading and evaluation pipeline](imgs/pipeline.png) Overview of the
-Temporal Graph Benchmark (TGB) pipeline: - TGB includes large-scale and
+Temporal Graph Benchmark for Machine Learning on Temporal Graphs Overview of
+the Temporal Graph Benchmark (TGB) pipeline: - TGB includes large-scale and
 realistic datasets from five different domains with both dynamic link
 prediction and node property prediction tasks - TGB automatically downloads
 datasets and processes them into `numpy`, `PyTorch` and `PyG compatible
 TemporalData` formats. - Novel TG models can be easily evaluated on TGB
 datasets via reproducible and realistic evaluation protocols. - TGB provides
 public and online leaderboards to track recent developments in temporal graph
-learning domain ### Pip Install You can install TGB via [pip](https://pypi.org/
-project/py-tgb/) ``` pip install py-tgb ``` ### Links and Datasets The project
-website can be found [here](https://tgb.complexdatalab.com/). The API
-documentations can be found [here](https://shenyanghuang.github.io/TGB/). all
-dataset download links can be found at [info.py](https://github.com/
-shenyangHuang/TGB/blob/main/tgb/utils/info.py) TGB dataloader will also
-automatically download the dataset as well as the negative samples for the link
-property prediction datasets. ### Running Example Methods - For the dynamic
-link property prediction task, see the [`examples/linkproppred`](https://
-github.com/shenyangHuang/TGB/tree/main/examples/linkproppred) folder for
-example scripts to run TGN, DyRep and EdgeBank on TGB datasets. - For the
-dynamic node property prediction task, see the [`examples/nodeproppred`](https:
-//github.com/shenyangHuang/TGB/tree/main/examples/nodeproppred) folder for
-example scripts to run TGN, DyRep and EdgeBank on TGB datasets. - For all other
-baselines, please see the [TGB_Baselines](https://github.com/fpour/
-TGB_Baselines) repo. ### Install dependency Our implementation works with
-python >= 3.9 and can be installed as follows 1. set up virtual environment
-(conda should work as well) ``` python -m venv ~/tgb_env/ source ~/tgb_env/bin/
-activate ``` 2. install external packages ``` pip install pandas==1.5.3 pip
-install matplotlib==3.7.1 pip install clint==0.5.1 ``` install Pytorch and PyG
-dependencies (needed to run the examples) ``` pip install torch==2.0.0 --index-
-url https://download.pytorch.org/whl/cu117 pip install torch_geometric==2.3.0
-pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv
--f https://data.pyg.org/whl/torch-2.0.0+cu117.html ``` 3. install local
-dependencies under root directory `/TGB` ``` pip install -e . ``` ###
-Instruction for tracking new documentation and running mkdocs locally 1. first
-run the mkdocs server locally in your terminal ``` mkdocs serve ``` 2. go to
-the local hosted web address similar to ``` [14:18:13] Browser connected: http:
-//127.0.0.1:8000/ ``` Example: to track documentation of a new hi.py file in
-tgb/edgeregression/hi.py 3. create docs/api/tgb.hi.md and add the following ```
-# `tgb.edgeregression` ::: tgb.edgeregression.hi ``` 4. edit mkdocs.yml ```
-nav: - Overview: index.md - About: about.md - API: other *.md files -
-tgb.edgeregression: api/tgb.hi.md ``` ### Creating new branch ### ``` git fetch
-origin git checkout -b test origin/test ``` ### dependencies for mkdocs
-(documentation) ``` pip install mkdocs pip install mkdocs-material pip install
-mkdocstrings-python pip install mkdocs-jupyter pip install notebook ``` ###
-full dependency list Our implementation works with python >= 3.9 and has the
-following dependencies ``` pytorch == 2.0.0 torch-geometric == 2.3.0 torch-
-scatter==2.1.1 torch-sparse==0.6.17 torch-spline-conv==1.2.2 pandas==1.5.3
-clint==0.5.1 ``` ### Acknowledgments We thank the [OGB](https://
-ogb.stanford.edu/) team for their support throughout this project and sharing
-their website code for the construction of [TGB website](https://
-tgb.complexdatalab.com/).
+learning domain ![TGB dataloading and evaluation pipeline](imgs/pipeline.png)
+### Annoucements **Please update to version `0.7.5`** the negative samples for
+the `tgbl-wiki` and `tgbl-review` dataset has been updated and redownload of
+the dataset would be needed (will be prompted automatically in this version
+when you use the dataloader) ### Pip Install You can install TGB via [pip]
+(https://pypi.org/project/py-tgb/) ``` pip install py-tgb ``` ### Links and
+Datasets The project website can be found [here](https://
+tgb.complexdatalab.com/). The API documentations can be found [here](https://
+shenyanghuang.github.io/TGB/). all dataset download links can be found at
+[info.py](https://github.com/shenyangHuang/TGB/blob/main/tgb/utils/info.py) TGB
+dataloader will also automatically download the dataset as well as the negative
+samples for the link property prediction datasets. ### Running Example Methods
+- For the dynamic link property prediction task, see the [`examples/
+linkproppred`](https://github.com/shenyangHuang/TGB/tree/main/examples/
+linkproppred) folder for example scripts to run TGN, DyRep and EdgeBank on TGB
+datasets. - For the dynamic node property prediction task, see the [`examples/
+nodeproppred`](https://github.com/shenyangHuang/TGB/tree/main/examples/
+nodeproppred) folder for example scripts to run TGN, DyRep and EdgeBank on TGB
+datasets. - For all other baselines, please see the [TGB_Baselines](https://
+github.com/fpour/TGB_Baselines) repo. ### Install dependency Our implementation
+works with python >= 3.9 and can be installed as follows 1. set up virtual
+environment (conda should work as well) ``` python -m venv ~/tgb_env/ source ~/
+tgb_env/bin/activate ``` 2. install external packages ``` pip install
+pandas==1.5.3 pip install matplotlib==3.7.1 pip install clint==0.5.1 ```
+install Pytorch and PyG dependencies (needed to run the examples) ``` pip
+install torch==2.0.0 --index-url https://download.pytorch.org/whl/cu117 pip
+install torch_geometric==2.3.0 pip install pyg_lib torch_scatter torch_sparse
+torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-
+2.0.0+cu117.html ``` 3. install local dependencies under root directory `/TGB`
+``` pip install -e . ``` ### Instruction for tracking new documentation and
+running mkdocs locally 1. first run the mkdocs server locally in your terminal
+``` mkdocs serve ``` 2. go to the local hosted web address similar to ``` [14:
+18:13] Browser connected: http://127.0.0.1:8000/ ``` Example: to track
+documentation of a new hi.py file in tgb/edgeregression/hi.py 3. create docs/
+api/tgb.hi.md and add the following ``` # `tgb.edgeregression` :::
+tgb.edgeregression.hi ``` 4. edit mkdocs.yml ``` nav: - Overview: index.md -
+About: about.md - API: other *.md files - tgb.edgeregression: api/tgb.hi.md ```
+### Creating new branch ### ``` git fetch origin git checkout -b test origin/
+test ``` ### dependencies for mkdocs (documentation) ``` pip install mkdocs pip
+install mkdocs-material pip install mkdocstrings-python pip install mkdocs-
+jupyter pip install notebook ``` ### full dependency list Our implementation
+works with python >= 3.9 and has the following dependencies ``` pytorch ==
+2.0.0 torch-geometric == 2.3.0 torch-scatter==2.1.1 torch-sparse==0.6.17 torch-
+spline-conv==1.2.2 pandas==1.5.3 clint==0.5.1 ``` ### Acknowledgments We thank
+the [OGB](https://ogb.stanford.edu/) team for their support throughout this
+project and sharing their website code for the construction of [TGB website]
+(https://tgb.complexdatalab.com/).
```

