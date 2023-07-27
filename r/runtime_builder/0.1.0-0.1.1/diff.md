# Comparing `tmp/runtime_builder-0.1.0.tar.gz` & `tmp/runtime_builder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtime_builder-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "runtime_builder-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `runtime_builder-0.1.0.tar` & `runtime_builder-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,25 @@
--rw-r--r--   0        0        0      556 2023-07-19 23:43:07.686633 runtime_builder-0.1.0/LICENSE
--rw-r--r--   0        0        0     4490 2023-07-19 23:43:12.156140 runtime_builder-0.1.0/README.md
--rw-r--r--   0        0        0      289 2023-07-19 23:43:12.156516 runtime_builder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1875 2023-07-19 23:10:51.010627 runtime_builder-0.1.0/runtime_builder.py
--rw-r--r--   0        0        0      111 2023-07-19 23:43:07.687063 runtime_builder-0.1.0/setup.py
--rw-r--r--   0        0        0       44 2023-07-19 23:43:23.003856 runtime_builder-0.1.0/tests/project_template/README.md
--rw-r--r--   0        0        0     1095 2023-07-19 23:43:23.004181 runtime_builder-0.1.0/tests/project_template/SConstruct
--rw-r--r--   0        0        0        6 2023-07-19 23:43:23.004477 runtime_builder-0.1.0/tests/project_template/proj/bar.source
--rw-r--r--   0        0        0        2 2023-07-19 23:43:23.004695 runtime_builder-0.1.0/tests/project_template/proj/foo.source
--rw-r--r--   0        0        0      744 2023-07-19 23:43:23.004842 runtime_builder-0.1.0/tests/project_template/proj/run_test.py
--rw-r--r--   0        0        0      701 2023-07-19 23:43:23.004985 runtime_builder-0.1.0/tests/project_template/proj/runtime_build
--rw-r--r--   0        0        0      294 2023-07-19 23:43:23.005138 runtime_builder-0.1.0/tests/project_template/pyproject.toml.template
--rwxr-xr-x   0        0        0      283 2023-07-19 23:43:23.005375 runtime_builder-0.1.0/tests/project_template/test_pip_install.sh
--rwxr-xr-x   0        0        0      467 2023-07-19 23:43:23.005614 runtime_builder-0.1.0/tests/project_template/test_pip_install_editable.sh
--rw-r--r--   0        0        0      791 2023-07-19 23:43:23.005771 runtime_builder-0.1.0/tests/test_builder.py
--rw-r--r--   0        0        0     4685 1970-01-01 00:00:00.000000 runtime_builder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      556 2023-07-27 05:46:10.422941 runtime_builder-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5001 2023-07-27 05:46:10.423075 runtime_builder-0.1.1/README.md
+-rw-r--r--   0        0        0      289 2023-07-27 05:46:10.423161 runtime_builder-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3893 2023-07-27 05:46:10.423256 runtime_builder-0.1.1/runtime_builder.py
+-rw-r--r--   0        0        0      111 2023-07-27 05:46:10.423457 runtime_builder-0.1.1/setup.py
+-rw-r--r--   0        0        0       44 2023-07-27 05:46:10.423619 runtime_builder-0.1.1/tests/project_template_enscons/README.md
+-rw-r--r--   0        0        0     1095 2023-07-27 05:46:10.423715 runtime_builder-0.1.1/tests/project_template_enscons/SConstruct
+-rw-r--r--   0        0        0        6 2023-07-27 05:46:10.423827 runtime_builder-0.1.1/tests/project_template_enscons/proj/bar.source
+-rw-r--r--   0        0        0        2 2023-07-27 05:46:10.423906 runtime_builder-0.1.1/tests/project_template_enscons/proj/foo.source
+-rw-r--r--   0        0        0      744 2023-07-27 05:46:10.423988 runtime_builder-0.1.1/tests/project_template_enscons/proj/run_test.py
+-rw-r--r--   0        0        0      701 2023-07-27 05:46:10.424066 runtime_builder-0.1.1/tests/project_template_enscons/proj/runtime_build
+-rw-r--r--   0        0        0      277 2023-07-27 05:46:10.424151 runtime_builder-0.1.1/tests/project_template_enscons/pyproject.toml.template
+-rwxr-xr-x   0        0        0      283 2023-07-27 05:46:10.424229 runtime_builder-0.1.1/tests/project_template_enscons/test_pip_install.sh
+-rwxr-xr-x   0        0        0      467 2023-07-27 05:46:10.424318 runtime_builder-0.1.1/tests/project_template_enscons/test_pip_install_editable.sh
+-rw-r--r--   0        0        0       63 2023-07-27 05:46:10.424438 runtime_builder-0.1.1/tests/project_template_setuptools/README.md
+-rw-r--r--   0        0        0        6 2023-07-27 05:46:10.424535 runtime_builder-0.1.1/tests/project_template_setuptools/proj/bar.source
+-rw-r--r--   0        0        0        2 2023-07-27 05:46:10.424605 runtime_builder-0.1.1/tests/project_template_setuptools/proj/foo.source
+-rw-r--r--   0        0        0      744 2023-07-27 05:46:10.424680 runtime_builder-0.1.1/tests/project_template_setuptools/proj/run_test.py
+-rw-r--r--   0        0        0      701 2023-07-27 05:46:10.424761 runtime_builder-0.1.1/tests/project_template_setuptools/proj/runtime_build
+-rw-r--r--   0        0        0      288 2023-07-27 05:46:10.424842 runtime_builder-0.1.1/tests/project_template_setuptools/pyproject.toml.template
+-rwxr-xr-x   0        0        0      308 2023-07-27 05:46:10.424918 runtime_builder-0.1.1/tests/project_template_setuptools/setup.py
+-rwxr-xr-x   0        0        0      283 2023-07-27 05:46:10.425002 runtime_builder-0.1.1/tests/project_template_setuptools/test_pip_install.sh
+-rwxr-xr-x   0        0        0      441 2023-07-27 05:46:10.425082 runtime_builder-0.1.1/tests/project_template_setuptools/test_pip_install_editable.sh
+-rw-r--r--   0        0        0     1140 2023-07-27 05:46:10.425163 runtime_builder-0.1.1/tests/test_builder.py
+-rw-r--r--   0        0        0     5196 1970-01-01 00:00:00.000000 runtime_builder-0.1.1/PKG-INFO
```

### Comparing `runtime_builder-0.1.0/LICENSE` & `runtime_builder-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `runtime_builder-0.1.0/README.md` & `runtime_builder-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,29 +4,45 @@
 
 When building the wheel, the blobs need to be generated. But it may also be nice to rebuild the blobs if the source have changed at runtime to automate a step of the edit/test cycle.
 
 This project lets you declare a single configuration describing how to build the artifacts, and build them at runtime during the development cycle or at wheel build time.
 
 ## Example
 
-There is an example project in `tests/project_template`.
+There are example projects in `tests/project_template_enscons` and `tests/project_template_setuptools`.
 
-project_template
+tests/project_template_setuptools
+├── README.md
+├── proj
+│   ├── bar.source
+│   ├── foo.source
+│   ├── run_test.py
+│   └── runtime_build
+├── pyproject.toml.template
+├── setup.py
+├── test_pip_install.sh
+└── test_pip_install_editable.sh
+
+This examples uses `setuptools` and `setup.py` to build. The `setup.py` and `runtime_build` files work together to make available artifacts built from the `.source` files.
+
+
+project_template_enscons
 ├── README.md
 ├── SConstruct
 ├── proj
 │   ├── bar.source
 │   ├── foo.source
 │   ├── run_test.py
 │   └── runtime_build
 ├── pyproject.toml.template
 ├── test_pip_install.sh
 └── test_pip_install_editable.sh
 
-Note that it uses `enscons` to build, as the more commonly used `setuptools` does not easily allow fine-grained control of the contents of the `sdist` and `wheel` files. In particular, this example takes pains to include the source files `runtime_build`, `foo.source`, `bar.source` and `program.source` in the sdist but not the wheel.
+Note that this example uses `enscons` to build, as `setuptools` does not easily allow fine-grained control of the contents of the `sdist` and `wheel` files. In particular, this example takes pains to include the source files `runtime_build`, `foo.source` and `bar.source` in the sdist but not the wheel.
+
 
 ### Configuration
 
 Artifacts to be build must be declared in a `runtime_build` file located in the destination module of the artifacts. Each submodule can have zero or one of these build files. In the `project_template` example above, `bar.source` and `foo.source` each produce an output in the `proj` submodule, and `runtime_build` defines what the artifacts are.
 
 This configuration file can be loaded at build time or at run time, so it *cannot* import anything that isn't made available in the `build-system.requires` section of `pyproject.toml`. In particular, it cannot import anything from the project being built since it has to be built before it can be installed in the build package, leading to a bootstrap problem.
```

