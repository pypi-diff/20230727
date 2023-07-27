# Comparing `tmp/Chronix2Grid-1.2.0.tar.gz` & `tmp/Chronix2Grid-1.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chronix2Grid-1.2.0.tar", last modified: Wed Jul 26 15:57:49 2023, max compression
+gzip compressed data, was "Chronix2Grid-1.2.0.post1.tar", last modified: Thu Jul 27 09:42:36 2023, max compression
```

## Comparing `Chronix2Grid-1.2.0.tar` & `Chronix2Grid-1.2.0.post1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.459732 Chronix2Grid-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/AUTHORS.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.399730 Chronix2Grid-1.2.0/Chronix2Grid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-07-26 15:57:49.000000 Chronix2Grid-1.2.0/Chronix2Grid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-26 15:57:49.000000 Chronix2Grid-1.2.0/Chronix2Grid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:57:49.000000 Chronix2Grid-1.2.0/Chronix2Grid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-26 15:57:49.000000 Chronix2Grid-1.2.0/Chronix2Grid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:57:49.000000 Chronix2Grid-1.2.0/Chronix2Grid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-26 15:57:49.000000 Chronix2Grid-1.2.0/Chronix2Grid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 15:57:49.000000 Chronix2Grid-1.2.0/Chronix2Grid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-07-26 15:57:49.455731 Chronix2Grid-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.399730 Chronix2Grid-1.2.0/RenewableGANBackend/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/RenewableGANBackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/RenewableGANBackend/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/RenewableGANBackend/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/RenewableGANBackend/gan_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/RenewableGANBackend/generate_solar_wind_gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.403730 Chronix2Grid-1.2.0/chronix2grid/
--rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/GeneratorBackend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      512 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19055 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/default_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.403730 Chronix2Grid-1.2.0/chronix2grid/generation/
--rwxr-xr-x   0 runner    (1001) docker     (123)      483 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.403730 Chronix2Grid-1.2.0/chronix2grid/generation/_dispatch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.403730 Chronix2Grid-1.2.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/PypsaEconomicDispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.403730 Chronix2Grid-1.2.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/run_economic_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/_dispatch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.403730 Chronix2Grid-1.2.0/chronix2grid/generation/consumption/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/consumption/ConsumptionGeneratorBackend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/consumption/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9961 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/consumption/consumption_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4520 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/consumption/generate_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.403730 Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/DispatchBackend.py
--rw-r--r--   0 runner    (1001) docker     (123)    22165 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/EconomicDispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.403730 Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/PypsaDispatchBackend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.403730 Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/PypsaDispatchBackend/EDispatch_L2RPN2020/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/PypsaDispatchBackend/EDispatch_L2RPN2020/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/PypsaDispatchBackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/dispatch_loss_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/generate_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2545 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/generate_chronics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/generation_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.403730 Chronix2Grid-1.2.0/chronix2grid/generation/hydro/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/hydro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/hydro/make_hydro_guide_curves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.407730 Chronix2Grid-1.2.0/chronix2grid/generation/loss/
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/loss/LossBackend.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/loss/generate_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.407730 Chronix2Grid-1.2.0/chronix2grid/generation/renewable/
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/renewable/RenewableBackend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/renewable/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10569 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/renewable/generate_solar_wind.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11087 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/generation/renewable/solar_wind_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.407730 Chronix2Grid-1.2.0/chronix2grid/getting_started/
--rwxr-xr-x   0 runner    (1001) docker     (123)      483 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.407730 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/
--rwxr-xr-x   0 runner    (1001) docker     (123)      483 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.407730 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/
--rwxr-xr-x   0 runner    (1001) docker     (123)      483 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.407730 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.407730 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/config.py
--rw-r--r--   0 runner    (1001) docker     (123)   157483 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/grid.json
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/grid_layout.json
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/loads_charac.csv
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/params_load.json
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/params_loss.json
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/params_opf.json
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/params_res.json
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/prods_charac.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.443731 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4825656 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/hydro_french.csv
--rw-r--r--   0 runner    (1001) docker     (123)  4662662 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/hydro_raw_2018.csv
--rw-r--r--   0 runner    (1001) docker     (123)  5140153 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/hydro_smooth_2018.csv
--rw-r--r--   0 runner    (1001) docker     (123)  8081173 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/load_weekly_pattern.csv
--rw-r--r--   0 runner    (1001) docker     (123)  4086848 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/load_weekly_pattern.csv.bk
--rw-r--r--   0 runner    (1001) docker     (123)  2108172 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/loss_pattern.csv
--rw-r--r--   0 runner    (1001) docker     (123)    70216 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/solar_pattern.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.395730 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.443731 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.399730 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.447731 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/eco2mix/
--rw-r--r--   0 runner    (1001) docker     (123)  2604328 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/eco2mix/eCO2mix_RTE_Hauts-de-France_Annuel-Definitif_2012.csv
--rw-r--r--   0 runner    (1001) docker     (123)  2746589 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/eco2mix/eCO2mix_RTE_Nouvelle-Aquitaine_Annuel-Definitif_2012.csv
--rw-r--r--   0 runner    (1001) docker     (123)  2191697 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/eco2mix/eCO2mix_RTE_PACA_Annuel-Definitif_2012.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.451732 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/renewable_ninja/
--rw-r--r--   0 runner    (1001) docker     (123)   829863 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/renewable_ninja/solar.csv
--rw-r--r--   0 runner    (1001) docker     (123)   981611 2023-07-26 15:57:34.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/renewable_ninja/wind.csv
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/paramsKPI.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.455731 Chronix2Grid-1.2.0/chronix2grid/grid2op_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/grid2op_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/grid2op_utils/add_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    19431 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/grid2op_utils/gen_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/grid2op_utils/generate_one_episode.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/grid2op_utils/loads_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/grid2op_utils/noise_generation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50851 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/grid2op_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.455731 Chronix2Grid-1.2.0/chronix2grid/kpi/
--rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/kpi/Generator_parameter_checker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/kpi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.455731 Chronix2Grid-1.2.0/chronix2grid/kpi/deterministic/
--rwxr-xr-x   0 runner    (1001) docker     (123)      483 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/kpi/deterministic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/kpi/deterministic/hydro.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    53313 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/kpi/deterministic/kpis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/kpi/deterministic/nuclear.py
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/kpi/deterministic/solar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/kpi/deterministic/wind.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8256 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/kpi/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.455731 Chronix2Grid-1.2.0/chronix2grid/kpi/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/kpi/preprocessing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5141 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/kpi/preprocessing/pivot_KPI.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21147 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/kpi/preprocessing/pivot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:49.455731 Chronix2Grid-1.2.0/chronix2grid/kpi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/kpi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/kpi/utils/plot_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12735 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/output_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/seed_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-26 15:57:35.000000 Chronix2Grid-1.2.0/chronix2grid/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:57:49.459732 Chronix2Grid-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-26 15:57:36.000000 Chronix2Grid-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.805022 Chronix2Grid-1.2.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/AUTHORS.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.749021 Chronix2Grid-1.2.0.post1/Chronix2Grid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10566 2023-07-27 09:42:36.000000 Chronix2Grid-1.2.0.post1/Chronix2Grid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-27 09:42:36.000000 Chronix2Grid-1.2.0.post1/Chronix2Grid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 09:42:36.000000 Chronix2Grid-1.2.0.post1/Chronix2Grid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-27 09:42:36.000000 Chronix2Grid-1.2.0.post1/Chronix2Grid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 09:42:36.000000 Chronix2Grid-1.2.0.post1/Chronix2Grid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-27 09:42:36.000000 Chronix2Grid-1.2.0.post1/Chronix2Grid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 09:42:36.000000 Chronix2Grid-1.2.0.post1/Chronix2Grid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10566 2023-07-27 09:42:36.805022 Chronix2Grid-1.2.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.749021 Chronix2Grid-1.2.0.post1/RenewableGANBackend/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/RenewableGANBackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/RenewableGANBackend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/RenewableGANBackend/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/RenewableGANBackend/gan_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/RenewableGANBackend/generate_solar_wind_gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.753021 Chronix2Grid-1.2.0.post1/chronix2grid/
+-rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/GeneratorBackend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      512 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19055 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/default_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.753021 Chronix2Grid-1.2.0.post1/chronix2grid/generation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      483 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.753021 Chronix2Grid-1.2.0.post1/chronix2grid/generation/_dispatch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.753021 Chronix2Grid-1.2.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/PypsaEconomicDispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.753021 Chronix2Grid-1.2.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/run_economic_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/_dispatch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.753021 Chronix2Grid-1.2.0.post1/chronix2grid/generation/consumption/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/consumption/ConsumptionGeneratorBackend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/consumption/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9961 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/consumption/consumption_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4520 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/consumption/generate_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.753021 Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/DispatchBackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22165 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/EconomicDispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.753021 Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/PypsaDispatchBackend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.753021 Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/PypsaDispatchBackend/EDispatch_L2RPN2020/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/PypsaDispatchBackend/EDispatch_L2RPN2020/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/PypsaDispatchBackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/dispatch_loss_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/generate_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2545 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/generate_chronics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/generation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.753021 Chronix2Grid-1.2.0.post1/chronix2grid/generation/hydro/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/hydro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/hydro/make_hydro_guide_curves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.757021 Chronix2Grid-1.2.0.post1/chronix2grid/generation/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/loss/LossBackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/loss/generate_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.757021 Chronix2Grid-1.2.0.post1/chronix2grid/generation/renewable/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/renewable/RenewableBackend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/renewable/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10569 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/renewable/generate_solar_wind.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11087 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/generation/renewable/solar_wind_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.757021 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      483 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.757021 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      483 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.757021 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      483 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.757021 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.761021 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157483 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/grid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/grid_layout.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/loads_charac.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/params_load.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/params_loss.json
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/params_opf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/params_res.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/prods_charac.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.789021 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4825656 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/hydro_french.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  4662662 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/hydro_raw_2018.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  5140153 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/hydro_smooth_2018.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  8081173 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/load_weekly_pattern.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  4086848 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/load_weekly_pattern.csv.bk
+-rw-r--r--   0 runner    (1001) docker     (123)  2108172 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/loss_pattern.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    70216 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/solar_pattern.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.749021 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.789021 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.749021 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.797021 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/eco2mix/
+-rw-r--r--   0 runner    (1001) docker     (123)  2604328 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/eco2mix/eCO2mix_RTE_Hauts-de-France_Annuel-Definitif_2012.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  2746589 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/eco2mix/eCO2mix_RTE_Nouvelle-Aquitaine_Annuel-Definitif_2012.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  2191697 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/eco2mix/eCO2mix_RTE_PACA_Annuel-Definitif_2012.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.801021 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/renewable_ninja/
+-rw-r--r--   0 runner    (1001) docker     (123)   829863 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/renewable_ninja/solar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   981611 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/renewable_ninja/wind.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/paramsKPI.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.801021 Chronix2Grid-1.2.0.post1/chronix2grid/grid2op_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/grid2op_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/grid2op_utils/add_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19431 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/grid2op_utils/gen_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/grid2op_utils/generate_one_episode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/grid2op_utils/loads_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/grid2op_utils/noise_generation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50851 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/grid2op_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.801021 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/
+-rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/Generator_parameter_checker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.801021 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/deterministic/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      483 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/deterministic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/deterministic/hydro.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    53313 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/deterministic/kpis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/deterministic/nuclear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/deterministic/solar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/deterministic/wind.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8256 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.805022 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/preprocessing/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5141 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/preprocessing/pivot_KPI.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21147 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/preprocessing/pivot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:36.805022 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/kpi/utils/plot_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12735 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/output_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/seed_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-27 09:42:24.000000 Chronix2Grid-1.2.0.post1/chronix2grid/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 09:42:36.805022 Chronix2Grid-1.2.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-27 09:42:26.000000 Chronix2Grid-1.2.0.post1/setup.py
```

### Comparing `Chronix2Grid-1.2.0/AUTHORS.txt` & `Chronix2Grid-1.2.0.post1/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/Chronix2Grid.egg-info/PKG-INFO` & `Chronix2Grid-1.2.0.post1/Chronix2Grid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chronix2Grid
-Version: 1.2.0
+Version: 1.2.0.post1
 Summary: A python package to generate "en-masse" chronics for loads and productions (thermal, renewable)
 Home-page: https://github.com/BDonnot/ChroniX2Grid
 Author: Mario Jothy, Nicolas Megel, Vincent Renault, Benjamin Donnot
 Author-email: mario.jothy@artelys.com
 License: Mozilla Public License 2.0 (MPL 2.0)
 Keywords: ML powergrid optmization RL power-systems chronics generation production load network
 Platform: Windows
