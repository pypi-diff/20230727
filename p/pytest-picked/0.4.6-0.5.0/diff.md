# Comparing `tmp/pytest-picked-0.4.6.tar.gz` & `tmp/pytest-picked-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-picked-0.4.6.tar", last modified: Wed Dec 23 09:43:32 2020, max compression
+gzip compressed data, was "pytest-picked-0.5.0.tar", last modified: Thu Jul 27 15:48:38 2023, max compression
```

## Comparing `pytest-picked-0.4.6.tar` & `pytest-picked-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 ana       (1000) ana       (1000)        0 2020-12-23 09:43:32.268894 pytest-picked-0.4.6/
--rw-r--r--   0 ana       (1000) ana       (1000)     1083 2020-12-23 09:38:08.000000 pytest-picked-0.4.6/LICENSE
--rw-r--r--   0 ana       (1000) ana       (1000)       97 2020-12-23 09:38:08.000000 pytest-picked-0.4.6/MANIFEST.in
--rw-r--r--   0 ana       (1000) ana       (1000)     5946 2020-12-23 09:43:32.268894 pytest-picked-0.4.6/PKG-INFO
--rw-r--r--   0 ana       (1000) ana       (1000)     4118 2020-12-23 09:38:08.000000 pytest-picked-0.4.6/README.rst
-drwxr-xr-x   0 ana       (1000) ana       (1000)        0 2020-12-23 09:43:32.268894 pytest-picked-0.4.6/pytest_picked/
--rw-r--r--   0 ana       (1000) ana       (1000)        0 2020-12-23 09:38:08.000000 pytest-picked-0.4.6/pytest_picked/__init__.py
--rw-r--r--   0 ana       (1000) ana       (1000)     4667 2020-12-23 09:38:08.000000 pytest-picked-0.4.6/pytest_picked/modes.py
--rw-r--r--   0 ana       (1000) ana       (1000)     2929 2020-12-23 09:38:08.000000 pytest-picked-0.4.6/pytest_picked/plugin.py
-drwxr-xr-x   0 ana       (1000) ana       (1000)        0 2020-12-23 09:43:32.268894 pytest-picked-0.4.6/pytest_picked.egg-info/
--rw-r--r--   0 ana       (1000) ana       (1000)     5946 2020-12-23 09:43:32.000000 pytest-picked-0.4.6/pytest_picked.egg-info/PKG-INFO
--rw-r--r--   0 ana       (1000) ana       (1000)      346 2020-12-23 09:43:32.000000 pytest-picked-0.4.6/pytest_picked.egg-info/SOURCES.txt
--rw-r--r--   0 ana       (1000) ana       (1000)        1 2020-12-23 09:43:32.000000 pytest-picked-0.4.6/pytest_picked.egg-info/dependency_links.txt
--rw-r--r--   0 ana       (1000) ana       (1000)       42 2020-12-23 09:43:32.000000 pytest-picked-0.4.6/pytest_picked.egg-info/entry_points.txt
--rw-r--r--   0 ana       (1000) ana       (1000)       14 2020-12-23 09:43:32.000000 pytest-picked-0.4.6/pytest_picked.egg-info/requires.txt
--rw-r--r--   0 ana       (1000) ana       (1000)       14 2020-12-23 09:43:32.000000 pytest-picked-0.4.6/pytest_picked.egg-info/top_level.txt
--rw-r--r--   0 ana       (1000) ana       (1000)       69 2020-12-23 09:43:32.268894 pytest-picked-0.4.6/setup.cfg
--rw-r--r--   0 ana       (1000) ana       (1000)     1223 2020-12-23 09:38:08.000000 pytest-picked-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:48:38.503997 pytest-picked-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-27 15:48:31.000000 pytest-picked-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-27 15:48:31.000000 pytest-picked-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-27 15:48:38.503997 pytest-picked-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-27 15:48:31.000000 pytest-picked-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:48:38.503997 pytest-picked-0.5.0/pytest_picked/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:48:31.000000 pytest-picked-0.5.0/pytest_picked/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-07-27 15:48:31.000000 pytest-picked-0.5.0/pytest_picked/modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-27 15:48:31.000000 pytest-picked-0.5.0/pytest_picked/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:48:38.503997 pytest-picked-0.5.0/pytest_picked.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-27 15:48:38.000000 pytest-picked-0.5.0/pytest_picked.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-27 15:48:38.000000 pytest-picked-0.5.0/pytest_picked.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:48:38.000000 pytest-picked-0.5.0/pytest_picked.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 15:48:38.000000 pytest-picked-0.5.0/pytest_picked.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 15:48:38.000000 pytest-picked-0.5.0/pytest_picked.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 15:48:38.000000 pytest-picked-0.5.0/pytest_picked.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 15:48:38.503997 pytest-picked-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-27 15:48:31.000000 pytest-picked-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:48:38.503997 pytest-picked-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-27 15:48:31.000000 pytest-picked-0.5.0/tests/test_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-27 15:48:31.000000 pytest-picked-0.5.0/tests/test_pytest_picked.py
```

### Comparing `pytest-picked-0.4.6/LICENSE` & `pytest-picked-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-picked-0.4.6/README.rst` & `pytest-picked-0.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,137 +1,125 @@
-===============
-pytest-picked
-===============
-
-.. image:: https://github.com/anapaulagomes/pytest-picked/workflows/Tests/badge.svg
-    :target: https://github.com/anapaulagomes/pytest-picked/actions?query=workflow%3ATests
-    :alt: See Test Status on Github Actions
-
-.. image:: https://github.com/anapaulagomes/pytest-picked/workflows/Publish%20to%20Test%20PyPi/badge.svg
-    :target: https://test.pypi.org/project/pytest-picked/
-    :alt: See Package Status on Test PyPI
-
-.. image:: https://github.com/anapaulagomes/pytest-picked/workflows/Publish%20to%20PyPI/badge.svg
-    :target: https://pypi.org/project/pytest-picked/
-    :alt: See Package Status on PyPI
-
-.. image:: https://img.shields.io/conda/vn/conda-forge/pytest-picked.svg
-    :target: https://anaconda.org/conda-forge/pytest-picked
-    :alt: Conda forge package
-
-.. image:: https://img.shields.io/pypi/pyversions/pytest-picked.svg
-    :target: https://pypi.org/project/pytest-picked
-    :alt: Supported Python versions
+Metadata-Version: 2.1
+Name: pytest-picked
+Version: 0.5.0
+Summary: Run the tests related to the changed files
+Home-page: https://github.com/anapaulagomes/pytest-picked
+Author: Ana Paula Gomes
+Author-email: apgomes88@gmail.com
+Maintainer: Ana Paula Gomes
+Maintainer-email: apgomes88@gmail.com
+License: MIT
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Testing
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pytest-picked
+
+[![See Test Status on Github Actions](https://github.com/anapaulagomes/pytest-picked/workflows/Tests/badge.svg)](https://github.com/anapaulagomes/pytest-picked/actions?query=workflow%3ATests)
 
-Run the tests related to the unstaged files or the current branch (according to Git)
+[![PyPI version](https://badge.fury.io/py/pytest-picked.svg)](https://badge.fury.io/py/pytest-picked)
 
----
-
-.. image:: demo.gif
-    :height: 400px
-    :alt: Demo
-
-Let's say you have the following output from ``git status``:
-
-::
+[![Conda forge package](https://img.shields.io/conda/vn/conda-forge/pytest-picked.svg)](https://anaconda.org/conda-forge/pytest-picked)
 
-  $ git status
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/pytest-picked.svg)](https://pypi.org/project/pytest-picked)
 
-  On branch master
-  Your branch is ahead of 'origin/master' by 1 commit.
-    (use "git push" to publish your local commits)
-
-  Untracked files:
-    (use "git add <file>..." to include in what will be committed)
-
-    api.py
-    tests/api/
-    tests/test_board.py
-
-  nothing added to commit but untracked files present (use "git add" to track)
+Run the tests related to the unstaged files or the current branch
+(according to Git)
 
+---
 
-Running ``pytest --picked``, the plugin will run all tests that come from this output.
+![Demo](demo.gif)
 
-::
+Let's say you have the following output from `git status`:
 
-  $ pytest --picked
+    $ git status
 
-  ============================= test session starts =============================
-  platform darwin -- Python 3.6.4, pytest-3.6.0, py-1.5.3, pluggy-0.6.0
-  rootdir: /Users/ana.gomes/personal-workspace/grandma, inifile:
-  plugins: picked-0.1.0, mock-1.10.0, flask-0.10.0, deadfixtures-2.0.1
-  collecting 34 items
-  Changed test files... 1. ['tests/test_board.py']
-  Changed test folders... 1. ['tests/api/']
-  collected 34 items
+    On branch main
+    Your branch is ahead of 'origin/main' by 1 commit.
+      (use "git push" to publish your local commits)
 
-  tests/test_board.py .                                                      [ 50%]
-  tests/api/test_new.py .                                                    [100%]
+    Untracked files:
+      (use "git add <file>..." to include in what will be committed)
 
-  =========================== 2 passed in 0.07 seconds ===========================
+      api.py
+      tests/api/
+      tests/test_board.py
 
-All tests will be run from files and folders which are modified but not yet committed.
-No more copy and paste!
+    nothing added to commit but untracked files present (use "git add" to track)
 
+Running `pytest --picked`, the plugin will run all tests that come from
+this output.
 
-Usage
------
+    $ pytest --picked
 
-::
+    ============================= test session starts =============================
+    platform darwin -- Python 3.6.4, pytest-3.6.0, py-1.5.3, pluggy-0.6.0
+    rootdir: /Users/ana.gomes/personal-workspace/grandma, inifile:
+    plugins: picked-0.1.0, mock-1.10.0, flask-0.10.0, deadfixtures-2.0.1
+    collecting 34 items
+    Changed test files... 1. ['tests/test_board.py']
+    Changed test folders... 1. ['tests/api/']
+    collected 34 items
 
-  $ pytest --picked
+    tests/test_board.py .                                                      [ 50%]
+    tests/api/test_new.py .                                                    [100%]
 
-  $ pytest --picked=first
+    =========================== 2 passed in 0.07 seconds ===========================
 
-  $ pytest --picked --mode=branch
+All tests will be run from files and folders which are modified but not
+yet committed. No more copy and paste!
 
-  $ pytest --picked --mode=unstaged  # default
+## Usage
 
-  $ pytest --picked --mode=branch --parent-branch=main # if your parent branch differs from "master"
+```bash
+pytest --picked
 
+pytest --picked=first
 
-Features
---------
+pytest --picked --mode=branch
 
-Using ``git status``, this plugin allows you to:
+pytest --picked --mode=unstaged  # default
 
-* Run only tests from modified test files
-* Run tests from modified test files first, followed by all unmodified tests
+pytest --picked --mode=branch --parent-branch=dev # if your parent branch differs from "main"
+```
 
-Installation
-------------
+## Features
 
-You can install ``pytest-picked`` via `pip`_ from `PyPI`_::
+Using `git status`, this plugin allows you to:
 
-    $ pip install pytest-picked
+- Run only tests from modified test files
+- Run tests from modified test files first, followed by all unmodified tests
 
+## Installation
 
-Contributing
-------------
-Contributions are very welcome. Tests can be run with `tox`_, please ensure
-the coverage at least stays the same before you submit a pull request.
+You can install `pytest-picked` via [PyPI](https://pypi.org/project/pytest-picked/):
 
+```bash
+pip install pytest-picked
+```
 
-License
--------
+## Contributing
 
-Distributed under the terms of the `MIT`_ license, "pytest-picked" is free and open source software
+Contributions are very welcome. Tests can be run with
+[tox](https://tox.readthedocs.io/en/latest/), so we can guarantee that it is working
+in different python versions. Also, make sure to add tests and use `pre-commit`
+before you submit a pull request.
 
+## License
 
-Issues
-------
+Distributed under the terms of the [MIT](http://opensource.org/licenses/MIT) license,
+`pytest-picked` is free and open source software
 
-If you encounter any problems, please `file an issue`_ along with a detailed description.
+## Issues
 
-.. _`Cookiecutter`: https://github.com/audreyr/cookiecutter
-.. _`@hackebrot`: https://github.com/hackebrot
-.. _`MIT`: http://opensource.org/licenses/MIT
-.. _`BSD-3`: http://opensource.org/licenses/BSD-3-Clause
-.. _`GNU GPL v3.0`: http://www.gnu.org/licenses/gpl-3.0.txt
-.. _`Apache Software License 2.0`: http://www.apache.org/licenses/LICENSE-2.0
-.. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
-.. _`file an issue`: https://github.com/anapaulagomes/pytest-picked/issues
-.. _`pytest`: https://github.com/pytest-dev/pytest
-.. _`tox`: https://tox.readthedocs.io/en/latest/
-.. _`pip`: https://pypi.org/project/pip/
-.. _`PyPI`: https://pypi.org/project
+If you encounter any problems, please [file an issue](https://github.com/anapaulagomes/pytest-picked/issues)
+along with a detailed description.
```

### Comparing `pytest-picked-0.4.6/pytest_picked/modes.py` & `pytest-picked-0.5.0/pytest_picked/modes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import subprocess  # nosec
+import warnings
 from abc import ABC, abstractmethod
 
 
 class Mode(ABC):
     def __init__(self, test_file_convention):
         self.test_file_convention = test_file_convention
 
@@ -45,16 +46,17 @@
 
     @abstractmethod
     def parser(self, candidate):
         pass
 
 
 class Branch(Mode):
-    def __init__(self, test_file_convention, parent_branch="master"):
+    def __init__(self, test_file_convention, parent_branch="main"):
         super().__init__(test_file_convention)
+        warnings.warn("Now `main` is the default parent branch")
         self.parent_branch = parent_branch
 
     def command(self):
         return ["git", "diff", "--name-status", "--relative", self.parent_branch]
 
     def parser(self, candidate):
         """
```

### Comparing `pytest-picked-0.4.6/pytest_picked/plugin.py` & `pytest-picked-0.5.0/pytest_picked/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,17 @@
         required=False,
         help="Options: unstaged, branch",
     )
     group.addoption(
         "--parent-branch",
         action="store",
         dest="parent_branch",
-        default="master",
+        default="main",
         required=False,
-        help="The main branch of your repo (master, main, trunk, etc)",
+        help="The main branch of your repo (main, develop, trunk etc)",
     )
 
 
 def _get_affected_paths(config):
     picked_mode = config.getoption("picked_mode")
     parent_branch = config.getoption("parent_branch")
     test_file_convention = config._getini("python_files")  # pylint: disable=W0212
```

### Comparing `pytest-picked-0.4.6/setup.py` & `pytest-picked-0.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
 import codecs
 import os
 
 from setuptools import find_packages, setup
 
 
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding="utf-8").read()
 
 
 setup(
     name="pytest-picked",
-    version="0.4.6",
+    version="0.5.0",
     author="Ana Paula Gomes",
     author_email="apgomes88@gmail.com",
     maintainer="Ana Paula Gomes",
     maintainer_email="apgomes88@gmail.com",
     license="MIT",
     url="https://github.com/anapaulagomes/pytest-picked",
     description="Run the tests related to the changed files",
-    long_description=read("README.rst"),
+    long_description=read("README.md"),
+    long_description_content_type="text/markdown",
     packages=find_packages(exclude=["tests", "docs"]),
-    python_requires=">=3.5",
-    install_requires=["pytest>=3.5.0"],
+    python_requires=">=3.7",
+    install_requires=["pytest>=3.7.0"],
     classifiers=[
         "Framework :: Pytest",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Testing",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
     ],
     entry_points={"pytest11": ["picked = pytest_picked.plugin"]},
 )
```

