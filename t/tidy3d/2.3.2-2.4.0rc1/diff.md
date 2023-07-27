# Comparing `tmp/tidy3d-2.3.2.tar.gz` & `tmp/tidy3d-2.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy3d-2.3.2.tar", last modified: Sat Jul 22 16:50:36 2023, max compression
+gzip compressed data, was "tidy3d-2.4.0rc1.tar", last modified: Thu Jul 27 21:20:53 2023, max compression
```

## Comparing `tidy3d-2.3.2.tar` & `tidy3d-2.4.0rc1.tar`

### file list

```diff
@@ -1,193 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.368388 tidy3d-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-22 16:50:20.000000 tidy3d-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-22 16:50:20.000000 tidy3d-2.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-22 16:50:36.368388 tidy3d-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-22 16:50:20.000000 tidy3d-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-22 16:50:20.000000 tidy3d-2.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.352388 tidy3d-2.3.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/basic.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/gdspy.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/gdstk.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/jax.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/trimesh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements/web.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-22 16:50:20.000000 tidy3d-2.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:50:36.368388 tidy3d-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-22 16:50:20.000000 tidy3d-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.352388 tidy3d-2.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.352388 tidy3d-2.3.2/tests/_test_local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/_test_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/_test_local/_test_adjoint_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/_test_local/_test_data_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/_test_local/_test_fit_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/_test_local/_test_plugins_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/_test_local/_test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.356388 tidy3d-2.3.2/tests/test_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    35660 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_meshgenerate.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_sidewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    54875 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_components/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.356388 tidy3d-2.3.2/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_data/test_data_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_data/test_monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_data/test_sim_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.356388 tidy3d-2.3.2/tests/test_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_package/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_package/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_package/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_package/test_make_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_package/test_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_package/test_parametric_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.356388 tidy3d-2.3.2/tests/test_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47180 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/test_adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/test_component_modeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/test_dispersion_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/test_mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/test_polyslab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/test_resonance_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_plugins/test_waveguide.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.356388 tidy3d-2.3.2/tests/test_web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/mock_web.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/test_material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/test_tidy3d_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/test_tidy3d_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     9391 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/test_tidy3d_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/test_web/test_webapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21275 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.360388 tidy3d-2.3.2/tidy3d/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.360388 tidy3d-2.3.2/tidy3d/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)    26944 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.360388 tidy3d-2.3.2/tidy3d/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    14518 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    84194 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)   147649 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/components/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/grid/grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    47562 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/grid/mesher.py
--rw-r--r--   0 runner    (1001) docker     (123)   124301 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    34086 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)   121422 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    33009 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/components/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/material_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/material_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62878 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/material_library/material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/material_library/material_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/material_library/parametric_materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/plugins/adjoint/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17841 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29109 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    22900 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    29884 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/adjoint/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/plugins/dispersion/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/dispersion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/dispersion/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/dispersion/fit_web.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/dispersion/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/plugins/mode/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/mode/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)    26106 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/mode/mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    30578 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/mode/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/mode/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16290 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/mode/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.364388 tidy3d-2.3.2/tidy3d/plugins/polyslab/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/polyslab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/polyslab/polyslab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.368388 tidy3d-2.3.2/tidy3d/plugins/resonance/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/resonance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/resonance/resonance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.368388 tidy3d-2.3.2/tidy3d/plugins/smatrix/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/smatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19900 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/smatrix/smatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.368388 tidy3d-2.3.2/tidy3d/plugins/waveguide/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/waveguide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35912 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/plugins/waveguide/rectangular_dielectric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.368388 tidy3d-2.3.2/tidy3d/web/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.368388 tidy3d-2.3.2/tidy3d/web/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    22414 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/http_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/httputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/material_libray.py
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/s3utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16788 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/simulation_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26567 2023-07-22 16:50:20.000000 tidy3d-2.3.2/tidy3d/web/webapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:36.360388 tidy3d-2.3.2/tidy3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-22 16:50:36.000000 tidy3d-2.3.2/tidy3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-22 16:50:36.000000 tidy3d-2.3.2/tidy3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:50:36.000000 tidy3d-2.3.2/tidy3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-22 16:50:36.000000 tidy3d-2.3.2/tidy3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-22 16:50:36.000000 tidy3d-2.3.2/tidy3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-22 16:50:36.000000 tidy3d-2.3.2/tidy3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.303851 tidy3d-2.4.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-27 21:20:53.299851 tidy3d-2.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.239848 tidy3d-2.4.0rc1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/requirements/basic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/requirements/gdspy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/requirements/gdstk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/requirements/jax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/requirements/trimesh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/requirements/web.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:20:53.303851 tidy3d-2.4.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.239848 tidy3d-2.4.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.243848 tidy3d-2.4.0rc1/tests/_test_local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/_test_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/_test_local/_test_adjoint_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/_test_local/_test_data_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/_test_local/_test_fit_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/_test_local/_test_plugins_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/_test_local/_test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.251848 tidy3d-2.4.0rc1/tests/test_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35660 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20503 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_meshgenerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_sidewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56886 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_components/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.251848 tidy3d-2.4.0rc1/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_data/test_data_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_data/test_monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_data/test_sim_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.255849 tidy3d-2.4.0rc1/tests/test_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_package/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_package/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_package/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_package/test_make_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_package/test_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_package/test_parametric_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.255849 tidy3d-2.4.0rc1/tests/test_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48095 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_plugins/test_adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_plugins/test_component_modeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_plugins/test_dispersion_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14120 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_plugins/test_mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_plugins/test_polyslab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_plugins/test_resonance_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_plugins/test_waveguide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.259849 tidy3d-2.4.0rc1/tests/test_web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_web/mock_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_web/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_web/test_material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_web/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_web/test_tidy3d_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_web/test_tidy3d_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9391 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_web/test_tidy3d_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/test_web/test_webapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.263849 tidy3d-2.4.0rc1/tidy3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.271849 tidy3d-2.4.0rc1/tidy3d/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26944 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.275850 tidy3d-2.4.0rc1/tidy3d/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84194 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147656 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.275850 tidy3d-2.4.0rc1/tidy3d/components/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/grid/grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47562 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/grid/mesher.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124301 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34086 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124277 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36679 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/components/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.279850 tidy3d-2.4.0rc1/tidy3d/material_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/material_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62878 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/material_library/material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/material_library/material_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/material_library/parametric_materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.279850 tidy3d-2.4.0rc1/tidy3d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.279850 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.283850 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.283850 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17841 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29109 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22900 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.283850 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/utils/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/utils/penalty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29884 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.287850 tidy3d-2.4.0rc1/tidy3d/plugins/dispersion/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/dispersion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/dispersion/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35338 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/dispersion/fit_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/dispersion/fit_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/dispersion/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.291851 tidy3d-2.4.0rc1/tidy3d/plugins/mode/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/mode/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29189 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/mode/mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30578 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/mode/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/mode/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/mode/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.291851 tidy3d-2.4.0rc1/tidy3d/plugins/polyslab/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/polyslab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/polyslab/polyslab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.291851 tidy3d-2.4.0rc1/tidy3d/plugins/resonance/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/resonance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/resonance/resonance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.291851 tidy3d-2.4.0rc1/tidy3d/plugins/smatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/smatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19603 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/smatrix/smatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.291851 tidy3d-2.4.0rc1/tidy3d/plugins/waveguide/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/waveguide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35912 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/plugins/waveguide/rectangular_dielectric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.299851 tidy3d-2.4.0rc1/tidy3d/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.299851 tidy3d-2.4.0rc1/tidy3d/web/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22411 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/http_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/httputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/material_libray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/simulation_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27140 2023-07-27 21:20:34.000000 tidy3d-2.4.0rc1/tidy3d/web/webapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:20:53.267849 tidy3d-2.4.0rc1/tidy3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-27 21:20:53.000000 tidy3d-2.4.0rc1/tidy3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-27 21:20:53.000000 tidy3d-2.4.0rc1/tidy3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:20:53.000000 tidy3d-2.4.0rc1/tidy3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 21:20:53.000000 tidy3d-2.4.0rc1/tidy3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-27 21:20:53.000000 tidy3d-2.4.0rc1/tidy3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-27 21:20:53.000000 tidy3d-2.4.0rc1/tidy3d.egg-info/top_level.txt
```

### Comparing `tidy3d-2.3.2/LICENSE` & `tidy3d-2.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/PKG-INFO` & `tidy3d-2.4.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.3.2
+Version: 2.4.0rc1
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.3.2/README.md` & `tidy3d-2.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/setup.py` & `tidy3d-2.4.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/_test_local/_test_adjoint_performance.py` & `tidy3d-2.4.0rc1/tests/_test_local/_test_adjoint_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/_test_local/_test_data_performance.py` & `tidy3d-2.4.0rc1/tests/_test_local/_test_data_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/_test_local/_test_fit_web.py` & `tidy3d-2.4.0rc1/tests/_test_local/_test_fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/_test_local/_test_plugins_web.py` & `tidy3d-2.4.0rc1/tests/_test_local/_test_plugins_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/_test_local/_test_web.py` & `tidy3d-2.4.0rc1/tests/_test_local/_test_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_components/test_IO.py` & `tidy3d-2.4.0rc1/tests/test_components/test_IO.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,17 +33,23 @@
 def set_datasets_to_none(sim):
     sim_dict = sim.dict()
     for src in sim_dict["sources"]:
         if src["type"] == "CustomFieldSource":
             src["field_dataset"] = None
         elif src["type"] == "CustomCurrentSource":
             src["current_dataset"] = None
+        if src["source_time"]["type"] == "CustomSourceTime":
+            src["source_time"]["source_time_dataset"] = None
     for structure in sim_dict["structures"]:
         if structure["geometry"]["type"] == "TriangleMesh":
             structure["geometry"]["mesh_dataset"] = None
+        if structure["geometry"]["type"] == "GeometryGroup":
+            for geometry in structure["geometry"]["geometries"]:
+                if geometry["type"] == "TriangleMesh":
+                    geometry["mesh_dataset"] = None
         if "Custom" in structure["medium"]["type"]:
             if structure["medium"]["type"] == "CustomMedium":
                 structure["medium"]["eps_dataset"] = None
             elif structure["medium"]["type"] == "CustomPoleResidue":
                 structure["medium"]["poles"] = []
             else:
                 structure["medium"]["coeffs"] = []