### Comparing `runtime_builder-0.1.0/tests/project_template/SConstruct` & `runtime_builder-0.1.1/tests/project_template_enscons/SConstruct`

 * *Files identical despite different names*

### Comparing `runtime_builder-0.1.0/tests/project_template/proj/run_test.py` & `runtime_builder-0.1.1/tests/project_template_enscons/proj/run_test.py`

 * *Files identical despite different names*

### Comparing `runtime_builder-0.1.0/tests/project_template/proj/runtime_build` & `runtime_builder-0.1.1/tests/project_template_enscons/proj/runtime_build`

 * *Files identical despite different names*

### Comparing `runtime_builder-0.1.0/PKG-INFO` & `runtime_builder-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,55 @@
 Metadata-Version: 2.1
 Name: runtime_builder
-Version: 0.1.0
+Version: 0.1.1
 Summary: Allow automatic builds in edit mode
 Author-email: Richard Kiss <him@richardkiss.com>
 Description-Content-Type: text/markdown
 
 # Runtime Builder
 
 Sometimes python developers want to include compiled output or other binary blob artifacts in their wheels. The source materials for this output is checked into git, but the blobs are not, since they're not source material and are at risk getting out of sync with the source distribution.
 
 When building the wheel, the blobs need to be generated. But it may also be nice to rebuild the blobs if the source have changed at runtime to automate a step of the edit/test cycle.
 
 This project lets you declare a single configuration describing how to build the artifacts, and build them at runtime during the development cycle or at wheel build time.
 
 ## Example
 
