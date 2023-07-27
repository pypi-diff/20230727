# Comparing `tmp/pytao-0.2.4.tar.gz` & `tmp/pytao-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pytao/pytao/dist/.tmp-wkqdkud6/pytao-0.2.4.tar", last modified: Sat Jul  1 21:42:57 2023, max compression
+gzip compressed data, was "/home/runner/work/pytao/pytao/dist/.tmp-ybogoc5a/pytao-0.2.5.tar", last modified: Thu Jul 27 18:45:07 2023, max compression
```

## Comparing `pytao-0.2.4.tar` & `pytao-0.2.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 21:42:46.000000 pytao-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-01 21:42:46.000000 pytao-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-01 21:42:57.000000 pytao-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-01 21:42:46.000000 pytao-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/data_type_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    34616 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/module_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    63664 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_base_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_beam_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    50559 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_data_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_ele_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    62214 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_lat_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_misc_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_mpl_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_plot_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    95292 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_plot_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    40433 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_var_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)    42615 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    65690 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/taoplot.py
--rw-r--r--   0 runner    (1001) docker     (123)   114650 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/interface_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/misc/csr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/misc/csr_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/misc/markers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/tao_ctypes/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_ctypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_ctypes/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_ctypes/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_ctypes/extra_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_ctypes/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_ctypes/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/tao_pexpect/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_pexpect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_pexpect/tao_pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    28283 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tests/test_interface_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/util/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/util/evaluate_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/util/lattice_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/util/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/util/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 21:42:46.000000 pytao-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-01 21:42:57.000000 pytao-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-01 21:42:46.000000 pytao-0.2.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-07-01 21:42:46.000000 pytao-0.2.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-27 18:44:56.000000 pytao-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-27 18:44:56.000000 pytao-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-27 18:45:07.000000 pytao-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-27 18:44:56.000000 pytao-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/data_type_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34616 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/module_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63664 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_base_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_beam_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50559 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_data_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_ele_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62214 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_lat_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_misc_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_mpl_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_plot_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95292 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_plot_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40433 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_var_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42615 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/tao_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65690 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/gui/taoplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114650 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/interface_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/misc/csr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/misc/csr_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/misc/markers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/tao_ctypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_ctypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17716 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_ctypes/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_ctypes/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_ctypes/extra_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_ctypes/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_ctypes/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/tao_pexpect/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_pexpect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tao_pexpect/tao_pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28283 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/tests/test_interface_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/util/evaluate_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/util/lattice_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/util/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-27 18:44:56.000000 pytao-0.2.5/pytao/util/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 18:45:07.000000 pytao-0.2.5/pytao.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 18:44:56.000000 pytao-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-27 18:45:07.000000 pytao-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-27 18:44:56.000000 pytao-0.2.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-07-27 18:44:56.000000 pytao-0.2.5/versioneer.py
```

### Comparing `pytao-0.2.4/LICENSE` & `pytao-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/PKG-INFO` & `pytao-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytao
-Version: 0.2.4
+Version: 0.2.5
 Home-page: https://www.classe.cornell.edu/bmad/tao.html
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyTao
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytao Version: 0.2.4 Home-page: https://
+Metadata-Version: 2.1 Name: pytao Version: 0.2.5 Home-page: https://
 www.classe.cornell.edu/bmad/tao.html Requires-Python: >=3.6 Description-
 Content-Type: text/markdown License-File: LICENSE # PyTao [PyTao]((https://
 bmad-sim.github.io/pytao/index.html)) is Python interface for [Tao](https://
 www.classe.cornell.edu/bmad/tao.html), which is based on the Bmad subroutine
 library for relativistic chargedâparticle and X-ray simulations in
 accelerators and storage rings. Documentation for Bmad and Tao, as well as
 information for downloading the code if needed is given on the [Bmad website]