```

### Comparing `tidy3d-2.3.2/tests/test_components/test_apodization.py` & `tidy3d-2.4.0rc1/tests/test_components/test_apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_components/test_base.py` & `tidy3d-2.4.0rc1/tests/test_components/test_base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_components/test_boundaries.py` & `tidy3d-2.4.0rc1/tests/test_components/test_boundaries.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_components/test_custom.py` & `tidy3d-2.4.0rc1/tests/test_components/test_custom.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_components/test_field_projection.py` & `tidy3d-2.4.0rc1/tests/test_components/test_field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_components/test_geometry.py` & `tidy3d-2.4.0rc1/tests/test_components/test_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -561,7 +561,21 @@
 
     # test zero area triangles
     vertices = np.array([[1, 0, 0], [1, 0, 0], [0, 1, 0], [0, 0, 1]])
     faces = np.array([[1, 2, 3], [0, 3, 2], [0, 1, 3], [0, 2, 1]])
     tetrahedron = trimesh.Trimesh(vertices, faces)
     with pytest.raises(pydantic.ValidationError):
         geom = td.TriangleMesh.from_trimesh(tetrahedron)
+
+    # test trimesh.Scene
+    import_geom = td.TriangleMesh.from_stl("tests/data/two_boxes_separate.stl")
+    sim = sim = td.Simulation(
+        size=(10, 10, 10),
+        grid_spec=td.GridSpec.uniform(dl=0.1),
+        sources=[],
+        structures=[td.Structure(geometry=import_geom, medium=td.Medium(permittivity=2))],
+        monitors=[],
+        run_time=1e-12,
+        boundary_spec=td.BoundarySpec.all_sides(td.PML()),
+    )
+    _, ax = plt.subplots()
+    _ = sim.plot(y=0, ax=ax)
```

### Comparing `tidy3d-2.3.2/tests/test_components/test_grid.py` & `tidy3d-2.4.0rc1/tests/test_components/test_grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_components/test_grid_spec.py` & `tidy3d-2.4.0rc1/tests/test_components/test_grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_components/test_medium.py` & `tidy3d-2.4.0rc1/tests/test_components/test_medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_components/test_meshgenerate.py` & `tidy3d-2.4.0rc1/tests/test_components/test_meshgenerate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_components/test_mode.py` & `tidy3d-2.4.0rc1/tests/test_components/test_mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_components/test_monitor.py` & `tidy3d-2.4.0rc1/tests/test_components/test_monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_components/test_sidewall.py` & `tidy3d-2.4.0rc1/tests/test_components/test_sidewall.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_components/test_simulation.py` & `tidy3d-2.4.0rc1/tests/test_components/test_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,76 @@
     sim.frequency_range
     sim.grid
     sim.num_cells
     sim.discretize(m)
     sim.epsilon(m)
 
 
