# Comparing `tmp/scyan-1.4.0.tar.gz` & `tmp/scyan-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scyan-1.4.0.tar", max compression
+gzip compressed data, was "scyan-1.5.0.tar", max compression
```

## Comparing `scyan-1.4.0.tar` & `scyan-1.5.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0     1523 2022-06-21 14:16:37.061943 scyan-1.4.0/LICENSE
--rw-r--r--   0        0        0     5749 2023-03-15 14:16:25.446130 scyan-1.4.0/README.md
--rw-r--r--   0        0        0     2523 2023-03-17 08:10:19.859692 scyan-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      428 2023-03-01 17:15:22.116887 scyan-1.4.0/scyan/__init__.py
--rw-r--r--   0        0        0     7320 2023-03-14 16:05:04.745898 scyan-1.4.0/scyan/_io.py
--rw-r--r--   0        0        0      105 2023-02-02 17:56:56.555541 scyan-1.4.0/scyan/data/__init__.py
--rw-r--r--   0        0        0    10653 2023-03-01 17:45:55.532100 scyan-1.4.0/scyan/data/datasets.py
--rw-r--r--   0        0        0     2247 2023-03-15 14:48:14.832966 scyan-1.4.0/scyan/data/tensors.py
--rw-r--r--   0        0        0    23454 2023-03-15 14:25:46.743924 scyan-1.4.0/scyan/model.py
--rw-r--r--   0        0        0      154 2023-01-05 12:05:28.230767 scyan-1.4.0/scyan/module/__init__.py
--rw-r--r--   0        0        0     3026 2023-01-05 16:14:36.477088 scyan-1.4.0/scyan/module/coupling_layer.py
--rw-r--r--   0        0        0     4359 2023-03-14 16:15:25.976570 scyan-1.4.0/scyan/module/distribution.py
--rw-r--r--   0        0        0     2295 2023-01-05 16:14:36.477914 scyan-1.4.0/scyan/module/real_nvp.py
--rw-r--r--   0        0        0     6263 2023-03-13 16:20:29.003824 scyan-1.4.0/scyan/module/scyan_module.py
--rw-r--r--   0        0        0      265 2023-02-16 16:57:44.440578 scyan-1.4.0/scyan/plot/__init__.py
--rw-r--r--   0        0        0      277 2023-02-16 16:57:44.440808 scyan-1.4.0/scyan/plot/_scanpy_plot/README.md
--rw-r--r--   0        0        0       80 2023-02-16 16:57:44.440973 scyan-1.4.0/scyan/plot/_scanpy_plot/__init__.py
--rw-r--r--   0        0        0     5600 2023-02-16 16:57:44.441177 scyan-1.4.0/scyan/plot/_scanpy_plot/palettes.py
--rw-r--r--   0        0        0     2073 2023-02-21 12:51:49.284931 scyan-1.4.0/scyan/plot/_scanpy_plot/plot_settings.py
--rw-r--r--   0        0        0    32523 2023-02-22 14:33:55.801223 scyan-1.4.0/scyan/plot/_scanpy_plot/umap.py
--rw-r--r--   0        0        0     2709 2023-01-26 08:49:41.793824 scyan-1.4.0/scyan/plot/density.py
--rw-r--r--   0        0        0     5369 2023-02-16 16:57:44.442294 scyan-1.4.0/scyan/plot/dot.py
--rw-r--r--   0        0        0     5886 2023-01-26 08:49:41.893290 scyan-1.4.0/scyan/plot/expressions.py
--rw-r--r--   0        0        0     2093 2023-02-15 14:11:08.556874 scyan-1.4.0/scyan/plot/graph.py
--rw-r--r--   0        0        0     1930 2023-01-26 08:49:41.776081 scyan-1.4.0/scyan/plot/heatmap.py
--rw-r--r--   0        0        0     5116 2023-01-26 08:49:41.864417 scyan-1.4.0/scyan/plot/utils.py
--rw-r--r--   0        0        0     8721 2023-03-13 08:54:14.228057 scyan-1.4.0/scyan/preprocess.py
--rw-r--r--   0        0        0      176 2023-02-15 09:32:10.262198 scyan-1.4.0/scyan/tools/__init__.py
--rw-r--r--   0        0        0     5160 2023-03-01 17:03:54.505888 scyan-1.4.0/scyan/tools/biomarkers.py
--rw-r--r--   0        0        0     3717 2023-02-15 14:11:21.750476 scyan-1.4.0/scyan/tools/colors.py
--rw-r--r--   0        0        0     3863 2023-03-01 17:43:33.842136 scyan-1.4.0/scyan/tools/gating.py
--rw-r--r--   0        0        0     7485 2023-03-01 17:43:49.793672 scyan-1.4.0/scyan/tools/representation.py
--rw-r--r--   0        0        0     9800 2023-03-13 16:43:17.342607 scyan-1.4.0/scyan/utils.py
--rw-r--r--   0        0        0     7978 1970-01-01 00:00:00.000000 scyan-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1523 2022-06-21 14:16:37.061943 scyan-1.5.0/LICENSE
+-rw-r--r--   0        0        0     4834 2023-07-27 13:37:29.674996 scyan-1.5.0/README.md
+-rw-r--r--   0        0        0     2523 2023-07-27 13:35:26.327643 scyan-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      428 2023-03-01 17:15:22.116887 scyan-1.5.0/scyan/__init__.py
+-rw-r--r--   0        0        0     7320 2023-03-14 16:05:04.745898 scyan-1.5.0/scyan/_io.py
+-rw-r--r--   0        0        0     4972 2023-05-24 14:13:19.499852 scyan-1.5.0/scyan/baseline.py
+-rw-r--r--   0        0        0      105 2023-02-02 17:56:56.555541 scyan-1.5.0/scyan/data/__init__.py
+-rw-r--r--   0        0        0    10800 2023-07-19 11:10:11.286051 scyan-1.5.0/scyan/data/datasets.py
+-rw-r--r--   0        0        0     2247 2023-03-15 14:48:14.832966 scyan-1.5.0/scyan/data/tensors.py
+-rw-r--r--   0        0        0    24063 2023-07-19 15:05:26.018831 scyan-1.5.0/scyan/model.py
+-rw-r--r--   0        0        0      154 2023-01-05 12:05:28.230767 scyan-1.5.0/scyan/module/__init__.py
+-rw-r--r--   0        0        0     3026 2023-01-05 16:14:36.477088 scyan-1.5.0/scyan/module/coupling_layer.py
+-rw-r--r--   0        0        0     4511 2023-06-28 07:26:54.995994 scyan-1.5.0/scyan/module/distribution.py
+-rw-r--r--   0        0        0     2295 2023-01-05 16:14:36.477914 scyan-1.5.0/scyan/module/real_nvp.py
+-rw-r--r--   0        0        0     6263 2023-03-13 16:20:29.003824 scyan-1.5.0/scyan/module/scyan_module.py
+-rw-r--r--   0        0        0      334 2023-06-28 09:48:01.928525 scyan-1.5.0/scyan/plot/__init__.py
+-rw-r--r--   0        0        0      277 2023-02-16 16:57:44.440808 scyan-1.5.0/scyan/plot/_scanpy_plot/README.md
+-rw-r--r--   0        0        0       80 2023-02-16 16:57:44.440973 scyan-1.5.0/scyan/plot/_scanpy_plot/__init__.py
+-rw-r--r--   0        0        0     5600 2023-02-16 16:57:44.441177 scyan-1.5.0/scyan/plot/_scanpy_plot/palettes.py
+-rw-r--r--   0        0        0     2082 2023-06-19 07:50:37.617579 scyan-1.5.0/scyan/plot/_scanpy_plot/plot_settings.py
+-rw-r--r--   0        0        0    32523 2023-02-22 14:33:55.801223 scyan-1.5.0/scyan/plot/_scanpy_plot/umap.py
+-rw-r--r--   0        0        0     3755 2023-06-05 11:18:50.309892 scyan-1.5.0/scyan/plot/density.py
+-rw-r--r--   0        0        0     5369 2023-02-16 16:57:44.442294 scyan-1.5.0/scyan/plot/dot.py
+-rw-r--r--   0        0        0     5886 2023-01-26 08:49:41.893290 scyan-1.5.0/scyan/plot/expressions.py
+-rw-r--r--   0        0        0     2093 2023-02-15 14:11:08.556874 scyan-1.5.0/scyan/plot/graph.py
+-rw-r--r--   0        0        0     1930 2023-01-26 08:49:41.776081 scyan-1.5.0/scyan/plot/heatmap.py
+-rw-r--r--   0        0        0     5256 2023-06-28 13:00:11.423543 scyan-1.5.0/scyan/plot/ratios.py
+-rw-r--r--   0        0        0     5116 2023-01-26 08:49:41.864417 scyan-1.5.0/scyan/plot/utils.py
+-rw-r--r--   0        0        0     8721 2023-03-13 08:54:14.228057 scyan-1.5.0/scyan/preprocess.py
+-rw-r--r--   0        0        0      176 2023-02-15 09:32:10.262198 scyan-1.5.0/scyan/tools/__init__.py
+-rw-r--r--   0        0        0     5554 2023-07-19 11:20:34.296000 scyan-1.5.0/scyan/tools/biomarkers.py
+-rw-r--r--   0        0        0     3717 2023-02-15 14:11:21.750476 scyan-1.5.0/scyan/tools/colors.py
+-rw-r--r--   0        0        0     3863 2023-03-01 17:43:33.842136 scyan-1.5.0/scyan/tools/gating.py
+-rw-r--r--   0        0        0     7485 2023-03-01 17:43:49.793672 scyan-1.5.0/scyan/tools/representation.py
+-rw-r--r--   0        0        0     9784 2023-06-28 09:38:54.166009 scyan-1.5.0/scyan/utils.py
+-rw-r--r--   0        0        0     7063 1970-01-01 00:00:00.000000 scyan-1.5.0/PKG-INFO
```

### Comparing `scyan-1.4.0/LICENSE` & `scyan-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/pyproject.toml` & `scyan-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scyan"
-version = "1.4.0"
+version = "1.5.0"
 description = "Single-cell Cytometry Annotation Network"
 documentation = "https://mics-lab.github.io/scyan/"
 homepage = "https://mics-lab.github.io/scyan/"
 repository = "https://github.com/MICS-Lab/scyan"
 authors = ["Blampey Quentin <quentin.blampey@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `scyan-1.4.0/scyan/_io.py` & `scyan-1.5.0/scyan/_io.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/data/datasets.py` & `scyan-1.5.0/scyan/data/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,20 +178,20 @@
             names[file_path.suffix].add(file_path.stem)
 
     if dataset_name == "aml":
         add_remote_names(
             names,
             "default.csv",
             "default.h5ad",
-            "default.umap",
-            "groups_demo.csv",
             "short.h5ad",
         )
     elif dataset_name == "bmmc":
-        add_remote_names(names, "default.csv", "default.h5ad", "discovery.csv")
+        add_remote_names(names, "default.csv", "default.h5ad")
+    elif dataset_name == "poised":
+        add_remote_names(names, "default.csv", "full.csv", "short.csv", "default.h5ad")
     elif dataset_name == "debarcoding":
         add_remote_names(
             names,
             "default.csv",
             "default.h5ad",
         )
 
@@ -213,15 +213,15 @@
         log.info(f"Listing versions inside {dataset_path}:")
         list_path(dataset_path)
         return
 
     log.info(f"List of existing datasets inside {data_path}:")
     dataset_paths = set(data_path.iterdir())
 
-    for public_dataset in ["aml", "bmmc", "debarcoding"]:
+    for public_dataset in ["poised", "aml", "bmmc", "debarcoding"]:
         dataset_path = Path(data_path / public_dataset)
         dataset_path.mkdir(parents=True, exist_ok=True)
         dataset_paths.add(dataset_path)
 
     for dataset_path in dataset_paths:
         if dataset_path.is_dir():
             list_path(dataset_path)
@@ -253,23 +253,23 @@
 
 def load(
     dataset_name: str,
     version: Optional[str] = "default",
     table: Optional[str] = "default",
     reducer: Optional[str] = None,
 ) -> Tuple[AnnData, pd.DataFrame]:
-    """Load a dataset, i.e. its `AnnData` object and its knowledge table. Public datasets available are `"aml"`, `"bmmc"`, and `"debarcoding"`; note that, if the dataset was not loaded yet, it is automatically downloaded (requires internet connection). Existing dataset names and versions/tables can be listed using [scyan.data.list][].
+    """Load a dataset, i.e. its `AnnData` object and its knowledge table. Public datasets available are `"poised"`, `"aml"`, `"bmmc"`, and `"debarcoding"`; note that, if the dataset was not loaded yet, it is automatically downloaded (requires internet connection). Existing dataset names and versions/tables can be listed using [scyan.data.list][].
 
     !!! note
         If you want to load your own dataset, you first have to [create it](../../advanced/data).
     !!! note
-        If `scyan` repository was cloned, then the data will be saved in the `data` folder of the repository, else at `<home_path>/.scyan_data`
+        The data is saved by default inside `<home_path>/.scyan_data`. Optionally, if `scyan` repository was cloned, you can create `<scyan_repository_path>/data` and use it instead of the default data folder.
 
     Args:
-        dataset_name: Name of the dataset. Either one of your dataset, or one public dataset among `"aml"`, `"bmmc"`, and `"debarcoding"`.
+        dataset_name: Name of the dataset. Either one of your dataset, or one public dataset among `"poised"`, `"aml"`, `"bmmc"`, and `"debarcoding"`.
         version: Name of the `anndata` file (.h5ad) that should be loaded. The available versions can be listed with `scyan.data.list()`. If `None`, don't return an `adata` object.
         table: Name of the knowledge table that should be loaded. If `None`, don't return the `table` dataframe.
         reducer: Name of the umap reducer that should be loaded. If `None`, don't return the `UMAP` reducer.
 
     Returns:
         Tuple containing the requested data, i.e. by default a tuple `(adata, table)` is returned (the adata instance and the knowledge table). But, for instance, if `version is None` and `reducer` is provided, then it returns a tuple `(table, reducer)`.
     """
```

### Comparing `scyan-1.4.0/scyan/data/tensors.py` & `scyan-1.5.0/scyan/data/tensors.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/model.py` & `scyan-1.5.0/scyan/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         continuous_covariates: Optional[List[str]] = None,
         categorical_covariates: Optional[List[str]] = None,
         continuum_markers: Optional[List[str]] = None,
         hidden_size: int = 16,
         n_hidden_layers: int = 6,
         n_layers: int = 7,
         prior_std: float = 0.3,
+        warm_up: Optional[tuple[float, int]] = (0.35, 4),
         lr: float = 5e-4,
         batch_size: int = 8_192,
         temperature: float = 0.5,
         modulo_temp: int = 3,
         max_samples: Optional[int] = 200_000,
         batch_key: Optional[str] = None,
     ):
@@ -60,14 +61,15 @@
             continuous_covariates: Optional list of keys in `adata.obs` that refers to continuous variables to use during the training.
             categorical_covariates: Optional list of keys in `adata.obs` that refers to categorical variables to use during the training.
             continuum_markers: Optional list of markers from the table whose expression is a continuum (for instance, it is often the case for PD1/PDL1). We advise to use it carefully, and keep values of -1 and 1 in the table.
             hidden_size: Hidden size of the MLP (`s`, `t`).
             n_hidden_layers: Number of hidden layers in the MLP.
             n_layers: Number of coupling layers.
             prior_std: Standard deviation $\sigma$ of the cell-specific random variable $H$.
+            warm_up: If not `None`, sets the model prior standard deviation to `max(warm_up[0], prior_std)` during the first `warm_up[1]` epochs.
             lr: Model learning rate.
             batch_size: Model batch size.
             temperature: Temperature to favor small populations.
             modulo_temp: At which frequency temperature has to be applied.
             max_samples: Maximum number of samples per epoch.
             batch_key: Key in `adata.obs` referring to the cell batch variable.
         """
@@ -97,15 +99,15 @@
         self.module = ScyanModule(
             torch.tensor(table.values, dtype=torch.float32),
             self.covariates.shape[1],
             torch.tensor(np.isin(self.var_names, self.continuum_markers)),
             hidden_size,
             n_hidden_layers,
             n_layers,
-            prior_std,
+            max(warm_up[0], prior_std) if warm_up is not None else prior_std,
             temperature,
         )
 
         log.info(f"Initialized {self}")
 
     def __repr__(self) -> str:
         covs = self.continuous_covariates + self.categorical_covariates
@@ -303,14 +305,22 @@
         use_temp = self.current_epoch % self.hparams.modulo_temp > 0
         loss = self.module.kl(*data, use_temp)
 
         self.log("loss", loss, on_epoch=True, on_step=True)
 
         return loss
 
+    def on_train_epoch_end(self):
+        if (
+            self.hparams.warm_up is not None
+            and self.current_epoch == self.hparams.warm_up[1] - 1
+        ):
+            print("Ended warm up epochs")
+            self.module.prior.prior_std = self.hparams.prior_std
+
     @_requires_fit
     @torch.no_grad()
     def predict(
         self,
         key_added: Optional[str] = "scyan_pop",
         add_levels: bool = True,
         log_prob_th: float = -50,
@@ -325,14 +335,15 @@
             add_levels: If `True`, and if [hierarchical population names](../../tutorials/usage/#working-with-hierarchical-populations) were provided, then it also saves the prediction for every population level.
             log_prob_th: If the log-probability of the most probable population for one cell is below this threshold, this cell will not be annotated (`np.nan`).
 
         Returns:
             Population predictions (pandas `Series` of length $N$ cells).
         """
         df = self.predict_proba()
+        self.adata.obs["scyan_log_probs"] = df["max_log_prob_u"].values
 
         populations = df.iloc[:, : self.n_pops].idxmax(axis=1).astype("category")
         populations[df["max_log_prob_u"] < log_prob_th] = np.nan
 
         if key_added is not None:
             self.adata.obs[key_added] = pd.Categorical(
                 populations, categories=self.pop_names
@@ -534,10 +545,10 @@
                 logger=logger,
                 **trainer_args,
             )
 
         trainer.fit(self)
 
         self._is_fitted = True
-        log.info("Successfully ended traning.")
+        log.info("Successfully ended training.")
 
         return self
```

### Comparing `scyan-1.4.0/scyan/module/coupling_layer.py` & `scyan-1.5.0/scyan/module/coupling_layer.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/module/distribution.py` & `scyan-1.5.0/scyan/module/distribution.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,39 +17,45 @@
         Args:
             rho: Tensor $\rho$ representing the knowledge table (size $P$ x $M$)
             is_continuum_marker: tensor of size $M$ whose values tell if the marker is a continuum of expressions.
             prior_std: Standard deviation $\sigma$ for $H$.
             n_markers: Number of markers in the table.
         """
         super().__init__()
-        self.prior_std = prior_std
         self.n_markers = n_markers
         self.is_continuum_marker = is_continuum_marker
 
         self.register_buffer("rho", rho)
         self.register_buffer("loc", torch.zeros((n_markers)))
-        self.register_buffer("cov", torch.eye((n_markers)) * self.prior_std**2)
         self.set_rho_mask()
 
+        self.prior_std = prior_std
         self.uniform = distributions.Uniform(-1, 1)
-        self.normal = distributions.Normal(0, self.prior_std)
+
+    @property
+    def prior_std(self):
+        return self._prior_std
+
+    @prior_std.setter
+    def prior_std(self, std: float) -> None:
+        self._prior_std = std
+        self.register_buffer("cov", torch.eye((self.n_markers)) * std**2)
+        self.normal = distributions.Normal(0, std)
+        self.compute_constant_terms()
 
     def set_rho_mask(self) -> None:
         rho_mask = self.rho.isnan()
         self.rho[rho_mask] = 0
         self.register_buffer("rho_mask", rho_mask)
-        self.update()
+        self.compute_modes()
 
     def fill_rho(self, means: torch.Tensor) -> None:
         # TODO: what if one population was not predicted?
         self.rho[self.rho_mask] = means[self.rho_mask]
         self.register_buffer("rho_mask", torch.full_like(self.rho, False, dtype=bool))
-        self.update()
-
-    def update(self):
         self.compute_modes()
         self.compute_constant_terms()
 
     def compute_modes(self):
         self.factor = torch.ones(self.n_markers, dtype=torch.float32)
         self.factor[self.is_continuum_marker] = 5
         self.factor = self.factor[None, None, :]
```

### Comparing `scyan-1.4.0/scyan/module/real_nvp.py` & `scyan-1.5.0/scyan/module/real_nvp.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/module/scyan_module.py` & `scyan-1.5.0/scyan/module/scyan_module.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/plot/_scanpy_plot/palettes.py` & `scyan-1.5.0/scyan/plot/_scanpy_plot/palettes.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/plot/_scanpy_plot/plot_settings.py` & `scyan-1.5.0/scyan/plot/_scanpy_plot/plot_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Copied from https://github.com/scverse/scanpy (and modified)
 
-import matplotlib_inline.backend_inline
 from cycler import cycler
 from matplotlib import rcParams
 
 from . import palettes
 
 
 def set_rcParams_scanpy(fontsize):
@@ -67,13 +66,15 @@
     rcParams["grid.color"] = ".8"
 
 
 def quality_settings():
     import builtins
 
     if getattr(builtins, "__IPYTHON__", False):
+        import matplotlib_inline.backend_inline
+
         matplotlib_inline.backend_inline.set_matplotlib_formats("png2x")
 
 
 def reset_plot_settings(fontsize: int = 10):
     quality_settings()
     set_rcParams_scanpy(fontsize)
```

### Comparing `scyan-1.4.0/scyan/plot/_scanpy_plot/umap.py` & `scyan-1.5.0/scyan/plot/_scanpy_plot/umap.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/plot/density.py` & `scyan-1.5.0/scyan/plot/density.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import List, Optional, Union
 
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from anndata import AnnData
 
 from ..utils import _get_subset_indices
 from .utils import check_population, get_palette_others, plot_decorator, select_markers
@@ -82,7 +83,32 @@
         col_wrap=ncols,
         kind="kde",
         common_norm=False,
         facet_kws=dict(sharey=False),
         palette=get_palette_others(df, key),
         hue_order=sorted(df[key].unique(), key="Others".__eq__),
     )
+
+
+@plot_decorator(adata=True)
+def log_prob_threshold(adata: AnnData, show: bool = True):
+    """Plot the number of cells annotated depending on the log probability threshold (below which cells are left non-classified). It can be helpful to determine the best threshold value, i.e. before a significative decrease in term of number of cells annotated.
+
+    !!! note
+        To use this function, you first need to fit a `scyan.Scyan` model and use the `model.predict()` method.
+
+    Args:
+        adata: The `anndata` object used during the model training.
+        show: Whether or not to display the figure.
+    """
+    assert (
+        "scyan_log_probs" in adata.obs
+    ), f"Cannot find 'scyan_log_probs' in adata.obs. Have you run model.predict()?"
+
+    x = np.sort(adata.obs["scyan_log_probs"])
+    y = 1 - np.arange(len(x)) / float(len(x))
+
+    plt.plot(x, y)
+    plt.xlim(-100, x.max())
+    sns.despine(offset=10, trim=True)
+    plt.ylabel("Ratio of predicted cells")
+    plt.xlabel("Log density threshold")
```

### Comparing `scyan-1.4.0/scyan/plot/dot.py` & `scyan-1.5.0/scyan/plot/dot.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/plot/expressions.py` & `scyan-1.5.0/scyan/plot/expressions.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/plot/graph.py` & `scyan-1.5.0/scyan/plot/graph.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/plot/heatmap.py` & `scyan-1.5.0/scyan/plot/heatmap.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/plot/utils.py` & `scyan-1.5.0/scyan/plot/utils.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/preprocess.py` & `scyan-1.5.0/scyan/preprocess.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/tools/biomarkers.py` & `scyan-1.5.0/scyan/tools/biomarkers.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,48 +18,53 @@
 def cell_type_ratios(
     adata: AnnData,
     groupby: Union[str, List[str], None] = None,
     normalize: bool = True,
     key: str = "scyan_pop",
     among: str = None,
 ) -> pd.DataFrame:
-    """Count for each patient (or group) the number of cells for each population.
+    """Computes the ratio of cells per population. This ratio can be provided for each patient (or for any kind of 'group').
 
     Args:
         adata: An `AnnData` object.
         groupby: Key(s) of `adata.obs` used to create groups (e.g. the patient ID).
-        normalize: If `False`, returns counts instead of percentages.
+        normalize: If `False`, returns counts instead of ratios. If `"%"`, use percentage instead of ratios in `[0, 1]`;
         key: Key of `adata.obs` containing the population names (or the values to count).
-        among: Key of `adata.obs` containing the parent population name. For example, if 'T CD4 RM' is found in `adata.obs[key]`, then we may find something like 'T cell' in `adata.obs[among]`. Typically, if using hierarchical populations, you can provide `'scyan_pop_level'` with your level name.
+        among: Key of `adata.obs` containing the parent population name. Typically, if using hierarchical populations, you can provide `'scyan_pop_level'` with your level name. E.g., if the parent of population of "T CD4 RM" is called "T cells" in `adata.obs[among]`, then this function computes the 'T CD4 RM ratio among T cells'.
 
     Returns:
-        A DataFrame of counts (one row per group, one column per population).
+        A DataFrame of ratios or counts (one row per group, one column per population). If `normalize=False`, then each row sums to 1 (for `among=None`).
     """
-    normalize = among is not None or normalize
-    column_suffix = "percentage" if normalize else "count"
+    assert (
+        among is None or normalize
+    ), "If 'among' is `None`, then normalize can't be `False`"
+
+    column_suffix = (
+        ("percentage" if normalize == "%" else "ratio") if normalize else "count"
+    )
 
     counts = _get_counts(adata, groupby, key, normalize)
 
     if among is None:
         counts.columns = [f"{name} {column_suffix}" for name in counts.columns]
-        return counts
+        return counts.mul(100) if normalize == "%" else counts
 
     parents_count = _get_counts(adata, groupby, among, normalize)
 
     df_parent = adata.obs.groupby(among)[key].apply(lambda s: s.value_counts()).unstack()
     assert (
-        (df_parent > 0).sum(0) == 1
-    ).all(), f"Each population from adata.obs['{key}'] should have one and only one parent population in adata.obs['{among}']"
+        (df_parent > 0).sum(0) <= 1
+    ).all(), f"Each population from adata.obs['{key}'] should have only one parent population in adata.obs['{among}']"
     to_parent_dict = dict(df_parent.idxmax())
 
     counts /= parents_count[[to_parent_dict[pop] for pop in counts.columns]].values
     counts.columns = [
         f"{pop} {column_suffix} among {to_parent_dict[pop]}" for pop in counts.columns
     ]
-    return counts
+    return counts.mul(100) if normalize == "%" else counts
 
 
 def mean_intensities(
     adata: AnnData,
     groupby: Union[str, List[str], None] = None,
     layer: Optional[str] = None,
     key: str = "scyan_pop",
```

### Comparing `scyan-1.4.0/scyan/tools/colors.py` & `scyan-1.5.0/scyan/tools/colors.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/tools/gating.py` & `scyan-1.5.0/scyan/tools/gating.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/tools/representation.py` & `scyan-1.5.0/scyan/tools/representation.py`

 * *Files identical despite different names*

### Comparing `scyan-1.4.0/scyan/utils.py` & `scyan-1.5.0/scyan/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,15 +260,15 @@
             f"Found {ratio_nan:.1%} of NA in the table, which is very high. If this is intended, just ignore the warning."
         )
 
     X = adata[:, df.columns].X
 
     _check_is_processed(X)
 
-    if np.abs(X.std(axis=0) - 1).max() > 0.2 or X.min(0).max() >= 0:
+    if np.abs(adata.X.std(axis=0).mean() - 1) > 0.1:
         log.warning(
             "It seems that the data is not standardised. We advise using scaling (scyan.preprocess.scale) before initializing the model."
         )
 
     duplicates = df.duplicated()
     if duplicates.any():
         duplicates_names = duplicates[duplicates].index.get_level_values(0)
```

### Comparing `scyan-1.4.0/PKG-INFO` & `scyan-1.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scyan
-Version: 1.4.0
+Version: 1.5.0
 Summary: Single-cell Cytometry Annotation Network
 Home-page: https://mics-lab.github.io/scyan/
 License: BSD-3-Clause
 Author: Blampey Quentin
 Author-email: quentin.blampey@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: BSD License
@@ -125,52 +125,34 @@
 This code should run in approximately 40 seconds (once the dataset is loaded).
 For more usage demo, read the [tutorials](https://mics-lab.github.io/scyan/tutorials/usage/) or the complete [documentation](https://mics-lab.github.io/scyan/).
 
 # Technical description
 
 Scyan is a **Python** library based on:
 
-- [_Pytorch_](https://pytorch.org/), a deep learning framework
 - [_AnnData_](https://anndata.readthedocs.io/en/latest/), a data library that works nicely with single-cell data
-- [_Pytorch Lighning_](https://www.pytorchlightning.ai/), for model training
-- [_Hydra_](https://hydra.cc/docs/intro/), for project configuration (optional)
-- [_Weight & Biases_](https://wandb.ai/site), for model monitoring (optional)
-
-# Project layout
-
-    .github/      # Github CI and templates
-    config/       # Hydra configuration folder (optional use)
-    data/         # Data folder containing adata files and csv tables
-    docs/         # The folder used to build the documentation
-    scripts/      # Scripts to reproduce the results from the article
-    tests/        # Folder containing tests
-    scyan/                    # Library source code
-        data/                 # Folder with data-related functions and classes
-            datasets.py       # Load and save datasets
-            tensors.py        # Pytorch data-related classes for training
-        module/               # Folder containing neural network modules
-            coupling_layer.py # Coupling layer
-            distribution.py   # Prior distribution (called U in the article)
-            real_nvp.py       # Normalizing Flow
-            scyan_module      # Core module
-        plot/                 # Plots
-            ...
-        tools/
-            ...               # Tools (umap, subclustering, ...)
-        model.py              # Scyan model class
-        _io.py                # Input / output functions
-        preprocess.py         # Preprocessing functions
-        utils.py              # Misc functions
-    .gitattributes
-    .gitignore
-    CONTRIBUTING.md   # To read before contributing
-    LICENSE
-    mkdocs.yml        # The docs configuration file
-    poetry.lock
-    pyproject.toml    # Dependencies, project metadata, and more
-    README.md
-    setup.py          # Setup file, see `pyproject.toml`
+- [_Pytorch_](https://pytorch.org/), a deep learning framework
+- [_Pytorch Lightning_](https://www.pytorchlightning.ai/), for model training
+
+Optionally, it also supports:
+- [_Hydra_](https://hydra.cc/docs/intro/), for project configuration
+- [_Weight & Biases_](https://wandb.ai/site), for model monitoring
 
 # Cite us
 
-Our paper is not published yet. Meanwhile, you can [read our preprint on arXiv](https://arxiv.org/abs/2208.05745).
+Our paper is published in ***Briefings in Bioinformatics*** and is available [here](https://doi.org/10.1093/bib/bbad260).
+```txt
+@article{10.1093/bib/bbad260,
+    author = {Blampey, Quentin and Bercovici, Nadège and Dutertre, Charles-Antoine and Pic, Isabelle and Ribeiro, Joana Mourato and André, Fabrice and Cournède, Paul-Henry},
+    title = "{A biology-driven deep generative model for cell-type annotation in cytometry}",
+    journal = {Briefings in Bioinformatics},
+    pages = {bbad260},
+    year = {2023},
+    month = {07},
+    issn = {1477-4054},
+    doi = {10.1093/bib/bbad260},
+    url = {https://doi.org/10.1093/bib/bbad260},
+    eprint = {https://academic.oup.com/bib/advance-article-pdf/doi/10.1093/bib/bbad260/50973199/bbad260.pdf},
+}
+
+```
```