@@ -12,14 +12,15 @@
 Platform: Mac OS-X
 Platform: Unix
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 Provides-Extra: optional
```

### Comparing `Chronix2Grid-1.2.0/Chronix2Grid.egg-info/SOURCES.txt` & `Chronix2Grid-1.2.0.post1/Chronix2Grid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/Chronix2Grid.egg-info/requires.txt` & `Chronix2Grid-1.2.0.post1/Chronix2Grid.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/LICENSE` & `Chronix2Grid-1.2.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/PKG-INFO` & `Chronix2Grid-1.2.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chronix2Grid
-Version: 1.2.0
+Version: 1.2.0.post1
 Summary: A python package to generate "en-masse" chronics for loads and productions (thermal, renewable)
 Home-page: https://github.com/BDonnot/ChroniX2Grid
 Author: Mario Jothy, Nicolas Megel, Vincent Renault, Benjamin Donnot
 Author-email: mario.jothy@artelys.com
 License: Mozilla Public License 2.0 (MPL 2.0)
 Keywords: ML powergrid optmization RL power-systems chronics generation production load network
 Platform: Windows
@@ -12,14 +12,15 @@
 Platform: Mac OS-X
 Platform: Unix
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 Provides-Extra: optional
```

### Comparing `Chronix2Grid-1.2.0/README.md` & `Chronix2Grid-1.2.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/RenewableGANBackend/backend.py` & `Chronix2Grid-1.2.0.post1/RenewableGANBackend/backend.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/RenewableGANBackend/config.py` & `Chronix2Grid-1.2.0.post1/RenewableGANBackend/config.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/RenewableGANBackend/gan_utils.py` & `Chronix2Grid-1.2.0.post1/RenewableGANBackend/gan_utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/RenewableGANBackend/generate_solar_wind_gan.py` & `Chronix2Grid-1.2.0.post1/RenewableGANBackend/generate_solar_wind_gan.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/GeneratorBackend.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/GeneratorBackend.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/__init__.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 # See AUTHORS.txt
 # This Source Code Form is subject to the terms of the Mozilla Public License, version 2.0.
 # If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
 # you can obtain one at http://mozilla.org/MPL/2.0/.
 # SPDX-License-Identifier: MPL-2.0
 # This file is part of Chronix2Grid, A python package to generate "en-masse" chronics for loads and productions (thermal, renewable)
 