+def test_monitors_data_size():
+    """make sure a simulation can be initialized"""
+
+    sim = td.Simulation(
+        size=(2.0, 2.0, 2.0),
+        run_time=1e-12,
+        structures=[
+            td.Structure(
+                geometry=td.Box(size=(1, 1, 1), center=(-1, 0, 0)),
+                medium=td.Medium(permittivity=2.0),
+            ),
+            td.Structure(
+                geometry=td.Box(size=(1, 1, 1), center=(0, 0, 0)),
+                medium=td.Medium(permittivity=1.0, conductivity=3.0),
+            ),
+            td.Structure(
+                geometry=td.Sphere(radius=1.4, center=(1.0, 0.0, 1.0)), medium=td.Medium()
+            ),
+            td.Structure(
+                geometry=td.Cylinder(radius=1.4, length=2.0, center=(1.0, 0.0, -1.0), axis=1),
+                medium=td.Medium(),
+            ),
+        ],
+        sources=[
+            td.UniformCurrentSource(
+                size=(0, 0, 0),
+                center=(0, -0.5, 0),
+                polarization="Hx",
+                source_time=td.GaussianPulse(
+                    freq0=1e14,
+                    fwidth=1e12,
+                ),
+                name="my_dipole",
+            ),
+            td.PointDipole(
+                center=(0, 0, 0),
+                polarization="Ex",
+                source_time=td.GaussianPulse(
+                    freq0=1e14,
+                    fwidth=1e12,
+                ),
+            ),
+        ],
+        monitors=[
+            td.FieldMonitor(size=(0, 0, 0), center=(0, 0, 0), freqs=[1, 2], name="point"),
+            td.FluxTimeMonitor(size=(1, 1, 0), center=(0, 0, 0), interval=10, name="plane"),
+        ],
+        symmetry=(0, 1, -1),
+        boundary_spec=td.BoundarySpec(
+            x=td.Boundary.pml(num_layers=20),
+            y=td.Boundary.stable_pml(num_layers=30),
+            z=td.Boundary.absorber(num_layers=100),
+        ),
+        shutoff=1e-6,
+        courant=0.8,
+        subpixel=False,
+    )
+
+    datas = sim.monitors_data_size
+    assert len(datas) == 2
+
+
 def test_deprecation_defaults(log_capture):
     """Make sure deprecation warnings NOT thrown if defaults used."""
     s = td.Simulation(
         size=(1, 1, 1),
         run_time=1e-12,
         grid_spec=td.GridSpec.uniform(dl=0.1),
         sources=[
```

### Comparing `tidy3d-2.3.2/tests/test_components/test_source.py` & `tidy3d-2.4.0rc1/tests/test_components/test_source.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 _, AX = plt.subplots()
 
 ST = td.GaussianPulse(freq0=2e14, fwidth=1e14)
 S = td.PointDipole(source_time=ST, polarization="Ex")
 
 
+ATOL = 1e-8
+
+
 def test_plot_source_time():
 
     for val in ("real", "imag", "abs"):
         ST.plot(times=[1e-15, 2e-15, 3e-15], val=val, ax=AX)
         ST.plot_spectrum(times=[1e-15, 2e-15, 3e-15], num_freqs=4, val=val, ax=AX)
 
     with pytest.raises(ValueError):
@@ -243,7 +246,50 @@
             size=(0, 1, 1),
             direction="+",
             source_time=g,
             mode_spec=mode_spec,
             mode_index=0,
             num_freqs=-10,
         )
+
+
+def test_custom_source_time():
+    g = td.GaussianPulse(freq0=1, fwidth=0.1)
+    ts = np.linspace(0, 30, 1001)
+    amp_time = g.amp_time(ts)
+
+    # basic test
+    cst = td.CustomSourceTime.from_values(freq0=1, fwidth=0.1, values=amp_time, dt=ts[1] - ts[0])
+    assert np.allclose(cst.amp_time(ts), amp_time, rtol=0, atol=ATOL)
+
+    # test single value validation error
+    with pytest.raises(pydantic.ValidationError):
+        vals = td.components.data.data_array.TimeDataArray([1], coords=dict(t=[0]))
+        dataset = td.components.data.dataset.TimeDataset(values=vals)
+        cst = td.CustomSourceTime(source_time_dataset=dataset, freq0=1, fwidth=0.1)
+        assert np.allclose(cst.amp_time([0]), [1], rtol=0, atol=ATOL)
+
+    # test interpolation
+    cst = td.CustomSourceTime.from_values(freq0=1, fwidth=0.1, values=np.linspace(0, 9, 10), dt=0.1)
+    assert np.allclose(cst.amp_time(0.09), [0.9], rtol=0, atol=ATOL)
+
+    # test sampling warning
+    cst = td.CustomSourceTime.from_values(freq0=1, fwidth=0.1, values=np.linspace(0, 9, 10), dt=0.1)
+    source = td.PointDipole(center=(0, 0, 0), source_time=cst, polarization="Ex")
+    sim = td.Simulation(
+        size=(10, 10, 10),
+        run_time=1e-12,
+        grid_spec=td.GridSpec.uniform(dl=0.1),
+        sources=[source],
+    )
+
+    # test out of range validation error
+    with pytest.raises(td.exceptions.ValidationError):
+        vals = np.cos(sim.tmesh[:-2])
+        cst = td.CustomSourceTime.from_values(freq0=1, fwidth=0.1, values=vals, dt=sim.dt)
+        source = td.PointDipole(center=(0, 0, 0), source_time=cst, polarization="Ex")
+        sim = sim.updated_copy(sources=[source])
+
+    vals = np.cos(sim.tmesh[:-1])
+    cst = td.CustomSourceTime.from_values(freq0=1, fwidth=0.1, values=vals, dt=sim.dt)
+    source = td.PointDipole(center=(0, 0, 0), source_time=cst, polarization="Ex")
+    sim = sim.updated_copy(sources=[source])
```

### Comparing `tidy3d-2.3.2/tests/test_components/test_types.py` & `tidy3d-2.4.0rc1/tests/test_components/test_types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_components/test_viz.py` & `tidy3d-2.4.0rc1/tests/test_components/test_viz.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_data/test_data_arrays.py` & `tidy3d-2.4.0rc1/tests/test_data/test_data_arrays.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_data/test_monitor_data.py` & `tidy3d-2.4.0rc1/tests/test_data/test_monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_data/test_sim_data.py` & `tidy3d-2.4.0rc1/tests/test_data/test_sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_package/test_config.py` & `tidy3d-2.4.0rc1/tests/test_package/test_config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_package/test_log.py` & `tidy3d-2.4.0rc1/tests/test_package/test_log.py`

 * *Files 12% similar despite different names*

```diff
@@ -127,7 +127,24 @@
     sim_json = sim.json()
 
     td.log.set_capture(True)
     sim = td.Simulation.parse_raw(sim_json)
     warning_list = td.log.captured_warnings()
     assert len(warning_list) == 15
     td.log.set_capture(False)
+
+
+def test_log_suppression():
+    with td.log as suppressed_log:
+        assert td.log._counts is not None
+        for i in range(4):
+            suppressed_log.warning("Warning message")
+        assert td.log._counts[30] == 3
+
+    td.config.log_suppression = False
+    with td.log as suppressed_log:
+        assert td.log._counts is None
+        for i in range(4):
+            suppressed_log.warning("Warning message")
+        assert td.log._counts is None
+
+    td.config.log_suppression = True
```

### Comparing `tidy3d-2.3.2/tests/test_package/test_make_script.py` & `tidy3d-2.4.0rc1/tests/test_package/test_make_script.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_package/test_material_library.py` & `tidy3d-2.4.0rc1/tests/test_package/test_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_package/test_parametric_variants.py` & `tidy3d-2.4.0rc1/tests/test_package/test_parametric_variants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_plugins/test_adjoint.py` & `tidy3d-2.4.0rc1/tests/test_plugins/test_adjoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 from tidy3d.plugins.adjoint.components.data.sim_data import JaxSimulationData
 from tidy3d.plugins.adjoint.components.data.monitor_data import JaxModeData, JaxDiffractionData
 from tidy3d.plugins.adjoint.components.data.data_array import JaxDataArray, JAX_DATA_ARRAY_TAG
 from tidy3d.plugins.adjoint.components.data.dataset import JaxPermittivityDataset
 from tidy3d.plugins.adjoint.web import run, run_async
 from tidy3d.plugins.adjoint.web import run_local, run_async_local
 from tidy3d.plugins.adjoint.components.data.data_array import VALUE_FILTER_THRESHOLD
+from tidy3d.plugins.adjoint.utils.penalty import RadiusPenalty
+from tidy3d.plugins.adjoint.utils.filter import ConicFilter, BinaryProjector
 from tidy3d.web.container import BatchData
 from tidy3d.web import run as run_regular
 
 from ..utils import run_emulated, assert_log_level, log_capture, run_async_emulated
 from ..utils import SIM_DATA_PATH, SIM_FULL, TMP_DIR
 
 FWD_SIM_DATA_FILE = TMP_DIR + "adjoint_grad_data_fwd.hdf5"
@@ -1406,7 +1408,29 @@
         struct = sim.input_structures[0]
         return sim.updated_copy(input_structures=num_input_structures * [struct])
 
     sim = make_sim_(num_input_structures=MAX_NUM_INPUT_STRUCTURES)
 
     with pytest.raises(pydantic.ValidationError):
         sim = make_sim_(num_input_structures=MAX_NUM_INPUT_STRUCTURES + 1)
+
+
+@pytest.mark.parametrize("strict_binarize", (True, False))
+def test_adjoint_utils(strict_binarize):
+    """Test filtering, projection, and optimization routines."""
+
+    sim = make_sim(permittivity=EPS, size=SIZE, vertices=VERTICES, base_eps_val=BASE_EPS_VAL)
+
+    # projection / filtering
+    image = sim.input_structures[2].medium.eps_dataset.eps_xx.values
+
+    filter = ConicFilter(feature_size=1.5, design_region_dl=0.1)
+    filter.evaluate(image)
+    projector = BinaryProjector(vmin=1.0, vmax=2.0, beta=1.5, strict_binarize=strict_binarize)
+    projector.evaluate(image)
+
+    # radius of curvature
+
+    polyslab = sim.input_structures[3].geometry
+
+    radius_penalty = RadiusPenalty(min_radius=0.2, wrap=True)
+    penalty = radius_penalty.evaluate(polyslab.vertices)
```

### Comparing `tidy3d-2.3.2/tests/test_plugins/test_component_modeler.py` & `tidy3d-2.4.0rc1/tests/test_plugins/test_component_modeler.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_plugins/test_dispersion_fitter.py` & `tidy3d-2.4.0rc1/tests/test_plugins/test_dispersion_fitter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import numpy as np
 import pytest
 import responses
 
+import matplotlib.pylab as plt
+
 import tidy3d as td
-from tidy3d.plugins.dispersion import DispersionFitter
+from tidy3d.plugins.dispersion import DispersionFitter, FastDispersionFitter
+from tidy3d.plugins.dispersion import AdvancedFastFitterParam
 from tidy3d.plugins.dispersion.web import run as run_fitter
 
+advanced_param = AdvancedFastFitterParam(num_iters=1, passivity_num_iters=1)
+
+
+_, AX = plt.subplots()
+
 
 @pytest.fixture
 def random_data():
     data_points = 11
     wvl_um = np.linspace(1, 2, data_points)
     n_data = np.random.random(data_points)
     k_data = np.random.random(data_points)
@@ -59,63 +67,85 @@
     """perform fitting on random data"""
     wvl_um, n_data, _ = random_data
     fitter = DispersionFitter(wvl_um=wvl_um.tolist(), n_data=tuple(n_data))
     medium, rms = fitter._fit_single()
     medium, rms = fitter.fit(num_tries=2)
     medium, rms = run_fitter(fitter)
 
+    fitter = FastDispersionFitter(wvl_um=wvl_um.tolist(), n_data=tuple(n_data))
+    medium, rms = fitter.fit(advanced_param=advanced_param)
+
 
 @responses.activate
 def test_lossy_dispersion(random_data, mock_remote_api):
     """perform fitting on random lossy data"""
     wvl_um, n_data, k_data = random_data
     fitter = DispersionFitter(wvl_um=wvl_um, n_data=n_data, k_data=k_data)
     medium, rms = fitter._fit_single()
     medium, rms = fitter.fit(num_tries=2)
     medium, rms = run_fitter(fitter)
 
+    fitter = FastDispersionFitter(wvl_um=wvl_um.tolist(), n_data=n_data, k_data=k_data)
+    medium, rms = fitter.fit(advanced_param=advanced_param)
+
 
 def test_dispersion_load():
     """loads dispersion model from nk data file"""
     fitter = DispersionFitter.from_file("tests/data/nk_data.csv", skiprows=1, delimiter=",")
     medium, rms = fitter.fit(num_tries=20)
 
+    fitter = FastDispersionFitter.from_file("tests/data/nk_data.csv", skiprows=1, delimiter=",")
+    medium, rms = fitter.fit(advanced_param=advanced_param)
+
 
 def test_dispersion_plot(random_data):
     """plots a medium fit from file"""
     wvl_um, n_data, k_data = random_data
 
     fitter = DispersionFitter(wvl_um=wvl_um, n_data=n_data)
-    fitter.plot()
+    fitter.plot(ax=AX)
     medium, rms = fitter.fit(num_tries=2)
-    fitter.plot(medium)
+    fitter.plot(medium, ax=AX)
 
     fitter = DispersionFitter(wvl_um=wvl_um, n_data=n_data, k_data=k_data)
     fitter.plot()
     medium, rms = fitter.fit(num_tries=2)
-    fitter.plot(medium)
+    fitter.plot(medium, ax=AX)
 
 
 def test_dispersion_set_wvg_range(random_data):
     """set wavelength range function"""
     wvl_um, n_data, k_data = random_data
     fitter = DispersionFitter(wvl_um=wvl_um, n_data=n_data)
+    fastfitter = FastDispersionFitter(wvl_um=wvl_um, n_data=n_data)
 
     wvl_range = [1.2, 1.8]
     fitter = fitter.copy(update={"wvl_range": wvl_range})
     assert len(fitter.freqs) == 7
     medium, rms = fitter.fit(num_tries=2)
+    fastfitter = fastfitter.copy(update={"wvl_range": wvl_range})
+    assert len(fastfitter.freqs) == 7
+    medium, rms = fastfitter.fit(advanced_param=advanced_param)
 
     wvl_range = [1.2, 2.8]
     fitter = fitter.copy(update={"wvl_range": wvl_range, "k_data": k_data})
     assert len(fitter.freqs) == 9
     medium, rms = fitter.fit(num_tries=2)
+    fastfitter = fastfitter.copy(update={"wvl_range": wvl_range})
+    assert len(fastfitter.freqs) == 9
+    medium, rms = fastfitter.fit(advanced_param=advanced_param)
 
     wvl_range = [0.2, 1.8]
     fitter = fitter.copy(update={"wvl_range": wvl_range})
     assert len(fitter.freqs) == 9
     medium, rms = fitter.fit(num_tries=2)
+    fastfitter = fastfitter.copy(update={"wvl_range": wvl_range})
+    assert len(fastfitter.freqs) == 9
+    medium, rms = fastfitter.fit(advanced_param=advanced_param)
 
     wvl_range = [0.2, 2.8]
     fitter = fitter.copy(update={"wvl_range": wvl_range, "k_data": k_data})
     assert len(fitter.freqs) == 11
     medium, rms = fitter.fit(num_tries=2)
+    fastfitter = fastfitter.copy(update={"wvl_range": wvl_range})
+    assert len(fastfitter.freqs) == 11
+    medium, rms = fastfitter.fit(advanced_param=advanced_param)
```

### Comparing `tidy3d-2.3.2/tests/test_plugins/test_mode_solver.py` & `tidy3d-2.4.0rc1/tests/test_plugins/test_mode_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -200,14 +200,24 @@
         plane=PLANE,
         mode_spec=mode_spec,
         freqs=freqs,
         direction="-",
     )
     _ = ms.solve() if local else msweb.run(ms)
 
