# Comparing `tmp/hssm-0.1.2.tar.gz` & `tmp/hssm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hssm-0.1.2.tar", max compression
+gzip compressed data, was "hssm-0.1.3.tar", max compression
```

## Comparing `hssm-0.1.2.tar` & `hssm-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1100 2023-06-28 13:42:06.739838 hssm-0.1.2/LICENSE
--rw-r--r--   0        0        0     5903 2023-07-24 23:59:30.490702 hssm-0.1.2/README.md
--rw-r--r--   0        0        0     4002 2023-07-24 23:59:30.513816 hssm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      434 2023-07-24 23:59:30.514119 hssm-0.1.2/src/hssm/__init__.py
--rw-r--r--   0        0        0     4898 2023-07-24 23:59:30.514548 hssm-0.1.2/src/hssm/config.py
--rw-r--r--   0        0        0   193800 2023-06-29 17:28:42.110365 hssm-0.1.2/src/hssm/datasets/cavanagh_theta_nn.csv
--rw-r--r--   0        0        0     2451 2023-06-29 20:29:06.385419 hssm-0.1.2/src/hssm/datasets.py
--rw-r--r--   0        0        0      466 2023-06-29 20:29:06.385750 hssm-0.1.2/src/hssm/distribution_utils/__init__.py
--rw-r--r--   0        0        0    22158 2023-07-24 23:59:30.514923 hssm-0.1.2/src/hssm/distribution_utils/dist.py
--rw-r--r--   0        0        0      387 2023-06-29 20:29:06.386702 hssm-0.1.2/src/hssm/distribution_utils/onnx/__init__.py
--rw-r--r--   0        0        0     9978 2023-07-21 17:14:44.323287 hssm-0.1.2/src/hssm/distribution_utils/onnx/onnx.py
--rw-r--r--   0        0        0     1877 2023-06-27 19:37:55.283473 hssm-0.1.2/src/hssm/distribution_utils/onnx/onnx2pt.py
--rw-r--r--   0        0        0     5203 2023-06-27 19:37:55.283601 hssm-0.1.2/src/hssm/distribution_utils/onnx/onnx2xla.py
--rw-r--r--   0        0        0    34248 2023-07-24 23:59:30.515319 hssm-0.1.2/src/hssm/hssm.py
--rw-r--r--   0        0        0      180 2023-06-29 20:29:06.387621 hssm-0.1.2/src/hssm/likelihoods/__init__.py
--rw-r--r--   0        0        0     9587 2023-07-24 23:59:30.515907 hssm-0.1.2/src/hssm/likelihoods/analytical.py
--rw-r--r--   0        0        0    15270 2023-07-24 23:59:30.516258 hssm-0.1.2/src/hssm/param.py
--rw-r--r--   0        0        0     2504 2023-07-07 00:29:33.294967 hssm-0.1.2/src/hssm/simulator.py
--rw-r--r--   0        0        0    11168 2023-07-24 23:59:30.516691 hssm-0.1.2/src/hssm/utils.py
--rw-r--r--   0        0        0     7005 1970-01-01 00:00:00.000000 hssm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-07-26 21:57:17.003047 hssm-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5199 2023-07-26 21:57:17.003047 hssm-0.1.3/README.md
+-rw-r--r--   0        0        0     4002 2023-07-26 21:57:17.095048 hssm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      466 2023-07-26 21:57:17.095048 hssm-0.1.3/src/hssm/__init__.py
+-rw-r--r--   0        0        0     7309 2023-07-26 21:57:17.095048 hssm-0.1.3/src/hssm/config.py
+-rw-r--r--   0        0        0   193800 2023-07-26 21:57:17.095048 hssm-0.1.3/src/hssm/datasets/cavanagh_theta_nn.csv
+-rw-r--r--   0        0        0     2451 2023-07-26 21:57:17.095048 hssm-0.1.3/src/hssm/datasets.py
+-rw-r--r--   0        0        0      466 2023-07-26 21:57:17.095048 hssm-0.1.3/src/hssm/distribution_utils/__init__.py
+-rw-r--r--   0        0        0    22232 2023-07-26 21:57:17.099048 hssm-0.1.3/src/hssm/distribution_utils/dist.py
+-rw-r--r--   0        0        0      387 2023-07-26 21:57:17.099048 hssm-0.1.3/src/hssm/distribution_utils/onnx/__init__.py
+-rw-r--r--   0        0        0     9978 2023-07-26 21:57:17.099048 hssm-0.1.3/src/hssm/distribution_utils/onnx/onnx.py
+-rw-r--r--   0        0        0     1877 2023-07-26 21:57:17.099048 hssm-0.1.3/src/hssm/distribution_utils/onnx/onnx2pt.py
+-rw-r--r--   0        0        0     5203 2023-07-26 21:57:17.099048 hssm-0.1.3/src/hssm/distribution_utils/onnx/onnx2xla.py
+-rw-r--r--   0        0        0    35138 2023-07-26 21:57:17.099048 hssm-0.1.3/src/hssm/hssm.py
+-rw-r--r--   0        0        0      180 2023-07-26 21:57:17.099048 hssm-0.1.3/src/hssm/likelihoods/__init__.py
+-rw-r--r--   0        0        0     9631 2023-07-26 21:57:17.099048 hssm-0.1.3/src/hssm/likelihoods/analytical.py
+-rw-r--r--   0        0        0    16808 2023-07-26 21:57:17.099048 hssm-0.1.3/src/hssm/param.py
+-rw-r--r--   0        0        0     2504 2023-07-26 21:57:17.099048 hssm-0.1.3/src/hssm/simulator.py
+-rw-r--r--   0        0        0    11168 2023-07-26 21:57:17.099048 hssm-0.1.3/src/hssm/utils.py
+-rw-r--r--   0        0        0     6343 1970-01-01 00:00:00.000000 hssm-0.1.3/PKG-INFO
```

### Comparing `hssm-0.1.2/LICENSE` & `hssm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hssm-0.1.2/README.md` & `hssm-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 <div style="position: relative; width: 100%;">
   <img src="docs/images/mainlogo.png" style="width: 250px;">
   <a href="https://ccbs.carney.brown.edu/brainstorm" style="position: absolute; right: 0; top: 50%; transform: translateY(-50%);">
     <img src="docs/images/Brain-Bolt-%2B-Circuits.gif" style="width: 100px;">
   </a>
 </div>
 