-___version__ = "1.1.0.post1"
+___version__ = "1.2.0.post1"
```

### Comparing `Chronix2Grid-1.2.0/chronix2grid/config.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/config.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/constants.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/constants.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/default_backend.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/default_backend.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/PypsaEconomicDispatch.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/PypsaEconomicDispatch.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/__init__.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/__init__.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/run_economic_dispatch.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/run_economic_dispatch.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/utils.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/consumption/ConsumptionGeneratorBackend.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/consumption/ConsumptionGeneratorBackend.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/consumption/__init__.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/consumption/__init__.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/consumption/consumption_utils.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/consumption/consumption_utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/consumption/generate_load.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/consumption/generate_load.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/DispatchBackend.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/DispatchBackend.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/EconomicDispatch.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/EconomicDispatch.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/PypsaDispatchBackend/EDispatch_L2RPN2020/__init__.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/PypsaDispatchBackend/EDispatch_L2RPN2020/__init__.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/PypsaDispatchBackend/__init__.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/PypsaDispatchBackend/__init__.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/dispatch_loss_utils.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/dispatch_loss_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,22 +123,30 @@
     #if (agent_type == 'reco'):
     #    #runner = Runner(**env.get_params_for_runner(), agentClass=DoNothingAgent)
     #    runner = Runner(**env.get_params_for_runner(), agentClass=RecoPowerlineAgent)
     #else:
     runner = Runner(**env.get_params_for_runner())
     # do regular computation as you would with grid2op
     path_save = None
