# Comparing `tmp/power-grid-model-1.5.0rc9231316741137.tar.gz` & `tmp/power-grid-model-1.5.0rc9232816587778.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-grid-model-1.5.0rc9231316741137.tar", last modified: Wed Jul 26 12:06:16 2023, max compression
+gzip compressed data, was "power-grid-model-1.5.0rc9232816587778.tar", last modified: Thu Jul 27 14:27:55 2023, max compression
```

## Comparing `power-grid-model-1.5.0rc9231316741137.tar` & `power-grid-model-1.5.0rc9232816587778.tar`

### file list

```diff
@@ -1,593 +1,593 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.354492 power-grid-model-1.5.0rc9231316741137/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-26 12:06:16.354492 power-grid-model-1.5.0rc9231316741137/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-26 12:05:30.000000 power-grid-model-1.5.0rc9231316741137/PYPI_VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.282490 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.282490 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.274490 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.282490 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.286490 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.286490 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
--rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.286490 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.286490 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    53717 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.294490 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    41768 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    25143 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30907 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.294490 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.294490 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.294490 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
--rw-r--r--   0 runner    (1001) docker     (123)    55882 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.294490 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/buffer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    93852 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/handle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/handle.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/model.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/options.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/options.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:06:16.354492 power-grid-model-1.5.0rc9231316741137/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.278490 power-grid-model-1.5.0rc9231316741137/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.294490 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.298490 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/core/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/core/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/core/index_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/core/power_grid_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/core/power_grid_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/core/power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.298490 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/validation/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    35027 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/validation/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29999 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.298490 power-grid-model-1.5.0rc9231316741137/src/power_grid_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-26 12:06:16.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35498 2023-07-26 12:06:16.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:06:16.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-26 12:06:16.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 12:06:16.000000 power-grid-model-1.5.0rc9231316741137/src/power_grid_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.282490 power-grid-model-1.5.0rc9231316741137/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.282490 power-grid-model-1.5.0rc9231316741137/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.282490 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.298490 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.298490 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.302491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.302491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.302491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.302491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-incomplete-input/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.306491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.306491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.306491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-newton/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-newton/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-newton/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-newton/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-newton/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.306491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-i-n-optional/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-i-n-optional/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-i-n-optional/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.310491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/gaia-example/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/gaia-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/gaia-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/gaia-example/gaia_grid.gnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/gaia-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/gaia-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/gaia-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/gaia-example/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.310491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/multi-source-with-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/multi-source-with-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/multi-source-with-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/multi-source-with-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/multi-source-with-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/multi-source-with-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.278490 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.278490 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.278490 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.310491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.310491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.310491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.310491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.314491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.314491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.314491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.318491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.318491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.278490 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.318491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/basic-node/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.322491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.322491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.322491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.322491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.322491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.326491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.326491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.326491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.282490 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.278490 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.330491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.330491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.282490 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.330491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.330491 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.334492 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/r-state-estimation/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/r-state-estimation/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/r-state-estimation/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/r-state-estimation/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/r-state-estimation/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/r-state-estimation/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/r-state-estimation/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.334492 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/three-winding-transformer/
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/three-winding-transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/three-winding-transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/three-winding-transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/three-winding-transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/three-winding-transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/three-winding-transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.334492 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-example/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-example/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-example/vision_grid.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-example/vision_grid.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.338492 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-validation-network/
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-validation-network/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-validation-network/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-validation-network/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-validation-network/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-validation-network/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-validation-network/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-validation-network/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-validation-network/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.282490 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.338492 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/single_phase_to_ground/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/single_phase_to_ground/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/single_phase_to_ground/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/single_phase_to_ground/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/single_phase_to_ground/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   243263 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/single_phase_to_ground/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/single_phase_to_ground/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.338492 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/three_phase/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/three_phase/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/three_phase/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/three_phase/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/three_phase/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58928 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/three_phase/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/three_phase/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/three_phase/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/three_phase/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.342492 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   236282 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.342492 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase_to_ground/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase_to_ground/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase_to_ground/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase_to_ground/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase_to_ground/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   242819 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase_to_ground/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase_to_ground/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.282490 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.342492 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.342492 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr-no-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr-no-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr-no-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr-no-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr-no-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.346492 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.346492 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/dummy-test-sym/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/dummy-test-sym/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/dummy-test-sym/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/dummy-test-sym/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/dummy-test-sym/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/dummy-test-sym/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.346492 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.346492 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/residual-test/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/residual-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/residual-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/residual-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/residual-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/residual-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/residual-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.346492 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/single-line-load/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/single-line-load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/single-line-load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/single-line-load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/single-line-load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/single-line-load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/single-line-load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.350492 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/three_winding_transformer/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.350492 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.350492 power-grid-model-1.5.0rc9231316741137/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/unit/test_0Z_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/unit/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/unit/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/unit/test_power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/unit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:06:16.354492 power-grid-model-1.5.0rc9231316741137/tests/unit/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/unit/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/unit/validation/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/unit/validation/test_batch_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/unit/validation/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/unit/validation/test_input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/unit/validation/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/unit/validation/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-07-26 12:05:25.000000 power-grid-model-1.5.0rc9231316741137/tests/unit/validation/test_validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.655530 power-grid-model-1.5.0rc9232816587778/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-27 14:27:55.655530 power-grid-model-1.5.0rc9232816587778/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 14:27:08.000000 power-grid-model-1.5.0rc9232816587778/PYPI_VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.595528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.595528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.587528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.595528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.595528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.595528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.599528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.599528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23037 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    61980 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.599528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41768 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30907 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.599528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.599528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.599528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    55882 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.603528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/buffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    93852 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/handle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/handle.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/options.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:27:55.655530 power-grid-model-1.5.0rc9232816587778/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.587528 power-grid-model-1.5.0rc9232816587778/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.603528 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.603528 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/index_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/power_grid_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/power_grid_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.607529 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35027 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29999 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.603528 power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-27 14:27:55.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35498 2023-07-27 14:27:55.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:27:55.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-27 14:27:55.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 14:27:55.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.607529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.607529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.607529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.607529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.611528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.611528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.611528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.615529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.615529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.615529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.615529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/gaia_grid.gnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.615529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.619529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.619529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.619529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.619529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.619529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.623529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.623529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.623529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.623529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.627529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.627529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.627529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.627529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.627529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.631529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.631529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.631529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.631529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.635529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.635529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.635529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.635529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.639529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.639529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.639529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/vision_grid.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/vision_grid.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.639529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.643529 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   243263 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.643529 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58928 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.643529 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   236282 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.647529 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   242819 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.647529 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.647529 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.647529 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.647529 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.651530 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.651530 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/residual-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/residual-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/residual-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/residual-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/residual-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/residual-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/residual-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.651530 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.651530 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.651530 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.651530 power-grid-model-1.5.0rc9232816587778/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/test_0Z_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/test_power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.655530 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_batch_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_validation_functions.py
```

### Comparing `power-grid-model-1.5.0rc9231316741137/LICENSE` & `power-grid-model-1.5.0rc9232816587778/LICENSE`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/PKG-INFO` & `power-grid-model-1.5.0rc9232816587778/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9231316741137
+Version: 1.5.0rc9232816587778
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9231316741137/README.md` & `power-grid-model-1.5.0rc9232816587778/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/CMakeLists.txt` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -124,19 +124,19 @@
     IdxVector load_gen_power_sensor_indptr;     // indptr of the load_gen
     IdxVector shunt_power_sensor_indptr;        // indptr of the shunt
     IdxVector branch_from_power_sensor_indptr;  // indptr of the branch
     IdxVector branch_to_power_sensor_indptr;    // indptr of the branch
     IdxVector bus_power_sensor_indptr;          // indptr of the bus
 
     Idx n_bus() const {
-        return (Idx)phase_shift.size();
+        return static_cast<Idx>(phase_shift.size());
     }
 
     Idx n_branch() const {
-        return (Idx)branch_bus_idx.size();
+        return static_cast<Idx>(branch_bus_idx.size());
     }
 
     Idx n_source() const {
         return source_bus_indptr.back();
     }
 
     Idx n_shunt() const {
```

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,18 @@
         if constexpr (sym) {
             return get_output<true>(sym_u2si(u));
         }
         else {
             return get_output<false>(asym_u2si(u));
         }
     }
+    template <bool sym>
+    ApplianceShortCircuitOutput get_sc_output(ApplianceShortCircuitMathOutput<sym> const& appliance_math_output) const {
+        return get_sc_output(appliance_math_output.i);
+    }
 
    private:
     ID node_;
     bool status_;
     double base_i_;
 
     // pure virtual functions for translate from u to s/i
```

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -22,18 +22,18 @@
     using OutputType = BaseOutput;
     static constexpr char const* name = "base";
     virtual ComponentType math_model_type() const = 0;
 
     explicit Base(BaseInput const& base_input) : id_{base_input.id} {
     }
     virtual ~Base() = default;
-    ID id() const noexcept {
+    constexpr ID id() const noexcept {
         return id_;
     }
-    BaseOutput base_output(bool is_energized) const {
+    constexpr BaseOutput base_output(bool is_energized) const {
         return BaseOutput{id_, static_cast<IntS>(is_energized)};
     }
     virtual bool energized(bool is_connected_to_source) const = 0;
 
     Base(Base&&) = default;
     Base& operator=(Base&&) = default;
```

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -109,31 +109,35 @@
         output.s_to = base_power<sym> * cabs(branch_math_output.s_t);
         double const max_s = std::max(sum_val(output.s_from), sum_val(output.s_to));
         double const max_i = std::max(max_val(output.i_from), max_val(output.i_to));
         output.loading = loading(max_s, max_i);
         return output;
     }
 
+    BranchShortCircuitOutput get_sc_output(ComplexValue<true> const& i_f, ComplexValue<true> const& i_t) const {
+        return get_sc_output(BranchShortCircuitMathOutput<true>{.i_f = i_f, .i_t = i_t});
+    }
     BranchShortCircuitOutput get_sc_output(ComplexValue<false> const& i_f, ComplexValue<false> const& i_t) const {
-        // result object
+        return get_sc_output(BranchShortCircuitMathOutput<false>{.i_f = i_f, .i_t = i_t});
+    }
+
+    BranchShortCircuitOutput get_sc_output(BranchShortCircuitMathOutput<false> const& branch_math_output) const {
         BranchShortCircuitOutput output{};
         static_cast<BaseOutput&>(output) = base_output(true);
         // calculate result
-        output.i_from = base_i_from() * cabs(i_f);
-        output.i_to = base_i_to() * cabs(i_t);
-        output.i_from_angle = arg(i_f);
-        output.i_to_angle = arg(i_t);
+        output.i_from = base_i_from() * cabs(branch_math_output.i_f);
+        output.i_to = base_i_to() * cabs(branch_math_output.i_t);
+        output.i_from_angle = arg(branch_math_output.i_f);
+        output.i_to_angle = arg(branch_math_output.i_t);
         return output;
     }
 
-    BranchShortCircuitOutput get_sc_output(ComplexValue<true> const& i_f, ComplexValue<true> const& i_t) const {
-        // Convert the input of only positive sequence to abc
-        ComplexValue<false> const iabc_f{i_f};
-        ComplexValue<false> const iabc_t{i_t};
-        return get_sc_output(iabc_f, iabc_t);
+    BranchShortCircuitOutput get_sc_output(BranchShortCircuitMathOutput<true> const& branch_math_output) const {
+        return get_sc_output(BranchShortCircuitMathOutput<false>{.i_f = ComplexValue<false>{branch_math_output.i_f},
+                                                                 .i_t = ComplexValue<false>{branch_math_output.i_t}});
     }
 
     template <bool sym>
     BranchOutput<sym> get_null_output() const {
         BranchOutput<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(false);
         return output;
```

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -132,14 +132,20 @@
     Branch3ShortCircuitOutput get_sc_output(ComplexValue<true> const& i_1, ComplexValue<true> const& i_2,
                                             ComplexValue<true> const& i_3) const {
         ComplexValue<false> const iabc_1{i_1};
         ComplexValue<false> const iabc_2{i_2};
         ComplexValue<false> const iabc_3{i_3};
         return get_sc_output(iabc_1, iabc_2, iabc_3);
     }
+    template <bool sym>
+    Branch3ShortCircuitOutput get_sc_output(BranchShortCircuitMathOutput<sym> const& branch_math_output1,
+                                            BranchShortCircuitMathOutput<sym> const& branch_math_output2,
+                                            BranchShortCircuitMathOutput<sym> const& branch_math_output3) const {
+        return get_sc_output(branch_math_output1.i_f, branch_math_output2.i_f, branch_math_output3.i_f);
+    }
 
     template <bool sym>
     Branch3Output<sym> get_null_output() const {
         Branch3Output<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(false);
         return output;
     }
```

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -58,24 +58,24 @@
         // calculate the fault admittance in p.u.
         double const base_z = u_rated * u_rated / base_power_3p;
         param.y_fault = base_z / (r_f_ + 1.0i * x_f_);
         return param;
     }
 
     FaultOutput get_null_output() const {
-        FaultOutput output{};
-        static_cast<BaseOutput&>(output) = base_output(false);
-        return output;
+        return get_null_output_impl<FaultOutput>();
     }
     FaultOutput get_output() const {
         // During power flow and state estimation the fault object will have an empty output
         return get_null_output();
     }
 
-    // energized
+    FaultShortCircuitOutput get_null_sc_output() const {
+        return get_null_output_impl<FaultShortCircuitOutput>();
+    }
     FaultShortCircuitOutput get_sc_output(ComplexValue<false> i_f, double const u_rated) const {
         // translate pu to A
         double const base_i = base_power_3p / u_rated / sqrt3;
         i_f = i_f * base_i;
         // result object
         FaultShortCircuitOutput output{};
         static_cast<BaseOutput&>(output) = base_output(true);
@@ -85,14 +85,20 @@
     }
 
     FaultShortCircuitOutput get_sc_output(ComplexValue<true> i_f, double const u_rated) const {
         ComplexValue<false> const iabc_f{i_f};
         return get_sc_output(iabc_f, u_rated);
     }
 
+    template <bool sym>
+    FaultShortCircuitOutput get_sc_output(FaultShortCircuitMathOutput<sym> const& math_output,
+                                          double const u_rated) const {
+        return get_sc_output(math_output.i_fault, u_rated);
+    }
+
     // update faulted object
     UpdateChange update(FaultUpdate const& update) {
         assert(update.id == id());
         set_status(update.status);
         if (update.fault_type != FaultType::nan) {
             fault_type_ = update.fault_type;
         }
@@ -171,14 +177,21 @@
     bool status_;
     FaultType fault_type_;
     FaultPhase fault_phase_;
     ID fault_object_;
     double r_f_;
     double x_f_;
 
+    template <std::derived_from<BaseOutput> T>
+    T get_null_output_impl() const {
+        T output{};
+        static_cast<BaseOutput&>(output) = base_output(false);
+        return output;
+    }
+
     void check_sanity() {
         using enum FaultPhase;
 
         auto const check_supported = [&](auto const& iterable) {
             if (std::find(cbegin(iterable), cend(iterable), fault_phase_) == cend(iterable)) {
                 throw InvalidShortCircuitPhases(fault_type_, fault_phase_);
             }
```

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 class Node final : public Base {
    public:
     using InputType = NodeInput;
     template <bool sym>
     using OutputType = NodeOutput<sym>;
     using ShortCircuitOutputType = NodeShortCircuitOutput;
     static constexpr char const* name = "node";
-    ComponentType math_model_type() const final {
+    constexpr ComponentType math_model_type() const final {
         return ComponentType::node;
     }
 
     explicit Node(NodeInput const& node_input) : Base{node_input}, u_rated_{node_input.u_rated} {
     }
 
     // update node, nothing happens here
-    UpdateChange update(BaseUpdate const&) {
+    constexpr UpdateChange update(BaseUpdate const&) {
         return {false, false};
     }
 
     // energized
     template <bool sym>
     NodeOutput<sym> get_output(ComplexValue<sym> const& u_pu, ComplexValue<sym> const& bus_injection) const {
         NodeOutput<sym> output{};
@@ -72,18 +72,18 @@
 
     NodeShortCircuitOutput get_null_sc_output() const {
         NodeShortCircuitOutput output{};
         static_cast<BaseOutput&>(output) = base_output(false);
         return output;
     }
 
-    double u_rated() {
+    constexpr double u_rated() const {
         return u_rated_;
     }
-    bool energized(bool is_connected_to_source) const final {
+    constexpr bool energized(bool is_connected_to_source) const final {
         return is_connected_to_source;
     }
 
    private:
     double u_rated_;
 };
```

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,18 @@
     }
 
     template <bool sym>
     PowerSensorOutput<sym> get_null_output() const {
         return {{id(), false}, {}, {}};
     }
 
+    SensorShortCircuitOutput get_null_sc_output() const {
+        return {{id(), false}};
+    }
+
    protected:
     double convert_direction() const {
         if (terminal_type_ == MeasuredTerminalType::load || terminal_type_ == MeasuredTerminalType::shunt) {
             return -1.0;  // For shunt and load the direction in the math model is opposite to the direction in the
                           // physical model
         }
         else {
```

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,18 @@
     }
 
     template <bool sym>
     VoltageSensorOutput<sym> get_null_output() const {
         return {{id(), false}, {}, {}};
     }
 
+    SensorShortCircuitOutput get_null_sc_output() const {
+        return {{id(), false}};
+    }
+
    private:
     virtual VoltageSensorOutput<true> get_sym_output(ComplexValue<true> const& u) const = 0;
     virtual VoltageSensorOutput<false> get_asym_output(ComplexValue<false> const& u) const = 0;
 };
 
 template <bool sym>
 class VoltageSensor : public GenericVoltageSensor {
```

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     return state.comp_topo->power_sensor_object_idx.cbegin() +
            comp_sequence_offset<GenericPowerSensor, Component>(state);
 }
 
 template <std::same_as<Fault> Component, class ComponentContainer>
 requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr auto comp_base_sequence_cbegin(MainModelState<ComponentContainer> const& state) {
-    return state.comp_coup->fault.cbegin();
+    return state.comp_coup.fault.cbegin();
 }
 
 template <typename Component, typename IndexType, class ComponentContainer, std::forward_iterator ResIt,
           typename ResFunc>
 requires model_component_state<MainModelState, ComponentContainer, Component> &&
     std::invocable<std::remove_cvref_t<ResFunc>, Component const&, IndexType>&&
         std::convertible_to<std::invoke_result_t<ResFunc, Component const&, IndexType>, std::iter_value_t<ResIt>>&&
@@ -89,63 +89,102 @@
                           state.components.template citer<Component>().end(),
                           comp_base_sequence_cbegin<Component>(state), res_it, func);
 }
 
 }  // namespace detail
 
 // output node
-template <std::same_as<Node> Component, class ComponentContainer, math_output_type MathOutputType,
+template <std::same_as<Node> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
 requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Node, Idx2D>(state, res_it, [&math_output](Node const& node, Idx2D math_id) {
         constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
         if (math_id.group == -1) {
             return node.get_null_output<sym>();
         }
         return node.get_output<sym>(math_output[math_id.group].u[math_id.pos],
                                     math_output[math_id.group].bus_injection[math_id.pos]);
     });
 }
+template <std::same_as<Node> Component, class ComponentContainer, short_circuit_math_output_type MathOutputType,
+          std::forward_iterator ResIt>
+requires model_component_state<MainModelState, ComponentContainer, Component>
+constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
+                              std::vector<MathOutputType> const& math_output, ResIt res_it) {
+    return detail::produce_output<Node, Idx2D>(state, res_it, [&math_output](Node const& node, Idx2D math_id) {
+        if (math_id.group == -1) {
+            return node.get_null_sc_output();
+        }
+        return node.get_sc_output(math_output[math_id.group].u_bus[math_id.pos]);
+    });
+}
 
 // output branch
-template <std::derived_from<Branch> Component, class ComponentContainer, math_output_type MathOutputType,
+template <std::derived_from<Branch> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
 requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(state, res_it, [&math_output](Branch const& branch, Idx2D math_id) {
         constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
         if (math_id.group == -1) {
             return branch.get_null_output<sym>();
         }
         return branch.get_output<sym>(math_output[math_id.group].branch[math_id.pos]);
     });
 }
+template <std::derived_from<Branch> Component, class ComponentContainer, short_circuit_math_output_type MathOutputType,
+          std::forward_iterator ResIt>
+requires model_component_state<MainModelState, ComponentContainer, Component>
+constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
+                              std::vector<MathOutputType> const& math_output, ResIt res_it) {
+    return detail::produce_output<Component, Idx2D>(state, res_it, [&math_output](Branch const& branch, Idx2D math_id) {
+        if (math_id.group == -1) {
+            return branch.get_null_sc_output();
+        }
+        return branch.get_sc_output(math_output[math_id.group].branch[math_id.pos]);
+    });
+}
 
 // output branch3
-template <std::derived_from<Branch3> Component, class ComponentContainer, math_output_type MathOutputType,
+template <std::derived_from<Branch3> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
 requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2DBranch3>(
         state, res_it, [&math_output](Branch3 const& branch3, Idx2DBranch3 math_id) {
             constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
             if (math_id.group == -1) {
                 return branch3.get_null_output<sym>();
             }
 
-            return branch3.get_output<sym>(math_output[math_id.group].branch[math_id.pos[0]],
-                                           math_output[math_id.group].branch[math_id.pos[1]],
-                                           math_output[math_id.group].branch[math_id.pos[2]]);
+            auto const& branches = math_output[math_id.group].branch;
+            return branch3.get_output<sym>(branches[math_id.pos[0]], branches[math_id.pos[1]],
+                                           branches[math_id.pos[2]]);
+        });
+}
+template <std::derived_from<Branch3> Component, class ComponentContainer, short_circuit_math_output_type MathOutputType,
+          std::forward_iterator ResIt>
+requires model_component_state<MainModelState, ComponentContainer, Component>
+constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
+                              std::vector<MathOutputType> const& math_output, ResIt res_it) {
+    return detail::produce_output<Component, Idx2DBranch3>(
+        state, res_it, [&math_output](Branch3 const& branch3, Idx2DBranch3 math_id) {
+            if (math_id.group == -1) {
+                return branch3.get_null_sc_output();
+            }
+
+            auto const& branches = math_output[math_id.group].branch;
+            return branch3.get_sc_output(branches[math_id.pos[0]], branches[math_id.pos[1]], branches[math_id.pos[2]]);
         });
 }
 
 // output source, load_gen, shunt individually
 template <std::same_as<Appliance> Component, class ComponentContainer, math_output_type MathOutputType,
           std::forward_iterator ResIt>
 requires model_component_state<MainModelState, ComponentContainer, Component>
@@ -154,83 +193,127 @@
     res_it = output_result<Source>(state, math_output, res_it);
     res_it = output_result<GenericLoadGen>(state, math_output, res_it);
     res_it = output_result<Shunt>(state, math_output, res_it);
     return res_it;
 }
 
 // output source
-template <std::same_as<Source> Component, class ComponentContainer, math_output_type MathOutputType,
+template <std::same_as<Source> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
 requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(state, res_it, [&math_output](Source const& source, Idx2D math_id) {
         constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
         if (math_id.group == -1) {
             return source.get_null_output<sym>();
         }
         return source.get_output<sym>(math_output[math_id.group].source[math_id.pos]);
     });
 }
+template <std::same_as<Source> Component, class ComponentContainer, short_circuit_math_output_type MathOutputType,
+          std::forward_iterator ResIt>
+requires model_component_state<MainModelState, ComponentContainer, Component>
+constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
+                              std::vector<MathOutputType> const& math_output, ResIt res_it) {
+    return detail::produce_output<Component, Idx2D>(state, res_it, [&math_output](Source const& source, Idx2D math_id) {
+        if (math_id.group == -1) {
+            return source.get_null_sc_output();
+        }
+        return source.get_sc_output(math_output[math_id.group].source[math_id.pos]);
+    });
+}
 
 // output load gen
-template <std::derived_from<GenericLoadGen> Component, class ComponentContainer, math_output_type MathOutputType,
-          std::forward_iterator ResIt>
+template <std::derived_from<GenericLoadGen> Component, class ComponentContainer,
+          steady_state_math_output_type MathOutputType, std::forward_iterator ResIt>
 requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(
         state, res_it, [&math_output](GenericLoadGen const& load_gen, Idx2D math_id) {
             constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
             if (math_id.group == -1) {
                 return load_gen.get_null_output<sym>();
             }
             return load_gen.get_output<sym>(math_output[math_id.group].load_gen[math_id.pos]);
         });
 }
+template <std::derived_from<GenericLoadGen> Component, class ComponentContainer,
+          short_circuit_math_output_type MathOutputType, std::forward_iterator ResIt>
+requires model_component_state<MainModelState, ComponentContainer, Component>
+constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
+                              std::vector<MathOutputType> const& /* math_output */, ResIt res_it) {
+    return detail::produce_output<Component, Idx2D>(state, res_it,
+                                                    [](GenericLoadGen const& load_gen, Idx2D /* math_id */) {
+                                                        return load_gen.get_null_sc_output();
+                                                    });
+}
 
 // output shunt
-template <std::same_as<Shunt> Component, class ComponentContainer, math_output_type MathOutputType,
+template <std::same_as<Shunt> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
 requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(state, res_it, [&math_output](Shunt const& shunt, Idx2D math_id) {
         constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
         if (math_id.group == -1) {
             return shunt.get_null_output<sym>();
         }
         return shunt.get_output<sym>(math_output[math_id.group].shunt[math_id.pos]);
     });
 }
+template <std::same_as<Shunt> Component, class ComponentContainer, short_circuit_math_output_type MathOutputType,
+          std::forward_iterator ResIt>
+requires model_component_state<MainModelState, ComponentContainer, Component>
+constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
+                              std::vector<MathOutputType> const& math_output, ResIt res_it) {
+    return detail::produce_output<Component, Idx2D>(state, res_it, [&math_output](Shunt const& shunt, Idx2D math_id) {
+        if (math_id.group == -1) {
+            return shunt.get_null_sc_output();
+        }
+        return shunt.get_sc_output(math_output[math_id.group].shunt[math_id.pos]);
+    });
+}
 
 // output voltage sensor
-template <std::derived_from<GenericVoltageSensor> Component, class ComponentContainer, math_output_type MathOutputType,
-          std::forward_iterator ResIt>
+template <std::derived_from<GenericVoltageSensor> Component, class ComponentContainer,
+          steady_state_math_output_type MathOutputType, std::forward_iterator ResIt>
 requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx>(
         state, res_it, [&state, &math_output](GenericVoltageSensor const& voltage_sensor, Idx const node_seq) {
             constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
             Idx2D const node_math_id = state.topo_comp_coup->node[node_seq];
             if (node_math_id.group == -1) {
                 return voltage_sensor.get_null_output<sym>();
             }
             return voltage_sensor.get_output<sym>(math_output[node_math_id.group].u[node_math_id.pos]);
         });
 }
+template <std::derived_from<GenericVoltageSensor> Component, class ComponentContainer,
+          short_circuit_math_output_type MathOutputType, std::forward_iterator ResIt>
+requires model_component_state<MainModelState, ComponentContainer, Component>
+constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
+                              std::vector<MathOutputType> const& /* math_output */, ResIt res_it) {
+    return detail::produce_output<Component, Idx>(
+        state, res_it, [](GenericVoltageSensor const& voltage_sensor, Idx const /* node_seq */) {
+            return voltage_sensor.get_null_sc_output();
+        });
+}
 
 // output power sensor
-template <std::derived_from<GenericPowerSensor> Component, class ComponentContainer, math_output_type MathOutputType,
-          std::forward_iterator ResIt>
+template <std::derived_from<GenericPowerSensor> Component, class ComponentContainer,
+          steady_state_math_output_type MathOutputType, std::forward_iterator ResIt>
 requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx>(
         state, res_it, [&state, &math_output](GenericPowerSensor const& power_sensor, Idx const obj_seq) {
             constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
@@ -293,22 +376,48 @@
                     return power_sensor.get_output<sym>(math_output[obj_math_id.group].bus_injection[obj_math_id.pos]);
                 default:
                     throw MissingCaseForEnumError(std::string(GenericPowerSensor::name) + " output_result()",
                                                   terminal_type);
             }
         });
 }
+template <std::derived_from<GenericPowerSensor> Component, class ComponentContainer,
+          short_circuit_math_output_type MathOutputType, std::forward_iterator ResIt>
+requires model_component_state<MainModelState, ComponentContainer, Component>
+constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
+                              std::vector<MathOutputType> const& /* math_output */, ResIt res_it) {
+    return detail::produce_output<Component, Idx>(state, res_it,
+                                                  [](GenericPowerSensor const& power_sensor, Idx const /* node_seq */) {
+                                                      return power_sensor.get_null_sc_output();
+                                                  });
+}
 
 // output fault
-template <std::same_as<Fault> Component, class ComponentContainer, math_output_type MathOutputType,
+template <std::same_as<Fault> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
 requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& /* math_output */, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(state, res_it, [](Fault const& fault, Idx2D /* math_id */) {
         return fault.get_output();
     });
 }
+template <std::same_as<Fault> Component, class ComponentContainer, short_circuit_math_output_type MathOutputType,
+          std::forward_iterator ResIt>
+requires model_component_state<MainModelState, ComponentContainer, Component> &&
+    model_component_state<MainModelState, ComponentContainer, Node>
+constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
+                              std::vector<MathOutputType> const& math_output, ResIt res_it) {
+    return detail::produce_output<Component, Idx2D>(
+        state, res_it, [&state, &math_output](Fault const& fault, Idx2D math_id) {
+            if (math_id.group == -1) {
+                return fault.get_null_sc_output();
+            }
+
+            auto const u_rated = state.components.template get_item<Node>(fault.get_fault_object()).u_rated();
+            return fault.get_sc_output(math_output[math_id.group].fault[math_id.pos], u_rated);
+        });
+}
 
 }  // namespace power_grid_model::main_core
 
 #endif
```

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -14,26 +14,31 @@
 namespace power_grid_model::main_core {
 
 template <class CompContainer>
 struct MainModelState {
     using ComponentContainer = CompContainer;
 
     ComponentContainer components;
+
     // calculation parameters
     std::shared_ptr<ComponentTopology const> comp_topo;
-    std::shared_ptr<ComponentToMathCoupling> comp_coup;
+
+    std::vector<std::shared_ptr<MathModelTopology const>> math_topology;
     std::shared_ptr<TopologicalComponentToMathCoupling const> topo_comp_coup;
+
+    ComponentToMathCoupling comp_coup;
 };
 
 template <typename ContainerType, typename ComponentType>
-concept component_container = requires(ContainerType const& c) {
+concept component_container = requires(ContainerType const& c, ID id) {
     { c.template citer<ComponentType>().begin() } -> std::forward_iterator;
     { c.template citer<ComponentType>().end() } -> std::forward_iterator;
     { *(c.template citer<ComponentType>().begin()) } -> std::same_as<ComponentType const&>;
     { *(c.template citer<ComponentType>().end()) } -> std::same_as<ComponentType const&>;
+    { c.template get_item<ComponentType>(id) } -> std::convertible_to<ComponentType const&>;
 };
 
 template <template <typename T> class StateType, typename ContainerType, typename ComponentType>
 concept model_component_state =
     component_container<typename StateType<ContainerType>::ComponentContainer, ComponentType> &&
     std::same_as<StateType<ContainerType>, MainModelState<ContainerType>>;
```

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -310,17 +310,17 @@
         assert(construction_complete_);
         is_topology_up_to_date_ = false;
         is_sym_parameter_up_to_date_ = false;
         is_asym_parameter_up_to_date_ = false;
         n_math_solvers_ = 0;
         sym_solvers_.clear();
         asym_solvers_.clear();
-        math_topology_.clear();
-        state_.comp_coup.reset();
+        state_.math_topology.clear();
         state_.topo_comp_coup.reset();
+        state_.comp_coup = {};
     }
 
     /*
     the the sequence indexer given an input array of ID's for a given component type
     */
     void get_indexer(std::string const& component_type, ID const* id_begin, Idx size, Idx* indexer_begin) const {
         // static function array
@@ -343,60 +343,73 @@
         // if topology changed, everything is not up to date
         // if only param changed, set param to not up to date
         is_topology_up_to_date_ = is_topology_up_to_date_ && !changes.topo;
         is_sym_parameter_up_to_date_ = is_sym_parameter_up_to_date_ && !changes.topo && !changes.param;
         is_asym_parameter_up_to_date_ = is_asym_parameter_up_to_date_ && !changes.topo && !changes.param;
     }
 
-    template <bool sym, typename InputType, typename PrepareInputFn, typename SolveFn>
-    requires std::invocable<std::remove_cvref_t<PrepareInputFn>> && std::invocable < std::remove_cvref_t<SolveFn>,
-        MathSolver<sym>
-    &, InputType const& >
-           &&std::same_as<std::invoke_result_t<PrepareInputFn>, std::vector<InputType>>&&
-               std::same_as<std::invoke_result_t<SolveFn, MathSolver<sym>&, InputType const&>, MathOutput<sym>>
-                   std::vector<MathOutput<sym>> calculate_(PrepareInputFn&& prepare_input, SolveFn&& solve) {
+    template <math_output_type MathOutputType, typename MathSolverType, typename InputType, typename PrepareInputFn,
+              typename SolveFn>
+    requires std::invocable<std::remove_cvref_t<PrepareInputFn>> &&
+        std::invocable<std::remove_cvref_t<SolveFn>, MathSolverType&, InputType const&>&&
+            std::same_as<std::invoke_result_t<PrepareInputFn>, std::vector<InputType>>&&
+                std::same_as<std::invoke_result_t<SolveFn, MathSolverType&, InputType const&>, MathOutputType>
+                    std::vector<MathOutputType> calculate_(PrepareInputFn&& prepare_input, SolveFn&& solve) {
+        constexpr bool sym = symmetric_math_output_type<MathOutputType>;
+
         assert(construction_complete_);
         calculation_info_ = CalculationInfo{};
         // prepare
         Timer timer(calculation_info_, 2100, "Prepare");
         prepare_solvers<sym>();
         auto const& input = prepare_input();
         // calculate
         timer = Timer(calculation_info_, 2200, "Math Calculation");
         std::vector<MathSolver<sym>>& solvers = get_solvers<sym>();
-        std::vector<MathOutput<sym>> math_output(n_math_solvers_);
+        std::vector<MathOutputType> math_output(n_math_solvers_);
         std::transform(solvers.begin(), solvers.end(), input.cbegin(), math_output.begin(), solve);
         return math_output;
     }
 
     template <bool sym>
     std::vector<MathOutput<sym>> calculate_power_flow_(double err_tol, Idx max_iter,
                                                        CalculationMethod calculation_method) {
-        return calculate_<sym, PowerFlowInput<sym>>(
+        return calculate_<MathOutput<sym>, MathSolver<sym>, PowerFlowInput<sym>>(
             [this] {
                 return prepare_power_flow_input<sym>();
             },
-            [this, err_tol, max_iter, &calculation_method](MathSolver<sym>& solver, PowerFlowInput<sym> const& y) {
+            [this, err_tol, max_iter, calculation_method](MathSolver<sym>& solver, PowerFlowInput<sym> const& y) {
                 return solver.run_power_flow(y, err_tol, max_iter, calculation_info_, calculation_method);
             });
     }
 
     template <bool sym>
     std::vector<MathOutput<sym>> calculate_state_estimation_(double err_tol, Idx max_iter,
                                                              CalculationMethod calculation_method) {
-        return calculate_<sym, StateEstimationInput<sym>>(
+        return calculate_<MathOutput<sym>, MathSolver<sym>, StateEstimationInput<sym>>(
             [this] {
                 return prepare_state_estimation_input<sym>();
             },
-            [this, err_tol, max_iter, &calculation_method](MathSolver<sym>& solver,
-                                                           StateEstimationInput<sym> const& y) {
+            [this, err_tol, max_iter, calculation_method](MathSolver<sym>& solver, StateEstimationInput<sym> const& y) {
                 return solver.run_state_estimation(y, err_tol, max_iter, calculation_info_, calculation_method);
             });
     }
 
+    template <bool sym>
+    std::vector<ShortCircuitMathOutput<sym>> calculate_short_circuit_(double voltage_scaling_factor_c,
+                                                                      CalculationMethod calculation_method) {
+        return calculate_<ShortCircuitMathOutput<sym>, MathSolver<sym>, ShortCircuitInput>(
+            [this] {
+                return prepare_short_circuit_input<sym>();
+            },
+            [this, voltage_scaling_factor_c, calculation_method](MathSolver<sym>& solver, ShortCircuitInput const& y) {
+                return solver.run_short_circuit(y, voltage_scaling_factor_c, calculation_info_, calculation_method);
+            });
+    }
+
     // get sequence idx map for fast caching of component sequences
     // only applicable for independent update dataset
     std::map<std::string, std::vector<Idx2D>> get_sequence_idx_map(ConstDataset const& update_data) const {
         // function pointer array to get cached idx
         static constexpr std::array<GetSeqIdxFunc, n_types> get_seq_idx{
             [](MainModelImpl const& model, ConstDataPointer const& component_update) -> std::vector<Idx2D> {
                 using UpdateType = typename ComponentType::UpdateType;
@@ -425,32 +438,36 @@
             // add
             sequence_idx_map[entry.name] = get_seq_idx[entry.index](*this, found->second);
         }
         return sequence_idx_map;
     }
 
     /*
-    calculate power flow or state estimation in batch
-    provide update data
+    run the calculation function in batch on the provided update data.
+    The calculation function (required) should be able to run standalone.
+    The preparation function (optional) may be provided to allow speeding up calculations.
     threading
         < 0 sequential
         = 0 parallel, use number of hardware threads
         > 0 specify number of parallel threads
     raise a BatchCalculationError if any of the calculations in the batch raised an exception
     */
-    template <bool sym, std::vector<MathOutput<sym>> (MainModelImpl::*calculation_fn)(double, Idx, CalculationMethod)>
-    BatchParameter batch_calculation_(double err_tol, Idx max_iter, CalculationMethod calculation_method,
-                                      Dataset const& result_data, ConstDataset const& update_data, Idx threading = -1) {
+    template <typename Calculate, typename Prepare>
+    requires std::invocable<std::remove_cvref_t<Calculate>, MainModelImpl&>&&
+        std::invocable<std::remove_cvref_t<Prepare>, MainModelImpl&>
+            BatchParameter batch_calculation_(Calculate&& calculation_fn, Prepare&& preparation_fn,
+                                              Dataset const& result_data, ConstDataset const& update_data,
+                                              Idx threading = -1) {
         // if the update batch is one empty map without any component
         // execute one power flow in the current instance, no batch calculation is needed
         // NOTE: if the map is not empty but the datasets inside are empty
         //     that will be considered as a zero batch_size
         bool const all_empty = update_data.empty();
         if (all_empty) {
-            auto const math_output = (this->*calculation_fn)(err_tol, max_iter, calculation_method);
+            auto const math_output = calculation_fn(*this);
             output_result(math_output, result_data);
             return BatchParameter{};
         }
 
         // get number of batches (can't be empty, because then all_empty would have been true)
         Idx const n_batch = update_data.cbegin()->second.batch_size();
         // assert if all component types have the same number of batches
@@ -462,15 +479,15 @@
         // we consider in this case the batch set is independent and but not topology cachable
         if (n_batch == 0) {
             return BatchParameter{};
         }
 
         // calculate once to cache topology, ignore results, all math solvers are initialized
         try {
-            (this->*calculation_fn)(std::numeric_limits<double>::infinity(), 1, calculation_method);
+            preparation_fn(*this);
         }
         catch (const SparseMatrixError&) {
             // missing entries are provided in the update data
         }
 
         // const ref of current instance
         MainModelImpl const& base_model = *this;
@@ -480,23 +497,23 @@
             MainModelImpl::is_update_independent(update_data) ? get_sequence_idx_map(update_data)
                                                               : std::map<std::string, std::vector<Idx2D>>{};
 
         // error messages
         std::vector<std::string> exceptions(n_batch, "");
 
         // lambda for sub batch calculation
-        auto sub_batch = [&base_model, &exceptions, &result_data, &update_data, &sequence_idx_map, n_batch, err_tol,
-                          max_iter, calculation_method](Idx start, Idx stride) {
+        auto sub_batch = [&base_model, &exceptions, &calculation_fn, &result_data, &update_data, &sequence_idx_map,
+                          n_batch](Idx start, Idx stride) {
             // copy base model
             MainModelImpl model{base_model};
             for (Idx batch_number = start; batch_number < n_batch; batch_number += stride) {
                 // try to update model and run calculation
                 try {
                     model.update_component<cached_update_t>(update_data, batch_number, sequence_idx_map);
-                    auto const math_output = (model.*calculation_fn)(err_tol, max_iter, calculation_method);
+                    auto const math_output = calculation_fn(model);
                     model.output_result(math_output, result_data, batch_number);
                     model.restore_components();
                 }
                 catch (std::exception const& ex) {
                     exceptions[batch_number] = ex.what();
                 }
                 catch (...) {
@@ -543,14 +560,23 @@
         }
         if (!combined_error_message.empty()) {
             throw BatchCalculationError(combined_error_message, failed_scenarios, err_msgs);
         }
 
         return BatchParameter{};
     }
+    template <typename Calculate>
+    requires std::invocable<std::remove_cvref_t<Calculate>, MainModelImpl&> BatchParameter batch_calculation_(
+        Calculate&& calculation_fn, Dataset const& result_data, ConstDataset const& update_data, Idx threading = -1) {
+        return batch_calculation_(
+            calculation_fn,
+            [](MainModelImpl& /* model */) {  // nothing to prepare
+            },
+            result_data, update_data, threading);
+    }
 
    public:
     template <class Component>
     using UpdateType = typename Component::UpdateType;
 
     static bool is_update_independent(ConstDataset const& update_data) {
         // check all components
@@ -615,16 +641,22 @@
     }
 
     // Batch load flow calculation, propagating the results to result_data
     template <bool sym>
     BatchParameter calculate_power_flow(double err_tol, Idx max_iter, CalculationMethod calculation_method,
                                         Dataset const& result_data, ConstDataset const& update_data,
                                         Idx threading = -1) {
-        return batch_calculation_<sym, &MainModelImpl::calculate_power_flow_<sym>>(
-            err_tol, max_iter, calculation_method, result_data, update_data, threading);
+        return batch_calculation_(
+            [err_tol, max_iter, calculation_method](MainModelImpl& model) {
+                return model.calculate_power_flow_<sym>(err_tol, max_iter, calculation_method);
+            },
+            [calculation_method](MainModelImpl& model) {
+                model.calculate_power_flow_<sym>(std::numeric_limits<double>::max(), 1, calculation_method);
+            },
+            result_data, update_data, threading);
     }
 
     // Single state estimation calculation, returning math output results
     template <bool sym>
     std::vector<MathOutput<sym>> calculate_state_estimation(double err_tol, Idx max_iter,
                                                             CalculationMethod calculation_method) {
         return calculate_state_estimation_<sym>(err_tol, max_iter, calculation_method);
@@ -640,16 +672,57 @@
     }
 
     // Batch state estimation calculation, propagating the results to result_data
     template <bool sym>
     BatchParameter calculate_state_estimation(double err_tol, Idx max_iter, CalculationMethod calculation_method,
                                               Dataset const& result_data, ConstDataset const& update_data,
                                               Idx threading = -1) {
-        return batch_calculation_<sym, &MainModelImpl::calculate_state_estimation_<sym>>(
-            err_tol, max_iter, calculation_method, result_data, update_data, threading);
+        return batch_calculation_(
+            [err_tol, max_iter, calculation_method](MainModelImpl& model) {
+                return model.calculate_state_estimation_<sym>(err_tol, max_iter, calculation_method);
+            },
+            [calculation_method](MainModelImpl& model) {
+                model.calculate_state_estimation_<sym>(std::numeric_limits<double>::max(), 1, calculation_method);
+            },
+            result_data, update_data, threading);
+    }
+
+    // Single short circuit calculation, returning short circuit math output results
+    template <bool sym>
+    std::vector<ShortCircuitMathOutput<sym>> calculate_short_circuit(double voltage_scaling_factor_c,
+                                                                     CalculationMethod calculation_method) {
+        return calculate_short_circuit_<sym>(voltage_scaling_factor_c, calculation_method);
+    }
+
+    // Single short circuit calculation, propagating the results to result_data
+    void calculate_short_circuit(double voltage_scaling_factor_c, CalculationMethod calculation_method,
+                                 Dataset const& result_data, Idx pos = 0) {
+        assert(construction_complete_);
+        if (std::all_of(state_.components.template citer<Fault>().begin(),
+                        state_.components.template citer<Fault>().end(), [](Fault const& fault) {
+                            return fault.get_fault_type() == FaultType::three_phase;
+                        })) {
+            auto const math_output = calculate_short_circuit_<true>(voltage_scaling_factor_c, calculation_method);
+            output_result<true>(math_output, result_data, pos);
+        }
+        else {
+            auto const math_output = calculate_short_circuit_<false>(voltage_scaling_factor_c, calculation_method);
+            output_result<false>(math_output, result_data, pos);
+        }
+    }
+
+    // Batch short circuit calculation, propagating the results to result_data
+    BatchParameter calculate_short_circuit(double voltage_scaling_factor_c, CalculationMethod calculation_method,
+                                           Dataset const& result_data, ConstDataset const& update_data,
+                                           Idx threading = -1) {
+        return batch_calculation_(
+            [voltage_scaling_factor_c, calculation_method](MainModelImpl& model) {
+                return model.calculate_short_circuit_<false>(voltage_scaling_factor_c, calculation_method);
+            },
+            result_data, update_data, threading);
     }
 
     template <typename Component, math_output_type MathOutputType, std::forward_iterator ResIt>
     ResIt output_result(std::vector<MathOutputType> const& math_output, ResIt res_it) {
         assert(construction_complete_);
         return main_core::output_result<Component, ComponentContainer>(state_, math_output, res_it);
     }
@@ -694,15 +767,14 @@
     }
 
    private:
     double system_frequency_;
 
     MainModelState state_;
     // math model
-    std::vector<std::shared_ptr<MathModelTopology const>> math_topology_;
     std::vector<MathSolver<true>> sym_solvers_;
     std::vector<MathSolver<false>> asym_solvers_;
     Idx n_math_solvers_{0};
     bool is_topology_up_to_date_{false};
     bool is_sym_parameter_up_to_date_{false};
     bool is_asym_parameter_up_to_date_{false};
     UpdateChange cached_state_changes_{};
@@ -767,28 +839,28 @@
         std::transform(state_.components.template citer<Source>().begin(),
                        state_.components.template citer<Source>().end(), comp_conn.source_connected.begin(),
                        [](Source const& source) {
                            return source.status();
                        });
         // re build
         Topology topology{*state_.comp_topo, comp_conn};
-        std::tie(math_topology_, state_.topo_comp_coup) = topology.build_topology();
-        n_math_solvers_ = (Idx)math_topology_.size();
+        std::tie(state_.math_topology, state_.topo_comp_coup) = topology.build_topology();
+        n_math_solvers_ = static_cast<Idx>(state_.math_topology.size());
         is_topology_up_to_date_ = true;
         is_sym_parameter_up_to_date_ = false;
         is_asym_parameter_up_to_date_ = false;
     }
 
     template <bool sym>
     std::vector<MathModelParam<sym>> get_math_param() {
         std::vector<MathModelParam<sym>> math_param(n_math_solvers_);
         for (Idx i = 0; i != n_math_solvers_; ++i) {
-            math_param[i].branch_param.resize(math_topology_[i]->n_branch());
-            math_param[i].shunt_param.resize(math_topology_[i]->n_shunt());
-            math_param[i].source_param.resize(math_topology_[i]->n_source());
+            math_param[i].branch_param.resize(state_.math_topology[i]->n_branch());
+            math_param[i].shunt_param.resize(state_.math_topology[i]->n_shunt());
+            math_param[i].source_param.resize(state_.math_topology[i]->n_source());
         }
         // loop all branch
         for (Idx i = 0; i != (Idx)state_.comp_topo->branch_node_idx.size(); ++i) {
             Idx2D const math_idx = state_.topo_comp_coup->branch[i];
             if (math_idx.group == -1) {
                 continue;
             }
@@ -885,31 +957,65 @@
      *
      * @param include
      *      A lambda function (Idx i -> bool) which returns true if the component at Idx i should be included.
      * 	    The default lambda `include_all` always returns `true`.
      */
     template <bool sym, class CalcStructOut, typename CalcParamOut,
               std::vector<CalcParamOut>(CalcStructOut::*comp_vect), class ComponentIn,
-              typename PredicateIn = decltype(include_all)>
-    void prepare_input(std::vector<Idx2D> const& components, std::vector<CalcStructOut>& calc_input,
-                       PredicateIn include = include_all) {
+              std::invocable<Idx> PredicateIn = decltype(include_all)>
+    requires std::convertible_to < std::invoke_result_t<PredicateIn, Idx>,
+    bool > void prepare_input(std::vector<Idx2D> const& components, std::vector<CalcStructOut>& calc_input,
+                              PredicateIn include = include_all) {
+        for (Idx i = 0, n = (Idx)components.size(); i != n; ++i) {
+            if (include(i)) {
+                Idx2D const math_idx = components[i];
+                if (math_idx.group != -1) {
+                    auto const& component = state_.components.template get_item_by_seq<ComponentIn>(i);
+                    CalcParamOut const calc_param = calculate_param<sym>(component);
+                    CalcStructOut& math_model_input = calc_input[math_idx.group];
+                    std::vector<CalcParamOut>& math_model_input_vect = math_model_input.*comp_vect;
+                    math_model_input_vect[math_idx.pos] = calc_param;
+                }
+            }
+        }
+    }
+
+    template <bool sym, class CalcStructOut, typename CalcParamOut,
+              std::vector<CalcParamOut>(CalcStructOut::*comp_vect), class ComponentIn,
+              std::invocable<Idx> PredicateIn = decltype(include_all)>
+    requires std::convertible_to < std::invoke_result_t<PredicateIn, Idx>,
+    bool > void prepare_input(std::vector<Idx2D> const& components, std::vector<CalcStructOut>& calc_input,
+                              std::invocable<ComponentIn const&> auto extra_args, PredicateIn include = include_all) {
         for (Idx i = 0, n = (Idx)components.size(); i != n; ++i) {
             if (include(i)) {
                 Idx2D const math_idx = components[i];
                 if (math_idx.group != -1) {
-                    CalcParamOut const calc_param =
-                        state_.components.template get_item_by_seq<ComponentIn>(i).template calc_param<sym>();
+                    auto const& component = state_.components.template get_item_by_seq<ComponentIn>(i);
+                    CalcParamOut const calc_param = calculate_param<sym>(component, extra_args(component));
                     CalcStructOut& math_model_input = calc_input[math_idx.group];
                     std::vector<CalcParamOut>& math_model_input_vect = math_model_input.*comp_vect;
                     math_model_input_vect[math_idx.pos] = calc_param;
                 }
             }
         }
     }
 
+    template <bool sym>
+    auto calculate_param(auto const& c, auto const&... extra_args) {
+        if constexpr (requires { {c.calc_param(extra_args...)}; }) {
+            return c.calc_param(extra_args...);
+        }
+        else if constexpr (requires { {c.template calc_param<sym>(extra_args...)}; }) {
+            return c.template calc_param<sym>(extra_args...);
+        }
+        else {
+            return;
+        }
+    }
+
     template <bool sym, IntSVector(StateEstimationInput<sym>::*component), class Component>
     void prepare_input_status(std::vector<Idx2D> const& objects, std::vector<StateEstimationInput<sym>>& input) {
         for (Idx i = 0, n = (Idx)objects.size(); i != n; ++i) {
             Idx2D const math_idx = objects[i];
             if (math_idx.group == -1) {
                 continue;
             }
@@ -919,16 +1025,16 @@
     }
 
     template <bool sym>
     std::vector<PowerFlowInput<sym>> prepare_power_flow_input() {
         assert(is_topology_up_to_date_ && is_parameter_up_to_date<sym>());
         std::vector<PowerFlowInput<sym>> pf_input(n_math_solvers_);
         for (Idx i = 0; i != n_math_solvers_; ++i) {
-            pf_input[i].s_injection.resize(math_topology_[i]->n_load_gen());
-            pf_input[i].source.resize(math_topology_[i]->n_source());
+            pf_input[i].s_injection.resize(state_.math_topology[i]->n_load_gen());
+            pf_input[i].source.resize(state_.math_topology[i]->n_source());
         }
         prepare_input<sym, PowerFlowInput<sym>, DoubleComplex, &PowerFlowInput<sym>::source, Source>(
             state_.topo_comp_coup->source, pf_input);
 
         prepare_input<sym, PowerFlowInput<sym>, ComplexValue<sym>, &PowerFlowInput<sym>::s_injection, GenericLoadGen>(
             state_.topo_comp_coup->load_gen, pf_input);
 
@@ -938,24 +1044,24 @@
     template <bool sym>
     std::vector<StateEstimationInput<sym>> prepare_state_estimation_input() {
         assert(is_topology_up_to_date_ && is_parameter_up_to_date<sym>());
 
         std::vector<StateEstimationInput<sym>> se_input(n_math_solvers_);
 
         for (Idx i = 0; i != n_math_solvers_; ++i) {
-            se_input[i].shunt_status.resize(math_topology_[i]->n_shunt());
-            se_input[i].load_gen_status.resize(math_topology_[i]->n_load_gen());
-            se_input[i].source_status.resize(math_topology_[i]->n_source());
-            se_input[i].measured_voltage.resize(math_topology_[i]->n_voltage_sensor());
-            se_input[i].measured_source_power.resize(math_topology_[i]->n_source_power_sensor());
-            se_input[i].measured_load_gen_power.resize(math_topology_[i]->n_load_gen_power_sensor());
-            se_input[i].measured_shunt_power.resize(math_topology_[i]->n_shunt_power_power_sensor());
-            se_input[i].measured_branch_from_power.resize(math_topology_[i]->n_branch_from_power_sensor());
-            se_input[i].measured_branch_to_power.resize(math_topology_[i]->n_branch_to_power_sensor());
-            se_input[i].measured_bus_injection.resize(math_topology_[i]->n_bus_power_sensor());
+            se_input[i].shunt_status.resize(state_.math_topology[i]->n_shunt());
+            se_input[i].load_gen_status.resize(state_.math_topology[i]->n_load_gen());
+            se_input[i].source_status.resize(state_.math_topology[i]->n_source());
+            se_input[i].measured_voltage.resize(state_.math_topology[i]->n_voltage_sensor());
+            se_input[i].measured_source_power.resize(state_.math_topology[i]->n_source_power_sensor());
+            se_input[i].measured_load_gen_power.resize(state_.math_topology[i]->n_load_gen_power_sensor());
+            se_input[i].measured_shunt_power.resize(state_.math_topology[i]->n_shunt_power_power_sensor());
+            se_input[i].measured_branch_from_power.resize(state_.math_topology[i]->n_branch_from_power_sensor());
+            se_input[i].measured_branch_to_power.resize(state_.math_topology[i]->n_branch_to_power_sensor());
+            se_input[i].measured_bus_injection.resize(state_.math_topology[i]->n_bus_power_sensor());
         }
 
         prepare_input_status<sym, &StateEstimationInput<sym>::shunt_status, Shunt>(state_.topo_comp_coup->shunt,
                                                                                    se_input);
         prepare_input_status<sym, &StateEstimationInput<sym>::load_gen_status, GenericLoadGen>(
             state_.topo_comp_coup->load_gen, se_input);
         prepare_input_status<sym, &StateEstimationInput<sym>::source_status, Source>(state_.topo_comp_coup->source,
@@ -1000,14 +1106,61 @@
                 return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::node;
             });
 
         return se_input;
     }
 
     template <bool sym>
+    std::vector<ShortCircuitInput> prepare_short_circuit_input() {
+        assert(is_topology_up_to_date_ && is_parameter_up_to_date<sym>());
+
+        std::vector<IdxVector> topo_fault_indices(state_.math_topology.size());
+        std::vector<IdxVector> topo_bus_indices(state_.math_topology.size());
+
+        for (Idx fault_idx{0}; fault_idx < state_.components.template size<Fault>(); ++fault_idx) {
+            auto const& fault = state_.components.template get_item_by_seq<Fault>(fault_idx);
+            if (fault.status()) {
+                auto const node_idx = state_.components.template get_seq<Node>(fault.get_fault_object());
+                auto const topo_bus_idx = state_.topo_comp_coup->node[node_idx];
+
+                if (topo_bus_idx.group >= 0) {  // Consider non-isolated objects only
+                    topo_fault_indices[topo_bus_idx.group].push_back(fault_idx);
+                    topo_bus_indices[topo_bus_idx.group].push_back(topo_bus_idx.pos);
+                }
+            }
+        }
+
+        auto fault_coup = std::vector<Idx2D>(state_.components.template size<Fault>(), Idx2D{-1, -1});
+
+        std::vector<ShortCircuitInput> sc_input(n_math_solvers_);
+        for (Idx i = 0; i != n_math_solvers_; ++i) {
+            auto map = build_sparse_mapping(topo_bus_indices[i], state_.math_topology[i]->n_bus());
+
+            for (Idx reordered_idx{0}; reordered_idx < static_cast<Idx>(map.reorder.size()); ++reordered_idx) {
+                fault_coup[topo_fault_indices[i][map.reorder[reordered_idx]]] = Idx2D{i, reordered_idx};
+            }
+
+            sc_input[i].fault_bus_indptr = std::move(map.indptr);
+            sc_input[i].faults.resize(state_.components.template size<Fault>());
+            sc_input[i].source.resize(state_.math_topology[i]->n_source());
+        }
+
+        state_.comp_coup = ComponentToMathCoupling{.fault = std::move(fault_coup)};
+
+        prepare_input<sym, ShortCircuitInput, FaultCalcParam, &ShortCircuitInput::faults, Fault>(
+            state_.comp_coup.fault, sc_input, [this](Fault const& fault) {
+                return state_.components.template get_item<Node>(fault.get_fault_object()).u_rated();
+            });
+        prepare_input<sym, ShortCircuitInput, DoubleComplex, &ShortCircuitInput::source, Source>(
+            state_.topo_comp_coup->source, sc_input);
+
+        return sc_input;
+    }
+
+    template <bool sym>
     void prepare_solvers() {
         std::vector<MathSolver<sym>>& solvers = get_solvers<sym>();
         // also get the vector of other solvers (sym -> asym, or asym -> sym)
         std::vector<MathSolver<!sym>>& other_solvers = get_solvers<!sym>();
         // rebuild topology if needed
         if (!is_topology_up_to_date_) {
             rebuild_topology();
@@ -1020,21 +1173,21 @@
             solvers.reserve(n_math_solvers_);
             // get param, will be consumed
             std::vector<MathModelParam<sym>> math_params = get_math_param<sym>();
             // loop to build
             for (Idx i = 0; i != n_math_solvers_; ++i) {
                 // if other solver exists, construct from existing y bus struct
                 if (other_solver_exist) {
-                    solvers.emplace_back(math_topology_[i],
+                    solvers.emplace_back(state_.math_topology[i],
                                          std::make_shared<MathModelParam<sym> const>(std::move(math_params[i])),
                                          other_solvers[i].shared_y_bus_struct());
                 }
                 // else construct from scratch
                 else {
-                    solvers.emplace_back(math_topology_[i],
+                    solvers.emplace_back(state_.math_topology[i],
                                          std::make_shared<MathModelParam<sym> const>(std::move(math_params[i])));
                 }
             }
         }
         // if parameters are not up to date, update them
         else if (!is_parameter_up_to_date<sym>()) {
             // get param, will be consumed
```

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -73,30 +73,30 @@
         }
 
         // call calculation
         return iterative_linear_se_solver_.value().run_state_estimation(y_bus_, input, err_tol, max_iter,
                                                                         calculation_info);
     }
 
-    ShortCircuitMathOutput<sym> run_short_circuit(ShortCircuitInput const& input, double source_voltage_ref,
+    ShortCircuitMathOutput<sym> run_short_circuit(ShortCircuitInput const& input, double voltage_scaling_factor_c,
                                                   CalculationInfo& calculation_info,
                                                   CalculationMethod calculation_method) {
         if (calculation_method != CalculationMethod::default_method &&
             calculation_method != CalculationMethod::iec60909) {
             throw InvalidCalculationMethod{};
         }
 
         // construct model if needed
         if (!iec60909_sc_solver_.has_value()) {
             Timer const timer(calculation_info, 2210, "Create math solver");
             iec60909_sc_solver_.emplace(y_bus_, topo_ptr_);
         }
 
         // call calculation
-        return iec60909_sc_solver_.value().run_short_circuit(source_voltage_ref, y_bus_, input);
+        return iec60909_sc_solver_.value().run_short_circuit(voltage_scaling_factor_c, y_bus_, input);
     }
 
     void clear_solver() {
         newton_pf_solver_.reset();
         linear_pf_solver_.reset();
         iterative_current_pf_solver_.reset();
         iterative_linear_se_solver_.reset();
```

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
           n_source_{topo_ptr->n_source()},
           source_bus_indptr_{topo_ptr, &topo_ptr->source_bus_indptr},
           mat_data_(y_bus.nnz_lu()),
           sparse_solver_{y_bus.shared_indptr_lu(), y_bus.shared_indices_lu(), y_bus.shared_diag_lu()},
           perm_{static_cast<BlockPermArray>(n_bus_)} {
     }
 
-    ShortCircuitMathOutput<sym> run_short_circuit(double source_voltage_ref, YBus<sym> const& y_bus,
+    ShortCircuitMathOutput<sym> run_short_circuit(double voltage_scaling_factor_c, YBus<sym> const& y_bus,
                                                   ShortCircuitInput const& input) {
         check_input_valid(input);
 
         auto [fault_type, fault_phase] = extract_fault_type_phase(input.faults);
 
         // set phase 1 and 2 index for single and two phase faults
         auto const [phase_1, phase_2] = set_phase_index(fault_phase);
@@ -74,15 +74,15 @@
 
             // add all sources
             for (Idx source_number = source_bus_indptr[bus_number]; source_number != source_bus_indptr[bus_number + 1];
                  ++source_number) {
                 ComplexTensor<sym> const y_source = y_bus.math_model_param().source_param[source_number];
                 diagonal_element += y_source;  // add y_source to the diagonal of Ybus
                 u_bus += dot(y_source, ComplexValue<sym>{input.source[source_number] *
-                                                         source_voltage_ref});  // rhs += Y_source * U_source * c
+                                                         voltage_scaling_factor_c});  // rhs += Y_source * U_source * c
             }
             // skip if no fault
             if (!input.faults.empty()) {
                 // add all faults
                 for (Idx fault_number = fault_bus_indptr[bus_number]; fault_number != fault_bus_indptr[bus_number + 1];
                      ++fault_number) {
                     DoubleComplex const y_fault = input.faults[fault_number].y_fault;
@@ -206,15 +206,15 @@
         }
 
         // solve matrix
         sparse_solver_.prefactorize_and_solve(mat_data_, perm_, output.u_bus, output.u_bus);
 
         // post processing
         calculate_result(y_bus, input, output, infinite_admittance_fault_counter, fault_type, phase_1, phase_2,
-                         source_voltage_ref);
+                         voltage_scaling_factor_c);
 
         return output;
     }
 
    private:
     Idx n_bus_;
     Idx n_fault_;
@@ -225,15 +225,15 @@
     ComplexTensorVector<sym> mat_data_;
     // sparse solver
     SparseLUSolver<ComplexTensor<sym>, ComplexValue<sym>, ComplexValue<sym>> sparse_solver_;
     BlockPermArray perm_;
 
     void calculate_result(YBus<sym> const& y_bus, ShortCircuitInput const& input, ShortCircuitMathOutput<sym>& output,
                           IdxVector const& infinite_admittance_fault_counter, FaultType const fault_type,
-                          int const phase_1, int const phase_2, double const source_voltage_ref) {
+                          int const phase_1, int const phase_2, double const voltage_scaling_factor_c) const {
         // loop through all buses
         for (Idx bus_number = 0; bus_number != n_bus_; ++bus_number) {
             ComplexValue<sym> const x_bus_subtotal = output.u_bus[bus_number];
             double const infinite_admittance_fault_counter_bus =
                 static_cast<double>(infinite_admittance_fault_counter[bus_number]);
 
             if (!input.faults.empty()) {
@@ -307,20 +307,20 @@
                                 continue;
                             }
                         }
                     }
                 }
 
                 ComplexValue<sym> i_source_bus{};     // total source current in to the bus
-                ComplexValue<sym> i_source_inject{};  // total raw source current as a Norton equievalent
+                ComplexValue<sym> i_source_inject{};  // total raw source current as a Norton equivalent
                 for (Idx source_number = (*source_bus_indptr_)[bus_number];
                      source_number != (*source_bus_indptr_)[bus_number + 1]; ++source_number) {
                     ComplexTensor<sym> const y_source = y_bus.math_model_param().source_param[source_number];
                     ComplexValue<sym> const i_source_inject_single =
-                        dot(y_source, ComplexValue<sym>{input.source[source_number] * source_voltage_ref});
+                        dot(y_source, ComplexValue<sym>{input.source[source_number] * voltage_scaling_factor_c});
                     output.source[source_number].i = i_source_inject_single - dot(y_source, output.u_bus[bus_number]);
                     i_source_bus += output.source[source_number].i;
                     i_source_inject += i_source_inject_single;
                 }
 
                 // compensate source current into hard fault
                 // compensate source current into two phase to ground fault with impedance
@@ -471,8 +471,8 @@
 }  // namespace math_model_impl
 
 template <bool sym>
 using ShortCircuitSolver = math_model_impl::ShortCircuitSolver<sym>;
 
 }  // namespace power_grid_model
 
-#endif
+#endif
```

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/CMakeLists.txt` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/buffer.cpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/buffer.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/handle.cpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/handle.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/handle.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/handle.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/meta_data.cpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/meta_data.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/model.cpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/model.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -115,41 +115,47 @@
             // use dense batch
             update_dataset[update_components[i]] =
                 ConstDataPointer(update_data[i], n_scenarios, n_component_elements_per_scenario[i]);
         }
     }
     // call calculation
     try {
+        auto const calculation_method = static_cast<CalculationMethod>(opt->calculation_method);
         switch (opt->calculation_type) {
             case PGM_power_flow:
                 if (opt->symmetric) {
-                    handle->batch_parameter = model->calculate_power_flow<true>(
-                        opt->err_tol, opt->max_iter, (CalculationMethod)opt->calculation_method, output_dataset,
-                        update_dataset, opt->threading);
+                    handle->batch_parameter =
+                        model->calculate_power_flow<true>(opt->err_tol, opt->max_iter, calculation_method,
+                                                          output_dataset, update_dataset, opt->threading);
                 }
                 else {
-                    handle->batch_parameter = model->calculate_power_flow<false>(
-                        opt->err_tol, opt->max_iter, (CalculationMethod)opt->calculation_method, output_dataset,
-                        update_dataset, opt->threading);
+                    handle->batch_parameter =
+                        model->calculate_power_flow<false>(opt->err_tol, opt->max_iter, calculation_method,
+                                                           output_dataset, update_dataset, opt->threading);
                 }
                 break;
             case PGM_state_estimation:
                 if (opt->symmetric) {
-                    handle->batch_parameter = model->calculate_state_estimation<true>(
-                        opt->err_tol, opt->max_iter, (CalculationMethod)opt->calculation_method, output_dataset,
-                        update_dataset, opt->threading);
+                    handle->batch_parameter =
+                        model->calculate_state_estimation<true>(opt->err_tol, opt->max_iter, calculation_method,
+                                                                output_dataset, update_dataset, opt->threading);
                 }
                 else {
-                    handle->batch_parameter = model->calculate_state_estimation<false>(
-                        opt->err_tol, opt->max_iter, (CalculationMethod)opt->calculation_method, output_dataset,
-                        update_dataset, opt->threading);
+                    handle->batch_parameter =
+                        model->calculate_state_estimation<false>(opt->err_tol, opt->max_iter, calculation_method,
+                                                                 output_dataset, update_dataset, opt->threading);
                 }
                 break;
-            case PGM_short_circuit:
-                [[fallthrough]];
+            case PGM_short_circuit: {
+                [[fallthrough]];  // TODO(mgovers) remove
+                // constexpr double voltage_scaling_factor_c{1.1};
+                // handle->batch_parameter = model->calculate_short_circuit(
+                //     voltage_scaling_factor_c, calculation_method, output_dataset, update_dataset, opt->threading);
+                // break;
+            }
             default:
                 throw MissingCaseForEnumError{"CalculationType", opt->calculation_type};
         }
     }
     catch (BatchCalculationError& e) {
         handle->err_code = PGM_batch_error;
         handle->err_msg = e.what();
```

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/options.cpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/options.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/power_grid_model_c/power_grid_model_c/src/options.hpp` & `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/options.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/pyproject.toml` & `power-grid-model-1.5.0rc9232816587778/pyproject.toml`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/setup.py` & `power-grid-model-1.5.0rc9232816587778/setup.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/__init__.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/core/data_handling.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/data_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/core/error_handling.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/core/options.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/options.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/core/power_grid_core.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/power_grid_core.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/core/power_grid_meta.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/power_grid_meta.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/core/power_grid_model.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/data_types.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/data_types.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/enum.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/enum.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/utils.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/validation/__init__.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/validation/assertions.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/validation/errors.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/validation/rules.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/validation/utils.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model/validation/validation.py` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model.egg-info/PKG-INFO` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9231316741137
+Version: 1.5.0rc9232816587778
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9231316741137/src/power_grid_model.egg-info/SOURCES.txt` & `power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/1os2msr/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-batch-newton/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-i-n-optional/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/gaia-example/asym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/gaia-example/gaia_grid.gnf` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/gaia_grid.gnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/gaia-example/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/multi-source-with-angle/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/line/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/line/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/node/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/node/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/source/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/source/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/line/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/line/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/node/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/source/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/r-state-estimation/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/r-state-estimation/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/three-winding-transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/three-winding-transformer/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/three-winding-transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/three-winding-transformer/update_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-example/asym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-example/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-example/vision_grid.vnf` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/vision_grid.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-validation-network/asym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-validation-network/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-validation-network/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf` & `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/single_phase_to_ground/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/single_phase_to_ground/update_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/three_phase/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/three_phase/sc_output_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/three_phase/update_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase/sc_output_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase/update_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase_to_ground/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/short_circuit/two_phase_to_ground/update_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr-no-angle/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/1os2msr-no-angle/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/distribution-case/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/distribution-case/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/dummy-test-sym/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/dummy-test-sym/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/single-line-load/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/single-line-load/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/three_winding_transformer/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/transmission-case/README.md` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/transmission-case/input.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/data/state_estimation/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/unit/test_0Z_model_validation.py` & `power-grid-model-1.5.0rc9232816587778/tests/unit/test_0Z_model_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/unit/test_error_handling.py` & `power-grid-model-1.5.0rc9232816587778/tests/unit/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/unit/test_meta_data.py` & `power-grid-model-1.5.0rc9232816587778/tests/unit/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/unit/test_power_grid_model.py` & `power-grid-model-1.5.0rc9232816587778/tests/unit/test_power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/unit/test_utils.py` & `power-grid-model-1.5.0rc9232816587778/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/unit/utils.py` & `power-grid-model-1.5.0rc9232816587778/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/unit/validation/test_assertions.py` & `power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/unit/validation/test_batch_validation.py` & `power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_batch_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/unit/validation/test_errors.py` & `power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/unit/validation/test_input_validation.py` & `power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_input_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/unit/validation/test_rules.py` & `power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/unit/validation/test_utils.py` & `power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9231316741137/tests/unit/validation/test_validation_functions.py` & `power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_validation_functions.py`

 * *Files identical despite different names*