+    # Testing issue 807 functions
+    freq0 = td.C_0 / 1.55
+    source_time = td.GaussianPulse(freq0=freq0, fwidth=freq0 / 10)
+    nS_add_source = ms.sim_with_source(mode_index=0, direction="+", source_time=source_time)
+    nS_add_monitor = ms.sim_with_monitor(freqs=freqs, name="mode monitor")
+    nS_add_mode_solver_monitor = ms.sim_with_mode_solver_monitor(name="mode solver monitor")
+    assert len(nS_add_source.sources) == len(simulation.sources) + 1
+    assert len(nS_add_monitor.monitors) == len(simulation.monitors) + 1
+    assert len(nS_add_mode_solver_monitor.monitors) == len(simulation.monitors) + 1
+
 
 @pytest.mark.parametrize("local", [True, False])
 @responses.activate
 def test_mode_solver_custom_medium(mock_remote_api, local):
     """Test mode solver can work with custom medium. Consider a waveguide with varying
     permittivity along x-direction. The value of n_eff at different x position should be
     different.
@@ -246,14 +256,19 @@
             mode_spec=mode_spec,
             freqs=[freq0],
             direction="+",
         )
         modes = ms.solve() if local else msweb.run(ms)
         n_eff.append(modes.n_eff.values)
 
+        fname = "tests/tmp/ms_custom_medium.hdf5"
+        ms.to_file(fname)
+        m2 = ModeSolver.from_file(fname)
+        assert m2 == ms
+
     if local:
         assert n_eff[0] < 1.5
         assert n_eff[1] > 4
         assert n_eff[1] < 5
 
 
 def test_mode_solver_angle_bend():
```

### Comparing `tidy3d-2.3.2/tests/test_plugins/test_polyslab.py` & `tidy3d-2.4.0rc1/tests/test_plugins/test_polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_plugins/test_resonance_finder.py` & `tidy3d-2.4.0rc1/tests/test_plugins/test_resonance_finder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_plugins/test_waveguide.py` & `tidy3d-2.4.0rc1/tests/test_plugins/test_waveguide.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_web/test_cli.py` & `tidy3d-2.4.0rc1/tests/test_web/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_web/test_material_fitter.py` & `tidy3d-2.4.0rc1/tests/test_web/test_material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_web/test_tidy3d_folder.py` & `tidy3d-2.4.0rc1/tests/test_web/test_tidy3d_folder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_web/test_tidy3d_material_library.py` & `tidy3d-2.4.0rc1/tests/test_web/test_tidy3d_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_web/test_tidy3d_task.py` & `tidy3d-2.4.0rc1/tests/test_web/test_tidy3d_task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tests/test_web/test_webapi.py` & `tidy3d-2.4.0rc1/tests/test_web/test_webapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # Tests webapi and things that depend on it
-import tempfile
 import pytest
 import responses
 from _pytest import monkeypatch
 import os
 
 import tidy3d as td
-import tidy3d.web as web
 
 from responses import matchers
 
 from tidy3d.exceptions import SetupError
 from tidy3d.web.environment import Env
-from tidy3d.web.webapi import delete, delete_old, download, download_json, run
+from tidy3d.web.webapi import delete, delete_old, download, download_json, run, abort
 from tidy3d.web.webapi import download_log, estimate_cost, get_info, get_run_info, get_tasks
 from tidy3d.web.webapi import load, load_simulation, start, upload, monitor, real_cost
 from tidy3d.web.container import Job, Batch
-from tidy3d.web.task import TaskInfo
 from tidy3d.web.asynchronous import run_async
 
 from tidy3d.__main__ import main
 
 from ..utils import TMP_DIR
 
 # variables used below
@@ -147,20 +144,18 @@
         },
         status=200,
     )
 
 
 @pytest.fixture
 def mock_monitor(monkeypatch):
-
     status_count = [0]
     statuses = ("upload", "running", "running", "running", "running", "running", "success")
 
     def mock_get_status(task_id):
-
         current_count = min(status_count[0], len(statuses) - 1)
         current_status = statuses[current_count]
         status_count[0] += 1
         return current_status
         # return TaskInfo(status=current_status, taskName=TASK_NAME, taskId=task_id, realFlexUnit=1.0)
 
     run_count = [0]
@@ -284,15 +279,14 @@
 
     monkeypatch.setattr("tidy3d.web.simulation_task.download_file", mock_download)
     load(TASK_ID, "tmp/monitor_data.hdf5")
 
 
 @responses.activate
 def test_delete(set_api_key, mock_get_info):
-
     responses.add(
         responses.DELETE,
         f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}",
         json={
             "data": {
                 "taskId": TASK_ID,
                 "createdAt": CREATED_AT,
@@ -378,15 +372,14 @@
     )
 
     delete_old(100)
 
 
 @responses.activate
 def test_get_tasks(set_api_key):
-
     responses.add(
         responses.GET,
         f"{Env.current.web_api_endpoint}/tidy3d/project",
         match=[matchers.query_param_matcher({"projectName": PROJECT_NAME})],
         json={"data": {"projectId": TASK_ID, "projectName": PROJECT_NAME}},
         status=200,
     )
@@ -414,20 +407,38 @@
 
 
 @responses.activate
 def test_real_cost(mock_get_info):
     assert real_cost(TASK_ID) == FLEX_UNIT
 
 
+@responses.activate
+def test_abort_task(set_api_key):
+    responses.add(
+        responses.PUT,
+        f"{Env.current.web_api_endpoint}/tidy3d/tasks/abort",
+        match=[
+            matchers.json_params_matcher(
+                {
+                    "taskId": TASK_ID,
+                    "taskType": "FDTD",
+                }
+            )
+        ],
+        json={"result": True},
+        status=200,
+    )
+    abort(TASK_ID)
+
+
 """ Containers """
 
 
 @responses.activate
 def test_job(mock_webapi, monkeypatch):
-
     monkeypatch.setattr("tidy3d.web.container.Job.load", lambda *args, **kwargs: True)
     sim = make_sim()
     j = Job(simulation=sim, task_name=TASK_NAME, folder_name=PROJECT_NAME)
 
     sim_data = j.run(path=FNAME_TMP)
     j.status
     j.estimate_cost()
@@ -440,15 +451,14 @@
 def mock_job_status(monkeypatch):
     monkeypatch.setattr("tidy3d.web.container.Job.status", property(lambda self: "success"))
     monkeypatch.setattr("tidy3d.web.container.Job.load", lambda *args, **kwargs: True)
 
 
 @responses.activate
 def test_batch(mock_webapi, mock_job_status):
-
     # monkeypatch.setattr("tidy3d.web.container.Batch.monitor", lambda self: time.sleep(0.1))
     # monkeypatch.setattr("tidy3d.web.container.Job.status", property(lambda self: "success"))
 
     sims = {TASK_NAME: make_sim()}
     b = Batch(simulations=sims, folder_name=PROJECT_NAME)
     b.estimate_cost()
     batch_data = b.run(path_dir="tests/tmp/")
@@ -456,26 +466,24 @@
 
 
 """ Async """
 
 
 @responses.activate
 def test_async(mock_webapi, mock_job_status):
-
     # monkeypatch.setattr("tidy3d.web.container.Job.status", property(lambda self: "success"))
     sims = {TASK_NAME: make_sim()}
     batch_data = run_async(sims, folder_name=PROJECT_NAME)
 
 
 """ Main """
 
 
 @responses.activate
 def test_main(mock_webapi, monkeypatch, mock_job_status):
-
     # sims = {TASK_NAME: make_sim()}
     # batch_data = run_async(sims, folder_name=PROJECT_NAME)
 
     def save_sim_to_path(path: str) -> None:
         sim = make_sim()
         sim.to_file(path)
```

### Comparing `tidy3d-2.3.2/tests/utils.py` & `tidy3d-2.4.0rc1/tests/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -246,14 +246,20 @@
                         [[1, 1, 1], [1, 1, 1], [1, 1, 1]],
                         [[1, 1, 1], [1, 1, 1], [1, 1, 1]],
                     ]
                 )
             ),
             medium=td.Medium(permittivity=5),
         ),
+        Structure(
+            geometry=TriangleMesh.from_stl(
+                "tests/data/two_boxes_separate.stl", scale=0.1, origin=(0.5, 0.5, 0.5)
+            ),
+            medium=td.Medium(permittivity=5),
+        ),
     ],
     sources=[
         UniformCurrentSource(
             size=(0, 0, 0),
             center=(0, 0.5, 0),
             polarization="Hx",
             source_time=GaussianPulse(
@@ -355,14 +361,22 @@
                 fwidth=4e13,
             ),
             direction="+",
             angle_theta=np.pi / 6,
             angle_phi=np.pi / 5,
             injection_axis=2,
         ),
+        UniformCurrentSource(
+            size=(0, 0, 0),
+            center=(0, 0.5, 0),
+            polarization="Hx",
+            source_time=CustomSourceTime.from_values(
+                freq0=2e14, fwidth=4e13, values=np.linspace(0, 10, 1000), dt=1e-12 / 100
+            ),
+        ),
     ],
     monitors=(
         FieldMonitor(
             size=(0, 0, 0), center=(0, 0, 0), fields=["Ex"], freqs=[1.5e14, 2e14], name="field"
         ),
         FieldTimeMonitor(size=(0, 0, 0), center=(0, 0, 0), name="field_time", interval=100),
         FluxMonitor(size=(1, 1, 0), center=(0, 0, 0), freqs=[2e14, 2.5e14], name="flux"),
```

### Comparing `tidy3d-2.3.2/tidy3d/__init__.py` & `tidy3d-2.4.0rc1/tidy3d/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # modes
 from .components.mode import ModeSpec
 
 # apodization
 from .components.apodization import ApodizationSpec
 
 # sources
-from .components.source import GaussianPulse, ContinuousWave
+from .components.source import GaussianPulse, ContinuousWave, CustomSourceTime
 from .components.source import UniformCurrentSource, PlaneWave, ModeSource, PointDipole
 from .components.source import GaussianBeam, AstigmaticGaussianBeam
 from .components.source import CustomFieldSource, TFSF, CustomCurrentSource
 
 # monitors
 from .components.monitor import FieldMonitor, FieldTimeMonitor, FluxMonitor, FluxTimeMonitor
 from .components.monitor import ModeMonitor, ModeSolverMonitor, PermittivityMonitor
```

### Comparing `tidy3d-2.3.2/tidy3d/__main__.py` & `tidy3d-2.4.0rc1/tidy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/apodization.py` & `tidy3d-2.4.0rc1/tidy3d/components/apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/base.py` & `tidy3d-2.4.0rc1/tidy3d/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/boundary.py` & `tidy3d-2.4.0rc1/tidy3d/components/boundary.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/data/data_array.py` & `tidy3d-2.4.0rc1/tidy3d/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/data/dataset.py` & `tidy3d-2.4.0rc1/tidy3d/components/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import numpy as np
 import pydantic as pd
 
 from .data_array import DataArray
 from .data_array import ScalarFieldDataArray, ScalarFieldTimeDataArray, ScalarModeFieldDataArray
 from .data_array import ModeIndexDataArray
 from .data_array import TriangleMeshDataArray
+from .data_array import TimeDataArray
 
 from ..base import Tidy3dBaseModel
 from ..types import Axis
 from ...exceptions import DataError
 
 
 class Dataset(Tidy3dBaseModel, ABC):
@@ -399,7 +400,15 @@
 
     surface_mesh: TriangleMeshDataArray = pd.Field(
         ...,
         title="Surface mesh data",
         description="Dataset containing the surface triangles and corresponding face indices "
         "for a surface mesh.",
     )
+
+
+class TimeDataset(Dataset):
+    """Dataset for storing a function of time."""
+
+    values: TimeDataArray = pd.Field(
+        ..., title="Values", description="Values as a function of time."
+    )
```

### Comparing `tidy3d-2.3.2/tidy3d/components/data/monitor_data.py` & `tidy3d-2.4.0rc1/tidy3d/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/data/sim_data.py` & `tidy3d-2.4.0rc1/tidy3d/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/field_projection.py` & `tidy3d-2.4.0rc1/tidy3d/components/field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/geometry.py` & `tidy3d-2.4.0rc1/tidy3d/components/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -3448,15 +3448,15 @@
 
         cls._check_trimesh_library()
 
         scene = trimesh.load(filename, **kwargs)
         meshes = []
         if isinstance(scene, trimesh.Trimesh):
             meshes = [scene]
-        elif isinstance(scene.trimesh.Scene):
+        elif isinstance(scene, trimesh.Scene):
             meshes = scene.dump()
         else:
             raise ValidationError(
                 "Invalid trimesh type in file. Supported types are 'trimesh.Trimesh' "
                 "and 'trimesh.Scene'."
             )
 
@@ -3651,15 +3651,15 @@
         # permute so normal is aligned with z axis
         # and (y, z), (x, z), resp. (x, y) are aligned with (x, y)
         identity = np.eye(3)
         permutation = self.unpop_axis(identity[2], identity[0:2], axis=axis)
         mapping[:3, :3] = np.array(permutation).T
 
         section2d, _ = section.to_planar(to_2D=mapping)
-        return section2d.polygons_full
+        return list(section2d.polygons_full)
 
     def inside(
         self, x: np.ndarray[float], y: np.ndarray[float], z: np.ndarray[float]
     ) -> np.ndarray[bool]:
         """For input arrays ``x``, ``y``, ``z`` of arbitrary but identical shape, return an array
         with the same shape which is ``True`` for every point in zip(x, y, z) that is inside the
         volume of the :class:`Geometry`, and ``False`` otherwise.