-    if(write_results):
-        path_save=os.path.join(agent_results_path,'agent_results')
+    if write_results:
+        path_save = os.path.join(agent_results_path, 'agent_results')
         os.makedirs(path_save, exist_ok=True)
 
-    name_chron, cum_reward, nb_time_step, episode_data =runner.run_one_episode(path_save=path_save,
-                             indx=scen_id,
-                             pbar=True,
-                             detailed_output=True)
+    try:
+        # recent grid2op version: run_one_episode has the same signature as runner.run
+        *_, episode_data = runner.run_one_episode(path_save=path_save,
+                                                  indx=scen_id,
+                                                  pbar=True,
+                                                  detailed_output=True)
+    except ValueError:
+        # old grid2op version
+        name_chron, cum_reward, nb_time_step, episode_data = runner.run_one_episode(path_save=path_save,
+                                                                                    indx=scen_id,
+                                                                                    pbar=True,
+                                                                                    detailed_output=True)
     #res = runner.run(nb_episode=nb_episode, nb_process=NB_CORE, pbar=True, add_detailed_output=True)
     #                 #path_save=simulation_data_folder
     #id_chron, name_chron, cum_reward, nb_timestep, max_ts, episode_data = res.pop()
     print('---- end of simulation')
 
     return episode_data