-There is an example project in `tests/project_template`.
+There are example projects in `tests/project_template_enscons` and `tests/project_template_setuptools`.
 
-project_template
+tests/project_template_setuptools
+├── README.md
+├── proj
+│   ├── bar.source
+│   ├── foo.source
+│   ├── run_test.py
+│   └── runtime_build
+├── pyproject.toml.template
+├── setup.py
+├── test_pip_install.sh
+└── test_pip_install_editable.sh
+
+This examples uses `setuptools` and `setup.py` to build. The `setup.py` and `runtime_build` files work together to make available artifacts built from the `.source` files.
+
+
+project_template_enscons
 ├── README.md
 ├── SConstruct
 ├── proj
 │   ├── bar.source
 │   ├── foo.source
 │   ├── run_test.py
 │   └── runtime_build
 ├── pyproject.toml.template
 ├── test_pip_install.sh
 └── test_pip_install_editable.sh
 
-Note that it uses `enscons` to build, as the more commonly used `setuptools` does not easily allow fine-grained control of the contents of the `sdist` and `wheel` files. In particular, this example takes pains to include the source files `runtime_build`, `foo.source`, `bar.source` and `program.source` in the sdist but not the wheel.
+Note that this example uses `enscons` to build, as `setuptools` does not easily allow fine-grained control of the contents of the `sdist` and `wheel` files. In particular, this example takes pains to include the source files `runtime_build`, `foo.source` and `bar.source` in the sdist but not the wheel.
+
 
 ### Configuration
 
 Artifacts to be build must be declared in a `runtime_build` file located in the destination module of the artifacts. Each submodule can have zero or one of these build files. In the `project_template` example above, `bar.source` and `foo.source` each produce an output in the `proj` submodule, and `runtime_build` defines what the artifacts are.
 
 This configuration file can be loaded at build time or at run time, so it *cannot* import anything that isn't made available in the `build-system.requires` section of `pyproject.toml`. In particular, it cannot import anything from the project being built since it has to be built before it can be installed in the build package, leading to a bootstrap problem.
```