```

### Comparing `tidy3d-2.3.2/tidy3d/components/grid/grid.py` & `tidy3d-2.4.0rc1/tidy3d/components/grid/grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/grid/grid_spec.py` & `tidy3d-2.4.0rc1/tidy3d/components/grid/grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/grid/mesher.py` & `tidy3d-2.4.0rc1/tidy3d/components/grid/mesher.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/medium.py` & `tidy3d-2.4.0rc1/tidy3d/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/mode.py` & `tidy3d-2.4.0rc1/tidy3d/components/mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/monitor.py` & `tidy3d-2.4.0rc1/tidy3d/components/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/simulation.py` & `tidy3d-2.4.0rc1/tidy3d/components/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # pylint: disable=too-many-lines, too-many-arguments, too-many-statements
 """ Container holding all information about simulation and its components"""
 from __future__ import annotations
+
 from typing import Dict, Tuple, List, Set, Union
 from math import isclose
 
 import pydantic
 import numpy as np
 import xarray as xr
 import matplotlib.pylab as plt
 import matplotlib as mpl
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 from .base import cached_property
 from .validators import assert_unique_names, assert_objects_in_sim_bounds
 from .validators import validate_mode_objects_symmetry
-from .geometry import Box, TriangleMesh, Geometry, PolySlab, Cylinder
+from .geometry import Box, TriangleMesh, Geometry, PolySlab, Cylinder, GeometryGroup
 from .types import Ax, Shapely, FreqBound, Axis, annotate_type, Symmetry
 from .grid.grid import Coords1D, Grid, Coords
 from .grid.grid_spec import GridSpec, UniformGrid, AutoGrid
 from .medium import Medium, MediumType, AbstractMedium, PECMedium
 from .medium import AbstractCustomMedium, Medium2D, MediumType3D
 from .medium import AnisotropicMedium, FullyAnisotropicMedium
 from .boundary import BoundarySpec, BlochBoundary, PECBoundary, PMCBoundary, Periodic
 from .boundary import PML, StablePML, Absorber, AbsorberSpec
 from .structure import Structure
 from .source import SourceType, PlaneWave, GaussianBeam, AstigmaticGaussianBeam, CustomFieldSource
-from .source import CustomCurrentSource
+from .source import CustomCurrentSource, CustomSourceTime
 from .source import TFSF, Source
 from .monitor import MonitorType, Monitor, FreqMonitor, SurfaceIntegrationMonitor
 from .monitor import AbstractFieldMonitor, DiffractionMonitor, AbstractFieldProjectionMonitor
 from .data.dataset import Dataset
 from .viz import add_ax_if_none, equal_aspect
 
 from .viz import MEDIUM_CMAP, STRUCTURE_EPS_CMAP, PlotParams, plot_params_symmetry, polygon_path
@@ -64,14 +65,18 @@
 # for 2d materials. to find neighboring media, search a distance on either side
 # equal to this times the grid size
 DIST_NEIGHBOR_REL_2D_MED = 1e-5
 
 # height of the PML plotting boxes along any dimensions where sim.size[dim] == 0
 PML_HEIGHT_FOR_0_DIMS = 0.02
 
+# allow some numerical flexibility before warning about CustomSourceTime
+# in units of dt
+CUSTOMSOURCETIME_TOL = 1.1
+
 
 class Simulation(Box):  # pylint:disable=too-many-public-methods
     """Contains all information about Tidy3d simulation.
 
     Example
     -------
     >>> from tidy3d import Sphere, Cylinder, PolySlab
@@ -835,14 +840,15 @@
 
     """ Post-init validators """
 
     def _post_init_validators(self) -> None:
         """Call validators taking z`self` that get run after init."""
         self._validate_no_structures_pml()
         self._validate_tfsf_nonuniform_grid()
+        self._validate_customsourcetime()
 
     def _validate_no_structures_pml(self) -> None:
         """Ensure no structures terminate / have bounds inside of PML."""
 
         pml_thicks = np.array(self.pml_thicknesses).T
         sim_bounds = self.bounds
         bound_spec = self.boundary_spec.to_list
@@ -904,14 +910,42 @@
                             "to sub-optimal cancellation of the incident field in the "
                             "scattered-field region for the total-field scattered-field (TFSF) "
                             f"source '{source.name}'. For best results, we recommended ensuring a "
                             "uniform grid in both directions tangential to the TFSF injection "
                             f"axis, '{'xyz'[source.injection_axis]}'."
                         )
 
+    def _validate_customsourcetime(self) -> None:
+        """Make sure custom source time is not undersampled.
+        Also, make sure that all simulation.tmesh values are covered."""
+        for source in self.sources:
+            if isinstance(source.source_time, CustomSourceTime):
+                dataset = source.source_time.source_time_dataset
+                if dataset is None:
+                    continue
+                times = dataset.values.coords["t"].values
+                if (
+                    min(times) > self.tmesh[0]
+                    or max(times) < self.tmesh[-1] - CUSTOMSOURCETIME_TOL * self.dt
+                ):
+                    raise ValidationError(
+                        "'CustomSourceTime' found with time coordinates "
+                        "'times' that do not cover the entire 'Simulation.tmesh'. Currently, "
+                        f"'(min(times), max(times)) = ({min(times)}, {max(times)})', while "
+                        f"'(min(tmesh), max(tmesh)) = ({self.tmesh[0]}, {self.tmesh[-1]}).' "
+                    )
+                max_dt = np.amax(np.diff(times))
+                if max_dt > self.dt * CUSTOMSOURCETIME_TOL:
+                    log.warning(
+                        f"'CustomSourceTime' found with time step 'max(dt) = {max_dt:.3g}', "
+                        f"while the simulation time step is 'dt={self.dt}'. "
+                        "We recommend that the largest time step of the custom source "
+                        f"be smaller than the time step of the simulation."
+                    )
+
     """ Pre submit validation (before web.upload()) """
 
     def validate_pre_upload(self, source_required: bool = True) -> None:
         """Validate the fully initialized simulation is ok for upload to our servers.
 
         Parameters
         ----------
@@ -955,44 +989,53 @@
                 f"Simulation has {num_cells_times_steps:.2e} grid cells * time steps, "
                 f"a maximum of {MAX_CELLS_TIMES_STEPS:.2e} are allowed."
             )
 
     def _validate_monitor_size(self) -> None:
         """Ensures the monitors arent storing too much data before simulation is uploaded."""
 
-        tmesh = self.tmesh
-        grid = self.grid
-
         total_size_gb = 0
         with log as consolidated_logger:
-            for monitor in self.monitors:
-                monitor_inds = grid.discretize_inds(monitor, extend=True)
-                num_cells = [inds[1] - inds[0] for inds in monitor_inds]
-                # take monitor downsampling into account
-                if isinstance(monitor, AbstractFieldMonitor):
-                    num_cells = monitor.downsampled_num_cells(num_cells)
-                num_cells = np.prod(num_cells)
-                monitor_size = monitor.storage_size(num_cells=num_cells, tmesh=tmesh)
+            datas = self.monitors_data_size
+            for monitor_name, monitor_size in datas.items():
                 monitor_size_gb = monitor_size / 2**30
-
                 if monitor_size_gb > WARN_MONITOR_DATA_SIZE_GB:
                     consolidated_logger.warning(
-                        f"Monitor '{monitor.name}' estimated storage is {monitor_size_gb:1.2f}GB. "
+                        f"Monitor '{monitor_name}' estimated storage is {monitor_size_gb:1.2f}GB. "
                         "Consider making it smaller, using fewer frequencies, or spatial or "
                         "temporal downsampling using 'interval_space' and 'interval', respectively."
                     )
 
                 total_size_gb += monitor_size_gb
 
         if total_size_gb > MAX_SIMULATION_DATA_SIZE_GB:
             raise SetupError(
                 f"Simulation's monitors have {total_size_gb:.2f}GB of estimated storage, "
                 f"a maximum of {MAX_SIMULATION_DATA_SIZE_GB:.2f}GB are allowed."
             )
 