```

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/generate_dispatch.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/generate_dispatch.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/dispatch/utils.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/dispatch/utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/generate_chronics.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/generate_chronics.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/generation_utils.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/generation_utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/hydro/make_hydro_guide_curves.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/hydro/make_hydro_guide_curves.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/loss/LossBackend.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/loss/LossBackend.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/loss/generate_loss.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/loss/generate_loss.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/renewable/RenewableBackend.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/renewable/RenewableBackend.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/renewable/__init__.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/renewable/__init__.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/renewable/generate_solar_wind.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/renewable/generate_solar_wind.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/generation/renewable/solar_wind_utils.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/generation/renewable/solar_wind_utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/__init__.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/config.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/config.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/grid.json` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/grid.json`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/grid_layout.json` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/grid_layout.json`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/loads_charac.csv` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/loads_charac.csv`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/prods_charac.csv` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/case118_l2rpn_neurips_1x/prods_charac.csv`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/__init__.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/hydro_french.csv` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/hydro_french.csv`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/hydro_raw_2018.csv` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/hydro_raw_2018.csv`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/hydro_smooth_2018.csv` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/hydro_smooth_2018.csv`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/load_weekly_pattern.csv` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/load_weekly_pattern.csv`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/load_weekly_pattern.csv.bk` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/load_weekly_pattern.csv.bk`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/loss_pattern.csv` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/loss_pattern.csv`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/generation/patterns/solar_pattern.npy` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/generation/patterns/solar_pattern.npy`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/eco2mix/eCO2mix_RTE_Hauts-de-France_Annuel-Definitif_2012.csv` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/eco2mix/eCO2mix_RTE_Hauts-de-France_Annuel-Definitif_2012.csv`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/eco2mix/eCO2mix_RTE_Nouvelle-Aquitaine_Annuel-Definitif_2012.csv` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/eco2mix/eCO2mix_RTE_Nouvelle-Aquitaine_Annuel-Definitif_2012.csv`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/eco2mix/eCO2mix_RTE_PACA_Annuel-Definitif_2012.csv` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/eco2mix/eCO2mix_RTE_PACA_Annuel-Definitif_2012.csv`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/renewable_ninja/solar.csv` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/renewable_ninja/solar.csv`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/renewable_ninja/wind.csv` & `Chronix2Grid-1.2.0.post1/chronix2grid/getting_started/example/input/kpi/case118_l2rpn_neurips_1x/France/renewable_ninja/wind.csv`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/grid2op_utils/__init__.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/grid2op_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/grid2op_utils/add_data.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/grid2op_utils/add_data.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/grid2op_utils/gen_utils.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/grid2op_utils/gen_utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/grid2op_utils/generate_one_episode.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/grid2op_utils/generate_one_episode.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/grid2op_utils/loads_utils.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/grid2op_utils/loads_utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/grid2op_utils/noise_generation_utils.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/grid2op_utils/noise_generation_utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/grid2op_utils/utils.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/grid2op_utils/utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/kpi/Generator_parameter_checker.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/kpi/Generator_parameter_checker.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/kpi/deterministic/hydro.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/kpi/deterministic/hydro.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/kpi/deterministic/kpis.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/kpi/deterministic/kpis.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/kpi/deterministic/nuclear.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/kpi/deterministic/nuclear.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/kpi/deterministic/solar.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/kpi/deterministic/solar.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/kpi/deterministic/wind.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/kpi/deterministic/wind.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/kpi/main.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/kpi/main.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/kpi/preprocessing/pivot_KPI.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/kpi/preprocessing/pivot_KPI.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/kpi/preprocessing/pivot_utils.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/kpi/preprocessing/pivot_utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/kpi/utils/plot_tools.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/kpi/utils/plot_tools.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/main.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/main.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/output_processor.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/output_processor.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/seed_manager.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/seed_manager.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/chronix2grid/utils.py` & `Chronix2Grid-1.2.0.post1/chronix2grid/utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.2.0/setup.py` & `Chronix2Grid-1.2.0.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     
     
 setup(name='Chronix2Grid',
-      version='1.2.0',
+      version='1.2.0.post1',
       description='A python package to generate "en-masse" chronics for loads and productions (thermal, renewable)',
       long_description=long_description,
       long_description_content_type='text/markdown',
       classifiers=[
           'Development Status :: 4 - Beta',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
           "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
           "Intended Audience :: Developers",
           "Intended Audience :: Education",
           "Intended Audience :: Science/Research",
           "Natural Language :: English"
       ],
       keywords='ML powergrid optmization RL power-systems chronics generation production load network',
```

