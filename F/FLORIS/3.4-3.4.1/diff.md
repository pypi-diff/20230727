# Comparing `tmp/FLORIS-3.4.tar.gz` & `tmp/FLORIS-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLORIS-3.4.tar", last modified: Tue May 16 17:48:20 2023, max compression
+gzip compressed data, was "FLORIS-3.4.1.tar", last modified: Thu Jul 27 19:54:59 2023, max compression
```

## Comparing `FLORIS-3.4.tar` & `FLORIS-3.4.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.151147 FLORIS-3.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.131147 FLORIS-3.4/FLORIS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 17:48:20.000000 FLORIS-3.4/FLORIS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-16 17:48:20.000000 FLORIS-3.4/FLORIS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:48:20.000000 FLORIS-3.4/FLORIS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-16 17:48:20.000000 FLORIS-3.4/FLORIS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 17:48:20.000000 FLORIS-3.4/FLORIS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-16 17:48:08.000000 FLORIS-3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 17:48:20.151147 FLORIS-3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-16 17:48:08.000000 FLORIS-3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.131147 FLORIS-3.4/floris/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/logging_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.131147 FLORIS-3.4/floris/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15783 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/farm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/floris.py
--rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/flow_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    39069 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    58882 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    30621 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/turbine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.135147 FLORIS-3.4/floris/simulation/wake_combination/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_combination/fls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_combination/max.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_combination/sosfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.135147 FLORIS-3.4/floris/simulation/wake_deflection/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_deflection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_deflection/empirical_gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)    19670 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_deflection/gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_deflection/jimenez.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_deflection/none.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.135147 FLORIS-3.4/floris/simulation/wake_turbulence/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_turbulence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_turbulence/crespo_hernandez.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_turbulence/none.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_turbulence/wake_induced_mixing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.135147 FLORIS-3.4/floris/simulation/wake_velocity/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/cumulative_gauss_curl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/empirical_gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/jensen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/none.py
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/turbopark.py
--rw-r--r--   0 runner    (1001) docker     (123)  9163212 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/turbopark_lookup_table.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.147147 FLORIS-3.4/floris/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/cc_blade_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/cut_plane.py
--rw-r--r--   0 runner    (1001) docker     (123)    40510 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/floris_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/floris_interface_legacy_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/flow_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/interface_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/layout_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.147147 FLORIS-3.4/floris/tools/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.147147 FLORIS-3.4/floris/tools/optimization/layout_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/layout_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24334 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_boundary_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.147147 FLORIS-3.4/floris/tools/optimization/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.147147 FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/power_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/yaw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.147147 FLORIS-3.4/floris/tools/optimization/legacy/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/base_COE.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/cluster_turbines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/derive_downstream_turbines.py
--rw-r--r--   0 runner    (1001) docker     (123)    16134 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/layout_height.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    18216 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/power_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/power_density_1D.py
--rw-r--r--   0 runner    (1001) docker     (123)    30497 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw.py
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_clustered.py
--rw-r--r--   0 runner    (1001) docker     (123)    46052 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose.py
--rw-r--r--   0 runner    (1001) docker     (123)    21991 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose_clustered.py
--rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    30220 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel_clustered.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.147147 FLORIS-3.4/floris/tools/optimization/other/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13489 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/other/boundary_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.151147 FLORIS-3.4/floris/tools/optimization/yaw_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/yaw_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33490 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimization_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimization_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimizer_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimizer_sr.py
--rw-r--r--   0 runner    (1001) docker     (123)    20989 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/parallel_computing_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/power_rose.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/rews.py
--rw-r--r--   0 runner    (1001) docker     (123)    21079 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/sowfa_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    30200 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/uncertainty_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    23948 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    61639 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/wind_rose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.151147 FLORIS-3.4/floris/turbine_library/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/turbine_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/turbine_library/iea_10MW.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/turbine_library/iea_15MW.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/turbine_library/nrel_5MW.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    33041 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/turbine_library/turbine_previewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/turbine_library/x_20MW.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/type_dec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-16 17:48:08.000000 FLORIS-3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:48:20.151147 FLORIS-3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-16 17:48:08.000000 FLORIS-3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.269574 FLORIS-3.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.245573 FLORIS-3.4.1/FLORIS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-27 19:54:59.000000 FLORIS-3.4.1/FLORIS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-27 19:54:59.000000 FLORIS-3.4.1/FLORIS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:54:59.000000 FLORIS-3.4.1/FLORIS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-27 19:54:59.000000 FLORIS-3.4.1/FLORIS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 19:54:59.000000 FLORIS-3.4.1/FLORIS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-27 19:54:50.000000 FLORIS-3.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-27 19:54:59.269574 FLORIS-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-27 19:54:50.000000 FLORIS-3.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.245573 FLORIS-3.4.1/floris/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/logging_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.249573 FLORIS-3.4.1/floris/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/farm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/floris.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/flow_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39069 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58882 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30621 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/turbine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.249573 FLORIS-3.4.1/floris/simulation/wake_combination/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_combination/fls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_combination/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_combination/sosfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.253573 FLORIS-3.4.1/floris/simulation/wake_deflection/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_deflection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_deflection/empirical_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19670 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_deflection/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_deflection/jimenez.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_deflection/none.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.253573 FLORIS-3.4.1/floris/simulation/wake_turbulence/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_turbulence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_turbulence/crespo_hernandez.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_turbulence/none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_turbulence/wake_induced_mixing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.257573 FLORIS-3.4.1/floris/simulation/wake_velocity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_velocity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_velocity/cumulative_gauss_curl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_velocity/empirical_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_velocity/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_velocity/jensen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_velocity/none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_velocity/turbopark.py
+-rw-r--r--   0 runner    (1001) docker     (123)  9163212 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/simulation/wake_velocity/turbopark_lookup_table.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.265573 FLORIS-3.4.1/floris/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/cc_blade_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/cut_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40510 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/floris_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/floris_interface_legacy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/flow_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/interface_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/layout_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.265573 FLORIS-3.4.1/floris/tools/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.269574 FLORIS-3.4.1/floris/tools/optimization/layout_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/layout_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/layout_optimization/layout_optimization_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24334 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/layout_optimization/layout_optimization_boundary_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/layout_optimization/layout_optimization_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.269574 FLORIS-3.4.1/floris/tools/optimization/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.269574 FLORIS-3.4.1/floris/tools/optimization/legacy/pyoptsparse/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/pyoptsparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/pyoptsparse/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/pyoptsparse/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/pyoptsparse/power_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/pyoptsparse/yaw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.269574 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/base_COE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/cluster_turbines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/derive_downstream_turbines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16134 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/layout_height.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18216 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/power_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/power_density_1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30497 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/yaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/yaw_clustered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46052 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/yaw_wind_rose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21991 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/yaw_wind_rose_clustered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30220 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel_clustered.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.269574 FLORIS-3.4.1/floris/tools/optimization/other/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13489 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/other/boundary_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.269574 FLORIS-3.4.1/floris/tools/optimization/yaw_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/yaw_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33490 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/yaw_optimization/yaw_optimization_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/yaw_optimization/yaw_optimization_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/yaw_optimization/yaw_optimizer_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/optimization/yaw_optimization/yaw_optimizer_sr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20989 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/parallel_computing_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/power_rose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/rews.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21079 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/sowfa_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30200 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/uncertainty_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23948 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61639 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/tools/wind_rose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:54:59.269574 FLORIS-3.4.1/floris/turbine_library/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/turbine_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/turbine_library/iea_10MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/turbine_library/iea_15MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/turbine_library/nrel_5MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    33041 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/turbine_library/turbine_previewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/turbine_library/x_20MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/type_dec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 19:54:50.000000 FLORIS-3.4.1/floris/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-27 19:54:50.000000 FLORIS-3.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 19:54:59.269574 FLORIS-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-27 19:54:50.000000 FLORIS-3.4.1/setup.py
```

### Comparing `FLORIS-3.4/FLORIS.egg-info/PKG-INFO` & `FLORIS-3.4.1/FLORIS.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLORIS
-Version: 3.4
+Version: 3.4.1
 Summary: A controls-oriented engineering wake model.
 Home-page: https://github.com/NREL/FLORIS
 Author: NREL National Wind Technology Center
 Author-email: rafael.mudafort@nrel.gov
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `FLORIS-3.4/FLORIS.egg-info/SOURCES.txt` & `FLORIS-3.4.1/FLORIS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/LICENSE.txt` & `FLORIS-3.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/PKG-INFO` & `FLORIS-3.4.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLORIS
-Version: 3.4
+Version: 3.4.1
 Summary: A controls-oriented engineering wake model.
 Home-page: https://github.com/NREL/FLORIS
 Author: NREL National Wind Technology Center
 Author-email: rafael.mudafort@nrel.gov
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `FLORIS-3.4/README.md` & `FLORIS-3.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # FLORIS Wake Modeling and Wind Farm Controls Software
 
 FLORIS is a controls-focused wind farm simulation software incorporating
 steady-state engineering wake models into a performance-focused Python
 framework. It has been in active development at NREL since 2013 and the latest
