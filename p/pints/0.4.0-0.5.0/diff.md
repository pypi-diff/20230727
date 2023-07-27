# Comparing `tmp/pints-0.4.0.tar.gz` & `tmp/pints-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pints-0.4.0.tar", last modified: Tue Dec  7 11:00:28 2021, max compression
+gzip compressed data, was "pints-0.5.0.tar", last modified: Thu Jul 27 12:08:11 2023, max compression
```

## Comparing `pints-0.4.0.tar` & `pints-0.5.0.tar`

### file list

```diff
@@ -1,110 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 11:00:28.002136 pints-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1702 2021-12-07 11:00:13.000000 pints-0.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-12-07 11:00:13.000000 pints-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5555 2021-12-07 11:00:28.002136 pints-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5139 2021-12-07 11:00:13.000000 pints-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 11:00:27.994136 pints-0.4.0/pints/
--rw-r--r--   0 runner    (1001) docker     (121)     6287 2021-12-07 11:00:14.000000 pints-0.4.0/pints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5425 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (121)    12043 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     8302 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (121)    11728 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_error_measures.py
--rw-r--r--   0 runner    (1001) docker     (121)    19105 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (121)    36995 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_log_likelihoods.py
--rw-r--r--   0 runner    (1001) docker     (121)    17891 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_log_pdfs.py
--rw-r--r--   0 runner    (1001) docker     (121)    43780 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_log_priors.py
--rw-r--r--   0 runner    (1001) docker     (121)    14688 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 11:00:27.998136 pints-0.4.0/pints/_mcmc/
--rw-r--r--   0 runner    (1001) docker     (121)    43059 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9650 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_adaptive_covariance.py
--rw-r--r--   0 runner    (1001) docker     (121)    11031 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_differential_evolution.py
--rw-r--r--   0 runner    (1001) docker     (121)    10684 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_dram_ac.py
--rw-r--r--   0 runner    (1001) docker     (121)    15147 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_dream.py
--rw-r--r--   0 runner    (1001) docker     (121)     9041 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_dual_averaging.py
--rw-r--r--   0 runner    (1001) docker     (121)     7230 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_emcee_hammer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2467 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_haario_ac.py
--rw-r--r--   0 runner    (1001) docker     (121)     2991 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_haario_bardenet_ac.py
--rw-r--r--   0 runner    (1001) docker     (121)    14376 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (121)     9775 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_mala.py
--rw-r--r--   0 runner    (1001) docker     (121)     5824 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_metropolis.py
--rw-r--r--   0 runner    (1001) docker     (121)    19051 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_monomial_gamma_hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (121)    27040 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_nuts.py
--rw-r--r--   0 runner    (1001) docker     (121)    12654 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_population.py
--rw-r--r--   0 runner    (1001) docker     (121)     3072 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_rao_blackwell_ac.py
--rw-r--r--   0 runner    (1001) docker     (121)    21046 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_relativistic.py
--rw-r--r--   0 runner    (1001) docker     (121)    22390 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_slice_doubling.py
--rw-r--r--   0 runner    (1001) docker     (121)     9679 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_slice_rank_shrinking.py
--rw-r--r--   0 runner    (1001) docker     (121)    26239 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_slice_stepout.py
--rw-r--r--   0 runner    (1001) docker     (121)     6821 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_mcmc/_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 11:00:27.998136 pints-0.4.0/pints/_nested/
--rw-r--r--   0 runner    (1001) docker     (121)    29201 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_nested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13318 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_nested/_ellipsoid.py
--rw-r--r--   0 runner    (1001) docker     (121)     3228 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_nested/_rejection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 11:00:27.998136 pints-0.4.0/pints/_optimisers/
--rw-r--r--   0 runner    (1001) docker     (121)    40884 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_optimisers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7478 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_optimisers/_cmaes.py
--rw-r--r--   0 runner    (1001) docker     (121)    13798 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_optimisers/_cmaes_bare.py
--rw-r--r--   0 runner    (1001) docker     (121)     3324 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_optimisers/_gradient_descent.py
--rw-r--r--   0 runner    (1001) docker     (121)    10121 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_optimisers/_nelder_mead.py
--rw-r--r--   0 runner    (1001) docker     (121)    11155 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_optimisers/_pso.py
--rw-r--r--   0 runner    (1001) docker     (121)     6091 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_optimisers/_snes.py
--rw-r--r--   0 runner    (1001) docker     (121)     6259 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_optimisers/_xnes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4804 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_sample_initial_points.py
--rw-r--r--   0 runner    (1001) docker     (121)    39973 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_transformation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2915 2021-12-07 11:00:14.000000 pints-0.4.0/pints/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 11:00:27.998136 pints-0.4.0/pints/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2021-12-07 11:00:14.000000 pints-0.4.0/pints/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 11:00:27.998136 pints-0.4.0/pints/interfaces/stan/
--rw-r--r--   0 runner    (1001) docker     (121)      318 2021-12-07 11:00:14.000000 pints-0.4.0/pints/interfaces/stan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4440 2021-12-07 11:00:14.000000 pints-0.4.0/pints/interfaces/stan/_stan.py
--rw-r--r--   0 runner    (1001) docker     (121)     3401 2021-12-07 11:00:14.000000 pints-0.4.0/pints/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     9614 2021-12-07 11:00:14.000000 pints-0.4.0/pints/noise.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 11:00:28.002136 pints-0.4.0/pints/plot/
--rw-r--r--   0 runner    (1001) docker     (121)      520 2021-12-07 11:00:14.000000 pints-0.4.0/pints/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2021-12-07 11:00:14.000000 pints-0.4.0/pints/plot/_autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3131 2021-12-07 11:00:14.000000 pints-0.4.0/pints/plot/_function.py
--rw-r--r--   0 runner    (1001) docker     (121)     2548 2021-12-07 11:00:14.000000 pints-0.4.0/pints/plot/_function_between_points.py
--rw-r--r--   0 runner    (1001) docker     (121)     4724 2021-12-07 11:00:14.000000 pints-0.4.0/pints/plot/_histogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     9829 2021-12-07 11:00:14.000000 pints-0.4.0/pints/plot/_pairwise.py
--rw-r--r--   0 runner    (1001) docker     (121)     5445 2021-12-07 11:00:14.000000 pints-0.4.0/pints/plot/_series.py
--rw-r--r--   0 runner    (1001) docker     (121)    12466 2021-12-07 11:00:14.000000 pints-0.4.0/pints/plot/_surface.py
--rw-r--r--   0 runner    (1001) docker     (121)     4577 2021-12-07 11:00:14.000000 pints-0.4.0/pints/plot/_trace.py
--rw-r--r--   0 runner    (1001) docker     (121)    25515 2021-12-07 11:00:14.000000 pints-0.4.0/pints/residuals_diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 11:00:28.002136 pints-0.4.0/pints/toy/
--rw-r--r--   0 runner    (1001) docker     (121)     1695 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6057 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_annulus.py
--rw-r--r--   0 runner    (1001) docker     (121)     8176 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_beeler_reuter_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5002 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_cone.py
--rw-r--r--   0 runner    (1001) docker     (121)     3457 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_constant_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     6015 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_eight_schools.py
--rw-r--r--   0 runner    (1001) docker     (121)     3776 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_fitzhugh_nagumo_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (121)     4298 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_german_credit.py
--rw-r--r--   0 runner    (1001) docker     (121)     5358 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_german_credit_hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (121)     3668 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_goodwin_oscillator_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     6061 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_hes1_michaelis_menten.py
--rw-r--r--   0 runner    (1001) docker     (121)     7773 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_hh_ik_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5501 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_high_dimensional_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (121)     3221 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_logistic_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4341 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_lotka_volterra_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     7866 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_multimodal_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (121)     4496 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_neals_funnel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_parabola.py
--rw-r--r--   0 runner    (1001) docker     (121)     3936 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_repressilator_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3638 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (121)     4333 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_sho_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5353 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_simple_egg_box.py
--rw-r--r--   0 runner    (1001) docker     (121)     4850 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_sir_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     6016 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_stochastic_degradation_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5807 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_stochastic_logistic_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     8025 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_toy_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5778 2021-12-07 11:00:14.000000 pints-0.4.0/pints/toy/_twisted_gaussian_banana.py
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-12-07 11:00:14.000000 pints-0.4.0/pints/version
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 11:00:27.994136 pints-0.4.0/pints.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5555 2021-12-07 11:00:27.000000 pints-0.4.0/pints.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2021-12-07 11:00:27.000000 pints-0.4.0/pints.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-07 11:00:27.000000 pints-0.4.0/pints.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      167 2021-12-07 11:00:27.000000 pints-0.4.0/pints.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-12-07 11:00:27.000000 pints-0.4.0/pints.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-07 11:00:28.002136 pints-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2258 2021-12-07 11:00:14.000000 pints-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:08:11.939796 pints-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-27 12:08:02.000000 pints-0.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 12:08:02.000000 pints-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-27 12:08:11.939796 pints-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-27 12:08:02.000000 pints-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:08:11.931796 pints-0.5.0/pints/
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-27 12:08:02.000000 pints-0.5.0/pints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:08:11.931796 pints-0.5.0/pints/_abc/
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_abc/_abc_rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_abc/_abc_smc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_error_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20654 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44182 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_log_likelihoods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_log_pdfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43780 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_log_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:08:11.931796 pints-0.5.0/pints/_mcmc/
+-rw-r--r--   0 runner    (1001) docker     (123)    45235 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_adaptive_covariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_differential_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_dram_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15146 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_dream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_dual_averaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_emcee_hammer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_haario_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_haario_bardenet_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_mala.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19032 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_monomial_gamma_hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30316 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_rao_blackwell_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21045 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_relativistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22390 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_slice_doubling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_slice_rank_shrinking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26239 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_slice_stepout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_mcmc/_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:08:11.935796 pints-0.5.0/pints/_nested/
+-rw-r--r--   0 runner    (1001) docker     (123)    29185 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_nested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13318 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_nested/_ellipsoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_nested/_rejection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:08:11.935796 pints-0.5.0/pints/_optimisers/
+-rw-r--r--   0 runner    (1001) docker     (123)    44022 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_optimisers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_optimisers/_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_optimisers/_cmaes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_optimisers/_cmaes_bare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_optimisers/_gradient_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_optimisers/_irpropmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_optimisers/_nelder_mead.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_optimisers/_pso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_optimisers/_snes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_optimisers/_xnes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_sample_initial_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43867 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-27 12:08:02.000000 pints-0.5.0/pints/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:08:11.935796 pints-0.5.0/pints/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-27 12:08:02.000000 pints-0.5.0/pints/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:08:11.935796 pints-0.5.0/pints/interfaces/stan/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-27 12:08:02.000000 pints-0.5.0/pints/interfaces/stan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-27 12:08:02.000000 pints-0.5.0/pints/interfaces/stan/_stan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-27 12:08:02.000000 pints-0.5.0/pints/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-07-27 12:08:02.000000 pints-0.5.0/pints/noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:08:11.935796 pints-0.5.0/pints/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-27 12:08:02.000000 pints-0.5.0/pints/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-27 12:08:02.000000 pints-0.5.0/pints/plot/_autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-27 12:08:02.000000 pints-0.5.0/pints/plot/_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-27 12:08:02.000000 pints-0.5.0/pints/plot/_function_between_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-27 12:08:02.000000 pints-0.5.0/pints/plot/_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-07-27 12:08:02.000000 pints-0.5.0/pints/plot/_pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-27 12:08:02.000000 pints-0.5.0/pints/plot/_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-07-27 12:08:02.000000 pints-0.5.0/pints/plot/_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-27 12:08:02.000000 pints-0.5.0/pints/plot/_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-07-27 12:08:02.000000 pints-0.5.0/pints/residuals_diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:08:11.939796 pints-0.5.0/pints/toy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_annulus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_beeler_reuter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_cone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_constant_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_eight_schools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_fitzhugh_nagumo_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_german_credit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_german_credit_hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_goodwin_oscillator_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_hes1_michaelis_menten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_hh_ik_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_high_dimensional_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_logistic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_lotka_volterra_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_multimodal_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_neals_funnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_parabola.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_repressilator_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_sho_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_simple_egg_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_sir_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_toy_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/_twisted_gaussian_banana.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:08:11.939796 pints-0.5.0/pints/toy/stochastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/stochastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/stochastic/_degradation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/stochastic/_logistic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/stochastic/_markov_jump_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/stochastic/_michaelis_menten_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/stochastic/_production_degradation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-27 12:08:02.000000 pints-0.5.0/pints/toy/stochastic/_schlogl_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 12:08:02.000000 pints-0.5.0/pints/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:08:11.931796 pints-0.5.0/pints.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-27 12:08:11.000000 pints-0.5.0/pints.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-27 12:08:11.000000 pints-0.5.0/pints.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:08:11.000000 pints-0.5.0/pints.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 12:08:11.000000 pints-0.5.0/pints.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 12:08:11.000000 pints-0.5.0/pints.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:08:11.939796 pints-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-27 12:08:02.000000 pints-0.5.0/setup.py
```

### Comparing `pints-0.4.0/LICENSE.md` & `pints-0.5.0/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2017-2021, University of Oxford (University of Oxford means the
+Copyright (c) 2017-2023, University of Oxford (University of Oxford means the
 Chancellor, Masters and Scholars of the University of Oxford, having an
 administrative office at Wellington Square, Oxford OX1 2JD, UK).
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
```

### Comparing `pints-0.4.0/PKG-INFO` & `pints-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: pints
-Version: 0.4.0
+Version: 0.5.0
 Summary: Probabilistic Inference in Noisy Time-Series
 Home-page: https://github.com/pints-team/pints
 Maintainer: PINTS Team
 Maintainer-email: pints@maillist.ox.ac.uk
 License: BSD 3-clause license
-Platform: UNKNOWN
-Requires-Python: >=3.5
+Project-URL: Bug Tracker, https://github.com/pints-team/pints/issues
+Project-URL: Documentation, https://pints.readthedocs.io
+Project-URL: Source Code, https://github.com/pints-team/pints
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: stan
 License-File: LICENSE.md
 
-[![Unit tests on multiple python versions](https://github.com/pints-team/pints/workflows/Unit%20tests%20on%20multiple%20python%20versions/badge.svg)](https://github.com/pints-team/pints/actions)
-[![Unit tests on multiple operating systems](https://github.com/pints-team/pints/workflows/Unit%20tests%20on%20multiple%20operating%20systems/badge.svg)](https://github.com/pints-team/pints/actions)
-[![codecov](https://codecov.io/gh/pints-team/pints/branch/master/graph/badge.svg)](https://codecov.io/gh/pints-team/pints)
-[![Functional testing code](https://raw.githubusercontent.com/pints-team/functional-testing/master/badge-code.svg)](https://github.com/pints-team/functional-testing)
-[![Functional testing results](https://raw.githubusercontent.com/pints-team/functional-testing/master/badge-results.svg)](https://www.cs.ox.ac.uk/projects/PINTS/functional-testing)
-[![binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/pints-team/pints/master?filepath=examples)
+[![Unit tests on multiple python versions](https://github.com/pints-team/pints/actions/workflows/unit-test-python-coverage.yml/badge.svg)](https://github.com/pints-team/pints/actions/workflows/unit-test-python-coverage.yml)
+[![Unit tests on multiple operating systems](https://github.com/pints-team/pints/actions/workflows/unit-test-os-coverage.yml/badge.svg)](https://github.com/pints-team/pints/actions/workflows/unit-test-os-coverage.yml)
+[![codecov](https://codecov.io/gh/pints-team/pints/branch/main/graph/badge.svg)](https://codecov.io/gh/pints-team/pints)
+[![Change-point testing code](https://raw.githubusercontent.com/pints-team/change-point-testing/main/badge-code.svg)](https://github.com/pints-team/change-point-testing)
+[![Change-point testing results](https://raw.githubusercontent.com/pints-team/change-point-testing/main/badge-results.svg)](https://www.cs.ox.ac.uk/projects/PINTS/functional-testing)
+[![binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/pints-team/pints/main?filepath=examples)
 [![readthedocs](https://readthedocs.org/projects/pints/badge/?version=latest)](http://pints.readthedocs.io/en/latest/?badge=latest)
-[![BCH compliance](https://bettercodehub.com/edge/badge/pints-team/pints?branch=master)](https://bettercodehub.com/results/pints-team/pints)
 
 # What is Pints?
 
 PINTS (Probabilistic Inference on Noisy Time-Series) is a framework for optimisation and Bayesian inference on ODE models of noisy time-series, such as arise in electrochemistry and cardiac electrophysiology.
 
-PINTS is described in [this publication in JORS](http://doi.org/10.5334/jors.252), and can be cited using the information given in our [CITATION file](https://github.com/pints-team/pints/blob/master/CITATION).
-More information about PINTS papers can be found in the [papers directory](https://github.com/pints-team/pints/tree/master/papers).
+PINTS is described in [this publication in JORS](http://doi.org/10.5334/jors.252), and can be cited using the information given in our [CITATION file](https://github.com/pints-team/pints/blob/main/CITATION).
+More information about PINTS papers can be found in the [papers directory](https://github.com/pints-team/pints/tree/main/papers).
 
 
 ## Using PINTS
 
 PINTS can work with any model that implements the [pints.ForwardModel](http://pints.readthedocs.io/en/latest/core_classes_and_methods.html#forward-model) interface.
 This has just two methods:
 
@@ -40,40 +41,40 @@
 n_parameters() --> Returns the dimension of the parameter space.
 
 simulate(parameters, times) --> Returns a vector of model evaluations at
                                 the given times, using the given parameters
 ```
 
 Experimental data sets in PINTS are defined simply as lists (or arrays) of `times` and corresponding experimental `values`.
-If you have this kind of data, and if [your model (or model wrapper)](https://github.com/pints-team/pints/blob/master/examples/stats/custom-model.ipynb) implements the two methods above, then you are ready to start using PINTS to infer parameter values using [optimisation](https://github.com/pints-team/pints/blob/master/examples/optimisation/first-example.ipynb) or [sampling](https://github.com/pints-team/pints/blob/master/examples/sampling/first-example.ipynb).
+If you have this kind of data, and if [your model (or model wrapper)](https://github.com/pints-team/pints/blob/main/examples/stats/custom-model.ipynb) implements the two methods above, then you are ready to start using PINTS to infer parameter values using [optimisation](https://github.com/pints-team/pints/blob/main/examples/optimisation/first-example.ipynb) or [sampling](https://github.com/pints-team/pints/blob/main/examples/sampling/first-example.ipynb).
 
-A brief example is shown below:  
-![An example of using PINTS in an optimisation](https://raw.githubusercontent.com/pints-team/pints/master/example.svg)  
+A brief example is shown below:
+![An example of using PINTS in an optimisation](https://raw.githubusercontent.com/pints-team/pints/main/example.svg)
 _(Left)_ A noisy experimental time series and a computational forward model.
 _(Right)_ Example code for an optimisation problem.
-The full code can be [viewed here](https://github.com/pints-team/pints/blob/master/examples/sampling/readme-example.ipynb) but a friendlier, more elaborate, introduction can be found on the [examples page](https://github.com/pints-team/pints/blob/master/examples/README.md).
+The full code can be [viewed here](https://github.com/pints-team/pints/blob/main/examples/sampling/readme-example.ipynb) but a friendlier, more elaborate, introduction can be found on the [examples page](https://github.com/pints-team/pints/blob/main/examples/README.md).
 
 A graphical overview of the methods included in PINTS can be [viewed here](https://pints-team.github.io/pints-methods-overview/).
 
 ### Examples and documentation
 
-PINTS comes with a number of [detailed examples](https://github.com/pints-team/pints/blob/master/examples/README.md), hosted here on github.
+PINTS comes with a number of [detailed examples](https://github.com/pints-team/pints/blob/main/examples/README.md), hosted here on github.
 In addition, there is a [full API documentation](http://pints.readthedocs.io/en/latest/), hosted on readthedocs.io.
 
 
 ## Installing PINTS
 
 The latest release of PINTS can be installed without downloading (cloning) the git repository, by opening a console and typing
 
 ```
 $ pip install --upgrade pip
 $ pip install pints
 ```
 
-Note that you'll need Python 3.5 or newer.
+Note that you'll need Python 3.6 or newer.
 
 If you prefer to have the latest cutting-edge version, you can instead install from the repository, by typing
 
 ```
 $ git clone https://github.com/pints-team/pints.git
 $ cd pints
 $ pip install -e .[dev,docs]
@@ -84,27 +85,25 @@
 ```
 $ pip uninstall pints
 ```
 
 
 ## What's new in this version of PINTS?
 
-To see what's changed in the latest release, see the [CHANGELOG](https://github.com/pints-team/pints/blob/master/CHANGELOG.md).
+To see what's changed in the latest release, see the [CHANGELOG](https://github.com/pints-team/pints/blob/main/CHANGELOG.md).
 
 
 ## Contributing to PINTS
 
-If you'd like to help us develop PINTS by adding new methods, writing documentation, or fixing embarassing bugs, please have a look at these [guidelines](https://github.com/pints-team/pints/blob/master/CONTRIBUTING.md) first.
+If you'd like to help us develop PINTS by adding new methods, writing documentation, or fixing embarassing bugs, please have a look at these [guidelines](https://github.com/pints-team/pints/blob/main/CONTRIBUTING.md) first.
 
 
 ## License
 
-PINTS is fully open source. For more information about its license, see [LICENSE](https://github.com/pints-team/pints/blob/master/LICENSE.md).
+PINTS is fully open source. For more information about its license, see [LICENSE](https://github.com/pints-team/pints/blob/main/LICENSE.md).
 
 
 ## Get in touch
 
 Questions, suggestions, or bug reports? [Open an issue](https://github.com/pints-team/pints/issues) and let us know.
 
 Alternatively, feel free to email us at `pints at maillist.ox.ac.uk`.
-
-
```

### Comparing `pints-0.4.0/README.md` & `pints-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-[![Unit tests on multiple python versions](https://github.com/pints-team/pints/workflows/Unit%20tests%20on%20multiple%20python%20versions/badge.svg)](https://github.com/pints-team/pints/actions)
-[![Unit tests on multiple operating systems](https://github.com/pints-team/pints/workflows/Unit%20tests%20on%20multiple%20operating%20systems/badge.svg)](https://github.com/pints-team/pints/actions)
-[![codecov](https://codecov.io/gh/pints-team/pints/branch/master/graph/badge.svg)](https://codecov.io/gh/pints-team/pints)
-[![Functional testing code](https://raw.githubusercontent.com/pints-team/functional-testing/master/badge-code.svg)](https://github.com/pints-team/functional-testing)
-[![Functional testing results](https://raw.githubusercontent.com/pints-team/functional-testing/master/badge-results.svg)](https://www.cs.ox.ac.uk/projects/PINTS/functional-testing)
-[![binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/pints-team/pints/master?filepath=examples)
+[![Unit tests on multiple python versions](https://github.com/pints-team/pints/actions/workflows/unit-test-python-coverage.yml/badge.svg)](https://github.com/pints-team/pints/actions/workflows/unit-test-python-coverage.yml)
+[![Unit tests on multiple operating systems](https://github.com/pints-team/pints/actions/workflows/unit-test-os-coverage.yml/badge.svg)](https://github.com/pints-team/pints/actions/workflows/unit-test-os-coverage.yml)
+[![codecov](https://codecov.io/gh/pints-team/pints/branch/main/graph/badge.svg)](https://codecov.io/gh/pints-team/pints)
+[![Change-point testing code](https://raw.githubusercontent.com/pints-team/change-point-testing/main/badge-code.svg)](https://github.com/pints-team/change-point-testing)
+[![Change-point testing results](https://raw.githubusercontent.com/pints-team/change-point-testing/main/badge-results.svg)](https://www.cs.ox.ac.uk/projects/PINTS/functional-testing)
+[![binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/pints-team/pints/main?filepath=examples)
 [![readthedocs](https://readthedocs.org/projects/pints/badge/?version=latest)](http://pints.readthedocs.io/en/latest/?badge=latest)
-[![BCH compliance](https://bettercodehub.com/edge/badge/pints-team/pints?branch=master)](https://bettercodehub.com/results/pints-team/pints)
 
 # What is Pints?
 
 PINTS (Probabilistic Inference on Noisy Time-Series) is a framework for optimisation and Bayesian inference on ODE models of noisy time-series, such as arise in electrochemistry and cardiac electrophysiology.
 
-PINTS is described in [this publication in JORS](http://doi.org/10.5334/jors.252), and can be cited using the information given in our [CITATION file](https://github.com/pints-team/pints/blob/master/CITATION).
-More information about PINTS papers can be found in the [papers directory](https://github.com/pints-team/pints/tree/master/papers).
+PINTS is described in [this publication in JORS](http://doi.org/10.5334/jors.252), and can be cited using the information given in our [CITATION file](https://github.com/pints-team/pints/blob/main/CITATION).
+More information about PINTS papers can be found in the [papers directory](https://github.com/pints-team/pints/tree/main/papers).
 
 
 ## Using PINTS
 
 PINTS can work with any model that implements the [pints.ForwardModel](http://pints.readthedocs.io/en/latest/core_classes_and_methods.html#forward-model) interface.
 This has just two methods:
 
@@ -24,40 +23,40 @@
 n_parameters() --> Returns the dimension of the parameter space.
 
 simulate(parameters, times) --> Returns a vector of model evaluations at
                                 the given times, using the given parameters
 ```
 
 Experimental data sets in PINTS are defined simply as lists (or arrays) of `times` and corresponding experimental `values`.
-If you have this kind of data, and if [your model (or model wrapper)](https://github.com/pints-team/pints/blob/master/examples/stats/custom-model.ipynb) implements the two methods above, then you are ready to start using PINTS to infer parameter values using [optimisation](https://github.com/pints-team/pints/blob/master/examples/optimisation/first-example.ipynb) or [sampling](https://github.com/pints-team/pints/blob/master/examples/sampling/first-example.ipynb).
+If you have this kind of data, and if [your model (or model wrapper)](https://github.com/pints-team/pints/blob/main/examples/stats/custom-model.ipynb) implements the two methods above, then you are ready to start using PINTS to infer parameter values using [optimisation](https://github.com/pints-team/pints/blob/main/examples/optimisation/first-example.ipynb) or [sampling](https://github.com/pints-team/pints/blob/main/examples/sampling/first-example.ipynb).
 
-A brief example is shown below:  
-![An example of using PINTS in an optimisation](https://raw.githubusercontent.com/pints-team/pints/master/example.svg)  
+A brief example is shown below:
+![An example of using PINTS in an optimisation](https://raw.githubusercontent.com/pints-team/pints/main/example.svg)
 _(Left)_ A noisy experimental time series and a computational forward model.
 _(Right)_ Example code for an optimisation problem.
-The full code can be [viewed here](https://github.com/pints-team/pints/blob/master/examples/sampling/readme-example.ipynb) but a friendlier, more elaborate, introduction can be found on the [examples page](https://github.com/pints-team/pints/blob/master/examples/README.md).
+The full code can be [viewed here](https://github.com/pints-team/pints/blob/main/examples/sampling/readme-example.ipynb) but a friendlier, more elaborate, introduction can be found on the [examples page](https://github.com/pints-team/pints/blob/main/examples/README.md).
 
 A graphical overview of the methods included in PINTS can be [viewed here](https://pints-team.github.io/pints-methods-overview/).
 
 ### Examples and documentation
 
-PINTS comes with a number of [detailed examples](https://github.com/pints-team/pints/blob/master/examples/README.md), hosted here on github.
+PINTS comes with a number of [detailed examples](https://github.com/pints-team/pints/blob/main/examples/README.md), hosted here on github.
 In addition, there is a [full API documentation](http://pints.readthedocs.io/en/latest/), hosted on readthedocs.io.
 
 
 ## Installing PINTS
 
 The latest release of PINTS can be installed without downloading (cloning) the git repository, by opening a console and typing
 
 ```
 $ pip install --upgrade pip
 $ pip install pints
 ```
 
-Note that you'll need Python 3.5 or newer.
+Note that you'll need Python 3.6 or newer.
 
 If you prefer to have the latest cutting-edge version, you can instead install from the repository, by typing
 
 ```
 $ git clone https://github.com/pints-team/pints.git
 $ cd pints
 $ pip install -e .[dev,docs]
@@ -68,25 +67,25 @@
 ```
 $ pip uninstall pints
 ```
 
 
 ## What's new in this version of PINTS?
 
-To see what's changed in the latest release, see the [CHANGELOG](https://github.com/pints-team/pints/blob/master/CHANGELOG.md).
+To see what's changed in the latest release, see the [CHANGELOG](https://github.com/pints-team/pints/blob/main/CHANGELOG.md).
 
 
 ## Contributing to PINTS
 
-If you'd like to help us develop PINTS by adding new methods, writing documentation, or fixing embarassing bugs, please have a look at these [guidelines](https://github.com/pints-team/pints/blob/master/CONTRIBUTING.md) first.
+If you'd like to help us develop PINTS by adding new methods, writing documentation, or fixing embarassing bugs, please have a look at these [guidelines](https://github.com/pints-team/pints/blob/main/CONTRIBUTING.md) first.
 
 
 ## License
 
-PINTS is fully open source. For more information about its license, see [LICENSE](https://github.com/pints-team/pints/blob/master/LICENSE.md).
+PINTS is fully open source. For more information about its license, see [LICENSE](https://github.com/pints-team/pints/blob/main/LICENSE.md).
 
 
 ## Get in touch
 
 Questions, suggestions, or bug reports? [Open an issue](https://github.com/pints-team/pints/issues) and let us know.
 
 Alternatively, feel free to email us at `pints at maillist.ox.ac.uk`.
```

### Comparing `pints-0.4.0/pints/__init__.py` & `pints-0.5.0/pints/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,18 +111,20 @@
 # Log-likelihoods
 #
 from ._log_likelihoods import (
     AR1LogLikelihood,
     ARMA11LogLikelihood,
     CauchyLogLikelihood,
     ConstantAndMultiplicativeGaussianLogLikelihood,
+    GaussianIntegratedLogUniformLogLikelihood,
     GaussianIntegratedUniformLogLikelihood,
     GaussianKnownSigmaLogLikelihood,
     GaussianLogLikelihood,
     KnownNoiseLogLikelihood,
+    LogNormalLogLikelihood,
     MultiplicativeGaussianLogLikelihood,
     ScaledLogLikelihood,
     StudentTLogLikelihood,
     UnknownNoiseLogLikelihood,
 )
 
 #
@@ -152,33 +154,35 @@
 # Parallel function evaluation
 #
 from ._evaluation import (
     evaluate,
     Evaluator,
     ParallelEvaluator,
     SequentialEvaluator,
+    MultiSequentialEvaluator,
 )
 
 
 #
 # Optimisation
 #
 from ._optimisers import (
     curve_fit,
     fmin,
     Optimisation,
     OptimisationController,
     optimise,
     Optimiser,
     PopulationBasedOptimiser,
-    TriangleWaveTransform,
 )
+from ._optimisers._adam import Adam
 from ._optimisers._cmaes import CMAES
 from ._optimisers._cmaes_bare import BareCMAES
 from ._optimisers._gradient_descent import GradientDescent
+from ._optimisers._irpropmin import IRPropMin
 from ._optimisers._nelder_mead import NelderMead
 from ._optimisers._pso import PSO
 from ._optimisers._snes import SNES
 from ._optimisers._xnes import XNES
 
 
 #
@@ -234,18 +238,28 @@
 from ._nested import NestedSampler
 from ._nested import NestedController
 from ._nested._rejection import NestedRejectionSampler
 from ._nested._ellipsoid import NestedEllipsoidSampler
 
 
 #
+# ABC
+#
+from ._abc import ABCSampler
+from ._abc import ABCController
+from ._abc._abc_rejection import RejectionABC
+from ._abc._abc_smc import ABCSMC
+
+
+#
 # Sampling initialising
 #
 from ._sample_initial_points import sample_initial_points
 
+
 #
 # Transformations
 #
 from ._transformation import (
     ComposedTransformation,
     IdentityTransformation,
     LogitTransformation,
@@ -253,19 +267,21 @@
     RectangularBoundariesTransformation,
     ScalingTransformation,
     Transformation,
     TransformedBoundaries,
     TransformedErrorMeasure,
     TransformedLogPDF,
     TransformedLogPrior,
+    TransformedRectangularBoundaries,
+    UnitCubeTransformation,
 )
 
 
 #
 # Noise generators (always import!)
 #
 from . import noise
 
 #
 # Remove any imported modules, so we don't expose them as part of pints
 #
-del(os, sys)
+del os, sys
```

### Comparing `pints-0.4.0/pints/_boundaries.py` & `pints-0.5.0/pints/_boundaries.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     ----------
     log_pdf
         A :class:`pints.LogPdf` to use.
     threshold
         A threshold to determine whether a given log-prior value counts as
         within bounds. Anything _above_ the threshold counts as within bounds.
     """
-    def __init__(self, log_pdf, threshold=-float('inf')):
+    def __init__(self, log_pdf, threshold=-np.inf):
         super(LogPDFBoundaries, self).__init__()
 
         # Check log pdf
         if not isinstance(log_pdf, pints.LogPDF):
             raise ValueError('First argument must be a pints.LogPDF.')
         self._log_pdf = log_pdf
```

### Comparing `pints-0.4.0/pints/_core.py` & `pints-0.5.0/pints/_core.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_diagnostics.py` & `pints-0.5.0/pints/_diagnostics.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_error_measures.py` & `pints-0.5.0/pints/_error_measures.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,17 +95,16 @@
         elif self._n_outputs != len(weights):
             raise ValueError(
                 'Number of weights must match number of problem outputs.')
         # Check weights
         self._weights = np.asarray([float(w) for w in weights])
 
     def __call__(self, x):
-        return np.sum(((np.sum((self._problem.evaluate(x) - self._values)**2,
-                               axis=0) * self._weights) * self._ninv),
-                      axis=0)
+        return self._ninv * np.sum(self._weights * np.sum(
+            (self._problem.evaluate(x) - self._values)**2, axis=0), axis=0)
 
     def evaluateS1(self, x):
         """ See :meth:`ErrorMeasure.evaluateS1()`. """
         y, dy = self._problem.evaluateS1(x)
         dy = dy.reshape((self._n_times, self._n_outputs, self._n_parameters))
         r = y - self._values
         e = self._ninv * np.sum(np.sum(r**2, axis=0) * self._weights, axis=0)
```

### Comparing `pints-0.4.0/pints/_evaluation.py` & `pints-0.5.0/pints/_evaluation.py`

 * *Files 4% similar despite different names*

```diff
@@ -244,15 +244,15 @@
         """
         cleaned = 0
         for k in range(len(self._workers) - 1, -1, -1):
             w = self._workers[k]
             if w.exitcode is not None:  # pragma: no cover
                 w.join()
                 cleaned += 1
-                del(self._workers[k], w)
+                del self._workers[k], w
         if cleaned:     # pragma: no cover
             gc.collect()
         return cleaned
 
     @staticmethod
     def cpu_count():
         """
@@ -409,14 +409,55 @@
         # Free memory
         gc.collect()
 
         # Return errors
         return errors
 
 
+class MultiSequentialEvaluator(Evaluator):
+    """
+    Evaluates a list of functions (or callable objects) for a list of input
+    values of the same length, and returns a list containing the calculated
+    function evaluations.
+
+    This evaluator should be used in the case where each position (for example,
+    corresponding to each chain) needs to be evaluated on a separate function.
+    In this way, it differs from :class:`SequentialEvaluator` and
+    :class:`ParallelEvaluator`, which evaluate multiple positions on a single
+    callable function.
+
+    Extends :class:`Evaluator`.
+
+    Parameters
+    ----------
+    functions : list of callable
+        The functions to evaluate.
+    args : sequence
+        An optional tuple containing extra arguments to each element in
+        functions, ``f``. If ``args`` is specified, ``f`` will be called as
+        ``f(x, *args)``.
+    """
+    def __init__(self, functions, args=None):
+        super(MultiSequentialEvaluator, self).__init__(functions[0], args)
+
+        # Check functions
+        for function in functions:
+            if not callable(function):
+                raise ValueError('The given functions must be callable.')
+        self._functions = functions
+        self._n_functions = len(functions)
+
+    def _evaluate(self, positions):
+        if len(positions) != self._n_functions:
+            raise ValueError('Number of positions does not equal number of '
+                             'functions.')
+
+        return [f(x, *self._args) for f, x in zip(self._functions, positions)]
+
+
 class SequentialEvaluator(Evaluator):
     """
     Evaluates a function (or callable object) for a list of input values, and
     returns a list containing the calculated function evaluations.
 
     Runs sequentially, but shares an interface with the
     :class:`ParallelEvaluator`, allowing parallelism to be switched on/off.
@@ -518,8 +559,7 @@
                     # Check for errors in other workers
                     if self._error.is_set():
                         return
 
         except (Exception, KeyboardInterrupt, SystemExit):
             self._errors.put((self.pid, traceback.format_exc()))
             self._error.set()
-
```

### Comparing `pints-0.4.0/pints/_log_likelihoods.py` & `pints-0.5.0/pints/_log_likelihoods.py`

 * *Files 7% similar despite different names*

```diff
@@ -461,55 +461,138 @@
         # Collect partial derivatives
         dL = np.hstack((dtheta, dsigma_base, deta, dsigma_rel))
 
         # Return
         return L, dL
 
 
+class GaussianIntegratedLogUniformLogLikelihood(pints.ProblemLogLikelihood):
+    r"""
+    Calculates a log-likelihood assuming independent Gaussian-distributed noise
+    at each time point where :math:`p(\sigma)\propto 1/\sigma` has been
+    integrated out of the joint posterior of :math:`p(\theta,\sigma|X)`,
+
+    .. math::
+        \begin{align} p(\theta|X) &= \int_{0}^{\infty} p(\theta, \sigma|X)
+        \mathrm{d}\sigma\\
+        &\propto \int_{0}^{\infty} p(X|\theta, \sigma) p(\theta, \sigma)
+        \mathrm{d}\sigma.\end{align}
+
+    Note that this is exactly the same statistical model as
+    :class:`pints.GaussianLogLikelihood` with a uniform prior on
+    :math:`\sigma` in the logarithmic transformed space.
+    This is also known as Jeffrey's prior, as the standard deviation is a scale
+    parameter, as discussed here: https://doi.org/10.1093/gji/ggaa168.
+
+    A possible advantage of this log-likelihood compared with using a
+    :class:`pints.GaussianLogLikelihood`, is that it has one fewer parameters
+    (:math:`sigma`) which may speed up convergence to the posterior
+    distribution, especially for multi-output problems which will have
+    ``n_outputs`` fewer parameter dimensions.
+
+    The log-likelihood is given in terms of the sum of squared errors:
+
+    .. math::
+        SSE = \sum_{i=1}^n (f_i(\theta) - y_i)^2,
+
+    and is given up to a normalisation constant by:
+
+    .. math::
+        \begin{align}
+        \text{log} L =
+            & - n / 2 \text{log}(SSE) \\
+            & - (n - 2) / 2 \text{log}(2) \\
+            & + \text{log}\left[\Gamma(n / 2)\right],
+        \end{align}
+
+    where :math:`\Gamma(a)` is the incomplete gamma function.
+
+    This log-likelihood is inherently a Bayesian method since it assumes a
+    uniform prior on :math:`\sigma` _in the logarithmic transformed space.
+    However using this likelihood in optimisation routines should yield the
+    same estimates as the full :class:`pints.GaussianLogLikelihood`.
+
+    Extends :class:`ProblemLogLikelihood`.
+
+    Parameters
+    ----------
+    problem
+        A :class:`SingleOutputProblem` or :class:`MultiOutputProblem`.
+    """
+
+    def __init__(self, problem):
+        super(GaussianIntegratedLogUniformLogLikelihood,
+              self).__init__(problem)
+
+        # Get number of times, number of outputs
+        self._nt = len(self._times)
+        self._no = problem.n_outputs()
+
+        # Add parameters to problem
+        self._n_parameters = problem.n_parameters()
+
+        # Pre-calculate
+        n = self._nt
+        self._n_over_2 = n / 2
+        self._log_gamma = scipy.special.gammaln(self._n_over_2)
+        self._constant_1 = -np.log(2) * (n - 2) / 2
+        self._constant = self._constant_1 + self._log_gamma
+
+    def __call__(self, x):
+        error = self._values - self._problem.evaluate(x)
+        sse = np.sum(error**2, axis=0)
+
+        # Calculate
+        sse = pints.vector(sse)
+        return np.sum(self._constant - self._n_over_2 * np.log(sse))
+
+
 class GaussianIntegratedUniformLogLikelihood(pints.ProblemLogLikelihood):
     r"""
     Calculates a log-likelihood assuming independent Gaussian-distributed noise
     at each time point where :math:`\sigma\sim U(a,b)` has been integrated out
-    of the joint posterior of :math:`p(\theta,\sigma|X)`,
+    of the joint posterior of :math:`p(\theta,\sigma|X)` in the same way as in
+    :class:`pints.GaussianIntegratedLogUniformLogLikelihood`,
 
     .. math::
         \begin{align} p(\theta|X) &= \int_{0}^{\infty} p(\theta, \sigma|X)
         \mathrm{d}\sigma\\
         &\propto \int_{0}^{\infty} p(X|\theta, \sigma) p(\theta, \sigma)
-        \mathrm{d}\sigma,\end{align}
+        \mathrm{d}\sigma.\end{align}
 
     Note that this is exactly the same statistical model as
     :class:`pints.GaussianLogLikelihood` with a uniform prior on
     :math:`\sigma`.
 
-    A possible advantage of this log-likelihood compared with using a
+    Similar to :class:`pints.GaussianIntegratedLogUniformLogLikelihood`, a
+    possible advantage of this log-likelihood compared with using a
     :class:`pints.GaussianLogLikelihood`, is that it has one fewer parameters
     (:math:`sigma`) which may speed up convergence to the posterior
     distribution, especially for multi-output problems which will have
     ``n_outputs`` fewer parameter dimensions.
 
     The log-likelihood is given in terms of the sum of squared errors:
 
     .. math::
-        SSE = \sum_{i=1}^n (f_i(\theta) - y_i)^2
+        SSE = \sum_{i=1}^n (f_i(\theta) - y_i)^2,
 
     and is given up to a normalisation constant by:
 
     .. math::
         \begin{align}
         \text{log} L =
             & - n / 2 \text{log}(\pi) \\
             & - \text{log}(2 (b - a) \sqrt(2)) \\
             & + (1 / 2 - n / 2) \text{log}(SSE) \\
             & + \text{log}\left[\Gamma((n - 1) / 2, \frac{SSE}{2 b^2}) -
-                \Gamma((n - 1) / 2, \frac{SSE}{2 a^2}) \right]
+                \Gamma((n - 1) / 2, \frac{SSE}{2 a^2}) \right],
         \end{align}
 
     where :math:`\Gamma(u,v)` is the upper incomplete gamma function as defined
-    here: https://en.wikipedia.org/wiki/Incomplete_gamma_function
+    here: https://en.wikipedia.org/wiki/Incomplete_gamma_function.
 
     This log-likelihood is inherently a Bayesian method since it assumes a
     uniform prior on :math:`\sigma\sim U(a,b)`. However using this likelihood
     in optimisation routines should yield the same estimates as the full
     :class:`pints.GaussianLogLikelihood`.
 
     Extends :class:`ProblemLogLikelihood`.
@@ -786,14 +869,131 @@
         import warnings
         warnings.warn(
             'The class `pints.KnownNoiseLogLikelihood` is deprecated.'
             ' Please use `pints.GaussianKnownSigmaLogLikelihood` instead.')
         super(KnownNoiseLogLikelihood, self).__init__(problem, sigma)
 
 
+class LogNormalLogLikelihood(pints.ProblemLogLikelihood):
+    r"""
+    Calculates a log-likelihood assuming independent log-normal noise at each
+    time point, and adds a parameter representing the standard deviation
+    (sigma) of the noise on the log scale for each output.
+
+    Specifically, the sampling distribution takes the form:
+
+    .. math::
+        y(t) \sim \text{log-Normal}(\log f(\theta, t), \sigma)
+
+    which can alternatively be written:
+
+    .. math::
+        \log y(t) \sim \text{Normal}(\log f(\theta, t), \sigma)
+
+    Important to note is that:
+
+    .. math::
+        \mathbb{E}(y(t)) = f(\theta, t) \exp(\sigma^2 / 2)
+
+    As such, the optional parameter `mean_adjust` (if true) adjusts the mean of
+    the distribution so that its expectation is :math:`f(\theta, t)`. This
+    shifted distribution is of the form:
+
+    .. math::
+        y(t) \sim \text{log-Normal}(\log f(\theta, t) - \sigma^2/2, \sigma)
+
+    Extends :class:`ProblemLogLikelihood`.
+
+    Parameters
+    ----------
+    problem
+        A :class:`SingleOutputProblem` or :class:`MultiOutputProblem`. For a
+        single-output problem a single parameter is added, for a multi-output
+        problem ``n_outputs`` parameters are added.
+    mean_adjust
+        A Boolean. Adjusts the distribution so that its mean corresponds to the
+        function value. By default, this parameter if False.
+    """
+
+    def __init__(self, problem, mean_adjust=False):
+        super(LogNormalLogLikelihood, self).__init__(problem)
+
+        # Get number of times, number of outputs
+        self._nt = len(self._times)
+        self._no = problem.n_outputs()
+
+        # Add parameters to problem
+        self._n_parameters = problem.n_parameters() + self._no
+
+        # Pre-calculate parts
+        self._logn = 0.5 * self._nt * np.log(2 * np.pi)
+
+        # For a log-normal sampling distribution any data points being below
+        # zero would mean that the log-likelihood is always -infinity
+        vals = np.asarray(self._values)
+        if np.any(vals <= 0):
+            raise ValueError('All data points must exceed zero.')
+        self._log_values = np.log(self._values)
+
+        self._mean_adjust = mean_adjust
+
+    def __call__(self, x):
+        sigma = np.asarray(x[-self._no:])
+        if any(sigma < 0):
+            return -np.inf
+
+        soln = self._problem.evaluate(x[:-self._no])
+        if np.any(soln < 0):
+            return -np.inf
+
+        error = np.log(self._values) - np.log(soln)
+        if self._mean_adjust:
+            error += 0.5 * sigma**2
+        return np.sum(- self._logn - self._nt * np.log(sigma)
+                      - np.sum(self._log_values, axis=0)
+                      - np.sum(error**2, axis=0) / (2 * sigma**2))
+
+    def evaluateS1(self, x):
+        """ See :meth:`LogPDF.evaluateS1()`. """
+        # Calculate log-likelihood and when log-prob is infinite, gradients are
+        # not defined
+        L = self.__call__(x)
+        if L == -np.inf:
+            return L, np.tile(np.nan, self._n_parameters)
+
+        sigma = np.asarray(x[-self._no:])
+
+        # Evaluate, and get residuals
+        y, dy = self._problem.evaluateS1(x[:-self._no])
+
+        # Reshape dy, in case we're working with a single-output problem
+        dy = dy.reshape(self._nt, self._no, self._n_parameters - self._no)
+
+        # Note: Must be (np.log(data) - simulation), sign matters now since it
+        # must match that of the partial derivative below
+        error = np.log(self._values) - np.log(y)
+        if self._mean_adjust:
+            error += 0.5 * sigma**2
+
+        # Calculate derivatives in the model parameters
+        dL = np.sum(
+            (sigma**(-2.0) * np.sum((error.T * dy.T / y.T).T, axis=0).T).T,
+            axis=0)
+
+        # Calculate derivative wrt sigma
+        dsigma = -self._nt / sigma + sigma**(-3.0) * np.sum(error**2, axis=0)
+        if self._mean_adjust:
+            dsigma -= 1 / sigma * np.sum(error, axis=0)
+
+        dL = np.concatenate((dL, np.array(list(dsigma))))
+
+        # Return
+        return L, dL
+
+
 class MultiplicativeGaussianLogLikelihood(pints.ProblemLogLikelihood):
     r"""
     Calculates the log-likelihood for a time-series model assuming a
     heteroscedastic Gaussian error of the model predictions
     :math:`f(t, \theta )`.
 
     This likelihood introduces two new scalar parameters for each dimension of
@@ -1010,10 +1210,10 @@
     Deprecated alias of :class:`GaussianLogLikelihood`
     """
 
     def __init__(self, problem):
         # Deprecated on 2019-02-06
         import warnings
         warnings.warn(
-            'The class `pints.KnownNoiseLogLikelihood` is deprecated.'
+            'The class `pints.UnknownNoiseLogLikelihood` is deprecated.'
             ' Please use `pints.GaussianLogLikelihood` instead.')
         super(UnknownNoiseLogLikelihood, self).__init__(problem)
```

### Comparing `pints-0.4.0/pints/_log_pdfs.py` & `pints-0.5.0/pints/_log_pdfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         self._pooled = np.asarray(pooled)
         if len(self._pooled) != n_parameters:
             raise ValueError(
                 'The array-like input `pooled` needs to have the same length '
                 'as the number of parameters of the individual log-pdfs.')
 
         # Check that pooled contains only booleans
-        if self._pooled.dtype != np.bool:
+        if self._pooled.dtype != np.dtype('bool'):
             raise ValueError(
                 'The array-like input `pooled` passed to PooledLogPDFs '
                 'has to contain booleans exclusively.')
 
         # Get dimension of search space
         self._n_pooled = np.sum(self._pooled)
         n_individuals = len(self._log_pdfs)
@@ -371,15 +371,15 @@
                 'Given log_prior and log_likelihood must have same dimension.')
 
         # Store prior and likelihood
         self._log_prior = log_prior
         self._log_likelihood = log_likelihood
 
         # Store -inf, for later use
-        self._minf = -float('inf')
+        self._minf = -np.inf
 
     def __call__(self, x):
         # Evaluate log-prior first, assuming this is very cheap
         log_prior = self._log_prior(x)
         if log_prior == self._minf:
             return self._minf
         return log_prior + self._log_likelihood(x)
```

### Comparing `pints-0.4.0/pints/_log_priors.py` & `pints-0.5.0/pints/_log_priors.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_logger.py` & `pints-0.5.0/pints/_logger.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_mcmc/__init__.py` & `pints-0.5.0/pints/_mcmc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,15 +270,18 @@
     chains and/or evaluations generated by :meth:`run()` to a file, use
     :meth:`set_chain_filename()` and :meth:`set_log_pdf_filename()`.
 
     Parameters
     ----------
     log_pdf : pints.LogPDF
         A :class:`LogPDF` function that evaluates points in the parameter
-        space.
+        space, or a list of :class:`LogPDF` of the same length as `chains`. If
+        multiple LogPDFs are provided, each chain will call only its
+        corresponding LogPDF. Note that if multiple LogPDFs are provided,
+        parallel running is not possible.
     chains : int
         The number of MCMC chains to generate.
     x0
         A sequence of starting points. Can be a list of lists, a 2-dimensional
         array, or any other structure such that ``x0[i]`` is the starting point
         for chain ``i``.
     sigma0
@@ -297,32 +300,61 @@
         :class:`HaarioBardenetACMC` is used.
     """
 
     def __init__(
             self, log_pdf, chains, x0, sigma0=None, transformation=None,
             method=None):
 
-        # Check function
-        if not isinstance(log_pdf, pints.LogPDF):
-            raise ValueError('Given function must extend pints.LogPDF')
+        if isinstance(log_pdf, pints.LogPDF):
+            self._multi_logpdf = False
+
+        else:
+            self._multi_logpdf = True
+            try:
+                if len(log_pdf) != chains:
+                    raise ValueError(
+                        '`log_pdf` must either extend pints.LogPDF, '
+                        'or be a list of objects which extend '
+                        'pints.LogPDF of the same length as `chains`')
+            except TypeError:
+                raise TypeError('`log_pdf` must either extend pints.LogPDF, '
+                                'or be a list of objects which extend '
+                                'pints.LogPDF')
+
+            first_n_params = log_pdf[0].n_parameters()
+            for pdf in log_pdf:
+                # Check function
+                if not isinstance(pdf, pints.LogPDF):
+                    raise ValueError('Elements of `log_pdf` must extend '
+                                     'pints.LogPDF')
+                if pdf.n_parameters() != first_n_params:
+                    raise ValueError('All log_pdfs must have the same number '
+                                     'of parameters.')
 
         # Apply a transformation (if given). From this point onward the MCMC
         # sampler will see only the transformed search space and will know
         # nothing about the model parameter space.
         if transformation is not None:
             # Convert log pdf
-            log_pdf = transformation.convert_log_pdf(log_pdf)
+            if self._multi_logpdf:
+                log_pdf = [transformation.convert_log_pdf(pdf)
+                           for pdf in log_pdf]
+            else:
+                log_pdf = transformation.convert_log_pdf(log_pdf)
 
             # Convert initial positions
             x0 = [transformation.to_search(x) for x in x0]
 
             # Convert sigma0, if provided
             if sigma0 is not None:
                 sigma0 = np.asarray(sigma0)
-                n_parameters = log_pdf.n_parameters()
+                if not self._multi_logpdf:
+                    n_parameters = log_pdf.n_parameters()
+                else:
+                    n_parameters = log_pdf[0].n_parameters()
                 # Make sure sigma0 is a (covariance) matrix
                 if np.product(sigma0.shape) == n_parameters:
                     # Convert from 1d array
                     sigma0 = sigma0.reshape((n_parameters,))
                     sigma0 = np.diag(sigma0)
                 elif sigma0.shape != (n_parameters, n_parameters):
                     # Check if 2d matrix of correct size
@@ -337,15 +369,18 @@
         # screen should be detransformed first!
         self._transformation = transformation
 
         # Store function
         self._log_pdf = log_pdf
 
         # Get number of parameters
-        self._n_parameters = self._log_pdf.n_parameters()
+        if not self._multi_logpdf:
+            self._n_parameters = self._log_pdf.n_parameters()
+        else:
+            self._n_parameters = self._log_pdf[0].n_parameters()
 
         # Check number of chains
         self._n_chains = int(chains)
         if self._n_chains < 1:
             raise ValueError('Number of chains must be at least 1.')
 
         # Check initial position(s): Most checking is done by samplers!
@@ -524,23 +559,32 @@
         # Iteration and evaluation counting
         iteration = 0
         self._n_evaluations = 0
 
         # Choose method to evaluate
         f = self._log_pdf
         if self._needs_sensitivities:
-            f = f.evaluateS1
+            if not self._multi_logpdf:
+                f = f.evaluateS1
+            else:
+                f = [pdf.evaluateS1 for pdf in f]
 
         # Create evaluator object
         if self._parallel:
-            # Use at most n_workers workers
-            n_workers = min(self._n_workers, self._n_chains)
-            evaluator = pints.ParallelEvaluator(f, n_workers=n_workers)
+            if not self._multi_logpdf:
+                # Use at most n_workers workers
+                n_workers = min(self._n_workers, self._n_chains)
+                evaluator = pints.ParallelEvaluator(f, n_workers=n_workers)
+            else:
+                raise ValueError('Cannot run multiple logpdfs in parallel')
         else:
-            evaluator = pints.SequentialEvaluator(f)
+            if not self._multi_logpdf:
+                evaluator = pints.SequentialEvaluator(f)
+            else:
+                evaluator = pints.MultiSequentialEvaluator(f)
 
         # Initial phase
         if self._needs_initial_phase:
             for sampler in self._samplers:
                 sampler.set_initial_phase(True)
 
         # Storing evaluations to memory or disk
@@ -1037,14 +1081,17 @@
 
         If ``parallel=True``, the method will run using a number of worker
         processes equal to the detected cpu core count. The number of workers
         can be set explicitly by setting ``parallel`` to an integer greater
         than 0.
         Parallelisation can be disabled by setting ``parallel`` to ``0`` or
         ``False``.
+
+        Parallel evaluation is only supported when a single LogPDF has been
+        provided to the MCMC controller.
         """
         if parallel is True:
             self._parallel = True
             self._n_workers = pints.ParallelEvaluator.cpu_count()
         elif parallel >= 1:
             self._parallel = True
             self._n_workers = int(parallel)
```

### Comparing `pints-0.4.0/pints/_mcmc/_adaptive_covariance.py` & `pints-0.5.0/pints/_mcmc/_adaptive_covariance.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_mcmc/_differential_evolution.py` & `pints-0.5.0/pints/_mcmc/_differential_evolution.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_mcmc/_dram_ac.py` & `pints-0.5.0/pints/_mcmc/_dram_ac.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 #
 # This file is part of PINTS (https://github.com/pints-team/pints/) which is
 # released under the BSD 3-clause license. See accompanying LICENSE.md for
 # copyright notice and full license details.
 #
 import pints
 import numpy as np
-import scipy.stats as stats
 
 
 class DramACMC(pints.AdaptiveCovarianceMC):
     """
     DRAM (Delayed Rejection Adaptive Covariance) MCMC, as described in [1]_.
 
     In this method, rejections do not necessarily lead an iteration to end.
     Instead, if a rejection occurs, another point is proposed although
     typically from a narrower (i.e. more conservative) proposal kernel than was
     used for the first proposal.
 
+    The number of proposal kernels is fixed to 2.
+
     In this approach, in each iteration, the following steps return the next
-    state of the Markov chain (assuming the current state is ``theta_0`` and
-    that there are 2 proposal kernels)::
+    state of the Markov chain (assuming the current state is ``theta_0``)::
 
         theta_1 ~ N(theta_0, lambda * scale_1 * sigma)
         alpha_1(theta_0, theta_1) = min(1, p(theta_1|X) / p(theta_0|X))
         u_1 ~ uniform(0, 1)
         if alpha_1(theta_0, theta_1) > u_1:
             return theta_1
         theta_2 ~ N(theta_0, lambda * scale_2 * sigma0)
@@ -34,183 +34,120 @@
                    (p(theta_0|X) (1 - alpha_1(theta_0, theta_1))))
         u_2 ~ uniform(0, 1)
         if alpha_2(theta_0, theta_1, theta_2) > u_2:
             return theta_2
         else:
             return theta_0
 
-    Our implementation also allows more than 2 proposal kernels to be used.
-    This means that ``k`` accept-reject steps are taken. In each step (``i``),
-    the probability that a proposal ``theta_i`` is accepted is::
-
-        alpha_i(theta_0, theta_1, ..., theta_i) = min(1, p(theta_i|X) /
-                                                  p(theta_0|X) * n_i / d_i)
-
-    where::
-
-        n_i = (1 - alpha_1(theta_i, theta_i-1)) *
-              (1 - alpha_2(theta_i, theta_i-1, theta_i-2)) *
-               ...
-              (1 - alpha_i-1(theta_i, theta_i-1, ..., theta_0))
-        d_i = (1 - alpha_1(theta_0, theta_1)) *
-              (1 - alpha_2(theta_0, theta_1, theta_2)) *
-              ...
-              (1 - alpha_i-1(theta_0, theta_1, ..., theta_i-1))
-
-    If ``k`` proposals have been rejected, the initial point ``theta_0`` is
-    returned.
-
     At the end of each iterations, a 'base' proposal kernel is adapted::
 
         mu = (1 - gamma) mu + gamma theta
         sigma = (1 - gamma) sigma + gamma (theta - mu)(theta - mu)^t
         log_lambda = log_lambda + gamma (accepted - target_acceptance_rate)
 
     where ``gamma = adaptations^-eta``, ``theta`` is the current state of
     the Markov chain and ``accepted`` is a binary indicator for whether any of
-    the series of proposals were accepted. The kernels for the all proposals
-    are then adapted as ``[scale_1, scale_2, ..., scale_k] * sigma``, where the
+    the series of proposals were accepted. The kernels for the two proposals
+    are then adapted as ``[scale_1, scale_2] * sigma``, where the
     scale factors are set using ``set_sigma_scale``.
 
     *Extends:* :class:`GlobalAdaptiveCovarianceMC`
 
     References
     ----------
     .. [1] "DRAM: Efficient adaptive MCMC".
            H Haario, M Laine, A Mira, E Saksman, (2006) Statistical Computing
            https://doi.org/10.1007/s11222-006-9438-0
     """
     def __init__(self, x0, sigma0=None):
         super(DramACMC, self).__init__(x0, sigma0)
 
-        self._adapt_kernel = True
-        self._before_kernels_set = True
         self._log_lambda = 0
-        self._n_kernels = 2
+        self._n_kernels = 2  # This is fixed!
         self._proposal_count = 0
         self._sigma_base = np.copy(self._sigma)
-        self._upper_scale = 1000
-        self._Y = [None] * self._n_kernels
         self._Y_log_pdf = np.zeros(self._n_kernels)
+        self.set_sigma_scale([1, 0.01])  # scale used in [1]_ for experiments
 
     def _adapt_sigma(self):
         """
-        Updates the covariance matrices of the various kernels being used
-        according to adaptive Metropolis routine.
+        Updates the covariance matrices of the two kernels being used according
+        to adaptive Metropolis routine.
         """
         dsigm = np.reshape(self._current - self._mu, (self._n_parameters, 1))
         self._sigma_base = ((1 - self._gamma) * self._sigma_base +
                             self._gamma * np.dot(dsigm, dsigm.T))
         self._sigma = [self._sigma_scale[i] * self._sigma_base
                        for i in range(self._n_kernels)]
 
-    def _calculate_alpha_log(self, n, Y, log_Y):
+    def _alpha_1_log(self, fx, fy1):
         """
-        Calculates alpha expression necessary in eq. 3 of Haario et al. for
-        determining accept/reject
+        Calculates probability of acceptance in stage 1 of DRAM (eq. 1 in
+        [1]_).
         """
-        alpha_log = log_Y[n + 1] - log_Y[0]
-        if n == 0:
-            return min(0, alpha_log)
-        Y_rev = Y[::-1]
-        log_Y_rev = log_Y[::-1]
-        for i in range(n):
-            alpha_log += (
-                stats.multivariate_normal.logpdf(
-                    x=Y[n - i - 1],
-                    mean=Y[n + 1],
-                    cov=self._sigma[n],
-                    allow_singular=True) -
-                stats.multivariate_normal.logpdf(
-                    x=Y[i],
-                    mean=self._current,
-                    cov=self._sigma[0],
-                    allow_singular=True) +
-                np.log(1 - np.exp(self._calculate_alpha_log(
-                    i, Y_rev[0:(i + 2)], log_Y_rev[0:(i + 2)]))) -
-                np.log(1 - np.exp(self._calculate_alpha_log(
-                    i, Y[0:(i + 2)], log_Y[0:(i + 2)])))
-            )
+        alpha_log = fy1 - fx
         return min(0, alpha_log)
 
-    def _calculate_r_log(self, fx):
+    def _alpha_2_log(self, fx, fy1, fy2):
         """
-        Calculates value of logged acceptance ratio (eq. 3 in [1]_).
+        Calculates probability of acceptance in stage 1 of DRAM (eq. 2 in
+        [1]_).
         """
-        c = self._proposal_count
-        temp_Y = np.concatenate([[self._current], self._Y[0:(c + 1)]])
-        temp_log_Y = np.concatenate(
-            [[self._current_log_pdf], self._Y_log_pdf[0:(c + 1)]])
-        self._r_log = self._calculate_alpha_log(c, temp_Y, temp_log_Y)
+        alpha_log = (fy2 - fx +
+                     np.log1p(np.exp(self._alpha_1_log(fy2, fy1))) -
+                     np.log1p(np.exp(self._alpha_1_log(fx, fy1))))
+        return min(0, alpha_log)
 
     def _generate_proposal(self):
         """ See :meth:`AdaptiveCovarianceMC._generate_proposal()`. """
-        if self._before_kernels_set:
-            self.set_sigma_scale()
-            self._Y = [None] * self._n_kernels
-            self._Y_log_pdf = np.zeros(self._n_kernels)
-            self._before_kernels_set = False
-
         proposed = np.random.multivariate_normal(
             self._current, np.exp(self._log_lambda) *
             self._sigma[self._proposal_count])
-        self._Y[self._proposal_count] = proposed
         return proposed
 
     def name(self):
         """ See :meth:`pints.MCMCSampler.name()`. """
         return 'Delayed Rejection Adaptive Metropolis (Dram) MCMC'
 
-    def n_kernels(self):
-        """ Returns number of proposal kernels. """
-        return self._n_kernels
-
     def n_hyper_parameters(self):
         """ See :meth:`TunableMethod.n_hyper_parameters()`. """
         return 3
 
+    def _r_log(self):
+        """
+        Calculates value of logged acceptance ratio (eq. 3 in [1]_).
+        """
+        if self._proposal_count == 0:
+            r_log = self._alpha_1_log(
+                self._current_log_pdf, self._Y_log_pdf[0])
+        else:
+            r_log = self._alpha_2_log(
+                self._current_log_pdf, self._Y_log_pdf[0], self._Y_log_pdf[1])
+        return r_log
+
     def set_hyper_parameters(self, x):
         """
-        The hyper-parameter vector is ``[eta, n_kernels, upper_scale]``.
+        The hyper-parameter vector is ``[eta, sigma_scale_1, sigma_scale_2]``.
 
         See :meth:`TunableMethod.set_hyper_parameters()`.
         """
         self.set_eta(x[0])
-        self.set_n_kernels(x[1])
-        self.set_upper_scale(x[2])
+        self.set_sigma_scale(x[1:3])
 
-    def set_n_kernels(self, n_kernels):
-        """ Sets number of proposal kernels. """
-        if n_kernels < 1:
-            raise ValueError('Number of proposal kernels must be equal to ' +
-                             'or greater than 1.')
-        self._n_kernels = int(n_kernels)
-
-    def set_upper_scale(self, upper_scale):
-        """
-        Set the upper scale of initial covariance matrix multipliers for each
-        of the kernels: ``[0,...,upper]`` where the gradations are uniform on
-        the log10 scale meaning the proposal covariance matrices are:
-        ``[10^upper,..., 1] * sigma``.
-        """
-        if upper_scale < 0:
-            raise ValueError('Upper scale must be positive.')
-        self._upper_scale = upper_scale
-
-    def set_sigma_scale(self):
-        """
-        Set the scale of initial covariance matrix multipliers for each of the
-        kernels: ``[0,...,upper]`` where the gradations are uniform on the
-        log10 scale meaning the proposal covariance matrices are:
-        ``[10^upper,..., 1] * sigma``.
-        """
-        a_min = np.log10(1)
-        a_max = np.log10(self._upper_scale)
-        self._sigma_scale = 10**np.linspace(a_min, a_max, self._n_kernels)
-        self._sigma_scale = self._sigma_scale[::-1]
+    def set_sigma_scale(self, scales):
+        """
+        Set the scale of the mulipliers for the two proposal kernel
+        covariance matrices. Must be of the form ``[scale_1, scale_2]``.
+        """
+        if len(scales) != 2:
+            raise ValueError('Scales must be of length 2.')
+        for scale in scales:
+            if scale <= 0:
+                raise ValueError('Scales must be positive.')
+        self._sigma_scale = [scales[0], scales[1]]
         self._sigma = [self._sigma_scale[i] * self._sigma_base
                        for i in range(self._n_kernels)]
 
     def sigma_scale(self):
         """
         Returns scale factors used to multiply a base covariance matrix,
         resulting in proposal matrices for each accept-reject step.
@@ -222,67 +159,57 @@
         If first proposal, then accept with ordinary Metropolis probability; if
         a later proposal, use probability determined by [1]_.
         """
         # Check if we had a proposal
         if self._proposed is None:
             raise RuntimeError('Tell called before proposal was set.')
 
+        if self._proposal_count == 0:
+            self._iterations += 1
+
         # Ensure fx is a float
         fx = float(fx)
         self._Y_log_pdf[self._proposal_count] = fx
 
         # First point?
         if self._current is None:
             if not np.isfinite(fx):
                 raise ValueError(
                     'Initial point for MCMC must have finite logpdf.')
 
-            # Accept
             self._current = self._proposed
             self._current_log_pdf = fx
-
-            # Increase iteration count
-            self._iterations += 1
-
-            # Clear proposal
             self._proposed = None
 
             # Return first point for chain
             return self._current, self._current_log_pdf, True
 
         # Check if the proposed point can be accepted
-        accepted = 0
-
+        accept = 0
         if np.isfinite(fx):
-            self._calculate_r_log(fx)
+            r_log = self._r_log()
             u = np.log(np.random.uniform(0, 1))
-            if u < self._r_log:
-                accepted = 1
+            if u < r_log:
+                accept = 1
+                self._acceptance_count += 1
                 self._current = self._proposed
                 self._current_log_pdf = fx
-
+                self._proposal_count = 0
+                self._Y_log_pdf = np.zeros(self._n_kernels)
         self._proposed = None
 
-        if accepted == 0:
-            # rejected proposal
-            if self._n_kernels > 1 and (
-               self._proposal_count < (self._n_kernels - 1)):
+        if accept == 0:
+            if self._proposal_count < (self._n_kernels - 1):
                 self._proposal_count += 1
                 return None
             else:
                 self._proposal_count = 0
-        self._gamma = (self._adaptations**-self._eta)
-        self._adaptations += 1
 
         # Update mu, covariance matrix and log lambda
+        self._acceptance_rate = self._acceptance_count / self._iterations
+        self._gamma = self._adaptations**-self._eta
+        self._adaptations += 1
         self._adapt_mu()
         self._adapt_sigma()
         self._log_lambda += (self._gamma *
-                             (accepted - self._target_acceptance))
-        return self._current, self._current_log_pdf, accepted != 0
-
-    def upper_scale(self):
-        """
-        Returns upper scale limit (see
-        :meth:`pints.DramACMC.set_upper_scale()`).
-        """
-        return self._upper_scale
+                             (accept - self._target_acceptance))
+        return self._current, self._current_log_pdf, accept != 0
```

### Comparing `pints-0.4.0/pints/_mcmc/_dream.py` & `pints-0.5.0/pints/_mcmc/_dream.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
         return self._delta_max
 
     def _draw(self, i):
         """
         Select 2 random chains, not including chain i.
         """
         r1, r2 = np.random.choice(self._n_chains, 2, replace=False)
-        while(r1 == i or r2 == i or r1 == r2):
+        while r1 == i or r2 == i or r1 == r2:
             r1, r2 = np.random.choice(self._n_chains, 2, replace=False)
         return r1, r2
 
     def n_hyper_parameters(self):
         """ See :meth:`TunableMethod.n_hyper_parameters()`. """
         return 8
```

### Comparing `pints-0.4.0/pints/_mcmc/_dual_averaging.py` & `pints-0.5.0/pints/_mcmc/_dual_averaging.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         self._t0 = 10.0
         self._kappa = 0.75
 
         # variables for dual averaging
         self._epsilon = init_epsilon    # The adapted step size
         self._mass_matrix = None        # The adapted mass matrix (set below)
         self._inv_mass_matrix = None    # The inverse adapted mass matrix
+        self._use_dense_mass_matrix = None
 
         self._mu = np.log(10 * self._epsilon)
         self._log_epsilon_bar = np.log(1)
         self._h_bar = 0.0
         self._adapt_epsilon_counter = 0
 
         self.set_inv_mass_matrix(np.copy(init_inv_mass_matrix))
@@ -203,21 +204,23 @@
     def set_inv_mass_matrix(self, inv_mass_matrix):
         """
         We calculate the mass matrix whenever the inverse mass matrix is set.
         """
         if inv_mass_matrix.ndim == 1:
             self._mass_matrix = 1.0 / inv_mass_matrix
             self._inv_mass_matrix = inv_mass_matrix
+            self._use_dense_mass_matrix = False
         else:
             try:
                 self._mass_matrix = np.linalg.inv(inv_mass_matrix)
             except np.linalg.LinAlgError:
                 print('WARNING: adapted mass matrix is ill-conditioned')
                 return
             self._inv_mass_matrix = inv_mass_matrix
+            self._use_dense_mass_matrix = True
 
     def step(self, x, accept_prob):
         """
         Perform a single step of the adaption.
 
         Parameters
         ----------
@@ -253,7 +256,26 @@
                     self._warmup_steps - self._terminal_window
                 )
             self.init_sample_covariance(self._next_window - self._counter)
             return True
             #self._epsilon = self.final_epsilon()
 
         return False
+
+    def target_accept_prob(self):
+        """
+        Returns the target acceptance probability.
+        """
+        return self._target_accept_prob
+
+    def use_dense_mass_matrix(self):
+        """
+        Returns a boolean flag whether the adaption algorithm uses a dense
+        (``True``) or a diagonal (``False``) mass matrix.
+        """
+        return self._use_dense_mass_matrix
+
+    def warmup_steps(self):
+        """
+        Returns the number of warm up iterations.
+        """
+        return self._warmup_steps
```

### Comparing `pints-0.4.0/pints/_mcmc/_emcee_hammer.py` & `pints-0.5.0/pints/_mcmc/_emcee_hammer.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_mcmc/_haario_ac.py` & `pints-0.5.0/pints/_mcmc/_haario_ac.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_mcmc/_haario_bardenet_ac.py` & `pints-0.5.0/pints/_mcmc/_haario_bardenet_ac.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_mcmc/_hamiltonian.py` & `pints-0.5.0/pints/_mcmc/_hamiltonian.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,15 @@
 
         # Unpack reply
         energy, gradient = reply
 
         # Check reply, copy gradient
         energy = float(energy)
         gradient = pints.vector(gradient)
-        assert(gradient.shape == (self._n_parameters, ))
+        assert gradient.shape == (self._n_parameters, )
 
         # Energy = -log_pdf, so flip both signs!
         energy = -energy
         gradient = -gradient
 
         # Very first call
         if self._current is None:
```

### Comparing `pints-0.4.0/pints/_mcmc/_mala.py` & `pints-0.5.0/pints/_mcmc/_mala.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
 
         # Unpack reply
         fx, log_gradient = reply
 
         # Check reply, copy gradient
         fx = float(fx)
         log_gradient = pints.vector(log_gradient)
-        assert(log_gradient.shape == (self._n_parameters, ))
+        assert log_gradient.shape == (self._n_parameters, )
 
         # First point?
         if self._current is None:
             if not np.isfinite(fx):
                 raise ValueError(
                     'Initial point for MCMC must have finite log_pdf.')
```

### Comparing `pints-0.4.0/pints/_mcmc/_metropolis.py` & `pints-0.5.0/pints/_mcmc/_metropolis.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_mcmc/_monomial_gamma_hamiltonian.py` & `pints-0.5.0/pints/_mcmc/_monomial_gamma_hamiltonian.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         return self._c
 
     def _cdf(self, p, a, c, m, z):
         """
         Auxillary kinetic energy cumulative density defined in [1]_.
         """
         return integrate.quad(lambda p1: self._pdf(p1, a, c, m, z),
-                              -float('Inf'), p)[0]
+                              -np.inf, p)[0]
 
     def divergent_iterations(self):
         """
         Returns the iteration number of any divergent iterations.
         """
         return self._divergent
 
@@ -219,15 +219,15 @@
     def _initialise_ke(self):
         """
         Initialises functions needed for sampling from soft kinetic energy
         function defined in [1]_.
         """
         z = integrate.quad(
             lambda p: np.exp(-self._K_indiv(p, self._a, self._c, self._m)),
-            -float('Inf'), float('Inf'))[0]
+            -np.inf, np.inf)[0]
         self._f = self._inverse_cdf_calculator(self._a, self._c,
                                                self._m, z)
 
     def _inverse_cdf_calculator(self, a, c, m, z, pmax=100):
         """
         Estimates empirical cdf.
         """
@@ -425,15 +425,15 @@
 
         # Unpack reply
         energy, gradient = reply
 
         # Check reply, copy gradient
         energy = float(energy)
         gradient = pints.vector(gradient)
-        assert(gradient.shape == (self._n_parameters, ))
+        assert gradient.shape == (self._n_parameters, )
 
         # Energy = -log_pdf, so flip both signs!
         energy = -energy
         gradient = -gradient
 
         # Very first call
         if self._current is None:
```

### Comparing `pints-0.4.0/pints/_mcmc/_nuts.py` & `pints-0.5.0/pints/_mcmc/_nuts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #
 # No-U-Turn Sampler (NUTS) MCMC method
 #
 # This file is part of PINTS (https://github.com/pints-team/pints/) which is
 # released under the BSD 3-clause license. See accompanying LICENSE.md for
 # copyright notice and full license details.
 #
-import asyncio
+import _pickle as cPickle
+
 import pints
 import numpy as np
 
 
 class NutsState(object):
     """
     Class to hold information about the current state of the NUTS hamiltonian
@@ -151,15 +152,14 @@
         # for non-root merges accumulate tree weightings before probability
         # calculation
         if not root:
             self.n = np.logaddexp(self.n, other_state.n)
 
         # accept a new point based on the weighting of the two trees
         p = min(1, np.exp(other_state.n - self.n))
-
         if p > 0.0 and np.random.uniform() < p:
             self.theta = other_state.theta
             self.L = other_state.L
             self.grad_L = other_state.grad_L
 
         # for root merges accumulate tree weightings after probability
         # calculation
@@ -202,15 +202,14 @@
         return 0.5 * np.inner(r, inv_mass_matrix.dot(r))
 
 # All the functions below are written as coroutines to enable the recursive
 # nuts algorithm to be written using the ask-and-tell interface used by PINTS,
 # see main coroutine function ``nuts_sampler`` for more details
 
 
-@asyncio.coroutine
 def leapfrog(theta, L, grad_L, r, epsilon, inv_mass_matrix):
     """
     performs a leapfrog step using a step_size ``epsilon`` and an inverse mass
     matrix ``inv_mass_matrix``.
 
     The inverse mass matrix can be a 2 dimensional ndarray, in which case it is
     interpreted as a dense matrix, or a 1 dimensional ndarray, in which case it
@@ -222,15 +221,14 @@
     else:
         theta_new = theta + epsilon * inv_mass_matrix.dot(r_new)
     L_new, grad_L_new = (yield theta_new)
     r_new += 0.5 * epsilon * grad_L_new
     return L_new, grad_L_new, theta_new, r_new
 
 
-@asyncio.coroutine
 def build_tree(state, v, j, adaptor, hamiltonian0, hamiltonian_threshold):
     """
     Implicitly build up a subtree of depth ``j`` for the NUTS sampler.
     """
     if j == 0:
         # Base case - take one leapfrog in the direction v
         if v == -1:
@@ -243,28 +241,28 @@
             r = state.r_plus
             L = state.L_plus
             grad_L = state.grad_L_plus
 
         L_dash, grad_L_dash, theta_dash, r_dash = \
             yield from leapfrog(theta, L, grad_L, r, v * adaptor.get_epsilon(),
                                 adaptor.get_inv_mass_matrix())
+
         hamiltonian_dash = L_dash \
             - kinetic_energy(r_dash, adaptor.get_inv_mass_matrix())
 
         if np.isnan(hamiltonian_dash):
-            comparison = float('-inf')
+            comparison = -np.inf
         else:
             comparison = hamiltonian_dash - hamiltonian0
         n_dash = comparison
         alpha_dash = min(1.0, np.exp(comparison))
-
         divergent = -comparison > hamiltonian_threshold
         s_dash = int(not divergent)
-
         n_alpha_dash = 1
+
         return NutsState(
             theta_dash, r_dash, L_dash, grad_L_dash, n_dash, s_dash,
             alpha_dash, n_alpha_dash, divergent,
             adaptor.get_inv_mass_matrix()
         )
 
     else:
@@ -278,15 +276,46 @@
                 build_tree(state_dash, v, j - 1, adaptor, hamiltonian0,
                            hamiltonian_threshold)
             state_dash.update(state_double_dash, direction=v, root=False)
 
         return state_dash
 
 
-@asyncio.coroutine
+def initialise_adaptor(
+        theta, L, grad_L, num_adaption_steps, delta, sigma0,
+        use_dense_mass_matrix):
+    """
+    Creates a generator that terminates by returning an instance of the
+    pints.DualAveragingAdaption.
+
+    Initialisation of the adaptor requires a 'reasonable' epsilon which
+    is in turn also a generator. The find_reasonable_epsilon generator
+    terminates with return of a 'reasonable' epsilon. Intermediate returns
+    are the current position of the leapfrog integrator.
+    """
+
+    # pick the initial inverse mass matrix as the provided sigma0.
+    # reduce to a diagonal matrix if not using a dense mass matrix
+    if use_dense_mass_matrix:
+        init_inv_mass_matrix = sigma0
+        init_inv_mass_matrix = 1e-3 * np.eye(len(theta))
+    else:
+        init_inv_mass_matrix = np.diag(sigma0)
+        init_inv_mass_matrix = 1e-3 * np.ones(len(theta))
+
+    # find a good value to start epsilon at (this will later be refined so that
+    # the acceptance probability matches delta)
+    epsilon = yield from find_reasonable_epsilon(
+        theta, L, grad_L, init_inv_mass_matrix)
+
+    # create adaption for epsilon and mass matrix
+    return pints.DualAveragingAdaption(
+        num_adaption_steps, delta, epsilon, init_inv_mass_matrix)
+
+
 def find_reasonable_epsilon(theta, L, grad_L, inv_mass_matrix):
     """
     Pick a reasonable value of epsilon close to when the acceptance
     probability of the Langevin proposal crosses 0.5. This is based on
     Algorithm 4 in [1]_ (with scaled mass matrix as per section 4.2).
 
     Note: inv_mass_matrix can be a 1-d ndarray and in this case is interpreted
@@ -308,38 +337,36 @@
             np.linalg.inv(inv_mass_matrix)
         )
     hamiltonian = L - kinetic_energy(r, inv_mass_matrix)
     L_dash, grad_L_dash, theta_dash, r_dash = \
         yield from leapfrog(theta, L, grad_L, r, epsilon, inv_mass_matrix)
     hamiltonian_dash = L_dash - kinetic_energy(r_dash, inv_mass_matrix)
     if np.isnan(hamiltonian_dash):
-        comparison = float('-inf')
+        comparison = -np.inf
     else:
         comparison = hamiltonian_dash - hamiltonian
 
     # determine whether we are doubling or halving
     alpha = 2 * int(comparison > np.log(0.5)) - 1
 
     # double or half epsilon until acceptance probability crosses 0.5
     while comparison * alpha > np.log(2) * (-alpha):
         epsilon = 2**alpha * epsilon
         L_dash, grad_L_dash, theta_dash, r_dash = \
             yield from leapfrog(theta, L, grad_L, r, epsilon, inv_mass_matrix)
         hamiltonian_dash = L_dash - kinetic_energy(r_dash, inv_mass_matrix)
         if np.isnan(hamiltonian_dash):  # pragma: no cover
-            comparison = float('-inf')
+            comparison = -np.inf
         else:
             comparison = hamiltonian_dash - hamiltonian
     return epsilon
 
 
-@asyncio.coroutine
-def nuts_sampler(x0, delta, num_adaption_steps, sigma0,
-                 hamiltonian_threshold, max_tree_depth,
-                 use_dense_mass_matrix):
+def nuts_sampler(
+        x0, adaptor, sigma0, hamiltonian_threshold, max_tree_depth):
     """
     The dual averaging NUTS mcmc sampler given in Algorithm 6 of [1]_.
     Implements the multinomial sampling suggested in [2]_. Implements a mass
     matrix for the dynamics, which is detailed in [2]_. Both the step size and
     the mass matrix is adapted using a combination of the dual averaging
     detailed in [1]_ and the windowed adaption for the mass matrix and step
     size implemented in the Stan library (https://github.com/stan-dev/stan)
@@ -348,28 +375,23 @@
     evaluate (L, L') at. Users must send (L, L') back to the coroutine to
     continue execution. The end of an mcmc step is signalled by generating a
     tuple of values (theta, L, acceptance probability, number of leapfrog
     steps)
 
     Arguments
     ---------
-
     x0: ndarray
         starting point
-    delta: float
-        target acceptance probability (Dual Averaging scheme)
-    num_adaption_steps: int
-        number of adaption steps (Dual Averaging scheme)
+    adaptor: list or pints.DualAveragingAdaption
+        list with properties of the averaging algorithm [num_adaption_steps,
+        delta, use_dense_mass_matrix] or instance of averaging algorithm.
     hamiltonian_threshold: float
         threshold to test divergent iterations
     max_tree_depth: int
         maximum tree depth
-    use_dense_mass_matrix: bool
-        if False, use a diagonal mass matrix, if True use a fully dense mass
-        matrix
 
     References
     ----------
     .. [1] Hoffman, M. D., & Gelman, A. (2014). The No-U-Turn sampler:
            adaptively setting path lengths in Hamiltonian Monte Carlo.
            Journal of Machine Learning Research, 15(1), 1593-1623.
 
@@ -382,39 +404,28 @@
     L, grad_L = (yield theta)
 
     # Check first point is somewhere sensible
     if not np.isfinite(L):
         raise ValueError(
             'Initial point for MCMC must have finite logpdf.')
 
-    # pick the initial inverse mass matrix as the provided sigma0.
-    # reduce to a diagonal matrix if not using a dense mass matrix
-    if use_dense_mass_matrix:
-        init_inv_mass_matrix = sigma0
-        init_inv_mass_matrix = 1e-3 * np.eye(len(x0))
-    else:
-        init_inv_mass_matrix = np.diag(sigma0)
-        init_inv_mass_matrix = 1e-3 * np.ones(len(x0))
-
-    # find a good value to start epsilon at (this will later be refined so that
-    # the acceptance probability matches delta)
-    epsilon = yield from find_reasonable_epsilon(theta, L, grad_L,
-                                                 init_inv_mass_matrix)
-
-    # create adaption for epsilon and mass matrix
-    adaptor = pints.DualAveragingAdaption(
-        num_adaption_steps, delta, epsilon, init_inv_mass_matrix)
-
-    # start at iteration 1
-    m = 1
+    # If adaptor is not yet created, initialise it with the provided
+    # properties.
+    if isinstance(adaptor, list):
+        # Adaptor does currently not exist and is only specified by a list
+        # of properties.
+        num_adaption_steps, delta, use_dense_mass_matrix = adaptor
+        adaptor = yield from initialise_adaptor(
+            theta, L, grad_L, num_adaption_steps, delta, sigma0,
+            use_dense_mass_matrix)
 
     # provide an infinite generator of mcmc steps....
     while True:
         # randomly sample momentum
-        if use_dense_mass_matrix:
+        if adaptor.use_dense_mass_matrix():
             r0 = np.random.multivariate_normal(
                 np.zeros(len(theta)), adaptor.get_mass_matrix())
         else:
             r0 = np.random.normal(np.zeros(len(theta)),
                                   np.sqrt(adaptor.get_mass_matrix()))
 
         hamiltonian0 = L - kinetic_energy(r0, adaptor.get_inv_mass_matrix())
@@ -424,27 +435,25 @@
                           n=0.0, s=1, alpha=1, n_alpha=1, divergent=False,
                           inv_mass_matrix=adaptor.get_inv_mass_matrix())
         j = 0
 
         # build up an integration path with 2^j points, stopping when we either
         # encounter a U-Turn, or reach a max number of points 2^max_tree_depth
         while j < max_tree_depth and state.s == 1:
-
             # pick a random direction to integrate in
             # (to maintain detailed balance)
             if np.random.randint(0, 2):
                 vj = 1
             else:
                 vj = -1
 
             # recursivly build up tree in that direction
             state_dash = yield from \
                 build_tree(state, vj, j, adaptor,
                            hamiltonian0, hamiltonian_threshold)
-
             state.update(state_dash, direction=vj, root=True)
 
             j += 1
 
         # update current position in chain
         theta = state.theta
         L = state.L
@@ -462,18 +471,16 @@
         # signal calling process that mcmc step is complete by passing a tuple
         # (rather than an ndarray)
         yield (theta,
                L,
                grad_L,
                state.alpha / state.n_alpha,
                state.n_alpha,
-               state.divergent)
-
-        # next step
-        m += 1
+               state.divergent,
+               adaptor)
 
 
 class NoUTurnMCMC(pints.SingleChainMCMC):
     r"""
 
     Implements the No U-Turn Sampler (NUTS) with dual averaging, as described
     in Algorithm 6 in [1]_.
@@ -505,26 +512,28 @@
 
     """
 
     def __init__(self, x0, sigma0=None):
         super(NoUTurnMCMC, self).__init__(x0, sigma0)
 
         # hyperparameters
-        self._num_adaption_steps = 500
-        self._delta = 0.8
-        self._step_size = None
+        self._adaptor = [
+            500,           # Number of adaption steps
+            0.8,           # Target acceptance ratio (delta)
+            False,         # Uses dense mass matrix
+        ]
         self._max_tree_depth = 10
-        self._use_dense_mass_matrix = False
 
         # Default threshold for Hamiltonian divergences
         # (currently set to match Stan)
         self._hamiltonian_threshold = 10**3
 
         # coroutine nuts sampler
         self._nuts = None
+        self._nuts_state = None
 
         # number of mcmc iterations
         self._mcmc_iteration = 0
 
         # Logging
         self._last_log_write = 0
         self._mcmc_acceptance = 0
@@ -548,32 +557,35 @@
         """ See :meth:`SingleChainMCMC.ask()`. """
         # Check ask/tell pattern
         if self._ready_for_tell:
             raise RuntimeError('Ask() called when expecting call to tell().')
 
         # Initialise on first call
         if not self._running:
-            self._nuts = nuts_sampler(self._x0, self._delta,
-                                      self._num_adaption_steps,
-                                      self._sigma0,
-                                      self._hamiltonian_threshold,
-                                      self._max_tree_depth,
-                                      self._use_dense_mass_matrix)
+            self._nuts = nuts_sampler(
+                self._x0, self._adaptor, self._sigma0,
+                self._hamiltonian_threshold, self._max_tree_depth)
+
             # coroutine will ask for self._x0
             self._next = next(self._nuts)
             self._running = True
 
         self._ready_for_tell = True
         return np.array(self._next, copy=True)
 
     def delta(self):
         """
         Returns delta used in leapfrog algorithm.
         """
-        return self._delta
+        try:
+            # When adaptor has not been initialised
+            return self._adaptor[1]
+        except TypeError:
+            # Adaptor has been initialised
+            return self._adaptor.target_accept_prob()
 
     def divergent_iterations(self):
         """
         Returns the iteration number of any divergent iterations.
         """
         return self._divergent
 
@@ -598,14 +610,47 @@
         else:
             logger.log(self._mcmc_acceptance)
             logger.log(self._n_leapfrog)
         self._mcmc_acceptance = 0
         self._n_leapfrog = 0
         self._last_log_write = self._mcmc_iteration
 
+    def load_state(self, file):
+        """
+        Loads sampler state from a .pickle file and returns sampler.
+
+        Arguments
+        ---------
+        file: str
+            Path to file.
+        """
+        with open(file, "rb") as input_file:
+            method = cPickle.load(input_file)
+
+        # Recreate NUTS sampler state
+        method._nuts = nuts_sampler(
+            method._current, method._adaptor, method._sigma0,
+            method._hamiltonian_threshold, method._max_tree_depth)
+
+        # NOTE: This nuts_sampler still differs from before pickling, because
+        # before returning the mcmc proposal the nuts sampler starts the next
+        # leapfrog trajectory by sampling a new momentum and using the
+        # current gradient information to perform the first leapfrog step. We
+        # can't do this here, because we don't have the gradient information
+        # anymore.
+        # BUT we can prepare the ask method such that it returns the current
+        # position, such that after one more ask-tell cycle we have caught up
+        # with the sampler before pickling. Since this ask-tell cycle does not
+        # return anything to the user, this effectively reconstructs the
+        # sampler state. The momentum will however be resampled, which is ok
+        # since it's the start of a new trajectory.
+        method._next = next(method._nuts)
+
+        return method
+
     def max_tree_depth(self):
         """
         Returns the maximum tree depth ``D`` for the algorithm. For each
         iteration, the number of leapfrog steps will not be greater than
         ``2^D``.
         """
         return self._max_tree_depth
@@ -622,27 +667,51 @@
         """ See :meth:`pints.MCMCSampler.needs_sensitivities()`. """
         return True
 
     def number_adaption_steps(self):
         """
         Returns number of adaption steps used in the NUTS algorithm.
         """
-        return self._num_adaption_steps
+        try:
+            # When adaptor has not been initialised
+            return self._adaptor[0]
+        except TypeError:
+            # Adaptor has been initialised
+            return self._adaptor.warmup_steps()
+
+    def save_state(self, file):
+        """
+        Saves sampler state to pickle file.
+
+        Arguments
+        ---------
+        file: str
+            Path to file.
+        """
+        # Remove nuts_sampler generator
+        nuts = self._nuts
+        self._nuts = None
+        with open(file, "wb") as output_file:
+            cPickle.dump(self, output_file)
+
+        # Put generator back, in case the sampler is used further after
+        # pickling
+        self._nuts = nuts
 
     def set_delta(self, delta):
         """
         Sets delta for the nuts algorithm. This is the goal acceptance
         probability for the algorithm. Used to set the scalar magnitude of the
         leapfrog step size.
         """
         if self._running:
             raise RuntimeError('cannot set delta while sampler is running')
         if delta < 0 or delta > 1:
             raise ValueError('delta must be in [0, 1]')
-        self._delta = delta
+        self._adaptor[1] = delta
 
     def set_hamiltonian_threshold(self, hamiltonian_threshold):
         """
         Sets threshold difference in Hamiltonian value from one iteration to
         next which determines whether an iteration is divergent.
         """
         if hamiltonian_threshold < 0:
@@ -675,46 +744,52 @@
         epsilon, the scalar magnitude of the leafrog step size.
         """
         if self._running:
             raise RuntimeError(
                 'cannot set number of adaption steps while sampler is running')
         if n < 0:
             raise ValueError('number of adaption steps must be non-negative')
-        self._num_adaption_steps = int(n)
+        self._adaptor[0] = int(n)
 
     def set_use_dense_mass_matrix(self, use_dense_mass_matrix):
         """
         If ``use_dense_mass_matrix`` is False then algorithm uses a diagonal
         matrix for the mass matrix. If True then a fully dense mass matrix is
         used.
         """
-        self._use_dense_mass_matrix = bool(use_dense_mass_matrix)
+        if self._running:
+            raise RuntimeError(
+                'cannot set number of adaption steps while sampler is running')
+        self._adaptor[2] = bool(use_dense_mass_matrix)
 
     def tell(self, reply):
         """ See :meth:`pints.SingleChainMCMC.tell()`. """
         if not self._ready_for_tell:
             raise RuntimeError('Tell called before proposal was set.')
         self._ready_for_tell = False
 
         # send log likelihood and gradient to nuts coroutine,
-        # return value is the next theta to evaluate at
+        # return value is the next theta to evaluate at but not necessarily the
+        # proposed mcmc step. Final mcmc proposal is distinguished from
+        # intermediate steps by tuple type.
         self._next = self._nuts.send(reply)
 
         # coroutine signals end of current step by sending a tuple of
         # information about the last mcmc step
         if isinstance(self._next, tuple):
             # extract next point in chain, its logpdf, the acceptance
             # probability and the number of leapfrog steps taken during
             # the last mcmc step
             self._current = self._next[0]
             current_logpdf = self._next[1]
             current_gradient = self._next[2]
             current_acceptance = self._next[3]
             current_n_leapfrog = self._next[4]
             divergent = self._next[5]
+            self._adaptor = self._next[6]
 
             # Increase iteration count
             self._mcmc_iteration += 1
 
             # average quantities for logging
             n_it_since_log = self._mcmc_iteration - self._last_log_write
             self._mcmc_acceptance = (
@@ -745,8 +820,13 @@
             return None
 
     def use_dense_mass_matrix(self):
         """
         Returns if the algorithm uses a dense (True) or diagonal (False) mass
         matrix.
         """
-        return self._use_dense_mass_matrix
+        try:
+            # When adaptor has not been initialised
+            return self._adaptor[2]
+        except TypeError:
+            # Adaptor has been initialised
+            return self._adaptor.use_dense_mass_matrix()
```

### Comparing `pints-0.4.0/pints/_mcmc/_population.py` & `pints-0.5.0/pints/_mcmc/_population.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
         # Next chain to exchange / crossover with
         self._j = 1
 
         # Ask all inner samplers for first point, which should be x0
         for chain in self._chains:
             x0 = chain.ask()
-            assert(np.all(x0 == self._x0))
+            assert np.all(x0 == self._x0)
 
         # Update sampler state
         self._running = True
 
     def _log_init(self, logger):
         """ See :meth:`Loggable._log_init()`. """
         n = len(self._schedule)
```

### Comparing `pints-0.4.0/pints/_mcmc/_rao_blackwell_ac.py` & `pints-0.5.0/pints/_mcmc/_rao_blackwell_ac.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_mcmc/_relativistic.py` & `pints-0.5.0/pints/_mcmc/_relativistic.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,15 +448,15 @@
 
         # Unpack reply
         energy, gradient = reply
 
         # Check reply, copy gradient
         energy = float(energy)
         gradient = pints.vector(gradient)
-        assert(gradient.shape == (self._n_parameters, ))
+        assert gradient.shape == (self._n_parameters, )
 
         # Energy = -log_pdf, so flip both signs!
         energy = -energy
         gradient = -gradient
 
         # Very first call
         if self._current is None:
```

### Comparing `pints-0.4.0/pints/_mcmc/_slice_doubling.py` & `pints-0.5.0/pints/_mcmc/_slice_doubling.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_mcmc/_slice_rank_shrinking.py` & `pints-0.5.0/pints/_mcmc/_slice_rank_shrinking.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 
         # Unpack reply
         fx, grad = reply
 
         # Check reply, copy gradient
         fx = float(fx)
         grad = pints.vector(grad)
-        assert(grad.shape == (self._n_parameters, ))
+        assert grad.shape == (self._n_parameters, )
 
         # Very first call
         if self._current is None:
             # Check first point is somewhere sensible
             if not np.isfinite(fx):
                 raise ValueError(
                     'Initial point for MCMC must have finite logpdf.')
```

### Comparing `pints-0.4.0/pints/_mcmc/_slice_stepout.py` & `pints-0.5.0/pints/_mcmc/_slice_stepout.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_mcmc/_summary.py` & `pints-0.5.0/pints/_mcmc/_summary.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_nested/__init__.py` & `pints-0.5.0/pints/_nested/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         if not isinstance(log_prior, pints.LogPrior):
             raise ValueError('Given log_prior must extend pints.LogPrior')
 
         # prior accessed by subclasses to do prior sampling in ask() step
         self._log_prior = log_prior
 
         # Current value of the threshold log-likelihood value
-        self._running_log_likelihood = -float('inf')
+        self._running_log_likelihood = -np.inf
         self._proposed = None
 
         # Initialise active point containers
         self._n_active_points = 400
         self._n_parameters = self._log_prior.n_parameters()
         self._m_active = np.zeros((self._n_active_points,
                                    self._n_parameters + 1))
@@ -287,15 +287,15 @@
         # Total number of posterior samples
         self._posterior_samples = 1000
 
         # Convergence criterion in log-evidence
         self._marginal_log_likelihood_threshold = 0.5
 
         # Initial marginal difference
-        self._diff = np.float('-Inf')
+        self._diff = np.inf
 
         # By default use ellipsoidal sampling
         if method is None:
             method = pints.NestedEllipsoidSampler
         else:
             try:
                 ok = issubclass(method, pints.NestedSampler)
```

### Comparing `pints-0.4.0/pints/_nested/_ellipsoid.py` & `pints-0.5.0/pints/_nested/_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_nested/_rejection.py` & `pints-0.5.0/pints/_nested/_rejection.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_optimisers/__init__.py` & `pints-0.5.0/pints/_optimisers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
             # Tell the optimiser the evaluations; allowing it to update its
             # internal state.
             optimiser.tell(fs)
 
             # Check stopping criteria
             # At this point, custom stopping criteria can be added in
-            if optimiser.fbest() < threshold:
+            if optimiser.f_best() < threshold:
                 running = False
 
             # Check for optimiser issues
             if optimiser.stop():
                 running = False
 
             # At this point, code to visualise or benchmark optimiser behaviour
@@ -140,19 +140,48 @@
     def ask(self):
         """
         Returns a list of positions in the search space to evaluate.
         """
         raise NotImplementedError
 
     def fbest(self):
+        """Deprecated alias of :meth:`f_best()`."""
+        # Deprecated on 2021-11-29
+        import warnings
+        warnings.warn(
+            'The method `pints.Optimiser.fbest` is deprecated.'
+            ' Please use `pints.Optimiser.f_best` instead.')
+        return self.f_best()
+
+    def f_best(self):
         """
-        Returns the objective function evaluated at the current best position.
+        Returns the best objective function evaluation seen by this optimiser,
+        such that ``f_best = f(x_best)``.
         """
         raise NotImplementedError
 
+    def f_guessed(self):
+        """
+        For optimisers in which the best guess of the optimum
+        (see :meth:`x_guessed`) differs from the best-seen point (see
+        :meth:`x_best`), this method returns an estimate of the objective
+        function value at ``x_guessed``.
+
+        Notes:
+
+        1. For many optimisers the best guess is simply the best point seen
+           during the optimisation, so that this method is equivalent to
+           :meth:`f_best()`.
+        2. Because ``x_guessed`` is not required to be a point that the
+           optimiser has visited, the value ``f(x_guessed)`` may be unkown. In
+           these cases, an approximation of ``f(x_guessed)`` may be returned.
+
+        """
+        return self.f_best()
+
     def name(self):
         """
         Returns this method's full name.
         """
         raise NotImplementedError
 
     def needs_sensitivities(self):
@@ -185,19 +214,42 @@
         :meth:`needs_sensitivities`), ``fx`` should be a tuple
         ``(objective, sensitivities)``, containing the values returned by
         :meth:`pints.ErrorMeasure.evaluateS1()`.
         """
         raise NotImplementedError
 
     def xbest(self):
+        """Deprecated alias of :meth:`x_best()`."""
+        # Deprecated on 2021-11-29
+        import warnings
+        warnings.warn(
+            'The method `pints.Optimiser.xbest` is deprecated.'
+            ' Please use `pints.Optimiser.x_best` instead.')
+        return self.x_best()
+
+    def x_best(self):
         """
-        Returns the current best position.
+        Returns the best position seen during an optimisation, i.e. the point
+        for which the minimal error or maximum likelihood was observed.
         """
         raise NotImplementedError
 
+    def x_guessed(self):
+        """
+        Returns the optimiser's current best estimate of where the optimum is.
+
+        For many optimisers, this will simply be the point for which the
+        minimal error or maximum likelihood was observed, so that
+        ``x_guessed = x_best``. However, optimisers like :class:`pints.CMAES`
+        and its derivatives, maintain a separate "best guess" value that does
+        not necessarily correspond to any of the points evaluated during the
+        optimisation.
+        """
+        return self.x_best()
+
 
 class PopulationBasedOptimiser(Optimiser):
     """
     Base class for optimisers that work by moving multiple points through the
     search space.
 
     Extends :class:`Optimiser`.
@@ -353,26 +405,30 @@
         self._transformation = transformation
 
         # Store function
         if self._minimising:
             self._function = function
         else:
             self._function = pints.ProbabilityBasedError(function)
-        del(function)
+        del function
 
         # Create optimiser
         if method is None:
             method = pints.CMAES
         elif not issubclass(method, pints.Optimiser):
             raise ValueError('Method must be subclass of pints.Optimiser.')
         self._optimiser = method(x0, sigma0, boundaries)
 
         # Check if sensitivities are required
         self._needs_sensitivities = self._optimiser.needs_sensitivities()
 
+        # Track optimiser's f_best or f_guessed
+        self._use_f_guessed = None
+        self.set_f_guessed_tracking()
+
         # Logging
         self._log_to_screen = True
         self._log_filename = None
         self._log_csv = False
         self.set_log_interval()
 
         # Parallelisation
@@ -391,18 +447,21 @@
         #
 
         # Maximum iterations
         self._max_iterations = None
         self.set_max_iterations()
 
         # Maximum unchanged iterations
-        self._max_unchanged_iterations = None
-        self._min_significant_change = 1
+        self._unchanged_max_iterations = None  # n_iter w/o change until stop
+        self._unchanged_threshold = 1          # smallest significant f change
         self.set_max_unchanged_iterations()
 
+        # Maximum evaluations
+        self._max_evaluations = None
+
         # Threshold value
         self._threshold = None
 
         # Post-run statistics
         self._evaluations = None
         self._iterations = None
         self._time = None
@@ -410,14 +469,31 @@
     def evaluations(self):
         """
         Returns the number of evaluations performed during the last run, or
         ``None`` if the controller hasn't ran yet.
         """
         return self._evaluations
 
+    def max_evaluations(self):
+        """
+        Returns the maximum number of evaluations if this stopping criteria is
+        set, or ``None`` if it is not. See :meth:`set_max_evaluations`.
+        """
+        return self._max_evaluations
+
+    def f_guessed_tracking(self):
+        """
+        Returns ``True`` if the controller is set to track the optimiser
+        progress using :meth:`pints.Optimiser.f_guessed()` rather than
+        :meth:`pints.Optimiser.f_best()`.
+
+        See also :meth:`set_f_guessed_tracking`.
+        """
+        return self._use_f_guessed
+
     def iterations(self):
         """
         Returns the number of iterations performed during the last run, or
         ``None`` if the controller hasn't ran yet.
         """
         return self._iterations
 
@@ -428,19 +504,22 @@
         """
         return self._max_iterations
 
     def max_unchanged_iterations(self):
         """
         Returns a tuple ``(iterations, threshold)`` specifying a maximum
         unchanged iterations stopping criterion, or ``(None, None)`` if no such
-        criterion is set. See :meth:`set_max_unchanged_iterations()`.
+        criterion is set.
+
+        The entries in the tuple correspond directly to the arguments to
+        :meth:`set_max_unchanged_iterations()`.
         """
-        if self._max_unchanged_iterations is None:
+        if self._unchanged_max_iterations is None:
             return (None, None)
-        return (self._max_unchanged_iterations, self._min_significant_change)
+        return (self._unchanged_max_iterations, self._unchanged_threshold)
 
     def optimiser(self):
         """
         Returns the underlying optimiser object, allowing detailed
         configuration.
         """
         return self._optimiser
@@ -450,30 +529,31 @@
         Returns the number of parallel worker processes this routine will be
         run on, or ``False`` if parallelisation is disabled.
         """
         return self._n_workers if self._parallel else False
 
     def run(self):
         """
-        Runs the optimisation, returns a tuple ``(xbest, fbest)``.
+        Runs the optimisation, returns a tuple ``(x_best, f_best)``.
 
         An optional ``callback`` function can be passed in that will be called
         at the end of every iteration. The callback should take the arguments
         ``(iteration, optimiser)``, where ``iteration`` is the iteration count
         (an integer) and ``optimiser`` is the optimiser object.
         """
         # Can only run once for each controller instance
         if self._has_run:
             raise RuntimeError("Controller is valid for single use only")
         self._has_run = True
 
         # Check stopping criteria
         has_stopping_criterion = False
         has_stopping_criterion |= (self._max_iterations is not None)
-        has_stopping_criterion |= (self._max_unchanged_iterations is not None)
+        has_stopping_criterion |= (self._unchanged_max_iterations is not None)
+        has_stopping_criterion |= (self._max_evaluations is not None)
         has_stopping_criterion |= (self._threshold is not None)
         if not has_stopping_criterion:
             raise ValueError('At least one stopping criterion must be set.')
 
         # Iterations and function evaluations
         iteration = 0
         evaluations = 0
@@ -496,19 +576,22 @@
             # particles!
             if isinstance(self._optimiser, PopulationBasedOptimiser):
                 n_workers = min(n_workers, self._optimiser.population_size())
             evaluator = pints.ParallelEvaluator(f, n_workers=n_workers)
         else:
             evaluator = pints.SequentialEvaluator(f)
 
-        # Keep track of best position and score
-        fbest = float('inf')
+        # Keep track of current best and best-guess scores.
+        fb = fg = np.inf
 
-        # Internally we always minimise! Keep a 2nd value to show the user
-        fbest_user = fbest if self._minimising else -fbest
+        # Internally we always minimise! Keep a 2nd value to show the user.
+        fb_user, fg_user = (fb, fg) if self._minimising else (-fb, -fg)
+
+        # Keep track of the last significant change
+        f_sig = np.inf
 
         # Set up progress reporting
         next_message = 0
 
         # Start logging
         logging = self._log_to_screen or self._log_filename
         if logging:
@@ -541,18 +624,20 @@
             if not self._log_to_screen:
                 logger.set_stream(None)
             if self._log_filename:
                 logger.set_filename(self._log_filename, csv=self._log_csv)
 
             # Add fields to log
             max_iter_guess = max(self._max_iterations or 0, 10000)
-            max_eval_guess = max_iter_guess * pop_size
+            max_eval_guess = max(
+                self._max_evaluations or 0, max_iter_guess * pop_size)
             logger.add_counter('Iter.', max_value=max_iter_guess)
             logger.add_counter('Eval.', max_value=max_eval_guess)
             logger.add_float('Best')
+            logger.add_float('Current')
             self._optimiser._log_init(logger)
             logger.add_time('Time m:s')
 
         # Start searching
         timer = pints.Timer()
         running = True
         try:
@@ -562,38 +647,34 @@
 
                 # Calculate scores
                 fs = evaluator.evaluate(xs)
 
                 # Perform iteration
                 self._optimiser.tell(fs)
 
-                # Check if new best found
-                fnew = self._optimiser.fbest()
-                if fnew < fbest:
-                    # Check if this counts as a significant change
-                    if np.abs(fnew - fbest) < self._min_significant_change:
-                        unchanged_iterations += 1
-                    else:
-                        unchanged_iterations = 0
-
-                    # Update best
-                    fbest = fnew
-
-                    # Update user value of fbest
-                    fbest_user = fbest if self._minimising else -fbest
+                # Update current scores
+                fb = self._optimiser.f_best()
+                fg = self._optimiser.f_guessed()
+                fb_user, fg_user = (fb, fg) if self._minimising else (-fb, -fg)
+
+                # Check for significant changes
+                f_new = fg if self._use_f_guessed else fb
+                if np.abs(f_new - f_sig) >= self._unchanged_threshold:
+                    unchanged_iterations = 0
+                    f_sig = f_new
                 else:
                     unchanged_iterations += 1
 
                 # Update evaluation count
                 evaluations += len(fs)
 
                 # Show progress
                 if logging and iteration >= next_message:
                     # Log state
-                    logger.log(iteration, evaluations, fbest_user)
+                    logger.log(iteration, evaluations, fb_user, fg_user)
                     self._optimiser._log_write(logger)
                     logger.log(timer.time())
 
                     # Choose next logging point
                     if iteration < self._message_warm_up:
                         next_message = iteration + 1
                     else:
@@ -607,83 +688,97 @@
                 # Check stopping criteria
                 #
 
                 # Maximum number of iterations
                 if (self._max_iterations is not None and
                         iteration >= self._max_iterations):
                     running = False
-                    halt_message = ('Halting: Maximum number of iterations ('
+                    halt_message = ('Maximum number of iterations ('
                                     + str(iteration) + ') reached.')
 
                 # Maximum number of iterations without significant change
-                halt = (self._max_unchanged_iterations is not None and
-                        unchanged_iterations >= self._max_unchanged_iterations)
-                if halt:
+                halt = (self._unchanged_max_iterations is not None and
+                        unchanged_iterations >= self._unchanged_max_iterations)
+                if running and halt:
                     running = False
-                    halt_message = ('Halting: No significant change for ' +
+                    halt_message = ('No significant change for ' +
                                     str(unchanged_iterations) + ' iterations.')
 
+                # Maximum number of evaluations
+                if (self._max_evaluations is not None and
+                        evaluations >= self._max_evaluations):
+                    running = False
+                    halt_message = (
+                        'Maximum number of evaluations ('
+                        + str(self._max_evaluations) + ') reached.')
+
                 # Threshold value
-                if self._threshold is not None and fbest < self._threshold:
+                halt = (self._threshold is not None
+                        and f_new < self._threshold)
+                if running and halt:
                     running = False
-                    halt_message = ('Halting: Objective function crossed'
-                                    ' threshold: ' + str(self._threshold) +
-                                    '.')
+                    halt_message = ('Objective function crossed threshold: '
+                                    + str(self._threshold) + '.')
 
                 # Error in optimiser
                 error = self._optimiser.stop()
                 if error:   # pragma: no cover
                     running = False
-                    halt_message = ('Halting: ' + str(error))
+                    halt_message = str(error)
 
                 elif self._callback is not None:
                     self._callback(iteration - 1, self._optimiser)
 
         except (Exception, SystemExit, KeyboardInterrupt):  # pragma: no cover
             # Unexpected end!
             # Show last result and exit
             print('\n' + '-' * 40)
             print('Unexpected termination.')
-            print('Current best score: ' + str(fbest))
-            print('Current best position:')
-
-            # Inverse transform search parameters
-            if self._transformation:
-                xbest = self._transformation.to_model(self._optimiser.xbest())
-            else:
-                xbest = self._optimiser.xbest()
+            print('Current score: ' + str(fg_user))
+            print('Current position:')
 
-            for p in xbest:
+            # Show current parameters
+            x_user = self._optimiser.x_guessed()
+            if self._transformation is not None:
+                x_user = self._transformation.to_model(x_user)
+            for p in x_user:
                 print(pints.strfloat(p))
             print('-' * 40)
             raise
 
         # Stop timer
         self._time = timer.time()
 
         # Log final values and show halt message
         if logging:
-            logger.log(iteration, evaluations, fbest_user)
-            self._optimiser._log_write(logger)
-            logger.log(self._time)
+            if iteration - 1 < next_message:
+                logger.log(iteration, evaluations, fb_user, fg_user)
+                self._optimiser._log_write(logger)
+                logger.log(self._time)
             if self._log_to_screen:
-                print(halt_message)
+                print('Halting: ' + halt_message)
 
         # Save post-run statistics
         self._evaluations = evaluations
         self._iterations = iteration
 
-        # Inverse transform search parameters
-        if self._transformation:
-            xbest = self._transformation.to_model(self._optimiser.xbest())
+        # Get best parameters
+        if self._use_f_guessed:
+            x = self._optimiser.x_guessed()
+            f = self._optimiser.f_guessed()
         else:
-            xbest = self._optimiser.xbest()
+            x = self._optimiser.x_best()
+            f = self._optimiser.f_best()
+
+        # Inverse transform search parameters
+        if self._transformation is not None:
+            x = self._transformation.to_model(x)
 
         # Return best position and score
-        return xbest, fbest_user
+        return x, f if self._minimising else -f
 
     def set_callback(self, cb=None):
         """
         Allows a "callback" function to be passed in that will be called at the
         end of every iteration.
 
         This can be used for e.g. visualising optimiser progress.
@@ -696,14 +791,24 @@
             opt.set_callback(cb)
 
         """
         if cb is not None and not callable(cb):
             raise ValueError('The argument cb must be None or a callable.')
         self._callback = cb
 
+    def set_f_guessed_tracking(self, use_f_guessed=False):
+        """
+        Sets the method used to track the optimiser progress to
+        :meth:`pints.Optimiser.f_guessed()` or
+        :meth:`pints.Optimiser.f_best()` (default).
+
+        The tracked ``f`` value is used to evaluate stopping criteria.
+        """
+        self._use_f_guessed = bool(use_f_guessed)
+
     def set_log_interval(self, iters=20, warm_up=3):
         """
         Changes the frequency with which messages are logged.
 
         Parameters
         ----------
         ``interval``
@@ -738,14 +843,29 @@
 
     def set_log_to_screen(self, enabled):
         """
         Enables or disables logging to screen.
         """
         self._log_to_screen = True if enabled else False
 
+    def set_max_evaluations(self, evaluations=None):
+        """
+        Adds a stopping criterion, allowing the routine to halt after the
+        given number of ``evaluations``.
+
+        This criterion is disabled by default. To enable, pass in any positive
+        integer. To disable again, use ``set_max_evaluations(None)``.
+        """
+        if evaluations is not None:
+            evaluations = int(evaluations)
+            if evaluations < 0:
+                raise ValueError(
+                    'Maximum number of evaluations cannot be negative.')
+        self._max_evaluations = evaluations
+
     def set_max_iterations(self, iterations=10000):
         """
         Adds a stopping criterion, allowing the routine to halt after the
         given number of ``iterations``.
 
         This criterion is enabled by default. To disable it, use
         ``set_max_iterations(None)``.
@@ -772,16 +892,16 @@
                 raise ValueError(
                     'Maximum number of iterations cannot be negative.')
 
         threshold = float(threshold)
         if threshold < 0:
             raise ValueError('Minimum significant change cannot be negative.')
 
-        self._max_unchanged_iterations = iterations
-        self._min_significant_change = threshold
+        self._unchanged_max_iterations = iterations
+        self._unchanged_threshold = threshold
 
     def set_parallel(self, parallel=False):
         """
         Enables/disables parallel evaluation.
 
         If ``parallel=True``, the method will run using a number of worker
         processes equal to the detected cpu core count. The number of workers
@@ -858,86 +978,49 @@
         evaluates points in the parameter space.
     x0
         The starting point for searches in the parameter space. This value may
         be used directly (for example as the initial position of a particle in
         :class:`PSO`) or indirectly (for example as the center of a
         distribution in :class:`XNES`).
     sigma0
-        An optional initial standard deviation around ``x0``. Can be specified
-        either as a scalar value (one standard deviation for all coordinates)
-        or as an array with one entry per dimension. Not all methods will use
-        this information.
+        An optional initial standard deviation around ``x0``, or a parameter
+        representing the "scale" of the parameters. Can be specified either as
+        a scalar value (same value for all dimensions) or as an array with one
+        entry per dimension. Not all methods will use this information.
     boundaries
         An optional set of boundaries on the parameter space.
     transformation
         An optional :class:`pints.Transformation` to allow the optimiser to
         search in a transformed parameter space. If used, points shown or
         returned to the user will first be detransformed back to the original
         space.
     method
         The class of :class:`pints.Optimiser` to use for the optimisation.
         If no method is specified, :class:`CMAES` is used.
 
     Returns
     -------
-    xbest : numpy array
+    x_best : numpy array
         The best parameter set obtained
-    fbest : float
+    f_best : float
         The corresponding score.
     """
     return OptimisationController(
         function, x0, sigma0, boundaries, transformation, method).run()
 
 
-class TriangleWaveTransform(object):
-    """
-    Transforms from unbounded to (rectangular) bounded parameter space using a
-    periodic triangle-wave transform.
-
-    Note: The transform is applied _inside_ optimisation methods, there is no
-    need to wrap this around your own problem or score function.
-
-    This can be applied as a transformation on ``x`` to implement _rectangular_
-    boundaries in methods with no natural boundary mechanism. It effectively
-    mirrors the search space at every boundary, leading to a continuous (but
-    non-smooth) periodic landscape. While this effectively creates an infinite
-    number of minima/maxima, each one maps to the same point in parameter
-    space.
-
-    It should work well for methods that maintain a single search position or a
-    single search distribution (e.g. :class:`CMAES`, :class:`xNES`,
-    :class:`SNES`), which will end up in one of the many mirror images.
-    However, for methods that use independent search particles (e.g.
-    :class:`PSO`) it could lead to a scattered population, with different
-    particles exploring different mirror images. Other strategies should be
-    used for such problems.
-    """
-
-    def __init__(self, boundaries):
-        self._lower = boundaries.lower()
-        self._upper = boundaries.upper()
-        self._range = self._upper - self._lower
-        self._range2 = 2 * self._range
-
-    def __call__(self, x):
-        y = np.remainder(x - self._lower, self._range2)
-        z = np.remainder(y, self._range)
-        return ((self._lower + z) * (y < self._range)
-                + (self._upper - z) * (y >= self._range))
-
-
 def curve_fit(f, x, y, p0, boundaries=None, threshold=None, max_iter=None,
               max_unchanged=200, verbose=False, parallel=False, method=None):
     """
     Fits a function ``f(x, *p)`` to a dataset ``(x, y)`` by finding the value
     of ``p`` for which ``sum((y - f(x, *p))**2) / n`` is minimised (where ``n``
     is the number of entries in ``y``).
 
-    Returns a tuple ``(xbest, fbest)`` with the best position found, and the
-    corresponding value ``fbest = f(xbest)``.
+    Returns a tuple ``(x_best, f_best)`` with the best position found, and the
+    corresponding value ``f_best = f(x_best)``.
 
     Parameters
     ----------
     f : callable
         A function or callable class to be minimised.
     x
         The values of an independent variable, at which ``y`` was recorded.
@@ -967,17 +1050,17 @@
         integer greater than 0.
     method
         The :class:`pints.Optimiser` to use. If no method is specified,
         ``pints.CMAES`` is used.
 
     Returns
     -------
-    xbest : numpy array
+    x_best : numpy array
         The best parameter set obtained.
-    fbest : float
+    f_best : float
         The corresponding score.
 
     Example
     -------
     ::
 
         import numpy as np
@@ -1053,16 +1136,16 @@
 
 def fmin(f, x0, args=None, boundaries=None, threshold=None, max_iter=None,
          max_unchanged=200, verbose=False, parallel=False, method=None):
     """
     Minimises a callable function ``f``, starting from position ``x0``, using a
     :class:`pints.Optimiser`.
 
-    Returns a tuple ``(xbest, fbest)`` with the best position found, and the
-    corresponding value ``fbest = f(xbest)``.
+    Returns a tuple ``(x_best, f_best)`` with the best position found, and the
+    corresponding value ``f_best = f(x_best)``.
 
     Parameters
     ----------
     f
         A function or callable class to be minimised.
     x0
         The initial point to search at. Must be a 1-dimensional sequence (e.g.
```

### Comparing `pints-0.4.0/pints/_optimisers/_cmaes.py` & `pints-0.5.0/pints/_optimisers/_cmaes.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,16 @@
     def __init__(self, x0, sigma0=None, boundaries=None):
         super(CMAES, self).__init__(x0, sigma0, boundaries)
 
         # Set initial state
         self._running = False
         self._ready_for_tell = False
 
-        # Best solution found
-        self._xbest = pints.vector(x0)
-        self._fbest = float('inf')
+        # Estimated f(x_guessed)
+        self._f_guessed = np.inf
 
     def ask(self):
         """ See :meth:`Optimiser.ask()`. """
         # Initialise on first call
         if not self._running:
             self._initialise()
 
@@ -68,26 +67,28 @@
                     'All points requested by CMA-ES are outside the'
                     ' boundaries.')
 
         # Set as read-only and return
         self._user_xs.setflags(write=False)
         return self._user_xs
 
-    def fbest(self):
-        """ See :meth:`Optimiser.fbest()`. """
-        if not self._running:
-            return float('inf')
-        f = self._es.result.fbest
-        return float('inf') if f is None else f
+    def f_best(self):
+        """ See :meth:`Optimiser.f_best()`. """
+        f = self._es.result.fbest if self._running else None
+        return np.inf if f is None else f
+
+    def f_guessed(self):
+        """ See :meth:`Optimiser.f_guessed()`. """
+        return self._f_guessed
 
     def _initialise(self):
         """
         Initialises the optimiser for the first iteration.
         """
-        assert(not self._running)
+        assert not self._running
 
         # Import cma (may fail!)
         # Only the first time this is called in a running program incurs
         # much overhead.
         import cma
 
         # Set up simulation
@@ -196,13 +197,22 @@
             user_fx = fx
             fx = np.ones((self._population_size, )) * np.inf
             fx[self._user_ids] = user_fx
 
         # Tell CMA-ES
         self._es.tell(self._xs, fx)
 
-    def xbest(self):
-        """ See :meth:`Optimiser.xbest()`. """
-        if self._running:
-            x = self._es.result.xbest
-            return np.array(self._x0 if x is None else x, copy=True)
-        return np.array(self._x0, copy=True)
+        # Update f_guessed, on the assumption that the best value in our
+        # current set of points is a reasonable approximation of f(mu). This
+        # will become more true as the optimiser progresses.
+        self._f_guessed = np.min(fx)
+
+    def x_best(self):
+        """ See :meth:`Optimiser.x_best()`. """
+        x = self._es.result.xbest if self._running else None
+        return np.array(self._x0 if x is None else x)
+
+    def x_guessed(self):
+        """ See :meth:`Optimiser.x_guessed()`. """
+        x = self._es.result.xfavorite if self._running else None
+        return np.array(self._x0 if x is None else x)
+
```

### Comparing `pints-0.4.0/pints/_optimisers/_cmaes_bare.py` & `pints-0.5.0/pints/_optimisers/_cmaes_bare.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,23 +45,26 @@
         super(BareCMAES, self).__init__(x0, sigma0, boundaries)
 
         # Set initial state
         self._running = False
         self._ready_for_tell = False
 
         # Best solution found
-        self._xbest = pints.vector(x0)
-        self._fbest = float('inf')
+        self._x_best = pints.vector(x0)
+        self._f_best = np.inf
 
         # Number of iterations run
         self._iterations = 0
 
         # Mean of the proposal distribution
         self._mu = np.copy(self._x0)
 
+        # Approximate value at self._mu
+        self._f_guessed = np.inf
+
         # Step size
         self._eta = np.min(self._sigma0)
 
         # Covariance matrix C and decomposition in rotation R and scaling S
         # A decomposition C = R S S R.T can be made, such that R is the matrix
         # of eigenvectors of C, and S is a diagonal matrix containing the
         # square roots of the eigenvalues of C.
@@ -96,27 +99,22 @@
 
         # Centered samples: centered at zero, with rotation and scaling
         self._ys = np.array([self._R.dot(self._S).dot(z) for z in self._zs])
 
         # Samples from N(mu, eta**2 * C)
         self._xs = np.array([self._mu + self._eta * y for y in self._ys])
 
-        # Apply boundaries; creating safe points for evaluation
-        # Rectangular boundaries? Then perform boundary transform
-        if self._boundary_transform is not None:
-            self._xs = self._boundary_transform(self._xs)
-
-        # Manual boundaries? Then pass only xs that are within bounds
-        if self._manual_boundaries:
+        # Boundaries? Then only pass user xs that are within bounds
+        if self._boundaries is not None:
             self._user_ids = np.nonzero(
                 [self._boundaries.check(x) for x in self._xs])
             self._user_xs = self._xs[self._user_ids]
             if len(self._user_xs) == 0:     # pragma: no cover
-                warnings.warn('All points requested by CMA-ES are outside the'
-                              ' boundaries.')
+                warnings.warn('All points requested by BareCMAES are outside'
+                              ' the boundaries.')
         else:
             self._user_xs = self._xs
 
         # Set as read-only and return
         self._user_xs.setflags(write=False)
         return self._user_xs
 
@@ -131,39 +129,34 @@
         eigenvalues of ``C``, such that ``C = R S S R.T``.
         """
         if decomposed:
             return self._R, self._S
         else:
             return np.copy(self._C)
 
-    def fbest(self):
-        """ See :meth:`Optimiser.fbest()`. """
-        return self._fbest
+    def f_best(self):
+        """ See :meth:`Optimiser.f_best()`. """
+        return self._f_best
+
+    def f_guessed(self):
+        """ See :meth:`Optimiser.f_guessed()`. """
+        return self._f_guessed
 
     def mean(self):
         """
         Returns the current mean of the proposal distribution.
         """
-        return np.copy(self._mu)
+        return self.x_guessed()
 
     def _initialise(self):
         """
         Initialises the optimiser for the first iteration.
         """
         assert (not self._running)
 
-        # Create boundary transform, or use manual boundary checking
-        self._manual_boundaries = False
-        self._boundary_transform = None
-        if isinstance(self._boundaries, pints.RectangularBoundaries):
-            self._boundary_transform = pints.TriangleWaveTransform(
-                self._boundaries)
-        elif self._boundaries is not None:
-            self._manual_boundaries = True
-
         # Parent generation population size
         # The parameter parent_pop_size is the mu in the papers. It represents
         # the size of a parent population used to update our paramters.
         self._parent_pop_size = self._population_size // 2
 
         # Weights, all set equal for the moment
         # Sum of all positive weights should be 1
@@ -267,25 +260,25 @@
         self._iterations += 1
 
         # Some aliases for readability
         n = self._n_parameters
         npo = self._population_size
         npa = self._parent_pop_size
 
-        # Manual boundaries? Then reconstruct full fx vector
-        if self._manual_boundaries and len(fx) < npo:
+        # Boundaries? Then reconstruct full fx vector
+        if self._boundaries is not None and len(fx) < npo:
             user_fx = fx
-            fx = np.ones((npo, )) * float('inf')
+            fx = np.ones((npo, )) * np.inf
             fx[self._user_ids] = user_fx
 
         # Order the points from best to worst score
         order = np.argsort(fx)
-        xs = np.array(self._xs[order])
-        zs = np.array(self._zs[order])
-        ys = np.array(self._ys[order])
+        xs = self._xs[order]
+        zs = self._zs[order]
+        ys = self._ys[order]
 
         # Update the mean
         self._mu += self._cm * np.sum(
             ((xs[:npa] - self._mu).T * self._W[:npa]).T, axis=0)
 
         # Get the weighted means of y and z
         zmeans = np.sum((zs[:npa].T * self._W[:npa]).T, 0)
@@ -349,21 +342,23 @@
             self._csig / self._dsig * (norm(self._psig) / self._e - 1))
 
         # Update eigenvectors and eigenvalues of C
         eig = np.linalg.eigh(self._C)
         self._S = np.sqrt(np.diag(eig[0]))
         self._R = eig[1]
 
-        # Update xbest and fbest
-        # Note: The stored values are based on particles, not on the mean of
-        # all particles! This has the advantage that we don't require an extra
-        # evaluation at mu to get a pair (mu, f(mu)). The downside is that
-        # xbest isn't the very best point. However, xbest and mu seem to
-        # converge quite quickly, so that this difference disappears.
-        if self._fbest > fx[order[0]]:
-            self._fbest = fx[order[0]]
-            self._xbest = xs[0]
-
-    def xbest(self):
-        """ See :meth:`Optimiser.xbest()`. """
-        return self._xbest
-
+        # Update f_guessed on the assumption that the lowest value in our
+        # sample approximates f(mu)
+        self._f_guessed = fx[order[0]]
+
+        # Update x_best and f_best
+        if self._f_guessed < self._f_best:
+            self._f_best = self._f_guessed
+            self._x_best = np.array(xs[0], copy=True)
+
+    def x_best(self):
+        """ See :meth:`Optimiser.x_best()`. """
+        return self._x_best
+
+    def x_guessed(self):
+        """ See :meth:`Optimiser.x_guessed()`. """
+        return np.array(self._mu, copy=True)
```

### Comparing `pints-0.4.0/pints/_optimisers/_gradient_descent.py` & `pints-0.5.0/pints/_optimisers/_gradient_descent.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,40 @@
 # Fixed learning-rate gradient descent.
 #
 # This file is part of PINTS (https://github.com/pints-team/pints/) which is
 # released under the BSD 3-clause license. See accompanying LICENSE.md for
 # copyright notice and full license details.
 #
 import pints
+import numpy as np
 
 
 class GradientDescent(pints.Optimiser):
     """
     Gradient-descent method with a fixed learning rate.
+
+    The initial learning rate is set as ``min(sigma0)``, but this can be
+    changed at any time with :meth:`set_learning_rate()`.
+
+    This is an unbounded method: Any ``boundaries`` will be ignored.
     """
 
     def __init__(self, x0, sigma0=0.1, boundaries=None):
         super(GradientDescent, self).__init__(x0, sigma0, boundaries)
 
         # Set optimiser state
         self._running = False
         self._ready_for_tell = False
 
         # Best solution found
-        self._xbest = self._x0
-        self._fbest = float('inf')
+        self._x_best = self._x0
+        self._f_best = np.inf
 
         # Learning rate
-        self._eta = 0.01
+        self._eta = min(self._sigma0)
 
         # Current point, score, and gradient
         self._current = self._x0
         self._current_f = None
         self._current_df = None
 
         # Proposed next point (read-only, so can be passed to user)
@@ -42,17 +48,17 @@
         # Running, and ready for tell now
         self._ready_for_tell = True
         self._running = True
 
         # Return proposed points (just the one)
         return [self._proposed]
 
-    def fbest(self):
-        """ See :meth:`Optimiser.fbest()`. """
-        return self._fbest
+    def f_best(self):
+        """ See :meth:`Optimiser.f_best()`. """
+        return self._f_best
 
     def learning_rate(self):
         """ Returns this optimiser's learning rate. """
         return self._eta
 
     def name(self):
         """ See :meth:`Optimiser.name()`. """
@@ -108,16 +114,16 @@
         self._current_f = fx
         self._current_df = dfx
 
         # Propose next point
         self._proposed = self._current - self._eta * dfx
         self._proposed.setflags(write=False)
 
-        # Update xbest and fbest
-        if self._fbest > fx:
-            self._fbest = fx
-            self._xbest = self._current
-
-    def xbest(self):
-        """ See :meth:`Optimiser.xbest()`. """
-        return self._xbest
+        # Update x_best and f_best
+        if self._f_best > fx:
+            self._f_best = fx
+            self._x_best = self._current
+
+    def x_best(self):
+        """ See :meth:`Optimiser.x_best()`. """
+        return self._x_best
```

### Comparing `pints-0.4.0/pints/_optimisers/_nelder_mead.py` & `pints-0.5.0/pints/_optimisers/_nelder_mead.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,19 +210,17 @@
 
             # Ask for f(xr)
             return np.array([self._xr])
 
         # Extended iteration: ask for expansion or contraction point
         return np.array([self._xp])
 
-    def fbest(self):
-        """ See: :meth:`pints.Optimiser.fbest()`. """
-        if not self._running:
-            return float('inf')
-        return self._fs[0]
+    def f_best(self):
+        """ See: :meth:`pints.Optimiser.f_best()`. """
+        return self._fs[0] if self._running else np.inf
 
     def name(self):
         """ See: :meth:`pints.Optimiser.name()`. """
         return 'Nelder-Mead'
 
     def running(self):
         """ See: :meth:`pints.Optimiser.running()`. """
@@ -322,13 +320,11 @@
             # Reset and return: ask will set xr, get f(xr)
             self._xp = self._xr = self._fr = None
             return
 
         # Option 5: Shrink
         self._shrink = True
 
-    def xbest(self):
-        """ See: :meth:`pints.Optimiser.xbest()`. """
-        if not self._running:
-            return pints.vector(self._x0)
-        return pints.vector(self._xs[0])
+    def x_best(self):
+        """ See: :meth:`pints.Optimiser.x_best()`. """
+        return pints.vector(self._xs[0] if self._running else self._x0)
```

### Comparing `pints-0.4.0/pints/_optimisers/_pso.py` & `pints-0.5.0/pints/_optimisers/_pso.py`

 * *Files 13% similar despite different names*

```diff
@@ -91,85 +91,72 @@
         self._ready_for_tell = True
 
         # Return a copy of the filtered points (copy is used so that 1. the
         # user cannot modify the points and mess up the state, and 2. so that
         # the user can store the points without us modifying them).
         return np.copy(self._user_xs)
 
-    def fbest(self):
-        """ See :meth:`Optimiser.fbest()`. """
-        if self._running:
-            return self._fg
-        return float('inf')
+    def f_best(self):
+        """ See :meth:`Optimiser.f_best()`. """
+        return self._fg if self._running else np.inf
 
     def _initialise(self):
         """
         Initialises the optimiser for the first iteration.
         """
-        assert(not self._running)
+        assert not self._running
 
         # Initialize swarm
         self._xs = []     # Particle coordinate vectors
         self._vs = []     # Particle velocity vectors
         self._fl = []     # Best local score
         self._pl = []     # Best local position
 
         # Set initial positions
         self._xs.append(np.array(self._x0, copy=True))
+
+        # Attempt to sample n - 1 points from the boundaries
         if self._boundaries is not None:
-            # Attempt to sample n - 1 points from the boundaries
             try:
                 self._xs.extend(
                     self._boundaries.sample(self._population_size - 1))
             except NotImplementedError:
-                # Not all boundaries implement sampling
+                # Not all boundaries implement sampling.
                 pass
+
         # If we couldn't sample from the boundaries, use gaussian sampling
         # around x0.
-        for i in range(1, self._population_size):
-            self._xs.append(np.random.normal(self._x0, self._sigma0))
-        self._xs = np.array(self._xs, copy=True)
+        if len(self._xs) < self._population_size:
+            for i in range(self._population_size - 1):
+                self._xs.append(np.random.normal(self._x0, self._sigma0))
+        self._xs = np.array(self._xs)
 
         # Set initial velocities
         for i in range(self._population_size):
             self._vs.append(1e-1 * self._sigma0 *
                             np.random.uniform(0, 1, self._n_parameters))
 
         # Set initial scores and local best
         for i in range(self._population_size):
-            self._fl.append(float('inf'))
+            self._fl.append(np.inf)
             self._pl.append(self._xs[i])
 
         # Set global best position and score
-        self._fg = float('inf')
+        self._fg = np.inf
         self._pg = self._xs[0]
 
-        # Create boundary transform, or use manual boundary checking
-        self._manual_boundaries = False
-        self._boundary_transform = None
-        if isinstance(self._boundaries, pints.RectangularBoundaries):
-            self._boundary_transform = pints.TriangleWaveTransform(
-                self._boundaries)
-        elif self._boundaries is not None:
-            self._manual_boundaries = True
-
-        # Create safe xs to pass to user
-        if self._boundary_transform is not None:
-            # Rectangular boundaries? Then apply transform to xs
-            self._xs = self._boundary_transform(self._xs)
-        if self._manual_boundaries:
-            # Manual boundaries? Then filter out out-of-bounds points from xs
+        # Boundaries? Then filter out out-of-bounds points from xs
+        self._user_xs = self._xs
+        if self._boundaries is not None:
             self._user_ids = np.nonzero(
                 [self._boundaries.check(x) for x in self._xs])
             self._user_xs = self._xs[self._user_ids]
             if len(self._user_xs) == 0:     # pragma: no cover
                 warnings.warn(
                     'All initial PSO particles are outside the boundaries.')
-        else:
-            self._user_xs = self._xs
 
         # Set local/global exploration balance
         self.set_local_global_balance()
 
         # Update optimiser state
         self._running = True
 
@@ -192,16 +179,16 @@
     def running(self):
         """ See :meth:`Optimiser.running()`. """
         return self._running
 
     def set_local_global_balance(self, r=0.5):
         """
         Set the balance between local and global exploration for each particle,
-        using a parameter `r` such that `r = 1` is a fully local search and
-        `r = 0` is a fully global search.
+        using a parameter ``r`` such that ``r = 1`` is a fully local search and
+        ``r = 0`` is a fully global search.
         """
         if self._running:
             raise Exception('Cannot change settings during run.')
 
         # Check r
         r = float(r)
         if r < 0 or r > 1:
@@ -232,18 +219,18 @@
 
     def tell(self, fx):
         """ See :meth:`Optimiser.tell()`. """
         if not self._ready_for_tell:
             raise Exception('ask() not called before tell()')
         self._ready_for_tell = False
 
-        # Manual boundaries? Then reconstruct full fx vector
-        if self._manual_boundaries and len(fx) < self._population_size:
+        # Boundaries? Then reconstruct full fx vector
+        if self._boundaries is not None and len(fx) < self._population_size:
             user_fx = fx
-            fx = np.ones((self._population_size, )) * float('inf')
+            fx = np.ones((self._population_size, )) * np.inf
             fx[self._user_ids] = user_fx
 
         # Update particles
         for i in range(self._population_size):
 
             # Update best local position and score
             if fx[i] < self._fl[i]:
@@ -263,32 +250,28 @@
             if self._boundaries is not None:
                 if not self._boundaries.check(self._xs[i] + self._vs[i]):
                     self._vs[i] *= 0.5
 
             # Update position
             self._xs[i] += self._vs[i]
 
-        # Create safe xs to pass to user
-        if self._boundary_transform is not None:
-            # Rectangular boundaries? Then apply transform to xs
-            self._user_xs = self._xs = self._boundary_transform(self._xs)
-        elif self._manual_boundaries:
-            # Manual boundaries? Then filter out out-of-bounds points from xs
+        # Boundaries? Then filter out out-of-bounds points from xs
+        self._user_xs = self._xs
+        if self._boundaries is not None:
             self._user_ids = np.nonzero(
                 [self._boundaries.check(x) for x in self._xs])
             self._user_xs = self._xs[self._user_ids]
             if len(self._user_xs) == 0:     # pragma: no cover
                 warnings.warn('All PSO particles are outside the boundaries.')
-        else:
-            self._user_xs = self._xs
 
         # Update global best score
         i = np.argmin(self._fl)
         if self._fl[i] < self._fg:
             self._fg = self._fl[i]
             self._pg = np.array(self._pl[i], copy=True)
 
-    def xbest(self):
-        """ See :meth:`Optimiser.xbest()`. """
+    def x_best(self):
+        """ See :meth:`Optimiser.x_best()`. """
         if self._running:
             return np.array(self._pg, copy=True)
         return np.array(self._x0, copy=True)
+
```

### Comparing `pints-0.4.0/pints/_optimisers/_snes.py` & `pints-0.5.0/pints/_optimisers/_xnes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,134 +1,141 @@
 #
-# Seperable natural evolution strategy optimizer: SNES
+# Exponential natural evolution strategy optimizer: xNES
 #
 # This file is part of PINTS (https://github.com/pints-team/pints/) which is
 # released under the BSD 3-clause license. See accompanying LICENSE.md for
 # copyright notice and full license details.
 #
 # Some code in this file was adapted from Myokit (see http://myokit.org)
 #
 import numpy as np
 import pints
+import scipy
+import scipy.linalg
 import warnings
 
 
-class SNES(pints.PopulationBasedOptimiser):
+class XNES(pints.PopulationBasedOptimiser):
     """
-    Finds the best parameters using the SNES method described in [1]_, [2]_.
+    Finds the best parameters using the xNES method described in [1]_, [2]_.
 
-    SNES stands for Seperable Natural Evolution Strategy, and is designed for
-    non-linear derivative-free optimization problems in high dimensions and
-    with many local minima [1]_.
-
-    It treats each dimension separately, making it suitable for higher
-    dimensions.
+    xNES stands for Exponential Natural Evolution Strategy, and is
+    designed for non-linear derivative-free optimization problems [1]_.
 
     Extends :class:`PopulationBasedOptimiser`.
 
     References
     ----------
-    .. [1] Schaul, Glasmachers, Schmidhuber (2011) "High dimensions and heavy
-           tails for natural evolution strategies". Proceedings of the 13th
-           annual conference on Genetic and evolutionary computation.
-           https://doi.org/10.1145/2001576.2001692
+    .. [1] Glasmachers, Schaul, Schmidhuber et al. (2010) "Exponential natural
+           evolution strategies". Proceedings of the 12th annual conference on
+           Genetic and evolutionary computation.
+           https://doi.org/10.1145/1830483.1830557
 
     .. [2] PyBrain: The Python machine learning library
            http://pybrain.org
     """
     def __init__(self, x0, sigma0=None, boundaries=None):
-        super(SNES, self).__init__(x0, sigma0, boundaries)
+        super(XNES, self).__init__(x0, sigma0, boundaries)
 
         # Set initial state
         self._running = False
         self._ready_for_tell = False
 
-        # Best solution found
-        self._xbest = pints.vector(x0)
-        self._fbest = float('inf')
+        # Samples
+        self._zs = None       # Normalised samples
+        self._xs = None       # De-normalised samples (mu + A dot zs)
+        self._bounded_xs = None   # Subset of xs that are within the boundaries
+        self._bounded_ids = None  # Indices of those xs
+
+        # Normalisation / distribution
+        self._mu = np.array(self._x0)   # Mean
+        self._A = None                  # Covariance
+
+        # Best solution seen
+        self._x_best = pints.vector(x0)
+        self._f_best = np.inf
+
+        # Best guess of the solution is mu
+        # We don't have f(mu), so we approximate it by min f(sample)
+        self._f_guessed = np.inf
 
     def ask(self):
         """ See :meth:`Optimiser.ask()`. """
         # Initialise on first call
         if not self._running:
             self._initialise()
 
         # Ready for tell now
         self._ready_for_tell = True
 
-        # Create new samples
-        self._ss = np.array([np.random.normal(0, 1, self._n_parameters)
-                            for i in range(self._population_size)])
-        self._xs = self._mu + self._sigmas * self._ss
-
-        # Create safe xs to pass to user
-        if self._boundary_transform is not None:
-            # Rectangular boundaries? Then perform boundary transform
-            self._xs = self._boundary_transform(self._xs)
-        if self._manual_boundaries:
-            # Manual boundaries? Then pass only xs that are within bounds
-            self._user_ids = np.nonzero(
+        # Create new samples (normalised, and user values)
+        self._zs = np.array([np.random.normal(0, 1, self._n_parameters)
+                             for i in range(self._population_size)])
+        self._xs = np.array([self._mu + np.dot(self._A, self._zs[i])
+                             for i in range(self._population_size)])
+
+        # Boundaries? Then only pass user xs that are within bounds
+        if self._boundaries is not None:
+            self._bounded_ids = np.nonzero(
                 [self._boundaries.check(x) for x in self._xs])
-            self._user_xs = self._xs[self._user_ids]
-            if len(self._user_xs) == 0:     # pragma: no cover
+            self._bounded_xs = self._xs[self._bounded_ids]
+            if len(self._bounded_xs) == 0:     # pragma: no cover
                 warnings.warn(
-                    'All points requested by SNES are outside the boundaries.')
+                    'All points requested by XNES are outside the boundaries.')
         else:
-            self._user_xs = self._xs
+            self._bounded_xs = self._xs
 
         # Set as read-only and return
-        self._user_xs.setflags(write=False)
-        return self._user_xs
+        self._bounded_xs.setflags(write=False)
+        return self._bounded_xs
 
-    def fbest(self):
-        """ See :meth:`Optimiser.fbest()`. """
-        return self._fbest
+    def f_best(self):
+        """ See :meth:`Optimiser.f_best()`. """
+        return self._f_best
+
+    def f_guessed(self):
+        """ See :meth:`Optimiser.f_guessed()`. """
+        return self._f_guessed
 
     def _initialise(self):
         """
         Initialises the optimiser for the first iteration.
         """
-        assert(not self._running)
-
-        # Create boundary transform, or use manual boundary checking
-        self._manual_boundaries = False
-        self._boundary_transform = None
-        if isinstance(self._boundaries, pints.RectangularBoundaries):
-            self._boundary_transform = pints.TriangleWaveTransform(
-                self._boundaries)
-        elif self._boundaries is not None:
-            self._manual_boundaries = True
+        assert not self._running
 
         # Shorthands
         d = self._n_parameters
         n = self._population_size
 
         # Learning rates
         # TODO Allow changing before run() with method call
         self._eta_mu = 1
         # TODO Allow changing before run() with method call
-        self._eta_sigmas = 0.2 * (3 + np.log(d)) * d ** -0.5
+        self._eta_A = 0.6 * (3 + np.log(d)) * d ** -1.5
 
         # Pre-calculated utilities
         self._us = np.maximum(0, np.log(n / 2 + 1) - np.log(1 + np.arange(n)))
         self._us /= np.sum(self._us)
         self._us -= 1 / n
 
         # Center of distribution
         self._mu = np.array(self._x0, copy=True)
 
         # Initial square root of covariance matrix
-        self._sigmas = np.array(self._sigma0, copy=True)
+        self._A = np.eye(d) * self._sigma0
+
+        # Identity matrix of appropriate size
+        self._I = np.eye(d)
 
         # Update optimiser state
         self._running = True
 
     def name(self):
         """ See :meth:`Optimiser.name()`. """
-        return 'Seperable Natural Evolution Strategy (SNES)'
+        return 'Exponential Natural Evolution Strategy (xNES)'
 
     def running(self):
         """ See :meth:`Optimiser.running()`. """
         return self._running
 
     def _suggested_population_size(self):
         """ See :meth:`Optimiser._suggested_population_size(). """
@@ -136,38 +143,44 @@
 
     def tell(self, fx):
         """ See :meth:`Optimiser.tell()`. """
         if not self._ready_for_tell:
             raise Exception('ask() not called before tell()')
         self._ready_for_tell = False
 
-        # Manual boundaries? Then reconstruct full fx vector
-        if self._manual_boundaries and len(fx) < self._population_size:
-            user_fx = fx
-            fx = np.ones((self._population_size, )) * float('inf')
-            fx[self._user_ids] = user_fx
+        # Boundaries? Then reconstruct full fx vector
+        if self._boundaries is not None and len(fx) < self._population_size:
+            bounded_fx = fx
+            fx = np.ones((self._population_size, )) * np.inf
+            fx[self._bounded_ids] = bounded_fx
 
         # Order the normalized samples according to the scores
         order = np.argsort(fx)
-        self._ss = self._ss[order]
+        self._zs = self._zs[order]
 
         # Update center
-        self._mu += self._eta_mu * self._sigmas * np.dot(self._us, self._ss)
+        Gd = np.dot(self._us, self._zs)
+        self._mu += self._eta_mu * np.dot(self._A, Gd)
 
-        # Update variances
-        self._sigmas *= np.exp(
-            0.5 * self._eta_sigmas * np.dot(self._us, self._ss**2 - 1))
-
-        # Update xbest and fbest
-        # Note: The stored values are based on particles, not on the mean of
-        # all particles! This has the advantage that we don't require an extra
-        # evaluation at mu to get a pair (mu, f(mu)). The downside is that
-        # xbest isn't the very best point. However, xbest and mu seem to
-        # converge quite quickly, so that this difference disappears.
-        if fx[order[0]] < self._fbest:
-            self._xbest = self._xs[order[0]]
-            self._fbest = fx[order[0]]
-
-    def xbest(self):
-        """ See :meth:`Optimiser.xbest()`. """
-        return self._xbest
+        # Update root of covariance matrix
+        Gm = np.dot(
+            np.array([np.outer(z, z).T - self._I for z in self._zs]).T,
+            self._us)
+        self._A *= scipy.linalg.expm(np.dot(0.5 * self._eta_A, Gm))
+
+        # Update f_guessed on the assumption that the lowest value in our
+        # sample approximates f(mu)
+        self._f_guessed = fx[order[0]]
+
+        # Update x_best and f_best
+        if self._f_guessed < self._f_best:
+            self._x_best = np.array(self._xs[order[0]], copy=True)
+            self._f_best = fx[order[0]]
+
+    def x_best(self):
+        """ See :meth:`Optimiser.x_best()`. """
+        return self._x_best
+
+    def x_guessed(self):
+        """ See :meth:`Optimiser.x_guessed()`. """
+        return np.array(self._mu, copy=True)
```

### Comparing `pints-0.4.0/pints/_optimisers/_xnes.py` & `pints-0.5.0/pints/_optimisers/_snes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,136 +1,132 @@
 #
-# Exponential natural evolution strategy optimizer: xNES
+# Seperable natural evolution strategy optimizer: SNES
 #
 # This file is part of PINTS (https://github.com/pints-team/pints/) which is
 # released under the BSD 3-clause license. See accompanying LICENSE.md for
 # copyright notice and full license details.
 #
 # Some code in this file was adapted from Myokit (see http://myokit.org)
 #
 import numpy as np
 import pints
-import scipy
-import scipy.linalg
 import warnings
 
 
-class XNES(pints.PopulationBasedOptimiser):
+class SNES(pints.PopulationBasedOptimiser):
     """
-    Finds the best parameters using the xNES method described in [1]_, [2]_.
+    Finds the best parameters using the SNES method described in [1]_, [2]_.
 
-    xNES stands for Exponential Natural Evolution Strategy, and is
-    designed for non-linear derivative-free optimization problems [1]_.
+    SNES stands for Seperable Natural Evolution Strategy, and is designed for
+    non-linear derivative-free optimization problems in high dimensions and
+    with many local minima [1]_.
+
+    It treats each dimension separately, making it suitable for higher
+    dimensions.
 
     Extends :class:`PopulationBasedOptimiser`.
 
     References
     ----------
-    .. [1] Glasmachers, Schaul, Schmidhuber et al. (2010) "Exponential natural
-           evolution strategies". Proceedings of the 12th annual conference on
-           Genetic and evolutionary computation.
-           https://doi.org/10.1145/1830483.1830557
+    .. [1] Schaul, Glasmachers, Schmidhuber (2011) "High dimensions and heavy
+           tails for natural evolution strategies". Proceedings of the 13th
+           annual conference on Genetic and evolutionary computation.
+           https://doi.org/10.1145/2001576.2001692
 
     .. [2] PyBrain: The Python machine learning library
            http://pybrain.org
     """
     def __init__(self, x0, sigma0=None, boundaries=None):
-        super(XNES, self).__init__(x0, sigma0, boundaries)
+        super(SNES, self).__init__(x0, sigma0, boundaries)
 
         # Set initial state
         self._running = False
         self._ready_for_tell = False
 
+        # Mean
+        self._mu = np.array(self._x0, copy=True)
+
         # Best solution found
-        self._xbest = pints.vector(x0)
-        self._fbest = float('inf')
+        self._x_best = pints.vector(x0)
+        self._f_best = np.inf
+
+        # Best guess of the solution is mu
+        # We don't have f(mu), so we approximate it by max f(sample)
+        self._f_guessed = np.inf
 
     def ask(self):
         """ See :meth:`Optimiser.ask()`. """
         # Initialise on first call
         if not self._running:
             self._initialise()
 
         # Ready for tell now
         self._ready_for_tell = True
 
-        # Create new samples (normalised, and user values)
-        self._zs = np.array([np.random.normal(0, 1, self._n_parameters)
-                             for i in range(self._population_size)])
-        self._xs = np.array([self._mu + np.dot(self._A, self._zs[i])
-                             for i in range(self._population_size)])
-
-        # Create safe xs to pass to user
-        if self._boundary_transform is not None:
-            # Rectangular boundaries? Then perform boundary transform
-            self._xs = self._boundary_transform(self._xs)
-        if self._manual_boundaries:
-            # Manual boundaries? Then pass only xs that are within bounds
+        # Create new samples
+        self._ss = np.array([np.random.normal(0, 1, self._n_parameters)
+                            for i in range(self._population_size)])
+        self._xs = self._mu + self._sigmas * self._ss
+
+        # Boundaries? Then only pass user xs that are within bounds
+        if self._boundaries is not None:
             self._user_ids = np.nonzero(
                 [self._boundaries.check(x) for x in self._xs])
             self._user_xs = self._xs[self._user_ids]
             if len(self._user_xs) == 0:     # pragma: no cover
                 warnings.warn(
-                    'All points requested by XNES are outside the boundaries.')
+                    'All points requested by SNES are outside the boundaries.')
         else:
             self._user_xs = self._xs
 
         # Set as read-only and return
         self._user_xs.setflags(write=False)
         return self._user_xs
 
-    def fbest(self):
-        """ See :meth:`Optimiser.fbest()`. """
-        return self._fbest
+    def f_best(self):
+        """ See :meth:`Optimiser.f_best()`. """
+        return self._f_best
+
+    def f_guessed(self):
+        """ See :meth:`Optimiser.f_guessed()`. """
+        return self._f_guessed
 
     def _initialise(self):
         """
         Initialises the optimiser for the first iteration.
         """
-        assert(not self._running)
-
-        # Create boundary transform, or use manual boundary checking
-        self._manual_boundaries = False
-        self._boundary_transform = None
-        if isinstance(self._boundaries, pints.RectangularBoundaries):
-            self._boundary_transform = pints.TriangleWaveTransform(
-                self._boundaries)
-        elif self._boundaries is not None:
-            self._manual_boundaries = True
+        assert not self._running
 
         # Shorthands
         d = self._n_parameters
         n = self._population_size
 
         # Learning rates
         # TODO Allow changing before run() with method call
         self._eta_mu = 1
         # TODO Allow changing before run() with method call
-        self._eta_A = 0.6 * (3 + np.log(d)) * d ** -1.5
+        self._eta_sigmas = 0.2 * (3 + np.log(d)) * d ** -0.5
 
         # Pre-calculated utilities
         self._us = np.maximum(0, np.log(n / 2 + 1) - np.log(1 + np.arange(n)))
         self._us /= np.sum(self._us)
         self._us -= 1 / n
 
         # Center of distribution
         self._mu = np.array(self._x0, copy=True)
 
         # Initial square root of covariance matrix
-        self._A = np.eye(d) * self._sigma0
-
-        # Identity matrix of appropriate size
-        self._I = np.eye(d)
+        self._sigmas = np.array(self._sigma0, copy=True)
 
         # Update optimiser state
         self._running = True
 
     def name(self):
         """ See :meth:`Optimiser.name()`. """
-        return 'Exponential Natural Evolution Strategy (xNES)'
+        return 'Seperable Natural Evolution Strategy (SNES)'
 
     def running(self):
         """ See :meth:`Optimiser.running()`. """
         return self._running
 
     def _suggested_population_size(self):
         """ See :meth:`Optimiser._suggested_population_size(). """
@@ -138,41 +134,41 @@
 
     def tell(self, fx):
         """ See :meth:`Optimiser.tell()`. """
         if not self._ready_for_tell:
             raise Exception('ask() not called before tell()')
         self._ready_for_tell = False
 
-        # Manual boundaries? Then reconstruct full fx vector
-        if self._manual_boundaries and len(fx) < self._population_size:
+        # Boundaries? Then reconstruct full fx vector
+        if self._boundaries is not None and len(fx) < self._population_size:
             user_fx = fx
-            fx = np.ones((self._population_size, )) * float('inf')
+            fx = np.ones((self._population_size, )) * np.inf
             fx[self._user_ids] = user_fx
 
         # Order the normalized samples according to the scores
         order = np.argsort(fx)
-        self._zs = self._zs[order]
+        self._ss = self._ss[order]
 
         # Update center
-        Gd = np.dot(self._us, self._zs)
-        self._mu += self._eta_mu * np.dot(self._A, Gd)
+        self._mu += self._eta_mu * self._sigmas * np.dot(self._us, self._ss)
 
-        # Update xbest and fbest
-        # Note: The stored values are based on particles, not on the mean of
-        # all particles! This has the advantage that we don't require an extra
-        # evaluation at mu to get a pair (mu, f(mu)). The downside is that
-        # xbest isn't the very best point. However, xbest and mu seem to
-        # converge quite quickly, so that this difference disappears.
-        if fx[order[0]] < self._fbest:
-            self._xbest = self._xs[order[0]]
-            self._fbest = fx[order[0]]
-
-        # Update root of covariance matrix
-        Gm = np.dot(
-            np.array([np.outer(z, z).T - self._I for z in self._zs]).T,
-            self._us)
-        self._A *= scipy.linalg.expm(np.dot(0.5 * self._eta_A, Gm))
-
-    def xbest(self):
-        """ See :meth:`Optimiser.xbest()`. """
-        return self._xbest
+        # Update variances
+        self._sigmas *= np.exp(
+            0.5 * self._eta_sigmas * np.dot(self._us, self._ss**2 - 1))
+
+        # Update f_guessed on the assumption that the lowest value in our
+        # sample approximates f(mu)
+        self._f_guessed = fx[order[0]]
+
+        # Update x_best and f_best
+        if self._f_guessed < self._f_best:
+            self._x_best = np.array(self._xs[order[0]], copy=True)
+            self._f_best = fx[order[0]]
+
+    def x_best(self):
+        """ See :meth:`Optimiser.x_best()`. """
+        return self._x_best
+
+    def x_guessed(self):
+        """ See :meth:`Optimiser.x_guessed()`. """
+        return np.array(self._mu, copy=True)
```

### Comparing `pints-0.4.0/pints/_sample_initial_points.py` & `pints-0.5.0/pints/_sample_initial_points.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/_transformation.py` & `pints-0.5.0/pints/_transformation.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,17 @@
         """
         return TransformedErrorMeasure(error_measure, self)
 
     def convert_boundaries(self, boundaries):
         """
         Returns a transformed boundaries class.
         """
+        if isinstance(boundaries, pints.RectangularBoundaries):
+            if self.elementwise():
+                return TransformedRectangularBoundaries(boundaries, self)
         return TransformedBoundaries(boundaries, self)
 
     def convert_covariance_matrix(self, C, q):
         r"""
         Converts a convariance matrix ``C`` from the model space to the search
         space around a parameter vector ``q`` provided in the search space.
 
@@ -752,14 +755,16 @@
                                                                    [4, 5, 6])
 
     or::
 
         boundaries = pints.RectangularBoundaries([0, 1, 2], [4, 5, 6])
         transformation = pints.RectangularBoundariesTransformation(boundaries)
 
+    Not to be confused with :class:`pints.TransformedRectangularBoundaries`.
+
     Extends :class:`Transformation`.
     """
     def __init__(self, lower_or_boundaries, upper=None):
         # Parse input arguments
         if upper is None:
             if not isinstance(lower_or_boundaries,
                               pints.RectangularBoundaries):
@@ -774,15 +779,15 @@
                                                      upper)
 
         self._a = boundaries.lower()
         self._b = boundaries.upper()
 
         # Cache dimension
         self._n_parameters = boundaries.n_parameters()
-        del(boundaries)
+        del boundaries
 
     def elementwise(self):
         """ See :meth:`Transformation.elementwise()`. """
         return True
 
     def jacobian(self, q):
         """ See :meth:`Transformation.jacobian()`. """
@@ -830,59 +835,78 @@
     def _softplus(self, q):
         """ Returns the softplus function. """
         return np.log(1. + np.exp(q))
 
 
 class ScalingTransformation(Transformation):
     """
-    Scaling transformation scales the input parameters by multiplying with an
-    array ``scalings`` element-wisely. And its Jacobian matrix is a diagonal
-    matrix with the values of ``1 / scalings`` on the diagonal.
+    Scales the input parameters by multiplying with an array ``scalings`` and
+    adding an optional array ``translation``.
+
+    The transformation from model parameters ``p`` to search parameters ``q``
+    is performed as::
+
+        q = (p + translation) * scalings
+
+    Its Jacobian matrix is a diagonal matrix with ``1 / scalings`` on the
+    diagonal.
 
     Extends :class:`Transformation`.
     """
-    def __init__(self, scalings):
-        self.s = pints.vector(scalings)
-        self.inv_s = 1. / self.s
-        self._n_parameters = len(self.s)
+    def __init__(self, scalings, translation=None):
+        self._s = pints.vector(scalings)
+        self._inv_s = 1. / self._s
+        self._n_parameters = len(self._s)
+
+        self._translation = None
+        if translation is not None:
+            self._translation = pints.vector(translation)
+            if len(self._translation) != self._n_parameters:
+                raise ValueError(
+                    'Translation must be None or be a vector of the same'
+                    ' length as the scalings.')
 
     def elementwise(self):
         """ See :meth:`Transformation.elementwise()`. """
         return True
 
     def jacobian(self, q):
         """ See :meth:`Transformation.jacobian()`. """
-        return np.diag(self.inv_s)
+        return np.diag(self._inv_s)
 
     def jacobian_S1(self, q):
         """ See :meth:`Transformation.jacobian_S1()`. """
         n = self._n_parameters
         return self.jacobian(q), np.zeros((n, n, n))
 
     def log_jacobian_det(self, q):
         """ See :meth:`Transformation.log_jacobian_det()`. """
-        return np.sum(np.log(np.abs(self.inv_s)))
+        return np.sum(np.log(np.abs(self._inv_s)))
 
     def log_jacobian_det_S1(self, q):
         """ See :meth:`Transformation.log_jacobian_det_S1()`. """
         return self.log_jacobian_det(q), np.zeros(self._n_parameters)
 
     def n_parameters(self):
         """ See :meth:`Transformation.n_parameters()`. """
         return self._n_parameters
 
     def to_model(self, q):
         """ See :meth:`Transformation.to_model()`. """
-        q = pints.vector(q)
-        return self.inv_s * q
+        p = self._inv_s * pints.vector(q)
+        if self._translation is not None:
+            p -= self._translation
+        return p
 
     def to_search(self, p):
         """ See :meth:`Transformation.to_search()`. """
         p = pints.vector(p)
-        return self.s * p
+        if self._translation is not None:
+            p = p + self._translation
+        return self._s * p
 
 
 class TransformedBoundaries(pints.Boundaries):
     """
     A :class:`pints.Boundaries` that accepts parameters in a transformed
     search space.
 
@@ -911,21 +935,76 @@
         # Check Boundaries in the model space
         return self._boundaries.check(p)
 
     def n_parameters(self):
         """ See :meth:`Boundaries.n_parameters()`. """
         return self._n_parameters
 
-    def range(self):
-        """
-        Returns the size of the search space (i.e. ``upper - lower``).
-        """
-        upper = self._transform.to_search(self._boundaries.upper())
-        lower = self._transform.to_search(self._boundaries.lower())
-        return upper - lower
+    def sample(self, n=1):
+        """ See :meth:`Boundaries.sample()`. """
+        return [
+            self._transform.to_search(p) for p in self._boundaries.sample(n)]
+
+
+class TransformedRectangularBoundaries(pints.RectangularBoundaries):
+    """
+    A :class:`pints.RectangularBoundaries` that accepts parameters in a
+    transformed search space.
+
+    This transformation handles the special case where:
+
+    - the boundaries being transformed are :class:`pints.RectangularBoundaries`
+    - the transformation is element-wise.
+
+    When these conditions are met, the lower and upper boundaries can simply be
+    transformed and methods like :meth:`lower()` and :meth:`range()` can be
+    provided.
+
+    Not to be confused with :class:`pints.RectangularBoundariesTransformation`.
+
+    Extends :class:`pints.RectangularBoundaries`.
+
+    Parameters
+    ----------
+    boundaries
+        A :class:`pints.RectangularBoundaries` object.
+    transformation
+        An element-wise transformation.
+    """
+    def __init__(self, boundaries, transformation):
+
+        # Check input
+        if not isinstance(boundaries, pints.RectangularBoundaries):
+            raise ValueError('A TransformedRectangularBoundaries can only be'
+                             ' created from a RectangularBoundaries object.')
+        if not transformation.elementwise():
+            raise ValueError('A TransformedRectangularBoundaries can only be'
+                             ' created from an element-wise transformation.')
+        if transformation.n_parameters() != boundaries.n_parameters():
+            raise ValueError('Number of parameters for boundaries and '
+                             'transformation must match.')
+
+        # Transform upper and lower boundaries
+        a = transformation.to_search(boundaries.lower())
+        b = transformation.to_search(boundaries.upper())
+        lower = np.minimum(a, b)
+        upper = np.maximum(a, b)
+
+        # Pass transformed boundaries to RectangularBoundaries
+        super().__init__(lower, upper)
+
+        # Store input
+        self._boundaries = boundaries
+        self._transformation = transformation
+
+    def sample(self, n=1):
+        """ See :meth:`Boundaries.sample()`. """
+        # Sample from the original boundaries, but transform to new space
+        return [self._transformation.to_search(p)
+                for p in self._boundaries.sample(n)]
 
 
 class TransformedErrorMeasure(pints.ErrorMeasure):
     r"""
     A :class:`pints.ErrorMeasure` that accepts parameters in a transformed
     search space.
 
@@ -1127,7 +1206,36 @@
         simply transforms the samples from the original log-prior.*
         """
         ps = self._log_pdf.sample(n)
         qs = np.zeros(ps.shape)
         for i, p in enumerate(ps):
             qs[i, :] = self._transform.to_search(p)
         return qs
+
+
+class UnitCubeTransformation(ScalingTransformation):
+    """
+    Maps a parameter space onto the unit (hyper)cube.
+
+    Transformations from model parameters ``p`` to search parameters ``q`` are
+    made as::
+
+        q = (p - lower) / (upper - lower)
+
+    Extends :class:`ScalingTransformation`.
+    """
+    def __init__(self, lower, upper):
+
+        # Check input
+        self._lower = pints.vector(lower)
+        self._upper = pints.vector(upper)
+        self._n_parameters = len(lower)
+        del lower, upper
+
+        if len(self._upper) != self._n_parameters:
+            raise ValueError(
+                'Lower and upper bounds must have the same length.')
+        if not np.all(self._upper > self._lower):
+            raise ValueError('Upper bounds must exceed lower bounds.')
+
+        super().__init__(1 / (self._upper - self._lower), -self._lower)
+
```

### Comparing `pints-0.4.0/pints/_util.py` & `pints-0.5.0/pints/_util.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/interfaces/stan/_stan.py` & `pints-0.5.0/pints/toy/_cone.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,122 +1,153 @@
 #
-# LogPDF that uses Stan models.
+# Cone toy log pdf.
 #
 # This file is part of PINTS (https://github.com/pints-team/pints/) which is
 # released under the BSD 3-clause license. See accompanying LICENSE.md for
 # copyright notice and full license details.
 #
 import numpy as np
-import pystan
-import pints
-import warnings
-
-
-class StanLogPDF(pints.LogPDF):
-    def __init__(self, stan_code, stan_data=None):
-        """
-        Creates a :class:`pints.LogPDF` object from Stan code and data, which
-        can then be used in sampling, optimisation etc.
-
-        This class uses Pystan to interface with Stan, which compiles the Stan
-        model code (see [1]_). This can take some time (typically minutes).
-
-        Note that the interface assumes that the parameters are on the
-        unconstrained scale (according to Stan's "constraint transforms" [1]_).
-        So, for example, if a variable is declared to have a lower bound of
-        zero, sampling happens on the log-transformed space. The interface
-        takes care of Jacobian transformations, so a user only needs to
-        transform the variable back to the constrained space (in the example,
-        using a ``exp`` transform) to obtain appropriate samples.
-
-        Parameters are ordered as in the stan model. Vector and matrix
-        parameters are "flattened" into a sequence by Stan, use
-        :meth:`StanLogPDF.names()` to see the result.
-
-        Extends :class:`pints.LogPDF`.
-
-        Parameters
-        ----------
-        stan_code
-            Stan code describing the model.
-        stan_data
-            Data in Python dictionary format as required by PyStan. Defaults to
-            None in which case ``update_data`` must be called to create a valid
-            Stan model fit object before calling.
-
-        References
-        ----------
-        .. [1] "Stan: a probabilistic programming language".
-               B Carpenter et al., (2017), Journal of Statistical Software
-        """
-        self._fit = None
-        self._log_prob = None
-        self._grad_log_prob = None
-        self._n_parameters = None
-        self._names = None
-
-        # compile stan
-        self._compiled_stan = pystan.StanModel(model_code=stan_code)
-
-        # only create stanfit if data supplied
-        if stan_data is not None:
-            self.update_data(stan_data)
+import scipy
+
+from . import ToyLogPDF
+
+
+class ConeLogPDF(ToyLogPDF):
+    r"""
+    Toy distribution based on a d-dimensional distribution of the form,
+
+    .. math::
+
+        f(x) \propto e^{-|x|^\beta}
+
+    where ``x`` is a d-dimensional real, and ``|x|`` is the Euclidean norm. The
+    mean and variance that are returned relate to expectations on ``|x|`` not
+    the multidimensional ``x``.
+
+    Extends :class:`pints.LogPDF`.
+
+    Parameters
+    ----------
+    dimensions : int
+        The dimensionality of the cone.
+    beta : float
+        The power to which ``|x|`` is raised in the exponential term, which
+        must be positive.
+    """
+    def __init__(self, dimensions=2, beta=1):
+        if dimensions < 1:
+            raise ValueError('Dimensions must not be less than 1.')
+        self._n_parameters = int(dimensions)
+        beta = float(beta)
+        if beta <= 0:
+            raise ValueError('beta must be positive.')
+        self._beta = beta
+
+    def beta(self):
+        """
+        Returns the exponent in the pdf
+        """
+        return self._beta
 
     def __call__(self, x):
-        if self._fit is None:
-            raise RuntimeError(
-                'No data supplied to create Stan model fit object. '
-                'Run `update_data` first.')
-        vals = x
-        try:
-            return self._log_prob(vals, adjust_transform=True)
-        # if Pints proposes a value outside of Stan's parameter bounds
-        except (RuntimeError, ValueError) as e:
-            warnings.warn('RuntimeError or ValueError encountered when '
-                          'calling `pints.LogPDF`: ' + str(e))
-            return -np.inf
+        if not len(x) == self._n_parameters:
+            raise ValueError('x must be of same dimensions as density')
+        return -np.linalg.norm(x)**self._beta
+
+    def CDF(self, x):
+        """
+        Returns the cumulative density function in terms of ``|x|``.
+        """
+        x = float(x)
+        if x < 0:
+            raise ValueError('Normed distance must be non-negative.')
+        n = self._n_parameters
+        beta = self._beta
+        if x == 0:
+            return 0
+        else:
+            return (-(x**n) * ((x**beta)**(-(n / beta))) *
+                    scipy.special.gammaincc(n / beta, x**beta) + 1)
+
+    def distance(self, samples):
+        """
+        Calculates a measure of normed distance of samples from exact mean and
+        covariance matrix assuming uniform prior with bounds given by
+        :meth:`suggested_bounds()`.
+
+        See :meth:`pints.toy.ToyLogPDF.distance()`.
+        """
+        # Check size of input
+        if not len(samples.shape) == 2:
+            raise ValueError('Given samples list must be n x 2.')
+        if samples.shape[1] != self.n_parameters():
+            raise ValueError(
+                'Given samples must have length ' +
+                str(self.n_parameters()))
+        # calculate normed distance
+        d = list(map(lambda x: np.linalg.norm(x), samples))
+        diff = (
+            np.abs(self.mean_normed() - np.mean(d)) +
+            np.abs(self.var_normed() - np.var(d))
+        )
+        return diff
 
     def evaluateS1(self, x):
         """ See :meth:`LogPDF.evaluateS1()`. """
-        if self._fit is None:
-            raise RuntimeError(
-                'No data supplied to create Stan model fit object. '
-                'Run `update_data` first.')
-        try:
-            val = self._log_prob(x, adjust_transform=True)
-            dp = self._grad_log_prob(x, adjust_transform=True)
-            return val, dp.reshape(-1)
-        except (RuntimeError, ValueError) as e:
-            warnings.warn('RuntimeError or ValueError encountered when '
-                          'calling `pints.LogPDF`: ' + str(e))
-            return -np.inf, np.ones(self._n_parameters)
-
-    def names(self):
-        """ Returns names of Stan parameters. """
-        return self._names
+        L = self.__call__(x)
+
+        norm = np.linalg.norm(x)**2
+        norm = self._beta * norm**(-1.0 + self._beta / 2.0)
+        dL = np.array([-var * norm for var in x])
+        return L, dL
+
+    def mean_normed(self):
+        """
+        Returns the mean of the normed distance from the origin
+        """
+        g1 = scipy.special.gamma((1 + self._n_parameters) / self._beta)
+        g2 = scipy.special.gamma(self._n_parameters / self._beta)
+        return g1 / g2
 
     def n_parameters(self):
-        """ See `pints.LogPDF.n_parameters`. """
         return self._n_parameters
 
-    def update_data(self, stan_data):
-        """
-        Updates data passed to the underlying Stan model.
+    def sample(self, n_samples):
+        """ See :meth:`ToyLogPDF.sample()`. """
+        n_samples = int(n_samples)
+        if n_samples < 1:
+            raise ValueError(
+                'Number of samples must be greater than or equal to 1.')
+        n = self._n_parameters
+
+        # Determine empirical inverse-CDF
+        x_max = scipy.optimize.minimize(lambda x: (
+            np.abs((self.CDF(x) - 1))), 8)['x'][0] * 10
+        x_range = np.linspace(0, x_max, 100)
+        cdf = [self.CDF(x) for x in x_range]
+        f = scipy.interpolate.interp1d(cdf, x_range)
+
+        # Do inverse-transform sampling to obtain independent r samples
+        u = np.random.rand(n_samples)
+        r = f(u)
+
+        # For each value of r select a value uniformly at random on
+        # hypersphere of that radius
+        X_norm = np.random.normal(size=(n_samples, n))
+        lambda_x = np.sqrt(np.sum(X_norm**2, axis=1))
+        x_unit = [r[i] * X_norm[i] / y for i, y in enumerate(lambda_x)]
+        return np.array(x_unit)
+
+    def suggested_bounds(self):
+        """ See :meth:`ToyLogPDF.suggested_bounds()`. """
+        magnitude = 1000
+        bounds = np.tile([-magnitude, magnitude], (self._n_parameters, 1))
+        return np.transpose(bounds).tolist()
 
-        Parameters
-        ----------
-        stan_data
-            Data in Python dictionary format as required by PyStan.
-        """
-        self._fit = self._compiled_stan.sampling(
-            data=stan_data,
-            iter=1,
-            chains=1,
-            verbose=False,
-            refresh=0,
-            control={'adapt_engaged': False})
-
-        self._log_prob = self._fit.log_prob
-        self._grad_log_prob = self._fit.grad_log_prob
-        self._names = self._fit.unconstrained_param_names()
-        self._n_parameters = len(self._names)
+    def var_normed(self):
+        """
+        Returns the variance of the normed distance from the origin.
+        """
+        g1 = scipy.special.gamma((2 + self._n_parameters) / self._beta)
+        g2 = scipy.special.gamma(self._n_parameters / self._beta)
+        return g1 / g2 - self.mean_normed()**2
```

### Comparing `pints-0.4.0/pints/io.py` & `pints-0.5.0/pints/io.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/noise.py` & `pints-0.5.0/pints/noise.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/plot/__init__.py` & `pints-0.5.0/pints/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/plot/_autocorrelation.py` & `pints-0.5.0/pints/plot/_autocorrelation.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/plot/_function.py` & `pints-0.5.0/pints/plot/_function.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/plot/_function_between_points.py` & `pints-0.5.0/pints/plot/_function_between_points.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/plot/_histogram.py` & `pints-0.5.0/pints/plot/_histogram.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,33 +52,26 @@
         < LooseVersion("2.2")
 
     # If we switch to Python3 exclusively, bins and alpha can be keyword-only
     # arguments
     bins = 40
     alpha = 0.5
 
-    samples = np.asarray(samples)
+    samples = np.array(samples)
     n_list = len(samples)
     _, n_param = samples[0].shape
 
     # Check parameter names
     if parameter_names is None:
         parameter_names = ['Parameter' + str(i + 1) for i in range(n_param)]
     elif len(parameter_names) != n_param:
         raise ValueError(
             'Length of `parameter_names` must be same as number of'
             ' parameters.')
 
-    # Check number of parameters
-    for samples_j in samples:
-        if n_param != samples_j.shape[1]:
-            raise ValueError(
-                'All samples must have the same number of parameters.'
-            )
-
     # Check reference parameters
     if ref_parameters is not None:
         if len(ref_parameters) != n_param:
             raise ValueError(
                 'Length of `ref_parameters` must be same as number of'
                 ' parameters.')
```

### Comparing `pints-0.4.0/pints/plot/_pairwise.py` & `pints-0.5.0/pints/plot/_pairwise.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,25 +39,24 @@
         is the number of parameters.
     kde
         Set to ``True`` to use kernel-density estimation for the
         histograms and scatter plots. Cannot use together with ``heatmap``.
     heatmap
         Set to ``True`` to plot heatmap for the pairwise plots.
         Cannot be used together with ``kde``.
-    Opacity
+    opacity
         This value can be used to manually set the opacity of the
         points in the scatter plots (when ``kde=False`` and ``heatmap=False``
         only).
     n_percentiles
         Shows only the middle n-th percentiles of the distribution.
         Default shows all samples in ``samples``.
     parameter_names
-        A list of parameter names, which will be displayed on the x-axis of the
-        trace subplots. If no names are provided, the parameters are
-        enumerated.
+        A list of parameter names, which will be displayed on the axes of the
+        subplots. If no names are provided, the parameters are enumerated.
     ref_parameters
         A set of parameters for reference in the plot. For example,
         if true values of parameters are known, they can be passed in for
         plotting.
     """
     import matplotlib
     import matplotlib.pyplot as plt
```

### Comparing `pints-0.4.0/pints/plot/_series.py` & `pints-0.5.0/pints/plot/_series.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/plot/_surface.py` & `pints-0.5.0/pints/plot/_surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     if len(values) != n:
         raise ValueError(
             'The number of values must match the number of points.')
 
     # Extract x and y points
     x = points[:, 0]
     y = points[:, 1]
-    del(points)
+    del points
 
     # Check boundaries
     if boundaries is None:
         xmin, xmax = np.min(x), np.max(x)
         r = 0.1 * (xmax - xmin)
         xmin -= r
         xmax += r
```

### Comparing `pints-0.4.0/pints/plot/_trace.py` & `pints-0.5.0/pints/plot/_trace.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/residuals_diagnostics.py` & `pints-0.5.0/pints/residuals_diagnostics.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/__init__.py` & `pints-0.5.0/pints/toy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,9 +28,7 @@
 from ._parabola import ParabolicError
 from ._repressilator_model import RepressilatorModel
 from ._rosenbrock import RosenbrockError, RosenbrockLogPDF
 from ._sho_model import SimpleHarmonicOscillatorModel
 from ._simple_egg_box import SimpleEggBoxLogPDF
 from ._sir_model import SIRModel
 from ._twisted_gaussian_banana import TwistedGaussianLogPDF
-from ._stochastic_degradation_model import StochasticDegradationModel
-from ._stochastic_logistic_model import StochasticLogisticModel
```

### Comparing `pints-0.4.0/pints/toy/_annulus.py` & `pints-0.5.0/pints/toy/_annulus.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_beeler_reuter_model.py` & `pints-0.5.0/pints/toy/_beeler_reuter_model.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_cone.py` & `pints-0.5.0/pints/toy/_neals_funnel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,153 +1,142 @@
 #
-# Cone toy log pdf.
+# Neal's funnel log pdf.
 #
 # This file is part of PINTS (https://github.com/pints-team/pints/) which is
 # released under the BSD 3-clause license. See accompanying LICENSE.md for
 # copyright notice and full license details.
 #
 import numpy as np
 import scipy
+import scipy.stats
 
 from . import ToyLogPDF
 
 
-class ConeLogPDF(ToyLogPDF):
+class NealsFunnelLogPDF(ToyLogPDF):
     r"""
     Toy distribution based on a d-dimensional distribution of the form,
 
     .. math::
 
-        f(x) \propto e^{-|x|^\beta}
+        f(x_1, x_2,...,x_d,\nu) =
+            \left[\prod_{i=1}^d\mathcal{N}(x_i|0,e^{\nu/2})\right] \times
+            \mathcal{N}(\nu|0,3)
 
-    where ``x`` is a d-dimensional real, and ``|x|`` is the Euclidean norm. The
-    mean and variance that are returned relate to expectations on ``|x|`` not
-    the multidimensional ``x``.
+    where ``x`` is a d-dimensional real. This distribution was introduced in
+    [1]_.
 
-    Extends :class:`pints.LogPDF`.
+    Extends :class:`pints.toy.ToyLogPDF`.
 
     Parameters
     ----------
     dimensions : int
-        The dimensionality of the cone.
-    beta : float
-        The power to which ``|x|`` is raised in the exponential term, which
-        must be positive.
+        The dimensionality of funnel (by default equal to 10) which must
+        exceed 1.
+
+    References
+    ----------
+    .. [1] "Slice sampling". R. Neal, Annals of statistics, 705 (2003)
+           https://doi.org/10.1214/aos/1056562461
     """
-    def __init__(self, dimensions=2, beta=1):
-        if dimensions < 1:
-            raise ValueError('Dimensions must not be less than 1.')
+    def __init__(self, dimensions=10):
+        if dimensions < 2:
+            raise ValueError('Dimensions must exceed 1.')
         self._n_parameters = int(dimensions)
-        beta = float(beta)
-        if beta <= 0:
-            raise ValueError('beta must be positive.')
-        self._beta = beta
-
-    def beta(self):
-        """
-        Returns the exponent in the pdf
-        """
-        return self._beta
+        self._s1 = 9.0
+        self._s1_inv = 1.0 / self._s1
+        self._m1 = 0
 
     def __call__(self, x):
-        if not len(x) == self._n_parameters:
-            raise ValueError('x must be of same dimensions as density')
-        return -np.linalg.norm(x)**self._beta
-
-    def CDF(self, x):
-        """
-        Returns the cumulative density function in terms of ``|x|``.
-        """
-        x = float(x)
-        if x < 0:
-            raise ValueError('Normed distance must be non-negative.')
-        n = self._n_parameters
-        beta = self._beta
-        if x == 0:
-            return 0
-        else:
-            return (-(x**n) * ((x**beta)**(-(n / beta))) *
-                    scipy.special.gammaincc(n / beta, x**beta) + 1)
+        if len(x) != self._n_parameters:
+            raise ValueError(
+                'Length of x must be equal number of parameters')
+        nu = x[-1]
+        x_temp = x[:-1]
+        x_log_pdf = [scipy.stats.norm.logpdf(y, 0, np.exp(nu / 2))
+                     for y in x_temp]
+        return np.sum(x_log_pdf) + scipy.stats.norm.logpdf(nu, 0, 3)
 
     def distance(self, samples):
-        """
-        Calculates a measure of normed distance of samples from exact mean and
-        covariance matrix assuming uniform prior with bounds given by
-        :meth:`suggested_bounds()`.
+        """ See :meth:`pints.toy.ToyLogPDF.distance()`. """
+        return self.kl_divergence(samples)
 
-        See :meth:`pints.toy.ToyLogPDF.distance()`.
+    def evaluateS1(self, x):
+        """ See :meth:`LogPDF.evaluateS1()`. """
+        L = self.__call__(x)
+
+        nu = x[-1]
+        x_temp = x[:-1]
+        cons = np.exp(-nu)
+        dnu_first = [0.5 * (cons * var**2 - 1) for var in x_temp]
+        dnu = np.sum(dnu_first) - nu / 9.0
+        dL = [-var * cons for var in x_temp]
+        dL.append(dnu)
+        dL = np.array(dL)
+        return L, dL
+
+    def kl_divergence(self, samples):
+        r"""
+        Calculates the KL divergence of samples of the :math:`nu` parameter
+        of Neal's funnel from the analytic :math:`\mathcal{N}(0, 3)` result.
         """
         # Check size of input
         if not len(samples.shape) == 2:
             raise ValueError('Given samples list must be n x 2.')
-        if samples.shape[1] != self.n_parameters():
+        if samples.shape[1] != self._n_parameters:
             raise ValueError(
-                'Given samples must have length ' +
-                str(self.n_parameters()))
-        # calculate normed distance
-        d = list(map(lambda x: np.linalg.norm(x), samples))
-        diff = (
-            np.abs(self.mean_normed() - np.mean(d)) +
-            np.abs(self.var_normed() - np.var(d))
+                'Given samples must have length ' + str(self._n_parameters))
+        nu = samples[:, self._n_parameters - 1]
+        m0 = np.mean(nu)
+        s0 = np.var(nu)
+
+        return 0.5 * (np.sum(self._s1_inv * s0) +
+                      (self._m1 - m0) * self._s1_inv * (self._m1 - m0) -
+                      np.log(s0) +
+                      np.log(self._s1) -
+                      1)
+
+    def marginal_log_pdf(self, x, nu):
+        r"""
+        Yields the marginal density :math:`\text{log } p(x_i,\nu)`.
+        """
+        return (
+            scipy.stats.norm.logpdf(x, 0, np.exp(nu / 2)) +
+            scipy.stats.norm.logpdf(nu, 0, 3)
         )
-        return diff
-
-    def evaluateS1(self, x):
-        """ See :meth:`LogPDF.evaluateS1()`. """
-        L = self.__call__(x)
-
-        norm = np.linalg.norm(x)**2
-        norm = self._beta * norm**(-1.0 + self._beta / 2.0)
-        dL = np.array([-var * norm for var in x])
-        return L, dL
 
-    def mean_normed(self):
+    def mean(self):
         """
-        Returns the mean of the normed distance from the origin
+        Returns the mean of the target distribution in each dimension.
         """
-        g1 = scipy.special.gamma((1 + self._n_parameters) / self._beta)
-        g2 = scipy.special.gamma(self._n_parameters / self._beta)
-        return g1 / g2
+        return np.zeros(self._n_parameters)
 
     def n_parameters(self):
+        """ See :meth:`pints.LogPDF.n_parameters()`. """
         return self._n_parameters
 
     def sample(self, n_samples):
-        """ See :meth:`ToyLogPDF.sample()`. """
-        n_samples = int(n_samples)
-        if n_samples < 1:
-            raise ValueError(
-                'Number of samples must be greater than or equal to 1.')
+        """ See :meth:`pints.toy.ToyLogPDF.sample()`. """
         n = self._n_parameters
-
-        # Determine empirical inverse-CDF
-        x_max = scipy.optimize.minimize(lambda x: (
-            np.abs((self.CDF(x) - 1))), 8)['x'][0] * 10
-        x_range = np.linspace(0, x_max, 100)
-        cdf = [self.CDF(x) for x in x_range]
-        f = scipy.interpolate.interp1d(cdf, x_range)
-
-        # Do inverse-transform sampling to obtain independent r samples
-        u = np.random.rand(n_samples)
-        r = f(u)
-
-        # For each value of r select a value uniformly at random on
-        # hypersphere of that radius
-        X_norm = np.random.normal(size=(n_samples, n))
-        lambda_x = np.sqrt(np.sum(X_norm**2, axis=1))
-        x_unit = [r[i] * X_norm[i] / y for i, y in enumerate(lambda_x)]
-        return np.array(x_unit)
+        samples = np.zeros((n_samples, n))
+        for i in range(n_samples):
+            nu = np.random.normal(0, 3, 1)[0]
+            sd = np.exp(nu / 2)
+            x = np.random.normal(0, sd, n - 1)
+            samples[i, 0:(n - 1)] = x
+            samples[i, n - 1] = nu
+        return samples
 
     def suggested_bounds(self):
-        """ See :meth:`ToyLogPDF.suggested_bounds()`. """
-        magnitude = 1000
-        bounds = np.tile([-magnitude, magnitude], (self._n_parameters, 1))
+        """ See :meth:`pints.toy.ToyLogPDF.suggested_bounds()`. """
+        magnitude = 30
+        bounds = np.tile([-magnitude, magnitude],
+                         (self._n_parameters, 1))
         return np.transpose(bounds).tolist()
 
-    def var_normed(self):
+    def var(self):
         """
-        Returns the variance of the normed distance from the origin.
+        Returns the variance of the target distribution in each dimension.
+        Note :math:`nu` is the last entry.
         """
-        g1 = scipy.special.gamma((2 + self._n_parameters) / self._beta)
-        g2 = scipy.special.gamma(self._n_parameters / self._beta)
-        return g1 / g2 - self.mean_normed()**2
+        return np.concatenate((np.repeat(90, self._n_parameters - 1), [9]))
```

### Comparing `pints-0.4.0/pints/toy/_constant_model.py` & `pints-0.5.0/pints/toy/_constant_model.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_eight_schools.py` & `pints-0.5.0/pints/toy/_eight_schools.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_fitzhugh_nagumo_model.py` & `pints-0.5.0/pints/toy/_fitzhugh_nagumo_model.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_gaussian.py` & `pints-0.5.0/pints/toy/_gaussian.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_german_credit.py` & `pints-0.5.0/pints/toy/_german_credit.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_german_credit_hierarchical.py` & `pints-0.5.0/pints/toy/_german_credit_hierarchical.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_goodwin_oscillator_model.py` & `pints-0.5.0/pints/toy/_goodwin_oscillator_model.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_hes1_michaelis_menten.py` & `pints-0.5.0/pints/toy/_hes1_michaelis_menten.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_hh_ik_model.py` & `pints-0.5.0/pints/toy/_hh_ik_model.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_high_dimensional_gaussian.py` & `pints-0.5.0/pints/toy/_high_dimensional_gaussian.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_logistic_model.py` & `pints-0.5.0/pints/toy/_logistic_model.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_lotka_volterra_model.py` & `pints-0.5.0/pints/toy/_lotka_volterra_model.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_multimodal_gaussian.py` & `pints-0.5.0/pints/toy/_multimodal_gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         # See page 45 of
         # http://www.math.uwaterloo.ca/~hwolkowi//matrixcookbook.pdf
         self._sigma_invs = [
             np.linalg.inv(self._covs[i]) for i, mode in enumerate(self._modes)]
 
     def __call__(self, x):
         f = np.sum([var.pdf(x) for var in self._vars])
-        return -float('inf') if f == 0 else np.log(f)
+        return -np.inf if f == 0 else np.log(f)
 
     def distance(self, samples):
         """
         Calculates :meth:`per mode approximate KL divergence <kl_divergence>`
         then sums these.
 
         See :meth:`pints.toy.ToyLogPDF.distance()`.
@@ -142,15 +142,15 @@
         if samples.shape[1] != self._n_parameters:
             raise ValueError(
                 'Given samples must have length ' + str(self._n_parameters))
 
         best_mode = np.zeros(samples.shape[0])
         for i in range(samples.shape[0]):
             a_sample = samples[i, :]
-            a_log_pdf = -float('Inf')
+            a_log_pdf = -np.inf
             a_max_index = -1
             for j, var in enumerate(self._vars):
                 a_test_log_pdf = var.logpdf(a_sample)
                 if a_test_log_pdf > a_log_pdf:
                     a_log_pdf = a_test_log_pdf
                     a_max_index = j
             best_mode[i] = a_max_index
```

### Comparing `pints-0.4.0/pints/toy/_parabola.py` & `pints-0.5.0/pints/toy/_parabola.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_repressilator_model.py` & `pints-0.5.0/pints/toy/_repressilator_model.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_rosenbrock.py` & `pints-0.5.0/pints/toy/_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_sho_model.py` & `pints-0.5.0/pints/toy/_sho_model.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_simple_egg_box.py` & `pints-0.5.0/pints/toy/_simple_egg_box.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         # See page 45 of
         # http://www.math.uwaterloo.ca/~hwolkowi//matrixcookbook.pdf
         self._sigma_invs = [np.linalg.inv(self._covs[i])
                             for i, mode in enumerate(self._modes)]
 
     def __call__(self, x):
         f = np.sum([var.pdf(x) for var in self._vars])
-        return -float('inf') if f == 0 else np.log(f)
+        return -np.inf if f == 0 else np.log(f)
 
     def distance(self, samples):
         """
         Calculates :meth:`approximate mode-wise KL divergence<kl_divergence>`.
 
         See :meth:`pints.toy.ToyLogPDF.distance()`.
         """
```

### Comparing `pints-0.4.0/pints/toy/_sir_model.py` & `pints-0.5.0/pints/toy/_sir_model.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_toy_classes.py` & `pints-0.5.0/pints/toy/_toy_classes.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints/toy/_twisted_gaussian_banana.py` & `pints-0.5.0/pints/toy/_twisted_gaussian_banana.py`

 * *Files identical despite different names*

### Comparing `pints-0.4.0/pints.egg-info/PKG-INFO` & `pints-0.5.0/pints.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: pints
-Version: 0.4.0
+Version: 0.5.0
 Summary: Probabilistic Inference in Noisy Time-Series
 Home-page: https://github.com/pints-team/pints
 Maintainer: PINTS Team
 Maintainer-email: pints@maillist.ox.ac.uk
 License: BSD 3-clause license
-Platform: UNKNOWN
-Requires-Python: >=3.5
+Project-URL: Bug Tracker, https://github.com/pints-team/pints/issues
+Project-URL: Documentation, https://pints.readthedocs.io
+Project-URL: Source Code, https://github.com/pints-team/pints
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: stan
 License-File: LICENSE.md
 
-[![Unit tests on multiple python versions](https://github.com/pints-team/pints/workflows/Unit%20tests%20on%20multiple%20python%20versions/badge.svg)](https://github.com/pints-team/pints/actions)
-[![Unit tests on multiple operating systems](https://github.com/pints-team/pints/workflows/Unit%20tests%20on%20multiple%20operating%20systems/badge.svg)](https://github.com/pints-team/pints/actions)
-[![codecov](https://codecov.io/gh/pints-team/pints/branch/master/graph/badge.svg)](https://codecov.io/gh/pints-team/pints)
-[![Functional testing code](https://raw.githubusercontent.com/pints-team/functional-testing/master/badge-code.svg)](https://github.com/pints-team/functional-testing)
-[![Functional testing results](https://raw.githubusercontent.com/pints-team/functional-testing/master/badge-results.svg)](https://www.cs.ox.ac.uk/projects/PINTS/functional-testing)
-[![binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/pints-team/pints/master?filepath=examples)
+[![Unit tests on multiple python versions](https://github.com/pints-team/pints/actions/workflows/unit-test-python-coverage.yml/badge.svg)](https://github.com/pints-team/pints/actions/workflows/unit-test-python-coverage.yml)
+[![Unit tests on multiple operating systems](https://github.com/pints-team/pints/actions/workflows/unit-test-os-coverage.yml/badge.svg)](https://github.com/pints-team/pints/actions/workflows/unit-test-os-coverage.yml)
+[![codecov](https://codecov.io/gh/pints-team/pints/branch/main/graph/badge.svg)](https://codecov.io/gh/pints-team/pints)
+[![Change-point testing code](https://raw.githubusercontent.com/pints-team/change-point-testing/main/badge-code.svg)](https://github.com/pints-team/change-point-testing)
+[![Change-point testing results](https://raw.githubusercontent.com/pints-team/change-point-testing/main/badge-results.svg)](https://www.cs.ox.ac.uk/projects/PINTS/functional-testing)
+[![binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/pints-team/pints/main?filepath=examples)
 [![readthedocs](https://readthedocs.org/projects/pints/badge/?version=latest)](http://pints.readthedocs.io/en/latest/?badge=latest)
-[![BCH compliance](https://bettercodehub.com/edge/badge/pints-team/pints?branch=master)](https://bettercodehub.com/results/pints-team/pints)
 
 # What is Pints?
 
 PINTS (Probabilistic Inference on Noisy Time-Series) is a framework for optimisation and Bayesian inference on ODE models of noisy time-series, such as arise in electrochemistry and cardiac electrophysiology.
 
-PINTS is described in [this publication in JORS](http://doi.org/10.5334/jors.252), and can be cited using the information given in our [CITATION file](https://github.com/pints-team/pints/blob/master/CITATION).
-More information about PINTS papers can be found in the [papers directory](https://github.com/pints-team/pints/tree/master/papers).
+PINTS is described in [this publication in JORS](http://doi.org/10.5334/jors.252), and can be cited using the information given in our [CITATION file](https://github.com/pints-team/pints/blob/main/CITATION).
+More information about PINTS papers can be found in the [papers directory](https://github.com/pints-team/pints/tree/main/papers).
 
 
 ## Using PINTS
 
 PINTS can work with any model that implements the [pints.ForwardModel](http://pints.readthedocs.io/en/latest/core_classes_and_methods.html#forward-model) interface.
 This has just two methods:
 
@@ -40,40 +41,40 @@
 n_parameters() --> Returns the dimension of the parameter space.
 
 simulate(parameters, times) --> Returns a vector of model evaluations at
                                 the given times, using the given parameters
 ```
 
 Experimental data sets in PINTS are defined simply as lists (or arrays) of `times` and corresponding experimental `values`.
-If you have this kind of data, and if [your model (or model wrapper)](https://github.com/pints-team/pints/blob/master/examples/stats/custom-model.ipynb) implements the two methods above, then you are ready to start using PINTS to infer parameter values using [optimisation](https://github.com/pints-team/pints/blob/master/examples/optimisation/first-example.ipynb) or [sampling](https://github.com/pints-team/pints/blob/master/examples/sampling/first-example.ipynb).
+If you have this kind of data, and if [your model (or model wrapper)](https://github.com/pints-team/pints/blob/main/examples/stats/custom-model.ipynb) implements the two methods above, then you are ready to start using PINTS to infer parameter values using [optimisation](https://github.com/pints-team/pints/blob/main/examples/optimisation/first-example.ipynb) or [sampling](https://github.com/pints-team/pints/blob/main/examples/sampling/first-example.ipynb).
 
-A brief example is shown below:  
-![An example of using PINTS in an optimisation](https://raw.githubusercontent.com/pints-team/pints/master/example.svg)  
+A brief example is shown below:
+![An example of using PINTS in an optimisation](https://raw.githubusercontent.com/pints-team/pints/main/example.svg)
 _(Left)_ A noisy experimental time series and a computational forward model.
 _(Right)_ Example code for an optimisation problem.
-The full code can be [viewed here](https://github.com/pints-team/pints/blob/master/examples/sampling/readme-example.ipynb) but a friendlier, more elaborate, introduction can be found on the [examples page](https://github.com/pints-team/pints/blob/master/examples/README.md).
+The full code can be [viewed here](https://github.com/pints-team/pints/blob/main/examples/sampling/readme-example.ipynb) but a friendlier, more elaborate, introduction can be found on the [examples page](https://github.com/pints-team/pints/blob/main/examples/README.md).
 
 A graphical overview of the methods included in PINTS can be [viewed here](https://pints-team.github.io/pints-methods-overview/).
 
 ### Examples and documentation
 
-PINTS comes with a number of [detailed examples](https://github.com/pints-team/pints/blob/master/examples/README.md), hosted here on github.
+PINTS comes with a number of [detailed examples](https://github.com/pints-team/pints/blob/main/examples/README.md), hosted here on github.
 In addition, there is a [full API documentation](http://pints.readthedocs.io/en/latest/), hosted on readthedocs.io.
 
 
 ## Installing PINTS
 
 The latest release of PINTS can be installed without downloading (cloning) the git repository, by opening a console and typing
 
 ```
 $ pip install --upgrade pip
 $ pip install pints
 ```
 
-Note that you'll need Python 3.5 or newer.
+Note that you'll need Python 3.6 or newer.
 
 If you prefer to have the latest cutting-edge version, you can instead install from the repository, by typing
 
 ```
 $ git clone https://github.com/pints-team/pints.git
 $ cd pints
 $ pip install -e .[dev,docs]
@@ -84,27 +85,25 @@
 ```
 $ pip uninstall pints
 ```
 
 
 ## What's new in this version of PINTS?
 
-To see what's changed in the latest release, see the [CHANGELOG](https://github.com/pints-team/pints/blob/master/CHANGELOG.md).
+To see what's changed in the latest release, see the [CHANGELOG](https://github.com/pints-team/pints/blob/main/CHANGELOG.md).
 
 
 ## Contributing to PINTS
 
-If you'd like to help us develop PINTS by adding new methods, writing documentation, or fixing embarassing bugs, please have a look at these [guidelines](https://github.com/pints-team/pints/blob/master/CONTRIBUTING.md) first.
+If you'd like to help us develop PINTS by adding new methods, writing documentation, or fixing embarassing bugs, please have a look at these [guidelines](https://github.com/pints-team/pints/blob/main/CONTRIBUTING.md) first.
 
 
 ## License
 
-PINTS is fully open source. For more information about its license, see [LICENSE](https://github.com/pints-team/pints/blob/master/LICENSE.md).
+PINTS is fully open source. For more information about its license, see [LICENSE](https://github.com/pints-team/pints/blob/main/LICENSE.md).
 
 
 ## Get in touch
 
 Questions, suggestions, or bug reports? [Open an issue](https://github.com/pints-team/pints/issues) and let us know.
 
 Alternatively, feel free to email us at `pints at maillist.ox.ac.uk`.
-
-
```

### Comparing `pints-0.4.0/pints.egg-info/SOURCES.txt` & `pints-0.5.0/pints.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 pints/residuals_diagnostics.py
 pints/version
 pints.egg-info/PKG-INFO
 pints.egg-info/SOURCES.txt
 pints.egg-info/dependency_links.txt
 pints.egg-info/requires.txt
 pints.egg-info/top_level.txt
+pints/_abc/__init__.py
+pints/_abc/_abc_rejection.py
+pints/_abc/_abc_smc.py
 pints/_mcmc/__init__.py
 pints/_mcmc/_adaptive_covariance.py
 pints/_mcmc/_differential_evolution.py
 pints/_mcmc/_dram_ac.py
 pints/_mcmc/_dream.py
 pints/_mcmc/_dual_averaging.py
 pints/_mcmc/_emcee_hammer.py
@@ -45,17 +48,19 @@
 pints/_mcmc/_slice_rank_shrinking.py
 pints/_mcmc/_slice_stepout.py
 pints/_mcmc/_summary.py
 pints/_nested/__init__.py
 pints/_nested/_ellipsoid.py
 pints/_nested/_rejection.py
 pints/_optimisers/__init__.py
+pints/_optimisers/_adam.py
 pints/_optimisers/_cmaes.py
 pints/_optimisers/_cmaes_bare.py
 pints/_optimisers/_gradient_descent.py
+pints/_optimisers/_irpropmin.py
 pints/_optimisers/_nelder_mead.py
 pints/_optimisers/_pso.py
 pints/_optimisers/_snes.py
 pints/_optimisers/_xnes.py
 pints/interfaces/__init__.py
 pints/interfaces/stan/__init__.py
 pints/interfaces/stan/_stan.py
@@ -88,11 +93,16 @@
 pints/toy/_neals_funnel.py
 pints/toy/_parabola.py
 pints/toy/_repressilator_model.py
 pints/toy/_rosenbrock.py
 pints/toy/_sho_model.py
 pints/toy/_simple_egg_box.py
 pints/toy/_sir_model.py
-pints/toy/_stochastic_degradation_model.py
-pints/toy/_stochastic_logistic_model.py
 pints/toy/_toy_classes.py
-pints/toy/_twisted_gaussian_banana.py
+pints/toy/_twisted_gaussian_banana.py
+pints/toy/stochastic/__init__.py
+pints/toy/stochastic/_degradation_model.py
+pints/toy/stochastic/_logistic_model.py
+pints/toy/stochastic/_markov_jump_model.py
+pints/toy/stochastic/_michaelis_menten_model.py
+pints/toy/stochastic/_production_degradation_model.py
+pints/toy/stochastic/_schlogl_model.py
```

### Comparing `pints-0.4.0/setup.py` & `pints-0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,14 +41,21 @@
     # Maintainer information
     # author='',
     # author_email='',
     maintainer='PINTS Team',
     maintainer_email='pints@maillist.ox.ac.uk',
     url='https://github.com/pints-team/pints',
 
+    # Project URLs
+    project_urls={
+        'Bug Tracker': 'https://github.com/pints-team/pints/issues',
+        'Documentation': 'https://pints.readthedocs.io',
+        'Source Code': 'https://github.com/pints-team/pints',
+    },
+
     # Packages to include
     packages=find_packages(include=('pints', 'pints.*')),
 
     # Include non-python files (via MANIFEST.in)
     include_package_data=True,
 
     # List of dependencies
@@ -70,12 +77,12 @@
         'dev': [
             'flake8>=3',            # For code style checking
             'jupyter',              # For documentation and testing
             'nbconvert',
             'traitlets',
         ],
         'stan': [
-            'pystan==2.19.1.1',
+            'pystan>=3',
         ]
     },
-    python_requires='>=3.5',
+    python_requires='>=3.7',
 )
```