+    @cached_property
+    def monitors_data_size(self) -> Dict[str, float]:
+        """Dictionary mapping monitor names to their estimated storage size in bytes."""
+        tmesh = self.tmesh
+        grid = self.grid
+        data_size = {}
+        for monitor in self.monitors:
+            name = monitor.name
+            monitor_inds = grid.discretize_inds(monitor, extend=True)
+            num_cells = [inds[1] - inds[0] for inds in monitor_inds]
+            # take monitor downsampling into account
+            if isinstance(monitor, AbstractFieldMonitor):
+                num_cells = monitor.downsampled_num_cells(num_cells)
+            num_cells = np.prod(num_cells)
+            monitor_size = monitor.storage_size(num_cells=num_cells, tmesh=tmesh)
+            data_size[name] = float(monitor_size)
+
+        return data_size
+
     def _validate_datasets_not_none(self) -> None:
         """Ensures that all custom datasets are defined."""
         if any(dataset is None for dataset in self.custom_datasets):
             raise SetupError(
                 "Data for a custom data component is missing. This can happen for example if the "
                 "Simulation has been loaded from json. To save and load simulations with custom "
                 "data, use hdf5 format instead."
@@ -2253,17 +2296,25 @@
         """
         source_ranges = [source.source_time.frequency_range() for source in self.sources]
         freq_min = min((freq_range[0] for freq_range in source_ranges), default=0.0)
         freq_max = max((freq_range[1] for freq_range in source_ranges), default=0.0)
 
         return (freq_min, freq_max)
 
-    def plot_3d(self) -> None:
-        """Render 3D plot of ``Simulation`` (in jupyter notebook only)."""
-        return plot_sim_3d(self)
+    def plot_3d(self, width=800, height=800) -> None:
+        """Render 3D plot of ``Simulation`` (in jupyter notebook only).
+        Parameters
+        ----------
+        width : float = 800
+            width of the 3d view dom's size
+        height : float = 800
+            height of the 3d view dom's size
+
+        """
+        return plot_sim_3d(self, width=width, height=height)
 
     """ Discretization """
 
     @cached_property
     def dt(self) -> float:
         """Simulation time step (distance).
 
@@ -2671,27 +2722,42 @@
         return make_eps_data(coords)
 
     @property
     def custom_datasets(self) -> List[Dataset]:
         """List of custom datasets for verification purposes. If the list is not empty, then
         the simulation needs to be exported to hdf5 to store the data.
         """
+        datasets_source_time = [
+            src.source_time.source_time_dataset
+            for src in self.sources
+            if isinstance(src.source_time, CustomSourceTime)
+        ]
         datasets_field_source = [
             src.field_dataset for src in self.sources if isinstance(src, CustomFieldSource)
         ]
         datasets_current_source = [
             src.current_dataset for src in self.sources if isinstance(src, CustomCurrentSource)
         ]
         datasets_medium = [mat for mat in self.mediums if isinstance(mat, AbstractCustomMedium)]
-        datasets_geometry = [
-            struct.geometry.mesh_dataset
-            for struct in self.structures
-            if isinstance(struct.geometry, TriangleMesh)
-        ]
-        return datasets_field_source + datasets_current_source + datasets_medium + datasets_geometry
+        datasets_geometry = []
+
+        for struct in self.structures:
+            if isinstance(struct.geometry, TriangleMesh):
+                datasets_geometry += struct.geometry.mesh_dataset
+            elif isinstance(struct.geometry, GeometryGroup):
+                for geometry in struct.geometry.geometries:
+                    datasets_geometry += geometry.mesh_dataset
+
+        return (
+            datasets_source_time
+            + datasets_field_source
+            + datasets_current_source
+            + datasets_medium
+            + datasets_geometry
+        )
 
     def _volumetric_structures_grid(self, grid: Grid) -> Tuple[Structure]:
         """Generate a tuple of structures wherein any 2D materials are converted to 3D
         volumetric equivalents, using ``grid`` as the simulation grid."""
 
         if not any(isinstance(medium, Medium2D) for medium in self.mediums):
             return self.structures
```

### Comparing `tidy3d-2.3.2/tidy3d/components/source.py` & `tidy3d-2.4.0rc1/tidy3d/components/source.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """Defines electric current sources for injecting light into simulation."""
+# pylint: disable=too-many-lines
 
+from __future__ import annotations
 from abc import ABC, abstractmethod
 from typing import Union, Tuple, Optional
 
 from typing_extensions import Literal
 import pydantic
 import numpy as np
 
 from .base import Tidy3dBaseModel, cached_property
 
-from .types import Direction, Polarization, Ax, FreqBound, ArrayFloat1D, Axis, PlotVal
+from .types import Direction, Polarization, Ax, FreqBound
+from .types import ArrayFloat1D, Axis, PlotVal, ArrayComplex1D
 from .validators import assert_plane, assert_volumetric, validate_name_str, get_value
 from .validators import warn_if_dataset_none, assert_single_freq_in_range
-from .data.dataset import FieldDataset
+from .data.dataset import FieldDataset, TimeDataset
+from .data.data_array import TimeDataArray
 from .geometry import Box, Coordinate
 from .mode import ModeSpec
 from .viz import add_ax_if_none, PlotParams, plot_params_source
 from .viz import ARROW_COLOR_SOURCE, ARROW_ALPHA, ARROW_COLOR_POLARIZATION
 from ..constants import RADIAN, HERTZ, MICROMETER, GLANCING_CUTOFF
 from ..constants import inf  # pylint:disable=unused-import
-from ..exceptions import SetupError
+from ..exceptions import SetupError, ValidationError
 from ..log import log
 
 
 # in spectrum computation, discard amplitudes with relative magnitude smaller than cutoff
 DFT_CUTOFF = 1e-8
 # when checking if custom data spans the source plane, allow for a small tolerance
 # due to numerical precision
@@ -287,15 +291,107 @@
         offset = np.exp(1j * self.phase)
         oscillation = np.exp(-1j * omega0 * time)
         amp = 1 / (1 + np.exp(-time_shifted / twidth)) * self.amplitude
 
         return const * offset * oscillation * amp
 
 
-SourceTimeType = Union[GaussianPulse, ContinuousWave]
+class CustomSourceTime(Pulse):
+    """Custom source time dependence, real or complex valued.
+
+    Note
+    ----
+    The source time dependence is linearly interpolated to the simulation time steps.
+    To ensure that this interpolation does not introduce artifacts, it is necessary
+    to use a sampling rate that is sufficiently fast relative to the simulation time step.
+
+    Example
+    -------
+    >>> cst = td.CustomSourceTime.from_values(freq0=1, fwidth=0.1,
+    >>>     values=np.linspace(0, 9, 10), dt=0.1)
+    """
+
+    source_time_dataset: Optional[TimeDataset] = pydantic.Field(
+        ..., title="Source time dataset", description="Dataset for storing the custom source time."
+    )
+
+    _source_time_dataset_none_warning = warn_if_dataset_none("source_time_dataset")
+
+    @pydantic.validator("source_time_dataset", always=True)
+    def _more_than_one_time(cls, val):
+        """Must have more than one time to interpolate."""
+        if val is None:
+            return val
+        if val.values.size <= 1:
+            raise ValidationError("'CustomSourceTime' must have more than one time coordinate.")
+        return val
+
+    @classmethod
+    def from_values(
+        cls, freq0: float, fwidth: float, values: ArrayComplex1D, dt: float
+    ) -> CustomSourceTime:
+        """Create a :class:`.CustomSourceTime` from a numpy array.
+
+        Parameters
+        ----------
+        freq0 : float
+            Estimated central frequency of the source.
+        fwidth : float
+            Estimated frequency width of the source.
+        values: ArrayComplex1D
+            Complex values of the source amplitude.
+        dt: float
+            Time step for the `values` array. This value should be sufficiently small
+            relative to the simulation `dt` in order to avoid interpolation artifacts.
+
+
+        Returns
+        -------
+        CustomSourceTime
+            :class:`.CustomSourceTime` with these values, and time coordinates evenly spaced
+            between 0 and dt * (N-1) with a step size of `dt`, where N is the length of
+            the values array.
+        """
+        times = np.arange(len(values)) * dt
+        source_time_dataarray = TimeDataArray(values, coords=dict(t=times))
+        source_time_dataset = TimeDataset(values=source_time_dataarray)
+        return CustomSourceTime(
+            freq0=freq0,
+            fwidth=fwidth,
+            source_time_dataset=source_time_dataset,
+        )
+
+    def amp_time(self, time: float) -> complex:
+        """Complex-valued source amplitude as a function of time.
+
+        Parameters
+        ----------
+        time : float
+            Time in seconds.
+
+        Returns
+        -------
+        complex
+            Complex-valued source amplitude at that time.
+        """
+        if self.source_time_dataset is None:
+            return None
+        times = self.source_time_dataset.values.coords["t"].values.squeeze()
+        if isinstance(time, float):
+            if time < min(times) or time > max(times):
+                return self.source_time_dataset.values.sel(t=time, method="nearest").to_numpy()
+            return self.source_time_dataset.values.interp(t=time).to_numpy()
+        val = np.zeros(len(time), dtype=complex)
+        mask = (time < min(times)) | (time > max(times))
+        val[mask] = self.source_time_dataset.values.sel(t=time[mask], method="nearest").to_numpy()
+        val[~mask] = self.source_time_dataset.values.interp(t=time[~mask]).to_numpy()
+        return val
+
+
+SourceTimeType = Union[GaussianPulse, ContinuousWave, CustomSourceTime]
 
 """ Source objects """
 
 
 class Source(Box, ABC):
     """Abstract base class for all sources."""
```

### Comparing `tidy3d-2.3.2/tidy3d/components/structure.py` & `tidy3d-2.4.0rc1/tidy3d/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/transformation.py` & `tidy3d-2.4.0rc1/tidy3d/components/transformation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/types.py` & `tidy3d-2.4.0rc1/tidy3d/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/validators.py` & `tidy3d-2.4.0rc1/tidy3d/components/validators.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/components/viz.py` & `tidy3d-2.4.0rc1/tidy3d/components/viz.py`

 * *Files 3% similar despite different names*

```diff
@@ -223,15 +223,15 @@
     return PathPatch(polygon_path(polygon), **kwargs)
 
 
 """End descartes modification
 ================================================================================================="""
 
 
-def plot_sim_3d(sim) -> None:
+def plot_sim_3d(sim, width=800, height=800) -> None:
     """Make 3D display of simulation in ipyython notebook."""
 
     try:
         # pylint:disable=import-outside-toplevel
         from IPython.display import display, HTML
     except ImportError as e:
         raise SetupError(
@@ -254,14 +254,14 @@
     );
     """
     viewer_url = (
         "https://feature-simulation-viewer.d3a9gfg7glllfq.amplifyapp.com/simulation-viewer?uuid="
         + str(uuid)
     )
     html_code = f"""
-    <iframe id="simulation-viewer{uuid}" src={viewer_url} width="800" height="800"></iframe>
+    <iframe id="simulation-viewer{uuid}" src={viewer_url} width="{width}" height="{height}" allowfullscreen="true"></iframe>
     <script>
         {js_code}
     </script>
     """
 
     return display(HTML(html_code))
```

### Comparing `tidy3d-2.3.2/tidy3d/config.py` & `tidy3d-2.4.0rc1/tidy3d/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Sets the configuration of the script, can be changed with `td.config.config_name = new_val`."""
 
 import pydantic as pd
 
-from .log import DEFAULT_LEVEL, LogLevel, set_logging_level
+from .log import DEFAULT_LEVEL, LogLevel, set_logging_level, set_log_suppression
 
 
 class Tidy3dConfig(pd.BaseModel):
     """configuration of tidy3d"""
 
     class Config:
         """Config of the config."""
@@ -21,16 +21,29 @@
     logging_level: LogLevel = pd.Field(
         DEFAULT_LEVEL,
         title="Logging Level",
         description="The lowest level of logging output that will be displayed. "
         'Can be "DEBUG", "INFO", "WARNING", "ERROR", or "CRITICAL".',
     )
 
+    log_suppression: bool = pd.Field(
+        True,
+        title="Log suppression",
+        description="Enable or disable suppression of certain log messages when they are repeated "
+        "for several elements.",
+    )
+
     @pd.validator("logging_level", pre=True, always=True)
     def _set_logging_level(cls, val):
         """Set the logging level if logging_level is changed."""
         set_logging_level(val)
         return val
 
+    @pd.validator("log_suppression", pre=True, always=True)
+    def _set_log_suppression(cls, val):
+        """Control log suppression when log_suppression is changed."""
+        set_log_suppression(val)
+        return val
+
 
 # instance of the config that can be modified.
 config = Tidy3dConfig()
```

### Comparing `tidy3d-2.3.2/tidy3d/constants.py` & `tidy3d-2.4.0rc1/tidy3d/constants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/exceptions.py` & `tidy3d-2.4.0rc1/tidy3d/exceptions.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/log.py` & `tidy3d-2.4.0rc1/tidy3d/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     messages can then be recovered through 'captured_warnings'.
     """
 
     _static_cache = set()
 
     def __init__(self):
         self.handlers = {}
+        self.suppression = True
         self._counts = None
         self._stack = None
         self._capture = False
         self._captured_warnings = []
 
     def set_capture(self, capture: bool):
         """Turn on/off tree-like capturing of log messages."""
@@ -100,16 +101,17 @@
     def captured_warnings(self):
         """Get the formatted list of captured log messages."""
         captured_warnings = self._captured_warnings
         self._captured_warnings = []
         return captured_warnings
 
     def __enter__(self):
-        """Enter a consolidation context (only a single message is emitted)."""
-        if self._counts is None:
+        """If suppression is enables, enter a consolidation context (only a single message is
+        emitted)."""
+        if self.suppression and self._counts is None:
             self._counts = {}
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         """Exist a consolidation context (report the number of messages discarded)."""
         if self._counts is not None:
             total = sum(v for v in self._counts.values())
@@ -279,14 +281,19 @@
         The lowest priority level of logging messages to display. One of ``{'DEBUG', 'INFO',
         'WARNING', 'ERROR', 'CRITICAL'}`` (listed in increasing priority).
     """
     if "console" in log.handlers:
         log.handlers["console"].level = _get_level_int(level)
 
 
+def set_log_suppression(value: bool) -> None:
+    """Control log suppression for repeated messages."""
+    log.suppression = value
+
+
 def set_logging_console(stderr: bool = False) -> None:
     """Set stdout or stderr as console output
 
     Parameters
     ----------
     stderr : bool
         If False, logs are directed to stdout, otherwise to stderr.
```

### Comparing `tidy3d-2.3.2/tidy3d/material_library/material_library.py` & `tidy3d-2.4.0rc1/tidy3d/material_library/material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/material_library/material_reference.py` & `tidy3d-2.4.0rc1/tidy3d/material_library/material_reference.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/material_library/parametric_materials.py` & `tidy3d-2.4.0rc1/tidy3d/material_library/parametric_materials.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/adjoint/__init__.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/base.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/data_array.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/dataset.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/monitor_data.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/data/sim_data.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/geometry.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/medium.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/simulation.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/structure.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/adjoint/components/types.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/adjoint/web.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/adjoint/web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/dispersion/fit.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/dispersion/fit.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/dispersion/web.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/dispersion/web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/mode/derivatives.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/mode/derivatives.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/mode/mode_solver.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/mode/mode_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -575,14 +575,97 @@
             center=self.plane.center,
             mode_spec=self.mode_spec,
             freqs=self.freqs,
             direction=self.direction,
             name=name,
         )
 
+    def sim_with_source(
+        self,
+        source_time: SourceTime,
+        direction: Direction,
+        mode_index: pydantic.NonNegativeInt = 0,
+    ) -> Simulation:
+        """Creates :class:`Simulation` from a :class:`ModeSolver`. Creates a copy of
+        the ModeSolver's original simulation with a ModeSource added corresponding to
+        the ModeSolver parameters.
+
+        Parameters
+        ----------
+        source_time: :class:`.SourceTime`
+            Specification of the source time-dependence.
+        direction : Direction
+            Whether source will inject in ``"+"`` or ``"-"`` direction relative to plane normal.
+        mode_index : int = 0
+            Index into the list of modes returned by mode solver to use in source.
+
+        Returns
+        -------
+        :class:`.Simulation`
+            Copy of the simulation with a :class:`.ModeSource` with specifications taken
+            from the ModeSolver instance and the method inputs.
+        """
+        mode_source = self.to_source(
+            mode_index=mode_index, direction=direction, source_time=source_time
+        )
+        new_sources = list(self.simulation.sources) + [mode_source]
+        new_sim = self.simulation.updated_copy(sources=new_sources)
+        return new_sim
+
+    def sim_with_monitor(
+        self,
+        freqs: List[float],
+        name: str,
+    ) -> Simulation:
+        """Creates :class:`.Simulation` from a :class:`ModeSolver`. Creates a copy of
+        the ModeSolver's original simulation with a mode monitor added corresponding to
+        the ModeSolver parameters.
+
+        Parameters
+        ----------
+        freqs : List[float]
+            Frequencies to include in Monitor (Hz).
+        name : str
+            Required name of monitor.
+
+        Returns
+        -------
+        :class:`.Simulation`
+            Copy of the simulation with a :class:`.ModeMonitor` with specifications taken
+            from the ModeSolver instance and the method inputs.
+        """
+        mode_monitor = self.to_monitor(freqs=freqs, name=name)
+        new_monitors = list(self.simulation.monitors) + [mode_monitor]
+        new_sim = self.simulation.updated_copy(monitors=new_monitors)
+        return new_sim
+
+    def sim_with_mode_solver_monitor(
+        self,
+        name: str,
+    ) -> Simulation:
+        """Creates :class:`Simulation` from a :class:`ModeSolver`. Creates a
+        copy of the ModeSolver's original simulation with a mode solver monitor
+        added corresponding to the ModeSolver parameters.
+
+        Parameters
+        ----------
+        name : str
+            Name of the monitor.
+
+        Returns
+        -------
+        :class:`.Simulation`
+            Copy of the simulation with a :class:`.ModeSolverMonitor` with specifications taken
+            from the ModeSolver instance and ``name``.
+        """
+        mode_solver_monitor = self.to_mode_solver_monitor(name=name)
+        new_monitors = list(self.simulation.monitors) + [mode_solver_monitor]
+        new_sim = self.simulation.updated_copy(monitors=new_monitors)
+        return new_sim
+
     # pylint:disable=too-many-arguments
     def plot_field(
         self,
         field_name: str,
         val: Literal["real", "imag", "abs"] = "real",
         scale: PlotScale = "lin",
         eps_alpha: float = 0.2,
```

### Comparing `tidy3d-2.3.2/tidy3d/plugins/mode/solver.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/mode/solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/mode/transforms.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/mode/transforms.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/mode/web.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/mode/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,14 +327,20 @@
     def delete(self):
         """Delete the mode solver and its corresponding task from the server."""
         # Delete mode solver
         http.delete(f"{MODESOLVER_API}/{self.task_id}/{self.solver_id}")
         # Delete parent task
         http.delete(f"tidy3d/tasks/{self.task_id}")
 
+    def abort(self):
+        """Abort the mode solver and its corresponding task from the server."""
+        return http.put(
+            "tidy3d/tasks/abort", json={"taskType": "MODE_SOLVER", "taskId": self.solver_id}
+        )
+
     def get_modesolver(
         self,
         to_file: str = "mode_solver.json",
         sim_file: str = "simulation.json",
         verbose: bool = True,
         progress_callback: Callable[[float], None] = None,
     ) -> ModeSolver:
```

### Comparing `tidy3d-2.3.2/tidy3d/plugins/polyslab/polyslab.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/polyslab/polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/resonance/resonance.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/resonance/resonance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/plugins/smatrix/smatrix.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/smatrix/smatrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from typing import List, Tuple, Optional, Dict
 import os
 
 import pydantic as pd
 import numpy as np
 
-from ...constants import HERTZ, C_0
+from ...constants import HERTZ
 from ...components.simulation import Simulation
 from ...components.geometry import Box
 from ...components.mode import ModeSpec
 from ...components.monitor import ModeMonitor
 from ...components.source import ModeSource, GaussianPulse
 from ...components.data.sim_data import SimulationData
 from ...components.data.data_array import DataArray
@@ -364,22 +364,17 @@
         port_monitor_data = sim_data[port_source.name]
         mode_index = sim_data.simulation.sources[0].mode_index
 
         normalize_amps = port_monitor_data.amps.sel(
             f=self.freqs,
             direction=port_source.direction,
             mode_index=mode_index,
-        ).values
-
-        normalize_n_eff = port_monitor_data.n_eff.sel(f=self.freqs, mode_index=mode_index).values
+        )
 
-        k0s = 2 * np.pi * C_0 / np.array(self.freqs)
-        k_effs = k0s * normalize_n_eff
-        shift_value = self._shift_value_signed(port=port_source)
-        return normalize_amps * np.exp(1j * k_effs * shift_value)
+        return normalize_amps.values
 
     @cached_property
     def max_mode_index(self) -> Tuple[int, int]:
         """maximum mode indices for the smatrix dataset for the in and out ports, respectively."""
 
         def get_max_mode_indices(matrix_elements: Tuple[str, int]) -> int:
             """Get the maximum mode index for a list of (port name, mode index)."""
```

### Comparing `tidy3d-2.3.2/tidy3d/plugins/waveguide/rectangular_dielectric.py` & `tidy3d-2.4.0rc1/tidy3d/plugins/waveguide/rectangular_dielectric.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/updater.py` & `tidy3d-2.4.0rc1/tidy3d/updater.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/web/asynchronous.py` & `tidy3d-2.4.0rc1/tidy3d/web/asynchronous.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/web/cacert.pem` & `tidy3d-2.4.0rc1/tidy3d/web/cacert.pem`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/web/cli/app.py` & `tidy3d-2.4.0rc1/tidy3d/web/cli/app.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/web/cli/migrate.py` & `tidy3d-2.4.0rc1/tidy3d/web/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/web/container.py` & `tidy3d-2.4.0rc1/tidy3d/web/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,14 @@
         # the type of job to upload (to generalize to subclasses)
         JobType = cls.__fields__["jobs"].type_  # pylint:disable=invalid-name
         parent_tasks = values.get("parent_tasks")
 
         verbose = bool(values.get("verbose"))
         jobs = {}
         for task_name, simulation in values.get("simulations").items():
-
             # pylint:disable=protected-access
             upload_kwargs = {key: values.get(key) for key in JobType._upload_fields}
             upload_kwargs["task_name"] = task_name
             upload_kwargs["simulation"] = simulation
             upload_kwargs["verbose"] = verbose
             if parent_tasks and task_name in parent_tasks:
                 upload_kwargs["parent_tasks"] = parent_tasks[task_name]
@@ -481,15 +480,14 @@
                 console.log(
                     f"Maximum FlexCredit cost: {est_flex_unit:1.3f} for the whole batch. "
                     "Use 'Batch.real_cost()' to "
                     "get the billed FlexCredit cost after the Batch has completed."
                 )
 
             with Progress(console=console) as progress:
-
                 # create progressbars
                 pbar_tasks = {}
                 for task_name, job in self.jobs.items():
                     status = job.status
                     description = pbar_description(task_name, status)
                     pbar = progress.add_task(description, total=len(run_statuses) - 1)
                     pbar_tasks[task_name] = pbar
@@ -612,15 +610,14 @@
 
         if self.jobs is None:
             raise DataError("Can't load batch results, hasn't been uploaded.")
 
         task_paths = {}
         task_ids = {}
         for task_name, job in self.jobs.items():
-
             if "error" in job.status:
                 log.warning(f"Not loading '{task_name}' as the task errored.")
                 continue
 
             task_paths[task_name] = self._job_data_path(task_id=job.task_id, path_dir=path_dir)
             task_ids[task_name] = self.jobs[task_name].task_id
```

### Comparing `tidy3d-2.3.2/tidy3d/web/environment.py` & `tidy3d-2.4.0rc1/tidy3d/web/environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Environment Setup."""
 import os
 
 from pydantic import BaseSettings, Field
 
+from tidy3d import log
+
 
 class EnvironmentConfig(BaseSettings):
     """Basic Configuration for definition environment."""
 
     def __hash__(self):
         return hash((type(self),) + tuple(self.__dict__.values()))
 
@@ -63,23 +65,35 @@
 
     Example
     -------
     >>> Env.dev.active()
     >>> Env.current.name == "dev"
     """
 
+    env_map = dict(
+        dev=dev,
+        uat=uat,
+        prod=prod,
+    )
+
     def __init__(self):
         """Initialize the environment."""
         env_key = os.environ.get("TIDY3D_ENV")
-        if env_key is None:
+        env_key = env_key.lower() if env_key else env_key
+        log.info(f"env_key is {env_key}")
+        if not env_key:
+            self._current = prod
+        elif env_key in self.env_map:
+            self._current = self.env_map[env_key]
+        else:
+            log.warning(
+                f"The value '{env_key}' for the environment variable TIDY3D_ENV is not supported. "
+                f"Using prod as default."
+            )
             self._current = prod
-        elif env_key == "dev":
-            self._current = dev
-        elif env_key == "uat":
-            self._current = uat
 
     @property
     def current(self) -> EnvironmentConfig:
         """Get the current environment.
 
         Returns
         -------
```

### Comparing `tidy3d-2.3.2/tidy3d/web/http_management.py` & `tidy3d-2.4.0rc1/tidy3d/web/http_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         """Create the resource."""
         return self.session.post(Env.current.get_real_url(path), json=json, auth=api_key_auth)
 
     @http_interceptor
     def put(self, path: str, json=None, files=None):
         """Update the resource."""
         return self.session.put(
-            Env.current.get_real_url(path), data=json, auth=api_key_auth, files=files
+            Env.current.get_real_url(path), json=json, auth=api_key_auth, files=files
         )
 
     @http_interceptor
     def delete(self, path: str):
         """Delete the resource."""
         return self.session.delete(Env.current.get_real_url(path), auth=api_key_auth)
```

### Comparing `tidy3d-2.3.2/tidy3d/web/httputils.py` & `tidy3d-2.4.0rc1/tidy3d/web/httputils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/web/material_fitter.py` & `tidy3d-2.4.0rc1/tidy3d/web/material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/web/material_libray.py` & `tidy3d-2.4.0rc1/tidy3d/web/material_libray.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/web/s3utils.py` & `tidy3d-2.4.0rc1/tidy3d/web/s3utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/web/simulation_task.py` & `tidy3d-2.4.0rc1/tidy3d/web/simulation_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,7 +533,13 @@
         return download_file(
             self.task_id,
             SIM_LOG_FILE,
             to_file=to_file,
             verbose=verbose,
             progress_callback=progress_callback,
         )
+
+    def abort(self):
+        """Abort current task from server."""
+        if not self.task_id:
+            raise ValueError("Task id not found.")
+        return http.put("tidy3d/tasks/abort", json={"taskType": "FDTD", "taskId": self.task_id})
```

### Comparing `tidy3d-2.3.2/tidy3d/web/task.py` & `tidy3d-2.4.0rc1/tidy3d/web/task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/web/types.py` & `tidy3d-2.4.0rc1/tidy3d/web/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.2/tidy3d/web/webapi.py` & `tidy3d-2.4.0rc1/tidy3d/web/webapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
     ----
     To load results when finished, may call :meth:`load`.
     """
 
     task_info = get_info(task_id)
     task_name = task_info.taskName
 
-    break_statuses = ("success", "error", "diverged", "deleted", "draft")
+    break_statuses = ("success", "error", "diverged", "deleted", "draft", "abort")
 
     console = Console() if verbose else None
 
     def get_estimated_cost() -> float:
         """Get estimated cost, if None, is not ready."""
         task_info = get_info(task_id)
         block_info = task_info.taskBlockInfo
@@ -380,23 +380,22 @@
 
     # while running but before the percentage done is available, keep waiting
     while get_run_info(task_id)[0] is None and get_status(task_id) == "running":
         time.sleep(REFRESH_TIME)
 
     # while running but percentage done is available
     if verbose:
-
         # verbose case, update progressbar
         console.log("running solver")
         console.log(
-            "To cancel the simulation, use 'web.delete(task_id)' or delete the task in the web"
+            "To cancel the simulation, use 'web.abort(task_id)' or 'web.delete(task_id)' "
+            "or abort/delete the task in the web"
             " UI. Terminating the Python script will not stop the job running on the cloud."
         )
         with Progress(console=console) as progress:
-
             pbar_pd = progress.add_task("% done", total=100)
             perc_done, _ = get_run_info(task_id)
 
             while perc_done is not None and perc_done < 100 and get_status(task_id) == "running":
                 perc_done, field_decay = get_run_info(task_id)
                 new_description = f"solver progress (field decay = {field_decay:.2e})"
                 progress.update(pbar_pd, completed=perc_done, description=new_description)
@@ -405,24 +404,22 @@
             perc_done, field_decay = get_run_info(task_id)
             if perc_done is not None and perc_done < 100 and field_decay > 0:
                 console.log("early shutoff detected, exiting.")
 
             progress.update(pbar_pd, completed=100, refresh=True)
 
     else:
-
         # non-verbose case, just keep checking until status is not running or perc_done >= 100
         perc_done, _ = get_run_info(task_id)
         while perc_done is not None and perc_done < 100 and get_status(task_id) == "running":
             perc_done, field_decay = get_run_info(task_id)
             time.sleep(1.0)
 
     # post processing
     if verbose:
-
         status = get_status(task_id)
         if status != "running":
             console.log(f"status = {status}")
 
         with console.status(f"[bold green]Finishing '{task_name}'...", spinner="runner"):
             while status not in break_statuses:
                 new_status = get_status(task_id)
@@ -673,14 +670,35 @@
         filter(lambda t: t.created_at < datetime.now(pytz.utc) - timedelta(days=days_old), tasks)
     )
     for task in tasks:
         task.delete()
     return len(tasks)
 
 
+@wait_for_connection
+def abort(task_id: TaskId) -> TaskInfo:
+    """Abort server-side data associated with task.
+
+    Parameters
+    ----------
+    task_id : str
+        Unique identifier of task on server.  Returned by :meth:`upload`.
+
+    Returns
+    -------
+    TaskInfo
+        Object containing information about status, size, credits of task.
+    """
+
+    # task = SimulationTask.get(task_id)
+    task = SimulationTask(taskId=task_id)
+    task.abort()
+    return TaskInfo(**{"taskId": task.task_id, **task.dict()})
+
+
 # TODO: make this return a list of TaskInfo instead?
 @wait_for_connection
 def get_tasks(
     num_tasks: int = None, order: Literal["new", "old"] = "new", folder: str = "default"
 ) -> List[Dict]:
     """Get a list with the metadata of the last ``num_tasks`` tasks.
```

### Comparing `tidy3d-2.3.2/tidy3d.egg-info/PKG-INFO` & `tidy3d-2.4.0rc1/tidy3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.3.2
+Version: 2.4.0rc1
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.3.2/tidy3d.egg-info/SOURCES.txt` & `tidy3d-2.4.0rc1/tidy3d.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,20 @@
 tidy3d/plugins/adjoint/components/structure.py
 tidy3d/plugins/adjoint/components/types.py
 tidy3d/plugins/adjoint/components/data/__init__.py
 tidy3d/plugins/adjoint/components/data/data_array.py
 tidy3d/plugins/adjoint/components/data/dataset.py
 tidy3d/plugins/adjoint/components/data/monitor_data.py
 tidy3d/plugins/adjoint/components/data/sim_data.py
+tidy3d/plugins/adjoint/utils/__init__.py
+tidy3d/plugins/adjoint/utils/filter.py
+tidy3d/plugins/adjoint/utils/penalty.py
 tidy3d/plugins/dispersion/__init__.py
 tidy3d/plugins/dispersion/fit.py
+tidy3d/plugins/dispersion/fit_fast.py
 tidy3d/plugins/dispersion/fit_web.py
 tidy3d/plugins/dispersion/web.py
 tidy3d/plugins/mode/__init__.py
 tidy3d/plugins/mode/derivatives.py
 tidy3d/plugins/mode/mode_solver.py
 tidy3d/plugins/mode/solver.py
 tidy3d/plugins/mode/transforms.py
```

### Comparing `tidy3d-2.3.2/tidy3d.egg-info/requires.txt` & `tidy3d-2.4.0rc1/tidy3d.egg-info/requires.txt`

 * *Files identical despite different names*