-release is [FLORIS v3.4](https://github.com/NREL/floris/releases/latest).
+release is [FLORIS v3.4.1](https://github.com/NREL/floris/releases/latest).
 Online documentation is available at https://nrel.github.io/floris.
 
 The software is in active development and engagement with the development team
 is highly encouraged. If you are interested in using FLORIS to conduct studies
 of a wind farm or extending FLORIS to include your own wake model, please join
 the conversation in [GitHub Discussions](https://github.com/NREL/floris/discussions/)!
```

### Comparing `FLORIS-3.4/floris/__init__.py` & `FLORIS-3.4.1/floris/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/logging_manager.py` & `FLORIS-3.4.1/floris/logging_manager.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/__init__.py` & `FLORIS-3.4.1/floris/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/base.py` & `FLORIS-3.4.1/floris/simulation/base.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/farm.py` & `FLORIS-3.4.1/floris/simulation/farm.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,34 +58,47 @@
     # TODO: turbine_type should be immutable
     turbine_type: List = field(validator=iter_validator(list, (dict, str)))
     turbine_library_path: Path = field(
         default=default_turbine_library_path, converter=convert_to_path
     )
 
     turbine_definitions: list = field(init=False, validator=iter_validator(list, dict))
+    coordinates: List[Vec3] = field(init=False)
+    turbine_fCts: tuple = field(init=False, default=[])
+    turbine_fTilts: list = field(init=False, default=[])
+
     yaw_angles: NDArrayFloat = field(init=False)
     yaw_angles_sorted: NDArrayFloat = field(init=False)
+
     tilt_angles: NDArrayFloat = field(init=False)
     tilt_angles_sorted: NDArrayFloat = field(init=False)
-    coordinates: List[Vec3] = field(init=False)
+
     hub_heights: NDArrayFloat = field(init=False)
     hub_heights_sorted: NDArrayFloat = field(init=False, default=[])
-    turbine_fCts: tuple = field(init=False, default=[])
+
+    turbine_type_map: NDArrayObject = field(init=False, default=[])
     turbine_type_map_sorted: NDArrayObject = field(init=False, default=[])
+
+    rotor_diameters: NDArrayFloat = field(init=False, default=[])
     rotor_diameters_sorted: NDArrayFloat = field(init=False, default=[])
+
+    TSRs: NDArrayFloat = field(init=False, default=[])
     TSRs_sorted: NDArrayFloat = field(init=False, default=[])
+
     pPs: NDArrayFloat = field(init=False, default=[])
     pPs_sorted: NDArrayFloat = field(init=False, default=[])
+
     pTs: NDArrayFloat = field(init=False, default=[])
     pTs_sorted: NDArrayFloat = field(init=False, default=[])
+
     ref_tilt_cp_cts: NDArrayFloat = field(init=False, default=[])
     ref_tilt_cp_cts_sorted: NDArrayFloat = field(init=False, default=[])
+
     correct_cp_ct_for_tilt: NDArrayFloat = field(init=False, default=[])
     correct_cp_ct_for_tilt_sorted: NDArrayFloat = field(init=False, default=[])
-    turbine_fTilts: list = field(init=False, default=[])
 
     def __attrs_post_init__(self) -> None:
         # Turbine definitions can be supplied in three ways:
         # - A string selecting a turbine in the floris turbine library
         # - A Python dict representation of a turbine definition
         #   - There's an option to use the yaml keyword "!include" which results in the yaml
         #     library preprocessing the inputs and loading the specified file directly into
@@ -297,23 +310,24 @@
             axis=2
         )
         self.pTs_sorted = np.take_along_axis(
             self.pTs * template_shape,
             sorted_coord_indices,
             axis=2
         )
+
+        # NOTE: Tilt angles are sorted twice - here and in initialize()
         self.tilt_angles_sorted = np.take_along_axis(
             self.tilt_angles * template_shape,
             sorted_coord_indices,
             axis=2
         )
-        self.turbine_type_names_sorted = [turb["turbine_type"] for turb in self.turbine_definitions]
         self.turbine_type_map_sorted = np.take_along_axis(
             np.reshape(
-                self.turbine_type_names_sorted * n_wind_directions,
+                [turb["turbine_type"] for turb in self.turbine_definitions] * n_wind_directions,
                 np.shape(sorted_coord_indices)
             ),
             sorted_coord_indices,
             axis=2
         )
 
     def set_yaw_angles(self, n_wind_directions: int, n_wind_speeds: int):
@@ -362,14 +376,30 @@
             axis=2
         )
         self.TSRs = np.take_along_axis(
             self.TSRs_sorted,
             unsorted_indices[:,:,:,0,0],
             axis=2
         )
+        # TODO: do these need to be unsorted? Maybe we should just for completeness...
+        self.ref_density_cp_cts = np.take_along_axis(
+            self.ref_density_cp_cts_sorted,
+            unsorted_indices[:,:,:,0,0],
+            axis=2
+        )
+        self.ref_tilt_cp_cts = np.take_along_axis(
+            self.ref_tilt_cp_cts_sorted,
+            unsorted_indices[:,:,:,0,0],
+            axis=2
+        )
+        self.correct_cp_ct_for_tilt = np.take_along_axis(
+            self.correct_cp_ct_for_tilt_sorted,
+            unsorted_indices[:,:,:,0,0],
+            axis=2
+        )
         self.pPs = np.take_along_axis(
             self.pPs_sorted,
             unsorted_indices[:,:,:,0,0],
             axis=2
         )
         self.pTs = np.take_along_axis(
             self.pTs_sorted,
```

### Comparing `FLORIS-3.4/floris/simulation/floris.py` & `FLORIS-3.4.1/floris/simulation/floris.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/flow_field.py` & `FLORIS-3.4.1/floris/simulation/flow_field.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/grid.py` & `FLORIS-3.4.1/floris/simulation/grid.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/solver.py` & `FLORIS-3.4.1/floris/simulation/solver.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/turbine.py` & `FLORIS-3.4.1/floris/simulation/turbine.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake.py` & `FLORIS-3.4.1/floris/simulation/wake.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_combination/__init__.py` & `FLORIS-3.4.1/floris/simulation/wake_combination/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_combination/fls.py` & `FLORIS-3.4.1/floris/simulation/wake_combination/fls.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_combination/max.py` & `FLORIS-3.4.1/floris/simulation/wake_combination/max.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_combination/sosfs.py` & `FLORIS-3.4.1/floris/simulation/wake_combination/sosfs.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_deflection/__init__.py` & `FLORIS-3.4.1/floris/simulation/wake_deflection/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_deflection/empirical_gauss.py` & `FLORIS-3.4.1/floris/simulation/wake_deflection/empirical_gauss.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_deflection/gauss.py` & `FLORIS-3.4.1/floris/simulation/wake_deflection/gauss.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_deflection/jimenez.py` & `FLORIS-3.4.1/floris/simulation/wake_deflection/jimenez.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_deflection/none.py` & `FLORIS-3.4.1/floris/simulation/wake_deflection/none.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_turbulence/__init__.py` & `FLORIS-3.4.1/floris/simulation/wake_turbulence/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_turbulence/crespo_hernandez.py` & `FLORIS-3.4.1/floris/simulation/wake_turbulence/crespo_hernandez.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_turbulence/none.py` & `FLORIS-3.4.1/floris/simulation/wake_turbulence/none.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_turbulence/wake_induced_mixing.py` & `FLORIS-3.4.1/floris/simulation/wake_turbulence/wake_induced_mixing.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_velocity/__init__.py` & `FLORIS-3.4.1/floris/simulation/wake_velocity/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_velocity/cumulative_gauss_curl.py` & `FLORIS-3.4.1/floris/simulation/wake_velocity/cumulative_gauss_curl.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_velocity/empirical_gauss.py` & `FLORIS-3.4.1/floris/simulation/wake_velocity/empirical_gauss.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_velocity/gauss.py` & `FLORIS-3.4.1/floris/simulation/wake_velocity/gauss.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_velocity/jensen.py` & `FLORIS-3.4.1/floris/simulation/wake_velocity/jensen.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_velocity/none.py` & `FLORIS-3.4.1/floris/simulation/wake_velocity/none.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_velocity/turbopark.py` & `FLORIS-3.4.1/floris/simulation/wake_velocity/turbopark.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/simulation/wake_velocity/turbopark_lookup_table.mat` & `FLORIS-3.4.1/floris/simulation/wake_velocity/turbopark_lookup_table.mat`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/__init__.py` & `FLORIS-3.4.1/floris/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/cc_blade_utilities.py` & `FLORIS-3.4.1/floris/tools/cc_blade_utilities.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/cut_plane.py` & `FLORIS-3.4.1/floris/tools/cut_plane.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/floris_interface.py` & `FLORIS-3.4.1/floris/tools/floris_interface.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/floris_interface_legacy_reader.py` & `FLORIS-3.4.1/floris/tools/floris_interface_legacy_reader.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/flow_data.py` & `FLORIS-3.4.1/floris/tools/flow_data.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/interface_utilities.py` & `FLORIS-3.4.1/floris/tools/interface_utilities.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/layout_functions.py` & `FLORIS-3.4.1/floris/tools/layout_functions.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_base.py` & `FLORIS-3.4.1/floris/tools/optimization/layout_optimization/layout_optimization_base.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_boundary_grid.py` & `FLORIS-3.4.1/floris/tools/optimization/layout_optimization/layout_optimization_boundary_grid.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse.py` & `FLORIS-3.4.1/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py` & `FLORIS-3.4.1/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_scipy.py` & `FLORIS-3.4.1/floris/tools/optimization/layout_optimization/layout_optimization_scipy.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/layout.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/pyoptsparse/layout.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/optimization.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/pyoptsparse/optimization.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/power_density.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/pyoptsparse/power_density.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/yaw.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/pyoptsparse/yaw.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/scipy/base_COE.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/base_COE.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/scipy/cluster_turbines.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/cluster_turbines.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/scipy/derive_downstream_turbines.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/derive_downstream_turbines.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/scipy/layout.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/layout.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/scipy/layout_height.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/layout_height.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/scipy/optimization.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/optimization.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/scipy/power_density.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/power_density.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/scipy/power_density_1D.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/power_density_1D.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/yaw.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_clustered.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/yaw_clustered.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/yaw_wind_rose.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose_clustered.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/yaw_wind_rose_clustered.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel_clustered.py` & `FLORIS-3.4.1/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel_clustered.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/other/boundary_grid.py` & `FLORIS-3.4.1/floris/tools/optimization/other/boundary_grid.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimization_base.py` & `FLORIS-3.4.1/floris/tools/optimization/yaw_optimization/yaw_optimization_base.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimization_tools.py` & `FLORIS-3.4.1/floris/tools/optimization/yaw_optimization/yaw_optimization_tools.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimizer_scipy.py` & `FLORIS-3.4.1/floris/tools/optimization/yaw_optimization/yaw_optimizer_scipy.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimizer_sr.py` & `FLORIS-3.4.1/floris/tools/optimization/yaw_optimization/yaw_optimizer_sr.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/parallel_computing_interface.py` & `FLORIS-3.4.1/floris/tools/parallel_computing_interface.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/power_rose.py` & `FLORIS-3.4.1/floris/tools/power_rose.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/rews.py` & `FLORIS-3.4.1/floris/tools/rews.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/sowfa_utilities.py` & `FLORIS-3.4.1/floris/tools/sowfa_utilities.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/uncertainty_interface.py` & `FLORIS-3.4.1/floris/tools/uncertainty_interface.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/visualization.py` & `FLORIS-3.4.1/floris/tools/visualization.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/tools/wind_rose.py` & `FLORIS-3.4.1/floris/tools/wind_rose.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/turbine_library/iea_10MW.yaml` & `FLORIS-3.4.1/floris/turbine_library/iea_10MW.yaml`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/turbine_library/iea_15MW.yaml` & `FLORIS-3.4.1/floris/turbine_library/iea_15MW.yaml`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/turbine_library/nrel_5MW.yaml` & `FLORIS-3.4.1/floris/turbine_library/nrel_5MW.yaml`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/turbine_library/turbine_previewer.py` & `FLORIS-3.4.1/floris/turbine_library/turbine_previewer.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/turbine_library/x_20MW.yaml` & `FLORIS-3.4.1/floris/turbine_library/x_20MW.yaml`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/type_dec.py` & `FLORIS-3.4.1/floris/type_dec.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/floris/utilities.py` & `FLORIS-3.4.1/floris/utilities.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/pyproject.toml` & `FLORIS-3.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FLORIS-3.4/setup.py` & `FLORIS-3.4.1/setup.py`

 * *Files identical despite different names*