```

### Comparing `pytao-0.2.4/README.md` & `pytao-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/__init__.py` & `pytao-0.2.5/pytao/__init__.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/__init__.py` & `pytao-0.2.5/pytao/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/data_type_list.py` & `pytao-0.2.5/pytao/gui/data_type_list.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/main.py` & `pytao-0.2.5/pytao/gui/main.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/module_check.py` & `pytao-0.2.5/pytao/gui/module_check.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/tao_base_windows.py` & `pytao-0.2.5/pytao/gui/tao_base_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/tao_beam_windows.py` & `pytao-0.2.5/pytao/gui/tao_beam_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/tao_console.py` & `pytao-0.2.5/pytao/gui/tao_console.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/tao_data_windows.py` & `pytao-0.2.5/pytao/gui/tao_data_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/tao_ele_location.py` & `pytao-0.2.5/pytao/gui/tao_ele_location.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/tao_interface.py` & `pytao-0.2.5/pytao/gui/tao_interface.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/tao_lat_windows.py` & `pytao-0.2.5/pytao/gui/tao_lat_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/tao_misc_windows.py` & `pytao-0.2.5/pytao/gui/tao_misc_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/tao_mpl_toolbar.py` & `pytao-0.2.5/pytao/gui/tao_mpl_toolbar.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/tao_plot_dict.py` & `pytao-0.2.5/pytao/gui/tao_plot_dict.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/tao_plot_windows.py` & `pytao-0.2.5/pytao/gui/tao_plot_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/tao_set.py` & `pytao-0.2.5/pytao/gui/tao_set.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/tao_var_windows.py` & `pytao-0.2.5/pytao/gui/tao_var_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/tao_widget.py` & `pytao-0.2.5/pytao/gui/tao_widget.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/gui/taoplot.py` & `pytao-0.2.5/pytao/gui/taoplot.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/interface_commands.py` & `pytao-0.2.5/pytao/interface_commands.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/misc/csr.py` & `pytao-0.2.5/pytao/misc/csr.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/misc/csr_plot.py` & `pytao-0.2.5/pytao/misc/csr_plot.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/misc/markers.py` & `pytao-0.2.5/pytao/misc/markers.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/tao_ctypes/core.py` & `pytao-0.2.5/pytao/tao_ctypes/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,18 @@
     # Only python commands that load the real array buffer can be used with this method.
 
     def cmd_real (self, cmd, raises=True):
         logger.debug(f'Tao> {cmd}')
         
         self.so_lib.tao_c_command(cmd.encode('utf-8'))
         n = self.so_lib.tao_c_real_array_size()
+        # Empty array
+        if n == 0:
+            return np.array([], dtype=float)     
+            
         self.so_lib.tao_c_get_real_array.restype = ctypes.POINTER(ctypes.c_double * n)
 
         # Check the output for errors
         lines = self.get_output(reset=False)
         err = error_in_lines(lines)
         if err:
             self.reset_output()
@@ -245,14 +249,18 @@
     # Only python commands that load the integer array buffer can be used with this method.
 
     def cmd_integer (self, cmd, raises=True):
         logger.debug(f'Tao> {cmd}')
         
         self.so_lib.tao_c_command(cmd.encode('utf-8'))
         n = self.so_lib.tao_c_integer_array_size()
+        # Empty array
+        if n == 0:
+            return np.array([], dtype=int)
+
         self.so_lib.tao_c_get_integer_array.restype = ctypes.POINTER(ctypes.c_int * n)
 
         # Check the output for errors
         lines = self.get_output(reset=False)
         err = error_in_lines(lines)
         if err:
             self.reset_output()
```

### Comparing `pytao-0.2.4/pytao/tao_ctypes/evaluate.py` & `pytao-0.2.5/pytao/tao_ctypes/evaluate.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/tao_ctypes/extra_commands.py` & `pytao-0.2.5/pytao/tao_ctypes/extra_commands.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/tao_ctypes/tools.py` & `pytao-0.2.5/pytao/tao_ctypes/tools.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/tao_ctypes/util.py` & `pytao-0.2.5/pytao/tao_ctypes/util.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/tao_interface.py` & `pytao-0.2.5/pytao/tao_interface.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/tao_pexpect/tao_pipe.py` & `pytao-0.2.5/pytao/tao_pexpect/tao_pipe.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/tests/test_interface_commands.py` & `pytao-0.2.5/pytao/tests/test_interface_commands.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/util/data.py` & `pytao-0.2.5/pytao/util/data.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/util/evaluate_expression.py` & `pytao-0.2.5/pytao/util/evaluate_expression.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/util/lattice_element.py` & `pytao-0.2.5/pytao/util/lattice_element.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/util/parameters.py` & `pytao-0.2.5/pytao/util/parameters.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao/util/parsers.py` & `pytao-0.2.5/pytao/util/parsers.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/pytao.egg-info/PKG-INFO` & `pytao-0.2.5/pytao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytao
-Version: 0.2.4
+Version: 0.2.5
 Home-page: https://www.classe.cornell.edu/bmad/tao.html
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyTao
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytao Version: 0.2.4 Home-page: https://
+Metadata-Version: 2.1 Name: pytao Version: 0.2.5 Home-page: https://
 www.classe.cornell.edu/bmad/tao.html Requires-Python: >=3.6 Description-
 Content-Type: text/markdown License-File: LICENSE # PyTao [PyTao]((https://
 bmad-sim.github.io/pytao/index.html)) is Python interface for [Tao](https://
 www.classe.cornell.edu/bmad/tao.html), which is based on the Bmad subroutine
 library for relativistic chargedâparticle and X-ray simulations in
 accelerators and storage rings. Documentation for Bmad and Tao, as well as
 information for downloading the code if needed is given on the [Bmad website]
```

### Comparing `pytao-0.2.4/pytao.egg-info/SOURCES.txt` & `pytao-0.2.5/pytao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/setup.py` & `pytao-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.4/versioneer.py` & `pytao-0.2.5/versioneer.py`

 * *Files identical despite different names*