-
 ## HSSM - Hierarchical Sequential Sampling Modeling
 
 ![PyPI](https://img.shields.io/pypi/v/hssm)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hssm)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/lnccbrown/HSSM)
 ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/lnccbrown/HSSM/run_tests.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 ### Overview
 
-HSSM is a Python toolbox that provides a seamless combination of state-of-the-art likelihood approximation methods with the wider ecosystem of probabilistic programming languages. It facilitates flexible hierarchical model building and inference via modern MCMC samplers. HSSM is user-friendly and provides the ability to rigorously estimate the impact of neural and other trial-by-trial covariates through parameter-wise mixed-effects models for a large variety of cognitive process models. HSSM is a  <a href="https://ccbs.carney.brown.edu/brainstorm">BRAINSTORM</a> project in collaboration with the Center for Computation and Visualization and the Center for Computational Brain Science within the Carney Institute at Brown University. 
+HSSM is a Python toolbox that provides a seamless combination of state-of-the-art likelihood approximation methods with the wider ecosystem of probabilistic programming languages. It facilitates flexible hierarchical model building and inference via modern MCMC samplers. HSSM is user-friendly and provides the ability to rigorously estimate the impact of neural and other trial-by-trial covariates through parameter-wise mixed-effects models for a large variety of cognitive process models. HSSM is a <a href="https://ccbs.carney.brown.edu/brainstorm">BRAINSTORM</a> project in collaboration with the Center for Computation and Visualization and the Center for Computational Brain Science within the Carney Institute at Brown University.
 
 - Allows approximate hierarchical Bayesian inference via various likelihood approximators.
 - Estimate impact of neural and other trial-by-trial covariates via native hierarchical mixed-regression support.
 - Extensible for users to add novel models with corresponding likelihoods.
 - Built on PyMC with support from the Python Bayesian ecosystem at large.
 - Incorporates Bambi's intuitive `lmer`-like regression parameter specification for within- and between-subject effects.
 - Native ArviZ support for plotting and other convenience functions to aid the Bayesian workflow.
@@ -37,53 +36,20 @@
 ```
 
 You can also install the bleeding edge version of `hssm` directly from this repo:
 
 ```
 pip install git+https://github.com/lnccbrown/HSSM.git
 ```
-**Note**: Possible solutions to any issues with installations with hssm can be located [here](https://github.com/lnccbrown/HSSM/discussions). We recommend leveraging an environment manager with Python 3.9~3.11 to prevent any problems with dependencies during the installation process. Please note that hssm is tested for python 3.9, 3.10, 3.11. Use other python versions with caution. For more detailed guidance, please refer to this [discussion](https://github.com/lnccbrown/HSSM/discussions/152). 
-
-### Optional Installation
-
-**Dependency for graph() Function**
-
-Note: In addition to the installation of the main hssm class, there is an optional dependency for the graph() function. This dependency requires graphviz, which can be installed conveniently using conda with the following command:
-
-```
-conda install -c conda-forge python-graphviz
-```
-
-Alternatively, you have the option to install the graphviz binaries manually and then install the Python bindings using pip with the following command:
-
-```
-pip install graphviz
-```
-
-**Dependency for sampler="nuts_numpyro"**
 
-To utilize the nuts_numpyro sampler, please follow these steps:
+You will need optional dependencies to use JAX-based samplers and graph the models.
+Please refer to our [installation guide](https://lnccbrown.github.io/HSSM/getting_started/installation/)
+for more detailed instructions.
 
-1. Install numpyro by executing the following command:
-
-```
-pip install numpyro
-```
-
-2. Import the necessary modules and configure the required settings:
-
-```
-import numpyro
-from jax.config import config
-
-numpyro.set_host_device_count(jax.local_device_count())
-config.update("jax_enable_x64", False)
-```
-
-For more information please refer to [jax documentation](https://jax.readthedocs.io/en/latest/installation.html).
+**Note**: Possible solutions to any issues with installations with hssm can be located [here](https://github.com/lnccbrown/HSSM/discussions). We recommend leveraging an environment manager with Python 3.9~3.11 to prevent any problems with dependencies during the installation process. Please note that hssm is tested for python 3.9, 3.10, 3.11. Use other python versions with caution.
 
 ## Example
 
 Here is a simple example of how to use HSSM:
 
 ```python
 import hssm
@@ -99,28 +65,31 @@
 model = hssm.HSSM(
     model="ddm",
     data=cav_data,
     include=[
         {
             "name": "v",
             "prior": {
-                "Intercept": {"name": "Uniform", "lower": -3.0, "upper": 3.0},
-                "theta": {"name": "Uniform", "lower": -1.0, "upper": 1.0},
+                "Intercept": {"name": "Normal", "mu": 0.0, "sigma": 0.0},
+                "theta": {"name": "Normal", "mu": 0.0, "sigma": 0.0},
             },
-            "formula": "v ~ (1|subj_idx) + theta",
+            "formula": "v ~ (1|participant_id) + theta",
             "link": "identity",
         },
     ],
 )
 
 # Sample from the posterior for this model
 model.sample()
 ```
 
-## Example
+To quickly get started with HSSM, please follow [this tutorial](https://lnccbrown.github.io/HSSM/getting_started/getting_started/).
+For a deeper dive into HSSM, please follow [our main tutorial](https://lnccbrown.github.io/HSSM/tutorials/main_tutorial/).
+
+## License
 
 HSSM is licensed under [Copyright 2023, Brown University, Providence, RI](LICENSE)
 
 ## Support
 
 For questions, bug reports, or other unexpected issues, please open an issue on the GitHub repository.
```

#### html2text {}

```diff
@@ -24,50 +24,40 @@
 effects. - Native ArviZ support for plotting and other convenience functions to
 aid the Bayesian workflow. - Utilizes the ONNX format for translation of
 differentiable likelihood approximators across backends. ### Official
 documentation link can be found [here](https://lnccbrown.github.io/HSSM/). ##
 Installation `hssm` is available through PyPI. You can install it with Pip via:
 ``` pip install hssm ``` You can also install the bleeding edge version of
 `hssm` directly from this repo: ``` pip install git+https://github.com/
-lnccbrown/HSSM.git ``` **Note**: Possible solutions to any issues with
-installations with hssm can be located [here](https://github.com/lnccbrown/
-HSSM/discussions). We recommend leveraging an environment manager with Python
-3.9~3.11 to prevent any problems with dependencies during the installation
-process. Please note that hssm is tested for python 3.9, 3.10, 3.11. Use other
-python versions with caution. For more detailed guidance, please refer to this
-[discussion](https://github.com/lnccbrown/HSSM/discussions/152). ### Optional
-Installation **Dependency for graph() Function** Note: In addition to the
-installation of the main hssm class, there is an optional dependency for the
-graph() function. This dependency requires graphviz, which can be installed
-conveniently using conda with the following command: ``` conda install -
-c conda-forge python-graphviz ``` Alternatively, you have the option to install
-the graphviz binaries manually and then install the Python bindings using pip
-with the following command: ``` pip install graphviz ``` **Dependency for
-sampler="nuts_numpyro"** To utilize the nuts_numpyro sampler, please follow
-these steps: 1. Install numpyro by executing the following command: ``` pip
-install numpyro ``` 2. Import the necessary modules and configure the required
-settings: ``` import numpyro from jax.config import config
-numpyro.set_host_device_count(jax.local_device_count()) config.update
-("jax_enable_x64", False) ``` For more information please refer to [jax
-documentation](https://jax.readthedocs.io/en/latest/installation.html). ##
-Example Here is a simple example of how to use HSSM: ```python import hssm #
-Set float type to float32 to avoid a current bug in PyMC # This will not be
-necessary in the future hssm.set_floatX("float32") # Load a package-supplied
-dataset cav_data = hssm.load_data('cavanagh_theta') # Define a basic
-hierarchical model with trial-level covariates model = hssm.HSSM( model="ddm",
-data=cav_data, include=[ { "name": "v", "prior": { "Intercept": {"name":
-"Uniform", "lower": -3.0, "upper": 3.0}, "theta": {"name": "Uniform", "lower":
--1.0, "upper": 1.0}, }, "formula": "v ~ (1|subj_idx) + theta", "link":
+lnccbrown/HSSM.git ``` You will need optional dependencies to use JAX-based
+samplers and graph the models. Please refer to our [installation guide](https:/
+/lnccbrown.github.io/HSSM/getting_started/installation/) for more detailed
+instructions. **Note**: Possible solutions to any issues with installations
+with hssm can be located [here](https://github.com/lnccbrown/HSSM/discussions).
+We recommend leveraging an environment manager with Python 3.9~3.11 to prevent
+any problems with dependencies during the installation process. Please note
+that hssm is tested for python 3.9, 3.10, 3.11. Use other python versions with
+caution. ## Example Here is a simple example of how to use HSSM: ```python
+import hssm # Set float type to float32 to avoid a current bug in PyMC # This
+will not be necessary in the future hssm.set_floatX("float32") # Load a
+package-supplied dataset cav_data = hssm.load_data('cavanagh_theta') # Define a
+basic hierarchical model with trial-level covariates model = hssm.HSSM
+( model="ddm", data=cav_data, include=[ { "name": "v", "prior": { "Intercept":
+{"name": "Normal", "mu": 0.0, "sigma": 0.0}, "theta": {"name": "Normal", "mu":
+0.0, "sigma": 0.0}, }, "formula": "v ~ (1|participant_id) + theta", "link":
 "identity", }, ], ) # Sample from the posterior for this model model.sample()
-``` ## Example HSSM is licensed under [Copyright 2023, Brown University,
-Providence, RI](LICENSE) ## Support For questions, bug reports, or other
-unexpected issues, please open an issue on the GitHub repository. ##
-Contribution If you want to contribute to this project, please familiarize
-yourself with our [contribution guidelines](docs/CONTRIBUTING.md). ##
-Acknowledgements We would like to extend our gratitude to the following
+``` To quickly get started with HSSM, please follow [this tutorial](https://
+lnccbrown.github.io/HSSM/getting_started/getting_started/). For a deeper dive
+into HSSM, please follow [our main tutorial](https://lnccbrown.github.io/HSSM/
+tutorials/main_tutorial/). ## License HSSM is licensed under [Copyright 2023,
+Brown University, Providence, RI](LICENSE) ## Support For questions, bug
+reports, or other unexpected issues, please open an issue on the GitHub
+repository. ## Contribution If you want to contribute to this project, please
+familiarize yourself with our [contribution guidelines](docs/CONTRIBUTING.md).
+## Acknowledgements We would like to extend our gratitude to the following
 individuals for their valuable contributions to the development of the HSSM
 package: - [Bambi](https://github.com/bambinos/bambi) - A special thanks to the
 Bambi project for providing inspiration, guidance, and support throughout the
 development process. [TomÃ¡s Capretto](https://github.com/tomicapretto), a key
 contributor to Bambi, provided invaluable assistance in the development of the
 HSSM package. Those contributions have greatly enhanced the functionality and
 quality of the HSSM.
```

### Comparing `hssm-0.1.2/pyproject.toml` & `hssm-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "HSSM"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = [
     "Aisulu Omar <aisulu_omar@brown.edu>",
     "Paul Xu <yang_xu@brown.edu>",
     "Alexander Fengler <alexander_fengler@brown.edu>",
     "Michael Frank <michael_frank@brown.edu>",
 ]
@@ -23,27 +23,27 @@
 onnx = "^1.12.0"
 jax = "^0.4.0"
 jaxlib = "^0.4.0"
 ssm-simulators = "^0.3.0"
 huggingface-hub = "^0.15.1"
 onnxruntime = "^1.15.0"
 bambi = "^0.12.0"
+numpyro = "^0.12.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = {extras = ["jupyter"], version = "^23.7.0"}
 mypy = "^1.4.1"
 pre-commit = "^2.20.0"
 jupyterlab = "^4.0.2"
 ipykernel = "^6.16.0"
 hddm-wfpt = { git = "https://github.com/brown-ccv/hddm-wfpt.git" }
 ipywidgets = "^8.0.3"
 graphviz = "^0.20.1"
 ruff = "^0.0.272"
-numpyro = "^0.12.1"
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.17"
 mkdocstrings-python = "^1.1.2"
 mkdocs-jupyter = "^0.24.1"
 
 [tool.black]
 line-length = 88
```

### Comparing `hssm-0.1.2/src/hssm/datasets/cavanagh_theta_nn.csv` & `hssm-0.1.3/src/hssm/datasets/cavanagh_theta_nn.csv`

 * *Files identical despite different names*

### Comparing `hssm-0.1.2/src/hssm/datasets.py` & `hssm-0.1.3/src/hssm/datasets.py`

 * *Files identical despite different names*

### Comparing `hssm-0.1.2/src/hssm/distribution_utils/dist.py` & `hssm-0.1.3/src/hssm/distribution_utils/dist.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,56 +336,60 @@
     Returns
     -------
     Type[pm.Distribution]
         A pymc.Distribution that uses the log-likelihood function.
     """
     random_variable = make_ssm_rv(rv, list_params, lapse) if isinstance(rv, str) else rv
 
-    if lapse is not None and list_params[-1] != "p_outlier":
-        list_params.append("p_outlier")
+    if lapse is not None:
+        if list_params[-1] != "p_outlier":
+            list_params.append("p_outlier")
+
+        data = pt.dvector()
+        lapse_logp = pm.logp(
+            get_distribution_from_prior(lapse).dist(**lapse.args),
+            data,
+        )
+        lapse_func = pytensor.function(
+            [data],
+            lapse_logp,
+        )
 
     class SSMDistribution(pm.Distribution):
         """Wiener first-passage time (WFPT) log-likelihood for LANs."""
 
         # This is just a placeholder because pm.Distribution requires an rv_op
         # Might be updated in the future once
 
         # NOTE: rv_op is an INSTANCE of RandomVariable
         rv_op = random_variable()
         params = list_params
-        _lapse = lapse
 
         @classmethod
         def dist(cls, **kwargs):  # pylint: disable=arguments-renamed
             dist_params = [
                 pt.as_tensor_variable(pm.floatX(kwargs[param])) for param in cls.params
             ]
             other_kwargs = {k: v for k, v in kwargs.items() if k not in cls.params}
             return super().dist(dist_params, **other_kwargs)
 
         def logp(data, *dist_params):  # pylint: disable=E0213
             if list_params[-1] == "p_outlier":
                 p_outlier = dist_params[-1]
                 dist_params = dist_params[:-1]
+                lapse_logp = lapse_func(data[:, 0].eval())
 
-            logp = loglik(data, *dist_params)
-
-            if list_params[-1] == "p_outlier":
-                dist = get_distribution_from_prior(lapse).dist(**lapse.args)
+                logp = loglik(data, *dist_params)
                 logp = pt.log(
                     (1.0 - p_outlier) * pt.exp(logp)
-                    + p_outlier
-                    * pt.exp(
-                        pm.logp(
-                            dist,
-                            data[:, 0],
-                        )
-                    )
+                    + p_outlier * pt.exp(lapse_logp)
                     + 1e-29
                 )
+            else:
+                logp = loglik(data, *dist_params)
 
             if bounds is None:
                 return logp
 
             return apply_param_bounds_to_loglik(
                 logp, list_params, *dist_params, bounds=bounds
             )
@@ -393,15 +397,15 @@
     return SSMDistribution
 
 
 def make_distribution_from_onnx(
     rv: str | Type[RandomVariable],
     list_params: list[str],
     onnx_model: str | PathLike | onnx.ModelProto,
-    backend: str = "pytensor",
+    backend: str = "jax",
     bounds: dict | None = None,
     params_is_reg: list[bool] | None = None,
     lapse: bmb.Prior | None = None,
 ) -> Type[pm.Distribution]:
     """Make a PyMC distribution from an ONNX model.
 
     Produces a PyMC distribution that uses the provided base or ONNX model as
```

### Comparing `hssm-0.1.2/src/hssm/distribution_utils/onnx/onnx.py` & `hssm-0.1.3/src/hssm/distribution_utils/onnx/onnx.py`

 * *Files identical despite different names*

### Comparing `hssm-0.1.2/src/hssm/distribution_utils/onnx/onnx2pt.py` & `hssm-0.1.3/src/hssm/distribution_utils/onnx/onnx2pt.py`

 * *Files identical despite different names*

### Comparing `hssm-0.1.2/src/hssm/distribution_utils/onnx/onnx2xla.py` & `hssm-0.1.3/src/hssm/distribution_utils/onnx/onnx2xla.py`

 * *Files identical despite different names*

### Comparing `hssm-0.1.2/src/hssm/hssm.py` & `hssm-0.1.3/src/hssm/hssm.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,14 +258,20 @@
             else:
                 # For supported models without configs,
                 # We don't require a model_config (because list_params is known)
                 model = cast(SupportedModels, model)
                 self.model_config = {} if model_config is None else model_config
                 self.list_params = default_params[model][:]
 
+        if (
+            loglik_kind == "approx_differentiable"
+            and "backend" not in self.model_config
+        ):
+            self.model_config["backend"] = "jax"
+
         # Logic for determining if p_outlier and lapse is specified correctly.
         # Basically, avoid situations where only one of them is specified.
         self._parent = self.list_params[0]
         if self.has_lapse and lapse is None:
             raise ValueError(
                 "You have specified `p_outlier`. Please also specify `lapse`."
             )
@@ -388,31 +394,20 @@
                 if not Path(self.loglik).exists():
                     self.loglik = download_hf(self.loglik)
 
             self.model_distribution = make_distribution_from_onnx(
                 rv=self.model_config.get("rv", self.model_name),
                 onnx_model=self.loglik,
                 list_params=self.list_params,
-                backend=self.model_config.get("backend", "pytensor"),
+                backend=self.model_config.get("backend", "jax"),
                 params_is_reg=params_is_reg,
                 bounds=self.bounds,
                 lapse=self.lapse,
             )
 
-            # TODO: Fix jax backend
-            if (
-                self.model_config.get("backend", "pytensor") == "jax"
-                and any(params_is_reg)
-                and self.has_lapse
-            ):
-                raise ValueError(
-                    "'jax' backend with regression is not working right now when lapse "
-                    + "distribution is enabled."
-                )
-
         self.family = make_family(
             self.model_distribution,
             self.list_params,
             self.link,
             self._parent,
         )
 
@@ -488,39 +483,50 @@
 
         sorted_params = {k: params[k] for k in self.list_params}
 
         return sorted_params, *_parse_bambi(list(sorted_params.values()))
 
     def sample(
         self,
-        sampler: Literal[
-            "mcmc", "nuts_numpyro", "nuts_blackjax", "laplace", "vi"
-        ] = "mcmc",
+        sampler: Literal["mcmc", "nuts_numpyro", "nuts_blackjax", "laplace", "vi"]
+        | None = None,
         **kwargs,
     ) -> az.InferenceData | pm.Approximation:
         """Perform sampling using the `fit` method via bambi.Model.
 
         Parameters
         ----------
         sampler
-            The sampler to use. Can be either "mcmc" (default), "nuts_numpyro",
+            The sampler to use. Can be one of "mcmc", "nuts_numpyro",
             "nuts_blackjax", "laplace", or "vi". If using `blackbox` likelihoods,
-            this cannot be "nuts_numpyro" or "nuts_blackjax".
+            this cannot be "nuts_numpyro" or "nuts_blackjax". By default it is None, and
+            sampler will automatically be chosen: when the model uses the
+            `approx_differentiable` likelihood, and `jax` backend, "nuts_numpyro" will
+            be used. Otherwise, "mcmc" (the default PyMC NUTS sampler) will be used.
         kwargs
             Other arguments passed to bmb.Model.fit(). Please see [here]
             (https://bambinos.github.io/bambi/api_reference.html#bambi.models.Model.fit)
             for full documentation.
 
         Returns
         -------
         az.InferenceData | pm.Approximation
             An ArviZ `InferenceData` instance if inference_method is `"mcmc"`
             (default), "nuts_numpyro", "nuts_blackjax" or "laplace". An `Approximation`
             object if `"vi"`.
         """
+        if sampler is None:
+            if (
+                self.loglik_kind == "approx_differentiable"
+                and self.model_config.get("backend") == "jax"
+            ):
+                sampler = "nuts_numpyro"
+            else:
+                sampler = "mcmc"
+
         supported_samplers = ["mcmc", "nuts_numpyro", "nuts_blackjax", "laplace", "vi"]
 
         if sampler not in supported_samplers:
             raise ValueError(
                 f"Unsupported sampler '{sampler}', must be one of {supported_samplers}"
             )
 
@@ -529,14 +535,26 @@
                 raise ValueError(
                     f"{sampler} sampler does not work with blackbox likelihoods."
                 )
 
             if "step" not in kwargs:
                 kwargs["step"] = pm.Slice(model=self.pymc_model)
 
+        if (
+            self.loglik_kind == "approx_differentiable"
+            and self.model_config.get("backend") == "jax"
+            and sampler == "mcmc"
+            and kwargs.get("cores", None) != 1
+        ):
+            _logger.warning(
+                "Parallel sampling might not work with `jax` backend and the PyMC NUTS "
+                + "sampler on some platforms. Please consider using `nuts_numpyro` or "
+                + "`nuts_blackjax` sampler if that is a problem."
+            )
+
         self._inference_obj = self.model.fit(inference_method=sampler, **kwargs)
 
         return self.traces
 
     def sample_posterior_predictive(
         self,
         idata: az.InferenceData | None = None,
@@ -737,22 +755,22 @@
                 for _, common_term in component.common_terms.items():
                     output.append(_print_prior(common_term))
                 for _, group_specific_term in component.group_specific_terms.items():
                     output.append(_print_prior(group_specific_term))
                 output.append(f"    Link: {param.link}")
             # None regression case
             else:
-                if param.is_parent:
+                if param.prior is None:
                     prior = (
                         component.intercept_term.prior
-                        if param.prior is None
-                        else param.prior
+                        if param.is_parent
+                        else component.prior
                     )
                 else:
-                    prior = component.prior
+                    prior = param._prior if param.is_truncated else param.prior
                 output.append(f"    Prior: {prior}")
             output.append(f"    Explicit bounds: {param.bounds}")
 
         if self.p_outlier is not None:
             # TODO: Allow regression for self.p_outlier
             # Need to determine what the output should look like
             # and whether p should be hierarchical when self.hierarchical is True.
@@ -841,14 +859,16 @@
         if "prior" not in param or param["prior"] is None:
             if (
                 "default_priors" in model_config
                 and name in model_config["default_priors"]
                 and "formula" not in model_config
             ):
                 prior = model_config["default_priors"][name]
+            else:
+                prior = None
         else:
             prior = param["prior"]
         return Param(
             name=name,
             prior=prior,
             formula=param.get("formula"),
             link=param.get("link"),
```

### Comparing `hssm-0.1.2/src/hssm/likelihoods/analytical.py` & `hssm-0.1.3/src/hssm/likelihoods/analytical.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from typing import Type
 
 import numpy as np
 import pymc as pm
 import pytensor
 import pytensor.tensor as pt
+from numpy import inf
 from pymc.distributions.dist_math import check_parameters
 
 from ..distribution_utils.dist import make_distribution
 
 LOGP_LB = pm.floatX(-66.1)
 
 
@@ -353,20 +354,21 @@
     checked_logp = check_parameters(logp, a >= 0, msg="a >= 0")
     checked_logp = check_parameters(checked_logp, z >= 0, msg="z >= 0")
     checked_logp = check_parameters(checked_logp, z <= 1, msg="z <= 1")
     checked_logp = check_parameters(checked_logp, sv > 0, msg="sv > 0")
     return checked_logp
 
 
-ddm_bounds = {"z": (0.0, 1.0)}
-ddm_sdv_bounds = ddm_bounds | {
-    "v": (-3.0, 3.0),
-    "a": (0.3, 2.5),
-    "t": (0.0, 2.0),
+ddm_bounds = {
+    "v": (-inf, inf),
+    "a": (0.0, inf),
+    "z": (0.0, 1.0),
+    "t": (0.0, inf),
 }
+ddm_sdv_bounds = ddm_bounds | {"sv": (0.0, inf)}
 
 ddm_params = ["v", "a", "z", "t"]
 ddm_sdv_params = ddm_params + ["sv"]
 
 DDM: Type[pm.Distribution] = make_distribution(
     "ddm",
     logp_ddm,
```

### Comparing `hssm-0.1.2/src/hssm/param.py` & `hssm-0.1.3/src/hssm/param.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """The Param utility class."""
 
 from __future__ import annotations
 
 from typing import Any, Callable, Union, cast
 
 import bambi as bmb
+import numpy as np
 import pymc as pm
 from bambi.backend.utils import get_distribution
 
 # PEP604 union operator "|" not supported by pylint
 # Fall back to old syntax
 
 # Explicitly define types so they are more expressive
@@ -65,14 +66,24 @@
     ):
         self.name = name
         self.formula = formula
         self._parent = is_parent
         self.bounds = tuple(float(x) for x in bounds) if bounds is not None else None
         self._is_truncated = False
 
+        if self.bounds is not None:
+            self.bounds = cast(BoundsSpec, self.bounds)
+            if any(not np.isscalar(bound) for bound in self.bounds):
+                raise ValueError(f"The bounds of {self.name} should both be scalar.")
+            lower, upper = self.bounds
+            assert lower < upper, (
+                f"The lower bound of {self.name} should be less than "
+                + "its upper bound."
+            )
+
         if isinstance(prior, int):
             prior = float(prior)
 
         if formula is not None:
             # The regression case
 
             self.formula = formula if "~" in formula else f"{name} ~ {formula}"
@@ -89,33 +100,33 @@
 
             self.link = "identity" if link is None else link
 
         else:
             # The non-regression case
 
             if prior is None:
-                if bounds is None:
+                if self.bounds is None:
                     raise ValueError(
                         f"Please specify the prior or bounds for {self.name}."
                     )
-                self.prior = bmb.Prior(name="Uniform", lower=bounds[0], upper=bounds[1])
+                self.prior = _make_default_prior(self.bounds)
             else:
                 # Explicitly cast the type of prior, no runtime performance penalty
                 prior = cast(ParamSpec, prior)
 
-                if bounds is None:
+                if self.bounds is None:
                     if isinstance(prior, (float, bmb.Prior)):
                         self.prior = prior
                     else:
                         self.prior = bmb.Prior(**prior)
                 else:
                     if isinstance(prior, float):
                         self.prior = prior
                     else:
-                        self.prior = make_bounded_prior(prior, bounds)
+                        self.prior = make_bounded_prior(prior, self.bounds)
                         # self._prior is internally used for informative output
                         # Not used in inference
                         self._prior = (
                             bmb.Prior(**prior) if isinstance(prior, dict) else prior
                         )
                         self._is_truncated = True
 
@@ -419,18 +430,22 @@
                 f"The fixed prior should be between {lower:.4f} and {upper:.4f}, "
                 + f"got {prior:.4f}."
             )
 
         return prior
 
     if isinstance(prior, dict):
+        if np.isinf(lower) and np.isinf(upper):
+            return bmb.Prior(**prior)
         dist = make_truncated_dist(lower, upper, **prior)
         return bmb.Prior(name=prior["name"], dist=dist)
 
     # After handling the constant and dict case, now handle the bmb.Prior case
+    if np.isinf(lower) and np.isinf(upper):
+        return prior
     if prior.dist is not None:
         return prior
 
     name = prior.name
     args = prior.args
 
     dist = make_truncated_dist(lower, upper, name=name, **args)
@@ -464,13 +479,38 @@
     initval = dist_kwargs.pop("initval") if "initval" in dist_kwargs else None
 
     def TruncatedDist(name):
         dist = get_distribution(dist_name).dist(**dist_kwargs)
         return pm.Truncated(
             name=name,
             dist=dist,
-            lower=lower_bound,
-            upper=upper_bound,
+            lower=lower_bound if np.isfinite(lower_bound) else None,
+            upper=upper_bound if np.isfinite(upper_bound) else None,
             initval=initval,
         )
 
     return TruncatedDist
+
+
+def _make_default_prior(bounds: tuple[float, float]) -> bmb.Prior:
+    """Make a default prior from bounds.
+
+    Parameters
+    ----------
+    bounds
+        The (lower, upper) bounds for the default prior.
+
+    Returns
+    -------
+        A bmb.Prior object representing the default prior for the provided bounds.
+    """
+    lower, upper = bounds
+    if np.isinf(lower) and np.isinf(upper):
+        return bmb.Prior("Normal", mu=0.0, sigma=2.0)
+    elif np.isinf(lower) and not np.isinf(upper):
+        return bmb.Prior("TruncatedNormal", mu=upper, upper=upper, sigma=2.0)
+    elif not np.isinf(lower) and np.isinf(upper):
+        if lower == 0:
+            return bmb.Prior("HalfNormal", sigma=2.0)
+        return bmb.Prior("TruncatedNormal", mu=lower, lower=lower, sigma=2.0)
+    else:
+        return bmb.Prior(name="Uniform", lower=lower, upper=upper)
```

### Comparing `hssm-0.1.2/src/hssm/simulator.py` & `hssm-0.1.3/src/hssm/simulator.py`

 * *Files identical despite different names*

### Comparing `hssm-0.1.2/src/hssm/utils.py` & `hssm-0.1.3/src/hssm/utils.py`

 * *Files identical despite different names*

### Comparing `hssm-0.1.2/PKG-INFO` & `hssm-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hssm
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/lnccbrown/HSSM
 License: Copyright 2023, Brown University, Providence, RI.
 Keywords: HSSM,sequential sampling models,bayesian,bayes,mcmc
 Author: Aisulu Omar
 Author-email: aisulu_omar@brown.edu
 Requires-Python: >=3.9,<3.12
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arviz (>=0.14.0,<0.15.0)
 Requires-Dist: bambi (>=0.12.0,<0.13.0)
 Requires-Dist: huggingface-hub (>=0.15.1,<0.16.0)
 Requires-Dist: jax (>=0.4.0,<0.5.0)
 Requires-Dist: jaxlib (>=0.4.0,<0.5.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
+Requires-Dist: numpyro (>=0.12.1,<0.13.0)
 Requires-Dist: onnx (>=1.12.0,<2.0.0)
 Requires-Dist: onnxruntime (>=1.15.0,<2.0.0)
 Requires-Dist: pymc (>=5.6.0,<6.0.0)
 Requires-Dist: scipy (==1.10.1)
 Requires-Dist: ssm-simulators (>=0.3.0,<0.4.0)
 Project-URL: Repository, https://github.com/lnccbrown/HSSM
 Description-Content-Type: text/markdown
@@ -30,26 +31,25 @@
 <div style="position: relative; width: 100%;">
   <img src="docs/images/mainlogo.png" style="width: 250px;">
   <a href="https://ccbs.carney.brown.edu/brainstorm" style="position: absolute; right: 0; top: 50%; transform: translateY(-50%);">
     <img src="docs/images/Brain-Bolt-%2B-Circuits.gif" style="width: 100px;">
   </a>
 </div>
 
-
 ## HSSM - Hierarchical Sequential Sampling Modeling
 
 ![PyPI](https://img.shields.io/pypi/v/hssm)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hssm)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/lnccbrown/HSSM)
 ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/lnccbrown/HSSM/run_tests.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 ### Overview
 
-HSSM is a Python toolbox that provides a seamless combination of state-of-the-art likelihood approximation methods with the wider ecosystem of probabilistic programming languages. It facilitates flexible hierarchical model building and inference via modern MCMC samplers. HSSM is user-friendly and provides the ability to rigorously estimate the impact of neural and other trial-by-trial covariates through parameter-wise mixed-effects models for a large variety of cognitive process models. HSSM is a  <a href="https://ccbs.carney.brown.edu/brainstorm">BRAINSTORM</a> project in collaboration with the Center for Computation and Visualization and the Center for Computational Brain Science within the Carney Institute at Brown University. 
+HSSM is a Python toolbox that provides a seamless combination of state-of-the-art likelihood approximation methods with the wider ecosystem of probabilistic programming languages. It facilitates flexible hierarchical model building and inference via modern MCMC samplers. HSSM is user-friendly and provides the ability to rigorously estimate the impact of neural and other trial-by-trial covariates through parameter-wise mixed-effects models for a large variety of cognitive process models. HSSM is a <a href="https://ccbs.carney.brown.edu/brainstorm">BRAINSTORM</a> project in collaboration with the Center for Computation and Visualization and the Center for Computational Brain Science within the Carney Institute at Brown University.
 
 - Allows approximate hierarchical Bayesian inference via various likelihood approximators.
 - Estimate impact of neural and other trial-by-trial covariates via native hierarchical mixed-regression support.
 - Extensible for users to add novel models with corresponding likelihoods.
 - Built on PyMC with support from the Python Bayesian ecosystem at large.
 - Incorporates Bambi's intuitive `lmer`-like regression parameter specification for within- and between-subject effects.
 - Native ArviZ support for plotting and other convenience functions to aid the Bayesian workflow.
@@ -66,53 +66,20 @@
 ```
 
 You can also install the bleeding edge version of `hssm` directly from this repo:
 
 ```
 pip install git+https://github.com/lnccbrown/HSSM.git
 ```
-**Note**: Possible solutions to any issues with installations with hssm can be located [here](https://github.com/lnccbrown/HSSM/discussions). We recommend leveraging an environment manager with Python 3.9~3.11 to prevent any problems with dependencies during the installation process. Please note that hssm is tested for python 3.9, 3.10, 3.11. Use other python versions with caution. For more detailed guidance, please refer to this [discussion](https://github.com/lnccbrown/HSSM/discussions/152). 
-
-### Optional Installation
-
-**Dependency for graph() Function**
-
-Note: In addition to the installation of the main hssm class, there is an optional dependency for the graph() function. This dependency requires graphviz, which can be installed conveniently using conda with the following command:
-
-```
-conda install -c conda-forge python-graphviz
-```
-
-Alternatively, you have the option to install the graphviz binaries manually and then install the Python bindings using pip with the following command:
-
-```
-pip install graphviz
-```
-
-**Dependency for sampler="nuts_numpyro"**
 
-To utilize the nuts_numpyro sampler, please follow these steps:
+You will need optional dependencies to use JAX-based samplers and graph the models.
+Please refer to our [installation guide](https://lnccbrown.github.io/HSSM/getting_started/installation/)
+for more detailed instructions.
 
-1. Install numpyro by executing the following command:
-
-```
-pip install numpyro
-```
-
-2. Import the necessary modules and configure the required settings:
-
-```
-import numpyro
-from jax.config import config
-
-numpyro.set_host_device_count(jax.local_device_count())
-config.update("jax_enable_x64", False)
-```
-
-For more information please refer to [jax documentation](https://jax.readthedocs.io/en/latest/installation.html).
+**Note**: Possible solutions to any issues with installations with hssm can be located [here](https://github.com/lnccbrown/HSSM/discussions). We recommend leveraging an environment manager with Python 3.9~3.11 to prevent any problems with dependencies during the installation process. Please note that hssm is tested for python 3.9, 3.10, 3.11. Use other python versions with caution.
 
 ## Example
 
 Here is a simple example of how to use HSSM:
 
 ```python
 import hssm
@@ -128,28 +95,31 @@
 model = hssm.HSSM(
     model="ddm",
     data=cav_data,
     include=[
         {
             "name": "v",
             "prior": {
-                "Intercept": {"name": "Uniform", "lower": -3.0, "upper": 3.0},
-                "theta": {"name": "Uniform", "lower": -1.0, "upper": 1.0},
+                "Intercept": {"name": "Normal", "mu": 0.0, "sigma": 0.0},
+                "theta": {"name": "Normal", "mu": 0.0, "sigma": 0.0},
             },
-            "formula": "v ~ (1|subj_idx) + theta",
+            "formula": "v ~ (1|participant_id) + theta",
             "link": "identity",
         },
     ],
 )
 
 # Sample from the posterior for this model
 model.sample()
 ```
 
-## Example
+To quickly get started with HSSM, please follow [this tutorial](https://lnccbrown.github.io/HSSM/getting_started/getting_started/).
+For a deeper dive into HSSM, please follow [our main tutorial](https://lnccbrown.github.io/HSSM/tutorials/main_tutorial/).
+
+## License
 
 HSSM is licensed under [Copyright 2023, Brown University, Providence, RI](LICENSE)
 
 ## Support
 
 For questions, bug reports, or other unexpected issues, please open an issue on the GitHub repository.
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: hssm Version: 0.1.2 Summary: Home-page: https://
+Metadata-Version: 2.1 Name: hssm Version: 0.1.3 Summary: Home-page: https://
 github.com/lnccbrown/HSSM License: Copyright 2023, Brown University,
 Providence, RI. Keywords: HSSM,sequential sampling models,bayesian,bayes,mcmc
 Author: Aisulu Omar Author-email: aisulu_omar@brown.edu Requires-Python:
 >=3.9,<3.12 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: arviz (>=0.14.0,<0.15.0)
 Requires-Dist: bambi (>=0.12.0,<0.13.0) Requires-Dist: huggingface-hub
 (>=0.15.1,<0.16.0) Requires-Dist: jax (>=0.4.0,<0.5.0) Requires-Dist: jaxlib
-(>=0.4.0,<0.5.0) Requires-Dist: numpy (>=1.23.4,<2.0.0) Requires-Dist: onnx
-(>=1.12.0,<2.0.0) Requires-Dist: onnxruntime (>=1.15.0,<2.0.0) Requires-Dist:
-pymc (>=5.6.0,<6.0.0) Requires-Dist: scipy (==1.10.1) Requires-Dist: ssm-
-simulators (>=0.3.0,<0.4.0) Project-URL: Repository, https://github.com/
-lnccbrown/HSSM Description-Content-Type: text/markdown
+(>=0.4.0,<0.5.0) Requires-Dist: numpy (>=1.23.4,<2.0.0) Requires-Dist: numpyro
+(>=0.12.1,<0.13.0) Requires-Dist: onnx (>=1.12.0,<2.0.0) Requires-Dist:
+onnxruntime (>=1.15.0,<2.0.0) Requires-Dist: pymc (>=5.6.0,<6.0.0) Requires-
+Dist: scipy (==1.10.1) Requires-Dist: ssm-simulators (>=0.3.0,<0.4.0) Project-
+URL: Repository, https://github.com/lnccbrown/HSSM Description-Content-Type:
+text/markdown
 [docs/images/mainlogo.png] [docs/images/Brain-Bolt-%2B-Circuits.gif]
 ## HSSM - Hierarchical Sequential Sampling Modeling ![PyPI](https://
 img.shields.io/pypi/v/hssm) ![PyPI - Python Version](https://img.shields.io/
 pypi/pyversions/hssm) ![GitHub pull requests](https://img.shields.io/github/
 issues-pr/lnccbrown/HSSM) ![GitHub Workflow Status (with event)](https://
 img.shields.io/github/actions/workflow/status/lnccbrown/HSSM/run_tests.yml) [!
 [Code style: black](https://img.shields.io/badge/code%20style-black-
@@ -39,50 +40,40 @@
 effects. - Native ArviZ support for plotting and other convenience functions to
 aid the Bayesian workflow. - Utilizes the ONNX format for translation of
 differentiable likelihood approximators across backends. ### Official
 documentation link can be found [here](https://lnccbrown.github.io/HSSM/). ##
 Installation `hssm` is available through PyPI. You can install it with Pip via:
 ``` pip install hssm ``` You can also install the bleeding edge version of
 `hssm` directly from this repo: ``` pip install git+https://github.com/
-lnccbrown/HSSM.git ``` **Note**: Possible solutions to any issues with
-installations with hssm can be located [here](https://github.com/lnccbrown/
-HSSM/discussions). We recommend leveraging an environment manager with Python
-3.9~3.11 to prevent any problems with dependencies during the installation
-process. Please note that hssm is tested for python 3.9, 3.10, 3.11. Use other
-python versions with caution. For more detailed guidance, please refer to this
-[discussion](https://github.com/lnccbrown/HSSM/discussions/152). ### Optional
-Installation **Dependency for graph() Function** Note: In addition to the
-installation of the main hssm class, there is an optional dependency for the
-graph() function. This dependency requires graphviz, which can be installed
-conveniently using conda with the following command: ``` conda install -
-c conda-forge python-graphviz ``` Alternatively, you have the option to install
-the graphviz binaries manually and then install the Python bindings using pip
-with the following command: ``` pip install graphviz ``` **Dependency for
-sampler="nuts_numpyro"** To utilize the nuts_numpyro sampler, please follow
-these steps: 1. Install numpyro by executing the following command: ``` pip
-install numpyro ``` 2. Import the necessary modules and configure the required
-settings: ``` import numpyro from jax.config import config
-numpyro.set_host_device_count(jax.local_device_count()) config.update
-("jax_enable_x64", False) ``` For more information please refer to [jax
-documentation](https://jax.readthedocs.io/en/latest/installation.html). ##
-Example Here is a simple example of how to use HSSM: ```python import hssm #
-Set float type to float32 to avoid a current bug in PyMC # This will not be
-necessary in the future hssm.set_floatX("float32") # Load a package-supplied
-dataset cav_data = hssm.load_data('cavanagh_theta') # Define a basic
-hierarchical model with trial-level covariates model = hssm.HSSM( model="ddm",
-data=cav_data, include=[ { "name": "v", "prior": { "Intercept": {"name":
-"Uniform", "lower": -3.0, "upper": 3.0}, "theta": {"name": "Uniform", "lower":
--1.0, "upper": 1.0}, }, "formula": "v ~ (1|subj_idx) + theta", "link":
+lnccbrown/HSSM.git ``` You will need optional dependencies to use JAX-based
+samplers and graph the models. Please refer to our [installation guide](https:/
+/lnccbrown.github.io/HSSM/getting_started/installation/) for more detailed
+instructions. **Note**: Possible solutions to any issues with installations
+with hssm can be located [here](https://github.com/lnccbrown/HSSM/discussions).
+We recommend leveraging an environment manager with Python 3.9~3.11 to prevent
+any problems with dependencies during the installation process. Please note
+that hssm is tested for python 3.9, 3.10, 3.11. Use other python versions with
+caution. ## Example Here is a simple example of how to use HSSM: ```python
+import hssm # Set float type to float32 to avoid a current bug in PyMC # This
+will not be necessary in the future hssm.set_floatX("float32") # Load a
+package-supplied dataset cav_data = hssm.load_data('cavanagh_theta') # Define a
+basic hierarchical model with trial-level covariates model = hssm.HSSM
+( model="ddm", data=cav_data, include=[ { "name": "v", "prior": { "Intercept":
+{"name": "Normal", "mu": 0.0, "sigma": 0.0}, "theta": {"name": "Normal", "mu":
+0.0, "sigma": 0.0}, }, "formula": "v ~ (1|participant_id) + theta", "link":
 "identity", }, ], ) # Sample from the posterior for this model model.sample()
-``` ## Example HSSM is licensed under [Copyright 2023, Brown University,
-Providence, RI](LICENSE) ## Support For questions, bug reports, or other
-unexpected issues, please open an issue on the GitHub repository. ##
-Contribution If you want to contribute to this project, please familiarize
-yourself with our [contribution guidelines](docs/CONTRIBUTING.md). ##
-Acknowledgements We would like to extend our gratitude to the following
+``` To quickly get started with HSSM, please follow [this tutorial](https://
+lnccbrown.github.io/HSSM/getting_started/getting_started/). For a deeper dive
+into HSSM, please follow [our main tutorial](https://lnccbrown.github.io/HSSM/
+tutorials/main_tutorial/). ## License HSSM is licensed under [Copyright 2023,
+Brown University, Providence, RI](LICENSE) ## Support For questions, bug
+reports, or other unexpected issues, please open an issue on the GitHub
+repository. ## Contribution If you want to contribute to this project, please
+familiarize yourself with our [contribution guidelines](docs/CONTRIBUTING.md).
+## Acknowledgements We would like to extend our gratitude to the following
 individuals for their valuable contributions to the development of the HSSM
 package: - [Bambi](https://github.com/bambinos/bambi) - A special thanks to the
 Bambi project for providing inspiration, guidance, and support throughout the
 development process. [TomÃ¡s Capretto](https://github.com/tomicapretto), a key
 contributor to Bambi, provided invaluable assistance in the development of the
 HSSM package. Those contributions have greatly enhanced the functionality and
 quality of the HSSM.
```

